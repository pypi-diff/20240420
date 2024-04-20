# Comparing `tmp/coconut-develop-3.1.0.post0.dev8.tar.gz` & `tmp/coconut-develop-3.1.0.post0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coconut-develop-3.1.0.post0.dev8.tar", last modified: Sat Mar 23 21:42:41 2024, max compression
+gzip compressed data, was "dist/coconut-develop-3.1.0.post0.dev9.tar", last modified: Mon Apr 15 06:18:45 2024, max compression
```

## Comparing `coconut-develop-3.1.0.post0.dev8.tar` & `coconut-develop-3.1.0.post0.dev9.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/
--rw-r--r--   0 runner    (1001) docker     (127)    21396 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/_pyparsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    39680 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/root.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/command/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/command/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/command/resources/zcoconut.pth
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49248 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/command/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/command/command.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/command/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    29403 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/command/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/command/mypy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/command/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/icoconut/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/icoconut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/icoconut/coconut/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/icoconut/coconut/kernel.json
--rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/icoconut/root.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/icoconut/coconut_py3/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/icoconut/coconut_py3/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/icoconut/coconut_py2/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/icoconut/coconut_py2/kernel.json
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/icoconut/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/icoconut/coconut_py/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/icoconut/coconut_py/kernel.json
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/icoconut/embed.py
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/highlighter.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/__coconut__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/__coconut__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13348 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/convenience.py
--rw-r--r--   0 runner    (1001) docker     (127)    24288 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)    14388 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/runner.coco
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/runnable.coco
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_35/
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_35/py35_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_2/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_2/py2_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_3/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_3/py3_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_311/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_311/py311_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/specific.coco
--rw-r--r--   0 runner    (1001) docker     (127)    15411 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/tutorial.coco
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/main.coco
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/__init__.coco
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/__main__.coco
--rw-r--r--   0 runner    (1001) docker     (127)    49541 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/util.coco
--rw-r--r--   0 runner    (1001) docker     (127)    44503 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/suite.coco
--rw-r--r--   0 runner    (1001) docker     (127)    20677 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/primary_2.coco
--rw-r--r--   0 runner    (1001) docker     (127)    50108 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/primary_1.coco
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_38/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_38/py38_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_sys/
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_36/
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_36/py36_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/non_strict/
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
--rw-r--r--   0 runner    (1001) docker     (127)    28547 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/extras.coco
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/src/importable.coco
--rw-r--r--   0 runner    (1001) docker     (127)    36688 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/main_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/tests/constants_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)   226356 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)   113465 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/compiler/grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut/compiler/templates/
--rw-r--r--   0 runner    (1001) docker     (127)   111667 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/compiler/templates/header.py_template
--rw-r--r--   0 runner    (1001) docker     (127)    39710 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/compiler/header.py
--rw-r--r--   0 runner    (1001) docker     (127)    62370 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/compiler/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)    75011 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/compiler/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/coconut/convenience.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/xontrib/
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/xontrib/coconut.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut_develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/coconut_develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/FAQ.md
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    65131 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/HELP.md
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/_coconut/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/_coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/_coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/_coconut/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/__coconut__/
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/__coconut__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/__coconut__/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    68070 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/__coconut__/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13807 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)   218039 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/DOCS.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-03-23 21:42:41.000000 coconut-develop-3.1.0.post0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-23 20:41:44.000000 coconut-develop-3.1.0.post0.dev8/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)    65138 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/HELP.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/
+-rw-r--r--   0 runner    (1001) docker     (127)    24288 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14388 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/__coconut__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39702 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13348 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)    75011 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/compiler/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)   226496 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62370 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/compiler/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/compiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)   111626 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/compiler/templates/header.py_template
+-rw-r--r--   0 runner    (1001) docker     (127)    40157 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/compiler/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113465 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/compiler/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/constants_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36763 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    28626 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/extras.coco
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/runner.coco
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (127)    44618 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/suite.coco
+-rw-r--r--   0 runner    (1001) docker     (127)    15411 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/tutorial.coco
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/__main__.coco
+-rw-r--r--   0 runner    (1001) docker     (127)    50073 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/util.coco
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/main.coco
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/specific.coco
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/__init__.coco
+-rw-r--r--   0 runner    (1001) docker     (127)    20724 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/primary_2.coco
+-rw-r--r--   0 runner    (1001) docker     (127)    50108 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/primary_1.coco
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/non_strict/
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_35/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_35/py35_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_3/py3_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_36/
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_36/py36_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_311/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_311/py311_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_38/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_38/py38_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_sys/
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_2/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_2/py2_test.coco
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/importable.coco
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/tests/src/runnable.coco
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/convenience.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21396 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/_pyparsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/api.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/icoconut/
+-rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/icoconut/root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/icoconut/coconut/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-15 06:18:44.000000 coconut-develop-3.1.0.post0.dev9/coconut/icoconut/coconut/kernel.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/icoconut/coconut_py/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/icoconut/coconut_py/kernel.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/icoconut/coconut_py3/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/icoconut/coconut_py3/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/icoconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/icoconut/embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/icoconut/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/icoconut/coconut_py2/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/icoconut/coconut_py2/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/__coconut__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/command/
+-rw-r--r--   0 runner    (1001) docker     (127)    29403 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/command/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut/command/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/command/resources/zcoconut.pth
+-rw-r--r--   0 runner    (1001) docker     (127)    49248 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/command/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/command/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/command/mypy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/command/command.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/coconut/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut_develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/coconut_develop.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/_coconut/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/_coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/_coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/_coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/xontrib/coconut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/__coconut__/
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/__coconut__/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/__coconut__/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    68137 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/__coconut__/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   220530 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/DOCS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/FAQ.md
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-15 06:18:45.000000 coconut-develop-3.1.0.post0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13807 2024-04-15 05:14:06.000000 coconut-develop-3.1.0.post0.dev9/CONTRIBUTING.md
```

### Comparing `coconut-develop-3.1.0.post0.dev8/conf.py` & `coconut-develop-3.1.0.post0.dev9/conf.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/README.rst` & `coconut-develop-3.1.0.post0.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/_pyparsing.py` & `coconut-develop-3.1.0.post0.dev9/coconut/_pyparsing.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/constants.py` & `coconut-develop-3.1.0.post0.dev9/coconut/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -835,14 +835,15 @@
 # builtins that must be imported from the exact right target header
 must_use_specific_target_builtins = (
     "super",
 )
 
 coconut_exceptions = (
     "MatchError",
+    "CoconutWarning",
 )
 
 highlight_builtins = coconut_specific_builtins + interp_only_builtins + python_builtins
 highlight_exceptions = coconut_exceptions + python_exceptions
 all_builtins = frozenset(
     python_builtins
     + python_exceptions
```

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/__init__.py` & `coconut-develop-3.1.0.post0.dev9/coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/root.py` & `coconut-develop-3.1.0.post0.dev9/coconut/root.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -----------------------------------------------------------------------------------------------------------------------
 # VERSION:
 # -----------------------------------------------------------------------------------------------------------------------
 
 VERSION = "3.1.0"
 VERSION_NAME = None
 # False for release, int >= 1 for develop
-DEVELOP = 8
+DEVELOP = 9
 ALPHA = False  # for pre releases rather than post releases
 
 assert DEVELOP is False or DEVELOP >= 1, "DEVELOP must be False or an int >= 1"
 assert DEVELOP or not ALPHA, "alpha releases are only for develop"
 
 # -----------------------------------------------------------------------------------------------------------------------
 # UTILITIES:
```

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/command/__init__.py` & `coconut-develop-3.1.0.post0.dev9/coconut/command/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/command/command.py` & `coconut-develop-3.1.0.post0.dev9/coconut/command/command.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/command/command.pyi` & `coconut-develop-3.1.0.post0.dev9/coconut/command/command.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/command/cli.py` & `coconut-develop-3.1.0.post0.dev9/coconut/command/cli.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/command/util.py` & `coconut-develop-3.1.0.post0.dev9/coconut/command/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/command/mypy.py` & `coconut-develop-3.1.0.post0.dev9/coconut/command/mypy.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/command/watch.py` & `coconut-develop-3.1.0.post0.dev9/coconut/command/watch.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/api.pyi` & `coconut-develop-3.1.0.post0.dev9/coconut/api.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/icoconut/__init__.py` & `coconut-develop-3.1.0.post0.dev9/coconut/icoconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/icoconut/root.py` & `coconut-develop-3.1.0.post0.dev9/coconut/icoconut/root.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/icoconut/__main__.py` & `coconut-develop-3.1.0.post0.dev9/coconut/icoconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/icoconut/embed.py` & `coconut-develop-3.1.0.post0.dev9/coconut/icoconut/embed.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/requirements.py` & `coconut-develop-3.1.0.post0.dev9/coconut/requirements.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/main.py` & `coconut-develop-3.1.0.post0.dev9/coconut/main.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/highlighter.py` & `coconut-develop-3.1.0.post0.dev9/coconut/highlighter.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/__init__.pyi` & `coconut-develop-3.1.0.post0.dev9/coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/__main__.py` & `coconut-develop-3.1.0.post0.dev9/coconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/__coconut__.pyi` & `coconut-develop-3.1.0.post0.dev9/coconut/__coconut__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,2 +1,2 @@
 from __coconut__ import *
-from __coconut__ import _coconut_tail_call, _coconut_tco, _coconut_call_set_names, _coconut_handle_cls_kwargs, _coconut_handle_cls_stargs, _namedtuple_of, _coconut, _coconut_Expected, _coconut_MatchError, _coconut_SupportsAdd, _coconut_SupportsMinus, _coconut_SupportsMul, _coconut_SupportsPow, _coconut_SupportsTruediv, _coconut_SupportsFloordiv, _coconut_SupportsMod, _coconut_SupportsAnd, _coconut_SupportsXor, _coconut_SupportsOr, _coconut_SupportsLshift, _coconut_SupportsRshift, _coconut_SupportsMatmul, _coconut_SupportsInv, _coconut_Expected, _coconut_MatchError, _coconut_iter_getitem, _coconut_base_compose, _coconut_forward_compose, _coconut_back_compose, _coconut_forward_star_compose, _coconut_back_star_compose, _coconut_forward_dubstar_compose, _coconut_back_dubstar_compose, _coconut_pipe, _coconut_star_pipe, _coconut_dubstar_pipe, _coconut_back_pipe, _coconut_back_star_pipe, _coconut_back_dubstar_pipe, _coconut_none_pipe, _coconut_none_star_pipe, _coconut_none_dubstar_pipe, _coconut_bool_and, _coconut_bool_or, _coconut_none_coalesce, _coconut_minus, _coconut_map, _coconut_partial, _coconut_complex_partial, _coconut_get_function_match_error, _coconut_base_pattern_func, _coconut_addpattern, _coconut_sentinel, _coconut_assert, _coconut_raise, _coconut_mark_as_match, _coconut_reiterable, _coconut_self_match_types, _coconut_dict_merge, _coconut_exec, _coconut_comma_op, _coconut_arr_concat_op, _coconut_mk_anon_namedtuple, _coconut_matmul, _coconut_py_str, _coconut_flatten, _coconut_multiset, _coconut_back_none_pipe, _coconut_back_none_star_pipe, _coconut_back_none_dubstar_pipe, _coconut_forward_none_compose, _coconut_back_none_compose, _coconut_forward_none_star_compose, _coconut_back_none_star_compose, _coconut_forward_none_dubstar_compose, _coconut_back_none_dubstar_compose, _coconut_call_or_coefficient, _coconut_in, _coconut_not_in, _coconut_attritemgetter, _coconut_if_op
+from __coconut__ import _coconut_tail_call, _coconut_tco, _coconut_call_set_names, _coconut_handle_cls_kwargs, _coconut_handle_cls_stargs, _namedtuple_of, _coconut, _coconut_Expected, _coconut_MatchError, _coconut_SupportsAdd, _coconut_SupportsMinus, _coconut_SupportsMul, _coconut_SupportsPow, _coconut_SupportsTruediv, _coconut_SupportsFloordiv, _coconut_SupportsMod, _coconut_SupportsAnd, _coconut_SupportsXor, _coconut_SupportsOr, _coconut_SupportsLshift, _coconut_SupportsRshift, _coconut_SupportsMatmul, _coconut_SupportsInv, _coconut_Expected, _coconut_MatchError, _coconut_iter_getitem, _coconut_base_compose, _coconut_forward_compose, _coconut_back_compose, _coconut_forward_star_compose, _coconut_back_star_compose, _coconut_forward_dubstar_compose, _coconut_back_dubstar_compose, _coconut_pipe, _coconut_star_pipe, _coconut_dubstar_pipe, _coconut_back_pipe, _coconut_back_star_pipe, _coconut_back_dubstar_pipe, _coconut_none_pipe, _coconut_none_star_pipe, _coconut_none_dubstar_pipe, _coconut_bool_and, _coconut_bool_or, _coconut_none_coalesce, _coconut_minus, _coconut_map, _coconut_partial, _coconut_complex_partial, _coconut_get_function_match_error, _coconut_base_pattern_func, _coconut_addpattern, _coconut_sentinel, _coconut_assert, _coconut_raise, _coconut_mark_as_match, _coconut_reiterable, _coconut_self_match_types, _coconut_dict_merge, _coconut_exec, _coconut_comma_op, _coconut_arr_concat_op, _coconut_mk_anon_namedtuple, _coconut_matmul, _coconut_py_str, _coconut_flatten, _coconut_multiset, _coconut_back_none_pipe, _coconut_back_none_star_pipe, _coconut_back_none_dubstar_pipe, _coconut_forward_none_compose, _coconut_back_none_compose, _coconut_forward_none_star_compose, _coconut_back_none_star_compose, _coconut_forward_none_dubstar_compose, _coconut_back_none_dubstar_compose, _coconut_call_or_coefficient, _coconut_in, _coconut_not_in, _coconut_attritemgetter, _coconut_if_op, _coconut_CoconutWarning
```

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/__coconut__.py` & `coconut-develop-3.1.0.post0.dev9/coconut/__coconut__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/api.py` & `coconut-develop-3.1.0.post0.dev9/coconut/api.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/exceptions.py` & `coconut-develop-3.1.0.post0.dev9/coconut/exceptions.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/convenience.py` & `coconut-develop-3.1.0.post0.dev9/coconut/convenience.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/terminal.py` & `coconut-develop-3.1.0.post0.dev9/coconut/terminal.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/util.py` & `coconut-develop-3.1.0.post0.dev9/coconut/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/__init__.py` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_35/py35_test.coco` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_35/py35_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_3/py3_test.coco` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_3/py3_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/specific.coco` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/specific.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/tutorial.coco` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/tutorial.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/main.coco` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/main.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/util.coco` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/util.coco`

 * *Files 2% similar despite different names*

```diff
@@ -789,14 +789,28 @@
     match tree() in t:
         return 0
     match tree(n=n) in t:
         return 1
     match tree(l=l, r=r) in t:
         return 1 + max([depth_2(l), depth_2(r)])
 
+case def depth_3:
+    match(tree()) = 0
+    match(tree(n=n)) = 1
+    match(tree(l=l, r=r)) = 1 + max(depth_3(l), depth_3(r))
+
+def size(empty()) = 0
+addpattern def size(leaf(n)) = 1  # type: ignore
+addpattern def size(node(l, r)) = size(l) + size(r)  # type: ignore
+
+case def size_:
+    match(empty()) = 0
+    match(leaf(n)) = 1
+    match(node(l, r)) = size_(l) + size_(r)
+
 class Tree
 data Node(*children) from Tree
 data Leaf(elem) from Tree
 
 def tree_depth(Leaf(_)) = 0
 addpattern def tree_depth(Node(*children)) =  # type: ignore
     children |> map$(tree_depth) |> max |> (.+1)
@@ -1942,14 +1956,20 @@
 
 def twin_primes(_ :: [p, (.-2) -> p] :: ps) =
     [(p, p+2)] :: twin_primes([p + 2] :: ps)
 
 addpattern def twin_primes() =  # type: ignore
     twin_primes(primes())
 
+case def twin_primes_:
+    match(_ :: [p, (.-2) -> p] :: ps) =
+        [(p, p+2)] :: twin_primes_([p + 2] :: ps)
+    match() =
+        twin_primes_(primes())
+
 
 # class matching
 class HasElems:
     def __init__(self, *elems):
         self.elems = elems
 
 class HasVal:
```

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/suite.coco` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/suite.coco`

 * *Files 0% similar despite different names*

```diff
@@ -149,17 +149,19 @@
     assert duplicate_first1([1,2,3]) == [1,1,2,3] == duplicate_first2([1,2,3]) |> list
     assert one_to_five([1,2,3,4,5]) == [2,3,4]
     assert not one_to_five([0,1,2,3,4,5])
     assert one_to_five([1,5]) == []
     assert -4 == neg_square_u(2) ≠ 4 ∩ 0 ≤ neg_square_u(0) ≤ 0
     assert is_null(null1())
     assert is_null(null2())
-    assert empty() |> depth_1 == 0 == empty() |> depth_2
-    assert leaf(5) |> depth_1 == 1 == leaf(5) |> depth_2
-    assert node(leaf(2), node(empty(), leaf(3))) |> depth_1 == 3 == node(leaf(2), node(empty(), leaf(3))) |> depth_2
+    for depth in (depth_1, depth_2, depth_3):
+        assert empty() |> depth == 0  # type: ignore
+        assert leaf(5) |> depth == 1  # type: ignore
+        assert node(leaf(2), node(empty(), leaf(3))) |> depth == 3  # type: ignore
+    assert size(node(empty(), leaf(10))) == 1 == size_(node(empty(), leaf(10)))
     assert maybes(5, square, plus1) == 26
     assert maybes(None, square, plus1) is None
     assert square <| 2 == 4
     assert (5, 3) |*> mod == 2 == mod <*| (5, 3)
     assert Just(5) <| square <| plus1 == Just(26)  # type: ignore
     assert Nothing() <| square <| plus1 == Nothing()  # type: ignore
     assert not Nothing() == ()
@@ -867,15 +869,15 @@
     assert split1_comma("1,2,3") == ("1", "2,3")
     assert split1_comma("ab,cd,ef") == ("ab", "cd,ef")
     assert split1_comma("1,") == ("1", "")
     assert split1_comma(",2") == ("", "2")
     assert split1_comma(",") == ("", "")
     assert split1_comma("abcd") == ("abcd", "")
     assert primes()$[:5] |> tuple == (2, 3, 5, 7, 11)
-    assert twin_primes()$[:5] |> list == [(3, 5), (5, 7), (11, 13), (17, 19), (29, 31)]
+    assert twin_primes()$[:5] |> list == [(3, 5), (5, 7), (11, 13), (17, 19), (29, 31)] == twin_primes_()$[:5] |> list
     assert stored_default(2) == [2, 1] == stored_default_cls()(2)
     assert stored_default(2) == [2, 1, 2, 1] == stored_default_cls()(2)
     if sys.version_info >= (3,):  # naive namespace classes don't work on py2
         assert stored_default_cls.stored_default(3) == [2, 1, 2, 1, 3, 2, 1]  # type: ignore
     bad = assert_raises$(exc=TypeError)
     tr = triangle(1, 2, 3)
     tv = typed_vector(1, 2)
```

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/primary_2.coco` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/primary_2.coco`

 * *Files 0% similar despite different names*

```diff
@@ -454,14 +454,15 @@
     assert (x -> x -> def y -> (x, y))(1)(2)(3) == (2, 3)
     match def maybe_dup(x, y=x) = (x, y)
     assert maybe_dup(1) == (1, 1) == maybe_dup(x=1)
     assert maybe_dup(1, 2) == (1, 2) == maybe_dup(x=1, y=2)
     assert min((), default=10) == 10 == max((), default=10)
     assert py_min(3, 4) == 3 == py_max(2, 3)
     assert len(zip()) == 0 == len(zip_longest())  # type: ignore
+    assert CoconutWarning `issubclass` Warning
 
     with process_map.multiple_sequential_calls():  # type: ignore
         assert map((+), range(3), range(4)$[:-1], strict=True) |> list == [0, 2, 4] == process_map((+), range(3), range(4)$[:-1], strict=True) |> list  # type: ignore
         assert range(3) |> map$((.+1), strict=True) |> list == [1, 2, 3] == range(3) |> process_map$((.+1), strict=True) |> list  # type: ignore
         my_match_err = MatchError("my match error", 123)
         assert process_map(ident, [my_match_err]) |> list |> str == str([my_match_err])  # type: ignore
         # repeat the same thing again now that my_match_err.str has been called
```

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/agnostic/primary_1.coco` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/agnostic/primary_1.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_sys/target_sys_test.coco` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_sys/target_sys_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/target_36/py36_test.coco` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/target_36/py36_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/src/cocotest/non_strict/non_strict_test.coco` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/src/cocotest/non_strict/non_strict_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/src/extras.coco` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/src/extras.coco`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 from collections.abc import Sequence
 
 os.environ["COCONUT_USE_COLOR"] = "False"
 
 from coconut.__coconut__ import consume as coc_consume
 from coconut.constants import (
     IPY,
@@ -10,14 +11,15 @@
     PY34,
     PY35,
     PY36,
     PY39,
     PYPY,
 )  # type: ignore
 from coconut._pyparsing import USE_COMPUTATION_GRAPH  # type: ignore
+from coconut.terminal import logger
 from coconut.exceptions import (
     CoconutSyntaxError,
     CoconutStyleError,
     CoconutTargetError,
     CoconutParseError,
 )  # type: ignore
 from coconut.convenience import (
@@ -321,15 +323,16 @@
     assert "builder" in parse("[def x -> (x, y) for y in range(10)]", "lenient")
     assert parse("[def x -> (x, y) for y in range(10)]", "lenient").count("def") == 2
     assert parse("123  # derp", "lenient") == "123  # derp"
 
     return True
 
 
-def test_convenience() -> bool:
+def test_api() -> bool:
+    assert not logger.enable_colors(sys.stdout)
     if IPY:
         import coconut.highlighter  # noqa # type: ignore
 
     assert_raises(-> cmd("-f"), SystemExit)
     assert_raises(-> cmd("-pa ."), SystemExit)
     assert_raises(-> cmd("-n . ."), SystemExit)
 
@@ -729,15 +732,15 @@
         assert test_pandas() is True  # .
     print(".", end="")
     if not PYPY and PY39:
         assert test_xarray() is True # ..
     print(".")  # newline bc we print stuff after this
     assert test_setup_none() is True  # ...
     print(".")  # ditto
-    assert test_convenience() is True  # ....
+    assert test_api() is True  # ....
     # everything after here uses incremental parsing, so it must come last
     print(".", end="")
     assert test_incremental() is True  # .....
     if IPY:
         print(".", end="")
         assert test_kernel() is True  # ......
     return True
```

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/main_test.py` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/main_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,16 +170,18 @@
     "OSError: handle is closed",
 )
 
 ignore_last_lines_with = (
     "DeprecationWarning: The distutils package is deprecated",
     "from distutils.version import LooseVersion",
     ": SyntaxWarning: 'int' object is not ",
+    ": CoconutWarning: Deprecated use of ",
     " assert_raises(",
     "Populating initial parsing cache",
+    "_coconut.warnings.warn(",
 )
 
 kernel_installation_msg = (
     "Coconut: Successfully installed Jupyter kernels: '"
     + "', '".join((icoconut_custom_kernel_name,) + icoconut_default_kernel_names) + "'"
 )
```

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/__main__.py` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/tests/constants_test.py` & `coconut-develop-3.1.0.post0.dev9/coconut/tests/constants_test.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/compiler/compiler.py` & `coconut-develop-3.1.0.post0.dev9/coconut/compiler/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -2386,14 +2386,15 @@
             addpattern_decorator = self.get_temp_var("addpattern", loc)
             out.append(
                 handle_indentation(
                     """
 try:
     {addpattern_decorator} = _coconut_addpattern({func_name}) {type_ignore}
 except _coconut.NameError:
+    _coconut.warnings.warn("Deprecated use of 'addpattern def {func_name}' with no prior 'match def {func_name}'", _coconut_CoconutWarning)
     {addpattern_decorator} = lambda f: f
                     """,
                     add_newline=True,
                 ).format(
                     func_name=func_name,
                     addpattern_decorator=addpattern_decorator,
                     type_ignore=self.type_ignore_comment(),
```

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/compiler/grammar.py` & `coconut-develop-3.1.0.post0.dev9/coconut/compiler/grammar.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/compiler/__init__.py` & `coconut-develop-3.1.0.post0.dev9/coconut/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/compiler/templates/header.py_template` & `coconut-develop-3.1.0.post0.dev9/coconut/compiler/templates/header.py_template`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,18 @@
         return obj.to_pandas()
 def _coconut_xarray_to_numpy(obj):
     import xarray
     if isinstance(obj, xarray.Dataset):
         return obj.to_dataframe().to_numpy()
     else:
         return obj.to_numpy()
+class CoconutWarning(Warning{comma_object}):
+    """Exception class used for all Coconut warnings."""
+    __slots__ = ()
+_coconut_CoconutWarning = CoconutWarning
 class MatchError(_coconut_baseclass, Exception):
     """Pattern-matching error. Has attributes .pattern, .value, and .message."""{COMMENT.no_slots_to_allow_setattr_below}
     max_val_repr_len = 500
     def __init__(self, pattern=None, value=None):
         self.pattern = pattern
         self.value = value
         self._message = None
@@ -1435,15 +1439,15 @@
     """Decorator to add new cases to a pattern-matching function (where the new case is checked last).
 
     Pass allow_any_func=True to allow any object as the base_func rather than just pattern-matching functions.
     If add_funcs are passed, addpattern(base_func, add_func) is equivalent to addpattern(base_func)(add_func).
     """
     allow_any_func = kwargs.pop("allow_any_func", False)
     if not allow_any_func and not _coconut.getattr(base_func, "_coconut_is_match", False):
-        _coconut.warnings.warn("Possible misuse of addpattern with non-pattern-matching function " + _coconut.repr(base_func) + " (pass allow_any_func=True to dismiss)", stacklevel=2)
+        _coconut.warnings.warn("Possible misuse of addpattern with non-pattern-matching function " + _coconut.repr(base_func) + " (pass allow_any_func=True to dismiss)", _coconut_CoconutWarning, 2)
     if kwargs:
         raise _coconut.TypeError("addpattern() got unexpected keyword arguments " + _coconut.repr(kwargs))
     if add_funcs:
         return _coconut_base_pattern_func(base_func, *add_funcs)
     return _coconut_partial(_coconut_base_pattern_func, base_func)
 _coconut_addpattern = addpattern
 class _coconut_complex_partial(_coconut_base_callable):
@@ -1705,21 +1709,15 @@
     Accepts one keyword-only argument, side_effect, which specifies a function to call on the argument before it is returned."""
     side_effect = kwargs.pop("side_effect", None)
     if kwargs:
         raise _coconut.TypeError("ident() got unexpected keyword arguments " + _coconut.repr(kwargs))
     if side_effect is not None:
         side_effect(x)
     return x
-def call(_coconut_f{comma_slash}, *args, **kwargs):
-    """Function application operator function.
-
-    Equivalent to:
-        def call(f, /, *args, **kwargs) = f(*args, **kwargs).
-    """
-    return _coconut_f(*args, **kwargs)
+{def_call}
 def safe_call(_coconut_f{comma_slash}, *args, **kwargs):
     """safe_call is a version of call that catches any Exceptions and
     returns an Expected containing either the result or the error.
 
     Equivalent to:
         def safe_call(f, /, *args, **kwargs):
             try:
```

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/compiler/header.py` & `coconut-develop-3.1.0.post0.dev9/coconut/compiler/header.py`

 * *Files 1% similar despite different names*

```diff
@@ -637,15 +637,15 @@
         ),
     )
 
     # second round for format dict elements that use the format dict
     #  (extra_format_dict is to keep indentation levels matching)
     extra_format_dict = dict(
         # when anything is added to this list it must also be added to *both* __coconut__ stub files
-        underscore_imports="{tco_comma}{call_set_names_comma}{handle_cls_args_comma}_namedtuple_of, _coconut, _coconut_Expected, _coconut_MatchError, _coconut_SupportsAdd, _coconut_SupportsMinus, _coconut_SupportsMul, _coconut_SupportsPow, _coconut_SupportsTruediv, _coconut_SupportsFloordiv, _coconut_SupportsMod, _coconut_SupportsAnd, _coconut_SupportsXor, _coconut_SupportsOr, _coconut_SupportsLshift, _coconut_SupportsRshift, _coconut_SupportsMatmul, _coconut_SupportsInv, _coconut_iter_getitem, _coconut_base_compose, _coconut_forward_compose, _coconut_back_compose, _coconut_forward_star_compose, _coconut_back_star_compose, _coconut_forward_dubstar_compose, _coconut_back_dubstar_compose, _coconut_pipe, _coconut_star_pipe, _coconut_dubstar_pipe, _coconut_back_pipe, _coconut_back_star_pipe, _coconut_back_dubstar_pipe, _coconut_none_pipe, _coconut_none_star_pipe, _coconut_none_dubstar_pipe, _coconut_bool_and, _coconut_bool_or, _coconut_none_coalesce, _coconut_minus, _coconut_map, _coconut_partial, _coconut_complex_partial, _coconut_get_function_match_error, _coconut_base_pattern_func, _coconut_addpattern, _coconut_sentinel, _coconut_assert, _coconut_raise, _coconut_mark_as_match, _coconut_reiterable, _coconut_self_match_types, _coconut_dict_merge, _coconut_exec, _coconut_comma_op, _coconut_arr_concat_op, _coconut_mk_anon_namedtuple, _coconut_matmul, _coconut_py_str, _coconut_flatten, _coconut_multiset, _coconut_back_none_pipe, _coconut_back_none_star_pipe, _coconut_back_none_dubstar_pipe, _coconut_forward_none_compose, _coconut_back_none_compose, _coconut_forward_none_star_compose, _coconut_back_none_star_compose, _coconut_forward_none_dubstar_compose, _coconut_back_none_dubstar_compose, _coconut_call_or_coefficient, _coconut_in, _coconut_not_in, _coconut_attritemgetter, _coconut_if_op".format(**format_dict),
+        underscore_imports="{tco_comma}{call_set_names_comma}{handle_cls_args_comma}_namedtuple_of, _coconut, _coconut_Expected, _coconut_MatchError, _coconut_SupportsAdd, _coconut_SupportsMinus, _coconut_SupportsMul, _coconut_SupportsPow, _coconut_SupportsTruediv, _coconut_SupportsFloordiv, _coconut_SupportsMod, _coconut_SupportsAnd, _coconut_SupportsXor, _coconut_SupportsOr, _coconut_SupportsLshift, _coconut_SupportsRshift, _coconut_SupportsMatmul, _coconut_SupportsInv, _coconut_iter_getitem, _coconut_base_compose, _coconut_forward_compose, _coconut_back_compose, _coconut_forward_star_compose, _coconut_back_star_compose, _coconut_forward_dubstar_compose, _coconut_back_dubstar_compose, _coconut_pipe, _coconut_star_pipe, _coconut_dubstar_pipe, _coconut_back_pipe, _coconut_back_star_pipe, _coconut_back_dubstar_pipe, _coconut_none_pipe, _coconut_none_star_pipe, _coconut_none_dubstar_pipe, _coconut_bool_and, _coconut_bool_or, _coconut_none_coalesce, _coconut_minus, _coconut_map, _coconut_partial, _coconut_complex_partial, _coconut_get_function_match_error, _coconut_base_pattern_func, _coconut_addpattern, _coconut_sentinel, _coconut_assert, _coconut_raise, _coconut_mark_as_match, _coconut_reiterable, _coconut_self_match_types, _coconut_dict_merge, _coconut_exec, _coconut_comma_op, _coconut_arr_concat_op, _coconut_mk_anon_namedtuple, _coconut_matmul, _coconut_py_str, _coconut_flatten, _coconut_multiset, _coconut_back_none_pipe, _coconut_back_none_star_pipe, _coconut_back_none_dubstar_pipe, _coconut_forward_none_compose, _coconut_back_none_compose, _coconut_forward_none_star_compose, _coconut_back_none_star_compose, _coconut_forward_none_dubstar_compose, _coconut_back_none_dubstar_compose, _coconut_call_or_coefficient, _coconut_in, _coconut_not_in, _coconut_attritemgetter, _coconut_if_op, _coconut_CoconutWarning".format(**format_dict),
         import_typing=pycondition(
             (3, 5),
             if_ge='''
 import typing as _typing
 for _name in dir(_typing):
     if not hasattr(typing, _name):
         setattr(typing, _name, getattr(_typing, _name))
@@ -861,14 +861,29 @@
     """async_map not available on Python < 3.5"""
     raise _coconut.NameError("async_map not available on Python < 3.5")
             ''',
             needs_vars={
                 "{_coconut_}zip".format(**format_dict): "zip",
             },
         ),
+        def_call=pycondition(
+            (3, 11),
+            if_ge=r'''
+call = _coconut.operator.call
+            ''',
+            if_lt=r'''
+def call(_coconut_f{comma_slash}, *args, **kwargs):
+    """Function application operator function.
+
+    Equivalent to:
+        def call(f, /, *args, **kwargs) = f(*args, **kwargs).
+    """
+    return _coconut_f(*args, **kwargs)
+            '''.format(**format_dict),
+        ),
     )
     format_dict.update(extra_format_dict)
 
     return format_dict
 
 
 # -----------------------------------------------------------------------------------------------------------------------
