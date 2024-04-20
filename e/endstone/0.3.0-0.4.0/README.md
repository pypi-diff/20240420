# Comparing `tmp/endstone-0.3.0.tar.gz` & `tmp/endstone-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endstone-0.3.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "endstone-0.4.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `endstone-0.3.0.tar` & `endstone-0.4.0.tar`

### file list

```diff
@@ -1,180 +1,281 @@
--rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 endstone-0.3.0/.clang-format
--rw-r--r--   0        0        0     4224 2022-11-09 12:37:21.000000 endstone-0.3.0/.clang-tidy
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 endstone-0.3.0/.dockerignore
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 endstone-0.3.0/.git_archival.txt
--rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 endstone-0.3.0/.github/conan_profiles/linux
--rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 endstone-0.3.0/.github/conan_profiles/windows
--rw-r--r--   0        0        0     2221 2022-11-09 12:37:21.000000 endstone-0.3.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1628 2022-11-09 12:37:21.000000 endstone-0.3.0/.github/workflows/docker.yml
--rw-r--r--   0        0        0     1854 2022-11-09 12:37:21.000000 endstone-0.3.0/.github/workflows/linux.yml
--rw-r--r--   0        0        0     5120 2022-11-09 12:37:21.000000 endstone-0.3.0/.github/workflows/wheel.yml
--rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 endstone-0.3.0/.github/workflows/windows.yml
--rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 endstone-0.3.0/.gitignore
--rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 endstone-0.3.0/.readthedocs.yaml
--rw-r--r--   0        0        0     3751 2022-11-09 12:37:21.000000 endstone-0.3.0/CMakeLists.txt
--rw-r--r--   0        0        0     2534 2022-11-09 12:37:21.000000 endstone-0.3.0/Dockerfile
--rw-r--r--   0        0        0    11356 2022-11-09 12:37:21.000000 endstone-0.3.0/LICENSE
--rw-r--r--   0        0        0     8645 2022-11-09 12:37:21.000000 endstone-0.3.0/README.md
--rw-r--r--   0        0        0       88 2022-11-09 12:37:21.000000 endstone-0.3.0/codecov.yml
--rw-r--r--   0        0        0     6297 2022-11-09 12:37:21.000000 endstone-0.3.0/conanfile.py
--rw-r--r--   0        0        0      315 2022-11-09 12:37:21.000000 endstone-0.3.0/docker-compose.yml
--rw-r--r--   0        0        0      491 2022-11-09 12:37:21.000000 endstone-0.3.0/docs/index.md
--rw-r--r--   0        0        0       16 2022-11-09 12:37:21.000000 endstone-0.3.0/docs/requirements.txt
--rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/bedrock.h
--rw-r--r--   0        0        0     1772 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/bedrock_log.h
--rw-r--r--   0        0        0     1506 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/command/command.h
--rw-r--r--   0        0        0     2823 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/command/command_flag.h
--rw-r--r--   0        0        0     4708 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/command/command_origin.h
--rw-r--r--   0        0        0     1996 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/command/command_output.h
--rw-r--r--   0        0        0      806 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/command/command_permission_level.h
--rw-r--r--   0        0        0    12032 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/command/command_registry.h
--rw-r--r--   0        0        0      715 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/command/command_version.h
--rw-r--r--   0        0        0     1224 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/command/minecraft_commands.h
--rw-r--r--   0        0        0      780 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/common.h
--rw-r--r--   0        0        0      704 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/core.h
--rw-r--r--   0        0        0     1705 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/forward.h
--rw-r--r--   0        0        0      943 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/i18n.h
--rw-r--r--   0        0        0      814 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/minecraft.h
--rw-r--r--   0        0        0     2452 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/network/game/available_commands_packet.h
--rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/network/packet.h
--rw-r--r--   0        0        0      813 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/network/packet_sender.h
--rw-r--r--   0        0        0     5387 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/server/level/player.h
--rw-r--r--   0        0        0      854 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/server/level/server_player.h
--rw-r--r--   0        0        0     1057 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/server/server_instance.h
--rw-r--r--   0        0        0      936 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/type_id.h
--rw-r--r--   0        0        0      841 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/uuid.h
--rw-r--r--   0        0        0    10445 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/world/actor/actor.h
--rw-r--r--   0        0        0     3163 2022-11-09 12:37:21.000000 endstone-0.3.0/include/bedrock/world/actor/mob.h
--rw-r--r--   0        0        0     7632 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/command/command.h
--rw-r--r--   0        0        0     1419 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/command/command_executor.h
--rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/command/command_map.h
--rw-r--r--   0        0        0     2055 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/command/command_sender.h
--rw-r--r--   0        0        0     2767 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/command/plugin_command.h
--rw-r--r--   0        0        0     1014 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/command/bedrock_command.h
--rw-r--r--   0        0        0     1870 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/command/command_adapter.h
--rw-r--r--   0        0        0     2908 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/command/command_lexer.h
--rw-r--r--   0        0        0     1514 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/command/command_map.h
--rw-r--r--   0        0        0     1751 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/command/command_sender.h
--rw-r--r--   0        0        0     1494 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/command/command_usage_parser.h
--rw-r--r--   0        0        0     1018 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/command/defaults/plugins_command.h
--rw-r--r--   0        0        0     1162 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/command/defaults/version_command.h
--rw-r--r--   0        0        0      842 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/command/endstone_command.h
--rw-r--r--   0        0        0     1094 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/command/server_command_sender.h
--rw-r--r--   0        0        0     6256 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/hook.h
--rw-r--r--   0        0        0      863 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/logger_factory.h
--rw-r--r--   0        0        0      903 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/os.h
--rw-r--r--   0        0        0     1542 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/permissions/default_permissions.h
--rw-r--r--   0        0        0     2606 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/permissions/permissible_base.h
--rw-r--r--   0        0        0     1252 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/plugin/cpp_plugin_loader.h
--rw-r--r--   0        0        0     5358 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/plugin/plugin_description_builder.h
--rw-r--r--   0        0        0     3530 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/plugin/plugin_manager.h
--rw-r--r--   0        0        0     1255 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/plugin/python_plugin_loader.h
--rw-r--r--   0        0        0     2397 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/server.h
--rw-r--r--   0        0        0     1254 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/singleton.h
--rw-r--r--   0        0        0     1055 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/spdlog/level_formatter.h
--rw-r--r--   0        0        0     3174 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/spdlog/log_sink.h
--rw-r--r--   0        0        0     1193 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/spdlog/spdlog_adapter.h
--rw-r--r--   0        0        0     3229 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/detail/spdlog/text_formatter.h
--rw-r--r--   0        0        0     1165 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/endstone.h
--rw-r--r--   0        0        0     3490 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/logger.h
--rw-r--r--   0        0        0     3961 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/permissions/permissible.h
--rw-r--r--   0        0        0     5773 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/permissions/permission.h
--rw-r--r--   0        0        0     4597 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/permissions/permission_attachment.h
--rw-r--r--   0        0        0     2204 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/permissions/permission_attachment_info.h
--rw-r--r--   0        0        0      796 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/permissions/permission_default.h
--rw-r--r--   0        0        0     1221 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/permissions/server_operator.h
--rw-r--r--   0        0        0     6667 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/plugin/plugin.h
--rw-r--r--   0        0        0     7486 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/plugin/plugin_description.h
--rw-r--r--   0        0        0     1042 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/plugin/plugin_load_order.h
--rw-r--r--   0        0        0     2746 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/plugin/plugin_loader.h
--rw-r--r--   0        0        0     7719 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/plugin/plugin_manager.h
--rw-r--r--   0        0        0     2544 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/server.h
--rw-r--r--   0        0        0     2855 2022-11-09 12:37:21.000000 endstone-0.3.0/include/endstone/util/color_format.h
--rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 endstone-0.3.0/mkdocs.yml
--rw-r--r--   0        0        0     1957 2022-11-09 12:37:21.000000 endstone-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 endstone-0.3.0/python/.gitignore
--rw-r--r--   0        0        0      140 2022-11-09 12:37:21.000000 endstone-0.3.0/python/src/endstone/__init__.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 endstone-0.3.0/python/src/endstone/_internal/__init__.py
--rw-r--r--   0        0        0     3130 2022-11-09 12:37:21.000000 endstone-0.3.0/python/src/endstone/_internal/bootstrap/__init__.py
--rw-r--r--   0        0        0    10393 2022-11-09 12:37:21.000000 endstone-0.3.0/python/src/endstone/_internal/bootstrap/base.py
--rw-r--r--   0        0        0     2178 2022-11-09 12:37:21.000000 endstone-0.3.0/python/src/endstone/_internal/bootstrap/linux.py
--rw-r--r--   0        0        0     6831 2022-11-09 12:37:21.000000 endstone-0.3.0/python/src/endstone/_internal/bootstrap/windows.py
--rw-r--r--   0        0        0    22943 2022-11-09 12:37:21.000000 endstone-0.3.0/python/src/endstone/_internal/endstone_python.pyi
--rw-r--r--   0        0        0     4090 2022-11-09 12:37:21.000000 endstone-0.3.0/python/src/endstone/_internal/plugin_loader.py
--rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 endstone-0.3.0/python/src/endstone/_internal/version.py
--rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 endstone-0.3.0/python/src/endstone/command.py
--rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 endstone-0.3.0/python/src/endstone/logger.py
--rw-r--r--   0        0        0      277 2022-11-09 12:37:21.000000 endstone-0.3.0/python/src/endstone/permissions.py
--rw-r--r--   0        0        0     3842 2022-11-09 12:37:21.000000 endstone-0.3.0/python/src/endstone/plugin.py
--rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 endstone-0.3.0/python/src/endstone/server.py
--rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 endstone-0.3.0/python/src/endstone/util.py
--rw-r--r--   0        0        0     1635 2022-11-09 12:37:21.000000 endstone-0.3.0/python/tests/test_color_format.py
--rw-r--r--   0        0        0      506 2022-11-09 12:37:21.000000 endstone-0.3.0/python/tests/test_imports.py
--rw-r--r--   0        0        0     2315 2022-11-09 12:37:21.000000 endstone-0.3.0/python/tests/test_plugin_description.py
--rw-r--r--   0        0        0     1004 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/command/bedrock_command.cpp
--rw-r--r--   0        0        0     4621 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/command/command_adapter.cpp
--rw-r--r--   0        0        0     3153 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/command/command_lexer.cpp
--rw-r--r--   0        0        0     8683 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/command/command_map.cpp
--rw-r--r--   0        0        0     2194 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/command/command_sender.cpp
--rw-r--r--   0        0        0     4793 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/command/command_usage_parser.cpp
--rw-r--r--   0        0        0     2003 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/command/defaults/plugins_command.cpp
--rw-r--r--   0        0        0     3938 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/command/defaults/version_command.cpp
--rw-r--r--   0        0        0     1325 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/command/server_command_sender.cpp
--rw-r--r--   0        0        0     1514 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/logger_factory.cpp
--rw-r--r--   0        0        0     2556 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/permissions/default_permissions.cpp
--rw-r--r--   0        0        0     6393 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/permissions/permissible_base.cpp
--rw-r--r--   0        0        0     4831 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/plugin/cpp_plugin_loader.cpp
--rw-r--r--   0        0        0     9057 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/plugin/plugin_manager.cpp
--rw-r--r--   0        0        0     3852 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/server.cpp
--rw-r--r--   0        0        0     1553 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/spdlog/level_formatter.cpp
--rw-r--r--   0        0        0     3586 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/spdlog/log_sink.cpp
--rw-r--r--   0        0        0     1415 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/spdlog/spdlog_adapter.cpp
--rw-r--r--   0        0        0     2239 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_core/spdlog/text_formatter.cpp
--rw-r--r--   0        0        0     4917 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_python/command.cpp
--rw-r--r--   0        0        0     1956 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_python/endstone_python.cpp
--rw-r--r--   0        0        0     2735 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_python/logger.cpp
--rw-r--r--   0        0        0     8639 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_python/permissions.cpp
--rw-r--r--   0        0        0    12925 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_python/plugin.cpp
--rw-r--r--   0        0        0     2198 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_python/server.cpp
--rw-r--r--   0        0        0     2182 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_python/util.cpp
--rw-r--r--   0        0        0     2401 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/bedrock/bedrock_log.cpp
--rw-r--r--   0        0        0      889 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/bedrock/command/command.cpp
--rw-r--r--   0        0        0     1542 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/bedrock/command/command_output.cpp
--rw-r--r--   0        0        0     6564 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/bedrock/command/command_registry.cpp
--rw-r--r--   0        0        0      830 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/bedrock/common.cpp
--rw-r--r--   0        0        0      997 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/bedrock/i18n.cpp
--rw-r--r--   0        0        0      949 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/bedrock/minecraft.cpp
--rw-r--r--   0        0        0     2480 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/bedrock/server/level/player.cpp
--rw-r--r--   0        0        0      862 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/bedrock/server/level/server_player.cpp
--rw-r--r--   0        0        0     2992 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/bedrock/server/server_instance.cpp
--rw-r--r--   0        0        0     5787 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/linux/hook.cpp
--rw-r--r--   0        0        0     2635 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/linux/os.cpp
--rw-r--r--   0        0        0     2491 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/main.cpp
--rw-r--r--   0        0        0     2088 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/plugin/python_plugin_loader.cpp
--rw-r--r--   0        0        0     6781 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/windows/hook.cpp
--rw-r--r--   0        0        0     2661 2022-11-09 12:37:21.000000 endstone-0.3.0/src/endstone_runtime/windows/os.cpp
--rw-r--r--   0        0        0      203 2022-11-09 12:37:21.000000 endstone-0.3.0/test_package/.gitignore
--rw-r--r--   0        0        0      308 2022-11-09 12:37:21.000000 endstone-0.3.0/test_package/CMakeLists.txt
--rw-r--r--   0        0        0     2235 2022-11-09 12:37:21.000000 endstone-0.3.0/test_package/conanfile.py
--rw-r--r--   0        0        0     1790 2022-11-09 12:37:21.000000 endstone-0.3.0/test_package/src/test_plugin.cpp
--rw-r--r--   0        0        0     4485 2022-11-09 12:37:21.000000 endstone-0.3.0/test_package/src/test_server.cpp
--rw-r--r--   0        0        0     4234 2022-11-09 12:37:21.000000 endstone-0.3.0/tests/test_command_lexer.cpp
--rw-r--r--   0        0        0     8575 2022-11-09 12:37:21.000000 endstone-0.3.0/tests/test_command_usage_parser.cpp
--rw-r--r--   0        0        0     1781 2022-11-09 12:37:21.000000 endstone-0.3.0/tests/test_logger.cpp
--rw-r--r--   0        0        0     1621 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/.gitignore
--rw-r--r--   0        0        0      358 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/funchook/conandata.yml
--rw-r--r--   0        0        0     3514 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/funchook/conanfile.py
--rw-r--r--   0        0        0     2134 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/funchook/patches/1.1.3-0001-cmake-use-cci-capstone.patch
--rw-r--r--   0        0        0     1506 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/funchook/test_package/CMakeLists.txt
--rw-r--r--   0        0        0      704 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/funchook/test_package/conanfile.py
--rw-r--r--   0        0        0      477 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/funchook/test_package/libfunchook_test.c
--rw-r--r--   0        0        0     2249 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/funchook/test_package/libfunchook_test_aarch64_gas.S
--rw-r--r--   0        0        0      267 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/funchook/test_package/libfunchook_test_noasm.c
--rw-r--r--   0        0        0     1060 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/funchook/test_package/libfunchook_test_x86_64_gas.S
--rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/funchook/test_package/libfunchook_test_x86_64_masm.asm
--rw-r--r--   0        0        0     2634 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/funchook/test_package/libfunchook_test_x86_gas.S
--rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/funchook/test_package/libfunchook_test_x86_masm.asm
--rw-r--r--   0        0        0     4092 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/funchook/test_package/suffix.list
--rw-r--r--   0        0        0    20695 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/funchook/test_package/test_main.c
--rw-r--r--   0        0        0    10659 2022-11-09 12:37:21.000000 endstone-0.3.0/third_party/funchook/test_package/x86_test.S
--rw-r--r--   0        0        0    22834 2022-11-09 12:37:21.000000 endstone-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 endstone-0.4.0/.clang-format
+-rw-r--r--   0        0        0     4248 2022-11-09 12:37:21.000000 endstone-0.4.0/.clang-tidy
+-rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 endstone-0.4.0/.dockerignore
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 endstone-0.4.0/.git_archival.txt
+-rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/conan_profiles/linux
+-rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/conan_profiles/windows
+-rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2251 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1628 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     1886 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/workflows/linux.yml
+-rw-r--r--   0        0        0     5258 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/workflows/wheel.yml
+-rw-r--r--   0        0        0     1167 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/workflows/windows.yml
+-rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 endstone-0.4.0/.gitignore
+-rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 endstone-0.4.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     4674 2022-11-09 12:37:21.000000 endstone-0.4.0/CMakeLists.txt
+-rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 endstone-0.4.0/Dockerfile
+-rw-r--r--   0        0        0    11356 2022-11-09 12:37:21.000000 endstone-0.4.0/LICENSE
+-rw-r--r--   0        0        0     8645 2022-11-09 12:37:21.000000 endstone-0.4.0/README.md
+-rw-r--r--   0        0        0       88 2022-11-09 12:37:21.000000 endstone-0.4.0/codecov.yml
+-rw-r--r--   0        0        0     6535 2022-11-09 12:37:21.000000 endstone-0.4.0/conanfile.py
+-rw-r--r--   0        0        0      315 2022-11-09 12:37:21.000000 endstone-0.4.0/docker-compose.yml
+-rw-r--r--   0        0        0      491 2022-11-09 12:37:21.000000 endstone-0.4.0/docs/index.md
+-rw-r--r--   0        0        0       16 2022-11-09 12:37:21.000000 endstone-0.4.0/docs/requirements.txt
+-rw-r--r--   0        0        0      943 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/automatic_id.h
+-rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/bedrock.h
+-rw-r--r--   0        0        0     1777 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/bedrock_log.h
+-rw-r--r--   0        0        0     1506 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command.h
+-rw-r--r--   0        0        0     1175 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_context.h
+-rw-r--r--   0        0        0     2106 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_flag.h
+-rw-r--r--   0        0        0     4945 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_origin.h
+-rw-r--r--   0        0        0     1996 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_output.h
+-rw-r--r--   0        0        0      806 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_permission_level.h
+-rw-r--r--   0        0        0    12075 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_registry.h
+-rw-r--r--   0        0        0      836 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_utils.h
+-rw-r--r--   0        0        0      715 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_version.h
+-rw-r--r--   0        0        0     1596 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/minecraft_commands.h
+-rw-r--r--   0        0        0      780 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/common.h
+-rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/core.h
+-rw-r--r--   0        0        0     1023 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/details.h
+-rw-r--r--   0        0        0     5062 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/forward.h
+-rw-r--r--   0        0        0      943 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/i18n.h
+-rw-r--r--   0        0        0      935 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/mce.h
+-rw-r--r--   0        0        0     1303 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/memory.h
+-rw-r--r--   0        0        0      814 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/minecraft.h
+-rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/network_identifier.h
+-rw-r--r--   0        0        0      684 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/protocol/certificate.h
+-rw-r--r--   0        0        0     2132 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/protocol/game/available_commands_packet.h
+-rw-r--r--   0        0        0     1495 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/protocol/game/text_packet.h
+-rw-r--r--   0        0        0      926 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/protocol/minecraft_packets.h
+-rw-r--r--   0        0        0     1001 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/protocol/packet.h
+-rw-r--r--   0        0        0      822 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/protocol/packet_sender.h
+-rw-r--r--   0        0        0      693 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/protocol/sub_client_id.h
+-rw-r--r--   0        0        0     1469 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/raknet/socket2.h
+-rw-r--r--   0        0        0     1126 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/raknet/types.h
+-rw-r--r--   0        0        0      987 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/server/level/server_level.h
+-rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/server/level/server_player.h
+-rw-r--r--   0        0        0     1086 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/server/network/server_network_handler.h
+-rw-r--r--   0        0        0      788 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/server/server_instance.h
+-rw-r--r--   0        0        0      998 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/threading.h
+-rw-r--r--   0        0        0      941 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/type_id.h
+-rw-r--r--   0        0        0    12542 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/actor.h
+-rw-r--r--   0        0        0      843 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/actor_initialization_method.h
+-rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/actor_runtime_id.h
+-rw-r--r--   0        0        0      740 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/actor_unique_id.h
+-rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/components/abilities_component.h
+-rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/components/actor_owner_component.h
+-rw-r--r--   0        0        0      759 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/components/actor_unique_id_component.h
+-rw-r--r--   0        0        0      756 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/components/runtime_id_component.h
+-rw-r--r--   0        0        0     1160 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/components/user_entity_identifier_component.h
+-rw-r--r--   0        0        0     3163 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/mob/mob.h
+-rw-r--r--   0        0        0      973 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/player/permissions_handler.h
+-rw-r--r--   0        0        0     5687 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/player/player.h
+-rw-r--r--   0        0        0      773 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/player/player_permission_level.h
+-rw-r--r--   0        0        0     2624 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/registry/entity_context.h
+-rw-r--r--   0        0        0     2127 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/registry/entity_registry.h
+-rw-r--r--   0        0        0     1801 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/dimension/dimension.h
+-rw-r--r--   0        0        0      780 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/dimension/dimension_height_range.h
+-rw-r--r--   0        0        0      921 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/dimension/dimension_interface.h
+-rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/dimension/vanilla_dimensions.h
+-rw-r--r--   0        0        0     3703 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/actor_event.h
+-rw-r--r--   0        0        0     2655 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/block_event.h
+-rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/coordinator_result.h
+-rw-r--r--   0        0        0     2726 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/event_coordinator.h
+-rw-r--r--   0        0        0      729 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/event_ref.h
+-rw-r--r--   0        0        0      726 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/event_result.h
+-rw-r--r--   0        0        0     1324 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/gameplay_handler.h
+-rw-r--r--   0        0        0     2621 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/item_event.h
+-rw-r--r--   0        0        0     2313 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/level_event.h
+-rw-r--r--   0        0        0     5082 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/player_event.h
+-rw-r--r--   0        0        0     1964 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/server_event.h
+-rw-r--r--   0        0        0      744 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/level.h
+-rw-r--r--   0        0        0    28182 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/level_interface.h
+-rw-r--r--   0        0        0      735 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/level_listener.h
+-rw-r--r--   0        0        0      905 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/storage/saved_data.h
+-rw-r--r--   0        0        0      725 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/math/vec3.h
+-rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/actor/actor.h
+-rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/actor/human.h
+-rw-r--r--   0        0        0     2863 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/color_format.h
+-rw-r--r--   0        0        0     7632 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/command/command.h
+-rw-r--r--   0        0        0     1419 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/command/command_executor.h
+-rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/command/command_map.h
+-rw-r--r--   0        0        0     2055 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/command/command_sender.h
+-rw-r--r--   0        0        0     2767 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/command/plugin_command.h
+-rw-r--r--   0        0        0     2238 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/actor/actor.h
+-rw-r--r--   0        0        0     2160 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/actor/human.h
+-rw-r--r--   0        0        0     2431 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/cast.h
+-rw-r--r--   0        0        0     1014 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/bedrock_command.h
+-rw-r--r--   0        0        0     1652 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/command_adapter.h
+-rw-r--r--   0        0        0     2923 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/command_lexer.h
+-rw-r--r--   0        0        0     1514 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/command_map.h
+-rw-r--r--   0        0        0     1751 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/command_sender.h
+-rw-r--r--   0        0        0     1494 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/command_usage_parser.h
+-rw-r--r--   0        0        0      951 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/defaults/debug_command.h
+-rw-r--r--   0        0        0     1018 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/defaults/plugins_command.h
+-rw-r--r--   0        0        0     1162 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/defaults/version_command.h
+-rw-r--r--   0        0        0      842 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/endstone_command.h
+-rw-r--r--   0        0        0     1094 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/server_command_sender.h
+-rw-r--r--   0        0        0     5808 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/hook.h
+-rw-r--r--   0        0        0     1557 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/level.h
+-rw-r--r--   0        0        0      863 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/logger_factory.h
+-rw-r--r--   0        0        0      903 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/os.h
+-rw-r--r--   0        0        0     1502 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/permissions/default_permissions.h
+-rw-r--r--   0        0        0     2513 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/permissions/permissible_base.h
+-rw-r--r--   0        0        0     2417 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/player.h
+-rw-r--r--   0        0        0     1226 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/plugin/cpp_plugin_loader.h
+-rw-r--r--   0        0        0     5357 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/plugin/plugin_description_builder.h
+-rw-r--r--   0        0        0     3882 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/plugin/plugin_manager.h
+-rw-r--r--   0        0        0     1255 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/plugin/python_plugin_loader.h
+-rw-r--r--   0        0        0     3035 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/pybind_type_caster.h
+-rw-r--r--   0        0        0     2766 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/server.h
+-rw-r--r--   0        0        0      758 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/signal_handler.h
+-rw-r--r--   0        0        0     1055 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/spdlog/level_formatter.h
+-rw-r--r--   0        0        0     3184 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/spdlog/log_sink.h
+-rw-r--r--   0        0        0     1193 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/spdlog/spdlog_adapter.h
+-rw-r--r--   0        0        0     3206 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/spdlog/text_formatter.h
+-rw-r--r--   0        0        0     2947 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/virtual_table.h
+-rw-r--r--   0        0        0      785 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/dimension.h
+-rw-r--r--   0        0        0     1437 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/endstone.h
+-rw-r--r--   0        0        0     1195 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/actor/actor_event.h
+-rw-r--r--   0        0        0     1429 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/actor/actor_remove_event.h
+-rw-r--r--   0        0        0     1329 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/actor/actor_spawn_event.h
+-rw-r--r--   0        0        0     3097 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/event.h
+-rw-r--r--   0        0        0     2041 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/event_handler.h
+-rw-r--r--   0        0        0     1716 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/event_priority.h
+-rw-r--r--   0        0        0     3747 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/handler_list.h
+-rw-r--r--   0        0        0     1768 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/player/player_chat_event.h
+-rw-r--r--   0        0        0     1157 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/player/player_event.h
+-rw-r--r--   0        0        0     1220 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/player/player_join_event.h
+-rw-r--r--   0        0        0     1221 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/player/player_quit_event.h
+-rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/server/plugin_disable_event.h
+-rw-r--r--   0        0        0     1409 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/server/plugin_enable_event.h
+-rw-r--r--   0        0        0     2246 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/server/server_command_event.h
+-rw-r--r--   0        0        0     5526 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/server/server_list_ping_event.h
+-rw-r--r--   0        0        0     1352 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/server/server_load_event.h
+-rw-r--r--   0        0        0     1527 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/weather/thunder_change_event.h
+-rw-r--r--   0        0        0     1531 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/weather/weather_change_event.h
+-rw-r--r--   0        0        0     1152 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/weather/weather_event.h
+-rw-r--r--   0        0        0     1363 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/game_mode.h
+-rw-r--r--   0        0        0     1543 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/level.h
+-rw-r--r--   0        0        0     3495 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/logger.h
+-rw-r--r--   0        0        0     4267 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/permissions/permissible.h
+-rw-r--r--   0        0        0     5770 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/permissions/permission.h
+-rw-r--r--   0        0        0     4597 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/permissions/permission_attachment.h
+-rw-r--r--   0        0        0     2204 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/permissions/permission_attachment_info.h
+-rw-r--r--   0        0        0      796 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/permissions/permission_default.h
+-rw-r--r--   0        0        0     1707 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/player.h
+-rw-r--r--   0        0        0     7348 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/plugin/plugin.h
+-rw-r--r--   0        0        0     7486 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/plugin/plugin_description.h
+-rw-r--r--   0        0        0     1042 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/plugin/plugin_load_order.h
+-rw-r--r--   0        0        0     3062 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/plugin/plugin_loader.h
+-rw-r--r--   0        0        0     8500 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/plugin/plugin_manager.h
+-rw-r--r--   0        0        0     3596 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/server.h
+-rw-r--r--   0        0        0     4223 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/util/uuid.h
+-rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 endstone-0.4.0/mkdocs.yml
+-rw-r--r--   0        0        0     1964 2022-11-09 12:37:21.000000 endstone-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 endstone-0.4.0/python/.gitignore
+-rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/__init__.py
+-rw-r--r--   0        0        0     3110 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/bootstrap/__init__.py
+-rw-r--r--   0        0        0    10393 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/bootstrap/base.py
+-rw-r--r--   0        0        0     2178 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/bootstrap/linux.py
+-rw-r--r--   0        0        0     7266 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/bootstrap/windows.py
+-rw-r--r--   0        0        0    37546 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/endstone_python.pyi
+-rw-r--r--   0        0        0     4090 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/plugin_loader.py
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/version.py
+-rw-r--r--   0        0        0      100 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/actor.py
+-rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/command.py
+-rw-r--r--   0        0        0     1084 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/event.py
+-rw-r--r--   0        0        0      277 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/permissions.py
+-rw-r--r--   0        0        0     5200 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/plugin.py
+-rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/util.py
+-rw-r--r--   0        0        0     1630 2022-11-09 12:37:21.000000 endstone-0.4.0/python/tests/test_color_format.py
+-rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 endstone-0.4.0/python/tests/test_imports.py
+-rw-r--r--   0        0        0     2315 2022-11-09 12:37:21.000000 endstone-0.4.0/python/tests/test_plugin_description.py
+-rw-r--r--   0        0        0     2562 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/actor/actor.cpp
+-rw-r--r--   0        0        0     2687 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/actor/human.cpp
+-rw-r--r--   0        0        0     1004 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/bedrock_command.cpp
+-rw-r--r--   0        0        0     5046 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/command_adapter.cpp
+-rw-r--r--   0        0        0     3153 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/command_lexer.cpp
+-rw-r--r--   0        0        0     9109 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/command_map.cpp
+-rw-r--r--   0        0        0     2179 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/command_sender.cpp
+-rw-r--r--   0        0        0     4793 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/command_usage_parser.cpp
+-rw-r--r--   0        0        0     1845 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/defaults/debug_command.cpp
+-rw-r--r--   0        0        0     1934 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/defaults/plugins_command.cpp
+-rw-r--r--   0        0        0     3846 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/defaults/version_command.cpp
+-rw-r--r--   0        0        0     1325 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/server_command_sender.cpp
+-rw-r--r--   0        0        0     2155 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/event/server/server_list_ping_event.cpp
+-rw-r--r--   0        0        0     2086 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/level.cpp
+-rw-r--r--   0        0        0     1514 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/logger_factory.cpp
+-rw-r--r--   0        0        0     2750 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/permissions/default_permissions.cpp
+-rw-r--r--   0        0        0     6405 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/permissions/permissible_base.cpp
+-rw-r--r--   0        0        0     4513 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/player.cpp
+-rw-r--r--   0        0        0     4796 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/plugin/cpp_plugin_loader.cpp
+-rw-r--r--   0        0        0    11062 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/plugin/plugin_manager.cpp
+-rw-r--r--   0        0        0     5425 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/server.cpp
+-rw-r--r--   0        0        0     1553 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/spdlog/level_formatter.cpp
+-rw-r--r--   0        0        0     3601 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/spdlog/log_sink.cpp
+-rw-r--r--   0        0        0     1415 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/spdlog/spdlog_adapter.cpp
+-rw-r--r--   0        0        0     2244 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/spdlog/text_formatter.cpp
+-rw-r--r--   0        0        0      977 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_python/actor.cpp
+-rw-r--r--   0        0        0     4917 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_python/command.cpp
+-rw-r--r--   0        0        0    11142 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_python/endstone_python.cpp
+-rw-r--r--   0        0        0     8623 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_python/event.cpp
+-rw-r--r--   0        0        0     8641 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_python/permissions.cpp
+-rw-r--r--   0        0        0    16268 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_python/plugin.cpp
+-rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_python/util.cpp
+-rw-r--r--   0        0        0     2402 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/bedrock_log.cpp
+-rw-r--r--   0        0        0      889 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/command/command.cpp
+-rw-r--r--   0        0        0     1542 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/command/command_output.cpp
+-rw-r--r--   0        0        0     4960 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/command/command_registry.cpp
+-rw-r--r--   0        0        0      914 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/command/command_utils.cpp
+-rw-r--r--   0        0        0     1878 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/command/minecraft_commands.cpp
+-rw-r--r--   0        0        0      830 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/common.cpp
+-rw-r--r--   0        0        0      997 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/i18n.cpp
+-rw-r--r--   0        0        0      876 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/minecraft.cpp
+-rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/network/protocol/minecraft_packets.cpp
+-rw-r--r--   0        0        0     3401 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/network/raknet/socket2.cpp
+-rw-r--r--   0        0        0     1086 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/network/raknet/types.cpp
+-rw-r--r--   0        0        0     1377 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/server/level/server_level.cpp
+-rw-r--r--   0        0        0     1462 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/server/level/server_player.cpp
+-rw-r--r--   0        0        0     1804 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/server/network/server_network_handler.cpp
+-rw-r--r--   0        0        0      879 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/server/server_instance.cpp
+-rw-r--r--   0        0        0      879 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/threading.cpp
+-rw-r--r--   0        0        0     2907 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/world/actor/actor.cpp
+-rw-r--r--   0        0        0     2074 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/world/actor/player/player.cpp
+-rw-r--r--   0        0        0      760 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/world/level/dimension/dimension.cpp
+-rw-r--r--   0        0        0      977 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/world/level/dimension/vanilla_dimensions.cpp
+-rw-r--r--   0        0        0     7382 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/world/level/event/event_coordinator.cpp
+-rw-r--r--   0        0        0     3196 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/world/level/event/gameplay_handler.cpp
+-rw-r--r--   0        0        0     4489 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/hook.cpp
+-rw-r--r--   0        0        0     4343 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/linux/hook.cpp
+-rw-r--r--   0        0        0     2660 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/linux/os.cpp
+-rw-r--r--   0        0        0     1734 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/linux/signal_handler.cpp
+-rw-r--r--   0        0        0     3759 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/magic.cpp
+-rw-r--r--   0        0        0     2491 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/main.cpp
+-rw-r--r--   0        0        0     2088 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/plugin/python_plugin_loader.cpp
+-rw-r--r--   0        0        0     4776 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/windows/hook.cpp
+-rw-r--r--   0        0        0     2661 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/windows/os.cpp
+-rw-r--r--   0        0        0     1696 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/windows/signal_handler.cpp
+-rw-r--r--   0        0        0     4234 2022-11-09 12:37:21.000000 endstone-0.4.0/tests/command/test_command_lexer.cpp
+-rw-r--r--   0        0        0     8575 2022-11-09 12:37:21.000000 endstone-0.4.0/tests/command/test_command_usage_parser.cpp
+-rw-r--r--   0        0        0     3696 2022-11-09 12:37:21.000000 endstone-0.4.0/tests/plugin/test_cpp_plugin_loader.cpp
+-rw-r--r--   0        0        0     1750 2022-11-09 12:37:21.000000 endstone-0.4.0/tests/plugin/test_plugin.cpp
+-rw-r--r--   0        0        0     1781 2022-11-09 12:37:21.000000 endstone-0.4.0/tests/test_logger_factory.cpp
+-rw-r--r--   0        0        0     1621 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/.gitignore
+-rw-r--r--   0        0        0      358 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/conandata.yml
+-rw-r--r--   0        0        0     3514 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/conanfile.py
+-rw-r--r--   0        0        0     2134 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/patches/1.1.3-0001-cmake-use-cci-capstone.patch
+-rw-r--r--   0        0        0     1506 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/CMakeLists.txt
+-rw-r--r--   0        0        0      704 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/conanfile.py
+-rw-r--r--   0        0        0      477 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/libfunchook_test.c
+-rw-r--r--   0        0        0     2249 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_aarch64_gas.S
+-rw-r--r--   0        0        0      267 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_noasm.c
+-rw-r--r--   0        0        0     1060 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_x86_64_gas.S
+-rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_x86_64_masm.asm
+-rw-r--r--   0        0        0     2634 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_x86_gas.S
+-rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_x86_masm.asm
+-rw-r--r--   0        0        0     4092 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/suffix.list
+-rw-r--r--   0        0        0    20695 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/test_main.c
+-rw-r--r--   0        0        0    10659 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/x86_test.S
+-rw-r--r--   0        0        0    22834 2022-11-09 12:37:21.000000 endstone-0.4.0/PKG-INFO
```

