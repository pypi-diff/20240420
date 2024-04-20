# Comparing `tmp/maestral-cocoa-1.9.3.dev0.tar.gz` & `tmp/maestral_cocoa-1.9.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestral-cocoa-1.9.3.dev0.tar", last modified: Wed Mar 27 22:46:05 2024, max compression
+gzip compressed data, was "maestral_cocoa-1.9.3.dev1.tar", last modified: Sat Apr 13 13:51:40 2024, max compression
```

## Comparing `maestral-cocoa-1.9.3.dev0.tar` & `maestral_cocoa-1.9.3.dev1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:46:05.022549 maestral-cocoa-1.9.3.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-27 22:46:05.022549 maestral-cocoa-1.9.3.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-27 22:46:05.022549 maestral-cocoa-1.9.3.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:46:05.010549 maestral-cocoa-1.9.3.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:46:05.014549 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)    17561 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/autostart.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/bandwidth_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/dbx_location_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:46:05.018549 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:46:05.018549 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/implementation/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/implementation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:46:05.018549 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/implementation/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/implementation/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/implementation/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/implementation/cocoa/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22656 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/implementation/cocoa/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:46:05.018549 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/implementation/gtk/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/implementation/gtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/implementation/gtk/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    19822 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:46:05.022549 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48199 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/faceholder.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   842676 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/maestral.icns
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/release_notes.css
--rw-r--r--   0 runner    (1001) docker     (127)    51081 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/systray-disconnected.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    47443 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/systray-error.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    52917 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/systray-idle.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    52604 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/systray-info.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    46340 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/systray-paused.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    50085 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/systray-syncing.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/selective_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/selective_sync_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11846 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/settings_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/setup_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/syncissues.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-03-27 22:45:56.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:46:05.022549 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-27 22:46:04.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-27 22:46:05.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 22:46:04.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-27 22:46:05.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 22:46:04.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-27 22:46:05.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-27 22:46:05.000000 maestral-cocoa-1.9.3.dev0/src/maestral_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.872508 maestral_cocoa-1.9.3.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-13 13:51:40.872508 maestral_cocoa-1.9.3.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-13 13:51:40.872508 maestral_cocoa-1.9.3.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.856508 maestral_cocoa-1.9.3.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.864508 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17561 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/autostart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/bandwidth_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/dbx_location_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/dialogs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.864508 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.864508 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.864508 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24641 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.864508 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/gtk/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/gtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/gtk/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19822 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.868508 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48199 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/faceholder.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   842676 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/maestral.icns
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/release_notes.css
+-rw-r--r--   0 runner    (1001) docker     (127)    51081 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-disconnected.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    47443 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-error.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    52917 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-idle.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    52604 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-info.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    46340 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-paused.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    50085 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-syncing.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/selective_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/selective_sync_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11846 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/settings_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/setup_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/syncissues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-13 13:51:32.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:40.868508 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-13 13:51:40.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-13 13:51:40.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:51:40.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 13:51:40.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:51:40.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-13 13:51:40.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 13:51:40.000000 maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/top_level.txt
```

### Comparing `maestral-cocoa-1.9.3.dev0/LICENSE.txt` & `maestral_cocoa-1.9.3.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/PKG-INFO` & `maestral_cocoa-1.9.3.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral-cocoa
-Version: 1.9.3.dev0
+Version: 1.9.3.dev1
 Summary: Open-source Dropbox client for macOS and Linux.
 Home-page: https://maestral.app
 Author: Sam Schott
 Author-email: sam.schott@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: click
-Requires-Dist: maestral>=1.9.3.dev0
+Requires-Dist: maestral>=1.9.3.dev1
 Requires-Dist: markdown2
 Requires-Dist: toga==0.4.2
 Requires-Dist: rubicon-objc>=0.4.5
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
```

### Comparing `maestral-cocoa-1.9.3.dev0/pyproject.toml` & `maestral_cocoa-1.9.3.dev1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.briefcase]
 project_name = "Maestral"
 bundle = "com.samschott.maestral"
-version = "1.9.3.dev0"
+version = "1.9.3.dev1"
 url = "https://maestral.app"
 license = "MIT license"
 author = "Sam Schott"
 author_email = "sam.schott@outlook.com"
 template = "https://github.com/samschott/briefcase-macOS-Xcode-template.git"
 template_branch = "maestral-v2"
 
