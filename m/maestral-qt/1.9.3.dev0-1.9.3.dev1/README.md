# Comparing `tmp/maestral-qt-1.9.3.dev0.tar.gz` & `tmp/maestral_qt-1.9.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestral-qt-1.9.3.dev0.tar", last modified: Wed Mar 27 22:45:57 2024, max compression
+gzip compressed data, was "maestral_qt-1.9.3.dev1.tar", last modified: Sat Apr 13 13:51:32 2024, max compression
```

## Comparing `maestral-qt-1.9.3.dev0.tar` & `maestral_qt-1.9.3.dev1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:45:57.071478 maestral-qt-1.9.3.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-27 22:45:57.071478 maestral-qt-1.9.3.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-27 22:45:57.071478 maestral-qt-1.9.3.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:45:57.059478 maestral-qt-1.9.3.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:45:57.059478 maestral-qt-1.9.3.dev0/src/maestral_qt/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:45:57.063478 maestral-qt-1.9.3.dev0/src/maestral_qt/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/__pyinstaller/hook-maestral_qt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/activity_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/autostart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/bandwidth_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/dropbox_location_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    20646 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/relink_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:45:57.067478 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   204933 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/faceholder.png
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/file
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral.desktop
--rw-r--r--   0 runner    (1001) docker     (127)   842667 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral.icns
--rw-r--r--   0 runner    (1001) docker     (127)   137001 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral.png
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-disconnected-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-disconnected-light.svg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-error-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-error-light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-idle-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-idle-light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-info-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-info-light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-paused-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-paused-light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-syncing-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-syncing-light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_bandwidth_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_dropbox_location_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_relink_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_selective_sync_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    13222 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_settings_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    21923 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_setup_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_sync_event_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_sync_issue_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_sync_issues_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_unlink_dialog.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20745 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/selective_sync_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/settings_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/setup_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/sync_issues_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    11493 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21720 2024-03-27 22:45:49.000000 maestral-qt-1.9.3.dev0/src/maestral_qt/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:45:57.067478 maestral-qt-1.9.3.dev0/src/maestral_qt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-27 22:45:57.000000 maestral-qt-1.9.3.dev0/src/maestral_qt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-27 22:45:57.000000 maestral-qt-1.9.3.dev0/src/maestral_qt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 22:45:57.000000 maestral-qt-1.9.3.dev0/src/maestral_qt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-27 22:45:57.000000 maestral-qt-1.9.3.dev0/src/maestral_qt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 22:45:57.000000 maestral-qt-1.9.3.dev0/src/maestral_qt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-27 22:45:57.000000 maestral-qt-1.9.3.dev0/src/maestral_qt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-27 22:45:57.000000 maestral-qt-1.9.3.dev0/src/maestral_qt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:32.083010 maestral_qt-1.9.3.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-13 13:51:32.083010 maestral_qt-1.9.3.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-13 13:51:32.087010 maestral_qt-1.9.3.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:32.075010 maestral_qt-1.9.3.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:32.075010 maestral_qt-1.9.3.dev1/src/maestral_qt/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:32.079010 maestral_qt-1.9.3.dev1/src/maestral_qt/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/__pyinstaller/hook-maestral_qt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/activity_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/autostart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/bandwidth_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/dropbox_location_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20646 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/relink_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:32.083010 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   204933 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/faceholder.png
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/file
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)   842667 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral.icns
+-rw-r--r--   0 runner    (1001) docker     (127)   137001 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-disconnected-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-disconnected-light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-error-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-error-light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-idle-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-idle-light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-info-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-info-light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-paused-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-paused-light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-syncing-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-syncing-light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_bandwidth_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_dropbox_location_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_relink_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_selective_sync_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13222 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_settings_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21923 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_setup_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_sync_event_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_sync_issue_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_sync_issues_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_unlink_dialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20745 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/selective_sync_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/settings_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/setup_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/sync_issues_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11493 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21720 2024-04-13 13:51:27.000000 maestral_qt-1.9.3.dev1/src/maestral_qt/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:51:32.083010 maestral_qt-1.9.3.dev1/src/maestral_qt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-13 13:51:32.000000 maestral_qt-1.9.3.dev1/src/maestral_qt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-13 13:51:32.000000 maestral_qt-1.9.3.dev1/src/maestral_qt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:51:32.000000 maestral_qt-1.9.3.dev1/src/maestral_qt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-13 13:51:32.000000 maestral_qt-1.9.3.dev1/src/maestral_qt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:51:32.000000 maestral_qt-1.9.3.dev1/src/maestral_qt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-13 13:51:32.000000 maestral_qt-1.9.3.dev1/src/maestral_qt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 13:51:32.000000 maestral_qt-1.9.3.dev1/src/maestral_qt.egg-info/top_level.txt
```

### Comparing `maestral-qt-1.9.3.dev0/LICENSE.txt` & `maestral_qt-1.9.3.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/PKG-INFO` & `maestral_qt-1.9.3.dev1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral-qt
-Version: 1.9.3.dev0
+Version: 1.9.3.dev1
 Summary: A Qt GUI for the Maestral daemon
 Home-page: https://maestral.app
 Author: Sam Schott
 Author-email: sam.schott@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: click>=7.1.1