```

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/compiler/matching.py` & `coconut-develop-3.1.0.post0.dev9/coconut/compiler/matching.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/compiler/util.py` & `coconut-develop-3.1.0.post0.dev9/coconut/compiler/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/integrations.py` & `coconut-develop-3.1.0.post0.dev9/coconut/integrations.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut/convenience.pyi` & `coconut-develop-3.1.0.post0.dev9/coconut/convenience.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/xontrib/coconut.py` & `coconut-develop-3.1.0.post0.dev9/xontrib/coconut.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/coconut_develop.egg-info/SOURCES.txt` & `coconut-develop-3.1.0.post0.dev9/coconut_develop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/FAQ.md` & `coconut-develop-3.1.0.post0.dev9/FAQ.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/setup.py` & `coconut-develop-3.1.0.post0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/HELP.md` & `coconut-develop-3.1.0.post0.dev9/HELP.md`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
         case int() if n > 0:
             return range(1, n+1) |> reduce$(*)
     else:
         raise TypeError("the argument to factorial must be an integer >= 0")
 ```
 
 By making use of the [Coconut `addpattern` syntax](./DOCS.md#addpattern), we can take that from three indentation levels down to one. Take a look:
-```
+```coconut
 def factorial(0) = 1
 
 addpattern def factorial(int() as n if n > 0) =
     """Compute n! where n is an integer >= 0."""
     range(1, n+1) |> reduce$(*)
 
 # Test cases:
```

