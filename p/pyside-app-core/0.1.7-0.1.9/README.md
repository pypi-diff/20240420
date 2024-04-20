# Comparing `tmp/pyside-app-core-0.1.7.tar.gz` & `tmp/pyside_app_core-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyside-app-core-0.1.7.tar", last modified: Mon Jul 24 18:33:33 2023, max compression
+gzip compressed data, was "pyside_app_core-0.1.9.tar", last modified: Sat Apr 20 20:34:53 2024, max compression
```

## Comparing `pyside-app-core-0.1.7.tar` & `pyside_app_core-0.1.9.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.649434 pyside-app-core-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    42292 2023-07-24 18:33:33.649434 pyside-app-core-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:33:33.649434 pyside-app-core-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.637434 pyside-app-core-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.637434 pyside-app-core-0.1.7/src/pyside_app_core/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/errors/basic_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/errors/encode_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/errors/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/errors/serial_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/generate_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/console.svg
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/down-arrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/grab-corner.svg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/reload.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/save.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/spin-down/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/spin-down/disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/spin-down/normal.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/spin-up/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/spin-up/disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/spin-up/normal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/standard_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/style_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/templates/resources.qrc.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/templates/style.qss.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/log/
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/qt/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.645434 pyside-app-core-0.1.7/src/pyside_app_core/qt/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/util/pixel_val.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/util/s_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/util/style_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.645434 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/about_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/base_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/error_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.645434 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/base_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/base_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/window_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/window_shade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/menu_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/multi_combo_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/object_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/settings_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/tool_bar_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/tool_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/tool_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/window_settings_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.645434 pyside-app-core-0.1.7/src/pyside_app_core/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/application_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/debug_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/platform_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.645434 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/serial_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.645434 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/conversion_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/float_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.649434 pyside-app-core-0.1.7/src/pyside_app_core/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/types/numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.649434 pyside-app-core-0.1.7/src/pyside_app_core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/utils/compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42292 2023-07-24 18:33:33.000000 pyside-app-core-0.1.7/src/pyside_app_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-24 18:33:33.000000 pyside-app-core-0.1.7/src/pyside_app_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:33:33.000000 pyside-app-core-0.1.7/src/pyside_app_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-24 18:33:33.000000 pyside-app-core-0.1.7/src/pyside_app_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 18:33:33.000000 pyside-app-core-0.1.7/src/pyside_app_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 18:33:33.000000 pyside-app-core-0.1.7/src/pyside_app_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.818882 pyside_app_core-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42650 2024-04-20 20:34:53.818882 pyside_app_core-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 20:34:53.818882 pyside_app_core-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.802882 pyside_app_core-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.806882 pyside_app_core-0.1.9/src/pyside_app_core/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.806882 pyside_app_core-0.1.9/src/pyside_app_core/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/errors/basic_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/errors/encode_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/errors/excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/errors/serial_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/generate_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/console.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/down-arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/grab-corner.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/reload.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/save.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/spin-down/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/spin-down/disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/spin-down/normal.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/spin-up/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/spin-up/disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/spin-up/normal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/standard_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/style_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/templates/resources.qrc.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/templates/style.qss.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/log/
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/qt/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/util/pixel_val.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/util/s_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/util/style_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.814882 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/about_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/base_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/error_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.814882 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/base_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/base_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/window_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/window_shade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/menu_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/multi_combo_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/object_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/settings_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/tool_bar_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/tool_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/tool_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/window_settings_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.814882 pyside_app_core-0.1.9/src/pyside_app_core/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/application_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/debug_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/platform_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.814882 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/serial_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.814882 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/conversion_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/float_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.818882 pyside_app_core-0.1.9/src/pyside_app_core/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/types/numeric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.818882 pyside_app_core-0.1.9/src/pyside_app_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/utils/compare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.818882 pyside_app_core-0.1.9/src/pyside_app_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42650 2024-04-20 20:34:53.000000 pyside_app_core-0.1.9/src/pyside_app_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-20 20:34:53.000000 pyside_app_core-0.1.9/src/pyside_app_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 20:34:53.000000 pyside_app_core-0.1.9/src/pyside_app_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 20:34:53.000000 pyside_app_core-0.1.9/src/pyside_app_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-20 20:34:53.000000 pyside_app_core-0.1.9/src/pyside_app_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-20 20:34:53.000000 pyside_app_core-0.1.9/src/pyside_app_core.egg-info/top_level.txt
```

### Comparing `pyside-app-core-0.1.7/LICENSE` & `pyside_app_core-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/PKG-INFO` & `pyside_app_core-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyside-app-core
-Version: 0.1.7
+Version: 0.1.9
 Summary: Framework for PySide Applications
 Author-email: Leo Covarrubias <leo@leocov.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,16 +686,24 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: pyside6<7.0.0,>=6.5.0
