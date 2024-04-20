# Comparing `tmp/nodriver-0.27rc3.tar.gz` & `tmp/nodriver-0.28rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodriver-0.27rc3.tar", last modified: Sun Mar 10 03:05:04 2024, max compression
+gzip compressed data, was "nodriver-0.28rc1.tar", last modified: Sat Apr 20 15:14:10 2024, max compression
```

## Comparing `nodriver-0.27rc3.tar` & `nodriver-0.28rc1.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxrwxrwx   0        0        0        0 2024-03-10 03:05:04.866546 nodriver-0.27rc3/
--rw-rw-rw-   0        0        0    32693 2024-01-18 14:05:42.000000 nodriver-0.27rc3/LICENSE.txt
--rw-rw-rw-   0        0        0      121 2024-02-25 19:31:30.000000 nodriver-0.27rc3/MANIFEST.in
--rw-rw-rw-   0        0        0    47611 2024-03-10 03:05:04.866546 nodriver-0.27rc3/PKG-INFO
--rw-rw-rw-   0        0        0     8430 2024-02-25 18:42:37.000000 nodriver-0.27rc3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-10 03:05:04.841641 nodriver-0.27rc3/nodriver/
--rw-rw-rw-   0        0        0      616 2024-03-10 03:03:41.000000 nodriver-0.27rc3/nodriver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-10 03:05:04.862547 nodriver-0.27rc3/nodriver/cdp/
--rw-rw-rw-   0        0        0      172 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/README.md
--rw-rw-rw-   0        0        0     1011 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/__init__.py
--rw-rw-rw-   0        0        0    25019 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/accessibility.py
--rw-rw-rw-   0        0        0    11919 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/animation.py
--rw-rw-rw-   0        0        0    65075 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/audits.py
--rw-rw-rw-   0        0        0     8168 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/autofill.py
--rw-rw-rw-   0        0        0     6359 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/background_service.py
--rw-rw-rw-   0        0        0    22888 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/browser.py
--rw-rw-rw-   0        0        0     9549 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/cache_storage.py
--rw-rw-rw-   0        0        0     4565 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/cast.py
--rw-rw-rw-   0        0        0     3004 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/console.py
--rw-rw-rw-   0        0        0    80456 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/css.py
--rw-rw-rw-   0        0        0     4358 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/database.py
--rw-rw-rw-   0        0        0    54782 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/debugger.py
--rw-rw-rw-   0        0        0     3497 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/device_access.py
--rw-rw-rw-   0        0        0     1187 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/device_orientation.py
--rw-rw-rw-   0        0        0    66246 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/dom.py
--rw-rw-rw-   0        0        0    10211 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/dom_debugger.py
--rw-rw-rw-   0        0        0    43435 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/dom_snapshot.py
--rw-rw-rw-   0        0        0     6124 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/dom_storage.py
--rw-rw-rw-   0        0        0    34831 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/emulation.py
--rw-rw-rw-   0        0        0     1501 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/event_breakpoints.py
--rw-rw-rw-   0        0        0     7347 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/fed_cm.py
--rw-rw-rw-   0        0        0    21611 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/fetch.py
--rw-rw-rw-   0        0        0     5219 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/headless_experimental.py
--rw-rw-rw-   0        0        0    14457 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/heap_profiler.py
--rw-rw-rw-   0        0        0    18362 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/indexed_db.py
--rw-rw-rw-   0        0        0    29314 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/input_.py
--rw-rw-rw-   0        0        0     1743 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/inspector.py
--rw-rw-rw-   0        0        0     3120 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/io.py
--rw-rw-rw-   0        0        0    16878 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/layer_tree.py
--rw-rw-rw-   0        0        0     6092 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/log.py
--rw-rw-rw-   0        0        0     8215 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/media.py
--rw-rw-rw-   0        0        0     7279 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/memory.py
--rw-rw-rw-   0        0        0   147161 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/network.py
--rw-rw-rw-   0        0        0    60483 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/overlay.py
--rw-rw-rw-   0        0        0   117573 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/page.py
--rw-rw-rw-   0        0        0     3203 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/performance.py
--rw-rw-rw-   0        0        0     7587 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/performance_timeline.py
--rw-rw-rw-   0        0        0    22524 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/preload.py
--rw-rw-rw-   0        0        0    14302 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/profiler.py
--rw-rw-rw-   0        0        0        0 2024-01-18 14:08:24.000000 nodriver-0.27rc3/nodriver/cdp/py.typed
--rw-rw-rw-   0        0        0    67631 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/runtime.py
--rw-rw-rw-   0        0        0     1196 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/schema.py
--rw-rw-rw-   0        0        0    18824 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/security.py
--rw-rw-rw-   0        0        0    12358 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/service_worker.py
--rw-rw-rw-   0        0        0    61377 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/storage.py
--rw-rw-rw-   0        0        0    12914 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/system_info.py
--rw-rw-rw-   0        0        0    25505 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/target.py
--rw-rw-rw-   0        0        0     1533 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/tethering.py
--rw-rw-rw-   0        0        0    14682 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/tracing.py
--rw-rw-rw-   0        0        0      470 2024-02-02 09:23:34.000000 nodriver-0.27rc3/nodriver/cdp/util.py
--rw-rw-rw-   0        0        0    18513 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/web_audio.py
--rw-rw-rw-   0        0        0    18390 2024-02-21 01:38:45.000000 nodriver-0.27rc3/nodriver/cdp/web_authn.py
-drwxrwxrwx   0        0        0        0 2024-03-10 03:05:04.864546 nodriver-0.27rc3/nodriver/core/
--rw-rw-rw-   0        0        0     3828 2024-02-04 19:44:05.000000 nodriver-0.27rc3/nodriver/core/_contradict.py
--rw-rw-rw-   0        0        0    28613 2024-03-10 03:03:41.000000 nodriver-0.27rc3/nodriver/core/browser.py
--rw-rw-rw-   0        0        0    10142 2024-03-10 03:03:41.000000 nodriver-0.27rc3/nodriver/core/config.py
--rw-rw-rw-   0        0        0    21191 2024-03-10 03:03:41.000000 nodriver-0.27rc3/nodriver/core/connection.py
--rw-rw-rw-   0        0        0    34626 2024-03-10 03:03:41.000000 nodriver-0.27rc3/nodriver/core/element.py
--rw-rw-rw-   0        0        0    50403 2024-03-10 03:03:41.000000 nodriver-0.27rc3/nodriver/core/tab.py
--rw-rw-rw-   0        0        0     9399 2024-03-10 03:04:45.000000 nodriver-0.27rc3/nodriver/core/util.py
-drwxrwxrwx   0        0        0        0 2024-03-10 03:05:04.865546 nodriver-0.27rc3/nodriver.egg-info/
--rw-rw-rw-   0        0        0    47611 2024-03-10 03:05:04.000000 nodriver-0.27rc3/nodriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1805 2024-03-10 03:05:04.000000 nodriver-0.27rc3/nodriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-10 03:05:04.000000 nodriver-0.27rc3/nodriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-03-10 03:05:04.000000 nodriver-0.27rc3/nodriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-10 03:05:04.000000 nodriver-0.27rc3/nodriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3560 2024-03-10 03:04:45.000000 nodriver-0.27rc3/pyproject.toml
--rw-rw-rw-   0        0        0       85 2024-03-10 03:05:04.866546 nodriver-0.27rc3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 15:14:10.209216 nodriver-0.28rc1/
+-rw-rw-rw-   0        0        0    32693 2024-01-18 14:05:42.000000 nodriver-0.28rc1/LICENSE.txt
+-rw-rw-rw-   0        0        0      121 2024-02-25 19:31:30.000000 nodriver-0.28rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0    47611 2024-04-20 15:14:10.209216 nodriver-0.28rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     8430 2024-02-25 18:42:37.000000 nodriver-0.28rc1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 15:14:10.177217 nodriver-0.28rc1/nodriver/
+-rw-rw-rw-   0        0        0      616 2024-03-10 03:03:41.000000 nodriver-0.28rc1/nodriver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:14:10.204216 nodriver-0.28rc1/nodriver/cdp/
+-rw-rw-rw-   0        0        0      172 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/README.md
+-rw-rw-rw-   0        0        0     1011 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/__init__.py
+-rw-rw-rw-   0        0        0    25019 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/accessibility.py
+-rw-rw-rw-   0        0        0    11919 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/animation.py
+-rw-rw-rw-   0        0        0    65075 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/audits.py
+-rw-rw-rw-   0        0        0     8168 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/autofill.py
+-rw-rw-rw-   0        0        0     6359 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/background_service.py
+-rw-rw-rw-   0        0        0    22888 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/browser.py
+-rw-rw-rw-   0        0        0     9549 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/cache_storage.py
+-rw-rw-rw-   0        0        0     4565 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/cast.py
+-rw-rw-rw-   0        0        0     3004 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/console.py
+-rw-rw-rw-   0        0        0    80456 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/css.py
+-rw-rw-rw-   0        0        0     4358 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/database.py
+-rw-rw-rw-   0        0        0    54782 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/debugger.py
+-rw-rw-rw-   0        0        0     3497 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/device_access.py
+-rw-rw-rw-   0        0        0     1187 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/device_orientation.py
+-rw-rw-rw-   0        0        0    66246 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/dom.py
+-rw-rw-rw-   0        0        0    10211 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/dom_debugger.py
+-rw-rw-rw-   0        0        0    43435 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/dom_snapshot.py
+-rw-rw-rw-   0        0        0     6124 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/dom_storage.py
+-rw-rw-rw-   0        0        0    34831 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/emulation.py
+-rw-rw-rw-   0        0        0     1501 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/event_breakpoints.py
+-rw-rw-rw-   0        0        0     7347 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/fed_cm.py
+-rw-rw-rw-   0        0        0    21611 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/fetch.py
+-rw-rw-rw-   0        0        0     5219 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/headless_experimental.py
+-rw-rw-rw-   0        0        0    14457 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/heap_profiler.py
+-rw-rw-rw-   0        0        0    18362 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/indexed_db.py
+-rw-rw-rw-   0        0        0    29314 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/input_.py
+-rw-rw-rw-   0        0        0     1743 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/inspector.py
+-rw-rw-rw-   0        0        0     3120 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/io.py
+-rw-rw-rw-   0        0        0    16878 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/layer_tree.py
+-rw-rw-rw-   0        0        0     6092 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/log.py
+-rw-rw-rw-   0        0        0     8215 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/media.py
+-rw-rw-rw-   0        0        0     7279 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/memory.py
+-rw-rw-rw-   0        0        0   147161 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/network.py
+-rw-rw-rw-   0        0        0    60483 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/overlay.py
+-rw-rw-rw-   0        0        0   117573 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/page.py
+-rw-rw-rw-   0        0        0     3203 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/performance.py
+-rw-rw-rw-   0        0        0     7587 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/performance_timeline.py
+-rw-rw-rw-   0        0        0    22524 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/preload.py
+-rw-rw-rw-   0        0        0    14302 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/profiler.py
+-rw-rw-rw-   0        0        0        0 2024-01-18 14:08:24.000000 nodriver-0.28rc1/nodriver/cdp/py.typed
+-rw-rw-rw-   0        0        0    67631 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/runtime.py
+-rw-rw-rw-   0        0        0     1196 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/schema.py
+-rw-rw-rw-   0        0        0    18824 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/security.py
+-rw-rw-rw-   0        0        0    12358 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/service_worker.py
+-rw-rw-rw-   0        0        0    61377 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/storage.py
+-rw-rw-rw-   0        0        0    12914 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/system_info.py
+-rw-rw-rw-   0        0        0    25505 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/target.py
+-rw-rw-rw-   0        0        0     1533 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/tethering.py
+-rw-rw-rw-   0        0        0    14682 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/tracing.py
+-rw-rw-rw-   0        0        0      470 2024-02-02 09:23:34.000000 nodriver-0.28rc1/nodriver/cdp/util.py
+-rw-rw-rw-   0        0        0    18513 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/web_audio.py
+-rw-rw-rw-   0        0        0    18390 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/web_authn.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:14:10.207218 nodriver-0.28rc1/nodriver/core/
+-rw-rw-rw-   0        0        0     3828 2024-02-04 19:44:05.000000 nodriver-0.28rc1/nodriver/core/_contradict.py
+-rw-rw-rw-   0        0        0    28628 2024-04-20 15:13:01.000000 nodriver-0.28rc1/nodriver/core/browser.py
+-rw-rw-rw-   0        0        0    10142 2024-03-10 03:03:41.000000 nodriver-0.28rc1/nodriver/core/config.py
+-rw-rw-rw-   0        0        0    21366 2024-04-20 14:29:31.000000 nodriver-0.28rc1/nodriver/core/connection.py
+-rw-rw-rw-   0        0        0    35674 2024-04-20 15:13:01.000000 nodriver-0.28rc1/nodriver/core/element.py
+-rw-rw-rw-   0        0        0     1282 2024-03-26 18:00:57.000000 nodriver-0.28rc1/nodriver/core/extra.py
+-rw-rw-rw-   0        0        0    50251 2024-04-20 15:13:01.000000 nodriver-0.28rc1/nodriver/core/tab.py
+-rw-rw-rw-   0        0        0     9399 2024-03-10 03:04:45.000000 nodriver-0.28rc1/nodriver/core/util.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:14:10.208217 nodriver-0.28rc1/nodriver.egg-info/
+-rw-rw-rw-   0        0        0    47611 2024-04-20 15:14:10.000000 nodriver-0.28rc1/nodriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1828 2024-04-20 15:14:10.000000 nodriver-0.28rc1/nodriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 15:14:10.000000 nodriver-0.28rc1/nodriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-04-20 15:14:10.000000 nodriver-0.28rc1/nodriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-20 15:14:10.000000 nodriver-0.28rc1/nodriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3560 2024-04-20 15:13:00.000000 nodriver-0.28rc1/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2024-04-20 15:14:10.209216 nodriver-0.28rc1/setup.cfg
```

### Comparing `nodriver-0.27rc3/LICENSE.txt` & `nodriver-0.28rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/PKG-INFO` & `nodriver-0.28rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodriver
-Version: 0.27rc3
+Version: 0.28rc1
 Summary: * Official successor of Undetected Chromedriver
 Author-email: UltrafunkAmsterdam <doesnotexist@ultrafunk.nl>
 Maintainer-email: UltrafunkAmsterdam <doesnotexist@ultrafunk.nl>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `nodriver-0.27rc3/README.md` & `nodriver-0.28rc1/README.md`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/__init__.py` & `nodriver-0.28rc1/nodriver/__init__.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/__init__.py` & `nodriver-0.28rc1/nodriver/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/accessibility.py` & `nodriver-0.28rc1/nodriver/cdp/accessibility.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/animation.py` & `nodriver-0.28rc1/nodriver/cdp/animation.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/audits.py` & `nodriver-0.28rc1/nodriver/cdp/audits.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/autofill.py` & `nodriver-0.28rc1/nodriver/cdp/autofill.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/background_service.py` & `nodriver-0.28rc1/nodriver/cdp/background_service.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/browser.py` & `nodriver-0.28rc1/nodriver/cdp/browser.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/cache_storage.py` & `nodriver-0.28rc1/nodriver/cdp/cache_storage.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/cast.py` & `nodriver-0.28rc1/nodriver/cdp/cast.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/console.py` & `nodriver-0.28rc1/nodriver/cdp/console.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/css.py` & `nodriver-0.28rc1/nodriver/cdp/css.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/database.py` & `nodriver-0.28rc1/nodriver/cdp/database.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/debugger.py` & `nodriver-0.28rc1/nodriver/cdp/debugger.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/device_access.py` & `nodriver-0.28rc1/nodriver/cdp/device_access.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/device_orientation.py` & `nodriver-0.28rc1/nodriver/cdp/device_orientation.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/dom.py` & `nodriver-0.28rc1/nodriver/cdp/dom.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/dom_debugger.py` & `nodriver-0.28rc1/nodriver/cdp/dom_debugger.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/dom_snapshot.py` & `nodriver-0.28rc1/nodriver/cdp/dom_snapshot.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/dom_storage.py` & `nodriver-0.28rc1/nodriver/cdp/dom_storage.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/emulation.py` & `nodriver-0.28rc1/nodriver/cdp/emulation.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/event_breakpoints.py` & `nodriver-0.28rc1/nodriver/cdp/event_breakpoints.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/fed_cm.py` & `nodriver-0.28rc1/nodriver/cdp/fed_cm.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/fetch.py` & `nodriver-0.28rc1/nodriver/cdp/fetch.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/headless_experimental.py` & `nodriver-0.28rc1/nodriver/cdp/headless_experimental.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/heap_profiler.py` & `nodriver-0.28rc1/nodriver/cdp/heap_profiler.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/indexed_db.py` & `nodriver-0.28rc1/nodriver/cdp/indexed_db.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/input_.py` & `nodriver-0.28rc1/nodriver/cdp/input_.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/inspector.py` & `nodriver-0.28rc1/nodriver/cdp/inspector.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/io.py` & `nodriver-0.28rc1/nodriver/cdp/io.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/layer_tree.py` & `nodriver-0.28rc1/nodriver/cdp/layer_tree.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/log.py` & `nodriver-0.28rc1/nodriver/cdp/log.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/media.py` & `nodriver-0.28rc1/nodriver/cdp/media.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/memory.py` & `nodriver-0.28rc1/nodriver/cdp/memory.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/network.py` & `nodriver-0.28rc1/nodriver/cdp/network.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/overlay.py` & `nodriver-0.28rc1/nodriver/cdp/overlay.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/page.py` & `nodriver-0.28rc1/nodriver/cdp/page.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/performance.py` & `nodriver-0.28rc1/nodriver/cdp/performance.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/performance_timeline.py` & `nodriver-0.28rc1/nodriver/cdp/performance_timeline.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/preload.py` & `nodriver-0.28rc1/nodriver/cdp/preload.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/profiler.py` & `nodriver-0.28rc1/nodriver/cdp/profiler.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/runtime.py` & `nodriver-0.28rc1/nodriver/cdp/runtime.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/schema.py` & `nodriver-0.28rc1/nodriver/cdp/schema.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/security.py` & `nodriver-0.28rc1/nodriver/cdp/security.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/service_worker.py` & `nodriver-0.28rc1/nodriver/cdp/service_worker.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/storage.py` & `nodriver-0.28rc1/nodriver/cdp/storage.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/system_info.py` & `nodriver-0.28rc1/nodriver/cdp/system_info.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/target.py` & `nodriver-0.28rc1/nodriver/cdp/target.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/tethering.py` & `nodriver-0.28rc1/nodriver/cdp/tethering.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/tracing.py` & `nodriver-0.28rc1/nodriver/cdp/tracing.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/web_audio.py` & `nodriver-0.28rc1/nodriver/cdp/web_audio.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/cdp/web_authn.py` & `nodriver-0.28rc1/nodriver/cdp/web_authn.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/core/_contradict.py` & `nodriver-0.28rc1/nodriver/core/_contradict.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/core/browser.py` & `nodriver-0.28rc1/nodriver/core/browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         elif isinstance(event, cdp.target.TargetCreated):
             target_info: cdp.target.TargetInfo = event.target_info
             from .tab import Tab
 
             new_target = Tab(
                 (
                     f"ws://{self.config.host}:{self.config.port}"
-                    f"/devtools/{target_info.type_.lower()}"
+                    f"/devtools/page"  # all types are 'page' internally in chrome apparently
                     f"/{target_info.target_id}"
                 ),
                 target=target_info,
                 browser=self,
             )
 
             self.targets.append(new_target)