### Comparing `coconut-develop-3.1.0.post0.dev8/_coconut/__init__.py` & `coconut-develop-3.1.0.post0.dev9/_coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/_coconut/__init__.pyi` & `coconut-develop-3.1.0.post0.dev9/_coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/__coconut__/__init__.py` & `coconut-develop-3.1.0.post0.dev9/__coconut__/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/__coconut__/__init__.pyi` & `coconut-develop-3.1.0.post0.dev9/__coconut__/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -235,14 +235,19 @@
 ) -> _t.Iterable[_T]:
     """Reduce func over iterable, yielding intermediate results,
     optionally starting from initial."""
     ...
 _coconut_scan = scan
 
 
+class CoconutWarning(Warning):
+    pass
+_coconut_CoconutWarning = CoconutWarning
+
+
 class MatchError(Exception):
     """Pattern-matching error. Has attributes .pattern, .value, and .message."""
     pattern: _t.Optional[_t.Text]
     value: _t.Any
     def __init__(self, pattern: _t.Optional[_t.Text] = None, value: _t.Any = None) -> None: ...
     @property
     def message(self) -> _t.Text: ...
@@ -275,51 +280,52 @@
 @_t.overload
 def call(
     _func: _t.Callable[[_T, _U, _V], _W],
     _x: _T,
     _y: _U,
     _z: _V,
 ) -> _W: ...
