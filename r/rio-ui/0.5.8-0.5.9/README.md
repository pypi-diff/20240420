# Comparing `tmp/rio_ui-0.5.8.tar.gz` & `tmp/rio_ui-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio_ui-0.5.8.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `rio_ui-0.5.8.tar` & `rio_ui-0.5.9.tar`

### file list

```diff
@@ -1,216 +1,343 @@
--rw-r--r--   0        0        0    35149 2024-04-06 18:09:28.058340 rio_ui-0.5.8/LICENSE.txt
--rw-r--r--   0        0        0     7536 2024-04-15 19:47:20.290142 rio_ui-0.5.8/README.md
--rw-r--r--   0        0        0     2441 2024-04-16 20:42:01.961956 rio_ui-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      731 2024-04-16 20:40:48.375159 rio_ui-0.5.8/rio/__init__.py
--rw-r--r--   0        0        0       91 2024-04-06 18:09:28.078340 rio_ui-0.5.8/rio/__main__.py
--rw-r--r--   0        0        0    19313 2024-04-09 19:38:54.555684 rio_ui-0.5.8/rio/app.py
--rw-r--r--   0        0        0    32193 2024-04-16 20:40:48.375159 rio_ui-0.5.8/rio/app_server.py
--rw-r--r--   0        0        0      233 2024-04-06 18:09:28.081673 rio_ui-0.5.8/rio/assets/hosted/README.md
--rw-r--r--   0        0        0   557380 2024-04-06 18:09:28.088340 rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf
--rw-r--r--   0        0        0   401608 2024-04-06 18:09:28.091673 rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf
--rw-r--r--   0        0        0   403724 2024-04-06 18:09:28.095007 rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf
--rw-r--r--   0        0        0   556216 2024-04-06 18:09:28.098340 rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf
--rw-r--r--   0        0        0     4449 2024-04-06 18:09:28.098340 rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/OFL.txt
--rw-r--r--   0        0        0    11560 2024-04-06 18:09:28.101673 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   167336 2024-04-06 18:09:28.101673 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2024-04-06 18:09:28.105007 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2024-04-06 18:09:28.105007 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   168260 2024-04-06 18:09:28.105007 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0    11560 2024-04-06 18:09:28.098340 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt
--rw-r--r--   0        0        0    87392 2024-04-06 18:09:28.098340 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf
--rw-r--r--   0        0        0    94636 2024-04-06 18:09:28.101673 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
--rw-r--r--   0        0        0    94372 2024-04-06 18:09:28.101673 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf
--rw-r--r--   0        0        0    87236 2024-04-06 18:09:28.101673 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf
--rw-r--r--   0        0        0    54189 2024-04-08 17:00:05.405088 rio_ui-0.5.8/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
--rw-r--r--   0        0        0    31665 2024-04-06 18:09:28.105007 rio_ui-0.5.8/rio/assets/hosted/rio-logos/rio-logo-square.png
--rw-r--r--   0        0        0  1081400 2024-04-07 20:27:02.369218 rio_ui-0.5.8/rio/assets/icon-sets/material.tar.xz
--rw-r--r--   0        0        0    14992 2024-04-14 09:27:29.097282 rio_ui-0.5.8/rio/assets/icon-sets/rio.tar.xz
--rw-r--r--   0        0        0     1096 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/assets/icon-sets/styling.tar.xz
--rw-r--r--   0        0        0     8798 2024-04-12 12:19:28.613327 rio_ui-0.5.8/rio/assets.py
--rw-r--r--   0        0        0     3316 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/byte_serving.py
--rw-r--r--   0        0        0     7445 2024-04-16 20:40:48.375159 rio_ui-0.5.8/rio/cli/__init__.py
--rw-r--r--   0        0        0     2392 2024-04-08 18:37:44.152450 rio_ui-0.5.8/rio/cli/cli_instance.py
--rw-r--r--   0        0        0     6642 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/cli/nice_traceback.py
--rw-r--r--   0        0        0    13832 2024-04-12 10:18:09.239288 rio_ui-0.5.8/rio/cli/project.py
--rw-r--r--   0        0        0    12661 2024-04-15 19:46:56.423852 rio_ui-0.5.8/rio/cli/project_setup.py
--rw-r--r--   0        0        0     4172 2024-04-08 18:37:44.152450 rio_ui-0.5.8/rio/cli/rio_api.py
--rw-r--r--   0        0        0     2278 2024-04-08 18:37:44.152450 rio_ui-0.5.8/rio/cli/rioignore.py
--rw-r--r--   0        0        0       40 2024-04-14 14:22:40.220263 rio_ui-0.5.8/rio/cli/run_project/__init__.py
--rw-r--r--   0        0        0     5404 2024-04-08 16:50:31.798904 rio_ui-0.5.8/rio/cli/run_project/app_loading.py
--rw-r--r--   0        0        0    22196 2024-04-16 20:40:48.375159 rio_ui-0.5.8/rio/cli/run_project/arbiter.py
--rw-r--r--   0        0        0     1656 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/cli/run_project/file_watcher_worker.py
--rw-r--r--   0        0        0      423 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/cli/run_project/run_models.py
--rw-r--r--   0        0        0      476 2024-04-08 18:37:44.152450 rio_ui-0.5.8/rio/cli/run_project/run_utils.py
--rw-r--r--   0        0        0     4097 2024-04-16 20:40:48.375159 rio_ui-0.5.8/rio/cli/run_project/uvicorn_worker.py
--rw-r--r--   0        0        0     2229 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/cli/run_project/webview_worker.py
--rw-r--r--   0        0        0     3982 2024-04-08 18:37:44.152450 rio_ui-0.5.8/rio/cli/tomlconfig.py
--rw-r--r--   0        0        0    19604 2024-04-09 19:38:54.559018 rio_ui-0.5.8/rio/color.py
--rw-r--r--   0        0        0     9824 2024-04-16 20:40:48.378492 rio_ui-0.5.8/rio/common.py
--rw-r--r--   0        0        0     1552 2024-04-10 18:34:30.899371 rio_ui-0.5.8/rio/components/__init__.py
--rw-r--r--   0        0        0     4469 2024-04-12 12:17:57.040111 rio_ui-0.5.8/rio/components/app_root.py
--rw-r--r--   0        0        0     4055 2024-04-08 18:37:44.152450 rio_ui-0.5.8/rio/components/auto_form.py
--rw-r--r--   0        0        0     4751 2024-04-09 19:38:54.559018 rio_ui-0.5.8/rio/components/banner.py
--rw-r--r--   0        0        0      889 2024-04-07 08:57:25.524848 rio_ui-0.5.8/rio/components/build_failed.py
--rw-r--r--   0        0        0    13570 2024-04-12 20:47:24.392283 rio_ui-0.5.8/rio/components/button.py
--rw-r--r--   0        0        0     5064 2024-04-09 19:38:54.559018 rio_ui-0.5.8/rio/components/card.py
--rw-r--r--   0        0        0     1025 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/components/class_container.py
--rw-r--r--   0        0        0      352 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/components/code_explorer.py
--rw-r--r--   0        0        0     3745 2024-04-09 19:38:54.559018 rio_ui-0.5.8/rio/components/color_picker.py
--rw-r--r--   0        0        0    26039 2024-04-12 12:19:28.613327 rio_ui-0.5.8/rio/components/component.py
--rw-r--r--   0        0        0     1029 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/components/component_tree.py
--rw-r--r--   0        0        0     1225 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/container.py
--rw-r--r--   0        0        0      215 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/components/debugger_connector.py
--rw-r--r--   0        0        0     4067 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/components/devel_component.py
--rw-r--r--   0        0        0     3889 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/drawer.py
--rw-r--r--   0        0        0     6670 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/dropdown.py
--rw-r--r--   0        0        0     2922 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/flow_container.py
--rw-r--r--   0        0        0     5867 2024-04-10 17:00:38.844482 rio_ui-0.5.8/rio/components/fundamental_component.py
--rw-r--r--   0        0        0     7057 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/grid.py
--rw-r--r--   0        0        0      604 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/html.py
--rw-r--r--   0        0        0     7782 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/icon.py
--rw-r--r--   0        0        0     3676 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/image.py
--rw-r--r--   0        0        0    13127 2024-04-09 19:38:54.565684 rio_ui-0.5.8/rio/components/key_event_listener.py
--rw-r--r--   0        0        0     2981 2024-04-12 12:17:57.116777 rio_ui-0.5.8/rio/components/labeled_column.py
--rw-r--r--   0        0        0     8968 2024-04-09 19:38:54.585684 rio_ui-0.5.8/rio/components/linear_containers.py
--rw-r--r--   0        0        0     4478 2024-04-09 19:38:54.565684 rio_ui-0.5.8/rio/components/link.py
--rw-r--r--   0        0        0    10184 2024-04-12 12:17:57.146777 rio_ui-0.5.8/rio/components/list_items.py
--rw-r--r--   0        0        0     3527 2024-04-09 19:38:54.565684 rio_ui-0.5.8/rio/components/list_view.py
--rw-r--r--   0        0        0     1389 2024-04-09 19:38:54.565684 rio_ui-0.5.8/rio/components/markdown.py
--rw-r--r--   0        0        0     4917 2024-04-09 19:38:54.565684 rio_ui-0.5.8/rio/components/media_player.py
--rw-r--r--   0        0        0     6919 2024-04-09 19:38:54.565684 rio_ui-0.5.8/rio/components/mouse_event_listener.py
--rw-r--r--   0        0        0     5165 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/multi_line_text_input.py
--rw-r--r--   0        0        0     1422 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/node_input.py
--rw-r--r--   0        0        0     1426 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/node_output.py
--rw-r--r--   0        0        0     8478 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/number_input.py
--rw-r--r--   0        0        0     2190 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/overlay.py
--rw-r--r--   0        0        0     5116 2024-04-16 20:40:48.378492 rio_ui-0.5.8/rio/components/page_view.py
--rw-r--r--   0        0        0     4959 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/plot.py
--rw-r--r--   0        0        0     3280 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/popup.py
--rw-r--r--   0        0        0      975 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/progress_bar.py
--rw-r--r--   0        0        0     3560 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/progress_circle.py
--rw-r--r--   0        0        0     4106 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/rectangle.py
--rw-r--r--   0        0        0     3688 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/revealer.py
--rw-r--r--   0        0        0     1914 2024-04-16 20:40:48.378492 rio_ui-0.5.8/rio/components/root_components.py
--rw-r--r--   0        0        0     1889 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/scroll_container.py
--rw-r--r--   0        0        0     1213 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/scroll_target.py
--rw-r--r--   0        0        0     1114 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/separator.py
--rw-r--r--   0        0        0     6120 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/slider.py
--rw-r--r--   0        0        0     3649 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/slideshow.py
--rw-r--r--   0        0        0     1442 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/spacer.py
--rw-r--r--   0        0        0     2762 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/stack.py
--rw-r--r--   0        0        0     3154 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/switch.py
--rw-r--r--   0        0        0      879 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/switcher.py
--rw-r--r--   0        0        0     9237 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/switcher_bar.py
--rw-r--r--   0        0        0     2305 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/table.py
--rw-r--r--   0        0        0     2018 2024-04-09 19:38:54.575684 rio_ui-0.5.8/rio/components/text.py
--rw-r--r--   0        0        0     5380 2024-04-09 19:38:54.575684 rio_ui-0.5.8/rio/components/text_input.py
--rw-r--r--   0        0        0     1231 2024-04-09 19:38:54.575684 rio_ui-0.5.8/rio/components/theme_context_switcher.py
--rw-r--r--   0        0        0     2861 2024-04-09 19:38:54.575684 rio_ui-0.5.8/rio/components/tooltip.py
--rw-r--r--   0        0        0      633 2024-04-09 19:38:54.575684 rio_ui-0.5.8/rio/components/website.py
--rw-r--r--   0        0        0      123 2024-04-08 18:37:44.152450 rio_ui-0.5.8/rio/cursor_style.py
--rw-r--r--   0        0        0     5753 2024-04-15 19:47:20.290142 rio_ui-0.5.8/rio/dataclass.py
--rw-r--r--   0        0        0       53 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/debug/__init__.py
--rw-r--r--   0        0        0       63 2024-04-14 14:22:40.220263 rio_ui-0.5.8/rio/debug/client_side_debugger/__init__.py
--rw-r--r--   0        0        0    10723 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/debug/client_side_debugger/component_details.py
--rw-r--r--   0        0        0     3589 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/debug/client_side_debugger/debugger.py
--rw-r--r--   0        0        0      795 2024-04-12 12:17:57.210110 rio_ui-0.5.8/rio/debug/client_side_debugger/deploy_page.py
--rw-r--r--   0        0        0      782 2024-04-12 12:17:57.210110 rio_ui-0.5.8/rio/debug/client_side_debugger/docs_page.py
--rw-r--r--   0        0        0    12359 2024-04-12 12:17:57.423443 rio_ui-0.5.8/rio/debug/client_side_debugger/icons_page.py
--rw-r--r--   0        0        0     1055 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/debug/client_side_debugger/layout_preview.py
--rw-r--r--   0        0        0     2379 2024-04-12 12:17:57.236777 rio_ui-0.5.8/rio/debug/client_side_debugger/project_page.py
--rw-r--r--   0        0        0     2265 2024-04-08 18:37:44.155783 rio_ui-0.5.8/rio/debug/client_side_debugger/sample_icons_grid.py
--rw-r--r--   0        0        0    16597 2024-04-12 12:17:57.400110 rio_ui-0.5.8/rio/debug/client_side_debugger/theme_picker_page.py
--rw-r--r--   0        0        0     1089 2024-04-10 18:34:30.899371 rio_ui-0.5.8/rio/debug/client_side_debugger/tree_page.py
--rw-r--r--   0        0        0     7224 2024-04-08 18:37:44.155783 rio_ui-0.5.8/rio/debug/monkeypatches.py
--rw-r--r--   0        0        0      567 2024-04-08 18:37:44.155783 rio_ui-0.5.8/rio/debug/typing_utils.py
--rw-r--r--   0        0        0    14210 2024-04-12 12:19:28.613327 rio_ui-0.5.8/rio/debug/validator.py
--rw-r--r--   0        0        0       31 2024-04-16 20:40:48.378492 rio_ui-0.5.8/rio/docs/__init__.py
--rw-r--r--   0        0        0     4884 2024-04-16 20:40:48.378492 rio_ui-0.5.8/rio/docs/custom.py
--rw-r--r--   0        0        0      960 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/errors.py
--rw-r--r--   0        0        0     3173 2024-04-08 18:37:44.155783 rio_ui-0.5.8/rio/event.py
--rw-r--r--   0        0        0     6732 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/fills.py
--rw-r--r--   0        0        0   529611 2024-04-16 20:44:03.208838 rio_ui-0.5.8/rio/generated/index.html
--rw-r--r--   0        0        0      897 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/global_state.py
--rw-r--r--   0        0        0     9940 2024-04-07 11:32:34.208243 rio_ui-0.5.8/rio/icon_registry.py
--rw-r--r--   0        0        0     3500 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/inspection.py
--rw-r--r--   0        0        0     3625 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/maybes.py
--rw-r--r--   0        0        0     1577 2024-04-12 20:47:24.392283 rio_ui-0.5.8/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
--rw-r--r--   0        0        0     1531 2024-04-12 20:47:24.392283 rio_ui-0.5.8/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
--rw-r--r--   0        0        0      757 2024-04-15 19:47:20.290142 rio_ui-0.5.8/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
--rw-r--r--   0        0        0      374 2024-04-15 19:47:20.290142 rio_ui-0.5.8/rio/patches_for_3rd_party_stuff/__init__.py
--rw-r--r--   0        0        0     7380 2024-04-09 19:38:54.575684 rio_ui-0.5.8/rio/routing.py
--rw-r--r--   0        0        0      417 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/self_serializing.py
--rw-r--r--   0        0        0     8463 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/serialization.py
--rw-r--r--   0        0        0    75851 2024-04-16 20:40:48.378492 rio_ui-0.5.8/rio/session.py
--rw-r--r--   0        0        0     1395 2024-04-06 18:09:28.115007 rio_ui-0.5.8/rio/snippets/README.md
--rw-r--r--   0        0        0    12479 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/snippets/__init__.py
--rw-r--r--   0        0        0     1318 2024-04-09 16:47:56.822558 rio_ui-0.5.8/rio/snippets/snippet-files/other-examples/simple_counter_app.py
--rw-r--r--   0        0        0      684 2024-04-06 18:08:52.814883 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
--rw-r--r--   0        0        0      326 2024-04-14 14:22:40.220263 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
--rw-r--r--   0        0        0     1829 2024-04-13 20:00:32.294184 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
--rw-r--r--   0        0        0     1196 2024-04-08 18:37:44.155783 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
--rw-r--r--   0        0        0     3728 2024-04-08 18:37:44.155783 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
--rw-r--r--   0        0        0      517 2024-04-08 18:37:44.159116 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
--rw-r--r--   0        0        0     2227 2024-04-07 09:24:53.378316 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
--rw-r--r--   0        0        0      184 2024-04-07 18:38:03.958535 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
--rw-r--r--   0        0        0       44 2024-04-14 14:22:40.220263 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
--rw-r--r--   0        0        0     5823 2024-04-10 17:01:52.457775 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
--rw-r--r--   0        0        0      863 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
--rw-r--r--   0        0        0     3344 2024-04-06 18:08:52.814883 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
--rw-r--r--   0        0        0        0 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
--rw-r--r--   0        0        0     7595 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
--rw-r--r--   0        0        0      156 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
--rw-r--r--   0        0        0     6866 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
--rw-r--r--   0        0        0     4602 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
--rw-r--r--   0        0        0     3359 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
--rw-r--r--   0        0        0      628 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
--rw-r--r--   0        0        0      226 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
--rw-r--r--   0        0        0       59 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
--rw-r--r--   0        0        0     6789 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
--rw-r--r--   0        0        0        0 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
--rw-r--r--   0        0        0     3586 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
--rw-r--r--   0        0        0        0 2024-04-06 18:09:28.115007 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Empty/README.md
--rw-r--r--   0        0        0       98 2024-04-07 08:04:03.043617 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Empty/meta.json
--rw-r--r--   0        0        0        0 2024-04-06 18:09:28.115007 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
--rw-r--r--   0        0        0      504 2024-04-12 10:18:09.242621 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
--rw-r--r--   0        0        0        0 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Empty/root_init.py
--rw-r--r--   0        0        0     3344 2024-04-06 18:09:28.115007 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
--rw-r--r--   0        0        0      714 2024-04-12 10:18:09.225955 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
--rw-r--r--   0        0        0       94 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
--rw-r--r--   0        0        0     4821 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
--rw-r--r--   0        0        0     4139 2024-04-12 10:18:09.225955 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
--rw-r--r--   0        0        0     1685 2024-04-12 10:18:09.225955 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
--rw-r--r--   0        0        0       55 2024-04-10 18:59:11.048460 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
--rw-r--r--   0        0        0       44 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
--rw-r--r--   0        0        0     6969 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
--rw-r--r--   0        0        0        0 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
--rw-r--r--   0        0        0     3586 2024-04-10 16:49:08.284483 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
--rw-r--r--   0        0        0      490 2024-04-08 13:25:22.132597 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
--rw-r--r--   0        0        0       34 2024-04-12 12:20:05.616618 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
--rw-r--r--   0        0        0     2049 2024-04-12 12:19:28.609994 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
--rw-r--r--   0        0        0       92 2024-04-08 13:26:20.426025 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
--rw-r--r--   0        0        0       61 2024-04-14 14:22:40.220263 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
--rw-r--r--   0        0        0     4659 2024-04-12 12:19:28.593327 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0        0 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
--rw-r--r--   0        0        0     3344 2024-04-08 13:24:10.679136 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
--rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
--rw-r--r--   0        0        0      806 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
--rw-r--r--   0        0        0     1070 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
--rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
--rw-r--r--   0        0        0      875 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
--rw-r--r--   0        0        0     1070 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
--rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
--rw-r--r--   0        0        0     2216 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
--rw-r--r--   0        0        0     1256 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
--rw-r--r--   0        0        0        0 2024-04-12 20:47:24.412283 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
--rw-r--r--   0        0        0     4328 2024-04-12 20:47:24.412283 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0     8134 2024-04-08 18:37:44.159116 rio_ui-0.5.8/rio/state_properties.py
--rw-r--r--   0        0        0     3077 2024-04-06 18:09:28.115007 rio_ui-0.5.8/rio/text_style.py
--rw-r--r--   0        0        0    19432 2024-04-09 19:38:54.575684 rio_ui-0.5.8/rio/theme.py
--rw-r--r--   0        0        0     5167 2024-04-06 18:09:28.115007 rio_ui-0.5.8/rio/user_settings_module.py
--rw-r--r--   0        0        0     3890 2024-04-06 18:09:28.115007 rio_ui-0.5.8/rio/world_units.py
--rw-r--r--   0        0        0    10093 1970-01-01 00:00:00.000000 rio_ui-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 rio_ui-0.5.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rio_ui-0.5.9/.prettierrc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 rio_ui-0.5.9/.python-version
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 rio_ui-0.5.9/.sassrc
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 rio_ui-0.5.9/README-DEV.md
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 rio_ui-0.5.9/__init__.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 rio_ui-0.5.9/package.json
+-rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 rio_ui-0.5.9/requirements-dev.lock
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 rio_ui-0.5.9/requirements.lock
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 rio_ui-0.5.9/vite.config.js
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/index.html
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/app.ts
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/colorConversion.ts
+-rw-r--r--   0        0        0    20430 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/componentManagement.ts
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/cssUtils.ts
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/dataModels.ts
+-rw-r--r--   0        0        0     7224 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/designApplication.ts
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/easeFunctions.ts
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/eventHandling.ts
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/inputBoxTools.ts
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/layoutHelpers.ts
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/layouting.ts
+-rw-r--r--   0        0        0    11599 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/rpc.ts
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/rpcFunctions.ts
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/utils.ts
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/align.ts
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/buildFailed.ts
+-rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/button.ts
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/card.ts
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/classContainer.ts
+-rw-r--r--   0        0        0    14169 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/codeExplorer.ts
+-rw-r--r--   0        0        0    13816 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/colorPicker.ts
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/componentBase.ts
+-rw-r--r--   0        0        0    14330 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/componentTree.ts
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/customListItem.ts
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/debuggerConnector.ts
+-rw-r--r--   0        0        0    11396 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/drawer.ts
+-rw-r--r--   0        0        0    16995 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/dropdown.ts
+-rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/flowContainer.ts
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/fundamentalRootComponent.ts
+-rw-r--r--   0        0        0    11000 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/grid.ts
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/headingListItem.ts
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/html.ts
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/icon.ts
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/image.ts
+-rw-r--r--   0        0        0    19835 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/keyEventListener.ts
+-rw-r--r--   0        0        0    13880 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/linearContainers.ts
+-rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/link.ts
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/listView.ts
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/margin.ts
+-rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/markdown.ts
+-rw-r--r--   0        0        0    27578 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/mediaPlayer.ts
+-rw-r--r--   0        0        0     5944 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/mouseEventListener.ts
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/multiLineTextInput.ts
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/nodeInput.ts
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/nodeOutput.ts
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/overlay.ts
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/placeholder.ts
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/plot.ts
+-rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/popup.ts
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/progressBar.ts
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/progressCircle.ts
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/rectangle.ts
+-rw-r--r--   0        0        0    10551 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/revealer.ts
+-rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/scrollContainer.ts
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/scrollTarget.ts
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/separator.ts
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/separatorListItem.ts
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/singleContainer.ts
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/slider.ts
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/slideshow.ts
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/stack.ts
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/switch.ts
+-rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/switcher.ts
+-rw-r--r--   0        0        0    20315 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/switcherBar.ts
+-rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/table.ts
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/text.ts
+-rw-r--r--   0        0        0     7379 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/textInput.ts
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/themeContextSwitcher.ts
+-rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/tooltip.ts
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/code/components/website.ts
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/css/fonts.scss
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/css/highlightjs-default-dark.css
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/css/highlightjs-default-light.css
+-rw-r--r--   0        0        0    63395 2020-02-02 00:00:00.000000 rio_ui-0.5.9/frontend/css/style.scss
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 rio_ui-0.5.9/prototyping/icon_search.py
+-rw-r--r--   0        0        0     7315 2020-02-02 00:00:00.000000 rio_ui-0.5.9/prototyping/pack.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 rio_ui-0.5.9/prototyping/webgl.html
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 rio_ui-0.5.9/prototyping/node_editor/__main__.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 rio_ui-0.5.9/prototyping/node_editor/index.html
+-rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 rio_ui-0.5.9/prototyping/node_editor/script.ts
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 rio_ui-0.5.9/prototyping/node_editor/styles.scss
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/custom-material-icons/twinkle.svg
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/custom-material-icons/fill/twinkle.svg
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/logo.svg
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/color/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/color/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/color/logo.svg
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/fill/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/fill/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/rio/fill/logo.svg
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/styling/corner-round-bottom-left.svg
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/styling/corner-round-bottom-right.svg
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/styling/corner-round-top-left.svg
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 rio_ui-0.5.9/raw-icons/styling/corner-round-top-right.svg
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rio_ui-0.5.9/scripts/benchmark.py
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 rio_ui-0.5.9/scripts/build_material_icon_set.py
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 rio_ui-0.5.9/scripts/check_docs.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rio_ui-0.5.9/scripts/cloc.sh
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rio_ui-0.5.9/scripts/code_coverage.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 rio_ui-0.5.9/scripts/publish_new_release.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/__main__.py
+-rw-r--r--   0        0        0    18767 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/app.py
+-rw-r--r--   0        0        0    32239 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/app_server.py
+-rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/byte_serving.py
+-rw-r--r--   0        0        0    19606 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/color.py
+-rw-r--r--   0        0        0     9924 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/common.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cursor_style.py
+-rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/dataclass.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/errors.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/event.py
+-rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/fills.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/global_state.py
+-rw-r--r--   0        0        0     9799 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/icon_registry.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/inspection.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/maybes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/py.typed
+-rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/routing.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/self_serializing.py
+-rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/serialization.py
+-rw-r--r--   0        0        0    76883 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/session.py
+-rw-r--r--   0        0        0     8134 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/state_properties.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/text_style.py
+-rw-r--r--   0        0        0    19432 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/theme.py
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/user_settings_module.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/world_units.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/README.md
+-rw-r--r--   0        0        0   557380 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf
+-rw-r--r--   0        0        0   401608 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf
+-rw-r--r--   0        0        0   403724 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf
+-rw-r--r--   0        0        0   556216 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/OFL.txt
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt
+-rw-r--r--   0        0        0    87392 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf
+-rw-r--r--   0        0        0    94636 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
+-rw-r--r--   0        0        0    94372 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf
+-rw-r--r--   0        0        0    87236 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf
+-rw-r--r--   0        0        0    54189 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
+-rw-r--r--   0        0        0    31665 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/hosted/rio-logos/rio-logo-square.png
+-rw-r--r--   0        0        0  1081336 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/icon-sets/material.tar.xz
+-rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/icon-sets/rio.tar.xz
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/assets/icon-sets/styling.tar.xz
+-rw-r--r--   0        0        0     7445 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/__init__.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/cli_instance.py
+-rw-r--r--   0        0        0     6642 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/nice_traceback.py
+-rw-r--r--   0        0        0    13832 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/project.py
+-rw-r--r--   0        0        0    12831 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/project_setup.py
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/rio_api.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/rioignore.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/tomlconfig.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/__init__.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/app_loading.py
+-rw-r--r--   0        0        0    22196 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/arbiter.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/file_watcher_worker.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/run_models.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/run_utils.py
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/uvicorn_worker.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/cli/run_project/webview_worker.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/__init__.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/app_root.py
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/auto_form.py
+-rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/banner.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/build_failed.py
+-rw-r--r--   0        0        0    13594 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/button.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/card.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/class_container.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/code_explorer.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/color_picker.py
+-rw-r--r--   0        0        0    26038 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/component.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/component_tree.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/container.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/debugger_connector.py
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/devel_component.py
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/drawer.py
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/dropdown.py
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/flow_container.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/fundamental_component.py
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/grid.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/html.py
+-rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/icon.py
+-rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/image.py
+-rw-r--r--   0        0        0    13129 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/key_event_listener.py
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/labeled_column.py
+-rw-r--r--   0        0        0     8964 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/linear_containers.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/link.py
+-rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/list_items.py
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/list_view.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/markdown.py
+-rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/media_player.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/mouse_event_listener.py
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/multi_line_text_input.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/node_input.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/node_output.py
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/number_input.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/overlay.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/page_view.py
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/plot.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/popup.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/progress_bar.py
+-rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/progress_circle.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/rectangle.py
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/revealer.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/root_components.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/scroll_container.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/scroll_target.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/separator.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/slider.py
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/slideshow.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/spacer.py
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/stack.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/switch.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/switcher.py
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/switcher_bar.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/table.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/text.py
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/text_input.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/theme_context_switcher.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/tooltip.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/components/website.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/__init__.py
+-rw-r--r--   0        0        0     7224 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/monkeypatches.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/typing_utils.py
+-rw-r--r--   0        0        0    14210 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/validator.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/__init__.py
+-rw-r--r--   0        0        0    10733 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/component_details.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/debugger.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/deploy_page.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/docs_page.py
+-rw-r--r--   0        0        0    12359 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/icons_page.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/layout_preview.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/project_page.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/sample_icons_grid.py
+-rw-r--r--   0        0        0    16597 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/theme_picker_page.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/debug/client_side_debugger/tree_page.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/docs/__init__.py
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/docs/custom.py
+-rw-r--r--   0        0        0   942785 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/generated/index.html
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/patches_for_3rd_party_stuff/__init__.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/README.md
+-rw-r--r--   0        0        0    12479 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/__init__.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/other-examples/simple_counter_app.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
+-rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
+-rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
+-rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Empty/README.md
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Empty/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Empty/root_init.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
+-rw-r--r--   0        0        0     6971 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_app_build.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_custom_components.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_docstring_code_blocks.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_events.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_project_templates.py
+-rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_reconciliation.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_refresh.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_session.py
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_state_bindings.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_user_settings.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/test_zzz_guardrails.py
+-rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 rio_ui-0.5.9/tests/utils.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 rio_ui-0.5.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 rio_ui-0.5.9/LICENSE.txt
+-rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 rio_ui-0.5.9/README.md
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 rio_ui-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     9725 2020-02-02 00:00:00.000000 rio_ui-0.5.9/PKG-INFO
```