@@ -496,15 +496,15 @@
                     break
             else:
 
                 self.targets.append(
                     Connection(
                         (
                             f"ws://{self.config.host}:{self.config.port}"
-                            f"/devtools/{t.type_.lower()}"
+                            f"/devtools/page"  # all types are 'page' somehow
                             f"/{t.target_id}"
                         ),
                         target=t,
                         _owner=self,
                     )
                 )
 
@@ -547,15 +547,14 @@
         except RuntimeError:
             if self.connection:
                 try:
                     # asyncio.run(self.connection.send(cdp.browser.close()))
                     asyncio.run(self.connection.aclose())
                     logger.debug("closed the connection using asyncio.run()")
                 except Exception:
-                    logger.exception("exccc while closing", exc_info=True)
                     pass
 
         for _ in range(3):
             try:
                 self._process.terminate()
                 logger.info(
                     "terminated browser with pid %d successfully" % self._process.pid
@@ -793,15 +792,17 @@
     async def get(self, endpoint: str):
         return await self._request(endpoint)
 
     async def post(self, endpoint, data):
         return await self._request(endpoint, data)
 
     async def _request(self, endpoint, method: str = "get", data: dict = None):
-        url = urllib.parse.urljoin(self.api, "/".join(["json", endpoint]))
+        url = urllib.parse.urljoin(
+            self.api, f"json/{endpoint}" if endpoint else "/json"
+        )
         if data and method.lower() == "get":
             raise ValueError("get requests cannot contain data")
         if not url:
             url = self.api + endpoint
         request = urllib.request.Request(url)
         request.method = method
         request.data = None
```

### Comparing `nodriver-0.27rc3/nodriver/core/config.py` & `nodriver-0.28rc1/nodriver/core/config.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver/core/connection.py` & `nodriver-0.28rc1/nodriver/core/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,24 +197,22 @@
         _owner: "Browser" = None,
         **kwargs,
     ):
         super().__init__()
         self._target = target
         self.__count__ = itertools.count(0)
         self._owner = _owner
