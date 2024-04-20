# Comparing `tmp/cdp_patches-1.0.tar.gz` & `tmp/cdp_patches-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdp_patches-1.0.tar", last modified: Sat Mar 23 19:46:43 2024, max compression
+gzip compressed data, was "cdp_patches-1.0.1.tar", last modified: Sat Apr 20 18:44:29 2024, max compression
```

## Comparing `cdp_patches-1.0.tar` & `cdp_patches-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 19:46:43.798834 cdp_patches-1.0/
--rw-rw-rw-   0        0        0      119 2024-03-23 19:46:43.798287 cdp_patches-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       18 2024-03-23 19:46:17.000000 cdp_patches-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-23 19:46:43.790597 cdp_patches-1.0/cdp_patches/
--rw-rw-rw-   0        0        0       40 2024-03-23 19:43:00.000000 cdp_patches-1.0/cdp_patches/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 19:46:43.797174 cdp_patches-1.0/cdp_patches.egg-info/
--rw-rw-rw-   0        0        0      119 2024-03-23 19:46:43.000000 cdp_patches-1.0/cdp_patches.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-03-23 19:46:43.000000 cdp_patches-1.0/cdp_patches.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 19:46:43.000000 cdp_patches-1.0/cdp_patches.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-03-23 19:46:43.000000 cdp_patches-1.0/cdp_patches.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2024-03-23 19:45:18.000000 cdp_patches-1.0/pyproject.toml
--rw-rw-rw-   0        0        0      261 2024-03-23 19:46:43.799889 cdp_patches-1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 18:44:29.768024 cdp_patches-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-10-19 14:25:33.000000 cdp_patches-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     7365 2024-04-20 18:44:29.768024 cdp_patches-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5334 2024-04-20 18:09:53.000000 cdp_patches-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 18:44:29.740071 cdp_patches-1.0.1/cdp_patches/
+-rw-rw-rw-   0        0        0      333 2024-04-20 18:44:19.000000 cdp_patches-1.0.1/cdp_patches/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:44:29.754814 cdp_patches-1.0.1/cdp_patches/input/
+-rw-rw-rw-   0        0        0     5171 2024-04-05 18:23:02.000000 cdp_patches-1.0.1/cdp_patches/input/__init__.py
+-rw-rw-rw-   0        0        0     7910 2024-04-18 12:31:36.000000 cdp_patches-1.0.1/cdp_patches/input/async_input.py
+-rw-rw-rw-   0        0        0    13234 2024-04-18 12:54:55.000000 cdp_patches-1.0.1/cdp_patches/input/browsers.py
+-rw-rw-rw-   0        0        0      437 2024-04-18 12:53:35.000000 cdp_patches-1.0.1/cdp_patches/input/exceptions.py
+-rw-rw-rw-   0        0        0     8789 2024-03-28 14:25:09.000000 cdp_patches-1.0.1/cdp_patches/input/mouse_trajectory.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:44:29.757827 cdp_patches-1.0.1/cdp_patches/input/os_base/
+-rw-rw-rw-   0        0        0        0 2024-04-19 13:51:42.000000 cdp_patches-1.0.1/cdp_patches/input/os_base/__init__.py
+-rw-rw-rw-   0        0        0    11846 2024-04-18 13:34:06.000000 cdp_patches-1.0.1/cdp_patches/input/os_base/linux.py
+-rw-rw-rw-   0        0        0     6591 2024-04-18 13:11:59.000000 cdp_patches-1.0.1/cdp_patches/input/os_base/windows.py
+-rw-rw-rw-   0        0        0     7601 2024-04-18 12:31:36.000000 cdp_patches-1.0.1/cdp_patches/input/sync_input.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:44:29.765018 cdp_patches-1.0.1/cdp_patches.egg-info/
+-rw-rw-rw-   0        0        0     7365 2024-04-20 18:44:29.000000 cdp_patches-1.0.1/cdp_patches.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      724 2024-04-20 18:44:29.000000 cdp_patches-1.0.1/cdp_patches.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 18:44:29.000000 cdp_patches-1.0.1/cdp_patches.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-20 18:42:44.000000 cdp_patches-1.0.1/cdp_patches.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      317 2024-04-20 18:44:29.000000 cdp_patches-1.0.1/cdp_patches.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-20 18:44:29.000000 cdp_patches-1.0.1/cdp_patches.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      705 2024-03-24 19:53:33.000000 cdp_patches-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1646 2024-04-20 18:44:29.769024 cdp_patches-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 18:44:29.763958 cdp_patches-1.0.1/tests/
+-rw-rw-rw-   0        0        0    11897 2024-04-18 14:26:23.000000 cdp_patches-1.0.1/tests/test_async_driverless.py
+-rw-rw-rw-   0        0        0     8747 2024-04-20 17:19:43.000000 cdp_patches-1.0.1/tests/test_async_playwright.py
+-rw-rw-rw-   0        0        0    11647 2024-04-20 17:19:43.000000 cdp_patches-1.0.1/tests/test_selenium.py
+-rw-rw-rw-   0        0        0    11324 2024-04-20 17:19:43.000000 cdp_patches-1.0.1/tests/test_sync_driverless.py
+-rw-rw-rw-   0        0        0     8053 2024-04-20 17:19:43.000000 cdp_patches-1.0.1/tests/test_sync_playwright.py
```

