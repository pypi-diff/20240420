# Comparing `tmp/cli_command_parser-2023.7.30.tar.gz` & `tmp/cli_command_parser-2024.4.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_command_parser-2023.7.30.tar", last modified: Sun Jul 30 20:03:19 2023, max compression
+gzip compressed data, was "cli_command_parser-2024.4.20.tar", last modified: Sat Apr 20 20:56:14 2024, max compression
```

## Comparing `cli_command_parser-2023.7.30.tar` & `cli_command_parser-2024.4.20.tar`

### file list

```diff
@@ -1,70 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.998197 cli_command_parser-2023.7.30/
--rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.30/LICENSE
--rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.30/MANIFEST.in
--rw-rw-rw-   0        0        0     5611 2023-07-30 20:03:18.998197 cli_command_parser-2023.7.30/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.844197 cli_command_parser-2023.7.30/lib/
-drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.905198 cli_command_parser-2023.7.30/lib/cli_command_parser/
--rw-rw-rw-   0        0        0     1158 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/__init__.py
--rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/__main__.py
--rw-rw-rw-   0        0        0      295 2023-07-30 20:03:08.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/__version__.py
--rw-rw-rw-   0        0        0     2430 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/annotations.py
--rw-rw-rw-   0        0        0    19228 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/command_parameters.py
--rw-rw-rw-   0        0        0    12852 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/commands.py
--rw-rw-rw-   0        0        0     5101 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/compat.py
--rw-rw-rw-   0        0        0    18620 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/config.py
--rw-rw-rw-   0        0        0    19945 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/context.py
-drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.943197 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/
--rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/__init__.py
--rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/__main__.py
--rw-rw-rw-   0        0        0    12711 2023-05-08 11:55:32.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/argparse_ast.py
--rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/argparse_utils.py
--rw-rw-rw-   0        0        0    24279 2023-05-08 11:55:32.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/command_builder.py
--rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/utils.py
--rw-rw-rw-   0        0        0     7375 2023-05-08 11:55:32.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/visitor.py
--rw-rw-rw-   0        0        0    12518 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/core.py
--rw-rw-rw-   0        0        0    15359 2023-05-13 19:45:03.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/documentation.py
--rw-rw-rw-   0        0        0     6787 2023-04-29 17:20:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/error_handling.py
--rw-rw-rw-   0        0        0     8297 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.957196 cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/
--rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/__init__.py
--rw-rw-rw-   0        0        0     9604 2023-07-29 13:17:30.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/commands.py
--rw-rw-rw-   0        0        0    21721 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/params.py
--rw-rw-rw-   0        0        0     9377 2023-05-13 19:45:03.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/restructured_text.py
--rw-rw-rw-   0        0        0     5306 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.985197 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/
--rw-rw-rw-   0        0        0     2591 2023-05-14 19:11:26.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/__init__.py
--rw-rw-rw-   0        0        0     1550 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/base.py
--rw-rw-rw-   0        0        0     6582 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/choices.py
--rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/exceptions.py
--rw-rw-rw-   0        0        0     8897 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/files.py
--rw-rw-rw-   0        0        0     8341 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/numeric.py
--rw-rw-rw-   0        0        0     7601 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/patterns.py
--rw-rw-rw-   0        0        0    22732 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/time.py
--rw-rw-rw-   0        0        0     6523 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/utils.py
--rw-rw-rw-   0        0        0    13618 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/metadata.py
--rw-rw-rw-   0        0        0     8144 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/nargs.py
-drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.998197 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/
--rw-rw-rw-   0        0        0      313 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/__init__.py
--rw-rw-rw-   0        0        0    17329 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/actions.py
--rw-rw-rw-   0        0        0    25178 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/base.py
--rw-rw-rw-   0        0        0    16732 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/choice_map.py
--rw-rw-rw-   0        0        0    10656 2023-05-13 19:45:03.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/groups.py
--rw-rw-rw-   0        0        0     8242 2023-05-21 20:53:58.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/option_strings.py
--rw-rw-rw-   0        0        0    25683 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/options.py
--rw-rw-rw-   0        0        0      896 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/pass_thru.py
--rw-rw-rw-   0        0        0     4543 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/positionals.py
--rw-rw-rw-   0        0        0    11295 2023-05-21 20:53:58.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parse_tree.py
--rw-rw-rw-   0        0        0    16709 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parser.py
--rw-rw-rw-   0        0        0    12348 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/testing.py
--rw-rw-rw-   0        0        0     1977 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/typing.py
--rw-rw-rw-   0        0        0     5695 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.917196 cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/
--rw-rw-rw-   0        0        0     5611 2023-07-30 20:03:18.000000 cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2367 2023-07-30 20:03:18.000000 cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 20:03:18.000000 cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-07-30 20:03:18.000000 cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-30 20:03:18.000000 cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      316 2023-05-02 11:35:36.000000 cli_command_parser-2023.7.30/pyproject.toml
--rw-rw-rw-   0        0        0     4414 2023-05-02 11:35:36.000000 cli_command_parser-2023.7.30/readme.rst
--rw-rw-rw-   0        0        0      111 2023-04-10 12:30:46.000000 cli_command_parser-2023.7.30/requirements-dev.txt
--rw-rw-rw-   0        0        0     1293 2023-07-30 20:03:18.999198 cli_command_parser-2023.7.30/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 20:56:14.606003 cli_command_parser-2024.4.20/
+-rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2024.4.20/LICENSE
+-rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2024.4.20/MANIFEST.in
+-rw-rw-rw-   0        0        0     5947 2024-04-20 20:56:14.606003 cli_command_parser-2024.4.20/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/entry_points.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 20:56:14.469003 cli_command_parser-2024.4.20/lib/
+drwxrwxrwx   0        0        0        0 2024-04-20 20:56:14.522003 cli_command_parser-2024.4.20/lib/cli_command_parser/
+-rw-rw-rw-   0        0        0     1172 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/__init__.py
+-rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/__main__.py
+-rw-rw-rw-   0        0        0      295 2024-04-20 20:55:58.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/__version__.py
+-rw-rw-rw-   0        0        0     2812 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/annotations.py
+-rw-rw-rw-   0        0        0    19229 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/command_parameters.py
+-rw-rw-rw-   0        0        0    17747 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/commands.py
+-rw-rw-rw-   0        0        0     5101 2023-07-30 20:03:01.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/compat.py
+-rw-rw-rw-   0        0        0    18605 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/config.py
+-rw-rw-rw-   0        0        0    19931 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/context.py
+drwxrwxrwx   0        0        0        0 2024-04-20 20:56:14.558002 cli_command_parser-2024.4.20/lib/cli_command_parser/conversion/
+-rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/conversion/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/conversion/__main__.py
+-rw-rw-rw-   0        0        0    12711 2023-05-08 11:55:32.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/conversion/argparse_ast.py
+-rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/conversion/argparse_utils.py
+-rw-rw-rw-   0        0        0     2047 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/conversion/cli.py
+-rw-rw-rw-   0        0        0    24279 2023-05-08 11:55:32.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/conversion/command_builder.py
+-rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/conversion/utils.py
+-rw-rw-rw-   0        0        0     8927 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/conversion/visitor.py
+-rw-rw-rw-   0        0        0    12518 2023-05-29 16:32:28.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/core.py
+-rw-rw-rw-   0        0        0    15359 2023-05-13 19:45:03.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/documentation.py
+-rw-rw-rw-   0        0        0     6787 2023-04-29 17:20:11.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/error_handling.py
+-rw-rw-rw-   0        0        0     8407 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-20 20:56:14.570003 cli_command_parser-2024.4.20/lib/cli_command_parser/formatting/
+-rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/formatting/__init__.py
+-rw-rw-rw-   0        0        0     9550 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/formatting/commands.py
+-rw-rw-rw-   0        0        0    21528 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/formatting/params.py
+-rw-rw-rw-   0        0        0     9377 2023-05-13 19:45:03.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/formatting/restructured_text.py
+-rw-rw-rw-   0        0        0     5306 2023-07-30 20:03:01.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/formatting/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 20:56:14.589002 cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/
+-rw-rw-rw-   0        0        0     2591 2023-05-14 19:11:26.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/__init__.py
+-rw-rw-rw-   0        0        0     1550 2023-05-20 18:50:11.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/base.py
+-rw-rw-rw-   0        0        0     6695 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/choices.py
+-rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/exceptions.py
+-rw-rw-rw-   0        0        0     9096 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/files.py
+-rw-rw-rw-   0        0        0     8341 2023-05-20 18:50:11.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/numeric.py
+-rw-rw-rw-   0        0        0     7596 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/patterns.py
+-rw-rw-rw-   0        0        0    22732 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/time.py
+-rw-rw-rw-   0        0        0     6523 2023-05-20 18:50:11.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/utils.py
+-rw-rw-rw-   0        0        0    17663 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/metadata.py
+-rw-rw-rw-   0        0        0     8144 2023-05-29 16:32:28.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/nargs.py
+drwxrwxrwx   0        0        0        0 2024-04-20 20:56:14.604003 cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/
+-rw-rw-rw-   0        0        0      313 2023-06-14 11:32:55.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/__init__.py
+-rw-rw-rw-   0        0        0    17329 2023-07-30 20:03:01.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/actions.py
+-rw-rw-rw-   0        0        0    26658 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/base.py
+-rw-rw-rw-   0        0        0    16689 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/choice_map.py
+-rw-rw-rw-   0        0        0    11219 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/groups.py
+-rw-rw-rw-   0        0        0     8253 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/option_strings.py
+-rw-rw-rw-   0        0        0    25510 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/options.py
+-rw-rw-rw-   0        0        0      896 2023-05-29 16:32:28.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/pass_thru.py
+-rw-rw-rw-   0        0        0     4543 2023-07-30 20:03:01.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/positionals.py
+-rw-rw-rw-   0        0        0    11295 2023-05-21 20:53:58.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/parse_tree.py
+-rw-rw-rw-   0        0        0    16866 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/parser.py
+-rw-rw-rw-   0        0        0    12374 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/testing.py
+-rw-rw-rw-   0        0        0     1999 2023-10-14 13:44:15.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/typing.py
+-rw-rw-rw-   0        0        0     5864 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.20/lib/cli_command_parser/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 20:56:14.605005 cli_command_parser-2024.4.20/lib/cli_command_parser.egg-info/
+-rw-rw-rw-   0        0        0     5947 2024-04-20 20:56:14.000000 cli_command_parser-2024.4.20/lib/cli_command_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2474 2024-04-20 20:56:14.000000 cli_command_parser-2024.4.20/lib/cli_command_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 20:56:14.000000 cli_command_parser-2024.4.20/lib/cli_command_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-04-20 20:56:14.000000 cli_command_parser-2024.4.20/lib/cli_command_parser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       81 2024-04-20 20:56:14.000000 cli_command_parser-2024.4.20/lib/cli_command_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-20 20:56:14.000000 cli_command_parser-2024.4.20/lib/cli_command_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      316 2023-05-02 11:35:36.000000 cli_command_parser-2024.4.20/pyproject.toml
+-rw-rw-rw-   0        0        0     4428 2023-10-14 13:44:15.000000 cli_command_parser-2024.4.20/readme.rst
+-rw-rw-rw-   0        0        0      111 2023-04-10 12:30:46.000000 cli_command_parser-2024.4.20/requirements-dev.txt
+-rw-rw-rw-   0        0        0     1500 2024-04-20 20:56:14.607003 cli_command_parser-2024.4.20/setup.cfg
```

### Comparing `cli_command_parser-2023.7.30/LICENSE` & `cli_command_parser-2024.4.20/LICENSE`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/PKG-INFO` & `cli_command_parser-2024.4.20/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 Metadata-Version: 2.1
 Name: cli_command_parser
-Version: 2023.7.30
+Version: 2024.4.20
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
+Project-URL: Documentation, https://dskrypa.github.io/cli_command_parser
+Project-URL: Issues, https://github.com/dskrypa/cli_command_parser/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 Provides-Extra: wcwidth
+Requires-Dist: wcwidth; extra == "wcwidth"
 Provides-Extra: conversion
-License-File: LICENSE
+Requires-Dist: astunparse; python_version < "3.9" and extra == "conversion"
 
 CLI Command Parser
 ##################
 
 |downloads| |py_version| |coverage_badge| |build_status| |Blue|
 
-.. |py_version| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue
+.. |py_version| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12%20-blue
     :target: https://pypi.org/project/cli-command-parser/
 
 .. |coverage_badge| image:: https://codecov.io/gh/dskrypa/cli_command_parser/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/dskrypa/cli_command_parser
 
 .. |build_status| image:: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml
@@ -110,15 +115,15 @@
     $ pip install -U cli-command-parser[wcwidth]
 
 
 Python Version Compatibility
 ============================
 
 Python versions 3.8 and above are currently supported.  The last release of CLI Command Parser that supported 3.7 was
-2023-04-30.  Support for Python 3.7 `officially ends on 2023-06-27 <https://devguide.python.org/versions/>`__.
+2023-04-30.  Support for Python 3.7 `officially ended on 2023-06-27 <https://devguide.python.org/versions/>`__.
 
 When using Python 3.8, some additional packages that backport functionality that was added in later Python versions
 are required for compatibility.
 
 To use the argparse to cli-command-parser conversion script with Python 3.8, there is a dependency on
 `astunparse <https://astunparse.readthedocs.io>`__.  If you are using Python 3.9 or above, then ``astunparse`` is not
 necessary because the relevant code was added to the stdlib ``ast`` module.  If you're unsure, you can install
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/__init__.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     CommandConfig,
     ShowDefaults,
     OptionNameMode,
     SubcommandAliasHelpMode,
     AmbiguousComboMode,
     AllowLeadingDash,
 )
