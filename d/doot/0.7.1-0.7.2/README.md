# Comparing `tmp/doot-0.7.1.tar.gz` & `tmp/doot-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doot-0.7.1.tar", last modified: Wed Apr 17 20:06:27 2024, max compression
+gzip compressed data, was "doot-0.7.2.tar", last modified: Sat Apr 20 15:42:47 2024, max compression
```

## Comparing `doot-0.7.1.tar` & `doot-0.7.2.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:27.000570 doot-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-17 20:06:21.000000 doot-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-17 20:06:27.000570 doot-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-17 20:06:21.000000 doot-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.972570 doot-0.7.1/doot/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.972570 doot-0.7.1/doot/__data/
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__data/aliases.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__data/constants.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.976570 doot-0.7.1/doot/__templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__templates/basic_toml
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__templates/stub_task_py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__templates/tasks_toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.976570 doot-0.7.1/doot/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__tests/test_inits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.976570 doot-0.7.1/doot/_abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/dbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/overlord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.980569 doot-0.7.1/doot/_structs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.980569 doot-0.7.1/doot/_structs/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_action_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_code_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_key_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_key_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_key_path_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_key_string_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_key_type_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_param_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_task_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_task_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/action_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/code_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)    27177 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/param_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/sname.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/structured_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/task_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    12733 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/task_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/toml_loc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.984570 doot-0.7.1/doot/actions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.988570 doot-0.7.1/doot/actions/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_base_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_control_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_job_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_job_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_job_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_job_queuing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_postbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/base_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/control_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    12967 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/job_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/job_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/job_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/job_queuing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/postbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/speak.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/templater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.988570 doot-0.7.1/doot/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.988570 doot-0.7.1/doot/cmds/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/__tests/test_list_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/base_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/clean_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/graph_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/help_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/list_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/locs_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/plugins_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/step_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/stub_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.992570 doot-0.7.1/doot/control/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.992570 doot-0.7.1/doot/control/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/__tests/test_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/__tests/test_overlord.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/__tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/__tests/test_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    19677 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/base_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/overlord.py
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/step_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-17 20:06:21.000000 doot-0.7.1/doot/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-17 20:06:21.000000 doot-0.7.1/doot/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.992570 doot-0.7.1/doot/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:21.000000 doot-0.7.1/doot/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.992570 doot-0.7.1/doot/loaders/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-17 20:06:21.000000 doot-0.7.1/doot/loaders/__tests/test_cmd_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-17 20:06:21.000000 doot-0.7.1/doot/loaders/__tests/test_plugin_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-17 20:06:21.000000 doot-0.7.1/doot/loaders/__tests/test_task_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-17 20:06:21.000000 doot-0.7.1/doot/loaders/cmd_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-17 20:06:21.000000 doot-0.7.1/doot/loaders/plugin_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-04-17 20:06:21.000000 doot-0.7.1/doot/loaders/task_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.992570 doot-0.7.1/doot/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/fail_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/human_numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/param_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/path_manip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/zipper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.992570 doot-0.7.1/doot/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:21.000000 doot-0.7.1/doot/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.992570 doot-0.7.1/doot/parsers/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13792 2024-04-17 20:06:21.000000 doot-0.7.1/doot/parsers/__tests/test_flexible.py
--rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-04-17 20:06:21.000000 doot-0.7.1/doot/parsers/flexible.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.996570 doot-0.7.1/doot/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:21.000000 doot-0.7.1/doot/reporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.996570 doot-0.7.1/doot/reporters/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-17 20:06:21.000000 doot-0.7.1/doot/reporters/__tests/test_stack_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-17 20:06:21.000000 doot-0.7.1/doot/reporters/__tests/test_summary_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-17 20:06:21.000000 doot-0.7.1/doot/reporters/basic_reporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-17 20:06:21.000000 doot-0.7.1/doot/reporters/stack_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-17 20:06:21.000000 doot-0.7.1/doot/reporters/summary_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-17 20:06:21.000000 doot-0.7.1/doot/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.996570 doot-0.7.1/doot/task/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.996570 doot-0.7.1/doot/task/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/__tests/test_base_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/__tests/test_base_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/__tests/test_check_locs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/base_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/base_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/check_locs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/specialised_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:27.000570 doot-0.7.1/doot/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:27.000570 doot-0.7.1/doot/utils/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/__tests/test_action_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/action_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/chain_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/check_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     9018 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/log_colour.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/log_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/mock_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/plugin_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/signal_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/testing_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/trace_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/url_expand.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:27.000570 doot-0.7.1/doot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-17 20:06:26.000000 doot-0.7.1/doot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-17 20:06:26.000000 doot-0.7.1/doot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:06:26.000000 doot-0.7.1/doot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 20:06:26.000000 doot-0.7.1/doot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-17 20:06:26.000000 doot-0.7.1/doot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-17 20:06:26.000000 doot-0.7.1/doot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-17 20:06:21.000000 doot-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:06:27.000570 doot-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.842469 doot-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-20 15:42:41.000000 doot-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-20 15:42:47.838469 doot-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-20 15:42:41.000000 doot-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.814468 doot-0.7.2/doot/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.814468 doot-0.7.2/doot/__data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__data/aliases.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__data/constants.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.814468 doot-0.7.2/doot/__templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__templates/basic_toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__templates/stub_task_py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__templates/tasks_toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.814468 doot-0.7.2/doot/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-20 15:42:41.000000 doot-0.7.2/doot/__tests/test_inits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.818468 doot-0.7.2/doot/_abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/dbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/overlord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_abstract/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.818468 doot-0.7.2/doot/_structs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.822468 doot-0.7.2/doot/_structs/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_action_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_code_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_key_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_key_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_key_path_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_key_string_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_key_type_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_param_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_task_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/__tests/test_task_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/action_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/code_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27177 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/param_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/sname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/structured_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/task_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/task_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/toml_loc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-20 15:42:41.000000 doot-0.7.2/doot/_structs/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.826468 doot-0.7.2/doot/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.826468 doot-0.7.2/doot/actions/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_base_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_job_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_job_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_job_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_job_queuing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_postbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/__tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/base_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12967 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/job_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/job_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/job_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/job_queuing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/postbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/speak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/templater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-20 15:42:41.000000 doot-0.7.2/doot/actions/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.826468 doot-0.7.2/doot/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.830469 doot-0.7.2/doot/cmds/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/__tests/test_list_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/base_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/clean_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/graph_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/help_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/list_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/locs_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/plugins_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/step_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-04-20 15:42:41.000000 doot-0.7.2/doot/cmds/stub_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.830469 doot-0.7.2/doot/control/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.830469 doot-0.7.2/doot/control/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/__tests/test_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/__tests/test_overlord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/__tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/__tests/test_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19677 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/base_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/overlord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/step_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-20 15:42:41.000000 doot-0.7.2/doot/control/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-20 15:42:41.000000 doot-0.7.2/doot/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-20 15:42:41.000000 doot-0.7.2/doot/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.830469 doot-0.7.2/doot/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:41.000000 doot-0.7.2/doot/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.830469 doot-0.7.2/doot/loaders/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-20 15:42:41.000000 doot-0.7.2/doot/loaders/__tests/test_cmd_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-20 15:42:41.000000 doot-0.7.2/doot/loaders/__tests/test_plugin_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-20 15:42:41.000000 doot-0.7.2/doot/loaders/__tests/test_task_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-20 15:42:41.000000 doot-0.7.2/doot/loaders/cmd_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-20 15:42:41.000000 doot-0.7.2/doot/loaders/plugin_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11922 2024-04-20 15:42:41.000000 doot-0.7.2/doot/loaders/task_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.834468 doot-0.7.2/doot/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/fail_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/human_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/param_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/path_manip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-20 15:42:41.000000 doot-0.7.2/doot/mixins/zipper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.834468 doot-0.7.2/doot/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:41.000000 doot-0.7.2/doot/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.834468 doot-0.7.2/doot/parsers/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13792 2024-04-20 15:42:41.000000 doot-0.7.2/doot/parsers/__tests/test_flexible.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-04-20 15:42:41.000000 doot-0.7.2/doot/parsers/flexible.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.834468 doot-0.7.2/doot/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:41.000000 doot-0.7.2/doot/reporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.834468 doot-0.7.2/doot/reporters/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-20 15:42:41.000000 doot-0.7.2/doot/reporters/__tests/test_stack_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-20 15:42:41.000000 doot-0.7.2/doot/reporters/__tests/test_summary_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-20 15:42:41.000000 doot-0.7.2/doot/reporters/basic_reporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-20 15:42:41.000000 doot-0.7.2/doot/reporters/stack_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-20 15:42:41.000000 doot-0.7.2/doot/reporters/summary_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-20 15:42:41.000000 doot-0.7.2/doot/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.834468 doot-0.7.2/doot/task/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.834468 doot-0.7.2/doot/task/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/__tests/test_base_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/__tests/test_base_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/__tests/test_check_locs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/base_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/check_locs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-20 15:42:41.000000 doot-0.7.2/doot/task/specialised_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.838469 doot-0.7.2/doot/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.838469 doot-0.7.2/doot/utils/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/__tests/test_action_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/action_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/chain_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/check_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/log_colour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/log_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/mock_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/plugin_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/signal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/testing_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/trace_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-20 15:42:41.000000 doot-0.7.2/doot/utils/url_expand.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:42:47.838469 doot-0.7.2/doot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-20 15:42:47.000000 doot-0.7.2/doot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-20 15:42:47.000000 doot-0.7.2/doot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 15:42:47.000000 doot-0.7.2/doot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 15:42:47.000000 doot-0.7.2/doot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-20 15:42:47.000000 doot-0.7.2/doot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 15:42:47.000000 doot-0.7.2/doot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-20 15:42:41.000000 doot-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 15:42:47.842469 doot-0.7.2/setup.cfg
```

### Comparing `doot-0.7.1/LICENSE` & `doot-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/PKG-INFO` & `doot-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doot
-Version: 0.7.1
+Version: 0.7.2
 Summary: An opinionated, TOML based task runner
 Author-email: jgrey <jgrey.n.plus.one@gmail.com>
 License:  ACAB License © 2022-12-09 John Grey
         
         
         To the maximum extent applicable by law, and any licenses of components of this work:
         