-Requires-Dist: maestral>=1.9.3.dev0
+Requires-Dist: maestral>=1.9.3.dev1
 Requires-Dist: markdown2
 Requires-Dist: packaging
 Requires-Dist: PyQt6
 
 [![PyPi Release](https://img.shields.io/pypi/v/maestral-qt.svg)](https://pypi.org/project/maestral-qt/)
 [![Pyversions](https://img.shields.io/pypi/pyversions/maestral-qt.svg)](https://pypi.org/pypi/maestral-qt/)
```

### Comparing `maestral-qt-1.9.3.dev0/setup.cfg` & `maestral_qt-1.9.3.dev1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = maestral-qt
-version = 1.9.3.dev0
+version = 1.9.3.dev1
 author = Sam Schott
 author_email = sam.schott@outlook.com
 license = MIT
 description = A Qt GUI for the Maestral daemon
 url = https://maestral.app
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -24,15 +24,15 @@
 packages = find:
 package_dir = 
 	= src
 zip_safe = False
 setup_requires = wheel
 install_requires = 
 	click>=7.1.1
-	maestral>=1.9.3.dev0
+	maestral>=1.9.3.dev1
 	markdown2
 	packaging
 	PyQt6
 python_requires = >=3.7
 
 [options.packages.find]
 where = src
```

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/activity_window.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/activity_window.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/autostart.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/autostart.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/bandwidth_dialog.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/bandwidth_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/dropbox_location_dialog.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/dropbox_location_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/main.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/main.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/relink_dialog.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/relink_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/__init__.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/faceholder.png` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/faceholder.png`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral.icns` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral.icns`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral.png` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral.png`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-disconnected-dark.svg` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-disconnected-dark.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-disconnected-light.svg` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-disconnected-light.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-error-dark.svg` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-error-dark.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-error-light.svg` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-error-light.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-idle-dark.svg` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-idle-dark.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-idle-light.svg` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-idle-light.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-info-dark.svg` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-info-dark.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-info-light.svg` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-info-light.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-paused-dark.svg` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-paused-dark.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-paused-light.svg` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-paused-light.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-syncing-dark.svg` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-syncing-dark.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/maestral_tray-syncing-light.svg` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/maestral_tray-syncing-light.svg`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_bandwidth_dialog.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_bandwidth_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_dropbox_location_dialog.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_dropbox_location_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_relink_dialog.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_relink_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_selective_sync_dialog.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_selective_sync_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_settings_window.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_settings_window.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_setup_dialog.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_setup_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_sync_event_widget.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_sync_event_widget.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_sync_issue_widget.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_sync_issue_widget.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_sync_issues_window.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_sync_issues_window.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/resources/ui_unlink_dialog.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/resources/ui_unlink_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/selective_sync_dialog.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/selective_sync_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/settings_window.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/settings_window.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/setup_dialog.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/setup_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/sync_issues_window.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/sync_issues_window.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/utils.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/utils.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt/widgets.py` & `maestral_qt-1.9.3.dev1/src/maestral_qt/widgets.py`

 * *Files identical despite different names*

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt.egg-info/PKG-INFO` & `maestral_qt-1.9.3.dev1/src/maestral_qt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral-qt
-Version: 1.9.3.dev0
+Version: 1.9.3.dev1
 Summary: A Qt GUI for the Maestral daemon
 Home-page: https://maestral.app
 Author: Sam Schott
 Author-email: sam.schott@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: click>=7.1.1
-Requires-Dist: maestral>=1.9.3.dev0
+Requires-Dist: maestral>=1.9.3.dev1
 Requires-Dist: markdown2
 Requires-Dist: packaging
 Requires-Dist: PyQt6
 
 [![PyPi Release](https://img.shields.io/pypi/v/maestral-qt.svg)](https://pypi.org/project/maestral-qt/)
 [![Pyversions](https://img.shields.io/pypi/pyversions/maestral-qt.svg)](https://pypi.org/pypi/maestral-qt/)
```

### Comparing `maestral-qt-1.9.3.dev0/src/maestral_qt.egg-info/SOURCES.txt` & `maestral_qt-1.9.3.dev1/src/maestral_qt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