-
         self.websocket_url: str = websocket_url
         self.websocket = None
         self.mapper = {}
         self.handlers = collections.defaultdict(list)
         self.recv_task = None
         self.enabled_domains = []
         self._last_result = []
         self.listener: Listener = None
-
         self.__dict__.update(**kwargs)
 
     @property
     def target(self) -> cdp.target.TargetInfo:
         return self._target
 
     @target.setter
@@ -247,18 +245,16 @@
         handlers can be regular callback functions or async coroutine functions (and also just lamba's).
         for example, you want to check the network traffic:
 
         .. code-block::
 
             page.add_handler(cdp.network.RequestWillBeSent, lambda event: print('network event => %s' % event.request))
 
-
         the next time you make network traffic you will see your console print like crazy.
 
-
         :param event_type_or_domain:
         :type event_type_or_domain:
         :param handler:
         :type handler:
         :return:
         :rtype:
         """
@@ -306,52 +302,53 @@
 
         await self._register_handlers()
 
     async def aclose(self):
         """
         closes the websocket connection. should not be called manually by users.
         """
-
         if self.websocket and not self.websocket.closed:
             if self.listener and self.listener.running:
                 self.listener.cancel()
                 self.enabled_domains.clear()
             await self.websocket.close()
             logger.debug("\n❌ closed websocket connection to %s", self.websocket_url)
 
     async def sleep(self, t: Union[int, float] = 0.25):
         await self.update_target()
         await asyncio.sleep(t)
 
     async def wait(self, t: Union[int, float] = None):
         """
-        waits until the event listener
-        reports idle (which is when no new events had been received in .5 seconds
-        or, 1 second when in interactive mode)
+        waits until the event listener reports idle (no new events received in certain timespan).
+        when `t` is provided, ensures waiting for `t` seconds, no matter what.
 
         :param t:
         :type t:
         :return:
         :rtype:
         """
         await self.update_target()
-
+        loop = asyncio.get_running_loop()
+        start_time = loop.time()
         try:
-
-            await asyncio.wait_for(self.listener.idle.wait(), timeout=t)
+            if isinstance(t, (int, float)):
+                await asyncio.wait_for(self.listener.idle.wait(), timeout=t)
+                while (loop.time() - start_time) < t:
+                    await asyncio.sleep(0.1)
+            else:
+                await self.listener.idle.wait()
         except asyncio.TimeoutError:
-            if t is not None:
+            if isinstance(t, (int, float)):
                 # explicit time is given, which is now passed
                 # so bail out early
                 return
         except AttributeError:
             # no listener created yet
             pass
-        if t is not None:
-            await self.sleep(t)
 
     def __getattr__(self, item):
         """:meta private:"""
         try:
             return getattr(self.target, item)
         except AttributeError:
             raise
@@ -403,42 +400,38 @@
         try:
             tx = Transaction(cdp_obj)
             tx.connection = self
             if not self.mapper:
                 self.__count__ = itertools.count(0)
             tx.id = next(self.__count__)
             self.mapper.update({tx.id: tx})
-
             if not _is_update:
                 await self._register_handlers()
             await self.websocket.send(tx.message)
             try:
                 return await tx
             except ProtocolException as e:
                 e.message += f"\ncommand:{tx.method}\nparams:{tx.params}"
                 raise e
-
         except Exception:
             await self.aclose()
 
     async def _register_handlers(self):
         """
         ensure that for current (event) handlers, the corresponding
         domain is enabled in the protocol.
 
         """
         seen = []
-
         # save a copy of current enabled domains in a variable
         # domains will be removed from this variable
         # if it is still needed according to the set handlers
         # so at the end this variable will hold the domains that
         # are not represented by handlers, and can be removed
         enabled_domains = self.enabled_domains.copy()
-
         for event_type in self.handlers.copy():
             domain_mod = None
             if len(self.handlers[event_type]) == 0:
                 self.handlers.pop(event_type)
                 continue
             if isinstance(event_type, type):
                 domain_mod = util.cdp_get_module(event_type.__module__)
@@ -469,15 +462,14 @@
                         continue
                 finally:
                     continue
         for ed in enabled_domains:
             # we started with a copy of self.enabled_domains and removed a domain from this
             # temp variable when we registered it or saw handlers for it.
             # items still present at this point are unused and need removal
-
             self.enabled_domains.remove(ed)
 
 
 class Listener:
     def __init__(self, connection: Connection):
         self.connection = connection
         self.history = collections.deque()
@@ -530,51 +522,53 @@
             try:
                 msg = await asyncio.wait_for(
                     self.connection.websocket.recv(), self.time_before_considered_idle
                 )
             except asyncio.TimeoutError:
                 self.idle.set()
                 # breathe
-                await asyncio.sleep(self.time_before_considered_idle / 10)
+                # await asyncio.sleep(self.time_before_considered_idle / 10)
                 continue
-            except (Exception,):
+            except (Exception,) as e:
                 # break on any other exception
                 # which is mostly socket is closed or does not exist
                 # or is not allowed
+
+                logger.debug(
+                    "connection listener exception while reading websocket:\n%s", e
+                )
                 break
 
-            # async for msg in self.connection.websocket:
             if not self.running:
+                # if we have been cancelled or otherwise stopped running
+                # break this loop
                 break
+
+            # since we are at this point, we are not "idle" anymore.
             self.idle.clear()
+
             message = json.loads(msg)
             if "id" in message:
                 # response to our command
                 if message["id"] in self.connection.mapper:
+                    # get the corresponding Transaction
                     tx = self.connection.mapper[message["id"]]
+                    logger.debug("got answer for %s", tx)
+                    # complete the transaction, which is a Future object
+                    # and thus will return to anyone awaiting it.
                     tx(**message)
             else:
                 # probably an event
                 try:
                     event = cdp.util.parse_json_event(message)
-                    # self.history.append(event)
                     event_tx = EventTransaction(event)
-                    # getattr(globals(), event.__class__.__module__)
                     if not self.connection.mapper:
                         self.connection.__count__ = itertools.count(0)
                     event_tx.id = next(self.connection.__count__)
                     self.connection.mapper[event_tx.id] = event_tx
-                    # while len(self.connection.mapper) > self.max_history:
-                    #     for k,v in self.connection.mapper.copy().items():
-                    #         # only remove old events
-                    #         if type(v) is not Transaction:
-                    #             self.connection.mapper.pop(k)
-
-                    # while len(self.history) >= self.max_history:
-                    #     self.history.popleft()
                 except Exception as e:
                     logger.info(
                         "%s: %s  during parsing of json from event : %s"
                         % (type(e).__name__, e.args, message),
                         exc_info=True,
                     )
                     continue
@@ -582,25 +576,22 @@
                     logger.info("some lousy KeyError %s" % e, exc_info=True)
                     continue
                 try:
                     if type(event) in self.connection.handlers:
                         callbacks = self.connection.handlers[type(event)]
                     else:
                         continue
-
                     if not len(callbacks):
                         continue
-
                     for callback in callbacks:
                         try:
                             if iscoroutinefunction(callback) or iscoroutine(callback):
                                 await callback(event)
                             else:
                                 callback(event)
-
                         except Exception as e:
                             logger.warning(
                                 "exception in callback %s for event %s => %s",
                                 callback,
                                 event.__class__.__name__,
                                 e,
                                 exc_info=True,
```

### Comparing `nodriver-0.27rc3/nodriver/core/element.py` & `nodriver-0.28rc1/nodriver/core/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,19 @@
 
     def __getitem__(self, item):
         # we probably deal with an attribute of
         # the html element, so forward it
         return self.attrs.get(item, None)
 
     async def save_to_dom(self):
+        """
+        saves a screenshot of this element only
+        :return:
+        :rtype:
+        """
         self._remote_object = await self._tab.send(
             cdp.dom.resolve_node(backend_node_id=self.backend_node_id)
         )
         await self._tab.send(cdp.dom.set_outer_html(self.node_id, outer_html=str(self)))
         await self.update()
 
     async def remove_from_dom(self):
@@ -854,14 +859,40 @@
                 object_id=self._remote_object.object_id,
                 arguments=arguments,
                 await_promise=True,
                 user_gesture=True,
             )
         )
 
+    async def highlight_overlay(self):
+        """
+        highlights the element devtools-style. To remove the highlight,
+        call the method again.
+        :return:
+        :rtype:
+        """
+
+        if getattr(self, "_is_highlighted", False):
+            del self._is_highlighted
+            await self.tab.send(cdp.overlay.hide_highlight())
+            await self.tab.send(cdp.dom.disable())
+            await self.tab.send(cdp.overlay.disable())
+            return
+        await self.tab.send(cdp.dom.enable())
+        await self.tab.send(cdp.overlay.enable())
+        conf = cdp.overlay.HighlightConfig(
+            show_info=True, show_extension_lines=True, show_styles=True
+        )
+        await self.tab.send(
+            cdp.overlay.highlight_node(
+                highlight_config=conf, backend_node_id=self.backend_node_id
+            )
+        )
+        setattr(self, "_is_highlighted", 1)
+
     async def record_video(
         self,
         filename: typing.Optional[str] = None,
         folder: typing.Optional[str] = None,
         duration: typing.Optional[typing.Union[int, float]] = None,
     ):
         """
```

### Comparing `nodriver-0.27rc3/nodriver/core/tab.py` & `nodriver-0.28rc1/nodriver/core/tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,25 +191,27 @@
                  # ignore the return_enclosing_element flag if the found node is NOT a text node but a
                  # regular element (one having a tag) in which case that is exactly what we need.
          :type return_enclosing_element: bool
         :param timeout: raise timeout exception when after this many seconds nothing is found.
         :type timeout: float,int
         """
         loop = asyncio.get_running_loop()
-        now = loop.time()
+        start_time = loop.time()
+
+        text = text.strip()
 
         item = await self.find_element_by_text(
             text, best_match, return_enclosing_element
         )
         while not item:
             await self
             item = await self.find_element_by_text(
                 text, best_match, return_enclosing_element
             )
-            if loop.time() - now > timeout:
+            if loop.time() - start_time > timeout:
                 raise asyncio.TimeoutError(
                     "time ran out while waiting for text: %s" % text
                 )
             await self.sleep(0.5)
         return item
 
     async def select(
@@ -225,21 +227,23 @@
         :type selector: str
 
         :param timeout: raise timeout exception when after this many seconds nothing is found.
         :type timeout: float,int
 
         """
         loop = asyncio.get_running_loop()
-        now = loop.time()
+        start_time = loop.time()
 
+        selector = selector.strip()
         item = await self.query_selector(selector)
+
         while not item:
             await self
             item = await self.query_selector(selector)
-            if loop.time() - now > timeout:
+            if loop.time() - start_time > timeout:
                 raise asyncio.TimeoutError(
                     "time ran out while waiting for %s" % selector
                 )
             await self.sleep(0.5)
         return item
 
     async def find_all(
@@ -256,24 +260,26 @@
 
         :param timeout: raise timeout exception when after this many seconds nothing is found.
         :type timeout: float,int
         """
         loop = asyncio.get_running_loop()
         now = loop.time()
 
-        results = await self.find_elements_by_text(text)
-        while not results:
+        text = text.strip()
+        items = await self.find_elements_by_text(text)
+
+        while not items:
             await self
             results = await self.find_elements_by_text(text)
             if loop.time() - now > timeout:
                 raise asyncio.TimeoutError(
                     "time ran out while waiting for text: %s" % text
                 )
             await self.sleep(0.5)
-        return results
+        return items
 
     async def select_all(
         self,
         selector: str,
         timeout: Union[int, float] = 10,
     ) -> List[nodriver.Element]:
         """
@@ -284,24 +290,26 @@
         :type selector: str
         :param timeout: raise timeout exception when after this many seconds nothing is found.
         :type timeout: float,int
         """
 
         loop = asyncio.get_running_loop()
         now = loop.time()
-        results = await self.query_selector_all(selector)
-        while not results:
+        selector = selector.strip()
+
+        items = await self.query_selector_all(selector)
+        while not items:
             await self
-            results = await self.query_selector_all(selector)
+            items = await self.query_selector_all(selector)
             if loop.time() - now > timeout:
                 raise asyncio.TimeoutError(
                     "time ran out while waiting for %s" % selector
                 )
             await self.sleep(0.5)
-        return results
+        return items
 
     async def get(
         self, url="chrome://welcome", new_tab: bool = False, new_window: bool = False
     ):
         """top level get. utilizes the first tab to retrieve given url.
 
         convenience function known from selenium.
@@ -373,40 +381,41 @@
                     )
                     return await self.query_selector_all(selector, _node)
             else:
                 await self.send(cdp.dom.disable())
                 raise
         if not node_ids:
             return []
-        results = []
+        items = []
 
         for nid in node_ids:
             node = util.filter_recurse(doc, lambda n: n.node_id == nid)
             # we pass along the retrieved document tree,
             # to improve performance
             if not node:
                 continue
             elem = element.create(node, self, doc)
-            results.append(elem)
+            items.append(elem)
 
-        return results
+        return items
 
     async def query_selector(
         self,
         selector: str,
         _node: Optional[Union[cdp.dom.Node, element.Element]] = None,
     ):
         """
         find single element based on css selector string
 
         :param selector: css selector(s)
         :type selector: str
         :return:
         :rtype:
         """
+        selector = selector.strip()
 
         if not _node:
             doc: cdp.dom.Node = await self.send(cdp.dom.get_document(-1, True))
         else:
             doc = _node
             if _node.node_name == "IFRAME":
                 doc = _node.content_document
@@ -451,27 +460,27 @@
         :param text:
         :type text:
         :param tag_hint: when provided, narrows down search to only elements which match given tag eg: a, div, script, span
         :type tag_hint: str
         :return:
         :rtype:
         """
-
+        text = text.strip()
         doc = await self.send(cdp.dom.get_document(-1, True))
         search_id, nresult = await self.send(cdp.dom.perform_search(text, True))
         if nresult:
             node_ids = await self.send(
                 cdp.dom.get_search_results(search_id, 0, nresult)
             )
         else:
             node_ids = []
 
         await self.send(cdp.dom.discard_search_results(search_id))
 
-        results = []
+        items = []
         for nid in node_ids:
             node = util.filter_recurse(doc, lambda n: n.node_id == nid)
             if not node:
                 node = await self.send(cdp.dom.resolve_node(node_id=nid))
                 if not node:
                     continue
                 # remote_object = await self.send(cdp.dom.resolve_node(backend_node_id=node.backend_node_id))
@@ -485,21 +494,21 @@
                 # we return the parent element of the node (which is often a tag which can have text between their
                 # opening and closing tags (that is most tags, except for example "img" and "video", "br")
 
                 if not elem.parent:
                     # check if parent actually has a parent and update it to be absolutely sure
                     await elem.update()
 
-                results.append(
+                items.append(
                     elem.parent or elem
                 )  # when it really has no parent, use the text node itself
                 continue
             else:
                 # just add the element itself
-                results.append(elem)
+                items.append(elem)
 
         # since we already fetched the entire doc, including shadow and frames
         # let's also search through the iframes
         iframes = util.filter_recurse_all(doc, lambda node: node.node_name == "IFRAME")
         if iframes:
             iframes_elems = [
                 element.create(iframe, self, iframe.content_document)
@@ -513,19 +522,19 @@
                         and text.lower() in node.node_value.lower(),
                     )
                     if iframe_text_nodes:
                         iframe_text_elems = [
                             element.create(text_node, self, iframe_elem.tree)
                             for text_node in iframe_text_nodes
                         ]
-                        results.extend(
+                        items.extend(
                             text_node.parent for text_node in iframe_text_elems
                         )
         await self.send(cdp.dom.disable())
-        return results or []
+        return items or []
 
     async def find_element_by_text(
         self,
         text: str,
         best_match: Optional[bool] = False,
         return_enclosing_element: Optional[bool] = True,
     ) -> Union[element.Element, None]:
@@ -543,22 +552,22 @@
         :param return_enclosing_element:
         :type return_enclosing_element:
         :return:
         :rtype:
         """
         doc = await self.send(cdp.dom.get_document(-1, True))
         search_id, nresult = await self.send(cdp.dom.perform_search(text, True))
-        # if nresult == 0:
-        #     return
+        text = text.strip()
+
         node_ids = await self.send(cdp.dom.get_search_results(search_id, 0, nresult))
         await self.send(cdp.dom.discard_search_results(search_id))
 
         if not node_ids:
             node_ids = []
-        results = []
+        items = []
         for nid in node_ids:
             node = util.filter_recurse(doc, lambda n: n.node_id == nid)
             try:
                 elem = element.create(node, self, doc)
             except:  # noqa
                 continue
             if elem.node_type == 3:
@@ -566,21 +575,21 @@
                 # we return the parent element of the node (which is often a tag which can have text between their
                 # opening and closing tags (that is most tags, except for example "img" and "video", "br")
 
                 if not elem.parent:
                     # check if parent actually has a parent and update it to be absolutely sure
                     await elem.update()
 
-                results.append(
+                items.append(
                     elem.parent or elem
                 )  # when it really has no parent, use the text node itself
                 continue
             else:
                 # just add the element itself
-                results.append(elem)
+                items.append(elem)
 
         # since we already fetched the entire doc, including shadow and frames
         # let's also search through the iframes
         iframes = util.filter_recurse_all(doc, lambda node: node.node_name == "IFRAME")
         if iframes:
             iframes_elems = [
                 element.create(iframe, self, iframe.content_document)
@@ -593,28 +602,28 @@
                     and text.lower() in node.node_value.lower(),
                 )
                 if iframe_text_nodes:
                     iframe_text_elems = [
                         element.create(text_node, self, iframe_elem.tree)
                         for text_node in iframe_text_nodes
                     ]
-                    results.extend(text_node.parent for text_node in iframe_text_elems)
+                    items.extend(text_node.parent for text_node in iframe_text_elems)
         try:
-            if not results:
+            if not items:
                 return
             if best_match:
                 closest_by_length = min(
-                    results, key=lambda el: abs(len(text) - len(el.text_all))
+                    items, key=lambda el: abs(len(text) - len(el.text_all))
                 )
-                elem = closest_by_length or results[0]
+                elem = closest_by_length or items[0]
 
                 return elem
             else:
                 # naively just return the first result
-                for elem in results:
+                for elem in items:
                     if elem:
                         return elem
         finally:
             await self.send(cdp.dom.disable())
 
     async def back(self):
         """
@@ -655,37 +664,27 @@
     ):
         remote_object, errors = await self.send(
             cdp.runtime.evaluate(
                 expression=expression,
                 user_gesture=True,
                 await_promise=await_promise,
                 return_by_value=return_by_value,
+                allow_unsafe_eval_blocked_by_csp=True,
             )
         )
         if errors:
             raise ProtocolException(errors)
-            if not return_by_value:
-                return remote_object, errors
-            return errors.to_json()
+
         if remote_object:
             if return_by_value:
                 if remote_object.value:
                     return remote_object.value
 
             else:
                 return remote_object, errors
-            # if getattr(remote_object, "subtype", None) == "error":
-            #     val = remote_object.description
-            #     return {"error": val, "stack": errors}
-        #     try:
-        #         return json.loads(remote_object.value)
-        #     except:
-        #         return remote_object.value
-        # if exc:
-        #     return exc
 
     async def js_dumps(
         self, obj_name: str, return_by_value: Optional[bool] = True
     ) -> typing.Union[
         typing.Dict,
         typing.Tuple[cdp.runtime.RemoteObject, cdp.runtime.ExceptionDetails],
     ]:
@@ -943,15 +942,18 @@
         """
         await self.activate()
 
     async def set_window_state(
         self, left=0, top=0, width=1280, height=720, state="normal"
     ):
         """
-        sets the window size and state.
+        sets the window size or state.
+
+        for state you can provide the full name like minimized, maximized, normal, fullscreen, or
+        something which leads to either of those, like min, mini, mi,  max, ma, maxi, full, fu, no, nor
         in case state is set other than "normal", the left, top, width, and height are ignored.
 
         :param left:
             desired offset from left, in pixels
         :type left: int
 
         :param top:
@@ -991,19 +993,17 @@
             )
         window_state = getattr(
             cdp.browser.WindowState, state_name.upper(), cdp.browser.WindowState.NORMAL
         )
         if window_state == cdp.browser.WindowState.NORMAL:
             bounds = cdp.browser.Bounds(left, top, width, height, window_state)
         else:
-            window_id, current_bounds = await self.get_window()
-            if current_bounds.window_state != cdp.browser.WindowState.NORMAL:
-                # min, max, full can only be used when current state == NORMAL
-                # therefore we first switch to NORMAL
-                await self.set_window_state(state="normal")
+            # min, max, full can only be used when current state == NORMAL
+            # therefore we first switch to NORMAL
+            await self.set_window_state(state="normal")
             bounds = cdp.browser.Bounds(window_state=window_state)
 
         await self.send(cdp.browser.set_window_bounds(window_id, bounds=bounds))
 
     async def scroll_down(self, amount=25):
         """
         scrolls down maybe
@@ -1205,15 +1205,17 @@
             dt_str = datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
             candidate = f"{parsed.hostname}__{last_part}_{dt_str}"
             path = pathlib.Path(candidate + ext)  # noqa
         else:
             path = pathlib.Path(filename)
         path.parent.mkdir(parents=True, exist_ok=True)
         data = await self.send(
-            cdp.page.capture_screenshot(format_=format, capture_beyond_viewport=True)
+            cdp.page.capture_screenshot(
+                format_=format, capture_beyond_viewport=full_page
+            )
         )
         if not data:
             raise ProtocolException(
                 "could not take screenshot. most possible cause is the page has not finished loading yet."
             )
         import base64
 
@@ -1276,14 +1278,15 @@
                         )
                         if not abs_url.startswith(("http", "//", "ws")):
                             continue
                         res.append(abs_url)
         return res
 
     async def verify_cf(self):
+        """an attempt.."""
         checkbox = None
         checkbox_sibling = await self.wait_for(text="verify you are human")
         if checkbox_sibling:
             parent = checkbox_sibling.parent
             while parent:
                 checkbox = await parent.query_selector("input[type=checkbox]")
                 if checkbox:
```

### Comparing `nodriver-0.27rc3/nodriver/core/util.py` & `nodriver-0.28rc1/nodriver/core/util.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.27rc3/nodriver.egg-info/PKG-INFO` & `nodriver-0.28rc1/nodriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodriver
-Version: 0.27rc3
+Version: 0.28rc1
 Summary: * Official successor of Undetected Chromedriver
 Author-email: UltrafunkAmsterdam <doesnotexist@ultrafunk.nl>
 Maintainer-email: UltrafunkAmsterdam <doesnotexist@ultrafunk.nl>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `nodriver-0.27rc3/nodriver.egg-info/SOURCES.txt` & `nodriver-0.28rc1/nodriver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,9 +64,10 @@
 nodriver/cdp/web_audio.py
 nodriver/cdp/web_authn.py
 nodriver/core/_contradict.py
 nodriver/core/browser.py
 nodriver/core/config.py
 nodriver/core/connection.py
 nodriver/core/element.py
+nodriver/core/extra.py
 nodriver/core/tab.py
 nodriver/core/util.py
```

### Comparing `nodriver-0.27rc3/pyproject.toml` & `nodriver-0.28rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nodriver" # Required
-version = "0.27rc3"  # Required
+version = "0.28rc1"  # Required
 description = """
     * Official successor of Undetected Chromedriver
     * Can be made to work for for all chromium based browsers.
     * Dropped selenium and chromedriver binary requirements.
     * fully asynchronous == bizarre performance gains, and more granular control
 
     Part of undetected-chromedriver, or merely the successor of it, this library is a full rewrite, providing a
```