-# @_t.overload
-# def call(
-#     _func: _t.Callable[_t.Concatenate[_T, _P], _U],
-#     _x: _T,
-#     *args: _t.Any,
-#     **kwargs: _t.Any,
-# ) -> _U: ...
-# @_t.overload
-# def call(
-#     _func: _t.Callable[_t.Concatenate[_T, _U, _P], _V],
-#     _x: _T,
-#     _y: _U,
-#     *args: _t.Any,
-#     **kwargs: _t.Any,
-# ) -> _V: ...
-# @_t.overload
-# def call(
-#     _func: _t.Callable[_t.Concatenate[_T, _U, _V, _P], _W],
-#     _x: _T,
-#     _y: _U,
-#     _z: _V,
-#     *args: _t.Any,
-#     **kwargs: _t.Any,
-# ) -> _W: ...
+@_t.overload
+def call(
+    _func: _t.Callable[_t.Concatenate[_T, _P], _U],
+    _x: _T,
+    *args: _t.Any,
+    **kwargs: _t.Any,
+) -> _U: ...
+@_t.overload
+def call(
+    _func: _t.Callable[_t.Concatenate[_T, _U, _P], _V],
+    _x: _T,
+    _y: _U,
+    *args: _t.Any,
+    **kwargs: _t.Any,
+) -> _V: ...
+@_t.overload
+def call(
+    _func: _t.Callable[_t.Concatenate[_T, _U, _V, _P], _W],
+    _x: _T,
+    _y: _U,
+    _z: _V,
+    *args: _t.Any,
+    **kwargs: _t.Any,
+) -> _W: ...
 @_t.overload
 def call(
     _func: _t.Callable[..., _T],
     *args: _t.Any,
     **kwargs: _t.Any,
 ) -> _T:
     """Function application operator function.
 
     Equivalent to:
         def call(f, /, *args, **kwargs) = f(*args, **kwargs).
     """
     ...
 
