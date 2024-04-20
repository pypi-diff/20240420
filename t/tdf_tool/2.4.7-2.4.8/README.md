# Comparing `tmp/tdf_tool-2.4.7.tar.gz` & `tmp/tdf_tool-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdf_tool-2.4.7.tar", max compression
+gzip compressed data, was "tdf_tool-2.4.8.tar", max compression
```

## Comparing `tdf_tool-2.4.7.tar` & `tdf_tool-2.4.8.tar`

### file list

```diff
@@ -1,165 +1,165 @@
--rw-r--r--   0        0        0     1068 2024-04-16 07:59:17.944743 tdf_tool-2.4.7/LICENSE
--rw-r--r--   0        0        0     9217 2024-04-16 07:59:17.944961 tdf_tool-2.4.7/README.md
--rw-r--r--   0        0        0     1608 2024-04-19 10:02:02.216830 tdf_tool-2.4.7/pyproject.toml
--rw-r--r--   0        0        0      321 2024-04-16 07:59:17.947227 tdf_tool-2.4.7/tdf_tool/app.py
--rw-r--r--   0        0        0     1106 2024-04-18 09:33:56.862188 tdf_tool-2.4.7/tdf_tool/pipeline.py
--rw-r--r--   0        0        0     8469 2024-04-18 09:33:56.862568 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc
--rw-r--r--   0        0        0     4497 2024-04-19 02:17:38.880307 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc
--rw-r--r--   0        0        0     7766 2024-04-19 10:01:22.245312 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc
--rw-r--r--   0        0        0      424 2024-04-16 07:59:17.947648 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/cmd.cpython-39.pyc
--rw-r--r--   0        0        0     2567 2024-04-16 07:59:17.947827 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc
--rw-r--r--   0        0        0     1676 2024-04-19 02:17:38.888443 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc
--rw-r--r--   0        0        0     2668 2024-04-16 07:59:17.948134 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc
--rw-r--r--   0        0        0     1619 2024-04-19 02:17:38.894201 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc
--rw-r--r--   0        0        0      496 2024-04-16 07:59:17.948441 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/init.cpython-39.pyc
--rw-r--r--   0        0        0     3015 2024-04-16 07:59:17.948597 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc
--rw-r--r--   0        0        0     2292 2024-04-19 02:17:38.497917 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc
--rw-r--r--   0        0        0     2981 2024-04-16 07:59:17.948929 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc
--rw-r--r--   0        0        0     2243 2024-04-19 02:17:38.892162 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc
--rw-r--r--   0        0        0    36213 2024-04-16 07:59:17.949402 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc
--rw-r--r--   0        0        0    16038 2024-04-19 09:06:09.150577 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc
--rw-r--r--   0        0        0     3262 2024-04-16 07:59:17.950144 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc
--rw-r--r--   0        0        0     1989 2024-04-19 02:17:38.771913 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc
--rw-r--r--   0        0        0      817 2024-04-16 07:59:17.950609 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc
--rw-r--r--   0        0        0      621 2024-04-18 09:33:56.866062 tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc
--rw-r--r--   0        0        0     5130 2024-04-18 09:33:56.866355 tdf_tool-2.4.7/tdf_tool/pipelines/annotation.py
--rw-r--r--   0        0        0     7845 2024-04-19 10:01:18.301914 tdf_tool-2.4.7/tdf_tool/pipelines/api_interaction.py
--rw-r--r--   0        0        0     1244 2024-04-18 09:33:56.867085 tdf_tool-2.4.7/tdf_tool/pipelines/fix_header.py
--rw-r--r--   0        0        0     1211 2024-04-18 09:33:56.867471 tdf_tool-2.4.7/tdf_tool/pipelines/git.py
--rw-r--r--   0        0        0     1889 2024-04-18 09:33:56.867849 tdf_tool-2.4.7/tdf_tool/pipelines/module.py
--rw-r--r--   0        0        0     1630 2024-04-18 09:33:56.868234 tdf_tool-2.4.7/tdf_tool/pipelines/package.py
--rw-r--r--   0        0        0    21886 2024-04-19 08:19:40.561443 tdf_tool-2.4.7/tdf_tool/pipelines/router.py
--rw-r--r--   0        0        0     1656 2024-04-18 09:33:56.869173 tdf_tool-2.4.7/tdf_tool/pipelines/translate.py
--rw-r--r--   0        0        0      179 2024-04-16 07:59:17.952763 tdf_tool-2.4.7/tdf_tool/pipelines/upgrade.py
--rw-r--r--   0        0        0     1653 2024-04-16 07:59:17.953204 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc
--rw-r--r--   0        0        0     1064 2024-04-18 09:33:56.869593 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc
--rw-r--r--   0        0        0    10270 2024-04-16 07:59:17.953777 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc
--rw-r--r--   0        0        0     5149 2024-04-18 09:33:56.870029 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc
--rw-r--r--   0        0        0     1328 2024-04-16 07:59:17.954419 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/env.cpython-311.pyc
--rw-r--r--   0        0        0     1113 2024-04-19 09:46:49.061939 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/env.cpython-39.pyc
--rw-r--r--   0        0        0      890 2024-04-19 09:59:10.596913 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/generator.cpython-39.pyc
--rw-r--r--   0        0        0     2480 2024-04-16 07:59:17.954948 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc
--rw-r--r--   0        0        0     1464 2024-04-18 09:33:56.871044 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc
--rw-r--r--   0        0        0     2969 2024-04-16 07:59:17.955456 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/print.cpython-311.pyc
--rw-r--r--   0        0        0     2040 2024-04-19 09:43:51.505624 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/print.cpython-39.pyc
--rw-r--r--   0        0        0     9661 2024-04-16 07:59:17.955984 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc
--rw-r--r--   0        0        0     6181 2024-04-18 09:33:56.871935 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc
--rw-r--r--   0        0        0    10739 2024-04-16 07:59:17.956576 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc
--rw-r--r--   0        0        0     5620 2024-04-19 02:17:38.568605 tdf_tool-2.4.7/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc
--rw-r--r--   0        0        0    11432 2024-04-16 07:59:17.957426 tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc
--rw-r--r--   0        0        0     7694 2024-04-18 09:33:56.873380 tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc
--rw-r--r--   0        0        0     7216 2024-04-16 07:59:17.958050 tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc
--rw-r--r--   0        0        0     4018 2024-04-18 09:33:56.873929 tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc
--rw-r--r--   0        0        0     1835 2024-04-18 09:33:56.874377 tdf_tool-2.4.7/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc
--rw-r--r--   0        0        0     1628 2024-04-16 07:59:17.959126 tdf_tool-2.4.7/tdf_tool/tools/cli/bean/deps_item.py
--rw-r--r--   0        0        0    12287 2024-04-16 07:59:17.959442 tdf_tool-2.4.7/tdf_tool/tools/cli/module_deps_rewrite.py
--rw-r--r--   0        0        0     5041 2024-04-16 07:59:17.959734 tdf_tool-2.4.7/tdf_tool/tools/cli/project_cli.py
--rw-r--r--   0        0        0     1919 2024-04-18 09:33:56.874872 tdf_tool-2.4.7/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc
--rw-r--r--   0        0        0     1833 2024-04-16 07:59:17.960396 tdf_tool-2.4.7/tdf_tool/tools/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      559 2024-04-16 07:59:17.960648 tdf_tool-2.4.7/tdf_tool/tools/cmd.py
--rw-r--r--   0        0        0     7002 2024-04-16 07:59:17.961174 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     3385 2024-04-18 09:33:56.875378 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0     2717 2024-04-16 07:59:17.961718 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc
--rw-r--r--   0        0        0     1491 2024-04-19 02:17:38.769502 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc
--rw-r--r--   0        0        0     2693 2024-04-16 07:59:17.962260 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc
--rw-r--r--   0        0        0     2732 2024-04-16 07:59:17.962513 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc
--rw-r--r--   0        0        0     2103 2024-04-19 02:17:38.774000 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc
--rw-r--r--   0        0        0     9155 2024-04-16 07:59:17.963058 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc
--rw-r--r--   0        0        0     4496 2024-04-18 09:33:56.876915 tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc
--rw-r--r--   0        0        0     3983 2024-04-16 07:59:17.963572 tdf_tool-2.4.7/tdf_tool/tools/config/config.py
--rw-r--r--   0        0        0     1310 2024-04-18 09:33:56.877413 tdf_tool-2.4.7/tdf_tool/tools/config/initial_json_config.py
--rw-r--r--   0        0        0     1267 2024-04-18 09:33:56.877960 tdf_tool-2.4.7/tdf_tool/tools/config/module_json_config.py
--rw-r--r--   0        0        0     5593 2024-04-16 07:59:17.964325 tdf_tool-2.4.7/tdf_tool/tools/config/packages_config.py
--rw-r--r--   0        0        0     7704 2024-04-16 07:59:17.964588 tdf_tool-2.4.7/tdf_tool/tools/dependencies_analysis.py
--rw-r--r--   0        0        0      776 2024-04-19 09:46:46.688382 tdf_tool-2.4.7/tdf_tool/tools/env.py
--rw-r--r--   0        0        0     6312 2024-04-16 07:59:17.965341 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc
--rw-r--r--   0        0        0     3616 2024-04-18 09:33:56.878578 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc
--rw-r--r--   0        0        0     3174 2024-04-16 07:59:17.965839 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc
--rw-r--r--   0        0        0     2004 2024-04-18 09:33:56.879118 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc
--rw-r--r--   0        0        0     4314 2024-04-16 07:59:17.966355 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc
--rw-r--r--   0        0        0     2464 2024-04-18 09:33:56.879669 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc
--rw-r--r--   0        0        0     6437 2024-04-16 07:59:17.966902 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc
--rw-r--r--   0        0        0     3681 2024-04-18 09:33:56.880258 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc
--rw-r--r--   0        0        0     2422 2024-04-16 07:59:17.967708 tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc
--rw-r--r--   0        0        0     3345 2024-04-16 07:59:17.967959 tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_entry.py
--rw-r--r--   0        0        0     1586 2024-04-16 07:59:17.968270 tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_lint.py
--rw-r--r--   0        0        0     2137 2024-04-16 07:59:17.968589 tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_lint_tool.py
--rw-r--r--   0        0        0     4095 2024-04-16 07:59:17.968850 tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_replace_tool.py
--rw-r--r--   0        0        0     1159 2024-04-16 07:59:17.969195 tdf_tool-2.4.7/tdf_tool/tools/flutter_script.py
--rw-r--r--   0        0        0      444 2024-04-19 09:59:03.824969 tdf_tool-2.4.7/tdf_tool/tools/generator.py
--rw-r--r--   0        0        0     7243 2024-04-16 07:59:17.969845 tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc
--rw-r--r--   0        0        0     4190 2024-04-18 09:33:56.880901 tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc
--rw-r--r--   0        0        0     7055 2024-04-16 07:59:17.970442 tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc
--rw-r--r--   0        0        0     3786 2024-04-18 09:33:56.881487 tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc
--rw-r--r--   0        0        0      593 2024-04-16 07:59:17.971051 tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc
--rw-r--r--   0        0        0     5019 2024-04-16 07:59:17.971732 tdf_tool-2.4.7/tdf_tool/tools/gitlab/gitlab_utils.py
--rw-r--r--   0        0        0     3814 2024-04-16 07:59:17.972085 tdf_tool-2.4.7/tdf_tool/tools/gitlab/python_gitlab_api.py
--rw-r--r--   0        0        0     2482 2024-04-16 07:59:17.972678 tdf_tool-2.4.7/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc
--rw-r--r--   0        0        0     1412 2024-04-18 09:33:56.882138 tdf_tool-2.4.7/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc
--rw-r--r--   0        0        0     1063 2024-04-16 07:59:17.973603 tdf_tool-2.4.7/tdf_tool/tools/module/module_tools.py
--rw-r--r--   0        0        0    11056 2024-04-16 07:59:17.974266 tdf_tool-2.4.7/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc
--rw-r--r--   0        0        0     5267 2024-04-18 09:33:56.882719 tdf_tool-2.4.7/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc
--rw-r--r--   0        0        0     9752 2024-04-16 07:59:17.974933 tdf_tool-2.4.7/tdf_tool/tools/package/seal_off_package_utils.py
--rw-r--r--   0        0        0      911 2024-04-16 07:59:17.975191 tdf_tool-2.4.7/tdf_tool/tools/platform_tools.py
--rw-r--r--   0        0        0     1226 2024-04-19 09:43:13.615410 tdf_tool-2.4.7/tdf_tool/tools/print.py
--rw-r--r--   0        0        0     7598 2024-04-16 07:59:17.975770 tdf_tool-2.4.7/tdf_tool/tools/regular_tool.py
--rw-r--r--   0        0        0     5718 2024-04-18 09:33:56.883146 tdf_tool-2.4.7/tdf_tool/tools/shell_dir.py
--rw-r--r--   0        0        0     3840 2024-04-16 07:59:17.976600 tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc
--rw-r--r--   0        0        0     2161 2024-04-18 09:33:56.883746 tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc
--rw-r--r--   0        0        0     2695 2024-04-16 07:59:17.977108 tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc
--rw-r--r--   0        0        0     1678 2024-04-18 09:33:56.884279 tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc
--rw-r--r--   0        0        0    11711 2024-04-16 07:59:17.977716 tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0     1999 2024-04-16 07:59:17.977961 tdf_tool-2.4.7/tdf_tool/tools/translate/file_util.py
--rw-r--r--   0        0        0    15484 2024-04-16 07:59:17.978545 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc
--rw-r--r--   0        0        0     8285 2024-04-18 09:33:56.884733 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc
--rw-r--r--   0        0        0    26818 2024-04-16 07:59:17.979344 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc
--rw-r--r--   0        0        0    13427 2024-04-18 09:33:56.885241 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0    10691 2024-04-16 07:59:17.980114 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/flutter_translate_lint.py
--rw-r--r--   0        0        0    18954 2024-04-16 07:59:17.980464 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/flutter_translate_tools.py
--rw-r--r--   0        0        0     8395 2024-04-16 07:59:17.981075 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc
--rw-r--r--   0        0        0     4595 2024-04-18 09:33:56.885795 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc
--rw-r--r--   0        0        0     5228 2024-04-16 07:59:17.981648 tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py
--rw-r--r--   0        0        0      859 2024-04-16 07:59:17.982222 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc
--rw-r--r--   0        0        0     7351 2024-04-16 07:59:17.982702 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc
--rw-r--r--   0        0        0     7599 2024-04-16 07:59:17.983077 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc
--rw-r--r--   0        0        0     4216 2024-04-18 09:33:56.886328 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc
--rw-r--r--   0        0        0     3952 2024-04-16 07:59:17.983786 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc
--rw-r--r--   0        0        0     2347 2024-04-18 09:33:56.886740 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc
--rw-r--r--   0        0        0      870 2024-04-16 07:59:17.984330 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc
--rw-r--r--   0        0        0     4766 2024-04-16 07:59:17.984706 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0     6219 2024-04-16 07:59:17.985086 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc
--rw-r--r--   0        0        0     2631 2024-04-16 07:59:17.985435 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc
--rw-r--r--   0        0        0     4438 2024-04-16 07:59:17.985774 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/ios_translate.py
--rw-r--r--   0        0        0     2000 2024-04-16 07:59:17.986154 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/ios_translate_lint.py
--rw-r--r--   0        0        0     5061 2024-04-16 07:59:17.986697 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc
--rw-r--r--   0        0        0     2852 2024-04-18 09:33:56.887291 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc
--rw-r--r--   0        0        0    17576 2024-04-16 07:59:17.987402 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc
--rw-r--r--   0        0        0     9306 2024-04-18 09:33:56.887836 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc
--rw-r--r--   0        0        0     7901 2024-04-16 07:59:17.988120 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc
--rw-r--r--   0        0        0     4398 2024-04-18 09:33:56.888413 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc
--rw-r--r--   0        0        0     1158 2024-04-16 07:59:17.988695 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc
--rw-r--r--   0        0        0     1028 2024-04-18 09:33:56.889038 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc
--rw-r--r--   0        0        0    10070 2024-04-16 07:59:17.989363 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc
--rw-r--r--   0        0        0     5366 2024-04-18 09:33:56.889482 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0     2773 2024-04-16 07:59:17.989983 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc
--rw-r--r--   0        0        0     2689 2024-04-18 09:33:56.889936 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc
--rw-r--r--   0        0        0    11353 2024-04-16 07:59:17.990542 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc
--rw-r--r--   0        0        0     6226 2024-04-18 09:33:56.890414 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc
--rw-r--r--   0        0        0     4943 2024-04-16 07:59:17.991277 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc
--rw-r--r--   0        0        0     2687 2024-04-18 09:33:56.890983 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc
--rw-r--r--   0        0        0     3270 2024-04-16 07:59:17.991799 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py
--rw-r--r--   0        0        0    14326 2024-04-16 07:59:17.992093 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_module.py
--rw-r--r--   0        0        0     5223 2024-04-16 07:59:17.992380 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py
--rw-r--r--   0        0        0     1189 2024-04-16 07:59:17.992605 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py
--rw-r--r--   0        0        0     8191 2024-04-16 07:59:17.992866 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py
--rw-r--r--   0        0        0     2337 2024-04-16 07:59:17.993215 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/location_string_temp.py
--rw-r--r--   0        0        0     8684 2024-04-16 07:59:17.993505 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/podspec.py
--rw-r--r--   0        0        0     2886 2024-04-16 07:59:17.993759 tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/string_util.py
--rw-r--r--   0        0        0     8625 2024-04-16 07:59:17.994344 tdf_tool-2.4.7/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc
--rw-r--r--   0        0        0     5032 2024-04-18 09:33:56.891445 tdf_tool-2.4.7/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc
--rw-r--r--   0        0        0     5111 2024-04-16 07:59:17.994952 tdf_tool-2.4.7/tdf_tool/tools/translate/tools/translate_tool.py
--rw-r--r--   0        0        0     1408 2024-04-16 07:59:17.995250 tdf_tool-2.4.7/tdf_tool/tools/translate/translate_lint.py
--rw-r--r--   0        0        0     1268 2024-04-16 07:59:17.996782 tdf_tool-2.4.7/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc
--rw-r--r--   0        0        0      880 2024-04-18 09:33:56.891894 tdf_tool-2.4.7/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc
--rw-r--r--   0        0        0      440 2024-04-16 07:59:17.997353 tdf_tool-2.4.7/tdf_tool/tools/vscode/vscode.py
--rw-r--r--   0        0        0    10568 1970-01-01 00:00:00.000000 tdf_tool-2.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-16 07:59:17.944743 tdf_tool-2.4.8/LICENSE
+-rw-r--r--   0        0        0     9217 2024-04-16 07:59:17.944961 tdf_tool-2.4.8/README.md
+-rw-r--r--   0        0        0     1608 2024-04-20 02:38:19.860796 tdf_tool-2.4.8/pyproject.toml
+-rw-r--r--   0        0        0      321 2024-04-16 07:59:17.947227 tdf_tool-2.4.8/tdf_tool/app.py
+-rw-r--r--   0        0        0     1106 2024-04-18 09:33:56.862188 tdf_tool-2.4.8/tdf_tool/pipeline.py
+-rw-r--r--   0        0        0     8469 2024-04-18 09:33:56.862568 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc
+-rw-r--r--   0        0        0     4497 2024-04-19 02:17:38.880307 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc
+-rw-r--r--   0        0        0     7799 2024-04-20 02:32:50.400921 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc
+-rw-r--r--   0        0        0      424 2024-04-16 07:59:17.947648 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/cmd.cpython-39.pyc
+-rw-r--r--   0        0        0     2567 2024-04-16 07:59:17.947827 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc
+-rw-r--r--   0        0        0     1676 2024-04-19 02:17:38.888443 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc
+-rw-r--r--   0        0        0     2668 2024-04-16 07:59:17.948134 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc
+-rw-r--r--   0        0        0     1619 2024-04-19 02:17:38.894201 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc
+-rw-r--r--   0        0        0      496 2024-04-16 07:59:17.948441 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/init.cpython-39.pyc
+-rw-r--r--   0        0        0     3015 2024-04-16 07:59:17.948597 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc
+-rw-r--r--   0        0        0     2292 2024-04-19 02:17:38.497917 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc
+-rw-r--r--   0        0        0     2981 2024-04-16 07:59:17.948929 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc
+-rw-r--r--   0        0        0     2243 2024-04-19 02:17:38.892162 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc
+-rw-r--r--   0        0        0    36213 2024-04-16 07:59:17.949402 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc
+-rw-r--r--   0        0        0    16038 2024-04-19 09:06:09.150577 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc
+-rw-r--r--   0        0        0     3262 2024-04-16 07:59:17.950144 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc
+-rw-r--r--   0        0        0     1989 2024-04-19 02:17:38.771913 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc
+-rw-r--r--   0        0        0      817 2024-04-16 07:59:17.950609 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc
+-rw-r--r--   0        0        0      621 2024-04-18 09:33:56.866062 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc
+-rw-r--r--   0        0        0     5130 2024-04-18 09:33:56.866355 tdf_tool-2.4.8/tdf_tool/pipelines/annotation.py
+-rw-r--r--   0        0        0     7878 2024-04-20 02:32:38.597752 tdf_tool-2.4.8/tdf_tool/pipelines/api_interaction.py
+-rw-r--r--   0        0        0     1244 2024-04-18 09:33:56.867085 tdf_tool-2.4.8/tdf_tool/pipelines/fix_header.py
+-rw-r--r--   0        0        0     1211 2024-04-18 09:33:56.867471 tdf_tool-2.4.8/tdf_tool/pipelines/git.py
+-rw-r--r--   0        0        0     1889 2024-04-18 09:33:56.867849 tdf_tool-2.4.8/tdf_tool/pipelines/module.py
+-rw-r--r--   0        0        0     1630 2024-04-18 09:33:56.868234 tdf_tool-2.4.8/tdf_tool/pipelines/package.py
+-rw-r--r--   0        0        0    21886 2024-04-19 08:19:40.561443 tdf_tool-2.4.8/tdf_tool/pipelines/router.py
+-rw-r--r--   0        0        0     1656 2024-04-18 09:33:56.869173 tdf_tool-2.4.8/tdf_tool/pipelines/translate.py
+-rw-r--r--   0        0        0      179 2024-04-16 07:59:17.952763 tdf_tool-2.4.8/tdf_tool/pipelines/upgrade.py
+-rw-r--r--   0        0        0     1653 2024-04-16 07:59:17.953204 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc
+-rw-r--r--   0        0        0     1064 2024-04-18 09:33:56.869593 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc
+-rw-r--r--   0        0        0    10270 2024-04-16 07:59:17.953777 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc
+-rw-r--r--   0        0        0     5149 2024-04-18 09:33:56.870029 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc
+-rw-r--r--   0        0        0     1328 2024-04-16 07:59:17.954419 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/env.cpython-311.pyc
+-rw-r--r--   0        0        0     1113 2024-04-19 09:46:49.061939 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/env.cpython-39.pyc
+-rw-r--r--   0        0        0      890 2024-04-19 09:59:10.596913 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/generator.cpython-39.pyc
+-rw-r--r--   0        0        0     2480 2024-04-16 07:59:17.954948 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     1464 2024-04-18 09:33:56.871044 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     2969 2024-04-16 07:59:17.955456 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/print.cpython-311.pyc
+-rw-r--r--   0        0        0     2040 2024-04-19 09:43:51.505624 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/print.cpython-39.pyc
+-rw-r--r--   0        0        0     9661 2024-04-16 07:59:17.955984 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     6181 2024-04-18 09:33:56.871935 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc
+-rw-r--r--   0        0        0    10739 2024-04-16 07:59:17.956576 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc
+-rw-r--r--   0        0        0     5620 2024-04-19 02:17:38.568605 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc
+-rw-r--r--   0        0        0    11432 2024-04-16 07:59:17.957426 tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc
+-rw-r--r--   0        0        0     7694 2024-04-18 09:33:56.873380 tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc
+-rw-r--r--   0        0        0     7216 2024-04-16 07:59:17.958050 tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc
+-rw-r--r--   0        0        0     4018 2024-04-18 09:33:56.873929 tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc
+-rw-r--r--   0        0        0     1835 2024-04-18 09:33:56.874377 tdf_tool-2.4.8/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc
+-rw-r--r--   0        0        0     1628 2024-04-16 07:59:17.959126 tdf_tool-2.4.8/tdf_tool/tools/cli/bean/deps_item.py
+-rw-r--r--   0        0        0    12287 2024-04-16 07:59:17.959442 tdf_tool-2.4.8/tdf_tool/tools/cli/module_deps_rewrite.py
+-rw-r--r--   0        0        0     5041 2024-04-16 07:59:17.959734 tdf_tool-2.4.8/tdf_tool/tools/cli/project_cli.py
+-rw-r--r--   0        0        0     1919 2024-04-18 09:33:56.874872 tdf_tool-2.4.8/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     1833 2024-04-16 07:59:17.960396 tdf_tool-2.4.8/tdf_tool/tools/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      559 2024-04-16 07:59:17.960648 tdf_tool-2.4.8/tdf_tool/tools/cmd.py
+-rw-r--r--   0        0        0     7002 2024-04-16 07:59:17.961174 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     3385 2024-04-18 09:33:56.875378 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0        0        0     2717 2024-04-16 07:59:17.961718 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc
+-rw-r--r--   0        0        0     1491 2024-04-19 02:17:38.769502 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc
+-rw-r--r--   0        0        0     2693 2024-04-16 07:59:17.962260 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc
+-rw-r--r--   0        0        0     2732 2024-04-16 07:59:17.962513 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc
+-rw-r--r--   0        0        0     2103 2024-04-19 02:17:38.774000 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc
+-rw-r--r--   0        0        0     9155 2024-04-16 07:59:17.963058 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc
+-rw-r--r--   0        0        0     4496 2024-04-18 09:33:56.876915 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc
+-rw-r--r--   0        0        0     3983 2024-04-16 07:59:17.963572 tdf_tool-2.4.8/tdf_tool/tools/config/config.py
+-rw-r--r--   0        0        0     1310 2024-04-18 09:33:56.877413 tdf_tool-2.4.8/tdf_tool/tools/config/initial_json_config.py
+-rw-r--r--   0        0        0     1267 2024-04-18 09:33:56.877960 tdf_tool-2.4.8/tdf_tool/tools/config/module_json_config.py
+-rw-r--r--   0        0        0     5593 2024-04-16 07:59:17.964325 tdf_tool-2.4.8/tdf_tool/tools/config/packages_config.py
+-rw-r--r--   0        0        0     7704 2024-04-16 07:59:17.964588 tdf_tool-2.4.8/tdf_tool/tools/dependencies_analysis.py
+-rw-r--r--   0        0        0      776 2024-04-19 09:46:46.688382 tdf_tool-2.4.8/tdf_tool/tools/env.py
+-rw-r--r--   0        0        0     6312 2024-04-16 07:59:17.965341 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc
+-rw-r--r--   0        0        0     3616 2024-04-18 09:33:56.878578 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc
+-rw-r--r--   0        0        0     3174 2024-04-16 07:59:17.965839 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     2004 2024-04-18 09:33:56.879118 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc
+-rw-r--r--   0        0        0     4314 2024-04-16 07:59:17.966355 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     2464 2024-04-18 09:33:56.879669 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     6437 2024-04-16 07:59:17.966902 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     3681 2024-04-18 09:33:56.880258 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     2422 2024-04-16 07:59:17.967708 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     3345 2024-04-16 07:59:17.967959 tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_entry.py
+-rw-r--r--   0        0        0     1586 2024-04-16 07:59:17.968270 tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_lint.py
+-rw-r--r--   0        0        0     2137 2024-04-16 07:59:17.968589 tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_lint_tool.py
+-rw-r--r--   0        0        0     4095 2024-04-16 07:59:17.968850 tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_replace_tool.py
+-rw-r--r--   0        0        0     1159 2024-04-16 07:59:17.969195 tdf_tool-2.4.8/tdf_tool/tools/flutter_script.py
+-rw-r--r--   0        0        0      444 2024-04-19 09:59:03.824969 tdf_tool-2.4.8/tdf_tool/tools/generator.py
+-rw-r--r--   0        0        0     7243 2024-04-16 07:59:17.969845 tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc
+-rw-r--r--   0        0        0     4190 2024-04-18 09:33:56.880901 tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     7055 2024-04-16 07:59:17.970442 tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc
+-rw-r--r--   0        0        0     3786 2024-04-18 09:33:56.881487 tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc
+-rw-r--r--   0        0        0      593 2024-04-16 07:59:17.971051 tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc
+-rw-r--r--   0        0        0     5019 2024-04-16 07:59:17.971732 tdf_tool-2.4.8/tdf_tool/tools/gitlab/gitlab_utils.py
+-rw-r--r--   0        0        0     3814 2024-04-16 07:59:17.972085 tdf_tool-2.4.8/tdf_tool/tools/gitlab/python_gitlab_api.py
+-rw-r--r--   0        0        0     2482 2024-04-16 07:59:17.972678 tdf_tool-2.4.8/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     1412 2024-04-18 09:33:56.882138 tdf_tool-2.4.8/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     1063 2024-04-16 07:59:17.973603 tdf_tool-2.4.8/tdf_tool/tools/module/module_tools.py
+-rw-r--r--   0        0        0    11056 2024-04-16 07:59:17.974266 tdf_tool-2.4.8/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc
+-rw-r--r--   0        0        0     5267 2024-04-18 09:33:56.882719 tdf_tool-2.4.8/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     9752 2024-04-16 07:59:17.974933 tdf_tool-2.4.8/tdf_tool/tools/package/seal_off_package_utils.py
+-rw-r--r--   0        0        0      911 2024-04-16 07:59:17.975191 tdf_tool-2.4.8/tdf_tool/tools/platform_tools.py
+-rw-r--r--   0        0        0     1226 2024-04-19 09:43:13.615410 tdf_tool-2.4.8/tdf_tool/tools/print.py
+-rw-r--r--   0        0        0     7598 2024-04-16 07:59:17.975770 tdf_tool-2.4.8/tdf_tool/tools/regular_tool.py
+-rw-r--r--   0        0        0     5718 2024-04-18 09:33:56.883146 tdf_tool-2.4.8/tdf_tool/tools/shell_dir.py
+-rw-r--r--   0        0        0     3840 2024-04-16 07:59:17.976600 tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc
+-rw-r--r--   0        0        0     2161 2024-04-18 09:33:56.883746 tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc
+-rw-r--r--   0        0        0     2695 2024-04-16 07:59:17.977108 tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     1678 2024-04-18 09:33:56.884279 tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc
+-rw-r--r--   0        0        0    11711 2024-04-16 07:59:17.977716 tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     1999 2024-04-16 07:59:17.977961 tdf_tool-2.4.8/tdf_tool/tools/translate/file_util.py
+-rw-r--r--   0        0        0    15484 2024-04-16 07:59:17.978545 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     8285 2024-04-18 09:33:56.884733 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc
+-rw-r--r--   0        0        0    26818 2024-04-16 07:59:17.979344 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc
+-rw-r--r--   0        0        0    13427 2024-04-18 09:33:56.885241 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0    10691 2024-04-16 07:59:17.980114 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/flutter_translate_lint.py
+-rw-r--r--   0        0        0    18954 2024-04-16 07:59:17.980464 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/flutter_translate_tools.py
+-rw-r--r--   0        0        0     8395 2024-04-16 07:59:17.981075 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc
+-rw-r--r--   0        0        0     4595 2024-04-18 09:33:56.885795 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc
+-rw-r--r--   0        0        0     5228 2024-04-16 07:59:17.981648 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py
+-rw-r--r--   0        0        0      859 2024-04-16 07:59:17.982222 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc
+-rw-r--r--   0        0        0     7351 2024-04-16 07:59:17.982702 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc
+-rw-r--r--   0        0        0     7599 2024-04-16 07:59:17.983077 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc
+-rw-r--r--   0        0        0     4216 2024-04-18 09:33:56.886328 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc
+-rw-r--r--   0        0        0     3952 2024-04-16 07:59:17.983786 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     2347 2024-04-18 09:33:56.886740 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc
+-rw-r--r--   0        0        0      870 2024-04-16 07:59:17.984330 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc
+-rw-r--r--   0        0        0     4766 2024-04-16 07:59:17.984706 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     6219 2024-04-16 07:59:17.985086 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc
+-rw-r--r--   0        0        0     2631 2024-04-16 07:59:17.985435 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc
+-rw-r--r--   0        0        0     4438 2024-04-16 07:59:17.985774 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/ios_translate.py
+-rw-r--r--   0        0        0     2000 2024-04-16 07:59:17.986154 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/ios_translate_lint.py
+-rw-r--r--   0        0        0     5061 2024-04-16 07:59:17.986697 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     2852 2024-04-18 09:33:56.887291 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc
+-rw-r--r--   0        0        0    17576 2024-04-16 07:59:17.987402 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc
+-rw-r--r--   0        0        0     9306 2024-04-18 09:33:56.887836 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc
+-rw-r--r--   0        0        0     7901 2024-04-16 07:59:17.988120 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc
+-rw-r--r--   0        0        0     4398 2024-04-18 09:33:56.888413 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc
+-rw-r--r--   0        0        0     1158 2024-04-16 07:59:17.988695 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc
+-rw-r--r--   0        0        0     1028 2024-04-18 09:33:56.889038 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc
+-rw-r--r--   0        0        0    10070 2024-04-16 07:59:17.989363 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     5366 2024-04-18 09:33:56.889482 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     2773 2024-04-16 07:59:17.989983 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc
+-rw-r--r--   0        0        0     2689 2024-04-18 09:33:56.889936 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc
+-rw-r--r--   0        0        0    11353 2024-04-16 07:59:17.990542 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc
+-rw-r--r--   0        0        0     6226 2024-04-18 09:33:56.890414 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc
+-rw-r--r--   0        0        0     4943 2024-04-16 07:59:17.991277 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc
+-rw-r--r--   0        0        0     2687 2024-04-18 09:33:56.890983 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc
+-rw-r--r--   0        0        0     3270 2024-04-16 07:59:17.991799 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py
+-rw-r--r--   0        0        0    14326 2024-04-16 07:59:17.992093 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_module.py
+-rw-r--r--   0        0        0     5223 2024-04-16 07:59:17.992380 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py
+-rw-r--r--   0        0        0     1189 2024-04-16 07:59:17.992605 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py
+-rw-r--r--   0        0        0     8191 2024-04-16 07:59:17.992866 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py
+-rw-r--r--   0        0        0     2337 2024-04-16 07:59:17.993215 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/location_string_temp.py
+-rw-r--r--   0        0        0     8684 2024-04-16 07:59:17.993505 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/podspec.py
+-rw-r--r--   0        0        0     2886 2024-04-16 07:59:17.993759 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/string_util.py
+-rw-r--r--   0        0        0     8625 2024-04-16 07:59:17.994344 tdf_tool-2.4.8/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     5032 2024-04-18 09:33:56.891445 tdf_tool-2.4.8/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     5111 2024-04-16 07:59:17.994952 tdf_tool-2.4.8/tdf_tool/tools/translate/tools/translate_tool.py
+-rw-r--r--   0        0        0     1408 2024-04-16 07:59:17.995250 tdf_tool-2.4.8/tdf_tool/tools/translate/translate_lint.py
+-rw-r--r--   0        0        0     1268 2024-04-16 07:59:17.996782 tdf_tool-2.4.8/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc
+-rw-r--r--   0        0        0      880 2024-04-18 09:33:56.891894 tdf_tool-2.4.8/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc
+-rw-r--r--   0        0        0      440 2024-04-16 07:59:17.997353 tdf_tool-2.4.8/tdf_tool/tools/vscode/vscode.py
+-rw-r--r--   0        0        0    10568 1970-01-01 00:00:00.000000 tdf_tool-2.4.8/PKG-INFO
```

### Comparing `tdf_tool-2.4.7/LICENSE` & `tdf_tool-2.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/README.md` & `tdf_tool-2.4.8/README.md`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/pyproject.toml` & `tdf_tool-2.4.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 项目信息
 [tool.poetry]
 name = "tdf_tool"
-version = "2.4.7"
+version = "2.4.8"
 description = "二维火 flutter 脚手架工具"
 authors = ["Jian Xu <3386218996@qq.com>", "FanJiao Gai <gaijiaofan@2dfire.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://git.2dfire.net/app/flutter/tools/package_tools"
 repository = "https://git.2dfire.net/app/flutter/tools/package_tools.git"
 keywords = ["tdf", "tdf-tool", "tdf_tool"]
```