### Comparing `rio_ui-0.5.8/LICENSE.txt` & `rio_ui-0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/README.md` & `rio_ui-0.5.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 Rio brings React-style components to Python. Pull from a wealth of built-in
 components and combine them to create your own custom components. Then combine
 those into entire apps. Best of all, Rio apps can run both locally on your
 machine and on the web.
 
 ## Features 🧩
 
-- Modern, **declarative UI** framework
-- **100% Python** - Zero HTML, CSS, or JavaScript required
-- Over **50 Built-in components** for common UI elements, such as `rio.Switch`, `rio.Button`, and `rio.Text`, and many more
-- Integrates with **modern Python tooling**: Thanks to being **entirely Type Safe** editors can give you instant suggestions and highlight problems right away
-- Apps can run **both locally and on the web**
-- **Open Source & Free forever**
+-   Modern, **declarative UI** framework
+-   **100% Python** - Zero HTML, CSS, or JavaScript required
+-   Over **50 Built-in components** for common UI elements, such as `rio.Switch`, `rio.Button`, and `rio.Text`, and many more
+-   Integrates with **modern Python tooling**: Thanks to being **entirely Type Safe** editors can give you instant suggestions and highlight problems right away
+-   Apps can run **both locally and on the web**
+-   **Open Source & Free forever**
 
 ## Installation 🛠️
 
 Rio is available on PyPI, so you can install it using pip:
 
 ```bash
 pip install rio-ui
@@ -46,15 +46,15 @@
 ```bash
 rio new
 ```
 
 You can choose from a variety of built-in templates to get you started. Here's a complete example to create a project based on the tic-tac-toe template:
 
 ```bash