-from .commands import Command, main
+from .commands import Command, AsyncCommand, main
 from .context import Context, get_current_context, ctx, get_parsed, get_context, get_raw_arg
 from .exceptions import (
     CommandParserException,
     CommandDefinitionError,
     ParameterDefinitionError,
     UsageError,
     ParamUsageError,
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/annotations.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/annotations.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,19 +13,22 @@
 except ImportError:  # Added in 3.10
     NoneType = type(None)
 
 __all__ = ['get_descriptor_value_type']
 
 
 def get_descriptor_value_type(command_cls: type, attr: str) -> Optional[type]:
+    # TODO: Optimize this to cache get_type_hints for a given class?
     try:
         annotation = get_type_hints(command_cls)[attr]
     except (KeyError, NameError):  # KeyError due to attr missing; NameError for forward references
         return None
-
+    # Note: `inspect.get_annotations(obj)` returns a dict of where values are the string representations of the
+    # discovered annotations; values in the dict returned by `typing.get_type_hints` are the actual classes / typing
+    # aliases that were used, which are significantly more useful for this analysis.
     return get_annotation_value_type(annotation)
 
 
 def get_annotation_value_type(annotation, from_union: bool = True, from_collection: bool = True) -> Optional[type]:
     origin = get_origin(annotation)
     # Note: get_origin returns `list` for `List[str]`, `List`, and `list[str]`; it returns `None` for `list`
     if origin is None and isinstance(annotation, type):
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/command_parameters.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/command_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,18 +88,18 @@
             if not self.parent.sub_command:
                 return self.parent.all_positionals + self.positionals
         except AttributeError:
             pass
         return self.positionals
 
     def get_positionals_to_parse(self, ctx: Context) -> List[BasePositional]:
-        if positionals := self.all_positionals:
-            for i, param in enumerate(positionals):
+        if self.all_positionals:
+            for i, param in enumerate(self.all_positionals):
                 if not ctx.num_provided(param):
-                    return [p for p in positionals[i:]]
+                    return [p for p in self.all_positionals[i:]]
 
         return []
 
     @cached_property
     def formatter(self) -> CommandHelpFormatter:
         from .formatting.commands import CommandHelpFormatter
 
@@ -387,23 +387,23 @@
 
     def iter_params(self, exclude: Collection[Parameter] = ()) -> Iterator[Parameter]:
         if exclude:
             yield from (p for g in (self.all_positionals, self.options) for p in g if p not in exclude)
         else:
             yield from self.all_positionals
             yield from self.options
-        if (pass_thru := self.pass_thru) and pass_thru not in exclude:
-            yield pass_thru
+        if self.pass_thru and self.pass_thru not in exclude:
+            yield self.pass_thru
 
     def required_check_params(self) -> Iterator[Parameter]:
         ignore = SubCommand
         yield from (p for p in self.all_positionals if p.required and not p.group and not isinstance(p, ignore))
         yield from (p for p in self.options if p.required and not p.group)
-        if (pass_thru := self._pass_thru) and pass_thru.required and not pass_thru.group:
-            yield pass_thru
+        if self._pass_thru and self._pass_thru.required and not self._pass_thru.group:
+            yield self._pass_thru
 
 
 def _find_ambiguous_combos(
     single_char_combos: OptionMap, multi_char_combos: OptionMap
 ) -> Dict[str, Tuple[BaseOption, OptionMap]]:
     ambiguous_combo_options = {}
     for combo, param in multi_char_combos.items():
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/commands.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,27 +11,31 @@
 from contextlib import ExitStack
 from typing import TYPE_CHECKING, Type, Sequence, Optional, overload
 
 from .core import CommandMeta, get_top_level_commands, get_params
 from .context import Context, ActionPhase, get_or_create_context
 from .exceptions import ParamConflict
 from .parser import parse_args_and_get_next_cmd
+from .utils import maybe_await
 
 if TYPE_CHECKING:
     from .typing import Bool, CommandObj
 
 __all__ = ['Command', 'main']
 log = logging.getLogger(__name__)
 
 Argv = Sequence[str]
 
 
 class Command(ABC, metaclass=CommandMeta):
     """The main class that other Commands should extend."""
 
+    # TODO: Make the distinction between help/description clearer, or merge them?
+    # TODO: Pull help text from docstring for subcommands if not specified as help=?
+
     #: The parsing Context used for this Command. Provided here for convenience - this reference to it is not used by
     #: any CLI Command Parser internals, so it is safe for subclasses to redefine / overwrite it.
     ctx: Context
 
     def __new__(cls):
         # By storing the Context here instead of __init__, every single subclass won't need to
         # call super().__init__(...) from their own __init__ for this step
@@ -151,40 +155,45 @@
                     self._after_main_(*args, **kwargs)
                 raise
             else:
                 self._after_main_(*args, **kwargs)
 
         return ctx.actions_taken
 
-    def _pre_init_actions_(self, *args, **kwargs):
-        """
-        The first method called by :meth:`.__call__` (before :meth:`.main` and others).
-
-        Validates the number of ActionFlags that were specified, and calls all of the specified
-        :func:`~.options.before_main` / :obj:`~.options.action_flag` actions such as ``--help`` that were
-        defined with ``before_main=True`` and ``always_available=True`` in their configured order.
-
-        :param args: Positional arguments to pass to the :obj:`~.options.action_flag` methods
-        :param kwargs: Keyword arguments to pass to the :obj:`~.options.action_flag` methods
-        """
+    def _check_param_conflicts_(self):
         # TODO: --help should take precedence over input validation - right now, if a Path input expecting a
         #  non-existent file receives a file that exists, that error is reported instead of showing help text
         ctx = self.__ctx
         n_flags = ctx.action_flag_count
         if n_flags and not ctx.config.multiple_action_flags and n_flags > 1:
             raise ParamConflict(ctx.all_action_flags, 'combining multiple action flags is disabled')
 
         if before := ctx.categorized_action_flags[ActionPhase.BEFORE_MAIN]:
             action = get_params(self).action
             if action is not None and not ctx.config.action_after_action_flags:
                 raise ParamConflict([action, *before], 'combining an action with action flags is disabled')
 
-        for param in ctx.iter_action_flags(ActionPhase.PRE_INIT):
+    def _run_actions_(self, phase: ActionPhase, args: tuple, kwargs: dict):
+        for param in self.__ctx.iter_action_flags(phase):
             param.func(self, *args, **kwargs)
 
+    def _pre_init_actions_(self, *args, **kwargs):
+        """
+        The first method called by :meth:`.__call__` (before :meth:`.main` and others).
+
+        Validates the number of ActionFlags that were specified, and calls all of the specified
+        :func:`~.options.before_main` / :obj:`~.options.action_flag` actions such as ``--help`` that were
+        defined with ``before_main=True`` and ``always_available=True`` in their configured order.
+
+        :param args: Positional arguments to pass to the :obj:`~.options.action_flag` methods
+        :param kwargs: Keyword arguments to pass to the :obj:`~.options.action_flag` methods
+        """
+        self._check_param_conflicts_()
+        self._run_actions_(ActionPhase.PRE_INIT, args, kwargs)
+
     def _init_command_(self, *args, **kwargs):
         """
         Called by :meth:`.__call__` after :meth:`._pre_init_actions_` and before :meth:`._before_main_`.
 
         Safe to override without calling ``super()._init_command_()`` - the base implementation is a placeholder
         intended to allow subclasses to perform initialization tasks.  This method is called after actions like
         ``--help`` have been processed, so more resource-intensive initialization operations or those that may have
@@ -204,16 +213,15 @@
 
         Calls all of the specified :func:`~.options.before_main` / :obj:`~.options.action_flag` actions that
         were defined with ``before_main=True`` and ``always_available=False`` in their configured order.
 
         :param args: Positional arguments to pass to the :obj:`~.options.action_flag` methods
         :param kwargs: Keyword arguments to pass to the :obj:`~.options.action_flag` methods
         """
-        for param in self.__ctx.iter_action_flags(ActionPhase.BEFORE_MAIN):
-            param.func(self, *args, **kwargs)
+        self._run_actions_(ActionPhase.BEFORE_MAIN, args, kwargs)
 
     def main(self, *args, **kwargs) -> Optional[int]:
         """
         Primary method that is called when running a Command.
 
         If any arguments were specified that are associated with triggering a method that was decorated / registered as
         a positional :class:`~.choice_map.Action`'s target method, then that method is called here.
@@ -241,16 +249,119 @@
         Called by :meth:`.__call__` after :meth:`.main` is called.  Calls all of the specified
         :func:`~.options.after_main` / :obj:`~.options.action_flag` actions that were defined with
         ``before_main=False`` in their configured order.
 
         :param args: Positional arguments to pass to the :obj:`~.options.action_flag` methods
         :param kwargs: Keyword arguments to pass to the :obj:`~.options.action_flag` methods
         """
-        for param in self.__ctx.iter_action_flags(ActionPhase.AFTER_MAIN):
-            param.func(self, *args, **kwargs)
+        self._run_actions_(ActionPhase.AFTER_MAIN, args, kwargs)
+
+
+class AsyncCommand(Command, ABC):
+    """
+    Asynchronous version of the main class that other Commands should extend.
+
+    To run an AsyncCommand, both :func:`main` and :meth:`.parse_and_run` can be used as if running a synchronous
+    :class:`Command`.  The asynchronous version of :meth:`.parse_and_run` handles calling :func:`python:asyncio.run`.
+
+    For applications that need more direct control over how the event loop is run, :meth:`.parse_and_await` can be
+    used instead.
+
+    All `_sunder_` methods supported by :class:`Command` may be overridden with either synchronous or async versions,
+    and :class:`~.choice_map.Action` target methods may similarly be defined either way as well.
+    """
+
+    @classmethod
+    def parse_and_run(cls, argv=None, **kwargs):
+        """
+        Asynchronous version of :meth:`Command.parse_and_run`.  Argument parsing is handled synchronously, then
+        :func:`python:asyncio.run` is called with the parsed command's :meth:`.__call__` coroutine.
+
+        For applications that need more direct control over how the event loop is run, :meth:`.parse_and_await` can be
+        used instead.
+        """
+        import asyncio
+
+        ctx = get_or_create_context(cls, argv)
+        with ctx.get_error_handler():
+            self = cls.parse(argv)
+
+        try:
+            self
+        except UnboundLocalError:  # There was an error handled during parsing, so self was not defined
+            return None
+        else:
+            asyncio.run(self(**kwargs))
+            return self
+
+    @classmethod
+    async def parse_and_await(cls, argv=None, **kwargs):
+        """
+        Coroutine alternative to :meth:`.parse_and_run`.  This method does NOT call :func:`python:asyncio.run` - it is
+        meant to be used as ``await MyCommand.parse_and_await()`` with an existing event loop.
+
+        Simpler applications can likely use the easier :func:`main` function or :meth:`.parse_and_run` instead.
+        """
+        ctx = get_or_create_context(cls, argv)
+        with ctx.get_error_handler():
+            self = cls.parse(argv)
+
+        try:
+            self
+        except UnboundLocalError:  # There was an error handled during parsing, so self was not defined
+            return None
+        else:
+            await maybe_await(self(**kwargs))
+            return self
+
+    async def __call__(self, *args, **kwargs) -> int:
+        """Asynchronous version of :meth:`Command.__call__`."""
+        with self._Command__ctx as ctx, ctx.get_error_handler():  # noqa
+            await maybe_await(self._pre_init_actions_(*args, **kwargs))
+            await maybe_await(self._init_command_(*args, **kwargs))
+            await maybe_await(self._before_main_(*args, **kwargs))
+            try:
+                await maybe_await(self.main(*args, **kwargs))
+            except BaseException:
+                if ctx.config.always_run_after_main:
+                    log.debug('Caught exception - running _after_main_ before propagating', exc_info=True)
+                    await maybe_await(self._after_main_(*args, **kwargs))
+                raise
+            else:
+                await maybe_await(self._after_main_(*args, **kwargs))
+
+        return ctx.actions_taken
+
+    async def _run_actions_(self, phase: ActionPhase, args: tuple, kwargs: dict):
+        """Asynchronous version of :meth:`Command._run_actions_`."""
+        for param in self._Command__ctx.iter_action_flags(phase):  # noqa
+            await maybe_await(param.func(self, *args, **kwargs))
+
+    async def _pre_init_actions_(self, *args, **kwargs):
+        """Asynchronous version of :meth:`Command._pre_init_actions_`."""
+        self._check_param_conflicts_()
+        await self._run_actions_(ActionPhase.PRE_INIT, args, kwargs)
+
+    async def _before_main_(self, *args, **kwargs):
+        """Asynchronous version of :meth:`Command._before_main_`."""
+        await self._run_actions_(ActionPhase.BEFORE_MAIN, args, kwargs)
+
+    async def main(self, *args, **kwargs) -> Optional[int]:
+        """Asynchronous version of :meth:`Command.main`."""
+        with self._Command__ctx as ctx:  # noqa
+            action = get_params(self).action
+            if action is not None and (ctx.actions_taken == 0 or ctx.config.action_after_action_flags):
+                ctx.actions_taken += 1
+                await maybe_await(action.target()(self, *args, **kwargs))
+
+        return ctx.actions_taken
+
+    async def _after_main_(self, *args, **kwargs):
+        """Asynchronous version of :meth:`Command._after_main_`."""
+        await self._run_actions_(ActionPhase.AFTER_MAIN, args, kwargs)
 
 
 def main(argv: Argv = None, return_command: Bool = False, **kwargs) -> Optional[CommandObj]:
     """
     Convenience function that can be used as the main entry point for a program.
 
     As long as only one :class:`Command` subclass is present, this function will detect it and call its
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/compat.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/compat.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/config.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,16 +240,16 @@
         if instance is None:
             return self
         return instance._data.get(self.name, self.default)
 
     def __set__(self, instance: CommandConfig, value: ConfigValue):
         if instance._read_only:
             raise AttributeError(f'Unable to set attribute {self.name}={value!r} because {instance} is read-only')
-        elif (type_func := self.type) is not None:
-            value = type_func(value)
+        elif self.type is not None:
+            value = self.type(value)
         instance._data[self.name] = value
 
     def __delete__(self, instance: CommandConfig):
         if instance._read_only:
             raise AttributeError(f'Unable to delete attribute {self.name} because {instance} is read-only')
         try:
             del instance._data[self.name]
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/context.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,16 +142,16 @@
             return True
 
     # endregion
 
     @property
     def terminal_width(self) -> int:
         """Returns the current terminal width as the number of characters that fit on a single line."""
-        if (width := self._terminal_width) is not None:
-            return width
+        if self._terminal_width is not None:
+            return self._terminal_width
         return _TERMINAL.width
 
     def get_parsed(
         self,
         command: Command = None,
         *,
         exclude: Collection[Parameter] = (),
@@ -174,26 +174,26 @@
           user-provided values will be included.
         :return: A dictionary containing all of the arguments that were parsed.  The keys in the returned dict match
           the names assigned to the Parameters in the Command associated with this Context.
         """
         if command is None:
             command = self.command
         with self:
-            if recursive and (parent := self.parent):
-                parsed = parent.get_parsed(
+            if recursive and self.parent:
+                parsed = self.parent.get_parsed(
                     command, exclude=exclude, recursive=recursive, default=default, include_defaults=include_defaults
                 )
             else:
                 parsed = {}
 
             # TODO: Add way to get a nested dict with ParamGroup names as the keys of the nested sections?
-            if params := self.params:
-                for param in params.iter_params(exclude):
+            if self.params:
+                for param in self.params.iter_params(exclude):
                     if include_defaults or param in self._parsed:
-                        parsed[param.name] = param.result_value(command, default)
+                        parsed[param.name] = param.result(command, default)
 
         return parsed
 
     @cached_property
     def params(self) -> Optional[CommandParameters]:
         """
         The :class:`.CommandParameters` object that contains the categorized Parameters from the Command associated
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/argparse_ast.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/conversion/argparse_ast.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/argparse_utils.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/conversion/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/command_builder.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/conversion/command_builder.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/utils.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/visitor.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/conversion/visitor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import logging
+import re
 from ast import NodeVisitor, AST, Assign, Call, For, Attribute, Name, Import, ImportFrom, expr
 from collections import ChainMap, defaultdict
 from functools import partial, wraps
 from typing import Iterator, Union, Callable, Collection, Tuple, List, Dict, Set
 
 from .argparse_ast import AstArgumentParser
 from .utils import get_name_repr
@@ -39,15 +40,15 @@
     visit_FunctionDef = visit_AsyncFunctionDef = ScopedVisit()
     visit_Lambda = ScopedVisit()
     visit_ClassDef = ScopedVisit()
     visit_While = ScopedVisit()
 
     def __init__(self, smart_loop_handling: bool = True, track_refs: Collection[TrackedRef] = ()):
         self.smart_loop_handling = smart_loop_handling
-        self.scopes = ChainMap()
+        self.scopes = ChainMap()  # ChainMap that tracks the var/class/func/etc names available in a given scope
         self._tracked_refs = set()
         self._mod_name_tracked_map = defaultdict(dict)
         for ref in track_refs:
             self.track_refs_to(ref)
 
     def track_callable(self, module: str, name: str, cb: Callable):
         self._mod_name_tracked_map[module][name] = cb
@@ -70,19 +71,40 @@
         for module_name, as_name in imp_names(node):
             if name_tracked_map := self._mod_name_tracked_map.get(module_name):
                 log.debug(f'Found module import: {module_name} as {as_name}')
                 for name, tracked in name_tracked_map.items():
                     self.scopes[f'{as_name}.{name}'] = tracked
 
     def visit_ImportFrom(self, node: ImportFrom):
-        if name_tracked_map := self._mod_name_tracked_map.get(node.module):
-            for name, as_name in imp_names(node):
-                if tracked := name_tracked_map.get(name):
-                    log.debug(f'Found tracked import: {node.module}.{name} as {as_name}')
-                    self.scopes[as_name] = tracked
+        """
+        Processes a ``from module import names`` statement.  If the module name matches one from which members were
+        registered to be tracked, then the imported names (and any ``as`` aliases) are processed.  Members with
+        canonical names that match an item that was registered to be tracked are added to the current scope / variable
+        namespace.
+
+        Relative module imports are handled fuzzily - no attempt is made to determine the fully qualified module name
+        for the source file or to resolve what the relative import's fully qualified module name would be.  This may
+        result in incorrect items being tracked if the name matched a tracked name in the matched tracked module.
+        """
+        if level := node.level:
+            # For absolute imports, the level is 0
+            # For relative imports, the level is a positive int, representing the number of relative package levels
+            matches = re.compile(r'[^.]+\.' * level + re.escape(node.module) + '$').search
+            for module, name_tracked_map in self._mod_name_tracked_map.items():
+                if matches(module):
+                    log.debug(f'Found fuzzy relative name match for {"." * level + node.module!r} to {module=}')
+                    self._maybe_track_import_from(node, name_tracked_map)
+        elif name_tracked_map := self._mod_name_tracked_map.get(node.module):
+            self._maybe_track_import_from(node, name_tracked_map)
+
+    def _maybe_track_import_from(self, node: ImportFrom, name_tracked_map):
+        for name, as_name in imp_names(node):
+            if tracked := name_tracked_map.get(name):
+                log.debug(f'Found tracked import: {node.module}.{name} as {as_name}')
+                self.scopes[as_name] = tracked
 
     # endregion
 
     # region Scope Changes
 
     @scoped
     def visit_For(self, node: For):
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/core.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/core.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/documentation.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/documentation.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/error_handling.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/error_handling.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/exceptions.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 # region User Errors
 
 
 class UsageError(CommandParserException):
     """Base exception for user errors"""
 
     message: str = None
+    # TODO: Document that this is a recommended exception type to use when performing manual input validation
 
 
 class ParamUsageError(UsageError):
     """Error raised when a Parameter was not used correctly"""
 
     def __init__(self, param: Optional[ParamOrGroup], message: str = None):
         self.param = param
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/commands.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/formatting/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,16 @@
         for param in params:
             self.maybe_add_option(param)
 
     def _iter_params(self) -> Iterator[Union[BasePositional, BaseOption, PassThru]]:
         params = self.params
         yield from params.all_positionals
         yield from params.options
-        if (pass_thru := params.pass_thru) is not None:
-            yield pass_thru
+        if params.pass_thru is not None:
+            yield params.pass_thru
 
     def _usage_parts(self, sub_cmd_choice: str = None, allow_sys_argv: Bool = True) -> Iterator[str]:
         yield 'usage:'
         yield self._meta.get_prog(allow_sys_argv)
         if sub_cmd_choice:
             yield sub_cmd_choice
         else:
@@ -187,27 +187,26 @@
 
         for cmd_name, choice in sub_command.choices.items():
             # TODO: There are some cases where multiple aliases for the same command (possibly local choices, possibly
             #  multiple choices all handled by a single class) would be better documented without separate sections for
             #  each choice value (should probably be configurable to explode or condense)
             choice_str = f'{choice_base} {cmd_name}' if choice_base else cmd_name
             yield from spaced_rst_header(f'Subcommand: {choice_str}', level)
-            if choice_help := choice.help:
-                yield choice_help
+            if choice.help:
+                yield choice.help
                 yield ''
 
             if (command := choice.target) is None:
                 # When choice.target is None, that means it is the default choice, pointing back to the same Command
                 yield from self._cmd_rst_lines(config, choice_str, allow_sys_argv)
             else:
                 params = get_params(command)
-                formatter = params.formatter
-                yield from formatter._cmd_rst_lines(config, choice_str, allow_sys_argv)
+                yield from params.formatter._cmd_rst_lines(config, choice_str, allow_sys_argv)
                 if nested_sub_cmd := params.sub_command:
-                    yield from formatter._sub_cmds_rst_lines(
+                    yield from params.formatter._sub_cmds_rst_lines(
                         config, nested_sub_cmd, level, choice_str, depth + 1, allow_sys_argv
                     )
 
     # endregion
 
 
 def _fix_name(name: str) -> str:
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/params.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/formatting/params.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,23 +40,22 @@
     @classmethod
     def for_param_cls(cls, param_cls: Type[ParamOrGroup]):
         try:
             return cls._param_cls_fmt_cls_map[param_cls]
         except KeyError:
             pass
 
-        for p_cls, f_cls in reversed(tuple(cls._param_cls_fmt_cls_map.items())):  # tuple() only for 3.7 compatibility
+        for p_cls, f_cls in reversed(cls._param_cls_fmt_cls_map.items()):
             if issubclass(param_cls, p_cls):
                 return f_cls
 
         return ParamHelpFormatter
 
     def __new__(cls, param: ParamOrGroup):
-        fmt_cls = cls.for_param_cls(param.__class__) if cls is ParamHelpFormatter else cls
-        return super().__new__(fmt_cls)
+        return super().__new__(cls.for_param_cls(param.__class__) if cls is ParamHelpFormatter else cls)
 
     def __init__(self, param: ParamOrGroup):
         self.param = param
 
     def maybe_wrap_usage(self, text: str) -> str:
         """
         Wraps the provided text in parentheses / brackets / etc based on whether the associated Parameter is required,
@@ -89,14 +88,27 @@
                 pass
             else:
                 if name != '<lambda>':
                     return name.upper()
 
         return param.name.upper()
 
+    def _format_usage_metavar(self, full: Bool = True) -> str:
+        metavar = self.format_metavar()
+        if not full:
+            return metavar
+
+        nargs: Nargs = self.param.nargs
+        variable = nargs.variable and nargs.max != 1
+        if 0 in nargs:
+            return f'[{metavar} ...]' if variable else f'[{metavar}]'
+        elif variable:
+            return f'{metavar} [{metavar} ...]'
+        return metavar
+
     def format_basic_usage(self) -> str:
         """Format the Parameter for use in the ``usage:`` line"""
         return self.maybe_wrap_usage(self.format_usage(True))
 
     def format_usage(self, include_meta: Bool = False, full: Bool = False, delim: str = ', ') -> str:
         """Format the Parameter for use in both the ``usage:`` line and in the list of Parameters"""
         return self.format_metavar()
@@ -132,34 +144,26 @@
     def rst_rows(self) -> Iterator[Tuple[str, str]]:
         yield self.rst_row()
 
     # endregion
 
 
 class PositionalHelpFormatter(ParamHelpFormatter, param_cls=BasePositional):
+    param: BasePositional
+
     def format_usage(self, include_meta: Bool = False, full: Bool = False, delim: str = ', ') -> str:
-        metavar = self.format_metavar()
-        return metavar if not full or self.param.nargs == 1 else f'{metavar} [{metavar} ...]'
+        return self._format_usage_metavar(full)
 
 
 class OptionHelpFormatter(ParamHelpFormatter, param_cls=BaseOption):
-    def _format_usage_metavar(self) -> str:
-        metavar = self.format_metavar()
-        nargs: Nargs = self.param.nargs
-        variable = nargs.variable and nargs.max != 1
-        if 0 in nargs:
-            return f'[{metavar} ...]' if variable else f'[{metavar}]'
-        elif variable:
-            return f'{metavar} [{metavar} ...]'
-        return metavar
+    param: BaseOption
 
     def iter_usage_parts(self, include_meta: Bool = False, full: Bool = False) -> Iterator[str]:
-        param: BaseOption = self.param
-        opts = param.option_strs
-        if param.nargs == 0:
+        opts = self.param.option_strs
+        if self.param.nargs == 0:
             yield from opts.option_strs()
         else:
             metavar = self._format_usage_metavar()
             yield from (f'{opt} {metavar}' for opt in opts.option_strs())
 
     def format_description(self, rst: Bool = False, description: str = None) -> str:
         description = super().format_description(rst, description)
@@ -174,17 +178,16 @@
 
         return description
 
     def format_usage(self, include_meta: Bool = False, full: Bool = False, delim: str = ', ') -> str:
         if full:
             return delim.join(self.iter_usage_parts())
 
-        param: BaseOption = self.param
-        opt = param.option_strs.get_usage_opt()
-        if not include_meta or param.nargs == 0:
+        opt = self.param.option_strs.get_usage_opt()
+        if not include_meta or self.param.nargs == 0:
             return opt
         return f'{opt} {self._format_usage_metavar()}'
 
     def rst_usage(self) -> str:
         return ', '.join(f'``{part}``' for part in self.iter_usage_parts())
 
 
@@ -197,61 +200,60 @@
             return f'{primary} | {alts}'
         else:
             return f'{opts.get_usage_opt(False)} | {opts.get_usage_opt(True)}'
 
     def format_description(self, rst: Bool = False, alt: bool = False) -> str:
         if not alt:
             return super().format_description(rst=rst)
-        if alt_help := self.param.alt_help:
-            return super().format_description(rst=rst, description=alt_help)
+        elif self.param.alt_help:
+            return super().format_description(rst=rst, description=self.param.alt_help)
         return ''
 
     def format_help(self, prefix: str = '', tw_offset: int = 0) -> str:
-        opts = self.param.option_strs
+        opts: TriFlagOptionStrings = self.param.option_strs
         primary = format_help_entry(opts.primary_option_strs(), self.format_description(), prefix, tw_offset)
         alt_desc = self.format_description(alt=True)
         alt_entry = format_help_entry(opts.alt_option_strs(), alt_desc, prefix, tw_offset, lpad=2 if alt_desc else 4)
         return f'{primary}\n{alt_entry}'
 
     def rst_rows(self) -> Iterator[Tuple[str, str]]:
-        opts = self.param.option_strs
+        opts: TriFlagOptionStrings = self.param.option_strs
         for alt in (False, True):
             usage = ', '.join(f'``{part}``' for part in opts.option_strs(alt))
-            description = self.format_description(rst=True, alt=alt)
-            yield usage, description
+            yield usage, self.format_description(rst=True, alt=alt)
 
 
 class ChoiceMapHelpFormatter(ParamHelpFormatter, param_cls=ChoiceMap):
+    param: ChoiceMap
+
     @cached_property
     def choice_groups(self) -> Iterable[ChoiceGroup]:
         return ChoiceGroup.group_choices(self.param.choices.values())
 
     def format_metavar(self) -> str:
-        param: ChoiceMap = self.param
-        if param.choices:
+        if self.param.choices:
             config = ctx.config
             choices = (str(c) for c in (c.choice for cg in self.choice_groups for c in cg.choices) if c is not None)
             if config.sort_choices:
                 choices = sorted(choices)
             return f'{{{config.choice_delim.join(choices)}}}'
         else:
-            return param.metavar or param.name.upper()
+            return self.param.metavar or self.param.name.upper()
 
     def format_usage(self, include_meta: Bool = False, full: Bool = False, delim: str = ', ') -> str:
         return self.format_metavar()
 
     def format_help(self, prefix: str = '', tw_offset: int = 0) -> str:
-        param: ChoiceMap = self.param
-        help_entry = format_help_entry(self.iter_usage_parts(), param.description, prefix, tw_offset, lpad=2)
+        help_entry = format_help_entry(self.iter_usage_parts(), self.param.description, prefix, tw_offset, lpad=2)
         choices = self._format_choices(prefix, tw_offset)
         if ctx.config.sort_choices:
             choices = sorted(choices)
 
         parts = (
-            f'{prefix}{param.title or param._default_title}:',
+            f'{prefix}{self.param.title or self.param._default_title}:',
             help_entry,
             *choices,
             prefix.rstrip(),
         )
         return '\n'.join(parts)
 
     def _format_choices(self, prefix: str = '', tw_offset: int = 0) -> Iterator[str]:
@@ -260,16 +262,15 @@
             yield from choice_group.format(mode, tw_offset, prefix)
 
     def rst_table(self) -> RstTable:
         rows = self._format_rst_rows()
         if ctx.config.sort_choices:
             rows = sorted(rows)
 
-        param = self.param
-        table = RstTable(param.title or param._default_title, param.description)
+        table = RstTable(self.param.title or self.param._default_title, self.param.description)
         table.add_rows(rows)
         return table
 
     def _format_rst_rows(self) -> Iterator[Tuple[str, OptStr]]:
         mode = ctx.config.cmd_alias_mode or SubcommandAliasHelpMode.ALIAS
         for choice_group in self.choice_groups:
             for choice, usage, description in choice_group.prepare(mode):
@@ -284,17 +285,16 @@
 
     Used for formatting help text based on the configured :attr:`.CommandConfig.cmd_alias_mode`.
     """
 
     __slots__ = ('choice_strs', 'choices')
 
     def __init__(self, choice: Choice):
-        choice_str = choice.choice
         self.choices = [choice]
-        self.choice_strs = [choice_str] if choice_str else []
+        self.choice_strs = [choice.choice] if choice.choice else []
 
     @classmethod
     def group_choices(cls, choices: Iterable[Choice]) -> Iterable[ChoiceGroup]:
         """
         Processes the given Choices to group them by target and configured help text.  If two choices have the same
         target but different help text values, then they are considered different, so they are not grouped together.
 
@@ -309,16 +309,16 @@
             except KeyError:
                 target_choice_map[key] = cls(choice)
 
         return target_choice_map.values()
 
     def add(self, choice: Choice):
         self.choices.append(choice)
-        if choice_str := choice.choice:
-            self.choice_strs.append(choice_str)
+        if choice.choice:
+            self.choice_strs.append(choice.choice)
 
     def format(self, default_mode: CmdAliasMode, tw_offset: int = 0, prefix: str = '') -> Iterator[str]:
         """
         :param default_mode: The default :class:`.SubcommandAliasHelpMode` to use if no mode was explicitly configured,
           or the format string to use for subcommand aliases.
         :param tw_offset: Terminal width offset for text width calculations.
         :param prefix: Prefix to add to every line (primarily intended for use with nested groups).
@@ -333,19 +333,18 @@
         mode.
 
         :param default_mode: The default :class:`.SubcommandAliasHelpMode` to use if no mode was explicitly configured,
           or the format string to use for subcommand aliases.
         :return: Generator that yields 3-tuples containing the :class:`.Choice` object, the choice string value, and
           the help text / description for that choice / alias.
         """
-        first = self.choices[0]
         # If it's not a Command, get_config will return None.  If it is a Command, then it will use its config.  If the
         # alias mode is not set on that target Command, but it is set on its parent, then this will use that parent's
         # setting.
-        if config := get_config(first.target):
+        if config := get_config(self.choices[0].target):
             mode = config.cmd_alias_mode or default_mode
         else:
             mode = default_mode
 
         if mode == SubcommandAliasHelpMode.ALIAS:
             yield from self.prepare_aliases()
         elif mode == SubcommandAliasHelpMode.REPEAT:
@@ -413,29 +412,28 @@
 
 
 class PassThruHelpFormatter(ParamHelpFormatter, param_cls=PassThru):
     required_formatter_map = {True: '-- {}'.format, False: '[-- {}]'.format}
 
 
 class GroupHelpFormatter(ParamHelpFormatter, param_cls=ParamGroup):  # noqa  # pylint: disable=W0223
+    param: ParamGroup
     required_formatter_map: BoolFormatterMap = {True: '{{{}}}'.format, False: '[{}]'.format}
 
     def _get_choice_delim(self) -> str:
-        param: ParamGroup = self.param
-        if param.mutually_dependent:
+        if self.param.mutually_dependent:
             return ' + '
-        elif param.mutually_exclusive:
+        elif self.param.mutually_exclusive:
             return ' | '
         else:
             return ', '
 
     def format_usage(self, include_meta: Bool = False, full: Bool = False, delim: str = ', ') -> str:
-        choice_delim = self._get_choice_delim()
-        members = choice_delim.join(mem.formatter.format_usage(include_meta, full, delim) for mem in self.param.members)
-        return self.maybe_wrap_usage(choice_delim.join(members))
+        members = (mem.formatter.format_usage(include_meta, full, delim) for mem in self.param.members)
+        return self.maybe_wrap_usage(self._get_choice_delim().join(members))
 
     def format_description(self, rst: Bool = False, description: str = None) -> str:
         if description:
             return description
         group = self.param
         if group.description or group._name:
             description = group.description or f'{group.name} options'
@@ -445,47 +443,44 @@
         elif ctx.config.show_group_type and (group.mutually_exclusive or group.mutually_dependent):
             return f'Mutually {"exclusive" if group.mutually_exclusive else "dependent"} options'
 
         adjective = 'Required' if group.required else 'Other' if group.contains_required else 'Optional'
         return f'{adjective} arguments'
 
     def _get_spacer(self) -> str:
-        group = self.param
-        if group.mutually_exclusive:
+        # TODO: Config option to set these chars OR to have them just be spaces
+        if self.param.mutually_exclusive:
             return '\u00A6 '  # BROKEN BAR
-        elif group.mutually_dependent:
+        elif self.param.mutually_dependent:
             return '\u2551 '  # BOX DRAWINGS DOUBLE VERTICAL
         else:
             return '\u2502 '  # BOX DRAWINGS LIGHT VERTICAL
 
     def format_help(self, prefix: str = '', tw_offset: int = 0, clean: Bool = True) -> str:
         """
         Prepare the help text for this group.
 
         :param prefix: Prefix to add to every line (primarily intended for use with nested groups)
         :param tw_offset: Terminal width offset for text width calculations
         :param clean: If this group only contains other groups or Action or SubCommand parameters, then omit the
           description.
         :return: The formatted help text.
         """
-        description = self.format_description()
-        parts = [f'{prefix}{description}:']
-
         if ctx.config.show_group_tree:
             spacer = prefix + self._get_spacer()
             tw_offset += 2
         else:
             spacer = prefix
 
-        nested, params = 0, 0
+        parts = [f'{prefix}{self.format_description()}:']
+        nested = params = 0
         for member in self.param.members:
             if not member.show_in_help:
                 continue
-
-            if isinstance(member, (ChoiceMap, ParamGroup)):
+            elif isinstance(member, (ChoiceMap, ParamGroup)):
                 nested += 1
                 parts.append(spacer.rstrip())  # Add space for readability
             else:
                 params += 1
             parts.append(member.formatter.format_help(prefix=spacer, tw_offset=tw_offset))
 
         if clean and nested and not params:
@@ -511,10 +506,9 @@
                     sub_table.show_title = False
                     table.add_row(sub_table.title, str(sub_table))
 
         return table
 
 
 def _pad_and_quote(description: str, rst: bool) -> Tuple[str, str]:
-    pad = ' ' if description else ''
-    quote = '``' if rst else ''
-    return pad, quote
+    """Returns a 2-tuple of ``(pad char, quote string)``"""
+    return ' ' if description else '', '``' if rst else ''
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/restructured_text.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/formatting/restructured_text.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/utils.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/formatting/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/__init__.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/base.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/base.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/choices.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/choices.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
     """
 
     __slots__ = ()
     choices: Mapping[Any, T]
 
     def __init__(self, choices: Mapping[Any, T], *args, **kwargs):
         super().__init__(choices, *args, **kwargs)
+        # TODO: Alternate ChoiceMap where values are used as help text, similar to SubCommand with local_choices
 
     def __call__(self, value: str) -> T:
         value = self._normalize(value)
         for val in self._iter_normalized(value):
             try:
                 return self.choices[val]
             except KeyError:
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/exceptions.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/exceptions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/files.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,17 @@
     """
     :param kwargs: Additional keyword arguments to pass to :class:`.File`
     """
 
     def __init__(self, *, mode: str = 'rb', **kwargs):
         import json
 
+        # TODO: catch JSONDecodeError and provide a standardized cleaner error message (with a way to disable this error handling)
+        # TODO: Update docs to not suggest importing `inputs as i`
+
         write = allows_write(mode, True)
         kwargs['pass_file'] = write  # json.load just calls loads with f.read()
         super().__init__(json.dump if write else json.loads, mode=mode, **kwargs)
 
 
 class Pickle(Serialized):
     """
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/numeric.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/numeric.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/patterns.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/patterns.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,16 +120,16 @@
         if (mode := self.mode) == RegexMode.STRING:
             return value
         elif mode == RegexMode.MATCH:
             return m
         elif mode == RegexMode.GROUP:
             return m.group(self.group)
         elif mode == RegexMode.GROUPS:
-            if groups := self.groups:
-                return tuple(m.group(g) for g in groups)
+            if self.groups:
+                return tuple(m.group(g) for g in self.groups)
             return m.groups()
         else:  # mode == RegexMode.DICT
             return m.groupdict()
 
 
 class Glob(PatternInput[str]):
     """
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/time.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,24 +52,24 @@
     __slots__ = ('locale', 'original')
 
     def __init__(self, locale: Optional[Locale]):
         self.locale = locale
 
     def __enter__(self):
         self._lock.acquire()
-        if not (locale := self.locale):
+        if not self.locale:
             return
         # locale.getlocale does not support LC_ALL, but `setlocale(LC_ALL)` with no locale to set will return a str
         # containing all of the current locale settings as `key1=val1;key2=val2;...;keyN=valN`
         self.original = setlocale(LC_ALL)
         # The calendar.different_locale implementation only calls setlocale with LC_TIME, which caused LC_CTYPE
         # to remain set to `English_United States.1252` on Windows 10, which resulted in incorrectly encoded results.
         # Using f'LC_CTYPE={locale};LC_TIME={locale}' seemed cleaner than setting LC_ALL in its entirety, but it
         # resulted in `locale.Error: unsupported locale setting` on Ubuntu/WSL.
-        setlocale(LC_ALL, locale)
+        setlocale(LC_ALL, self.locale)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self.locale:
             setlocale(LC_ALL, self.original)
         self._lock.release()
 
 
@@ -208,21 +208,21 @@
 
         raise InvalidChoiceError(value, self.choices(), self.dt_type)
 
     def __call__(self, value: str) -> Union[str, int]:
         normalized = self.parse(value)
         if normalized < self._min_index:
             raise InvalidChoiceError(value, self.choices(), self.dt_type)
-        elif (out_mode := self.out_format) in (DTFormatMode.NUMERIC, DTFormatMode.NUMERIC_ISO):
-            return self._formats[out_mode][normalized]
-        elif (names_or_abbreviations := self._formats.get(out_mode)) is not None:
+        elif self.out_format in (DTFormatMode.NUMERIC, DTFormatMode.NUMERIC_ISO):
+            return self._formats[self.out_format][normalized]
+        elif (names_or_abbreviations := self._formats.get(self.out_format)) is not None:
             with different_locale(self.out_locale):
                 return names_or_abbreviations[normalized]
 
-        raise ValueError(f'Unexpected output format={out_mode!r} for {self.dt_type}={normalized}')
+        raise ValueError(f'Unexpected output format={self.out_format!r} for {self.dt_type}={normalized}')
 
 
 class Day(CalendarUnitInput, dt_type='day of the week'):
     __slots__ = ('iso',)
     _formats = {
         DTFormatMode.FULL: day_name,
         DTFormatMode.ABBREVIATION: day_abbr,
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/utils.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/inputs/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/metadata.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/metadata.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 """
 # pylint: disable=R0801
 
 from __future__ import annotations
 
 from collections import defaultdict
 from functools import cached_property
-from importlib.metadata import entry_points, EntryPoint
+from importlib.metadata import entry_points, EntryPoint, Distribution
 from inspect import getmodule
 from pathlib import Path
 from sys import modules
 from textwrap import dedent
-from typing import TYPE_CHECKING, Any, Type, Callable, Optional, Union, Iterator, Tuple, Dict
+from typing import TYPE_CHECKING, Any, Type, Callable, Optional, Union, Iterator, Tuple, Dict, Set
 from urllib.parse import urlparse
 
 from .context import ctx, NoActiveContext
 
 if TYPE_CHECKING:
     from .typing import Bool, CommandType, OptStr
 
@@ -56,15 +56,15 @@
             instance.__dict__[self.name] = value
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}({", ".join(f"{a}={v}" for a, v in self._attrs())})'
 
     def _attrs(self) -> Iterator[Tuple[str, Any]]:
         for base in self.__class__.mro()[:-1]:
-            for attr in base.__slots__:
+            for attr in base.__slots__:  # noqa
                 if attr != 'name':
                     value = getattr(self, attr)
                     yield attr, (getattr(value, '__qualname__', value) if attr == 'func' else repr(value))
 
     def get_parent(self, instance: ProgramMetadata) -> Optional[ProgramMetadata]:
         # if (parent := instance.parent) and parent.distribution == instance.distribution:
         if (parent := instance.parent) and parent.package == instance.package:
@@ -107,23 +107,20 @@
 
 # endregion
 
 
 class ProgramMetadata:
     _fields = {'parent'}
     parent: Optional[ProgramMetadata] = None
+    distribution: Distribution | None = Metadata(None, inheritable=False)
     path: Path = Metadata(None, inheritable=False)
     package: str = Metadata(None, inheritable=False)
     module: str = Metadata(None, inheritable=False)
     cmd_module: str = Metadata(None, inheritable=False)
     command: str = Metadata(None, inheritable=False)
-    url: str = Metadata(None)
-    docs_url: str = Metadata(None)
-    email: str = Metadata(None)
-    version: str = Metadata('')
     usage: str = Metadata(None)
     description: str = Metadata(None)
     epilog: str = Metadata(None)
     doc_str: str = Metadata('')
     pkg_doc_str: str = Metadata('')  # Set by :func:`~.documentation.load_commands` to capture package docstrings
 
     def __init__(self, **kwargs):
@@ -152,27 +149,28 @@
         version: str = None,
         usage: str = None,
         description: str = None,
         epilog: str = None,
         doc_name: str = None,
     ) -> ProgramMetadata:
         path, g = _path_and_globals(command, path)