@@ -13,15 +13,15 @@
 formal_name = "Maestral"
 description = "An open-source Dropbox client for macOS and Linux"
 icon = "icon/maestral"
 sources = ["src/maestral_cocoa"]
 requires = [
     "chardet==5.2.0",
     "click==8.1.7",
-    "maestral==1.9.3.dev0",
+    "maestral==1.9.3.dev1",
     "markdown2==2.4.13",
     "rubicon-objc==0.4.7",
     "toga==0.4.2",
 ]
 sparkle_feed_url = "https://maestral.app/appcast.xml"
 sparkle_public_key = "RugM2eM14xHixaeHpl5uWSq7+sDZvYi52Xpz4IXpAdA="
 
@@ -29,15 +29,15 @@
 entitlement."com.apple.security.cs.disable-library-validation" = false
 requires = [
     "toga-cocoa==0.4.2",
 ]
 cleanup_paths = [
     "*/unittest",
 ]
-build = "102"
+build = "103"
 
 [tool.briefcase.app.maestral-cocoa.linux]
 supported = false
 
 [tool.black]
 line-length = 88
 target-version = ["py37", "py38", "py39", "py310", "py311"]
```

### Comparing `maestral-cocoa-1.9.3.dev0/setup.cfg` & `maestral_cocoa-1.9.3.dev1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = maestral-cocoa
-version = 1.9.3.dev0
+version = 1.9.3.dev1
 author = Sam Schott
 author_email = sam.schott@outlook.com
 license = MIT
 description = Open-source Dropbox client for macOS and Linux.
 url = https://maestral.app
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -24,15 +24,15 @@
 packages = find:
 package_dir = 
 	= src
 zip_safe = False
 setup_requires = build
 install_requires = 
 	click
-	maestral>=1.9.3.dev0
+	maestral>=1.9.3.dev1
 	markdown2
 	toga==0.4.2
 	rubicon-objc>=0.4.5
 python_requires = >=3.8
 
 [options.packages.find]
 where = src