+# call = _coconut.operator.call
 _coconut_tail_call = call
 of = _deprecated("use call instead")(call)
 
 
 @_dataclass(frozen=True, slots=True)
 class _BaseExpected(_t.Generic[_T], _t.Tuple):
     result: _t.Optional[_T]
```

### Comparing `coconut-develop-3.1.0.post0.dev8/CONTRIBUTING.md` & `coconut-develop-3.1.0.post0.dev9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.1.0.post0.dev8/DOCS.md` & `coconut-develop-3.1.0.post0.dev9/DOCS.md`

 * *Files 1% similar despite different names*

```diff
@@ -1316,19 +1316,18 @@
 
 ```coconut
 class Tree
 data Empty() from Tree
 data Leaf(n) from Tree
 data Node(l, r) from Tree
 
-def depth(Tree()) = 0
-
-addpattern def depth(Tree(n)) = 1
-
-addpattern def depth(Tree(l, r)) = 1 + max([depth(l), depth(r)])
+case def depth:
+    match(Tree()) = 0
+    match(Tree(n)) = 1
+    match(Tree(l, r)) = 1 + max(depth(l), depth(r))
 
 Empty() |> depth |> print
 Leaf(5) |> depth |> print
 Node(Leaf(2), Node(Empty(), Leaf(3))) |> depth |> print
 ```
 _Showcases how the combination of data types and match statements can be used to powerful effect to replicate the usage of algebraic data types in other functional programming languages._
 