-        if (cmd_module := command.__module__) != 'cli_command_parser.commands':
+        if command.__module__ != 'cli_command_parser.commands':
             # Prevent inheritors from getting docstrings from the base Command
             doc_str = g.get('__doc__')
             doc = command.__doc__
         else:
             doc = doc_str = None
 
         return cls(
             parent=parent,
+            distribution=_dist_finder.dist_for_obj(command),
             path=path,
             package=g.get('__package__'),
             module=g.get('__module__'),
-            cmd_module=cmd_module,
+            cmd_module=command.__module__,
             command=command.__qualname__,
             prog=prog,
             url=url or g.get('__url__'),
             docs_url=docs_url,
             email=email or g.get('__author_email__'),
             version=version or g.get('__version__'),
             usage=usage,
@@ -207,21 +205,49 @@
         return self._get_prog(allow_sys_argv)[0]
 
     def _get_prog(self, allow_sys_argv: Bool = None) -> Tuple[str, str]:
         return self._prog_and_src if allow_sys_argv or allow_sys_argv is None else self._doc_prog_and_src
 
     @dynamic_metadata(inheritable=False)
     def doc_name(self) -> str:
+        # TODO: Bug: Explicitly provided value not used in rst page title sometimes?
         return Path(self._doc_prog_and_src[0]).stem
 
     # endregion
 
     @dynamic_metadata
+    def version(self) -> str:
+        if dist := self.distribution:
+            return dist.version
+        return ''
+
+    @dynamic_metadata
+    def email(self) -> OptStr:
+        if dist := self.distribution:
+            if email := dist.metadata['Author-email']:
+                # TODO: `Maintainer-email` instead if it's defined?  Is there a more appropriate key?
+                # https://packaging.python.org/en/latest/specifications/core-metadata/#core-metadata
+                return email
+        return None
+
+    @dynamic_metadata
+    def url(self) -> OptStr:
+        if (dist := self.distribution) and (urls := _dist_finder.get_urls(dist)):
+            for key in ('Source', 'Source Code', 'Home-page'):
+                if url := urls.get(key):
+                    return url
+        return None
+
+    @dynamic_metadata
     def docs_url(self) -> OptStr:
-        return _docs_url_from_repo_url(self.url)
+        if (dist := self.distribution) and (urls := _dist_finder.get_urls(dist)):
+            for key in ('Documentation', 'Docs', 'Doc', 'Home-page'):
+                if url := urls.get(key):
+                    return url
+        return _docs_url_from_repo_url(self.url)  # noqa
 
     def format_epilog(self, extended: Bool = True, allow_sys_argv: Bool = None) -> str:
         parts = [self.epilog] if self.epilog else []
         if parts and not extended:
             return parts[0]
 
         if version := self.version:
@@ -272,15 +298,15 @@
         return mod_obj_prog_map
 
     @classmethod
     def _get_console_scripts(cls) -> Tuple[EntryPoint, ...]:
         try:
             return entry_points(group='console_scripts')  # noqa
         except TypeError:  # Python 3.8 or 3.9
-            return entry_points()['console_scripts']
+            return entry_points()['console_scripts']  # noqa
 
     def normalize(
         self,
         cmd_path: Path,
         parent: Optional[ProgramMetadata],
         allow_sys_argv: Bool,
         cmd_module: str,
@@ -347,14 +373,85 @@
 
         return None
 
 
 _prog_finder = ProgFinder()
 
 
+class DistributionFinder:
+    def __init__(self):
+        self._dist_top_levels = {}
+        self._dist_urls = {}
+
+    @cached_property
+    def _distributions(self) -> dict[str, Distribution]:
+        # Note: Distribution.name was not added until 3.10, and it returns `self.metadata['Name']`
+        return {dist.metadata['Name']: dist for dist in Distribution.discover()}
+
+    def _get_top_levels(self, dist_name: str, dist: Distribution) -> Set[str]:
+        # dist_name = dist.metadata['Name']  # Distribution.name was not added until 3.10, and it returns this
+        if (top_levels := self._dist_top_levels.get(dist_name)) is not None:
+            return top_levels
+        elif raw := dist.read_text('top_level.txt'):
+            self._dist_top_levels[dist_name] = top_levels = {pkg for pkg in map(str.strip, raw.split()) if pkg}
+            return top_levels
+
+        # Below logic is copied from importlib.metadata._top_level_inferred from 3.10+
+        self._dist_top_levels[dist_name] = inferred = {
+            f.parts[0] if len(f.parts) > 1 else f.with_suffix('').name for f in dist.files if f.suffix == '.py'
+        }
+        return inferred
+
+    def dist_for_pkg(self, pkg_name: str) -> Distribution | None:
+        for dist_name, dist in self._distributions.items():
+            if pkg_name in self._get_top_levels(dist_name, dist):
+                return dist
+        return None
+
+    def dist_for_obj(self, obj) -> Distribution | None:
+        try:
+            mod_name: str = obj.__module__
+        except AttributeError:
+            return None
+
+        if mod_name == '__main__':  # May need to handle __mp_main__ and similar too
+            return self._dist_for_obj_main(obj)
+        return self.dist_for_pkg(mod_name.split('.', 1)[0])
+
+    def _dist_for_obj_main(self, obj) -> Distribution | None:
+        # Note: getmodule returns the module object (obj.__module__ only provides the name)
+        if (module := getmodule(obj)) is None or not module.__package__:
+            return None
+
+        # The package name may have a prefix like `lib` not included in top_level when interactive
+        for part in module.__package__.split('.'):
+            if (dist := self.dist_for_pkg(part)) is not None:
+                return dist
+        return None
+
+    def get_urls(self, dist: Distribution) -> Dict[str, str]:
+        metadata = dist.metadata
+        dist_name = metadata['Name']
+        if (urls := self._dist_urls.get(dist_name)) is not None:
+            return urls
+
+        urls = {}
+        for key, val in metadata.items():
+            if key == 'Home-page':
+                urls[key] = val
+            elif key == 'Project-URL':
+                url_type, url = val.split(',', 1)
+                urls[url_type.strip()] = url.strip()
+        self._dist_urls[dist_name] = urls
+        return urls
+
+
+_dist_finder = DistributionFinder()
+
+
 def _path_and_globals(command: CommandType, path: Path = None) -> Tuple[Path, Dict[str, Any]]:
     module = getmodule(command)  # Returns the module object (obj.__module__ just provides the name of the module)
     if path is None:
         try:
             path = Path(module.__file__).resolve()
         except AttributeError:  # module is None
             path = Path.cwd().joinpath(DEFAULT_FILE_NAME)
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/nargs.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/nargs.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/actions.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/actions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/base.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,24 +63,25 @@
     hide: Bool                      #: Whether this param/group should be hidden in ``--help`` text
 
     def __init__(self, name: str = None, required: Bool = False, help: str = None, hide: Bool = False):  # noqa
         self.__doc__ = help  # Prevent this class's docstring from showing up for params in generated documentation
         self.required = required
         self.help = help
         self.hide = hide
+        # TODO: Make the --help flag a counter and allow some `hide=True` params to be shown with `-hh` or similar?
         self.name = name
         if param_groups := _group_stack.get(None):  # If truthy, there's at least 1 active ParamGroup
             param_groups[-1].register(self)  # This sets self.group = group
 
     # region Name
 
     @property
     def name(self) -> str:
-        if (name := self._name) is not None:
-            return name
+        if self._name is not None:
+            return self._name
         return self._default_name()
 
     @name.setter
     def name(self, value: Optional[str]):
         if value is not None:
             self._name = value
 
@@ -150,23 +151,31 @@
 
     Custom parameter classes should generally extend :class:`BasePositional` or :class:`BaseOption` instead of this,
     otherwise additional handling may be necessary in the parser.
 
     :param action: The action to take on individual parsed values.  Actions must be defined as methods in classes
       that extend Parameter, and must be registered via :class:`parameter_action`.
     :param name: The name to use for this parameter.  Defaults to the name assigned to this parameter.
-    :param default: The default value for this parameter if it is not specified.  Defaults to ``None`` if this
-      parameter is not required; not used if it is required.
     :param required: Whether this parameter is required or not.  If it is required, then an exception will be
       raised if the user did not provide a value for this parameter.  Defaults to ``False``.
     :param metavar: The name to use as a placeholder for values in usage / help messages.
     :param help: A brief description of this parameter that will appear in ``--help`` text.
-    :param hide: If ``True``, this parameter will not be included in usage / help messages.  Defaults to ``False``.
+    :param default: The default value for this parameter if it is not specified.  Defaults to ``None`` if this
+      parameter is not required; not used if it is required.
+    :param default_cb: A default callback function (or other callable) may be provided instead of a static default
+      value (they cannot both be provided).  If ``cb_with_cmd`` is False (the default), then it must be callable with
+      no arguments, otherwise it must accept a single positional argument (the :class:`.Command` that contains this
+      Parameter).  Similar to when the ``default`` value would be used, it will only be called when no argument was
+      provided.  It is also possible to :ref:`register a method in a Command to be the default callback
+      <advanced:Dynamic Parameter Defaults>`.
+    :param cb_with_cmd: Whether the provided ``default_cb`` should be called with the :class:`.Command` that contains
+      this Parameter.  Ignored if ``default_cb`` is not provided.
     :param show_default: Override the :attr:`.CommandConfig.show_defaults` setting for this parameter to always or
       never include the default value in usage / help messages.  Default: follow the ``show_defaults`` setting.
+    :param hide: If ``True``, this parameter will not be included in usage / help messages.  Defaults to ``False``.
     """
 
     # region Attributes & Initialization
 
     # Class attributes
     _action_map: Dict[str, Type[ParamAction]] = {}
     _repr_attrs: Optional[Strings] = None           #: Attributes to include in ``repr()`` output
@@ -200,14 +209,15 @@
         help: str = None,  # noqa
         hide: Bool = False,
         metavar: str = None,
         name: str = None,
         required: Bool = False,
         default: Any = _NotSet,
         default_cb: DefaultFunc = None,
+        cb_with_cmd: Bool = False,
         show_default: Bool = None,
         strict_default: Bool = False,
     ):
         if not (param_action := self._action_map.get(action)):
             self._handle_bad_action(action)
         if required and default is not _NotSet:
             # TODO: For required mutually dependent groups, or a required group with all params having a default,
@@ -222,15 +232,15 @@
         if default is not _NotSet:
             if default_cb is not None:
                 raise ParameterDefinitionError(
                     f'{self.__class__.__name__}s can only have a {default=} xor {default_cb=}, not both'
                 )
             self.default = default
         elif default_cb is not None:
-            self.default_cb = DefaultCallback(default_cb)
+            self.default_cb = DefaultCallback(default_cb, cb_with_cmd)
         self.strict_default = strict_default
         if show_default is not None:
             self.show_default = show_default
 
     def _handle_bad_action(self, action: str) -> NoReturn:
         """
         Called when an action not supported by this type of Parameter was provided.  May be overwritten in subclasses
@@ -257,16 +267,16 @@
             self.type.type = annotated_type
         else:  # self.type must be None
             # Choices present earlier would have already been converted
             self.type = normalize_input_type(annotated_type, None)
 
     @property
     def has_choices(self) -> bool:
-        if type_attr := self.type:
-            return isinstance(type_attr, _ChoicesBase) and type_attr.choices
+        if self.type:
+            return isinstance(self.type, _ChoicesBase) and self.type.choices
         return False
 
     def register_default_cb(self, method: CommandMethod) -> CommandMethod:
         """
         Intended to be used as a decorator to register a method in a Command to be used as the default callback for
         this Parameter.  The method will only be called during parsing if no value was explicitly provided for this
         Parameter.  The decorated method is returned unchanged, so it can still be called directly if necessary.
@@ -289,16 +299,16 @@
         self.default_cb = DefaultCallback(method, True)
         return method
 
     # endregion
 
     def __repr__(self) -> str:
         names = ('action', 'const', 'default', 'default_cb', 'type', 'choices', 'required', 'hide', 'help')
-        if extra_attrs := self._repr_attrs:
-            names = chain(names, extra_attrs)
+        if self._repr_attrs:
+            names = chain(names, self._repr_attrs)
 
         skip = (None, _NotSet)
         attrs = (
             (a, str(v) if a == 'action' else v)
             for a in names
             if (v := getattr(self, a, None)) not in skip and not (a == 'hide' and not v)
         )
@@ -364,27 +374,30 @@
         with self._ctx(command):
             value = self.result(command)
 
         if self._attr_name:
             command.__dict__[self._attr_name] = value  # Skip __get__ on subsequent accesses
         return value
 
-    def result_value(self, command: CommandObj | None = None, missing_default: TD = _NotSet) -> Union[T_co, TD, None]:
-        value = ctx.get_parsed_value(self)
-        if value is _NotSet:
-            if self.required:
-                if missing_default is _NotSet:
-                    raise MissingArgument(self)
-                return missing_default
-            else:
+    def result(self, command: CommandObj | None = None, missing_default: TD = _NotSet) -> Union[T_co, TD, None]:
+        """The final result / parsed value for this Parameter that is returned upon access as a descriptor."""
+        if (value := ctx.get_parsed_value(self)) is not _NotSet:
+            return self.action.finalize_value(value)
+        elif self.required:
+            if missing_default is _NotSet:
+                raise MissingArgument(self)
+            return missing_default
+        else:
+            try:
                 return self.action.get_default(command, missing_default)
-
-        return self.action.finalize_value(value)
-
-    result = result_value
+            except InputValidationError as e:
+                # At this point, a default value was provided when this param was defined, but it wasn't acceptable
+                # TODO: Do any of the other cases handled by the `prepare_value` method need to be checked here?
+                #  Need to test choices - a non-acceptable choice may make sense as the default in some cases
+                raise BadArgument(self, f'bad default value - {e}') from e
 
     # endregion
 
     # region Usage / Help Text
 
     @property
     def show_in_help(self) -> bool:
@@ -500,24 +513,24 @@
     def _handle_bad_action(self, action: str) -> NoReturn:
         if action in ('store', 'append') and (fixed := f'{action}_const') in self._action_map:
             raise ParameterDefinitionError(f'Invalid {action=} for {self.__class__.__name__} - did you mean {fixed!r}?')
         super()._handle_bad_action(action)
 
     def __set_name__(self, command: CommandCls, name: str):
         super().__set_name__(command, name)
-        if not (option_strs := self.option_strs).name_mode:
-            option_strs.name_mode = self._config(command).option_name_mode
-        option_strs.update(name)
+        if not self.option_strs.name_mode:
+            self.option_strs.name_mode = self._config(command).option_name_mode
+        self.option_strs.update(name)
 
     def env_vars(self) -> Iterator[str]:
-        if env_var := self.env_var:
-            if isinstance(env_var, str):
-                yield env_var
+        if self.env_var:
+            if isinstance(self.env_var, str):
+                yield self.env_var
             else:
-                yield from env_var
+                yield from self.env_var
 
     def get_const(self, opt_str: OptStr = None):
         return self.const
 
 
 class AllowLeadingDashProperty:
     """
@@ -552,20 +565,20 @@
             value = AllowLeadingDash.ALWAYS
 
         if value is not None:
             instance.__dict__[self.name] = value
 
 
 class DefaultCallback:
-    __slots__ = ('func', 'is_method')
+    __slots__ = ('func', 'use_cmd')
 
-    def __init__(self, func: CommandMethod | DefaultFunc, is_method: bool = False):
+    def __init__(self, func: CommandMethod | DefaultFunc, use_cmd: bool = False):
         self.func = func
-        self.is_method = is_method
+        self.use_cmd = use_cmd
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__}({self.func!r}, is_method={self.is_method})>'
+        return f'<{self.__class__.__name__}({self.func!r}, use_cmd={self.use_cmd})>'
 
     def __call__(self, command: CommandObj | None) -> T_co:
-        # If the func is not a method, then `command` must not be None, but the default callback is intentionally
-        # not called by ParamAction.get_default (and its subclasses) when command is None.
-        return self.func(command) if self.is_method else self.func()
+        # If the func isn't a method / doesn't accept the command, then `command` must not be None, but the default
+        # callback is intentionally not called by ParamAction.get_default (and its subclasses) when command is None.
+        return self.func(command) if self.use_cmd else self.func()
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/choice_map.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/choice_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,36 +150,34 @@
         raise CommandDefinitionError(f'No choices were registered for {self}')
 
     # endregion
 
     # region Argument Handling
 
     def validate(self, value: str, joined: Bool = False):
-        if not (choices := self.choices):
+        if not self.choices:
             self._no_choices_error()
 
         parsed = ctx.get_parsed_value(self)
         values = (value,) if parsed is _NotSet else (*parsed, value)
-        if (choice := ' '.join(values)) in choices:
+        if (choice := ' '.join(values)) in self.choices:
             return
         elif len(values) > self.nargs.max:
             raise BadArgument(self, 'too many values')
         prefix = choice + ' '
-        if not any(c.startswith(prefix) for c in choices if c):
-            raise InvalidChoice(self, prefix[:-1], choices)
+        if not any(c.startswith(prefix) for c in self.choices if c):
+            raise InvalidChoice(self, prefix[:-1], self.choices)
 
-    def result_value(self, command: CommandObj | None = None, missing_default: TD = _NotSet) -> Union[OptStr, TD]:
+    def result(self, command: CommandObj | None = None, missing_default: TD = _NotSet) -> Union[OptStr, TD]:
         if not self.choices:
             self._no_choices_error()
-        return super().result_value(command, missing_default)
-
-    result = result_value
+        return super().result(command, missing_default)
 
     def target(self) -> T:
-        return self.choices[self.result_value(None)].target
+        return self.choices[self.result(None)].target
 
     # endregion
 
     # region Usage / Help Text
 
     @property
     def show_in_help(self) -> bool:
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/groups.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,16 +56,24 @@
         description: str = None,
         mutually_exclusive: Bool = False,
         mutually_dependent: Bool = False,
         required: Bool = False,
         hide: Bool = False,
     ):
         super().__init__(name=name, required=required, hide=hide)