### Comparing `endstone-0.3.0/.clang-format` & `endstone-0.4.0/.clang-format`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/.clang-tidy` & `endstone-0.4.0/.clang-tidy`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,17 @@
   modernize-*,
   performance-*,
   portability-*,
   readability-*,
   -bugprone-easily-swappable-parameters,
   -bugprone-exception-escape,
   -bugprone-implicit-widening-of-multiplication-result,
-  -misc-non-private-member-variables-in-classes,
   -misc-const-correctness,
+  -misc-non-private-member-variables-in-classes,
+  -misc-include-cleaner,
   -modernize-use-trailing-return-type,
   -modernize-avoid-c-arrays,
   -performance-enum-size,
   -readability-identifier-length,
   -readability-function-cognitive-complexity,
   -readability-magic-numbers,
   -readability-named-parameter
@@ -26,26 +27,26 @@
 
 CheckOptions:
   misc-unused-parameters.IgnoreVirtual: true
   readability-implicit-bool-conversion.AllowPointerConditions: true
   readability-implicit-bool-conversion.AllowIntegerConditions: true
   readability-identifier-naming.AbstractClassCase: CamelCase
   readability-identifier-naming.ClassCase: CamelCase
-  readability-identifier-naming.ClassConstantCase: UPPER_CASE
+  readability-identifier-naming.ClassConstantCase: CamelCase
   readability-identifier-naming.ClassMemberCase: CamelCase
   readability-identifier-naming.ClassMemberPrefix: 'm'
   readability-identifier-naming.ClassMethodCase: camelBack
   readability-identifier-naming.ConstantCase: lower_case
   readability-identifier-naming.ConstantMemberCase: lower_case
   readability-identifier-naming.ConstantMemberSuffix: ''
   readability-identifier-naming.ConstantParameterCase: lower_case
   readability-identifier-naming.ConstantPointerParameterCase: lower_case
   readability-identifier-naming.ConstexprFunctionCase: camelBack
   readability-identifier-naming.ConstexprMethodCase: camelBack
-  readability-identifier-naming.ConstexprVariableCase: CamelCase
+  readability-identifier-naming.ConstexprVariableCase: lower_case
   readability-identifier-naming.EnumCase: CamelCase
   readability-identifier-naming.EnumConstantCase: CamelCase
   readability-identifier-naming.FunctionCase: aNy_CasE
   readability-identifier-naming.GlobalConstantCase: UPPER_CASE
   readability-identifier-naming.GlobalConstantPointerCase: CamelCase
   readability-identifier-naming.GlobalVariableCase: CamelCase
   readability-identifier-naming.GlobalVariablePrefix: 'g'
@@ -77,10 +78,10 @@
   readability-identifier-naming.StructCase: CamelCase
   readability-identifier-naming.TemplateParameterCase: CamelCase
   readability-identifier-naming.TemplateTemplateParameterCase: CamelCase
   readability-identifier-naming.TypeAliasCase: CamelCase
   readability-identifier-naming.TypedefCase: CamelCase
   readability-identifier-naming.TypeTemplateParameterCase: CamelCase
   readability-identifier-naming.UnionCase: CamelCase
-  readability-identifier-naming.ValueTemplateParameterCase: lower_case
+  readability-identifier-naming.ValueTemplateParameterCase: CamelCase
   readability-identifier-naming.VariableCase: lower_case
   readability-identifier-naming.VirtualMethodCase: camelBack
```

### Comparing `endstone-0.3.0/.github/workflows/coverage.yml` & `endstone-0.4.0/.github/workflows/coverage.yml`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
           cache: 'pip'
 
       - name: Set up Clang 15
         env:
           LLVM_VERSION: 15
         run: |
           sudo apt-get update -y -q
-          sudo apt-get install -y -q lsb-release wget software-properties-common gnupg
+          sudo apt-get install -y -q build-essential lsb-release wget software-properties-common gnupg
           sudo wget https://apt.llvm.org/llvm.sh
           sudo chmod +x llvm.sh
           sudo ./llvm.sh ${LLVM_VERSION}
           sudo apt-get install -y -q libc++-${LLVM_VERSION}-dev libc++abi-${LLVM_VERSION}-dev
           sudo update-alternatives --install /usr/bin/clang clang /usr/bin/clang-${LLVM_VERSION} 100
           sudo update-alternatives --install /usr/bin/clang++ clang++ /usr/bin/clang++-${LLVM_VERSION} 100
           sudo update-alternatives --install /usr/bin/llvm-cov llvm-cov /usr/bin/llvm-cov-${LLVM_VERSION} 100
@@ -57,13 +57,13 @@
           cmake --preset conan-debug -DCMAKE_BUILD_TYPE=Debug -DCODE_COVERAGE=ON
           cmake --build build/Debug
 
       - name: Run Tests and Generate Coverage Data
         run: |
           pip install gcovr
           ctest --test-dir build/Debug
-          gcovr -r . --filter src/ --gcov-executable "llvm-cov gcov" --xml coverage.xml build/Debug
+          gcovr -r . --filter src/endstone_core/ --gcov-executable "llvm-cov gcov" --xml coverage.xml build/Debug
 
       - name: Upload Coverage Reports to Codecov
         uses: codecov/codecov-action@v4
         env:
           CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `endstone-0.3.0/.github/workflows/docker.yml` & `endstone-0.4.0/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/.github/workflows/linux.yml` & `endstone-0.4.0/.github/workflows/linux.yml`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 jobs:
   build:
     strategy:
       fail-fast: false
       matrix:
         os: [ ubuntu-20.04, ubuntu-22.04 ]
-        build_type: [ Debug, Release ]
+        build_type: [ Debug, Release, RelWithDebInfo ]
 
     name: Build on ${{ matrix.os }} (${{ matrix.build_type }})
     runs-on: ${{ matrix.os }}
 
     steps:
       - name: Checkout Code
         uses: actions/checkout@v4
@@ -33,15 +33,15 @@
           cache: 'pip'
 
       - name: Set up Clang 15
         env:
           LLVM_VERSION: 15
         run: |
           sudo apt-get update -y -q
-          sudo apt-get install -y -q lsb-release wget software-properties-common gnupg
+          sudo apt-get install -y -q build-essential lsb-release wget software-properties-common gnupg
           sudo wget https://apt.llvm.org/llvm.sh
           sudo chmod +x llvm.sh
           sudo ./llvm.sh ${LLVM_VERSION}
           sudo apt-get install -y -q libc++-${LLVM_VERSION}-dev libc++abi-${LLVM_VERSION}-dev
           sudo update-alternatives --install /usr/bin/clang clang /usr/bin/clang-${LLVM_VERSION} 100
           sudo update-alternatives --install /usr/bin/clang++ clang++ /usr/bin/clang++-${LLVM_VERSION} 100
           sudo update-alternatives --install /usr/bin/llvm-cov llvm-cov /usr/bin/llvm-cov-${LLVM_VERSION} 100
```

### Comparing `endstone-0.3.0/.github/workflows/wheel.yml` & `endstone-0.4.0/.github/workflows/wheel.yml`

 * *Files 4% similar despite different names*

```diff
@@ -42,35 +42,35 @@
         uses: lukka/get-cmake@latest
 
       - name: Set up Conan
         run: |
           python -m pip install -U conan
           conan profile detect --force
           conan export third_party/funchook --version 1.1.3
-          conan install . --build=missing -pr:a .github/conan_profiles/windows
+          conan install . --build=missing -s build_type=RelWithDebInfo -pr:a .github/conan_profiles/windows
 
       - name: Build Wheels
         run: |
           python -m pip install -U pip
           pip install wheel
           python -m pip wheel . --no-deps --wheel-dir=wheelhouse --verbose
 
       - name: Test Wheels
         run: |
           pip install pytest
-          Get-ChildItem ./wheelhouse/ -Filter *.whl | ForEach-Object {
+          Get-ChildItem ./wheelhouse/ -Filter *-win_amd64.whl | ForEach-Object {
               pip install $_.FullName
           }
           pytest python/tests
 
       - name: Upload Artifacts
         uses: actions/upload-artifact@v4
         with:
           name: endstone-wheels-windows-python${{ matrix.python }}
-          path: ./wheelhouse/*.whl
+          path: ./wheelhouse/*-win_amd64.whl
 
   build_wheels_linux:
     name: Build Wheels for Python ${{ matrix.python }} on Ubuntu
 
     strategy:
       fail-fast: false
       matrix:
@@ -90,15 +90,15 @@
           cache: 'pip'
 
       - name: Set up Clang 15
         env:
           LLVM_VERSION: 15
         run: |
           sudo apt-get update -y -q
-          sudo apt-get install -y -q lsb-release wget software-properties-common gnupg
+          sudo apt-get install -y -q build-essential lsb-release wget software-properties-common gnupg
           sudo wget https://apt.llvm.org/llvm.sh
           sudo chmod +x llvm.sh
           sudo ./llvm.sh ${LLVM_VERSION}
           sudo apt-get install -y -q libc++-${LLVM_VERSION}-dev libc++abi-${LLVM_VERSION}-dev
           sudo update-alternatives --install /usr/bin/clang clang /usr/bin/clang-${LLVM_VERSION} 100
           sudo update-alternatives --install /usr/bin/clang++ clang++ /usr/bin/clang++-${LLVM_VERSION} 100
           sudo update-alternatives --install /usr/bin/llvm-cov llvm-cov /usr/bin/llvm-cov-${LLVM_VERSION} 100
@@ -109,15 +109,15 @@
 
       - name: Set up Conan
         run: |
           python -m pip install -U pip
           pip install conan
           conan profile detect --force
           conan export third_party/funchook --version 1.1.3
-          conan install . --build=missing -pr:a .github/conan_profiles/linux
+          conan install . --build=missing -s build_type=RelWithDebInfo -pr:a .github/conan_profiles/linux
 
       - name: Build Wheels
         run: |
           python -m pip install -U pip
           pip install wheel
           python -m pip wheel . --no-deps --wheel-dir=wheelhouse --verbose
 
@@ -125,22 +125,22 @@
         run: |
           pip install auditwheel setuptools "patchelf>=0.14"
           python -m auditwheel --verbose repair --plat manylinux_2_31_x86_64 -w wheelhouse wheelhouse/*.whl
 
       - name: Test Wheels
         run: |
           pip install pytest
-          pip install wheelhouse/*.whl
+          pip install wheelhouse/*-manylinux_2_31_x86_64.whl
           pytest python/tests
 
       - name: Upload Artifacts
         uses: actions/upload-artifact@v4
         with:
           name: endstone-wheels-linux-python${{ matrix.python }}
-          path: ./wheelhouse/*.whl
+          path: ./wheelhouse/*-manylinux_2_31_x86_64.whl
 
   build_sdist:
     name: Build Source Distribution
     runs-on: ubuntu-latest
     steps:
       - name: Checkout Code
         uses: actions/checkout@v4
@@ -171,13 +171,13 @@
         uses: actions/download-artifact@v4
         with:
           pattern: endstone-*
           path: dist
           merge-multiple: true
 
       - name: Create a Release
-        uses: softprops/action-gh-release@v1
+        uses: softprops/action-gh-release@v2
         with:
           files: dist/*
 
       - name: Publish to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `endstone-0.3.0/.github/workflows/windows.yml` & `endstone-0.4.0/.github/workflows/windows.yml`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 jobs:
   build:
     strategy:
       fail-fast: false
       matrix:
         os: [ windows-2019, windows-2022 ]
-        build_type: [ Debug, Release ]
+        build_type: [ Debug, Release, RelWithDebInfo ]
 
     name: Build on ${{ matrix.os }} (${{ matrix.build_type }})
     runs-on: ${{ matrix.os }}
 
     steps:
       - name: Checkout Code
         uses: actions/checkout@v4
```