```

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/__main__.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/__main__.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/activity.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/activity.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/app.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/app.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/autostart.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/autostart.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/bandwidth.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/bandwidth.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/bandwidth_gui.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/bandwidth_gui.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/dbx_location_dialog.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/dbx_location_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/dialogs.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/dialogs.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/implementation/cocoa/constants.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/constants.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/implementation/cocoa/dialogs.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/dialogs.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/implementation/cocoa/factory.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/implementation/cocoa/factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,16 @@
     NSModalResponseOK,
     NSCompositingOperationCopy,
     NSURL,
     NSButton,
     NSSwitchButton,
     NSRadioButton,
     NSApplication,
+    NSData,
+    NSSize,
 )
 from toga_cocoa.colors import native_color
 from toga_cocoa.keys import cocoa_key
 from toga_cocoa.app import App as TogaApp
 from toga_cocoa.widgets.base import Widget
 from toga_cocoa.widgets.button import Button as TogaButton
 from toga_cocoa.window import Window as TogaWindow
@@ -115,58 +117,106 @@
     """Reimplements toga.Icon with support for
 
     1. Platform template images.
     2. Providing the icon for the file / folder type instead of loading an icon from
        the file content.
     """
 
+    EXTENSIONS = [".icns", ".png", ".pdf"]
+    SIZES = None
+
     _to_cocoa_template = {
         None: None,
         ImageTemplate.Refresh: NSImageNameRefreshFreestandingTemplate,
         ImageTemplate.FollowLink: NSImageNameFollowLinkFreestandingTemplate,
         ImageTemplate.Reveal: NSImageNameRevealFreestandingTemplate,
         ImageTemplate.InvalidData: NSImageNameInvalidDataFreestandingTemplate,
         ImageTemplate.StopProgress: NSImageNameStopProgressFreestandingTemplate,
     }
 
-    SIZES = None
-    EXTENSIONS = [".icns", ".png", ".pdf"]
-
-    def __init__(self, interface, path=None, for_path=None, template=None):
+    def __init__(self, interface, path, for_path=None, template=None):
         self.interface = interface
         self.interface._impl = self
-        self.path = str(path) if path else None
-        self.for_path = for_path
-        self.template = template
-
-        self._native = None
-
-    @property
-    def native(self):
-        if self._native:
-            return self._native
-
-        if self.path:
-            self._native = NSImage.alloc().initWithContentsOfFile(self.path)
-
-        elif self.for_path:
-            # always return a new pointer since an old one may be invalidated
-            # icons are cached by AppKit anyways
-            path = str(self.for_path)
+        self.path = path
+
+        if path:
+            self.native = NSImage.alloc().initWithContentsOfFile(str(path))
+            self.native.retain()
+
+        elif for_path:
+            path = str(for_path)
             if osp.exists(path):
-                self._native = NSWorkspace.sharedWorkspace.iconForFile(path)
+                self.native = NSWorkspace.sharedWorkspace.iconForFile(path)
             else:
                 _, extension = osp.splitext(path)
-                self._native = NSWorkspace.sharedWorkspace.iconForFileType(extension)
+                self.native = NSWorkspace.sharedWorkspace.iconForFileType(extension)
+
+        elif template:
+            cocoa_template = Icon._to_cocoa_template[template]
+            self.native = NSImage.imageNamed(cocoa_template)
+
+        self.native.retain()
 
-        elif self.template:
-            cocoa_template = Icon._to_cocoa_template[self.template]
-            self._native = NSImage.imageNamed(cocoa_template)
+    def __del__(self):
+        self.native.autorelease()
+
+    def _as_size(self, size):
+        image = self.native.copy()
+        image.setSize(NSSize(size, size))
+        return image
+
+
+# ==== image ===========================================================================
+
+
+class Image:
+    RAW_TYPE = NSImage
+
+    def __init__(self, interface, path=None, data=None, raw=None):
+        self.interface = interface
+        self._needs_release = False
+
+        try:
+            # We *should* be able to do a direct NSImage.alloc.init...(), but if the
+            # image file is invalid, the init fails, returns NULL, and releases the
+            # Objective-C object. Since we've created an ObjC instance, when the object
+            # passes out of scope, Rubicon tries to free it, which segfaults.
+            # To avoid this, we retain result of the alloc() (overriding the default
+            # Rubicon behavior of alloc), then release that reference once we're done.
+            # If the image was created successfully, we temporarily have a reference
+            # count that is 1 higher than it needs to be; if it fails, we don't end up
+            # with a stray release.
+            image = NSImage.alloc().retain()
+            if path:
+                self.native = image.initWithContentsOfFile(str(path))
+                if self.native is None:
+                    raise ValueError(f"Unable to load image from {path}")
+                else:
+                    self._needs_release = True
+            elif data:
+                nsdata = NSData.dataWithBytes(data, length=len(data))
+                self.native = image.initWithData(nsdata)
+                if self.native is None:
+                    raise ValueError("Unable to load image from data")
+                else:
+                    self._needs_release = True
+            else:
+                self.native = raw
+        finally:
+            # Calling `release` here disabled Rubicon's "release on delete" automation.
+            # We therefore add an explicit `release` call in __del__ if the NSImage was
+            # initialized successfully.
+            image.release()
+
+    def __del__(self):
+        if self._needs_release:
+            self.native.release()
 
-        return self._native
+    def get_width(self):
+        return self.native.size.width
 
 
 # ==== labels ==========================================================================
 
 
 class Label(Widget):
     """Reimplements toga_cocoa.Label with text wrapping."""
```

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/platform.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/platform.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/private/widgets.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/private/widgets.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/__init__.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/faceholder.pdf` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/faceholder.pdf`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/maestral.icns` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/maestral.icns`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/systray-disconnected.pdf` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-disconnected.pdf`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/systray-error.pdf` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-error.pdf`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/systray-idle.pdf` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-idle.pdf`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/systray-info.pdf` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-info.pdf`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/systray-paused.pdf` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-paused.pdf`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/resources/systray-syncing.pdf` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/resources/systray-syncing.pdf`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/selective_sync.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/selective_sync.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/selective_sync_gui.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/selective_sync_gui.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/settings.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/settings.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/settings_gui.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/settings_gui.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/setup.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/setup.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/setup_gui.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/setup_gui.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/syncissues.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/syncissues.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/updater.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/updater.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa/utils.py` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa/utils.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa.egg-info/PKG-INFO` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral-cocoa
-Version: 1.9.3.dev0
+Version: 1.9.3.dev1
 Summary: Open-source Dropbox client for macOS and Linux.
 Home-page: https://maestral.app
 Author: Sam Schott
 Author-email: sam.schott@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: click
-Requires-Dist: maestral>=1.9.3.dev0
+Requires-Dist: maestral>=1.9.3.dev1
 Requires-Dist: markdown2
 Requires-Dist: toga==0.4.2
 Requires-Dist: rubicon-objc>=0.4.5
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
```

### Comparing `maestral-cocoa-1.9.3.dev0/src/maestral_cocoa.egg-info/SOURCES.txt` & `maestral_cocoa-1.9.3.dev1/src/maestral_cocoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