+
+        # TODO: In a large group containing, say, 4 items, where 2 are mutually dependent / must both be provided if any
+        #  are provided, and 2 other items that are optional, but require those others to be defined, the
+        #  mutual_dependent / required handling needs to be refined.
+        #  Concrete example: fluentbit parser name/format are both required if either is specified, and a regex pattern
+        #  / type MAY be provided, but only if the name/format is also provided
+
         self._num = next(_GROUP_COUNTER)
         self.description = description
+        # TODO: Description from docstring just inside with block?  Is it possible?
         self.members = []
         if mutually_dependent and mutually_exclusive:
             name = self.name or 'Options'
             raise ParameterDefinitionError(f'group={name!r} cannot be both mutually_exclusive and mutually_dependent')
         self.mutually_exclusive = mutually_exclusive
         self.mutually_dependent = mutually_dependent
 
@@ -91,24 +99,21 @@
 
     def __lt__(self, other: ParamGroup) -> bool:
         # Sort order places nested groups before their parent groups
         if not isinstance(other, ParamGroup):
             return NotImplemented
         elif self in other.members:
             return True
-
-        group = self.group
-        other_group = other.group
-        if group != other_group:
-            if group is None:
+        elif self.group != other.group:
+            if self.group is None:
                 return False
-            elif other_group is None:
+            elif other.group is None:
                 return True
             else:
-                return group < other_group
+                return self.group < other.group
 
         # Even if a name was not explicitly provided, the auto-generated one from self._default_name() is returned here
         return self.name < other.name
 
     def __contains__(self, param: ParamOrGroup) -> bool:
         """
         Returns True if the given :class:`Parameter` or :class:`ParamGroup` is a member of this group, False otherwise.
@@ -204,17 +209,17 @@
             be = 'was' if len(provided) == 1 else 'were'
             raise ParamsMissing(missing, f'because {p_str} {be} provided')
         elif self.mutually_exclusive and not 0 <= len(provided) < 2:
             raise ParamConflict(provided, 'they are mutually exclusive - only one is allowed')
 
     @property
     def in_mutually_exclusive_group(self) -> bool:
-        if not (parent := self.group):
-            return False
-        return parent.mutually_exclusive
+        if not self.group:
+            return False  # This group has no parent group
+        return self.group.mutually_exclusive
 
     def validate(self):
         """
         Validate mutual dependency / exclusivity of members and that required members have been provided when they are
         expected to be (based on mutual dependence/exclusivity and nesting).
 
         This method is called during parsing, after initially parsing arguments, before evaluating whether a subcommand
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/option_strings.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/option_strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,17 +135,17 @@
             self._long.add(option)
             if mode_val & 8:  # OptionNameMode.BOTH_UNDERSCORE = OptionNameMode.DASH | 4 | 8
                 self._display_long.add(option)
 
     @property
     def alt_allowed(self) -> Set[str]:
         allowed = set(self._alt_long)