### Comparing `endstone-0.3.0/CMakeLists.txt` & `endstone-0.4.0/CMakeLists.txt`

 * *Files 17% similar despite different names*

```diff
@@ -10,39 +10,42 @@
         set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -g --coverage")
         set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -g --coverage")
     endif ()
 endif ()
 
 
 add_compile_definitions(PYBIND11_DETAILED_ERROR_MESSAGES)
-
+add_compile_definitions(ENTT_SPARSE_PAGE=2048)
+add_compile_definitions(ENTT_PACKED_PAGE=128)
 
 # ========
 # packages
 # ========
 find_package(fmt CONFIG REQUIRED)
 find_package(Python COMPONENTS Interpreter Development REQUIRED)
 find_package(pybind11 CONFIG REQUIRED)
 find_package(spdlog CONFIG REQUIRED)
 find_package(funchook CONFIG REQUIRED)
 find_package(magic_enum CONFIG REQUIRED)
+find_package(EnTT CONFIG REQUIRED)
+find_package(cpptrace CONFIG REQUIRED)
 if (UNIX)
-    find_package(LIEF CONFIG REQUIRED)
+    find_package(libelf CONFIG REQUIRED)
 endif ()
 
 find_package(GTest CONFIG REQUIRED)
 
 
 # =================
 # endstone::headers
 # =================
 add_library(endstone_headers INTERFACE)
 add_library(endstone::headers ALIAS endstone_headers)
 target_include_directories(endstone_headers INTERFACE include)
-target_link_libraries(endstone_headers INTERFACE fmt::fmt)
+target_link_libraries(endstone_headers INTERFACE fmt::fmt EnTT::EnTT)
 
 include(GNUInstallDirs)
 install(DIRECTORY include/ DESTINATION ${CMAKE_INSTALL_INCLUDEDIR})
 
 
 # ================
 # endstone::python
@@ -58,15 +61,15 @@
 
 # ==============
 # endstone::core
 # ==============
 file(GLOB_RECURSE ENDSTONE_CORE_SOURCE_FILES CONFIGURE_DEPENDS "src/endstone_core/*.cpp")
 add_library(endstone_core ${ENDSTONE_CORE_SOURCE_FILES})
 add_library(endstone::core ALIAS endstone_core)
-target_link_libraries(endstone_core PUBLIC endstone::headers spdlog::spdlog)
+target_link_libraries(endstone_core PUBLIC endstone::headers spdlog::spdlog magic_enum::magic_enum)
 if (UNIX)
     target_link_libraries(endstone_core PUBLIC ${CMAKE_DL_LIBS})
 endif ()
 target_compile_definitions(endstone_core PUBLIC ENDSTONE_VERSION="${ENDSTONE_VERSION}")
 
 include(GNUInstallDirs)
 install(TARGETS endstone_core
@@ -77,34 +80,46 @@
 
 # =================
 # endstone::runtime
 # =================
 file(GLOB_RECURSE ENDSTONE_RUNTIME_SOURCE_FILES CONFIGURE_DEPENDS "src/endstone_runtime/*.cpp")
 add_library(endstone_runtime SHARED ${ENDSTONE_RUNTIME_SOURCE_FILES})
 add_library(endstone::runtime ALIAS endstone_runtime)
-target_link_libraries(endstone_runtime PRIVATE endstone::core funchook::funchook magic_enum::magic_enum pybind11::embed)
+target_link_libraries(endstone_runtime PRIVATE endstone::core funchook::funchook pybind11::embed cpptrace::cpptrace)
 if (WIN32)
     target_link_libraries(endstone_runtime PRIVATE dbghelp.lib)
 elseif (UNIX)
-    target_link_libraries(endstone_runtime PRIVATE LIEF::LIEF)
+    target_link_libraries(endstone_runtime PRIVATE libelf::libelf)
     target_link_options(endstone_runtime PRIVATE "-Wl,--exclude-libs,ALL")
     target_compile_options(endstone_runtime PRIVATE "-fvisibility=hidden")
 endif ()
 
 include(GNUInstallDirs)
 install(TARGETS endstone_runtime
         ARCHIVE DESTINATION ${CMAKE_INSTALL_LIBDIR}
         LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
         RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR})
 install(TARGETS endstone_runtime DESTINATION "endstone/_internal/" COMPONENT endstone_wheel OPTIONAL)
-
+if (CMAKE_BUILD_TYPE STREQUAL "RelWithDebInfo")
+    if (MSVC)
+        install(FILES $<TARGET_PDB_FILE:endstone_runtime> DESTINATION "endstone/_internal/" COMPONENT endstone_wheel OPTIONAL)
+    elseif (UNIX)
+        add_custom_command(TARGET endstone_python POST_BUILD COMMAND ${CMAKE_STRIP} --strip-debug --strip-unneeded $<TARGET_FILE:endstone_python>)
+    endif ()
+endif ()
 
 # =====
 # tests
 # =====
 if (NOT BUILD_TESTING STREQUAL OFF)
-    file(GLOB ENDSTONE_TEST_FILES "tests/*.cpp")
+    add_library(test_plugin SHARED tests/plugin/test_plugin.cpp)
+    target_link_libraries(test_plugin PRIVATE endstone::headers)
+    set_target_properties(test_plugin PROPERTIES LIBRARY_OUTPUT_DIRECTORY "plugins")
+    set_target_properties(test_plugin PROPERTIES RUNTIME_OUTPUT_DIRECTORY "plugins")
+
+    file(GLOB_RECURSE ENDSTONE_TEST_FILES CONFIGURE_DEPENDS "tests/*.cpp")
     add_executable(endstone_test ${ENDSTONE_TEST_FILES})
-    target_link_libraries(endstone_test PRIVATE GTest::gtest_main endstone::core)
+    target_link_libraries(endstone_test PRIVATE endstone::core GTest::gtest_main GTest::gmock_main)
+
     include(GoogleTest)
     gtest_discover_tests(endstone_test)
 endif ()
```

### Comparing `endstone-0.3.0/Dockerfile` & `endstone-0.4.0/Dockerfile`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     PYTHONIOENCODING=UTF-8
 
 FROM base AS builder
 
 ARG LLVM_VERSION=15
 
 RUN apt-get update -y -q \
-    && apt-get install -y -q lsb-release wget software-properties-common gnupg \
+    && apt-get install -y -q build-essential lsb-release wget software-properties-common gnupg \
     && wget https://apt.llvm.org/llvm.sh \
     && chmod +x llvm.sh \
     && ./llvm.sh ${LLVM_VERSION} \
     && apt-get install -y -q libc++-${LLVM_VERSION}-dev libc++abi-${LLVM_VERSION}-dev \
     && update-alternatives --install /usr/bin/clang clang /usr/bin/clang-${LLVM_VERSION} 100 \
     && update-alternatives --install /usr/bin/clang++ clang++ /usr/bin/clang++-${LLVM_VERSION} 100 \
     && update-alternatives --install /usr/bin/llvm-cov llvm-cov /usr/bin/llvm-cov-${LLVM_VERSION} 100 \
@@ -37,21 +37,21 @@
 
 RUN git clone https://github.com/EndstoneMC/endstone.git .
 
 RUN python -m pip install --upgrade pip \
     && pip install conan \
     && conan profile detect --force \
     && conan export third_party/funchook --version 1.1.3 \
