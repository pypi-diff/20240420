# Comparing `tmp/tdf_tool-2.4.6.tar.gz` & `tmp/tdf_tool-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdf_tool-2.4.6.tar", max compression
+gzip compressed data, was "tdf_tool-2.4.7.tar", max compression
```

## Comparing `tdf_tool-2.4.6.tar` & `tdf_tool-2.4.7.tar`

### file list

```diff
@@ -1,164 +1,165 @@
--rw-r--r--   0        0        0     1068 2024-04-16 07:59:17.944743 tdf_tool-2.4.6/LICENSE
--rw-r--r--   0        0        0     9217 2024-04-16 07:59:17.944961 tdf_tool-2.4.6/README.md
--rw-r--r--   0        0        0     1608 2024-04-18 09:24:38.197320 tdf_tool-2.4.6/pyproject.toml
--rw-r--r--   0        0        0      321 2024-04-16 07:59:17.947227 tdf_tool-2.4.6/tdf_tool/app.py
--rw-r--r--   0        0        0     1106 2024-04-18 09:15:16.438690 tdf_tool-2.4.6/tdf_tool/pipeline.py
--rw-r--r--   0        0        0     8469 2024-04-17 06:16:22.770116 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc
--rw-r--r--   0        0        0     4497 2024-04-18 09:17:23.331958 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc
--rw-r--r--   0        0        0     7153 2024-04-18 09:13:55.372125 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc
--rw-r--r--   0        0        0      424 2024-04-16 07:59:17.947648 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/cmd.cpython-39.pyc
--rw-r--r--   0        0        0     2567 2024-04-16 07:59:17.947827 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc
--rw-r--r--   0        0        0     1676 2024-04-18 09:17:23.336387 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc
--rw-r--r--   0        0        0     2668 2024-04-16 07:59:17.948134 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc
--rw-r--r--   0        0        0     1619 2024-04-18 09:17:23.343761 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc
--rw-r--r--   0        0        0      496 2024-04-16 07:59:17.948441 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/init.cpython-39.pyc
--rw-r--r--   0        0        0     3015 2024-04-16 07:59:17.948597 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc
--rw-r--r--   0        0        0     2292 2024-04-18 09:24:25.297275 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc
--rw-r--r--   0        0        0     2981 2024-04-16 07:59:17.948929 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc
--rw-r--r--   0        0        0     2243 2024-04-18 09:17:23.340691 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc
--rw-r--r--   0        0        0    36213 2024-04-16 07:59:17.949402 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc
--rw-r--r--   0        0        0    16242 2024-04-17 09:18:30.993839 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc
--rw-r--r--   0        0        0     3262 2024-04-16 07:59:17.950144 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc
--rw-r--r--   0        0        0     1989 2024-04-18 09:17:23.215708 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc
--rw-r--r--   0        0        0      817 2024-04-16 07:59:17.950609 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc
--rw-r--r--   0        0        0      621 2024-04-17 03:42:57.704141 tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc
--rw-r--r--   0        0        0     5130 2024-04-18 09:17:19.625035 tdf_tool-2.4.6/tdf_tool/pipelines/annotation.py
--rw-r--r--   0        0        0     7388 2024-04-18 09:13:44.982922 tdf_tool-2.4.6/tdf_tool/pipelines/api_interaction.py
--rw-r--r--   0        0        0     1244 2024-04-18 09:17:03.333227 tdf_tool-2.4.6/tdf_tool/pipelines/fix_header.py
--rw-r--r--   0        0        0     1211 2024-04-18 09:16:07.773291 tdf_tool-2.4.6/tdf_tool/pipelines/git.py
--rw-r--r--   0        0        0     1889 2024-04-18 09:24:14.030083 tdf_tool-2.4.6/tdf_tool/pipelines/module.py
--rw-r--r--   0        0        0     1630 2024-04-18 09:16:33.493718 tdf_tool-2.4.6/tdf_tool/pipelines/package.py
--rw-r--r--   0        0        0    22055 2024-04-17 08:02:42.463284 tdf_tool-2.4.6/tdf_tool/pipelines/router.py
--rw-r--r--   0        0        0     1656 2024-04-18 09:16:44.448736 tdf_tool-2.4.6/tdf_tool/pipelines/translate.py
--rw-r--r--   0        0        0      179 2024-04-16 07:59:17.952763 tdf_tool-2.4.6/tdf_tool/pipelines/upgrade.py
--rw-r--r--   0        0        0     1653 2024-04-16 07:59:17.953204 tdf_tool-2.4.6/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc
--rw-r--r--   0        0        0     1064 2024-04-17 03:42:57.428644 tdf_tool-2.4.6/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc
--rw-r--r--   0        0        0    10270 2024-04-16 07:59:17.953777 tdf_tool-2.4.6/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc
--rw-r--r--   0        0        0     5149 2024-04-17 03:42:57.424677 tdf_tool-2.4.6/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc
--rw-r--r--   0        0        0     1328 2024-04-16 07:59:17.954419 tdf_tool-2.4.6/tdf_tool/tools/__pycache__/env.cpython-311.pyc
--rw-r--r--   0        0        0      899 2024-04-17 03:42:57.430200 tdf_tool-2.4.6/tdf_tool/tools/__pycache__/env.cpython-39.pyc
--rw-r--r--   0        0        0     2480 2024-04-16 07:59:17.954948 tdf_tool-2.4.6/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc
--rw-r--r--   0        0        0     1464 2024-04-17 03:42:57.562167 tdf_tool-2.4.6/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc
--rw-r--r--   0        0        0     2969 2024-04-16 07:59:17.955456 tdf_tool-2.4.6/tdf_tool/tools/__pycache__/print.cpython-311.pyc
--rw-r--r--   0        0        0     2040 2024-04-17 03:42:57.419685 tdf_tool-2.4.6/tdf_tool/tools/__pycache__/print.cpython-39.pyc
--rw-r--r--   0        0        0     9661 2024-04-16 07:59:17.955984 tdf_tool-2.4.6/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc
--rw-r--r--   0        0        0     6181 2024-04-17 03:42:57.564741 tdf_tool-2.4.6/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc
--rw-r--r--   0        0        0    10739 2024-04-16 07:59:17.956576 tdf_tool-2.4.6/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc
--rw-r--r--   0        0        0     5620 2024-04-17 07:17:19.963646 tdf_tool-2.4.6/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc
--rw-r--r--   0        0        0    11432 2024-04-16 07:59:17.957426 tdf_tool-2.4.6/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc
--rw-r--r--   0        0        0     7694 2024-04-17 03:42:57.185360 tdf_tool-2.4.6/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc
--rw-r--r--   0        0        0     7216 2024-04-16 07:59:17.958050 tdf_tool-2.4.6/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc
--rw-r--r--   0        0        0     4018 2024-04-17 03:42:57.112957 tdf_tool-2.4.6/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc
--rw-r--r--   0        0        0     1835 2024-04-17 03:42:57.418130 tdf_tool-2.4.6/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc
--rw-r--r--   0        0        0     1628 2024-04-16 07:59:17.959126 tdf_tool-2.4.6/tdf_tool/tools/cli/bean/deps_item.py
--rw-r--r--   0        0        0    12287 2024-04-16 07:59:17.959442 tdf_tool-2.4.6/tdf_tool/tools/cli/module_deps_rewrite.py
--rw-r--r--   0        0        0     5041 2024-04-16 07:59:17.959734 tdf_tool-2.4.6/tdf_tool/tools/cli/project_cli.py
--rw-r--r--   0        0        0     1919 2024-04-17 03:42:57.421774 tdf_tool-2.4.6/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc
--rw-r--r--   0        0        0     1833 2024-04-16 07:59:17.960396 tdf_tool-2.4.6/tdf_tool/tools/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      559 2024-04-16 07:59:17.960648 tdf_tool-2.4.6/tdf_tool/tools/cmd.py
--rw-r--r--   0        0        0     7002 2024-04-16 07:59:17.961174 tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     3385 2024-04-17 03:42:57.474812 tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0     2717 2024-04-16 07:59:17.961718 tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc
--rw-r--r--   0        0        0     1491 2024-04-17 07:06:18.116707 tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc
--rw-r--r--   0        0        0     2693 2024-04-16 07:59:17.962260 tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc
--rw-r--r--   0        0        0     2732 2024-04-16 07:59:17.962513 tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc
--rw-r--r--   0        0        0     2103 2024-04-17 09:18:30.887998 tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc
--rw-r--r--   0        0        0     9155 2024-04-16 07:59:17.963058 tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc
--rw-r--r--   0        0        0     4496 2024-04-17 03:42:57.689464 tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc
--rw-r--r--   0        0        0     3983 2024-04-16 07:59:17.963572 tdf_tool-2.4.6/tdf_tool/tools/config/config.py
--rw-r--r--   0        0        0     1310 2024-04-17 07:03:28.545530 tdf_tool-2.4.6/tdf_tool/tools/config/initial_json_config.py
--rw-r--r--   0        0        0     1267 2024-04-17 09:14:57.974794 tdf_tool-2.4.6/tdf_tool/tools/config/module_json_config.py
--rw-r--r--   0        0        0     5593 2024-04-16 07:59:17.964325 tdf_tool-2.4.6/tdf_tool/tools/config/packages_config.py
--rw-r--r--   0        0        0     7704 2024-04-16 07:59:17.964588 tdf_tool-2.4.6/tdf_tool/tools/dependencies_analysis.py
--rw-r--r--   0        0        0      662 2024-04-16 07:59:17.964838 tdf_tool-2.4.6/tdf_tool/tools/env.py
--rw-r--r--   0        0        0     6312 2024-04-16 07:59:17.965341 tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc
--rw-r--r--   0        0        0     3616 2024-04-17 03:42:57.693573 tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc
--rw-r--r--   0        0        0     3174 2024-04-16 07:59:17.965839 tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc
--rw-r--r--   0        0        0     2004 2024-04-17 03:42:57.692103 tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc
--rw-r--r--   0        0        0     4314 2024-04-16 07:59:17.966355 tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc
--rw-r--r--   0        0        0     2464 2024-04-17 03:42:57.694912 tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc
--rw-r--r--   0        0        0     6437 2024-04-16 07:59:17.966902 tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc
--rw-r--r--   0        0        0     3681 2024-04-17 03:42:57.696791 tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc
--rw-r--r--   0        0        0     2422 2024-04-16 07:59:17.967708 tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc
--rw-r--r--   0        0        0     3345 2024-04-16 07:59:17.967959 tdf_tool-2.4.6/tdf_tool/tools/fix_header/fix_header_entry.py
--rw-r--r--   0        0        0     1586 2024-04-16 07:59:17.968270 tdf_tool-2.4.6/tdf_tool/tools/fix_header/fix_header_lint.py
--rw-r--r--   0        0        0     2137 2024-04-16 07:59:17.968589 tdf_tool-2.4.6/tdf_tool/tools/fix_header/fix_header_lint_tool.py
--rw-r--r--   0        0        0     4095 2024-04-16 07:59:17.968850 tdf_tool-2.4.6/tdf_tool/tools/fix_header/fix_header_replace_tool.py
--rw-r--r--   0        0        0     1159 2024-04-16 07:59:17.969195 tdf_tool-2.4.6/tdf_tool/tools/flutter_script.py
--rw-r--r--   0        0        0     7243 2024-04-16 07:59:17.969845 tdf_tool-2.4.6/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc
--rw-r--r--   0        0        0     4190 2024-04-17 03:42:57.549550 tdf_tool-2.4.6/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc
--rw-r--r--   0        0        0     7055 2024-04-16 07:59:17.970442 tdf_tool-2.4.6/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc
--rw-r--r--   0        0        0     3786 2024-04-17 03:42:57.477039 tdf_tool-2.4.6/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc
--rw-r--r--   0        0        0      593 2024-04-16 07:59:17.971051 tdf_tool-2.4.6/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc
--rw-r--r--   0        0        0     5019 2024-04-16 07:59:17.971732 tdf_tool-2.4.6/tdf_tool/tools/gitlab/gitlab_utils.py
--rw-r--r--   0        0        0     3814 2024-04-16 07:59:17.972085 tdf_tool-2.4.6/tdf_tool/tools/gitlab/python_gitlab_api.py
--rw-r--r--   0        0        0     2482 2024-04-16 07:59:17.972678 tdf_tool-2.4.6/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc
--rw-r--r--   0        0        0     1412 2024-04-17 03:42:57.472617 tdf_tool-2.4.6/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc
--rw-r--r--   0        0        0     1063 2024-04-16 07:59:17.973603 tdf_tool-2.4.6/tdf_tool/tools/module/module_tools.py
--rw-r--r--   0        0        0    11056 2024-04-16 07:59:17.974266 tdf_tool-2.4.6/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc
--rw-r--r--   0        0        0     5267 2024-04-17 03:42:57.700870 tdf_tool-2.4.6/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc
--rw-r--r--   0        0        0     9752 2024-04-16 07:59:17.974933 tdf_tool-2.4.6/tdf_tool/tools/package/seal_off_package_utils.py
--rw-r--r--   0        0        0      911 2024-04-16 07:59:17.975191 tdf_tool-2.4.6/tdf_tool/tools/platform_tools.py
--rw-r--r--   0        0        0     1226 2024-04-16 07:59:17.975485 tdf_tool-2.4.6/tdf_tool/tools/print.py
--rw-r--r--   0        0        0     7598 2024-04-16 07:59:17.975770 tdf_tool-2.4.6/tdf_tool/tools/regular_tool.py
--rw-r--r--   0        0        0     5718 2024-04-17 07:17:09.536594 tdf_tool-2.4.6/tdf_tool/tools/shell_dir.py
--rw-r--r--   0        0        0     3840 2024-04-16 07:59:17.976600 tdf_tool-2.4.6/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc
--rw-r--r--   0        0        0     2161 2024-04-17 03:42:57.656262 tdf_tool-2.4.6/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc
--rw-r--r--   0        0        0     2695 2024-04-16 07:59:17.977108 tdf_tool-2.4.6/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc
--rw-r--r--   0        0        0     1678 2024-04-17 03:42:57.681260 tdf_tool-2.4.6/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc
--rw-r--r--   0        0        0    11711 2024-04-16 07:59:17.977716 tdf_tool-2.4.6/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0     1999 2024-04-16 07:59:17.977961 tdf_tool-2.4.6/tdf_tool/tools/translate/file_util.py
--rw-r--r--   0        0        0    15484 2024-04-16 07:59:17.978545 tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc
--rw-r--r--   0        0        0     8285 2024-04-17 03:42:57.652286 tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc
--rw-r--r--   0        0        0    26818 2024-04-16 07:59:17.979344 tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc
--rw-r--r--   0        0        0    13427 2024-04-17 03:42:57.558963 tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0    10691 2024-04-16 07:59:17.980114 tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/flutter_translate_lint.py
--rw-r--r--   0        0        0    18954 2024-04-16 07:59:17.980464 tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/flutter_translate_tools.py
--rw-r--r--   0        0        0     8395 2024-04-16 07:59:17.981075 tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc
--rw-r--r--   0        0        0     4595 2024-04-17 03:42:57.654824 tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc
--rw-r--r--   0        0        0     5228 2024-04-16 07:59:17.981648 tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py
--rw-r--r--   0        0        0      859 2024-04-16 07:59:17.982222 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc
--rw-r--r--   0        0        0     7351 2024-04-16 07:59:17.982702 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc
--rw-r--r--   0        0        0     7599 2024-04-16 07:59:17.983077 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc
--rw-r--r--   0        0        0     4216 2024-04-17 03:42:57.658661 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc
--rw-r--r--   0        0        0     3952 2024-04-16 07:59:17.983786 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc
--rw-r--r--   0        0        0     2347 2024-04-17 03:42:57.682489 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc
--rw-r--r--   0        0        0      870 2024-04-16 07:59:17.984330 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc
--rw-r--r--   0        0        0     4766 2024-04-16 07:59:17.984706 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0     6219 2024-04-16 07:59:17.985086 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc
--rw-r--r--   0        0        0     2631 2024-04-16 07:59:17.985435 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc
--rw-r--r--   0        0        0     4438 2024-04-16 07:59:17.985774 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/ios_translate.py
--rw-r--r--   0        0        0     2000 2024-04-16 07:59:17.986154 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/ios_translate_lint.py
--rw-r--r--   0        0        0     5061 2024-04-16 07:59:17.986697 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc
--rw-r--r--   0        0        0     2852 2024-04-17 03:42:57.660758 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc
--rw-r--r--   0        0        0    17576 2024-04-16 07:59:17.987402 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc
--rw-r--r--   0        0        0     9306 2024-04-17 03:42:57.664711 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc
--rw-r--r--   0        0        0     7901 2024-04-16 07:59:17.988120 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc
--rw-r--r--   0        0        0     4398 2024-04-17 03:42:57.679975 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc
--rw-r--r--   0        0        0     1158 2024-04-16 07:59:17.988695 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc
--rw-r--r--   0        0        0     1028 2024-04-17 03:42:57.666587 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc
--rw-r--r--   0        0        0    10070 2024-04-16 07:59:17.989363 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc
--rw-r--r--   0        0        0     5366 2024-04-17 03:42:57.668957 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0     2773 2024-04-16 07:59:17.989983 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc
--rw-r--r--   0        0        0     2689 2024-04-17 03:42:57.675374 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc
--rw-r--r--   0        0        0    11353 2024-04-16 07:59:17.990542 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc
--rw-r--r--   0        0        0     6226 2024-04-17 03:42:57.678045 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc
--rw-r--r--   0        0        0     4943 2024-04-16 07:59:17.991277 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc
--rw-r--r--   0        0        0     2687 2024-04-17 03:42:57.671087 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc
--rw-r--r--   0        0        0     3270 2024-04-16 07:59:17.991799 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py
--rw-r--r--   0        0        0    14326 2024-04-16 07:59:17.992093 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/ios_module.py
--rw-r--r--   0        0        0     5223 2024-04-16 07:59:17.992380 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py
--rw-r--r--   0        0        0     1189 2024-04-16 07:59:17.992605 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py
--rw-r--r--   0        0        0     8191 2024-04-16 07:59:17.992866 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py
--rw-r--r--   0        0        0     2337 2024-04-16 07:59:17.993215 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/location_string_temp.py
--rw-r--r--   0        0        0     8684 2024-04-16 07:59:17.993505 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/podspec.py
--rw-r--r--   0        0        0     2886 2024-04-16 07:59:17.993759 tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/string_util.py
--rw-r--r--   0        0        0     8625 2024-04-16 07:59:17.994344 tdf_tool-2.4.6/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc
--rw-r--r--   0        0        0     5032 2024-04-17 03:42:57.673624 tdf_tool-2.4.6/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc
--rw-r--r--   0        0        0     5111 2024-04-16 07:59:17.994952 tdf_tool-2.4.6/tdf_tool/tools/translate/tools/translate_tool.py
--rw-r--r--   0        0        0     1408 2024-04-16 07:59:17.995250 tdf_tool-2.4.6/tdf_tool/tools/translate/translate_lint.py
--rw-r--r--   0        0        0     1268 2024-04-16 07:59:17.996782 tdf_tool-2.4.6/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc
--rw-r--r--   0        0        0      880 2024-04-17 03:42:57.551180 tdf_tool-2.4.6/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc
--rw-r--r--   0        0        0      440 2024-04-16 07:59:17.997353 tdf_tool-2.4.6/tdf_tool/tools/vscode/vscode.py
--rw-r--r--   0        0        0    11029 2024-04-18 09:24:43.938725 tdf_tool-2.4.6/setup.py
--rw-r--r--   0        0        0    10466 2024-04-18 09:24:43.939683 tdf_tool-2.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-16 07:59:17.944743 tdf_tool-2.4.7/LICENSE
+-rw-r--r--   0        0        0     9217 2024-04-16 07:59:17.944961 tdf_tool-2.4.7/README.md
+-rw-r--r--   0        0        0     1608 2024-04-19 10:02:02.216830 tdf_tool-2.4.7/pyproject.toml
+-rw-r--r--   0        0        0      321 2024-04-16 07:59:17.947227 tdf_tool-2.4.7/tdf_tool/app.py
+-rw-r--r--   0        0        0     1106 2024-04-18 09:33:56.862188 tdf_tool-2.4.7/tdf_tool/pipeline.py
+-rw-r--r--   0        0        0     8469 2024-04-18 09:33:56.862568 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc
+-rw-r--r--   0        0        0     4497 2024-04-19 02:17:38.880307 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc
+-rw-r--r--   0        0        0     7766 2024-04-19 10:01:22.245312 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc
+-rw-r--r--   0        0        0      424 2024-04-16 07:59:17.947648 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/cmd.cpython-39.pyc
+-rw-r--r--   0        0        0     2567 2024-04-16 07:59:17.947827 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc
+-rw-r--r--   0        0        0     1676 2024-04-19 02:17:38.888443 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc
+-rw-r--r--   0        0        0     2668 2024-04-16 07:59:17.948134 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc
+-rw-r--r--   0        0        0     1619 2024-04-19 02:17:38.894201 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc
+-rw-r--r--   0        0        0      496 2024-04-16 07:59:17.948441 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/init.cpython-39.pyc
+-rw-r--r--   0        0        0     3015 2024-04-16 07:59:17.948597 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc
+-rw-r--r--   0        0        0     2292 2024-04-19 02:17:38.497917 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc
+-rw-r--r--   0        0        0     2981 2024-04-16 07:59:17.948929 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc
+-rw-r--r--   0        0        0     2243 2024-04-19 02:17:38.892162 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc
+-rw-r--r--   0        0        0    36213 2024-04-16 07:59:17.949402 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc
+-rw-r--r--   0        0        0    16038 2024-04-19 09:06:09.150577 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc
+-rw-r--r--   0        0        0     3262 2024-04-16 07:59:17.950144 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc
+-rw-r--r--   0        0        0     1989 2024-04-19 02:17:38.771913 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc
+-rw-r--r--   0        0        0      817 2024-04-16 07:59:17.950609 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc
+-rw-r--r--   0        0        0      621 2024-04-18 09:33:56.866062 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc
+-rw-r--r--   0        0        0     5130 2024-04-18 09:33:56.866355 tdf_tool-2.4.7/tdf_tool/pipelines/annotation.py
+-rw-r--r--   0        0        0     7845 2024-04-19 10:01:18.301914 tdf_tool-2.4.7/tdf_tool/pipelines/api_interaction.py
+-rw-r--r--   0        0        0     1244 2024-04-18 09:33:56.867085 tdf_tool-2.4.7/tdf_tool/pipelines/fix_header.py
+-rw-r--r--   0        0        0     1211 2024-04-18 09:33:56.867471 tdf_tool-2.4.7/tdf_tool/pipelines/git.py
+-rw-r--r--   0        0        0     1889 2024-04-18 09:33:56.867849 tdf_tool-2.4.7/tdf_tool/pipelines/module.py
+-rw-r--r--   0        0        0     1630 2024-04-18 09:33:56.868234 tdf_tool-2.4.7/tdf_tool/pipelines/package.py
+-rw-r--r--   0        0        0    21886 2024-04-19 08:19:40.561443 tdf_tool-2.4.7/tdf_tool/pipelines/router.py
+-rw-r--r--   0        0        0     1656 2024-04-18 09:33:56.869173 tdf_tool-2.4.7/tdf_tool/pipelines/translate.py
+-rw-r--r--   0        0        0      179 2024-04-16 07:59:17.952763 tdf_tool-2.4.7/tdf_tool/pipelines/upgrade.py
+-rw-r--r--   0        0        0     1653 2024-04-16 07:59:17.953204 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc
+-rw-r--r--   0        0        0     1064 2024-04-18 09:33:56.869593 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc
+-rw-r--r--   0        0        0    10270 2024-04-16 07:59:17.953777 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc
+-rw-r--r--   0        0        0     5149 2024-04-18 09:33:56.870029 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc
+-rw-r--r--   0        0        0     1328 2024-04-16 07:59:17.954419 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/env.cpython-311.pyc
+-rw-r--r--   0        0        0     1113 2024-04-19 09:46:49.061939 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/env.cpython-39.pyc
+-rw-r--r--   0        0        0      890 2024-04-19 09:59:10.596913 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/generator.cpython-39.pyc
+-rw-r--r--   0        0        0     2480 2024-04-16 07:59:17.954948 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     1464 2024-04-18 09:33:56.871044 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     2969 2024-04-16 07:59:17.955456 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/print.cpython-311.pyc
+-rw-r--r--   0        0        0     2040 2024-04-19 09:43:51.505624 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/print.cpython-39.pyc
+-rw-r--r--   0        0        0     9661 2024-04-16 07:59:17.955984 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     6181 2024-04-18 09:33:56.871935 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc
+-rw-r--r--   0        0        0    10739 2024-04-16 07:59:17.956576 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc
+-rw-r--r--   0        0        0     5620 2024-04-19 02:17:38.568605 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc
+-rw-r--r--   0        0        0    11432 2024-04-16 07:59:17.957426 tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc
+-rw-r--r--   0        0        0     7694 2024-04-18 09:33:56.873380 tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc
+-rw-r--r--   0        0        0     7216 2024-04-16 07:59:17.958050 tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc
+-rw-r--r--   0        0        0     4018 2024-04-18 09:33:56.873929 tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc
+-rw-r--r--   0        0        0     1835 2024-04-18 09:33:56.874377 tdf_tool-2.4.7/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc
+-rw-r--r--   0        0        0     1628 2024-04-16 07:59:17.959126 tdf_tool-2.4.7/tdf_tool/tools/cli/bean/deps_item.py
+-rw-r--r--   0        0        0    12287 2024-04-16 07:59:17.959442 tdf_tool-2.4.7/tdf_tool/tools/cli/module_deps_rewrite.py
+-rw-r--r--   0        0        0     5041 2024-04-16 07:59:17.959734 tdf_tool-2.4.7/tdf_tool/tools/cli/project_cli.py
+-rw-r--r--   0        0        0     1919 2024-04-18 09:33:56.874872 tdf_tool-2.4.7/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     1833 2024-04-16 07:59:17.960396 tdf_tool-2.4.7/tdf_tool/tools/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      559 2024-04-16 07:59:17.960648 tdf_tool-2.4.7/tdf_tool/tools/cmd.py
+-rw-r--r--   0        0        0     7002 2024-04-16 07:59:17.961174 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     3385 2024-04-18 09:33:56.875378 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0        0        0     2717 2024-04-16 07:59:17.961718 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc
+-rw-r--r--   0        0        0     1491 2024-04-19 02:17:38.769502 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc
+-rw-r--r--   0        0        0     2693 2024-04-16 07:59:17.962260 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc
+-rw-r--r--   0        0        0     2732 2024-04-16 07:59:17.962513 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc
+-rw-r--r--   0        0        0     2103 2024-04-19 02:17:38.774000 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc
+-rw-r--r--   0        0        0     9155 2024-04-16 07:59:17.963058 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc
+-rw-r--r--   0        0        0     4496 2024-04-18 09:33:56.876915 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc
+-rw-r--r--   0        0        0     3983 2024-04-16 07:59:17.963572 tdf_tool-2.4.7/tdf_tool/tools/config/config.py
+-rw-r--r--   0        0        0     1310 2024-04-18 09:33:56.877413 tdf_tool-2.4.7/tdf_tool/tools/config/initial_json_config.py
+-rw-r--r--   0        0        0     1267 2024-04-18 09:33:56.877960 tdf_tool-2.4.7/tdf_tool/tools/config/module_json_config.py
+-rw-r--r--   0        0        0     5593 2024-04-16 07:59:17.964325 tdf_tool-2.4.7/tdf_tool/tools/config/packages_config.py
+-rw-r--r--   0        0        0     7704 2024-04-16 07:59:17.964588 tdf_tool-2.4.7/tdf_tool/tools/dependencies_analysis.py
+-rw-r--r--   0        0        0      776 2024-04-19 09:46:46.688382 tdf_tool-2.4.7/tdf_tool/tools/env.py
+-rw-r--r--   0        0        0     6312 2024-04-16 07:59:17.965341 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc
+-rw-r--r--   0        0        0     3616 2024-04-18 09:33:56.878578 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc
+-rw-r--r--   0        0        0     3174 2024-04-16 07:59:17.965839 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     2004 2024-04-18 09:33:56.879118 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc
+-rw-r--r--   0        0        0     4314 2024-04-16 07:59:17.966355 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     2464 2024-04-18 09:33:56.879669 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     6437 2024-04-16 07:59:17.966902 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     3681 2024-04-18 09:33:56.880258 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     2422 2024-04-16 07:59:17.967708 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     3345 2024-04-16 07:59:17.967959 tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_entry.py
+-rw-r--r--   0        0        0     1586 2024-04-16 07:59:17.968270 tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_lint.py
+-rw-r--r--   0        0        0     2137 2024-04-16 07:59:17.968589 tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_lint_tool.py
+-rw-r--r--   0        0        0     4095 2024-04-16 07:59:17.968850 tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_replace_tool.py
+-rw-r--r--   0        0        0     1159 2024-04-16 07:59:17.969195 tdf_tool-2.4.7/tdf_tool/tools/flutter_script.py
+-rw-r--r--   0        0        0      444 2024-04-19 09:59:03.824969 tdf_tool-2.4.7/tdf_tool/tools/generator.py
+-rw-r--r--   0        0        0     7243 2024-04-16 07:59:17.969845 tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc
+-rw-r--r--   0        0        0     4190 2024-04-18 09:33:56.880901 tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     7055 2024-04-16 07:59:17.970442 tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc
+-rw-r--r--   0        0        0     3786 2024-04-18 09:33:56.881487 tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc
+-rw-r--r--   0        0        0      593 2024-04-16 07:59:17.971051 tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc
+-rw-r--r--   0        0        0     5019 2024-04-16 07:59:17.971732 tdf_tool-2.4.7/tdf_tool/tools/gitlab/gitlab_utils.py
+-rw-r--r--   0        0        0     3814 2024-04-16 07:59:17.972085 tdf_tool-2.4.7/tdf_tool/tools/gitlab/python_gitlab_api.py
+-rw-r--r--   0        0        0     2482 2024-04-16 07:59:17.972678 tdf_tool-2.4.7/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     1412 2024-04-18 09:33:56.882138 tdf_tool-2.4.7/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     1063 2024-04-16 07:59:17.973603 tdf_tool-2.4.7/tdf_tool/tools/module/module_tools.py
+-rw-r--r--   0        0        0    11056 2024-04-16 07:59:17.974266 tdf_tool-2.4.7/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc
+-rw-r--r--   0        0        0     5267 2024-04-18 09:33:56.882719 tdf_tool-2.4.7/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     9752 2024-04-16 07:59:17.974933 tdf_tool-2.4.7/tdf_tool/tools/package/seal_off_package_utils.py
+-rw-r--r--   0        0        0      911 2024-04-16 07:59:17.975191 tdf_tool-2.4.7/tdf_tool/tools/platform_tools.py
+-rw-r--r--   0        0        0     1226 2024-04-19 09:43:13.615410 tdf_tool-2.4.7/tdf_tool/tools/print.py
+-rw-r--r--   0        0        0     7598 2024-04-16 07:59:17.975770 tdf_tool-2.4.7/tdf_tool/tools/regular_tool.py
+-rw-r--r--   0        0        0     5718 2024-04-18 09:33:56.883146 tdf_tool-2.4.7/tdf_tool/tools/shell_dir.py
+-rw-r--r--   0        0        0     3840 2024-04-16 07:59:17.976600 tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc
+-rw-r--r--   0        0        0     2161 2024-04-18 09:33:56.883746 tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc
+-rw-r--r--   0        0        0     2695 2024-04-16 07:59:17.977108 tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     1678 2024-04-18 09:33:56.884279 tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc
+-rw-r--r--   0        0        0    11711 2024-04-16 07:59:17.977716 tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     1999 2024-04-16 07:59:17.977961 tdf_tool-2.4.7/tdf_tool/tools/translate/file_util.py
+-rw-r--r--   0        0        0    15484 2024-04-16 07:59:17.978545 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     8285 2024-04-18 09:33:56.884733 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc
+-rw-r--r--   0        0        0    26818 2024-04-16 07:59:17.979344 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc
+-rw-r--r--   0        0        0    13427 2024-04-18 09:33:56.885241 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0    10691 2024-04-16 07:59:17.980114 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/flutter_translate_lint.py
+-rw-r--r--   0        0        0    18954 2024-04-16 07:59:17.980464 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/flutter_translate_tools.py
+-rw-r--r--   0        0        0     8395 2024-04-16 07:59:17.981075 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc
+-rw-r--r--   0        0        0     4595 2024-04-18 09:33:56.885795 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc
+-rw-r--r--   0        0        0     5228 2024-04-16 07:59:17.981648 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py
+-rw-r--r--   0        0        0      859 2024-04-16 07:59:17.982222 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc
+-rw-r--r--   0        0        0     7351 2024-04-16 07:59:17.982702 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc
+-rw-r--r--   0        0        0     7599 2024-04-16 07:59:17.983077 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc
+-rw-r--r--   0        0        0     4216 2024-04-18 09:33:56.886328 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc
+-rw-r--r--   0        0        0     3952 2024-04-16 07:59:17.983786 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     2347 2024-04-18 09:33:56.886740 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc
+-rw-r--r--   0        0        0      870 2024-04-16 07:59:17.984330 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc
+-rw-r--r--   0        0        0     4766 2024-04-16 07:59:17.984706 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     6219 2024-04-16 07:59:17.985086 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc
+-rw-r--r--   0        0        0     2631 2024-04-16 07:59:17.985435 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc
+-rw-r--r--   0        0        0     4438 2024-04-16 07:59:17.985774 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/ios_translate.py
+-rw-r--r--   0        0        0     2000 2024-04-16 07:59:17.986154 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/ios_translate_lint.py
+-rw-r--r--   0        0        0     5061 2024-04-16 07:59:17.986697 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     2852 2024-04-18 09:33:56.887291 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc
+-rw-r--r--   0        0        0    17576 2024-04-16 07:59:17.987402 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc
+-rw-r--r--   0        0        0     9306 2024-04-18 09:33:56.887836 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc
+-rw-r--r--   0        0        0     7901 2024-04-16 07:59:17.988120 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc
+-rw-r--r--   0        0        0     4398 2024-04-18 09:33:56.888413 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc
+-rw-r--r--   0        0        0     1158 2024-04-16 07:59:17.988695 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc
+-rw-r--r--   0        0        0     1028 2024-04-18 09:33:56.889038 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc
+-rw-r--r--   0        0        0    10070 2024-04-16 07:59:17.989363 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     5366 2024-04-18 09:33:56.889482 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     2773 2024-04-16 07:59:17.989983 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc
+-rw-r--r--   0        0        0     2689 2024-04-18 09:33:56.889936 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc
+-rw-r--r--   0        0        0    11353 2024-04-16 07:59:17.990542 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc
+-rw-r--r--   0        0        0     6226 2024-04-18 09:33:56.890414 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc
+-rw-r--r--   0        0        0     4943 2024-04-16 07:59:17.991277 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc
+-rw-r--r--   0        0        0     2687 2024-04-18 09:33:56.890983 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc
+-rw-r--r--   0        0        0     3270 2024-04-16 07:59:17.991799 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py
+-rw-r--r--   0        0        0    14326 2024-04-16 07:59:17.992093 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_module.py
+-rw-r--r--   0        0        0     5223 2024-04-16 07:59:17.992380 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py
+-rw-r--r--   0        0        0     1189 2024-04-16 07:59:17.992605 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py
+-rw-r--r--   0        0        0     8191 2024-04-16 07:59:17.992866 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py
+-rw-r--r--   0        0        0     2337 2024-04-16 07:59:17.993215 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/location_string_temp.py
+-rw-r--r--   0        0        0     8684 2024-04-16 07:59:17.993505 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/podspec.py
+-rw-r--r--   0        0        0     2886 2024-04-16 07:59:17.993759 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/string_util.py
+-rw-r--r--   0        0        0     8625 2024-04-16 07:59:17.994344 tdf_tool-2.4.7/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     5032 2024-04-18 09:33:56.891445 tdf_tool-2.4.7/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     5111 2024-04-16 07:59:17.994952 tdf_tool-2.4.7/tdf_tool/tools/translate/tools/translate_tool.py
+-rw-r--r--   0        0        0     1408 2024-04-16 07:59:17.995250 tdf_tool-2.4.7/tdf_tool/tools/translate/translate_lint.py
+-rw-r--r--   0        0        0     1268 2024-04-16 07:59:17.996782 tdf_tool-2.4.7/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc
+-rw-r--r--   0        0        0      880 2024-04-18 09:33:56.891894 tdf_tool-2.4.7/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc
+-rw-r--r--   0        0        0      440 2024-04-16 07:59:17.997353 tdf_tool-2.4.7/tdf_tool/tools/vscode/vscode.py
+-rw-r--r--   0        0        0    10568 1970-01-01 00:00:00.000000 tdf_tool-2.4.7/PKG-INFO
```

### Comparing `tdf_tool-2.4.6/LICENSE` & `tdf_tool-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/README.md` & `tdf_tool-2.4.7/README.md`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/pyproject.toml` & `tdf_tool-2.4.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 项目信息
 [tool.poetry]
 name = "tdf_tool"
-version = "2.4.6"
+version = "2.4.7"
 description = "二维火 flutter 脚手架工具"
 authors = ["Jian Xu <3386218996@qq.com>", "FanJiao Gai <gaijiaofan@2dfire.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://git.2dfire.net/app/flutter/tools/package_tools"
 repository = "https://git.2dfire.net/app/flutter/tools/package_tools.git"
 keywords = ["tdf", "tdf-tool", "tdf_tool"]
```

### Comparing `tdf_tool-2.4.6/tdf_tool/pipeline.py` & `tdf_tool-2.4.7/tdf_tool/pipeline.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 18 09:17:19 2024 UTC, .py size: 5130 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1fe5 2066 0a14 0000  a......... f....
+00000000: 610d 0d0a 0000 0000 04e9 2066 0a14 0000  a......... f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6400 6407 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 18 09:13:44 2024 UTC, .py size: 7388 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,448 +1,486 @@
-00000000: 610d 0d0a 0000 0000 48e4 2066 dc1c 0000  a.......H. f....
+00000000: 610d 0d0a 0000 0000 ee40 2266 a51e 0000  a........@"f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
-00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
-00000050: 6403 6c05 6d06 5a06 0100 6400 6404 6c07  d.l.m.Z...d.d.l.
+00000020: 0003 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
+00000040: 5a02 6400 6402 6c03 5a03 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
+00000050: 6d05 5a05 6d06 5a06 0100 6400 6404 6c07  m.Z.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 0100 4700 6406 6407 8400 6407 8302 5a0b  ..G.d.d...d...Z.
-00000080: 4700 6408 6409 8400 6409 8302 5a0c 4700  G.d.d...d...Z.G.
-00000090: 640a 640b 8400 640b 8302 5a0d 6401 5300  d.d...d...Z.d.S.
-000000a0: 290c e900 0000 004e 2902 da0b 5061 636b  )......N)...Pack
-000000b0: 6167 654e 6f64 65da 1250 6163 6b61 6765  ageNode..Package
-000000c0: 734a 736f 6e43 6f6e 6669 6729 01da 0d50  sJsonConfig)...P
-000000d0: 6c61 7466 6f72 6d54 6f6f 6c73 2901 da05  latformTools)...
-000000e0: 5072 696e 7429 01da 0853 6865 6c6c 4469  Print)...ShellDi
-000000f0: 7263 0000 0000 0000 0000 0000 0000 0000  rc..............
-00000100: 0000 0200 0000 4000 0000 731c 0000 0065  ......@...s....e
-00000110: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
-00000120: 0364 0484 005a 0464 0553 0029 06da 0849  .d...Z.d.S.)...I
-00000130: 6d70 6c4e 6f64 6563 0100 0000 0000 0000  mplNodec........
-00000140: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00000150: 7316 0000 0064 017c 005f 0064 017c 005f  s....d.|._.d.|._
-00000160: 0164 017c 005f 0264 0053 00a9 024e da00  .d.|._.d.S...N..
-00000170: a903 da0b 7061 636b 6167 654e 616d 65da  ....packageName.
-00000180: 0b70 6163 6b61 6765 5061 7468 da08 6669  .packagePath..fi
-00000190: 6c65 5061 7468 a901 da04 7365 6c66 a900  lePath....self..
-000001a0: 7210 0000 00f5 6e00 0000 2f55 7365 7273  r.....n.../Users
-000001b0: 2f78 756a 6961 6e2f 446f 6375 6d65 6e74  /xujian/Document
-000001c0: 732f 3230 3234 2fe6 a8a1 e59d 97e9 97b4  s/2024/.........
-000001d0: e4ba a4e4 ba92 e9a1 b9e7 9bae 746c e58d  ............tl..
-000001e0: 87e7 baa7 2f70 6163 6b61 6765 5f74 6f6f  ..../package_too
-000001f0: 6c73 2f74 6466 5f74 6f6f 6c2f 7069 7065  ls/tdf_tool/pipe
-00000200: 6c69 6e65 732f 6170 695f 696e 7465 7261  lines/api_intera
-00000210: 6374 696f 6e2e 7079 da08 5f5f 696e 6974  ction.py..__init
-00000220: 5f5f 0a00 0000 7306 0000 0000 0106 0106  __....s.........
-00000230: 017a 1149 6d70 6c4e 6f64 652e 5f5f 696e  .z.ImplNode.__in
-00000240: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
-00000250: 0001 0000 0004 0000 0043 0000 0073 1e00  .........C...s..
-00000260: 0000 7400 a001 6401 7c00 6a02 1700 6402  ..t...d.|.j...d.
-00000270: 1700 7c00 6a03 1700 a101 0100 6400 5300  ..|.j.......d.S.
-00000280: a903 4e7a 0870 6163 6b61 6765 3afa 012f  ..Nz.package:../
-00000290: a904 7205 0000 00da 0679 656c 6c6f 7772  ..r......yellowr
-000002a0: 0b00 0000 720d 0000 0072 0e00 0000 7210  ....r....r....r.
-000002b0: 0000 0072 1000 0000 7211 0000 00da 0570  ...r....r......p
-000002c0: 7269 6e74 0f00 0000 7302 0000 0000 017a  rint....s......z
-000002d0: 0e49 6d70 6c4e 6f64 652e 7072 696e 744e  .ImplNode.printN
-000002e0: a905 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  ....__name__..__
-000002f0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000300: 6e61 6d65 5f5f 7212 0000 0072 1700 0000  name__r....r....
-00000310: 7210 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
-00000320: 1100 0000 7207 0000 0009 0000 0073 0400  ....r........s..
-00000330: 0000 0801 0805 7207 0000 0063 0000 0000  ......r....c....
-00000340: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00000350: 4000 0000 731c 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00000360: 0264 0164 0284 005a 0364 0364 0484 005a  .d.d...Z.d.d...Z
-00000370: 0464 0553 0029 06da 0741 7069 4e6f 6465  .d.S.)...ApiNode
-00000380: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000390: 0002 0000 0043 0000 0073 1600 0000 6401  .....C...s....d.
-000003a0: 7c00 5f00 6401 7c00 5f01 6401 7c00 5f02  |._.d.|._.d.|._.
-000003b0: 6400 5300 7208 0000 0072 0a00 0000 720e  d.S.r....r....r.
-000003c0: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
-000003d0: 0000 7212 0000 0014 0000 0073 0600 0000  ..r........s....
-000003e0: 0001 0601 0601 7a10 4170 694e 6f64 652e  ......z.ApiNode.
-000003f0: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
-00000400: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-00000410: 0073 1e00 0000 7400 a001 6401 7c00 6a02  .s....t...d.|.j.
-00000420: 1700 6402 1700 7c00 6a03 1700 a101 0100  ..d...|.j.......
-00000430: 6400 5300 7213 0000 0072 1500 0000 720e  d.S.r....r....r.
-00000440: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
-00000450: 0000 7217 0000 0019 0000 0073 0200 0000  ..r........s....
-00000460: 0001 7a0d 4170 694e 6f64 652e 7072 696e  ..z.ApiNode.prin
-00000470: 744e 7218 0000 0072 1000 0000 7210 0000  tNr....r....r...
-00000480: 0072 1000 0000 7211 0000 0072 1c00 0000  .r....r....r....
-00000490: 1300 0000 7304 0000 0008 0108 0572 1c00  ....s........r..
-000004a0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000004b0: 0000 0004 0000 0040 0000 0073 8200 0000  .......@...s....
-000004c0: 6500 5a01 6400 5a02 6401 5a03 6402 6403  e.Z.d.Z.d.Z.d.d.
-000004d0: 8400 5a04 6404 6405 8400 5a05 6406 6407  ..Z.d.d...Z.d.d.
-000004e0: 8400 5a06 6408 6409 8400 5a07 640a 640b  ..Z.d.d...Z.d.d.
-000004f0: 8400 5a08 640c 640d 8400 5a09 640e 640f  ..Z.d.d...Z.d.d.
-00000500: 8400 5a0a 6410 6411 8400 5a0b 650c 650c  ..Z.d.d...Z.e.e.
-00000510: 650c 6412 9c03 6413 6414 8404 5a0d 6415  e.d...d.d...Z.d.
-00000520: 6416 8400 5a0e 6417 6418 8400 5a0f 6419  d...Z.d.d...Z.d.
-00000530: 641a 8400 5a10 641b 641c 8400 5a11 641d  d...Z.d.d...Z.d.
-00000540: 5300 291e da0d 4170 6941 6e6e 6f74 6174  S.)...ApiAnnotat
-00000550: 696f 6e75 4400 0000 0a20 2020 20e6 a8a1  ionuD....    ...
-00000560: e59d 97e9 97b4 e4ba a4e4 ba92 e694 afe6  ................
-00000570: 8c81 e79b b8e5 85b3 e591 bde4 bba4 efbc  ................
-00000580: 9a74 6c20 6170 6920 2d68 20e6 9fa5 e79c  .tl api -h .....
-00000590: 8be8 afa6 e683 850a 2020 2020 6301 0000  ........    c...
-000005a0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-000005b0: 0043 0000 0073 3c00 0000 6400 7c00 5f00  .C...s<...d.|._.
-000005c0: 6401 7c00 5f01 6700 7c00 5f02 6402 7c00  d.|._.g.|._.d.|.
-000005d0: 5f03 6700 7c00 5f04 6403 7c00 5f05 6404  _.g.|._.d.|._.d.
-000005e0: 7c00 5f06 6700 7c00 5f07 7c00 a008 a100  |._.g.|._.|.....
-000005f0: 0100 6400 5300 2905 4e7a 0e2e 7464 665f  ..d.S.).Nz..tdf_
-00000600: 696d 706c 2e64 6172 747a 0d2e 7464 665f  impl.dartz..tdf_
-00000610: 6170 692e 6461 7274 5a07 7464 665f 6170  api.dartZ.tdf_ap
-00000620: 69da 1374 6466 5f6d 6f64 756c 655f 6170  i..tdf_module_ap
-00000630: 695f 616e 6e6f 2909 da02 6666 da1a 5f41  i_anno)...ff.._A
-00000640: 7069 416e 6e6f 7461 7469 6f6e 5f5f 696d  piAnnotation__im
-00000650: 706c 5375 6666 6978 da1c 5f41 7069 416e  plSuffix.._ApiAn
-00000660: 6e6f 7461 7469 6f6e 5f5f 696d 706c 4e6f  notation__implNo
-00000670: 6465 4c69 7374 da19 5f41 7069 416e 6e6f  deList.._ApiAnno
-00000680: 7461 7469 6f6e 5f5f 6170 6953 7566 6669  tation__apiSuffi
-00000690: 78da 1b5f 4170 6941 6e6e 6f74 6174 696f  x.._ApiAnnotatio
-000006a0: 6e5f 5f61 7069 4e6f 6465 4c69 7374 da1e  n__apiNodeList..
-000006b0: 5f41 7069 416e 6e6f 7461 7469 6f6e 5f5f  _ApiAnnotation__
-000006c0: 696e 7465 7261 6374 696f 6e44 6972 5a1e  interactionDirZ.
-000006d0: 5f41 7069 416e 6e6f 7461 7469 6f6e 5f5f  _ApiAnnotation__
-000006e0: 616e 6e6f 7461 7469 6f6e 4e61 6d65 da1c  annotationName..
-000006f0: 5f41 7069 416e 6e6f 7461 7469 6f6e 5f5f  _ApiAnnotation__
-00000700: 7061 636b 6167 6573 4c69 7374 da13 6665  packagesList..fe
-00000710: 7463 685f 7061 636b 6167 6573 5f6c 6973  tch_packages_lis
-00000720: 7472 0e00 0000 7210 0000 0072 1000 0000  tr....r....r....
-00000730: 7211 0000 0072 1200 0000 2200 0000 7312  r....r...."...s.
-00000740: 0000 0000 0106 0106 0106 0106 0106 0106  ................
-00000750: 0106 0106 027a 1641 7069 416e 6e6f 7461  .....z.ApiAnnota
-00000760: 7469 6f6e 2e5f 5f69 6e69 745f 5f63 0100  tion.__init__c..
-00000770: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00000780: 0000 4300 0000 731c 0000 0074 00a0 01a1  ..C...s....t....
-00000790: 0001 0074 0274 03a0 04a1 0083 016a 057c  ...t.t.......j.|
-000007a0: 005f 0664 0053 0029 014e 2907 7206 0000  ._.d.S.).N).r...
-000007b0: 00da 0c67 6f49 6e53 6865 6c6c 4469 7272  ...goInShellDirr
-000007c0: 0300 0000 da02 6f73 da06 6765 7463 7764  ......os..getcwd
-000007d0: da08 7061 636b 6167 6573 7225 0000 0072  ..packagesr%...r
-000007e0: 0e00 0000 7210 0000 0072 1000 0000 7211  ....r....r....r.
-000007f0: 0000 0072 2600 0000 2f00 0000 7304 0000  ...r&.../...s...
-00000800: 0000 0108 027a 2141 7069 416e 6e6f 7461  .....z!ApiAnnota
-00000810: 7469 6f6e 2e66 6574 6368 5f70 6163 6b61  tion.fetch_packa
-00000820: 6765 735f 6c69 7374 6301 0000 0000 0000  ges_listc.......
-00000830: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
-00000840: 0073 5000 0000 7c00 a000 a100 7d01 7401  .sP...|.....}.t.
-00000850: 6a02 a003 7c01 6401 a102 7d02 7404 7c02  j...|.d...}.t.|.
-00000860: 6402 8302 7c00 5f05 7c00 a006 a100 0100  d...|._.|.......
-00000870: 7c00 a007 a100 0100 7c00 a008 a100 0100  |.......|.......
-00000880: 7c00 6a05 a009 a100 0100 7c00 a00a a100  |.j.......|.....
-00000890: 0100 6400 5300 2903 4e7a 1161 7069 5f72  ..d.S.).Nz.api_r
-000008a0: 6567 6973 7465 722e 6461 7274 7a02 772b  egister.dartz.w+
-000008b0: 290b da13 6765 745f 696e 7465 7261 6374  )...get_interact
-000008c0: 696f 6e5f 6469 7272 2800 0000 da04 7061  ion_dirr(.....pa
-000008d0: 7468 da04 6a6f 696e da04 6f70 656e 721f  th..join..openr.
-000008e0: 0000 00da 275f 4170 6941 6e6e 6f74 6174  ....'_ApiAnnotat
-000008f0: 696f 6e5f 5f69 6e74 6567 7261 7465 5f74  ion__integrate_t
-00000900: 6466 5f61 7069 5f66 696c 6573 da28 5f41  df_api_files.(_A
-00000910: 7069 416e 6e6f 7461 7469 6f6e 5f5f 696e  piAnnotation__in
-00000920: 7465 6772 6174 655f 7464 665f 696d 706c  tegrate_tdf_impl
-00000930: 5f66 696c 6573 da26 5f41 7069 416e 6e6f  _files.&_ApiAnno
-00000940: 7461 7469 6f6e 5f5f 6765 6e65 7261 7465  tation__generate
-00000950: 5f72 6567 6973 7465 725f 636f 6465 da05  _register_code..
-00000960: 636c 6f73 65da 0a5f 5f66 6f72 6d61 745f  close..__format_
-00000970: 5f29 0372 0f00 0000 5a0b 7464 665f 6170  _).r....Z.tdf_ap
-00000980: 695f 6469 725a 1261 7574 6f5f 7265 6769  i_dirZ.auto_regi
-00000990: 7374 6572 5f66 696c 6572 1000 0000 7210  ster_filer....r.
-000009a0: 0000 0072 1100 0000 da0f 696e 7465 6772  ...r......integr
-000009b0: 6174 655f 7368 656c 6c35 0000 0073 1000  ate_shell5...s..
-000009c0: 0000 0002 0801 0e01 0c03 0803 0803 0802  ................
-000009d0: 0a03 7a1d 4170 6941 6e6e 6f74 6174 696f  ..z.ApiAnnotatio
-000009e0: 6e2e 696e 7465 6772 6174 655f 7368 656c  n.integrate_shel
-000009f0: 6c63 0100 0000 0000 0000 0000 0000 0300  lc..............
-00000a00: 0000 0700 0000 4300 0000 737c 0000 007c  ......C...s|...|
-00000a10: 006a 0044 005d 1c7d 017c 00a0 017c 006a  .j.D.].}.|...|.j
-00000a20: 027c 016a 037c 016a 047c 016a 03a1 0401  .|.j.|.j.|.j....
-00000a30: 0071 067c 006a 0544 005d 1c7d 017c 00a0  .q.|.j.D.].}.|..
-00000a40: 017c 006a 027c 016a 037c 016a 047c 016a  .|.j.|.j.|.j.|.j
-00000a50: 03a1 0401 0071 2a7c 00a0 067c 006a 0264  .....q*|...|.j.d
-00000a60: 0164 02a1 0301 0064 037d 027c 006a 02a0  .d.....d.}.|.j..
-00000a70: 077c 02a0 087c 00a0 09a1 007c 00a0 0aa1  .|...|.....|....
-00000a80: 00a1 02a1 0101 0064 0053 0029 044e 721e  .......d.S.).Nr.
-00000a90: 0000 007a 1874 6466 5f6d 6f64 756c 655f  ...z.tdf_module_
-00000aa0: 6170 695f 616e 6e6f 2e64 6172 7475 8602  api_anno.dartu..
-00000ab0: 0000 0a0a 2020 2020 2020 2020 636c 6173  ....        clas
-00000ac0: 7320 5444 4641 7069 496d 706c 4175 746f  s TDFApiImplAuto
-00000ad0: 5265 6769 7374 6572 207b 7b0a 2020 2020  Register {{.    
-00000ae0: 2020 2020 2020 7374 6174 6963 204c 6973        static Lis
-00000af0: 743c 5479 7065 3e20 6170 6973 203d 205b  t<Type> apis = [
-00000b00: 0a20 2020 2020 2020 2020 2020 207b 307d  .            {0}
-00000b10: 0a20 2020 2020 2020 2020 205d 3b0a 2020  .          ];.  
-00000b20: 2020 2020 2020 2020 2f2f 20e7 a1ae e4bf          // .....
-00000b30: 9de6 8980 e69c 89e8 a2ab e5bc 95e7 94a8  ................
-00000b40: e79a 8461 7069 e5ba 93e7 9a84 e5ae 9ee7  ...api..........
-00000b50: 8eb0 e7b1 bbe9 83bd e5b7 b2e6 b3a8 e586  ................
-00000b60: 8c0a 2020 2020 2020 2020 2020 7374 6174  ..          stat
-00000b70: 6963 2076 6f69 6420 5f65 6e73 7572 6541  ic void _ensureA
-00000b80: 7069 496d 706c 5265 6769 7374 6572 2829  piImplRegister()
-00000b90: 207b 7b0a 2020 2020 2020 2020 2020 2020   {{.            
-00000ba0: 6170 6973 2e66 6f72 4561 6368 2828 656c  apis.forEach((el
-00000bb0: 656d 656e 7429 207b 7b0a 2020 2020 2020  ement) {{.      
-00000bc0: 2020 2020 2020 2020 6966 2028 2141 7069          if (!Api
-00000bd0: 5265 6769 7374 6572 4365 6e74 6572 2e6b  RegisterCenter.k
-00000be0: 6579 732e 636f 6e74 6169 6e73 2865 6c65  eys.contains(ele
-00000bf0: 6d65 6e74 2929 207b 7b0a 2020 2020 2020  ment)) {{.      
-00000c00: 2020 2020 2020 2020 2020 7468 726f 7720            throw 
-00000c10: 4578 6365 7074 696f 6e28 2224 7b7b 656c  Exception("${{el
-00000c20: 656d 656e 747d 7de7 9a84 e5ae 9ee7 8eb0  ement}}.........
-00000c30: e7b1 bbe6 9caa e69c aae6 b3a8 e586 8cef  ................
-00000c40: bc81 efbc 81ef bc81 e8af b7e5 88a0 e999  ................
-00000c50: a4e5 ba93 247b 7b65 6c65 6d65 6e74 7d7d  ....${{element}}
-00000c60: e79a 84e5 bc95 e794 a8e6 8896 e880 85e5  ................
-00000c70: bc95 e585 a5e5 ae9e e78e b0e7 b1bb 2229  ..............")
-00000c80: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00000c90: 7d7d 0a20 2020 2020 2020 2020 2020 207d  }}.            }
-00000ca0: 7d29 3b0a 2020 2020 2020 2020 2020 7d7d  });.          }}
-00000cb0: 0a0a 2020 2020 2020 2020 2020 7374 6174  ..          stat
-00000cc0: 6963 2076 6f69 6420 6175 746f 5265 6769  ic void autoRegi
-00000cd0: 7374 6572 2829 207b 7b0a 2020 2020 2020  ster() {{.      
-00000ce0: 2020 2020 2020 2020 7b31 7d0a 2020 2020          {1}.    
-00000cf0: 2020 2020 2020 2020 2020 5f65 6e73 7572            _ensur
-00000d00: 6541 7069 496d 706c 5265 6769 7374 6572  eApiImplRegister
-00000d10: 2829 3b0a 2020 2020 2020 2020 2020 7d7d  ();.          }}
-00000d20: 0a20 2020 2020 2020 207d 7d0a 2020 2020  .        }}.    
-00000d30: 2020 2020 2020 2020 290b 7221 0000 00da          ).r!....
-00000d40: 255f 4170 6941 6e6e 6f74 6174 696f 6e5f  %_ApiAnnotation_
-00000d50: 5f5f 5f69 6d70 6f72 745f 6461 7461 5f63  ___import_data_c
-00000d60: 7265 6174 6f72 721f 0000 0072 0b00 0000  reatorr....r....
-00000d70: 720d 0000 0072 2300 0000 da31 5f41 7069  r....r#....1_Api
-00000d80: 416e 6e6f 7461 7469 6f6e 5f5f 696d 706f  Annotation__impo
-00000d90: 7274 5f64 6174 615f 6372 6561 746f 725f  rt_data_creator_
-00000da0: 7769 7468 6f75 745f 616c 6961 73da 0577  without_alias..w
-00000db0: 7269 7465 da06 666f 726d 6174 da10 6170  rite..format..ap
-00000dc0: 695f 6c69 7374 5f63 7265 6174 6f72 da25  i_list_creator.%
-00000dd0: 5f41 7069 416e 6e6f 7461 7469 6f6e 5f5f  _ApiAnnotation__
-00000de0: 7265 6769 7374 6572 5f6c 6973 745f 6372  register_list_cr
-00000df0: 6561 746f 7229 0372 0f00 0000 5a05 5f69  eator).r....Z._i
-00000e00: 7465 6dda 0763 6f6e 7465 6e74 7210 0000  tem..contentr...
-00000e10: 0072 1000 0000 7211 0000 005a 185f 5f67  .r....r....Z.__g
-00000e20: 656e 6572 6174 655f 7265 6769 7374 6572  enerate_register
-00000e30: 5f63 6f64 6549 0000 0073 1400 0000 0001  _codeI...s......
-00000e40: 0a01 1a01 0a01 1a02 1002 0415 0a01 0601  ................
-00000e50: 06fe 7a26 4170 6941 6e6e 6f74 6174 696f  ..z&ApiAnnotatio
-00000e60: 6e2e 5f5f 6765 6e65 7261 7465 5f72 6567  n.__generate_reg
-00000e70: 6973 7465 725f 636f 6465 6301 0000 0000  ister_codec.....
-00000e80: 0000 0000 0000 0003 0000 0006 0000 0043  ...............C
-00000e90: 0000 0073 2800 0000 6401 7d01 7c00 6a00  ...s(...d.}.|.j.
-00000ea0: 4400 5d18 7d02 7c01 6402 a001 7c02 6a02  D.].}.|.d...|.j.
-00000eb0: 7c02 6a02 a102 3700 7d01 710a 7c01 5300  |.j...7.}.q.|.S.
-00000ec0: 2903 4e72 0900 0000 7a69 0a20 2020 2020  ).Nr....zi.     
-00000ed0: 2020 2020 2020 2041 7069 5265 6769 7374         ApiRegist
-00000ee0: 6572 4365 6e74 6572 2e72 6567 6973 7465  erCenter.registe
-00000ef0: 7228 7b30 7d2e 4175 746f 5265 6769 7374  r({0}.AutoRegist
-00000f00: 6572 2e61 7069 5479 7065 2c7b 317d 2e41  er.apiType,{1}.A
-00000f10: 7574 6f52 6567 6973 7465 722e 7072 6f76  utoRegister.prov
-00000f20: 6964 6572 293b 0a20 2020 2020 2020 2020  ider);.         
-00000f30: 2020 2029 0372 2100 0000 7238 0000 0072     ).r!...r8...r
-00000f40: 0b00 0000 a903 720f 0000 0072 3b00 0000  ......r....r;...
-00000f50: da04 6974 656d 7210 0000 0072 1000 0000  ..itemr....r....
-00000f60: 7211 0000 005a 175f 5f72 6567 6973 7465  r....Z.__registe
-00000f70: 725f 6c69 7374 5f63 7265 6174 6f72 6a00  r_list_creatorj.
-00000f80: 0000 730c 0000 0000 0104 010a 0106 0208  ..s.............
-00000f90: fe08 037a 2541 7069 416e 6e6f 7461 7469  ...z%ApiAnnotati
-00000fa0: 6f6e 2e5f 5f72 6567 6973 7465 725f 6c69  on.__register_li
-00000fb0: 7374 5f63 7265 6174 6f72 6301 0000 0000  st_creatorc.....
-00000fc0: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
-00000fd0: 0000 0073 2400 0000 6401 7d01 7c00 6a00  ...s$...d.}.|.j.
-00000fe0: 4400 5d14 7d02 7c01 6402 a001 7c02 6a02  D.].}.|.d...|.j.
-00000ff0: a101 3700 7d01 710a 7c01 5300 2903 4e72  ..7.}.q.|.S.).Nr
-00001000: 0900 0000 7a43 0a20 2020 2020 2020 2020  ....zC.         
-00001010: 2020 207b 307d 2e54 4446 4170 6941 7574     {0}.TDFApiAut
-00001020: 6f49 6e76 616c 6964 6174 652e 6170 6954  oInvalidate.apiT
-00001030: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
-00001040: 2020 2020 2020 2020 2029 0372 2300 0000           ).r#...
-00001050: 7238 0000 0072 0b00 0000 723c 0000 0072  r8...r....r<...r
-00001060: 1000 0000 7210 0000 0072 1100 0000 7239  ....r....r....r9
-00001070: 0000 0072 0000 0073 0c00 0000 0001 0401  ...r...s........
-00001080: 0a01 0602 04fe 0803 7a1e 4170 6941 6e6e  ........z.ApiAnn
-00001090: 6f74 6174 696f 6e2e 6170 695f 6c69 7374  otation.api_list
-000010a0: 5f63 7265 6174 6f72 6301 0000 0000 0000  _creatorc.......
-000010b0: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
-000010c0: 0073 6200 0000 7400 a001 6401 a101 0100  .sb...t...d.....
-000010d0: 7c00 6a02 4400 5d4c 7d01 7c00 a003 7c01  |.j.D.]L}.|...|.
-000010e0: 6a04 7c00 6a05 a102 7d02 7c02 6400 7501  j.|.j...}.|.d.u.
-000010f0: 7210 7406 8300 7d03 7c01 6a04 7c03 5f04  r.t...}.|.j.|._.
-00001100: 7c01 6a07 7c03 5f07 7c02 7c03 5f08 7c03  |.j.|._.|.|._.|.
-00001110: a009 a100 0100 7c00 6a0a a00b 7c03 a101  ......|.j...|...
-00001120: 0100 7110 6400 5300 2902 4e75 1c00 0000  ..q.d.S.).Nu....
-00001130: e695 b4e5 9088 e689 80e6 9c89 e4ba a4e4  ................
-00001140: ba92 696d 706c e696 87e4 bbb6 290c 7205  ..impl......).r.
-00001150: 0000 00da 0574 6974 6c65 7225 0000 00da  .....titler%....
-00001160: 1f5f 4170 6941 6e6e 6f74 6174 696f 6e5f  ._ApiAnnotation_
-00001170: 5f67 6574 5f74 6172 6765 745f 6669 6c65  _get_target_file
-00001180: 720c 0000 0072 2000 0000 7207 0000 0072  r....r ...r....r
-00001190: 0b00 0000 720d 0000 0072 1700 0000 7221  ....r....r....r!
-000011a0: 0000 00da 0661 7070 656e 6429 0472 0f00  .....append).r..
-000011b0: 0000 da0b 7061 636b 6167 6549 7465 6dda  ....packageItem.
-000011c0: 195f 4170 6941 6e6e 6f74 6174 696f 6e5f  ._ApiAnnotation_
-000011d0: 5f66 696c 655f 7061 7468 5a09 5f69 6d70  _file_pathZ._imp
-000011e0: 6c4e 6f64 6572 1000 0000 7210 0000 0072  lNoder....r....r
-000011f0: 1100 0000 5a1a 5f5f 696e 7465 6772 6174  ....Z.__integrat
-00001200: 655f 7464 665f 696d 706c 5f66 696c 6573  e_tdf_impl_files
-00001210: 7a00 0000 7314 0000 0000 010a 010a 0110  z...s...........
-00001220: 0108 0106 0108 0108 0106 0108 017a 2841  .............z(A
-00001230: 7069 416e 6e6f 7461 7469 6f6e 2e5f 5f69  piAnnotation.__i
-00001240: 6e74 6567 7261 7465 5f74 6466 5f69 6d70  ntegrate_tdf_imp
-00001250: 6c5f 6669 6c65 7363 0100 0000 0000 0000  l_filesc........
-00001260: 0000 0000 0400 0000 0500 0000 4300 0000  ............C...
-00001270: 7362 0000 0074 00a0 0164 01a1 0101 007c  sb...t...d.....|
-00001280: 006a 0244 005d 4c7d 017c 00a0 037c 016a  .j.D.]L}.|...|.j
-00001290: 047c 006a 05a1 027d 027c 0264 0075 0172  .|.j...}.|.d.u.r
-000012a0: 1074 0683 007d 037c 016a 047c 035f 047c  .t...}.|.j.|._.|
-000012b0: 016a 077c 035f 077c 027c 035f 087c 03a0  .j.|._.|.|._.|..
-000012c0: 09a1 0001 007c 006a 0aa0 0b7c 03a1 0101  .....|.j...|....
-000012d0: 0071 1064 0053 0029 024e 751b 0000 00e6  .q.d.S.).Nu.....
-000012e0: 95b4 e590 88e6 8980 e69c 89e4 baa4 e4ba  ................
-000012f0: 9261 7069 e696 87e4 bbb6 290c 7205 0000  .api......).r...
-00001300: 0072 3e00 0000 7225 0000 0072 3f00 0000  .r>...r%...r?...
-00001310: 720c 0000 0072 2200 0000 721c 0000 0072  r....r"...r....r
-00001320: 0b00 0000 720d 0000 0072 1700 0000 7223  ....r....r....r#
-00001330: 0000 0072 4000 0000 2904 720f 0000 0072  ...r@...).r....r
-00001340: 4100 0000 7242 0000 005a 085f 6170 694e  A...rB...Z._apiN
-00001350: 6f64 6572 1000 0000 7210 0000 0072 1100  oder....r....r..
-00001360: 0000 5a19 5f5f 696e 7465 6772 6174 655f  ..Z.__integrate_
-00001370: 7464 665f 6170 695f 6669 6c65 7386 0000  tdf_api_files...
-00001380: 0073 1400 0000 0001 0a01 0a01 1001 0801  .s..............
-00001390: 0601 0801 0801 0601 0801 7a27 4170 6941  ..........z'ApiA
-000013a0: 6e6e 6f74 6174 696f 6e2e 5f5f 696e 7465  nnotation.__inte
-000013b0: 6772 6174 655f 7464 665f 6170 695f 6669  grate_tdf_api_fi
-000013c0: 6c65 7329 03da 0966 696c 655f 7061 7468  les)...file_path
-000013d0: da06 7375 6666 6978 da06 7265 7475 726e  ..suffix..return
-000013e0: 6303 0000 0000 0000 0000 0000 000c 0000  c...............
-000013f0: 0006 0000 0043 0000 0073 ce00 0000 7400  .....C...s....t.
-00001400: a001 a100 0100 7402 a003 7c01 a101 0100  ......t...|.....
-00001410: 6401 7d03 7402 a004 7405 a006 a100 a101  d.}.t...t.......
-00001420: a007 a100 a008 6402 a101 6401 1900 7d04  ......d...d...}.
-00001430: 7402 a009 7c04 a101 4400 5d66 5c03 7d05  t...|...D.]f\.}.
-00001440: 7d06 7d07 7c07 4400 5d56 7d08 7402 6a0a  }.}.|.D.]V}.t.j.
-00001450: a00b 7c05 7c08 a102 7d09 7c09 a00c 7c02  ..|.|...}.|...|.
-00001460: a101 724a 7c03 6403 3700 7d03 7405 a00d  ..rJ|.d.7.}.t...
-00001470: a100 7292 7c09 a008 6404 a101 6403 1900  ..r.|...d...d...
-00001480: 7d0a 7c0a a00e 6405 6406 a102 7d0b 714a  }.|...d.d...}.qJ
-00001490: 7c09 a008 6407 a101 6403 1900 7d0b 714a  |...d...d...}.qJ
-000014a0: 713c 7c03 6403 6b02 72b0 7c0b 5300 7c03  q<|.d.k.r.|.S.|.
-000014b0: 6403 6b04 72ca 740f 6408 a010 7c01 a101  d.k.r.t.d...|...
-000014c0: 8301 8201 6400 5300 6400 5300 2909 4e72  ....d.S.d.S.).Nr
-000014d0: 0100 0000 da01 0ae9 0100 0000 7a05 5c6c  ............z.\l
-000014e0: 6962 5cfa 015c 7214 0000 007a 052f 6c69  ib\..\r....z./li
-000014f0: 622f 7530 0000 00e6 a8a1 e59d 977b 307d  b/u0.........{0}
-00001500: e5ad 98e5 9ca8 e5a4 9ae4 b8aa e4ba a4e4  ................
-00001510: ba92 e696 87e4 bbb6 efbc 8ce8 afb7 e6a3  ................
-00001520: 80e6 9fa5 e29d 8c29 1172 0600 0000 7227  .......).r....r'
-00001530: 0000 0072 2800 0000 da05 6368 6469 72da  ...r(.....chdir.
-00001540: 0570 6f70 656e 7204 0000 00da 0770 7764  .popenr......pwd
-00001550: 5f63 6d64 da04 7265 6164 da05 7370 6c69  _cmd..read..spli
-00001560: 74da 0477 616c 6b72 2c00 0000 722d 0000  t..walkr,...r-..
-00001570: 00da 0865 6e64 7377 6974 68da 0a69 735f  ...endswith..is_
-00001580: 7769 6e64 6f77 73da 0772 6570 6c61 6365  windows..replace
-00001590: da09 4578 6365 7074 696f 6e72 3800 0000  ..Exceptionr8...
-000015a0: 290c 720f 0000 0072 4300 0000 7244 0000  ).r....rC...rD..
-000015b0: 00da 0563 6f75 6e74 da08 6e6f 7761 5061  ...count..nowaPa
-000015c0: 7468 da04 726f 6f74 da04 6469 7273 da05  th..root..dirs..
-000015d0: 6669 6c65 73da 0466 696c 65da 0873 7263  files..file..src
-000015e0: 5f66 696c 65da 0474 656d 705a 1b5f 4170  _file..tempZ._Ap
-000015f0: 6941 6e6e 6f74 6174 696f 6e5f 5f74 6172  iAnnotation__tar
-00001600: 6765 745f 6669 6c65 7210 0000 0072 1000  get_filer....r..
-00001610: 0000 7211 0000 005a 115f 5f67 6574 5f74  ..r....Z.__get_t
-00001620: 6172 6765 745f 6669 6c65 9300 0000 7326  arget_file....s&
-00001630: 0000 0000 0108 010a 0204 021c 0114 0108  ................
-00001640: 010e 010a 0108 0108 010e 010e 0212 0108  ................
-00001650: 0104 0108 010e 0104 017a 1f41 7069 416e  .........z.ApiAn
-00001660: 6e6f 7461 7469 6f6e 2e5f 5f67 6574 5f74  notation.__get_t
-00001670: 6172 6765 745f 6669 6c65 6301 0000 0000  arget_filec.....
-00001680: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
-00001690: 0000 0073 4e00 0000 7400 a001 a100 0100  ...sN...t.......
-000016a0: 7402 a003 6401 a101 0100 7402 6a04 a005  t...d.....t.j...
-000016b0: 7c00 6a06 a101 722c 7407 a008 7c00 6a06  |.j...r,t...|.j.
-000016c0: a101 0100 7402 a009 7c00 6a06 a101 0100  ....t...|.j.....
-000016d0: 7402 6a04 a00a 7400 a00b a100 6401 7c00  t.j...t.....d.|.
-000016e0: 6a06 a103 5300 2902 4eda 036c 6962 290c  j...S.).N..lib).
-000016f0: 7206 0000 0072 2700 0000 7228 0000 0072  r....r'...r(...r
-00001700: 4900 0000 722c 0000 00da 0665 7869 7374  I...r,.....exist
-00001710: 7372 2400 0000 da06 7368 7574 696c da06  sr$.....shutil..
-00001720: 726d 7472 6565 da05 6d6b 6469 7272 2d00  rmtree..mkdirr-.
-00001730: 0000 da0b 6765 7453 6865 6c6c 4469 7272  ....getShellDirr
-00001740: 0e00 0000 7210 0000 0072 1000 0000 7211  ....r....r....r.
-00001750: 0000 0072 2b00 0000 ab00 0000 730c 0000  ...r+.......s...
-00001760: 0000 0108 010a 010e 010c 010c 017a 2141  .............z!A
-00001770: 7069 416e 6e6f 7461 7469 6f6e 2e67 6574  piAnnotation.get
-00001780: 5f69 6e74 6572 6163 7469 6f6e 5f64 6972  _interaction_dir
-00001790: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000017a0: 0005 0000 0043 0000 0073 3200 0000 7400  .....C...s2...t.
-000017b0: a001 a100 0100 7402 6a03 a004 7400 a005  ......t.j...t...
-000017c0: a100 6401 7c00 6a06 a103 7d01 7402 a007  ..d.|.j...}.t...
-000017d0: 6402 a008 7c01 a101 a101 0100 6400 5300  d...|.......d.S.
-000017e0: 2903 4e72 5b00 0000 7a0f 6461 7274 2066  ).Nr[...z.dart f
-000017f0: 6f72 6d61 7420 7b30 7d29 0972 0600 0000  ormat {0}).r....
-00001800: da0f 676f 496e 5368 656c 6c4c 6962 4469  ..goInShellLibDi
-00001810: 7272 2800 0000 722c 0000 0072 2d00 0000  rr(...r,...r-...
-00001820: 7260 0000 0072 2400 0000 da06 7379 7374  r`...r$.....syst
-00001830: 656d 7238 0000 0029 0272 0f00 0000 5a14  emr8...).r....Z.
-00001840: 5f41 7069 416e 6e6f 7461 7469 6f6e 5f5f  _ApiAnnotation__
-00001850: 7061 7468 7210 0000 0072 1000 0000 7211  pathr....r....r.
-00001860: 0000 0072 3300 0000 b400 0000 7306 0000  ...r3.......s...
-00001870: 0000 0108 0116 017a 1841 7069 416e 6e6f  .......z.ApiAnno
-00001880: 7461 7469 6f6e 2e5f 5f66 6f72 6d61 745f  tation.__format_
-00001890: 5f63 0500 0000 0000 0000 0000 0000 0500  _c..............
-000018a0: 0000 0700 0000 4300 0000 7318 0000 007c  ......C...s....|
-000018b0: 01a0 0064 01a0 017c 027c 037c 04a1 03a1  ...d...|.|.|....
-000018c0: 0101 0064 0053 0029 024e 7a21 696d 706f  ...d.S.).Nz!impo
-000018d0: 7274 2022 7061 636b 6167 653a 7b30 7d2f  rt "package:{0}/
-000018e0: 7b31 7d22 2061 7320 7b32 7d3b 0aa9 0272  {1}" as {2};...r
-000018f0: 3700 0000 7238 0000 0029 0572 0f00 0000  7...r8...).r....
-00001900: da07 665f 7772 6974 65da 0b6d 6f64 756c  ..f_write..modul
-00001910: 655f 6e61 6d65 7243 0000 00da 0561 6c69  e_namerC.....ali
-00001920: 6173 7210 0000 0072 1000 0000 7211 0000  asr....r....r...
-00001930: 005a 175f 5f5f 5f69 6d70 6f72 745f 6461  .Z.____import_da
-00001940: 7461 5f63 7265 6174 6f72 ba00 0000 730a  ta_creator....s.
-00001950: 0000 0000 0304 0104 0106 ff02 ff7a 2541  .............z%A
-00001960: 7069 416e 6e6f 7461 7469 6f6e 2e5f 5f5f  piAnnotation.___
-00001970: 5f69 6d70 6f72 745f 6461 7461 5f63 7265  _import_data_cre
-00001980: 6174 6f72 6304 0000 0000 0000 0000 0000  atorc...........
-00001990: 0004 0000 0006 0000 0043 0000 0073 1600  .........C...s..
-000019a0: 0000 7c01 a000 6401 a001 7c02 7c03 a102  ..|...d...|.|...
-000019b0: a101 0100 6400 5300 2902 4e7a 1a69 6d70  ....d.S.).Nz.imp
-000019c0: 6f72 7420 2270 6163 6b61 6765 3a7b 307d  ort "package:{0}
-000019d0: 2f7b 317d 223b 0a72 6300 0000 2904 720f  /{1}";.rc...).r.
-000019e0: 0000 0072 6400 0000 7265 0000 0072 4300  ...rd...re...rC.
-000019f0: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00001a00: 005a 235f 5f69 6d70 6f72 745f 6461 7461  .Z#__import_data
-00001a10: 5f63 7265 6174 6f72 5f77 6974 686f 7574  _creator_without
-00001a20: 5f61 6c69 6173 c400 0000 730a 0000 0000  _alias....s.....
-00001a30: 0304 0104 0104 ff02 ff7a 3141 7069 416e  .........z1ApiAn
-00001a40: 6e6f 7461 7469 6f6e 2e5f 5f69 6d70 6f72  notation.__impor
-00001a50: 745f 6461 7461 5f63 7265 6174 6f72 5f77  t_data_creator_w
-00001a60: 6974 686f 7574 5f61 6c69 6173 4e29 1272  ithout_aliasN).r
-00001a70: 1900 0000 721a 0000 0072 1b00 0000 da07  ....r....r......
-00001a80: 5f5f 646f 635f 5f72 1200 0000 7226 0000  __doc__r....r&..
-00001a90: 0072 3400 0000 7231 0000 0072 3a00 0000  .r4...r1...r:...
-00001aa0: 7239 0000 0072 3000 0000 722f 0000 00da  r9...r0...r/....
-00001ab0: 0373 7472 723f 0000 0072 2b00 0000 7233  .strr?...r+...r3
-00001ac0: 0000 0072 3500 0000 7236 0000 0072 1000  ...r5...r6...r..
-00001ad0: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00001ae0: 0072 1d00 0000 1d00 0000 731c 0000 0008  .r........s.....
-00001af0: 0104 0408 0d08 0608 1408 2108 0808 0808  ..........!.....
-00001b00: 0c08 0d12 1808 0908 0608 0a72 1d00 0000  ...........r....
-00001b10: 290e 7228 0000 0072 5d00 0000 da25 7464  ).r(...r]....%td
-00001b20: 665f 746f 6f6c 2e74 6f6f 6c73 2e63 6f6e  f_tool.tools.con
-00001b30: 6669 672e 7061 636b 6167 6573 5f63 6f6e  fig.packages_con
-00001b40: 6669 6772 0200 0000 7203 0000 00da 1d74  figr....r......t
-00001b50: 6466 5f74 6f6f 6c2e 746f 6f6c 732e 706c  df_tool.tools.pl
-00001b60: 6174 666f 726d 5f74 6f6f 6c73 7204 0000  atform_toolsr...
-00001b70: 00da 1474 6466 5f74 6f6f 6c2e 746f 6f6c  ...tdf_tool.tool
-00001b80: 732e 7072 696e 7472 0500 0000 da18 7464  s.printr......td
-00001b90: 665f 746f 6f6c 2e74 6f6f 6c73 2e73 6865  f_tool.tools.she
-00001ba0: 6c6c 5f64 6972 7206 0000 0072 0700 0000  ll_dirr....r....
-00001bb0: 721c 0000 0072 1d00 0000 7210 0000 0072  r....r....r....r
-00001bc0: 1000 0000 7210 0000 0072 1100 0000 da08  ....r....r......
-00001bd0: 3c6d 6f64 756c 653e 0100 0000 7310 0000  <module>....s...
-00001be0: 0008 0108 0110 010c 010c 010c 030e 0a0e  ................
-00001bf0: 0a                                       .
+00000070: 0100 6400 6406 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
+00000080: 6407 6c0d 6d0e 5a0e 0100 4700 6408 6409  d.l.m.Z...G.d.d.
+00000090: 8400 6409 8302 5a0f 4700 640a 640b 8400  ..d...Z.G.d.d...
+000000a0: 640b 8302 5a10 4700 640c 640d 8400 640d  d...Z.G.d.d...d.
+000000b0: 8302 5a11 6402 5300 290e e900 0000 0029  ..Z.d.S.)......)
+000000c0: 01da 036d 6435 4e29 02da 0b50 6163 6b61  ...md5N)...Packa
+000000d0: 6765 4e6f 6465 da12 5061 636b 6167 6573  geNode..Packages
+000000e0: 4a73 6f6e 436f 6e66 6967 2901 da0d 506c  JsonConfig)...Pl
+000000f0: 6174 666f 726d 546f 6f6c 7329 01da 0550  atformTools)...P
+00000100: 7269 6e74 2901 da08 5368 656c 6c44 6972  rint)...ShellDir
+00000110: 2901 da10 4465 6661 756c 7447 656e 6572  )...DefaultGener
+00000120: 6174 6f72 6300 0000 0000 0000 0000 0000  atorc...........
+00000130: 0000 0000 0003 0000 0040 0000 0073 2a00  .........@...s*.
+00000140: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
+00000150: 5a03 6504 6403 9c01 6404 6405 8404 5a05  Z.e.d...d.d...Z.
+00000160: 6406 6407 8400 5a06 6408 5300 2909 da08  d.d...Z.d.S.)...
+00000170: 496d 706c 4e6f 6465 6301 0000 0000 0000  ImplNodec.......
+00000180: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00000190: 0073 1600 0000 6401 7c00 5f00 6401 7c00  .s....d.|._.d.|.
+000001a0: 5f01 6401 7c00 5f02 6400 5300 a902 4eda  _.d.|._.d.S...N.
+000001b0: 00a9 03da 0b70 6163 6b61 6765 4e61 6d65  .....packageName
+000001c0: da0b 7061 636b 6167 6550 6174 68da 0866  ..packagePath..f
+000001d0: 696c 6550 6174 68a9 01da 0473 656c 66a9  ilePath....self.
+000001e0: 0072 1200 0000 f56e 0000 002f 5573 6572  .r.....n.../User
+000001f0: 732f 7875 6a69 616e 2f44 6f63 756d 656e  s/xujian/Documen
+00000200: 7473 2f32 3032 342f e6a8 a1e5 9d97 e997  ts/2024/........
+00000210: b4e4 baa4 e4ba 92e9 a1b9 e79b ae74 6ce5  .............tl.
+00000220: 8d87 e7ba a72f 7061 636b 6167 655f 746f  ...../package_to
+00000230: 6f6c 732f 7464 665f 746f 6f6c 2f70 6970  ols/tdf_tool/pip
+00000240: 656c 696e 6573 2f61 7069 5f69 6e74 6572  elines/api_inter
+00000250: 6163 7469 6f6e 2e70 79da 085f 5f69 6e69  action.py..__ini
+00000260: 745f 5f0c 0000 0073 0600 0000 0001 0601  t__....s........
+00000270: 0601 7a11 496d 706c 4e6f 6465 2e5f 5f69  ..z.ImplNode.__i
+00000280: 6e69 745f 5fa9 01da 0672 6574 7572 6e63  nit__....returnc
+00000290: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000002a0: 0400 0000 4300 0000 731e 0000 0064 0174  ....C...s....d.t
+000002b0: 007c 006a 01a0 02a1 0083 01a0 03a1 0064  .|.j...........d
+000002c0: 0264 0385 0219 0017 0053 00a9 044e 5a04  .d.......S...NZ.
+000002d0: 6170 695f e908 0000 0069 f8ff ffff a904  api_.....i......
+000002e0: 7202 0000 0072 0f00 0000 da06 656e 636f  r....r......enco
+000002f0: 6465 da09 6865 7864 6967 6573 7472 1000  de..hexdigestr..
+00000300: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00000310: 00da 0869 6d70 6c5f 6d64 3511 0000 0073  ...impl_md5....s
+00000320: 0200 0000 0001 7a11 496d 706c 4e6f 6465  ......z.ImplNode
+00000330: 2e69 6d70 6c5f 6d64 3563 0100 0000 0000  .impl_md5c......
+00000340: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+00000350: 0000 731e 0000 0074 00a0 0164 017c 006a  ..s....t...d.|.j
+00000360: 0217 0064 0217 007c 006a 0317 00a1 0101  ...d...|.j......
+00000370: 0064 0053 00a9 034e 7a08 7061 636b 6167  .d.S...Nz.packag
+00000380: 653a fa01 2fa9 0472 0600 0000 da06 7965  e:../..r......ye
+00000390: 6c6c 6f77 720d 0000 0072 0f00 0000 7210  llowr....r....r.
+000003a0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+000003b0: 0000 da05 7072 696e 7414 0000 0073 0200  ....print....s..
+000003c0: 0000 0001 7a0e 496d 706c 4e6f 6465 2e70  ....z.ImplNode.p
+000003d0: 7269 6e74 4e29 07da 085f 5f6e 616d 655f  rintN)...__name_
+000003e0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+000003f0: 5f71 7561 6c6e 616d 655f 5f72 1400 0000  _qualname__r....
+00000400: da03 7374 7272 1c00 0000 7221 0000 0072  ..strr....r!...r
+00000410: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00000420: 0000 0072 0900 0000 0b00 0000 7306 0000  ...r........s...
+00000430: 0008 0108 050e 0372 0900 0000 6300 0000  .......r....c...
+00000440: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000450: 0040 0000 0073 2a00 0000 6500 5a01 6400  .@...s*...e.Z.d.
+00000460: 5a02 6401 6402 8400 5a03 6504 6403 9c01  Z.d.d...Z.e.d...
+00000470: 6404 6405 8404 5a05 6406 6407 8400 5a06  d.d...Z.d.d...Z.
+00000480: 6408 5300 2909 da07 4170 694e 6f64 6563  d.S.)...ApiNodec
+00000490: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000004a0: 0200 0000 4300 0000 7316 0000 0064 017c  ....C...s....d.|
+000004b0: 005f 0064 017c 005f 0164 017c 005f 0264  ._.d.|._.d.|._.d
+000004c0: 0053 0072 0a00 0000 720c 0000 0072 1000  .S.r....r....r..
+000004d0: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+000004e0: 0072 1400 0000 1900 0000 7306 0000 0000  .r........s.....
+000004f0: 0106 0106 017a 1041 7069 4e6f 6465 2e5f  .....z.ApiNode._
+00000500: 5f69 6e69 745f 5f72 1500 0000 6301 0000  _init__r....c...
+00000510: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+00000520: 0043 0000 0073 1e00 0000 6401 7400 7c00  .C...s....d.t.|.
+00000530: 6a01 a002 a100 8301 a003 a100 6402 6403  j...........d.d.
+00000540: 8502 1900 1700 5300 7217 0000 0072 1900  ......S.r....r..
+00000550: 0000 7210 0000 0072 1200 0000 7212 0000  ..r....r....r...
+00000560: 0072 1300 0000 da07 6170 695f 6d64 351e  .r......api_md5.
+00000570: 0000 0073 0200 0000 0001 7a0f 4170 694e  ...s......z.ApiN
+00000580: 6f64 652e 6170 695f 6d64 3563 0100 0000  ode.api_md5c....
+00000590: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+000005a0: 4300 0000 731e 0000 0074 00a0 0164 017c  C...s....t...d.|
+000005b0: 006a 0217 0064 0217 007c 006a 0317 00a1  .j...d...|.j....
+000005c0: 0101 0064 0053 0072 1d00 0000 721f 0000  ...d.S.r....r...
+000005d0: 0072 1000 0000 7212 0000 0072 1200 0000  .r....r....r....
+000005e0: 7213 0000 0072 2100 0000 2100 0000 7302  r....r!...!...s.
+000005f0: 0000 0000 017a 0d41 7069 4e6f 6465 2e70  .....z.ApiNode.p
+00000600: 7269 6e74 4e29 0772 2200 0000 7223 0000  rintN).r"...r#..
+00000610: 0072 2400 0000 7214 0000 0072 2500 0000  .r$...r....r%...
+00000620: 7227 0000 0072 2100 0000 7212 0000 0072  r'...r!...r....r
+00000630: 1200 0000 7212 0000 0072 1300 0000 7226  ....r....r....r&
+00000640: 0000 0018 0000 0073 0600 0000 0801 0805  .......s........
+00000650: 0e03 7226 0000 0063 0000 0000 0000 0000  ..r&...c........
+00000660: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
+00000670: 7382 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
+00000680: 0364 0264 0384 005a 0464 0464 0584 005a  .d.d...Z.d.d...Z
+00000690: 0564 0664 0784 005a 0664 0864 0984 005a  .d.d...Z.d.d...Z
+000006a0: 0764 0a64 0b84 005a 0864 0c64 0d84 005a  .d.d...Z.d.d...Z
+000006b0: 0964 0e64 0f84 005a 0a64 1064 1184 005a  .d.d...Z.d.d...Z
+000006c0: 0b65 0c65 0c65 0c64 129c 0364 1364 1484  .e.e.e.d...d.d..
+000006d0: 045a 0d64 1564 1684 005a 0e64 1764 1884  .Z.d.d...Z.d.d..
+000006e0: 005a 0f64 1964 1a84 005a 1064 1b64 1c84  .Z.d.d...Z.d.d..
+000006f0: 005a 1164 1d53 0029 1eda 0d41 7069 416e  .Z.d.S.)...ApiAn
+00000700: 6e6f 7461 7469 6f6e 7544 0000 000a 2020  notationuD....  
+00000710: 2020 e6a8 a1e5 9d97 e997 b4e4 baa4 e4ba    ..............
+00000720: 92e6 94af e68c 81e7 9bb8 e585 b3e5 91bd  ................
+00000730: e4bb a4ef bc9a 746c 2061 7069 202d 6820  ......tl api -h 
+00000740: e69f a5e7 9c8b e8af a6e6 8385 0a20 2020  .............   
+00000750: 2063 0100 0000 0000 0000 0000 0000 0100   c..............
+00000760: 0000 0200 0000 4300 0000 7342 0000 0064  ......C...sB...d
+00000770: 007c 005f 0064 017c 005f 0164 027c 005f  .|._.d.|._.d.|._
+00000780: 0267 007c 005f 0364 037c 005f 0467 007c  .g.|._.d.|._.g.|
+00000790: 005f 0564 047c 005f 0664 057c 005f 0767  ._.d.|._.d.|._.g
+000007a0: 007c 005f 087c 00a0 09a1 0001 0064 0053  .|._.|.......d.S
+000007b0: 0029 064e 5a16 4170 6941 6e6e 6f74 6174  .).NZ.ApiAnnotat
+000007c0: 696f 6e47 656e 6572 6174 6f72 7a0e 2e74  ionGeneratorz..t
+000007d0: 6466 5f69 6d70 6c2e 6461 7274 7a0d 2e74  df_impl.dartz..t
+000007e0: 6466 5f61 7069 2e64 6172 745a 0774 6466  df_api.dartZ.tdf
+000007f0: 5f61 7069 5a13 7464 665f 6d6f 6475 6c65  _apiZ.tdf_module
+00000800: 5f61 7069 5f61 6e6e 6f29 0ada 0266 66da  _api_anno)...ff.
+00000810: 195f 4170 6941 6e6e 6f74 6174 696f 6e5f  ._ApiAnnotation_
+00000820: 5f67 656e 6572 6174 6f72 da1a 5f41 7069  _generator.._Api
+00000830: 416e 6e6f 7461 7469 6f6e 5f5f 696d 706c  Annotation__impl
+00000840: 5375 6666 6978 da1c 5f41 7069 416e 6e6f  Suffix.._ApiAnno
+00000850: 7461 7469 6f6e 5f5f 696d 706c 4e6f 6465  tation__implNode
+00000860: 4c69 7374 da19 5f41 7069 416e 6e6f 7461  List.._ApiAnnota
+00000870: 7469 6f6e 5f5f 6170 6953 7566 6669 78da  tion__apiSuffix.
+00000880: 1b5f 4170 6941 6e6e 6f74 6174 696f 6e5f  ._ApiAnnotation_
+00000890: 5f61 7069 4e6f 6465 4c69 7374 da1e 5f41  _apiNodeList.._A
+000008a0: 7069 416e 6e6f 7461 7469 6f6e 5f5f 696e  piAnnotation__in
+000008b0: 7465 7261 6374 696f 6e44 6972 da1e 5f41  teractionDir.._A
+000008c0: 7069 416e 6e6f 7461 7469 6f6e 5f5f 616e  piAnnotation__an
+000008d0: 6e6f 7461 7469 6f6e 4e61 6d65 da1c 5f41  notationName.._A
+000008e0: 7069 416e 6e6f 7461 7469 6f6e 5f5f 7061  piAnnotation__pa
+000008f0: 636b 6167 6573 4c69 7374 da13 6665 7463  ckagesList..fetc
+00000900: 685f 7061 636b 6167 6573 5f6c 6973 7472  h_packages_listr
+00000910: 1000 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00000920: 0000 0072 1400 0000 2a00 0000 7314 0000  ...r....*...s...
+00000930: 0000 0106 0106 0106 0106 0106 0106 0106  ................
+00000940: 0106 0106 027a 1641 7069 416e 6e6f 7461  .....z.ApiAnnota
+00000950: 7469 6f6e 2e5f 5f69 6e69 745f 5f63 0100  tion.__init__c..
+00000960: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000970: 0000 4300 0000 731c 0000 0074 00a0 01a1  ..C...s....t....
+00000980: 0001 0074 0274 03a0 04a1 0083 016a 057c  ...t.t.......j.|
+00000990: 005f 0664 0053 0029 014e 2907 7207 0000  ._.d.S.).N).r...
+000009a0: 00da 0c67 6f49 6e53 6865 6c6c 4469 7272  ...goInShellDirr
+000009b0: 0400 0000 da02 6f73 da06 6765 7463 7764  ......os..getcwd
+000009c0: da08 7061 636b 6167 6573 7231 0000 0072  ..packagesr1...r
+000009d0: 1000 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+000009e0: 0000 0072 3200 0000 3800 0000 7304 0000  ...r2...8...s...
+000009f0: 0000 0108 027a 2141 7069 416e 6e6f 7461  .....z!ApiAnnota
+00000a00: 7469 6f6e 2e66 6574 6368 5f70 6163 6b61  tion.fetch_packa
+00000a10: 6765 735f 6c69 7374 6301 0000 0000 0000  ges_listc.......
+00000a20: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
+00000a30: 0073 5000 0000 7c00 a000 a100 7d01 7401  .sP...|.....}.t.
+00000a40: 6a02 a003 7c01 6401 a102 7d02 7404 7c02  j...|.d...}.t.|.
+00000a50: 6402 8302 7c00 5f05 7c00 a006 a100 0100  d...|._.|.......
+00000a60: 7c00 a007 a100 0100 7c00 a008 a100 0100  |.......|.......
+00000a70: 7c00 6a05 a009 a100 0100 7c00 a00a a100  |.j.......|.....
+00000a80: 0100 6400 5300 2903 4e7a 1161 7069 5f72  ..d.S.).Nz.api_r
+00000a90: 6567 6973 7465 722e 6461 7274 7a02 772b  egister.dartz.w+
+00000aa0: 290b da13 6765 745f 696e 7465 7261 6374  )...get_interact
+00000ab0: 696f 6e5f 6469 7272 3400 0000 da04 7061  ion_dirr4.....pa
+00000ac0: 7468 da04 6a6f 696e da04 6f70 656e 7229  th..join..openr)
+00000ad0: 0000 00da 275f 4170 6941 6e6e 6f74 6174  ....'_ApiAnnotat
+00000ae0: 696f 6e5f 5f69 6e74 6567 7261 7465 5f74  ion__integrate_t
+00000af0: 6466 5f61 7069 5f66 696c 6573 da28 5f41  df_api_files.(_A
+00000b00: 7069 416e 6e6f 7461 7469 6f6e 5f5f 696e  piAnnotation__in
+00000b10: 7465 6772 6174 655f 7464 665f 696d 706c  tegrate_tdf_impl
+00000b20: 5f66 696c 6573 da26 5f41 7069 416e 6e6f  _files.&_ApiAnno
+00000b30: 7461 7469 6f6e 5f5f 6765 6e65 7261 7465  tation__generate
+00000b40: 5f72 6567 6973 7465 725f 636f 6465 da05  _register_code..
+00000b50: 636c 6f73 65da 0a5f 5f66 6f72 6d61 745f  close..__format_
+00000b60: 5f29 0372 1100 0000 5a0b 7464 665f 6170  _).r....Z.tdf_ap
+00000b70: 695f 6469 725a 1261 7574 6f5f 7265 6769  i_dirZ.auto_regi
+00000b80: 7374 6572 5f66 696c 6572 1200 0000 7212  ster_filer....r.
+00000b90: 0000 0072 1300 0000 da0f 696e 7465 6772  ...r......integr
+00000ba0: 6174 655f 7368 656c 6c3e 0000 0073 1000  ate_shell>...s..
+00000bb0: 0000 0002 0801 0e01 0c03 0803 0803 0802  ................
+00000bc0: 0a03 7a1d 4170 6941 6e6e 6f74 6174 696f  ..z.ApiAnnotatio
+00000bd0: 6e2e 696e 7465 6772 6174 655f 7368 656c  n.integrate_shel
+00000be0: 6c63 0100 0000 0000 0000 0000 0000 0300  lc..............
+00000bf0: 0000 0800 0000 4300 0000 739c 0000 007c  ......C...s....|
+00000c00: 006a 00a0 0174 02a0 037c 006a 04a1 01a1  .j...t...|.j....
+00000c10: 0101 007c 006a 0544 005d 1e7d 017c 00a0  ...|.j.D.].}.|..
+00000c20: 067c 006a 007c 016a 077c 016a 087c 01a0  .|.j.|.j.|.j.|..
+00000c30: 09a1 00a1 0401 0071 1a7c 006a 0a44 005d  .......q.|.j.D.]
+00000c40: 1e7d 017c 00a0 067c 006a 007c 016a 077c  .}.|...|.j.|.j.|
+00000c50: 016a 087c 01a0 0ba1 00a1 0401 0071 407c  .j.|.........q@|
+00000c60: 00a0 0c7c 006a 007c 006a 0d7c 006a 0d64  ...|.j.|.j.|.j.d
+00000c70: 0117 00a1 0301 0064 027d 027c 006a 00a0  .......d.}.|.j..
+00000c80: 017c 02a0 0e7c 00a0 0fa1 007c 00a0 10a1  .|...|.....|....
+00000c90: 00a1 02a1 0101 0064 0053 0029 034e 7a05  .......d.S.).Nz.
+00000ca0: 2e64 6172 7475 8e02 0000 0a20 2020 2020  .dartu.....     
+00000cb0: 2020 200a 2020 2020 2020 2020 636c 6173     .        clas
+00000cc0: 7320 5444 4641 7069 496d 706c 4175 746f  s TDFApiImplAuto
+00000cd0: 5265 6769 7374 6572 207b 7b0a 2020 2020  Register {{.    
+00000ce0: 2020 2020 2020 7374 6174 6963 204c 6973        static Lis
+00000cf0: 743c 5479 7065 3e20 6170 6973 203d 205b  t<Type> apis = [
+00000d00: 0a20 2020 2020 2020 2020 2020 207b 307d  .            {0}
+00000d10: 0a20 2020 2020 2020 2020 205d 3b0a 2020  .          ];.  
+00000d20: 2020 2020 2020 2020 2f2f 20e7 a1ae e4bf          // .....
+00000d30: 9de6 8980 e69c 89e8 a2ab e5bc 95e7 94a8  ................
+00000d40: e79a 8461 7069 e5ba 93e7 9a84 e5ae 9ee7  ...api..........
+00000d50: 8eb0 e7b1 bbe9 83bd e5b7 b2e6 b3a8 e586  ................
+00000d60: 8c0a 2020 2020 2020 2020 2020 7374 6174  ..          stat
+00000d70: 6963 2076 6f69 6420 5f65 6e73 7572 6541  ic void _ensureA
+00000d80: 7069 496d 706c 5265 6769 7374 6572 2829  piImplRegister()
+00000d90: 207b 7b0a 2020 2020 2020 2020 2020 2020   {{.            
+00000da0: 6170 6973 2e66 6f72 4561 6368 2828 656c  apis.forEach((el
+00000db0: 656d 656e 7429 207b 7b0a 2020 2020 2020  ement) {{.      
+00000dc0: 2020 2020 2020 2020 6966 2028 2141 7069          if (!Api
+00000dd0: 5265 6769 7374 6572 4365 6e74 6572 2e6b  RegisterCenter.k
+00000de0: 6579 732e 636f 6e74 6169 6e73 2865 6c65  eys.contains(ele
+00000df0: 6d65 6e74 2929 207b 7b0a 2020 2020 2020  ment)) {{.      
+00000e00: 2020 2020 2020 2020 2020 7468 726f 7720            throw 
+00000e10: 4578 6365 7074 696f 6e28 2224 7b7b 656c  Exception("${{el
+00000e20: 656d 656e 747d 7de7 9a84 e5ae 9ee7 8eb0  ement}}.........
+00000e30: e7b1 bbe6 9caa e69c aae6 b3a8 e586 8cef  ................
+00000e40: bc81 efbc 81ef bc81 e8af b7e5 88a0 e999  ................
+00000e50: a4e5 ba93 247b 7b65 6c65 6d65 6e74 7d7d  ....${{element}}
+00000e60: e79a 84e5 bc95 e794 a8e6 8896 e880 85e5  ................
+00000e70: bc95 e585 a5e5 ae9e e78e b0e7 b1bb 2229  ..............")
+00000e80: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00000e90: 7d7d 0a20 2020 2020 2020 2020 2020 207d  }}.            }
+00000ea0: 7d29 3b0a 2020 2020 2020 2020 2020 7d7d  });.          }}
+00000eb0: 0a0a 2020 2020 2020 2020 2020 7374 6174  ..          stat
+00000ec0: 6963 2076 6f69 6420 6175 746f 5265 6769  ic void autoRegi
+00000ed0: 7374 6572 2829 207b 7b0a 2020 2020 2020  ster() {{.      
+00000ee0: 2020 2020 2020 2020 7b31 7d0a 2020 2020          {1}.    
+00000ef0: 2020 2020 2020 2020 2020 5f65 6e73 7572            _ensur
+00000f00: 6541 7069 496d 706c 5265 6769 7374 6572  eApiImplRegister
+00000f10: 2829 3b0a 2020 2020 2020 2020 2020 7d7d  ();.          }}
+00000f20: 0a20 2020 2020 2020 207d 7d0a 2020 2020  .        }}.    
+00000f30: 2020 2020 2020 2020 2911 7229 0000 00da          ).r)....
+00000f40: 0577 7269 7465 7208 0000 005a 1064 6566  .writer....Z.def
+00000f50: 6175 6c74 5469 746c 6544 6573 6372 2a00  aultTitleDescr*.
+00000f60: 0000 722c 0000 00da 255f 4170 6941 6e6e  ..r,....%_ApiAnn
+00000f70: 6f74 6174 696f 6e5f 5f5f 5f69 6d70 6f72  otation____impor
+00000f80: 745f 6461 7461 5f63 7265 6174 6f72 720d  t_data_creatorr.
+00000f90: 0000 0072 0f00 0000 721c 0000 0072 2e00  ...r....r....r..
+00000fa0: 0000 7227 0000 00da 315f 4170 6941 6e6e  ..r'....1_ApiAnn
+00000fb0: 6f74 6174 696f 6e5f 5f69 6d70 6f72 745f  otation__import_
+00000fc0: 6461 7461 5f63 7265 6174 6f72 5f77 6974  data_creator_wit
+00000fd0: 686f 7574 5f61 6c69 6173 7230 0000 00da  hout_aliasr0....
+00000fe0: 0666 6f72 6d61 74da 1061 7069 5f6c 6973  .format..api_lis
+00000ff0: 745f 6372 6561 746f 72da 255f 4170 6941  t_creator.%_ApiA
+00001000: 6e6e 6f74 6174 696f 6e5f 5f72 6567 6973  nnotation__regis
+00001010: 7465 725f 6c69 7374 5f63 7265 6174 6f72  ter_list_creator
+00001020: 2903 7211 0000 005a 055f 6974 656d da07  ).r....Z._item..
+00001030: 636f 6e74 656e 7472 1200 0000 7212 0000  contentr....r...
+00001040: 0072 1300 0000 5a18 5f5f 6765 6e65 7261  .r....Z.__genera
+00001050: 7465 5f72 6567 6973 7465 725f 636f 6465  te_register_code
+00001060: 5200 0000 731a 0000 0000 0114 020a 011c  R...s...........
+00001070: 010a 011c 0218 0204 1506 0104 0106 0106  ................
+00001080: fe02 ff7a 2641 7069 416e 6e6f 7461 7469  ...z&ApiAnnotati
+00001090: 6f6e 2e5f 5f67 656e 6572 6174 655f 7265  on.__generate_re
+000010a0: 6769 7374 6572 5f63 6f64 6563 0100 0000  gister_codec....
+000010b0: 0000 0000 0000 0000 0300 0000 0700 0000  ................
+000010c0: 4300 0000 732c 0000 0064 017d 017c 006a  C...s,...d.}.|.j
+000010d0: 0044 005d 1c7d 027c 0164 02a0 017c 02a0  .D.].}.|.d...|..
+000010e0: 02a1 007c 02a0 02a1 00a1 0237 007d 0171  ...|.......7.}.q
+000010f0: 0a7c 0153 0029 034e 720b 0000 007a 690a  .|.S.).Nr....zi.
+00001100: 2020 2020 2020 2020 2020 2020 4170 6952              ApiR
+00001110: 6567 6973 7465 7243 656e 7465 722e 7265  egisterCenter.re
+00001120: 6769 7374 6572 287b 307d 2e41 7574 6f52  gister({0}.AutoR
+00001130: 6567 6973 7465 722e 6170 6954 7970 652c  egister.apiType,
+00001140: 7b31 7d2e 4175 746f 5265 6769 7374 6572  {1}.AutoRegister
+00001150: 2e70 726f 7669 6465 7229 3b0a 2020 2020  .provider);.    
+00001160: 2020 2020 2020 2020 2903 722c 0000 0072          ).r,...r
+00001170: 4400 0000 721c 0000 00a9 0372 1100 0000  D...r......r....
+00001180: 7247 0000 00da 0469 7465 6d72 1200 0000  rG.....itemr....
+00001190: 7212 0000 0072 1300 0000 5a17 5f5f 7265  r....r....Z.__re
+000011a0: 6769 7374 6572 5f6c 6973 745f 6372 6561  gister_list_crea
+000011b0: 746f 7276 0000 0073 0c00 0000 0001 0401  torv...s........
+000011c0: 0a01 0602 0cfe 0803 7a25 4170 6941 6e6e  ........z%ApiAnn
+000011d0: 6f74 6174 696f 6e2e 5f5f 7265 6769 7374  otation.__regist
+000011e0: 6572 5f6c 6973 745f 6372 6561 746f 7263  er_list_creatorc
+000011f0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00001200: 0600 0000 4300 0000 7326 0000 0064 017d  ....C...s&...d.}
+00001210: 017c 006a 0044 005d 167d 027c 0164 02a0  .|.j.D.].}.|.d..
+00001220: 017c 02a0 02a1 00a1 0137 007d 0171 0a7c  .|.......7.}.q.|
+00001230: 0153 0029 034e 720b 0000 007a 430a 2020  .S.).Nr....zC.  
+00001240: 2020 2020 2020 2020 2020 7b30 7d2e 5444            {0}.TD
+00001250: 4641 7069 4175 746f 496e 7661 6c69 6461  FApiAutoInvalida
+00001260: 7465 2e61 7069 5479 7065 2c0a 2020 2020  te.apiType,.    
+00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001280: 2903 722e 0000 0072 4400 0000 7227 0000  ).r....rD...r'..
+00001290: 0072 4800 0000 7212 0000 0072 1200 0000  .rH...r....r....
+000012a0: 7213 0000 0072 4500 0000 7e00 0000 730c  r....rE...~...s.
+000012b0: 0000 0000 0104 010a 0106 0206 fe08 037a  ...............z
+000012c0: 1e41 7069 416e 6e6f 7461 7469 6f6e 2e61  .ApiAnnotation.a
+000012d0: 7069 5f6c 6973 745f 6372 6561 746f 7263  pi_list_creatorc
+000012e0: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+000012f0: 0500 0000 4300 0000 7362 0000 0074 00a0  ....C...sb...t..
+00001300: 0164 01a1 0101 007c 006a 0244 005d 4c7d  .d.....|.j.D.]L}
+00001310: 017c 00a0 037c 016a 047c 006a 05a1 027d  .|...|.j.|.j...}
+00001320: 027c 0264 0075 0172 1074 0683 007d 037c  .|.d.u.r.t...}.|
+00001330: 016a 047c 035f 047c 016a 077c 035f 077c  .j.|._.|.j.|._.|
+00001340: 027c 035f 087c 03a0 09a1 0001 007c 006a  .|._.|.......|.j
+00001350: 0aa0 0b7c 03a1 0101 0071 1064 0053 0029  ...|.....q.d.S.)
+00001360: 024e 751c 0000 00e6 95b4 e590 88e6 8980  .Nu.............
+00001370: e69c 89e4 baa4 e4ba 9269 6d70 6ce6 9687  .........impl...
+00001380: e4bb b629 0c72 0600 0000 da05 7469 746c  ...).r......titl
+00001390: 6572 3100 0000 da1f 5f41 7069 416e 6e6f  er1....._ApiAnno
+000013a0: 7461 7469 6f6e 5f5f 6765 745f 7461 7267  tation__get_targ
+000013b0: 6574 5f66 696c 6572 0e00 0000 722b 0000  et_filer....r+..
+000013c0: 0072 0900 0000 720d 0000 0072 0f00 0000  .r....r....r....
+000013d0: 7221 0000 0072 2c00 0000 da06 6170 7065  r!...r,.....appe
+000013e0: 6e64 2904 7211 0000 00da 0b70 6163 6b61  nd).r......packa
+000013f0: 6765 4974 656d da19 5f41 7069 416e 6e6f  geItem.._ApiAnno
+00001400: 7461 7469 6f6e 5f5f 6669 6c65 5f70 6174  tation__file_pat
+00001410: 685a 095f 696d 706c 4e6f 6465 7212 0000  hZ._implNoder...
+00001420: 0072 1200 0000 7213 0000 005a 1a5f 5f69  .r....r....Z.__i
+00001430: 6e74 6567 7261 7465 5f74 6466 5f69 6d70  ntegrate_tdf_imp
+00001440: 6c5f 6669 6c65 7386 0000 0073 1400 0000  l_files....s....
+00001450: 0001 0a01 0a01 1001 0801 0601 0801 0801  ................
+00001460: 0601 0801 7a28 4170 6941 6e6e 6f74 6174  ....z(ApiAnnotat
+00001470: 696f 6e2e 5f5f 696e 7465 6772 6174 655f  ion.__integrate_
+00001480: 7464 665f 696d 706c 5f66 696c 6573 6301  tdf_impl_filesc.
+00001490: 0000 0000 0000 0000 0000 0004 0000 0005  ................
+000014a0: 0000 0043 0000 0073 6200 0000 7400 a001  ...C...sb...t...
+000014b0: 6401 a101 0100 7c00 6a02 4400 5d4c 7d01  d.....|.j.D.]L}.
+000014c0: 7c00 a003 7c01 6a04 7c00 6a05 a102 7d02  |...|.j.|.j...}.
+000014d0: 7c02 6400 7501 7210 7406 8300 7d03 7c01  |.d.u.r.t...}.|.
+000014e0: 6a04 7c03 5f04 7c01 6a07 7c03 5f07 7c02  j.|._.|.j.|._.|.
+000014f0: 7c03 5f08 7c03 a009 a100 0100 7c00 6a0a  |._.|.......|.j.
+00001500: a00b 7c03 a101 0100 7110 6400 5300 2902  ..|.....q.d.S.).
+00001510: 4e75 1b00 0000 e695 b4e5 9088 e689 80e6  Nu..............
+00001520: 9c89 e4ba a4e4 ba92 6170 69e6 9687 e4bb  ........api.....
+00001530: b629 0c72 0600 0000 724a 0000 0072 3100  .).r....rJ...r1.
+00001540: 0000 724b 0000 0072 0e00 0000 722d 0000  ..rK...r....r-..
+00001550: 0072 2600 0000 720d 0000 0072 0f00 0000  .r&...r....r....
+00001560: 7221 0000 0072 2e00 0000 724c 0000 0029  r!...r....rL...)
+00001570: 0472 1100 0000 724d 0000 0072 4e00 0000  .r....rM...rN...
+00001580: 5a08 5f61 7069 4e6f 6465 7212 0000 0072  Z._apiNoder....r
+00001590: 1200 0000 7213 0000 005a 195f 5f69 6e74  ....r....Z.__int
+000015a0: 6567 7261 7465 5f74 6466 5f61 7069 5f66  egrate_tdf_api_f
+000015b0: 696c 6573 9200 0000 7314 0000 0000 010a  iles....s.......
+000015c0: 010a 0110 0108 0106 0108 0108 0106 0108  ................
+000015d0: 017a 2741 7069 416e 6e6f 7461 7469 6f6e  .z'ApiAnnotation
+000015e0: 2e5f 5f69 6e74 6567 7261 7465 5f74 6466  .__integrate_tdf
+000015f0: 5f61 7069 5f66 696c 6573 2903 da09 6669  _api_files)...fi
+00001600: 6c65 5f70 6174 68da 0673 7566 6669 7872  le_path..suffixr
+00001610: 1600 0000 6303 0000 0000 0000 0000 0000  ....c...........
+00001620: 000c 0000 0006 0000 0043 0000 0073 ce00  .........C...s..
+00001630: 0000 7400 a001 a100 0100 7402 a003 7c01  ..t.......t...|.
+00001640: a101 0100 6401 7d03 7402 a004 7405 a006  ....d.}.t...t...
+00001650: a100 a101 a007 a100 a008 6402 a101 6401  ..........d...d.
+00001660: 1900 7d04 7402 a009 7c04 a101 4400 5d66  ..}.t...|...D.]f
+00001670: 5c03 7d05 7d06 7d07 7c07 4400 5d56 7d08  \.}.}.}.|.D.]V}.
+00001680: 7402 6a0a a00b 7c05 7c08 a102 7d09 7c09  t.j...|.|...}.|.
+00001690: a00c 7c02 a101 724a 7c03 6403 3700 7d03  ..|...rJ|.d.7.}.
+000016a0: 7405 a00d a100 7292 7c09 a008 6404 a101  t.....r.|...d...
+000016b0: 6403 1900 7d0a 7c0a a00e 6405 6406 a102  d...}.|...d.d...
+000016c0: 7d0b 714a 7c09 a008 6407 a101 6403 1900  }.qJ|...d...d...
+000016d0: 7d0b 714a 713c 7c03 6403 6b02 72b0 7c0b  }.qJq<|.d.k.r.|.
+000016e0: 5300 7c03 6403 6b04 72ca 740f 6408 a010  S.|.d.k.r.t.d...
+000016f0: 7c01 a101 8301 8201 6400 5300 6400 5300  |.......d.S.d.S.
+00001700: 2909 4e72 0100 0000 da01 0ae9 0100 0000  ).Nr............
+00001710: 7a05 5c6c 6962 5cfa 015c 721e 0000 007a  z.\lib\..\r....z
+00001720: 052f 6c69 622f 7530 0000 00e6 a8a1 e59d  ./lib/u0........
+00001730: 977b 307d e5ad 98e5 9ca8 e5a4 9ae4 b8aa  .{0}............
+00001740: e4ba a4e4 ba92 e696 87e4 bbb6 efbc 8ce8  ................
+00001750: afb7 e6a3 80e6 9fa5 e29d 8c29 1172 0700  ...........).r..
+00001760: 0000 7233 0000 0072 3400 0000 da05 6368  ..r3...r4.....ch
+00001770: 6469 72da 0570 6f70 656e 7205 0000 00da  dir..popenr.....
+00001780: 0770 7764 5f63 6d64 da04 7265 6164 da05  .pwd_cmd..read..
+00001790: 7370 6c69 74da 0477 616c 6b72 3800 0000  split..walkr8...
+000017a0: 7239 0000 00da 0865 6e64 7377 6974 68da  r9.....endswith.
+000017b0: 0a69 735f 7769 6e64 6f77 73da 0772 6570  .is_windows..rep
+000017c0: 6c61 6365 da09 4578 6365 7074 696f 6e72  lace..Exceptionr
+000017d0: 4400 0000 290c 7211 0000 0072 4f00 0000  D...).r....rO...
+000017e0: 7250 0000 00da 0563 6f75 6e74 da08 6e6f  rP.....count..no
+000017f0: 7761 5061 7468 da04 726f 6f74 da04 6469  waPath..root..di
+00001800: 7273 da05 6669 6c65 73da 0466 696c 65da  rs..files..file.
+00001810: 0873 7263 5f66 696c 65da 0474 656d 705a  .src_file..tempZ
+00001820: 1b5f 4170 6941 6e6e 6f74 6174 696f 6e5f  ._ApiAnnotation_
+00001830: 5f74 6172 6765 745f 6669 6c65 7212 0000  _target_filer...
+00001840: 0072 1200 0000 7213 0000 005a 115f 5f67  .r....r....Z.__g
+00001850: 6574 5f74 6172 6765 745f 6669 6c65 9f00  et_target_file..
+00001860: 0000 7326 0000 0000 0108 010a 0204 021c  ..s&............
+00001870: 0114 0108 010e 010a 0108 0108 010e 010e  ................
+00001880: 0212 0108 0104 0108 010e 0104 017a 1f41  .............z.A
+00001890: 7069 416e 6e6f 7461 7469 6f6e 2e5f 5f67  piAnnotation.__g
+000018a0: 6574 5f74 6172 6765 745f 6669 6c65 6301  et_target_filec.
+000018b0: 0000 0000 0000 0000 0000 0001 0000 0005  ................
+000018c0: 0000 0043 0000 0073 4e00 0000 7400 a001  ...C...sN...t...
+000018d0: a100 0100 7402 a003 6401 a101 0100 7402  ....t...d.....t.
+000018e0: 6a04 a005 7c00 6a06 a101 722c 7407 a008  j...|.j...r,t...
+000018f0: 7c00 6a06 a101 0100 7402 a009 7c00 6a06  |.j.....t...|.j.
+00001900: a101 0100 7402 6a04 a00a 7400 a00b a100  ....t.j...t.....
+00001910: 6401 7c00 6a06 a103 5300 2902 4eda 036c  d.|.j...S.).N..l
+00001920: 6962 290c 7207 0000 0072 3300 0000 7234  ib).r....r3...r4
+00001930: 0000 0072 5400 0000 7238 0000 00da 0665  ...rT...r8.....e
+00001940: 7869 7374 7372 2f00 0000 da06 7368 7574  xistsr/.....shut
+00001950: 696c da06 726d 7472 6565 da05 6d6b 6469  il..rmtree..mkdi
+00001960: 7272 3900 0000 da0b 6765 7453 6865 6c6c  rr9.....getShell
+00001970: 4469 7272 1000 0000 7212 0000 0072 1200  Dirr....r....r..
+00001980: 0000 7213 0000 0072 3700 0000 b700 0000  ..r....r7.......
+00001990: 730c 0000 0000 0108 010a 010e 010c 010c  s...............
+000019a0: 017a 2141 7069 416e 6e6f 7461 7469 6f6e  .z!ApiAnnotation
+000019b0: 2e67 6574 5f69 6e74 6572 6163 7469 6f6e  .get_interaction
+000019c0: 5f64 6972 6301 0000 0000 0000 0000 0000  _dirc...........
+000019d0: 0002 0000 0005 0000 0043 0000 0073 3200  .........C...s2.
+000019e0: 0000 7400 a001 a100 0100 7402 6a03 a004  ..t.......t.j...
+000019f0: 7400 a005 a100 6401 7c00 6a06 a103 7d01  t.....d.|.j...}.
+00001a00: 7402 a007 6402 a008 7c01 a101 a101 0100  t...d...|.......
+00001a10: 6400 5300 2903 4e72 6600 0000 7a0f 6461  d.S.).Nrf...z.da
+00001a20: 7274 2066 6f72 6d61 7420 7b30 7d29 0972  rt format {0}).r
+00001a30: 0700 0000 da0f 676f 496e 5368 656c 6c4c  ......goInShellL
+00001a40: 6962 4469 7272 3400 0000 7238 0000 0072  ibDirr4...r8...r
+00001a50: 3900 0000 726b 0000 0072 2f00 0000 da06  9...rk...r/.....
+00001a60: 7379 7374 656d 7244 0000 0029 0272 1100  systemrD...).r..
+00001a70: 0000 5a14 5f41 7069 416e 6e6f 7461 7469  ..Z._ApiAnnotati
+00001a80: 6f6e 5f5f 7061 7468 7212 0000 0072 1200  on__pathr....r..
+00001a90: 0000 7213 0000 0072 3f00 0000 c000 0000  ..r....r?.......
+00001aa0: 7306 0000 0000 0108 0116 017a 1841 7069  s..........z.Api
+00001ab0: 416e 6e6f 7461 7469 6f6e 2e5f 5f66 6f72  Annotation.__for
+00001ac0: 6d61 745f 5f63 0500 0000 0000 0000 0000  mat__c..........
+00001ad0: 0000 0500 0000 0700 0000 4300 0000 7318  ..........C...s.
+00001ae0: 0000 007c 01a0 0064 01a0 017c 027c 037c  ...|...d...|.|.|
+00001af0: 04a1 03a1 0101 0064 0053 0029 024e 7a21  .......d.S.).Nz!
+00001b00: 696d 706f 7274 2022 7061 636b 6167 653a  import "package:
+00001b10: 7b30 7d2f 7b31 7d22 2061 7320 7b32 7d3b  {0}/{1}" as {2};
+00001b20: 0aa9 0272 4100 0000 7244 0000 0029 0572  ...rA...rD...).r
+00001b30: 1100 0000 da07 665f 7772 6974 65da 0b6d  ......f_write..m
+00001b40: 6f64 756c 655f 6e61 6d65 724f 0000 00da  odule_namerO....
+00001b50: 0561 6c69 6173 7212 0000 0072 1200 0000  .aliasr....r....
+00001b60: 7213 0000 005a 175f 5f5f 5f69 6d70 6f72  r....Z.____impor
+00001b70: 745f 6461 7461 5f63 7265 6174 6f72 c600  t_data_creator..
+00001b80: 0000 730a 0000 0000 0304 0104 0106 ff02  ..s.............
+00001b90: ff7a 2541 7069 416e 6e6f 7461 7469 6f6e  .z%ApiAnnotation
+00001ba0: 2e5f 5f5f 5f69 6d70 6f72 745f 6461 7461  .____import_data
+00001bb0: 5f63 7265 6174 6f72 6304 0000 0000 0000  _creatorc.......
+00001bc0: 0000 0000 0004 0000 0006 0000 0043 0000  .............C..
+00001bd0: 0073 1600 0000 7c01 a000 6401 a001 7c02  .s....|...d...|.
+00001be0: 7c03 a102 a101 0100 6400 5300 2902 4e7a  |.......d.S.).Nz
+00001bf0: 1a69 6d70 6f72 7420 2270 6163 6b61 6765  .import "package
+00001c00: 3a7b 307d 2f7b 317d 223b 0a72 6e00 0000  :{0}/{1}";.rn...
+00001c10: 2904 7211 0000 0072 6f00 0000 7270 0000  ).r....ro...rp..
+00001c20: 0072 4f00 0000 7212 0000 0072 1200 0000  .rO...r....r....
+00001c30: 7213 0000 005a 235f 5f69 6d70 6f72 745f  r....Z#__import_
+00001c40: 6461 7461 5f63 7265 6174 6f72 5f77 6974  data_creator_wit
+00001c50: 686f 7574 5f61 6c69 6173 d000 0000 730a  hout_alias....s.
+00001c60: 0000 0000 0304 0104 0104 ff02 ff7a 3141  .............z1A
+00001c70: 7069 416e 6e6f 7461 7469 6f6e 2e5f 5f69  piAnnotation.__i
+00001c80: 6d70 6f72 745f 6461 7461 5f63 7265 6174  mport_data_creat
+00001c90: 6f72 5f77 6974 686f 7574 5f61 6c69 6173  or_without_alias
+00001ca0: 4e29 1272 2200 0000 7223 0000 0072 2400  N).r"...r#...r$.
+00001cb0: 0000 da07 5f5f 646f 635f 5f72 1400 0000  ....__doc__r....
+00001cc0: 7232 0000 0072 4000 0000 723d 0000 0072  r2...r@...r=...r
+00001cd0: 4600 0000 7245 0000 0072 3c00 0000 723b  F...rE...r<...r;
+00001ce0: 0000 0072 2500 0000 724b 0000 0072 3700  ...r%...rK...r7.
+00001cf0: 0000 723f 0000 0072 4200 0000 7243 0000  ..r?...rB...rC..
+00001d00: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
+00001d10: 7213 0000 0072 2800 0000 2500 0000 731c  r....r(...%...s.
+00001d20: 0000 0008 0104 0408 0e08 0608 1408 2408  ..............$.
+00001d30: 0808 0808 0c08 0d12 1808 0908 0608 0a72  ...............r
+00001d40: 2800 0000 2912 da07 6861 7368 6c69 6272  (...)...hashlibr
+00001d50: 0200 0000 7234 0000 0072 6800 0000 da25  ....r4...rh....%
+00001d60: 7464 665f 746f 6f6c 2e74 6f6f 6c73 2e63  tdf_tool.tools.c
+00001d70: 6f6e 6669 672e 7061 636b 6167 6573 5f63  onfig.packages_c
+00001d80: 6f6e 6669 6772 0300 0000 7204 0000 00da  onfigr....r.....
+00001d90: 1d74 6466 5f74 6f6f 6c2e 746f 6f6c 732e  .tdf_tool.tools.
+00001da0: 706c 6174 666f 726d 5f74 6f6f 6c73 7205  platform_toolsr.
+00001db0: 0000 00da 1474 6466 5f74 6f6f 6c2e 746f  .....tdf_tool.to
+00001dc0: 6f6c 732e 7072 696e 7472 0600 0000 da18  ols.printr......
+00001dd0: 7464 665f 746f 6f6c 2e74 6f6f 6c73 2e73  tdf_tool.tools.s
+00001de0: 6865 6c6c 5f64 6972 7207 0000 005a 1874  hell_dirr....Z.t
+00001df0: 6466 5f74 6f6f 6c2e 746f 6f6c 732e 6765  df_tool.tools.ge
+00001e00: 6e65 7261 746f 7272 0800 0000 7209 0000  neratorr....r...
+00001e10: 0072 2600 0000 7228 0000 0072 1200 0000  .r&...r(...r....
+00001e20: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
+00001e30: 083c 6d6f 6475 6c65 3e01 0000 0073 1400  .<module>....s..
+00001e40: 0000 0c01 0801 0801 1001 0c01 0c01 0c01  ................
+00001e50: 0c03 0e0d 0e0d                           ......
```

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 18 09:17:03 2024 UTC, .py size: 1244 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 0fe5 2066 dc04 0000  a......... f....
+00000000: 610d 0d0a 0000 0000 04e9 2066 dc04 0000  a......... f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 8302 5a0a 6407 5300 2908 e900 0000 0029  ..Z.d.S.)......)
```

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 18 09:16:07 2024 UTC, .py size: 1211 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d7e4 2066 bb04 0000  a......... f....
+00000000: 610d 0d0a 0000 0000 04e9 2066 bb04 0000  a......... f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 8302 5a09  ..G.d.d...d...Z.
 00000070: 6407 5300 2908 e900 0000 0029 01da 1149  d.S.)......)...I
```

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 18 09:24:14 2024 UTC, .py size: 1889 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 bee6 2066 6107 0000  a......... fa...
+00000000: 610d 0d0a 0000 0000 04e9 2066 6107 0000  a......... fa...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6406 6407 8400 6407 8302 5a0b 6408 5300  d.d...d...Z.d.S.
```

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 18 09:16:33 2024 UTC, .py size: 1630 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 f1e4 2066 5e06 0000  a......... f^...
+00000000: 610d 0d0a 0000 0000 04e9 2066 5e06 0000  a......... f^...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6406 6407 8400 6407 8302 5a0b 6401 5300  d.d...d...Z.d.S.
```

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 17 08:02:42 2024 UTC, .py size: 22055 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,1016 +1,1003 @@
-00000000: 610d 0d0a 0000 0000 2282 1f66 2756 0000  a......."..f'V..
+00000000: 610d 0d0a 0000 0000 1c29 2266 7e55 0000  a........)"f~U..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a04 6400  m.Z...d.d.l.Z.d.
-00000050: 6403 6c05 5a05 6400 6403 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
-00000060: 6404 6c07 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
-00000070: 6d0a 5a0a 6d0b 5a0b 0100 6400 6406 6c0c  m.Z.m.Z...d.d.l.
-00000080: 6d0d 5a0d 6d0e 5a0e 0100 6400 6407 6c0f  m.Z.m.Z...d.d.l.
-00000090: 6d10 5a10 0100 6400 6408 6c11 6d12 5a12  m.Z...d.d.l.m.Z.
-000000a0: 0100 6400 6409 6c13 6d14 5a14 0100 4700  ..d.d.l.m.Z...G.
-000000b0: 640a 640b 8400 640b 8302 5a15 4700 640c  d.d...d...Z.G.d.
-000000c0: 640d 8400 640d 8302 5a16 6403 5300 290e  d...d...Z.d.S.).
-000000d0: e900 0000 0029 01da 036d 6435 2901 da0d  .....)...md5)...
-000000e0: 5465 7874 494f 5772 6170 7065 724e 2901  TextIOWrapperN).
-000000f0: da11 496e 6974 6961 6c4a 736f 6e43 6f6e  ..InitialJsonCon
-00000100: 6669 6729 02da 0e4d 6f64 756c 6549 7465  fig)...ModuleIte
-00000110: 6d54 7970 65da 104d 6f64 756c 654a 736f  mType..ModuleJso
-00000120: 6e43 6f6e 6669 6729 02da 0b50 6163 6b61  nConfig)...Packa
-00000130: 6765 4e6f 6465 da12 5061 636b 6167 6573  geNode..Packages
-00000140: 4a73 6f6e 436f 6e66 6967 2901 da0d 506c  JsonConfig)...Pl
-00000150: 6174 666f 726d 546f 6f6c 7329 01da 0550  atformTools)...P
-00000160: 7269 6e74 2901 da08 5368 656c 6c44 6972  rint)...ShellDir
-00000170: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000180: 0002 0000 0040 0000 0073 1400 0000 6500  .....@...s....e.
-00000190: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
-000001a0: 5300 2904 da0a 526f 7574 6572 4e6f 6465  S.)...RouterNode
-000001b0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000001c0: 0002 0000 0043 0000 0073 2800 0000 6401  .....C...s(...d.
-000001d0: 7c00 5f00 6401 7c00 5f01 6401 7c00 5f02  |._.d.|._.d.|._.
-000001e0: 6401 7c00 5f03 6401 7c00 5f04 6402 7c00  d.|._.d.|._.d.|.
-000001f0: 5f05 6400 5300 2903 4eda 0046 2906 da07  _.d.S.).N..F)...
-00000200: 7061 636b 6167 65da 0a72 6f75 7465 7250  package..routerP
-00000210: 6174 68da 0866 696c 6550 6174 68da 046e  ath..filePath..n
-00000220: 6f74 65da 0a70 6167 6557 6964 6765 74da  ote..pageWidget.
-00000230: 0a69 734d 6169 6e50 6167 65a9 01da 0473  .isMainPage....s
-00000240: 656c 66a9 0072 1600 0000 f565 0000 002f  elf..r.....e.../
-00000250: 5573 6572 732f 7875 6a69 616e 2f44 6f63  Users/xujian/Doc
-00000260: 756d 656e 7473 2f32 3032 342f e6a8 a1e5  uments/2024/....
-00000270: 9d97 e997 b4e4 baa4 e4ba 92e9 a1b9 e79b  ................
-00000280: ae74 6ce5 8d87 e7ba a72f 7061 636b 6167  .tl....../packag
-00000290: 655f 746f 6f6c 732f 7464 665f 746f 6f6c  e_tools/tdf_tool
-000002a0: 2f70 6970 656c 696e 6573 2f72 6f75 7465  /pipelines/route
-000002b0: 722e 7079 da08 5f5f 696e 6974 5f5f 0f00  r.py..__init__..
-000002c0: 0000 730c 0000 0000 0106 0106 0106 0106  ..s.............
-000002d0: 0106 017a 1352 6f75 7465 724e 6f64 652e  ...z.RouterNode.
-000002e0: 5f5f 696e 6974 5f5f 4e29 04da 085f 5f6e  __init__N)...__n
-000002f0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000300: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00000310: 1800 0000 7216 0000 0072 1600 0000 7216  ....r....r....r.
-00000320: 0000 0072 1700 0000 720c 0000 000e 0000  ...r....r.......
-00000330: 0073 0200 0000 0801 720c 0000 0063 0000  .s......r....c..
-00000340: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00000350: 0000 4000 0000 73c6 0000 0065 005a 0164  ..@...s....e.Z.d
-00000360: 005a 0264 015a 0364 0264 0384 005a 0464  .Z.d.Z.d.d...Z.d
-00000370: 0464 0584 005a 0564 0664 0784 005a 0664  .d...Z.d.d...Z.d
-00000380: 0864 0984 005a 0764 0a64 0b84 005a 0864  .d...Z.d.d...Z.d
-00000390: 0c64 0d84 005a 0964 0e64 0f84 005a 0a64  .d...Z.d.d...Z.d
-000003a0: 1064 1184 005a 0b64 1264 1384 005a 0c65  .d...Z.d.d...Z.e
-000003b0: 0d65 0e64 149c 0264 1564 1684 045a 0f65  .e.d...d.d...Z.e
-000003c0: 0d65 0e64 149c 0264 1764 1884 045a 1064  .e.d...d.d...Z.d
-000003d0: 1964 1a84 005a 1164 1b64 1c84 005a 1264  .d...Z.d.d...Z.d
-000003e0: 1d64 1e84 005a 1365 1464 1f9c 0164 2064  .d...Z.e.d...d d
-000003f0: 2184 045a 1564 2264 2384 005a 1664 2464  !..Z.d"d#..Z.d$d
-00000400: 2584 005a 1764 2664 2784 005a 1864 2864  %..Z.d&d'..Z.d(d
-00000410: 2984 005a 1964 2a64 2b84 005a 1a64 2c53  )..Z.d*d+..Z.d,S
-00000420: 0029 2dda 0652 6f75 7465 7275 3800 0000  .)-..Routeru8...
-00000430: 0a20 2020 20e8 b7af e794 b1e7 9bb8 e585  .    ...........
-00000440: b3e5 91bd e4bb a4ef bc9a 746c 2072 6f75  ..........tl rou
-00000450: 7465 7220 2d68 20e6 9fa5 e79c 8be8 afa6  ter -h .........
-00000460: e683 850a 2020 2020 6301 0000 0000 0000  ....    c.......
-00000470: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00000480: 0073 3800 0000 6700 7c00 5f00 6700 7c00  .s8...g.|._.g.|.
-00000490: 5f01 6700 7c00 5f02 6401 7c00 5f03 6402  _.g.|._.d.|._.d.
-000004a0: 7c00 5f04 6403 7c00 5f05 7406 a007 a100  |._.d.|._.t.....
-000004b0: 0100 7c00 a008 a100 0100 6400 5300 2904  ..|.......d.S.).
-000004c0: 4e7a 2774 6466 2d66 6c75 7474 6572 3a2f  Nz'tdf-flutter:/
-000004d0: 2f32 6466 6972 652e 636f 6d2f 6275 7369  /2dfire.com/busi
-000004e0: 6e65 7373 2f65 6e74 7279 7a0d 666c 7574  ness/entryz.flut
-000004f0: 7465 7220 656e 7472 795a 1954 5a52 6f75  ter entryZ.TZRou
-00000500: 7465 7242 7573 696e 6573 7345 6e74 7279  terBusinessEntry
-00000510: 5061 6765 2909 da15 5f52 6f75 7465 725f  Page)..._Router_
-00000520: 5f70 6163 6b61 6765 734c 6973 74da 185f  _packagesList.._
-00000530: 526f 7574 6572 5f5f 6d61 6344 6f77 6e44  Router__macDownD
-00000540: 6174 614c 6973 74da 155f 526f 7574 6572  ataList.._Router
-00000550: 5f5f 6d61 696e 5061 6765 4461 7461 da16  __mainPageData..
-00000560: 5f52 6f75 7465 725f 5f65 6e74 7279 5061  _Router__entryPa
-00000570: 6765 5061 7468 da16 5f52 6f75 7465 725f  gePath.._Router_
-00000580: 5f65 6e74 7279 5061 6765 4e6f 7465 da18  _entryPageNote..
-00000590: 5f52 6f75 7465 725f 5f65 6e74 7279 5061  _Router__entryPa
-000005a0: 6765 5769 6467 6574 720b 0000 00da 0d64  geWidgetr......d
-000005b0: 6972 496e 7661 6c69 6461 7465 da13 6665  irInvalidate..fe
-000005c0: 7463 685f 5f70 6163 6b61 6765 734c 6973  tch__packagesLis
-000005d0: 7472 1400 0000 7216 0000 0072 1600 0000  tr....r....r....
-000005e0: 7217 0000 0072 1800 0000 1d00 0000 7310  r....r........s.
-000005f0: 0000 0000 0106 0206 0206 0206 0106 0106  ................
-00000600: 0208 017a 0f52 6f75 7465 722e 5f5f 696e  ...z.Router.__in
-00000610: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
-00000620: 0001 0000 0003 0000 0043 0000 0073 2e00  .........C...s..
-00000630: 0000 7400 a001 a100 0100 7c00 a002 a100  ..t.......|.....
-00000640: 0100 7c00 a003 a100 0100 7404 a005 6401  ..|.......t...d.
-00000650: a101 0100 7406 6402 8301 0100 6403 5300  ....t.d.....d.S.
-00000660: 2904 7540 0000 000a 2020 2020 2020 2020  ).u@....        
-00000670: 746c 2072 6f75 7465 7220 696e 7465 6772  tl router integr
-00000680: 6174 65ef bc9a e5af b9e5 a3b3 e8bf 9be8  ate.............
-00000690: a18c e8b7 afe7 94b1 e695 b4e5 9088 0a20  ............... 
-000006a0: 2020 2020 2020 2075 1b00 0000 e5a3 b3e6         u........
-000006b0: a8a1 e59d 97e8 b7af e794 b1e6 95b4 e590  ................
-000006c0: 88e5 ae8c e688 9072 0100 0000 4e29 0772  .......r....N).r
-000006d0: 0b00 0000 7223 0000 0072 2400 0000 da0f  ....r#...r$.....
-000006e0: 696e 7465 6772 6174 655f 7368 656c 6c72  integrate_shellr
-000006f0: 0a00 0000 da05 7469 746c 65da 0465 7869  ......title..exi
-00000700: 7472 1400 0000 7216 0000 0072 1600 0000  tr....r....r....
-00000710: 7217 0000 00da 0969 6e74 6567 7261 7465  r......integrate
-00000720: 2b00 0000 730a 0000 0000 0408 0108 0108  +...s...........
-00000730: 010a 017a 1052 6f75 7465 722e 696e 7465  ...z.Router.inte
-00000740: 6772 6174 6563 0100 0000 0000 0000 0000  gratec..........
-00000750: 0000 0100 0000 0300 0000 4300 0000 731c  ..........C...s.
-00000760: 0000 0074 00a0 01a1 0001 0074 0274 03a0  ...t.......t.t..
-00000770: 04a1 0083 016a 057c 005f 0664 0053 00a9  .....j.|._.d.S..
-00000780: 014e 2907 720b 0000 00da 0c67 6f49 6e53  .N).r......goInS
-00000790: 6865 6c6c 4469 7272 0800 0000 da02 6f73  hellDirr......os
-000007a0: da06 6765 7463 7764 da08 7061 636b 6167  ..getcwd..packag
-000007b0: 6573 721d 0000 0072 1400 0000 7216 0000  esr....r....r...
-000007c0: 0072 1600 0000 7217 0000 0072 2400 0000  .r....r....r$...
-000007d0: 3600 0000 7304 0000 0000 0108 027a 1a52  6...s........z.R
-000007e0: 6f75 7465 722e 6665 7463 685f 5f70 6163  outer.fetch__pac
-000007f0: 6b61 6765 734c 6973 7463 0100 0000 0000  kagesListc......
-00000800: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00000810: 0000 732c 0000 007c 00a0 00a1 0001 007c  ..s,...|.......|
-00000820: 00a0 01a1 0001 007c 00a0 02a1 0001 007c  .......|.......|
-00000830: 00a0 03a1 0001 007c 00a0 04a1 0001 0064  .......|.......d
-00000840: 0053 0072 2900 0000 2905 da24 5f52 6f75  .S.r)...)..$_Rou
-00000850: 7465 725f 5f69 6e74 6567 7261 7465 5f61  ter__integrate_a
-00000860: 6c6c 5f72 6f75 7469 6e67 5f66 696c 6573  ll_routing_files
-00000870: da23 5f52 6f75 7465 725f 5f67 656e 6572  .#_Router__gener
-00000880: 6174 655f 726f 7574 6572 5f69 6e69 745f  ate_router_init_
-00000890: 6669 6c65 73da 245f 526f 7574 6572 5f5f  files.$_Router__
-000008a0: 6765 6e65 7261 7465 5f72 6f75 7465 725f  generate_router_
-000008b0: 656e 7472 795f 6669 6c65 73da 1c5f 526f  entry_files.._Ro
-000008c0: 7574 6572 5f5f 6765 6e65 7261 7465 5f72  uter__generate_r
-000008d0: 6f75 7465 725f 646f 63da 0a5f 5f66 6f72  outer_doc..__for
-000008e0: 6d61 745f 5f72 1400 0000 7216 0000 0072  mat__r....r....r
-000008f0: 1600 0000 7217 0000 0072 2500 0000 3c00  ....r....r%...<.
-00000900: 0000 730a 0000 0000 0208 0308 0308 0308  ..s.............
-00000910: 037a 1652 6f75 7465 722e 696e 7465 6772  .z.Router.integr
-00000920: 6174 655f 7368 656c 6c63 0100 0000 0000  ate_shellc......
-00000930: 0000 0000 0000 1000 0000 0900 0000 4300  ..............C.
-00000940: 0000 7306 0200 0074 00a0 0164 01a1 0101  ..s....t...d....
-00000950: 0074 02a0 03a1 0001 0074 04a0 0564 02a1  .t.......t...d..
-00000960: 0101 0074 046a 06a0 0764 03a1 0172 3274  ...t.j...d...r2t
-00000970: 08a0 0964 03a1 0101 0074 04a0 0a64 03a1  ...d.....t...d..
-00000980: 0101 0074 04a0 0564 03a1 0101 0074 04a0  ...t...d.....t..
-00000990: 0a64 04a1 0101 007c 006a 0b44 0090 015d  .d.....|.j.D...]
-000009a0: a87d 0174 02a0 03a1 0001 007c 00a0 0c7c  .}.t.......|...|
-000009b0: 016a 0da1 0172 5674 04a0 0574 02a0 0ea1  .j...rVt...t....
-000009c0: 0064 0517 00a1 0101 0074 04a0 0a7c 016a  .d.......t...|.j
-000009d0: 0fa1 0101 0074 04a0 057c 016a 0fa1 0101  .....t...|.j....
-000009e0: 0064 067d 0274 107c 0264 0783 027d 037c  .d.}.t.|.d...}.|
-000009f0: 00a0 117c 0364 08a1 0201 0074 02a0 03a1  ...|.d.....t....
-00000a00: 0001 0074 04a0 057c 016a 0da1 0101 0074  ...t...|.j.....t
-00000a10: 04a0 1274 13a0 14a1 00a1 01a0 15a1 00a0  ...t............
-00000a20: 1664 09a1 0164 0a19 007d 0467 007d 0567  .d...d...}.g.}.g
-00000a30: 007d 0674 04a0 177c 04a1 0144 005d aa5c  .}.t...|...D.].\
-00000a40: 037d 077d 087d 097c 0944 005d 9a7d 0a74  .}.}.}.|.D.].}.t
-00000a50: 046a 06a0 187c 077c 0aa1 027d 0b7c 0ba0  .j...|.|...}.|..
-00000a60: 1964 0ba1 0190 0172 047c 016a 0f7d 0c74  .d.....r.|.j.}.t
-00000a70: 13a0 1aa1 0090 0172 4e7c 0ba0 1664 0ca1  .......rN|...d..
-00000a80: 0164 0d19 007d 0d7c 0da0 1b64 0e64 0fa1  .d...}.|...d.d..
-00000a90: 027d 0e6e 0e7c 0ba0 1664 10a1 0164 0d19  .}.n.|...d...d..
-00000aa0: 007d 0e64 1174 1c7c 0ea0 1da1 0083 01a0  .}.d.t.|........
-00000ab0: 1ea1 0064 1264 1385 0219 0017 007d 0f7c  ...d.d.......}.|
-00000ac0: 00a0 1f7c 037c 0c7c 0e7c 0fa1 0401 007c  ...|.|.|.|.....|
-00000ad0: 05a0 207c 0fa1 0101 007c 06a0 207c 0ba1  .. |.....|.. |..
-00000ae0: 0101 0090 0171 0471 f674 217c 0583 0164  .....q.q.t!|...d
-00000af0: 0a6b 0490 0172 f874 00a0 2264 14a0 237c  .k...r.t.."d..#|
-00000b00: 016a 0f74 217c 0583 01a1 02a1 0101 007c  .j.t!|.........|
-00000b10: 00a0 247c 037c 016a 0f7c 05a1 0301 0074  ..$|.|.j.|.....t
-00000b20: 13a0 1aa1 0090 0172 ee7c 00a0 257c 06a1  .......r.|..%|..
-00000b30: 0101 006e 0a7c 00a0 267c 06a1 0101 007c  ...n.|..&|.....|
-00000b40: 03a0 27a1 0001 0071 5664 0053 0029 154e  ..'....qVd.S.).N
-00000b50: 7521 0000 00e6 95b4 e590 88e6 8980 e69c  u!..............
-00000b60: 89e8 b7af e794 b1e6 9687 e4bb b6e5 88b0  ................
-00000b70: e5a3 b3e9 878c da03 6c69 62da 0974 7a5f  ........lib..tz_
-00000b80: 726f 7574 6572 da05 6772 6f75 707a 152f  router..groupz./
-00000b90: 6c69 622f 747a 5f72 6f75 7465 722f 6772  lib/tz_router/gr
-00000ba0: 6f75 702f 7a0f 726f 7574 6572 5f6d 6170  oup/z.router_map
-00000bb0: 2e64 6172 74fa 0277 2bfa 2527 7061 636b  .dart..w+.%'pack
-00000bc0: 6167 653a 7464 665f 726f 7574 6572 2f74  age:tdf_router/t
-00000bd0: 6466 5f72 6f75 7465 722e 6461 7274 273b  df_router.dart';
-00000be0: da01 0a72 0100 0000 fa10 2e74 6466 5f72  ...r.......tdf_r
-00000bf0: 6f75 7465 722e 6461 7274 7a05 5c6c 6962  outer.dartz.\lib
-00000c00: 5ce9 0100 0000 fa01 5cfa 012f 7a05 2f6c  \.......\../z./l
-00000c10: 6962 2f5a 0b74 6466 5f72 6f75 7465 725f  ib/Z.tdf_router_
-00000c20: e908 0000 00e9 f8ff ffff 7529 0000 00e6  ..........u)....
-00000c30: a8a1 e59d 977b 3a3e 3330 7d20 20e6 a380  .....{:>30}  ...
-00000c40: e6b5 8be5 88b0 2020 7b3a 3e33 7d20 20e4  ......  {:>3}  .
-00000c50: b8aa e8b7 afe7 94b1 2928 720a 0000 0072  ........)(r....r
-00000c60: 2600 0000 720b 0000 0072 2a00 0000 722b  &...r....r*...r+
-00000c70: 0000 00da 0563 6864 6972 da04 7061 7468  .....chdir..path
-00000c80: da06 6578 6973 7473 da06 7368 7574 696c  ..exists..shutil
-00000c90: da06 726d 7472 6565 da05 6d6b 6469 7272  ..rmtree..mkdirr
-00000ca0: 1d00 0000 da1a 5f52 6f75 7465 725f 5f68  ......_Router__h
-00000cb0: 6173 526f 7574 6572 4461 7274 4669 6c65  asRouterDartFile
-00000cc0: da0b 7061 636b 6167 6550 6174 68da 0b67  ..packagePath..g
-00000cd0: 6574 5368 656c 6c44 6972 da0b 7061 636b  etShellDir..pack
-00000ce0: 6167 654e 616d 65da 046f 7065 6eda 1d5f  ageName..open.._
-00000cf0: 526f 7574 6572 5f5f 6465 6661 756c 7449  Router__defaultI
-00000d00: 6d70 6f72 7443 7265 6174 6f72 da05 706f  mportCreator..po
-00000d10: 7065 6e72 0900 0000 da07 7077 645f 636d  penr......pwd_cm
-00000d20: 64da 0472 6561 64da 0573 706c 6974 da04  d..read..split..
-00000d30: 7761 6c6b da04 6a6f 696e da08 656e 6473  walk..join..ends
-00000d40: 7769 7468 da0a 6973 5f77 696e 646f 7773  with..is_windows
-00000d50: da07 7265 706c 6163 6572 0200 0000 da06  ..replacer......
-00000d60: 656e 636f 6465 da09 6865 7864 6967 6573  encode..hexdiges
-00000d70: 74da 1a5f 526f 7574 6572 5f5f 696d 706f  t.._Router__impo
-00000d80: 7274 4461 7461 4372 6561 746f 72da 0661  rtDataCreator..a
-00000d90: 7070 656e 64da 036c 656e da05 7374 6167  ppend..len..stag
-00000da0: 65da 0666 6f72 6d61 74da 205f 526f 7574  e..format. _Rout
-00000db0: 6572 5f5f 6772 6f75 7052 6f75 7465 7243  er__groupRouterC
-00000dc0: 6c61 7373 4372 6561 746f 72da 1c5f 526f  lassCreator.._Ro
-00000dd0: 7574 6572 5f5f 6164 6449 6e57 696e 646f  uter__addInWindo
-00000de0: 7744 6f77 6e44 6174 61da 195f 526f 7574  wDownData.._Rout
-00000df0: 6572 5f5f 6164 6449 6e4d 6163 446f 776e  er__addInMacDown
-00000e00: 4461 7461 da05 636c 6f73 6529 1072 1500  Data..close).r..
-00000e10: 0000 da0b 7061 636b 6167 6549 7465 6dda  ....packageItem.
-00000e20: 0966 696c 655f 6e61 6d65 da01 66da 086e  .file_name..f..n
-00000e30: 6f77 6150 6174 685a 1372 6f75 7465 7241  owaPathZ.routerA
-00000e40: 6c69 6173 4669 6c65 4c69 7374 da0e 726f  liasFileList..ro
-00000e50: 7574 6572 4669 6c65 4c69 7374 da04 726f  uterFileList..ro
-00000e60: 6f74 da01 5fda 0566 696c 6573 da04 6669  ot.._..files..fi
-00000e70: 6c65 da08 7372 635f 6669 6c65 da0e 6974  le..src_file..it
-00000e80: 656d 4d6f 6475 6c65 4e61 6d65 da04 7465  emModuleName..te
-00000e90: 6d70 da0c 6974 656d 4669 6c65 5061 7468  mp..itemFilePath
-00000ea0: da0d 6974 656d 4669 6c65 416c 6961 7372  ..itemFileAliasr
-00000eb0: 1600 0000 7216 0000 0072 1700 0000 5a1d  ....r....r....Z.
-00000ec0: 5f5f 696e 7465 6772 6174 655f 616c 6c5f  __integrate_all_
-00000ed0: 726f 7574 696e 675f 6669 6c65 734e 0000  routing_filesN..
-00000ee0: 0073 7600 0000 0001 0a01 0801 0a01 0c01  .sv.............
-00000ef0: 0a01 0a01 0a01 0a02 0c02 0801 0c01 1201  ................
-00000f00: 0c01 0c01 0401 0a01 0401 04ff 0403 0801  ................
-00000f10: 0c02 1201 02ff 0201 02ff 0403 0401 0401  ................
-00000f20: 1401 0801 0e01 0c01 0601 0a01 0e01 0e02  ................
-00000f30: 0e02 0201 16ff 02ff 0205 0401 08ff 0403  ................
-00000f40: 0a01 1001 0e01 0401 0401 0aff 02ff 0405  ................
-00000f50: 0401 08ff 0403 0a01 0c02 0a02 7a24 526f  ............z$Ro
-00000f60: 7574 6572 2e5f 5f69 6e74 6567 7261 7465  uter.__integrate
-00000f70: 5f61 6c6c 5f72 6f75 7469 6e67 5f66 696c  _all_routing_fil
-00000f80: 6573 6301 0000 0000 0000 0000 0000 000e  esc.............
-00000f90: 0000 0007 0000 0043 0000 0073 5401 0000  .......C...sT...
-00000fa0: 7400 a001 6401 a101 0100 7402 a003 a100  t...d.....t.....
-00000fb0: 0100 7404 a005 6402 a101 0100 6403 7d01  ..t...d.....d.}.
-00000fc0: 7406 7c01 6404 8302 7d02 7404 6a07 a008  t.|.d...}.t.j...
-00000fd0: 6405 a101 6406 6b02 7244 7404 a009 6405  d...d.k.rDt...d.
-00000fe0: a101 0100 7404 a005 6405 a101 0100 7404  ....t...d.....t.
-00000ff0: a00a 740b a00c a100 a101 a00d a100 a00e  ..t.............
-00001000: 6407 a101 6408 1900 7d03 7c00 a00f 7c02  d...d...}.|...|.
-00001010: 6409 a102 0100 7c00 a00f 7c02 640a a102  d.....|...|.d...
-00001020: 0100 6700 7d04 7404 a010 7c03 a101 4400  ..g.}.t...|...D.
-00001030: 5da0 5c03 7d05 7d06 7d07 7c07 4400 5d90  ].\.}.}.}.|.D.].
-00001040: 7d08 7404 6a07 a011 7c05 7c08 a102 7d09  }.t.j...|.|...}.
-00001050: 7c09 a012 7c01 a101 640b 6b03 72c0 719e  |...|...d.k.r.q.
-00001060: 740b a013 a100 72e4 7c09 a00e 640c a101  t.....r.|...d...
-00001070: 640d 1900 7d0a 7c0a a014 640e 640f a102  d...}.|...d.d...
-00001080: 7d0b 6e0e 7c09 a00e 640c a101 640d 1900  }.n.|...d...d...
-00001090: 7d0b 6410 7415 7c0b a016 a100 8301 a017  }.d.t.|.........
-000010a0: a100 6411 6412 8502 1900 1700 7d0c 6413  ..d.d.......}.d.
-000010b0: a018 7c0b 7c0c a102 7d0d 7c02 a019 7c0d  ..|.|...}.|...|.
-000010c0: a101 0100 7c04 a01a 7c0c a101 0100 719e  ....|...|.....q.
-000010d0: 7190 7c02 a019 6414 a018 7c00 a01b 7c04  q.|...d...|...|.
-000010e0: a101 a101 a101 0100 7c02 a01c a100 0100  ........|.......
-000010f0: 6400 5300 2915 4e75 1b00 0000 e794 9fe6  d.S.).Nu........
-00001100: 8890 e8b7 afe7 94b1 e588 9de5 a78b e58c  ................
-00001110: 96e6 9687 e4bb b6fa 0d6c 6962 2f74 7a5f  .........lib/tz_
-00001120: 726f 7574 6572 7a09 696e 6974 2e64 6172  routerz.init.dar
-00001130: 7472 3600 0000 7235 0000 0046 7238 0000  tr6...r5...Fr8..
-00001140: 0072 0100 0000 7237 0000 007a 2227 656e  .r....r7...z"'en
-00001150: 7472 792f 747a 5f72 6f75 7465 725f 656e  try/tz_router_en
-00001160: 7472 795f 7061 6765 2e64 6172 7427 3be9  try_page.dart';.
-00001170: ffff ffff 7234 0000 0072 3a00 0000 723b  ....r4...r:...r;
-00001180: 0000 0072 3c00 0000 5a0b 726f 7574 6572  ...r<...Z.router
-00001190: 5f6d 6170 5f72 3d00 0000 723e 0000 007a  _map_r=...r>...z
-000011a0: 1669 6d70 6f72 7420 222e 7b30 7d22 2061  .import ".{0}" a
-000011b0: 7320 7b31 7d3b 0a7a d10a 0a20 2020 2020  s {1};.z...     
-000011c0: 2020 2063 6c61 7373 2054 5a52 6f75 7465     class TZRoute
-000011d0: 724d 616e 6167 6572 207b 7b0a 2020 2020  rManager {{.    
-000011e0: 2020 2020 2020 2020 7374 6174 6963 2063          static c
-000011f0: 6f6d 6269 6e65 4d61 7028 2920 7b7b 0a20  ombineMap() {{. 
-00001200: 2020 2020 2020 2020 2020 2020 2020 204d                 M
-00001210: 6170 3c53 7472 696e 672c 2054 4446 5061  ap<String, TDFPa
-00001220: 6765 4275 696c 6465 723e 206d 6170 203d  geBuilder> map =
-00001230: 204d 6170 2829 3b0a 2020 2020 2020 2020   Map();.        
-00001240: 2020 2020 2020 2020 7b30 7d0a 2020 2020          {0}.    
-00001250: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00001260: 726e 206d 6170 3b0a 2020 2020 2020 2020  rn map;.        
-00001270: 2020 2020 7d7d 0a20 2020 2020 2020 207d      }}.        }
-00001280: 7d0a 2020 2020 2020 2020 291d 720a 0000  }.        ).r...
-00001290: 0072 2600 0000 720b 0000 0072 2a00 0000  .r&...r....r*...
-000012a0: 722b 0000 0072 3f00 0000 7249 0000 0072  r+...r?...rI...r
-000012b0: 4000 0000 7241 0000 0072 4400 0000 724b  @...rA...rD...rK
-000012c0: 0000 0072 0900 0000 724c 0000 0072 4d00  ...r....rL...rM.
-000012d0: 0000 724e 0000 0072 4a00 0000 724f 0000  ..rN...rJ...rO..
-000012e0: 0072 5000 0000 da04 6669 6e64 7252 0000  .rP.....findrR..
-000012f0: 0072 5300 0000 7202 0000 0072 5400 0000  .rS...r....rT...
-00001300: 7255 0000 0072 5a00 0000 da05 7772 6974  rU...rZ.....writ
-00001310: 6572 5700 0000 da1e 5f52 6f75 7465 725f  erW....._Router_
-00001320: 5f6d 6170 4c69 7374 436f 6d62 696e 6543  _mapListCombineC
-00001330: 7265 6174 6572 725e 0000 0029 0e72 1500  reaterr^...).r..
-00001340: 0000 7260 0000 00da 0569 6e69 7446 7262  ..r`.....initFrb
-00001350: 0000 005a 076d 6170 4c69 7374 7264 0000  ...Z.mapListrd..
-00001360: 0072 6500 0000 7266 0000 0072 6700 0000  .re...rf...rg...
-00001370: 7268 0000 005a 0f74 6d70 4974 656d 4669  rh...Z.tmpItemFi
-00001380: 6c65 5061 7468 726b 0000 0072 6c00 0000  lePathrk...rl...
-00001390: 5a0d 696d 706f 7274 436f 6e74 656e 7472  Z.importContentr
-000013a0: 1600 0000 7216 0000 0072 1700 0000 5a1c  ....r....r....Z.
-000013b0: 5f5f 6765 6e65 7261 7465 5f72 6f75 7465  __generate_route
-000013c0: 725f 696e 6974 5f66 696c 6573 9100 0000  r_init_files....
-000013d0: 7350 0000 0000 010a 0108 010a 0204 010a  sP..............
-000013e0: 0310 010a 010a 011c 0104 0104 ff04 0304  ................
-000013f0: 0104 ff04 0204 0114 0108 010e 010e 0102  ................
-00001400: 0108 010e 010e 020e 0210 0106 ff04 ff02  ................
-00001410: 0404 0104 ff04 030a 010e 0204 0104 0a08  ................
-00001420: f602 ff04 0f7a 2352 6f75 7465 722e 5f5f  .....z#Router.__
-00001430: 6765 6e65 7261 7465 5f72 6f75 7465 725f  generate_router_
-00001440: 696e 6974 5f66 696c 6573 6301 0000 0000  init_filesc.....
-00001450: 0000 0000 0000 0003 0000 0009 0000 0043  ...............C
-00001460: 0000 0073 ca00 0000 7400 a001 6401 a101  ...s....t...d...
-00001470: 0100 7402 a003 a100 0100 7404 a005 6402  ..t.......t...d.
-00001480: a101 0100 7404 6a06 a007 6403 a101 6404  ....t.j...d...d.
-00001490: 6b02 7236 7404 a008 6403 a101 0100 7404  k.r6t...d.....t.
-000014a0: a005 6403 a101 0100 6405 7d01 7409 7c01  ..d.....d.}.t.|.
-000014b0: 6406 6407 6408 8d03 7d02 7c00 a00a 7c02  d.d.d...}.|...|.
-000014c0: 6409 a102 0100 7c00 a00a 7c02 640a a102  d.....|...|.d...
-000014d0: 0100 7c00 a00a 7c02 640b a102 0100 7c00  ..|...|.d.....|.
-000014e0: a00a 7c02 640c a102 0100 7c00 a00a 7c02  ..|.d.....|...|.
-000014f0: 640d a102 0100 7c00 a00a 7c02 640e a102  d.....|...|.d...
-00001500: 0100 7c02 a00b 640f a00c 7c00 6a0d 7c00  ..|...d...|.j.|.
-00001510: 6a0e 7c00 6a0f 7c00 a010 a100 7c00 6a0e  j.|.j.|.....|.j.
-00001520: a105 a101 0100 7c02 a011 a100 0100 6400  ......|.......d.
-00001530: 5300 2910 4e75 1800 0000 e794 9fe6 8890  S.).Nu..........
-00001540: e8b7 afe7 94b1 e585 a5e5 8fa3 e696 87e4  ................
-00001550: bbb6 726d 0000 00da 0565 6e74 7279 467a  ..rm.....entryFz
-00001560: 1974 7a5f 726f 7574 6572 5f65 6e74 7279  .tz_router_entry
-00001570: 5f70 6167 652e 6461 7274 7236 0000 00da  _page.dartr6....
-00001580: 0475 7466 38a9 01da 0865 6e63 6f64 696e  .utf8....encodin
-00001590: 677a 2027 7061 636b 6167 653a 666c 7574  gz 'package:flut
-000015a0: 7465 722f 6d61 7465 7269 616c 2e64 6172  ter/material.dar
-000015b0: 7427 3b72 3700 0000 7a32 2770 6163 6b61  t';r7...z2'packa
-000015c0: 6765 3a74 6466 5f72 6f75 7465 725f 616e  ge:tdf_router_an
-000015d0: 6e6f 2f72 6f75 7465 722f 726f 7574 6572  no/router/router
-000015e0: 5f61 6e6e 6f2e 6461 7274 273b 7a2d 2770  _anno.dart';z-'p
-000015f0: 6163 6b61 6765 3a74 6466 5f62 6173 655f  ackage:tdf_base_
-00001600: 7574 696c 732f 7464 665f 6261 7365 5f75  utils/tdf_base_u
-00001610: 7469 6c73 2e64 6172 7427 3b7a 3227 7061  tils.dart';z2'pa
-00001620: 636b 6167 653a 7464 665f 7769 6467 6574  ckage:tdf_widget
-00001630: 732f 7464 665f 636f 6d6d 6f6e 5f62 746e  s/tdf_common_btn
-00001640: 2f74 6466 5f62 746e 2e64 6172 7427 3b7a  /tdf_btn.dart';z
-00001650: 3327 7061 636b 6167 653a 7464 665f 7769  3'package:tdf_wi
-00001660: 6467 6574 732f 7469 746c 655f 6261 722f  dgets/title_bar/
-00001670: 7464 665f 7469 746c 655f 6261 722e 6461  tdf_title_bar.da
-00001680: 7274 273b 7563 0d00 000a 0a40 545a 526f  rt';uc.....@TZRo
-00001690: 7574 6572 2870 6174 683a 2027 7b30 7d27  uter(path: '{0}'
-000016a0: 2c20 6e6f 7465 3a20 277b 317d 2729 0a63  , note: '{1}').c
-000016b0: 6c61 7373 207b 327d 2065 7874 656e 6473  lass {2} extends
-000016c0: 2053 7461 7465 6675 6c57 6964 6765 7420   StatefulWidget 
-000016d0: 7b7b 0a20 2020 2066 696e 616c 204d 6170  {{.    final Map
-000016e0: 2070 6172 616d 733b 0a0a 2020 2020 7b32   params;..    {2
-000016f0: 7d28 7468 6973 2e70 6172 616d 7329 3b0a  }(this.params);.
-00001700: 0a20 2020 2040 6f76 6572 7269 6465 0a20  .    @override. 
-00001710: 2020 205f 7b32 7d53 7461 7465 2063 7265     _{2}State cre
-00001720: 6174 6553 7461 7465 2829 203d 3e20 5f7b  ateState() => _{
-00001730: 327d 5374 6174 6528 293b 0a7d 7d0a 0a63  2}State();.}}..c
-00001740: 6c61 7373 205f 7b32 7d53 7461 7465 2065  lass _{2}State e
-00001750: 7874 656e 6473 2053 7461 7465 3c7b 327d  xtends State<{2}
-00001760: 3e20 7b7b 0a20 2020 2066 696e 616c 2054  > {{.    final T
-00001770: 6578 7445 6469 7469 6e67 436f 6e74 726f  extEditingContro
-00001780: 6c6c 6572 2072 6f75 7465 7243 6f6e 7472  ller routerContr
-00001790: 6f6c 6c65 7220 3d20 6e65 7720 5465 7874  oller = new Text
-000017a0: 4564 6974 696e 6743 6f6e 7472 6f6c 6c65  EditingControlle
-000017b0: 7228 293b 0a20 2020 2066 696e 616c 2054  r();.    final T
-000017c0: 6578 7445 6469 7469 6e67 436f 6e74 726f  extEditingContro
-000017d0: 6c6c 6572 2063 6f6e 7472 6f6c 6c65 7220  ller controller 
-000017e0: 3d20 6e65 7720 5465 7874 4564 6974 696e  = new TextEditin
-000017f0: 6743 6f6e 7472 6f6c 6c65 7228 293b 0a20  gController();. 
-00001800: 2020 2066 696e 616c 204d 6170 3c53 7472     final Map<Str
-00001810: 696e 672c 2053 7472 696e 673e 2070 6167  ing, String> pag
-00001820: 654d 6170 203d 207b 7b0a 2020 2020 7b33  eMap = {{.    {3
-00001830: 7d0a 2020 2020 7d7d 3b0a 0a20 2020 2040  }.    }};..    @
-00001840: 6f76 6572 7269 6465 0a20 2020 2057 6964  override.    Wid
-00001850: 6765 7420 6275 696c 6428 4275 696c 6443  get build(BuildC
-00001860: 6f6e 7465 7874 2063 6f6e 7465 7874 2920  ontext context) 
-00001870: 7b7b 0a20 2020 2020 2020 2054 4446 5363  {{.        TDFSc
-00001880: 7265 656e 2e69 6e69 7428 636f 6e74 6578  reen.init(contex
-00001890: 7429 3b0a 2020 2020 2020 2020 7265 7475  t);.        retu
-000018a0: 726e 2053 6361 6666 6f6c 6428 0a20 2020  rn Scaffold(.   
-000018b0: 2020 2020 2020 2020 2062 6163 6b67 726f           backgro
-000018c0: 756e 6443 6f6c 6f72 3a20 436f 6c6f 7228  undColor: Color(
-000018d0: 3078 6666 6666 6666 6666 292c 0a20 2020  0xffffffff),.   
-000018e0: 2020 2020 2020 2020 2061 7070 4261 723a           appBar:
-000018f0: 2054 4446 5469 746c 6542 6172 280a 2020   TDFTitleBar(.  
-00001900: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00001910: 746c 6543 6f6e 7465 6e74 3a20 227b 347d  tleContent: "{4}
-00001920: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00001930: 2020 2062 6163 6b54 7970 653a 2054 4446     backType: TDF
-00001940: 5469 746c 6542 6163 6b57 6964 6765 7454  TitleBackWidgetT
-00001950: 7970 652e 4445 4641 554c 545f 4241 434b  ype.DEFAULT_BACK
-00001960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001970: 2020 7269 6768 7443 6f6e 7465 6e74 3a20    rightContent: 
-00001980: 2255 49e6 a087 e587 86e5 8c96 222c 0a20  "UI.........",. 
-00001990: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000019a0: 6967 6874 436f 6e74 656e 7443 6f6c 6f72  ightContentColor
-000019b0: 3a20 3078 6666 3030 3838 6666 2c0a 2020  : 0xff0088ff,.  
-000019c0: 2020 2020 2020 2020 2020 2020 2020 7269                ri
-000019d0: 6768 7454 6578 7442 746e 436c 6963 6b3a  ghtTextBtnClick:
-000019e0: 2028 2920 7b7b 0a20 2020 2020 2020 2020   () {{.         
-000019f0: 2020 2020 2020 2054 4446 526f 7574 6572         TDFRouter
-00001a00: 2e6f 7065 6e28 2274 6466 2d6d 616e 6167  .open("tdf-manag
-00001a10: 6572 3a2f 2f32 6466 6972 652e 636f 6d2f  er://2dfire.com/
-00001a20: 7469 636b 6574 2f69 6e64 6578 222c 2075  ticket/index", u
-00001a30: 726c 5061 7261 6d73 3a20 7b7b 0a20 2020  rlParams: {{.   
+00000050: 6403 6c05 5a05 6400 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
+00000060: 6d08 5a08 0100 6400 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
+00000070: 0100 6400 6406 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
+00000080: 6407 6c0d 6d0e 5a0e 0100 4700 6408 6409  d.l.m.Z...G.d.d.
+00000090: 8400 6409 8302 5a0f 4700 640a 640b 8400  ..d...Z.G.d.d...
+000000a0: 640b 8302 5a10 6403 5300 290c e900 0000  d...Z.d.S.).....
+000000b0: 0029 01da 036d 6435 2901 da0d 5465 7874  .)...md5)...Text
+000000c0: 494f 5772 6170 7065 724e 2902 da0b 5061  IOWrapperN)...Pa
+000000d0: 636b 6167 654e 6f64 65da 1250 6163 6b61  ckageNode..Packa
+000000e0: 6765 734a 736f 6e43 6f6e 6669 6729 01da  gesJsonConfig)..
+000000f0: 0d50 6c61 7466 6f72 6d54 6f6f 6c73 2901  .PlatformTools).
+00000100: da05 5072 696e 7429 01da 0853 6865 6c6c  ..Print)...Shell
+00000110: 4469 7263 0000 0000 0000 0000 0000 0000  Dirc............
+00000120: 0000 0000 0200 0000 4000 0000 7314 0000  ........@...s...
+00000130: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
+00000140: 0364 0353 0029 04da 0a52 6f75 7465 724e  .d.S.)...RouterN
+00000150: 6f64 6563 0100 0000 0000 0000 0000 0000  odec............
+00000160: 0100 0000 0200 0000 4300 0000 7328 0000  ........C...s(..
+00000170: 0064 017c 005f 0064 017c 005f 0164 017c  .d.|._.d.|._.d.|
+00000180: 005f 0264 017c 005f 0364 017c 005f 0464  ._.d.|._.d.|._.d
+00000190: 027c 005f 0564 0053 0029 034e da00 4629  .|._.d.S.).N..F)
+000001a0: 06da 0770 6163 6b61 6765 da0a 726f 7574  ...package..rout
+000001b0: 6572 5061 7468 da08 6669 6c65 5061 7468  erPath..filePath
+000001c0: da04 6e6f 7465 da0a 7061 6765 5769 6467  ..note..pageWidg
+000001d0: 6574 da0a 6973 4d61 696e 5061 6765 a901  et..isMainPage..
+000001e0: da04 7365 6c66 a900 7213 0000 00f5 6500  ..self..r.....e.
+000001f0: 0000 2f55 7365 7273 2f78 756a 6961 6e2f  ../Users/xujian/
+00000200: 446f 6375 6d65 6e74 732f 3230 3234 2fe6  Documents/2024/.
+00000210: a8a1 e59d 97e9 97b4 e4ba a4e4 ba92 e9a1  ................
+00000220: b9e7 9bae 746c e58d 87e7 baa7 2f70 6163  ....tl....../pac
+00000230: 6b61 6765 5f74 6f6f 6c73 2f74 6466 5f74  kage_tools/tdf_t
+00000240: 6f6f 6c2f 7069 7065 6c69 6e65 732f 726f  ool/pipelines/ro
+00000250: 7574 6572 2e70 79da 085f 5f69 6e69 745f  uter.py..__init_
+00000260: 5f0c 0000 0073 0c00 0000 0001 0601 0601  _....s..........
+00000270: 0601 0601 0601 7a13 526f 7574 6572 4e6f  ......z.RouterNo
+00000280: 6465 2e5f 5f69 6e69 745f 5f4e 2904 da08  de.__init__N)...
+00000290: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000002a0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000002b0: 5f5f 7215 0000 0072 1300 0000 7213 0000  __r....r....r...
+000002c0: 0072 1300 0000 7214 0000 0072 0900 0000  .r....r....r....
+000002d0: 0b00 0000 7302 0000 0008 0172 0900 0000  ....s......r....
+000002e0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000002f0: 0003 0000 0040 0000 0073 c600 0000 6500  .....@...s....e.
+00000300: 5a01 6400 5a02 6401 5a03 6402 6403 8400  Z.d.Z.d.Z.d.d...
+00000310: 5a04 6404 6405 8400 5a05 6406 6407 8400  Z.d.d...Z.d.d...
+00000320: 5a06 6408 6409 8400 5a07 640a 640b 8400  Z.d.d...Z.d.d...
+00000330: 5a08 640c 640d 8400 5a09 640e 640f 8400  Z.d.d...Z.d.d...
+00000340: 5a0a 6410 6411 8400 5a0b 6412 6413 8400  Z.d.d...Z.d.d...
+00000350: 5a0c 650d 650e 6414 9c02 6415 6416 8404  Z.e.e.d...d.d...
+00000360: 5a0f 650d 650e 6414 9c02 6417 6418 8404  Z.e.e.d...d.d...
+00000370: 5a10 6419 641a 8400 5a11 641b 641c 8400  Z.d.d...Z.d.d...
+00000380: 5a12 641d 641e 8400 5a13 6514 641f 9c01  Z.d.d...Z.e.d...
+00000390: 6420 6421 8404 5a15 6422 6423 8400 5a16  d d!..Z.d"d#..Z.
+000003a0: 6424 6425 8400 5a17 6426 6427 8400 5a18  d$d%..Z.d&d'..Z.
+000003b0: 6428 6429 8400 5a19 642a 642b 8400 5a1a  d(d)..Z.d*d+..Z.
+000003c0: 642c 5300 292d da06 526f 7574 6572 7538  d,S.)-..Routeru8
+000003d0: 0000 000a 2020 2020 e8b7 afe7 94b1 e79b  ....    ........
+000003e0: b8e5 85b3 e591 bde4 bba4 efbc 9a74 6c20  .............tl 
+000003f0: 726f 7574 6572 202d 6820 e69f a5e7 9c8b  router -h ......
+00000400: e8af a6e6 8385 0a20 2020 2063 0100 0000  .......    c....
+00000410: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00000420: 4300 0000 7338 0000 0067 007c 005f 0067  C...s8...g.|._.g
+00000430: 007c 005f 0167 007c 005f 0264 017c 005f  .|._.g.|._.d.|._
+00000440: 0364 027c 005f 0464 037c 005f 0574 06a0  .d.|._.d.|._.t..
+00000450: 07a1 0001 007c 00a0 08a1 0001 0064 0053  .....|.......d.S
+00000460: 0029 044e 7a27 7464 662d 666c 7574 7465  .).Nz'tdf-flutte
+00000470: 723a 2f2f 3264 6669 7265 2e63 6f6d 2f62  r://2dfire.com/b
+00000480: 7573 696e 6573 732f 656e 7472 797a 0d66  usiness/entryz.f
+00000490: 6c75 7474 6572 2065 6e74 7279 5a19 545a  lutter entryZ.TZ
+000004a0: 526f 7574 6572 4275 7369 6e65 7373 456e  RouterBusinessEn
+000004b0: 7472 7950 6167 6529 09da 155f 526f 7574  tryPage)..._Rout
+000004c0: 6572 5f5f 7061 636b 6167 6573 4c69 7374  er__packagesList
+000004d0: da18 5f52 6f75 7465 725f 5f6d 6163 446f  .._Router__macDo
+000004e0: 776e 4461 7461 4c69 7374 da15 5f52 6f75  wnDataList.._Rou
+000004f0: 7465 725f 5f6d 6169 6e50 6167 6544 6174  ter__mainPageDat
+00000500: 61da 165f 526f 7574 6572 5f5f 656e 7472  a.._Router__entr
+00000510: 7950 6167 6550 6174 68da 165f 526f 7574  yPagePath.._Rout
+00000520: 6572 5f5f 656e 7472 7950 6167 654e 6f74  er__entryPageNot
+00000530: 65da 185f 526f 7574 6572 5f5f 656e 7472  e.._Router__entr
+00000540: 7950 6167 6557 6964 6765 7472 0800 0000  yPageWidgetr....
+00000550: da0d 6469 7249 6e76 616c 6964 6174 65da  ..dirInvalidate.
+00000560: 1366 6574 6368 5f5f 7061 636b 6167 6573  .fetch__packages
+00000570: 4c69 7374 7211 0000 0072 1300 0000 7213  Listr....r....r.
+00000580: 0000 0072 1400 0000 7215 0000 001a 0000  ...r....r.......
+00000590: 0073 1000 0000 0001 0602 0602 0602 0601  .s..............
+000005a0: 0601 0602 0801 7a0f 526f 7574 6572 2e5f  ......z.Router._
+000005b0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+000005c0: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+000005d0: 732e 0000 0074 00a0 01a1 0001 007c 00a0  s....t.......|..
+000005e0: 02a1 0001 007c 00a0 03a1 0001 0074 04a0  .....|.......t..
+000005f0: 0564 01a1 0101 0074 0664 0283 0101 0064  .d.....t.d.....d
+00000600: 0353 0029 0475 4000 0000 0a20 2020 2020  .S.).u@....     
+00000610: 2020 2074 6c20 726f 7574 6572 2069 6e74     tl router int
+00000620: 6567 7261 7465 efbc 9ae5 afb9 e5a3 b3e8  egrate..........
+00000630: bf9b e8a1 8ce8 b7af e794 b1e6 95b4 e590  ................
+00000640: 880a 2020 2020 2020 2020 751b 0000 00e5  ..        u.....
+00000650: a3b3 e6a8 a1e5 9d97 e8b7 afe7 94b1 e695  ................
+00000660: b4e5 9088 e5ae 8ce6 8890 7201 0000 004e  ..........r....N
+00000670: 2907 7208 0000 0072 2000 0000 7221 0000  ).r....r ...r!..
+00000680: 00da 0f69 6e74 6567 7261 7465 5f73 6865  ...integrate_she
+00000690: 6c6c 7207 0000 00da 0574 6974 6c65 da04  llr......title..
+000006a0: 6578 6974 7211 0000 0072 1300 0000 7213  exitr....r....r.
+000006b0: 0000 0072 1400 0000 da09 696e 7465 6772  ...r......integr
+000006c0: 6174 6528 0000 0073 0a00 0000 0004 0801  ate(...s........
+000006d0: 0801 0801 0a01 7a10 526f 7574 6572 2e69  ......z.Router.i
+000006e0: 6e74 6567 7261 7465 6301 0000 0000 0000  ntegratec.......
+000006f0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00000700: 0073 1c00 0000 7400 a001 a100 0100 7402  .s....t.......t.
+00000710: 7403 a004 a100 8301 6a05 7c00 5f06 6400  t.......j.|._.d.
+00000720: 5300 a901 4e29 0772 0800 0000 da0c 676f  S...N).r......go
+00000730: 496e 5368 656c 6c44 6972 7205 0000 00da  InShellDirr.....
+00000740: 026f 73da 0667 6574 6377 64da 0870 6163  .os..getcwd..pac
+00000750: 6b61 6765 7372 1a00 0000 7211 0000 0072  kagesr....r....r
+00000760: 1300 0000 7213 0000 0072 1400 0000 7221  ....r....r....r!
+00000770: 0000 0033 0000 0073 0400 0000 0001 0802  ...3...s........
+00000780: 7a1a 526f 7574 6572 2e66 6574 6368 5f5f  z.Router.fetch__
+00000790: 7061 636b 6167 6573 4c69 7374 6301 0000  packagesListc...
+000007a0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+000007b0: 0043 0000 0073 2c00 0000 7c00 a000 a100  .C...s,...|.....
+000007c0: 0100 7c00 a001 a100 0100 7c00 a002 a100  ..|.......|.....
+000007d0: 0100 7c00 a003 a100 0100 7c00 a004 a100  ..|.......|.....
+000007e0: 0100 6400 5300 7226 0000 0029 05da 245f  ..d.S.r&...)..$_
+000007f0: 526f 7574 6572 5f5f 696e 7465 6772 6174  Router__integrat
+00000800: 655f 616c 6c5f 726f 7574 696e 675f 6669  e_all_routing_fi
+00000810: 6c65 73da 235f 526f 7574 6572 5f5f 6765  les.#_Router__ge
+00000820: 6e65 7261 7465 5f72 6f75 7465 725f 696e  nerate_router_in
+00000830: 6974 5f66 696c 6573 da24 5f52 6f75 7465  it_files.$_Route
+00000840: 725f 5f67 656e 6572 6174 655f 726f 7574  r__generate_rout
+00000850: 6572 5f65 6e74 7279 5f66 696c 6573 da1c  er_entry_files..
+00000860: 5f52 6f75 7465 725f 5f67 656e 6572 6174  _Router__generat
+00000870: 655f 726f 7574 6572 5f64 6f63 da0a 5f5f  e_router_doc..__
+00000880: 666f 726d 6174 5f5f 7211 0000 0072 1300  format__r....r..
+00000890: 0000 7213 0000 0072 1400 0000 7222 0000  ..r....r....r"..
+000008a0: 0039 0000 0073 0a00 0000 0002 0803 0803  .9...s..........
+000008b0: 0803 0803 7a16 526f 7574 6572 2e69 6e74  ....z.Router.int
+000008c0: 6567 7261 7465 5f73 6865 6c6c 6301 0000  egrate_shellc...
+000008d0: 0000 0000 0000 0000 0010 0000 0009 0000  ................
+000008e0: 0043 0000 0073 0602 0000 7400 a001 6401  .C...s....t...d.
+000008f0: a101 0100 7402 a003 a100 0100 7404 a005  ....t.......t...
+00000900: 6402 a101 0100 7404 6a06 a007 6403 a101  d.....t.j...d...
+00000910: 7232 7408 a009 6403 a101 0100 7404 a00a  r2t...d.....t...
+00000920: 6403 a101 0100 7404 a005 6403 a101 0100  d.....t...d.....
+00000930: 7404 a00a 6404 a101 0100 7c00 6a0b 4400  t...d.....|.j.D.
+00000940: 9001 5da8 7d01 7402 a003 a100 0100 7c00  ..].}.t.......|.
+00000950: a00c 7c01 6a0d a101 7256 7404 a005 7402  ..|.j...rVt...t.
+00000960: a00e a100 6405 1700 a101 0100 7404 a00a  ....d.......t...
+00000970: 7c01 6a0f a101 0100 7404 a005 7c01 6a0f  |.j.....t...|.j.
+00000980: a101 0100 6406 7d02 7410 7c02 6407 8302  ....d.}.t.|.d...
+00000990: 7d03 7c00 a011 7c03 6408 a102 0100 7402  }.|...|.d.....t.
+000009a0: a003 a100 0100 7404 a005 7c01 6a0d a101  ......t...|.j...
+000009b0: 0100 7404 a012 7413 a014 a100 a101 a015  ..t...t.........
+000009c0: a100 a016 6409 a101 640a 1900 7d04 6700  ....d...d...}.g.
+000009d0: 7d05 6700 7d06 7404 a017 7c04 a101 4400  }.g.}.t...|...D.
+000009e0: 5daa 5c03 7d07 7d08 7d09 7c09 4400 5d9a  ].\.}.}.}.|.D.].
+000009f0: 7d0a 7404 6a06 a018 7c07 7c0a a102 7d0b  }.t.j...|.|...}.
+00000a00: 7c0b a019 640b a101 9001 7204 7c01 6a0f  |...d.....r.|.j.
+00000a10: 7d0c 7413 a01a a100 9001 724e 7c0b a016  }.t.......rN|...
+00000a20: 640c a101 640d 1900 7d0d 7c0d a01b 640e  d...d...}.|...d.
+00000a30: 640f a102 7d0e 6e0e 7c0b a016 6410 a101  d...}.n.|...d...
+00000a40: 640d 1900 7d0e 6411 741c 7c0e a01d a100  d...}.d.t.|.....
+00000a50: 8301 a01e a100 6412 6413 8502 1900 1700  ......d.d.......
+00000a60: 7d0f 7c00 a01f 7c03 7c0c 7c0e 7c0f a104  }.|...|.|.|.|...
+00000a70: 0100 7c05 a020 7c0f a101 0100 7c06 a020  ..|.. |.....|.. 
+00000a80: 7c0b a101 0100 9001 7104 71f6 7421 7c05  |.......q.q.t!|.
+00000a90: 8301 640a 6b04 9001 72f8 7400 a022 6414  ..d.k...r.t.."d.
+00000aa0: a023 7c01 6a0f 7421 7c05 8301 a102 a101  .#|.j.t!|.......
+00000ab0: 0100 7c00 a024 7c03 7c01 6a0f 7c05 a103  ..|..$|.|.j.|...
+00000ac0: 0100 7413 a01a a100 9001 72ee 7c00 a025  ..t.......r.|..%
+00000ad0: 7c06 a101 0100 6e0a 7c00 a026 7c06 a101  |.....n.|..&|...
+00000ae0: 0100 7c03 a027 a100 0100 7156 6400 5300  ..|..'....qVd.S.
+00000af0: 2915 4e75 2100 0000 e695 b4e5 9088 e689  ).Nu!...........
+00000b00: 80e6 9c89 e8b7 afe7 94b1 e696 87e4 bbb6  ................
+00000b10: e588 b0e5 a3b3 e987 8cda 036c 6962 da09  ...........lib..
+00000b20: 747a 5f72 6f75 7465 72da 0567 726f 7570  tz_router..group
+00000b30: 7a15 2f6c 6962 2f74 7a5f 726f 7574 6572  z./lib/tz_router
+00000b40: 2f67 726f 7570 2f7a 0f72 6f75 7465 725f  /group/z.router_
+00000b50: 6d61 702e 6461 7274 fa02 772b fa25 2770  map.dart..w+.%'p
+00000b60: 6163 6b61 6765 3a74 6466 5f72 6f75 7465  ackage:tdf_route
+00000b70: 722f 7464 665f 726f 7574 6572 2e64 6172  r/tdf_router.dar
+00000b80: 7427 3bda 010a 7201 0000 00fa 102e 7464  t';...r.......td
+00000b90: 665f 726f 7574 6572 2e64 6172 747a 055c  f_router.dartz.\
+00000ba0: 6c69 625c e901 0000 00fa 015c fa01 2f7a  lib\.......\../z
+00000bb0: 052f 6c69 622f 5a0b 7464 665f 726f 7574  ./lib/Z.tdf_rout
+00000bc0: 6572 5fe9 0800 0000 e9f8 ffff ff75 2900  er_..........u).
+00000bd0: 0000 e6a8 a1e5 9d97 7b3a 3e33 307d 2020  ........{:>30}  
+00000be0: e6a3 80e6 b58b e588 b020 207b 3a3e 337d  .........  {:>3}
+00000bf0: 2020 e4b8 aae8 b7af e794 b129 2872 0700    .........)(r..
+00000c00: 0000 7223 0000 0072 0800 0000 7227 0000  ..r#...r....r'..
+00000c10: 0072 2800 0000 da05 6368 6469 72da 0470  .r(.....chdir..p
+00000c20: 6174 68da 0665 7869 7374 73da 0673 6875  ath..exists..shu
+00000c30: 7469 6cda 0672 6d74 7265 65da 056d 6b64  til..rmtree..mkd
+00000c40: 6972 721a 0000 00da 1a5f 526f 7574 6572  irr......_Router
+00000c50: 5f5f 6861 7352 6f75 7465 7244 6172 7446  __hasRouterDartF
+00000c60: 696c 65da 0b70 6163 6b61 6765 5061 7468  ile..packagePath
+00000c70: da0b 6765 7453 6865 6c6c 4469 72da 0b70  ..getShellDir..p
+00000c80: 6163 6b61 6765 4e61 6d65 da04 6f70 656e  ackageName..open
+00000c90: da1d 5f52 6f75 7465 725f 5f64 6566 6175  .._Router__defau
+00000ca0: 6c74 496d 706f 7274 4372 6561 746f 72da  ltImportCreator.
+00000cb0: 0570 6f70 656e 7206 0000 00da 0770 7764  .popenr......pwd
+00000cc0: 5f63 6d64 da04 7265 6164 da05 7370 6c69  _cmd..read..spli
+00000cd0: 74da 0477 616c 6bda 046a 6f69 6eda 0865  t..walk..join..e
+00000ce0: 6e64 7377 6974 68da 0a69 735f 7769 6e64  ndswith..is_wind
+00000cf0: 6f77 73da 0772 6570 6c61 6365 7202 0000  ows..replacer...
+00000d00: 00da 0665 6e63 6f64 65da 0968 6578 6469  ...encode..hexdi
+00000d10: 6765 7374 da1a 5f52 6f75 7465 725f 5f69  gest.._Router__i
+00000d20: 6d70 6f72 7444 6174 6143 7265 6174 6f72  mportDataCreator
+00000d30: da06 6170 7065 6e64 da03 6c65 6eda 0573  ..append..len..s
+00000d40: 7461 6765 da06 666f 726d 6174 da20 5f52  tage..format. _R
+00000d50: 6f75 7465 725f 5f67 726f 7570 526f 7574  outer__groupRout
+00000d60: 6572 436c 6173 7343 7265 6174 6f72 da1c  erClassCreator..
+00000d70: 5f52 6f75 7465 725f 5f61 6464 496e 5769  _Router__addInWi
+00000d80: 6e64 6f77 446f 776e 4461 7461 da19 5f52  ndowDownData.._R
+00000d90: 6f75 7465 725f 5f61 6464 496e 4d61 6344  outer__addInMacD
+00000da0: 6f77 6e44 6174 61da 0563 6c6f 7365 2910  ownData..close).
+00000db0: 7212 0000 00da 0b70 6163 6b61 6765 4974  r......packageIt
+00000dc0: 656d da09 6669 6c65 5f6e 616d 65da 0166  em..file_name..f
+00000dd0: da08 6e6f 7761 5061 7468 5a13 726f 7574  ..nowaPathZ.rout
+00000de0: 6572 416c 6961 7346 696c 654c 6973 74da  erAliasFileList.
+00000df0: 0e72 6f75 7465 7246 696c 654c 6973 74da  .routerFileList.
+00000e00: 0472 6f6f 74da 015f da05 6669 6c65 73da  .root.._..files.
+00000e10: 0466 696c 65da 0873 7263 5f66 696c 65da  .file..src_file.
+00000e20: 0e69 7465 6d4d 6f64 756c 654e 616d 65da  .itemModuleName.
+00000e30: 0474 656d 70da 0c69 7465 6d46 696c 6550  .temp..itemFileP
+00000e40: 6174 68da 0d69 7465 6d46 696c 6541 6c69  ath..itemFileAli
+00000e50: 6173 7213 0000 0072 1300 0000 7214 0000  asr....r....r...
+00000e60: 005a 1d5f 5f69 6e74 6567 7261 7465 5f61  .Z.__integrate_a
+00000e70: 6c6c 5f72 6f75 7469 6e67 5f66 696c 6573  ll_routing_files
+00000e80: 4b00 0000 7376 0000 0000 010a 0108 010a  K...sv..........
+00000e90: 010c 010a 010a 010a 010a 020c 0208 010c  ................
+00000ea0: 0112 010c 010c 0104 010a 0104 0104 ff04  ................
+00000eb0: 0308 010c 0212 0102 ff02 0102 ff04 0304  ................
+00000ec0: 0104 0114 0108 010e 010c 0106 010a 010e  ................
+00000ed0: 010e 020e 0202 0116 ff02 ff02 0504 0108  ................
+00000ee0: ff04 030a 0110 010e 0104 0104 010a ff02  ................
+00000ef0: ff04 0504 0108 ff04 030a 010c 020a 027a  ...............z
+00000f00: 2452 6f75 7465 722e 5f5f 696e 7465 6772  $Router.__integr
+00000f10: 6174 655f 616c 6c5f 726f 7574 696e 675f  ate_all_routing_
+00000f20: 6669 6c65 7363 0100 0000 0000 0000 0000  filesc..........
+00000f30: 0000 0e00 0000 0700 0000 4300 0000 7354  ..........C...sT
+00000f40: 0100 0074 00a0 0164 01a1 0101 0074 02a0  ...t...d.....t..
+00000f50: 03a1 0001 0074 04a0 0564 02a1 0101 0064  .....t...d.....d
+00000f60: 037d 0174 067c 0164 0483 027d 0274 046a  .}.t.|.d...}.t.j
+00000f70: 07a0 0864 05a1 0164 066b 0272 4474 04a0  ...d...d.k.rDt..
+00000f80: 0964 05a1 0101 0074 04a0 0564 05a1 0101  .d.....t...d....
+00000f90: 0074 04a0 0a74 0ba0 0ca1 00a1 01a0 0da1  .t...t..........
+00000fa0: 00a0 0e64 07a1 0164 0819 007d 037c 00a0  ...d...d...}.|..
+00000fb0: 0f7c 0264 09a1 0201 007c 00a0 0f7c 0264  .|.d.....|...|.d
+00000fc0: 0aa1 0201 0067 007d 0474 04a0 107c 03a1  .....g.}.t...|..
+00000fd0: 0144 005d a05c 037d 057d 067d 077c 0744  .D.].\.}.}.}.|.D
+00000fe0: 005d 907d 0874 046a 07a0 117c 057c 08a1  .].}.t.j...|.|..
+00000ff0: 027d 097c 09a0 127c 01a1 0164 0b6b 0372  .}.|...|...d.k.r
+00001000: c071 9e74 0ba0 13a1 0072 e47c 09a0 0e64  .q.t.....r.|...d
+00001010: 0ca1 0164 0d19 007d 0a7c 0aa0 1464 0e64  ...d...}.|...d.d
+00001020: 0fa1 027d 0b6e 0e7c 09a0 0e64 0ca1 0164  ...}.n.|...d...d
+00001030: 0d19 007d 0b64 1074 157c 0ba0 16a1 0083  ...}.d.t.|......
+00001040: 01a0 17a1 0064 1164 1285 0219 0017 007d  .....d.d.......}
+00001050: 0c64 13a0 187c 0b7c 0ca1 027d 0d7c 02a0  .d...|.|...}.|..
+00001060: 197c 0da1 0101 007c 04a0 1a7c 0ca1 0101  .|.....|...|....
+00001070: 0071 9e71 907c 02a0 1964 14a0 187c 00a0  .q.q.|...d...|..
+00001080: 1b7c 04a1 01a1 01a1 0101 007c 02a0 1ca1  .|.........|....
+00001090: 0001 0064 0053 0029 154e 751b 0000 00e7  ...d.S.).Nu.....
+000010a0: 949f e688 90e8 b7af e794 b1e5 889d e5a7  ................
+000010b0: 8be5 8c96 e696 87e4 bbb6 fa0d 6c69 622f  ............lib/
+000010c0: 747a 5f72 6f75 7465 727a 0969 6e69 742e  tz_routerz.init.
+000010d0: 6461 7274 7233 0000 0072 3200 0000 4672  dartr3...r2...Fr
+000010e0: 3500 0000 7201 0000 0072 3400 0000 7a22  5...r....r4...z"
+000010f0: 2765 6e74 7279 2f74 7a5f 726f 7574 6572  'entry/tz_router
+00001100: 5f65 6e74 7279 5f70 6167 652e 6461 7274  _entry_page.dart
+00001110: 273b e9ff ffff ff72 3100 0000 7237 0000  ';.....r1...r7..
+00001120: 0072 3800 0000 7239 0000 005a 0b72 6f75  .r8...r9...Z.rou
+00001130: 7465 725f 6d61 705f 723a 0000 0072 3b00  ter_map_r:...r;.
+00001140: 0000 7a16 696d 706f 7274 2022 2e7b 307d  ..z.import ".{0}
+00001150: 2220 6173 207b 317d 3b0a 7ad1 0a0a 2020  " as {1};.z...  
+00001160: 2020 2020 2020 636c 6173 7320 545a 526f        class TZRo
+00001170: 7574 6572 4d61 6e61 6765 7220 7b7b 0a20  uterManager {{. 
+00001180: 2020 2020 2020 2020 2020 2073 7461 7469             stati
+00001190: 6320 636f 6d62 696e 654d 6170 2829 207b  c combineMap() {
+000011a0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000011b0: 2020 4d61 703c 5374 7269 6e67 2c20 5444    Map<String, TD
+000011c0: 4650 6167 6542 7569 6c64 6572 3e20 6d61  FPageBuilder> ma
+000011d0: 7020 3d20 4d61 7028 293b 0a20 2020 2020  p = Map();.     
+000011e0: 2020 2020 2020 2020 2020 207b 307d 0a20             {0}. 
+000011f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00001200: 6574 7572 6e20 6d61 703b 0a20 2020 2020  eturn map;.     
+00001210: 2020 2020 2020 207d 7d0a 2020 2020 2020         }}.      
+00001220: 2020 7d7d 0a20 2020 2020 2020 2029 1d72    }}.        ).r
+00001230: 0700 0000 7223 0000 0072 0800 0000 7227  ....r#...r....r'
+00001240: 0000 0072 2800 0000 723c 0000 0072 4600  ...r(...r<...rF.
+00001250: 0000 723d 0000 0072 3e00 0000 7241 0000  ..r=...r>...rA..
+00001260: 0072 4800 0000 7206 0000 0072 4900 0000  .rH...r....rI...
+00001270: 724a 0000 0072 4b00 0000 7247 0000 0072  rJ...rK...rG...r
+00001280: 4c00 0000 724d 0000 00da 0466 696e 6472  L...rM.....findr
+00001290: 4f00 0000 7250 0000 0072 0200 0000 7251  O...rP...r....rQ
+000012a0: 0000 0072 5200 0000 7257 0000 00da 0577  ...rR...rW.....w
+000012b0: 7269 7465 7254 0000 00da 1e5f 526f 7574  riterT....._Rout
+000012c0: 6572 5f5f 6d61 704c 6973 7443 6f6d 6269  er__mapListCombi
+000012d0: 6e65 4372 6561 7465 7272 5b00 0000 290e  neCreaterr[...).
+000012e0: 7212 0000 0072 5d00 0000 da05 696e 6974  r....r].....init
+000012f0: 4672 5f00 0000 5a07 6d61 704c 6973 7472  Fr_...Z.mapListr
+00001300: 6100 0000 7262 0000 0072 6300 0000 7264  a...rb...rc...rd
+00001310: 0000 0072 6500 0000 5a0f 746d 7049 7465  ...re...Z.tmpIte
+00001320: 6d46 696c 6550 6174 6872 6800 0000 7269  mFilePathrh...ri
+00001330: 0000 005a 0d69 6d70 6f72 7443 6f6e 7465  ...Z.importConte
+00001340: 6e74 7213 0000 0072 1300 0000 7214 0000  ntr....r....r...
+00001350: 005a 1c5f 5f67 656e 6572 6174 655f 726f  .Z.__generate_ro
+00001360: 7574 6572 5f69 6e69 745f 6669 6c65 738e  uter_init_files.
+00001370: 0000 0073 5000 0000 0001 0a01 0801 0a02  ...sP...........
+00001380: 0401 0a03 1001 0a01 0a01 1c01 0401 04ff  ................
+00001390: 0403 0401 04ff 0402 0401 1401 0801 0e01  ................
+000013a0: 0e01 0201 0801 0e01 0e02 0e02 1001 06ff  ................
+000013b0: 04ff 0204 0401 04ff 0403 0a01 0e02 0401  ................
+000013c0: 040a 08f6 02ff 040f 7a23 526f 7574 6572  ........z#Router
+000013d0: 2e5f 5f67 656e 6572 6174 655f 726f 7574  .__generate_rout
+000013e0: 6572 5f69 6e69 745f 6669 6c65 7363 0100  er_init_filesc..
+000013f0: 0000 0000 0000 0000 0000 0300 0000 0900  ................
+00001400: 0000 4300 0000 73ca 0000 0074 00a0 0164  ..C...s....t...d
+00001410: 01a1 0101 0074 02a0 03a1 0001 0074 04a0  .....t.......t..
+00001420: 0564 02a1 0101 0074 046a 06a0 0764 03a1  .d.....t.j...d..
+00001430: 0164 046b 0272 3674 04a0 0864 03a1 0101  .d.k.r6t...d....
+00001440: 0074 04a0 0564 03a1 0101 0064 057d 0174  .t...d.....d.}.t
+00001450: 097c 0164 0664 0764 088d 037d 027c 00a0  .|.d.d.d...}.|..
+00001460: 0a7c 0264 09a1 0201 007c 00a0 0a7c 0264  .|.d.....|...|.d
+00001470: 0aa1 0201 007c 00a0 0a7c 0264 0ba1 0201  .....|...|.d....
+00001480: 007c 00a0 0a7c 0264 0ca1 0201 007c 00a0  .|...|.d.....|..
+00001490: 0a7c 0264 0da1 0201 007c 00a0 0a7c 0264  .|.d.....|...|.d
+000014a0: 0ea1 0201 007c 02a0 0b64 0fa0 0c7c 006a  .....|...d...|.j
+000014b0: 0d7c 006a 0e7c 006a 0f7c 00a0 10a1 007c  .|.j.|.j.|.....|
+000014c0: 006a 0ea1 05a1 0101 007c 02a0 11a1 0001  .j.......|......
+000014d0: 0064 0053 0029 104e 7518 0000 00e7 949f  .d.S.).Nu.......
+000014e0: e688 90e8 b7af e794 b1e5 85a5 e58f a3e6  ................
+000014f0: 9687 e4bb b672 6a00 0000 da05 656e 7472  .....rj.....entr
+00001500: 7946 7a19 747a 5f72 6f75 7465 725f 656e  yFz.tz_router_en
+00001510: 7472 795f 7061 6765 2e64 6172 7472 3300  try_page.dartr3.
+00001520: 0000 da04 7574 6638 a901 da08 656e 636f  ....utf8....enco
+00001530: 6469 6e67 7a20 2770 6163 6b61 6765 3a66  dingz 'package:f
+00001540: 6c75 7474 6572 2f6d 6174 6572 6961 6c2e  lutter/material.
+00001550: 6461 7274 273b 7234 0000 007a 3227 7061  dart';r4...z2'pa
+00001560: 636b 6167 653a 7464 665f 726f 7574 6572  ckage:tdf_router
+00001570: 5f61 6e6e 6f2f 726f 7574 6572 2f72 6f75  _anno/router/rou
+00001580: 7465 725f 616e 6e6f 2e64 6172 7427 3b7a  ter_anno.dart';z
+00001590: 2d27 7061 636b 6167 653a 7464 665f 6261  -'package:tdf_ba
+000015a0: 7365 5f75 7469 6c73 2f74 6466 5f62 6173  se_utils/tdf_bas
+000015b0: 655f 7574 696c 732e 6461 7274 273b 7a32  e_utils.dart';z2
+000015c0: 2770 6163 6b61 6765 3a74 6466 5f77 6964  'package:tdf_wid
+000015d0: 6765 7473 2f74 6466 5f63 6f6d 6d6f 6e5f  gets/tdf_common_
+000015e0: 6274 6e2f 7464 665f 6274 6e2e 6461 7274  btn/tdf_btn.dart
+000015f0: 273b 7a33 2770 6163 6b61 6765 3a74 6466  ';z3'package:tdf
+00001600: 5f77 6964 6765 7473 2f74 6974 6c65 5f62  _widgets/title_b
+00001610: 6172 2f74 6466 5f74 6974 6c65 5f62 6172  ar/tdf_title_bar
+00001620: 2e64 6172 7427 3b75 630d 0000 0a0a 4054  .dart';uc.....@T
+00001630: 5a52 6f75 7465 7228 7061 7468 3a20 277b  ZRouter(path: '{
+00001640: 307d 272c 206e 6f74 653a 2027 7b31 7d27  0}', note: '{1}'
+00001650: 290a 636c 6173 7320 7b32 7d20 6578 7465  ).class {2} exte
+00001660: 6e64 7320 5374 6174 6566 756c 5769 6467  nds StatefulWidg
+00001670: 6574 207b 7b0a 2020 2020 6669 6e61 6c20  et {{.    final 
+00001680: 4d61 7020 7061 7261 6d73 3b0a 0a20 2020  Map params;..   
+00001690: 207b 327d 2874 6869 732e 7061 7261 6d73   {2}(this.params
+000016a0: 293b 0a0a 2020 2020 406f 7665 7272 6964  );..    @overrid
+000016b0: 650a 2020 2020 5f7b 327d 5374 6174 6520  e.    _{2}State 
+000016c0: 6372 6561 7465 5374 6174 6528 2920 3d3e  createState() =>
+000016d0: 205f 7b32 7d53 7461 7465 2829 3b0a 7d7d   _{2}State();.}}
+000016e0: 0a0a 636c 6173 7320 5f7b 327d 5374 6174  ..class _{2}Stat
+000016f0: 6520 6578 7465 6e64 7320 5374 6174 653c  e extends State<
+00001700: 7b32 7d3e 207b 7b0a 2020 2020 6669 6e61  {2}> {{.    fina
+00001710: 6c20 5465 7874 4564 6974 696e 6743 6f6e  l TextEditingCon
+00001720: 7472 6f6c 6c65 7220 726f 7574 6572 436f  troller routerCo
+00001730: 6e74 726f 6c6c 6572 203d 206e 6577 2054  ntroller = new T
+00001740: 6578 7445 6469 7469 6e67 436f 6e74 726f  extEditingContro
+00001750: 6c6c 6572 2829 3b0a 2020 2020 6669 6e61  ller();.    fina
+00001760: 6c20 5465 7874 4564 6974 696e 6743 6f6e  l TextEditingCon
+00001770: 7472 6f6c 6c65 7220 636f 6e74 726f 6c6c  troller controll
+00001780: 6572 203d 206e 6577 2054 6578 7445 6469  er = new TextEdi
+00001790: 7469 6e67 436f 6e74 726f 6c6c 6572 2829  tingController()
+000017a0: 3b0a 2020 2020 6669 6e61 6c20 4d61 703c  ;.    final Map<
+000017b0: 5374 7269 6e67 2c20 5374 7269 6e67 3e20  String, String> 
+000017c0: 7061 6765 4d61 7020 3d20 7b7b 0a20 2020  pageMap = {{.   
+000017d0: 207b 337d 0a20 2020 207d 7d3b 0a0a 2020   {3}.    }};..  
+000017e0: 2020 406f 7665 7272 6964 650a 2020 2020    @override.    
+000017f0: 5769 6467 6574 2062 7569 6c64 2842 7569  Widget build(Bui
+00001800: 6c64 436f 6e74 6578 7420 636f 6e74 6578  ldContext contex
+00001810: 7429 207b 7b0a 2020 2020 2020 2020 5444  t) {{.        TD
+00001820: 4653 6372 6565 6e2e 696e 6974 2863 6f6e  FScreen.init(con
+00001830: 7465 7874 293b 0a20 2020 2020 2020 2072  text);.        r
+00001840: 6574 7572 6e20 5363 6166 666f 6c64 280a  eturn Scaffold(.
+00001850: 2020 2020 2020 2020 2020 2020 6261 636b              back
+00001860: 6772 6f75 6e64 436f 6c6f 723a 2043 6f6c  groundColor: Col
+00001870: 6f72 2830 7866 6666 6666 6666 6629 2c0a  or(0xffffffff),.
+00001880: 2020 2020 2020 2020 2020 2020 6170 7042              appB
+00001890: 6172 3a20 5444 4654 6974 6c65 4261 7228  ar: TDFTitleBar(
+000018a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000018b0: 2074 6974 6c65 436f 6e74 656e 743a 2022   titleContent: "
+000018c0: 7b34 7d22 2c0a 2020 2020 2020 2020 2020  {4}",.          
+000018d0: 2020 2020 2020 6261 636b 5479 7065 3a20        backType: 
+000018e0: 5444 4654 6974 6c65 4261 636b 5769 6467  TDFTitleBackWidg
+000018f0: 6574 5479 7065 2e44 4546 4155 4c54 5f42  etType.DEFAULT_B
+00001900: 4143 4b2c 0a20 2020 2020 2020 2020 2020  ACK,.           
+00001910: 2020 2020 2072 6967 6874 436f 6e74 656e       rightConten
+00001920: 743a 2022 5549 e6a0 87e5 8786 e58c 9622  t: "UI........."
+00001930: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001940: 2020 7269 6768 7443 6f6e 7465 6e74 436f    rightContentCo
+00001950: 6c6f 723a 2030 7866 6630 3038 3866 662c  lor: 0xff0088ff,
+00001960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001970: 2072 6967 6874 5465 7874 4274 6e43 6c69   rightTextBtnCli
+00001980: 636b 3a20 2829 207b 7b0a 2020 2020 2020  ck: () {{.      
+00001990: 2020 2020 2020 2020 2020 5444 4652 6f75            TDFRou
+000019a0: 7465 722e 6f70 656e 2822 7464 662d 6d61  ter.open("tdf-ma
+000019b0: 6e61 6765 723a 2f2f 3264 6669 7265 2e63  nager://2dfire.c
+000019c0: 6f6d 2f74 6963 6b65 742f 696e 6465 7822  om/ticket/index"
+000019d0: 2c20 7572 6c50 6172 616d 733a 207b 7b0a  , urlParams: {{.
+000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019f0: 2020 2020 2261 7070 5f6b 6579 223a 2022      "app_key": "
+00001a00: 3230 3038 3030 222c 0a20 2020 2020 2020  200800",.       
+00001a10: 2020 2020 2020 2020 2020 2020 2022 6835               "h5
+00001a20: 7572 6c22 3a20 2268 7474 703a 2f2f 3130  url": "http://10
+00001a30: 2e31 2e31 362e 3134 3a38 3131 312f 220a  .1.16.14:8111/".
 00001a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a50: 2022 6170 705f 6b65 7922 3a20 2232 3030   "app_key": "200
-00001a60: 3830 3022 2c0a 2020 2020 2020 2020 2020  800",.          
-00001a70: 2020 2020 2020 2020 2020 2268 3575 726c            "h5url
-00001a80: 223a 2022 6874 7470 3a2f 2f31 302e 312e  ": "http://10.1.
-00001a90: 3136 2e31 343a 3831 3131 2f22 0a20 2020  16.14:8111/".   
-00001aa0: 2020 2020 2020 2020 2020 2020 207d 7d29               }})
-00001ab0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00001ac0: 2020 7d7d 2c0a 2020 2020 2020 2020 2020    }},.          
-00001ad0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00001ae0: 2062 6f64 793a 2053 696e 676c 6543 6869   body: SingleChi
-00001af0: 6c64 5363 726f 6c6c 5669 6577 280a 2020  ldScrollView(.  
-00001b00: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00001b10: 696c 643a 2043 6f6c 756d 6e28 0a20 2020  ild: Column(.   
-00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b30: 2063 6869 6c64 7265 6e3a 205f 6765 7442   children: _getB
-00001b40: 7574 746f 6e4c 6973 7428 292c 0a20 2020  uttonList(),.   
-00001b50: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
-00001b60: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00001b70: 2020 2020 2020 2029 3b0a 2020 2020 7d7d         );.    }}
-00001b80: 0a0a 2020 2020 4c69 7374 3c57 6964 6765  ..    List<Widge
-00001b90: 743e 205f 6765 7442 7574 746f 6e4c 6973  t> _getButtonLis
-00001ba0: 7428 2920 7b7b 0a20 2020 2020 2020 204c  t() {{.        L
-00001bb0: 6973 743c 5769 6467 6574 3e20 6c69 7374  ist<Widget> list
-00001bc0: 203d 205b 5d3b 0a20 2020 2020 2020 206c   = [];.        l
-00001bd0: 6973 742e 6164 6428 5f72 6f75 7465 724a  ist.add(_routerJ
-00001be0: 756d 7057 6964 6765 7428 2929 3b0a 2020  umpWidget());.  
-00001bf0: 2020 2020 2020 6c69 7374 2e61 6464 2850        list.add(P
-00001c00: 6164 6469 6e67 280a 2020 2020 2020 2020  adding(.        
-00001c10: 7061 6464 696e 673a 2045 6467 6549 6e73  padding: EdgeIns
-00001c20: 6574 732e 6f6e 6c79 2874 6f70 3a20 3230  ets.only(top: 20
-00001c30: 2e77 292c 0a20 2020 2020 2020 2063 6869  .w),.        chi
-00001c40: 6c64 3a20 5444 4642 7574 746f 6e28 0a20  ld: TDFButton(. 
-00001c50: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
-00001c60: 6e74 3a20 22e6 a0b9 e68d aee8 b7af e794  nt: "...........
-00001c70: b1e8 b7b3 e8bd ac22 2c0a 2020 2020 2020  .......",.      
-00001c80: 2020 2020 2020 6267 436f 6c6f 723a 2030        bgColor: 0
-00001c90: 7866 6630 3038 3866 662c 0a20 2020 2020  xff0088ff,.     
-00001ca0: 2020 2020 2020 2063 6f6e 7465 6e74 436f         contentCo
-00001cb0: 6c6f 723a 2030 7866 6666 6666 6666 662c  lor: 0xffffffff,
-00001cc0: 0a20 2020 2020 2020 2020 2020 206f 6e43  .            onC
-00001cd0: 6c69 636b 3a20 2829 207b 7b0a 2020 2020  lick: () {{.    
-00001ce0: 2020 2020 2020 2020 466f 6375 7353 636f          FocusSco
-00001cf0: 7065 2e6f 6628 636f 6e74 6578 7429 2e72  pe.of(context).r
-00001d00: 6571 7565 7374 466f 6375 7328 466f 6375  equestFocus(Focu
-00001d10: 734e 6f64 6528 2929 3b0a 2020 2020 2020  sNode());.      
-00001d20: 2020 2020 2020 5444 4652 6f75 7465 722e        TDFRouter.
-00001d30: 6f70 656e 2872 6f75 7465 7243 6f6e 7472  open(routerContr
-00001d40: 6f6c 6c65 722e 7465 7874 293b 0a20 2020  oller.text);.   
-00001d50: 2020 2020 2020 2020 207d 7d2c 0a20 2020           }},.   
-00001d60: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-00001d70: 2929 3b0a 2020 2020 2020 2020 6c69 7374  ));.        list
-00001d80: 2e61 6464 285f 7365 6172 6368 5769 6467  .add(_searchWidg
-00001d90: 6574 2829 293b 0a0a 2020 2020 2020 2020  et());..        
-00001da0: 4c69 7374 3c57 6964 6765 743e 2077 7261  List<Widget> wra
-00001db0: 7045 6e74 7279 6c69 7374 203d 205b 5d3b  pEntrylist = [];
-00001dc0: 0a20 2020 2020 2020 2070 6167 654d 6170  .        pageMap
-00001dd0: 2e66 6f72 4561 6368 2828 6b65 792c 2076  .forEach((key, v
-00001de0: 616c 7565 2920 7b7b 0a20 2020 2020 2020  alue) {{.       
-00001df0: 2069 6620 286b 6579 2e63 6f6e 7461 696e   if (key.contain
-00001e00: 7328 636f 6e74 726f 6c6c 6572 2e74 6578  s(controller.tex
-00001e10: 7429 2920 7b7b 0a20 2020 2020 2020 2020  t)) {{.         
-00001e20: 2020 2077 7261 7045 6e74 7279 6c69 7374     wrapEntrylist
-00001e30: 2e61 6464 2847 6573 7475 7265 4465 7465  .add(GestureDete
-00001e40: 6374 6f72 280a 2020 2020 2020 2020 2020  ctor(.          
-00001e50: 2020 2020 2020 6f6e 5461 703a 2028 2920        onTap: () 
-00001e60: 7b7b 0a20 2020 2020 2020 2020 2020 2020  {{.             
-00001e70: 2020 2046 6f63 7573 5363 6f70 652e 6f66     FocusScope.of
-00001e80: 2863 6f6e 7465 7874 292e 7265 7175 6573  (context).reques
-00001e90: 7446 6f63 7573 2846 6f63 7573 4e6f 6465  tFocus(FocusNode
-00001ea0: 2829 293b 0a20 2020 2020 2020 2020 2020  ());.           
-00001eb0: 2020 2020 2054 4446 526f 7574 6572 2e6f       TDFRouter.o
-00001ec0: 7065 6e28 7661 6c75 6529 3b0a 2020 2020  pen(value);.    
-00001ed0: 2020 2020 2020 2020 2020 2020 7d7d 2c0a              }},.
-00001ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ef0: 6368 696c 643a 2043 6c69 7052 5265 6374  child: ClipRRect
-00001f00: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00001f10: 2020 626f 7264 6572 5261 6469 7573 3a20    borderRadius: 
-00001f20: 426f 7264 6572 5261 6469 7573 2e61 6c6c  BorderRadius.all
-00001f30: 2852 6164 6975 732e 6369 7263 756c 6172  (Radius.circular
-00001f40: 2833 2e77 2929 2c0a 2020 2020 2020 2020  (3.w)),.        
-00001f50: 2020 2020 2020 2020 6368 696c 643a 2043          child: C
-00001f60: 6f6e 7461 696e 6572 280a 2020 2020 2020  ontainer(.      
-00001f70: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00001f80: 6c6f 723a 2043 6f6c 6f72 732e 626c 7565  lor: Colors.blue
-00001f90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001fa0: 2020 2020 2020 7061 6464 696e 673a 2045        padding: E
-00001fb0: 6467 6549 6e73 6574 732e 6f6e 6c79 280a  dgeInsets.only(.
-00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fd0: 2020 2020 2020 2020 6c65 6674 3a20 372e          left: 7.
-00001fe0: 772c 2072 6967 6874 3a20 372e 772c 2074  w, right: 7.w, t
-00001ff0: 6f70 3a20 342e 772c 2062 6f74 746f 6d3a  op: 4.w, bottom:
-00002000: 2034 2e77 292c 0a20 2020 2020 2020 2020   4.w),.         
-00002010: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-00002020: 3a20 5465 7874 280a 2020 2020 2020 2020  : Text(.        
-00002030: 2020 2020 2020 2020 2020 2020 6b65 792c              key,
-00002040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002050: 2020 2020 2073 7479 6c65 3a20 5465 7874       style: Text
-00002060: 5374 796c 6528 666f 6e74 5369 7a65 3a20  Style(fontSize: 
-00002070: 3133 2e77 292c 0a20 2020 2020 2020 2020  13.w),.         
-00002080: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-00002090: 2020 2020 2020 2020 2020 2020 2020 292c                ),
-000020a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000020b0: 2029 2929 3b0a 2020 2020 2020 2020 7d7d   )));.        }}
-000020c0: 0a20 2020 2020 2020 207d 7d29 3b0a 2020  .        }});.  
-000020d0: 2020 2020 2020 6c69 7374 2e61 6464 2853        list.add(S
-000020e0: 697a 6564 426f 7828 0a20 2020 2020 2020  izedBox(.       
-000020f0: 2068 6569 6768 743a 2032 302e 772c 0a20   height: 20.w,. 
-00002100: 2020 2020 2020 2029 293b 0a20 2020 2020         ));.     
-00002110: 2020 206c 6973 742e 6164 6428 5772 6170     list.add(Wrap
-00002120: 280a 2020 2020 2020 2020 7370 6163 696e  (.        spacin
-00002130: 673a 2031 352e 772c 0a20 2020 2020 2020  g: 15.w,.       
-00002140: 2072 756e 5370 6163 696e 673a 2031 302e   runSpacing: 10.
-00002150: 772c 0a20 2020 2020 2020 2063 6869 6c64  w,.        child
-00002160: 7265 6e3a 2077 7261 7045 6e74 7279 6c69  ren: wrapEntryli
-00002170: 7374 2c0a 2020 2020 2020 2020 2929 3b0a  st,.        ));.
-00002180: 2020 2020 2020 2020 7265 7475 726e 206c          return l
-00002190: 6973 743b 0a20 2020 207d 7d0a 0a20 2020  ist;.    }}..   
-000021a0: 2057 6964 6765 7420 5f72 6f75 7465 724a   Widget _routerJ
-000021b0: 756d 7057 6964 6765 7428 2920 7b7b 0a20  umpWidget() {{. 
-000021c0: 2020 2020 2020 2072 6574 7572 6e20 5465         return Te
-000021d0: 7874 4669 656c 6428 0a20 2020 2020 2020  xtField(.       
-000021e0: 2063 6f6e 7472 6f6c 6c65 723a 2072 6f75   controller: rou
-000021f0: 7465 7243 6f6e 7472 6f6c 6c65 722c 0a20  terController,. 
-00002200: 2020 2020 2020 2061 7574 6f66 6f63 7573         autofocus
-00002210: 3a20 6661 6c73 652c 0a20 2020 2020 2020  : false,.       
-00002220: 2064 6563 6f72 6174 696f 6e3a 2049 6e70   decoration: Inp
-00002230: 7574 4465 636f 7261 7469 6f6e 2868 696e  utDecoration(hin
-00002240: 7454 6578 743a 2022 e8be 93e5 85a5 e9a1  tText: "........
-00002250: b5e9 9da2 e8b7 afe7 94b1 2229 2c0a 2020  .........."),.  
-00002260: 2020 2020 2020 6f6e 4368 616e 6765 643a        onChanged:
-00002270: 2028 7661 6c75 6529 207b 7b0a 2020 2020   (value) {{.    
-00002280: 2020 2020 2020 2020 7365 7453 7461 7465          setState
-00002290: 2828 2920 7b7b 7d7d 293b 0a20 2020 2020  (() {{}});.     
-000022a0: 2020 2020 2020 207d 7d2c 0a20 2020 2020         }},.     
-000022b0: 2020 2029 3b0a 2020 2020 7d7d 0a0a 2020     );.    }}..  
-000022c0: 2020 5769 6467 6574 205f 7365 6172 6368    Widget _search
-000022d0: 5769 6467 6574 2829 207b 7b0a 2020 2020  Widget() {{.    
-000022e0: 2020 2020 7265 7475 726e 2054 6578 7446      return TextF
-000022f0: 6965 6c64 280a 2020 2020 2020 2020 2020  ield(.          
-00002300: 2020 636f 6e74 726f 6c6c 6572 3a20 636f    controller: co
-00002310: 6e74 726f 6c6c 6572 2c0a 2020 2020 2020  ntroller,.      
-00002320: 2020 2020 2020 6175 746f 666f 6375 733a        autofocus:
-00002330: 2066 616c 7365 2c0a 2020 2020 2020 2020   false,.        
-00002340: 2020 2020 6465 636f 7261 7469 6f6e 3a20      decoration: 
-00002350: 496e 7075 7444 6563 6f72 6174 696f 6e28  InputDecoration(
-00002360: 6869 6e74 5465 7874 3a20 22e7 ad9b e980  hintText: ".....
-00002370: 8922 292c 0a20 2020 2020 2020 2020 2020  ."),.           
-00002380: 206f 6e43 6861 6e67 6564 3a20 2876 616c   onChanged: (val
-00002390: 7565 2920 7b7b 0a20 2020 2020 2020 2020  ue) {{.         
-000023a0: 2020 2020 2020 2073 6574 5374 6174 6528         setState(
-000023b0: 2829 207b 7b7d 7d29 3b0a 2020 2020 2020  () {{}});.      
-000023c0: 2020 2020 2020 7d7d 2c0a 2020 2020 2020        }},.      
-000023d0: 2020 293b 0a20 2020 207d 7d0a 2020 2020    );.    }}.    
-000023e0: 0a7d 7d0a 2020 2020 2020 2020 2912 720a  .}}.        ).r.
-000023f0: 0000 0072 2600 0000 720b 0000 0072 2a00  ...r&...r....r*.
-00002400: 0000 722b 0000 0072 3f00 0000 7240 0000  ..r+...r?...r@..
-00002410: 0072 4100 0000 7244 0000 0072 4900 0000  .rA...rD...rI...
-00002420: 724a 0000 0072 7000 0000 725a 0000 0072  rJ...rp...rZ...r
-00002430: 2000 0000 7221 0000 0072 2200 0000 da1c   ...r!...r".....
-00002440: 5f52 6f75 7465 725f 5f6d 6169 6e50 6167  _Router__mainPag
-00002450: 6544 6174 6143 7265 6174 6f72 725e 0000  eDataCreatorr^..
-00002460: 0029 0372 1500 0000 7260 0000 005a 0a65  .).r....r`...Z.e
-00002470: 6e74 7279 5061 6765 4672 1600 0000 7216  ntryPageFr....r.
-00002480: 0000 0072 1700 0000 5a1d 5f5f 6765 6e65  ...r....Z.__gene
-00002490: 7261 7465 5f72 6f75 7465 725f 656e 7472  rate_router_entr
-000024a0: 795f 6669 6c65 73cb 0000 0073 4800 0000  y_files....sH...
-000024b0: 0001 0a01 0801 0a02 1001 0a02 0a02 0401  ................
-000024c0: 0e02 0401 04ff 0402 0401 04ff 0402 0401  ................
-000024d0: 04ff 0403 0401 04ff 0403 0401 04ff 0403  ................
-000024e0: 0401 04ff 0403 0401 0476 0401 0401 0401  .........v......
-000024f0: 0601 0486 02ff 047e 7a24 526f 7574 6572  .......~z$Router
-00002500: 2e5f 5f67 656e 6572 6174 655f 726f 7574  .__generate_rout
-00002510: 6572 5f65 6e74 7279 5f66 696c 6573 6301  er_entry_filesc.
-00002520: 0000 0000 0000 0000 0000 000b 0000 000e  ................
-00002530: 0000 0043 0000 0073 0e02 0000 7400 a001  ...C...s....t...
-00002540: 6401 a101 0100 7402 a003 a100 0100 7404  d.....t.......t.
-00002550: 6a05 a006 6402 a101 6403 6b02 722c 7407  j...d...d.k.r,t.
-00002560: a008 6402 a101 0100 7404 a009 6402 a101  ..d.....t...d...
-00002570: 0100 7404 a00a 6402 a101 0100 740b 6404  ..t...d.....t.d.
-00002580: 6405 8302 7d01 7402 a003 a100 0100 7402  d...}.t.......t.
-00002590: a00c a100 7d02 7404 a00d 7c02 a101 4400  ....}.t...|...D.
-000025a0: 9001 5d36 5c03 7d03 7d04 7d05 7c05 4400  ..]6\.}.}.}.|.D.
-000025b0: 9001 5d24 7d06 7404 6a05 a00e 7c03 7c06  ..]$}.t.j...|.|.
-000025c0: a102 7d07 7c07 a00f 6406 a101 6407 6b03  ..}.|...d...d.k.
-000025d0: 7274 7410 a011 a100 9001 722a 740b 6406  rtt.......r*t.d.
-000025e0: 6408 8302 8f6c 7d08 7c08 4400 5d56 7d09  d....l}.|.D.]V}.
-000025f0: 7c09 a00f 7412 6409 640a 640b 8d02 a101  |...t.d.d.d.....
-00002600: 6407 6b03 9001 7200 7c01 a013 640c a014  d.k...r.|...d...
-00002610: 7c09 a015 7412 6409 640a 640b 8d02 a101  |...t.d.d.d.....
-00002620: 640d 1900 a015 7412 640e 640a 640b 8d02  d.....t.d.d.d...
-00002630: a101 640f 1900 a101 a101 0100 0100 9001  ..d.............
-00002640: 7108 71b0 5700 6400 0400 0400 8303 0100  q.q.W.d.........
-00002650: 6e12 3100 9001 731e 3000 0100 0100 0100  n.1...s.0.......
-00002660: 5900 0100 7174 740b 6406 8301 8f56 7d08  Y...qtt.d....V}.
-00002670: 7c08 4400 5d40 7d09 7c09 a00f 6409 a101  |.D.]@}.|...d...
-00002680: 6407 6b03 9001 7270 7c01 a013 640c a014  d.k...rp|...d...
-00002690: 7c09 a015 6409 a101 640d 1900 a015 640e  |...d...d.....d.
-000026a0: a101 640f 1900 a101 a101 0100 0100 9001  ..d.............
-000026b0: 717a 9001 7138 5700 6400 0400 0400 8303  qz..q8W.d.......
-000026c0: 0100 7174 3100 9001 7390 3000 0100 0100  ..qt1...s.0.....
-000026d0: 0100 5900 0100 7174 7164 7c01 a013 6410  ..Y...qtqd|...d.
-000026e0: a014 6411 6412 6413 a103 a101 0100 7c01  ..d.d.d.......|.
-000026f0: a013 6414 a101 0100 7c00 6a16 4400 5d34  ..d.....|.j.D.]4
-00002700: 7d0a 7c01 a013 6415 a014 7c0a 6a17 7c0a  }.|...d...|.j.|.
-00002710: 6a18 6416 7c0a 6a19 1700 6417 7c0a 6a1a  j.d.|.j...d.|.j.
-00002720: 1700 6418 7c0a 6a1b 1700 a105 a101 0100  ..d.|.j.........
-00002730: 9001 71c2 7c01 a013 6419 a101 0100 7c01  ..q.|...d.....|.
-00002740: a01c a100 0100 6400 5300 291a 4e75 1200  ......d.S.).Nu..
-00002750: 0000 e794 9fe6 8890 e8b7 afe7 94b1 e696  ................
-00002760: 87e6 a1a3 750c 0000 00e8 b7af e794 b1e6  ....u...........
-00002770: 9687 e6a1 a354 7a0b 646f 6375 6d65 6e74  .....Tz.document
-00002780: 2e6d 6472 3600 0000 7a0c 7075 6273 7065  .mdr6...z.pubspe
-00002790: 632e 7961 6d6c 726e 0000 00da 0272 627a  c.yamlrn.....rbz
-000027a0: 066e 616d 653a 2072 7400 0000 7275 0000  .name: rt...ru..
-000027b0: 0075 2600 0000 2323 2046 6c75 7474 6572  .u&...## Flutter
-000027c0: e5a3 b3e5 ba94 e794 a8ef bc88 7b30 7def  ............{0}.
-000027d0: bc89 e8b7 afe7 94b1 e8a1 a80a 723a 0000  ............r:..
-000027e0: 0072 3800 0000 7201 0000 007a 683c 7461  .r8...r....zh<ta
-000027f0: 626c 653e 3c74 6865 6164 3e3c 7472 3e3c  ble><thead><tr><
-00002800: 7468 3e7b 307d 3c2f 7468 3e3c 7468 2073  th>{0}</th><th s
-00002810: 7479 6c65 203d 2022 6d69 6e2d 7769 6474  tyle = "min-widt
-00002820: 683a 3135 3070 7820 2169 6d70 6f72 7461  h:150px !importa
-00002830: 6e74 223e 7b31 7d3c 2f74 683e 3c74 683e  nt">{1}</th><th>
-00002840: 7b32 7d3c 2f74 683e 3c2f 7472 3e3c 2f74  {2}</th></tr></t
-00002850: 6865 6164 3e75 0900 0000 e7bb 84e4 bbb6  head>u..........
-00002860: e590 8d75 0600 0000 e68f 8fe8 bfb0 7506  ...u..........u.
-00002870: 0000 00e8 afa6 e683 857a 073c 7462 6f64  .........z.<tbod
-00002880: 793e 7a3e 3c74 723e 3c74 683e 7b30 7d3c  y>z><tr><th>{0}<
-00002890: 2f74 683e 3c74 683e 7b31 7d3c 2f74 683e  /th><th>{1}</th>
-000028a0: 3c74 683e 7b32 7d3c 6272 2f3e 7b33 7d3c  <th>{2}<br/>{3}<
-000028b0: 6272 2f3e 7b34 7d3c 2f74 683e 3c2f 7472  br/>{4}</th></tr
-000028c0: 3e0a 7509 0000 00e7 b1bb e590 8d3a 2020  >.u..........:  
-000028d0: 7509 0000 00e8 b7af e794 b13a 2020 7509  u..........:  u.
-000028e0: 0000 00e6 9687 e4bb b63a 2020 7a10 3c2f  .........:  z.</
-000028f0: 7462 6f64 793e 3c2f 7461 626c 653e 291d  tbody></table>).
-00002900: 720a 0000 0072 2600 0000 720b 0000 0072  r....r&...r....r
-00002910: 2a00 0000 722b 0000 0072 4000 0000 7241  *...r+...r@...rA
-00002920: 0000 0072 4200 0000 7243 0000 0072 4400  ...rB...rC...rD.
-00002930: 0000 723f 0000 0072 4900 0000 7247 0000  ..r?...rI...rG..
-00002940: 0072 4f00 0000 7250 0000 0072 6f00 0000  .rO...rP...ro...
-00002950: 7209 0000 0072 5200 0000 da05 6279 7465  r....rR.....byte
-00002960: 7372 7000 0000 725a 0000 0072 4e00 0000  srp...rZ...rN...
-00002970: 721e 0000 0072 0e00 0000 7211 0000 0072  r....r....r....r
-00002980: 1200 0000 720f 0000 0072 1000 0000 725e  ....r....r....r^
-00002990: 0000 0029 0b72 1500 0000 7261 0000 005a  ...).r....ra...Z
-000029a0: 0663 7572 4469 7272 6400 0000 da04 6469  .curDirrd.....di
-000029b0: 7273 7266 0000 0072 6700 0000 7268 0000  rsrf...rg...rh..
-000029c0: 00da 056c 696e 6573 da04 6c69 6e65 da04  ...lines..line..
-000029d0: 6974 656d 7216 0000 0072 1600 0000 7217  itemr....r....r.
-000029e0: 0000 005a 155f 5f67 656e 6572 6174 655f  ...Z.__generate_
-000029f0: 726f 7574 6572 5f64 6f63 6901 0000 7384  router_doci...s.
-00002a00: 0000 0000 010a 0108 0110 010a 010a 010a  ................
-00002a10: 020a 0208 0208 0116 010a 010e 010e 010a  ................
-00002a20: 010c 0108 0118 0104 0104 0104 0102 0104  ................
-00002a30: ff04 ff02 0302 fd04 030a fd02 0302 fd02  ................
-00002a40: ff02 ff04 082a 020a 0108 0110 0104 0104  .....*..........
-00002a50: 0108 0102 ff04 0102 ff02 0102 ff02 ff02  ................
-00002a60: ff04 062e 0204 0104 0106 ff02 ff04 050a  ................
-00002a70: 020a 0104 0104 0104 0104 0108 0108 0108  ................
-00002a80: fb02 ff08 0a0a 027a 1c52 6f75 7465 722e  .......z.Router.
-00002a90: 5f5f 6765 6e65 7261 7465 5f72 6f75 7465  __generate_route
-00002aa0: 725f 646f 6363 0100 0000 0000 0000 0000  r_docc..........
-00002ab0: 0000 0100 0000 0300 0000 4300 0000 7316  ..........C...s.
-00002ac0: 0000 0074 00a0 01a1 0001 0074 02a0 0364  ...t.......t...d
-00002ad0: 01a1 0101 0064 0053 0029 024e 7a17 6461  .....d.S.).Nz.da
-00002ae0: 7274 2066 6f72 6d61 7420 2e2f 747a 5f72  rt format ./tz_r
-00002af0: 6f75 7465 7229 0472 0b00 0000 da0f 676f  outer).r......go
-00002b00: 496e 5368 656c 6c4c 6962 4469 7272 2b00  InShellLibDirr+.
-00002b10: 0000 da06 7379 7374 656d 7214 0000 0072  ....systemr....r
-00002b20: 1600 0000 7216 0000 0072 1700 0000 7232  ....r....r....r2
-00002b30: 0000 00aa 0100 0073 0400 0000 0001 0801  .......s........
-00002b40: 7a11 526f 7574 6572 2e5f 5f66 6f72 6d61  z.Router.__forma
-00002b50: 745f 5f29 0272 7c00 0000 da06 7265 7475  t__).r|.....retu
-00002b60: 726e 6302 0000 0000 0000 0000 0000 0005  rnc.............
-00002b70: 0000 0004 0000 0043 0000 0073 8200 0000  .......C...s....
-00002b80: 7c01 a000 6401 a101 6402 1900 7d02 7c01  |...d...d...}.|.
-00002b90: a000 6401 a101 6403 1900 a001 6404 6405  ..d...d.....d.d.
-00002ba0: a102 7d03 7c02 a002 6406 a101 6407 6b03  ..}.|...d...d.k.
-00002bb0: 727e 7403 8300 7d04 7c02 7c04 5f04 7405  r~t...}.|.|._.t.
-00002bc0: a006 a100 725e 7c03 6403 7407 7c03 8301  ....r^|.d.t.|...
-00002bd0: 6408 1800 8502 1900 7c04 5f08 6e16 7c03  d.......|._.n.|.
-00002be0: 6402 7407 7c03 8301 6408 1800 8502 1900  d.t.|...d.......
-00002bf0: 7c04 5f08 6409 7c04 5f09 7c04 5300 6400  |._.d.|._.|.S.d.
-00002c00: 5300 290a 4e7a 083a 6669 6c65 3a2f 2f72  S.).Nz.:file://r
-00002c10: 0100 0000 723a 0000 00fa 0325 3235 fa01  ....r:.....%25..
-00002c20: 25da 0374 6466 726e 0000 00e9 0500 0000  %..tdfrn........
-00002c30: 5429 0a72 4e00 0000 7253 0000 0072 6f00  T).rN...rS...ro.
-00002c40: 0000 7207 0000 0072 4800 0000 7209 0000  ..r....rH...r...
-00002c50: 0072 5200 0000 7258 0000 0072 4600 0000  .rR...rX...rF...
-00002c60: da08 6973 5265 6d6f 7465 a905 7215 0000  ..isRemote..r...
-00002c70: 0072 7c00 0000 7248 0000 0072 4600 0000  .r|...rH...rF...
-00002c80: da0b 7061 636b 6167 654e 6f64 6572 1600  ..packageNoder..
-00002c90: 0000 7216 0000 0072 1700 0000 da1a 5f5f  ..r....r......__
-00002ca0: 6765 7452 656d 6f74 6543 6f64 6550 6163  getRemoteCodePac
-00002cb0: 6b61 6765 5061 7468 af01 0000 7314 0000  kagePath....s...
-00002cc0: 0000 010e 0116 010e 0106 0106 0108 0118  ................
-00002cd0: 0216 0106 017a 2152 6f75 7465 722e 5f5f  .....z!Router.__
-00002ce0: 6765 7452 656d 6f74 6543 6f64 6550 6163  getRemoteCodePac
-00002cf0: 6b61 6765 5061 7468 6302 0000 0000 0000  kagePathc.......
-00002d00: 0000 0000 0005 0000 0004 0000 0043 0000  .............C..
-00002d10: 0073 6200 0000 7c01 a000 6401 a101 6402  .sb...|...d...d.
-00002d20: 1900 7d02 7c01 a000 6401 a101 6403 1900  ..}.|...d...d...
-00002d30: a001 6404 6405 a102 7d03 7c02 a002 6406  ..d.d...}.|...d.
-00002d40: a101 6407 6b03 725e 7403 8300 7d04 7c02  ..d.k.r^t...}.|.
-00002d50: 7c04 5f04 7c03 6402 7405 7c03 8301 6408  |._.|.d.t.|...d.
-00002d60: 1800 8502 1900 7c04 5f06 6409 7c04 5f07  ......|._.d.|._.
-00002d70: 7c04 5300 6400 5300 290a 4efa 013a 7201  |.S.d.S.).N..:r.
-00002d80: 0000 0072 3a00 0000 7281 0000 0072 8200  ...r:...r....r..
-00002d90: 0000 7283 0000 0072 6e00 0000 7284 0000  ..r....rn...r...
-00002da0: 0046 2908 724e 0000 0072 5300 0000 726f  .F).rN...rS...ro
-00002db0: 0000 0072 0700 0000 7248 0000 0072 5800  ...r....rH...rX.
-00002dc0: 0000 7246 0000 0072 8500 0000 7286 0000  ..rF...r....r...
-00002dd0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00002de0: da1a 5f5f 6765 7453 6f75 7263 6543 6f64  ..__getSourceCod
-00002df0: 6550 6163 6b61 6765 5061 7468 bc01 0000  ePackagePath....
-00002e00: 7310 0000 0000 010e 0116 010e 0106 0106  s...............
-00002e10: 0116 0106 017a 2152 6f75 7465 722e 5f5f  .....z!Router.__
-00002e20: 6765 7453 6f75 7263 6543 6f64 6550 6163  getSourceCodePac
-00002e30: 6b61 6765 5061 7468 6302 0000 0000 0000  kagePathc.......
-00002e40: 0000 0000 0008 0000 0006 0000 0043 0000  .............C..
-00002e50: 0073 6a00 0000 7400 a001 7c01 a101 0100  .sj...t...|.....
-00002e60: 7400 a002 7403 a004 a100 a101 a005 a100  t...t...........
-00002e70: a006 6401 a101 6402 1900 7d02 7400 a007  ..d...d...}.t...
-00002e80: 7c02 a101 4400 5d34 5c03 7d03 7d04 7d05  |...D.]4\.}.}.}.
-00002e90: 7c05 4400 5d24 7d06 7400 6a08 a009 7c03  |.D.]$}.t.j...|.
-00002ea0: 7c06 a102 7d07 7c07 a00a 6403 a101 723e  |...}.|...d...r>
-00002eb0: 0100 0100 6404 5300 713e 7130 6405 5300  ....d.S.q>q0d.S.
-00002ec0: 2906 4e72 3800 0000 7201 0000 0072 3900  ).Nr8...r....r9.
-00002ed0: 0000 5446 290b 722b 0000 0072 3f00 0000  ..TF).r+...r?...
-00002ee0: 724b 0000 0072 0900 0000 724c 0000 0072  rK...r....rL...r
-00002ef0: 4d00 0000 724e 0000 0072 4f00 0000 7240  M...rN...rO...r@
-00002f00: 0000 0072 5000 0000 7251 0000 0029 0872  ...rP...rQ...).r
-00002f10: 1500 0000 5a07 6469 7250 6174 6872 6200  ....Z.dirPathrb.
-00002f20: 0000 7264 0000 0072 7a00 0000 7266 0000  ..rd...rz...rf..
-00002f30: 0072 6700 0000 7268 0000 0072 1600 0000  .rg...rh...r....
-00002f40: 7216 0000 0072 1700 0000 5a13 5f5f 6861  r....r....Z.__ha
-00002f50: 7352 6f75 7465 7244 6172 7446 696c 65c7  sRouterDartFile.
-00002f60: 0100 0073 1000 0000 0001 0a01 1c01 1401  ...s............
-00002f70: 0801 0e01 0a01 0c01 7a1a 526f 7574 6572  ........z.Router
-00002f80: 2e5f 5f68 6173 526f 7574 6572 4461 7274  .__hasRouterDart
-00002f90: 4669 6c65 6303 0000 0000 0000 0000 0000  Filec...........
-00002fa0: 0003 0000 0005 0000 0043 0000 0073 1400  .........C...s..
-00002fb0: 0000 7c01 a000 6401 a001 7c02 a101 a101  ..|...d...|.....
-00002fc0: 0100 6400 5300 2902 4e7a 0b69 6d70 6f72  ..d.S.).Nz.impor
-00002fd0: 7420 7b30 7d0a a902 7270 0000 0072 5a00  t {0}...rp...rZ.
-00002fe0: 0000 2903 7215 0000 00da 0b6d 4669 6c65  ..).r......mFile
-00002ff0: 5772 6974 6572 da07 636f 6e74 656e 7472  Writer..contentr
-00003000: 1600 0000 7216 0000 0072 1700 0000 5a16  ....r....r....Z.
-00003010: 5f5f 6465 6661 756c 7449 6d70 6f72 7443  __defaultImportC
-00003020: 7265 6174 6f72 d101 0000 7302 0000 0000  reator....s.....
-00003030: 017a 1d52 6f75 7465 722e 5f5f 6465 6661  .z.Router.__defa
-00003040: 756c 7449 6d70 6f72 7443 7265 6174 6f72  ultImportCreator
-00003050: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
-00003060: 0007 0000 0043 0000 0073 1800 0000 7c01  .....C...s....|.
-00003070: a000 6401 a001 7c02 7c03 7c04 a103 a101  ..d...|.|.|.....
-00003080: 0100 6400 5300 2902 4e7a 2169 6d70 6f72  ..d.S.).Nz!impor
-00003090: 7420 2270 6163 6b61 6765 3a7b 307d 2f7b  t "package:{0}/{
-000030a0: 317d 2220 6173 207b 327d 3b0a 728b 0000  1}" as {2};.r...
-000030b0: 0029 0572 1500 0000 728c 0000 0072 6900  .).r....r....ri.
-000030c0: 0000 5a09 6d46 696c 6550 6174 6872 6c00  ..Z.mFilePathrl.
-000030d0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-000030e0: 005a 135f 5f69 6d70 6f72 7444 6174 6143  .Z.__importDataC
-000030f0: 7265 6174 6f72 d501 0000 730a 0000 0000  reator....s.....
-00003100: 0304 0104 0106 ff02 ff7a 1a52 6f75 7465  .........z.Route
-00003110: 722e 5f5f 696d 706f 7274 4461 7461 4372  r.__importDataCr
-00003120: 6561 746f 7229 0172 8c00 0000 6304 0000  eator).r....c...
-00003130: 0000 0000 0000 0000 0005 0000 0008 0000  ................
-00003140: 0043 0000 0073 2000 0000 6401 7d04 7c01  .C...s ...d.}.|.
-00003150: a000 7c04 a001 7c02 7c00 a002 7c03 a101  ..|...|.|...|...
-00003160: a102 a101 0100 6400 5300 2902 4e7a 700a  ......d.S.).Nzp.
-00003170: 2020 2020 726f 7574 6572 4d61 7028 2920      routerMap() 
-00003180: 7b7b 0a20 2020 2020 2020 204d 6170 3c53  {{.        Map<S
-00003190: 7472 696e 672c 2054 4446 5061 6765 4275  tring, TDFPageBu
-000031a0: 696c 6465 723e 206d 6170 203d 204d 6170  ilder> map = Map
-000031b0: 2829 3b0a 2020 2020 2020 2020 7b31 7d0a  ();.        {1}.
-000031c0: 2020 2020 2020 2020 7265 7475 726e 206d          return m
-000031d0: 6170 3b0a 2020 2020 7d7d 0a20 2020 2029  ap;.    }}.    )
-000031e0: 0372 7000 0000 725a 0000 00da 1a5f 526f  .rp...rZ....._Ro
-000031f0: 7574 6572 5f5f 6d61 7041 6464 4c69 7374  uter__mapAddList
-00003200: 4372 6561 746f 7229 0572 1500 0000 728c  Creator).r....r.
-00003210: 0000 00da 0a6d 6f64 756c 654e 616d 65da  .....moduleName.
-00003220: 046c 6973 7472 8d00 0000 7216 0000 0072  .listr....r....r
-00003230: 1600 0000 7217 0000 005a 195f 5f67 726f  ....r....Z.__gro
-00003240: 7570 526f 7574 6572 436c 6173 7343 7265  upRouterClassCre
-00003250: 6174 6f72 df01 0000 7308 0000 0000 0104  ator....s.......
-00003260: 0708 010a ff7a 2052 6f75 7465 722e 5f5f  .....z Router.__
-00003270: 6772 6f75 7052 6f75 7465 7243 6c61 7373  groupRouterClass
-00003280: 4372 6561 746f 7263 0200 0000 0000 0000  Creatorc........
-00003290: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
-000032a0: 7322 0000 0064 017d 027c 0144 005d 147d  s"...d.}.|.D.].}
-000032b0: 037c 0264 02a0 007c 037c 03a1 0237 007d  .|.d...|.|...7.}
-000032c0: 0271 087c 0253 0029 034e 720d 0000 007a  .q.|.S.).Nr....z
-000032d0: 7b6d 6170 2e70 7574 4966 4162 7365 6e74  {map.putIfAbsent
-000032e0: 287b 307d 2e67 6574 526f 7574 6572 5061  ({0}.getRouterPa
-000032f0: 7468 2829 2c20 2829 203d 3e20 2028 5374  th(), () =>  (St
-00003300: 7269 6e67 2070 6167 654e 616d 652c 204d  ring pageName, M
-00003310: 6170 2070 6172 616d 732c 2053 7472 696e  ap params, Strin
-00003320: 6720 5f29 203d 3e20 7b31 7d2e 6765 7450  g _) => {1}.getP
-00003330: 6167 6557 6964 6765 7428 7061 7261 6d73  ageWidget(params
-00003340: 2929 3b0a 2020 2020 2020 2020 2901 725a  ));.        ).rZ
-00003350: 0000 00a9 0472 1500 0000 7290 0000 0072  .....r....r....r
-00003360: 8d00 0000 727d 0000 0072 1600 0000 7216  ....r}...r....r.
-00003370: 0000 0072 1700 0000 5a13 5f5f 6d61 7041  ...r....Z.__mapA
-00003380: 6464 4c69 7374 4372 6561 746f 72ea 0100  ddListCreator...
-00003390: 0073 0c00 0000 0001 0401 0801 0602 04fe  .s..............
-000033a0: 0804 7a1a 526f 7574 6572 2e5f 5f6d 6170  ..z.Router.__map
-000033b0: 4164 644c 6973 7443 7265 6174 6f72 6302  AddListCreatorc.
-000033c0: 0000 0000 0000 0000 0000 000a 0000 000a  ................
-000033d0: 0000 0043 0000 0073 0002 0000 7400 6401  ...C...s....t.d.
-000033e0: 6402 6403 8d02 7d02 7c01 4400 9001 5de8  d.d...}.|.D...].
-000033f0: 7d03 7c03 7d04 7401 7c03 8301 6404 6b04  }.|.}.t.|...d.k.
-00003400: 7236 6405 7d05 7c03 7d06 7c05 7c03 1700  r6d.}.|.}.|.|...
-00003410: 7d04 7402 7c04 6406 8302 9001 8fa6 7d07  }.t.|.d.......}.
-00003420: 7403 8300 7d08 7c07 4400 9001 5d64 7d09  t...}.|.D...]d}.
-00003430: 7c09 a004 7400 6407 6402 6403 8d02 a101  |...t.d.d.d.....
-00003440: 6408 6b03 728c 7c09 a005 7400 6409 6402  d.k.r.|...t.d.d.
-00003450: 6403 8d02 a101 640a 1900 a005 7c02 a101  d.....d.....|...
-00003460: 640b 1900 7c08 5f06 7c09 a004 7400 640c  d...|._.|...t.d.
-00003470: 6402 6403 8d02 a101 6408 6b03 72c4 7c09  d.d.....d.k.r.|.
-00003480: a005 7400 640c 6402 6403 8d02 a101 640a  ..t.d.d.d.....d.
-00003490: 1900 a005 7c02 a101 640b 1900 7c08 5f07  ....|...d...|._.
-000034a0: 7c09 a004 7400 640d 6402 6403 8d02 a101  |...t.d.d.d.....
-000034b0: 6408 6b03 72fc 7c09 a005 7400 640d 6402  d.k.r.|...t.d.d.
-000034c0: 6403 8d02 a101 640a 1900 a005 7c02 a101  d.....d.....|...
-000034d0: 640b 1900 7c08 5f08 7c09 a004 7400 640e  d...|._.|...t.d.
-000034e0: 6402 6403 8d02 a101 6408 6b03 9001 723e  d.d.....d.k...r>
-000034f0: 7409 7c09 a005 7400 640e 6402 6403 8d02  t.|...t.d.d.d...
-00003500: a101 640a 1900 a005 7c02 a101 640b 1900  ..d.....|...d...
-00003510: 6402 6403 8d02 7c08 5f0a 7c09 a004 7400  d.d...|._.|...t.
-00003520: 640f 6402 6403 8d02 a101 6408 6b03 9001  d.d.d.....d.k...
-00003530: 7278 7c09 a005 7400 640f 6402 6403 8d02  rx|...t.d.d.d...
-00003540: a101 640a 1900 a005 7c02 a101 640b 1900  ..d.....|...d...
-00003550: 7c08 5f0b 7c09 a004 7400 6410 6402 6403  |._.|...t.d.d.d.
-00003560: 8d02 a101 6408 6b03 724e 7c09 a005 7400  ....d.k.rN|...t.
-00003570: 6410 6402 6403 8d02 a101 640a 1900 a005  d.d.d.....d.....
-00003580: 7c02 a101 640b 1900 6411 6b02 7c08 5f0c  |...d...d.k.|._.
-00003590: 714e 7c00 6a0d a00e 7c08 a101 0100 7c08  qN|.j...|.....|.
-000035a0: 6a0c 6412 6b02 9001 72da 7c00 6a0f a00e  j.d.k...r.|.j...
-000035b0: 7c08 a101 0100 5700 6400 0400 0400 8303  |.....W.d.......
-000035c0: 0100 7110 3100 9001 73f0 3000 0100 0100  ..q.1...s.0.....
-000035d0: 0100 5900 0100 7110 6400 5300 2913 4e72  ..Y...q.d.S.).Nr
-000035e0: 3800 0000 7274 0000 0072 7500 0000 6904  8...rt...ru...i.
-000035f0: 0100 007a 045c 5c3f 5c72 7800 0000 7a0e  ...z.\\?\rx...z.
-00003600: 202f 2f23 7061 636b 6167 6523 2f2f 726e   //#package#//rn
-00003610: 0000 00fa 0d2f 2f23 7061 636b 6167 6523  .....//#package#
-00003620: 2f2f 723a 0000 0072 0100 0000 fa10 2f2f  //r:...r......//
-00003630: 2372 6f75 7465 7250 6174 6823 2f2f fa0e  #routerPath#//..
-00003640: 2f2f 2366 696c 6550 6174 6823 2f2f fa0a  //#filePath#//..
-00003650: 2f2f 236e 6f74 6523 2f2f fa10 2f2f 2370  //#note#//..//#p
-00003660: 6167 6557 6964 6765 7423 2f2f fa10 2f2f  ageWidget#//..//
-00003670: 2369 734d 6169 6e50 6167 6523 2f2f da04  #isMainPage#//..
-00003680: 7472 7565 5429 1072 7900 0000 7258 0000  trueT).ry...rX..
-00003690: 0072 4900 0000 720c 0000 0072 6f00 0000  .rI...r....ro...
-000036a0: 724e 0000 0072 0e00 0000 720f 0000 0072  rN...r....r....r
-000036b0: 1000 0000 da03 7374 7272 1100 0000 7212  ......strr....r.
-000036c0: 0000 0072 1300 0000 721e 0000 0072 5700  ...r....r....rW.
-000036d0: 0000 721f 0000 0029 0a72 1500 0000 7263  ..r....).r....rc
-000036e0: 0000 005a 0962 7974 6573 5465 6d70 da08  ...Z.bytesTemp..
-000036f0: 6669 6c65 4974 656d da06 7265 7375 6c74  fileItem..result
-00003700: 726a 0000 005a 0574 656d 7032 727b 0000  rj...Z.temp2r{..
-00003710: 00da 046e 6f64 6572 7c00 0000 7216 0000  ...noder|...r...
-00003720: 0072 1600 0000 7217 0000 005a 155f 5f61  .r....r....Z.__a
-00003730: 6464 496e 5769 6e64 6f77 446f 776e 4461  ddInWindowDownDa
-00003740: 7461 f301 0000 7392 0000 0000 010c 010a  ta....s.........
-00003750: 0104 010c 0104 0104 0108 010e 0106 010a  ................
-00003760: 0116 0104 010a ff02 0202 fe04 0202 fe02  ................
-00003770: 0202 fe06 0316 0104 010a ff02 0202 fe04  ................
-00003780: 0202 fe02 0202 fe06 0316 0104 010a ff02  ................
-00003790: 0202 fe04 0202 fe02 0202 fe06 0318 0102  ................
-000037a0: 0116 0102 ff02 0202 fe02 0302 fc08 0618  ................
-000037b0: 0104 010a ff02 0202 fe04 0202 fe02 0202  ................
-000037c0: fe06 0316 0210 0102 ff04 0202 fe02 0202  ................
-000037d0: fe02 0302 fd02 ff06 060c 010c 017a 1c52  .............z.R
-000037e0: 6f75 7465 722e 5f5f 6164 6449 6e57 696e  outer.__addInWin
-000037f0: 646f 7744 6f77 6e44 6174 6163 0200 0000  dowDownDatac....
-00003800: 0000 0000 0000 0000 0600 0000 0900 0000  ................
-00003810: 4300 0000 7364 0100 007c 0144 0090 015d  C...sd...|.D...]
-00003820: 587d 0274 007c 0283 0190 018f 387d 0374  X}.t.|......8}.t
-00003830: 0183 007d 047c 0344 005d f87d 057c 05a0  ...}.|.D.].}.|..
-00003840: 0264 01a1 0164 026b 0372 4c7c 05a0 0364  .d...d.k.rL|...d
-00003850: 01a1 0164 0319 00a0 0364 04a1 0164 0519  ...d.....d...d..
-00003860: 007c 045f 047c 05a0 0264 06a1 0164 026b  .|._.|...d...d.k
-00003870: 0372 747c 05a0 0364 06a1 0164 0319 00a0  .rt|...d...d....
-00003880: 0364 04a1 0164 0519 007c 045f 057c 05a0  .d...d...|._.|..
-00003890: 0264 07a1 0164 026b 0372 9c7c 05a0 0364  .d...d.k.r.|...d
-000038a0: 07a1 0164 0319 00a0 0364 04a1 0164 0519  ...d.....d...d..
-000038b0: 007c 045f 067c 05a0 0264 08a1 0164 026b  .|._.|...d...d.k
-000038c0: 0372 c47c 05a0 0364 08a1 0164 0319 00a0  .r.|...d...d....
-000038d0: 0364 04a1 0164 0519 007c 045f 077c 05a0  .d...d...|._.|..
-000038e0: 0264 09a1 0164 026b 0372 ec7c 05a0 0364  .d...d.k.r.|...d
-000038f0: 09a1 0164 0319 00a0 0364 04a1 0164 0519  ...d.....d...d..
-00003900: 007c 045f 087c 05a0 0264 0aa1 0164 026b  .|._.|...d...d.k
-00003910: 0372 207c 05a0 0364 0aa1 0164 0319 00a0  .r |...d...d....
-00003920: 0364 04a1 0164 0519 0064 0b6b 027c 045f  .d...d...d.k.|._
-00003930: 0971 207c 006a 0aa0 0b7c 04a1 0101 007c  .q |.j...|.....|
-00003940: 046a 0964 0c6b 0290 0172 3e7c 006a 0ca0  .j.d.k...r>|.j..
-00003950: 0b7c 04a1 0101 0057 0064 0004 0004 0083  .|.....W.d......
-00003960: 0301 0071 0431 0090 0173 5430 0001 0001  ...q.1...sT0....
-00003970: 0001 0059 0001 0071 0464 0053 0029 0d4e  ...Y...q.d.S.).N
-00003980: 7292 0000 0072 6e00 0000 723a 0000 0072  r....rn...r:...r
-00003990: 3800 0000 7201 0000 0072 9300 0000 7294  8...r....r....r.
-000039a0: 0000 0072 9500 0000 7296 0000 0072 9700  ...r....r....r..
-000039b0: 0000 7298 0000 0054 290d 7249 0000 0072  ..r....T).rI...r
-000039c0: 0c00 0000 726f 0000 0072 4e00 0000 720e  ....ro...rN...r.
-000039d0: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
-000039e0: 0000 7212 0000 0072 1300 0000 721e 0000  ..r....r....r...
-000039f0: 0072 5700 0000 721f 0000 0029 0672 1500  .rW...r....).r..
-00003a00: 0000 7263 0000 0072 9a00 0000 727b 0000  ..rc...r....r{..
-00003a10: 0072 9c00 0000 727c 0000 0072 1600 0000  .r....r|...r....
-00003a20: 7216 0000 0072 1700 0000 5a12 5f5f 6164  r....r....Z.__ad
-00003a30: 6449 6e4d 6163 446f 776e 4461 7461 2002  dInMacDownData .
-00003a40: 0000 7364 0000 0000 010a 010c 0106 0108  ..sd............
-00003a50: 010e 0104 0102 ff02 0102 ff04 0102 ff02  ................
-00003a60: 0102 ff06 020e 0112 0102 ff06 030e 0104  ................
-00003a70: 0102 ff02 0102 ff04 0102 ff02 0102 ff06  ................
-00003a80: 020e 011a 010e 0112 0102 ff06 030e 0204  ................
-00003a90: 0102 ff02 0102 ff04 0102 ff02 0102 ff02  ................
-00003aa0: 0102 ff02 ff06 040c 010c 017a 1952 6f75  ...........z.Rou
-00003ab0: 7465 722e 5f5f 6164 6449 6e4d 6163 446f  ter.__addInMacDo
-00003ac0: 776e 4461 7461 6302 0000 0000 0000 0000  wnDatac.........
-00003ad0: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
-00003ae0: 3400 0000 6401 7d02 7c01 4400 5d12 7d03  4...d.}.|.D.].}.
-00003af0: 7c02 6402 a000 7c03 a101 3700 7d02 7108  |.d...|...7.}.q.
-00003b00: 7c02 6403 a000 7c00 6a01 7c00 6a02 a102  |.d...|.j.|.j...
-00003b10: 3700 7d02 7c02 5300 2904 4e72 0d00 0000  7.}.|.S.).Nr....
-00003b20: 7a1d 6d61 702e 6164 6441 6c6c 287b 307d  z.map.addAll({0}
-00003b30: 2e72 6f75 7465 724d 6170 2829 293b 0a7a  .routerMap());.z
-00003b40: 556d 6170 2e70 7574 4966 4162 7365 6e74  Umap.putIfAbsent
-00003b50: 2822 7b30 7d22 2c20 2829 203d 3e20 2853  ("{0}", () => (S
-00003b60: 7472 696e 6720 7061 6765 4e61 6d65 2c20  tring pageName, 
-00003b70: 4d61 7020 7061 7261 6d73 2c20 5374 7269  Map params, Stri
-00003b80: 6e67 205f 2920 3d3e 207b 317d 2870 6172  ng _) => {1}(par
-00003b90: 616d 7329 293b 2903 725a 0000 0072 2000  ams));).rZ...r .
-00003ba0: 0000 7222 0000 0072 9100 0000 7216 0000  ..r"...r....r...
-00003bb0: 0072 1600 0000 7217 0000 005a 175f 5f6d  .r....r....Z.__m
-00003bc0: 6170 4c69 7374 436f 6d62 696e 6543 7265  apListCombineCre
-00003bd0: 6174 6572 3e02 0000 730e 0000 0000 0104  ater>...s.......
-00003be0: 0108 0110 0106 0108 ff06 037a 1e52 6f75  ...........z.Rou
-00003bf0: 7465 722e 5f5f 6d61 704c 6973 7443 6f6d  ter.__mapListCom
-00003c00: 6269 6e65 4372 6561 7465 7263 0100 0000  bineCreaterc....
-00003c10: 0000 0000 0000 0000 0300 0000 0600 0000  ................
-00003c20: 4300 0000 732e 0000 0064 017d 017c 006a  C...s....d.}.|.j
-00003c30: 0044 005d 1e7d 027c 026a 0172 0a7c 0164  .D.].}.|.j.r.|.d
-00003c40: 02a0 027c 026a 037c 026a 04a1 0237 007d  ...|.j.|.j...7.}
-00003c50: 0171 0a7c 0153 0029 034e 720d 0000 007a  .q.|.S.).Nr....z
-00003c60: 0d22 7b30 7d22 3a22 7b31 7d22 2c0a 2905  ."{0}":"{1}",.).
-00003c70: 721f 0000 0072 1300 0000 725a 0000 0072  r....r....rZ...r
-00003c80: 1100 0000 720f 0000 0029 0372 1500 0000  ....r....).r....
-00003c90: 728d 0000 0072 7d00 0000 7216 0000 0072  r....r}...r....r
-00003ca0: 1600 0000 7217 0000 005a 155f 5f6d 6169  ....r....Z.__mai
-00003cb0: 6e50 6167 6544 6174 6143 7265 6174 6f72  nPageDataCreator
-00003cc0: 4702 0000 730a 0000 0000 0104 010a 0106  G...s...........
-00003cd0: 0116 017a 1c52 6f75 7465 722e 5f5f 6d61  ...z.Router.__ma
-00003ce0: 696e 5061 6765 4461 7461 4372 6561 746f  inPageDataCreato
-00003cf0: 724e 291b 7219 0000 0072 1a00 0000 721b  rN).r....r....r.
-00003d00: 0000 00da 075f 5f64 6f63 5f5f 7218 0000  .....__doc__r...
-00003d10: 0072 2800 0000 7224 0000 0072 2500 0000  .r(...r$...r%...
-00003d20: 722e 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
-00003d30: 3100 0000 7232 0000 0072 9900 0000 7207  1...r2...r....r.
-00003d40: 0000 005a 215f 526f 7574 6572 5f5f 6765  ...Z!_Router__ge
-00003d50: 7452 656d 6f74 6543 6f64 6550 6163 6b61  tRemoteCodePacka
-00003d60: 6765 5061 7468 5a21 5f52 6f75 7465 725f  gePathZ!_Router_
-00003d70: 5f67 6574 536f 7572 6365 436f 6465 5061  _getSourceCodePa
-00003d80: 636b 6167 6550 6174 6872 4500 0000 724a  ckagePathrE...rJ
-00003d90: 0000 0072 5600 0000 7203 0000 0072 5b00  ...rV...r....r[.
-00003da0: 0000 728e 0000 0072 5c00 0000 725d 0000  ..r....r\...r]..
-00003db0: 0072 7100 0000 7277 0000 0072 1600 0000  .rq...rw...r....
-00003dc0: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00003dd0: 1c00 0000 1800 0000 732c 0000 0008 0104  ........s,......
-00003de0: 0408 0e08 0b08 0608 1208 4308 3a08 7f00  ..........C.:...
-00003df0: 1f08 4108 0510 0d10 0b08 0a08 0408 0a0e  ..A.............
-00003e00: 0b08 0908 2d08 1e08 0972 1c00 0000 2917  ....-....r....).
-00003e10: da07 6861 7368 6c69 6272 0200 0000 da02  ..hashlibr......
-00003e20: 696f 7203 0000 0072 2b00 0000 7242 0000  ior....r+...rB..
-00003e30: 00da 0373 7973 da29 7464 665f 746f 6f6c  ...sys.)tdf_tool
-00003e40: 2e74 6f6f 6c73 2e63 6f6e 6669 672e 696e  .tools.config.in
-00003e50: 6974 6961 6c5f 6a73 6f6e 5f63 6f6e 6669  itial_json_confi
-00003e60: 6772 0400 0000 da28 7464 665f 746f 6f6c  gr.....(tdf_tool
-00003e70: 2e74 6f6f 6c73 2e63 6f6e 6669 672e 6d6f  .tools.config.mo
-00003e80: 6475 6c65 5f6a 736f 6e5f 636f 6e66 6967  dule_json_config
-00003e90: 7205 0000 0072 0600 0000 da25 7464 665f  r....r.....%tdf_
-00003ea0: 746f 6f6c 2e74 6f6f 6c73 2e63 6f6e 6669  tool.tools.confi
-00003eb0: 672e 7061 636b 6167 6573 5f63 6f6e 6669  g.packages_confi
-00003ec0: 6772 0700 0000 7208 0000 00da 1d74 6466  gr....r......tdf
-00003ed0: 5f74 6f6f 6c2e 746f 6f6c 732e 706c 6174  _tool.tools.plat
-00003ee0: 666f 726d 5f74 6f6f 6c73 7209 0000 00da  form_toolsr.....
-00003ef0: 1474 6466 5f74 6f6f 6c2e 746f 6f6c 732e  .tdf_tool.tools.
-00003f00: 7072 696e 7472 0a00 0000 da18 7464 665f  printr......tdf_
-00003f10: 746f 6f6c 2e74 6f6f 6c73 2e73 6865 6c6c  tool.tools.shell
-00003f20: 5f64 6972 720b 0000 0072 0c00 0000 721c  _dirr....r....r.
-00003f30: 0000 0072 1600 0000 7216 0000 0072 1600  ...r....r....r..
-00003f40: 0000 7217 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00003f50: 3e01 0000 0073 1800 0000 0c01 0c01 0801  >....s..........
-00003f60: 0801 0801 0c01 1001 1001 0c01 0c01 0c03  ................
-00003f70: 0e0a                                     ..
+00001a50: 7d7d 293b 0a20 2020 2020 2020 2020 2020  }});.           
+00001a60: 2020 2020 207d 7d2c 0a20 2020 2020 2020       }},.       
+00001a70: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+00001a80: 2020 2020 626f 6479 3a20 5369 6e67 6c65      body: Single
+00001a90: 4368 696c 6453 6372 6f6c 6c56 6965 7728  ChildScrollView(
+00001aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001ab0: 2063 6869 6c64 3a20 436f 6c75 6d6e 280a   child: Column(.
+00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ad0: 2020 2020 6368 696c 6472 656e 3a20 5f67      children: _g
+00001ae0: 6574 4275 7474 6f6e 4c69 7374 2829 2c0a  etButtonList(),.
+00001af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b00: 292c 0a20 2020 2020 2020 2020 2020 2029  ),.            )
+00001b10: 2c0a 2020 2020 2020 2020 293b 0a20 2020  ,.        );.   
+00001b20: 207d 7d0a 0a20 2020 204c 6973 743c 5769   }}..    List<Wi
+00001b30: 6467 6574 3e20 5f67 6574 4275 7474 6f6e  dget> _getButton
+00001b40: 4c69 7374 2829 207b 7b0a 2020 2020 2020  List() {{.      
+00001b50: 2020 4c69 7374 3c57 6964 6765 743e 206c    List<Widget> l
+00001b60: 6973 7420 3d20 5b5d 3b0a 2020 2020 2020  ist = [];.      
+00001b70: 2020 6c69 7374 2e61 6464 285f 726f 7574    list.add(_rout
+00001b80: 6572 4a75 6d70 5769 6467 6574 2829 293b  erJumpWidget());
+00001b90: 0a20 2020 2020 2020 206c 6973 742e 6164  .        list.ad
+00001ba0: 6428 5061 6464 696e 6728 0a20 2020 2020  d(Padding(.     
+00001bb0: 2020 2070 6164 6469 6e67 3a20 4564 6765     padding: Edge
+00001bc0: 496e 7365 7473 2e6f 6e6c 7928 746f 703a  Insets.only(top:
+00001bd0: 2032 302e 7729 2c0a 2020 2020 2020 2020   20.w),.        
+00001be0: 6368 696c 643a 2054 4446 4275 7474 6f6e  child: TDFButton
+00001bf0: 280a 2020 2020 2020 2020 2020 2020 636f  (.            co
+00001c00: 6e74 656e 743a 2022 e6a0 b9e6 8dae e8b7  ntent: "........
+00001c10: afe7 94b1 e8b7 b3e8 bdac 222c 0a20 2020  ..........",.   
+00001c20: 2020 2020 2020 2020 2062 6743 6f6c 6f72           bgColor
+00001c30: 3a20 3078 6666 3030 3838 6666 2c0a 2020  : 0xff0088ff,.  
+00001c40: 2020 2020 2020 2020 2020 636f 6e74 656e            conten
+00001c50: 7443 6f6c 6f72 3a20 3078 6666 6666 6666  tColor: 0xffffff
+00001c60: 6666 2c0a 2020 2020 2020 2020 2020 2020  ff,.            
+00001c70: 6f6e 436c 6963 6b3a 2028 2920 7b7b 0a20  onClick: () {{. 
+00001c80: 2020 2020 2020 2020 2020 2046 6f63 7573             Focus
+00001c90: 5363 6f70 652e 6f66 2863 6f6e 7465 7874  Scope.of(context
+00001ca0: 292e 7265 7175 6573 7446 6f63 7573 2846  ).requestFocus(F
+00001cb0: 6f63 7573 4e6f 6465 2829 293b 0a20 2020  ocusNode());.   
+00001cc0: 2020 2020 2020 2020 2054 4446 526f 7574           TDFRout
+00001cd0: 6572 2e6f 7065 6e28 726f 7574 6572 436f  er.open(routerCo
+00001ce0: 6e74 726f 6c6c 6572 2e74 6578 7429 3b0a  ntroller.text);.
+00001cf0: 2020 2020 2020 2020 2020 2020 7d7d 2c0a              }},.
+00001d00: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00001d10: 2020 2029 293b 0a20 2020 2020 2020 206c     ));.        l
+00001d20: 6973 742e 6164 6428 5f73 6561 7263 6857  ist.add(_searchW
+00001d30: 6964 6765 7428 2929 3b0a 0a20 2020 2020  idget());..     
+00001d40: 2020 204c 6973 743c 5769 6467 6574 3e20     List<Widget> 
+00001d50: 7772 6170 456e 7472 796c 6973 7420 3d20  wrapEntrylist = 
+00001d60: 5b5d 3b0a 2020 2020 2020 2020 7061 6765  [];.        page
+00001d70: 4d61 702e 666f 7245 6163 6828 286b 6579  Map.forEach((key
+00001d80: 2c20 7661 6c75 6529 207b 7b0a 2020 2020  , value) {{.    
+00001d90: 2020 2020 6966 2028 6b65 792e 636f 6e74      if (key.cont
+00001da0: 6169 6e73 2863 6f6e 7472 6f6c 6c65 722e  ains(controller.
+00001db0: 7465 7874 2929 207b 7b0a 2020 2020 2020  text)) {{.      
+00001dc0: 2020 2020 2020 7772 6170 456e 7472 796c        wrapEntryl
+00001dd0: 6973 742e 6164 6428 4765 7374 7572 6544  ist.add(GestureD
+00001de0: 6574 6563 746f 7228 0a20 2020 2020 2020  etector(.       
+00001df0: 2020 2020 2020 2020 206f 6e54 6170 3a20           onTap: 
+00001e00: 2829 207b 7b0a 2020 2020 2020 2020 2020  () {{.          
+00001e10: 2020 2020 2020 466f 6375 7353 636f 7065        FocusScope
+00001e20: 2e6f 6628 636f 6e74 6578 7429 2e72 6571  .of(context).req
+00001e30: 7565 7374 466f 6375 7328 466f 6375 734e  uestFocus(FocusN
+00001e40: 6f64 6528 2929 3b0a 2020 2020 2020 2020  ode());.        
+00001e50: 2020 2020 2020 2020 5444 4652 6f75 7465          TDFRoute
+00001e60: 722e 6f70 656e 2876 616c 7565 293b 0a20  r.open(value);. 
+00001e70: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00001e80: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00001e90: 2020 2063 6869 6c64 3a20 436c 6970 5252     child: ClipRR
+00001ea0: 6563 7428 0a20 2020 2020 2020 2020 2020  ect(.           
+00001eb0: 2020 2020 2062 6f72 6465 7252 6164 6975       borderRadiu
+00001ec0: 733a 2042 6f72 6465 7252 6164 6975 732e  s: BorderRadius.
+00001ed0: 616c 6c28 5261 6469 7573 2e63 6972 6375  all(Radius.circu
+00001ee0: 6c61 7228 332e 7729 292c 0a20 2020 2020  lar(3.w)),.     
+00001ef0: 2020 2020 2020 2020 2020 2063 6869 6c64             child
+00001f00: 3a20 436f 6e74 6169 6e65 7228 0a20 2020  : Container(.   
+00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f20: 2063 6f6c 6f72 3a20 436f 6c6f 7273 2e62   color: Colors.b
+00001f30: 6c75 652c 0a20 2020 2020 2020 2020 2020  lue,.           
+00001f40: 2020 2020 2020 2020 2070 6164 6469 6e67           padding
+00001f50: 3a20 4564 6765 496e 7365 7473 2e6f 6e6c  : EdgeInsets.onl
+00001f60: 7928 0a20 2020 2020 2020 2020 2020 2020  y(.             
+00001f70: 2020 2020 2020 2020 2020 206c 6566 743a             left:
+00001f80: 2037 2e77 2c20 7269 6768 743a 2037 2e77   7.w, right: 7.w
+00001f90: 2c20 746f 703a 2034 2e77 2c20 626f 7474  , top: 4.w, bott
+00001fa0: 6f6d 3a20 342e 7729 2c0a 2020 2020 2020  om: 4.w),.      
+00001fb0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+00001fc0: 696c 643a 2054 6578 7428 0a20 2020 2020  ild: Text(.     
+00001fd0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+00001fe0: 6579 2c0a 2020 2020 2020 2020 2020 2020  ey,.            
+00001ff0: 2020 2020 2020 2020 7374 796c 653a 2054          style: T
+00002000: 6578 7453 7479 6c65 2866 6f6e 7453 697a  extStyle(fontSiz
+00002010: 653a 2031 332e 7729 2c0a 2020 2020 2020  e: 13.w),.      
+00002020: 2020 2020 2020 2020 2020 2020 2020 292c                ),
+00002030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002040: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00002050: 2020 2020 2929 293b 0a20 2020 2020 2020      )));.       
+00002060: 207d 7d0a 2020 2020 2020 2020 7d7d 293b   }}.        }});
+00002070: 0a20 2020 2020 2020 206c 6973 742e 6164  .        list.ad
+00002080: 6428 5369 7a65 6442 6f78 280a 2020 2020  d(SizedBox(.    
+00002090: 2020 2020 6865 6967 6874 3a20 3230 2e77      height: 20.w
+000020a0: 2c0a 2020 2020 2020 2020 2929 3b0a 2020  ,.        ));.  
+000020b0: 2020 2020 2020 6c69 7374 2e61 6464 2857        list.add(W
+000020c0: 7261 7028 0a20 2020 2020 2020 2073 7061  rap(.        spa
+000020d0: 6369 6e67 3a20 3135 2e77 2c0a 2020 2020  cing: 15.w,.    
+000020e0: 2020 2020 7275 6e53 7061 6369 6e67 3a20      runSpacing: 
+000020f0: 3130 2e77 2c0a 2020 2020 2020 2020 6368  10.w,.        ch
+00002100: 696c 6472 656e 3a20 7772 6170 456e 7472  ildren: wrapEntr
+00002110: 796c 6973 742c 0a20 2020 2020 2020 2029  ylist,.        )
+00002120: 293b 0a20 2020 2020 2020 2072 6574 7572  );.        retur
+00002130: 6e20 6c69 7374 3b0a 2020 2020 7d7d 0a0a  n list;.    }}..
+00002140: 2020 2020 5769 6467 6574 205f 726f 7574      Widget _rout
+00002150: 6572 4a75 6d70 5769 6467 6574 2829 207b  erJumpWidget() {
+00002160: 7b0a 2020 2020 2020 2020 7265 7475 726e  {.        return
+00002170: 2054 6578 7446 6965 6c64 280a 2020 2020   TextField(.    
+00002180: 2020 2020 636f 6e74 726f 6c6c 6572 3a20      controller: 
+00002190: 726f 7574 6572 436f 6e74 726f 6c6c 6572  routerController
+000021a0: 2c0a 2020 2020 2020 2020 6175 746f 666f  ,.        autofo
+000021b0: 6375 733a 2066 616c 7365 2c0a 2020 2020  cus: false,.    
+000021c0: 2020 2020 6465 636f 7261 7469 6f6e 3a20      decoration: 
+000021d0: 496e 7075 7444 6563 6f72 6174 696f 6e28  InputDecoration(
+000021e0: 6869 6e74 5465 7874 3a20 22e8 be93 e585  hintText: ".....
+000021f0: a5e9 a1b5 e99d a2e8 b7af e794 b122 292c  ............."),
+00002200: 0a20 2020 2020 2020 206f 6e43 6861 6e67  .        onChang
+00002210: 6564 3a20 2876 616c 7565 2920 7b7b 0a20  ed: (value) {{. 
+00002220: 2020 2020 2020 2020 2020 2073 6574 5374             setSt
+00002230: 6174 6528 2829 207b 7b7d 7d29 3b0a 2020  ate(() {{}});.  
+00002240: 2020 2020 2020 2020 2020 7d7d 2c0a 2020            }},.  
+00002250: 2020 2020 2020 293b 0a20 2020 207d 7d0a        );.    }}.
+00002260: 0a20 2020 2057 6964 6765 7420 5f73 6561  .    Widget _sea
+00002270: 7263 6857 6964 6765 7428 2920 7b7b 0a20  rchWidget() {{. 
+00002280: 2020 2020 2020 2072 6574 7572 6e20 5465         return Te
+00002290: 7874 4669 656c 6428 0a20 2020 2020 2020  xtField(.       
+000022a0: 2020 2020 2063 6f6e 7472 6f6c 6c65 723a       controller:
+000022b0: 2063 6f6e 7472 6f6c 6c65 722c 0a20 2020   controller,.   
+000022c0: 2020 2020 2020 2020 2061 7574 6f66 6f63           autofoc
+000022d0: 7573 3a20 6661 6c73 652c 0a20 2020 2020  us: false,.     
+000022e0: 2020 2020 2020 2064 6563 6f72 6174 696f         decoratio
+000022f0: 6e3a 2049 6e70 7574 4465 636f 7261 7469  n: InputDecorati
+00002300: 6f6e 2868 696e 7454 6578 743a 2022 e7ad  on(hintText: "..
+00002310: 9be9 8089 2229 2c0a 2020 2020 2020 2020  ...."),.        
+00002320: 2020 2020 6f6e 4368 616e 6765 643a 2028      onChanged: (
+00002330: 7661 6c75 6529 207b 7b0a 2020 2020 2020  value) {{.      
+00002340: 2020 2020 2020 2020 2020 7365 7453 7461            setSta
+00002350: 7465 2828 2920 7b7b 7d7d 293b 0a20 2020  te(() {{}});.   
+00002360: 2020 2020 2020 2020 207d 7d2c 0a20 2020           }},.   
+00002370: 2020 2020 2029 3b0a 2020 2020 7d7d 0a20       );.    }}. 
+00002380: 2020 200a 7d7d 0a20 2020 2020 2020 2029     .}}.        )
+00002390: 1272 0700 0000 7223 0000 0072 0800 0000  .r....r#...r....
+000023a0: 7227 0000 0072 2800 0000 723c 0000 0072  r'...r(...r<...r
+000023b0: 3d00 0000 723e 0000 0072 4100 0000 7246  =...r>...rA...rF
+000023c0: 0000 0072 4700 0000 726d 0000 0072 5700  ...rG...rm...rW.
+000023d0: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+000023e0: 00da 1c5f 526f 7574 6572 5f5f 6d61 696e  ..._Router__main
+000023f0: 5061 6765 4461 7461 4372 6561 746f 7272  PageDataCreatorr
+00002400: 5b00 0000 2903 7212 0000 0072 5d00 0000  [...).r....r]...
+00002410: 5a0a 656e 7472 7950 6167 6546 7213 0000  Z.entryPageFr...
+00002420: 0072 1300 0000 7214 0000 005a 1d5f 5f67  .r....r....Z.__g
+00002430: 656e 6572 6174 655f 726f 7574 6572 5f65  enerate_router_e
+00002440: 6e74 7279 5f66 696c 6573 c800 0000 7348  ntry_files....sH
+00002450: 0000 0000 010a 0108 010a 0210 010a 020a  ................
+00002460: 0204 010e 0204 0104 ff04 0204 0104 ff04  ................
+00002470: 0204 0104 ff04 0304 0104 ff04 0304 0104  ................
+00002480: ff04 0304 0104 ff04 0304 0104 7604 0104  ............v...
+00002490: 0104 0106 0104 8602 ff04 7e7a 2452 6f75  ..........~z$Rou
+000024a0: 7465 722e 5f5f 6765 6e65 7261 7465 5f72  ter.__generate_r
+000024b0: 6f75 7465 725f 656e 7472 795f 6669 6c65  outer_entry_file
+000024c0: 7363 0100 0000 0000 0000 0000 0000 0b00  sc..............
+000024d0: 0000 0e00 0000 4300 0000 730e 0200 0074  ......C...s....t
+000024e0: 00a0 0164 01a1 0101 0074 02a0 03a1 0001  ...d.....t......
+000024f0: 0074 046a 05a0 0664 02a1 0164 036b 0272  .t.j...d...d.k.r
+00002500: 2c74 07a0 0864 02a1 0101 0074 04a0 0964  ,t...d.....t...d
+00002510: 02a1 0101 0074 04a0 0a64 02a1 0101 0074  .....t...d.....t
+00002520: 0b64 0464 0583 027d 0174 02a0 03a1 0001  .d.d...}.t......
+00002530: 0074 02a0 0ca1 007d 0274 04a0 0d7c 02a1  .t.....}.t...|..
+00002540: 0144 0090 015d 365c 037d 037d 047d 057c  .D...]6\.}.}.}.|
+00002550: 0544 0090 015d 247d 0674 046a 05a0 0e7c  .D...]$}.t.j...|
+00002560: 037c 06a1 027d 077c 07a0 0f64 06a1 0164  .|...}.|...d...d
+00002570: 076b 0372 7474 10a0 11a1 0090 0172 2a74  .k.rtt.......r*t
+00002580: 0b64 0664 0883 028f 6c7d 087c 0844 005d  .d.d....l}.|.D.]
+00002590: 567d 097c 09a0 0f74 1264 0964 0a64 0b8d  V}.|...t.d.d.d..
+000025a0: 02a1 0164 076b 0390 0172 007c 01a0 1364  ...d.k...r.|...d
+000025b0: 0ca0 147c 09a0 1574 1264 0964 0a64 0b8d  ...|...t.d.d.d..
+000025c0: 02a1 0164 0d19 00a0 1574 1264 0e64 0a64  ...d.....t.d.d.d
+000025d0: 0b8d 02a1 0164 0f19 00a1 01a1 0101 0001  .....d..........
+000025e0: 0090 0171 0871 b057 0064 0004 0004 0083  ...q.q.W.d......
+000025f0: 0301 006e 1231 0090 0173 1e30 0001 0001  ...n.1...s.0....
+00002600: 0001 0059 0001 0071 7474 0b64 0683 018f  ...Y...qtt.d....
+00002610: 567d 087c 0844 005d 407d 097c 09a0 0f64  V}.|.D.]@}.|...d
+00002620: 09a1 0164 076b 0390 0172 707c 01a0 1364  ...d.k...rp|...d
+00002630: 0ca0 147c 09a0 1564 09a1 0164 0d19 00a0  ...|...d...d....
+00002640: 1564 0ea1 0164 0f19 00a1 01a1 0101 0001  .d...d..........
+00002650: 0090 0171 7a90 0171 3857 0064 0004 0004  ...qz..q8W.d....
+00002660: 0083 0301 0071 7431 0090 0173 9030 0001  .....qt1...s.0..
+00002670: 0001 0001 0059 0001 0071 7471 647c 01a0  .....Y...qtqd|..
+00002680: 1364 10a0 1464 1164 1264 13a1 03a1 0101  .d...d.d.d......
+00002690: 007c 01a0 1364 14a1 0101 007c 006a 1644  .|...d.....|.j.D
+000026a0: 005d 347d 0a7c 01a0 1364 15a0 147c 0a6a  .]4}.|...d...|.j
+000026b0: 177c 0a6a 1864 167c 0a6a 1917 0064 177c  .|.j.d.|.j...d.|
+000026c0: 0a6a 1a17 0064 187c 0a6a 1b17 00a1 05a1  .j...d.|.j......
+000026d0: 0101 0090 0171 c27c 01a0 1364 19a1 0101  .....q.|...d....
+000026e0: 007c 01a0 1ca1 0001 0064 0053 0029 1a4e  .|.......d.S.).N
+000026f0: 7512 0000 00e7 949f e688 90e8 b7af e794  u...............
+00002700: b1e6 9687 e6a1 a375 0c00 0000 e8b7 afe7  .......u........
+00002710: 94b1 e696 87e6 a1a3 547a 0b64 6f63 756d  ........Tz.docum
+00002720: 656e 742e 6d64 7233 0000 007a 0c70 7562  ent.mdr3...z.pub
+00002730: 7370 6563 2e79 616d 6c72 6b00 0000 da02  spec.yamlrk.....
+00002740: 7262 7a06 6e61 6d65 3a20 7271 0000 0072  rbz.name: rq...r
+00002750: 7200 0000 7526 0000 0023 2320 466c 7574  r...u&...## Flut
+00002760: 7465 72e5 a3b3 e5ba 94e7 94a8 efbc 887b  ter............{
+00002770: 307d efbc 89e8 b7af e794 b1e8 a1a8 0a72  0}.............r
+00002780: 3700 0000 7235 0000 0072 0100 0000 7a68  7...r5...r....zh
+00002790: 3c74 6162 6c65 3e3c 7468 6561 643e 3c74  <table><thead><t
+000027a0: 723e 3c74 683e 7b30 7d3c 2f74 683e 3c74  r><th>{0}</th><t
+000027b0: 6820 7374 796c 6520 3d20 226d 696e 2d77  h style = "min-w
+000027c0: 6964 7468 3a31 3530 7078 2021 696d 706f  idth:150px !impo
+000027d0: 7274 616e 7422 3e7b 317d 3c2f 7468 3e3c  rtant">{1}</th><
+000027e0: 7468 3e7b 327d 3c2f 7468 3e3c 2f74 723e  th>{2}</th></tr>
+000027f0: 3c2f 7468 6561 643e 7509 0000 00e7 bb84  </thead>u.......
+00002800: e4bb b6e5 908d 7506 0000 00e6 8f8f e8bf  ......u.........
+00002810: b075 0600 0000 e8af a6e6 8385 7a07 3c74  .u..........z.<t
+00002820: 626f 6479 3e7a 3e3c 7472 3e3c 7468 3e7b  body>z><tr><th>{
+00002830: 307d 3c2f 7468 3e3c 7468 3e7b 317d 3c2f  0}</th><th>{1}</
+00002840: 7468 3e3c 7468 3e7b 327d 3c62 722f 3e7b  th><th>{2}<br/>{
+00002850: 337d 3c62 722f 3e7b 347d 3c2f 7468 3e3c  3}<br/>{4}</th><
+00002860: 2f74 723e 0a75 0900 0000 e7b1 bbe5 908d  /tr>.u..........
+00002870: 3a20 2075 0900 0000 e8b7 afe7 94b1 3a20  :  u..........: 
+00002880: 2075 0900 0000 e696 87e4 bbb6 3a20 207a   u..........:  z
+00002890: 103c 2f74 626f 6479 3e3c 2f74 6162 6c65  .</tbody></table
+000028a0: 3e29 1d72 0700 0000 7223 0000 0072 0800  >).r....r#...r..
+000028b0: 0000 7227 0000 0072 2800 0000 723d 0000  ..r'...r(...r=..
+000028c0: 0072 3e00 0000 723f 0000 0072 4000 0000  .r>...r?...r@...
+000028d0: 7241 0000 0072 3c00 0000 7246 0000 0072  rA...r<...rF...r
+000028e0: 4400 0000 724c 0000 0072 4d00 0000 726c  D...rL...rM...rl
+000028f0: 0000 0072 0600 0000 724f 0000 00da 0562  ...r....rO.....b
+00002900: 7974 6573 726d 0000 0072 5700 0000 724b  ytesrm...rW...rK
+00002910: 0000 0072 1b00 0000 720b 0000 0072 0e00  ...r....r....r..
+00002920: 0000 720f 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00002930: 0072 5b00 0000 290b 7212 0000 0072 5e00  .r[...).r....r^.
+00002940: 0000 5a06 6375 7244 6972 7261 0000 00da  ..Z.curDirra....
+00002950: 0464 6972 7372 6300 0000 7264 0000 0072  .dirsrc...rd...r
+00002960: 6500 0000 da05 6c69 6e65 73da 046c 696e  e.....lines..lin
+00002970: 65da 0469 7465 6d72 1300 0000 7213 0000  e..itemr....r...
+00002980: 0072 1400 0000 5a15 5f5f 6765 6e65 7261  .r....Z.__genera
+00002990: 7465 5f72 6f75 7465 725f 646f 6366 0100  te_router_docf..
+000029a0: 0073 8400 0000 0001 0a01 0801 1001 0a01  .s..............
+000029b0: 0a01 0a02 0a02 0802 0801 1601 0a01 0e01  ................
+000029c0: 0e01 0a01 0c01 0801 1801 0401 0401 0401  ................
+000029d0: 0201 04ff 04ff 0203 02fd 0403 0afd 0203  ................
+000029e0: 02fd 02ff 02ff 0408 2a02 0a01 0801 1001  ........*.......
+000029f0: 0401 0401 0801 02ff 0401 02ff 0201 02ff  ................
+00002a00: 02ff 02ff 0406 2e02 0401 0401 06ff 02ff  ................
+00002a10: 0405 0a02 0a01 0401 0401 0401 0401 0801  ................
+00002a20: 0801 08fb 02ff 080a 0a02 7a1c 526f 7574  ..........z.Rout
+00002a30: 6572 2e5f 5f67 656e 6572 6174 655f 726f  er.__generate_ro
+00002a40: 7574 6572 5f64 6f63 6301 0000 0000 0000  uter_docc.......
+00002a50: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00002a60: 0073 1600 0000 7400 a001 a100 0100 7402  .s....t.......t.
+00002a70: a003 6401 a101 0100 6400 5300 2902 4e7a  ..d.....d.S.).Nz
+00002a80: 1764 6172 7420 666f 726d 6174 202e 2f74  .dart format ./t
+00002a90: 7a5f 726f 7574 6572 2904 7208 0000 00da  z_router).r.....
+00002aa0: 0f67 6f49 6e53 6865 6c6c 4c69 6244 6972  .goInShellLibDir
+00002ab0: 7228 0000 00da 0673 7973 7465 6d72 1100  r(.....systemr..
+00002ac0: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00002ad0: 0072 2f00 0000 a701 0000 7304 0000 0000  .r/.......s.....
+00002ae0: 0108 017a 1152 6f75 7465 722e 5f5f 666f  ...z.Router.__fo
+00002af0: 726d 6174 5f5f 2902 7279 0000 00da 0672  rmat__).ry.....r
+00002b00: 6574 7572 6e63 0200 0000 0000 0000 0000  eturnc..........
+00002b10: 0000 0500 0000 0400 0000 4300 0000 7382  ..........C...s.
+00002b20: 0000 007c 01a0 0064 01a1 0164 0219 007d  ...|...d...d...}
+00002b30: 027c 01a0 0064 01a1 0164 0319 00a0 0164  .|...d...d.....d
+00002b40: 0464 05a1 027d 037c 02a0 0264 06a1 0164  .d...}.|...d...d
+00002b50: 076b 0372 7e74 0383 007d 047c 027c 045f  .k.r~t...}.|.|._
+00002b60: 0474 05a0 06a1 0072 5e7c 0364 0374 077c  .t.....r^|.d.t.|
+00002b70: 0383 0164 0818 0085 0219 007c 045f 086e  ...d.......|._.n
+00002b80: 167c 0364 0274 077c 0383 0164 0818 0085  .|.d.t.|...d....
+00002b90: 0219 007c 045f 0864 097c 045f 097c 0453  ...|._.d.|._.|.S
+00002ba0: 0064 0053 0029 0a4e 7a08 3a66 696c 653a  .d.S.).Nz.:file:
+00002bb0: 2f2f 7201 0000 0072 3700 0000 fa03 2532  //r....r7.....%2
+00002bc0: 35fa 0125 da03 7464 6672 6b00 0000 e905  5..%..tdfrk.....
+00002bd0: 0000 0054 290a 724b 0000 0072 5000 0000  ...T).rK...rP...
+00002be0: 726c 0000 0072 0400 0000 7245 0000 0072  rl...r....rE...r
+00002bf0: 0600 0000 724f 0000 0072 5500 0000 7243  ....rO...rU...rC
+00002c00: 0000 00da 0869 7352 656d 6f74 65a9 0572  .....isRemote..r
+00002c10: 1200 0000 7279 0000 0072 4500 0000 7243  ....ry...rE...rC
+00002c20: 0000 00da 0b70 6163 6b61 6765 4e6f 6465  .....packageNode
+00002c30: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
+00002c40: 1a5f 5f67 6574 5265 6d6f 7465 436f 6465  .__getRemoteCode
+00002c50: 5061 636b 6167 6550 6174 68ac 0100 0073  PackagePath....s
+00002c60: 1400 0000 0001 0e01 1601 0e01 0601 0601  ................
+00002c70: 0801 1802 1601 0601 7a21 526f 7574 6572  ........z!Router
+00002c80: 2e5f 5f67 6574 5265 6d6f 7465 436f 6465  .__getRemoteCode
+00002c90: 5061 636b 6167 6550 6174 6863 0200 0000  PackagePathc....
+00002ca0: 0000 0000 0000 0000 0500 0000 0400 0000  ................
+00002cb0: 4300 0000 7362 0000 007c 01a0 0064 01a1  C...sb...|...d..
+00002cc0: 0164 0219 007d 027c 01a0 0064 01a1 0164  .d...}.|...d...d
+00002cd0: 0319 00a0 0164 0464 05a1 027d 037c 02a0  .....d.d...}.|..
+00002ce0: 0264 06a1 0164 076b 0372 5e74 0383 007d  .d...d.k.r^t...}
+00002cf0: 047c 027c 045f 047c 0364 0274 057c 0383  .|.|._.|.d.t.|..
+00002d00: 0164 0818 0085 0219 007c 045f 0664 097c  .d.......|._.d.|
+00002d10: 045f 077c 0453 0064 0053 0029 0a4e fa01  ._.|.S.d.S.).N..
+00002d20: 3a72 0100 0000 7237 0000 0072 7e00 0000  :r....r7...r~...
+00002d30: 727f 0000 0072 8000 0000 726b 0000 0072  r....r....rk...r
+00002d40: 8100 0000 4629 0872 4b00 0000 7250 0000  ....F).rK...rP..
+00002d50: 0072 6c00 0000 7204 0000 0072 4500 0000  .rl...r....rE...
+00002d60: 7255 0000 0072 4300 0000 7282 0000 0072  rU...rC...r....r
+00002d70: 8300 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
+00002d80: 0000 00da 1a5f 5f67 6574 536f 7572 6365  .....__getSource
+00002d90: 436f 6465 5061 636b 6167 6550 6174 68b9  CodePackagePath.
+00002da0: 0100 0073 1000 0000 0001 0e01 1601 0e01  ...s............
+00002db0: 0601 0601 1601 0601 7a21 526f 7574 6572  ........z!Router
+00002dc0: 2e5f 5f67 6574 536f 7572 6365 436f 6465  .__getSourceCode
+00002dd0: 5061 636b 6167 6550 6174 6863 0200 0000  PackagePathc....
+00002de0: 0000 0000 0000 0000 0800 0000 0600 0000  ................
+00002df0: 4300 0000 736a 0000 0074 00a0 017c 01a1  C...sj...t...|..
+00002e00: 0101 0074 00a0 0274 03a0 04a1 00a1 01a0  ...t...t........
+00002e10: 05a1 00a0 0664 01a1 0164 0219 007d 0274  .....d...d...}.t
+00002e20: 00a0 077c 02a1 0144 005d 345c 037d 037d  ...|...D.]4\.}.}
+00002e30: 047d 057c 0544 005d 247d 0674 006a 08a0  .}.|.D.]$}.t.j..
+00002e40: 097c 037c 06a1 027d 077c 07a0 0a64 03a1  .|.|...}.|...d..
+00002e50: 0172 3e01 0001 0064 0453 0071 3e71 3064  .r>....d.S.q>q0d
+00002e60: 0553 0029 064e 7235 0000 0072 0100 0000  .S.).Nr5...r....
+00002e70: 7236 0000 0054 4629 0b72 2800 0000 723c  r6...TF).r(...r<
+00002e80: 0000 0072 4800 0000 7206 0000 0072 4900  ...rH...r....rI.
+00002e90: 0000 724a 0000 0072 4b00 0000 724c 0000  ..rJ...rK...rL..
+00002ea0: 0072 3d00 0000 724d 0000 0072 4e00 0000  .r=...rM...rN...
+00002eb0: 2908 7212 0000 005a 0764 6972 5061 7468  ).r....Z.dirPath
+00002ec0: 725f 0000 0072 6100 0000 7277 0000 0072  r_...ra...rw...r
+00002ed0: 6300 0000 7264 0000 0072 6500 0000 7213  c...rd...re...r.
+00002ee0: 0000 0072 1300 0000 7214 0000 005a 135f  ...r....r....Z._
+00002ef0: 5f68 6173 526f 7574 6572 4461 7274 4669  _hasRouterDartFi
+00002f00: 6c65 c401 0000 7310 0000 0000 010a 011c  le....s.........
+00002f10: 0114 0108 010e 010a 010c 017a 1a52 6f75  ...........z.Rou
+00002f20: 7465 722e 5f5f 6861 7352 6f75 7465 7244  ter.__hasRouterD
+00002f30: 6172 7446 696c 6563 0300 0000 0000 0000  artFilec........
+00002f40: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
+00002f50: 7314 0000 007c 01a0 0064 01a0 017c 02a1  s....|...d...|..
+00002f60: 01a1 0101 0064 0053 0029 024e 7a0b 696d  .....d.S.).Nz.im
+00002f70: 706f 7274 207b 307d 0aa9 0272 6d00 0000  port {0}...rm...
+00002f80: 7257 0000 0029 0372 1200 0000 da0b 6d46  rW...).r......mF
+00002f90: 696c 6557 7269 7465 72da 0763 6f6e 7465  ileWriter..conte
+00002fa0: 6e74 7213 0000 0072 1300 0000 7214 0000  ntr....r....r...
+00002fb0: 005a 165f 5f64 6566 6175 6c74 496d 706f  .Z.__defaultImpo
+00002fc0: 7274 4372 6561 746f 72ce 0100 0073 0200  rtCreator....s..
+00002fd0: 0000 0001 7a1d 526f 7574 6572 2e5f 5f64  ....z.Router.__d
+00002fe0: 6566 6175 6c74 496d 706f 7274 4372 6561  efaultImportCrea
+00002ff0: 746f 7263 0500 0000 0000 0000 0000 0000  torc............
+00003000: 0500 0000 0700 0000 4300 0000 7318 0000  ........C...s...
+00003010: 007c 01a0 0064 01a0 017c 027c 037c 04a1  .|...d...|.|.|..
+00003020: 03a1 0101 0064 0053 0029 024e 7a21 696d  .....d.S.).Nz!im
+00003030: 706f 7274 2022 7061 636b 6167 653a 7b30  port "package:{0
+00003040: 7d2f 7b31 7d22 2061 7320 7b32 7d3b 0a72  }/{1}" as {2};.r
+00003050: 8800 0000 2905 7212 0000 0072 8900 0000  ....).r....r....
+00003060: 7266 0000 005a 096d 4669 6c65 5061 7468  rf...Z.mFilePath
+00003070: 7269 0000 0072 1300 0000 7213 0000 0072  ri...r....r....r
+00003080: 1400 0000 5a13 5f5f 696d 706f 7274 4461  ....Z.__importDa
+00003090: 7461 4372 6561 746f 72d2 0100 0073 0a00  taCreator....s..
+000030a0: 0000 0003 0401 0401 06ff 02ff 7a1a 526f  ............z.Ro
+000030b0: 7574 6572 2e5f 5f69 6d70 6f72 7444 6174  uter.__importDat
+000030c0: 6143 7265 6174 6f72 2901 7289 0000 0063  aCreator).r....c
+000030d0: 0400 0000 0000 0000 0000 0000 0500 0000  ................
+000030e0: 0800 0000 4300 0000 7320 0000 0064 017d  ....C...s ...d.}
+000030f0: 047c 01a0 007c 04a0 017c 027c 00a0 027c  .|...|...|.|...|
+00003100: 03a1 01a1 02a1 0101 0064 0053 0029 024e  .........d.S.).N
+00003110: 7a70 0a20 2020 2072 6f75 7465 724d 6170  zp.    routerMap
+00003120: 2829 207b 7b0a 2020 2020 2020 2020 4d61  () {{.        Ma
+00003130: 703c 5374 7269 6e67 2c20 5444 4650 6167  p<String, TDFPag
+00003140: 6542 7569 6c64 6572 3e20 6d61 7020 3d20  eBuilder> map = 
+00003150: 4d61 7028 293b 0a20 2020 2020 2020 207b  Map();.        {
+00003160: 317d 0a20 2020 2020 2020 2072 6574 7572  1}.        retur
+00003170: 6e20 6d61 703b 0a20 2020 207d 7d0a 2020  n map;.    }}.  
+00003180: 2020 2903 726d 0000 0072 5700 0000 da1a    ).rm...rW.....
+00003190: 5f52 6f75 7465 725f 5f6d 6170 4164 644c  _Router__mapAddL
+000031a0: 6973 7443 7265 6174 6f72 2905 7212 0000  istCreator).r...
+000031b0: 0072 8900 0000 da0a 6d6f 6475 6c65 4e61  .r......moduleNa
+000031c0: 6d65 da04 6c69 7374 728a 0000 0072 1300  me..listr....r..
+000031d0: 0000 7213 0000 0072 1400 0000 5a19 5f5f  ..r....r....Z.__
+000031e0: 6772 6f75 7052 6f75 7465 7243 6c61 7373  groupRouterClass
+000031f0: 4372 6561 746f 72dc 0100 0073 0800 0000  Creator....s....
+00003200: 0001 0407 0801 0aff 7a20 526f 7574 6572  ........z Router
+00003210: 2e5f 5f67 726f 7570 526f 7574 6572 436c  .__groupRouterCl
+00003220: 6173 7343 7265 6174 6f72 6302 0000 0000  assCreatorc.....
+00003230: 0000 0000 0000 0004 0000 0006 0000 0043  ...............C
+00003240: 0000 0073 2200 0000 6401 7d02 7c01 4400  ...s"...d.}.|.D.
+00003250: 5d14 7d03 7c02 6402 a000 7c03 7c03 a102  ].}.|.d...|.|...
+00003260: 3700 7d02 7108 7c02 5300 2903 4e72 0a00  7.}.q.|.S.).Nr..
+00003270: 0000 7a7b 6d61 702e 7075 7449 6641 6273  ..z{map.putIfAbs
+00003280: 656e 7428 7b30 7d2e 6765 7452 6f75 7465  ent({0}.getRoute
+00003290: 7250 6174 6828 292c 2028 2920 3d3e 2020  rPath(), () =>  
+000032a0: 2853 7472 696e 6720 7061 6765 4e61 6d65  (String pageName
+000032b0: 2c20 4d61 7020 7061 7261 6d73 2c20 5374  , Map params, St
+000032c0: 7269 6e67 205f 2920 3d3e 207b 317d 2e67  ring _) => {1}.g
+000032d0: 6574 5061 6765 5769 6467 6574 2870 6172  etPageWidget(par
+000032e0: 616d 7329 293b 0a20 2020 2020 2020 2029  ams));.        )
+000032f0: 0172 5700 0000 a904 7212 0000 0072 8d00  .rW.....r....r..
+00003300: 0000 728a 0000 0072 7a00 0000 7213 0000  ..r....rz...r...
+00003310: 0072 1300 0000 7214 0000 005a 135f 5f6d  .r....r....Z.__m
+00003320: 6170 4164 644c 6973 7443 7265 6174 6f72  apAddListCreator
+00003330: e701 0000 730c 0000 0000 0104 0108 0106  ....s...........
+00003340: 0204 fe08 047a 1a52 6f75 7465 722e 5f5f  .....z.Router.__
+00003350: 6d61 7041 6464 4c69 7374 4372 6561 746f  mapAddListCreato
+00003360: 7263 0200 0000 0000 0000 0000 0000 0a00  rc..............
+00003370: 0000 0a00 0000 4300 0000 7300 0200 0074  ......C...s....t
+00003380: 0064 0164 0264 038d 027d 027c 0144 0090  .d.d.d...}.|.D..
+00003390: 015d e87d 037c 037d 0474 017c 0383 0164  .].}.|.}.t.|...d
+000033a0: 046b 0472 3664 057d 057c 037d 067c 057c  .k.r6d.}.|.}.|.|
+000033b0: 0317 007d 0474 027c 0464 0683 0290 018f  ...}.t.|.d......
+000033c0: a67d 0774 0383 007d 087c 0744 0090 015d  .}.t...}.|.D...]
+000033d0: 647d 097c 09a0 0474 0064 0764 0264 038d  d}.|...t.d.d.d..
+000033e0: 02a1 0164 086b 0372 8c7c 09a0 0574 0064  ...d.k.r.|...t.d
+000033f0: 0964 0264 038d 02a1 0164 0a19 00a0 057c  .d.d.....d.....|
+00003400: 02a1 0164 0b19 007c 085f 067c 09a0 0474  ...d...|._.|...t
+00003410: 0064 0c64 0264 038d 02a1 0164 086b 0372  .d.d.d.....d.k.r
+00003420: c47c 09a0 0574 0064 0c64 0264 038d 02a1  .|...t.d.d.d....
+00003430: 0164 0a19 00a0 057c 02a1 0164 0b19 007c  .d.....|...d...|
+00003440: 085f 077c 09a0 0474 0064 0d64 0264 038d  ._.|...t.d.d.d..
+00003450: 02a1 0164 086b 0372 fc7c 09a0 0574 0064  ...d.k.r.|...t.d
+00003460: 0d64 0264 038d 02a1 0164 0a19 00a0 057c  .d.d.....d.....|
+00003470: 02a1 0164 0b19 007c 085f 087c 09a0 0474  ...d...|._.|...t
+00003480: 0064 0e64 0264 038d 02a1 0164 086b 0390  .d.d.d.....d.k..
+00003490: 0172 3e74 097c 09a0 0574 0064 0e64 0264  .r>t.|...t.d.d.d
+000034a0: 038d 02a1 0164 0a19 00a0 057c 02a1 0164  .....d.....|...d
+000034b0: 0b19 0064 0264 038d 027c 085f 0a7c 09a0  ...d.d...|._.|..
+000034c0: 0474 0064 0f64 0264 038d 02a1 0164 086b  .t.d.d.d.....d.k
+000034d0: 0390 0172 787c 09a0 0574 0064 0f64 0264  ...rx|...t.d.d.d
+000034e0: 038d 02a1 0164 0a19 00a0 057c 02a1 0164  .....d.....|...d
+000034f0: 0b19 007c 085f 0b7c 09a0 0474 0064 1064  ...|._.|...t.d.d
+00003500: 0264 038d 02a1 0164 086b 0372 4e7c 09a0  .d.....d.k.rN|..
+00003510: 0574 0064 1064 0264 038d 02a1 0164 0a19  .t.d.d.d.....d..
+00003520: 00a0 057c 02a1 0164 0b19 0064 116b 027c  ...|...d...d.k.|
+00003530: 085f 0c71 4e7c 006a 0da0 0e7c 08a1 0101  ._.qN|.j...|....
+00003540: 007c 086a 0c64 126b 0290 0172 da7c 006a  .|.j.d.k...r.|.j
+00003550: 0fa0 0e7c 08a1 0101 0057 0064 0004 0004  ...|.....W.d....
+00003560: 0083 0301 0071 1031 0090 0173 f030 0001  .....q.1...s.0..
+00003570: 0001 0001 0059 0001 0071 1064 0053 0029  .....Y...q.d.S.)
+00003580: 134e 7235 0000 0072 7100 0000 7272 0000  .Nr5...rq...rr..
+00003590: 0069 0401 0000 7a04 5c5c 3f5c 7275 0000  .i....z.\\?\ru..
+000035a0: 007a 0e20 2f2f 2370 6163 6b61 6765 232f  .z. //#package#/
+000035b0: 2f72 6b00 0000 fa0d 2f2f 2370 6163 6b61  /rk.....//#packa
+000035c0: 6765 232f 2f72 3700 0000 7201 0000 00fa  ge#//r7...r.....
+000035d0: 102f 2f23 726f 7574 6572 5061 7468 232f  .//#routerPath#/
+000035e0: 2ffa 0e2f 2f23 6669 6c65 5061 7468 232f  /..//#filePath#/
+000035f0: 2ffa 0a2f 2f23 6e6f 7465 232f 2ffa 102f  /..//#note#//../
+00003600: 2f23 7061 6765 5769 6467 6574 232f 2ffa  /#pageWidget#//.
+00003610: 102f 2f23 6973 4d61 696e 5061 6765 232f  .//#isMainPage#/
+00003620: 2fda 0474 7275 6554 2910 7276 0000 0072  /..trueT).rv...r
+00003630: 5500 0000 7246 0000 0072 0900 0000 726c  U...rF...r....rl
+00003640: 0000 0072 4b00 0000 720b 0000 0072 0c00  ...rK...r....r..
+00003650: 0000 720d 0000 00da 0373 7472 720e 0000  ..r......strr...
+00003660: 0072 0f00 0000 7210 0000 0072 1b00 0000  .r....r....r....
+00003670: 7254 0000 0072 1c00 0000 290a 7212 0000  rT...r....).r...
+00003680: 0072 6000 0000 5a09 6279 7465 7354 656d  .r`...Z.bytesTem
+00003690: 70da 0866 696c 6549 7465 6dda 0672 6573  p..fileItem..res
+000036a0: 756c 7472 6700 0000 5a05 7465 6d70 3272  ultrg...Z.temp2r
+000036b0: 7800 0000 da04 6e6f 6465 7279 0000 0072  x.....nodery...r
+000036c0: 1300 0000 7213 0000 0072 1400 0000 5a15  ....r....r....Z.
+000036d0: 5f5f 6164 6449 6e57 696e 646f 7744 6f77  __addInWindowDow
+000036e0: 6e44 6174 61f0 0100 0073 9200 0000 0001  nData....s......
+000036f0: 0c01 0a01 0401 0c01 0401 0401 0801 0e01  ................
+00003700: 0601 0a01 1601 0401 0aff 0202 02fe 0402  ................
+00003710: 02fe 0202 02fe 0603 1601 0401 0aff 0202  ................
+00003720: 02fe 0402 02fe 0202 02fe 0603 1601 0401  ................
+00003730: 0aff 0202 02fe 0402 02fe 0202 02fe 0603  ................
+00003740: 1801 0201 1601 02ff 0202 02fe 0203 02fc  ................
+00003750: 0806 1801 0401 0aff 0202 02fe 0402 02fe  ................
+00003760: 0202 02fe 0603 1602 1001 02ff 0402 02fe  ................
+00003770: 0202 02fe 0203 02fd 02ff 0606 0c01 0c01  ................
+00003780: 7a1c 526f 7574 6572 2e5f 5f61 6464 496e  z.Router.__addIn
+00003790: 5769 6e64 6f77 446f 776e 4461 7461 6302  WindowDownDatac.
+000037a0: 0000 0000 0000 0000 0000 0006 0000 0009  ................
+000037b0: 0000 0043 0000 0073 6401 0000 7c01 4400  ...C...sd...|.D.
+000037c0: 9001 5d58 7d02 7400 7c02 8301 9001 8f38  ..]X}.t.|......8
+000037d0: 7d03 7401 8300 7d04 7c03 4400 5df8 7d05  }.t...}.|.D.].}.
+000037e0: 7c05 a002 6401 a101 6402 6b03 724c 7c05  |...d...d.k.rL|.
+000037f0: a003 6401 a101 6403 1900 a003 6404 a101  ..d...d.....d...
+00003800: 6405 1900 7c04 5f04 7c05 a002 6406 a101  d...|._.|...d...
+00003810: 6402 6b03 7274 7c05 a003 6406 a101 6403  d.k.rt|...d...d.
+00003820: 1900 a003 6404 a101 6405 1900 7c04 5f05  ....d...d...|._.
+00003830: 7c05 a002 6407 a101 6402 6b03 729c 7c05  |...d...d.k.r.|.
+00003840: a003 6407 a101 6403 1900 a003 6404 a101  ..d...d.....d...
+00003850: 6405 1900 7c04 5f06 7c05 a002 6408 a101  d...|._.|...d...
+00003860: 6402 6b03 72c4 7c05 a003 6408 a101 6403  d.k.r.|...d...d.
+00003870: 1900 a003 6404 a101 6405 1900 7c04 5f07  ....d...d...|._.
+00003880: 7c05 a002 6409 a101 6402 6b03 72ec 7c05  |...d...d.k.r.|.
+00003890: a003 6409 a101 6403 1900 a003 6404 a101  ..d...d.....d...
+000038a0: 6405 1900 7c04 5f08 7c05 a002 640a a101  d...|._.|...d...
+000038b0: 6402 6b03 7220 7c05 a003 640a a101 6403  d.k.r |...d...d.
+000038c0: 1900 a003 6404 a101 6405 1900 640b 6b02  ....d...d...d.k.
+000038d0: 7c04 5f09 7120 7c00 6a0a a00b 7c04 a101  |._.q |.j...|...
+000038e0: 0100 7c04 6a09 640c 6b02 9001 723e 7c00  ..|.j.d.k...r>|.
+000038f0: 6a0c a00b 7c04 a101 0100 5700 6400 0400  j...|.....W.d...
+00003900: 0400 8303 0100 7104 3100 9001 7354 3000  ......q.1...sT0.
+00003910: 0100 0100 0100 5900 0100 7104 6400 5300  ......Y...q.d.S.
+00003920: 290d 4e72 8f00 0000 726b 0000 0072 3700  ).Nr....rk...r7.
+00003930: 0000 7235 0000 0072 0100 0000 7290 0000  ..r5...r....r...
+00003940: 0072 9100 0000 7292 0000 0072 9300 0000  .r....r....r....
+00003950: 7294 0000 0072 9500 0000 5429 0d72 4600  r....r....T).rF.
+00003960: 0000 7209 0000 0072 6c00 0000 724b 0000  ..r....rl...rK..
+00003970: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00003980: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00003990: 1b00 0000 7254 0000 0072 1c00 0000 2906  ....rT...r....).
+000039a0: 7212 0000 0072 6000 0000 7297 0000 0072  r....r`...r....r
+000039b0: 7800 0000 7299 0000 0072 7900 0000 7213  x...r....ry...r.
+000039c0: 0000 0072 1300 0000 7214 0000 005a 125f  ...r....r....Z._
+000039d0: 5f61 6464 496e 4d61 6344 6f77 6e44 6174  _addInMacDownDat
+000039e0: 611d 0200 0073 6400 0000 0001 0a01 0c01  a....sd.........
+000039f0: 0601 0801 0e01 0401 02ff 0201 02ff 0401  ................
+00003a00: 02ff 0201 02ff 0602 0e01 1201 02ff 0603  ................
+00003a10: 0e01 0401 02ff 0201 02ff 0401 02ff 0201  ................
+00003a20: 02ff 0602 0e01 1a01 0e01 1201 02ff 0603  ................
+00003a30: 0e02 0401 02ff 0201 02ff 0401 02ff 0201  ................
+00003a40: 02ff 0201 02ff 02ff 0604 0c01 0c01 7a19  ..............z.
+00003a50: 526f 7574 6572 2e5f 5f61 6464 496e 4d61  Router.__addInMa
+00003a60: 6344 6f77 6e44 6174 6163 0200 0000 0000  cDownDatac......
+00003a70: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
+00003a80: 0000 7334 0000 0064 017d 027c 0144 005d  ..s4...d.}.|.D.]
+00003a90: 127d 037c 0264 02a0 007c 03a1 0137 007d  .}.|.d...|...7.}
+00003aa0: 0271 087c 0264 03a0 007c 006a 017c 006a  .q.|.d...|.j.|.j
+00003ab0: 02a1 0237 007d 027c 0253 0029 044e 720a  ...7.}.|.S.).Nr.
+00003ac0: 0000 007a 1d6d 6170 2e61 6464 416c 6c28  ...z.map.addAll(
+00003ad0: 7b30 7d2e 726f 7574 6572 4d61 7028 2929  {0}.routerMap())
+00003ae0: 3b0a 7a55 6d61 702e 7075 7449 6641 6273  ;.zUmap.putIfAbs
+00003af0: 656e 7428 227b 307d 222c 2028 2920 3d3e  ent("{0}", () =>
+00003b00: 2028 5374 7269 6e67 2070 6167 654e 616d   (String pageNam
+00003b10: 652c 204d 6170 2070 6172 616d 732c 2053  e, Map params, S
+00003b20: 7472 696e 6720 5f29 203d 3e20 7b31 7d28  tring _) => {1}(
+00003b30: 7061 7261 6d73 2929 3b29 0372 5700 0000  params));).rW...
+00003b40: 721d 0000 0072 1f00 0000 728e 0000 0072  r....r....r....r
+00003b50: 1300 0000 7213 0000 0072 1400 0000 5a17  ....r....r....Z.
+00003b60: 5f5f 6d61 704c 6973 7443 6f6d 6269 6e65  __mapListCombine
+00003b70: 4372 6561 7465 723b 0200 0073 0e00 0000  Creater;...s....
+00003b80: 0001 0401 0801 1001 0601 08ff 0603 7a1e  ..............z.
+00003b90: 526f 7574 6572 2e5f 5f6d 6170 4c69 7374  Router.__mapList
+00003ba0: 436f 6d62 696e 6543 7265 6174 6572 6301  CombineCreaterc.
+00003bb0: 0000 0000 0000 0000 0000 0003 0000 0006  ................
+00003bc0: 0000 0043 0000 0073 2e00 0000 6401 7d01  ...C...s....d.}.
+00003bd0: 7c00 6a00 4400 5d1e 7d02 7c02 6a01 720a  |.j.D.].}.|.j.r.
+00003be0: 7c01 6402 a002 7c02 6a03 7c02 6a04 a102  |.d...|.j.|.j...
+00003bf0: 3700 7d01 710a 7c01 5300 2903 4e72 0a00  7.}.q.|.S.).Nr..
+00003c00: 0000 7a0d 227b 307d 223a 227b 317d 222c  ..z."{0}":"{1}",
+00003c10: 0a29 0572 1c00 0000 7210 0000 0072 5700  .).r....r....rW.
+00003c20: 0000 720e 0000 0072 0c00 0000 2903 7212  ..r....r....).r.
+00003c30: 0000 0072 8a00 0000 727a 0000 0072 1300  ...r....rz...r..
+00003c40: 0000 7213 0000 0072 1400 0000 5a15 5f5f  ..r....r....Z.__
+00003c50: 6d61 696e 5061 6765 4461 7461 4372 6561  mainPageDataCrea
+00003c60: 746f 7244 0200 0073 0a00 0000 0001 0401  torD...s........
+00003c70: 0a01 0601 1601 7a1c 526f 7574 6572 2e5f  ......z.Router._
+00003c80: 5f6d 6169 6e50 6167 6544 6174 6143 7265  _mainPageDataCre
+00003c90: 6174 6f72 4e29 1b72 1600 0000 7217 0000  atorN).r....r...
+00003ca0: 0072 1800 0000 da07 5f5f 646f 635f 5f72  .r......__doc__r
+00003cb0: 1500 0000 7225 0000 0072 2100 0000 7222  ....r%...r!...r"
+00003cc0: 0000 0072 2b00 0000 722c 0000 0072 2d00  ...r+...r,...r-.
+00003cd0: 0000 722e 0000 0072 2f00 0000 7296 0000  ..r....r/...r...
+00003ce0: 0072 0400 0000 5a21 5f52 6f75 7465 725f  .r....Z!_Router_
+00003cf0: 5f67 6574 5265 6d6f 7465 436f 6465 5061  _getRemoteCodePa
+00003d00: 636b 6167 6550 6174 685a 215f 526f 7574  ckagePathZ!_Rout
+00003d10: 6572 5f5f 6765 7453 6f75 7263 6543 6f64  er__getSourceCod
+00003d20: 6550 6163 6b61 6765 5061 7468 7242 0000  ePackagePathrB..
+00003d30: 0072 4700 0000 7253 0000 0072 0300 0000  .rG...rS...r....
+00003d40: 7258 0000 0072 8b00 0000 7259 0000 0072  rX...r....rY...r
+00003d50: 5a00 0000 726e 0000 0072 7400 0000 7213  Z...rn...rt...r.
+00003d60: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
+00003d70: 0000 7219 0000 0015 0000 0073 2c00 0000  ..r........s,...
+00003d80: 0801 0404 080e 080b 0806 0812 0843 083a  .............C.:
+00003d90: 087f 001f 0841 0805 100d 100b 080a 0804  .....A..........
+00003da0: 080a 0e0b 0809 082d 081e 0809 7219 0000  .......-....r...
+00003db0: 0029 11da 0768 6173 686c 6962 7202 0000  .)...hashlibr...
+00003dc0: 00da 0269 6f72 0300 0000 7228 0000 0072  ...ior....r(...r
+00003dd0: 3f00 0000 da25 7464 665f 746f 6f6c 2e74  ?....%tdf_tool.t
+00003de0: 6f6f 6c73 2e63 6f6e 6669 672e 7061 636b  ools.config.pack
+00003df0: 6167 6573 5f63 6f6e 6669 6772 0400 0000  ages_configr....
+00003e00: 7205 0000 00da 1d74 6466 5f74 6f6f 6c2e  r......tdf_tool.
+00003e10: 746f 6f6c 732e 706c 6174 666f 726d 5f74  tools.platform_t
+00003e20: 6f6f 6c73 7206 0000 00da 1474 6466 5f74  oolsr......tdf_t
+00003e30: 6f6f 6c2e 746f 6f6c 732e 7072 696e 7472  ool.tools.printr
+00003e40: 0700 0000 da18 7464 665f 746f 6f6c 2e74  ......tdf_tool.t
+00003e50: 6f6f 6c73 2e73 6865 6c6c 5f64 6972 7208  ools.shell_dirr.
+00003e60: 0000 0072 0900 0000 7219 0000 0072 1300  ...r....r....r..
+00003e70: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00003e80: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00003e90: 1200 0000 0c01 0c01 0801 0801 1001 0c01  ................
+00003ea0: 0c01 0c03 0e0a                           ......
```

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 18 09:16:44 2024 UTC, .py size: 1656 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 fce4 2066 7806 0000  a......... fx...
+00000000: 610d 0d0a 0000 0000 04e9 2066 7806 0000  a......... fx...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 8302 5a09  ..G.d.d...d...Z.
 00000070: 6407 5300 2908 e900 0000 0029 02da 0b50  d.S.)......)...P
```

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/annotation.py` & `tdf_tool-2.4.7/tdf_tool/pipelines/annotation.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/api_interaction.py` & `tdf_tool-2.4.7/tdf_tool/pipelines/api_interaction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,51 @@
+from hashlib import md5
 import os
 import shutil
 from tdf_tool.tools.config.packages_config import PackageNode, PackagesJsonConfig
 from tdf_tool.tools.platform_tools import PlatformTools
 from tdf_tool.tools.print import Print
 from tdf_tool.tools.shell_dir import ShellDir
+from tdf_tool.tools.generator import DefaultGenerator
 
 
 class ImplNode:
     def __init__(self):
         self.packageName = ""
         self.packagePath = ""
         self.filePath = ""
 
+    def impl_md5(self) -> str:
+        return "api_" + md5(self.filePath.encode()).hexdigest()[8:-8]
+
     def print(self):
         Print.yellow("package:" + self.packageName + "/" + self.filePath)
 
 
 class ApiNode:
     def __init__(self):
         self.packageName = ""
         self.packagePath = ""
         self.filePath = ""
 
+    def api_md5(self) -> str:
+        return "api_" + md5(self.filePath.encode()).hexdigest()[8:-8]
+
     def print(self):
         Print.yellow("package:" + self.packageName + "/" + self.filePath)
 
 
 class ApiAnnotation:
     """
     模块间交互支持相关命令：tl api -h 查看详情
     """
 
     def __init__(self):
         self.ff = None
+        self.__generator: str = "ApiAnnotationGenerator"  # 生成器名
         self.__implSuffix: str = ".tdf_impl.dart"  # 交互描述文件后缀
         self.__implNodeList: list[ImplNode] = []  # impl描述文件列表
         self.__apiSuffix: str = ".tdf_api.dart"  # 交互api描述文件后缀
         self.__apiNodeList: list[ApiNode] = []  # api描述文件列表
         self.__interactionDir: str = "tdf_api"  # 交互文件目录
         self.__annotationName: str = "tdf_module_api_anno"  # 注解库名
         self.__packagesList: list[PackageNode] = []  # 壳依赖的所有库
@@ -67,23 +76,25 @@
 
         self.ff.close()
 
         # 全部生成文件format
         self.__format__()
 
     def __generate_register_code(self):
+        self.ff.write(DefaultGenerator.defaultTitleDesc(self.__generator))
+
         for _item in self.__implNodeList:
-            self.____import_data_creator(self.ff, _item.packageName, _item.filePath, _item.packageName)
+            self.____import_data_creator(self.ff, _item.packageName, _item.filePath, _item.impl_md5())
         for _item in self.__apiNodeList:
-            self.____import_data_creator(self.ff, _item.packageName, _item.filePath, _item.packageName)
+            self.____import_data_creator(self.ff, _item.packageName, _item.filePath, _item.api_md5())
 
-        self.__import_data_creator_without_alias(self.ff, "tdf_module_api_anno", "tdf_module_api_anno.dart")
+        self.__import_data_creator_without_alias(self.ff, self.__annotationName, self.__annotationName + ".dart")
 
         content = """
-
+        
         class TDFApiImplAutoRegister {{
           static List<Type> apis = [
             {0}
           ];
           // 确保所有被引用的api库的实现类都已注册
           static void _ensureApiImplRegister() {{
             apis.forEach((element) {{
@@ -95,32 +106,33 @@
 
           static void autoRegister() {{
               {1}
               _ensureApiImplRegister();
           }}
         }}
             """
-        self.ff.write(content.format(
-            self.api_list_creator(),
-            self.__register_list_creator()))
+        self.ff.write(
+            content.format(
+                self.api_list_creator(),
+                self.__register_list_creator()))
 
     def __register_list_creator(self):
         content = ""
         for item in self.__implNodeList:
             content += """
             ApiRegisterCenter.register({0}.AutoRegister.apiType,{1}.AutoRegister.provider);
-            """.format(item.packageName, item.packageName)
+            """.format(item.impl_md5(), item.impl_md5())
         return content
 
     def api_list_creator(self):
         content = ""
         for item in self.__apiNodeList:
             content += """
             {0}.TDFApiAutoInvalidate.apiType,
-                    """.format(item.packageName)
+                    """.format(item.api_md5())
         return content
 
     def __integrate_tdf_impl_files(self):
         Print.title("整合所有交互impl文件")
         for packageItem in self.__packagesList:
             __file_path = self.__get_target_file(packageItem.packagePath, self.__implSuffix)
             if __file_path is not None:
```

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/fix_header.py` & `tdf_tool-2.4.7/tdf_tool/pipelines/fix_header.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/git.py` & `tdf_tool-2.4.7/tdf_tool/pipelines/git.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/module.py` & `tdf_tool-2.4.7/tdf_tool/pipelines/module.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/package.py` & `tdf_tool-2.4.7/tdf_tool/pipelines/package.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/router.py` & `tdf_tool-2.4.7/tdf_tool/pipelines/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from hashlib import md5
 from io import TextIOWrapper
 import os
 import shutil
-import sys
-from tdf_tool.tools.config.initial_json_config import InitialJsonConfig
-from tdf_tool.tools.config.module_json_config import ModuleItemType, ModuleJsonConfig
 from tdf_tool.tools.config.packages_config import PackageNode, PackagesJsonConfig
 from tdf_tool.tools.platform_tools import PlatformTools
 from tdf_tool.tools.print import Print
 from tdf_tool.tools.shell_dir import ShellDir
 
 
 class RouterNode:
```

### Comparing `tdf_tool-2.4.6/tdf_tool/pipelines/translate.py` & `tdf_tool-2.4.7/tdf_tool/pipelines/translate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/__pycache__/env.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/env.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/__pycache__/env.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/env.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Apr 16 07:59:17 2024 UTC, .py size: 662 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,70 @@
-00000000: 610d 0d0a 0000 0000 d52f 1e66 9602 0000  a......../.f....
+00000000: 610d 0d0a 0000 0000 863d 2266 0803 0000  a........="f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
+00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
-00000050: 8302 5a04 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
-00000060: 01da 0345 6e76 2901 da05 5072 696e 7463  ...Env)...Printc
-00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: 0300 0000 4000 0000 7328 0000 0065 005a  ....@...s(...e.Z
-00000090: 0164 005a 0265 0364 019c 0164 0264 0384  .d.Z.e.d...d.d..
-000000a0: 045a 0465 0564 019c 0164 0464 0584 045a  .Z.e.d...d.d...Z
-000000b0: 0664 0653 0029 07da 0745 6e76 546f 6f6c  .d.S.)...EnvTool
-000000c0: 2901 da06 7265 7475 726e 6300 0000 0000  )...returnc.....
-000000d0: 0000 0000 0000 0002 0000 0006 0000 0043  ...............C
-000000e0: 0000 0073 3200 0000 7a1e 7400 8300 7d00  ...s2...z.t...}.
-000000f0: 7c00 a001 a100 0100 7c00 a002 6401 a101  |.......|...d...
-00000100: 7d01 7c01 5700 5300 0100 0100 0100 5900  }.|.W.S.......Y.
-00000110: 6402 5300 3000 6400 5300 2903 4e5a 0e54  d.S.0.d.S.).NZ.T
-00000120: 4446 544f 4f4c 535f 4445 4255 4746 2903  DFTOOLS_DEBUGF).
-00000130: 7202 0000 00da 0872 6561 645f 656e 76da  r......read_env.
-00000140: 0462 6f6f 6c29 02da 0365 6e76 da06 5f64  .bool)...env.._d
-00000150: 6562 7567 a900 720a 0000 00f5 5e00 0000  ebug..r.....^...
-00000160: 2f55 7365 7273 2f78 756a 6961 6e2f 446f  /Users/xujian/Do
-00000170: 6375 6d65 6e74 732f 3230 3234 2fe6 a8a1  cuments/2024/...
-00000180: e59d 97e9 97b4 e4ba a4e4 ba92 e9a1 b9e7  ................
-00000190: 9bae 746c e58d 87e7 baa7 2f70 6163 6b61  ..tl....../packa
-000001a0: 6765 5f74 6f6f 6c73 2f74 6466 5f74 6f6f  ge_tools/tdf_too
-000001b0: 6c2f 746f 6f6c 732f 656e 762e 7079 da08  l/tools/env.py..
-000001c0: 6973 5f64 6562 7567 0b00 0000 730e 0000  is_debug....s...
-000001d0: 0000 0102 0106 0108 010a 0106 0106 017a  ...............z
-000001e0: 1045 6e76 546f 6f6c 2e69 735f 6465 6275  .EnvTool.is_debu
-000001f0: 6763 0000 0000 0000 0000 0000 0000 0200  gc..............
-00000200: 0000 0600 0000 4300 0000 7332 0000 007a  ......C...s2...z
-00000210: 1e74 0083 007d 007c 00a0 01a1 0001 007c  .t...}.|.......|
-00000220: 00a0 0264 01a1 017d 017c 0157 0053 0001  ...d...}.|.W.S..
-00000230: 0001 0001 0059 0064 0053 0030 0064 0053  .....Y.d.S.0.d.S
-00000240: 0029 024e 5a12 5444 4654 4f4f 4c53 5f57  .).NZ.TDFTOOLS_W
-00000250: 4f52 4b53 5041 4345 2903 7202 0000 0072  ORKSPACE).r....r
-00000260: 0600 0000 da03 7374 7229 0272 0800 0000  ......str).r....
-00000270: da0a 5f77 6f72 6b73 7061 6365 720a 0000  .._workspacer...
-00000280: 0072 0a00 0000 720b 0000 00da 0977 6f72  .r....r......wor
-00000290: 6b73 7061 6365 1400 0000 730e 0000 0000  kspace....s.....
-000002a0: 0102 0106 0108 010a 0106 0106 017a 1145  .............z.E
-000002b0: 6e76 546f 6f6c 2e77 6f72 6b73 7061 6365  nvTool.workspace
-000002c0: 4e29 07da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-000002d0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-000002e0: 6c6e 616d 655f 5f72 0700 0000 720c 0000  lname__r....r...
-000002f0: 0072 0d00 0000 720f 0000 0072 0a00 0000  .r....r....r....
-00000300: 720a 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-00000310: 0400 0000 0a00 0000 7304 0000 0008 010e  ........s.......
-00000320: 0972 0400 0000 4e29 055a 0865 6e76 6972  .r....N).Z.envir
-00000330: 6f6e 7372 0200 0000 da14 7464 665f 746f  onsr......tdf_to
-00000340: 6f6c 2e74 6f6f 6c73 2e70 7269 6e74 7203  ol.tools.printr.
-00000350: 0000 0072 0400 0000 720a 0000 0072 0a00  ...r....r....r..
-00000360: 0000 720a 0000 0072 0b00 0000 da08 3c6d  ..r....r......<m
-00000370: 6f64 756c 653e 0100 0000 7304 0000 000c  odule>....s.....
-00000380: 020c 07                                  ...
+00000040: 5a03 6400 6403 6c04 6d05 5a05 0100 4700  Z.d.d.l.m.Z...G.
+00000050: 6404 6405 8400 6405 8302 5a06 6402 5300  d.d...d...Z.d.S.
+00000060: 2906 e900 0000 0029 01da 0345 6e76 4e29  )......)...EnvN)
+00000070: 01da 0550 7269 6e74 6300 0000 0000 0000  ...Printc.......
+00000080: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000090: 0073 3600 0000 6500 5a01 6400 5a02 6503  .s6...e.Z.d.Z.e.
+000000a0: 6401 9c01 6402 6403 8404 5a04 6505 6401  d...d.d...Z.e.d.
+000000b0: 9c01 6404 6405 8404 5a06 6505 6401 9c01  ..d.d...Z.e.d...
+000000c0: 6406 6407 8404 5a07 6408 5300 2909 da07  d.d...Z.d.S.)...
+000000d0: 456e 7654 6f6f 6c29 01da 0672 6574 7572  EnvTool)...retur
+000000e0: 6e63 0000 0000 0000 0000 0000 0000 0200  nc..............
+000000f0: 0000 0600 0000 4300 0000 7332 0000 007a  ......C...s2...z
+00000100: 1e74 0083 007d 007c 00a0 01a1 0001 007c  .t...}.|.......|
+00000110: 00a0 0264 01a1 017d 017c 0157 0053 0001  ...d...}.|.W.S..
+00000120: 0001 0001 0059 0064 0253 0030 0064 0053  .....Y.d.S.0.d.S
+00000130: 0029 034e 5a0e 5444 4654 4f4f 4c53 5f44  .).NZ.TDFTOOLS_D
+00000140: 4542 5547 4629 0372 0200 0000 da08 7265  EBUGF).r......re
+00000150: 6164 5f65 6e76 da04 626f 6f6c 2902 da03  ad_env..bool)...
+00000160: 656e 76da 065f 6465 6275 67a9 0072 0a00  env.._debug..r..
+00000170: 0000 f55e 0000 002f 5573 6572 732f 7875  ...^.../Users/xu
+00000180: 6a69 616e 2f44 6f63 756d 656e 7473 2f32  jian/Documents/2
+00000190: 3032 342f e6a8 a1e5 9d97 e997 b4e4 baa4  024/............
+000001a0: e4ba 92e9 a1b9 e79b ae74 6ce5 8d87 e7ba  .........tl.....
+000001b0: a72f 7061 636b 6167 655f 746f 6f6c 732f  ./package_tools/
+000001c0: 7464 665f 746f 6f6c 2f74 6f6f 6c73 2f65  tdf_tool/tools/e
+000001d0: 6e76 2e70 79da 0869 735f 6465 6275 670c  nv.py..is_debug.
+000001e0: 0000 0073 0e00 0000 0001 0201 0601 0801  ...s............
+000001f0: 0a01 0601 0601 7a10 456e 7654 6f6f 6c2e  ......z.EnvTool.
+00000200: 6973 5f64 6562 7567 6300 0000 0000 0000  is_debugc.......
+00000210: 0000 0000 0002 0000 0006 0000 0043 0000  .............C..
+00000220: 0073 3200 0000 7a1e 7400 8300 7d00 7c00  .s2...z.t...}.|.
+00000230: a001 a100 0100 7c00 a002 6401 a101 7d01  ......|...d...}.
+00000240: 7c01 5700 5300 0100 0100 0100 5900 6400  |.W.S.......Y.d.
+00000250: 5300 3000 6400 5300 2902 4e5a 1254 4446  S.0.d.S.).NZ.TDF
+00000260: 544f 4f4c 535f 574f 524b 5350 4143 4529  TOOLS_WORKSPACE)
+00000270: 0372 0200 0000 7206 0000 00da 0373 7472  .r....r......str
+00000280: 2902 7208 0000 00da 0a5f 776f 726b 7370  ).r......_worksp
+00000290: 6163 6572 0a00 0000 720a 0000 0072 0b00  acer....r....r..
+000002a0: 0000 da09 776f 726b 7370 6163 6515 0000  ....workspace...
+000002b0: 0073 0e00 0000 0001 0201 0601 0801 0a01  .s..............
+000002c0: 0601 0601 7a11 456e 7654 6f6f 6c2e 776f  ....z.EnvTool.wo
+000002d0: 726b 7370 6163 6563 0000 0000 0000 0000  rkspacec........
+000002e0: 0000 0000 0000 0000 0300 0000 4300 0000  ............C...
+000002f0: 730c 0000 0074 006a 01a0 0264 01a1 0153  s....t.j...d...S
+00000300: 0029 024e 7a08 7464 662d 746f 6f6c 2903  .).Nz.tdf-tool).
+00000310: da09 696d 706f 7274 6c69 62da 086d 6574  ..importlib..met
+00000320: 6164 6174 61da 0776 6572 7369 6f6e 720a  adata..versionr.
+00000330: 0000 0072 0a00 0000 720a 0000 0072 0b00  ...r....r....r..
+00000340: 0000 da0e 7464 6654 6f6f 6c56 6572 7369  ....tdfToolVersi
+00000350: 6f6e 1e00 0000 7302 0000 0000 017a 1645  on....s......z.E
+00000360: 6e76 546f 6f6c 2e74 6466 546f 6f6c 5665  nvTool.tdfToolVe
+00000370: 7273 696f 6e4e 2908 da08 5f5f 6e61 6d65  rsionN)...__name
+00000380: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000390: 5f5f 7175 616c 6e61 6d65 5f5f 7207 0000  __qualname__r...
+000003a0: 0072 0c00 0000 720d 0000 0072 0f00 0000  .r....r....r....
+000003b0: 7213 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
+000003c0: 0a00 0000 720b 0000 0072 0400 0000 0b00  ....r....r......
+000003d0: 0000 7306 0000 0008 010e 090e 0972 0400  ..s..........r..
+000003e0: 0000 2907 5a08 656e 7669 726f 6e73 7202  ..).Z.environsr.
+000003f0: 0000 00da 1269 6d70 6f72 746c 6962 2e6d  .....importlib.m
+00000400: 6574 6164 6174 6172 1000 0000 da14 7464  etadatar......td
+00000410: 665f 746f 6f6c 2e74 6f6f 6c73 2e70 7269  f_tool.tools.pri
+00000420: 6e74 7203 0000 0072 0400 0000 720a 0000  ntr....r....r...
+00000430: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000440: da08 3c6d 6f64 756c 653e 0100 0000 7306  ..<module>....s.
+00000450: 0000 000c 0108 020c 07                   .........
```

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/__pycache__/print.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/print.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/__pycache__/print.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/print.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Apr 16 07:59:17 2024 UTC, .py size: 1226 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d52f 1e66 ca04 0000  a......../.f....
+00000000: 610d 0d0a 0000 0000 b13c 2266 ca04 0000  a........<"f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 8302 5a01 6401 5300 2904 e900 0000 004e  ..Z.d.S.)......N
 00000050: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000060: 0004 0000 0040 0000 0073 8600 0000 6500  .....@...s....e.
 00000070: 5a01 6400 5a02 6401 6402 8400 5a03 6504  Z.d.Z.d.d...Z.e.
```

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 17 07:17:09 2024 UTC, .py size: 5718 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7577 1f66 5616 0000  a.......uw.fV...
+00000000: 610d 0d0a 0000 0000 04e9 2066 5616 0000  a......... fV...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6407 6408 8400 6408 6501 8303  ..G.d.d...d.e...
```

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/cli/bean/deps_item.py` & `tdf_tool-2.4.7/tdf_tool/tools/cli/bean/deps_item.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/cli/module_deps_rewrite.py` & `tdf_tool-2.4.7/tdf_tool/tools/cli/module_deps_rewrite.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/cli/project_cli.py` & `tdf_tool-2.4.7/tdf_tool/tools/cli/project_cli.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/cli/utils/yaml_utils.py` & `tdf_tool-2.4.7/tdf_tool/tools/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/cmd.py` & `tdf_tool-2.4.7/tdf_tool/tools/cmd.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 17 07:03:28 2024 UTC, .py size: 1310 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 4074 1f66 1e05 0000  a.......@t.f....
+00000000: 610d 0d0a 0000 0000 04e9 2066 1e05 0000  a......... f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 8302 5a08  ..G.d.d...d...Z.
 00000070: 6401 5300 2907 e900 0000 004e 2901 da05  d.S.)......N)...
```

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 17 09:14:57 2024 UTC, .py size: 1267 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1193 1f66 f304 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 04e9 2066 f304 0000  a......... f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6507  d.l.m.Z.m.Z...e.
 00000060: 4700 6405 6406 8400 6406 6506 8303 8301  G.d.d...d.e.....
 00000070: 5a08 4700 6407 6408 8400 6408 8302 5a09  Z.G.d.d...d...Z.
```

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/config/config.py` & `tdf_tool-2.4.7/tdf_tool/tools/config/config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/config/initial_json_config.py` & `tdf_tool-2.4.7/tdf_tool/tools/config/initial_json_config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/config/module_json_config.py` & `tdf_tool-2.4.7/tdf_tool/tools/config/module_json_config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/config/packages_config.py` & `tdf_tool-2.4.7/tdf_tool/tools/config/packages_config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/dependencies_analysis.py` & `tdf_tool-2.4.7/tdf_tool/tools/dependencies_analysis.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/fix_header/fix_header_entry.py` & `tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_entry.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/fix_header/fix_header_lint.py` & `tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/fix_header/fix_header_lint_tool.py` & `tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_lint_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/fix_header/fix_header_replace_tool.py` & `tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_replace_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/flutter_script.py` & `tdf_tool-2.4.7/tdf_tool/tools/flutter_script.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/gitlab/gitlab_utils.py` & `tdf_tool-2.4.7/tdf_tool/tools/gitlab/gitlab_utils.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/gitlab/python_gitlab_api.py` & `tdf_tool-2.4.7/tdf_tool/tools/gitlab/python_gitlab_api.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/module/module_tools.py` & `tdf_tool-2.4.7/tdf_tool/tools/module/module_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/package/seal_off_package_utils.py` & `tdf_tool-2.4.7/tdf_tool/tools/package/seal_off_package_utils.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/platform_tools.py` & `tdf_tool-2.4.7/tdf_tool/tools/platform_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/print.py` & `tdf_tool-2.4.7/tdf_tool/tools/print.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/regular_tool.py` & `tdf_tool-2.4.7/tdf_tool/tools/regular_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/shell_dir.py` & `tdf_tool-2.4.7/tdf_tool/tools/shell_dir.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/file_util.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/file_util.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/flutter_translate_lint.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/flutter_translate_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/flutter_translate_tools.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/flutter_translate_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/ios_translate.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/ios_translate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/ios_translate_lint.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/ios_translate_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/ios_module.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_module.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/location_string_temp.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/location_string_temp.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/podspec.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/podspec.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/ios/tools/string_util.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/string_util.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/tools/translate_tool.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/tools/translate_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/translate/translate_lint.py` & `tdf_tool-2.4.7/tdf_tool/tools/translate/translate_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc` & `tdf_tool-2.4.7/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.6/setup.py` & `tdf_tool-2.4.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,400 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tdf_tool
+Version: 2.4.7
+Summary: 二维火 flutter 脚手架工具
+Home-page: https://git.2dfire.net/app/flutter/tools/package_tools
+License: MIT
+Keywords: tdf,tdf-tool,tdf_tool
+Author: Jian Xu
+Author-email: 3386218996@qq.com
+Requires-Python: >=3.9.0,<4.0.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: environs (>=9.5.0,<10.0.0)
+Requires-Dist: fire (>=0.4.0,<0.5.0)
+Requires-Dist: googletrans (==3.1.0a0)
+Requires-Dist: python-gitlab (==1.15.0)
+Requires-Dist: requests (==2.27.1)
+Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
+Project-URL: Repository, https://git.2dfire.net/app/flutter/tools/package_tools.git
+Description-Content-Type: text/markdown
 
-packages = \
-['tdf_tool',
- 'tdf_tool.pipelines',
- 'tdf_tool.tools',
- 'tdf_tool.tools.cli',
- 'tdf_tool.tools.cli.bean',
- 'tdf_tool.tools.cli.utils',
- 'tdf_tool.tools.config',
- 'tdf_tool.tools.fix_header',
- 'tdf_tool.tools.gitlab',
- 'tdf_tool.tools.module',
- 'tdf_tool.tools.package',
- 'tdf_tool.tools.translate',
- 'tdf_tool.tools.translate.flutter',
- 'tdf_tool.tools.translate.flutter.tools',
- 'tdf_tool.tools.translate.ios',
- 'tdf_tool.tools.translate.ios.tools',
- 'tdf_tool.tools.translate.tools',
- 'tdf_tool.tools.vscode']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['environs>=9.5.0,<10.0.0',
- 'fire>=0.4.0,<0.5.0',
- 'googletrans==3.1.0a0',
- 'python-gitlab==1.15.0',
- 'requests==2.27.1',
- 'ruamel.yaml>=0.17.21,<0.18.0']
-
-entry_points = \
-{'console_scripts': ['tdf_tool = tdf_tool.app:main', 'tl = tdf_tool.app:main']}
-
-setup_kwargs = {
-    'name': 'tdf-tool',
-    'version': '2.4.6',
-    'description': '二维火 flutter 脚手架工具',
-    'long_description': '## 帮助文档\n\n```shell\nNAME\n    tdf_tool - 二维火 Flutter 脚手架工具，包含项目构建，依赖分析，git等功能。。\n\nSYNOPSIS\n    tdf_tool GROUP | COMMAND\n\nDESCRIPTION\n    二维火 Flutter 脚手架工具，包含项目构建，依赖分析，git等功能。。\n\nGROUPS\n    GROUP is one of the following:\n\n     module\n       模块相关工具： tdf_tool module -h 查看详情\n\n     package\n       封包工具相关：tdf_tool package -h 查看详情\n\n     translate\n       国际化相关：tdf_tool translate -h 查看详情\n\nCOMMANDS\n    COMMAND is one of the following:\n\n     git\n       tdf_tool git【git 命令】：批量操作 git 命令, 例如 tdf_tool git push\n\n     router\n       tdf_tool router：会以交互式进行路由操作，对指定的模块执行路由生成和路由注册逻辑\n\n     upgrade\n       tdf_tool upgrade：升级插件到最新版本\n        \n```\n\n\n\n## 插件安装方式\n\n安装python包\n\n```\npip3 install tdf-tool --user\n```\n\n安装并更新python包\n\n```\npip3 install --upgrade tdf-tool --user\n```\n\n安装测试环境python包\n\n```\npip3 install -i https://test.pypi.org/simple/ tdf-tool --user\n```\n\n安装并更新测试环境python包\n\n```\npip3 install --upgrade -i https://test.pypi.org/simple/ tdf-tool --user\n```\n\n\n\n## 工具使用流程说明\n\n### 1.准备工作\n\n- 确保python的bin插件目录已经被配置到环境变量中（这一步不满足的话，插件安装之后是无法识别到本插件命令的）\n\n- 在~目录下，创建.tdf_tool_config文件并配置相关必需属性如下\n\n```json\ngit_private_token=***\n```\n\ngit_private_token是gitlab的token\n\n获取途径：进入gitlab页面，点击右上角头像，选择Preferences，选择左侧列表中的AccessToken进行创建\n\n**上述步骤如果没有做，会在使用插件时，会有提示**\n\n### 2.初始化\n\n#### i.进入壳目录（确保执行命令在壳目录内）\n\n#### ii.执行tdf_tool module init\n\n- 判断当前目录是否存在tdf_cache，若不存在，则会自动创建tdf_cache\n- 自动读取当前壳模块名称，写入initial_config.json配置文件；\n- 读取当前壳分支，写入initial_config.json配置文件；\n- 交互式提示用户输入需要开发的模块名并写入initial_config.json配置文件的moduleNameList列表字段中\n- ！退出，即输入完成\n- 自动clone所有开发模块到  ```../.tdf_flutter```  隐藏目录中；\n- 将所有开发模块分支切换至与壳一致；\n- 自动分析依赖树，并**由下至上**对所有模块自动执行```flutter pub upgrade```;\n\n#### iii.开发过程中\n\n##### 1.开发模块添加\n\n- 若是有新模块需要添加入开发模块中，可直接修改initial_config.json配置文件，修改moduleNameList字段；\n- 执行tdf_tool deps更新依赖\n\n##### 2.新开发模块添加\n\n- 添加新模块后，会提示找不到模块，实际查找的是```tdf_cache```文件夹中的module_config.json文件；\n- 如果没有找到该模块，则可以执行```tdf_tool module-update```,更新远程module_config.json文件；\n- 删掉本地的module_config.json文件，重新执行命令即可，脚本会自动判断本地是否存在该配置文件，如果不存在会**下载**；\n\n<span style="color:#ff0000">请确保gitlab仓库的新开发模块master分支是一个flutter模块，如果判定不是flutter模块，则会报错（判定条件为存在pubspec.yaml文件）</span>\n\n\n\n### 3.版本控制\n\n版本控制请使用tdf_tool命令，命令详情可使用  ```tdf_tool -h```  查看，现已支持大部分命令，若有特殊命令需要执行，可以使用  ```tdf_tool <git命令>``` ，如：```tdf_tool git add .```\n\n\n\n### 4.自动打包发布\n\n暂未接入打包工具，预计下一季度进行支持；\n\n\n\n**<span style="color:#ff0000">FAQ</span>**\n\nwindows系统请使用bash命令；\n\n\n\n## 额外功能说明\n\n### 1.二维数组表达依赖树\n\n生成一个二维数组，可根据该二维数组的数据进行**并发**打tag，每一层的模块，都可以同时进行打tag发布操作，减少发布耗时；\n\n```json\n[\n\t["tdf_channel", "tdf_event", "tdf_network"], \n\t["tdf_widgets"], \n\t["tdf_smart_devices", "tdf_account_module"], \n\t["flutter_reset_module"]\n]\n```\n\n如上数据，数组中每一个节点中的模块均可同时打tag，节点之间需要由上至下的顺序进行tag操作\n\n\n\n### 2.插件更新\n\n执行 ```tdf_tool upgrade```\n\n\n\n### 3.远程模块配置文件更新\n\n执行 ```tdf_tool module module_update```\n\n\n\n## 依赖树分析原理\n\n采用有向有/无环图进行依赖树的分析\n\n数据结构采用如下：\n\n```python\nclass DependencyNode:\n    def __init__(self):\n        self.nodeName = \'\'\n        self.parent = []  # 父亲节点列表\n        self.children = []  # 子孙节点列表\n        self.delete = False\n```\n\n![dependency](./README_DIR/dependency.png)\n\n如上图1：一个正常的依赖树表示；\n\n如上图2：对图1中，依赖树所有节点去重，变换为图2有向图；\t\n\n\n\n**分析流程：**\n\n**依赖图构建**\n\n```python\n# 生成依赖图\n    def _generateDependenciesMap(self):\n        for package in self.__moduleDependenciesMap:\n            for module in moduleNameList:\n                if package == module:\n                    # 到这一步表明当前这个模块属于开发模块且在当前模块的依赖模块列表中，是当前模块的子模块\n                    self._mNodeDict[self.__moduleName].children.append(package)\n                    self._mNodeDict[package].parent.append(self.__moduleName)\n```\n\n- 共5个节点\n\n  - node构建：\n\n    - ```python\n      {\n      \t"模块1":{\n          "nodeNmae": "模块1",\n          "parent": [],\n          "children": ["模块2","模块3","模块4","模块5"],\n          "delete": False\n      \t},\n      \t"模块2":{\n          "nodeNmae": "模块2",\n          "parent": ["模块1"],\n          "children": ["模块4","模块5"],\n          "delete": False\n      \t}\n      \t"模块3":{\n          "nodeNmae": "模块3",\n          "parent": ["模块1"],\n          "children": ["模块5"],\n          "delete": False\n      \t}\n      \t"模块4":{\n          "nodeNmae": "模块4",\n          "parent": ["模块1","模块2"],\n          "children": [],\n          "delete": False\n      \t}\n      \t"模块5":{\n          "nodeNmae": "模块5",\n          "parent": ["模块1","模块2","模块3"],\n          "children": [],\n          "delete": False\n      \t}\n      }\n      ```\n\n**依赖图解析伪代码（以一维数组为例）**\n\n```python\n# 返回二维数组，用于并发打tag\n    def _generateDependenciesOrder(self):\n        resList = []\n        while 存在节点delete属性不为True:\n            \n            for：查找子节点为0的节点\n            \t设置节点delete属性为True\n              \n            for：deleteItemList = 拿到所有delete属性为true的节点\n\n            for：遍历所有节点，如果节点的子节点中包含deleteItemList的节点，则将其从子节点列表中删除\n```\n\n\n\n\n\n- **initial_config.json文件说明**\n\n  ```json\n  {\n      "featureBranch": "feature/test_dev_1", // 开发分支\n      "shellName": "flutter_reset_module",\n      // 项目需要开发的模块,可自由配置\n      "moduleNameList": [\n          "flutter_reset_module",\n          "tdf_smart_devices",\n          "tdf_widgets",\n          "tdf_channel"\n      ]\n  }\n  ```\n\n- **module_config.json文件说明**\n\n  ```json\n  {\n      "flutter_globalyun_us_module": {\n        \t"id": "11111"\n          "type": "shell",\n          "git": "git@git.2dfire.net:app/flutter/app/flutter_globalyun_us_module.git"\n      },\n      "tdf_router_anno": {\n          "type": "base",\n          "git": "git@git.2dfire.net:app/flutter/app/tdf_router_anno.git"\n      },\n  }\n  //语意\n  {\n    "模块名":{\n      "id": 项目gitlab id\n      "类型": gitlab group名\n      "git": gitlab地址\n    }\n  }\n  ```\n\n\n\n## 后续计划\n\n<span style="color:#ff0000">**问题：**</span>由于现在flutter ci 【lint】【tag】任务脚本成功率过于低，很多时候是因为项目模块的配置问题导致的，且后续会接入一键打tag工具\n\n方案：在执行统一push前，对所有模块的项目配置信息进行校验，确保数据规范；\n\n\n\n## 插件打包发布命令\n\n**插件打包命令**\n\n```\npoetry build\n```\n**插件发布命令**\n\n```\npoetry publish\n```\n\n## History\n\n### 2.1.00\n\n- 路由功能支持flutter版本3.3.10，兼容flutter版本2.2.3；\n\n### 2.0.61\n\n- Flutter国际化字符串整合；\n\n### 2.0.38\n\n- 路由生成完后增加路由相关代码format（解决windows代码生成后顺序错乱）；\n\n### 2.0.01\n\n- Cli 框架升级；\n- 代码重构；\n\n### **1.1.00（2022-4-28）**\n\n- 国际化解决输出json中包含转义字符的问题，如\\n；\n- 四类语言输出文件自动格式化\n\n### **1.0.55（2022-4-28）**\n\n- 国际化key使用中文（依照ios项目开发形式）；\n\n### **1.0.53（2022-4-28）**\n\n- 国际化流程中，兼容解决部分json解析失败问题，譬如字符串中包含"="符号；\n\n> 错误日志如：Unterminated string starting at: line 1 column 5650 (char 5649)\n\n### **1.0.50（2022-4-28）**\n\n- 国际化增加繁体字翻译；\n\n',
-    'author': 'Jian Xu',
-    'author_email': '3386218996@qq.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://git.2dfire.net/app/flutter/tools/package_tools',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9.0,<4.0.0',
-}
+## 帮助文档
+
+```shell
+NAME
+    tdf_tool - 二维火 Flutter 脚手架工具，包含项目构建，依赖分析，git等功能。。
+
+SYNOPSIS
+    tdf_tool GROUP | COMMAND
+
+DESCRIPTION
+    二维火 Flutter 脚手架工具，包含项目构建，依赖分析，git等功能。。
+
+GROUPS
+    GROUP is one of the following:
+
+     module
+       模块相关工具： tdf_tool module -h 查看详情
+
+     package
+       封包工具相关：tdf_tool package -h 查看详情
+
+     translate
+       国际化相关：tdf_tool translate -h 查看详情
+
+COMMANDS
+    COMMAND is one of the following:
+
+     git
+       tdf_tool git【git 命令】：批量操作 git 命令, 例如 tdf_tool git push
+
+     router
+       tdf_tool router：会以交互式进行路由操作，对指定的模块执行路由生成和路由注册逻辑
+
+     upgrade
+       tdf_tool upgrade：升级插件到最新版本
+        
+```
+
+
+
+## 插件安装方式
+
+安装python包
+
+```
+pip3 install tdf-tool --user
+```
+
+安装并更新python包
+
+```
+pip3 install --upgrade tdf-tool --user
+```
+
+安装测试环境python包
+
+```
+pip3 install -i https://test.pypi.org/simple/ tdf-tool --user
+```
+
+安装并更新测试环境python包
+
+```
+pip3 install --upgrade -i https://test.pypi.org/simple/ tdf-tool --user
+```
+
+
+
+## 工具使用流程说明
+
+### 1.准备工作
+
+- 确保python的bin插件目录已经被配置到环境变量中（这一步不满足的话，插件安装之后是无法识别到本插件命令的）
+
+- 在~目录下，创建.tdf_tool_config文件并配置相关必需属性如下
+
+```json
+git_private_token=***
+```
+
+git_private_token是gitlab的token
+
+获取途径：进入gitlab页面，点击右上角头像，选择Preferences，选择左侧列表中的AccessToken进行创建
+
+**上述步骤如果没有做，会在使用插件时，会有提示**
+
+### 2.初始化
+
+#### i.进入壳目录（确保执行命令在壳目录内）
+
+#### ii.执行tdf_tool module init
+
+- 判断当前目录是否存在tdf_cache，若不存在，则会自动创建tdf_cache
+- 自动读取当前壳模块名称，写入initial_config.json配置文件；
+- 读取当前壳分支，写入initial_config.json配置文件；
+- 交互式提示用户输入需要开发的模块名并写入initial_config.json配置文件的moduleNameList列表字段中
+- ！退出，即输入完成
+- 自动clone所有开发模块到  ```../.tdf_flutter```  隐藏目录中；
+- 将所有开发模块分支切换至与壳一致；
+- 自动分析依赖树，并**由下至上**对所有模块自动执行```flutter pub upgrade```;
+
+#### iii.开发过程中
+
+##### 1.开发模块添加
+
+- 若是有新模块需要添加入开发模块中，可直接修改initial_config.json配置文件，修改moduleNameList字段；
+- 执行tdf_tool deps更新依赖
+
+##### 2.新开发模块添加
+
+- 添加新模块后，会提示找不到模块，实际查找的是```tdf_cache```文件夹中的module_config.json文件；
+- 如果没有找到该模块，则可以执行```tdf_tool module-update```,更新远程module_config.json文件；
+- 删掉本地的module_config.json文件，重新执行命令即可，脚本会自动判断本地是否存在该配置文件，如果不存在会**下载**；
+
+<span style="color:#ff0000">请确保gitlab仓库的新开发模块master分支是一个flutter模块，如果判定不是flutter模块，则会报错（判定条件为存在pubspec.yaml文件）</span>
+
+
+
+### 3.版本控制
+
+版本控制请使用tdf_tool命令，命令详情可使用  ```tdf_tool -h```  查看，现已支持大部分命令，若有特殊命令需要执行，可以使用  ```tdf_tool <git命令>``` ，如：```tdf_tool git add .```
+
+
+
+### 4.自动打包发布
+
+暂未接入打包工具，预计下一季度进行支持；
+
+
+
+**<span style="color:#ff0000">FAQ</span>**
+
+windows系统请使用bash命令；
+
+
+
+## 额外功能说明
+
+### 1.二维数组表达依赖树
+
+生成一个二维数组，可根据该二维数组的数据进行**并发**打tag，每一层的模块，都可以同时进行打tag发布操作，减少发布耗时；
+
+```json
+[
+	["tdf_channel", "tdf_event", "tdf_network"], 
+	["tdf_widgets"], 
+	["tdf_smart_devices", "tdf_account_module"], 
+	["flutter_reset_module"]
+]
+```
+
+如上数据，数组中每一个节点中的模块均可同时打tag，节点之间需要由上至下的顺序进行tag操作
+
+
+
+### 2.插件更新
+
+执行 ```tdf_tool upgrade```
+
+
+
+### 3.远程模块配置文件更新
+
+执行 ```tdf_tool module module_update```
+
+
+
+## 依赖树分析原理
+
+采用有向有/无环图进行依赖树的分析
+
+数据结构采用如下：
+
+```python
+class DependencyNode:
+    def __init__(self):
+        self.nodeName = ''
+        self.parent = []  # 父亲节点列表
+        self.children = []  # 子孙节点列表
+        self.delete = False
+```
+
+![dependency](./README_DIR/dependency.png)
+
+如上图1：一个正常的依赖树表示；
+
+如上图2：对图1中，依赖树所有节点去重，变换为图2有向图；	
+
+
+
+**分析流程：**
+
+**依赖图构建**
+
+```python
+# 生成依赖图
+    def _generateDependenciesMap(self):
+        for package in self.__moduleDependenciesMap:
+            for module in moduleNameList:
+                if package == module:
+                    # 到这一步表明当前这个模块属于开发模块且在当前模块的依赖模块列表中，是当前模块的子模块
+                    self._mNodeDict[self.__moduleName].children.append(package)
+                    self._mNodeDict[package].parent.append(self.__moduleName)
+```
+
+- 共5个节点
+
+  - node构建：
+
+    - ```python
+      {
+      	"模块1":{
+          "nodeNmae": "模块1",
+          "parent": [],
+          "children": ["模块2","模块3","模块4","模块5"],
+          "delete": False
+      	},
+      	"模块2":{
+          "nodeNmae": "模块2",
+          "parent": ["模块1"],
+          "children": ["模块4","模块5"],
+          "delete": False
+      	}
+      	"模块3":{
+          "nodeNmae": "模块3",
+          "parent": ["模块1"],
+          "children": ["模块5"],
+          "delete": False
+      	}
+      	"模块4":{
+          "nodeNmae": "模块4",
+          "parent": ["模块1","模块2"],
+          "children": [],
+          "delete": False
+      	}
+      	"模块5":{
+          "nodeNmae": "模块5",
+          "parent": ["模块1","模块2","模块3"],
+          "children": [],
+          "delete": False
+      	}
+      }
+      ```
+
+**依赖图解析伪代码（以一维数组为例）**
+
+```python
+# 返回二维数组，用于并发打tag
+    def _generateDependenciesOrder(self):
+        resList = []
+        while 存在节点delete属性不为True:
+            
+            for：查找子节点为0的节点
+            	设置节点delete属性为True
+              
+            for：deleteItemList = 拿到所有delete属性为true的节点
+
+            for：遍历所有节点，如果节点的子节点中包含deleteItemList的节点，则将其从子节点列表中删除
+```
+
+
+
+
+
+- **initial_config.json文件说明**
+
+  ```json
+  {
+      "featureBranch": "feature/test_dev_1", // 开发分支
+      "shellName": "flutter_reset_module",
+      // 项目需要开发的模块,可自由配置
+      "moduleNameList": [
+          "flutter_reset_module",
+          "tdf_smart_devices",
+          "tdf_widgets",
+          "tdf_channel"
+      ]
+  }
+  ```
+
+- **module_config.json文件说明**
+
+  ```json
+  {
+      "flutter_globalyun_us_module": {
+        	"id": "11111"
+          "type": "shell",
+          "git": "git@git.2dfire.net:app/flutter/app/flutter_globalyun_us_module.git"
+      },
+      "tdf_router_anno": {
+          "type": "base",
+          "git": "git@git.2dfire.net:app/flutter/app/tdf_router_anno.git"
+      },
+  }
+  //语意
+  {
+    "模块名":{
+      "id": 项目gitlab id
+      "类型": gitlab group名
+      "git": gitlab地址
+    }
+  }
+  ```
+
+
+
+## 后续计划
+
+<span style="color:#ff0000">**问题：**</span>由于现在flutter ci 【lint】【tag】任务脚本成功率过于低，很多时候是因为项目模块的配置问题导致的，且后续会接入一键打tag工具
+
+方案：在执行统一push前，对所有模块的项目配置信息进行校验，确保数据规范；
+
+
+
+## 插件打包发布命令
+
+**插件打包命令**
+
+```
+poetry build
+```
+**插件发布命令**
+
+```
+poetry publish
+```
+
+## History
+
+### 2.1.00
+
+- 路由功能支持flutter版本3.3.10，兼容flutter版本2.2.3；
+
+### 2.0.61
+
+- Flutter国际化字符串整合；
+
+### 2.0.38
+
+- 路由生成完后增加路由相关代码format（解决windows代码生成后顺序错乱）；
+
+### 2.0.01
+
+- Cli 框架升级；
+- 代码重构；
+
+### **1.1.00（2022-4-28）**
+
+- 国际化解决输出json中包含转义字符的问题，如\n；
+- 四类语言输出文件自动格式化
+
+### **1.0.55（2022-4-28）**
+
+- 国际化key使用中文（依照ios项目开发形式）；
+
+### **1.0.53（2022-4-28）**
+
+- 国际化流程中，兼容解决部分json解析失败问题，譬如字符串中包含"="符号；
+
+> 错误日志如：Unterminated string starting at: line 1 column 5650 (char 5649)
+
+### **1.0.50（2022-4-28）**
+
+- 国际化增加繁体字翻译；
 
 
-setup(**setup_kwargs)
```