-        if short := self._alt_short:
-            allowed.add(short)
-            allowed.add(short[1:])
+        if self._alt_short:
+            allowed.add(self._alt_short)
+            allowed.add(self._alt_short[1:])
         return allowed
 
     # @property
     # def long_primary(self) -> List[str]:
     #     return [opt for opt in self.long if opt not in self._alt_long]
 
     @property
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/options.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,23 +403,17 @@
         self.func = func
         return self
 
     def __get__(self, command: Optional[CommandObj], owner: CommandCls) -> Union[ActionFlag, Callable]:
         # Allow the method to be called, regardless of whether it was specified
         if command is None:
             return self
+        # Note: If func is None, then CommandParameters._process_action_flags raises ParameterDefinitionError
         return partial(self.func, command)  # imitates a bound method
 
-    def result(self, command: CommandObj | None = None) -> Optional[Callable]:
-        if self.result_value(command):
-            if self.func:
-                return self.func
-            raise ParameterDefinitionError(f'No function was registered for {self}')
-        return None
-
 
 #: Alias for :class:`ActionFlag`
 action_flag = ActionFlag  # pylint: disable=C0103
 
 
 def before_main(*option_strs: str, order: Union[int, float] = 1, func: Callable = None, **kwargs) -> ActionFlag:
     """An ActionFlag that will be executed before :meth:`.Command.main`"""
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/pass_thru.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/pass_thru.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/positionals.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/parameters/positionals.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/parse_tree.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/parse_tree.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/parser.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 raise
             return None
 
     def get_next_cmd(self, ctx: Context) -> Optional[CommandType]:
         self._parse_args(ctx)
         self._validate_groups()
         missing = ctx.get_missing()