-    && conan install . --build=missing -pr:a .github/conan_profiles/linux
+    && conan install . --build=missing -s build_type=RelWithDebInfo -pr:a .github/conan_profiles/linux
 
 RUN python -m pip install --upgrade pip \
     && pip install wheel auditwheel setuptools "patchelf>=0.14" pytest \
     && python -m pip wheel . --no-deps --wheel-dir=wheelhouse --verbose \
     && python -m auditwheel --verbose repair --plat manylinux_2_31_x86_64 -w wheelhouse wheelhouse/*.whl \
-    && pip install wheelhouse/*.whl \
+    && pip install wheelhouse/*-manylinux_2_31_x86_64.whl \
     && pytest python/tests
 
 FROM base AS final
 
 RUN apt-get update -y -q \
     && apt-get install -y -q curl \
     && apt-get clean -y -q \
@@ -63,15 +63,15 @@
     && printf "endstone ALL= NOPASSWD: ALL\\n" >> /etc/sudoers
 
 WORKDIR /home/endstone
 
 COPY --from=builder /usr/src/endstone/wheelhouse .
 
 RUN python -m pip install --upgrade pip \
-    && pip install ./*.whl \
+    && pip install ./*-manylinux_2_31_x86_64.whl \
     && rm ./*.whl
 
 USER endstone
 
 EXPOSE 19132/udp 19133/udp
 
 CMD ["endstone"]
```

### Comparing `endstone-0.3.0/LICENSE` & `endstone-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/README.md` & `endstone-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 </p>
 
 [![Windows](https://github.com/EndstoneMC/endstone/actions/workflows/windows.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/windows.yml)
 [![Linux](https://github.com/EndstoneMC/endstone/actions/workflows/linux.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/linux.yml)
 [![Wheel](https://github.com/EndstoneMC/endstone/actions/workflows/wheel.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/wheel.yml)
 [![Docker](https://github.com/EndstoneMC/endstone/actions/workflows/docker.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/docker.yml)
 [![Documentation](https://img.shields.io/readthedocs/endstone)](https://endstone.readthedocs.io/)
-[![Minecraft - Version](https://img.shields.io/badge/minecraft-v1.20.72%20(Bedrock)-green)](https://feedback.minecraft.net/hc/en-us/sections/360001186971-Release-Changelogs)
+[![Minecraft - Version](https://img.shields.io/badge/minecraft-v1.20.73%20(Bedrock)-green)](https://feedback.minecraft.net/hc/en-us/sections/360001186971-Release-Changelogs)
 [![PyPI - Version](https://img.shields.io/pypi/v/endstone)](https://pypi.org/project/endstone)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/endstone)](https://pypi.org/project/endstone)
 [![Python](https://img.shields.io/badge/Python-3-blue?logo=python&logoColor=white)](https://www.python.org/)
 [![GitHub License](https://img.shields.io/github/license/endstonemc/endstone)](LICENSE)
 [![Codacy Badge](https://img.shields.io/codacy/grade/8877402fc70b40f5a8c4b325d890e3f7?logo=codacy)](https://app.codacy.com/gh/EndstoneMC/endstone/dashboard)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -150,15 +150,15 @@
 - [Python Example Plugin](https://github.com/EndstoneMC/python-plugin-template)
 
 | Milestone                                | Duration   | Core | C++ API | Python API | Since  |
 |------------------------------------------|------------|------|---------|------------|--------|
 | **🔌 Plugin Loader**                     | 1-2 months | ✅    | ✅       | ✅          | v0.1.0 |
 | **⌨️ Command System**                    | 2-3 months | ✅    | ✅       | ✅          | v0.2.0 |
 | **🔐 Permission System**                 | 2-3 months | ✅    | ✅       | ✅          | v0.3.0 |
-| **🎈 Event System**                      | 2-3 months | 🚧   | ⏳       | ⏳          |        |
+| **🎈 Event System**                      | 2-3 months | 🚧   | ✅       | ✅          |        |
 | **🛠 Minecraft Core Features**           | 4-5 months | ⏳    | ⏳       | ⏳          |        |
 | **🖼 GUI & Inventory System**            | 3-4 months | ⏳    | ⏳       | ⏳          |        |
 | **🌟 Advanced Features & Refinements**   | 4-6 months | ⏳    | ⏳       | ⏳          |        |
 | **🧪 Beta Testing & Community Feedback** | 3 months   | ⏳    | ⏳       | ⏳          |        |
 | **🚀 Official Release & Support**        | -          | ⏳    | ⏳       | ⏳          |        |
 
 Here's a legend to guide you:
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 actions/workflows/linux.yml/badge.svg)](https://github.com/EndstoneMC/endstone/
 actions/workflows/linux.yml) [![Wheel](https://github.com/EndstoneMC/endstone/
 actions/workflows/wheel.yml/badge.svg)](https://github.com/EndstoneMC/endstone/
 actions/workflows/wheel.yml) [![Docker](https://github.com/EndstoneMC/endstone/
     actions/workflows/docker.yml/badge.svg)](https://github.com/EndstoneMC/
        endstone/actions/workflows/docker.yml) [![Documentation](https://
   img.shields.io/readthedocs/endstone)](https://endstone.readthedocs.io/) [!
-   [Minecraft - Version](https://img.shields.io/badge/minecraft-v1.20.72%20
+   [Minecraft - Version](https://img.shields.io/badge/minecraft-v1.20.73%20
       (Bedrock)-green)](https://feedback.minecraft.net/hc/en-us/sections/
   360001186971-Release-Changelogs) [![PyPI - Version](https://img.shields.io/
    pypi/v/endstone)](https://pypi.org/project/endstone) [![PyPI - Downloads]
 (https://img.shields.io/pypi/dm/endstone)](https://pypi.org/project/endstone)
                [![Python](https://img.shields.io/badge/Python-3-
 blue?logo=python&logoColor=white)](https://www.python.org/) [![GitHub License]
 (https://img.shields.io/github/license/endstonemc/endstone)](LICENSE) [![Codacy
@@ -80,15 +80,15 @@
 Plugin](https://github.com/EndstoneMC/cpp-plugin-template) - [Python Example
 Plugin](https://github.com/EndstoneMC/python-plugin-template) | Milestone |
 Duration | Core | C++ API | Python API | Since | |-----------------------------
 -------------|------------|------|---------|------------|--------| | **ð
 Plugin Loader** | 1-2 months | â | â | â | v0.1.0 | | **â¨ï¸ Command
 System** | 2-3 months | â | â | â | v0.2.0 | | **ð Permission System**
 | 2-3 months | â | â | â | v0.3.0 | | **ð Event System** | 2-3 months
-| ð§ | â³ | â³ | | | **ð  Minecraft Core Features** | 4-5 months | â³ |
+| ð§ | â | â | | | **ð  Minecraft Core Features** | 4-5 months | â³ |
 â³ | â³ | | | **ð¼ GUI & Inventory System** | 3-4 months | â³ | â³ | â³
 | | | **ð Advanced Features & Refinements** | 4-6 months | â³ | â³ | â³ |
 | | **ð§ª Beta Testing & Community Feedback** | 3 months | â³ | â³ | â³ | |
 | **ð Official Release & Support** | - | â³ | â³ | â³ | | Here's a legend
 to guide you: - â: Task is completed. Woohoo! ð - ð§: Task is under way.
 We're on it! ðª - â³: Task is up next. Exciting things are coming! ð  ##
 ð Contributing [ð](#-table-of-contents) We warmly welcome contributions
```

### Comparing `endstone-0.3.0/conanfile.py` & `endstone-0.4.0/conanfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,20 +52,25 @@
 
         git = Git(self)
         tag = git.run("describe --tags --long")
 
         import re
 
         tag, num_commits, commit_hash = re.match(r"^v?(\S+)-(\d+)-g([a-f0-9]+)$", tag).groups()
+        num_commits = int(num_commits)
         version = Version(tag)
+
+        if num_commits > 0:
+            version = version.bump(len(version._items) - 1)
+
         value = ".".join(str(i) for i in version.main)
         if version.pre:
             value += f"-{version.pre}"
 
-        if (num_commits := int(num_commits)) > 0:
+        if num_commits > 0:
             value += f".dev{num_commits}"
 
         if version.build:
             value += f"+{version.build}"
 
         self.version = value
 
@@ -108,16 +113,18 @@
 
     def requirements(self):
         self.requires("spdlog/1.12.0")
         self.requires("fmt/[>=10.1.1]", transitive_headers=True, transitive_libs=True)
         self.requires("pybind11/2.11.1")
         self.requires("funchook/1.1.3")
         self.requires("magic_enum/0.9.5")
+        self.requires("entt/3.13.0")
+        self.requires("cpptrace/0.5.2")
         if self.settings.os == "Linux":
-            self.requires("lief/0.10.1")
+            self.requires("libelf/0.8.13")
 
         self.test_requires("gtest/1.14.0")
 
     def config_options(self):
         if self.settings.os == "Windows":
             self.options.rm_safe("fPIC")
 
@@ -145,15 +152,15 @@
         cmake = CMake(self)
         cmake.install()
 
     def package_info(self):
         self.cpp_info.components["headers"].libs = []
         self.cpp_info.components["headers"].libdirs = []
         self.cpp_info.components["headers"].set_property("cmake_target_name", "endstone::headers")
-        self.cpp_info.components["headers"].requires = ["fmt::fmt"]
+        self.cpp_info.components["headers"].requires = ["fmt::fmt", "entt::entt"]
 
         self.cpp_info.components["core"].libs = ["endstone_core"]
         self.cpp_info.components["core"].set_property("cmake_target_name", "endstone::core")
         self.cpp_info.components["core"].requires = ["spdlog::spdlog"]
         self.cpp_info.components["core"].defines = ["PYBIND11_USE_SMART_HOLDER_AS_DEFAULT"]
         if self.settings.os == "Linux":
             self.cpp_info.components["core"].system_libs.extend(["dl", "stdc++fs"])
@@ -161,12 +168,13 @@
         self.cpp_info.components["runtime"].libs = ["endstone_runtime"]
         self.cpp_info.components["runtime"].set_property("cmake_target_name", "endstone::runtime")
         self.cpp_info.components["runtime"].requires = [
             "core",
             "funchook::funchook",
             "magic_enum::magic_enum",
             "pybind11::pybind11",
+            "cpptrace::cpptrace",
         ]
         if self.settings.os == "Linux":
-            self.cpp_info.components["runtime"].requires.extend(["lief::lief"])
+            self.cpp_info.components["runtime"].requires.extend(["libelf::libelf"])
         if self.settings.os == "Windows":
             self.cpp_info.components["runtime"].system_libs.extend(["dbghelp"])
```

### Comparing `endstone-0.3.0/include/bedrock/bedrock.h` & `endstone-0.4.0/include/bedrock/bedrock.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/bedrock/bedrock_log.h` & `endstone-0.4.0/include/bedrock/bedrock_log.h`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 #include <bitset>
 #include <cstdarg>
 #include <cstdio>
 
 #include "bedrock/bedrock.h"
 
-using LogLevel = uint32_t;
+using LogLevel = std::uint32_t;
 
 enum class LogAreaID {
     All,
     Platform,
     Entity,
     Database,
     GUI,
```

### Comparing `endstone-0.3.0/include/bedrock/command/command.h` & `endstone-0.4.0/include/bedrock/command/command.h`

 * *Files 17% similar despite different names*

```diff
@@ -33,10 +33,10 @@
     virtual void execute(CommandOrigin const &, CommandOutput &) const = 0;
 
 private:
     int version_ = 0;
     CommandRegistry *registry_ = nullptr;                                         // +16
     CommandRegistry::Symbol symbol_;                                              // +24
     CommandPermissionLevel permission_level_ = CommandPermissionLevel::Internal;  // +28
-    CommandFlag flag_ = CommandFlag::NONE;                                        // +30
+    CommandFlag flag_ = CommandFlag::None;                                        // +30
 };
 static_assert(sizeof(Command) == 32);
```

### Comparing `endstone-0.3.0/include/bedrock/command/command_origin.h` & `endstone-0.4.0/include/bedrock/command/command_origin.h`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,26 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
+#include <optional>
+
 #include "bedrock/command/command_permission_level.h"
 #include "bedrock/forward.h"
-#include "bedrock/uuid.h"
+#include "bedrock/mce.h"
+#include "bedrock/network/network_identifier.h"
+#include "bedrock/network/protocol/sub_client_id.h"
+#include "bedrock/world/level/dimension/dimension.h"
+#include "bedrock/world/math/vec3.h"
+
+class Actor;
+class Level;
 
 enum class CommandOriginType : char {
     Player = 0,
     CommandBlock = 1,
     MinecartCommandBlock = 2,
     DevConsole = 3,
     Test = 4,
```

### Comparing `endstone-0.3.0/include/bedrock/command/command_output.h` & `endstone-0.4.0/include/bedrock/command/command_output.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/bedrock/command/command_permission_level.h` & `endstone-0.4.0/include/bedrock/command/command_permission_level.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/bedrock/command/command_registry.h` & `endstone-0.4.0/include/bedrock/command/command_registry.h`

 * *Files 6% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 #include <vector>
 
 #include "bedrock/bedrock.h"
 #include "bedrock/command/command_flag.h"
 #include "bedrock/command/command_origin.h"
 #include "bedrock/command/command_permission_level.h"
 #include "bedrock/command/command_version.h"
-#include "bedrock/network/game/available_commands_packet.h"
+#include "bedrock/network/protocol/game/available_commands_packet.h"
 #include "bedrock/type_id.h"
 
-enum SemanticConstraint : uint8_t;
+enum SemanticConstraint : std::uint8_t;
 
 class Command;
 class CommandParameterData;
 
 class CommandRegistry {
 public:
     struct Overload {
@@ -43,43 +43,43 @@
             : version(version), factory(factory)
         {
         }
 
         CommandVersion version;                    // +0
         std::unique_ptr<Command> (*factory)();     // +8
         std::vector<CommandParameterData> params;  // +16
-        int32_t unknown1{-1};                      // +40
-        int8_t unknown2{0};                        // +44
-        uint64_t unknown3{0};                      // +48
-        uint64_t unknown4{0};                      // +56
-        uint64_t unknown5{0};                      // +64
+        std::int32_t unknown1{-1};                 // +40
+        std::int8_t unknown2{0};                   // +44
+        std::uint64_t unknown3{0};                 // +48
+        std::uint64_t unknown4{0};                 // +56
+        std::uint64_t unknown5{0};                 // +64
     };
 
     class Symbol {
     public:
         int value = -1;
-        static const Symbol INT;
-        static const Symbol FLOAT;
-        static const Symbol RELATIVE_FLOAT;
-        static const Symbol WILDCARD_INT;
-        static const Symbol OPERATOR;
-        static const Symbol COMPARE_OPERATOR;
-        static const Symbol SELECTOR;
-        static const Symbol WILDCARD_ACTOR_SELECTOR;
-        static const Symbol FILE_PATH;
-        static const Symbol INTEGER_RANGE;
-        static const Symbol EQUIPMENT_SLOT;
-        static const Symbol STRING;
-        static const Symbol POSITION;
-        static const Symbol POSITION_FLOAT;
-        static const Symbol MESSAGE;
-        static const Symbol RAW_TEXT;
-        static const Symbol JSON;
-        static const Symbol BLOCK_STATE;
-        static const Symbol COMMAND;
+        static const Symbol Int;
+        static const Symbol Float;
+        static const Symbol RelativeFloat;
+        static const Symbol WildcardInt;
+        static const Symbol Operator;
+        static const Symbol CompareOperator;
+        static const Symbol Selector;
+        static const Symbol WildcardActorSelector;
+        static const Symbol FilePath;
+        static const Symbol IntegerRange;
+        static const Symbol EquipmentSlot;
+        static const Symbol String;
+        static const Symbol Position;
+        static const Symbol PositionFloat;
+        static const Symbol Message;
+        static const Symbol RawText;
+        static const Symbol Json;
+        static const Symbol BlockState;
+        static const Symbol Command;
     };
 
     struct Signature {
         std::string name;                                  // +0
         std::string description;                           // +32
         std::vector<CommandRegistry::Overload> overloads;  // +64
         std::vector<int> subcommand_values;                // +88
@@ -87,23 +87,23 @@
         CommandRegistry::Symbol symbol;                    // +116
         CommandRegistry::Symbol enum_symbol;               // +120
         CommandFlag command_flag;                          // +124
         int unknown3;                                      // +128
         int symbol_index;                                  // +132
         int optional_index;                                // +136
         char unknown6;                                     // +140
-        int64_t unknown7;                                  // +144
+        std::int64_t unknown7;                             // +144
     };
 
     struct ParseToken {
         std::unique_ptr<ParseToken> child;  // +0
         std::unique_ptr<ParseToken> next;   // +8
         ParseToken *parent;                 // +16
         char const *data;                   // +24
-        uint32_t size;                      // +32
+        std::uint32_t size;                 // +32
         Symbol symbol;                      // +36
 
         friend std::ostream &operator<<(std::ostream &os, const ParseToken &token);
     };
     static_assert(sizeof(CommandRegistry::ParseToken) == 40);
 
     using ParseRule = bool (CommandRegistry::*)(void *, const CommandRegistry::ParseToken &, const CommandOrigin &, int,
@@ -112,18 +112,18 @@
     template <typename T>
     bool parse(void *value, const CommandRegistry::ParseToken &parse_token, const CommandOrigin &, int, std::string &,
                std::vector<std::string> &) const;
 
     class ParseTable;
     class Enum {
     public:
-        std::string name;                                   // +0
-        Bedrock::typeid_t<CommandRegistry> type_id;         // +32
-        ParseRule parse_rule;                               // +40
-        std::vector<std::pair<uint64_t, uint64_t>> values;  // +48
+        std::string name;                                             // +0
+        Bedrock::typeid_t<CommandRegistry> type_id;                   // +32
+        ParseRule parse_rule;                                         // +40
+        std::vector<std::pair<std::uint64_t, std::uint64_t>> values;  // +48
     };
     class SoftEnum;
 
     BEDROCK_API void registerCommand(const std::string &name, char const *description, CommandPermissionLevel level,
                                      CommandFlag flag1, CommandFlag flag2);
     BEDROCK_API void registerAlias(std::string name, std::string alias);
     BEDROCK_API int addEnumValues(const std::string &name, const std::vector<std::string> &values);
@@ -156,15 +156,15 @@
     {
         return describe(signature, signature.name, overload, 0, nullptr, nullptr);
     }
 
     std::function<void(class Packet const &)> network_update_callback;                      // +0
     std::function<int(bool &, std::string const &, class Actor const &)> score_callback;    // +56
     std::vector<void *> unknown1;                                                           // +128
-    std::map<uint32_t, CommandRegistry::ParseTable> parse_tables;                           // +152
+    std::map<std::uint32_t, CommandRegistry::ParseTable> parse_tables;                      // +152
     std::vector<void *> optionals;                                                          // +168
     std::vector<std::string> literals;                                                      // +192
     std::vector<CommandRegistry::Enum> enums;                                               // +216
     std::vector<std::string> subcommands;                                                   // +240
     std::vector<CommandRegistry::Enum> chained_subcommands;                                 // +264
     std::vector<CommandRegistry::Symbol> symbols;                                           // +288
     std::vector<std::string> postfixes;                                                     // +312
@@ -175,15 +175,15 @@
     std::vector<CommandRegistry::Symbol> command_symbols;                                   // +400
     std::map<std::string, CommandRegistry::Signature> commands;                             // +424
     std::map<Bedrock::typeid_t<CommandRegistry>, int> type_ids;                             // +440
     std::map<std::string, std::string> aliases;                                             // +456
     std::vector<SemanticConstraint> semantic_constraints;                                   // +472
     std::map<SemanticConstraint, unsigned char> constrained_values;                         // +496
     std::vector<void *> constrained_value_data;                                             // +512
-    std::map<std::pair<uint64_t, uint32_t>, uint32_t> unknown8;                             // +536
+    std::map<std::pair<std::uint64_t, std::uint32_t>, std::uint32_t> unknown8;              // +536
     std::vector<CommandRegistry::SoftEnum> soft_enums;                                      // +552
     std::map<std::string, int> soft_enum_symbol_index;                                      // +576
     std::vector<void *> unknown10;                                                          // +592
     char param_symbols[96];                                                                 // +616
     std::unordered_map<unsigned char, unsigned char> unknown11;                             // +712
     std::unordered_map<unsigned char, unsigned char> unknown12;                             // +776
     std::function<void(CommandFlag &, std::string const &)> command_registration_override;  // +840
```

### Comparing `endstone-0.3.0/include/bedrock/command/command_version.h` & `endstone-0.4.0/include/bedrock/command/command_version.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/bedrock/command/minecraft_commands.h` & `endstone-0.4.0/include/bedrock/command/minecraft_commands.h`

 * *Files 18% similar despite different names*

```diff
@@ -10,29 +10,41 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
+#include "bedrock/command/command_context.h"
 #include "bedrock/command/command_output.h"
 #include "bedrock/command/command_registry.h"
 
+struct MCRESULT {
+    bool is_success;
+    std::uint8_t category;
+    std::uint16_t error_code;
+};
+inline MCRESULT const MCRESULT_Success{true};                  // NOLINT
+inline MCRESULT const MCRESULT_CommandsDisabled{false, 0, 7};  // NOLINT
+
 class MinecraftCommands {
 public:
     virtual ~MinecraftCommands() = default;
 
     [[nodiscard]] CommandOutputSender &getOutputSender() const
     {
         return *output_sender_;
     }
 
     [[nodiscard]] CommandRegistry &getRegistry() const
     {
         return *registry_;
     }
 
+    BEDROCK_API MCRESULT executeCommand(CommandContext &ctx, bool flag) const;
+
 private:
     std::unique_ptr<CommandOutputSender> output_sender_;  // +8
     std::unique_ptr<CommandRegistry> registry_;           // +16
 };
+
 static_assert(sizeof(MinecraftCommands) == 24);
```

### Comparing `endstone-0.3.0/include/bedrock/common.h` & `endstone-0.4.0/include/bedrock/common.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/bedrock/core.h` & `endstone-0.4.0/include/bedrock/core.h`

 * *Files 14% similar despite different names*

```diff
@@ -12,8 +12,11 @@
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
 namespace Core {
 class FilePathManager;
-}
+
+template <typename T>
+class PathBuffer;
+}  // namespace Core
```

### Comparing `endstone-0.3.0/include/bedrock/i18n.h` & `endstone-0.4.0/include/bedrock/i18n.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/bedrock/minecraft.h` & `endstone-0.4.0/include/bedrock/minecraft.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/bedrock/network/game/available_commands_packet.h` & `endstone-0.4.0/include/bedrock/network/protocol/game/available_commands_packet.h`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 #pragma once
 
 #include <string>
 #include <vector>
 
 #include "bedrock/command/command_flag.h"
-#include "bedrock/network/packet.h"
+#include "bedrock/network/protocol/packet.h"
 
 class AvailableCommandsPacket : public Packet {
 public:
     struct OverloadData;
     struct ChainedSubcommandData;
     struct EnumData;
     struct SoftEnumData;
@@ -36,20 +36,14 @@
         std::vector<int> subcommand_values;       // +96
         int enum_symbol_index = -1;               // +120
     };
     // static_assert(sizeof(CommandData) == 128);
 
     ~AvailableCommandsPacket() override = default;
 
-    int unknown1;                               // +8
-    int unknown2;                               // +12
-    int unknown3;                               // +16
-    int64_t unknown4;                           // +24
-    int64_t unknown5;                           // +32
-    int unknown6;                               // +40
     std::vector<std::string> enum_names;        // +48
     std::vector<std::string> subcommand_names;  // +72
     std::vector<void *> enums;                  // +96  std::vector<EnumData>
     std::vector<std::string> postfixes;         // +120
     std::vector<void *> chained_subcommands;    // +144 std::vector<ChainedSubcommandData>
     std::vector<CommandData> commands;          // +168 std::vector<CommandData>
     std::vector<void *> soft_enums;             // +192 std::vector<SoftEnumData>
```

### Comparing `endstone-0.3.0/include/bedrock/network/packet.h` & `endstone-0.4.0/include/bedrock/world/level/level_listener.h`

 * *Files 4% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
-class Packet {
+class LevelListener {
 public:
-    virtual ~Packet() = default;
+    virtual ~LevelListener() = default;
 };
```

### Comparing `endstone-0.3.0/include/bedrock/network/packet_sender.h` & `endstone-0.4.0/include/bedrock/network/protocol/packet_sender.h`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
-#include "bedrock/network/packet.h"
+#include "bedrock/network/protocol/packet.h"
 
 class PacketSender {
 public:
     virtual ~PacketSender() = default;
     virtual void send(Packet &packet) = 0;
 };
```

### Comparing `endstone-0.3.0/include/bedrock/server/level/player.h` & `endstone-0.4.0/include/bedrock/world/actor/player/player.h`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,19 @@
 #pragma once
 
 #include <cstddef>
 #include <memory>
 
 #include "bedrock/bedrock.h"
 #include "bedrock/command/command_permission_level.h"
-#include "bedrock/network/packet_sender.h"
-#include "bedrock/world/actor/mob.h"
+#include "bedrock/network/protocol/packet_sender.h"
+#include "bedrock/world/actor/mob/mob.h"
+#include "bedrock/world/level/event/event_coordinator.h"
+#include "endstone/detail/player.h"
+#include "endstone/player.h"
 
 class Player : public Mob {
 public:
     ~Player() override = 0;
 
     virtual void prepareRegion(ChunkSource &) = 0;
     virtual void destroyRegion() = 0;
@@ -91,15 +94,15 @@
     virtual void sendComplexInventoryTransaction(std::unique_ptr<ComplexInventoryTransaction>) const = 0;
     virtual void sendNetworkPacket(Packet &) const = 0;
     virtual PlayerEventCoordinator &getPlayerEventCoordinator() = 0;
     virtual bool isSimulated() = 0;
     [[nodiscard]] virtual std::string getXuid() const = 0;
     [[nodiscard]] virtual PlayerMovementSettings getMovementSettings() const = 0;
     virtual void requestMissingSubChunk(SubChunkPos const &) = 0;
-    [[nodiscard]] virtual uint8_t getMaxChunkBuildRadius() const = 0;
+    [[nodiscard]] virtual std::uint8_t getMaxChunkBuildRadius() const = 0;
     virtual void onMovePlayerPacketNormal(Vec3 const &, Vec2 const &, float) = 0;
 
 protected:
     virtual std::shared_ptr<ChunkViewSource> _createChunkSource(ChunkSource &) = 0;
 
 public:
     virtual void setAbilities(LayeredAbilities const &) = 0;
@@ -108,11 +111,16 @@
 
 protected:
     [[nodiscard]] virtual int _getSpawnChunkLimit() const = 0;
     virtual void updateChunkPublisherView(Vec3 const &, float) = 0;
 
 public:
     BEDROCK_API void setPermissions(CommandPermissionLevel level);
+    [[nodiscard]] BEDROCK_API const std::string &getName() const;
+
+private:
+public:
+    [[nodiscard]] endstone::detail::EndstonePlayer &getEndstonePlayer() const;  // Endstone
 
 protected:
-    void sendCommands();  // TODO: move to endstone::Player
+    void sendCommands() const;  // Endstone
 };
```

### Comparing `endstone-0.3.0/include/bedrock/server/level/server_player.h` & `endstone-0.4.0/include/bedrock/network/protocol/sub_client_id.h`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,8 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
-#include "bedrock/bedrock.h"
-#include "bedrock/server/level/player.h"
-
-class ServerPlayer : public Player {
-public:
-    ~ServerPlayer() override = 0;
-    BEDROCK_API void doInitialSpawn();
-};
+enum class SubClientId : char;
```

### Comparing `endstone-0.3.0/include/bedrock/server/server_instance.h` & `endstone-0.4.0/include/bedrock/threading.h`

 * *Files 23% similar despite different names*

```diff
@@ -10,21 +10,27 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
+#include <thread>
+
 #include "bedrock/bedrock.h"
-#include "bedrock/minecraft.h"
 
-class ServerInstance {
-public:
-    Minecraft &getMinecraft();
-};
+namespace Bedrock::Threading {
 
-class ServerInstanceEventCoordinator {
+class AssignedThread {
 public:
-    BEDROCK_API void sendServerInitializeStart(ServerInstance &instance);
-    BEDROCK_API void sendServerThreadStarted(ServerInstance &instance);
-    BEDROCK_API void sendServerThreadStopped(ServerInstance &instance);
+    bool isOnThread()
+    {
+        return std::this_thread::get_id() == assigned_id_;
+    }
+
+private:
+    std::thread::id assigned_id_;
 };
+
+BEDROCK_API AssignedThread &getServerThread();
+
+}  // namespace Bedrock::Threading
```

### Comparing `endstone-0.3.0/include/bedrock/type_id.h` & `endstone-0.4.0/include/bedrock/type_id.h`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 #include "bedrock/bedrock.h"
 
 namespace Bedrock {
 
 template <typename Context>
 class typeid_t {  // NOLINT(*-identifier-naming)
 public:
-    uint16_t id;
+    std::uint16_t id;
 };
 
 template <typename Context, typename Type>
 typeid_t<Context> type_id();
 
 }  // namespace Bedrock
```

### Comparing `endstone-0.3.0/include/bedrock/uuid.h` & `endstone-0.4.0/include/bedrock/world/actor/actor_unique_id.h`

 * *Files 18% similar despite different names*

```diff
@@ -10,16 +10,13 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
-#include <array>
 #include <cstdint>
 
-namespace mce {
-struct UUID {
-    uint64_t msb;  // most significant bits
-    uint64_t lsb;  // least significant bits
+class ActorUniqueID {
+public:
+    std::int64_t id{-1};
 };
-}  // namespace mce
```

### Comparing `endstone-0.3.0/include/bedrock/world/actor/actor.h` & `endstone-0.4.0/include/bedrock/world/actor/actor.h`

 * *Files 23% similar despite different names*

```diff
@@ -15,15 +15,31 @@
 #pragma once
 
 #include <cstdint>
 #include <optional>
 #include <string>
 #include <vector>
 
+#include "bedrock/automatic_id.h"
+#include "bedrock/bedrock.h"
+#include "bedrock/command/command_permission_level.h"
 #include "bedrock/forward.h"
+#include "bedrock/mce.h"
+#include "bedrock/memory.h"
+#include "bedrock/world/actor/actor_initialization_method.h"
+#include "bedrock/world/actor/actor_runtime_id.h"
+#include "bedrock/world/actor/actor_unique_id.h"
+#include "bedrock/world/actor/registry/entity_context.h"
+#include "bedrock/world/actor/registry/entity_registry.h"
+#include "bedrock/world/level/dimension/dimension.h"
+#include "bedrock/world/math/vec3.h"
+#include "endstone/detail/actor/actor.h"
+
+class Player;
+class Level;
 
 class Actor {
 public:
     virtual bool getStatusFlag(ActorFlags flags) = 0;
     virtual void setStatusFlag(ActorFlags flags, bool value) = 0;
 #ifdef _WIN32
     virtual bool hasComponent(HashedString const &) = 0;
@@ -41,15 +57,15 @@
 public:
 #ifdef __linux__
     virtual bool hasComponent(HashedString const &) = 0;
 #endif
     virtual ~Actor() = 0;
     virtual void resetUserPos(bool) = 0;
     virtual ActorType getOwnerEntityType() = 0;
-    virtual void remove() = 0;
+    BEDROCK_API virtual void remove();
     virtual bool isRuntimePredictedMovementEnabled() = 0;
     [[nodiscard]] virtual Vec3 getFiringPos() const = 0;
     [[nodiscard]] virtual float getInterpolatedBodyRot(float) const = 0;
     [[nodiscard]] virtual float getInterpolatedHeadRot(float) const = 0;
     [[nodiscard]] virtual float getInterpolatedBodyYaw(float) const = 0;
     [[nodiscard]] virtual float getYawSpeedInDegreesPerSecond() const = 0;
     [[nodiscard]] virtual Vec3 getInterpolatedRidingOffset(float, int) const = 0;
@@ -145,15 +161,15 @@
     virtual void sendMotionPacketIfNeeded(PlayerMovementSettings const &) = 0;
     [[nodiscard]] virtual bool canSynchronizeNewEntity() const = 0;
     virtual void startSwimming() = 0;
     virtual void stopSwimming() = 0;
     virtual void buildDebugInfo(std::string &) const = 0;
     [[nodiscard]] virtual CommandPermissionLevel getCommandPermissionLevel() const = 0;
     [[nodiscard]] virtual int getDeathTime() const = 0;
-    [[nodiscard]] virtual bool canBeAffected(uint32_t) const = 0;
+    [[nodiscard]] virtual bool canBeAffected(std::uint32_t) const = 0;
     [[nodiscard]] virtual bool canBeAffectedByArrow(MobEffectInstance const &) const = 0;
     virtual void onEffectRemoved(MobEffectInstance &) = 0;
     [[nodiscard]] virtual bool canObstructSpawningAndBlockPlacement() const = 0;
     virtual AnimationComponent &getAnimationComponent() = 0;
     virtual void openContainerComponent(Player &) = 0;
     virtual void swing() = 0;
     virtual void useItem(ItemStackBase &, ItemUseMethod, bool) = 0;
@@ -195,8 +211,47 @@
 public:
     virtual void readAdditionalSaveData(CompoundTag const &, DataLoadHelper &) = 0;
     virtual void addAdditionalSaveData(CompoundTag &) = 0;
 
 protected:
     virtual void _playStepSound(BlockPos const &, Block const &) = 0;
     virtual void _doAutoAttackOnTouch(Actor &) = 0;
+
+public:
+    template <typename Component>
+    Component *tryGetComponent()
+    {
+        return context_.tryGetComponent<Component>();
+    }
+
+    template <typename Component>
+    Component *tryGetComponent() const
+    {
+        return context_.tryGetComponent<Component>();
+    }
+
+    BEDROCK_API void setDimension(WeakRef<Dimension>);
+
+    [[nodiscard]] bool isRemoved() const;
+    [[nodiscard]] Dimension &getDimension() const;
+    [[nodiscard]] Level &getLevel() const;
+    [[nodiscard]] Vec3 const &getPosition() const;
+    [[nodiscard]] ActorRuntimeID getRuntimeID() const;
+
+    static Actor *tryGetFromEntity(EntityContext const &, bool include_removed);
+
+protected:
+    EntityContext context_;                            // +8
+    ActorInitializationMethod initialization_method_;  // +32
+    std::string unknown2_;                             // +40
+    std::array<char[16], 10> unknown3_;                // +72
+    std::int16_t unknown4_;                            // +232
+    ActorDefinitionGroup *actor_definitions_;          // +240
+    char pad_[336];                                    // +248 TODO: figure out the structure
+    WeakRef<Dimension> dimension_;                     // +584
+    Level *level_;                                     // +600
+    char pad2_[56];                                    // +608
+    Vec3 position_;                                    // +664
+
+public:
+    [[nodiscard]] endstone::detail::EndstoneActor &getEndstoneActor() const;
 };
```

### Comparing `endstone-0.3.0/include/bedrock/world/actor/mob.h` & `endstone-0.4.0/include/bedrock/world/actor/mob/mob.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/command/command.h` & `endstone-0.4.0/include/endstone/command/command.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/command/command_executor.h` & `endstone-0.4.0/include/endstone/command/command_executor.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/command/command_map.h` & `endstone-0.4.0/include/endstone/command/command_map.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/command/command_sender.h` & `endstone-0.4.0/include/endstone/command/command_sender.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/command/plugin_command.h` & `endstone-0.4.0/include/endstone/command/plugin_command.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/detail/command/bedrock_command.h` & `endstone-0.4.0/include/endstone/detail/command/bedrock_command.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/detail/command/command_adapter.h` & `endstone-0.4.0/include/endstone/detail/command/command_adapter.h`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 #pragma once
 
 #include "bedrock/command/command.h"
 #include "endstone/command/command_sender.h"
 #include "endstone/detail/permissions/permissible_base.h"
 #include "endstone/detail/server.h"
-#include "endstone/detail/singleton.h"
 
 namespace endstone::detail {
 
 class CommandSenderAdapter : public BaseCommandSender {
 public:
     CommandSenderAdapter(const CommandOrigin &origin, CommandOutput &output);
     void sendMessage(const std::string &message) const override;
@@ -42,11 +41,8 @@
 
 private:
     friend class EndstoneCommandMap;
     friend class ::CommandRegistry;
     std::vector<std::string> args_;
 };
 
-bool customParseRule(CommandRegistry *, void *, const CommandRegistry::ParseToken &, const CommandOrigin &, int,
-                     std::string &, std::vector<std::string> &);
-
 }  // namespace endstone::detail
```

### Comparing `endstone-0.3.0/include/endstone/detail/command/command_lexer.h` & `endstone-0.4.0/include/endstone/detail/command/command_lexer.h`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #include <string>
 #include <string_view>
 
 namespace endstone::detail {
 
 class CommandLexer {
 public:
-    enum class TokenType : uint8_t {
+    enum class TokenType : std::uint8_t {
         Number,
         Identifier,
         LeftParen,
         RightParen,
         LeftSquare,
         RightSquare,
         LeftCurly,
@@ -77,15 +77,15 @@
     Token peek();
 
     void reset()
     {
         position_ = 0;
     }
 
-    [[nodiscard]] size_t getPosition() const
+    [[nodiscard]] std::size_t getPosition() const
     {
         return position_;
     }
 
 private:
     [[nodiscard]] char peekChar() const
     {
@@ -119,10 +119,10 @@
 
     static bool isIdentifierCharacter(char c)
     {
         return (c >= 'a' && c <= 'z') || (c >= 'A' && c <= 'Z') || isDigit(c) || c == '_';
     }
 
     std::string_view value_;
-    size_t position_ = 0;
+    std::size_t position_ = 0;
 };
 }  // namespace endstone::detail
```

### Comparing `endstone-0.3.0/include/endstone/detail/command/command_map.h` & `endstone-0.4.0/include/endstone/detail/command/command_map.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/detail/command/command_sender.h` & `endstone-0.4.0/include/endstone/detail/command/command_sender.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/detail/command/command_usage_parser.h` & `endstone-0.4.0/include/endstone/detail/command/command_usage_parser.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/detail/command/defaults/plugins_command.h` & `endstone-0.4.0/include/endstone/detail/command/defaults/plugins_command.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/detail/command/defaults/version_command.h` & `endstone-0.4.0/include/endstone/detail/command/defaults/version_command.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/detail/command/endstone_command.h` & `endstone-0.4.0/include/endstone/detail/command/endstone_command.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/detail/command/server_command_sender.h` & `endstone-0.4.0/include/endstone/detail/command/server_command_sender.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/detail/hook.h` & `endstone-0.4.0/include/endstone/detail/hook.h`

 * *Files 17% similar despite different names*

```diff
@@ -11,175 +11,129 @@
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
 #include <functional>
+#include <optional>
 #include <system_error>
 
+#include "endstone/detail/cast.h"
+
 namespace endstone::detail::hook {
 void install();
 const std::error_category &hook_error_category();
 }  // namespace endstone::detail::hook
 
 namespace endstone::detail::hook {
 
-/**
- * @brief Cast a function pointer to void pointer
- *
- * @tparam Return The return type of the function.
- * @tparam Args The argument types of the function.
- *
- * @param fp The function pointer to be casted.
- *
- * @return A void pointer to the function.
- */
-template <typename Return, typename... Args>
-void *fp_cast(Return (*fp)(Args...))
-{
-    union {
-        Return (*p)(Args...);
-        void *v;
-    } temp;
-    temp.p = fp;
-    return temp.v;
-}
+void *get_original(void *detour);
+void *get_original(const std::string &name);
 
-/**
- * @brief Cast a member function pointer to void pointer.
- *
- * @tparam Return The return type of the member function.
- * @tparam Class The class type that the member function belongs to.
- * @tparam Args The argument types of the member function.
- *
- * @param fp Pointer to the member function to be casted.
- *
- * @return A void pointer to the member function.
- */
-template <typename Return, typename Class, typename... Args>
-void *fp_cast(Return (Class::*fp)(Args...))
-{
-    union {
-        Return (Class::*p)(Args...);
-        void *v;
-    } temp;
-    temp.p = fp;
-    return temp.v;
-}
+const std::unordered_map<std::string, void *> &get_targets();
+const std::unordered_map<std::string, void *> &get_detours();
 