### Comparing `tdf_tool-2.4.7/tdf_tool/pipeline.py` & `tdf_tool-2.4.8/tdf_tool/pipeline.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 19 10:01:18 2024 UTC, .py size: 7845 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 ee40 2266 a51e 0000  a........@"f....
+00000000: 610d 0d0a 0000 0000 4629 2366 c61e 0000  a.......F)#f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6404 6c07  m.Z.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
@@ -119,368 +119,370 @@
 00000760: 0000 0200 0000 4300 0000 7342 0000 0064  ......C...sB...d
 00000770: 007c 005f 0064 017c 005f 0164 027c 005f  .|._.d.|._.d.|._
 00000780: 0267 007c 005f 0364 037c 005f 0467 007c  .g.|._.d.|._.g.|
 00000790: 005f 0564 047c 005f 0664 057c 005f 0767  ._.d.|._.d.|._.g
 000007a0: 007c 005f 087c 00a0 09a1 0001 0064 0053  .|._.|.......d.S
 000007b0: 0029 064e 5a16 4170 6941 6e6e 6f74 6174  .).NZ.ApiAnnotat
 000007c0: 696f 6e47 656e 6572 6174 6f72 7a0e 2e74  ionGeneratorz..t
-000007d0: 6466 5f69 6d70 6c2e 6461 7274 7a0d 2e74  df_impl.dartz..t
-000007e0: 6466 5f61 7069 2e64 6172 745a 0774 6466  df_api.dartZ.tdf
-000007f0: 5f61 7069 5a13 7464 665f 6d6f 6475 6c65  _apiZ.tdf_module
-00000800: 5f61 7069 5f61 6e6e 6f29 0ada 0266 66da  _api_anno)...ff.
-00000810: 195f 4170 6941 6e6e 6f74 6174 696f 6e5f  ._ApiAnnotation_
-00000820: 5f67 656e 6572 6174 6f72 da1a 5f41 7069  _generator.._Api
-00000830: 416e 6e6f 7461 7469 6f6e 5f5f 696d 706c  Annotation__impl
-00000840: 5375 6666 6978 da1c 5f41 7069 416e 6e6f  Suffix.._ApiAnno
-00000850: 7461 7469 6f6e 5f5f 696d 706c 4e6f 6465  tation__implNode
-00000860: 4c69 7374 da19 5f41 7069 416e 6e6f 7461  List.._ApiAnnota
-00000870: 7469 6f6e 5f5f 6170 6953 7566 6669 78da  tion__apiSuffix.
-00000880: 1b5f 4170 6941 6e6e 6f74 6174 696f 6e5f  ._ApiAnnotation_
-00000890: 5f61 7069 4e6f 6465 4c69 7374 da1e 5f41  _apiNodeList.._A
-000008a0: 7069 416e 6e6f 7461 7469 6f6e 5f5f 696e  piAnnotation__in
-000008b0: 7465 7261 6374 696f 6e44 6972 da1e 5f41  teractionDir.._A
-000008c0: 7069 416e 6e6f 7461 7469 6f6e 5f5f 616e  piAnnotation__an
-000008d0: 6e6f 7461 7469 6f6e 4e61 6d65 da1c 5f41  notationName.._A
-000008e0: 7069 416e 6e6f 7461 7469 6f6e 5f5f 7061  piAnnotation__pa
-000008f0: 636b 6167 6573 4c69 7374 da13 6665 7463  ckagesList..fetc
-00000900: 685f 7061 636b 6167 6573 5f6c 6973 7472  h_packages_listr
-00000910: 1000 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00000920: 0000 0072 1400 0000 2a00 0000 7314 0000  ...r....*...s...
-00000930: 0000 0106 0106 0106 0106 0106 0106 0106  ................
-00000940: 0106 0106 027a 1641 7069 416e 6e6f 7461  .....z.ApiAnnota
-00000950: 7469 6f6e 2e5f 5f69 6e69 745f 5f63 0100  tion.__init__c..
-00000960: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00000970: 0000 4300 0000 731c 0000 0074 00a0 01a1  ..C...s....t....
-00000980: 0001 0074 0274 03a0 04a1 0083 016a 057c  ...t.t.......j.|
-00000990: 005f 0664 0053 0029 014e 2907 7207 0000  ._.d.S.).N).r...
-000009a0: 00da 0c67 6f49 6e53 6865 6c6c 4469 7272  ...goInShellDirr
-000009b0: 0400 0000 da02 6f73 da06 6765 7463 7764  ......os..getcwd
-000009c0: da08 7061 636b 6167 6573 7231 0000 0072  ..packagesr1...r
-000009d0: 1000 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-000009e0: 0000 0072 3200 0000 3800 0000 7304 0000  ...r2...8...s...
-000009f0: 0000 0108 027a 2141 7069 416e 6e6f 7461  .....z!ApiAnnota
-00000a00: 7469 6f6e 2e66 6574 6368 5f70 6163 6b61  tion.fetch_packa
-00000a10: 6765 735f 6c69 7374 6301 0000 0000 0000  ges_listc.......
-00000a20: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
-00000a30: 0073 5000 0000 7c00 a000 a100 7d01 7401  .sP...|.....}.t.
-00000a40: 6a02 a003 7c01 6401 a102 7d02 7404 7c02  j...|.d...}.t.|.
-00000a50: 6402 8302 7c00 5f05 7c00 a006 a100 0100  d...|._.|.......
-00000a60: 7c00 a007 a100 0100 7c00 a008 a100 0100  |.......|.......
-00000a70: 7c00 6a05 a009 a100 0100 7c00 a00a a100  |.j.......|.....
-00000a80: 0100 6400 5300 2903 4e7a 1161 7069 5f72  ..d.S.).Nz.api_r
-00000a90: 6567 6973 7465 722e 6461 7274 7a02 772b  egister.dartz.w+
-00000aa0: 290b da13 6765 745f 696e 7465 7261 6374  )...get_interact
-00000ab0: 696f 6e5f 6469 7272 3400 0000 da04 7061  ion_dirr4.....pa
-00000ac0: 7468 da04 6a6f 696e da04 6f70 656e 7229  th..join..openr)
-00000ad0: 0000 00da 275f 4170 6941 6e6e 6f74 6174  ....'_ApiAnnotat
-00000ae0: 696f 6e5f 5f69 6e74 6567 7261 7465 5f74  ion__integrate_t
-00000af0: 6466 5f61 7069 5f66 696c 6573 da28 5f41  df_api_files.(_A
-00000b00: 7069 416e 6e6f 7461 7469 6f6e 5f5f 696e  piAnnotation__in
-00000b10: 7465 6772 6174 655f 7464 665f 696d 706c  tegrate_tdf_impl
-00000b20: 5f66 696c 6573 da26 5f41 7069 416e 6e6f  _files.&_ApiAnno
-00000b30: 7461 7469 6f6e 5f5f 6765 6e65 7261 7465  tation__generate
-00000b40: 5f72 6567 6973 7465 725f 636f 6465 da05  _register_code..
-00000b50: 636c 6f73 65da 0a5f 5f66 6f72 6d61 745f  close..__format_
-00000b60: 5f29 0372 1100 0000 5a0b 7464 665f 6170  _).r....Z.tdf_ap
-00000b70: 695f 6469 725a 1261 7574 6f5f 7265 6769  i_dirZ.auto_regi
-00000b80: 7374 6572 5f66 696c 6572 1200 0000 7212  ster_filer....r.
-00000b90: 0000 0072 1300 0000 da0f 696e 7465 6772  ...r......integr
-00000ba0: 6174 655f 7368 656c 6c3e 0000 0073 1000  ate_shell>...s..
-00000bb0: 0000 0002 0801 0e01 0c03 0803 0803 0802  ................
-00000bc0: 0a03 7a1d 4170 6941 6e6e 6f74 6174 696f  ..z.ApiAnnotatio
-00000bd0: 6e2e 696e 7465 6772 6174 655f 7368 656c  n.integrate_shel
-00000be0: 6c63 0100 0000 0000 0000 0000 0000 0300  lc..............
-00000bf0: 0000 0800 0000 4300 0000 739c 0000 007c  ......C...s....|
-00000c00: 006a 00a0 0174 02a0 037c 006a 04a1 01a1  .j...t...|.j....
-00000c10: 0101 007c 006a 0544 005d 1e7d 017c 00a0  ...|.j.D.].}.|..
-00000c20: 067c 006a 007c 016a 077c 016a 087c 01a0  .|.j.|.j.|.j.|..
-00000c30: 09a1 00a1 0401 0071 1a7c 006a 0a44 005d  .......q.|.j.D.]
-00000c40: 1e7d 017c 00a0 067c 006a 007c 016a 077c  .}.|...|.j.|.j.|
-00000c50: 016a 087c 01a0 0ba1 00a1 0401 0071 407c  .j.|.........q@|
-00000c60: 00a0 0c7c 006a 007c 006a 0d7c 006a 0d64  ...|.j.|.j.|.j.d
-00000c70: 0117 00a1 0301 0064 027d 027c 006a 00a0  .......d.}.|.j..
-00000c80: 017c 02a0 0e7c 00a0 0fa1 007c 00a0 10a1  .|...|.....|....
-00000c90: 00a1 02a1 0101 0064 0053 0029 034e 7a05  .......d.S.).Nz.
-00000ca0: 2e64 6172 7475 8e02 0000 0a20 2020 2020  .dartu.....     
-00000cb0: 2020 200a 2020 2020 2020 2020 636c 6173     .        clas
-00000cc0: 7320 5444 4641 7069 496d 706c 4175 746f  s TDFApiImplAuto
-00000cd0: 5265 6769 7374 6572 207b 7b0a 2020 2020  Register {{.    
-00000ce0: 2020 2020 2020 7374 6174 6963 204c 6973        static Lis
-00000cf0: 743c 5479 7065 3e20 6170 6973 203d 205b  t<Type> apis = [
-00000d00: 0a20 2020 2020 2020 2020 2020 207b 307d  .            {0}
-00000d10: 0a20 2020 2020 2020 2020 205d 3b0a 2020  .          ];.  
-00000d20: 2020 2020 2020 2020 2f2f 20e7 a1ae e4bf          // .....
-00000d30: 9de6 8980 e69c 89e8 a2ab e5bc 95e7 94a8  ................
-00000d40: e79a 8461 7069 e5ba 93e7 9a84 e5ae 9ee7  ...api..........
-00000d50: 8eb0 e7b1 bbe9 83bd e5b7 b2e6 b3a8 e586  ................
-00000d60: 8c0a 2020 2020 2020 2020 2020 7374 6174  ..          stat
-00000d70: 6963 2076 6f69 6420 5f65 6e73 7572 6541  ic void _ensureA
-00000d80: 7069 496d 706c 5265 6769 7374 6572 2829  piImplRegister()
-00000d90: 207b 7b0a 2020 2020 2020 2020 2020 2020   {{.            
-00000da0: 6170 6973 2e66 6f72 4561 6368 2828 656c  apis.forEach((el
-00000db0: 656d 656e 7429 207b 7b0a 2020 2020 2020  ement) {{.      
-00000dc0: 2020 2020 2020 2020 6966 2028 2141 7069          if (!Api
-00000dd0: 5265 6769 7374 6572 4365 6e74 6572 2e6b  RegisterCenter.k
-00000de0: 6579 732e 636f 6e74 6169 6e73 2865 6c65  eys.contains(ele
-00000df0: 6d65 6e74 2929 207b 7b0a 2020 2020 2020  ment)) {{.      
-00000e00: 2020 2020 2020 2020 2020 7468 726f 7720            throw 
-00000e10: 4578 6365 7074 696f 6e28 2224 7b7b 656c  Exception("${{el
-00000e20: 656d 656e 747d 7de7 9a84 e5ae 9ee7 8eb0  ement}}.........
-00000e30: e7b1 bbe6 9caa e69c aae6 b3a8 e586 8cef  ................
-00000e40: bc81 efbc 81ef bc81 e8af b7e5 88a0 e999  ................
-00000e50: a4e5 ba93 247b 7b65 6c65 6d65 6e74 7d7d  ....${{element}}
-00000e60: e79a 84e5 bc95 e794 a8e6 8896 e880 85e5  ................
-00000e70: bc95 e585 a5e5 ae9e e78e b0e7 b1bb 2229  ..............")
-00000e80: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00000e90: 7d7d 0a20 2020 2020 2020 2020 2020 207d  }}.            }
-00000ea0: 7d29 3b0a 2020 2020 2020 2020 2020 7d7d  });.          }}
-00000eb0: 0a0a 2020 2020 2020 2020 2020 7374 6174  ..          stat
-00000ec0: 6963 2076 6f69 6420 6175 746f 5265 6769  ic void autoRegi
-00000ed0: 7374 6572 2829 207b 7b0a 2020 2020 2020  ster() {{.      
-00000ee0: 2020 2020 2020 2020 7b31 7d0a 2020 2020          {1}.    
-00000ef0: 2020 2020 2020 2020 2020 5f65 6e73 7572            _ensur
-00000f00: 6541 7069 496d 706c 5265 6769 7374 6572  eApiImplRegister
-00000f10: 2829 3b0a 2020 2020 2020 2020 2020 7d7d  ();.          }}
-00000f20: 0a20 2020 2020 2020 207d 7d0a 2020 2020  .        }}.    
-00000f30: 2020 2020 2020 2020 2911 7229 0000 00da          ).r)....
-00000f40: 0577 7269 7465 7208 0000 005a 1064 6566  .writer....Z.def
-00000f50: 6175 6c74 5469 746c 6544 6573 6372 2a00  aultTitleDescr*.
-00000f60: 0000 722c 0000 00da 255f 4170 6941 6e6e  ..r,....%_ApiAnn
-00000f70: 6f74 6174 696f 6e5f 5f5f 5f69 6d70 6f72  otation____impor
-00000f80: 745f 6461 7461 5f63 7265 6174 6f72 720d  t_data_creatorr.
-00000f90: 0000 0072 0f00 0000 721c 0000 0072 2e00  ...r....r....r..
-00000fa0: 0000 7227 0000 00da 315f 4170 6941 6e6e  ..r'....1_ApiAnn
-00000fb0: 6f74 6174 696f 6e5f 5f69 6d70 6f72 745f  otation__import_
-00000fc0: 6461 7461 5f63 7265 6174 6f72 5f77 6974  data_creator_wit
-00000fd0: 686f 7574 5f61 6c69 6173 7230 0000 00da  hout_aliasr0....
-00000fe0: 0666 6f72 6d61 74da 1061 7069 5f6c 6973  .format..api_lis
-00000ff0: 745f 6372 6561 746f 72da 255f 4170 6941  t_creator.%_ApiA
-00001000: 6e6e 6f74 6174 696f 6e5f 5f72 6567 6973  nnotation__regis
-00001010: 7465 725f 6c69 7374 5f63 7265 6174 6f72  ter_list_creator
-00001020: 2903 7211 0000 005a 055f 6974 656d da07  ).r....Z._item..
-00001030: 636f 6e74 656e 7472 1200 0000 7212 0000  contentr....r...
-00001040: 0072 1300 0000 5a18 5f5f 6765 6e65 7261  .r....Z.__genera
-00001050: 7465 5f72 6567 6973 7465 725f 636f 6465  te_register_code
-00001060: 5200 0000 731a 0000 0000 0114 020a 011c  R...s...........
-00001070: 010a 011c 0218 0204 1506 0104 0106 0106  ................
-00001080: fe02 ff7a 2641 7069 416e 6e6f 7461 7469  ...z&ApiAnnotati
-00001090: 6f6e 2e5f 5f67 656e 6572 6174 655f 7265  on.__generate_re
-000010a0: 6769 7374 6572 5f63 6f64 6563 0100 0000  gister_codec....
-000010b0: 0000 0000 0000 0000 0300 0000 0700 0000  ................
-000010c0: 4300 0000 732c 0000 0064 017d 017c 006a  C...s,...d.}.|.j
-000010d0: 0044 005d 1c7d 027c 0164 02a0 017c 02a0  .D.].}.|.d...|..
-000010e0: 02a1 007c 02a0 02a1 00a1 0237 007d 0171  ...|.......7.}.q
-000010f0: 0a7c 0153 0029 034e 720b 0000 007a 690a  .|.S.).Nr....zi.
-00001100: 2020 2020 2020 2020 2020 2020 4170 6952              ApiR
-00001110: 6567 6973 7465 7243 656e 7465 722e 7265  egisterCenter.re
-00001120: 6769 7374 6572 287b 307d 2e41 7574 6f52  gister({0}.AutoR
-00001130: 6567 6973 7465 722e 6170 6954 7970 652c  egister.apiType,
-00001140: 7b31 7d2e 4175 746f 5265 6769 7374 6572  {1}.AutoRegister
-00001150: 2e70 726f 7669 6465 7229 3b0a 2020 2020  .provider);.    
-00001160: 2020 2020 2020 2020 2903 722c 0000 0072          ).r,...r
-00001170: 4400 0000 721c 0000 00a9 0372 1100 0000  D...r......r....
-00001180: 7247 0000 00da 0469 7465 6d72 1200 0000  rG.....itemr....
-00001190: 7212 0000 0072 1300 0000 5a17 5f5f 7265  r....r....Z.__re
-000011a0: 6769 7374 6572 5f6c 6973 745f 6372 6561  gister_list_crea
-000011b0: 746f 7276 0000 0073 0c00 0000 0001 0401  torv...s........
-000011c0: 0a01 0602 0cfe 0803 7a25 4170 6941 6e6e  ........z%ApiAnn
-000011d0: 6f74 6174 696f 6e2e 5f5f 7265 6769 7374  otation.__regist
-000011e0: 6572 5f6c 6973 745f 6372 6561 746f 7263  er_list_creatorc
-000011f0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00001200: 0600 0000 4300 0000 7326 0000 0064 017d  ....C...s&...d.}
-00001210: 017c 006a 0044 005d 167d 027c 0164 02a0  .|.j.D.].}.|.d..
-00001220: 017c 02a0 02a1 00a1 0137 007d 0171 0a7c  .|.......7.}.q.|
-00001230: 0153 0029 034e 720b 0000 007a 430a 2020  .S.).Nr....zC.  
-00001240: 2020 2020 2020 2020 2020 7b30 7d2e 5444            {0}.TD
-00001250: 4641 7069 4175 746f 496e 7661 6c69 6461  FApiAutoInvalida
-00001260: 7465 2e61 7069 5479 7065 2c0a 2020 2020  te.apiType,.    
-00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001280: 2903 722e 0000 0072 4400 0000 7227 0000  ).r....rD...r'..
-00001290: 0072 4800 0000 7212 0000 0072 1200 0000  .rH...r....r....
-000012a0: 7213 0000 0072 4500 0000 7e00 0000 730c  r....rE...~...s.
-000012b0: 0000 0000 0104 010a 0106 0206 fe08 037a  ...............z
-000012c0: 1e41 7069 416e 6e6f 7461 7469 6f6e 2e61  .ApiAnnotation.a
-000012d0: 7069 5f6c 6973 745f 6372 6561 746f 7263  pi_list_creatorc
-000012e0: 0100 0000 0000 0000 0000 0000 0400 0000  ................
-000012f0: 0500 0000 4300 0000 7362 0000 0074 00a0  ....C...sb...t..
-00001300: 0164 01a1 0101 007c 006a 0244 005d 4c7d  .d.....|.j.D.]L}
-00001310: 017c 00a0 037c 016a 047c 006a 05a1 027d  .|...|.j.|.j...}
-00001320: 027c 0264 0075 0172 1074 0683 007d 037c  .|.d.u.r.t...}.|
-00001330: 016a 047c 035f 047c 016a 077c 035f 077c  .j.|._.|.j.|._.|
-00001340: 027c 035f 087c 03a0 09a1 0001 007c 006a  .|._.|.......|.j
-00001350: 0aa0 0b7c 03a1 0101 0071 1064 0053 0029  ...|.....q.d.S.)
-00001360: 024e 751c 0000 00e6 95b4 e590 88e6 8980  .Nu.............
-00001370: e69c 89e4 baa4 e4ba 9269 6d70 6ce6 9687  .........impl...
-00001380: e4bb b629 0c72 0600 0000 da05 7469 746c  ...).r......titl
-00001390: 6572 3100 0000 da1f 5f41 7069 416e 6e6f  er1....._ApiAnno
-000013a0: 7461 7469 6f6e 5f5f 6765 745f 7461 7267  tation__get_targ
-000013b0: 6574 5f66 696c 6572 0e00 0000 722b 0000  et_filer....r+..
-000013c0: 0072 0900 0000 720d 0000 0072 0f00 0000  .r....r....r....
-000013d0: 7221 0000 0072 2c00 0000 da06 6170 7065  r!...r,.....appe
-000013e0: 6e64 2904 7211 0000 00da 0b70 6163 6b61  nd).r......packa
-000013f0: 6765 4974 656d da19 5f41 7069 416e 6e6f  geItem.._ApiAnno
-00001400: 7461 7469 6f6e 5f5f 6669 6c65 5f70 6174  tation__file_pat
-00001410: 685a 095f 696d 706c 4e6f 6465 7212 0000  hZ._implNoder...
-00001420: 0072 1200 0000 7213 0000 005a 1a5f 5f69  .r....r....Z.__i
-00001430: 6e74 6567 7261 7465 5f74 6466 5f69 6d70  ntegrate_tdf_imp
-00001440: 6c5f 6669 6c65 7386 0000 0073 1400 0000  l_files....s....
-00001450: 0001 0a01 0a01 1001 0801 0601 0801 0801  ................
-00001460: 0601 0801 7a28 4170 6941 6e6e 6f74 6174  ....z(ApiAnnotat
-00001470: 696f 6e2e 5f5f 696e 7465 6772 6174 655f  ion.__integrate_
-00001480: 7464 665f 696d 706c 5f66 696c 6573 6301  tdf_impl_filesc.
-00001490: 0000 0000 0000 0000 0000 0004 0000 0005  ................
-000014a0: 0000 0043 0000 0073 6200 0000 7400 a001  ...C...sb...t...
-000014b0: 6401 a101 0100 7c00 6a02 4400 5d4c 7d01  d.....|.j.D.]L}.
-000014c0: 7c00 a003 7c01 6a04 7c00 6a05 a102 7d02  |...|.j.|.j...}.
-000014d0: 7c02 6400 7501 7210 7406 8300 7d03 7c01  |.d.u.r.t...}.|.
-000014e0: 6a04 7c03 5f04 7c01 6a07 7c03 5f07 7c02  j.|._.|.j.|._.|.
-000014f0: 7c03 5f08 7c03 a009 a100 0100 7c00 6a0a  |._.|.......|.j.
-00001500: a00b 7c03 a101 0100 7110 6400 5300 2902  ..|.....q.d.S.).
-00001510: 4e75 1b00 0000 e695 b4e5 9088 e689 80e6  Nu..............
-00001520: 9c89 e4ba a4e4 ba92 6170 69e6 9687 e4bb  ........api.....
-00001530: b629 0c72 0600 0000 724a 0000 0072 3100  .).r....rJ...r1.
-00001540: 0000 724b 0000 0072 0e00 0000 722d 0000  ..rK...r....r-..
-00001550: 0072 2600 0000 720d 0000 0072 0f00 0000  .r&...r....r....
-00001560: 7221 0000 0072 2e00 0000 724c 0000 0029  r!...r....rL...)
-00001570: 0472 1100 0000 724d 0000 0072 4e00 0000  .r....rM...rN...
-00001580: 5a08 5f61 7069 4e6f 6465 7212 0000 0072  Z._apiNoder....r
-00001590: 1200 0000 7213 0000 005a 195f 5f69 6e74  ....r....Z.__int
-000015a0: 6567 7261 7465 5f74 6466 5f61 7069 5f66  egrate_tdf_api_f
-000015b0: 696c 6573 9200 0000 7314 0000 0000 010a  iles....s.......
-000015c0: 010a 0110 0108 0106 0108 0108 0106 0108  ................
-000015d0: 017a 2741 7069 416e 6e6f 7461 7469 6f6e  .z'ApiAnnotation
-000015e0: 2e5f 5f69 6e74 6567 7261 7465 5f74 6466  .__integrate_tdf
-000015f0: 5f61 7069 5f66 696c 6573 2903 da09 6669  _api_files)...fi
-00001600: 6c65 5f70 6174 68da 0673 7566 6669 7872  le_path..suffixr
-00001610: 1600 0000 6303 0000 0000 0000 0000 0000  ....c...........
-00001620: 000c 0000 0006 0000 0043 0000 0073 ce00  .........C...s..
-00001630: 0000 7400 a001 a100 0100 7402 a003 7c01  ..t.......t...|.
-00001640: a101 0100 6401 7d03 7402 a004 7405 a006  ....d.}.t...t...
-00001650: a100 a101 a007 a100 a008 6402 a101 6401  ..........d...d.
-00001660: 1900 7d04 7402 a009 7c04 a101 4400 5d66  ..}.t...|...D.]f
-00001670: 5c03 7d05 7d06 7d07 7c07 4400 5d56 7d08  \.}.}.}.|.D.]V}.
-00001680: 7402 6a0a a00b 7c05 7c08 a102 7d09 7c09  t.j...|.|...}.|.
-00001690: a00c 7c02 a101 724a 7c03 6403 3700 7d03  ..|...rJ|.d.7.}.
-000016a0: 7405 a00d a100 7292 7c09 a008 6404 a101  t.....r.|...d...
-000016b0: 6403 1900 7d0a 7c0a a00e 6405 6406 a102  d...}.|...d.d...
-000016c0: 7d0b 714a 7c09 a008 6407 a101 6403 1900  }.qJ|...d...d...
-000016d0: 7d0b 714a 713c 7c03 6403 6b02 72b0 7c0b  }.qJq<|.d.k.r.|.
-000016e0: 5300 7c03 6403 6b04 72ca 740f 6408 a010  S.|.d.k.r.t.d...
-000016f0: 7c01 a101 8301 8201 6400 5300 6400 5300  |.......d.S.d.S.
-00001700: 2909 4e72 0100 0000 da01 0ae9 0100 0000  ).Nr............
-00001710: 7a05 5c6c 6962 5cfa 015c 721e 0000 007a  z.\lib\..\r....z
-00001720: 052f 6c69 622f 7530 0000 00e6 a8a1 e59d  ./lib/u0........
-00001730: 977b 307d e5ad 98e5 9ca8 e5a4 9ae4 b8aa  .{0}............
-00001740: e4ba a4e4 ba92 e696 87e4 bbb6 efbc 8ce8  ................
-00001750: afb7 e6a3 80e6 9fa5 e29d 8c29 1172 0700  ...........).r..
-00001760: 0000 7233 0000 0072 3400 0000 da05 6368  ..r3...r4.....ch
-00001770: 6469 72da 0570 6f70 656e 7205 0000 00da  dir..popenr.....
-00001780: 0770 7764 5f63 6d64 da04 7265 6164 da05  .pwd_cmd..read..
-00001790: 7370 6c69 74da 0477 616c 6b72 3800 0000  split..walkr8...
-000017a0: 7239 0000 00da 0865 6e64 7377 6974 68da  r9.....endswith.
-000017b0: 0a69 735f 7769 6e64 6f77 73da 0772 6570  .is_windows..rep
-000017c0: 6c61 6365 da09 4578 6365 7074 696f 6e72  lace..Exceptionr
-000017d0: 4400 0000 290c 7211 0000 0072 4f00 0000  D...).r....rO...
-000017e0: 7250 0000 00da 0563 6f75 6e74 da08 6e6f  rP.....count..no
-000017f0: 7761 5061 7468 da04 726f 6f74 da04 6469  waPath..root..di
-00001800: 7273 da05 6669 6c65 73da 0466 696c 65da  rs..files..file.
-00001810: 0873 7263 5f66 696c 65da 0474 656d 705a  .src_file..tempZ
-00001820: 1b5f 4170 6941 6e6e 6f74 6174 696f 6e5f  ._ApiAnnotation_
-00001830: 5f74 6172 6765 745f 6669 6c65 7212 0000  _target_filer...
-00001840: 0072 1200 0000 7213 0000 005a 115f 5f67  .r....r....Z.__g
-00001850: 6574 5f74 6172 6765 745f 6669 6c65 9f00  et_target_file..
-00001860: 0000 7326 0000 0000 0108 010a 0204 021c  ..s&............
-00001870: 0114 0108 010e 010a 0108 0108 010e 010e  ................
-00001880: 0212 0108 0104 0108 010e 0104 017a 1f41  .............z.A
-00001890: 7069 416e 6e6f 7461 7469 6f6e 2e5f 5f67  piAnnotation.__g
-000018a0: 6574 5f74 6172 6765 745f 6669 6c65 6301  et_target_filec.
-000018b0: 0000 0000 0000 0000 0000 0001 0000 0005  ................
-000018c0: 0000 0043 0000 0073 4e00 0000 7400 a001  ...C...sN...t...
-000018d0: a100 0100 7402 a003 6401 a101 0100 7402  ....t...d.....t.
-000018e0: 6a04 a005 7c00 6a06 a101 722c 7407 a008  j...|.j...r,t...
-000018f0: 7c00 6a06 a101 0100 7402 a009 7c00 6a06  |.j.....t...|.j.
-00001900: a101 0100 7402 6a04 a00a 7400 a00b a100  ....t.j...t.....
-00001910: 6401 7c00 6a06 a103 5300 2902 4eda 036c  d.|.j...S.).N..l
-00001920: 6962 290c 7207 0000 0072 3300 0000 7234  ib).r....r3...r4
-00001930: 0000 0072 5400 0000 7238 0000 00da 0665  ...rT...r8.....e
-00001940: 7869 7374 7372 2f00 0000 da06 7368 7574  xistsr/.....shut
-00001950: 696c da06 726d 7472 6565 da05 6d6b 6469  il..rmtree..mkdi
-00001960: 7272 3900 0000 da0b 6765 7453 6865 6c6c  rr9.....getShell
-00001970: 4469 7272 1000 0000 7212 0000 0072 1200  Dirr....r....r..
-00001980: 0000 7213 0000 0072 3700 0000 b700 0000  ..r....r7.......
-00001990: 730c 0000 0000 0108 010a 010e 010c 010c  s...............
-000019a0: 017a 2141 7069 416e 6e6f 7461 7469 6f6e  .z!ApiAnnotation
-000019b0: 2e67 6574 5f69 6e74 6572 6163 7469 6f6e  .get_interaction
-000019c0: 5f64 6972 6301 0000 0000 0000 0000 0000  _dirc...........
-000019d0: 0002 0000 0005 0000 0043 0000 0073 3200  .........C...s2.
-000019e0: 0000 7400 a001 a100 0100 7402 6a03 a004  ..t.......t.j...
-000019f0: 7400 a005 a100 6401 7c00 6a06 a103 7d01  t.....d.|.j...}.
-00001a00: 7402 a007 6402 a008 7c01 a101 a101 0100  t...d...|.......
-00001a10: 6400 5300 2903 4e72 6600 0000 7a0f 6461  d.S.).Nrf...z.da
-00001a20: 7274 2066 6f72 6d61 7420 7b30 7d29 0972  rt format {0}).r
-00001a30: 0700 0000 da0f 676f 496e 5368 656c 6c4c  ......goInShellL
-00001a40: 6962 4469 7272 3400 0000 7238 0000 0072  ibDirr4...r8...r
-00001a50: 3900 0000 726b 0000 0072 2f00 0000 da06  9...rk...r/.....
-00001a60: 7379 7374 656d 7244 0000 0029 0272 1100  systemrD...).r..
-00001a70: 0000 5a14 5f41 7069 416e 6e6f 7461 7469  ..Z._ApiAnnotati
-00001a80: 6f6e 5f5f 7061 7468 7212 0000 0072 1200  on__pathr....r..
-00001a90: 0000 7213 0000 0072 3f00 0000 c000 0000  ..r....r?.......
-00001aa0: 7306 0000 0000 0108 0116 017a 1841 7069  s..........z.Api
-00001ab0: 416e 6e6f 7461 7469 6f6e 2e5f 5f66 6f72  Annotation.__for
-00001ac0: 6d61 745f 5f63 0500 0000 0000 0000 0000  mat__c..........
-00001ad0: 0000 0500 0000 0700 0000 4300 0000 7318  ..........C...s.
-00001ae0: 0000 007c 01a0 0064 01a0 017c 027c 037c  ...|...d...|.|.|
-00001af0: 04a1 03a1 0101 0064 0053 0029 024e 7a21  .......d.S.).Nz!
-00001b00: 696d 706f 7274 2022 7061 636b 6167 653a  import "package:
-00001b10: 7b30 7d2f 7b31 7d22 2061 7320 7b32 7d3b  {0}/{1}" as {2};
-00001b20: 0aa9 0272 4100 0000 7244 0000 0029 0572  ...rA...rD...).r
-00001b30: 1100 0000 da07 665f 7772 6974 65da 0b6d  ......f_write..m
-00001b40: 6f64 756c 655f 6e61 6d65 724f 0000 00da  odule_namerO....
-00001b50: 0561 6c69 6173 7212 0000 0072 1200 0000  .aliasr....r....
-00001b60: 7213 0000 005a 175f 5f5f 5f69 6d70 6f72  r....Z.____impor
-00001b70: 745f 6461 7461 5f63 7265 6174 6f72 c600  t_data_creator..
-00001b80: 0000 730a 0000 0000 0304 0104 0106 ff02  ..s.............
-00001b90: ff7a 2541 7069 416e 6e6f 7461 7469 6f6e  .z%ApiAnnotation
-00001ba0: 2e5f 5f5f 5f69 6d70 6f72 745f 6461 7461  .____import_data
-00001bb0: 5f63 7265 6174 6f72 6304 0000 0000 0000  _creatorc.......
-00001bc0: 0000 0000 0004 0000 0006 0000 0043 0000  .............C..
-00001bd0: 0073 1600 0000 7c01 a000 6401 a001 7c02  .s....|...d...|.
-00001be0: 7c03 a102 a101 0100 6400 5300 2902 4e7a  |.......d.S.).Nz
-00001bf0: 1a69 6d70 6f72 7420 2270 6163 6b61 6765  .import "package
-00001c00: 3a7b 307d 2f7b 317d 223b 0a72 6e00 0000  :{0}/{1}";.rn...
-00001c10: 2904 7211 0000 0072 6f00 0000 7270 0000  ).r....ro...rp..
-00001c20: 0072 4f00 0000 7212 0000 0072 1200 0000  .rO...r....r....
-00001c30: 7213 0000 005a 235f 5f69 6d70 6f72 745f  r....Z#__import_
-00001c40: 6461 7461 5f63 7265 6174 6f72 5f77 6974  data_creator_wit
-00001c50: 686f 7574 5f61 6c69 6173 d000 0000 730a  hout_alias....s.
-00001c60: 0000 0000 0304 0104 0104 ff02 ff7a 3141  .............z1A
-00001c70: 7069 416e 6e6f 7461 7469 6f6e 2e5f 5f69  piAnnotation.__i
-00001c80: 6d70 6f72 745f 6461 7461 5f63 7265 6174  mport_data_creat
-00001c90: 6f72 5f77 6974 686f 7574 5f61 6c69 6173  or_without_alias
-00001ca0: 4e29 1272 2200 0000 7223 0000 0072 2400  N).r"...r#...r$.
-00001cb0: 0000 da07 5f5f 646f 635f 5f72 1400 0000  ....__doc__r....
-00001cc0: 7232 0000 0072 4000 0000 723d 0000 0072  r2...r@...r=...r
-00001cd0: 4600 0000 7245 0000 0072 3c00 0000 723b  F...rE...r<...r;
-00001ce0: 0000 0072 2500 0000 724b 0000 0072 3700  ...r%...rK...r7.
-00001cf0: 0000 723f 0000 0072 4200 0000 7243 0000  ..r?...rB...rC..
-00001d00: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
-00001d10: 7213 0000 0072 2800 0000 2500 0000 731c  r....r(...%...s.
-00001d20: 0000 0008 0104 0408 0e08 0608 1408 2408  ..............$.
-00001d30: 0808 0808 0c08 0d12 1808 0908 0608 0a72  ...............r
-00001d40: 2800 0000 2912 da07 6861 7368 6c69 6272  (...)...hashlibr
-00001d50: 0200 0000 7234 0000 0072 6800 0000 da25  ....r4...rh....%
-00001d60: 7464 665f 746f 6f6c 2e74 6f6f 6c73 2e63  tdf_tool.tools.c
-00001d70: 6f6e 6669 672e 7061 636b 6167 6573 5f63  onfig.packages_c
-00001d80: 6f6e 6669 6772 0300 0000 7204 0000 00da  onfigr....r.....
-00001d90: 1d74 6466 5f74 6f6f 6c2e 746f 6f6c 732e  .tdf_tool.tools.
-00001da0: 706c 6174 666f 726d 5f74 6f6f 6c73 7205  platform_toolsr.
-00001db0: 0000 00da 1474 6466 5f74 6f6f 6c2e 746f  .....tdf_tool.to
-00001dc0: 6f6c 732e 7072 696e 7472 0600 0000 da18  ols.printr......
-00001dd0: 7464 665f 746f 6f6c 2e74 6f6f 6c73 2e73  tdf_tool.tools.s
-00001de0: 6865 6c6c 5f64 6972 7207 0000 005a 1874  hell_dirr....Z.t
-00001df0: 6466 5f74 6f6f 6c2e 746f 6f6c 732e 6765  df_tool.tools.ge
-00001e00: 6e65 7261 746f 7272 0800 0000 7209 0000  neratorr....r...
-00001e10: 0072 2600 0000 7228 0000 0072 1200 0000  .r&...r(...r....
-00001e20: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00001e30: 083c 6d6f 6475 6c65 3e01 0000 0073 1400  .<module>....s..
-00001e40: 0000 0c01 0801 0801 1001 0c01 0c01 0c01  ................
-00001e50: 0c03 0e0d 0e0d                           ......
+000007d0: 6466 5f69 6d70 6c2e 6461 7274 7a1a 2e74  df_impl.dartz..t
+000007e0: 6466 5f6d 6f64 756c 655f 696e 7465 7266  df_module_interf
+000007f0: 6163 652e 6461 7274 5a0f 7464 665f 696e  ace.dartZ.tdf_in
+00000800: 7465 7261 6374 696f 6e5a 1374 6466 5f6d  teractionZ.tdf_m
+00000810: 6f64 756c 655f 6170 695f 616e 6e6f 290a  odule_api_anno).
+00000820: da02 6666 da19 5f41 7069 416e 6e6f 7461  ..ff.._ApiAnnota
+00000830: 7469 6f6e 5f5f 6765 6e65 7261 746f 72da  tion__generator.
+00000840: 1a5f 4170 6941 6e6e 6f74 6174 696f 6e5f  ._ApiAnnotation_
+00000850: 5f69 6d70 6c53 7566 6669 78da 1c5f 4170  _implSuffix.._Ap
+00000860: 6941 6e6e 6f74 6174 696f 6e5f 5f69 6d70  iAnnotation__imp
+00000870: 6c4e 6f64 654c 6973 74da 195f 4170 6941  lNodeList.._ApiA
+00000880: 6e6e 6f74 6174 696f 6e5f 5f61 7069 5375  nnotation__apiSu
+00000890: 6666 6978 da1b 5f41 7069 416e 6e6f 7461  ffix.._ApiAnnota
+000008a0: 7469 6f6e 5f5f 6170 694e 6f64 654c 6973  tion__apiNodeLis
+000008b0: 74da 1e5f 4170 6941 6e6e 6f74 6174 696f  t.._ApiAnnotatio
+000008c0: 6e5f 5f69 6e74 6572 6163 7469 6f6e 4469  n__interactionDi
+000008d0: 72da 1e5f 4170 6941 6e6e 6f74 6174 696f  r.._ApiAnnotatio
+000008e0: 6e5f 5f61 6e6e 6f74 6174 696f 6e4e 616d  n__annotationNam
+000008f0: 65da 1c5f 4170 6941 6e6e 6f74 6174 696f  e.._ApiAnnotatio
+00000900: 6e5f 5f70 6163 6b61 6765 734c 6973 74da  n__packagesList.
+00000910: 1366 6574 6368 5f70 6163 6b61 6765 735f  .fetch_packages_
+00000920: 6c69 7374 7210 0000 0072 1200 0000 7212  listr....r....r.
+00000930: 0000 0072 1300 0000 7214 0000 002a 0000  ...r....r....*..
+00000940: 0073 1400 0000 0001 0601 0601 0601 0601  .s..............
+00000950: 0601 0601 0601 0601 0602 7a16 4170 6941  ..........z.ApiA
+00000960: 6e6e 6f74 6174 696f 6e2e 5f5f 696e 6974  nnotation.__init
+00000970: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
+00000980: 0000 0003 0000 0043 0000 0073 1c00 0000  .......C...s....
+00000990: 7400 a001 a100 0100 7402 7403 a004 a100  t.......t.t.....
+000009a0: 8301 6a05 7c00 5f06 6400 5300 2901 4e29  ..j.|._.d.S.).N)
+000009b0: 0772 0700 0000 da0c 676f 496e 5368 656c  .r......goInShel
+000009c0: 6c44 6972 7204 0000 00da 026f 73da 0667  lDirr......os..g
+000009d0: 6574 6377 64da 0870 6163 6b61 6765 7372  etcwd..packagesr
+000009e0: 3100 0000 7210 0000 0072 1200 0000 7212  1...r....r....r.
+000009f0: 0000 0072 1300 0000 7232 0000 0038 0000  ...r....r2...8..
+00000a00: 0073 0400 0000 0001 0802 7a21 4170 6941  .s........z!ApiA
+00000a10: 6e6e 6f74 6174 696f 6e2e 6665 7463 685f  nnotation.fetch_
+00000a20: 7061 636b 6167 6573 5f6c 6973 7463 0100  packages_listc..
+00000a30: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00000a40: 0000 4300 0000 7350 0000 007c 00a0 00a1  ..C...sP...|....
+00000a50: 007d 0174 016a 02a0 037c 0164 01a1 027d  .}.t.j...|.d...}
+00000a60: 0274 047c 0264 0283 027c 005f 057c 00a0  .t.|.d...|._.|..
+00000a70: 06a1 0001 007c 00a0 07a1 0001 007c 00a0  .....|.......|..
+00000a80: 08a1 0001 007c 006a 05a0 09a1 0001 007c  .....|.j.......|
+00000a90: 00a0 0aa1 0001 0064 0053 0029 034e 7a11  .......d.S.).Nz.
+00000aa0: 6170 695f 7265 6769 7374 6572 2e64 6172  api_register.dar
+00000ab0: 747a 0277 2b29 0bda 1367 6574 5f69 6e74  tz.w+)...get_int
+00000ac0: 6572 6163 7469 6f6e 5f64 6972 7234 0000  eraction_dirr4..
+00000ad0: 00da 0470 6174 68da 046a 6f69 6eda 046f  ...path..join..o
+00000ae0: 7065 6e72 2900 0000 da27 5f41 7069 416e  penr)....'_ApiAn
+00000af0: 6e6f 7461 7469 6f6e 5f5f 696e 7465 6772  notation__integr
+00000b00: 6174 655f 7464 665f 6170 695f 6669 6c65  ate_tdf_api_file
+00000b10: 73da 285f 4170 6941 6e6e 6f74 6174 696f  s.(_ApiAnnotatio
+00000b20: 6e5f 5f69 6e74 6567 7261 7465 5f74 6466  n__integrate_tdf
+00000b30: 5f69 6d70 6c5f 6669 6c65 73da 265f 4170  _impl_files.&_Ap
+00000b40: 6941 6e6e 6f74 6174 696f 6e5f 5f67 656e  iAnnotation__gen
+00000b50: 6572 6174 655f 7265 6769 7374 6572 5f63  erate_register_c
+00000b60: 6f64 65da 0563 6c6f 7365 da0a 5f5f 666f  ode..close..__fo
+00000b70: 726d 6174 5f5f 2903 7211 0000 005a 0b74  rmat__).r....Z.t
+00000b80: 6466 5f61 7069 5f64 6972 5a12 6175 746f  df_api_dirZ.auto
+00000b90: 5f72 6567 6973 7465 725f 6669 6c65 7212  _register_filer.
+00000ba0: 0000 0072 1200 0000 7213 0000 00da 0f69  ...r....r......i
+00000bb0: 6e74 6567 7261 7465 5f73 6865 6c6c 3e00  ntegrate_shell>.
+00000bc0: 0000 7310 0000 0000 0208 010e 010c 0308  ..s.............
+00000bd0: 0308 0308 020a 037a 1d41 7069 416e 6e6f  .......z.ApiAnno
+00000be0: 7461 7469 6f6e 2e69 6e74 6567 7261 7465  tation.integrate
+00000bf0: 5f73 6865 6c6c 6301 0000 0000 0000 0000  _shellc.........
+00000c00: 0000 0003 0000 0008 0000 0043 0000 0073  ...........C...s
+00000c10: 9c00 0000 7c00 6a00 a001 7402 a003 7c00  ....|.j...t...|.
+00000c20: 6a04 a101 a101 0100 7c00 6a05 4400 5d1e  j.......|.j.D.].
+00000c30: 7d01 7c00 a006 7c00 6a00 7c01 6a07 7c01  }.|...|.j.|.j.|.
+00000c40: 6a08 7c01 a009 a100 a104 0100 711a 7c00  j.|.........q.|.
+00000c50: 6a0a 4400 5d1e 7d01 7c00 a006 7c00 6a00  j.D.].}.|...|.j.
+00000c60: 7c01 6a07 7c01 6a08 7c01 a00b a100 a104  |.j.|.j.|.......
+00000c70: 0100 7140 7c00 a00c 7c00 6a00 7c00 6a0d  ..q@|...|.j.|.j.
+00000c80: 7c00 6a0d 6401 1700 a103 0100 6402 7d02  |.j.d.......d.}.
+00000c90: 7c00 6a00 a001 7c02 a00e 7c00 a00f a100  |.j...|...|.....
+00000ca0: 7c00 a010 a100 a102 a101 0100 6400 5300  |...........d.S.
+00000cb0: 2903 4e7a 052e 6461 7274 758e 0200 000a  ).Nz..dartu.....
+00000cc0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000cd0: 2063 6c61 7373 2054 4446 4170 6949 6d70   class TDFApiImp
+00000ce0: 6c41 7574 6f52 6567 6973 7465 7220 7b7b  lAutoRegister {{
+00000cf0: 0a20 2020 2020 2020 2020 2073 7461 7469  .          stati
+00000d00: 6320 4c69 7374 3c54 7970 653e 2061 7069  c List<Type> api
+00000d10: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
+00000d20: 2020 7b30 7d0a 2020 2020 2020 2020 2020    {0}.          
+00000d30: 5d3b 0a20 2020 2020 2020 2020 202f 2f20  ];.          // 
+00000d40: e7a1 aee4 bf9d e689 80e6 9c89 e8a2 abe5  ................
+00000d50: bc95 e794 a8e7 9a84 6170 69e5 ba93 e79a  ........api.....
+00000d60: 84e5 ae9e e78e b0e7 b1bb e983 bde5 b7b2  ................
+00000d70: e6b3 a8e5 868c 0a20 2020 2020 2020 2020  .......         
+00000d80: 2073 7461 7469 6320 766f 6964 205f 656e   static void _en
+00000d90: 7375 7265 4170 6949 6d70 6c52 6567 6973  sureApiImplRegis
+00000da0: 7465 7228 2920 7b7b 0a20 2020 2020 2020  ter() {{.       
+00000db0: 2020 2020 2061 7069 732e 666f 7245 6163       apis.forEac
+00000dc0: 6828 2865 6c65 6d65 6e74 2920 7b7b 0a20  h((element) {{. 
+00000dd0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00000de0: 2821 4170 6952 6567 6973 7465 7243 656e  (!ApiRegisterCen
+00000df0: 7465 722e 6b65 7973 2e63 6f6e 7461 696e  ter.keys.contain
+00000e00: 7328 656c 656d 656e 7429 2920 7b7b 0a20  s(element)) {{. 
+00000e10: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00000e20: 6872 6f77 2045 7863 6570 7469 6f6e 2822  hrow Exception("
+00000e30: 247b 7b65 6c65 6d65 6e74 7d7d e79a 84e5  ${{element}}....
+00000e40: ae9e e78e b0e7 b1bb e69c aae6 9caa e6b3  ................
+00000e50: a8e5 868c efbc 81ef bc81 efbc 81e8 afb7  ................
+00000e60: e588 a0e9 99a4 e5ba 9324 7b7b 656c 656d  .........${{elem
+00000e70: 656e 747d 7de7 9a84 e5bc 95e7 94a8 e688  ent}}...........
+00000e80: 96e8 8085 e5bc 95e5 85a5 e5ae 9ee7 8eb0  ................
+00000e90: e7b1 bb22 293b 0a20 2020 2020 2020 2020  ...");.         
+00000ea0: 2020 2020 207d 7d0a 2020 2020 2020 2020       }}.        
+00000eb0: 2020 2020 7d7d 293b 0a20 2020 2020 2020      }});.       
+00000ec0: 2020 207d 7d0a 0a20 2020 2020 2020 2020     }}..         
+00000ed0: 2073 7461 7469 6320 766f 6964 2061 7574   static void aut
+00000ee0: 6f52 6567 6973 7465 7228 2920 7b7b 0a20  oRegister() {{. 
+00000ef0: 2020 2020 2020 2020 2020 2020 207b 317d               {1}
+00000f00: 0a20 2020 2020 2020 2020 2020 2020 205f  .              _
+00000f10: 656e 7375 7265 4170 6949 6d70 6c52 6567  ensureApiImplReg
+00000f20: 6973 7465 7228 293b 0a20 2020 2020 2020  ister();.       
+00000f30: 2020 207d 7d0a 2020 2020 2020 2020 7d7d     }}.        }}
+00000f40: 0a20 2020 2020 2020 2020 2020 2029 1172  .            ).r
+00000f50: 2900 0000 da05 7772 6974 6572 0800 0000  ).....writer....
+00000f60: 5a10 6465 6661 756c 7454 6974 6c65 4465  Z.defaultTitleDe
+00000f70: 7363 722a 0000 0072 2c00 0000 da25 5f41  scr*...r,....%_A
+00000f80: 7069 416e 6e6f 7461 7469 6f6e 5f5f 5f5f  piAnnotation____
+00000f90: 696d 706f 7274 5f64 6174 615f 6372 6561  import_data_crea
+00000fa0: 746f 7272 0d00 0000 720f 0000 0072 1c00  torr....r....r..
+00000fb0: 0000 722e 0000 0072 2700 0000 da31 5f41  ..r....r'....1_A
+00000fc0: 7069 416e 6e6f 7461 7469 6f6e 5f5f 696d  piAnnotation__im
+00000fd0: 706f 7274 5f64 6174 615f 6372 6561 746f  port_data_creato
+00000fe0: 725f 7769 7468 6f75 745f 616c 6961 7372  r_without_aliasr
+00000ff0: 3000 0000 da06 666f 726d 6174 da10 6170  0.....format..ap
+00001000: 695f 6c69 7374 5f63 7265 6174 6f72 da25  i_list_creator.%
+00001010: 5f41 7069 416e 6e6f 7461 7469 6f6e 5f5f  _ApiAnnotation__
+00001020: 7265 6769 7374 6572 5f6c 6973 745f 6372  register_list_cr
+00001030: 6561 746f 7229 0372 1100 0000 5a05 5f69  eator).r....Z._i
+00001040: 7465 6dda 0763 6f6e 7465 6e74 7212 0000  tem..contentr...
+00001050: 0072 1200 0000 7213 0000 005a 185f 5f67  .r....r....Z.__g
+00001060: 656e 6572 6174 655f 7265 6769 7374 6572  enerate_register
+00001070: 5f63 6f64 6552 0000 0073 1a00 0000 0001  _codeR...s......
+00001080: 1402 0a01 1c01 0a01 1c02 1802 0415 0601  ................
+00001090: 0401 0601 06fe 02ff 7a26 4170 6941 6e6e  ........z&ApiAnn
+000010a0: 6f74 6174 696f 6e2e 5f5f 6765 6e65 7261  otation.__genera
+000010b0: 7465 5f72 6567 6973 7465 725f 636f 6465  te_register_code
+000010c0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+000010d0: 0007 0000 0043 0000 0073 2c00 0000 6401  .....C...s,...d.
+000010e0: 7d01 7c00 6a00 4400 5d1c 7d02 7c01 6402  }.|.j.D.].}.|.d.
+000010f0: a001 7c02 a002 a100 7c02 a002 a100 a102  ..|.....|.......
+00001100: 3700 7d01 710a 7c01 5300 2903 4e72 0b00  7.}.q.|.S.).Nr..
+00001110: 0000 7a69 0a20 2020 2020 2020 2020 2020  ..zi.           
+00001120: 2041 7069 5265 6769 7374 6572 4365 6e74   ApiRegisterCent
+00001130: 6572 2e72 6567 6973 7465 7228 7b30 7d2e  er.register({0}.
+00001140: 4175 746f 5265 6769 7374 6572 2e61 7069  AutoRegister.api
+00001150: 5479 7065 2c7b 317d 2e41 7574 6f52 6567  Type,{1}.AutoReg
+00001160: 6973 7465 722e 7072 6f76 6964 6572 293b  ister.provider);
+00001170: 0a20 2020 2020 2020 2020 2020 2029 0372  .            ).r
+00001180: 2c00 0000 7244 0000 0072 1c00 0000 a903  ,...rD...r......
+00001190: 7211 0000 0072 4700 0000 da04 6974 656d  r....rG.....item
+000011a0: 7212 0000 0072 1200 0000 7213 0000 005a  r....r....r....Z
+000011b0: 175f 5f72 6567 6973 7465 725f 6c69 7374  .__register_list
+000011c0: 5f63 7265 6174 6f72 7600 0000 730c 0000  _creatorv...s...
+000011d0: 0000 0104 010a 0106 020c fe08 037a 2541  .............z%A
+000011e0: 7069 416e 6e6f 7461 7469 6f6e 2e5f 5f72  piAnnotation.__r
+000011f0: 6567 6973 7465 725f 6c69 7374 5f63 7265  egister_list_cre
+00001200: 6174 6f72 6301 0000 0000 0000 0000 0000  atorc...........
+00001210: 0003 0000 0006 0000 0043 0000 0073 2600  .........C...s&.
+00001220: 0000 6401 7d01 7c00 6a00 4400 5d16 7d02  ..d.}.|.j.D.].}.
+00001230: 7c01 6402 a001 7c02 a002 a100 a101 3700  |.d...|.......7.
+00001240: 7d01 710a 7c01 5300 2903 4e72 0b00 0000  }.q.|.S.).Nr....
+00001250: 7a4f 0a20 2020 2020 2020 2020 2020 207b  zO.            {
+00001260: 307d 2e54 4446 4d6f 6475 6c65 496e 7465  0}.TDFModuleInte
+00001270: 7266 6163 6541 7574 6f49 6e76 616c 6964  rfaceAutoInvalid
+00001280: 6174 652e 6170 6954 7970 652c 0a20 2020  ate.apiType,.   
+00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012a0: 2029 0372 2e00 0000 7244 0000 0072 2700   ).r....rD...r'.
+000012b0: 0000 7248 0000 0072 1200 0000 7212 0000  ..rH...r....r...
+000012c0: 0072 1300 0000 7245 0000 007e 0000 0073  .r....rE...~...s
+000012d0: 0c00 0000 0001 0401 0a01 0602 06fe 0803  ................
+000012e0: 7a1e 4170 6941 6e6e 6f74 6174 696f 6e2e  z.ApiAnnotation.
+000012f0: 6170 695f 6c69 7374 5f63 7265 6174 6f72  api_list_creator
+00001300: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+00001310: 0005 0000 0043 0000 0073 6200 0000 7400  .....C...sb...t.
+00001320: a001 6401 a101 0100 7c00 6a02 4400 5d4c  ..d.....|.j.D.]L
+00001330: 7d01 7c00 a003 7c01 6a04 7c00 6a05 a102  }.|...|.j.|.j...
+00001340: 7d02 7c02 6400 7501 7210 7406 8300 7d03  }.|.d.u.r.t...}.
+00001350: 7c01 6a04 7c03 5f04 7c01 6a07 7c03 5f07  |.j.|._.|.j.|._.
+00001360: 7c02 7c03 5f08 7c03 a009 a100 0100 7c00  |.|._.|.......|.
+00001370: 6a0a a00b 7c03 a101 0100 7110 6400 5300  j...|.....q.d.S.
+00001380: 2902 4e75 1c00 0000 e695 b4e5 9088 e689  ).Nu............
+00001390: 80e6 9c89 e4ba a4e4 ba92 696d 706c e696  ..........impl..
+000013a0: 87e4 bbb6 290c 7206 0000 00da 0574 6974  ....).r......tit
+000013b0: 6c65 7231 0000 00da 1f5f 4170 6941 6e6e  ler1....._ApiAnn
+000013c0: 6f74 6174 696f 6e5f 5f67 6574 5f74 6172  otation__get_tar
+000013d0: 6765 745f 6669 6c65 720e 0000 0072 2b00  get_filer....r+.
+000013e0: 0000 7209 0000 0072 0d00 0000 720f 0000  ..r....r....r...
+000013f0: 0072 2100 0000 722c 0000 00da 0661 7070  .r!...r,.....app
+00001400: 656e 6429 0472 1100 0000 da0b 7061 636b  end).r......pack
+00001410: 6167 6549 7465 6dda 195f 4170 6941 6e6e  ageItem.._ApiAnn
+00001420: 6f74 6174 696f 6e5f 5f66 696c 655f 7061  otation__file_pa
+00001430: 7468 5a09 5f69 6d70 6c4e 6f64 6572 1200  thZ._implNoder..
+00001440: 0000 7212 0000 0072 1300 0000 5a1a 5f5f  ..r....r....Z.__
+00001450: 696e 7465 6772 6174 655f 7464 665f 696d  integrate_tdf_im
+00001460: 706c 5f66 696c 6573 8600 0000 7314 0000  pl_files....s...
+00001470: 0000 010a 010a 0110 0108 0106 0108 0108  ................
+00001480: 0106 0108 017a 2841 7069 416e 6e6f 7461  .....z(ApiAnnota
+00001490: 7469 6f6e 2e5f 5f69 6e74 6567 7261 7465  tion.__integrate
+000014a0: 5f74 6466 5f69 6d70 6c5f 6669 6c65 7363  _tdf_impl_filesc
+000014b0: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+000014c0: 0500 0000 4300 0000 7362 0000 0074 00a0  ....C...sb...t..
+000014d0: 0164 01a1 0101 007c 006a 0244 005d 4c7d  .d.....|.j.D.]L}
+000014e0: 017c 00a0 037c 016a 047c 006a 05a1 027d  .|...|.j.|.j...}
+000014f0: 027c 0264 0075 0172 1074 0683 007d 037c  .|.d.u.r.t...}.|
+00001500: 016a 047c 035f 047c 016a 077c 035f 077c  .j.|._.|.j.|._.|
+00001510: 027c 035f 087c 03a0 09a1 0001 007c 006a  .|._.|.......|.j
+00001520: 0aa0 0b7c 03a1 0101 0071 1064 0053 0029  ...|.....q.d.S.)
+00001530: 024e 751b 0000 00e6 95b4 e590 88e6 8980  .Nu.............
+00001540: e69c 89e4 baa4 e4ba 9261 7069 e696 87e4  .........api....
+00001550: bbb6 290c 7206 0000 0072 4a00 0000 7231  ..).r....rJ...r1
+00001560: 0000 0072 4b00 0000 720e 0000 0072 2d00  ...rK...r....r-.
+00001570: 0000 7226 0000 0072 0d00 0000 720f 0000  ..r&...r....r...
+00001580: 0072 2100 0000 722e 0000 0072 4c00 0000  .r!...r....rL...
+00001590: 2904 7211 0000 0072 4d00 0000 724e 0000  ).r....rM...rN..
+000015a0: 005a 085f 6170 694e 6f64 6572 1200 0000  .Z._apiNoder....
+000015b0: 7212 0000 0072 1300 0000 5a19 5f5f 696e  r....r....Z.__in
+000015c0: 7465 6772 6174 655f 7464 665f 6170 695f  tegrate_tdf_api_
+000015d0: 6669 6c65 7392 0000 0073 1400 0000 0001  files....s......
+000015e0: 0a01 0a01 1001 0801 0601 0801 0801 0601  ................
+000015f0: 0801 7a27 4170 6941 6e6e 6f74 6174 696f  ..z'ApiAnnotatio
+00001600: 6e2e 5f5f 696e 7465 6772 6174 655f 7464  n.__integrate_td
+00001610: 665f 6170 695f 6669 6c65 7329 03da 0966  f_api_files)...f
+00001620: 696c 655f 7061 7468 da06 7375 6666 6978  ile_path..suffix
+00001630: 7216 0000 0063 0300 0000 0000 0000 0000  r....c..........
+00001640: 0000 0c00 0000 0600 0000 4300 0000 73ce  ..........C...s.
+00001650: 0000 0074 00a0 01a1 0001 0074 02a0 037c  ...t.......t...|
+00001660: 01a1 0101 0064 017d 0374 02a0 0474 05a0  .....d.}.t...t..
+00001670: 06a1 00a1 01a0 07a1 00a0 0864 02a1 0164  ...........d...d
+00001680: 0119 007d 0474 02a0 097c 04a1 0144 005d  ...}.t...|...D.]
+00001690: 665c 037d 057d 067d 077c 0744 005d 567d  f\.}.}.}.|.D.]V}
+000016a0: 0874 026a 0aa0 0b7c 057c 08a1 027d 097c  .t.j...|.|...}.|
+000016b0: 09a0 0c7c 02a1 0172 4a7c 0364 0337 007d  ...|...rJ|.d.7.}
+000016c0: 0374 05a0 0da1 0072 927c 09a0 0864 04a1  .t.....r.|...d..
+000016d0: 0164 0319 007d 0a7c 0aa0 0e64 0564 06a1  .d...}.|...d.d..
+000016e0: 027d 0b71 4a7c 09a0 0864 07a1 0164 0319  .}.qJ|...d...d..
+000016f0: 007d 0b71 4a71 3c7c 0364 036b 0272 b07c  .}.qJq<|.d.k.r.|
+00001700: 0b53 007c 0364 036b 0472 ca74 0f64 08a0  .S.|.d.k.r.t.d..
+00001710: 107c 01a1 0183 0182 0164 0053 0064 0053  .|.......d.S.d.S
+00001720: 0029 094e 7201 0000 00da 010a e901 0000  .).Nr...........
+00001730: 007a 055c 6c69 625c fa01 5c72 1e00 0000  .z.\lib\..\r....
+00001740: 7a05 2f6c 6962 2f75 3000 0000 e6a8 a1e5  z./lib/u0.......
+00001750: 9d97 7b30 7de5 ad98 e59c a8e5 a49a e4b8  ..{0}...........
+00001760: aae4 baa4 e4ba 92e6 9687 e4bb b6ef bc8c  ................
+00001770: e8af b7e6 a380 e69f a5e2 9d8c 2911 7207  ............).r.
+00001780: 0000 0072 3300 0000 7234 0000 00da 0563  ...r3...r4.....c
+00001790: 6864 6972 da05 706f 7065 6e72 0500 0000  hdir..popenr....
+000017a0: da07 7077 645f 636d 64da 0472 6561 64da  ..pwd_cmd..read.
+000017b0: 0573 706c 6974 da04 7761 6c6b 7238 0000  .split..walkr8..
+000017c0: 0072 3900 0000 da08 656e 6473 7769 7468  .r9.....endswith
+000017d0: da0a 6973 5f77 696e 646f 7773 da07 7265  ..is_windows..re
+000017e0: 706c 6163 65da 0945 7863 6570 7469 6f6e  place..Exception
+000017f0: 7244 0000 0029 0c72 1100 0000 724f 0000  rD...).r....rO..
+00001800: 0072 5000 0000 da05 636f 756e 74da 086e  .rP.....count..n
+00001810: 6f77 6150 6174 68da 0472 6f6f 74da 0464  owaPath..root..d
+00001820: 6972 73da 0566 696c 6573 da04 6669 6c65  irs..files..file
+00001830: da08 7372 635f 6669 6c65 da04 7465 6d70  ..src_file..temp
+00001840: 5a1b 5f41 7069 416e 6e6f 7461 7469 6f6e  Z._ApiAnnotation
+00001850: 5f5f 7461 7267 6574 5f66 696c 6572 1200  __target_filer..
+00001860: 0000 7212 0000 0072 1300 0000 5a11 5f5f  ..r....r....Z.__
+00001870: 6765 745f 7461 7267 6574 5f66 696c 659f  get_target_file.
+00001880: 0000 0073 2600 0000 0001 0801 0a02 0402  ...s&...........
+00001890: 1c01 1401 0801 0e01 0a01 0801 0801 0e01  ................
+000018a0: 0e02 1201 0801 0401 0801 0e01 0401 7a1f  ..............z.
+000018b0: 4170 6941 6e6e 6f74 6174 696f 6e2e 5f5f  ApiAnnotation.__
+000018c0: 6765 745f 7461 7267 6574 5f66 696c 6563  get_target_filec
+000018d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000018e0: 0500 0000 4300 0000 734e 0000 0074 00a0  ....C...sN...t..
+000018f0: 01a1 0001 0074 02a0 0364 01a1 0101 0074  .....t...d.....t
+00001900: 026a 04a0 057c 006a 06a1 0172 2c74 07a0  .j...|.j...r,t..
+00001910: 087c 006a 06a1 0101 0074 02a0 097c 006a  .|.j.....t...|.j
+00001920: 06a1 0101 0074 026a 04a0 0a74 00a0 0ba1  .....t.j...t....
+00001930: 0064 017c 006a 06a1 0353 0029 024e da03  .d.|.j...S.).N..
+00001940: 6c69 6229 0c72 0700 0000 7233 0000 0072  lib).r....r3...r
+00001950: 3400 0000 7254 0000 0072 3800 0000 da06  4...rT...r8.....
+00001960: 6578 6973 7473 722f 0000 00da 0673 6875  existsr/.....shu
+00001970: 7469 6cda 0672 6d74 7265 65da 056d 6b64  til..rmtree..mkd
+00001980: 6972 7239 0000 00da 0b67 6574 5368 656c  irr9.....getShel
+00001990: 6c44 6972 7210 0000 0072 1200 0000 7212  lDirr....r....r.
+000019a0: 0000 0072 1300 0000 7237 0000 00b7 0000  ...r....r7......
+000019b0: 0073 0c00 0000 0001 0801 0a01 0e01 0c01  .s..............
+000019c0: 0c01 7a21 4170 6941 6e6e 6f74 6174 696f  ..z!ApiAnnotatio
+000019d0: 6e2e 6765 745f 696e 7465 7261 6374 696f  n.get_interactio
+000019e0: 6e5f 6469 7263 0100 0000 0000 0000 0000  n_dirc..........
+000019f0: 0000 0200 0000 0500 0000 4300 0000 7332  ..........C...s2
+00001a00: 0000 0074 00a0 01a1 0001 0074 026a 03a0  ...t.......t.j..
+00001a10: 0474 00a0 05a1 0064 017c 006a 06a1 037d  .t.....d.|.j...}
+00001a20: 0174 02a0 0764 02a0 087c 01a1 01a1 0101  .t...d...|......
+00001a30: 0064 0053 0029 034e 7266 0000 007a 0f64  .d.S.).Nrf...z.d
+00001a40: 6172 7420 666f 726d 6174 207b 307d 2909  art format {0}).
+00001a50: 7207 0000 00da 0f67 6f49 6e53 6865 6c6c  r......goInShell
+00001a60: 4c69 6244 6972 7234 0000 0072 3800 0000  LibDirr4...r8...
+00001a70: 7239 0000 0072 6b00 0000 722f 0000 00da  r9...rk...r/....
+00001a80: 0673 7973 7465 6d72 4400 0000 2902 7211  .systemrD...).r.
+00001a90: 0000 005a 145f 4170 6941 6e6e 6f74 6174  ...Z._ApiAnnotat
+00001aa0: 696f 6e5f 5f70 6174 6872 1200 0000 7212  ion__pathr....r.
+00001ab0: 0000 0072 1300 0000 723f 0000 00c0 0000  ...r....r?......
+00001ac0: 0073 0600 0000 0001 0801 1601 7a18 4170  .s..........z.Ap
+00001ad0: 6941 6e6e 6f74 6174 696f 6e2e 5f5f 666f  iAnnotation.__fo
+00001ae0: 726d 6174 5f5f 6305 0000 0000 0000 0000  rmat__c.........
+00001af0: 0000 0005 0000 0007 0000 0043 0000 0073  ...........C...s
+00001b00: 1800 0000 7c01 a000 6401 a001 7c02 7c03  ....|...d...|.|.
+00001b10: 7c04 a103 a101 0100 6400 5300 2902 4e7a  |.......d.S.).Nz
+00001b20: 2169 6d70 6f72 7420 2270 6163 6b61 6765  !import "package
+00001b30: 3a7b 307d 2f7b 317d 2220 6173 207b 327d  :{0}/{1}" as {2}
+00001b40: 3b0a a902 7241 0000 0072 4400 0000 2905  ;...rA...rD...).
+00001b50: 7211 0000 00da 0766 5f77 7269 7465 da0b  r......f_write..
+00001b60: 6d6f 6475 6c65 5f6e 616d 6572 4f00 0000  module_namerO...
+00001b70: da05 616c 6961 7372 1200 0000 7212 0000  ..aliasr....r...
+00001b80: 0072 1300 0000 5a17 5f5f 5f5f 696d 706f  .r....Z.____impo
+00001b90: 7274 5f64 6174 615f 6372 6561 746f 72c6  rt_data_creator.
+00001ba0: 0000 0073 0a00 0000 0003 0401 0401 06ff  ...s............
+00001bb0: 02ff 7a25 4170 6941 6e6e 6f74 6174 696f  ..z%ApiAnnotatio
+00001bc0: 6e2e 5f5f 5f5f 696d 706f 7274 5f64 6174  n.____import_dat
+00001bd0: 615f 6372 6561 746f 7263 0400 0000 0000  a_creatorc......
+00001be0: 0000 0000 0000 0400 0000 0600 0000 4300  ..............C.
+00001bf0: 0000 7316 0000 007c 01a0 0064 01a0 017c  ..s....|...d...|
+00001c00: 027c 03a1 02a1 0101 0064 0053 0029 024e  .|.......d.S.).N
+00001c10: 7a1a 696d 706f 7274 2022 7061 636b 6167  z.import "packag
+00001c20: 653a 7b30 7d2f 7b31 7d22 3b0a 726e 0000  e:{0}/{1}";.rn..
+00001c30: 0029 0472 1100 0000 726f 0000 0072 7000  .).r....ro...rp.
+00001c40: 0000 724f 0000 0072 1200 0000 7212 0000  ..rO...r....r...
+00001c50: 0072 1300 0000 5a23 5f5f 696d 706f 7274  .r....Z#__import
+00001c60: 5f64 6174 615f 6372 6561 746f 725f 7769  _data_creator_wi
+00001c70: 7468 6f75 745f 616c 6961 73d0 0000 0073  thout_alias....s
+00001c80: 0a00 0000 0003 0401 0401 04ff 02ff 7a31  ..............z1
+00001c90: 4170 6941 6e6e 6f74 6174 696f 6e2e 5f5f  ApiAnnotation.__
+00001ca0: 696d 706f 7274 5f64 6174 615f 6372 6561  import_data_crea
+00001cb0: 746f 725f 7769 7468 6f75 745f 616c 6961  tor_without_alia
+00001cc0: 734e 2912 7222 0000 0072 2300 0000 7224  sN).r"...r#...r$
+00001cd0: 0000 00da 075f 5f64 6f63 5f5f 7214 0000  .....__doc__r...
+00001ce0: 0072 3200 0000 7240 0000 0072 3d00 0000  .r2...r@...r=...
+00001cf0: 7246 0000 0072 4500 0000 723c 0000 0072  rF...rE...r<...r
+00001d00: 3b00 0000 7225 0000 0072 4b00 0000 7237  ;...r%...rK...r7
+00001d10: 0000 0072 3f00 0000 7242 0000 0072 4300  ...r?...rB...rC.
+00001d20: 0000 7212 0000 0072 1200 0000 7212 0000  ..r....r....r...
+00001d30: 0072 1300 0000 7228 0000 0025 0000 0073  .r....r(...%...s
+00001d40: 1c00 0000 0801 0404 080e 0806 0814 0824  ...............$
+00001d50: 0808 0808 080c 080d 1218 0809 0806 080a  ................
+00001d60: 7228 0000 0029 12da 0768 6173 686c 6962  r(...)...hashlib
+00001d70: 7202 0000 0072 3400 0000 7268 0000 00da  r....r4...rh....
+00001d80: 2574 6466 5f74 6f6f 6c2e 746f 6f6c 732e  %tdf_tool.tools.
+00001d90: 636f 6e66 6967 2e70 6163 6b61 6765 735f  config.packages_
+00001da0: 636f 6e66 6967 7203 0000 0072 0400 0000  configr....r....
+00001db0: da1d 7464 665f 746f 6f6c 2e74 6f6f 6c73  ..tdf_tool.tools
+00001dc0: 2e70 6c61 7466 6f72 6d5f 746f 6f6c 7372  .platform_toolsr
+00001dd0: 0500 0000 da14 7464 665f 746f 6f6c 2e74  ......tdf_tool.t
+00001de0: 6f6f 6c73 2e70 7269 6e74 7206 0000 00da  ools.printr.....
+00001df0: 1874 6466 5f74 6f6f 6c2e 746f 6f6c 732e  .tdf_tool.tools.
+00001e00: 7368 656c 6c5f 6469 7272 0700 0000 5a18  shell_dirr....Z.
+00001e10: 7464 665f 746f 6f6c 2e74 6f6f 6c73 2e67  tdf_tool.tools.g
+00001e20: 656e 6572 6174 6f72 7208 0000 0072 0900  eneratorr....r..
+00001e30: 0000 7226 0000 0072 2800 0000 7212 0000  ..r&...r(...r...
+00001e40: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00001e50: da08 3c6d 6f64 756c 653e 0100 0000 7314  ..<module>....s.
+00001e60: 0000 000c 0108 0108 0110 010c 010c 010c  ................
+00001e70: 010c 030e 0d0e 0d                        .......
```

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/annotation.py` & `tdf_tool-2.4.8/tdf_tool/pipelines/annotation.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/api_interaction.py` & `tdf_tool-2.4.8/tdf_tool/pipelines/api_interaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,17 @@
     """
 
     def __init__(self):
         self.ff = None
         self.__generator: str = "ApiAnnotationGenerator"  # 生成器名
         self.__implSuffix: str = ".tdf_impl.dart"  # 交互描述文件后缀
         self.__implNodeList: list[ImplNode] = []  # impl描述文件列表
-        self.__apiSuffix: str = ".tdf_api.dart"  # 交互api描述文件后缀
+        self.__apiSuffix: str = ".tdf_module_interface.dart"  # 交互api描述文件后缀
         self.__apiNodeList: list[ApiNode] = []  # api描述文件列表
-        self.__interactionDir: str = "tdf_api"  # 交互文件目录
+        self.__interactionDir: str = "tdf_interaction"  # 交互文件目录
         self.__annotationName: str = "tdf_module_api_anno"  # 注解库名
         self.__packagesList: list[PackageNode] = []  # 壳依赖的所有库
 
         self.fetch_packages_list()
 
     # 遍历壳应用.packages下的所有package,将所有tdf开头的模块都添加入packagesList中
     def fetch_packages_list(self):
@@ -123,15 +123,15 @@
             """.format(item.impl_md5(), item.impl_md5())
         return content
 
     def api_list_creator(self):
         content = ""
         for item in self.__apiNodeList:
             content += """
-            {0}.TDFApiAutoInvalidate.apiType,
+            {0}.TDFModuleInterfaceAutoInvalidate.apiType,
                     """.format(item.api_md5())
         return content
 
     def __integrate_tdf_impl_files(self):
         Print.title("整合所有交互impl文件")
         for packageItem in self.__packagesList:
             __file_path = self.__get_target_file(packageItem.packagePath, self.__implSuffix)
```

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/fix_header.py` & `tdf_tool-2.4.8/tdf_tool/pipelines/fix_header.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/git.py` & `tdf_tool-2.4.8/tdf_tool/pipelines/git.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/module.py` & `tdf_tool-2.4.8/tdf_tool/pipelines/module.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/package.py` & `tdf_tool-2.4.8/tdf_tool/pipelines/package.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/router.py` & `tdf_tool-2.4.8/tdf_tool/pipelines/router.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/pipelines/translate.py` & `tdf_tool-2.4.8/tdf_tool/pipelines/translate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/env.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/env.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/env.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/env.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/generator.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/generator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/print.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/print.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/print.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/print.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/cli/bean/deps_item.py` & `tdf_tool-2.4.8/tdf_tool/tools/cli/bean/deps_item.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/cli/module_deps_rewrite.py` & `tdf_tool-2.4.8/tdf_tool/tools/cli/module_deps_rewrite.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/cli/project_cli.py` & `tdf_tool-2.4.8/tdf_tool/tools/cli/project_cli.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/cli/utils/yaml_utils.py` & `tdf_tool-2.4.8/tdf_tool/tools/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/cmd.py` & `tdf_tool-2.4.8/tdf_tool/tools/cmd.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/config/config.py` & `tdf_tool-2.4.8/tdf_tool/tools/config/config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/config/initial_json_config.py` & `tdf_tool-2.4.8/tdf_tool/tools/config/initial_json_config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/config/module_json_config.py` & `tdf_tool-2.4.8/tdf_tool/tools/config/module_json_config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/config/packages_config.py` & `tdf_tool-2.4.8/tdf_tool/tools/config/packages_config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/dependencies_analysis.py` & `tdf_tool-2.4.8/tdf_tool/tools/dependencies_analysis.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/env.py` & `tdf_tool-2.4.8/tdf_tool/tools/env.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_entry.py` & `tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_entry.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_lint.py` & `tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_lint_tool.py` & `tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_lint_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/fix_header/fix_header_replace_tool.py` & `tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_replace_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/flutter_script.py` & `tdf_tool-2.4.8/tdf_tool/tools/flutter_script.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/gitlab/gitlab_utils.py` & `tdf_tool-2.4.8/tdf_tool/tools/gitlab/gitlab_utils.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/gitlab/python_gitlab_api.py` & `tdf_tool-2.4.8/tdf_tool/tools/gitlab/python_gitlab_api.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/module/module_tools.py` & `tdf_tool-2.4.8/tdf_tool/tools/module/module_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/package/seal_off_package_utils.py` & `tdf_tool-2.4.8/tdf_tool/tools/package/seal_off_package_utils.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/platform_tools.py` & `tdf_tool-2.4.8/tdf_tool/tools/platform_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/print.py` & `tdf_tool-2.4.8/tdf_tool/tools/print.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/regular_tool.py` & `tdf_tool-2.4.8/tdf_tool/tools/regular_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/shell_dir.py` & `tdf_tool-2.4.8/tdf_tool/tools/shell_dir.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/file_util.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/file_util.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/flutter_translate_lint.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/flutter_translate_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/flutter_translate_tools.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/flutter_translate_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/ios_translate.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/ios_translate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/ios_translate_lint.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/ios_translate_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_module.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_module.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/location_string_temp.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/location_string_temp.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/podspec.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/podspec.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/ios/tools/string_util.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/string_util.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/tools/translate_tool.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/tools/translate_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/translate/translate_lint.py` & `tdf_tool-2.4.8/tdf_tool/tools/translate/translate_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc` & `tdf_tool-2.4.8/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.7/PKG-INFO` & `tdf_tool-2.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdf_tool
-Version: 2.4.7
+Version: 2.4.8
 Summary: 二维火 flutter 脚手架工具
 Home-page: https://git.2dfire.net/app/flutter/tools/package_tools
 License: MIT
 Keywords: tdf,tdf-tool,tdf_tool
 Author: Jian Xu
 Author-email: 3386218996@qq.com
 Requires-Python: >=3.9.0,<4.0.0
```