-rio new my-app --type website --template "Tic-Tac-Toe"
+rio new my-project --type website --template "Tic-Tac-Toe"
 cd my-project
 rio run
 ```
 
 You'll have your first app up and running in seconds!
 
 ## How it works 🧠
@@ -66,15 +66,14 @@
 import rio
 from openai import AsyncOpenAI
 
 client = AsyncOpenAI()
 
 
 class DallEPage(rio.Component):
-
     prompt: str = ""
     image_url: str = ""
     is_loading: bool = False
 
     async def get_image(self) -> None:
         """Get an image by prompt."""
 
@@ -137,23 +136,23 @@
         )
 
 
 # Run the app
 app = rio.App(
     pages=[
         rio.Page(
+            name="Home",
             page_url="",
             build=DallEPage,
         ),
     ],
 )
+```
 
 ## Status: In Development 🚧
 
 Rio is still in development. We're working hard to bring you the best possible
-experience. If you have any feedback, please let us know on our Discord server.
+experience. If you have any feedback, please let us know on [our Discord server](https://discord.gg/7ejXaPwhyH).
 
 ## Contributing 🤝
 
-Write how someone can contribute to the project. :)
-
-```
+TODO: Write how someone can contribute to the project. :)
```

### Comparing `rio_ui-0.5.8/rio/__init__.py` & `rio_ui-0.5.9/src/rio/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-import logging
-
-_logger = logging.getLogger(__name__)
-
-# Re-export dataclass stuff for easy use.
-from dataclasses import KW_ONLY as KW_ONLY
-from dataclasses import field as field
-
-# URLs are used as an important datatype within rio. Re-export them for easy
-# use.
-from yarl import URL as URL
-
-# Fix issues in 3rd-party code (like asyncio)
-from . import event as event
-from . import patches_for_3rd_party_stuff
-from .app import *
-from .color import *
-from .common import *
-from .components import *
-from .cursor_style import *
-from .errors import *
-from .fills import *
-from .routing import *
-from .session import *
-from .text_style import *
-from .theme import *
-from .user_settings_module import *
-
-del patches_for_3rd_party_stuff
+__version__ = "0.5.9"
+
+import logging
+
+_logger = logging.getLogger(__name__)
+
+# Re-export dataclass stuff for easy use.
+from dataclasses import KW_ONLY as KW_ONLY
+from dataclasses import field as field
+
+# URLs are used as an important datatype within rio. Re-export them for easy
+# use.
+from yarl import URL as URL
+
+# Fix issues in 3rd-party code (like asyncio)
+from . import event as event
+from . import patches_for_3rd_party_stuff
+from .app import *
+from .color import *
+from .common import *
+from .components import *
+from .cursor_style import *
+from .errors import *
+from .fills import *
+from .routing import *
+from .session import *
+from .text_style import *
+from .theme import *
+from .user_settings_module import *
+
+del patches_for_3rd_party_stuff
```

### Comparing `rio_ui-0.5.8/rio/app.py` & `rio_ui-0.5.9/src/rio/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,33 +26,14 @@
 
 
 __all__ = [
     "App",
 ]
 
 