-/**
- * @brief Cast a constant member function pointer to void pointer.
- *
- * @tparam Return The return type of the constant member function.
- * @tparam Class The class type that the constant member function belongs to.
- * @tparam Args The argument types of the constant member function.
- *
- * @param fp Pointer to the constant member function to be casted.
- *
- * @return A void pointer to the constant member function.
- */
-template <typename Return, typename Class, typename... Args>
-void *fp_cast(Return (Class::*fp)(Args...) const)
-{
-    union {
-        Return (Class::*p)(Args...) const;
-        void *v;
-    } temp;
-    temp.p = fp;
-    return temp.v;
-}
 }  // namespace endstone::detail::hook
 
 namespace endstone::detail::hook {
-void *get_original(void *detour);
-}
-
-namespace endstone::detail::hook {
 /**
  * @brief Construct a std::function from a function pointer
  */
 template <typename Return, typename... Arg>
 inline std::function<Return(Arg...)> get_original(Return (*fp)(Arg...))
 {
     return reinterpret_cast<Return (*)(Arg...)>(get_original(fp_cast(fp)));
 }
 
 /**
  * @brief Construct a std::function from a class method (non-const, no ref-qualifier)
  */
 template <typename Return, typename Class, typename... Arg>
-inline std::function<Return(Class *, Arg...)> get_original(Return (Class::*fp)(Arg...))
+inline std::function<Return(Class *, Arg...)> get_original(Return (Class::*fp)(Arg...),
+                                                           std::optional<std::string> name = std::nullopt)
 {
-    auto func = reinterpret_cast<Return (*)(Class *, Arg...)>(get_original(fp_cast(fp)));
+    auto *original = name.has_value() ? get_original(name.value()) : get_original(fp_cast(fp));
+    auto func = reinterpret_cast<Return (*)(Class *, Arg...)>(original);
     return [func](Class *obj, Arg... args) -> Return {
         return func(obj, std::forward<Arg>(args)...);
     };
 }
 
 /**
  * @brief Construct a std::function from a class method (const, no ref-qualifier)
  */
 template <typename Return, typename Class, typename... Arg>
-inline std::function<Return(const Class *, Arg...)> get_original(Return (Class::*fp)(Arg...) const)
+inline std::function<Return(const Class *, Arg...)> get_original(Return (Class::*fp)(Arg...) const,
+                                                                 std::optional<std::string> name = std::nullopt)
 {
-    auto func = reinterpret_cast<Return (*)(const Class *, Arg...)>(get_original(fp_cast(fp)));
+    auto *original = name.has_value() ? get_original(name.value()) : get_original(fp_cast(fp));
+    auto func = reinterpret_cast<Return (*)(const Class *, Arg...)>(original);
     return [func](const Class *obj, Arg... args) -> Return {
         return func(obj, std::forward<Arg>(args)...);
     };
 }
 }  // namespace endstone::detail::hook
-#define ENDSTONE_HOOK_CALL_ORIGINAL(fp, ...) endstone::detail::hook::get_original(fp)(__VA_ARGS__)
+#define ENDSTONE_HOOK_CALL_ORIGINAL(fp, ...)            endstone::detail::hook::get_original(fp)(__VA_ARGS__)
+#define ENDSTONE_HOOK_CALL_ORIGINAL_NAME(fp, name, ...) endstone::detail::hook::get_original(fp, name)(__VA_ARGS__)
 
 namespace endstone::detail::hook {
 /**
  * @brief Construct a std::function from a function pointer
  * with Return Value Optimization (RVO).
  */
 template <typename Return, typename... Arg>
-inline std::function<Return *(Return *, Arg...)> get_original_rvo(Return (*fp)(Arg...))
+inline std::function<Return *(Return *, Arg...)> get_original_rvo(Return (*fp)(Arg...),
+                                                                  std::optional<std::string> name = std::nullopt)
 {
-    return reinterpret_cast<Return *(*)(Return *, Arg...)>(get_original(fp_cast(fp)));
+    auto *original = name.has_value() ? get_original(name.value()) : get_original(fp_cast(fp));
+    return reinterpret_cast<Return *(*)(Return *, Arg...)>(original);
 }
 
 /**
  * @brief Construct a std::function from a class method (non-const, no ref-qualifier)
  * with Return Value Optimization (RVO).
  */
 template <typename Return, typename Class, typename... Arg>
-inline std::function<Return *(Return *, Class *, Arg...)> get_original_rvo(Return (Class::*fp)(Arg...))
+inline std::function<Return *(Return *, Class *, Arg...)> get_original_rvo(
+    Return (Class::*fp)(Arg...), std::optional<std::string> name = std::nullopt)
 {
+    auto *original = name.has_value() ? get_original(name.value()) : get_original(fp_cast(fp));
 #ifdef _WIN32
-    auto func = reinterpret_cast<Return *(*)(Class *, Return *, Arg...)>(get_original(fp_cast(fp)));
+    auto func = reinterpret_cast<Return *(*)(Class *, Return *, Arg...)>(original);
     return [func](Return *ret, Class *obj, Arg... args) -> Return * {
         return func(obj, ret, std::forward<Arg>(args)...);
     };
 #elif __linux__
-    auto func = reinterpret_cast<Return *(*)(Return *, Class *, Arg...)>(get_original(fp_cast(fp)));
+    auto func = reinterpret_cast<Return *(*)(Return *, Class *, Arg...)>(original);
     return [func](Return *ret, Class *obj, Arg... args) -> Return * {
         return func(ret, obj, std::forward<Arg>(args)...);
     };
 #endif
 }
 
 /**
  * @brief Construct a std::function from a class method (const, no ref-qualifier)
  * with Return Value Optimization (RVO).
  */
 template <typename Return, typename Class, typename... Arg>
-inline std::function<Return *(Return *, const Class *, Arg...)> get_original_rvo(Return (Class::*fp)(Arg...) const)
+inline std::function<Return *(Return *, const Class *, Arg...)> get_original_rvo(
+    Return (Class::*fp)(Arg...) const, std::optional<std::string> name = std::nullopt)
 {
+    auto *original = name.has_value() ? get_original(name.value()) : get_original(fp_cast(fp));
 #ifdef _WIN32
-    auto func = reinterpret_cast<Return *(*)(const Class *, Return *, Arg...)>(get_original(fp_cast(fp)));
+    auto func = reinterpret_cast<Return *(*)(const Class *, Return *, Arg...)>(original);
     return [func](Return *ret, const Class *obj, Arg... args) -> Return * {
         return func(obj, ret, std::forward<Arg>(args)...);
     };
 #elif __linux__
-    auto func = reinterpret_cast<Return *(*)(Return *, const Class *, Arg...)>(get_original(fp_cast(fp)));
+    auto func = reinterpret_cast<Return *(*)(Return *, const Class *, Arg...)>(original);
     return [func](Return *ret, const Class *obj, Arg... args) -> Return * {
         return func(ret, obj, std::forward<Arg>(args)...);
     };
 #endif
 }
 }  // namespace endstone::detail::hook
 
 #define ENDSTONE_HOOK_CALL_ORIGINAL_RVO(fp, ret, ...) *endstone::detail::hook::get_original_rvo(fp)(&ret, __VA_ARGS__)
+#define ENDSTONE_HOOK_CALL_ORIGINAL_RVO_NAME(fp, name, ret, ...) \
+    *endstone::detail::hook::get_original_rvo(fp, name)(&ret, __VA_ARGS__)
```

### Comparing `endstone-0.3.0/include/endstone/detail/logger_factory.h` & `endstone-0.4.0/include/endstone/detail/logger_factory.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/detail/os.h` & `endstone-0.4.0/include/endstone/detail/os.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/detail/permissions/default_permissions.h` & `endstone-0.4.0/include/endstone/detail/permissions/default_permissions.h`

 * *Files 12% similar despite different names*

```diff
@@ -15,25 +15,24 @@
 #pragma once
 
 #include <memory>
 #include <string>
 #include <unordered_map>
 
 #include "endstone/detail/server.h"
-#include "endstone/detail/singleton.h"
 #include "endstone/permissions/permission.h"
 
 namespace endstone::detail {
 
 class DefaultPermissions {
 public:
     static Permission *registerPermission(std::unique_ptr<Permission> perm, Permission *parent = nullptr);
 
     static Permission *registerPermission(const std::string &name, Permission *parent = nullptr,
                                           const std::string &desc = "",
-                                          PermissionDefault default_value = Permission::DEFAULT_PERMISSION,
+                                          PermissionDefault default_value = Permission::DefaultPermission,
                                           const std::unordered_map<std::string, bool> &children = {});
     static void registerCorePermissions();
     static void registerCommandPermissions(Permission *parent);
 };
 
 }  // namespace endstone::detail
```

### Comparing `endstone-0.3.0/include/endstone/detail/permissions/permissible_base.h` & `endstone-0.4.0/include/endstone/detail/permissions/permissible_base.h`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 namespace endstone::detail {
 
 /**
  * Base Permissible for use in any Permissible object via proxy or extension
  */
 class PermissibleBase : public Permissible {
 public:
-    explicit PermissibleBase(ServerOperator *opable) : opable_(opable), parent_(*this) {}
     explicit PermissibleBase(Permissible *opable) : opable_(opable), parent_(opable ? *opable : *this) {}
 
     [[nodiscard]] bool isOp() const override;
     void setOp(bool value) override;
     [[nodiscard]] bool isPermissionSet(std::string name) const override;
     [[nodiscard]] bool isPermissionSet(const Permission &perm) const override;
     [[nodiscard]] bool hasPermission(std::string name) const override;
@@ -45,13 +44,13 @@
     void recalculatePermissions() override;
     [[nodiscard]] std::unordered_set<PermissionAttachmentInfo *> getEffectivePermissions() const override;
 
 private:
     void calculateChildPermissions(const std::unordered_map<std::string, bool> &children, bool invert,
                                    PermissionAttachment *attachment);
     [[nodiscard]] static bool hasPermission(PermissionDefault default_value, bool op);
-    ServerOperator *opable_;
+    Permissible *opable_;
     Permissible &parent_;
     std::vector<std::unique_ptr<PermissionAttachment>> attachments_{};
     std::unordered_map<std::string, std::unique_ptr<PermissionAttachmentInfo>> permissions_{};
 };
 }  // namespace endstone::detail
```

### Comparing `endstone-0.3.0/include/endstone/detail/plugin/cpp_plugin_loader.h` & `endstone-0.4.0/include/endstone/detail/plugin/cpp_plugin_loader.h`

 * *Files 4% similar despite different names*

```diff
@@ -16,24 +16,22 @@
 
 #include <memory>
 #include <string>
 #include <vector>
 
 #include "endstone/plugin/plugin_loader.h"
 
-namespace endstone {
-namespace detail {
+namespace endstone::detail {
 
 class CppPluginLoader : public PluginLoader {
 public:
     using PluginLoader::PluginLoader;
 
     [[nodiscard]] std::vector<Plugin *> loadPlugins(const std::string &directory) override;
     [[nodiscard]] std::unique_ptr<Plugin> loadPlugin(const std::string &file);
     [[nodiscard]] std::vector<std::string> getPluginFileFilters() const;
 
 private:
     std::vector<std::unique_ptr<Plugin>> plugins_;
 };
 
-}  // namespace detail
-}  // namespace endstone
+}  // namespace endstone::detail
```

### Comparing `endstone-0.3.0/include/endstone/detail/plugin/plugin_description_builder.h` & `endstone-0.4.0/include/endstone/detail/plugin/plugin_description_builder.h`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     {
         return Permission(name_, description_, default_value_, children_);
     }
 
 private:
     std::string name_;
     std::string description_;