-        if (sub_cmd_param := self.params.sub_command) and (next_cmd := sub_cmd_param.target()) is not None:
+        if self.params.sub_command and (next_cmd := self.params.sub_command.target()) is not None:
             if missing and not ctx.categorized_action_flags[_PRE_INIT] and get_parent(next_cmd) is not ctx.command_cls:
                 raise ParamsMissing(missing)
             return next_cmd
         elif missing and not ctx.config.allow_missing and (not self.params.action or self.params.action not in missing):
             if not ctx.categorized_action_flags[_PRE_INIT]:  # No pre-init action was triggered
                 raise ParamsMissing(missing)
         elif ctx.remaining and not ctx.config.ignore_unknown:  # Note: ctx.remaining is self.deferred at this point
@@ -175,28 +175,28 @@
             found += param.action.add_value(arg_deque.popleft())
         return found
 
     # endregion
 
     def handle_positional(self, arg: str):
         # log.debug(f'handle_positional({arg=})')
-        if positionals := self.positionals:
-            param: BasePositional = positionals.pop(0)
+        if self.positionals:
+            param: BasePositional = self.positionals.pop(0)
             if param.nargs.max is REMAINDER:
                 self.handle_remainder(param, arg)
             else:
                 try:
                     found = param.action.add_value(arg)
                 except UsageError:
-                    positionals.insert(0, param)
+                    self.positionals.insert(0, param)
                     raise
                 try:
                     self.consume_values(param, found=found)
                 except Backtrack:
-                    positionals.insert(0, param)
+                    self.positionals.insert(0, param)
                 else:
                     self._last = param
         else:
             self.deferred.append(arg)
 
     # region Option Handling
 
@@ -275,17 +275,17 @@
         Parameter being processed accepts a variable number of arguments, then check to see if it's possible to
         backtrack to move some of those values to the remaining positionals.
 
         :param param: The :class:`.Parameter` that was consuming values when the arg_deque became empty
         :param found: The number of values that were consumed by the given Parameter
         :return: The updated found count, if backtracking was possible, otherwise the unmodified found count
         """
-        if positionals := self.positionals:
+        if self.positionals:
             can_pop = param.action.get_maybe_poppable_counts()
-            if rollback_count := _to_pop(positionals, can_pop, found - 1):
+            if rollback_count := _to_pop(self.positionals, can_pop, found - 1):
                 self.arg_deque.extendleft(reversed(self.ctx.roll_back_parsed_values(param, rollback_count)))
                 return found - rollback_count
         return found
 
     def _maybe_backtrack_last(self, param: BasePositional, found: int):
         """
         Similar to :meth:`._maybe_backtrack`, but allows backtracking even after starting to process a Positional.
@@ -341,14 +341,17 @@
 
             try:
                 found += param.action.add_value(value)
             except UsageError as e:
                 # log.debug(f'{value=} was rejected by {param=}', exc_info=True)
                 return self._finalize_consume(param, value, found, e)
 
+        # TODO: Positional(nargs='?') with no values will steal values intended for an Option(nargs='+')
+        #  (likely occurs with nargs='*' for the Positional as well)
+
         # log.debug(f'Ran out of values in deque while processing {param=}')
         if found >= 2 and self.config.allow_backtrack:
             found = self._maybe_backtrack(param, found)
         return self._finalize_consume(param, None, found)
 
     def _finalize_consume(self, param: Parameter, value: OptStr, found: int, exc: Optional[Exception] = None) -> int:
         nargs = param.nargs
@@ -360,16 +363,16 @@
             # log.debug(f'consume_values {found=} for {param=}')
             return found
         elif exc:
             raise exc
         elif self._last and isinstance(param, BasePositional) and param.action.can_reset():
             self._maybe_backtrack_last(param, found)
 
-        s = '' if (n := nargs.min) == 1 else 's'
-        raise MissingArgument(param, f'expected {n} value{s}, but only found {found}')
+        s = '' if nargs.min == 1 else 's'
+        raise MissingArgument(param, f'expected {nargs.min} value{s}, but only found {found}')
 
 
 parse_args_and_get_next_cmd = CommandParser.parse_args_and_get_next_cmd
 
 
 def _to_pop(positionals: Iterable[BasePositional], can_pop: List[int], available: int, req_mod: int = 0) -> int:
     if not can_pop:
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/testing.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,24 +90,26 @@
     # def subTest(self, *args, **kwargs):
     #     print()
     #     return super().subTest(*args, **kwargs)
 
     def assert_dict_equal(self, d1, d2, msg: str = None):
         self.assertIsInstance(d1, dict, 'First argument is not a dictionary')
         self.assertIsInstance(d2, dict, 'Second argument is not a dictionary')
+        self._assert_dict_equal(d1, d2, msg)
+
+    def _assert_dict_equal(self, d1, d2, msg: str = None):
         if d1 != d2:
             self.fail(self._formatMessage(msg, f'{d1} != {d2}\n{format_dict_diff(d1, d2)}'))
 
     def assert_raises_contains_str(self, expected_exc: Type[BaseException], expected_text: str, msg: str = None):
         return AssertRaisesWithStringContext(self, expected_exc, expected_text, msg)
 
     def assert_parse_results(self, cmd_cls: CommandCls, argv: Argv, expected: Expected, msg: str = None) -> Command:
         cmd = cmd_cls.parse(argv)
-        parsed = cmd.ctx.get_parsed(cmd, exclude=EXCLUDE_ACTIONS)
-        self.assert_dict_equal(expected, parsed, msg)
+        self._assert_dict_equal(expected, cmd.ctx.get_parsed(cmd, exclude=EXCLUDE_ACTIONS), msg)
         return cmd
 
     def assert_parse_results_cases(self, cmd_cls: CommandCls, cases: Iterable[Case], msg: str = None):
         for argv, expected in cases:
             with self.subTest(expected='results', argv=argv):
                 self.assert_parse_results(cmd_cls, argv, expected, msg)
 
@@ -216,17 +218,15 @@
 
 def _colored(text: str, color: int, end: str = '\n'):
     return f'\x1b[38;5;{color}m{text}\x1b[0m{end}'
 
 
 def format_diff(a: str, b: str, name_a: str = 'expected', name_b: str = '  actual', n: int = 3) -> str:
     sio = StringIO()
-    a = a.splitlines()
-    b = b.splitlines()
-    for i, line in enumerate(unified_diff(a, b, name_a, name_b, n=n, lineterm='')):
+    for i, line in enumerate(unified_diff(a.splitlines(), b.splitlines(), name_a, name_b, n=n, lineterm='')):
         if line.startswith('+') and i > 1:
             sio.write(_colored(line, 2))
         elif line.startswith('-') and i > 1:
             sio.write(_colored(line, 1))
         elif line.startswith('@@ '):
             sio.write(_colored(line, 6, '\n\n'))
         else:
@@ -258,17 +258,15 @@
                 if val_a == val_b:
                     formatted_a.append(str_a)
                     formatted_b.append(str_b)
                 else:
                     formatted_a.append(_colored(str_a, 2, ''))
                     formatted_b.append(_colored(str_b, 1, ''))
 
-    kvs_a = ', '.join(formatted_a)
-    kvs_b = ', '.join(formatted_b)
-    return f'- {{{kvs_a}}}\n+ {{{kvs_b}}}'
+    return f'- {{{", ".join(formatted_a)}}}\n+ {{{", ".join(formatted_b)}}}'
 
 
 # endregion
 
 
 class RedirectStreams(AbstractContextManager):
     _stdin: Union[IO, str, bytes, None] = None
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/typing.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,9 +56,9 @@
 ParamOrGroup = Union[Param, 'ParamGroup']
 
 CommandObj = TypeVar('CommandObj', bound='Command')
 CommandType = TypeVar('CommandType', bound='CommandMeta')
 CommandCls = Union[CommandType, Type[CommandObj]]
 CommandAny = Union[CommandCls, CommandObj]
 
-DefaultFunc = Callable[[], T_co]
 CommandMethod = Callable[[CommandObj], T_co]
+DefaultFunc = Union[Callable[[], T_co], CommandMethod]
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser/utils.py` & `cli_command_parser-2024.4.20/lib/cli_command_parser/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
 from enum import Flag, EnumMeta
+from inspect import isawaitable
 from shutil import get_terminal_size
 from time import monotonic
-from typing import Any, Callable, TypeVar, List
+from typing import Any, Callable, TypeVar, Awaitable, List
 
 try:
     from enum import CONFORM
 except ImportError:
     CONFORM = None
 
 try:
     from wcwidth import wcwidth
 except ImportError:
     wcwidth = len
 
 FlagEnum = TypeVar('FlagEnum', bound='FixedFlag')
+T = TypeVar('T')
 _NotSet = object()
 
 # region Text Processing / Formatting
 
 
 def camel_to_snake_case(text: str, delim: str = '_') -> str:
     return ''.join(f'{delim}{c}' if i and c.isupper() else c for i, c in enumerate(text)).lower()
@@ -136,15 +138,15 @@
                     return tmp
 
         raise KeyError
 
     def _decompose(self) -> List[FlagEnum]:
         if self._name_ is None or '|' in self._name_:  # | check is for 3.11 where pseudo-members are assigned names
             val = self._value_
-            return sorted(mem for mem in self.__class__ if (mem_val := mem._value_) & val == mem_val)  # noqa
+            return sorted(mem for mem in self.__class__ if mem._value_ & val == mem._value_)  # noqa
         return [self]
 
     def __lt__(self, other: FlagEnum) -> bool:
         return self._value_ < other._value_
 
 
 class Terminal:  # pylint: disable=R0903
@@ -180,7 +182,13 @@
     try:
         value = int(value)
     except (ValueError, TypeError) as e:
         raise TypeError(f'Invalid {value=} - expected {expected} >= {min_val}') from e
     if value < min_val:
         raise ValueError(f'Invalid {value=} - expected {expected} >= {min_val}')
     return value
+
+
+async def maybe_await(obj: T | Awaitable[T]) -> T:
+    if isawaitable(obj):
+        return await obj
+    return obj
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/PKG-INFO` & `cli_command_parser-2024.4.20/lib/cli_command_parser.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 Metadata-Version: 2.1
-Name: cli-command-parser
-Version: 2023.7.30
+Name: cli_command_parser
+Version: 2024.4.20
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
+Project-URL: Documentation, https://dskrypa.github.io/cli_command_parser
+Project-URL: Issues, https://github.com/dskrypa/cli_command_parser/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 Provides-Extra: wcwidth
+Requires-Dist: wcwidth; extra == "wcwidth"
 Provides-Extra: conversion
-License-File: LICENSE
+Requires-Dist: astunparse; python_version < "3.9" and extra == "conversion"
 
 CLI Command Parser
 ##################
 
 |downloads| |py_version| |coverage_badge| |build_status| |Blue|
 
-.. |py_version| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue
+.. |py_version| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12%20-blue
     :target: https://pypi.org/project/cli-command-parser/
 
 .. |coverage_badge| image:: https://codecov.io/gh/dskrypa/cli_command_parser/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/dskrypa/cli_command_parser
 
 .. |build_status| image:: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml
@@ -110,15 +115,15 @@
     $ pip install -U cli-command-parser[wcwidth]
 
 
 Python Version Compatibility
 ============================
 
 Python versions 3.8 and above are currently supported.  The last release of CLI Command Parser that supported 3.7 was
-2023-04-30.  Support for Python 3.7 `officially ends on 2023-06-27 <https://devguide.python.org/versions/>`__.
+2023-04-30.  Support for Python 3.7 `officially ended on 2023-06-27 <https://devguide.python.org/versions/>`__.
 
 When using Python 3.8, some additional packages that backport functionality that was added in later Python versions
 are required for compatibility.
 
 To use the argparse to cli-command-parser conversion script with Python 3.8, there is a dependency on
 `astunparse <https://astunparse.readthedocs.io>`__.  If you are using Python 3.9 or above, then ``astunparse`` is not
 necessary because the relevant code was added to the stdlib ``ast`` module.  If you're unsure, you can install
```

### Comparing `cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/SOURCES.txt` & `cli_command_parser-2024.4.20/lib/cli_command_parser.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 MANIFEST.in
+entry_points.txt
 pyproject.toml
 readme.rst
 requirements-dev.txt
 setup.cfg
 lib/cli_command_parser/__init__.py
 lib/cli_command_parser/__main__.py
 lib/cli_command_parser/__version__.py
@@ -23,20 +24,22 @@
 lib/cli_command_parser/parser.py
 lib/cli_command_parser/testing.py
 lib/cli_command_parser/typing.py
 lib/cli_command_parser/utils.py
 lib/cli_command_parser.egg-info/PKG-INFO
 lib/cli_command_parser.egg-info/SOURCES.txt
 lib/cli_command_parser.egg-info/dependency_links.txt
+lib/cli_command_parser.egg-info/entry_points.txt
 lib/cli_command_parser.egg-info/requires.txt
 lib/cli_command_parser.egg-info/top_level.txt
 lib/cli_command_parser/conversion/__init__.py
 lib/cli_command_parser/conversion/__main__.py
 lib/cli_command_parser/conversion/argparse_ast.py
 lib/cli_command_parser/conversion/argparse_utils.py