@@ -67,15 +67,15 @@
 Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pipreqs; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 
 ![doot](https://github.com/jgrey4296/doot/assets/5943270/170a5631-6175-4d92-8d66-e26aa2c2e472)
 # doot
-Version : 0.7.1  
+Version : 0.7.2  
 Author  : John Grey  
 Date    : 2022-12-09  
 
 ## Overview
 This started out as an opinionated rewrite of the [doit](https://pydoit.org/contents.html) task runner.
 For other, more mature alternatives, see [Luigi](https://github.com/spotify/luigi), and [SnakeMake](https://github.com/snakemake/snakemake)
 and, of course, [GNU Make](https://www.gnu.org/software/make/).
```

### Comparing `doot-0.7.1/README.md` & `doot-0.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![doot](https://github.com/jgrey4296/doot/assets/5943270/170a5631-6175-4d92-8d66-e26aa2c2e472)
 # doot
-Version : 0.7.1  
+Version : 0.7.2  
 Author  : John Grey  
 Date    : 2022-12-09  
 
 ## Overview
 This started out as an opinionated rewrite of the [doit](https://pydoit.org/contents.html) task runner.
 For other, more mature alternatives, see [Luigi](https://github.com/spotify/luigi), and [SnakeMake](https://github.com/snakemake/snakemake)
 and, of course, [GNU Make](https://www.gnu.org/software/make/).
```

### Comparing `doot-0.7.1/doot/__data/aliases.toml` & `doot-0.7.2/doot/__data/aliases.toml`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/__data/constants.toml` & `doot-0.7.2/doot/__data/constants.toml`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/__init__.py` & `doot-0.7.2/doot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ##-- logging
 logging         = logmod.getLogger(__name__)
 printer         = logmod.getLogger("doot._printer")
 ##-- end logging
 
 # Global, single points of truth:
-__version__          : Final[str]         = "0.7.1"
+__version__          : Final[str]         = "0.7.2"
 
 CONSTANT_PREFIX      : Final[str]         = "doot.constants"
 ALIAS_PREFIX         : Final[str]         = "doot.aliases"
 TOOL_PREFIX          : Final[str]         = "tool.doot"
 
 config               : TG.TomlGuard       = TG.TomlGuard() # doot config
 constants            : TG.TomlGuard       = TG.TomlGuard.load(constants_file).remove_prefix(CONSTANT_PREFIX)
```

### Comparing `doot-0.7.1/doot/__main__.py` & `doot-0.7.2/doot/__main__.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/__templates/basic_toml` & `doot-0.7.2/doot/__templates/basic_toml`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/__templates/stub_task_py` & `doot-0.7.2/doot/__templates/stub_task_py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/__tests/test_basic.py` & `doot-0.7.2/doot/__tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/__tests/test_inits.py` & `doot-0.7.2/doot/__tests/test_inits.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_abstract/__init__.py` & `doot-0.7.2/doot/_abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_abstract/cmd.py` & `doot-0.7.2/doot/_abstract/cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_abstract/control.py` & `doot-0.7.2/doot/_abstract/control.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_abstract/dbm.py` & `doot-0.7.2/doot/_abstract/dbm.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_abstract/loader.py` & `doot-0.7.2/doot/_abstract/loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_abstract/overlord.py` & `doot-0.7.2/doot/_abstract/overlord.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_abstract/parser.py` & `doot-0.7.2/doot/_abstract/parser.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_abstract/policy.py` & `doot-0.7.2/doot/_abstract/policy.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_abstract/reporter.py` & `doot-0.7.2/doot/_abstract/reporter.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_abstract/structs.py` & `doot-0.7.2/doot/_abstract/structs.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_abstract/task.py` & `doot-0.7.2/doot/_abstract/task.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/__tests/test_action_spec.py` & `doot-0.7.2/doot/_structs/__tests/test_action_spec.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/__tests/test_artifact.py` & `doot-0.7.2/doot/_structs/__tests/test_artifact.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/__tests/test_code_ref.py` & `doot-0.7.2/doot/_structs/__tests/test_code_ref.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/__tests/test_formatter.py` & `doot-0.7.2/doot/_structs/__tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/__tests/test_key.py` & `doot-0.7.2/doot/_structs/__tests/test_key.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/__tests/test_key_decorators.py` & `doot-0.7.2/doot/_structs/__tests/test_key_decorators.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/__tests/test_key_multi.py` & `doot-0.7.2/doot/_structs/__tests/test_key_multi.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/__tests/test_key_path_expansion.py` & `doot-0.7.2/doot/_structs/__tests/test_key_path_expansion.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/__tests/test_key_string_expansion.py` & `doot-0.7.2/doot/_structs/__tests/test_key_string_expansion.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/__tests/test_key_type_expansion.py` & `doot-0.7.2/doot/_structs/__tests/test_key_type_expansion.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/__tests/test_param_spec.py` & `doot-0.7.2/doot/_structs/__tests/test_param_spec.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/__tests/test_stub.py` & `doot-0.7.2/doot/_structs/__tests/test_stub.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/__tests/test_task_name.py` & `doot-0.7.2/doot/_structs/__tests/test_task_name.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/__tests/test_task_spec.py` & `doot-0.7.2/doot/_structs/__tests/test_task_spec.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/action_spec.py` & `doot-0.7.2/doot/_structs/action_spec.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/artifact.py` & `doot-0.7.2/doot/_structs/artifact.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/code_ref.py` & `doot-0.7.2/doot/_structs/code_ref.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/key.py` & `doot-0.7.2/doot/_structs/key.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/param_spec.py` & `doot-0.7.2/doot/_structs/param_spec.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/sname.py` & `doot-0.7.2/doot/_structs/sname.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/structured_name.py` & `doot-0.7.2/doot/_structs/structured_name.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/stub.py` & `doot-0.7.2/doot/_structs/stub.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,20 +111,18 @@
         parts.append(self.parts['doc'])
         if 'ctor' in self.parts:
             parts.append(self.parts['ctor'])
         elif isinstance(self.ctor, type):
             parts.append(TaskStubPart("ctor", type="type", default=f"\"{self.ctor.__module__}{doot.constants.patterns.IMPORT_SEP}{self.ctor.__name__}\""))
         else:
             parts.append(TaskStubPart("ctor", type="type", default=f"\"{self.ctor}\""))
-        if "mixins" in self.parts:
-            parts.append(self.parts['mixins'])
 
         delayed_actions = []
         for key, part in sorted(self.parts.items(), key=lambda x: x[1]):
-            if key in ["name", "version", "ctor", "mixins", 'doc']:
+            if key in ["name", "version", "ctor", "doc"]:
                 continue
             if 'actions' in key:
                 delayed_actions.append(part)
                 continue
             parts.append(part)
 
         # Actions always go at the end
```

### Comparing `doot-0.7.1/doot/_structs/task_name.py` & `doot-0.7.2/doot/_structs/task_name.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/task_spec.py` & `doot-0.7.2/doot/_structs/task_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     depends_on                   : list[DootTaskName|DootTaskArtifact|DootActionSpec]                      = field(default_factory=list)
     setup                        : list[DootTaskName|DootActionSpec]                                       = field(default_factory=list)
     cleanup                      : list[DootTaskName|DootActionSpec]                                       = field(default_factory=list)
     on_fail                      : list[DootTaskName|DootAcitonSpec]                                       = field(default_factory=list)
     priority                     : int                                                                     = field(default=10)
     ctor                         : DootTaskName|DootCodeReference                                          = field(default=None)
     # Any additional information:
-    version                      : str                                                                     = field(default="0.1")
+    version                      : str                                                                     = field(default=doot.__version__)
     # TODO version               : dict                                                                    = field(default_factory=dict)
     print_levels                 : TomlGuard                                                               = field(default_factory=TomlGuard)
     flags                        : TaskFlags                                                               = field(default=TaskFlags.TASK)
 
     extra                        : TomlGuard                                                               = field(default_factory=TomlGuard)
 
     queue_behaviour              : TaskQueueMeta                                                 = field(default=TaskQueueMeta.default)
```

### Comparing `doot-0.7.1/doot/_structs/toml_loc.py` & `doot-0.7.2/doot/_structs/toml_loc.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/_structs/trace.py` & `doot-0.7.2/doot/_structs/trace.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/__tests/test_base_action.py` & `doot-0.7.2/doot/actions/__tests/test_base_action.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/__tests/test_control_flow.py` & `doot-0.7.2/doot/actions/__tests/test_control_flow.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/__tests/test_io.py` & `doot-0.7.2/doot/actions/__tests/test_io.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/__tests/test_job_actions.py` & `doot-0.7.2/doot/actions/__tests/test_job_actions.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/__tests/test_job_expansion.py` & `doot-0.7.2/doot/actions/__tests/test_job_expansion.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/__tests/test_job_injection.py` & `doot-0.7.2/doot/actions/__tests/test_job_injection.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/__tests/test_job_queuing.py` & `doot-0.7.2/doot/actions/__tests/test_job_queuing.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/__tests/test_postbox.py` & `doot-0.7.2/doot/actions/__tests/test_postbox.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/__tests/test_shell.py` & `doot-0.7.2/doot/actions/__tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/__tests/test_state.py` & `doot-0.7.2/doot/actions/__tests/test_state.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/base_action.py` & `doot-0.7.2/doot/actions/base_action.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/compression.py` & `doot-0.7.2/doot/actions/compression.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/control_flow.py` & `doot-0.7.2/doot/actions/control_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         if _fail:
             result = self.ActRE.SKIP
 
         roots = self._build_roots(spec, state, _bases)
         try:
             for arg in args:
                 path = DootKey.build(arg, explicit=True).to_path(spec, state, on_fail=None)
-                match self._get_relative(fpath, roots), _invert:
+                match self._get_relative(path, roots), _invert:
                     case None, True:
                         return
                     case None, False:
                         return result
                     case _, True:
                         return result
                     case _, False:
```

### Comparing `doot-0.7.1/doot/actions/io.py` & `doot-0.7.2/doot/actions/io.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/job_actions.py` & `doot-0.7.2/doot/actions/job_actions.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/job_expansion.py` & `doot-0.7.2/doot/actions/job_expansion.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/job_injection.py` & `doot-0.7.2/doot/actions/job_injection.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/job_queuing.py` & `doot-0.7.2/doot/actions/job_queuing.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     def _build_from(self, base, _from) -> list:
         result = []
         head = base.task_head()
         match _from:
             case None:
                 pass
             case list() as l:
-                queue += l
+                result += l
 
         return result
 
 class JobQueueHead(Action_p):
     """ Queue the head/on_completion task of this job"""
 
     @DootKey.dec.types("base")
```

### Comparing `doot-0.7.1/doot/actions/json.py` & `doot-0.7.2/doot/actions/json.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/postbox.py` & `doot-0.7.2/doot/actions/postbox.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/shell.py` & `doot-0.7.2/doot/actions/shell.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/speak.py` & `doot-0.7.2/doot/actions/speak.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/state.py` & `doot-0.7.2/doot/actions/state.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/templater.py` & `doot-0.7.2/doot/actions/templater.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/actions/util.py` & `doot-0.7.2/doot/actions/util.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/cmds/__tests/test_list_cmd.py` & `doot-0.7.2/doot/cmds/__tests/test_list_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/cmds/base_cmd.py` & `doot-0.7.2/doot/cmds/base_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/cmds/clean_cmd.py` & `doot-0.7.2/doot/cmds/clean_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/cmds/graph_cmd.py` & `doot-0.7.2/doot/cmds/graph_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/cmds/help_cmd.py` & `doot-0.7.2/doot/cmds/help_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/cmds/list_cmd.py` & `doot-0.7.2/doot/cmds/list_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/cmds/locs_cmd.py` & `doot-0.7.2/doot/cmds/locs_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/cmds/plugins_cmd.py` & `doot-0.7.2/doot/cmds/plugins_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/cmds/run_cmd.py` & `doot-0.7.2/doot/cmds/run_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/cmds/step_cmd.py` & `doot-0.7.2/doot/cmds/step_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/cmds/stub_cmd.py` & `doot-0.7.2/doot/cmds/stub_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,14 @@
             self.build_param("cli",                       default=False,           desc="Generate a stub cli arg dict",      prefix="-"),
             self.build_param("printer",                   default=False,           desc="Generate a stub cli arg dict",      prefix="-"),
 
             self.build_param("Flags",                     default=False,           desc="Help Stub Task Flags",              prefix="-"),
 
             self.build_param("name",        type=str,     default=None,            desc="The Name of the new task",                          positional=True),
             self.build_param("ctor",        type=str,     default="task",          desc="The short type name of the task generator",         positional=True),
-            self.build_param("mixins",      type=list,    default=[],              desc="Mixins to add to task/job", prefix="--"),
             self.build_param("suppress-header",           default=True, invisible=True)
             ]
 
     def _import_task_class(self, ctor_name):
         try:
             code_ref = DootCodeReference.build(ctor_name)
             return code_ref.try_import()
@@ -112,49 +111,46 @@
 
     def _stub_task_toml(self, tasks, plugins):
         """
         This creates a toml stub using default values, as best it can
         """
         logging.info("Building Task Toml Stub")
         task_iden                   : DootCodeReference       = DootCodeReference.from_alias(doot.args.on_fail("task").cmd.args.ctor(), "task", plugins)
-        task_iden_with_mixins       : DootCodeReference       = task_iden.add_mixins(*doot.args.on_fail([]).cmd.args.mixins(), plugins=plugins)
 
         if (name:=doot.args.on_fail((None,)).cmd.args.name()) is None:
             raise doot.errors.DootCommandError("No Name Provided for Stub")
 
         # Create stub toml, with some basic information
-        stub                          = TaskStub(ctor=task_iden_with_mixins)
+        stub                          = TaskStub(ctor=task_iden)
         stub['name'].default          = DootTaskName.build(name)
-        stub['mixins'].set(type="list", default=[], comment="mix in additional capabilities")
 
         # add ctor specific fields,
         # such as for dir_walker: roots [], exts [], recursive bool, subtask "", head_task ""
         # works *towards* the task_type, not away, so more specific elements are added over the top of more general elements
         try:
-            task_mro = task_iden_with_mixins.try_import().mro()
+            task_mro = task_iden.try_import().mro()
         except TypeError as err:
             logging.error(err.args[0].replace("\n", ""))
             task_mro = []
             return
 
         for cls in reversed(task_mro):
             try:
                 cls.stub_class(stub)
                 if issubclass(cls, Task_i):
-                    stub['version'].default         = cls.version
-                    stub['doc'].default             = [x for x in cls.class_help().split("\n") if bool(x)]
+                    stub['version'].default         = doot.__version__
+                    stub['doc'].default             = []
             except NotImplementedError:
                 pass
             except AttributeError:
                 pass
 
         # Convert to alises
-        base_a, mixin_a= task_iden_with_mixins.to_aliases("task", plugins)
+        base_a, mixin_a= task_iden.to_aliases("task", plugins)
         stub['ctor'].default   = base_a
-        stub['mixins'].default = mixin_a
 
         # extend the name if there are already tasks with that name
         original_name = stub['name'].default.task
         while str(stub['name'].default) in tasks:
             stub['name'].default.tail.append("$conflicted$")
 
         if original_name != stub['name'].default.task:
```

### Comparing `doot-0.7.1/doot/control/__tests/test_locations.py` & `doot-0.7.2/doot/control/__tests/test_locations.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/control/__tests/test_overlord.py` & `doot-0.7.2/doot/control/__tests/test_overlord.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/control/__tests/test_runner.py` & `doot-0.7.2/doot/control/__tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/control/__tests/test_tracker.py` & `doot-0.7.2/doot/control/__tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/control/base_runner.py` & `doot-0.7.2/doot/control/base_runner.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/control/base_tracker.py` & `doot-0.7.2/doot/control/base_tracker.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/control/locations.py` & `doot-0.7.2/doot/control/locations.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/control/overlord.py` & `doot-0.7.2/doot/control/overlord.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/control/runner.py` & `doot-0.7.2/doot/control/runner.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/control/step_runner.py` & `doot-0.7.2/doot/control/step_runner.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/control/tracker.py` & `doot-0.7.2/doot/control/tracker.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/enums.py` & `doot-0.7.2/doot/enums.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/errors.py` & `doot-0.7.2/doot/errors.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/loaders/__tests/test_cmd_loader.py` & `doot-0.7.2/doot/loaders/__tests/test_cmd_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/loaders/__tests/test_plugin_loader.py` & `doot-0.7.2/doot/loaders/__tests/test_plugin_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/loaders/__tests/test_task_loader.py` & `doot-0.7.2/doot/loaders/__tests/test_task_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/loaders/cmd_loader.py` & `doot-0.7.2/doot/loaders/cmd_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/loaders/plugin_loader.py` & `doot-0.7.2/doot/loaders/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/loaders/task_loader.py` & `doot-0.7.2/doot/loaders/task_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,16 +204,15 @@
                     # case {"name": task_name} if task_name in command_names:
                     #     raise doot.errors.DootTaskLoadError("Name conflict: %s is already a Command", task_name)
                     case {"name": task_name, "group": group} if dont_allow_overloads(task_name, group): # complain on overload
                         raise doot.errors.DootTaskLoadError("Task Name Overloaded: %s : %s", task_name, group)
                     case {"name": task_name, "ctor": str() as task_alias} if task_alias in self.task_builders: # build named plugin type
                         logging.info("Building Task from short name: %s : %s", task_name, task_alias)
                         task_iden                   : DootCodeReference       = DootCodeReference.from_alias(task_alias, "task", self.plugins)
-                        task_iden_with_mixins       : DootCodeReference       = task_iden.add_mixins(*spec.get("mixins", []), plugins=self.plugins)
-                        spec['ctor'] = task_iden_with_mixins
+                        spec['ctor'] = task_iden
                         task_spec = DootTaskSpec.build(spec)
                         if str(task_spec.name) in task_descriptions:
                             logging.warning("Overloading Task: %s : %s", str(task_spec.name), task_alias)
 
                         task_spec.check(ensure=Task_i)
                         task_descriptions[str(task_spec.name)] = task_spec
                     case {"name": task_name}:
```

### Comparing `doot-0.7.1/doot/mixins/enums.py` & `doot-0.7.2/doot/mixins/enums.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/mixins/fail_handler.py` & `doot-0.7.2/doot/mixins/fail_handler.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/mixins/human_numbers.py` & `doot-0.7.2/doot/mixins/human_numbers.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/mixins/importer.py` & `doot-0.7.2/doot/mixins/importer.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/mixins/param_spec.py` & `doot-0.7.2/doot/mixins/param_spec.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/mixins/path_manip.py` & `doot-0.7.2/doot/mixins/path_manip.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/mixins/zipper.py` & `doot-0.7.2/doot/mixins/zipper.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/parsers/__tests/test_flexible.py` & `doot-0.7.2/doot/parsers/__tests/test_flexible.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/parsers/flexible.py` & `doot-0.7.2/doot/parsers/flexible.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/reporters/__tests/test_stack_manager.py` & `doot-0.7.2/doot/reporters/__tests/test_stack_manager.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/reporters/__tests/test_summary_manager.py` & `doot-0.7.2/doot/reporters/__tests/test_summary_manager.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/reporters/basic_reporters.py` & `doot-0.7.2/doot/reporters/basic_reporters.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/reporters/stack_manager.py` & `doot-0.7.2/doot/reporters/stack_manager.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/reporters/summary_manager.py` & `doot-0.7.2/doot/reporters/summary_manager.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/structs.py` & `doot-0.7.2/doot/structs.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/task/__tests/test_base_job.py` & `doot-0.7.2/doot/task/__tests/test_base_job.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/task/__tests/test_base_task.py` & `doot-0.7.2/doot/task/__tests/test_base_task.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/task/__tests/test_check_locs.py` & `doot-0.7.2/doot/task/__tests/test_check_locs.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/task/base_job.py` & `doot-0.7.2/doot/task/base_job.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/task/base_task.py` & `doot-0.7.2/doot/task/base_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 printer = logmod.getLogger("doot._printer")
 
 import doot
 import doot.errors
 import tomlguard
 from doot._abstract import Task_i, Job_i, Action_p, PluginLoader_p
-from doot.enums import TaskFlags, TaskStateEnum
+from doot.enums import TaskFlags, TaskStateEnum, TaskQueueMeta
 from doot.structs import TaskStub, TaskStubPart, DootActionSpec, DootCodeReference, DootTaskName, DootTaskArtifact
 from doot.actions.base_action import DootBaseAction
 from doot.errors import DootTaskLoadError, DootTaskError
 
 from doot.mixins.param_spec import ParamSpecMaker_m
 from doot.mixins.importer import Importer_m
 
@@ -187,24 +187,24 @@
         """ Create a basic toml stub for this task"""
         if bool(list(filter(lambda x: x[0] == "task", TASK_ALISES))):
             stub.ctor = "task"
         else:
             stub.ctor                   = cls
 
         # Come first
-        stub['active_when'].priority    = -90
         stub['required_for'].priority   = -90
         stub['depends_on'].priority     = -100
 
         stub['print_levels'].type       = f"Dict: {PRINT_LOCATIONS}"
         stub['print_levels'].default    = {"head":"INFO","build":"INFO","sleep":"INFO","action":"INFO", "execute":"INFO"}
 
         stub['priority'].default        = 10
         stub['queue_behaviour'].default = "default"
-        stub['queue_behaviour'].comment = "default | auto | reactive"
+        stub['queue_behaviour'].comment = " | ".join({x.name for x in TaskQueueMeta})
+        stub['flags'].comment = " | ".join({x.name for x in TaskFlags})
         return stub
 
     def stub_instance(self, stub) -> TaskStub:
         """ extend the class toml stub with details from this instance """
         stub['name'].default      = self.fullname
         if bool(self.doc):
             stub['doc'].default   = self.doc[:]
```

### Comparing `doot-0.7.1/doot/task/check_locs.py` & `doot-0.7.2/doot/task/check_locs.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/task/specialised_jobs.py` & `doot-0.7.2/doot/task/specialised_jobs.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/utils/__tests/test_action_decorators.py` & `doot-0.7.2/doot/utils/__tests/test_action_decorators.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/utils/action_decorators.py` & `doot-0.7.2/doot/utils/action_decorators.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/utils/chain_get.py` & `doot-0.7.2/doot/utils/chain_get.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/utils/check_protocol.py` & `doot-0.7.2/doot/utils/check_protocol.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/utils/decorators.py` & `doot-0.7.2/doot/utils/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
            actions are (self?, spec, state)
           with and extracted keys from the spec and state.
           This truncates the signature of the action to what is *called*, not what is *used*.
 
           TODO: could take a callable as the prototype to build the signature from
         """
         sig = inspect.signature(fn)
-        min_index = len(sig.parameters) - len(getattr(fn, "_doot_keys"))
+        min_index = len(sig.parameters) - len(getattr(fn, KEY_ANNOTS))
         newsig = sig.replace(parameters=list(sig.parameters.values())[:min_index])
         fn.__signature__ = newsig
         return fn
 
     @staticmethod
     def _update_key_annotations(fn, keys:list[DootKey]) -> True:
         """ update the declared expansion keys on the wrapped action """
```

### Comparing `doot-0.7.1/doot/utils/log_colour.py` & `doot-0.7.2/doot/utils/log_colour.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/utils/log_config.py` & `doot-0.7.2/doot/utils/log_config.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/utils/log_context.py` & `doot-0.7.2/doot/utils/log_context.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/utils/mock_gen.py` & `doot-0.7.2/doot/utils/mock_gen.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/utils/plugin_selector.py` & `doot-0.7.2/doot/utils/plugin_selector.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/utils/retrievers.py` & `doot-0.7.2/doot/utils/retrievers.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/utils/signal_handler.py` & `doot-0.7.2/doot/utils/signal_handler.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/utils/testing_fixtures.py` & `doot-0.7.2/doot/utils/testing_fixtures.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/utils/trace_helper.py` & `doot-0.7.2/doot/utils/trace_helper.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot/utils/url_expand.py` & `doot-0.7.2/doot/utils/url_expand.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/doot.egg-info/PKG-INFO` & `doot-0.7.2/doot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doot
-Version: 0.7.1
+Version: 0.7.2
 Summary: An opinionated, TOML based task runner
 Author-email: jgrey <jgrey.n.plus.one@gmail.com>
 License:  ACAB License © 2022-12-09 John Grey
         
         
         To the maximum extent applicable by law, and any licenses of components of this work:
         
@@ -67,15 +67,15 @@
 Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pipreqs; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 
 ![doot](https://github.com/jgrey4296/doot/assets/5943270/170a5631-6175-4d92-8d66-e26aa2c2e472)
 # doot
-Version : 0.7.1  
+Version : 0.7.2  
 Author  : John Grey  
 Date    : 2022-12-09  
 
 ## Overview
 This started out as an opinionated rewrite of the [doit](https://pydoit.org/contents.html) task runner.
 For other, more mature alternatives, see [Luigi](https://github.com/spotify/luigi), and [SnakeMake](https://github.com/snakemake/snakemake)
 and, of course, [GNU Make](https://www.gnu.org/software/make/).
```

### Comparing `doot-0.7.1/doot.egg-info/SOURCES.txt` & `doot-0.7.2/doot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doot-0.7.1/pyproject.toml` & `doot-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name            = "doot"
-version         = "0.7.1"
+version         = "0.7.2"
 description     = "An opinionated, TOML based task runner"
 readme          = "README.md"
 requires-python = ">=3.11"
 license         = {file = "LICENSE"}
 keywords        = ["toml","taskrunner"]
 authors         = [
   {email = "jgrey.n.plus.one@gmail.com", name  = "jgrey"}
@@ -86,15 +86,15 @@
 log_cli_level = "INFO"
 log_format    = "%(levelname)s %(name)s : %(message)s"
 
 ##-- end pytest
 
 ##-- bumpver
 [tool.bumpver]
-current_version    = "0.7.1"
+current_version    = "0.7.2"
 version_pattern    = "MAJOR.MINOR.PATCH"
 commit_message     = "[bump]: version {old_version} -> {new_version}"
 tag_message        = "{new_version}"
 tag_scope          = "default"
 commit             = true
 # tag                = true
 # push             = true
```