+Requires-Dist: jinja2~=3.1.2
+Provides-Extra: dev
+Requires-Dist: black~=23.3.0; extra == "dev"
+Requires-Dist: pytest~=7.3.1; extra == "dev"
+Requires-Dist: pytest_mock~=3.10.0; extra == "dev"
+Requires-Dist: pre-commit~=3.3.1; extra == "dev"
+Requires-Dist: import-linter~=1.9.0; extra == "dev"
+Requires-Dist: bumpver~=2023.1121; extra == "dev"
 
 # pyside-app-core
 
 Custom style, widgets, and utilities for cross-platform PySide 6.5 applications with a focus on 'frameless' styling.
 
 > This project should be considered experimental and subject to breaking changes until a 1.0.0 release.
```

### Comparing `pyside-app-core-0.1.7/README.md` & `pyside_app_core-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/pyproject.toml` & `pyside_app_core-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyside-app-core"
-version = "0.1.7"
+version = "0.1.9"
 description = "Framework for PySide Applications"
 readme = "README.md"
 authors = [{ name = "Leo Covarrubias", email = "leo@leocov.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Development Status :: 2 - Pre-Alpha",
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3",
     "Typing :: Typed",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = ["pyside", "pyside6", "frameless", "app", "style"]
 dependencies = [
-    "pyside6 ~= 6.5.0",
+    "pyside6 >=6.5.0,<7.0.0",
     "jinja2 ~= 3.1.2",
 ]
 requires-python = ">=3.11"
 
 [project.optional-dependencies]
 dev = [
     "black ~= 23.3.0",
@@ -62,15 +62,15 @@
     "src.pyside_app_core",
 ]
 forbidden_modules = [
     "examples.simple_app",
 ]
 
 [tool.bumpver]
-current_version = "0.1.7"
+current_version = "0.1.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/constants.py` & `pyside_app_core-0.1.9/src/pyside_app_core/constants.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/errors/excepthook.py` & `pyside_app_core-0.1.9/src/pyside_app_core/errors/excepthook.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/errors/serial_errors.py` & `pyside_app_core-0.1.9/src/pyside_app_core/errors/serial_errors.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/__main__.py` & `pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/generate_resources.py` & `pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/generate_resources.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/console.svg` & `pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/console.svg`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/reload.svg` & `pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/reload.svg`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/save.svg` & `pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/save.svg`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/standard_resources.py` & `pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/standard_resources.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/templates/style.qss.jinja2` & `pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/templates/style.qss.jinja2`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -123,20 +123,20 @@
 }
 QPushButton:default {
     background: {{ theme.widget_accent_main_color.darker() }};
 }
 QPushButton:default:hover {
     background: {{ theme.widget_accent_main_color }};
 }
+
 /* ------------------------------------------------------------------------- */
 QToolBar {
     spacing: 8px;
 }
 
-
 /* ------------------------------------------------------------------------- */
 QToolButton {
     color: {{ theme.text_color }};
     border: 1px solid {{ theme.widget_border_color }};
     padding: 4px 3px 3px 4px;
     background: {{ theme.widget_accent_neutral_color }};
     border-radius: {{ theme.widget_corner_radius }};
```

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/log/__init__.py` & `pyside_app_core-0.1.9/src/pyside_app_core/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/log/logger.py` & `pyside_app_core-0.1.9/src/pyside_app_core/log/logger.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/style.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/style.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/util/s_color.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/util/s_color.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/util/style_sheet.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/util/style_sheet.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/about_dialog.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/about_dialog.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/base_app.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/base_app.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/error_dialog.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/error_dialog.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/base_dialog.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/base_dialog.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/base_window.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/base_window.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         self._window_actions.close_clicked.connect(self.close)
         self._window_actions.minimize_clicked.connect(self._on_minimize)
         self._window_actions.maximize_clicked.connect(self._on_maximize)
 
         self._window_shade = FramelessWindowShade(parent=self)
 
     @property
-    def window_bar_rect(self) -> QRect:
+    def window_bar_geo(self) -> QRect:
         return QRect(
             0, 0, self.rect().width(), self._window_actions.geometry().height()
         )
 
     def setWindowTitle(self, title: str):
         self._title.setText(title)
         super().setWindowTitle(title)
@@ -90,15 +90,15 @@
             super().setFixedSize(args[0], args[1])
             self._can_maximize = False
             return
 
         raise ValueError
 
     def paintEvent(self, event: QPaintEvent) -> None:
-        super().paintEvent(event)
+        event.accept()
 
         p = QPainter(self)
         p.setRenderHint(QPainter.RenderHint.Antialiasing)
 
         p.setPen(Qt.GlobalColor.transparent)
         p.setBrush(self._theme.background_color)
 
@@ -110,15 +110,14 @@
 
         # TODO: a bit crude - we want the border to be on top of everything, but no need to call
         #  every time - how to call after all subclasses have added edited widgets? unknown...
         self._window_shade.raise_()
         self._window_actions.raise_()
 
         p.end()
-        event.accept()
 
     def resizeEvent(self, event: QResizeEvent) -> None:
         self._title.setFixedWidth(self.rect().width())
         self._window_actions.resizeEvent(event)
         super().resizeEvent(event)
 
     def _draw_border(self, p: QPainter, rect: QRect):
@@ -190,7 +189,12 @@
         super().mousePressEvent(event)
 
     def mouseReleaseEvent(self, event: QMouseEvent) -> None:
         self._moving = False
         self.update()
 
         super().mouseReleaseEvent(event)
+
+    def mouseDoubleClickEvent(self, event: QMouseEvent) -> None:
+        self._on_maximize()
+
+        super().mouseReleaseEvent(event)
```

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/main_window.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
         self._about_dialog = AboutDialog()
 
         self._central = QWidget(parent=self)
         self._central.setStyleSheet("""background-color: none;""")
         self.setCentralWidget(self._central)
 
-        # must in order to show grab handle
+        # must call in order to show grab handle
         self.statusBar().show()
 
         self._menu_bar = MenuBarContext(
             self,
             border_width=0
             if platform_service.is_macos
             else self._theme.win_divider_width,
```

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/window_actions.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/window_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,25 +63,25 @@
         self._side_offset = (
             self.contentsMargins().left()
             if platform_service.is_macos
             else self.contentsMargins().right()
         )
 
         if platform_service.is_macos:
-            _width = 14
-            _height = 14
-            _spacing = 5
+            _width = 13
+            _height = 13
+            _spacing = 7
         elif platform_service.is_windows:
             _width = 45
             _height = 35
             _spacing = 3
         else:
-            _width = 20
-            _height = 20
-            _spacing = 10
+            _width = 17
+            _height = 17
+            _spacing = 8
 
         self._a_rect = QRect(self._side_offset, _top_offset, _width, _height)
         self._b_rect = self._a_rect.translated(_width + _spacing, 0)
         self._c_rect = self._b_rect.translated(_width + _spacing, 0)
 
         if platform_service.is_macos:
             self.container_height = (
@@ -143,19 +143,21 @@
         _order = [2, 0, 1] if platform_service.is_macos else [0, 1, 2]
 
         self._rect_map = []
         for i, o in enumerate(_order):
             self._rect_map.append((_rect_list[i], _button_data[o]))
 
     def paintEvent(self, event: QPaintEvent) -> None:
+        event.accept()
+
         p = QPainter(self)
         p.setRenderHint(QPainter.RenderHint.Antialiasing)
 
-        p.setPen(Qt.GlobalColor.transparent)
-        p.setBrush(Qt.GlobalColor.transparent)
+        # p.setPen(Qt.GlobalColor.transparent)
+        # p.setBrush(Qt.GlobalColor.transparent)
 
         for rect, data in self._rect_map:
             enabled = self.isActiveWindow() and data.enabled_fn()
 
             self._draw_button(p, rect, data.color, data.action, enabled)
 
             if platform_service.is_macos and not enabled:
@@ -163,16 +165,14 @@
             else:
                 c_shape = data.color if enabled else data.color.darker(300)
                 c_shape = c_shape.darker(200) if platform_service.is_macos else c_shape
                 data.shape_fn(p, rect, c_shape, data.action)
 
         p.end()
 
-        event.accept()
-
     def mouseMoveEvent(self, event: QMouseEvent) -> None:
         prev = self._hover
         for rect, data in self._rect_map:
             if not data.enabled_fn():
                 continue
 
             if rect.contains(event.pos()):
```

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/window_shade.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/window_shade.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     def setDisabled(self, val: bool) -> None:
         self._disabled = val
 
     def setEnabled(self, val: bool) -> None:
         self.setDisabled(not val)
 
     def paintEvent(self, event: QPaintEvent) -> None:
+        event.accept()
+
         rect = self.parent().contentsRect()
         self.setFixedSize(rect.size())
 
         p = QPainter(self)
         p.setRenderHint(QPainter.RenderHint.Antialiasing)
         p.setPen(QPen(Qt.GlobalColor.transparent))
         p.setBrush(QBrush(Qt.GlobalColor.transparent))
```

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/menu_ctx.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/menu_ctx.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/multi_combo_box.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/multi_combo_box.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/object_name_mixin.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/object_name_mixin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/settings_mixin.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/settings_mixin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/tool_bar_ctx.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/tool_bar_ctx.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,31 +21,27 @@
 
 class ToolBarContext(ObjectNameMixin, QToolBar):
     def __init__(self, area: ToolBarArea, parent: QMainWindow, movable=False):
         self._area = area
         self._theme = application_service.get_app_theme()
         self._actions: List[QAction] = []
 
-        _margins = [0, 0, 0, 0]
-
         if area == "left":
             self._border_side = "right"
         elif area == "right":
             self._border_side = "left"
         elif area == "top":
             self._border_side = "bottom"
-            _margins[1] = 5
         else:
             self._border_side = "top"
-            _margins[3] = 5
 
         self.OBJECT_NAME = f"ToolBar_{area}"
         super(ToolBarContext, self).__init__(self.OBJECT_NAME, parent=parent)
 
-        self.setContentsMargins(*_margins)
+        self.setContentsMargins(0, 0, 0, 0)
         self.setGeometry(10, 10, self.width(), self.height())
         self.setMovable(movable)
         self.setIconSize(QSize(28, 28))
 
         parent.addToolBar(_TOOL_BAR_AREA_MAP[self._area], self)
 
         self._setup_style()
@@ -57,19 +53,28 @@
         action = QAction(text=name, parent=self)
         action.setObjectName(f"ToolBarAction_{name}")
         if icon:
             action.setIcon(icon)
 
         self._actions.append(action)
         if len(self._actions) == 1:
-            tool_button = [c for c in self.children() if isinstance(c, QToolButton)][0]
+            _ = [c for c in self.children() if isinstance(c, QToolButton)][0]
         yield action
         self.addAction(action)
 
     def _setup_style(self):
         self.setStyleSheet(
             f"""
-#{self.obj_name} {{
+QToolBar#{self.obj_name} {{
     border-{self._border_side}: {self._theme.win_divider_width} solid {self._theme.win_divider_color};
 }}
+QToolBar#{self.obj_name} > QToolButton {{
+    margin-left: 0px;
+    margin-top: 10px;
+    margin-bottom: 10px;
+    spacing: 0;
+}}
+QToolButton:first {{
+    background-color: red;
+}}
 """
         )
```

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/tool_button.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/tool_button.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/tool_stack.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/tool_stack.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/window_settings_mixin.py` & `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/window_settings_mixin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/services/application_service.py` & `pyside_app_core-0.1.9/src/pyside_app_core/services/application_service.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/serial_service.py` & `pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/serial_service.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py` & `pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Protocol, Self, TypeVar
 
 T = TypeVar("T")
 
 
-class CommandInterface(Protocol[T]):
+class CommandInterface(Protocol):
     def encode(self) -> bytearray:
         ...
 
     @classmethod
-    def decode(cls, raw_data: bytes) -> Self:
+    def decode(cls, raw_data: bytes):
         ...
 
 
-class TranscoderInterface(Protocol[T]):
+class TranscoderInterface(Protocol):
     @classmethod
     def encode_data(cls, command: CommandInterface) -> bytearray:
         pass
 
     @classmethod
     def decode_data(cls, data: bytearray) -> CommandInterface:
         pass
```

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/conversion_utils.py` & `pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/float_map.py` & `pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/float_map.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core.egg-info/PKG-INFO` & `pyside_app_core-0.1.9/src/pyside_app_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyside-app-core
-Version: 0.1.7
+Version: 0.1.9
 Summary: Framework for PySide Applications
 Author-email: Leo Covarrubias <leo@leocov.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,16 +686,24 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: pyside6<7.0.0,>=6.5.0
+Requires-Dist: jinja2~=3.1.2
+Provides-Extra: dev
+Requires-Dist: black~=23.3.0; extra == "dev"
+Requires-Dist: pytest~=7.3.1; extra == "dev"
+Requires-Dist: pytest_mock~=3.10.0; extra == "dev"
+Requires-Dist: pre-commit~=3.3.1; extra == "dev"
+Requires-Dist: import-linter~=1.9.0; extra == "dev"
+Requires-Dist: bumpver~=2023.1121; extra == "dev"
 
 # pyside-app-core
 
 Custom style, widgets, and utilities for cross-platform PySide 6.5 applications with a focus on 'frameless' styling.
 
 > This project should be considered experimental and subject to breaking changes until a 1.0.0 release.
```

### Comparing `pyside-app-core-0.1.7/src/pyside_app_core.egg-info/SOURCES.txt` & `pyside_app_core-0.1.9/src/pyside_app_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