-    PermissionDefault default_value_ = Permission::DEFAULT_PERMISSION;
+    PermissionDefault default_value_ = Permission::DefaultPermission;
     std::unordered_map<std::string, bool> children_ = {};
 };
 
 struct PluginDescriptionBuilder {
     std::string description;
     PluginLoadOrder load = PluginLoadOrder::PostWorld;
     std::vector<std::string> authors;
```

### Comparing `endstone-0.3.0/include/endstone/detail/plugin/plugin_manager.h` & `endstone-0.4.0/include/endstone/detail/plugin/plugin_manager.h`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #pragma once
 
 #include <memory>
 #include <string>
 #include <unordered_map>
 #include <vector>
 
+#include "endstone/event/handler_list.h"
 #include "endstone/permissions/permission.h"
 #include "endstone/plugin/plugin_loader.h"
 #include "endstone/plugin/plugin_manager.h"
 #include "endstone/server.h"
 
 namespace endstone::detail {
 
@@ -39,14 +40,19 @@
     std::vector<Plugin *> loadPlugins(const std::string &directory) override;
     void enablePlugin(Plugin &plugin) const override;
     void enablePlugins() const override;
     void disablePlugin(Plugin &plugin) const override;
     void disablePlugins() const override;
     void clearPlugins() override;
 
+    /** Event system */
+    void callEvent(Event &event) override;
+    void registerEvent(std::string event, std::function<void(Event &)> executor, EventPriority priority, Plugin &plugin,
+                       bool ignore_cancelled) override;
+
     /** Permission system */
     [[nodiscard]] Permission *getPermission(std::string name) const override;
     Permission *addPermission(std::unique_ptr<Permission> perm) override;
     void removePermission(Permission &perm) override;
     void removePermission(std::string name) override;
     [[nodiscard]] std::unordered_set<Permission *> getDefaultPermissions(bool op) const override;
     void recalculatePermissionDefaults(Permission &perm) override;
@@ -62,14 +68,15 @@
     friend class EndstoneServer;
     void calculatePermissionDefault(Permission &perm);
     void dirtyPermissibles(bool op) const;
     Server &server_;
     std::vector<std::unique_ptr<PluginLoader>> plugin_loaders_;
     std::vector<Plugin *> plugins_;
     std::unordered_map<std::string, Plugin *> lookup_names_;
+    std::unordered_map<std::string, HandlerList> event_handlers_;
     std::unordered_map<std::string, std::unique_ptr<Permission>> permissions_;
     std::unordered_map<bool, std::unordered_set<Permission *>> default_perms_;
     std::unordered_map<std::string, std::unordered_map<Permissible *, bool>> perm_subs_;
     std::unordered_map<bool, std::unordered_map<Permissible *, bool>> def_subs_;
 };
 
 }  // namespace endstone::detail
```

### Comparing `endstone-0.3.0/include/endstone/detail/plugin/python_plugin_loader.h` & `endstone-0.4.0/include/endstone/detail/plugin/python_plugin_loader.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/detail/server.h` & `endstone-0.4.0/include/endstone/detail/server.h`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #include <string>
 #include <string_view>
 
 #include "bedrock/server/server_instance.h"
 #include "endstone/detail/command/command_map.h"
 #include "endstone/detail/command/server_command_sender.h"
 #include "endstone/detail/plugin/plugin_manager.h"
+#include "endstone/level.h"
 #include "endstone/plugin/plugin_manager.h"
 #include "endstone/server.h"
 
 namespace endstone::detail {
 
 class EndstoneServer : public Server {
 public:
@@ -43,21 +44,29 @@
     [[nodiscard]] PluginCommand *getPluginCommand(std::string name) const override;
     [[nodiscard]] CommandSender &getCommandSender() const override;
 
     void loadPlugins();
     void enablePlugins(PluginLoadOrder type);
     void disablePlugins() const;
 
+    std::vector<Level *> getLevels() const override;
+    Level *getLevel(std::string name) const override;
+    void addLevel(std::unique_ptr<Level> level);
+
+    [[nodiscard]] Player *getPlayer(endstone::UUID id) const override;
+
     [[nodiscard]] std::string getName() const override;
     [[nodiscard]] std::string getVersion() const override;
     [[nodiscard]] std::string getMinecraftVersion() const override;
+    bool isPrimaryThread() const override;
 
 private:
     void enablePlugin(Plugin &plugin);
     ServerInstance &server_instance_;
     Logger &logger_;
     std::unique_ptr<EndstoneCommandMap> command_map_;
     std::unique_ptr<EndstonePluginManager> plugin_manager_;
     mutable ServerCommandSender command_sender_;
+    std::unordered_map<std::string, std::unique_ptr<Level>> levels_;
 };
 
 }  // namespace endstone::detail
```

### Comparing `endstone-0.3.0/include/endstone/detail/singleton.h` & `endstone-0.4.0/include/bedrock/world/level/dimension/dimension_interface.h`

 * *Files 24% similar despite different names*

```diff
@@ -10,40 +10,17 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
-#include <memory>
-#include <stdexcept>
+#include "bedrock/automatic_id.h"
 
-namespace endstone::detail {
-
-template <typename T>
-class Singleton {
+class Dimension;
 
+class IDimension {
 public:
-    Singleton() = delete;
-
-    static void setInstance(std::unique_ptr<T> instance)
-    {
-        if (mInstance) {
-            throw std::runtime_error("Instance is already set");
-        }
-        mInstance = std::move(instance);
-    }
-
-    static T &getInstance()
-    {
-        return *mInstance;
-    }
-
-    static void reset()
-    {
-        mInstance.reset();
-    }
-
-private:
-    inline static std::unique_ptr<T> mInstance = nullptr;
+    virtual ~IDimension() = 0;
+    [[nodiscard]] virtual bool isNaturalDimension() const = 0;
+    [[nodiscard]] virtual AutomaticID<Dimension, int> getDimensionId() const = 0;
 };
-}  // namespace endstone::detail
```

### Comparing `endstone-0.3.0/include/endstone/detail/spdlog/level_formatter.h` & `endstone-0.4.0/include/endstone/detail/spdlog/level_formatter.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/detail/spdlog/log_sink.h` & `endstone-0.4.0/include/endstone/detail/spdlog/log_sink.h`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     /// Bold colors
     const spdlog::string_view_t yellow_bold = "\033[33m\033[1m";
     const spdlog::string_view_t red_bold = "\033[31m\033[1m";
     const spdlog::string_view_t bold_on_red = "\033[1m\033[41m";
 
 private:
     void printColorCode(const spdlog::string_view_t &color_code);
-    void printRange(const spdlog::memory_buf_t &formatted, size_t start, size_t end);
+    void printRange(const spdlog::memory_buf_t &formatted, std::size_t start, std::size_t end);
     static std::string toString(const spdlog::string_view_t &sv);
 
     FILE *target_file_;
     bool should_do_colors_;
     std::array<std::string, spdlog::level::n_levels> colors_;
 };
```

### Comparing `endstone-0.3.0/include/endstone/detail/spdlog/spdlog_adapter.h` & `endstone-0.4.0/include/endstone/detail/spdlog/spdlog_adapter.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/detail/spdlog/text_formatter.h` & `endstone-0.4.0/include/endstone/detail/spdlog/text_formatter.h`

 * *Files 11% similar despite different names*

```diff
@@ -13,61 +13,61 @@
 // limitations under the License.
 
 #pragma once
 
 #include <spdlog/pattern_formatter.h>
 #include <spdlog/spdlog.h>
 
-#include "endstone/util/color_format.h"
+#include "endstone/color_format.h"
 
 namespace endstone::detail {
 
 class TextFormatter : public spdlog::custom_flag_formatter {
 public:
     explicit TextFormatter(bool should_do_colors) : should_do_colors_(should_do_colors){};
     void format(const spdlog::details::log_msg &msg, const std::tm &, spdlog::memory_buf_t &dest) override;
     [[nodiscard]] std::unique_ptr<custom_flag_formatter> clone() const override;
 
 private:
     const std::unordered_map<unsigned char, spdlog::string_view_t> ansi_codes = {
         // References: https://minecraft.wiki/w/Formatting_codes
 
         // Color codes
-        {ColorFormat::BLACK.back(), "\x1b[30m"},
-        {ColorFormat::DARK_BLUE.back(), "\x1b[34m"},
-        {ColorFormat::DARK_GREEN.back(), "\x1b[32m"},
-        {ColorFormat::DARK_AQUA.back(), "\x1b[36m"},
-        {ColorFormat::DARK_RED.back(), "\x1b[31m"},
-        {ColorFormat::DARK_PURPLE.back(), "\x1b[35m"},
-        {ColorFormat::GOLD.back(), "\x1b[33m"},
-        {ColorFormat::GRAY.back(), "\x1b[37m"},
-        {ColorFormat::DARK_GRAY.back(), "\x1b[90m"},
-        {ColorFormat::BLUE.back(), "\x1b[94m"},
-        {ColorFormat::GREEN.back(), "\x1b[92m"},
-        {ColorFormat::AQUA.back(), "\x1b[96m"},
-        {ColorFormat::RED.back(), "\x1b[91m"},
-        {ColorFormat::LIGHT_PURPLE.back(), "\x1b[95m"},
-        {ColorFormat::YELLOW.back(), "\x1b[93m"},
-        {ColorFormat::WHITE.back(), "\x1b[97m"},
-        {ColorFormat::MINECOIN_GOLD.back(), "\x1b[38;2;221;214;5m"},
-        {ColorFormat::MATERIAL_QUARTZ.back(), "\x1b[38;2;227;212;209m"},
-        {ColorFormat::MATERIAL_IRON.back(), "\x1b[38;2;206;202;202m"},
-        {ColorFormat::MATERIAL_NETHERITE.back(), "\x1b[38;2;68;58;59m"},
-        {ColorFormat::MATERIAL_REDSTONE.back(), "\x1b[38;2;151;22;7m"},
-        {ColorFormat::MATERIAL_COPPER.back(), "\x1b[38;2;180;104;77m"},
-        {ColorFormat::MATERIAL_GOLD.back(), "\x1b[38;2;222;177;45m"},
-        {ColorFormat::MATERIAL_EMERALD.back(), "\x1b[38;2;17;160;54m"},
-        {ColorFormat::MATERIAL_DIAMOND.back(), "\x1b[38;2;44;186;168m"},
-        {ColorFormat::MATERIAL_LAPIS.back(), "\x1b[38;2;33;73;123m"},
-        {ColorFormat::MATERIAL_AMETHYST.back(), "\x1b[38;2;154;92;198m"},
+        {ColorFormat::Black.back(), "\x1b[30m"},
+        {ColorFormat::DarkBlue.back(), "\x1b[34m"},
+        {ColorFormat::DarkGreen.back(), "\x1b[32m"},
+        {ColorFormat::DarkAqua.back(), "\x1b[36m"},
+        {ColorFormat::DarkRed.back(), "\x1b[31m"},
+        {ColorFormat::DarkPurple.back(), "\x1b[35m"},
+        {ColorFormat::Gold.back(), "\x1b[33m"},
+        {ColorFormat::Gray.back(), "\x1b[37m"},
+        {ColorFormat::DarkGray.back(), "\x1b[90m"},
+        {ColorFormat::Blue.back(), "\x1b[94m"},
+        {ColorFormat::Green.back(), "\x1b[92m"},
+        {ColorFormat::Aqua.back(), "\x1b[96m"},
+        {ColorFormat::Red.back(), "\x1b[91m"},
+        {ColorFormat::LightPurple.back(), "\x1b[95m"},
+        {ColorFormat::Yellow.back(), "\x1b[93m"},
+        {ColorFormat::White.back(), "\x1b[97m"},
+        {ColorFormat::MinecoinGold.back(), "\x1b[38;2;221;214;5m"},
+        {ColorFormat::MaterialQuartz.back(), "\x1b[38;2;227;212;209m"},
+        {ColorFormat::MaterialIron.back(), "\x1b[38;2;206;202;202m"},
+        {ColorFormat::MaterialNetherite.back(), "\x1b[38;2;68;58;59m"},
+        {ColorFormat::MaterialRedstone.back(), "\x1b[38;2;151;22;7m"},
+        {ColorFormat::MaterialCopper.back(), "\x1b[38;2;180;104;77m"},
+        {ColorFormat::MaterialGold.back(), "\x1b[38;2;222;177;45m"},
+        {ColorFormat::MaterialEmerald.back(), "\x1b[38;2;17;160;54m"},
+        {ColorFormat::MaterialDiamond.back(), "\x1b[38;2;44;186;168m"},
+        {ColorFormat::MaterialLapis.back(), "\x1b[38;2;33;73;123m"},
+        {ColorFormat::MaterialAmethyst.back(), "\x1b[38;2;154;92;198m"},
 
         // Formatting codes
-        {ColorFormat::OBFUSCATED.back(), "\x1b[8m"},
-        {ColorFormat::BOLD.back(), "\x1b[1m"},
-        {ColorFormat::ITALIC.back(), "\x1b[3m"},
-        {ColorFormat::RESET.back(), "\x1b[0m"},
+        {ColorFormat::Obfuscated.back(), "\x1b[8m"},
+        {ColorFormat::Bold.back(), "\x1b[1m"},
+        {ColorFormat::Italic.back(), "\x1b[3m"},
+        {ColorFormat::Reset.back(), "\x1b[0m"},
     };
 
     bool should_do_colors_;
 };
 
 }  // namespace endstone::detail
```

### Comparing `endstone-0.3.0/include/endstone/endstone.h` & `endstone-0.4.0/include/endstone/endstone.h`

 * *Files 19% similar despite different names*

```diff
@@ -14,18 +14,31 @@
 
 #pragma once
 
 #define ENDSTONE_STRINGIFY(x) #x
 #define ENDSTONE_TOSTRING(x)  ENDSTONE_STRINGIFY(x)
 
 #define ENDSTONE_VERSION_MAJOR 0
-#define ENDSTONE_VERSION_MINOR 3
+#define ENDSTONE_VERSION_MINOR 4
 #define ENDSTONE_VERSION_PATCH 0
 #define ENDSTONE_API_VERSION   ENDSTONE_TOSTRING(ENDSTONE_VERSION_MAJOR) "." ENDSTONE_TOSTRING(ENDSTONE_VERSION_MINOR);
 
 #if !defined(ENDSTONE_EXPORT)
 #if defined(WIN32) || defined(_WIN32)
 #define ENDSTONE_EXPORT __declspec(dllexport)
 #else
 #define ENDSTONE_EXPORT __attribute__((visibility("default")))
 #endif
+
+#if defined(_MSC_VER)
+#define ENDSTONE_NOINLINE __declspec(noinline) inline
+#else
+#define ENDSTONE_NOINLINE __attribute__((noinline)) inline
+#endif
+
+#ifdef _WIN32
+#define _WIN32_LINUX_(win32, linux) win32
+#elif __linux__
+#define _WIN32_LINUX_(win32, linux) linux
+#endif
+
 #endif
```

### Comparing `endstone-0.3.0/include/endstone/logger.h` & `endstone-0.4.0/include/endstone/logger.h`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  * @brief Logger class which can format and output varies levels of logs.
  */
 class Logger {
 public:
     /**
      * @brief Specifies the log level.
      */
-    enum Level : uint8_t {
+    enum Level : std::uint8_t {
         Trace = 0,
         Debug = 1,
         Info = 2,
         Warning = 3,
         Error = 4,
         Critical = 5,
         Off = 6,
```

### Comparing `endstone-0.3.0/include/endstone/permissions/permissible.h` & `endstone-0.4.0/include/endstone/permissions/permissible.h`

 * *Files 9% similar despite different names*

```diff
@@ -14,28 +14,41 @@
 
 #pragma once
 
 #include <string>
 #include <unordered_set>
 
 #include "endstone/permissions/permission_attachment_info.h"
-#include "endstone/permissions/server_operator.h"
 
 namespace endstone {
 
 class Plugin;
 class Permission;
 class PermissionAttachment;
 
 /**
- * Represents an object that may be assigned permissions
+ * Represents an object that may become a server operator and can be assigned permissions.
  */
-class Permissible : public ServerOperator {
+class Permissible {
 public:
-    ~Permissible() override = default;
+    virtual ~Permissible() = default;
+
+    /**
+     * @brief Checks if this object is a server operator
+     *
+     * @return true if this is an operator, otherwise false
+     */
+    [[nodiscard]] virtual bool isOp() const = 0;
+
+    /**
+     * @brief Sets the operator status of this object
+     *
+     * @param value New operator value
+     */
+    virtual void setOp(bool value) = 0;
 
     /**
      * Checks if this object contains an override for the specified permission, by fully qualified name
      *
      * @param name Name of the permission
      * @return true if the permission is set, otherwise false
      */
```

### Comparing `endstone-0.3.0/include/endstone/permissions/permission.h` & `endstone-0.4.0/include/endstone/permissions/permission.h`

 * *Files 3% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 namespace endstone {
 
 /**
  * Represents a unique permission that may be attached to a Permissible
  */
 class Permission {
 public:
-    static const PermissionDefault DEFAULT_PERMISSION = PermissionDefault::Operator;
+    static const PermissionDefault DefaultPermission = PermissionDefault::Operator;
 
     explicit Permission(std::string name, std::string description = "",
-                        PermissionDefault default_value = DEFAULT_PERMISSION,
+                        PermissionDefault default_value = DefaultPermission,
                         std::unordered_map<std::string, bool> children = {})
     {
         this->name_ = std::move(name);
         this->description_ = std::move(description);
         this->default_value_ = default_value;
         this->children_ = std::move(children);
     }
@@ -186,13 +186,13 @@
     {
         plugin_manager_ = &plugin_manager;
     }
 
 private:
     std::string name_;
     std::unordered_map<std::string, bool> children_;
-    PermissionDefault default_value_ = DEFAULT_PERMISSION;
+    PermissionDefault default_value_ = DefaultPermission;
     std::string description_;
     PluginManager *plugin_manager_;
 };
 
 }  // namespace endstone
```

### Comparing `endstone-0.3.0/include/endstone/permissions/permission_attachment.h` & `endstone-0.4.0/include/endstone/permissions/permission_attachment.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/permissions/permission_attachment_info.h` & `endstone-0.4.0/include/endstone/permissions/permission_attachment_info.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/permissions/permission_default.h` & `endstone-0.4.0/include/endstone/permissions/permission_default.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/permissions/server_operator.h` & `endstone-0.4.0/include/endstone/event/actor/actor_remove_event.h`

 * *Files 24% similar despite different names*

```diff
@@ -10,30 +10,37 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
+#include "endstone/event/actor/actor_event.h"
+
 namespace endstone {
+
 /**
- * @brief Represents an object that may become a server operator, such as a Player
+ * Called when an Actor is removed.
+ *
+ * This event should only be used for monitoring. Modifying the actor during or after this event leads to undefined
+ * behaviours. This event will not be called for Players.
  */
-class ServerOperator {
+class ActorRemoveEvent : public ActorEvent {
 public:
-    virtual ~ServerOperator() = default;
+    explicit ActorRemoveEvent(Actor &actor) : ActorEvent(actor) {}
+    ~ActorRemoveEvent() override = default;
+
+    inline static const std::string NAME = "ActorRemoveEvent";
+    [[nodiscard]] std::string getEventName() const override
+    {
+        return NAME;
+    }
 
-    /**
-     * @brief Checks if this object is a server operator
-     *
-     * @return true if this is an operator, otherwise false
-     */
-    [[nodiscard]] virtual bool isOp() const = 0;
-
-    /**
-     * @brief Sets the operator status of this object
-     *
-     * @param value New operator value
-     */
-    virtual void setOp(bool value) = 0;
+    [[nodiscard]] bool isCancellable() const override
+    {
+        return false;
+    }
+
+    // TODO(event): add remove cause
 };
+
 }  // namespace endstone
```

### Comparing `endstone-0.3.0/include/endstone/plugin/plugin.h` & `endstone-0.4.0/include/endstone/plugin/plugin.h`

 * *Files 15% similar despite different names*

```diff
@@ -133,14 +133,32 @@
      */
     [[nodiscard]] PluginCommand *getCommand(std::string name) const
     {
         std::transform(name.begin(), name.end(), name.begin(), [](unsigned char c) { return std::tolower(c); });
         return getServer().getPluginCommand(name);
     }
 
+    template <typename EventType, typename T>
+    void registerEvent(void (T::*func)(EventType &), T &instance, EventPriority priority = EventPriority::Normal,
+                       bool ignore_cancelled = false)
+    {
+        getServer().getPluginManager().registerEvent(
+            EventType::NAME, [func, &instance](Event &e) { (instance.*func)(static_cast<EventType &>(e)); }, priority,
+            *this, ignore_cancelled);
+    }
+
+    template <typename EventType>
+    void registerEvent(std::function<void(EventType &)> func, EventPriority priority = EventPriority::Normal,
+                       bool ignore_cancelled = false)
+    {
+        getServer().getPluginManager().registerEvent(
+            EventType::NAME, [func](Event &e) { func(static_cast<EventType &>(e)); }, priority, *this,
+            ignore_cancelled);
+    }
+
 private:
     friend class PluginLoader;
 
     /**
      * Sets the enabled state of this plugin
      *
      * @param enabled true if enabled, otherwise false
@@ -164,30 +182,31 @@
     Server *server_{nullptr};
     Logger *logger_{nullptr};
 };
 
 }  // namespace endstone
 
 #ifndef ENDSTONE_PLUGIN
-#define ENDSTONE_PLUGIN(Name, Version, MainClass)                                                       \
-    static endstone::detail::PluginDescriptionBuilder builder;                                          \
-    [[maybe_unused]] static void init_plugin_description(endstone::detail::PluginDescriptionBuilder &); \
-    class EndstonePluginImpl : public MainClass {                                                       \
-    public:                                                                                             \
-        EndstonePluginImpl() = default;                                                                 \
-        const endstone::PluginDescription &getDescription() const override                              \
-        {                                                                                               \
-            return description_;                                                                        \
-        }                                                                                               \
-                                                                                                        \
-    private:                                                                                            \
-        endstone::PluginDescription description_ = builder.build(Name, Version);                        \
-    };                                                                                                  \
-    extern "C" [[maybe_unused]] ENDSTONE_EXPORT endstone::Plugin *init_endstone_plugin();               \
-    extern "C" ENDSTONE_EXPORT endstone::Plugin *init_endstone_plugin()                                 \
-    {                                                                                                   \
-        init_plugin_description(builder);                                                               \
-        auto *p = new EndstonePluginImpl();                                                             \
-        return p;                                                                                       \
-    }                                                                                                   \
-    void init_plugin_description(endstone::detail::PluginDescriptionBuilder &plugin)
+#define ENDSTONE_PLUGIN(Name, Version, MainClass)                                            \
+    class PluginDescriptionBuilderImpl : public endstone::detail::PluginDescriptionBuilder { \
+    public:                                                                                  \
+        PluginDescriptionBuilderImpl();                                                      \
+    };                                                                                       \
+    static PluginDescriptionBuilderImpl builder;                                             \
+    class EndstonePluginImpl : public MainClass {                                            \
+    public:                                                                                  \
+        EndstonePluginImpl() = default;                                                      \
+        const endstone::PluginDescription &getDescription() const override                   \
+        {                                                                                    \
+            return description_;                                                             \
+        }                                                                                    \
+                                                                                             \
+    private:                                                                                 \
+        endstone::PluginDescription description_ = builder.build(Name, Version);             \
+    };                                                                                       \
+    extern "C" [[maybe_unused]] ENDSTONE_EXPORT endstone::Plugin *init_endstone_plugin()     \
+    {                                                                                        \
+        auto *p = new EndstonePluginImpl();                                                  \
+        return p;                                                                            \
+    }                                                                                        \
+    PluginDescriptionBuilderImpl::PluginDescriptionBuilderImpl()
 #endif
```

### Comparing `endstone-0.3.0/include/endstone/plugin/plugin_description.h` & `endstone-0.4.0/include/endstone/plugin/plugin_description.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/plugin/plugin_load_order.h` & `endstone-0.4.0/include/endstone/plugin/plugin_load_order.h`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/include/endstone/plugin/plugin_loader.h` & `endstone-0.4.0/include/endstone/plugin/plugin_loader.h`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 #pragma once
 
 #include <memory>
 #include <string>
 #include <vector>
 
+#include "endstone/event/server/plugin_disable_event.h"
+#include "endstone/event/server/plugin_enable_event.h"
 #include "endstone/logger.h"
 #include "endstone/plugin/plugin.h"
 #include "endstone/server.h"
 
 namespace endstone {
 
 class PluginLoader {
@@ -47,28 +49,32 @@
      * @param plugin Plugin to enable
      */
     virtual void enablePlugin(Plugin &plugin) const
     {
         if (!plugin.isEnabled()) {
             plugin.getLogger().info("Enabling {}", plugin.getDescription().getFullName());
             plugin.setEnabled(true);
+            PluginEnableEvent event(plugin);
+            server_.getPluginManager().callEvent(event);
         }
     }
 
     /**
      * Disables the specified plugin
      * Attempting to disable a plugin that is not enabled will have no effect
      *
      * @param plugin Plugin to disable
      */
     virtual void disablePlugin(Plugin &plugin) const
     {
         if (plugin.isEnabled()) {
             plugin.getLogger().info("Disabling {}", plugin.getDescription().getFullName());
             plugin.setEnabled(false);
+            PluginDisableEvent event(plugin);
+            server_.getPluginManager().callEvent(event);
         }
     }
 
     /**
      * @brief Retrieves the Server object associated with the PluginLoader.
      *
      * This function returns a reference to the Server object that the PluginLoader is associated with.
```

### Comparing `endstone-0.3.0/include/endstone/plugin/plugin_manager.h` & `endstone-0.4.0/include/endstone/plugin/plugin_manager.h`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,22 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
+#include <functional>
 #include <memory>
 #include <string>
 #include <vector>
 
+#include "endstone/event/event.h"
+#include "endstone/event/event_priority.h"
+
 namespace endstone {
 
 class Permission;
 class Permissible;
 class Plugin;
 class PluginLoader;
 
@@ -108,14 +112,34 @@
 
     /**
      * Disables and removes all plugins
      */
     virtual void clearPlugins() = 0;
 
     /**
+     * Calls an event which will be passed to plugins.
+     *
+     * @param event Event to be called
+     */
+    virtual void callEvent(Event &event) = 0;
+
+    /**
+     * Registers the given event
+     *
+     * @param event Event name to register
+     * @param executor EventExecutor to register
+     * @param priority Priority of this event
+     * @param plugin Plugin to register
+     * @param ignore_cancelled Do not call executor if event was already
+     *     cancelled
+     */
+    virtual void registerEvent(std::string event, std::function<void(Event &)> executor, EventPriority priority,
+                               Plugin &plugin, bool ignore_cancelled) = 0;
+
+    /**
      * Gets a Permission from its fully qualified name
      *
      * @param name Name of the permission
      * @return Permission, or null if none
      */
     [[nodiscard]] virtual Permission *getPermission(std::string name) const = 0;
```

### Comparing `endstone-0.3.0/mkdocs.yml` & `endstone-0.4.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/pyproject.toml` & `endstone-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 Homepage = "https://github.com/EndstoneMC/endstone"
 Issues = "https://github.com/EndstoneMC/endstone/issues"
 
 [project.scripts]
 endstone = "endstone._internal.bootstrap:cli"
 
 [tool.scikit-build]
-cmake.args = ["-G Ninja", "--preset conan-release"]
+cmake.args = ["-G Ninja", "--preset conan-relwithdebinfo"]
 cmake.define = { BUILD_TESTING = "OFF" }
 wheel.packages = ["python/src/endstone"]
 wheel.license-files = ["LICENSE"]
 install.components = ["endstone_wheel"]
 install.strip = false
 metadata.version.provider = "scikit_build_core.metadata.setuptools_scm"
 sdist.include = ["python/src/endstone/_internal/version.py"]
```

### Comparing `endstone-0.3.0/python/src/endstone/_internal/bootstrap/__init__.py` & `endstone-0.4.0/python/src/endstone/_internal/bootstrap/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import functools
 import logging
 import os
 import platform
 import sys
 
 import click
-from endstone._internal.version import __version__, __version_tuple__
+from endstone._internal.version import __version__
 
 logging.basicConfig(
     level=logging.INFO,
     format="[%(asctime)s.%(msecs)03d %(levelname)s] [%(name)s] %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 logger = logging.getLogger(__name__)
@@ -64,15 +64,15 @@
         install (bool): Whether to install the bedrock server if not already installed.
         remote (str): The remote URL to retrieve bedrock server data from.
 
     Raises:
         NotImplementedError: If the operating system is not supported.
         FileNotFoundError: If the server executable is not found and install is set to False.
     """
-    from endstone import __minecraft__version__ as minecraft_version
+    from endstone import __minecraft_version__ as minecraft_version
 
     system = platform.system()
     if system == "Windows":
         from endstone._internal.bootstrap.windows import WindowsBootstrap
 
         cls = WindowsBootstrap
```

### Comparing `endstone-0.3.0/python/src/endstone/_internal/bootstrap/base.py` & `endstone-0.4.0/python/src/endstone/_internal/bootstrap/base.py`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/python/src/endstone/_internal/bootstrap/linux.py` & `endstone-0.4.0/python/src/endstone/_internal/bootstrap/linux.py`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/python/src/endstone/_internal/bootstrap/windows.py` & `endstone-0.4.0/python/src/endstone/_internal/bootstrap/windows.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ctypes
+import os
 import subprocess
 from ctypes import get_last_error
 from ctypes.wintypes import (
     BOOL,
     DWORD,
     LPCSTR,
     LPCWSTR,
@@ -100,16 +101,26 @@
             return ret > 32
         else:
             return True
 
     def _create_process(self, *args, **kwargs) -> None:
         self._add_loopback_exemption()
 
+        # Add paths for symbol lookup
+        env = os.environ.copy()
+        symbol_path = env.get("_NT_SYMBOL_PATH", "")
+        symbol_path_list = symbol_path.split(os.pathsep)
+        symbol_path_list = [
+            str(self._endstone_runtime_path.parent.absolute()),
+            str(self.plugin_path.absolute()),
+        ] + symbol_path_list
+        env["_NT_SYMBOL_PATH"] = os.pathsep.join(symbol_path_list)
+
         # Create the process is a suspended state
-        super()._create_process(creationflags=CREATE_SUSPENDED)
+        super()._create_process(creationflags=CREATE_SUSPENDED, env=env)
         handle_proc = int(self._process._handle)
         lib_path = str(self._endstone_runtime_path.absolute())
 
         # Allocate memory for lib_path
         address = kernel32.VirtualAllocEx(
             handle_proc,  # hProcess
             0,  # lpAddress
```

### Comparing `endstone-0.3.0/python/src/endstone/_internal/plugin_loader.py` & `endstone-0.4.0/python/src/endstone/_internal/plugin_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from importlib.metadata import entry_points, metadata
 from typing import List
 
+from endstone import Server
 from endstone.command import Command
 from endstone.permissions import Permission, PermissionDefault
 from endstone.plugin import PluginDescription, PluginLoader, Plugin, PluginLoadOrder
-from endstone.server import Server
 
 
 class PythonPluginLoader(PluginLoader):
-    SUPPORTED_API = ["0.2", "0.3"]
+    SUPPORTED_API = ["0.2", "0.3", "0.4"]
 
     def __init__(self, server: Server):
         PluginLoader.__init__(self, server)
         self._plugins = []
 
     @staticmethod
     def _build_commands(commands: dict) -> list[Command]:
```

### Comparing `endstone-0.3.0/python/tests/test_color_format.py` & `endstone-0.4.0/python/tests/test_color_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import importlib
 
 import pytest
 
 
 @pytest.fixture
 def cls():
-    module = importlib.import_module("endstone.util")
+    module = importlib.import_module("endstone")
     return getattr(module, "ColorFormat")
 
 
 def test_color_format(cls):
     assert getattr(cls, "BLACK") == "§0"
     assert getattr(cls, "DARK_BLUE") == "§1"
     assert getattr(cls, "DARK_GREEN") == "§2"
```

### Comparing `endstone-0.3.0/python/tests/test_plugin_description.py` & `endstone-0.4.0/python/tests/test_plugin_description.py`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/src/endstone_core/command/bedrock_command.cpp` & `endstone-0.4.0/src/endstone_core/command/bedrock_command.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/src/endstone_core/command/command_adapter.cpp` & `endstone-0.4.0/src/endstone_core/command/command_adapter.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 #include "endstone/detail/command/command_adapter.h"
 
 #include <stack>
 #include <string>
 #include <vector>
 
+#include <entt/entt.hpp>
+
+#include "bedrock/world/actor/player/player.h"
 #include "endstone/detail/permissions/permissible_base.h"
 
 namespace endstone::detail {
 CommandSenderAdapter::CommandSenderAdapter(const CommandOrigin &origin, CommandOutput &output)
     : origin_(origin), output_(output)
 {
 }
@@ -54,39 +57,49 @@
 void CommandSenderAdapter::setOp(bool value)
 {
     getServer().getLogger().error("Changing the operator status of {} is not supported.", getName());
 }
 
 void CommandAdapter::execute(const CommandOrigin &origin, CommandOutput &output) const
 {
-    auto &server = Singleton<EndstoneServer>::getInstance();
+    auto &server = entt::locator<EndstoneServer>::value();
     auto &command_map = server.getCommandMap();
     auto command_name = getCommandName();
     auto *command = command_map.getCommand(command_name);
 
     if (!command) {
-        server.getLogger().error("Command '{}' was executed by {} but not registered.", origin.getName(), command_name);
+        server.getLogger().error("An unregistered command '{}' was executed by {}.", command_name, origin.getName());
         return;
     }
 
     bool success;
     switch (origin.getOriginType()) {
-    case CommandOriginType::DedicatedServer:
+    case CommandOriginType::DedicatedServer: {
         success = command->execute(server.getCommandSender(), args_);
         break;
-    case CommandOriginType::Player:
+    }
+    case CommandOriginType::Player: {
+        auto *entity = origin.getEntity();
+        if (!entity->isPlayer()) {
+            throw std::runtime_error("Command was executed by an non-player entity");
+        }
+        endstone::Player &player = static_cast<::Player *>(entity)->getEndstonePlayer();
+        success = command->execute(player, args_);
+        break;
+    }
     case CommandOriginType::Entity:
     case CommandOriginType::CommandBlock:
     case CommandOriginType::MinecartCommandBlock:
-        // TODO: add BlockCommandSender, Player, Entity and CommandMinecart
-    default:
+        // TODO(permission): add BlockCommandSender, Entity and CommandMinecart
+    default: {
         auto sender = CommandSenderAdapter(origin, output);
         success = command->execute(sender, args_);
         break;
     }
+    }
 
     if (success) {
         output.success();
     }
 }
 
 }  // namespace endstone::detail
```

### Comparing `endstone-0.3.0/src/endstone_core/command/command_lexer.cpp` & `endstone-0.4.0/src/endstone_core/command/command_lexer.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/src/endstone_core/command/command_map.cpp` & `endstone-0.4.0/src/endstone_core/command/command_map.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 #include "bedrock/command/command_registry.h"
 #include "bedrock/i18n.h"
 #include "bedrock/type_id.h"
 #include "endstone/command/plugin_command.h"
 #include "endstone/detail/command/bedrock_command.h"
 #include "endstone/detail/command/command_adapter.h"
 #include "endstone/detail/command/command_usage_parser.h"
+#include "endstone/detail/command/defaults/debug_command.h"
 #include "endstone/detail/command/defaults/plugins_command.h"
 #include "endstone/detail/command/defaults/version_command.h"
 #include "endstone/detail/server.h"
 
 namespace endstone::detail {
 
 EndstoneCommandMap::EndstoneCommandMap(EndstoneServer &server) : server_(server) {}
@@ -60,14 +61,15 @@
     }
 
     return it->second.get();
 }
 
 void EndstoneCommandMap::setDefaultCommands()
 {
+    registerCommand(std::make_unique<DebugCommand>());
     registerCommand(std::make_unique<PluginsCommand>());
     registerCommand(std::make_unique<VersionCommand>());
 }
 
 void EndstoneCommandMap::setMinecraftCommands()
 {
     auto &commands = server_.getMinecraftCommands();
@@ -99,28 +101,28 @@
 
         known_commands_.emplace(signature.name, std::move(command));
     }
 }
 
 namespace {
 std::unordered_map<std::string, CommandRegistry::Symbol> gTypeSymbols = {
-    {"int", CommandRegistry::Symbol::INT},
-    {"float", CommandRegistry::Symbol::FLOAT},
-    {"actor", CommandRegistry::Symbol::SELECTOR},
-    {"player", CommandRegistry::Symbol::SELECTOR},
-    {"target", CommandRegistry::Symbol::SELECTOR},
-    {"string", CommandRegistry::Symbol::STRING},
-    {"str", CommandRegistry::Symbol::STRING},
-    {"block_pos", CommandRegistry::Symbol::POSITION},
-    {"vec3i", CommandRegistry::Symbol::POSITION},
-    {"pos", CommandRegistry::Symbol::POSITION_FLOAT},
-    {"vec3", CommandRegistry::Symbol::POSITION_FLOAT},
-    {"vec3f", CommandRegistry::Symbol::POSITION_FLOAT},
-    {"message", CommandRegistry::Symbol::MESSAGE},
-    {"json", CommandRegistry::Symbol::JSON},
+    {"int", CommandRegistry::Symbol::Int},
+    {"float", CommandRegistry::Symbol::Float},
+    {"actor", CommandRegistry::Symbol::Selector},
+    {"player", CommandRegistry::Symbol::Selector},
+    {"target", CommandRegistry::Symbol::Selector},
+    {"string", CommandRegistry::Symbol::String},
+    {"str", CommandRegistry::Symbol::String},
+    {"block_pos", CommandRegistry::Symbol::Position},
+    {"vec3i", CommandRegistry::Symbol::Position},
+    {"pos", CommandRegistry::Symbol::PositionFloat},
+    {"vec3", CommandRegistry::Symbol::PositionFloat},
+    {"vec3f", CommandRegistry::Symbol::PositionFloat},
+    {"message", CommandRegistry::Symbol::Message},
+    {"json", CommandRegistry::Symbol::Json},
 };
 }  // namespace
 
 bool EndstoneCommandMap::registerCommand(std::shared_ptr<Command> command)
 {
     std::lock_guard lock(mutex_);
 
@@ -131,15 +133,15 @@
     auto name = command->getName();
     if (auto it = known_commands_.find(name); it != known_commands_.end() && it->second->getName() == it->first) {
         return false;  // the name was registered and is not an alias, we don't replace it
     }
 
     auto &registry = server_.getMinecraftCommands().getRegistry();
     registry.registerCommand(name, command->getDescription().c_str(), CommandPermissionLevel::Any,
-                             CommandFlag::NOT_REQUIRE_CHEAT, CommandFlag::NONE);
+                             CommandFlag::WithoutCheatEnabled, CommandFlag::None);
     known_commands_.emplace(name, command);
 
     std::vector<std::string> registered_alias;
     for (const auto &alias : command->getAliases()) {
         if (known_commands_.find(alias) == known_commands_.end()) {
             registry.registerAlias(name, alias);
             known_commands_.emplace(alias, command);
@@ -171,14 +173,20 @@
                         server_.getLogger().error("Unable to register enum '{}'.", parameter.type);
                         return false;
                     }
                     data.type = CommandParameterDataType::Enum;
                     data.enum_name = it->first.c_str();
                     data.enum_symbol = {symbol};
                 }
+                else if (parameter.type == "bool") {
+                    static auto symbol = registry.addEnumValues("Boolean", {});
+                    data.type = CommandParameterDataType::Enum;
+                    data.enum_name = "Boolean";
+                    data.enum_symbol = {symbol};
+                }
                 else {
                     auto it = gTypeSymbols.find(std::string(parameter.type));
                     if (it == gTypeSymbols.end()) {
                         server_.getLogger().error("Error occurred when registering usage '{}'. Unsupported type '{}'.",
                                                   usage, parameter.type);
                         return false;
                     }
```

### Comparing `endstone-0.3.0/src/endstone_core/command/command_sender.cpp` & `endstone-0.4.0/src/endstone_core/command/command_sender.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -12,26 +12,27 @@
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #include "endstone/detail/command/command_sender.h"
 
 #include <utility>
 
+#include <entt/entt.hpp>
+
 #include "endstone/detail/server.h"
-#include "endstone/detail/singleton.h"
 
 namespace endstone::detail {
 
 BaseCommandSender::BaseCommandSender() : perm_(this) {}
 
 BaseCommandSender::BaseCommandSender(PermissibleBase perm) : perm_(std::move(perm)) {}
 
 Server &BaseCommandSender::getServer() const
 {
-    return Singleton<EndstoneServer>::getInstance();
+    return entt::locator<EndstoneServer>::value();
 }
 
 bool BaseCommandSender::isPermissionSet(std::string name) const
 {
     return perm_.isPermissionSet(name);
 }
```

### Comparing `endstone-0.3.0/src/endstone_core/command/command_usage_parser.cpp` & `endstone-0.4.0/src/endstone_core/command/command_usage_parser.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/src/endstone_core/command/defaults/plugins_command.cpp` & `endstone-0.4.0/src/endstone_core/command/defaults/plugins_command.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 #include "endstone/detail/command/defaults/plugins_command.h"
 
 #include <sstream>
 #include <string>
 #include <vector>
 
-#include "endstone/detail/command/command_map.h"
+#include <entt/entt.hpp>
+
+#include "endstone/color_format.h"
 #include "endstone/detail/server.h"
-#include "endstone/detail/singleton.h"
-#include "endstone/util/color_format.h"
 
 namespace endstone::detail {
 
 PluginsCommand::PluginsCommand() : EndstoneCommand("plugins")
 {
     setDescription("Gets a list of plugins running on the server");
     setUsages("/plugins");
@@ -41,25 +41,25 @@
     sender.sendMessage("Plugins {}", getPluginList());
     return true;
 }
 
 std::string PluginsCommand::getPluginList() const
 {
     std::stringstream ss;
-    auto &server = Singleton<EndstoneServer>::getInstance();
+    auto &server = entt::locator<EndstoneServer>::value();
     auto plugins = server.getPluginManager().getPlugins();
 
     int i = 0;
     for (auto *plugin : plugins) {
         if (i > 0) {
-            ss << ColorFormat::WHITE;
+            ss << ColorFormat::White;
             ss << ", ";
         }
 
-        ss << (plugin->isEnabled() ? ColorFormat::GREEN : ColorFormat::RED);
+        ss << (plugin->isEnabled() ? ColorFormat::Green : ColorFormat::Red);
         ss << plugin->getDescription().getName();
         i++;
     }
 
     return "(" + std::to_string(plugins.size()) + "): " + ss.str();
 }
```

### Comparing `endstone-0.3.0/src/endstone_core/command/defaults/version_command.cpp` & `endstone-0.4.0/src/endstone_core/command/defaults/version_command.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #include "endstone/detail/command/defaults/version_command.h"
 
+#include <entt/entt.hpp>
+
+#include "endstone/color_format.h"
 #include "endstone/detail/command/command_map.h"
 #include "endstone/detail/server.h"
-#include "endstone/detail/singleton.h"
-#include "endstone/util/color_format.h"
 
 namespace endstone::detail {
 
 VersionCommand::VersionCommand() : EndstoneCommand("version")
 {
     setDescription("Gets the version of this server including any plugins in use.");
     setUsages("/version", "/version ()[plugin: PluginName]");
@@ -31,25 +32,24 @@
 
 bool VersionCommand::execute(CommandSender &sender, const std::vector<std::string> &args) const
 {
     if (!testPermission(sender)) {
         return true;
     }
 
+    auto &server = entt::locator<EndstoneServer>::value();
     if (args.empty()) {
-        auto &server = Singleton<EndstoneServer>::getInstance();
-        sender.sendMessage(ColorFormat::GOLD + "This server is running {} version: {} (Minecraft: {})",
+        sender.sendMessage(ColorFormat::Gold + "This server is running {} version: {} (Minecraft: {})",
                            server.getName(), server.getVersion(), server.getMinecraftVersion());
     }
     else {
         auto target_name = args[0];
         std::transform(target_name.begin(), target_name.end(), target_name.begin(),
                        [](unsigned char c) { return std::tolower(c); });
 
-        auto &server = Singleton<EndstoneServer>::getInstance();
         auto plugins = server.getPluginManager().getPlugins();
         for (auto *plugin : plugins) {
             auto name = plugin->getName();
             std::transform(name.begin(), name.end(), name.begin(), [](unsigned char c) { return std::tolower(c); });
 
             if (name == target_name) {
                 describeToSender(*plugin, sender);
@@ -64,53 +64,53 @@
 
     return true;
 }
 
 void VersionCommand::describeToSender(Plugin &plugin, CommandSender &sender) const
 {
     const auto &desc = plugin.getDescription();
-    sender.sendMessage(ColorFormat::GREEN + desc.getName() + ColorFormat::WHITE + " v" + desc.getVersion());
+    sender.sendMessage(ColorFormat::Green + desc.getName() + ColorFormat::White + " v" + desc.getVersion());
 
     if (!desc.getDescription().empty()) {
         sender.sendMessage(desc.getDescription());
     }
 
     if (!desc.getWebsite().empty()) {
-        sender.sendMessage("Website: " + ColorFormat::GREEN + desc.getWebsite());
+        sender.sendMessage("Website: " + ColorFormat::Green + desc.getWebsite());
     }
 
     if (!desc.getAuthors().empty()) {
         if (desc.getAuthors().size() == 1) {
             sender.sendMessage("Author: " + getNameList(desc.getAuthors()));
         }
         else {
             sender.sendMessage("Authors: " + getNameList(desc.getAuthors()));
         }
     }
 
-     if (!desc.getContributors().empty()) {
-         sender.sendMessage("Contributors: " + getNameList(desc.getContributors()));
-     }
+    if (!desc.getContributors().empty()) {
+        sender.sendMessage("Contributors: " + getNameList(desc.getContributors()));
+    }
 }
 
 std::string VersionCommand::getNameList(const std::vector<std::string> &names) const
 {
     std::string result;
     for (const auto &name : names) {
         if (!result.empty()) {
-            result += ColorFormat::WHITE;
+            result += ColorFormat::White;
             if (names.size() == 2) {
                 result += ", ";
             }
             else {
                 result += " and ";
             }
         }
 
-        result += ColorFormat::GREEN;
+        result += ColorFormat::Green;
         result += name;
     }
 
     return result;
 }
 
 };  // namespace endstone::detail
```

### Comparing `endstone-0.3.0/src/endstone_core/command/server_command_sender.cpp` & `endstone-0.4.0/src/endstone_core/command/server_command_sender.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/src/endstone_core/logger_factory.cpp` & `endstone-0.4.0/src/endstone_core/logger_factory.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/src/endstone_core/permissions/default_permissions.cpp` & `endstone-0.4.0/src/endstone_core/permissions/default_permissions.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #include "endstone/detail/permissions/default_permissions.h"
 
+#include <entt/entt.hpp>
+
 namespace endstone::detail {
 
 Permission *DefaultPermissions::registerPermission(std::unique_ptr<Permission> perm, Permission *parent)
 {
-    auto &server = Singleton<EndstoneServer>::getInstance();
+    auto &server = entt::locator<EndstoneServer>::value();
     auto *result = server.getPluginManager().addPermission(std::move(perm));
     if (parent != nullptr && result != nullptr) {
         parent->getChildren()[result->getName()] = true;
     }
     return result;
 }
 
@@ -42,14 +44,16 @@
     endstone->recalculatePermissibles();
 }
 
 void DefaultPermissions::registerCommandPermissions(Permission *parent)
 {
     auto *command =
         registerPermission("endstone.command", parent, "Gives the user the ability to use all Endstone command");
+    registerPermission("endstone.command.debug", command, "Allows the user to toggle the debug mode of this server",
+                       PermissionDefault::Operator);
     registerPermission("endstone.command.plugins", command,
                        "Allows the user to view the list of plugins running on this server", PermissionDefault::True);
     registerPermission("endstone.command.version", command, "Allows the user to view the version of the server",
                        PermissionDefault::True);
     command->recalculatePermissibles();
 }
```

### Comparing `endstone-0.3.0/src/endstone_core/permissions/permissible_base.cpp` & `endstone-0.4.0/src/endstone_core/permissions/permissible_base.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #include "endstone/detail/permissions/permissible_base.h"
 
 #include <memory>
 
+#include <entt/entt.hpp>
+
 #include "endstone/detail/server.h"
-#include "endstone/detail/singleton.h"
 #include "endstone/permissions/permission.h"
 #include "endstone/permissions/permission_attachment_info.h"
 
 namespace endstone::detail {
 
 bool PermissibleBase::isOp() const
 {
@@ -52,20 +53,20 @@
 bool PermissibleBase::hasPermission(std::string name) const
 {
     std::transform(name.begin(), name.end(), name.begin(), [](unsigned char c) { return std::tolower(c); });
     if (isPermissionSet(name)) {
         return permissions_.find(name)->second->getValue();
     }
 
-    auto &server = Singleton<EndstoneServer>::getInstance();
+    auto &server = entt::locator<EndstoneServer>::value();
     auto *perm = server.getPluginManager().getPermission(name);
     if (perm != nullptr) {
         return hasPermission(perm->getDefault(), isOp());
     }
-    return hasPermission(Permission::DEFAULT_PERMISSION, isOp());
+    return hasPermission(Permission::DefaultPermission, isOp());
 }
 
 bool PermissibleBase::hasPermission(const Permission &perm) const
 {
     auto name = perm.getName();
     std::transform(name.begin(), name.end(), name.begin(), [](unsigned char c) { return std::tolower(c); });
     if (isPermissionSet(name)) {
@@ -118,22 +119,22 @@
         }
 
         attachments_.erase(it);
         recalculatePermissions();
         return true;
     }
 
-    auto &server = Singleton<EndstoneServer>::getInstance();
+    auto &server = entt::locator<EndstoneServer>::value();
     server.getLogger().error("Given attachment is not part of Permissible object.");
     return false;
 }
 
 void PermissibleBase::recalculatePermissions()
 {
-    auto &server = Singleton<EndstoneServer>::getInstance();
+    auto &server = entt::locator<EndstoneServer>::value();
     auto &plugin_manager = server.getPluginManager();
 
     // Clear permissions
     for (const auto &[name, perm] : permissions_) {
         plugin_manager.unsubscribeFromPermission(name, parent_);
     }
     plugin_manager.unsubscribeFromDefaultPerms(false, parent_);
@@ -153,18 +154,19 @@
     }
 
     for (const auto &attachment : attachments_) {
         calculateChildPermissions(attachment->getPermissions(), false, attachment.get());
     }
 }
 
+// NOLINTNEXTLINE(*-no-recursion)
 void PermissibleBase::calculateChildPermissions(const std::unordered_map<std::string, bool> &children, bool invert,
                                                 PermissionAttachment *attachment)
 {
-    auto &server = Singleton<EndstoneServer>::getInstance();
+    auto &server = entt::locator<EndstoneServer>::value();
     auto &plugin_manager = server.getPluginManager();
 
     for (const auto &entry : children) {
         auto name = entry.first;
         std::transform(name.begin(), name.end(), name.begin(), [](unsigned char c) { return std::tolower(c); });
         bool value = entry.second ^ invert;
         permissions_.emplace(name, std::make_unique<PermissionAttachmentInfo>(parent_, name, attachment, value));
```

### Comparing `endstone-0.3.0/src/endstone_core/plugin/cpp_plugin_loader.cpp` & `endstone-0.4.0/src/endstone_core/plugin/cpp_plugin_loader.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -126,19 +126,15 @@
     }
     initPlugin(*plugin, LoggerFactory::getLogger(logger_name));
     return std::unique_ptr<Plugin>(plugin);
 }
 
 std::vector<std::string> CppPluginLoader::getPluginFileFilters() const
 {
-#ifdef _WIN32
-    return {"\\.dll$"};
-#elif __linux__
-    return {"\\.so$"};
-#endif
+    return {_WIN32_LINUX_("\\.dll$", "\\.so$")};
 }
 
 }  // namespace endstone::detail
 
 #undef LOAD_LIBRARY
 #undef GET_FUNCTION
 #undef GET_ERROR
```

### Comparing `endstone-0.3.0/src/endstone_core/plugin/plugin_manager.cpp` & `endstone-0.4.0/src/endstone_core/plugin/plugin_manager.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 #include <algorithm>
 #include <memory>
 #include <regex>
 #include <string>
 #include <utility>
 #include <vector>
 
+#include "endstone/event/event.h"
+#include "endstone/event/event_handler.h"
+#include "endstone/event/handler_list.h"
+#include "endstone/plugin/plugin.h"
 #include "endstone/plugin/plugin_loader.h"
 #include "endstone/server.h"
 
 namespace endstone::detail {
 
 EndstonePluginManager::EndstonePluginManager(Server &server)
     : server_(server), default_perms_({{true, {}}, {false, {}}})
@@ -73,15 +77,15 @@
     return it != plugins_.end() && plugin->isEnabled();
 }
 
 std::vector<Plugin *> EndstonePluginManager::loadPlugins(const std::string &directory)
 {
     std::vector<Plugin *> loaded_plugins;
 
-    // TODO: handling logic for depend, soft_depend, load_before and provides
+    // TODO(plugin): handling logic for depend, soft_depend, load_before and provides
     for (const auto &loader : plugin_loaders_) {
         auto plugins = loader->loadPlugins(directory);
         for (const auto &plugin : plugins) {
             if (!plugin) {
                 continue;
             }
 
@@ -142,14 +146,59 @@
     lookup_names_.clear();
     plugin_loaders_.clear();
     permissions_.clear();
     default_perms_[true].clear();
     default_perms_[false].clear();
 }
 
+void EndstonePluginManager::callEvent(Event &event)
+{
+    if (event.isAsynchronous() && server_.isPrimaryThread()) {
+        server_.getLogger().error("{} cannot be triggered asynchronously from server thread.", event.getEventName());
+        return;
+    }
+
+    if (!event.isAsynchronous() && !server_.isPrimaryThread()) {
+        server_.getLogger().error("{} must be triggered synchronously from server thread.", event.getEventName());
+        return;
+    }
+
+    auto &handler_list = event_handlers_.emplace(event.getEventName(), event.getEventName()).first->second;
+    for (const auto &handler : handler_list.getHandlers()) {
+        auto &plugin = handler->getPlugin();
+        if (!plugin.isEnabled()) {
+            continue;
+        }
+
+        try {
+            handler->callEvent(event);
+        }
+        catch (std::exception &e) {
+            server_.getLogger().critical("Could not pass event {} to plugin {}. {}", event.getEventName(),
+                                         plugin.getDescription().getFullName(), e.what());
+        }
+    }
+}
+
+void EndstonePluginManager::registerEvent(std::string event, std::function<void(Event &)> executor,
+                                          EventPriority priority, Plugin &plugin, bool ignore_cancelled)
+{
+    if (!plugin.isEnabled()) {
+        server_.getLogger().error("Plugin {} attempted to register listener for event {} while not enabled.",
+                                  plugin.getDescription().getFullName(), event);
+        return;
+    }
+
+    auto &handler_list = event_handlers_.emplace(event, event).first->second;
+    if (handler_list.registerHandler(
+            std::make_unique<EventHandler>(event, executor, priority, plugin, ignore_cancelled)) == nullptr) {
+        server_.getLogger().error("Plugin {} failed to register listener for event {}.", event);
+    }
+}
+
 Permission *EndstonePluginManager::getPermission(std::string name) const
 {
     std::transform(name.begin(), name.end(), name.begin(), [](unsigned char c) { return std::tolower(c); });
     auto it = permissions_.find(name);
     if (it == permissions_.end()) {
         return nullptr;
     }
```

### Comparing `endstone-0.3.0/src/endstone_core/server.cpp` & `endstone-0.4.0/src/endstone_core/server.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -15,16 +15,19 @@
 #include "endstone/detail/server.h"
 
 #include <filesystem>
 #include <memory>
 namespace fs = std::filesystem;
 
 #include "bedrock/common.h"
+#include "bedrock/threading.h"
+#include "bedrock/world/actor/player/player.h"
 #include "endstone/command/plugin_command.h"
 #include "endstone/detail/command/command_map.h"
+#include "endstone/detail/level.h"
 #include "endstone/detail/logger_factory.h"
 #include "endstone/detail/permissions/default_permissions.h"
 #include "endstone/detail/plugin/cpp_plugin_loader.h"
 #include "endstone/plugin/plugin.h"
 
 #if !defined(ENDSTONE_VERSION)
 #error ENDSTONE_VERSION is not defined
@@ -115,14 +118,57 @@
 }
 
 CommandSender &EndstoneServer::getCommandSender() const
 {
     return command_sender_;
 }
 
+std::vector<Level *> EndstoneServer::getLevels() const
+{
+    std::vector<Level *> levels;
+    levels.reserve(levels_.size());
+    for (const auto &it : levels_) {
+        levels.push_back(it.second.get());
+    }
+    return levels;
+}
+
+Level *EndstoneServer::getLevel(std::string name) const
+{
+    std::transform(name.begin(), name.end(), name.begin(), [](unsigned char c) { return std::tolower(c); });
+    auto it = levels_.find(name);
+    if (it == levels_.end()) {
+        return nullptr;
+    }
+    return it->second.get();
+}
+
+void EndstoneServer::addLevel(std::unique_ptr<Level> level)
+{
+    auto name = level->getName();
+    if (getLevel(name) != nullptr) {
+        getLogger().error("Level {} is a duplicate of another level and has been prevented from loading.", name);
+        return;
+    }
+    std::transform(name.begin(), name.end(), name.begin(), [](unsigned char c) { return std::tolower(c); });
+    levels_[name] = std::move(level);
+}
+
+Player *EndstoneServer::getPlayer(endstone::UUID id) const
+{
+    for (const auto *level : getLevels()) {
+        auto uuid = mce::UUID{id.bits.most_significant, id.bits.least_significant};
+        auto *player = static_cast<const EndstoneLevel *>(level)->getBedrockLevel().getPlayer(uuid);
+        if (player) {
+            return &player->getEndstonePlayer();
+        }
+    }
+    return nullptr;
+}
+
 std::string EndstoneServer::getName() const
 {
     return "Endstone";
 }
 
 std::string EndstoneServer::getVersion() const
 {
@@ -130,8 +176,13 @@
 }
 
 std::string EndstoneServer::getMinecraftVersion() const
 {
     return Common::getGameVersionString();
 }
 
+bool EndstoneServer::isPrimaryThread() const
+{
+    return Bedrock::Threading::getServerThread().isOnThread();
+}
+
 }  // namespace endstone::detail
```

### Comparing `endstone-0.3.0/src/endstone_core/spdlog/level_formatter.cpp` & `endstone-0.4.0/src/endstone_core/spdlog/level_formatter.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/src/endstone_core/spdlog/log_sink.cpp` & `endstone-0.4.0/src/endstone_core/spdlog/log_sink.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     msg.color_range_end = 0;
     spdlog::memory_buf_t formatted;
     formatter_->format(msg, formatted);
     if (should_do_colors_ && msg.color_range_end > msg.color_range_start) {
         // before color range
         printRange(formatted, 0, msg.color_range_start);
         // in color range
-        printColorCode(colors_.at(static_cast<size_t>(msg.level)));
+        printColorCode(colors_.at(static_cast<std::size_t>(msg.level)));
         printRange(formatted, msg.color_range_start, msg.color_range_end);
         printColorCode(reset);
         // after color range
         printRange(formatted, msg.color_range_end, formatted.size());
     }
     else  // no color
     {
@@ -89,13 +89,13 @@
 }
 
 void LogSink::printColorCode(const spdlog::string_view_t &color_code)
 {
     fwrite(color_code.data(), sizeof(char), color_code.size(), target_file_);
 }
 
-void LogSink::printRange(const spdlog::memory_buf_t &formatted, size_t start, size_t end)
+void LogSink::printRange(const spdlog::memory_buf_t &formatted, std::size_t start, std::size_t end)
 {
     fwrite(formatted.data() + start, sizeof(char), end - start, target_file_);
 }
 
 }  // namespace endstone::detail
```

### Comparing `endstone-0.3.0/src/endstone_core/spdlog/spdlog_adapter.cpp` & `endstone-0.4.0/src/endstone_core/spdlog/spdlog_adapter.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/src/endstone_core/spdlog/text_formatter.cpp` & `endstone-0.4.0/src/endstone_core/spdlog/text_formatter.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 namespace endstone::detail {
 
 void TextFormatter::format(const spdlog::details::log_msg &msg, const tm &, spdlog::memory_buf_t &dest)
 {
 
     const auto &input = msg.payload;
-    for (size_t i = 0; i < input.size(); i++) {
+    for (std::size_t i = 0; i < input.size(); i++) {
         // Check for the § character in UTF-8 (0xC2A7) and ensure there's a following character
         if (i + 2 < input.size() && static_cast<unsigned char>(input[i]) == 0xC2 &&
             static_cast<unsigned char>(input[i + 1]) == 0xA7) {
             i += 2;                  // Skip §
             if (i < input.size()) {  // if there's a color code character to after §
                 if (should_do_colors_) {
                     auto format_code = static_cast<unsigned char>(input[i]);
```

### Comparing `endstone-0.3.0/src/endstone_python/command.cpp` & `endstone-0.4.0/src/endstone_python/command.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/src/endstone_python/permissions.cpp` & `endstone-0.4.0/src/endstone_python/permissions.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -29,28 +29,28 @@
 
 namespace {
 Permission createPermission(std::string name, const std::optional<std::string> &description,
                             std::optional<PermissionDefault> default_value,
                             const std::optional<std::unordered_map<std::string, bool>> &children,
                             const py::args & /*args*/, const py::kwargs & /*kwargs*/)
 {
-    return Permission(std::move(name), description.value_or(""), default_value.value_or(Permission::DEFAULT_PERMISSION),
+    return Permission(std::move(name), description.value_or(""), default_value.value_or(Permission::DefaultPermission),
                       children.value_or(std::unordered_map<std::string, bool>{}));
 }
 }  // namespace
 
 void init_permissions(py::module_ &m, py::class_<Permissible> &permissible, py::class_<Permission> &permission,
                       py::enum_<PermissionDefault> &permission_default)
 {
     permission_default  //
         .value("TRUE", PermissionDefault::True)
         .value("FALSE", PermissionDefault::False)
         .value("OP", PermissionDefault::Operator)
         .value("OPERATOR", PermissionDefault::Operator)
-        .value("NOT_OP", PermissionDefault::Operator)
+        .value("NOT_OP", PermissionDefault::NotOperator)
         .value("NOT_OPERATOR", PermissionDefault::NotOperator);
 
     permission  //
         .def(py::init(&createPermission), py::arg("name"), py::arg("description") = py::none(),
              py::arg("default") = py::none(), py::arg("children") = py::none())
         .def_property_readonly("name", &Permission::getName, "Gets the unique fully qualified name of this Permission.")
         .def_property_readonly("children", &Permission::getChildren, py::return_value_policy::reference_internal,
```

### Comparing `endstone-0.3.0/src/endstone_python/plugin.cpp` & `endstone-0.4.0/src/endstone_python/plugin.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -10,18 +10,22 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #include "endstone/plugin/plugin.h"
 
+#include <utility>
+
+#include <pybind11/functional.h>
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 
 #include "endstone/command/plugin_command.h"
+#include "endstone/event/server/server_load_event.h"
 #include "endstone/logger.h"
 #include "endstone/plugin/plugin_loader.h"
 #include "endstone/plugin/plugin_manager.h"
 #include "endstone/server.h"
 
 namespace py = pybind11;
 
@@ -34,15 +38,15 @@
     [[nodiscard]] const PluginDescription &getDescription() const override
     {
         try {
             PYBIND11_OVERRIDE_PURE_NAME(const PluginDescription &, Plugin, "_get_description", getDescription);
         }
         catch (std::exception &e) {
             getLogger().error(e.what());
-            std::terminate();
+            throw e;
         }
     }
 
     void onLoad() override
     {
         try {
             PYBIND11_OVERRIDE_NAME(void, Plugin, "on_load", onLoad);
@@ -216,15 +220,53 @@
              py::arg("plugin"), "Checks if the given plugin is enabled or not")
         .def("load_plugins", &PluginManager::loadPlugins, py::arg("directory"),
              "Loads the plugin contained within the specified directory")
         .def("enable_plugin", &PluginManager::enablePlugin, py::arg("plugin"), "Enables the specified plugin")
         .def("enable_plugins", &PluginManager::enablePlugins, "Enable all the loaded plugins")
         .def("disable_plugin", &PluginManager::disablePlugin, py::arg("plugin"), "Disables the specified plugin")
         .def("disable_plugins", &PluginManager::disablePlugins, "Disables all the loaded plugins")
-        .def("clear_plugins", &PluginManager::clearPlugins, "Disables and removes all plugins");
+        .def("clear_plugins", &PluginManager::clearPlugins, "Disables and removes all plugins")
+        .def("call_event", &PluginManager::callEvent, py::arg("event"),
+             "Calls an event which will be passed to plugins.")
+        .def(
+            "register_event",
+            [](PluginManager &self, std::string event, const std::function<void(Event *)> &executor,
+               EventPriority priority, Plugin &plugin, bool ignore_cancelled) {
+                self.registerEvent(
+                    std::move(event), [executor](Event &e) { executor(&e); }, priority, plugin, ignore_cancelled);
+            },
+            py::arg("name"), py::arg("executor"), py::arg("priority"), py::arg("plugin"), py::arg("ignore_cancelled"),
+            "Registers the given event")
+        .def("get_permission", &PluginManager::getPermission, py::arg("name"), py::return_value_policy::reference,
+             "Gets a Permission from its fully qualified name.")
+        .def("remove_permission", py::overload_cast<Permission &>(&PluginManager::removePermission), py::arg("perm"),
+             "Removes a Permission registration from this plugin manager by permission object.")
+        .def("remove_permission", py::overload_cast<std::string>(&PluginManager::removePermission), py::arg("name"),
+             "Removes a Permission registration from this plugin manager by name.")
+        .def("get_default_permissions", &PluginManager::getDefaultPermissions, py::arg("op"),
+             py::return_value_policy::reference_internal, "Gets the default permissions for the given op status.")
+        .def("recalculate_permission_defaults", &PluginManager::recalculatePermissionDefaults, py::arg("perm"),
+             "Recalculates the defaults for the given Permission.")
+        .def("subscribe_to_permission", &PluginManager::subscribeToPermission, py::arg("permission"),
+             py::arg("permissible"), "Subscribes the given Permissible for information about the requested Permission.")
+        .def("unsubscribe_from_permission", &PluginManager::unsubscribeFromPermission, py::arg("permission"),
+             py::arg("permissible"),
+             "Unsubscribes the given Permissible for information about the requested Permission.")
+        .def("get_permission_subscriptions", &PluginManager::getPermissionSubscriptions, py::arg("permission"),
+             py::return_value_policy::reference_internal,
+             "Gets a set containing all subscribed Permissibles to the given permission.")
+        .def("subscribe_to_default_perms", &PluginManager::subscribeToDefaultPerms, py::arg("op"),
+             py::arg("permissible"), "Subscribes to the given Default permissions by operator status.")
+        .def("unsubscribe_from_default_perms", &PluginManager::unsubscribeFromDefaultPerms, py::arg("op"),
+             py::arg("permissible"), "Unsubscribes from the given Default permissions by operator status.")
+        .def("get_default_perm_subscriptions", &PluginManager::getDefaultPermSubscriptions, py::arg("op"),
+             py::return_value_policy::reference_internal,
+             "Gets a set containing all subscribed Permissibles to the given default list, by op status.")
+        .def_property_readonly("permissions", &PluginManager::getPermissions,
+                               "Gets a set of all registered permissions.");
 
     plugin_command
         .def_property("executor", &PluginCommand::getExecutor, &PluginCommand::setExecutor,
                       py::return_value_policy::reference, "The CommandExecutor to run when parsing this command")
         .def_property_readonly("plugin", &PluginCommand::getPlugin, "The owner of this PluginCommand");
 }
```

### Comparing `endstone-0.3.0/src/endstone_runtime/bedrock/bedrock_log.cpp` & `endstone-0.4.0/src/endstone_runtime/bedrock/bedrock_log.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -43,26 +43,25 @@
         log_level = iter->second;
     }
 
     std::va_list args_copy;
     va_copy(args_copy, args);
     std::vector<char> buf(1 + std::vsnprintf(nullptr, 0, format, args));
     va_end(args);
-    size_t len = std::vsnprintf(buf.data(), buf.size(), format, args_copy);
+    std::size_t len = std::vsnprintf(buf.data(), buf.size(), format, args_copy);
     va_end(args_copy);
 
     std::string message(buf.data(), len);
     message.erase(message.find_last_not_of(" \t\n\r\f\v") + 1);
 
-    std::string_view sv(message);
-    size_t start = 0;
-    size_t end;
+    std::size_t start = 0;
+    std::size_t end;
 
-    while ((end = sv.find('\n', start)) != std::string::npos) {
-        logger.log(log_level, sv.substr(start, end - start));
+    while ((end = message.find('\n', start)) != std::string::npos) {
+        logger.log(log_level, message.substr(start, end - start));
         start = end + 1;
     }
 
-    if (start < sv.length()) {
-        logger.log(log_level, sv.substr(start));
+    if (start < message.length()) {
+        logger.log(log_level, message.substr(start));
     }
 }
```

### Comparing `endstone-0.3.0/src/endstone_runtime/bedrock/command/command.cpp` & `endstone-0.4.0/src/endstone_runtime/bedrock/command/command.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/src/endstone_runtime/bedrock/command/command_output.cpp` & `endstone-0.4.0/src/endstone_runtime/bedrock/command/command_output.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/src/endstone_runtime/bedrock/common.cpp` & `endstone-0.4.0/src/endstone_runtime/bedrock/common.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/src/endstone_runtime/bedrock/i18n.cpp` & `endstone-0.4.0/src/endstone_runtime/bedrock/i18n.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/src/endstone_runtime/bedrock/minecraft.cpp` & `endstone-0.4.0/include/bedrock/network/protocol/minecraft_packets.h`

 * *Files 22% similar despite different names*

```diff
@@ -8,17 +8,22 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include "bedrock/minecraft.h"
+#pragma once
 
-MinecraftCommands &Minecraft::getCommands()
-{
-#ifdef __linux__
-    return **reinterpret_cast<MinecraftCommands **>(reinterpret_cast<size_t *>(this) + 22);
-#elif _WIN32
-    return **reinterpret_cast<MinecraftCommands **>(reinterpret_cast<size_t *>(this) + 23);
-#endif
-}
+#include <memory>
+
+#include "bedrock/bedrock.h"
+#include "bedrock/network/protocol/packet.h"
+
+enum class MinecraftPacketIds {
+    Text = 9,
+};
+
+class MinecraftPackets {
+public:
+    BEDROCK_API static std::shared_ptr<Packet> createPacket(MinecraftPacketIds id);
+};
```

### Comparing `endstone-0.3.0/src/endstone_runtime/bedrock/server/level/server_player.cpp` & `endstone-0.4.0/include/bedrock/server/level/server_player.h`

 * *Files 16% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include "bedrock/server/level/server_player.h"
+#pragma once
 
-#include "endstone/detail/hook.h"
+#include "bedrock/bedrock.h"
+#include "bedrock/world/actor/player/player.h"
 
-void ServerPlayer::doInitialSpawn()
-{
-    ENDSTONE_HOOK_CALL_ORIGINAL(&ServerPlayer::doInitialSpawn, this);
-    sendCommands();
-}
+class ServerPlayer : public Player {
+public:
+    ~ServerPlayer() override = 0;
+    BEDROCK_API void doInitialSpawn();
+    BEDROCK_API void disconnect();
+};
```

### Comparing `endstone-0.3.0/src/endstone_runtime/linux/hook.cpp` & `endstone-0.4.0/src/endstone_runtime/hook.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -8,118 +8,77 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#ifdef __linux__
-
 #include "endstone/detail/hook.h"
 
+#include <string>
+#include <system_error>
 #include <unordered_map>
 
-#include <LIEF/LIEF.hpp>
-#include <fmt/format.h>
 #include <funchook/funchook.h>
 #include <spdlog/spdlog.h>
 
-#include "endstone/detail/os.h"
-
 namespace endstone::detail::hook {
 
 namespace {
-std::unordered_map<void *, void *> gOriginals;
+std::unordered_map<void *, void *> gOriginalsByDetour;
+std::unordered_map<std::string, void *> gOriginalsByName;
 }  // namespace
 
 void *get_original(void *detour)
 {
-    auto it = gOriginals.find(detour);
-    if (it == gOriginals.end()) {
-        return nullptr;
+    auto it = gOriginalsByDetour.find(detour);
+    if (it == gOriginalsByDetour.end()) {
+        throw std::runtime_error(fmt::format("No original function can be found for address {}", detour));
     }
     return it->second;
 }
 
-void install()
+void *get_original(const std::string &name)
 {
-    // Find detours
-    auto *module_base = os::get_module_base();
-    auto module_pathname = os::get_module_pathname();
-
-    std::unordered_map<std::string, void *> detours;
-    {
-        spdlog::debug("{}", module_pathname);
-        auto elf = LIEF::ELF::Parser::parse(module_pathname);
-        for (const auto &symbol : elf->static_symbols()) {
-            if (!symbol.is_exported()) {
-                continue;
-            }
-
-            if (symbol.binding() != LIEF::ELF::SYMBOL_BINDINGS::STB_GLOBAL) {
-                continue;
-            }
-
-            auto name = symbol.name();
-            auto offset = symbol.value();
-            spdlog::debug("{} -> 0x{:x}", name, offset);
-            auto *detour = static_cast<char *>(module_base) + offset;
-            detours.emplace(symbol.name(), detour);
-        }
+    auto it = gOriginalsByName.find(name);
+    if (it == gOriginalsByName.end()) {
+        throw std::runtime_error(fmt::format("No original function can be found for name {}", name));
     }
+    return it->second;
+}
 
-    // Find targets
-    auto *executable_base = os::get_executable_base();
-    std::unordered_map<std::string, void *> targets;
-    const auto executable_pathname = os::get_executable_pathname() + "_symbols.debug";
-    {
-        auto elf = LIEF::ELF::Parser::parse(executable_pathname);
-        for (const auto &symbol : elf->symbols()) {
-            if (symbol.binding() != LIEF::ELF::SYMBOL_BINDINGS::STB_LOCAL) {
-                continue;
-            }
-
-            auto name = symbol.name();
-            auto offset = symbol.value();
-            auto it = detours.find(name);
-            if (it != detours.end()) {
-                spdlog::debug("{} -> 0x{:x}", name, offset);
-                auto *target = static_cast<char *>(executable_base) + offset;
-                targets.emplace(name, target);
-            }
-        }
-    }
+void install()
+{
+    auto detours = get_detours();
+    auto targets = get_targets();
 
-    // Install hooks
     for (const auto &[name, detour] : detours) {
         auto it = targets.find(name);
         if (it != targets.end()) {
             void *target = it->second;
             void *original = target;
 
-            spdlog::debug("{}: T = 0x{:p}", name, target);
-            spdlog::debug("{}: D = 0x{:p}", name, detour);
-
             funchook_t *hook = funchook_create();
             int status;
             status = funchook_prepare(hook, &original, detour);
             if (status != 0) {
                 throw std::system_error(status, hook_error_category());
             }
 
             status = funchook_install(hook, 0);
             if (status != 0) {
                 throw std::system_error(status, hook_error_category());
             }
 
-            spdlog::debug("{}: O = 0x{:p}", name, original);
-            gOriginals.emplace(detour, original);
+            spdlog::debug("{}: {} -> {} -> {}", name, target, detour, original);
+            gOriginalsByDetour.emplace(detour, original);
+            gOriginalsByName.emplace(name, original);
         }
         else {
-            throw std::runtime_error(fmt::format("Unable to find target function {} in the executable", name));
+            throw std::runtime_error(fmt::format("Unable to find target function {} to hook.", name));
         }
     }
 }
 
 const std::error_category &hook_error_category()
 {
     static const class HookErrorCategory : public std::error_category {
@@ -158,13 +117,11 @@
                 return "FUNCHOOK_ERROR_NOT_INSTALLED";
             case FUNCHOOK_ERROR_NO_AVAILABLE_REGISTERS:
                 return "FUNCHOOK_ERROR_NO_AVAILABLE_REGISTERS";
             default:
                 return "Unknown error.";
             }
         }
-    } CATEGORY;
-    return CATEGORY;
+    } category;
+    return category;
 }
 }  // namespace endstone::detail::hook
-
-#endif
```

### Comparing `endstone-0.3.0/src/endstone_runtime/linux/os.cpp` & `endstone-0.4.0/src/endstone_runtime/linux/os.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 namespace {
 struct ModuleInfo {
     void *base;
     std::string pathname;
 };
 
 struct MmapRegion {
-    size_t begin;
-    size_t end;
+    std::size_t begin;
+    std::size_t end;
     char perms[4 + 1];  // rwxp(4) + \0(1)
-    size_t offset;
+    std::size_t offset;
     char device[255 + 1];
-    size_t inode;
+    std::size_t inode;
     char pathname[PATH_MAX + 1];
 };
 
 ModuleInfo get_module_info(const char *module_name)
 {
     std::ifstream file("/proc/self/maps");
     if (!file.is_open()) {
@@ -51,15 +51,15 @@
         int r = sscanf(line.c_str(), "%lx-%lx %4s %lx %10s %ld %s", &region.begin, &region.end, region.perms,
                        &region.offset, region.device, &region.inode, region.pathname);
         if (r != 7) {
             continue;
         }
 
         auto pathname = std::string(region.pathname);
-        size_t pos = pathname.find_last_of('/');
+        std::size_t pos = pathname.find_last_of('/');
         if (pos != std::string::npos) {
             pathname = pathname.substr(pos + 1);
         }
 
         if (module_name == nullptr || pathname == module_name) {
             return {reinterpret_cast<void *>(region.begin), region.pathname};
         }
```

### Comparing `endstone-0.3.0/src/endstone_runtime/main.cpp` & `endstone-0.4.0/src/endstone_runtime/main.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/src/endstone_runtime/plugin/python_plugin_loader.cpp` & `endstone-0.4.0/src/endstone_runtime/plugin/python_plugin_loader.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/src/endstone_runtime/windows/os.cpp` & `endstone-0.4.0/src/endstone_runtime/windows/os.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/test_package/src/test_plugin.cpp` & `endstone-0.4.0/tests/plugin/test_plugin.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -30,25 +30,25 @@
     {
         getLogger().info("onDisable is called");
     }
 };
 
 ENDSTONE_PLUGIN("TestPlugin", "1.0.0", TestPlugin)
 {
-    plugin.description = "This is a test plugin";
-    plugin.website = "https://github.com/EndstoneMC/endstone";
-    plugin.authors = {"Endstone Developers <hello@endstone.dev>"};
-    plugin.load = endstone::PluginLoadOrder::PostWorld;
-    plugin.prefix = "TestPlugin";
+    description = "This is a test plugin";
+    website = "https://github.com/EndstoneMC/endstone";
+    authors = {"Endstone Developers <hello@endstone.dev>"};
+    load = endstone::PluginLoadOrder::PostWorld;
+    prefix = "TestPlugin";
 
-    plugin.permission("test_plugin.command.test").description("Allow users to use the test command");
-
-    plugin.permission("test_plugin.command")
+    permission("test_plugin.command.test")  //
+        .description("Allow users to use the test command");
+    permission("test_plugin.command")  //
         .description("Allow users to use all commands provided by this example plugin")
         .children("test_plugin.command.test", true);
 
-    plugin.command("test")
+    command("test")
         .description("Test command")
         .usages("/test")
         .aliases("tryme")
         .permissions("test_plugin.command.test");
 }
```

### Comparing `endstone-0.3.0/tests/test_command_lexer.cpp` & `endstone-0.4.0/tests/command/test_command_lexer.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/tests/test_command_usage_parser.cpp` & `endstone-0.4.0/tests/command/test_command_usage_parser.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/tests/test_logger.cpp` & `endstone-0.4.0/tests/test_logger_factory.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/third_party/.gitignore` & `endstone-0.4.0/third_party/.gitignore`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/third_party/funchook/conanfile.py` & `endstone-0.4.0/third_party/funchook/conanfile.py`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/third_party/funchook/patches/1.1.3-0001-cmake-use-cci-capstone.patch` & `endstone-0.4.0/third_party/funchook/patches/1.1.3-0001-cmake-use-cci-capstone.patch`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/third_party/funchook/test_package/CMakeLists.txt` & `endstone-0.4.0/third_party/funchook/test_package/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/third_party/funchook/test_package/conanfile.py` & `endstone-0.4.0/third_party/funchook/test_package/conanfile.py`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/third_party/funchook/test_package/libfunchook_test_aarch64_gas.S` & `endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_aarch64_gas.S`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/third_party/funchook/test_package/libfunchook_test_x86_64_gas.S` & `endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_x86_64_gas.S`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/third_party/funchook/test_package/libfunchook_test_x86_gas.S` & `endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_x86_gas.S`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/third_party/funchook/test_package/suffix.list` & `endstone-0.4.0/third_party/funchook/test_package/suffix.list`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/third_party/funchook/test_package/test_main.c` & `endstone-0.4.0/third_party/funchook/test_package/test_main.c`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/third_party/funchook/test_package/x86_test.S` & `endstone-0.4.0/third_party/funchook/test_package/x86_test.S`

 * *Files identical despite different names*

### Comparing `endstone-0.3.0/PKG-INFO` & `endstone-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: endstone
-Version: 0.3.0
+Version: 0.4.0
 Summary: Endstone offers a plugin API for Bedrock Dedicated Servers, supporting both Python and C++.
-Keywords: plugin python minecraft bedrock
+Keywords: plugin,python,minecraft,bedrock
 Author-Email: Vincent Wu <magicdroidx@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -242,15 +242,15 @@
 </p>
 
 [![Windows](https://github.com/EndstoneMC/endstone/actions/workflows/windows.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/windows.yml)
 [![Linux](https://github.com/EndstoneMC/endstone/actions/workflows/linux.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/linux.yml)
 [![Wheel](https://github.com/EndstoneMC/endstone/actions/workflows/wheel.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/wheel.yml)
 [![Docker](https://github.com/EndstoneMC/endstone/actions/workflows/docker.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/docker.yml)
 [![Documentation](https://img.shields.io/readthedocs/endstone)](https://endstone.readthedocs.io/)
-[![Minecraft - Version](https://img.shields.io/badge/minecraft-v1.20.72%20(Bedrock)-green)](https://feedback.minecraft.net/hc/en-us/sections/360001186971-Release-Changelogs)
+[![Minecraft - Version](https://img.shields.io/badge/minecraft-v1.20.73%20(Bedrock)-green)](https://feedback.minecraft.net/hc/en-us/sections/360001186971-Release-Changelogs)
 [![PyPI - Version](https://img.shields.io/pypi/v/endstone)](https://pypi.org/project/endstone)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/endstone)](https://pypi.org/project/endstone)
 [![Python](https://img.shields.io/badge/Python-3-blue?logo=python&logoColor=white)](https://www.python.org/)
 [![GitHub License](https://img.shields.io/github/license/endstonemc/endstone)](LICENSE)
 [![Codacy Badge](https://img.shields.io/codacy/grade/8877402fc70b40f5a8c4b325d890e3f7?logo=codacy)](https://app.codacy.com/gh/EndstoneMC/endstone/dashboard)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -380,15 +380,15 @@
 - [Python Example Plugin](https://github.com/EndstoneMC/python-plugin-template)
 
 | Milestone                                | Duration   | Core | C++ API | Python API | Since  |
 |------------------------------------------|------------|------|---------|------------|--------|
 | **🔌 Plugin Loader**                     | 1-2 months | ✅    | ✅       | ✅          | v0.1.0 |
 | **⌨️ Command System**                    | 2-3 months | ✅    | ✅       | ✅          | v0.2.0 |
 | **🔐 Permission System**                 | 2-3 months | ✅    | ✅       | ✅          | v0.3.0 |
-| **🎈 Event System**                      | 2-3 months | 🚧   | ⏳       | ⏳          |        |
+| **🎈 Event System**                      | 2-3 months | 🚧   | ✅       | ✅          |        |
 | **🛠 Minecraft Core Features**           | 4-5 months | ⏳    | ⏳       | ⏳          |        |
 | **🖼 GUI & Inventory System**            | 3-4 months | ⏳    | ⏳       | ⏳          |        |
 | **🌟 Advanced Features & Refinements**   | 4-6 months | ⏳    | ⏳       | ⏳          |        |
 | **🧪 Beta Testing & Community Feedback** | 3 months   | ⏳    | ⏳       | ⏳          |        |
 | **🚀 Official Release & Support**        | -          | ⏳    | ⏳       | ⏳          |        |
 
 Here's a legend to guide you:
```