-def _validate_build_function(
-    build_function: Callable[[], rio.Component],
-) -> Callable[[], rio.Component]:
-    assert callable(
-        build_function
-    ), f"The App requires a function that returns a component, not {build_function!r}"
-
-    def wrapper():
-        component = build_function()
-
-        assert isinstance(
-            component, rio.Component
-        ), f"The `build` function passed to the App must return a `Component` instance, not {component!r}."
-
-        return component
-
-    return wrapper
-
-
 def make_default_connection_lost_component() -> rio.Component:
     class DefaultConnectionLostComponent(rio.Component):
         def build(self) -> rio.Component:
             return rio.Rectangle(
                 content=rio.Row(
                     rio.Icon(
                         "material/error",
@@ -122,15 +103,15 @@
     Or create a server, without running it. This allows you to start the script
     externally with tools such as uvicorn:
 
     ```py
     fastapi_app = app.as_fastapi()
     ```
 
-    Attributes:
+    ## Attributes
         name: The name to display for this app. This can show up in window
             titles, error messages and wherever else the app needs to be
             referenced in a nice, human-readable way.
 
         pages: The pages that make up this app. You can navigate between these
             using `Session.navigate_to` or using `Link` components. If running
             as website the user can also access these pages directly via their
@@ -246,15 +227,15 @@
         # The `main_file` isn't detected correctly if the app is launched via
         # `rio run`. We'll store the user input so that `rio run` can fix the
         # assets dir.
         self._assets_dir = assets_dir
         self.assets_dir = main_file.parent / assets_dir
 
         self.name = name
-        self._build = _validate_build_function(build)
+        self._build = build
         self._icon = assets.Asset.from_image(icon)
         self.pages = tuple(pages)
         self._on_app_start = on_app_start
         self._on_app_close = on_app_close
         self._on_session_start = on_session_start
         self._on_session_close = on_session_close
         self.default_attachments: MutableSequence[Any] = list(default_attachments)
```

### Comparing `rio_ui-0.5.8/rio/app_server.py` & `rio_ui-0.5.9/src/rio/app_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         # time. When a file is uploaded the corresponding future is set.
         self._pending_file_uploads: timer_dict.TimerDict[
             str, asyncio.Future[list[common.FileInfo]]
         ] = timer_dict.TimerDict(default_duration=timedelta(minutes=15))
 
         # FastAPI
         self.add_api_route("/robots.txt", self._serve_robots, methods=["GET"])
-        self.add_api_route("/sitemap.xml", self._serve_sitemap, methods=["GET"])
+        self.add_api_route("/rio/sitemap", self._serve_sitemap, methods=["GET"])
         # self.add_api_route("/app.js.map", self._serve_js_map, methods=["GET"])
         # self.add_api_route("/style.css.map", self._serve_css_map, methods=["GET"])
         self.add_api_route("/rio/favicon.png", self._serve_favicon, methods=["GET"])
         self.add_api_route(
             "/rio/asset/{asset_id:path}", self._serve_asset, methods=["GET"]
         )
         self.add_api_route(
@@ -242,16 +242,14 @@
             print("Exception in `_on_app_close` event handler:")
             traceback.print_exc()
 
     @contextlib.asynccontextmanager
     async def _lifespan(self):
         # If running as a server, periodically clean up expired sessions
         if not self.running_in_window:
-            assert type(self) is AppServer  # Shut up pyright
-
             asyncio.create_task(
                 _periodically_clean_up_expired_sessions(weakref.ref(self)),
                 name="Periodic session cleanup",
             )
 
         # Trigger the app's startup event
         #
@@ -264,21 +262,25 @@
         if self.internal_on_app_start is not None:
             self.internal_on_app_start()
 
         try:
             yield
         finally:
             # Close all sessions
+            rio._logger.debug(
+                f"App server shutting down; closing"
+                f" {len(self._active_session_tokens)} active session(s)"
+            )
+
             results = await asyncio.gather(
                 *(sess._close(True) for sess in self._active_session_tokens.values()),
                 return_exceptions=True,
             )
             for result in results:
                 if isinstance(result, BaseException):
-                    print("Exception in `Session._close()`:")
                     traceback.print_exception(
                         type(result), result, result.__traceback__
                     )
 
             await self._call_on_app_close()
 
     def weakly_host_asset(self, asset: assets.HostedAsset) -> None:
@@ -396,17 +398,17 @@
         Handler for serving the `robots.txt` file via fastapi.
         """
 
         # TODO: Disallow internal API routes? Icons, assets, etc?
         request_url = URL(str(request.url))
         content = f"""
 User-agent: *
-Disallow:
+Allow: /
 
-Sitemap: {request_url.with_path("/sitemap.xml")}
+Sitemap: {request_url.with_path("/rio/sitemap")}
         """.strip()
 
         return fastapi.responses.Response(
             content=content,
             media_type="text/plain",
         )
```

### Comparing `rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf` & `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf` & `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf` & `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf` & `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/OFL.txt` & `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Noto Sans/OFL.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/LICENSE.txt` & `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf` & `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf` & `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf` & `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf` & `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt` & `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf` & `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf` & `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf` & `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf` & `rio_ui-0.5.9/src/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png` & `rio_ui-0.5.9/src/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/hosted/rio-logos/rio-logo-square.png` & `rio_ui-0.5.9/src/rio/assets/hosted/rio-logos/rio-logo-square.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/icon-sets/rio.tar.xz` & `rio_ui-0.5.9/src/rio/assets/icon-sets/rio.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets/icon-sets/styling.tar.xz` & `rio_ui-0.5.9/src/rio/assets/icon-sets/styling.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/assets.py` & `rio_ui-0.5.9/src/rio/assets.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/byte_serving.py` & `rio_ui-0.5.9/src/rio/byte_serving.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/cli/__init__.py` & `rio_ui-0.5.9/src/rio/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/cli/cli_instance.py` & `rio_ui-0.5.9/src/rio/cli/cli_instance.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/cli/nice_traceback.py` & `rio_ui-0.5.9/src/rio/cli/nice_traceback.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/cli/project.py` & `rio_ui-0.5.9/src/rio/cli/project.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/cli/project_setup.py` & `rio_ui-0.5.9/src/rio/cli/project_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,26 +63,31 @@
     Generate the `__init__.py` file for the main module of the project.
     """
     assert len(pages) > 0, pages
 
     # Prepare the different pages
     page_strings = []
     for snip in pages:
+        page_component_name = class_name_from_snippet(snip)
+
         # What's the URL segment for this page?
         if snip is main_page_snippet:
             url_segment = ""
+            page_nicename = "Home"
         else:
             assert snip.name.endswith(".py"), snip.name
             url_segment = snip.name[:-3].replace("_", "-").lower()
+            page_nicename = page_component_name
 
         page_strings.append(
             f"""
         rio.Page(
+            name="{page_nicename}",
             page_url={url_segment!r},
-            build=pages.{class_name_from_snippet(snip)},
+            build=pages.{page_component_name},
         ),"""
         )
 
     page_string = "\n".join(page_strings)
 
     # Imports
     default_theme = rio.Theme.from_color()
```

### Comparing `rio_ui-0.5.8/rio/cli/rio_api.py` & `rio_ui-0.5.9/src/rio/cli/rio_api.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/cli/rioignore.py` & `rio_ui-0.5.9/src/rio/cli/rioignore.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/cli/run_project/app_loading.py` & `rio_ui-0.5.9/src/rio/cli/run_project/app_loading.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/cli/run_project/arbiter.py` & `rio_ui-0.5.9/src/rio/cli/run_project/arbiter.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/cli/run_project/file_watcher_worker.py` & `rio_ui-0.5.9/src/rio/cli/run_project/file_watcher_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/cli/run_project/uvicorn_worker.py` & `rio_ui-0.5.9/src/rio/cli/run_project/uvicorn_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,14 @@
         serve_task = asyncio.create_task(
             self._uvicorn_server.serve(
                 sockets=[self.socket],
             ),
             name="uvicorn serve",
         )
 
-        serve_task = asyncio.shield(serve_task)
-
         # Uvicorn doesn't handle CancelledError properly, which results in ugly
         # output in the console. This monkeypatch suppresses that.
         original_receive = uvicorn.lifespan.on.LifespanOn.receive
 
         async def patched_receive(self) -> Any:
             try:
                 return await original_receive(self)
@@ -88,15 +86,15 @@
                     "type": "lifespan.shutdown",
                 }
 
         uvicorn.lifespan.on.LifespanOn.receive = patched_receive
 
         # Run the server
         try:
-            await serve_task
+            await asyncio.shield(serve_task)
         except asyncio.CancelledError:
             pass
         except Exception as err:
             rio.cli._logger.exception(f"Uvicorn has crashed")
 
             revel.error(f"Uvicorn has crashed:")
             print()
@@ -109,14 +107,16 @@
 
             # Make sure not to return before the task has returned, but also
             # avoid receiving any exceptions _again_
             try:
                 await serve_task
             except:
                 pass
+            finally:
+                rio.cli._logger.debug("Uvicorn serve task has ended")
 
     def replace_app(self, app: rio.App) -> None:
         """
         Replace the app currently running in the server with a new one. The
         worker must already be running for this to work.
         """
         assert self.app_server is not None
```

### Comparing `rio_ui-0.5.8/rio/cli/run_project/webview_worker.py` & `rio_ui-0.5.9/src/rio/cli/run_project/webview_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/cli/tomlconfig.py` & `rio_ui-0.5.9/src/rio/cli/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/color.py` & `rio_ui-0.5.9/src/rio/color.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     # Color(1.0, 0.0, 0.0, 1.0)  # Raises a `RuntimeError`
     ```
 
     Regardless of how the color was created, all of the color's components will
     be accessible as attributes. For example, you can access `color.red`, even
     if the color was created from HSV values.
 
-    Attributes:
+    ## Attributes
         BLACK: A pure black color.
         GREY: A medium grey color.
         WHITE: A pure white color.
         RED: A pure red color.
         GREEN: A pure green color.
         BLUE: A pure blue color.
         CYAN: A pure cyan color.
```

### Comparing `rio_ui-0.5.8/rio/common.py` & `rio_ui-0.5.9/src/rio/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     When asking the user to select a file, this class is used to represent the
     file. It contains metadata about the file, and can also be used to access
     the file's contents.
 
     Be careful when running your app as a webserver, since files will need to be
     uploaded by the user, which is a potentially very slow operation.
 
-    Attributes:
+    ## Attributes
         name: The name of the file, including the extension.
 
         size_in_bytes: The size of the file, in bytes.
 
         media_type: The MIMe type of the file, for example `text/plain` or
             `image/png`.
     """
@@ -308,26 +308,30 @@
         build_result = build_function()
 
     # The function has crashed. Return a placeholder instead
     except Exception as err:
         build_function_repr = _repr_build_function(build_function)
 
         rio._logger.exception(f"An exception occurred in `{build_function_repr}`")
-        return rio.components.build_failed.BuildFailed(
-            f"`{build_function_repr}` has crashed", repr(err)
-        )
+
+        from rio.components.build_failed import BuildFailed  # Screw circular imports
+
+        return BuildFailed(f"`{build_function_repr}` has crashed", repr(err))
 
     # Make sure the result meets expectations
     if not isinstance(build_result, rio.Component):  # type: ignore[unnecessary-isinstance]
         build_function_repr = _repr_build_function(build_function)
 
         rio._logger.error(
             f"The output of `build` methods must be instances of"
             f" `rio.Component`, but `{build_function_repr}` returned `{build_result!r}`"
         )
-        return rio.components.build_failed.BuildFailed(
+
+        from rio.components.build_failed import BuildFailed  # Screw circular imports
+
+        return BuildFailed(
             f"`{build_function_repr}` has returned an invalid result",
             f"Build functions must return instances of `rio.Component`, but the result was {build_result!r}",
         )
 
     # All is well
     return build_result
```

### Comparing `rio_ui-0.5.8/rio/components/__init__.py` & `rio_ui-0.5.9/src/rio/components/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/components/app_root.py` & `rio_ui-0.5.9/src/rio/components/app_root.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/components/auto_form.py` & `rio_ui-0.5.9/src/rio/components/auto_form.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/components/banner.py` & `rio_ui-0.5.9/src/rio/components/banner.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     to be communicated.
 
     The messages have one of four levels: success, info, warning, and error. The
     levels control the appearance of the notification bar, and allow you to
     quickly communicate the nature of the message to the user.
 
 
-    ## Attributes:
+    ## Attributes
 
     `text`: The text to display. If `None` or empty, the banner will disappear
             entirely.
 
     `style`: Controls the appearance of the banner. The style is one of
             `info`, `success`, `warning` and `danger`. Depending on the value
             the banner may change its colors and icon.
@@ -43,15 +43,15 @@
             plain text.
 
     `multiline`: Whether long text may be wrapped over multiple lines.
             Multiline banners are also styled slightly differently to make the
             icon fit their larger size. Use `"\n"` to add a line break.
 
 
-    ## Example:
+    ## Example
 
     This minimal example will simply display a banner with the text "This is a
     banner":
 
     ```python
     rio.Banner(text="This is a banner", style="info")
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/build_failed.py` & `rio_ui-0.5.9/src/rio/components/build_failed.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/components/button.py` & `rio_ui-0.5.9/src/rio/components/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,32 +27,32 @@
 
     A clickable button.
 
     The `Button` component allows the user to trigger an action by clicking on
     it. You can use it to trigger a function call, navigate to a different page,
     or perform other actions.
 
-    ## Attributes:
+    ## Attributes
 
     `content`: The text or child component to display inside of the button.
 
     `icon`: The name of an icon to display on the button, in the form
         "set/name:variant". See the `Icon` component for details of how
         icons work in Rio.
 
     `shape`: The shape of the button. This can be one of:
-    - `pill`: A rectangle where the left and right sides are completely round.
-    - `rounded`: A rectangle with rounded corners.
-    - `rectangle`: A rectangle with sharp corners.
+        - `pill`: A rectangle where the left and right sides are completely round.
+        - `rounded`: A rectangle with rounded corners.
+        - `rectangle`: A rectangle with sharp corners.
 
     `style`: Controls the button's appearance. This can be one of:
-    - `major`: A highly visible button with bold visuals.
-    - `minor`: A less visible button that blends into the background.
-    - `plain`: A button with no background or border. Use this to make
-            the button look like a link.
+        - `major`: A highly visible button with bold visuals.
+        - `minor`: A less visible button that blends into the background.
+        - `plain`: A button with no background or border. Use this to make
+                the button look like a link.
 
     `color`: The color scheme to use for the button.
 
     `is_sensitive`: Whether the button should respond to user input.
 
     `is_loading`: Whether the button should display a loading indicator. Use
         this to indicate to the user that an action is currently running.
@@ -61,15 +61,15 @@
         disabled for after it is first rendered. This is useful to prevent
         the user from accidentally triggering an action when the page is
         first loaded.
 
     `on_press`: Triggered when the user clicks on the button.
 
 
-    ## Example:
+    ## Example
 
     This minimal example will simply display a `Button` with the text "Click
     me!" and a castle icon:
 
     ```python
     rio.Button(content="Click me!", icon="material/castle")
     ```
@@ -239,15 +239,15 @@
     on it. You can use it to trigger a function call, navigate to a different
     page, or perform other actions.
 
     It is similar to the `Button` component, but it is specifically designed to
     display an icon, and it has a round shape.
 
 
-    ## Attributes:
+    ## Attributes
 
     `icon`: The name of an icon to display on the button, in the form
             "set/name:variant". See the `Icon` component for details of how
             icons work in Rio.
 
     `style`: Controls the button's appearance. This can be one of:
     - `major`: A highly visible button with bold visuals.
@@ -266,15 +266,15 @@
 
     `size`: The size of the button. This is the diameter of the button in
             font-size units.
 
     `on_press`: Triggered when the user clicks on the button.
 
 
-    ## Example:
+    ## Example
 
     This minimal example will simply display a `IconButton` with a castle icon:
 
     ```python
     rio.IconButton(icon="material/castle")
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/card.py` & `rio_ui-0.5.9/src/rio/components/card.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     structured way.
 
     Cards are also often used as large buttons. They can be configured to
     elevate slightly when the mouse hovers over them, indicating to the user
     that they support interaction.
 
 
-    ## Attributes:
+    ## Attributes
 
     `content`: The component to display inside the card.
 
     `corner_radius`: The radius of the card's corners. If set to `None`, it
             is picked from the active theme.
 
     `on_press`: An event handler that is called when the card is clicked.
@@ -51,15 +51,15 @@
             color if an `on_press` event handler is attached.
 
     `color`: The color scheme to use for the card. The color scheme controls
             the background color of the card, and the color of the text and
             icons inside it. Check `rio.Color` for details.
 
 
-    ## Example:
+    ## Example
 
     This minimal example will simply display a `Card` with the castle icon
     in it:
 
     ```python
     rio.Card(content=rio.Icon("material/castle"))
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/class_container.py` & `rio_ui-0.5.9/src/rio/components/class_container.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Component which holds a single child, and applies a list of CSS classes to
     it. This is enough to implement several components, preventing the need to
     create a whole bunch of almost identical JavaScript components.
 
     This component is only intended for internal use and is not part of the
     public API.
 
-    ## Attributes:
+    ## Attributes
 
     `content`: The child component to apply the classes to.
 
     `classes`: The list of classes to apply to the child component.
     """
 
     content: rio.Component | None
```

### Comparing `rio_ui-0.5.8/rio/components/color_picker.py` & `rio_ui-0.5.9/src/rio/components/color_picker.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,34 +22,34 @@
 
 
 @final
 class ColorPicker(FundamentalComponent):
     """
     # ColorPicker
 
-    Allows the user to pick an RGB(A) color.
+    Allows the user to pick a RGB(A) color.
 
     `ColorPicker` is a component that allows the user to pick a color. It
     displays a combination of colorful areas and sliders that the user can
     interact with to pick a color, and optionally an opacity slider to pick
     opacity.
 
 
-    ## Attributes:
+    ## Attributes
 
     `color`: The color that the user has picked.
 
     `pick_opacity`: Whether to allow the user to pick opacity. If `False`,
             the opacity slider will be hidden and the color value will be forced
             to be fully opaque.
 
     `on_change`: This event is triggered whenever the user changes the color.
 
 
-    ## Example:
+    ## Example
 
     This minimal example will simply display a `ColorPicker` with the default
     color red:
 
     ```python
     rio.ColorPicker(rio.Color.from_hex("#ff0000"))
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/component.py` & `rio_ui-0.5.9/src/rio/components/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
     Base class for all `rio` components.
 
     Components are the building blocks of `rio` apps. `rio` ships with many
     useful components out of the box, but you can also subclass a component to
     create your own.
 
 
-    ## Attributes:
+    ## Attributes
 
     `key`: A unique identifier for this component. If two components with the
         same key are present during reconciliation they will be considered
         the same component and their state will be preserved. If no key is
         specified, reconciliation falls back to a less precise method, by
         comparing the location of the component in the component tree.
```

### Comparing `rio_ui-0.5.8/rio/components/component_tree.py` & `rio_ui-0.5.9/src/rio/components/component_tree.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/components/container.py` & `rio_ui-0.5.9/src/rio/components/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,20 +19,20 @@
     A component holding a single child.
 
     `Container` is a simple container which holds a single child component. It
     is useful for when you receive a component as child and wish to add
     additional layout attributes such as a margin.
 
 
-    ## Attributes:
+    ## Attributes
 
     `content`: The component to place inside the container.
 
 
-    ## Example:
+    ## Example
 
     This minimal example will simply display a `container` with the text "Hello
     World!":
 
     ```python
     rio.Container(rio.Text("Hello World!"))
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/devel_component.py` & `rio_ui-0.5.9/src/rio/components/devel_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/components/drawer.py` & `rio_ui-0.5.9/src/rio/components/drawer.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     drawer. The `content` is located inside the drawer and is only visible when
     the drawer is open.
 
     Drawers have the ability to be `modal`. Modal drawers draw attention to
     themselves and prevent interaction with the anchor while open.
 
 
-    ## Attributes:
+    ## Attributes
 
     `anchor`: A component which is always visible and positions the drawer.
 
     `content`: A component which is only visible when the drawer is open.
 
     `on_open_or_close`: Triggered whenever the user opens or closes the
         drawer.
@@ -57,15 +57,15 @@
     `is_open`: Whether the drawer is currently open.
 
     `is_user_openable`: Whether the user can open or close the drawer. If this
         is `False`, the drawer can only be opened or closed
         programmatically.
 
 
-    ## Example:
+    ## Example
 
     A simple drawer with a button as the anchor and some text as content:
 
     ```python
     rio.Drawer(
         anchor=rio.Button("Click Me!"),
         content=rio.Text("It was clickbait!"),
```

### Comparing `rio_ui-0.5.8/rio/components/dropdown.py` & `rio_ui-0.5.9/src/rio/components/dropdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     Dropdowns present the user with a list of options, allowing them to select
     exactly one. In their default state dropdowns are compact and display the
     currently selected option. When activated, a popup menu appears with a list
     of all available options.
 
 
-    ## Attributes:
+    ## Attributes
 
     `options`: A mapping from option names to values. The names are displayed
             in the dropdown menu, and the corresponding value is returned when
             the user selects the option. The values must be comparable.
 
     `label`: A short text to display next to the dropdown.
 
@@ -52,15 +52,15 @@
     `is_valid`: Visually displays to the user whether the current option is
         valid. You can use this to signal to the user that their input needs
         to be changed.
 
     `on_change`: Triggered whenever the user selects an option.
 
 
-    ## Example:
+    ## Example
 
     This minimal example will simply display a dropdown with three options:
 
     ```python
     rio.Dropdown(["a", "b", "c"])
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/flow_container.py` & `rio_ui-0.5.9/src/rio/components/flow_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,27 +20,27 @@
     A container that lays out its children in a horizontal or vertical flow.
 
     `FlowContainer` is a container that lays out its children in a horizontal or
     vertical flow. It is similar to `Container`, but allows you to specify
     spacing between the children.
 
 
-    ## Attributes:
+    ## Attributes
 
     `children`: The components to place inside the container.
 
     `row_spacing`: The vertical spacing between the children.
 
     `column_spacing`: The horizontal spacing between the children.
 
     `justify`: The horizontal alignment of the children. Possible values are:
         `left`, `center`, `right`, `justified` and `grow`.
 
 
-    ## Example:
+    ## Example
 
     This minimal example will show a container with a horizontal flow:
 
     ```python
     rio.FlowContainer(
         rio.Text("Hello"),
         rio.Text("World!"),
```

### Comparing `rio_ui-0.5.8/rio/components/fundamental_component.py` & `rio_ui-0.5.9/src/rio/components/fundamental_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/components/grid.py` & `rio_ui-0.5.9/src/rio/components/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,22 +32,22 @@
     A container which arranges its children in a table-like grid.
 
     Grids arrange their children in a table-like grid. Each child is placed in
     one or more cells of the grid. You can add children to the grid either by
     passing them in as a list or by using the `grid_add` method.
 
 
-    ## Attributes:
+    ## Attributes
 
     `row_spacing`: The amount of space between rows of the grid.
 
     `column_spacing`: The amount of space between columns of the grid.
 
 
-    ## Example:
+    ## Example
 
     This code creates a grid layout with two rows and two columns, and adds
     children to the grid by passing them in as a list:
 
     ```python
     rio.Grid(
         [rio.Text("Hello"), rio.Text("World!")],  # 1. Row
```

### Comparing `rio_ui-0.5.8/rio/components/html.py` & `rio_ui-0.5.9/src/rio/components/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     Renders HTML.
 
     `Html` allows you to embed HTML in your app. It takes HTML code as input and
     renders it. If you want to embed an entire website, use the `Website`
     component instead.
 
 
-    ## Attributes:
+    ## Attributes
 
     `html`: The HTML to render.
 
-    ## Example:
+    ## Example
 
     This minimal example will render a simple HTML code:
     TODO: Add example
     """
 
     html: str
```

### Comparing `rio_ui-0.5.8/rio/components/icon.py` & `rio_ui-0.5.9/src/rio/components/icon.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,25 +42,25 @@
     run`.)
 
     The set name and variant can be omitted. If no set name is specified, it
     defaults to `material`. If no variant is specified, the default version of
     the icon, i.e. no variant, is used.
 
 
-    ## Attributes:
+    ## Attributes
 
     `icon`: The name of the icon to display, in the format
         `icon-set/name:variant`. You can browse all available icons in Rio's
         debugger sidebar.
 
     `fill`: The color scheme of the icon. The text color is used if no fill is
         specified.
 
 
-    ## Example:
+    ## Example
 
     This minimal example will simply display an Icon:
 
     ```python
     rio.Icon("material/castle")
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/image.py` & `rio_ui-0.5.9/src/rio/components/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
       maintaining its aspect ratio. This is the default.
     - `stretch`: The image is stretched to fill the shape, distorting it if
       necessary.
     - `zoom`: The image is scaled to fill the shape entirely, while maintaining
       its aspect ratio. This may cause the image to overflow the shape.
 
 
-    ## Attributes:
+    ## Attributes
 
     `image`: The image to display.
 
     `fill_mode`: How the image should be scaled to fit the shape. If `fit`,
             the image is scaled to fit entirely inside the shape. If `stretch`,
             the image is stretched to fill the shape exactly, possibly
             distorting it in the process. If `zoom`, the image is scaled to fill
@@ -51,15 +51,15 @@
     `corner_radius`: How round to make the corners of the image. If a single
             number is given, all four corners will be rounded equally. If a
             tuple of four numbers is given, they will be interpreted as the
             radii of the top-left, top-right, bottom-right, and bottom-left
             corners, in that order.
 
 
-    ## Example:
+    ## Example
 
     This minimal example will simply display an image with the URL
     "https://example.com/image.png":
 
     ```python
     rio.Image(rio.URL("https://example.com/image.png"))
     ````
```

### Comparing `rio_ui-0.5.8/rio/components/key_event_listener.py` & `rio_ui-0.5.9/src/rio/components/key_event_listener.py`

 * *Files 0% similar despite different names*

```diff
@@ -613,15 +613,15 @@
     `KeyEventListener` is a container for a single child component. It listens
     for keyboard events and calls corresponding event handlers when they occur.
 
     Keep in mind that `KeyEventListener` will only report events that have not
     been handled by a child component. For example, typing into a `TextInput`
     will not trigger a `KeyEventListener`.
 
-    Attributes:
+    ## Attributes
         content: The child component.
 
         on_key_down: A function to call when a key is pressed down.
 
         on_key_up: A function to call when a key is released.
 
         on_key_press: A function to call repeatedly while a key is held down.
```

### Comparing `rio_ui-0.5.8/rio/components/labeled_column.py` & `rio_ui-0.5.9/src/rio/components/labeled_column.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,20 +21,20 @@
     A container that lays out its children in a column, with labels for each child.
 
     `LabeledColumn` is a container that lays out its children in a column, with
     labels for each child. It is similar to `Column`, but allows you to specify
     labels for each child.
 
 
-    ## Attributes:
+    ## Attributes
 
     `content`: The components to place inside the container, with labels.
 
 
-    ## Example:
+    ## Example
 
     This minimal example will show a container with a column layout and labels:
 
     ```python
     rio.LabeledColumn(
         {
             "First Name": rio.TextInput(),
```

### Comparing `rio_ui-0.5.8/rio/components/linear_containers.py` & `rio_ui-0.5.9/src/rio/components/linear_containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,27 +65,27 @@
     unmistakable animated sprites.
 
     Getting rid of undefined space is easy: Depending on what look you're going
     for, either add a `Spacer` somewhere into your `Row`, assign one of the
     components a `"grow"` value as its height, or set the `Row`'s vertical
     alignment.
 
-    ## Attributes:
+    ## Attributes
 
     `children`: The components to place in this `Row`.
 
     `spacing`: How much empty space to leave between two adjacent children. No
             spacing is added before the first child or after the last child.
 
     `proportions`: If set, the children will grow according to these proportions.
         - `homogeneous`: All children will grow equally.
         - A list of floats: Each child will grow according to its proportion.
         - `None`: Allows all child components to expand as much as they need.
 
-    ## Example:
+    ## Example
 
     This minimal example will display a `Row` with two text components:
 
     ```python
     rio.Row(rio.Text("Hello"), rio.Text("World!"))
     ```
 
@@ -181,28 +181,28 @@
 
     Getting rid of undefined space is easy: Depending on what look you're going
     for, either add a `Spacer` somewhere into your `Column`, assign one of the
     components a `"grow"` value as its height, or set the `Column`'s vertical
     alignment.
 
 
-    ## Attributes:
+    ## Attributes
 
     `children`: The components to place in this `Column`.
 
     `spacing`: How much empty space to leave between two adjacent children. No
             spacing is added before the first child or after the last child.
 
     `proportions`: If set, the children will grow according to these proportions.
         - `homogeneous`: All children will grow equally.
         - A list of floats: Each child will grow according to its proportion.
         - `None`: Allows all child components to expand as much as they need.
 
 
-    ## Example:
+    ## Example
 
     This minimal example will display a `Column` with two text components:
 
     ```python
     rio.Column(rio.Text("Hello"), rio.Text("World!"))
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/link.py` & `rio_ui-0.5.9/src/rio/components/link.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 
     Navigates to a page or URL when clicked.
 
     `Link`s display a short text, or arbitrary component, and navigate to a page
     or URL when clicked.
 
 
-    ## Attributes:
+    ## Attributes
 
 
     `child_text`: The text to display inside the link.
 
     `child_component`: The component to display inside the link.
 
     `target_url`: The page or URL to navigate to when clicked.
 
     `open_in_new_tab`: Whether to open the link in a new tab. Defaults to `False`.
 
 
-    ## Example:
+    ## Example
 
     This minimal example will simply display a link with the URL
     "https://example.com" and a text "Click me!":
 
     ```python
     rio.Link("Click me!", "https://example.com")
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/list_items.py` & `rio_ui-0.5.9/src/rio/components/list_items.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 
     `HeadingListItem`s are the easiest way to create list items, which can take
     care of the most primitive task: Display a text. If your want a more generic
     list item with additional children, you can use the `SimpleListItem`. Or if
     you want to build a more complex list item, you can use the
     `CustomListItem`.
 
-    ## Attributes:
+    ## Attributes
 
     `text`: The text to display.
 
-    ## Example:
+    ## Example
 
     This minimal example will simply display a list item with the text "Click
     me!":
 
     ```python
     rio.HeadingListItem("Click me!", key="item1")
     ```
@@ -242,26 +242,26 @@
     A list item with custom content.
 
     Most of the time the `SimpleListItem` will do the job. With
     `CustomListItems` you can build more complex list items. You can add any
     component to the list item. This can be e.g. a `Row`, `Column`, `Text`,
     `Icon`, `Image` or any other component.
 
-    ## Attributes:
+    ## Attributes
 
     `content`: The content to display.
 
     `on_press`: Triggered when the list item is pressed.
 
     `key`: A unique key to identify the list item. This is used to avoid
         unintentional reconciliation with other items when the list is
         updated.
 
 
-    ## Example:
+    ## Example
 
     Instead of using the `SimpleListItem` you can use the `CustomListItem` to create
     a custom list item. This can be useful if you want to add more complex content
     to the list item. You can add any component to the list item.
 
     ```python
     class MyCustomListItemComponent(rio.Component):
```

### Comparing `rio_ui-0.5.8/rio/components/list_view.py` & `rio_ui-0.5.9/src/rio/components/list_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,23 +17,23 @@
     # ListView
 
     Vertically arranges and styles its children.
 
     A container which arranges its children in a vertical list. It is similar to `Column`,
     but it is optimized for displaying large numbers of items.
 
-    ## Attributes:
+    ## Attributes
 
     `children`: The children to display in the list.
 
     `key`: A unique key for this component. If the key changes, the component will be
             destroyed and recreated. This is useful for components which maintain state
             across rebuilds.
 
-    ## Example:
+    ## Example
 
     A minimal example of a `ListView` with two items will be shown:
 
     ```python
     rio.ListView(
         rio.SimpleListItem("Product 1", key="item1"),
         rio.SimpleListItem("Product 2", key="item2"),
```

### Comparing `rio_ui-0.5.8/rio/components/markdown.py` & `rio_ui-0.5.9/src/rio/components/markdown.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,29 +19,29 @@
     lightweight markup language that allows you to write text with simple
     formatting, such as **bold**, *italics*, and links.
 
     Markdown is a great way to write text that is both human-readable, yet
     beautifully formatted.
 
 
-    ## Attributes:
+    ## Attributes
 
     `text`: The markdown-formatted text to display.
 
     `default_language`: The default language to use for code blocks. If
         `None`, Rio will try to guess the language automatically. If a
         default is given, it will be used for all code blocks that don't
         specify a language explicitly.
 
         Inline code will always use the default language, since they are too
         short to reliably guess the language - so make sure to set a default
         language if you want your inline code to be syntax-highlighted.
 
 
-    ## Example:
+    ## Example
 
     This minimal example will simply display the bold text "Hello World!":
 
     ```python
     rio.Markdown("**Hello World!**")
     ```
     """
```

### Comparing `rio_ui-0.5.8/rio/components/media_player.py` & `rio_ui-0.5.9/src/rio/components/media_player.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     `MediaPlayer` plays back audio and video files. It can play local files and
     URLs.
 
     Note that the `MediaPlayer` component doesn't reserve any space for itself,
     it simply makes do with the space it is given by its parent component.
 
 
-    ## Attributes:
+    ## Attributes
     `media`: The media to play. This can be a file path, URL, or bytes.
 
     `media_type`: The mime type of the media file. May help the browser to
             play the file correctly.
 
     `loop`: Whether to automatically restart from the beginning when the
             playback ends.
@@ -51,15 +51,15 @@
     `on_playback_end`: An event handler to call when the media finishes
             playing.
 
     `on_error`: An event handler to call when an error occurs, for example if
             the file format isn't supported.
 
 
-    ## Example:
+    ## Example
 
     A minimal example of a `MediaPlayer` playing a local file will be shown:
 
     ```python
     rio.MediaPlayer(rio.URL("https://example.com/example_video.mp4"))
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/mouse_event_listener.py` & `rio_ui-0.5.9/src/rio/components/mouse_event_listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     """
     Allows you to listen for mouse events on a component.
 
     `MouseEventListeners` take a single child component and display it. They
     then listen for any mouse activity on the child component and report it
     through their event handlers.
 
-    Attributes:
+    ## Attributes
         content: The child component to display.
 
         on_press: Similar to `on_mouse_up`, but performs additional subtle
             checks, such as that the left mouse button was pressed.
 
         on_mouse_down: Triggered when a mouse button is pressed down while
             the mouse is placed over the child component.
```

### Comparing `rio_ui-0.5.8/rio/components/multi_line_text_input.py` & `rio_ui-0.5.9/src/rio/components/multi_line_text_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     It's similar to `TextInput`, but it allows the user to enter multiple lines of text.
 
     `MultiLineTextInput` allows the user to enter a short text. The text can either be
     shown in plain text or other sensitive information.
 
 
-    ## Attributes:
+    ## Attributes
 
     `text`: The text currently entered by the user.
 
     `label`: A short text to display next to the text input.
 
     `is_sensitive`: Whether the text input should respond to user input.
 
@@ -56,15 +56,15 @@
     `on_change`: Triggered when the user changes the text.
 
     `on_confirm`: Triggered when the user explicitly confirms their input,
             such as by pressing the "Enter" key. You can use this to trigger
             followup actions, such as logging in or submitting a form.
 
 
-    ## Example:
+    ## Example
 
     A minimal example of `MultiLineTextInput` with a default text of "" will be shown:
     `Note`: The text will not be updated if the user changes the text in the input field.
 
     ```python
     rio.MultiLineTextInput(text="")
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/node_input.py` & `rio_ui-0.5.9/src/rio/components/node_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/components/node_output.py` & `rio_ui-0.5.9/src/rio/components/node_output.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/components/number_input.py` & `rio_ui-0.5.9/src/rio/components/number_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     Number inputs go way beyond just parsing the input using `int` or `float`.
     They try their best to understand what the user is trying to enter, and also
     support suffixes such as "k" and "m" to represent thousands and millions
     respectively.
 
 
-    ## Attributes:
+    ## Attributes
 
     `value`: The number currently entered by the user.
 
     `label`: A short text to display next to the text input.
 
     `prefix_text`: A short text to display before the text input. Useful for
             displaying currency symbols or other prefixed units.
@@ -82,15 +82,15 @@
 
     `on_change`: Triggered when the user changes the number.
 
     `on_confirm`: Triggered when the user explicitly confirms their input,
             such as by pressing the "Enter" key.
 
 
-    ## Example:
+    ## Example
 
     A minimal example of `NumberInput` with a default value of 20.00 will be shown:
     Note: The text will not be updated if the user changes the value in the input field.
 
     ```python
     rio.NumberInput(value=20.00)
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/overlay.py` & `rio_ui-0.5.9/src/rio/components/overlay.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,22 +23,22 @@
     the page and is exempt from layouting.
 
     Components inside of overlays are allocated the entire screen, and are
     themselves responsible for positioning themselves as required. You can
     easily achieve this using the child's `align_x` and `align_y` properties.
 
 
-    ## Attributes:
+    ## Attributes
 
     `content`: The component to display in the overlay. It will take up the
         entire size of the screen, so make sure to use properties such as
         `align_x` and `align_y` to position it as needed.
 
 
-    ## Example:
+    ## Example
 
     A simple example will display an `Overlay` with the text "Hello, world!" centered on the screen:
 
     ```python
     rio.Overlay(
         rio.Text("Hello, world!"),
         align_x=0.5,
```

### Comparing `rio_ui-0.5.8/rio/components/page_view.py` & `rio_ui-0.5.9/src/rio/components/page_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,41 +59,43 @@
 
     Rio apps can consist of many pages. You might have a welcome page, a
     settings page, a login, and so on. Page views act as placeholders, that
     don't have an appearance of their own, but instead look up the currently
     active page, and display that.
 
 
-    ## Attributes:
+    ## Attributes
 
     `fallback_build`: A callback that is called if the current URL does not
         correspond to any page in the application. It should return a Rio
         component that is displayed instead. If not specified Rio will
         display a default error page.
 
 
-    ## Example:
+    ## Example
 
     A minimal example:
 
     ```python
     app = rio.App(
         build=lambda: rio.Column(
             rio.Text("Welcome to my page!"),
             rio.PageView(
                 width="grow",
                 height="grow",
             ),
         ),
         pages=[
             rio.Page(
+                "Home",
                 "",
                 build=lambda: rio.Text("This is the home page"),
             ),
             rio.Page(
+                "Subpage",
                 "subpage",
                 build=lambda: rio.Text("This is a subpage"),
             ),
         ],
     )
 
     app.run_in_browser()
```

### Comparing `rio_ui-0.5.8/rio/components/plot.py` & `rio_ui-0.5.9/src/rio/components/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 
 
 @final
 class Plot(FundamentalComponent):
     """
     # Plot
 
-    Displays a matplotlib, seaborn or plotly plot.
+    Displays a `matplotlib`, `seaborn` or `plotly` plot.
 
 
-    ## Attributes:
+    ## Attributes
 
     `figure`: The plot figure to display.
 
     `background`: The background color of the plot. If `None`, a color from
         the theme is used.
 
     `corner_radius`: The corner radius of the plot
 
 
-    ## Example:
+    ## Example
 
     A minimal example with a plotly plot:
 
     ```python
     import plotly.graph_objects as go
 
     fig = go.Figure()
```

### Comparing `rio_ui-0.5.8/rio/components/popup.py` & `rio_ui-0.5.9/src/rio/components/popup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     the popup is open.
 
     The location popups appear at can be customized using the `direction`,
     `alignment` and `gap` attributes. Popups wil do their best to honor those
     settings, but deviate if necessary to ensure they don't go off-screen.
 
 
-    ## Attributes:
+    ## Attributes
 
     `anchor`: A component which is always visible and positions the popup.
 
     `content`: A component which is only visible when the popup is open.
 
     `direction`: The direction into which the popup opens.
 
@@ -60,15 +60,15 @@
             effect popup opens centered.
 
     `is_open`: Whether the popup is currently open.
 
     `on_open_or_close`: Triggered when the popup is opened or closed.
 
 
-    ## Example:
+    ## Example
 
     A simple popup with a button as the anchor and a text input as the content:
 
     TODO: add example
 
     """
```

### Comparing `rio_ui-0.5.8/rio/components/progress_bar.py` & `rio_ui-0.5.9/src/rio/components/progress_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,21 @@
     display the exact progress as a fraction from 0 to 1, or it can display an
     indeterminate progress animation, which is useful when the exact progress
     isn't known.
 
     The circular counterpart to this component is the `ProgressCircle`.
 
 
-    ## Attributes:
+    ## Attributes
 
     `progress`: The progress to display, as a fraction from 0 to 1. If `None`,
             the progress indicator will be indeterminate.
 
 
-    ## Example:
+    ## Example
 
     A minimal example displaying a progress bar that is 50% complete.
 
     ```python
     rio.ProgressBar(progress=0.5)
     ```
     """
```

### Comparing `rio_ui-0.5.8/rio/components/progress_circle.py` & `rio_ui-0.5.9/src/rio/components/progress_circle.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,29 +26,29 @@
     Note that unlike most components in Rio, `ProgressCircle` does not have a
     `natural` size, since the circle can easily be scaled to fit any size.
     Therefore it defaults to a reasonable size which should fit most use cases.
 
     The linear counterpart to this component is the `ProgressBar`.
 
 
-    ## Attributes:
+    ## Attributes
 
     `progress`: The progress to display, as a fraction from 0 to 1. If `None`,
             the progress indicator will be indeterminate.
 
     `color`: The color scheme of the progress indicator. Keeping the default
                 is recommended, but it may make sense to change the color in
                 case the default is hard to perceive on your background.
 
     `size`: The size of the progress indicator. This is equivalent to setting
             a component's `width` and `height` to the same value.
 
 
 
-    ## Example:
+    ## Example
 
     A minimal example displaying a progress circle that is 50% complete.
 
     ```python
     rio.ProgressCircle(progress=0.5)
     ```
     """
```

### Comparing `rio_ui-0.5.8/rio/components/rectangle.py` & `rio_ui-0.5.9/src/rio/components/rectangle.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     Rectangles also act as a simple source of animations. They accept two
     styles: A default style for when the user isn't interacting with them, and a
     hover style for when the mouse hovers above them. This, along with their
     `transition_time` attribute allows you to make your app feel dynamic and
     alive.
 
 
-    ## Attributes:
+    ## Attributes
 
     `content`: The component to display inside the rectangle.
 
     `style`: How the rectangle should appear when the user isn't interacting
         with it.
 
     `hover_style`: The style of the rectangle when the mouse hovers above it.
@@ -51,15 +51,15 @@
 
     `cursor`: The cursor to display when the mouse hovers above the rectangle.
 
     `ripple`: Whether to display a Material Design ripple effect when the
         rectangle is hovered or clicked.
 
 
-    ## Example:
+    ## Example
 
     A minimal example of a rectangle with a text and red background will be shown:
 
     ```python
     rio.Rectangle(
         content=rio.Text("Hello World!"),
         fill=rio.Color.from_hex("ff0000"),
```

### Comparing `rio_ui-0.5.8/rio/components/revealer.py` & `rio_ui-0.5.9/src/rio/components/revealer.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     A component that can be used to hide and reveal content.
 
     `Revealer` is a versatile component that can be used to hide and reveal
     content. It can be used to create collapsible sections, or to hide and
     reveal content based on user input.
 
 
-    ## Attributes:
+    ## Attributes
 
     `header`: The header of the `Revealer`. If `None`, the `Revealer` will be
             hidden by default.
 
     `content`: The content to display when the `Revealer` is open.
 
     `header_style`: The style of the header. Can be one of `"heading1"`,
@@ -48,15 +48,15 @@
     `is_open`: Whether the `Revealer` is open or not.
 
     `on_change`: An event handler that is called when the `Revealer` is opened
             or closed. The event handler receives a `RevealerChangeEvent` as
             input.
 
 
-    ## Example:
+    ## Example
 
     A simple `Revealer` that displays "Hello" when opened:
 
     ```python
     rio.Revealer(header="Click to reveal", content=rio.Text("Hello"))
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/root_components.py` & `rio_ui-0.5.9/src/rio/components/root_components.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/components/scroll_container.py` & `rio_ui-0.5.9/src/rio/components/scroll_container.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     Displays a scroll bar if its child grows too large.
 
     `ScrollContainer` is a container which displays a scroll bar if its child
     component grows too large. It can scroll vertically and/or horizontally.
 
 
-    ## Attributes:
+    ## Attributes
 
     `content`: The child component to display inside the `ScrollContainer`.
 
     `scroll_x`: Controls horizontal scrolling. The default is `"auto"`, which
         means that a scroll bar will be displayed only if it is needed.
         `"always"` displays a scroll bar even if it isn't needed, and
         `"never"` disables horizontal scrolling altogether.
@@ -36,15 +36,15 @@
         `"never"` disables vertical scrolling altogether.
 
     `sticky_bottom`: If `True`, when the user has scrolled to the bottom and
         the content of the `ScrollContainer` grows larger, the scroll bar
         will automatically scroll to the bottom again.
 
 
-    ## Example:
+    ## Example
 
     A minimal example of `ScrollContainer` displaying an icon:
 
     ```python
     rio.ScrollContainer(
         content=rio.Icon("material/castle", width=50, height=50),
         height=10,
```

### Comparing `rio_ui-0.5.8/rio/components/scroll_target.py` & `rio_ui-0.5.9/src/rio/components/scroll_target.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,23 +19,23 @@
     `ScrollTarget` is a container which can be referenced by a URL fragment,
     which allows browsers to scroll to it when the page is loaded. For example,
     if your website contains a `ScrollTarget` with the ID `"my-section"`, then a
     browser visiting `https://your.website/#my-section` will immediately scroll
     it into view.
 
 
-    ## Attributes:
+    ## Attributes
 
     `id`: The ID of the `ScrollTarget`. This must be unique among all
             `ScrollTarget`s on the page.
 
     `content`: The child component to display inside the `ScrollTarget`.
 
 
-    ## Example:
+    ## Example
 
     A minimal example of `ScrollTarget` displaying an icon:
 
     #TODO: Better example
     ```python
     rio.ScrollTarget(
         id="my-section",
```

### Comparing `rio_ui-0.5.8/rio/components/separator.py` & `rio_ui-0.5.9/src/rio/components/separator.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,21 +20,21 @@
     A line to separate content.
 
     `Separator` is a horizontal or vertical line that can be used to separate content. It
     can be styled with a color. By default, it is a thin line with a light gray
     color.
 
 
-    ## Attributes:
+    ## Attributes
 
     `color`: The color of the `Separator`. If `None`, the color will be
             determined by the theme.
 
 
-    ## Example:
+    ## Example
 
     A minimal example of `Separator`:
 
     ```python
     rio.Separator()
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/slider.py` & `rio_ui-0.5.9/src/rio/components/slider.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,28 +29,28 @@
     A component for selecting a single value from a range.
 
     The `Slider` components allows the user to select a single real number value
     by dragging a handle along a line. The value can be any number within a
     range you can specify.
 
 
-    ## Attributes:
+    ## Attributes
 
     `minimum`: The minimum value the slider can be set to.
 
     `maximum`: The maximum value the slider can be set to.
 
     `value`: The current value of the slider.
 
     `is_sensitive`: Whether the slider should respond to user input.
 
     `on_change`: A callback that is called when the value of the slider changes.
 
 
-    ## Example:
+    ## Example
 
     A minimal example of a `Slider` ranging from 0 to 100 will be shown:
 
     ```python
     rio.Slider(minimum=0, maximum=100)
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/slideshow.py` & `rio_ui-0.5.9/src/rio/components/slideshow.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,27 +24,27 @@
 
     The `Slideshow` component is a container that can hold multiple components,
     and will display them one after the other, with smooth transitions in
     between. These are very useful for displaying a series of demos or news to
     visitors.
 
 
-    ## Attributes:
+    ## Attributes
 
     `children`: The components to transition between.
 
     `linger_time`: The time in seconds to display each component before
             switching to the next one.
 
     `corner_radius`: How rounded the slideshow's corners should be. If set to
             `None`, the slideshow will use a default corner radius from the
             current theme.
 
 
-    ## Example:
+    ## Example
 
     A minimal example of `Slideshow` displaying two images will be shown:
 
     ```python
     from pathlib import Path
 
     PATH = Path(__file__).parent
```

### Comparing `rio_ui-0.5.8/rio/components/spacer.py` & `rio_ui-0.5.9/src/rio/components/spacer.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     components. While similar effects can often be achieved using margins and
     alignment, code with spacers can sometimes be easier to read.
 
     Note that unlike most components in Rio, `Spacer` does not have a `natural`
     size. Therefore it defaults to a width and height of `grow`, as that is how
     they're frequently used.
 
-    ## Example:
+    ## Example
 
     A minimal example of `Spacer` will be shown:
 
     ```python
     rio.Spacer(height=5)
     ```
     """
```

### Comparing `rio_ui-0.5.8/rio/components/stack.py` & `rio_ui-0.5.9/src/rio/components/stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 
     `Stacks` are similar to rows and columns, but they stack their children in
     the Z direction instead of the X or Y direction. In other words, the stack's
     children overlap each other, with the first one at the bottom, the second
     one above that, and so on.
 
 
-    ## Attributes:
+    ## Attributes
 
     `children`: The components to place in this `Stack`.
 
-    ## Example:
+    ## Example
 
     A minimal example of `Stack` will be shown. This example will create a stack
     of three icons, each with a different size and color. The first icon will be
     at the bottom, the second one above that, and the third one at the top:
 
     ```python
     rio.Stack(
```

### Comparing `rio_ui-0.5.8/rio/components/switch.py` & `rio_ui-0.5.9/src/rio/components/switch.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,24 +29,24 @@
     An input for `True` / `False` values.
 
     Switches allow the user to toggle between an "on" and an "off" state. They
     thus correspond to a Python `bool` value. Use them to allow the user to
     enable or disable certain features, or to select between two options.
 
 
-    ## Attributes:
+    ## Attributes
 
     `is_on`: Whether the switch is currently in the "on" state.
 
     `is_sensitive`: Whether the switch should respond to user input.
 
     `on_change`: Triggered when the user toggles the switch.
 
 
-    ## Example:
+    ## Example
 
     A minimal example of a `Switch` will be shown:
 
     ```python
     rio.Switch(is_on=True)
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/switcher.py` & `rio_ui-0.5.9/src/rio/components/switcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 
     A container which can switch between different components.
 
     A `Switcher` is a container which can switch between different components.
     It is commonly used to switch between different views or modes. The
     `content` attribute can be used to change the currently displayed component.
 
-    ## Attributes:
+    ## Attributes
 
     `content`: The currently displayed component.
 
 
-    ## Example:
+    ## Example
 
     A minimal example of a `Switcher` will be shown:
     TODO: check if this is the correct example
 
     ```python
     rio.Switcher(content=rio.Text("Hello, world!"))
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/switcher_bar.py` & `rio_ui-0.5.9/src/rio/components/switcher_bar.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     A bar of options which can be switched between.
 
     A `SwitcherBar` is a bar of options which can be switched between. It is
     commonly used to switch between different views or modes.
 
 
-    ## Attributes:
+    ## Attributes
 
     `values`: The list of values which can be selected.
 
     `names`: The list of names to display for each value. If `None`, the
         string representation of each value is used.
 
     `icons`: The list of icons to display for each value.
@@ -54,15 +54,15 @@
     `selected_value`: The currently selected value.
 
     `allow_none`: Whether the switcher bar can have no value selected.
 
     `on_change`: Triggered whenever the selected value changes.
 
 
-    ## Example:
+    ## Example
 
     A simple switcher bar with three options:
 
     ```python
     rio.SwitcherBar(
         values=[1, 2, 3],
         names=["A-SwitchName", "B-SwitchName", "C-SwitchName"],
@@ -95,17 +95,17 @@
                         rio.Image(
                             self.session.assets / "example.png",
                             width=10,
                             height=2,
                         ),
                         rio.Spacer(),
                         rio.SwitcherBar(
-                            # values are the page_urls, which are the same as the page_url
-                            # of the rio.Page instances, e.g.: rio.Page(page_url="first-page", ...)
-                            # rio.App -> rio.Page(page_url="first-page", ...) -> "first-page"
+                            # For the values, we'll use the URL segments of the
+                            # pages in the app. This makes it easy to navigate
+                            # to them.
                             values=["/", "first-page", "second-page"],
                             names=["Home", "First Page", "Second Page"],
                             selected_value=self.session.active_page_instances[0].page_url,
                             align_y=0.5,
                             color="primary",
                             on_change=self._on_change,
                         ),
```

### Comparing `rio_ui-0.5.8/rio/components/table.py` & `rio_ui-0.5.9/src/rio/components/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,22 +29,22 @@
 
     Tables are a way to display data in a grid, with rows and columns. They are
     very useful for displaying data that is naturally tabular, such as
     spreadsheets, databases, or CSV files. Tables can be sorted by clicking on
     the column headers.
 
 
-    ## Attributes:
+    ## Attributes
 
     `data`: The data to display.
 
     `show_row_numbers`: Whether to show row numbers on the left side of the table.
 
 
-    ## Example:
+    ## Example
 
     A simple table with some data:
 
     ```python
     rio.Table(
         data={
             "Name": ["Alice", "Bob", "Charlie"],
```

### Comparing `rio_ui-0.5.8/rio/components/text.py` & `rio_ui-0.5.9/src/rio/components/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,29 +24,29 @@
     commonly used components in Rio.
 
     While the text itself is unformatted, you can still control the style of
     the text using the `style` attribute. This allows you to change the font
     size, color, and more.
 
 
-    ## Attributes:
+    ## Attributes
 
     `text`: The text to display.
 
     `multiline`: Whether the text may be split into multiple lines if not
         enough space is available.
 
     `selectable`: Whether the text can be selected by the user.
 
     `style`: The style of the text. This can either be a `TextStyle` instance,
         or one of the built-in styles: `heading1`, `heading2`, `heading3`,
         `text` or `dim`.
 
 
-    ## Example:
+    ## Example
 
     A minimal example of a `Text` will be shown:
 
     ```python
     rio.Text("Hello, world!")
     ```
     """
```

### Comparing `rio_ui-0.5.8/rio/components/text_input.py` & `rio_ui-0.5.9/src/rio/components/text_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     A user-editable text field.
 
     `TextInput` allows the user to enter a short text. The text can either be
     shown in plain text, or hidden when used for passwords or other sensitive
     information.
 
 
-    ## Attributes:
+    ## Attributes
 
     `text`: The text currently entered by the user.
 
     `label`: A short text to display next to the text input.
 
     `prefix_text`: A short text to display before the text input. Useful for
             displaying currency symbols or other prefixed units.
@@ -64,15 +64,15 @@
     `on_change`: Triggered when the user changes the text.
 
     `on_confirm`: Triggered when the user explicitly confirms their input,
             such as by pressing the "Enter" key. You can use this to trigger
             followup actions, such as logging in or submitting a form.
 
 
-    ## Example:
+    ## Example
 
     A simple `TextInput` with a default value of "John Doe" and a label:
     Note: The value will not be updated if the user changes the value in the input field.
 
     ```python
     rio.TextInput(text="John Doe", label="Name")
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/theme_context_switcher.py` & `rio_ui-0.5.9/src/rio/components/theme_context_switcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,22 +21,22 @@
     A container which can switch between different components.
 
     A `ThemeContextSwitcher` is a container which can switch between different
     components. It is commonly used to switch between different themes. The
     `content` attribute can be used to change the currently displayed component.
 
 
-    ## Attributes:
+    ## Attributes
 
     `content`: The currently displayed component.
 
     `color`: The color of the switcher bar.
 
 
-    ## Example:
+    ## Example
 
     A minimal example of a `ThemeContextSwitcher` will be shown:
     TODO: check if this is the correct example
 
     ```python
     rio.ThemeContextSwitcher(content=rio.Button("Button"), color="secondary")
     ```
```

### Comparing `rio_ui-0.5.8/rio/components/tooltip.py` & `rio_ui-0.5.9/src/rio/components/tooltip.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,25 +19,25 @@
     A small pop-up window that appears when the user hovers over an element.
 
     `Tooltip` is a small pop-up window that appears when the user hovers over an
     element. It is commonly used to provide additional information about the
     element, such as a description or a hint.
 
 
-    ## Attributes:
+    ## Attributes
 
     `anchor`: The component to which the tooltip is anchored.
 
     `tip`: The text or component to display in the tooltip.
 
     `position`: The position of the tooltip relative to the anchor. It can be
         one of the following values: `left`, `top`, `right`, `bottom`.
 
 
-    ## Example:
+    ## Example
 
     A minimal example of a `Tooltip` will be shown:
 
     ```python
     rio.Tooltip(
         anchor=rio.Icon("material/info"),
         tip="This is a tooltip.",
```

### Comparing `rio_ui-0.5.8/rio/components/website.py` & `rio_ui-0.5.9/src/rio/components/website.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     """
     # Website
 
     Displays a website.
 
     `Website` takes a URL as input and displays that website in your app.
 
-    ## Attributes:
+    ## Attributes
 
         `url`: The URL of the website you want to display.
 
-    ## Example:
+    ## Example
 
     A minimal example of a `Website` will be shown:
 
     ```python
     rio.Website(url=rio.URL("https://www.example.com"))
     ```
     """
```

### Comparing `rio_ui-0.5.8/rio/dataclass.py` & `rio_ui-0.5.9/src/rio/dataclass.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/debug/client_side_debugger/component_details.py` & `rio_ui-0.5.9/src/rio/debug/client_side_debugger/component_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 from typing import *  # type: ignore
 
 import rio
+import rio.docs
 
 from ... import common
 
 
 class ComponentDetails(rio.Component):
     component_id: int
 
@@ -304,15 +305,15 @@
 
             add_cell("align_y", 2, True)
             add_cell(str(debug_details.get("align_y", "-")), 3, False)
             row_index += 1
 
         # Link to docs
         if type(target)._rio_builtin_:
-            docs_url = f"https://rio.dev/docs/{type(target).__name__.lower()}"
+            docs_url = rio.docs.documentation_url(type(target).__name__)
             link_color = self.session.theme.secondary_color
 
             result.add(
                 rio.Link(
                     rio.Row(
                         rio.Icon("material/library-books", fill=link_color),
                         rio.Text("Docs", style=rio.TextStyle(fill=link_color)),
```

### Comparing `rio_ui-0.5.8/rio/debug/client_side_debugger/debugger.py` & `rio_ui-0.5.9/src/rio/debug/client_side_debugger/debugger.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/debug/client_side_debugger/deploy_page.py` & `rio_ui-0.5.9/src/rio/debug/client_side_debugger/deploy_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/debug/client_side_debugger/docs_page.py` & `rio_ui-0.5.9/src/rio/debug/client_side_debugger/docs_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/debug/client_side_debugger/icons_page.py` & `rio_ui-0.5.9/src/rio/debug/client_side_debugger/icons_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/debug/client_side_debugger/layout_preview.py` & `rio_ui-0.5.9/src/rio/debug/client_side_debugger/layout_preview.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/debug/client_side_debugger/project_page.py` & `rio_ui-0.5.9/src/rio/debug/client_side_debugger/project_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/debug/client_side_debugger/sample_icons_grid.py` & `rio_ui-0.5.9/src/rio/debug/client_side_debugger/sample_icons_grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/debug/client_side_debugger/theme_picker_page.py` & `rio_ui-0.5.9/src/rio/debug/client_side_debugger/theme_picker_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/debug/client_side_debugger/tree_page.py` & `rio_ui-0.5.9/src/rio/debug/client_side_debugger/tree_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/debug/monkeypatches.py` & `rio_ui-0.5.9/src/rio/debug/monkeypatches.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/debug/typing_utils.py` & `rio_ui-0.5.9/src/rio/debug/typing_utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/debug/validator.py` & `rio_ui-0.5.9/src/rio/debug/validator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/docs/custom.py` & `rio_ui-0.5.9/src/rio/docs/custom.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 Contains processing specific to the RIO project.
 """
 
+import dataclasses
 from typing import *  # type: ignore
 
 import imy.docstrings
 
 import rio
 
 
-def find_items_needing_documentation() -> Iterable[Type | Callable]:
+def find_objects_possibly_needing_documentation() -> Iterable[Type | Callable]:
     """
     Find all classes and functions in `Rio` that need to be documented.
     """
 
     # Hardcoded items
     yield rio.App
     yield rio.AssetError
@@ -89,15 +90,18 @@
 
     # Strip internal attributes
     index = 0
     while index < len(docs.attributes):
         attr = docs.attributes[index]
 
         # Decide whether to keep it
-        keep = not attr.name.startswith("_")
+        keep = True
+
+        keep = keep and not attr.name.startswith("_")
+        keep = keep and attr.type is not dataclasses.KW_ONLY
 
         # Strip it out, if necessary
         if keep:
             index += 1
         else:
             del docs.attributes[index]
```

### Comparing `rio_ui-0.5.8/rio/errors.py` & `rio_ui-0.5.9/src/rio/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class AssetError(Exception):
     """
     Raised when an error occurs related to assets.
 
     Signifies that some operation related to assets has failed. E.g. trying to
     access a nonexistent asset.
 
-    Attributes:
+    ## Attributes
         message: A human-readable error message.
     """
 
     def __init__(self, message: str):
         super().__init__(message)
 
     @property
```

### Comparing `rio_ui-0.5.8/rio/event.py` & `rio_ui-0.5.9/src/rio/event.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/fills.py` & `rio_ui-0.5.9/src/rio/fills.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 class SolidFill(Fill):
     """
     Fills a shape with a single color.
 
     `SolidFill` is the simplest of all fills. It fills the entire shape with a
     single, solid color.
 
-    Attributes:
+    ## Attributes
         color: The color to fill the shape with.
     """
 
     color: Color
 
     def _serialize(self, sess: rio.Session) -> Jsonable:
         return {
@@ -79,15 +79,15 @@
 
     `LinearGradientFill` fills the shape with a linear gradient. The gradient
     can have any number of stops, each with a color and a position. The gradient
     will smoothly transition between the colors at the given positions. The
     positions are given as are given as fractions, where 0 is the start of the
     gradient and 1 is the end.
 
-    Attributes:
+    ## Attributes
         stops: The different colors that comprise the gradient, along with where
             they are positioned.
 
             The stops are given as tuples. Each tuple contains a color and a
             position. The position is a fraction, where 0 is the start of the
             gradient and 1 is the end.
```

### Comparing `rio_ui-0.5.8/rio/global_state.py` & `rio_ui-0.5.9/src/rio/global_state.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/icon_registry.py` & `rio_ui-0.5.9/src/rio/icon_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,18 +61,14 @@
         variant. If the name is syntactically invalid (e.g. too many slashes),
         raise an `AssetError`.
         """
         # Determine the icon set
         sections = icon_name.split("/")
 
         if len(sections) == 1:
-            raise ValueError(
-                f"Missing icon set in icon `{icon_name}`"
-            )  # TODO: Decide on a default icon set
-
             icon_set = "material"
             icon_name = sections[0]
         elif len(sections) == 2:
             icon_set, icon_name = sections
         else:
             raise AssetError(
                 f"Invalid icon name `{icon_name}`. Icons names must be of the form `set/icon:variant`"
```

### Comparing `rio_ui-0.5.8/rio/inspection.py` & `rio_ui-0.5.9/src/rio/inspection.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/maybes.py` & `rio_ui-0.5.9/src/rio/maybes.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py` & `rio_ui-0.5.9/src/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py` & `rio_ui-0.5.9/src/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py` & `rio_ui-0.5.9/src/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/routing.py` & `rio_ui-0.5.9/src/rio/routing.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,34 +29,36 @@
     import rio
 
     app = rio.App(
         build=lambda: rio.Column(
             rio.Text("Welcome to my page!"), rio.PageView(
                 width="grow", height="grow",
             ),
-        ), pages=[
+        ),
+        pages=[
             rio.Page(
-                "", build=lambda: rio.Text("This is the home page"),
-            ), rio.Page(
-                "subpage", build=lambda: rio.Text("This is a subpage"),
+                "Home", "", build=lambda: rio.Text("This is the home page"),
+            ),
+            rio.Page(
+                "Subpage", "subpage", build=lambda: rio.Text("This is a subpage"),
             ),
         ],
     )
 
     app.run_in_browser()
     ```
 
     This will display "This is the home page" when navigating to the root URL,
     but "This is a subpage" when navigating to "/subpage". Note that on both
     pages the text "Welcome to my page!" is displayed above the page content.
     That's because it's not part of the `PageView`.
 
     # TODO: Link to the routing/multipage how-to page
 
-    Attributes:
+    ## Attributes
         page_url: The URL segment at which this page should be displayed. For
             example, if this is "subpage", then the page will be displayed at
             "https://yourapp.com/subpage". If this is "", then the page will be
             displayed at the root URL.
 
         build: A callback that is called when this page is displayed. It should
             return a Rio component.
@@ -74,19 +76,19 @@
             logged in.
 
             The callback should return `None` if the user is allowed to access
             the page, or a string or `rio.URL` if the user should be redirected
             to a different page.
     """
 
+    name: str
     page_url: str
     build: Callable[[], rio.Component]
     _: KW_ONLY
-    name: str | None = None
-    icon: str | None = None
+    icon: str = "rio/logo:color"
     show_in_navigation = True
     children: list[Page] = field(default_factory=list)
     guard: (
         Callable[[rio.Session, tuple[rio.Page, ...]], None | rio.URL | str] | None
     ) = None
 
     def __post_init__(self) -> None:
```

### Comparing `rio_ui-0.5.8/rio/serialization.py` & `rio_ui-0.5.9/src/rio/serialization.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/session.py` & `rio_ui-0.5.9/src/rio/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,30 @@
         # Trigger a resync
         if synchronize:
             self._session._save_settings_soon()
 
     def add(self, value: Any) -> None:
         self._add(value, synchronize=True)
 
+    def remove(self, typ: type) -> None:
+        # Remove the attachment, propagating any `KeyError`
+        old_value = self._attachments.pop(typ)
+
+        # User settings need special care
+        if not isinstance(old_value, user_settings_module.UserSettings):
+            return
+
+        # Unlink the value from the session
+        old_value._rio_session_ = None
+
+        # Trigger a resync
+        #
+        # TODO: `_save_settings_soon` doesn't currently delete any settings
+        self._session._save_settings_soon()
+
 
 class Session(unicall.Unicall):
     """
     Represents a single client connection to the app.
 
     A session corresponds to a single connection to a client. It maintains all
     state related to this client including local settings, the currently active
@@ -341,14 +357,34 @@
     def __getitem__(self, typ: type[T]) -> T:
         """
         Retrieves an attachment from this session. To attach values to the
         session, use `Session.attach`.
         """
         return self._attachments[typ]
 
+    def __delete__(self, typ: type) -> None:
+        """
+        Removes an attachment from this session.
+
+        ## Raises
+
+        `KeyError`: If no attachment of this type is attached to the session.
+        """
+        self._attachments.remove(typ)
+
+    def detach(self, typ: type) -> None:
+        """
+        Removes an attachment from this session.
+
+        ## Raises
+
+        `KeyError`: If no attachment of this type is attached to the session.
+        """
+        self._attachments.remove(typ)
+
     def close(self) -> None:
         """
         Ends the session, closing any window or browser tab.
         """
         self.create_task(self._close(True))
 
     async def _close(self, close_remote_session: bool) -> None:
```

### Comparing `rio_ui-0.5.8/rio/snippets/README.md` & `rio_ui-0.5.9/src/rio/snippets/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/__init__.py` & `rio_ui-0.5.9/src/rio/snippets/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/other-examples/simple_counter_app.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/other-examples/simple_counter_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 # </build>
 # </counter>
 
 
 # <app>
 app = rio.App(
     pages=[
-        rio.Page("", Counter),
+        rio.Page("Home", "", Counter),
     ],
 )
 # </app>
 
 # <run>
 app.run_in_browser()
 # </run>
```

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/README.md` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,20 +25,20 @@
     """
 
     # The entire message history
     messages: List[ChatMessage] = field(default_factory=list)
 
     async def respond(self, client: openai.AsyncOpenAI) -> ChatMessage:
         """
-        Creates an AI generated response for this conversation and appends it
-        to the messages list. Also returns the new message.
+          Creates an AI generated response for this conversation and appends it
+          to the messages list. Also returns the new message.
 
         ## Raises
 
-        `ValueError` if the most recent message is not by the user.
+          `ValueError` if the most recent message is not by the user.
         """
 
         # Make sure the last message was by the user
         if not self.messages or self.messages[-1].role != "user":
             raise ValueError("The most recent message must be by the user")
 
         # Convert all messages to the format needed by the API
```

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     These sections include a balance section displaying the total balance and the percentual
     difference in balance, and a bar chart section displaying a bar chart with a given color
     and hidden axes.
 
     The build method combines these sections into a single rio.Card component, creating a
     complete balance component for the dashboard.
 
-    Attributes:
+    ## Attributes
         data: A pandas DataFrame containing the data for the coins in MY_COINS.
     """
 
     data: pd.DataFrame
 
     def total_balance(self, idx: int) -> float:
         """
```

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import dataclasses
 from pathlib import Path
 from typing import *  # type:ignore
 
-import numpy as np
 
 # <additional-imports>
+import numpy as np
 import pandas as pd
 from pycoingecko import CoinGeckoAPI
 
 import rio
 
 from .. import components as comps
 from .. import data_models
@@ -44,15 +44,15 @@
 
     ###################################################
     #            BalanceCard        # CryptoCard(BTC) #
     #           Crypto Chart        # CryptoCard(LTC) #
     #          (Crypto Chart)       # CryptoCard(ETH) #
     ###################################################
 
-    Attributes:
+    ## Attributes
         coin_data: A pandas DataFrame that holds the historical data of three cryptocurrencies:
             Bitcoin, Litecoin, and Ethereum.
     """
 
     coin_data: pd.DataFrame = dataclasses.field(
         default=pd.DataFrame(
             {
```

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/README.md` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
     A component for editing a menu item.
 
     Returns a card component containing the menu item editor. The editor contains fields
     for name, description, price, and category of the menu item. The component also contains
     buttons for saving or canceling the changes.
 
-    Attributes:
+    ## Attributes
         currently_selected_menu_item: The currently selected menu item.
         new_entry: A boolean flag indicating if the menu item is a new entry.
         on_cancel_event: An event handler for the cancel button.
         on_save_event: An event handler for the save button.
     """
 
     currently_selected_menu_item: data_models.MenuItems
```

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class ItemList(rio.Component):
     """
     A component for displaying a list of menu items.
 
     Returns a list of menu items in a ListView component. Each item in the list contains the name,
     description, and a delete button. The delete button triggers an event to delete the item.
 
-    Attributes:
+    ## Attributes
         menu_item_set: The list of menu items to be displayed.
         on_add_new_item_event: An event handler for adding a new item.
         on_delete_item_event: An event handler for deleting an item.
         on_select_item_event: An event handler for selecting an item.
     """
 
     menu_item_set: list[data_models.MenuItems]
```

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 @dataclass
 class MenuItems:
     """
     MenuItems data model.
 
-    Attributes:
+    ## Attributes
         name: The name of the menu item.
         description: The description of the menu item.
         price: The price of the menu item.
         category: The category of the menu item.
     """
 
     name: str
```

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     The @rio.event.on_populate decorator is used to fetch data from a predefined data model and assign it to the
     menu_item_set attribute of the current instance. The on_press_delete_item, on_press_cancel_event, and
     on_press_save_event methods are used to handle delete, cancel, and save events, respectively. The on_press_add_new_item
     method is used to handle the add new item event. The on_press_select_menu_item method is used to handle the selection
     of a menu item.
 
-    Attributes:
+    ## Attributes
         menu_item_set: A list of menu items.
         currently_selected_menu_item: The currently selected menu item.
         banner_text: The text to be displayed in the banner.
         banner_style: The style of the banner (success, danger, info).
         is_new_entry: A flag to indicate if the currently selected menu item is a new entry.
     """
```

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py` & `rio_ui-0.5.9/src/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/state_properties.py` & `rio_ui-0.5.9/src/rio/state_properties.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/text_style.py` & `rio_ui-0.5.9/src/rio/text_style.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/theme.py` & `rio_ui-0.5.9/src/rio/theme.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/user_settings_module.py` & `rio_ui-0.5.9/src/rio/user_settings_module.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/rio/world_units.py` & `rio_ui-0.5.9/src/rio/world_units.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.8/PKG-INFO` & `rio_ui-0.5.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,56 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: rio-ui
-Version: 0.5.8
+Version: 0.5.9
 Summary: Build modern Websites and Apps just with Python
-Home-page: https://rio.dev
+Project-URL: homepage, https://rio.dev
+Project-URL: documentation, https://rio.dev/docs
+Author: Paul Pinterits
+Author-email: Jakob Pinterits <jakob.pinterits@gmail.com>
 License: LGPL-3.0
-Keywords: web-development,web-framework,framework,functional,type-safe,typing,typed,react,web,app,user-interface,web-app,local-app,modern,rio
-Author: Jakob Pinterits
-Author-email: jakob.pinterits@gmail.com
-Requires-Python: >=3.10,<4.0
+License-File: LICENSE.txt
+Keywords: app,framework,functional,local-app,modern,react,rio,type-safe,typed,typing,user-interface,web,web-app,web-development,web-framework
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.10
+Requires-Dist: aiofiles~=23.2.1
+Requires-Dist: fastapi~=0.110
+Requires-Dist: fuzzywuzzy~=0.18.0
+Requires-Dist: gitignore-parser~=0.1.9
+Requires-Dist: httpx~=0.25.1
+Requires-Dist: imy~=0.2.4
+Requires-Dist: introspection~=1.7.14
+Requires-Dist: isort~=5.13.2
+Requires-Dist: keyring~=24.3.0
+Requires-Dist: pillow~=10.2.0
+Requires-Dist: pytest~=7.3.1
+Requires-Dist: python-levenshtein~=0.23.0
+Requires-Dist: python-multipart~=0.0.6
+Requires-Dist: pytz~=2024.1
+Requires-Dist: revel~=0.9.0
+Requires-Dist: timer-dict~=1.0.0
+Requires-Dist: tomlkit~=0.12.3
+Requires-Dist: typing-extensions>=4.5.0
+Requires-Dist: unicall~=0.1.5
+Requires-Dist: uniserde~=0.3.12
+Requires-Dist: uvicorn[standard]~=0.23.2
+Requires-Dist: watchfiles~=0.21.0
+Requires-Dist: yarl~=1.9.2
 Provides-Extra: window
-Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
-Requires-Dist: cefpython3 (>=66.1,<67.0) ; (sys_platform == "windows") and (extra == "window")
-Requires-Dist: fastapi (>=0.109.1,<0.110.0)
-Requires-Dist: fuzzywuzzy (>=0.18.0,<0.19.0)
-Requires-Dist: gitignore-parser (>=0.1.9,<0.2.0)
-Requires-Dist: httpx (>=0.25.1,<0.26.0)
-Requires-Dist: imy (>=0.2.3,<0.3.0)
-Requires-Dist: introspection (>=1.7.14,<2.0.0)
-Requires-Dist: isort (>=5.13.2,<6.0.0)
-Requires-Dist: keyring (>=24.3.0,<25.0.0)
-Requires-Dist: pillow (>=10.2.0,<11.0.0)
-Requires-Dist: platformdirs (>=3.11.0,<4.0.0) ; extra == "window"
-Requires-Dist: pygobject (>=3.44.1,<4.0.0) ; (sys_platform == "linux") and (extra == "window")
-Requires-Dist: pytest (>=7.3.1,<8.0.0)
-Requires-Dist: python-levenshtein (>=0.23.0,<0.24.0)
-Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
-Requires-Dist: pytz (>=2024.1,<2025.0)
-Requires-Dist: pywebview (>=4.2.2,<5.0.0) ; extra == "window"
-Requires-Dist: revel (>=0.9.0,<0.10.0)
-Requires-Dist: timer-dict (>=1.0.0,<2.0.0)
-Requires-Dist: tomlkit (>=0.12.3,<0.13.0)
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
-Requires-Dist: unicall (>=0.1.5,<0.2.0)
-Requires-Dist: uniserde (>=0.3.12,<0.4.0)
-Requires-Dist: uvicorn[standard] (>=0.23.2,<0.24.0)
-Requires-Dist: watchfiles (>=0.21.0,<0.22.0)
-Requires-Dist: yarl (>=1.9.2,<2.0.0)
-Project-URL: Documentation, https://rio.dev/docs
+Requires-Dist: cefpython3~=66.1; (sys_platform == 'win32') and extra == 'window'
+Requires-Dist: platformdirs~=3.11.0; extra == 'window'
+Requires-Dist: pygobject~=3.44.1; (sys_platform == 'linux') and extra == 'window'
+Requires-Dist: pywebview~=4.2.2; extra == 'window'
 Description-Content-Type: text/markdown
 
 ![Rio](https://img.shields.io/badge/Rio-outline.svg?color=%2311e8e3e&link=https%3A%2F%2Frio.dev&style=flat-square&logo=data:image/svg%2bxml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgd2lkdGg9IjEwMDIuMTA1IgogICBoZWlnaHQ9IjE0OTkuODA1NyIKICAgdmlld0JveD0iMCAwIDI2NS4xNDAyOSAzOTYuODIzNTkiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2Zzg5NiIKICAgeG1sOnNwYWNlPSJwcmVzZXJ2ZSIKICAgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpzdmc9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpyZGY9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkvMDIvMjItcmRmLXN5bnRheC1ucyMiCiAgIHhtbG5zOmNjPSJodHRwOi8vY3JlYXRpdmVjb21tb25zLm9yZy9ucyMiCiAgIHhtbG5zOmRjPSJodHRwOi8vcHVybC5vcmcvZGMvZWxlbWVudHMvMS4xLyI+PGRlZnMKICAgICBpZD0iZGVmczg5MCIgLz48bWV0YWRhdGEKICAgICBpZD0ibWV0YWRhdGE4OTMiPjxyZGY6UkRGPjxjYzpXb3JrCiAgICAgICAgIHJkZjphYm91dD0iIj48ZGM6Zm9ybWF0PmltYWdlL3N2Zyt4bWw8L2RjOmZvcm1hdD48ZGM6dHlwZQogICAgICAgICAgIHJkZjpyZXNvdXJjZT0iaHR0cDovL3B1cmwub3JnL2RjL2RjbWl0eXBlL1N0aWxsSW1hZ2UiIC8+PC9jYzpXb3JrPjwvcmRmOlJERj48L21ldGFkYXRhPjxnCiAgICAgaWQ9ImxheWVyMSIKICAgICB0cmFuc2Zvcm09InRyYW5zbGF0ZSgyNi40MTM4NDcsNTAuMjcxMzUpIj48cGF0aAogICAgICAgaWQ9InBhdGgxIgogICAgICAgc3R5bGU9ImZpbGw6I2ZmZmZmZjtmaWxsLW9wYWNpdHk6MTtzdHJva2Utd2lkdGg6MC4yNjQ1ODMiCiAgICAgICBkPSJtIC04LjgwMzA4MDMsLTUwLjI3MTM1IGMgLTE1LjI3NjU1OTcsMC44NjA1MjQgLTE4LjYzMTgzNDcsMTcuNTQ0NTEyIC0xNy4zNjc0MTU3LDI5Ljk2ODk1MiAwLjUxMzcyNywxNi4yNDQxNjYxIC0xLjIxMzE5NywzMi43MTkyOTcgMS4yNjg1MTcsNDguNzY2NzkzIDguMTQxMTg1LDE0LjcxMDAxMiAyNi4wNzc2NzYxLDE4Ljg0OTk3MiAzOS44Nzc0ODIsMjYuNzcwMTM0IDMwLjM3ODk2MiwxNS4wNjY1NSA2MC43NTc5MjUsMzAuMTMzMTAxIDkxLjEzNjg4Nyw0NS4xOTk2NTEgLTM0LjgyMjM5OCwxNy42MDY2OCAtNzAuMjI2MTE3LDM0LjE0NzgzIC0xMDQuNjYwNTA2OCw1Mi40NjUyOCAtMjAuMDM3Nzc1MiwxMS40ODE0NCAtMzQuNzc4MTg3MiwzNi45NjY5OCAtMjQuMTAxMTk2Miw1OS41OTIxMSAxMS4yOTkzMSwyNS42MDQ3IDM5Ljc0MjkxMSwzMy43MTY5NSA2Mi40NzIyMDgsNDUuOTY4MDIgNTguOTU5MTAzLDI5LjA5NDExIDExNy43MTA1MzUsNTguNjQ4NDIgMTc2Ljc4OTE1NSw4Ny40NzU2IDE0LjA2MTIxLDMuOTY4MzYgMjQuMDM2NzYsLTEyLjAyMzEgMjEuODAwNzksLTI0LjUzMjIgLTAuNTQyODUsLTE3LjgzMTU3IDEuMjU4MTYsLTM1LjkwMjkyIC0xLjI2ODM2LC01My41MzY0OCAtOC4xNDA2MywtMTQuNzEwNzEgLTI2LjA3NjkyLC0xOC44NTE5OCAtMzkuODc3MTksLTI2Ljc3MTcyIC0zMC4zNzYwNiwtMTUuMDcxMTUgLTYwLjgwMDczLC0zMC4xNDExNyAtOTEuMTQ2NDIsLTQ1LjIxMzA0IDM0LjUwODc5LC0xNy4zNzM3NyA2OS40NTU5NywtMzMuOTI1NjUgMTAzLjY3Mjk4LC01MS44NDY2MyAyMC4xOTUxMywtMTEuMDA2MjggMzUuMzg2NDQsLTM2LjMwMDA1IDI1LjYwMzM4LC01OC45ODA5NCBDIDIyNC43MDYyMyw1OC44NzI1MzQgMTk2LjA1MDY3LDUwLjQ4NjY0MSAxNzMuMTY3MjYsMzguMjM4MTkxIDE1MS4xOTIyNiwyNy4zNDkyOTUgMTI2LjI0NjM5LDE0LjkzOTYzOCAxMDYuMTIxMTcsNC45OTc2Mjc4IDcwLjA0MTcxOSwtMTIuODk5Mjk5IDMzLjk2MjI2OCwtMzAuNzk2MjI1IC0yLjExNzE4MzQsLTQ4LjY5MzE1MiBsIC0zLjM3MjY3NzcsLTEuMjE4NDkyIHoiIC8+PC9nPjwvc3ZnPgo=)
 ![Version](https://img.shields.io/pypi/v/rio-ui?color=%2311e8e3e&style=flat-square)
 ![Discord](https://img.shields.io/discord/1213589765484576818?color=%2311e8e3e&label=discord&style=flat-square)
 ![Python Version](https://img.shields.io/pypi/pyversions/rio-ui?style=flat-square)
 ![License](https://img.shields.io/pypi/l/rio-ui?color=%2311e8e3e&style=flat-square)
@@ -74,20 +71,20 @@
 Rio brings React-style components to Python. Pull from a wealth of built-in
 components and combine them to create your own custom components. Then combine
 those into entire apps. Best of all, Rio apps can run both locally on your
 machine and on the web.
 
 ## Features 🧩
 
-- Modern, **declarative UI** framework
-- **100% Python** - Zero HTML, CSS, or JavaScript required
-- Over **50 Built-in components** for common UI elements, such as `rio.Switch`, `rio.Button`, and `rio.Text`, and many more
-- Integrates with **modern Python tooling**: Thanks to being **entirely Type Safe** editors can give you instant suggestions and highlight problems right away
-- Apps can run **both locally and on the web**
-- **Open Source & Free forever**
+-   Modern, **declarative UI** framework
+-   **100% Python** - Zero HTML, CSS, or JavaScript required
+-   Over **50 Built-in components** for common UI elements, such as `rio.Switch`, `rio.Button`, and `rio.Text`, and many more
+-   Integrates with **modern Python tooling**: Thanks to being **entirely Type Safe** editors can give you instant suggestions and highlight problems right away
+-   Apps can run **both locally and on the web**
+-   **Open Source & Free forever**
 
 ## Installation 🛠️
 
 Rio is available on PyPI, so you can install it using pip:
 
 ```bash
 pip install rio-ui
@@ -100,15 +97,15 @@
 ```bash
 rio new
 ```
 
 You can choose from a variety of built-in templates to get you started. Here's a complete example to create a project based on the tic-tac-toe template:
 
 ```bash
-rio new my-app --type website --template "Tic-Tac-Toe"
+rio new my-project --type website --template "Tic-Tac-Toe"
 cd my-project
 rio run
 ```
 
 You'll have your first app up and running in seconds!
 
 ## How it works 🧠
@@ -120,15 +117,14 @@
 import rio
 from openai import AsyncOpenAI
 
 client = AsyncOpenAI()
 
 
 class DallEPage(rio.Component):
-
     prompt: str = ""
     image_url: str = ""
     is_loading: bool = False
 
     async def get_image(self) -> None:
         """Get an image by prompt."""
 
@@ -191,24 +187,23 @@
         )
 
 
 # Run the app
 app = rio.App(
     pages=[
         rio.Page(
+            name="Home",
             page_url="",
             build=DallEPage,
         ),
     ],
 )
+```
 
 ## Status: In Development 🚧
 
 Rio is still in development. We're working hard to bring you the best possible
-experience. If you have any feedback, please let us know on our Discord server.
+experience. If you have any feedback, please let us know on [our Discord server](https://discord.gg/7ejXaPwhyH).
 
 ## Contributing 🤝
 
-Write how someone can contribute to the project. :)
-
-```
-
+TODO: Write how someone can contribute to the project. :)
```