@@ -1336,34 +1335,34 @@
 def duplicate_first([x] + xs as l) =
     [x] + l
 
 [1,2,3] |> duplicate_first |> print
 ```
 _Showcases head-tail splitting, one of the most common uses of pattern-matching, where a `+ <var>` (or `:: <var>` for any iterable) at the end of a list or tuple literal can be used to match the rest of the sequence._
 
-```
-def sieve([head] :: tail) =
-    [head] :: sieve(n for n in tail if n % head)
-
-addpattern def sieve((||)) = []
+```coconut
+case def sieve:
+    match([head] :: tail) =
+        [head] :: sieve(n for n in tail if n % head)
+    match((||)) = []
 ```
 _Showcases how to match against iterators, namely that the empty iterator case (`(||)`) must come last, otherwise that case will exhaust the whole iterator before any other pattern has a chance to match against it._
 
-```
+```coconut
 def odd_primes(p=3) =
     (p,) :: filter(=> _ % p != 0, odd_primes(p + 2))
 
 def primes() =
     (2,) :: odd_primes()
 
-def twin_primes(_ :: [p, (.-2) -> p] :: ps) =
-    [(p, p+2)] :: twin_primes([p + 2] :: ps)
-
-addpattern def twin_primes() =  # type: ignore
-    twin_primes(primes())
+case def twin_primes:
+    match(_ :: [p, (.-2) -> p] :: ps) =
+        [(p, p+2)] :: twin_primes([p + 2] :: ps)
+    match() =
+        twin_primes(primes())
 
 twin_primes()$[:5] |> list |> print
 ```
 _Showcases the use of an iterable search pattern and a view pattern to construct an iterator of all twin primes._
 
 **Python:**
 _Can't be done without a long series of checks for each `match` statement. See the compiled code for the Python syntax._
@@ -1518,23 +1517,22 @@
 _Showcases the syntax, features, and immutable nature of `data` types, as well as the use of default arguments and type annotations._
 
 ```coconut
 data Empty()
 data Leaf(n)
 data Node(l, r)
 