+lib/cli_command_parser/conversion/cli.py
 lib/cli_command_parser/conversion/command_builder.py
 lib/cli_command_parser/conversion/utils.py
 lib/cli_command_parser/conversion/visitor.py
 lib/cli_command_parser/formatting/__init__.py
 lib/cli_command_parser/formatting/commands.py
 lib/cli_command_parser/formatting/params.py
 lib/cli_command_parser/formatting/restructured_text.py
```

### Comparing `cli_command_parser-2023.7.30/readme.rst` & `cli_command_parser-2024.4.20/readme.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 CLI Command Parser
 ##################
 
 |downloads| |py_version| |coverage_badge| |build_status| |Blue|
 
-.. |py_version| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue
+.. |py_version| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12%20-blue
     :target: https://pypi.org/project/cli-command-parser/
 
 .. |coverage_badge| image:: https://codecov.io/gh/dskrypa/cli_command_parser/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/dskrypa/cli_command_parser
 
 .. |build_status| image:: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml
@@ -82,15 +82,15 @@
     $ pip install -U cli-command-parser[wcwidth]
 
 
 Python Version Compatibility
 ============================
 
 Python versions 3.8 and above are currently supported.  The last release of CLI Command Parser that supported 3.7 was
-2023-04-30.  Support for Python 3.7 `officially ends on 2023-06-27 <https://devguide.python.org/versions/>`__.
+2023-04-30.  Support for Python 3.7 `officially ended on 2023-06-27 <https://devguide.python.org/versions/>`__.
 
 When using Python 3.8, some additional packages that backport functionality that was added in later Python versions
 are required for compatibility.
 
 To use the argparse to cli-command-parser conversion script with Python 3.8, there is a dependency on
 `astunparse <https://astunparse.readthedocs.io>`__.  If you are using Python 3.9 or above, then ``astunparse`` is not
 necessary because the relevant code was added to the stdlib ``ast`` module.  If you're unsure, you can install
```

### Comparing `cli_command_parser-2023.7.30/setup.cfg` & `cli_command_parser-2024.4.20/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -10,72 +10,85 @@
 00000090: 3a2f 2f67 6974 6875 622e 636f 6d2f 6473  ://github.com/ds
 000000a0: 6b72 7970 612f 636c 695f 636f 6d6d 616e  krypa/cli_comman
 000000b0: 645f 7061 7273 6572 0d0a 7072 6f6a 6563  d_parser..projec
 000000c0: 745f 7572 6c73 203d 200d 0a09 536f 7572  t_urls = ...Sour
 000000d0: 6365 203d 2068 7474 7073 3a2f 2f67 6974  ce = https://git
 000000e0: 6875 622e 636f 6d2f 6473 6b72 7970 612f  hub.com/dskrypa/
 000000f0: 636c 695f 636f 6d6d 616e 645f 7061 7273  cli_command_pars
-00000100: 6572 0d0a 6c69 6365 6e73 6520 3d20 4170  er..license = Ap
-00000110: 6163 6865 2032 2e30 0d0a 6c69 6365 6e73  ache 2.0..licens
-00000120: 655f 6669 6c65 7320 3d20 4c49 4345 4e53  e_files = LICENS
-00000130: 450d 0a6c 6f6e 675f 6465 7363 7269 7074  E..long_descript
-00000140: 696f 6e20 3d20 6669 6c65 3a20 7265 6164  ion = file: read
-00000150: 6d65 2e72 7374 0d0a 6c6f 6e67 5f64 6573  me.rst..long_des
-00000160: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
-00000170: 5f74 7970 6520 3d20 7465 7874 2f78 2d72  _type = text/x-r
-00000180: 7374 0d0a 6175 7468 6f72 203d 2044 6f75  st..author = Dou
-00000190: 6720 536b 7279 7061 0d0a 6175 7468 6f72  g Skrypa..author
-000001a0: 5f65 6d61 696c 203d 2064 736b 7279 7061  _email = dskrypa
-000001b0: 4067 6d61 696c 2e63 6f6d 0d0a 636c 6173  @gmail.com..clas
-000001c0: 7369 6669 6572 7320 3d20 0d0a 0944 6576  sifiers = ...Dev
-000001d0: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-000001e0: 3a3a 2035 202d 2050 726f 6475 6374 696f  :: 5 - Productio
-000001f0: 6e2f 5374 6162 6c65 0d0a 0945 6e76 6972  n/Stable...Envir
-00000200: 6f6e 6d65 6e74 203a 3a20 436f 6e73 6f6c  onment :: Consol
-00000210: 650d 0a09 496e 7465 6e64 6564 2041 7564  e...Intended Aud
-00000220: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
-00000230: 6572 730d 0a09 4c69 6365 6e73 6520 3a3a  ers...License ::
-00000240: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-00000250: 2041 7061 6368 6520 536f 6674 7761 7265   Apache Software
-00000260: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
-00000270: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-00000280: 5320 496e 6465 7065 6e64 656e 740d 0a09  S Independent...
-00000290: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000002a0: 7561 6765 203a 3a20 5079 7468 6f6e 0d0a  uage :: Python..
-000002b0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000002c0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002d0: 3a3a 2033 0d0a 0950 726f 6772 616d 6d69  :: 3...Programmi
-000002e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000002f0: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
-00000300: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000310: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000320: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
-00000330: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000340: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
-00000350: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000360: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000370: 3a20 332e 3131 0d0a 0954 6f70 6963 203a  : 3.11...Topic :
-00000380: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-00000390: 6f70 6d65 6e74 203a 3a20 5573 6572 2049  opment :: User I
-000003a0: 6e74 6572 6661 6365 730d 0a09 546f 7069  nterfaces...Topi
-000003b0: 6320 3a3a 2054 6578 7420 5072 6f63 6573  c :: Text Proces
-000003c0: 7369 6e67 0d0a 0d0a 5b6f 7074 696f 6e73  sing....[options
-000003d0: 5d0d 0a69 6e63 6c75 6465 5f70 6163 6b61  ]..include_packa
-000003e0: 6765 5f64 6174 6120 3d20 5472 7565 0d0a  ge_data = True..
-000003f0: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
-00000400: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
-00000410: 3d20 6c69 620d 0a70 7974 686f 6e5f 7265  = lib..python_re
-00000420: 7175 6972 6573 203d 203e 3d33 2e38 0d0a  quires = >=3.8..
-00000430: 7465 7374 735f 7265 7175 6972 6520 3d20  tests_require = 
-00000440: 7465 7374 746f 6f6c 733b 2063 6f76 6572  testtools; cover
-00000450: 6167 650d 0a0d 0a5b 6f70 7469 6f6e 732e  age....[options.
-00000460: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
-00000470: 7768 6572 6520 3d20 6c69 620d 0a0d 0a5b  where = lib....[
-00000480: 6f70 7469 6f6e 732e 6578 7472 6173 5f72  options.extras_r
-00000490: 6571 7569 7265 5d0d 0a77 6377 6964 7468  equire]..wcwidth
-000004a0: 203d 200d 0a09 7763 7769 6474 680d 0a63   = ...wcwidth..c
-000004b0: 6f6e 7665 7273 696f 6e20 3d20 0d0a 0961  onversion = ...a
-000004c0: 7374 756e 7061 7273 653b 2070 7974 686f  stunparse; pytho
-000004d0: 6e5f 7665 7273 696f 6e3c 2233 2e39 220d  n_version<"3.9".
-000004e0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-000004f0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000500: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000100: 6572 0d0a 0944 6f63 756d 656e 7461 7469  er...Documentati
+00000110: 6f6e 203d 2068 7474 7073 3a2f 2f64 736b  on = https://dsk
+00000120: 7279 7061 2e67 6974 6875 622e 696f 2f63  rypa.github.io/c
+00000130: 6c69 5f63 6f6d 6d61 6e64 5f70 6172 7365  li_command_parse
+00000140: 720d 0a09 4973 7375 6573 203d 2068 7474  r...Issues = htt
+00000150: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000160: 6473 6b72 7970 612f 636c 695f 636f 6d6d  dskrypa/cli_comm
+00000170: 616e 645f 7061 7273 6572 2f69 7373 7565  and_parser/issue
+00000180: 730d 0a6c 6963 656e 7365 203d 2041 7061  s..license = Apa
+00000190: 6368 6520 322e 300d 0a6c 6963 656e 7365  che 2.0..license
+000001a0: 5f66 696c 6573 203d 204c 4943 454e 5345  _files = LICENSE
+000001b0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000001c0: 6f6e 203d 2066 696c 653a 2072 6561 646d  on = file: readm
+000001d0: 652e 7273 740d 0a6c 6f6e 675f 6465 7363  e.rst..long_desc
+000001e0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+000001f0: 7479 7065 203d 2074 6578 742f 782d 7273  type = text/x-rs
+00000200: 740d 0a61 7574 686f 7220 3d20 446f 7567  t..author = Doug
+00000210: 2053 6b72 7970 610d 0a61 7574 686f 725f   Skrypa..author_
+00000220: 656d 6169 6c20 3d20 6473 6b72 7970 6140  email = dskrypa@
+00000230: 676d 6169 6c2e 636f 6d0d 0a63 6c61 7373  gmail.com..class
+00000240: 6966 6965 7273 203d 200d 0a09 4465 7665  ifiers = ...Deve
+00000250: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
+00000260: 3a20 3520 2d20 5072 6f64 7563 7469 6f6e  : 5 - Production
+00000270: 2f53 7461 626c 650d 0a09 456e 7669 726f  /Stable...Enviro
+00000280: 6e6d 656e 7420 3a3a 2043 6f6e 736f 6c65  nment :: Console
+00000290: 0d0a 0949 6e74 656e 6465 6420 4175 6469  ...Intended Audi
+000002a0: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
+000002b0: 7273 0d0a 094c 6963 656e 7365 203a 3a20  rs...License :: 
+000002c0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+000002d0: 4170 6163 6865 2053 6f66 7477 6172 6520  Apache Software 
+000002e0: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
+000002f0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+00000300: 2049 6e64 6570 656e 6465 6e74 0d0a 0950   Independent...P
+00000310: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000320: 6167 6520 3a3a 2050 7974 686f 6e0d 0a09  age :: Python...
+00000330: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000340: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000350: 3a20 330d 0a09 5072 6f67 7261 6d6d 696e  : 3...Programmin
+00000360: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000370: 7468 6f6e 203a 3a20 332e 380d 0a09 5072  thon :: 3.8...Pr
+00000380: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000390: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000003a0: 332e 390d 0a09 5072 6f67 7261 6d6d 696e  3.9...Programmin
+000003b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000003c0: 7468 6f6e 203a 3a20 332e 3130 0d0a 0950  thon :: 3.10...P
+000003d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000003e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000003f0: 2033 2e31 310d 0a09 5072 6f67 7261 6d6d   3.11...Programm
+00000400: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000410: 5079 7468 6f6e 203a 3a20 332e 3132 0d0a  Python :: 3.12..
+00000420: 0954 6f70 6963 203a 3a20 536f 6674 7761  .Topic :: Softwa
+00000430: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
+00000440: 3a20 5573 6572 2049 6e74 6572 6661 6365  : User Interface
+00000450: 730d 0a09 546f 7069 6320 3a3a 2054 6578  s...Topic :: Tex
+00000460: 7420 5072 6f63 6573 7369 6e67 0d0a 0d0a  t Processing....
+00000470: 5b6f 7074 696f 6e73 5d0d 0a69 6e63 6c75  [options]..inclu
+00000480: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
+00000490: 3d20 5472 7565 0d0a 656e 7472 795f 706f  = True..entry_po
+000004a0: 696e 7473 203d 2066 696c 653a 2065 6e74  ints = file: ent
+000004b0: 7279 5f70 6f69 6e74 732e 7478 740d 0a70  ry_points.txt..p
+000004c0: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
+000004d0: 0a70 6163 6b61 6765 5f64 6972 203d 203d  .package_dir = =
+000004e0: 206c 6962 0d0a 7079 7468 6f6e 5f72 6571   lib..python_req
+000004f0: 7569 7265 7320 3d20 3e3d 332e 380d 0a74  uires = >=3.8..t
+00000500: 6573 7473 5f72 6571 7569 7265 203d 2074  ests_require = t
+00000510: 6573 7474 6f6f 6c73 3b20 636f 7665 7261  esttools; covera
+00000520: 6765 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  ge....[options.p
+00000530: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+00000540: 6865 7265 203d 206c 6962 0d0a 0d0a 5b6f  here = lib....[o
+00000550: 7074 696f 6e73 2e65 7874 7261 735f 7265  ptions.extras_re
+00000560: 7175 6972 655d 0d0a 7763 7769 6474 6820  quire]..wcwidth 
+00000570: 3d20 0d0a 0977 6377 6964 7468 0d0a 636f  = ...wcwidth..co
+00000580: 6e76 6572 7369 6f6e 203d 200d 0a09 6173  nversion = ...as
+00000590: 7475 6e70 6172 7365 3b20 7079 7468 6f6e  tunparse; python
+000005a0: 5f76 6572 7369 6f6e 3c22 332e 3922 0d0a  _version<"3.9"..
+000005b0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+000005c0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+000005d0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