-def size(Empty()) = 0
-
-addpattern def size(Leaf(n)) = 1
-
-addpattern def size(Node(l, r)) = size(l) + size(r)
+case def size:
+    match(Empty()) = 0
+    match(Leaf(n)) = 1
+    match(Node(l, r)) = size(l) + size(r)
 
 size(Node(Empty(), Leaf(10))) == 1
 ```
-_Showcases the algebraic nature of `data` types when combined with pattern-matching._
+_Showcases the use of pattern-matching to deconstruct `data` types._
 
 ```coconut
 data vector(*pts):
     """Immutable arbitrary-length vector."""
 
     def __abs__(self) =
         self.pts |> map$(pow$(?, 2)) |> sum |> pow$(?, 0.5)
@@ -2519,28 +2517,82 @@
 {"x":1, "y":2} |> xydict_to_xytuple |> print
 ```
 
 **Python:**
 _Can't be done without a long series of checks at the top of the function. See the compiled code for the Python syntax._
 
 
+### `case` Functions
+
+For easily defining a pattern-matching function with many different cases, Coconut provides the `case def` syntax based on Coconut's [`case`](#case) syntax. The basic syntax is
+```
+case def <name>:
+    match(<arg>, <arg>, ... [if <cond>]):
+        <body>
+    match(<arg>, <arg>, ... [if <cond>]):
+        <body>
+    ...
+```
+where the patterns in each `match` are checked in sequence until a match is found and the body under that match is executed, or a [`MatchError`](#matcherror) is raised. Each `match(...)` statement is effectively treated as a separate pattern-matching function signature that is checked independently, as if they had each been defined separately and then combined with [`addpattern`](#addpattern).
+
+Any individual body can also be defined with [assignment function syntax](#assignment-functions) such that
+```
+case def <name>:
+    match(<arg>, <arg>, ... [if <cond>]) = <body>
+```
+is equivalent to
+```
+case def <name>:
+    match(<arg>, <arg>, ... [if <cond>]): return <body>
+```
+
+`case` function definition can also be combined with `async` functions, [`copyclosure` functions](#copyclosure-functions), and [`yield` functions](#explicit-generators). The various keywords in front of the `def` can be put in any order.
+
+`case def` also allows for easily providing type annotations for pattern-matching functions. To add type annotations, inside the body of the `case def`, instead of just `match(...)` statements, include some `type(...)` statements as well, which will compile into [`typing.overload`](https://docs.python.org/3/library/typing.html#overload) declarations. The syntax is
+```
+case def <name>[<type vars>]:
+    type(<arg>: <type>, <arg>: <type>, ...) -> <type>
+    type(<arg>: <type>, <arg>: <type>, ...) -> <type>
+    ...
+```
+which can be interspersed with the `match(...)` statements.
+
+##### Example
+
+**Coconut:**
+```coconut
+case def my_min[T]:
+    type(x: T, y: T) -> T
+    match(x, y if x <= y) = x
+    match(x, y) = y
+
+    type(xs: T[]) -> T
+    match([x]) = x
+    match([x] + xs) = my_min(x, my_min(xs))
+```
+
+**Python:**
+_Can't be done without a long series of checks for each pattern-matching. See the compiled code for the Python syntax._
+
 ### `addpattern` Functions
 
 Coconut provides the `addpattern def` syntax as a shortcut for the full
 ```coconut
 @addpattern(func)
 match def func(...):
   ...
 ```
 syntax using the [`addpattern`](#addpattern) decorator.
 
-Additionally, `addpattern def` will act just like a normal [`match def`](#pattern-matching-functions) if the function has not previously been defined, allowing for `addpattern def` to be used for each case rather than requiring `match def` for the first case and `addpattern def` for future cases.
-
 If you want to put a decorator on an `addpattern def` function, make sure to put it on the _last_ pattern function.
 
+For complex multi-pattern functions, it is generally recommended to use [`case def`](#case-functions) over `addpattern def` in most situations.
+
+_Deprecated: `addpattern def` will act just like a normal [`match def`](#pattern-matching-functions) if the function has not previously been defined. This will show a [`CoconutWarning`](#coconutwarning) and is not recommended._
+
 ##### Example
 
 **Coconut:**
 ```coconut
 addpattern def factorial(0) = 1
 addpattern def factorial(n) = n * factorial(n - 1)
 ```
@@ -2950,15 +3002,15 @@
 #### `addpattern`
 
 **addpattern**(_base\_func_, *_add\_funcs_, _allow\_any\_func_=`False`)
 
 Takes one argument that is a [pattern-matching function](#pattern-matching-functions), and returns a decorator that adds the patterns in the existing function to the new function being decorated, where the existing patterns are checked first, then the new. `addpattern` also supports a shortcut syntax where the new patterns can be passed in directly.
 
 Roughly equivalent to:
-```
+```coconut_python
 def _pattern_adder(base_func, add_func):
     def add_pattern_func(*args, **kwargs):
         try:
             return base_func(*args, **kwargs)
         except MatchError:
             return add_func(*args, **kwargs)
     return add_pattern_func
@@ -2988,15 +3040,15 @@
 def print_type(int()):
     print("Received an int.")
 
 print_type()  # appears to work
 print_type(1) # TypeError: print_type() takes 0 positional arguments but 1 was given
 ```
 
-This can be fixed by using either the `match` or `addpattern` keyword. For example:
+This can be fixed by using either the `match` keyword. For example:
 ```coconut
 match def print_type():
     print("Received no arguments.")
 
 addpattern def print_type(int()):
     print("Received an int.")
 
@@ -3339,14 +3391,18 @@
 
 A `MatchError` is raised when a [destructuring assignment](#destructuring-assignment) or [pattern-matching function](#pattern-matching-functions) fails, and thus `MatchError` is provided as a built-in for catching those errors. `MatchError` objects support three attributes: `pattern`, which is a string describing the failed pattern; `value`, which is the object that failed to match that pattern; and `message` which is the full error message. To avoid unnecessary `repr` calls, `MatchError` only computes the `message` once it is actually requested.
 
 Additionally, if you are using [view patterns](#match), you might need to raise your own `MatchError` (though you can also just use a destructuring assignment or pattern-matching function definition to do so). To raise your own `MatchError`, just `raise MatchError(pattern, value)` (both arguments are optional).
 
 In some cases where there are multiple Coconut packages installed at the same time, there may be multiple `MatchError`s defined in different packages. Coconut can perform some magic under the hood to make sure that all these `MatchError`s will seamlessly interoperate, but only if all such packages are compiled in [`--package` mode rather than `--standalone` mode](#compilation-modes).
 
+### `CoconutWarning`
+
+`CoconutWarning` is the [`Warning`](https://docs.python.org/3/library/exceptions.html#Warning) subclass used for all runtime Coconut warnings; see [`warnings`](https://docs.python.org/3/library/warnings.html).
+
 
 ### Generic Built-In Functions
 
 ```{contents}
 ---
 local:
 depth: 1
```

### Comparing `coconut-develop-3.1.0.post0.dev8/PKG-INFO` & `coconut-develop-3.1.0.post0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coconut-develop
-Version: 3.1.0.post0.dev8
+Version: 3.1.0.post0.dev9
 Summary: Simple, elegant, Pythonic functional programming.
 Home-page: http://coconut-lang.org
 Author: Evan Hubinger
 Author-email: evanjhub@gmail.com
 License: Apache 2.0
 Description: |logo| Coconut
         ==============
@@ -85,15 +85,15 @@
         
         .. image:: https://opencollective.com/XX/sponsor/0/avatar.svg
             :target: https://opencollective.com/coconut/sponsor/0/website
         
         __ Sponsor_
         .. _Sponsor: https://opencollective.com/coconut#sponsor
         
-Keywords: functional,programming,language,compiler,pattern,pattern-matching,algebraic,data type,data types,lambda,lambdas,lazy,evaluation,lazy list,lazy lists,tail,recursion,call,recursive,recursive_iterator,infix,function,composition,compose,partial,application,currying,curry,pipeline,pipe,unicode,operator,operators,frozenset,literal,syntax,destructuring,assignment,fold,datamaker,prepattern,iterator,generator,none,coalesce,coalescing,statement,lru_cache,memoization,backport,typing,embed,PEP 622,overrides,islice,itertools,functools,TYPE_CHECKING,Expected,breakpoint,help,reduce,takewhile,dropwhile,tee,count,makedata,consume,process_map,thread_map,addpattern,recursive_generator,fmap,starmap,reiterable,scan,groupsof,memoize,zip_longest,override,flatten,ident,call,safe_call,flip,const,lift,lift_apart,all_equal,collectby,mapreduce,multi_enumerate,cartesian_product,multiset,cycle,windowsof,and_then,and_then_await,async_map,py_chr,py_dict,py_hex,py_input,py_int,py_map,py_object,py_oct,py_open,py_print,py_range,py_str,py_super,py_zip,py_filter,py_reversed,py_enumerate,py_raw_input,py_xrange,py_repr,py_breakpoint,py_min,py_max,_namedtuple_of,reveal_type,reveal_locals,MatchError,__fmap__,__iter_getitem__,data,match,case,cases,where,addpattern,then,operator,type,copyclosure,λ
+Keywords: functional,programming,language,compiler,pattern,pattern-matching,algebraic,data type,data types,lambda,lambdas,lazy,evaluation,lazy list,lazy lists,tail,recursion,call,recursive,recursive_iterator,infix,function,composition,compose,partial,application,currying,curry,pipeline,pipe,unicode,operator,operators,frozenset,literal,syntax,destructuring,assignment,fold,datamaker,prepattern,iterator,generator,none,coalesce,coalescing,statement,lru_cache,memoization,backport,typing,embed,PEP 622,overrides,islice,itertools,functools,TYPE_CHECKING,Expected,breakpoint,help,reduce,takewhile,dropwhile,tee,count,makedata,consume,process_map,thread_map,addpattern,recursive_generator,fmap,starmap,reiterable,scan,groupsof,memoize,zip_longest,override,flatten,ident,call,safe_call,flip,const,lift,lift_apart,all_equal,collectby,mapreduce,multi_enumerate,cartesian_product,multiset,cycle,windowsof,and_then,and_then_await,async_map,py_chr,py_dict,py_hex,py_input,py_int,py_map,py_object,py_oct,py_open,py_print,py_range,py_str,py_super,py_zip,py_filter,py_reversed,py_enumerate,py_raw_input,py_xrange,py_repr,py_breakpoint,py_min,py_max,_namedtuple_of,reveal_type,reveal_locals,MatchError,CoconutWarning,__fmap__,__iter_getitem__,data,match,case,cases,where,addpattern,then,operator,type,copyclosure,λ
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Compilers
```

### Comparing `coconut-develop-3.1.0.post0.dev8/LICENSE.txt` & `coconut-develop-3.1.0.post0.dev9/LICENSE.txt`

 * *Files identical despite different names*

