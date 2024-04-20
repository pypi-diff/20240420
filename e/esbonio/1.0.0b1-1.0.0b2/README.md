# Comparing `tmp/esbonio-1.0.0b1.tar.gz` & `tmp/esbonio-1.0.0b2.tar.gz`

## Comparing `esbonio-1.0.0b1.tar` & `esbonio-1.0.0b2.tar`

### file list

```diff
@@ -1,130 +1,90 @@
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/__main__.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/cli/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/cli/py.typed
--rw-r--r--   0        0        0    14374 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/__init__.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/log.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/py.typed
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/symbols.py
--rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/testing.py
--rw-r--r--   0        0        0    30273 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/directives/__init__.py
--rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/directives/completions.py
--rw-r--r--   0        0        0    28157 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/roles/__init__.py
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/roles/completions.py
--rw-r--r--   0        0        0    28663 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/rst/__init__.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/rst/__main__.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/rst/config.py
--rw-r--r--   0        0        0   116783 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/rst/directives.json
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/rst/directives.py
--rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/rst/io.py
--rw-r--r--   0        0        0    16171 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/rst/roles.json
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/rst/roles.py
--rw-r--r--   0        0        0    28699 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/sphinx/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/sphinx/__main__.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/sphinx/autodoc.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/sphinx/cli.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/sphinx/codeblocks.py
--rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/sphinx/config.py
--rw-r--r--   0        0        0   103678 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/sphinx/directives.json
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/sphinx/directives.py
--rw-r--r--   0        0        0    19868 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/sphinx/domains.py
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/sphinx/images.py
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/sphinx/includes.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/sphinx/line_number_transform.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/sphinx/preview.py
--rw-r--r--   0        0        0    47908 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/sphinx/roles.json
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/sphinx/roles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/util/__init__.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/util/filepaths.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/util/inspect.py
--rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/util/patterns.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/lsp/util/resources.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/__main__.py
--rw-r--r--   0        0        0    13414 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/_configuration.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/_log.py
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/cli.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/feature.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/py.typed
--rw-r--r--   0        0        0    14663 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/server.py
--rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/setup.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/testing.py
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/features/log.py
--rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/features/directives/__init__.py
--rw-r--r--   0        0        0    12669 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/features/directives/completion.py
--rw-r--r--   0        0        0     8149 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/features/preview_manager/__init__.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/features/preview_manager/webview.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/features/sphinx_manager/__init__.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/features/sphinx_manager/client.py
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/features/sphinx_manager/client_mock.py
--rw-r--r--   0        0        0    12457 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/features/sphinx_manager/client_subprocess.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/features/sphinx_manager/config.py
--rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/features/sphinx_manager/manager.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/features/sphinx_support/diagnostics.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/features/sphinx_support/directives.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/server/features/sphinx_support/symbols.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/__main__.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/app.py
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/config.py
--rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/database.py
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/log.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/patches.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/py.typed
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/server.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/transforms.py
--rw-r--r--   0        0        0    18553 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/types.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/util.py
--rw-r--r--   0        0        0     8936 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/handlers/__init__.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/handlers/diagnostics.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/handlers/directives.py
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/handlers/files.py
--rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/handlers/symbols.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/esbonio/sphinx_agent/static/webview.js
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/conftest.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/doctests/example_directive_option_pattern.txt
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/doctests/example_directive_pattern.txt
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/doctests/example_directive_substitution_pattern.txt
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/e2e/conftest.py
--rw-r--r--   0        0        0     5430 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/e2e/test_e2e_diagnostics.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/e2e/test_e2e_directives.py
--rw-r--r--   0        0        0     9680 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/e2e/test_e2e_symbols.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/server/conftest.py
--rw-r--r--   0        0        0    13646 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/server/test_configuration.py
--rw-r--r--   0        0        0    19841 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/server/test_patterns.py
--rw-r--r--   0        0        0    23840 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/server/features/test_directive_completion.py
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/server/features/test_sphinx_manager.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/sphinx-agent/conftest.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/sphinx-agent/test_app.py
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/sphinx-agent/test_sa_build.py
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/sphinx-agent/test_sa_create_app.py
--rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/sphinx-agent/test_sa_unit.py
--rw-r--r--   0        0        0    21815 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/sphinx-agent/test_sa_uri_class.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/sphinx-agent/handlers/test_database.py
--rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/sphinx-agent/handlers/test_diagnostics.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/unit_tests/test_directive_completions.py
--rw-r--r--   0        0        0    10108 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/unit_tests/test_directives.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/unit_tests/test_log.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/unit_tests/test_role_completions.py
--rw-r--r--   0        0        0     9771 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/unit_tests/test_roles.py
--rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/unit_tests/test_rst.py
--rw-r--r--   0        0        0    18049 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/unit_tests/test_sphinx.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/workspaces/demo/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/workspaces/demo/LICENSE
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/workspaces/demo/README.md
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/workspaces/demo/conf.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/workspaces/demo/demo_myst.md
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/workspaces/demo/demo_rst.rst
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/workspaces/demo/index.rst
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/workspaces/demo/pyproject.toml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/workspaces/demo/myst/directives.md
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/workspaces/demo/myst/symbols.md
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/workspaces/demo/rst/directives.rst
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/workspaces/demo/rst/symbols.rst
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/workspaces/demo-error/conf.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/tests/workspaces/demo-error-build/conf.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/README.md
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/hatch.toml
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 esbonio-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/__main__.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/__main__.py
+-rw-r--r--   0        0        0    15079 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/_configuration.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/cli.py
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/events.py
+-rw-r--r--   0        0        0     6316 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/feature.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/py.typed
+-rw-r--r--   0        0        0    15895 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/server.py
+-rw-r--r--   0        0        0    11175 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/setup.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/testing.py
+-rw-r--r--   0        0        0    11410 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/log.py
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/directives/__init__.py
+-rw-r--r--   0        0        0    12670 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/directives/completion.py
+-rw-r--r--   0        0        0     8720 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/preview_manager/__init__.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/preview_manager/webview.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/project_manager/__init__.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/project_manager/manager.py
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/project_manager/project.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/client.py
+-rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/client_subprocess.py
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/config.py
+-rw-r--r--   0        0        0    10847 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/manager.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_support/diagnostics.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_support/directives.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_support/symbols.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/__main__.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/app.py
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/config.py
+-rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/database.py
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/log.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/patches.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/py.typed
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/server.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/transforms.py
+-rw-r--r--   0        0        0    19398 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/types.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/util.py
+-rw-r--r--   0        0        0     7484 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/__init__.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/diagnostics.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/directives.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/files.py
+-rw-r--r--   0        0        0    11601 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/symbols.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/static/webview.js
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/conftest.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/doctests/example_directive_option_pattern.txt
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/doctests/example_directive_pattern.txt
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/doctests/example_directive_substitution_pattern.txt
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/e2e/conftest.py
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/e2e/test_e2e_diagnostics.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/e2e/test_e2e_directives.py
+-rw-r--r--   0        0        0     9680 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/e2e/test_e2e_symbols.py
+-rw-r--r--   0        0        0    11609 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/e2e/test_sphinx_manager.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/server/conftest.py
+-rw-r--r--   0        0        0    13646 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/server/test_configuration.py
+-rw-r--r--   0        0        0    19841 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/server/test_patterns.py
+-rw-r--r--   0        0        0    23840 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/server/features/test_directive_completion.py
+-rw-r--r--   0        0        0    11405 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/server/features/test_logging.py
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/server/features/test_sphinx_config.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/conftest.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/test_app.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/test_sa_build.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/test_sa_create_app.py
+-rw-r--r--   0        0        0    15331 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/test_sa_unit.py
+-rw-r--r--   0        0        0    23900 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/test_sa_uri_class.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/handlers/test_database.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/handlers/test_diagnostics.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/LICENSE
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/README.md
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/conf.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/demo_myst.md
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/demo_rst.rst
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/index.rst
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/pyproject.toml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/myst/diagnostics.md
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/myst/directives.md
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/myst/symbols.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/rst/diagnostics.rst
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/rst/directives.rst
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/rst/symbols.rst
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo-error/conf.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo-error-build/conf.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/README.md
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/hatch.toml
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/PKG-INFO
```

### Comparing `esbonio-1.0.0b1/esbonio/cli/__init__.py` & `esbonio-1.0.0b2/esbonio/server/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import argparse
 import logging
 import sys
 import warnings
-from typing import Literal
-from typing import Union
+from logging.handlers import MemoryHandler
+from typing import Optional
+from typing import Sequence
 
 from pygls.protocol import default_converter
 
+from .server import EsbonioLanguageServer
+from .server import __version__
+from .setup import create_language_server
 
-def esbonio_converter():
-    converter = default_converter()
-    converter.register_structure_hook(Union[Literal["auto"], int], lambda obj, _: obj)
 
-    return converter
-
-
-def setup_cli(progname: str, description: str) -> argparse.ArgumentParser:
+def build_parser() -> argparse.ArgumentParser:
     """Return an argument parser with the default command line options required for
     main.
     """
 
-    cli = argparse.ArgumentParser(prog=f"python -m {progname}", description=description)
+    cli = argparse.ArgumentParser(description="The Esbonio language server")
     cli.add_argument(
         "-p",
         "--port",
         type=int,
         default=None,
         help="start a TCP instance of the language server listening on the given port.",
     )
     cli.add_argument(
-        "--version", action="store_true", help="print the current version and exit."
+        "--version",
+        action="version",
+        version=__version__,
+        help="print the current version and exit.",
     )
 
     modules = cli.add_argument_group(
         "modules", "include/exclude language server modules."
     )
     modules.add_argument(
         "-i",
@@ -53,61 +54,54 @@
         dest="excluded_modules",
         help="exclude a module from the server configuration, can be given multiple times.",
     )
 
     return cli
 
 
-def main(cli: argparse.ArgumentParser):
-    """Standard main function for each of the default language servers."""
-
-    # Put these here to avoid circular import issues.
-    from esbonio.lsp import __version__
-    from esbonio.lsp import create_language_server
-    from esbonio.lsp.log import LOG_NAMESPACE
-    from esbonio.lsp.log import MemoryHandler
-
-    args = cli.parse_args()
-
-    if args.version:
-        print(f"v{__version__}")
-        sys.exit(0)
-
-    modules = list(args.modules)
+def main(argv: Optional[Sequence[str]] = None):
+    cli = build_parser()
+    args = cli.parse_args(argv)
+
+    # Order matters!
+    modules = [
+        "esbonio.server.features.log",
+        "esbonio.server.features.project_manager",
+        "esbonio.server.features.sphinx_manager",
+        "esbonio.server.features.preview_manager",
+        "esbonio.server.features.directives",
+        "esbonio.server.features.sphinx_support.diagnostics",
+        "esbonio.server.features.sphinx_support.symbols",
+        "esbonio.server.features.sphinx_support.directives",
+    ]
 
     for mod in args.included_modules:
         modules.append(mod)
 
     for mod in args.excluded_modules:
         if mod in modules:
             modules.remove(mod)
 
     # Ensure we can capture warnings.
     logging.captureWarnings(True)
-    warnlog = logging.getLogger("py.warnings")
 
     if not sys.warnoptions:
         warnings.simplefilter("default")  # Enable capture of DeprecationWarnings
 
     # Setup a temporary logging handler that can cache messages until the language server
     # is ready to forward them onto the client.
-    logger = logging.getLogger(LOG_NAMESPACE)
-    logger.setLevel(logging.DEBUG)
-
-    handler = MemoryHandler()
-    handler.setLevel(logging.DEBUG)
-    logger.addHandler(handler)
-    warnlog.addHandler(handler)
+    logging.basicConfig(
+        level=logging.DEBUG,
+        handlers=[MemoryHandler(999999, flushLevel=logging.CRITICAL)],
+    )
 
     server = create_language_server(
-        args.server_cls,
+        EsbonioLanguageServer,
         modules,
-        name="esbonio",
-        version=__version__,
-        # TODO: Figure out how to make this extensible
-        converter_factory=esbonio_converter,
+        logger=logging.getLogger("esbonio"),
+        converter_factory=default_converter,
     )
 
     if args.port:
         server.start_tcp("localhost", args.port)
     else:
         server.start_io()
```

### Comparing `esbonio-1.0.0b1/esbonio/lsp/directives/completions.py` & `esbonio-1.0.0b2/esbonio/server/features/directives/completion.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,104 +1,72 @@
-import re
-from typing import Optional
-from typing import Type
+"""Helper functions for completion support"""
 
-from docutils.parsers.rst import Directive
-from lsprotocol.types import CompletionItem
-from lsprotocol.types import CompletionItemKind
-from lsprotocol.types import InsertTextFormat
-from lsprotocol.types import Position
-from lsprotocol.types import Range
-from lsprotocol.types import TextEdit
+from __future__ import annotations
 
-from esbonio.lsp import CompletionContext
+import re
+import typing
 
-__all__ = ["render_directive_completion", "render_directive_option_completion"]
+from lsprotocol import types
 
+from esbonio import server
 
-WORD = re.compile("[a-zA-Z]+")
+if typing.TYPE_CHECKING:
+    from typing import Callable
+    from typing import Dict
+    from typing import Optional
+    from typing import Tuple
 
+    from . import Directive
 
-def render_directive_completion(
-    context: CompletionContext,
-    name: str,
-    directive: Type[Directive],
-) -> Optional[CompletionItem]:
-    """Render the given directive as a ``CompletionItem`` according to the current
-    context.
+    DirectiveRenderer = Callable[
+        [server.CompletionContext, Directive], Optional[types.CompletionItem]
+    ]
 
-    Parameters
-    ----------
-    context
-       The context in which the completion should be rendered.
 
-    name
-       The name of the directive, as it appears in an rst file.
+WORD = re.compile("[a-zA-Z]+")
+_DIRECTIVE_RENDERERS: Dict[Tuple[str, str], DirectiveRenderer] = {}
+"""CompletionItem rendering functions for directives."""
 
-    directive
-       The class that implements the directive.
 
-    Returns
-    -------
-    Optional[CompletionItem]
-       The final completion item or ``None``.
-       If ``None`` is returned, then the given completion should be skipped.
-    """
+def renderer(*, language: str, insert_behavior: str):
+    """Define a new rendering function."""
 
-    if context.config.preferred_insert_behavior == "insert":
-        return _render_directive_with_insert_text(context, name, directive)
+    def fn(f: DirectiveRenderer) -> DirectiveRenderer:
+        _DIRECTIVE_RENDERERS[(language, insert_behavior)] = f
+        return f
 
-    return _render_directive_with_text_edit(context, name, directive)
+    return fn
 
 
-def render_directive_option_completion(
-    context: CompletionContext,
-    name: str,
-    directive: str,
-    implementation: Type[Directive],
-) -> Optional[CompletionItem]:
-    """Render the given directive option as a ``CompletionItem`` according to the
-    current context.
+def get_directive_renderer(
+    language: str, insert_behavior: str
+) -> Optional[DirectiveRenderer]:
+    """Return the directive renderer to use.
 
     Parameters
     ----------
-    context
-       The context in which the completion should be rendered.
-
-    name
-       The name of the option, as it appears in an rst file.
+    language
+       The source language the completion item will be inserted into
 
-    directive
-       The name of the directive, as it appears in an rst file.
-
-    implementation
-       The class implementing the directive.
+    insert_behavior
+       How the completion should behave when inserted.
 
     Returns
     -------
-    Optional[CompletionItem]
-       The final completion item or ``None``.
-       If ``None`` is returned, the given completion should be skipped.
+    Optional[DirectiveRenderer]
+       The rendering function to use that matches the given criteria, if available.
     """
+    return _DIRECTIVE_RENDERERS.get((language, insert_behavior), None)
 
-    if context.config.preferred_insert_behavior == "insert":
-        return _render_directive_option_with_insert_text(
-            context, name, directive, implementation
-        )
 
-    return _render_directive_option_with_text_edit(
-        context, name, directive, implementation
-    )
-
-
-def _render_directive_with_insert_text(
-    context: CompletionContext,
-    name: str,
-    directive: Type[Directive],
-) -> Optional[CompletionItem]:
+@renderer(language="rst", insert_behavior="insert")
+def render_rst_directive_with_insert_text(
+    context: server.CompletionContext,
+    directive: Directive,
+) -> Optional[types.CompletionItem]:
     """Render a ``CompletionItem`` using ``insertText`` fields.
 
     This implements the ``insert`` behavior for directives.
     Parameters
     ----------
     context
        The context in which the completion is being generated.
@@ -106,19 +74,19 @@
     name
        The name of the directive, as it appears in an rst file.
 
     directive
        The class implementing the directive.
 
     """
-    insert_text = f".. {name}::"
+    insert_text = f".. {directive.name}::"
     user_text = context.match.group(0).strip()
 
     # Since we can't replace any existing text, it only makes sense
-    # to offer completions that ailgn with what the user has already written.
+    # to offer completions that align with what the user has already written.
     if not insert_text.startswith(user_text):
         return None
 
     # Except that's not entirely true... to quote the LSP spec. (emphasis added)
     #
     # > in the model the client should filter against what the user has already typed
     # > **using the word boundary rules of the language** (e.g. resolving the word
@@ -156,198 +124,288 @@
     # Look for groups of word chars, replace text until the start of the final group
     else:
         start_indices = [m.start() for m in WORD.finditer(user_text)] or [
             len(user_text)
         ]
         start_index = max(start_indices)
 
-    item = _render_directive_common(name, directive)
+    item = _render_directive_common(directive)
     item.insert_text = insert_text[start_index:]
+    item.insert_text_format = types.InsertTextFormat.PlainText
     return item
 
 
-def _render_directive_with_text_edit(
-    context: CompletionContext,
-    name: str,
-    directive: Type[Directive],
-) -> Optional[CompletionItem]:
-    """Render a directive's ``CompletionItem`` using the ``textEdit`` field.
-
-    This implements the ``replace`` insert behavior for directives.
+@renderer(language="rst", insert_behavior="replace")
+def render_rst_directive_with_text_edit(
+    context: server.CompletionContext,
+    directive: Directive,
+) -> Optional[types.CompletionItem]:
+    """Render a ``CompletionItem`` for a reStructuredText directive using the
+    ``textEdit`` field.
 
     Parameters
     ----------
     context
        The context in which the completion is being generated.
 
-    name
-       The name of the directive, as it appears in an rst file.
-
     directive
-       The class implementing the directive.
+       The directive to render.
 
+    Returns
+    -------
+    Optional[types.CompletionItem]
+       The rendered completion item
     """
     match = context.match
 
-    # Calculate the range of text the CompletionItems should edit.
-    # If there is an existing argument to the directive, we should leave it untouched
-    # otherwise, edit the whole line to insert any required arguments.
+    # Calculate the range of text the CompletionItems should edit, we don't need to
+    # touch indentation.
     start = match.span()[0] + match.group(0).find(".")
-    include_argument = context.snippet_support
-    end = match.span()[1]
 
     if match.group("argument"):
-        include_argument = False
+        # If there is an existing argument to the directive, we should leave it
+        # untouched
         end = match.span()[0] + match.group(0).find("::") + 2
-
-    range_ = Range(
-        start=Position(line=context.position.line, character=start),
-        end=Position(line=context.position.line, character=end),
-    )
-
-    # TODO: Give better names to arguments based on what they represent.
-    if include_argument:
-        insert_format = InsertTextFormat.Snippet
-        nargs = getattr(directive, "required_arguments", 0)
-        args = " " + " ".join("${{{0}:arg{0}}}".format(i) for i in range(1, nargs + 1))
     else:
-        args = ""
-        insert_format = InsertTextFormat.PlainText
+        end = match.span()[1]
 
-    insert_text = f".. {name}::{args}"
+    insert_text = f".. {directive.name}::"
 
-    item = _render_directive_common(name, directive)
+    item = _render_directive_common(directive)
     item.filter_text = insert_text
-    item.text_edit = TextEdit(range=range_, new_text=insert_text)
-    item.insert_text_format = insert_format
+    item.insert_text_format = types.InsertTextFormat.PlainText
+    item.text_edit = types.TextEdit(
+        new_text=insert_text,
+        range=types.Range(
+            start=types.Position(line=context.position.line, character=start),
+            end=types.Position(line=context.position.line, character=end),
+        ),
+    )
 
     return item
 
 
-def _render_directive_common(
-    name: str,
-    directive: Type[Directive],
-) -> CompletionItem:
-    """Render the common fields of a directive's completion item."""
+@renderer(language="markdown", insert_behavior="replace")
+def render_myst_directive_with_text_edit(
+    context: server.CompletionContext,
+    directive: Directive,
+) -> Optional[types.CompletionItem]:
+    """Render a ``CompletionItem`` for a MyST directive using the ``textEdit`` field.
 
-    try:
-        dotted_name = f"{directive.__module__}.{directive.__name__}"
-    except AttributeError:
-        dotted_name = f"{directive.__module__}.{directive.__class__.__name__}"
-
-    return CompletionItem(
-        label=name,
-        detail=dotted_name,
-        kind=CompletionItemKind.Class,
-        data={"completion_type": "directive"},
+    Parameters
+    ----------
+    context
+       The context in which the completion is being generated.
+
+    directive
+       The directive to render.
+
+    Returns
+    -------
+    Optional[types.CompletionItem]
+       The rendered completion item
+    """
+
+    # Calculate the range of text the CompletionItems should edit, we don't need to
+    # touch indentation.
+    start = context.match.span()[0] + context.match.group(0).find("`")
+
+    if has_argument := context.match.group("argument"):
+        end = context.match.span()[0] + context.match.group(0).find("}") + 1
+    else:
+        end = context.match.span()[1]
+
+    if context.snippet_support and not has_argument:
+        insert_text = f"```{{{directive.name}}} $0\n```"
+        insert_text_format = types.InsertTextFormat.Snippet
+    else:
+        insert_text = f"```{{{directive.name}}}"
+        insert_text_format = types.InsertTextFormat.PlainText
+
+    item = _render_directive_common(directive)
+    item.filter_text = insert_text
+    item.insert_text_format = insert_text_format
+    item.text_edit = types.TextEdit(
+        new_text=insert_text,
+        range=types.Range(
+            start=types.Position(line=context.position.line, character=start),
+            end=types.Position(line=context.position.line, character=end),
+        ),
     )
 
+    return item
 
-def _render_directive_option_with_insert_text(
-    context: CompletionContext,
-    name: str,
-    directive: str,
-    implementation: Type[Directive],
-) -> Optional[CompletionItem]:
-    """Render a directive option's ``CompletionItem`` using the ``insertText`` field.
 
-    This implements the ``insert`` insert behavior for directive options.
+@renderer(language="markdown", insert_behavior="insert")
+def render_myst_directive_with_insert_text(
+    context: server.CompletionContext,
+    directive: Directive,
+) -> Optional[types.CompletionItem]:
+    """Render a ``CompletionItem`` for a MyST directive using the ``insertText`` field.
 
     Parameters
     ----------
     context
        The context in which the completion is being generated.
 
-    name
-       The name of the directive option, as it appears in an rst file.
-
     directive
-       The name of the directive, as it appears in an rst file.
-
-    implementation
-       The class implementing the directive.
+       The directive to render.
 
+    Returns
+    -------
+    Optional[types.CompletionItem]
+       The rendered completion item
     """
+    if context.snippet_support:
+        insert_text = f"```{{{directive.name}}} $0\n```"
+        insert_text_format = types.InsertTextFormat.Snippet
+    else:
+        insert_text = f"```{{{directive.name}}}"
+        insert_text_format = types.InsertTextFormat.PlainText
 
-    insert_text = f":{name}:"
     user_text = context.match.group(0).strip()
 
+    # Since we can't replace any existing text, it only makes sense
+    # to offer completions that align with what the user has already written.
     if not insert_text.startswith(user_text):
         return None
 
-    if user_text.endswith((":", "-", " ")):
+    # See comment in `render_rst_directive_with_insert_text` above for an extended
+    # discussion on how `insertText` completions work.
+
+    # If the existing text ends with a delimiter, then we should simply remove the
+    # entire prefix
+    if user_text.endswith((":", "-", "{", "}", "`")):
         start_index = len(user_text)
 
     else:
+        # Look for groups of word chars, replace text until the start of the final group
         start_indices = [m.start() for m in WORD.finditer(user_text)] or [
             len(user_text)
         ]
         start_index = max(start_indices)
 
-    item = _render_directive_option_common(name, directive, implementation)
+    item = _render_directive_common(directive)
     item.insert_text = insert_text[start_index:]
+    item.insert_text_format = insert_text_format
+
     return item
 
 
-def _render_directive_option_with_text_edit(
-    context: CompletionContext,
-    name: str,
-    directive: str,
-    implementation: Type[Directive],
-) -> CompletionItem:
-    """Render a directive option's ``CompletionItem`` using the``textEdit`` field.
+def _render_directive_common(directive: Directive) -> types.CompletionItem:
+    """Render the common fields of a directive's completion item."""
 
-    This implements the ``replace`` insert behavior for directive options.
+    return types.CompletionItem(
+        label=directive.name,
+        detail=directive.implementation,
+        kind=types.CompletionItemKind.Class,
+        data={"completion_type": "directive"},
+    )
 
-    Parameters
-    ----------
-    context
-       The context in which the completion is being generated.
 
-    name
-       The name of the directive option, as it appears in an rst file.
+# def _render_directive_option_with_insert_text(
+#     context: CompletionContext,
+#     directive: Directive,
+# ) -> Optional[types.CompletionItem]:
+#     """Render a directive option's ``CompletionItem`` using the ``insertText`` field.
 
-    directive
-       The name of the directive, as it appears in an rst file.
+#     This implements the ``insert`` insert behavior for directive options.
 
-    implementation
-       The class implementing the directive.
+#     Parameters
+#     ----------
+#     context
+#        The context in which the completion is being generated.
 
-    """
+#     name
+#        The name of the directive option, as it appears in an rst file.
 
-    match = context.match
-    groups = match.groupdict()
+#     directive
+#        The name of the directive, as it appears in an rst file.
 
-    option = groups["option"]
-    start = match.span()[0] + match.group(0).find(option)
-    end = start + len(option)
-
-    range_ = Range(
-        start=Position(line=context.position.line, character=start),
-        end=Position(line=context.position.line, character=end),
-    )
+#     implementation
+#        The class implementing the directive.
 
-    insert_text = f":{name}:"
+#     """
 
-    item = _render_directive_option_common(name, directive, implementation)
-    item.filter_text = insert_text
-    item.text_edit = TextEdit(range=range_, new_text=insert_text)
+#     insert_text = f":{name}:"
+#     user_text = context.match.group(0).strip()
 
-    return item
+#     if not insert_text.startswith(user_text):
+#         return None
 
+#     if user_text.endswith((":", "-", " ")):
+#         start_index = len(user_text)
 
-def _render_directive_option_common(
-    name: str, directive: str, impl: Type[Directive]
-) -> CompletionItem:
-    """Render the common fields of a directive option's completion item."""
-
-    try:
-        impl_name = f"{impl.__module__}.{impl.__name__}"
-    except AttributeError:
-        impl_name = f"{impl.__module__}.{impl.__class__.__name__}"
-
-    return CompletionItem(
-        label=name,
-        detail=f"{impl_name}:{name}",
-        kind=CompletionItemKind.Field,
-        data={"completion_type": "directive_option", "for_directive": directive},
-    )
+#     else:
+#         start_indices = [m.start() for m in WORD.finditer(user_text)] or [
+#             len(user_text)
+#         ]
+#         start_index = max(start_indices)
+
+#     item = _render_directive_option_common(name, directive, implementation)
+#     item.insert_text = insert_text[start_index:]
+#     return item
+
+
+# def _render_directive_option_with_text_edit(
+#     context: CompletionContext,
+#     name: str,
+#     directive: str,
+#     implementation: Type[Directive],
+# ) -> CompletionItem:
+#     """Render a directive option's ``CompletionItem`` using the``textEdit`` field.
+
+#     This implements the ``replace`` insert behavior for directive options.
+
+#     Parameters
+#     ----------
+#     context
+#        The context in which the completion is being generated.
+
+#     name
+#        The name of the directive option, as it appears in an rst file.
+
+#     directive
+#        The name of the directive, as it appears in an rst file.
+
+#     implementation
+#        The class implementing the directive.
+
+#     """
+
+#     match = context.match
+#     groups = match.groupdict()
+
+#     option = groups["option"]
+#     start = match.span()[0] + match.group(0).find(option)
+#     end = start + len(option)
+
+#     range_ = Range(
+#         start=Position(line=context.position.line, character=start),
+#         end=Position(line=context.position.line, character=end),
+#     )
+
+#     insert_text = f":{name}:"
+
+#     item = _render_directive_option_common(name, directive, implementation)
+#     item.filter_text = insert_text
+#     item.text_edit = TextEdit(range=range_, new_text=insert_text)
+
+#     return item
+
+
+# def _render_directive_option_common(
+#     name: str, directive: str, impl: Type[Directive]
+# ) -> CompletionItem:
+#     """Render the common fields of a directive option's completion item."""
+
+#     try:
+#         impl_name = f"{impl.__module__}.{impl.__name__}"
+#     except AttributeError:
+#         impl_name = f"{impl.__module__}.{impl.__class__.__name__}"
+
+#     return CompletionItem(
+#         label=name,
+#         detail=f"{impl_name}:{name}",
+#         kind=CompletionItemKind.Field,
+#         data={"completion_type": "directive_option", "for_directive": directive},
+#     )
```

### Comparing `esbonio-1.0.0b1/esbonio/lsp/sphinx/images.py` & `esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/directives.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,114 +1,112 @@
-import os.path
-import pathlib
+import importlib
+import inspect
 from typing import List
 from typing import Optional
-from typing import Tuple
+from typing import Type
 
-import pygls.uris as Uri
-from lsprotocol.types import CompletionItem
-from lsprotocol.types import Location
-from lsprotocol.types import Position
-from lsprotocol.types import Range
-from pygls.workspace import Document
-
-from esbonio.lsp.directives import Directives
-from esbonio.lsp.rst import CompletionContext
-from esbonio.lsp.rst import DefinitionContext
-from esbonio.lsp.rst import DocumentLinkContext
-from esbonio.lsp.sphinx import SphinxLanguageServer
-from esbonio.lsp.util.filepaths import complete_sphinx_filepaths
-from esbonio.lsp.util.filepaths import path_to_completion_item
-
-
-class Images:
-    def __init__(self, rst: SphinxLanguageServer):
-        self.rst = rst
-        self.logger = rst.logger.getChild(self.__class__.__name__)
-
-    def complete_arguments(
-        self, context: CompletionContext, domain: str, name: str
-    ) -> List[CompletionItem]:
-        if domain or name not in {"figure", "image"}:
-            return []
-
-        if not self.rst.app:
-            return []
-
-        srcdir = self.rst.app.srcdir
-        partial = context.match.group("argument")
-        base = os.path.dirname(Uri.to_fs_path(context.doc.uri))
-        items = complete_sphinx_filepaths(srcdir, base, partial)  # type: ignore[arg-type]
-
-        return [path_to_completion_item(context, p) for p in items]
-
-    def find_definitions(
-        self,
-        context: DefinitionContext,
-        directive: str,
-        domain: Optional[str],
-        argument: str,
-    ) -> List[Location]:
-        if domain or directive not in {"figure", "image"}:
-            return []
-
-        uri = self.resolve_path(context.doc, argument)
-        if not uri:
-            return []
-
-        return [
-            Location(
-                uri=uri,
-                range=Range(
-                    start=Position(line=0, character=0),
-                    end=Position(line=1, character=0),
-                ),
-            )
-        ]
-
-    def resolve_link(
-        self,
-        context: DocumentLinkContext,
-        directive: str,
-        domain: Optional[str],
-        argument: str,
-    ) -> Tuple[Optional[str], Optional[str]]:
-        if domain or directive not in {"figure", "image"}:
-            return None, None
-
-        if argument.startswith("https://") or argument.startswith("http://"):
-            return argument, None
-
-        return self.resolve_path(context.doc, argument), None
-
-    def resolve_path(self, doc: Document, argument: str) -> Optional[str]:
-        if argument.startswith("/"):
-            if not self.rst.app:
-                return None
-
-            basedir = pathlib.Path(self.rst.app.srcdir)
-
-            # Remove the leading '/' otherwise is will wipe out the basedir when
-            # concatenated
-            argument = argument[1:]
-
-        else:
-            basedir = pathlib.Path(Uri.to_fs_path(doc.uri)).parent
-
-        try:
-            fullpath = basedir / argument
-            fpath = fullpath.resolve()
-
-            if fpath.exists():
-                return Uri.from_fs_path(str(fpath))
-        except Exception:
-            self.logger.debug("Unable to resolve filepath '%s'", fullpath)
+from docutils.parsers.rst import Directive
+from docutils.parsers.rst import directives as docutils_directives
 
+from .. import types
+from ..app import Database
+from ..app import Sphinx
+from ..util import as_json
+
+DIRECTIVES_TABLE = Database.Table(
+    "directives",
+    [
+        Database.Column(name="name", dtype="TEXT"),
+        Database.Column(name="implementation", dtype="TEXT"),
+        Database.Column(name="location", dtype="JSON"),
+    ],
+)
+
+
+def get_impl_name(directive: Type[Directive]) -> str:
+    try:
+        return f"{directive.__module__}.{directive.__name__}"
+    except AttributeError:
+        return f"{directive.__module__}.{directive.__class__.__name__}"
+
+
+def get_impl_location(impl: Type[Directive]) -> Optional[str]:
+    """Get the implementation location of the given directive"""
+
+    try:
+        if (filepath := inspect.getsourcefile(impl)) is None:
+            return None
+
+        uri = types.Uri.for_file(filepath).resolve()
+        source, line = inspect.getsourcelines(impl)
+
+        location = types.Location(
+            uri=str(uri),
+            range=types.Range(
+                start=types.Position(line=line - 1, character=0),
+                end=types.Position(line=line + len(source), character=0),
+            ),
+        )
+
+        return as_json(location)
+    except Exception:
+        # TODO: Log the error somewhere..
         return None
 
 
-def esbonio_setup(rst: SphinxLanguageServer, directives: Directives):
-    images = Images(rst)
+def index_directives(app: Sphinx):
+    """Index all the directives that are available to this app.
+
+    Note: While it would be ideal to resolve the implementation location of each
+    directive here, the ``get_impl_location`` function is too slow causing a noticable
+    lag when initializing the sphinx agent.
+
+    Perhaps it's worth investigating adding our own custom events. If we could register
+    a handler and do work on an "initial" doctree when it becomes available, then we can
+    resolve the location of just the directives that are used, as we see them for the
+    first time.
+    """
+
+    directives: List[types.Directive] = []
+
+    ignored_directives = {"restructuredtext-test-directive"}
+    found_directives = {
+        **docutils_directives._directive_registry,
+        **docutils_directives._directives,
+    }
+
+    for name, directive in found_directives.items():
+        if name in ignored_directives:
+            continue
+
+        # core docutils directives are a (module, Class) reference.
+        if isinstance(directive, tuple):
+            try:
+                mod, cls = directive
+                modulename = f"docutils.parsers.rst.directives.{mod}"
+                module = importlib.import_module(modulename)
+
+                directive = getattr(module, cls)
+            except Exception:
+                # TODO: Log the error somewhere...
+                directives.append((name, None, None))
+                continue
+
+        directives.append((name, get_impl_name(directive), None))
+
+    for prefix, domain in app.env.domains.items():
+        for name, directive in domain.directives.items():
+            directives.append(
+                (
+                    f"{prefix}:{name}",
+                    get_impl_name(directive),
+                    None,
+                )
+            )
+
+    app.esbonio.db.ensure_table(DIRECTIVES_TABLE)
+    app.esbonio.db.clear_table(DIRECTIVES_TABLE)
+    app.esbonio.db.insert_values(DIRECTIVES_TABLE, directives)
+
 
-    directives.add_argument_definition_provider(images)
-    directives.add_argument_completion_provider(images)
-    directives.add_argument_link_provider(images)
+def setup(app: Sphinx):
+    app.connect("builder-inited", index_directives)
```

### Comparing `esbonio-1.0.0b1/esbonio/server/_configuration.py` & `esbonio-1.0.0b2/esbonio/server/_configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,62 +1,85 @@
 from __future__ import annotations
 
+import asyncio
 import inspect
 import json
 import pathlib
+import traceback
 import typing
-from typing import Any
-from typing import Awaitable
-from typing import Callable
-from typing import Dict
+from functools import partial
 from typing import Generic
-from typing import List
-from typing import Optional
-from typing import Set
-from typing import Type
 from typing import TypeVar
-from typing import Union
 
 import attrs
 from lsprotocol import types
 from pygls.capabilities import get_capability
 
 from . import Uri
 
+T = TypeVar("T")
+
 if typing.TYPE_CHECKING:
+    from typing import Any
+    from typing import Awaitable
+    from typing import Callable
+    from typing import Dict
+    from typing import List
+    from typing import Optional
+    from typing import Set
+    from typing import Type
+    from typing import Union
+
     from .server import EsbonioLanguageServer
 
+    ConfigurationCallback = Callable[
+        ["ConfigChangeEvent"], Union[Awaitable[None], None]
+    ]
+
+
 try:
     import tomllib as toml
 except ImportError:
     import tomli as toml  # type: ignore[no-redef]
 
-T = TypeVar("T")
-
 
 @attrs.define(frozen=True)
 class Subscription(Generic[T]):
     """Represents a configuration subscription"""
 
     section: str
     """The configuration section."""
 
     spec: Type[T]
     """The subscription's class definition."""
 
-    callback: Callable[[T], Union[Awaitable[None], None]]
+    callback: ConfigurationCallback
     """The subscription's callback."""
 
     workspace_scope: str
     """The corresponding workspace scope for the subscription."""
 
     file_scope: str
     """The corresponding file scope for the subscription."""
 
 
+@attrs.define
+class ConfigChangeEvent(Generic[T]):
+    """Is sent to subscribers when a configuration change occurs."""
+
+    scope: str
+    """The scope at which this configuration change occured."""
+
+    value: T
+    """The latest configuration value."""
+
+    previous: Optional[T] = None
+    """The previous configuration value, (if any)."""
+
+
 class Configuration:
     """Manages the configuration values for the server.
 
     This will looks configuration in the following locations, in descending order of
     priority.
 
     - The server's ``initializationOptions``
@@ -87,14 +110,17 @@
 
         self._file_config: Dict[str, Dict[str, Any]] = {}
         """The cached configuration coming from configuration files."""
 
         self._subscriptions: Dict[Subscription, Any] = {}
         """Subscriptions and their last known value"""
 
+        self._tasks: Set[asyncio.Task] = set()
+        """Holds tasks that are currently executing an async config handler."""
+
     @property
     def initialization_options(self):
         return self._initialization_options
 
     @initialization_options.setter
     def initialization_options(self, value):
         """Ensure the init options are namespaced."""
@@ -117,19 +143,19 @@
     @property
     def supports_workspace_config(self):
         """Indicates if the client supports ``workspace/configuration`` requests."""
         return get_capability(
             self.server.client_capabilities, "workspace.configuration", False
         )
 
-    async def subscribe(
+    def subscribe(
         self,
         section: str,
         spec: Type[T],
-        callback: Callable[[T], Union[Awaitable[None], None]],
+        callback: ConfigurationCallback,
         scope: Optional[Uri] = None,
     ):
         """Subscribe to updates to the given configuration section.
 
         Parameters
         ----------
         section
@@ -150,30 +176,20 @@
             section, spec, callback, workspace_scope, file_scope
         )
 
         if subscription in self._subscriptions:
             self.logger.debug("Ignoring duplicate subscription: %s", subscription)
             return
 
-        # Wait until the server is ready before fetching the initial configuration
-        await self.server.ready
-
-        result = self.get(section, spec, scope)
-        self._subscriptions[subscription] = result
+        self._subscriptions[subscription] = None
 
-        try:
-            ret = callback(result)
-            if inspect.isawaitable(ret):
-                await ret
-        except Exception:
-            self.logger.error(
-                "Error in configuration callback: %s", callback, exc_info=True
-            )
+        # Once the server is ready, update all the subscriptions
+        self.server.ready.add_done_callback(self._notify_subscriptions)
 
-    async def _notify_subscriptions(self):
+    def _notify_subscriptions(self, *args):
         """Notify subscriptions about configuration changes, if necessary."""
 
         for subscription, previous_value in self._subscriptions.items():
             value = self._get_config(
                 subscription.section,
                 subscription.spec,
                 subscription.workspace_scope,
@@ -182,27 +198,48 @@
 
             # No need to notify if nothing has changed
             self.logger.debug("Previous: %s", previous_value)
             self.logger.debug("Current: %s", value)
             if previous_value == value:
                 continue
 
+            self._subscriptions[subscription] = value
+            change_event = ConfigChangeEvent(
+                scope=max(
+                    [subscription.file_scope, subscription.workspace_scope], key=len
+                ),
+                value=value,
+                previous=previous_value,
+            )
+            self.logger.info("%s", change_event)
+
             try:
-                ret = subscription.callback(value)
-                if inspect.isawaitable(ret):
-                    await ret
+                ret = subscription.callback(change_event)
+                if inspect.iscoroutine(ret):
+                    task = asyncio.create_task(ret)
+                    task.add_done_callback(partial(self._finish_task, subscription))
 
-                self._subscriptions[subscription] = value
             except Exception:
                 self.logger.error(
                     "Error in configuration callback: %s",
                     subscription.callback,
                     exc_info=True,
                 )
 
+    def _finish_task(self, subscription: Subscription, task: asyncio.Task[None]):
+        """Cleanup a finished task."""
+        self._tasks.discard(task)
+
+        if (exc := task.exception()) is not None:
+            self.logger.error(
+                "Error in async configuration handler '%s'\n%s",
+                subscription.callback,
+                "".join(traceback.format_exception(type(exc), exc, exc.__traceback__)),
+            )
+
     def get(self, section: str, spec: Type[T], scope: Optional[Uri] = None) -> T:
         """Get the requested configuration section.
 
         Parameters
         ----------
         section
            The configuration section to retrieve
@@ -219,14 +256,33 @@
            The requested configuration section parsed as an instance of ``T``.
         """
         file_scope = self._uri_to_file_scope(scope)
         workspace_scope = self._uri_to_workspace_scope(scope)
 
         return self._get_config(section, spec, workspace_scope, file_scope)
 
+    def scope_for(self, uri: Uri) -> str:
+        """Return the configuration scope that corresponds to the given uri.
+
+        Parameters
+        ----------
+        uri
+           The uri to return the scope for
+
+        Returns
+        -------
+        str
+           The scope corresponding with the given uri
+        """
+
+        file_scope = self._uri_to_file_scope(uri)
+        workspace_scope = self._uri_to_workspace_scope(uri)
+
+        return max([file_scope, workspace_scope], key=len)
+
     def _get_config(
         self, section: str, spec: Type[T], workspace_scope: str, file_scope: str
     ) -> T:
         """Get the requested configuration section."""
 
         self.logger.debug("File scope: '%s'", file_scope)
         self.logger.debug("Workspace scope: '%s'", workspace_scope)
@@ -289,17 +345,15 @@
             self.logger.debug("Scanning workspace folder: '%s'", folder_path)
             for p in pathlib.Path(folder_path).glob("**/pyproject.toml"):
                 self.logger.debug("Found '%s'", p)
                 paths.append(p)
 
         return paths
 
-    async def update_file_configuration(
-        self, paths: Optional[List[pathlib.Path]] = None
-    ):
+    def update_file_configuration(self, paths: Optional[List[pathlib.Path]] = None):
         """Update the internal cache of configuration coming from files.
 
         Parameters
         ----------
         paths
            A list of filepaths to read from.
            If not set, this method will scan each workspace folder for relevant files.
@@ -318,15 +372,15 @@
                     "File '%s' configuration: %s", scope, json.dumps(config, indent=2)
                 )
             except Exception:
                 self.logger.error(
                     "Unable to read configuration file: '%s'", exc_info=True
                 )
 
-        await self._notify_subscriptions()
+        self._notify_subscriptions()
 
     async def update_workspace_configuration(self):
         """Update the internal cache of the client's workspace configuration."""
         if not self.supports_workspace_config:
             return
 
         # Request configuration at the global scope, and at each workspace.
@@ -359,15 +413,15 @@
             result = result or {}
 
             if "esbonio" not in result:
                 result = dict(esbonio=result)
 
             self._workspace_config[scope or ""] = result
 
-        await self._notify_subscriptions()
+        self._notify_subscriptions()
 
 
 def _uri_to_scope(known_scopes: List[str], uri: Optional[Uri]) -> str:
     """Convert the given uri to a scope or the empty string if none could be found.
 
     Parameters
     ----------
```

### Comparing `esbonio-1.0.0b1/esbonio/server/feature.py` & `esbonio-1.0.0b2/esbonio/server/feature.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,19 @@
     ]
 
     DocumentSymbolResult = Union[
         Optional[List[types.DocumentSymbol]],
         Coroutine[Any, Any, Optional[List[types.DocumentSymbol]]],
     ]
 
+    MaybeAsyncNone = Union[
+        None,
+        Coroutine[Any, Any, None],
+    ]
+
     WorkspaceSymbolResult = Union[
         Optional[List[types.WorkspaceSymbol]],
         Coroutine[Any, Any, Optional[List[types.WorkspaceSymbol]]],
     ]
 
 
 class LanguageFeature:
@@ -47,30 +52,37 @@
     def converter(self):
         return self.server.converter
 
     @property
     def configuration(self):
         return self.server.configuration
 
-    def initialize(self, params: types.InitializeParams):
+    def initialize(self, params: types.InitializeParams) -> MaybeAsyncNone:
         """Called during ``initialize``."""
 
-    def initialized(self, params: types.InitializedParams):
+    def initialized(self, params: types.InitializedParams) -> MaybeAsyncNone:
         """Called when the ``initialized`` notification is received."""
 
-    def document_change(self, params: types.DidChangeTextDocumentParams):
+    def shutdown(self, params: None) -> MaybeAsyncNone:
+        """Called when the server is instructed to ``shutdown`` by the client."""
+
+    def document_change(
+        self, params: types.DidChangeTextDocumentParams
+    ) -> MaybeAsyncNone:
         """Called when a text document is changed."""
 
-    def document_close(self, params: types.DidCloseTextDocumentParams):
+    def document_close(
+        self, params: types.DidCloseTextDocumentParams
+    ) -> MaybeAsyncNone:
         """Called when a text document is closed."""
 
-    def document_open(self, params: types.DidOpenTextDocumentParams):
+    def document_open(self, params: types.DidOpenTextDocumentParams) -> MaybeAsyncNone:
         """Called when a text document is opened."""
 
-    def document_save(self, params: types.DidSaveTextDocumentParams):
+    def document_save(self, params: types.DidSaveTextDocumentParams) -> MaybeAsyncNone:
         """Called when a text document is saved."""
 
     completion_triggers: List["re.Pattern"] = []
 
     def completion(self, context: CompletionContext) -> CompletionResult:
         """Called when a completion request matches one of the specified triggers."""
```

### Comparing `esbonio-1.0.0b1/esbonio/server/server.py` & `esbonio-1.0.0b2/esbonio/server/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import collections
 import inspect
 import logging
+import platform
+import traceback
 import typing
 from typing import TypeVar
 from uuid import uuid4
 
 import cattrs
 from lsprotocol import types
 from pygls.capabilities import get_capability
@@ -17,23 +19,25 @@
 
 from . import Uri
 from ._configuration import Configuration
 
 if typing.TYPE_CHECKING:
     from typing import Any
     from typing import Callable
+    from typing import Coroutine
     from typing import Dict
     from typing import List
     from typing import Optional
+    from typing import Set
     from typing import Tuple
     from typing import Type
 
     from .feature import LanguageFeature
 
-__version__ = "1.0.0b1"
+__version__ = "1.0.0b2"
 T = TypeVar("T")
 LF = TypeVar("LF", bound="LanguageFeature")
 
 
 class EsbonioWorkspace(Workspace):
     """A modified version of pygls' workspace that ensures uris are always resolved."""
 
@@ -78,14 +82,17 @@
 
         self._features: Dict[Type[LanguageFeature], LanguageFeature] = {}
         """The collection of language features registered with the server."""
 
         self._ready: asyncio.Future[bool] = asyncio.Future()
         """Indicates if the server is ready."""
 
+        self._tasks: Set[asyncio.Task] = set()
+        """Used to hold running tasks"""
+
         self.logger = logger or logging.getLogger(__name__)
         """The logger instance to use."""
 
         self.configuration = Configuration(self)
         """Manages the fetching of configuration values."""
 
     def __iter__(self):
@@ -96,37 +103,67 @@
         return self._ready
 
     @property
     def converter(self) -> cattrs.Converter:
         """The cattrs converter instance we should use."""
         return self.lsp._converter
 
+    def _finish_task(self, task: asyncio.Task[Any]):
+        """Cleanup a finished task."""
+        self.logger.debug("Task finished: %s", task)
+        self._tasks.discard(task)
+
+        if (exc := task.exception()) is not None:
+            self.logger.error(
+                "Error in async task\n%s",
+                traceback.format_exception(type(exc), exc, exc.__traceback__),
+            )
+
+    def run_task(self, coro: Coroutine, *, name: Optional[str] = None) -> asyncio.Task:
+        """Convert a given coroutine into a task and ensure it is executed."""
+
+        task = asyncio.create_task(coro, name=name)
+        self.logger.debug("Scheduled task: %s", task)
+        task.add_done_callback(self._finish_task)
+
+        self._tasks.add(task)
+        return task
+
     def initialize(self, params: types.InitializeParams):
-        self.logger.info("Initialising esbonio v%s", __version__)
+        self.logger.info(
+            "Initialising esbonio v%s, using Python v%s on %s",
+            __version__,
+            platform.python_version(),
+            platform.platform(aliased=True, terse=True),
+        )
         if (client := params.client_info) is not None:
             self.logger.info("Language client: %s %s", client.name, client.version)
 
         # TODO: Propose patch to pygls for providing custom Workspace implementations.
         self.lsp._workspace = EsbonioWorkspace(
             self.workspace.root_uri,
             self.workspace._sync_kind,
             list(self.workspace.folders.values()),
         )
 
         self.configuration.initialization_options = params.initialization_options
 
     async def initialized(self, params: types.InitializedParams):
+        self.configuration.update_file_configuration()
+
         await asyncio.gather(
             self.configuration.update_workspace_configuration(),
-            self.configuration.update_file_configuration(),
             self._register_did_change_configuration_handler(),
             self._register_did_change_watched_files_handler(),
         )
         self._ready.set_result(True)
 
+    def lsp_shutdown(self, params: None):
+        """Called when the server is instructed to ``shutdown`` by the client."""
+
     def load_extension(self, name: str, setup: Callable):
         """Load the given setup function as an extension.
 
         If an extension with the given ``name`` already exists, the given setup function
         will be ignored.
 
         The ``setup`` function can declare dependencies in the form of type
```

### Comparing `esbonio-1.0.0b1/esbonio/server/setup.py` & `esbonio-1.0.0b2/esbonio/server/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,19 @@
     @server.feature(types.INITIALIZED)
     async def on_initialized(
         ls: EsbonioLanguageServer, params: types.InitializedParams
     ):
         await ls.initialized(params)
         await call_features(ls, "initialized", params)
 
+    @server.feature(types.SHUTDOWN)
+    async def on_shutdown(ls: EsbonioLanguageServer, params: None):
+        ls.lsp_shutdown(params)
+        await call_features(ls, "shutdown", params)
+
     @server.feature(types.TEXT_DOCUMENT_DID_CHANGE)
     async def on_document_change(
         ls: EsbonioLanguageServer, params: types.DidChangeTextDocumentParams
     ):
         await call_features(ls, "document_change", params)
 
     @server.feature(types.TEXT_DOCUMENT_DID_CLOSE)
```

### Comparing `esbonio-1.0.0b1/esbonio/server/features/directives/__init__.py` & `esbonio-1.0.0b2/esbonio/server/features/directives/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,25 +59,27 @@
         provider
            The directive provider
         """
         self._providers[id(provider)] = provider
 
     completion_triggers = [RST_DIRECTIVE, MYST_DIRECTIVE]
 
-    async def initialized(self, params: types.InitializedParams):
+    def initialized(self, params: types.InitializedParams):
         """Called once the initial handshake between client and server has finished."""
-        await self.configuration.subscribe(
+        self.configuration.subscribe(
             "esbonio.server.completion",
             server.CompletionConfig,
             self.update_configuration,
         )
 
-    def update_configuration(self, config: server.CompletionConfig):
+    def update_configuration(
+        self, event: server.ConfigChangeEvent[server.CompletionConfig]
+    ):
         """Called when the user's configuration is updated."""
-        self._insert_behavior = config.preferred_insert_behavior
+        self._insert_behavior = event.value.preferred_insert_behavior
 
     async def completion(
         self, context: server.CompletionContext
     ) -> Optional[List[types.CompletionItem]]:
         """Provide auto-completion suggestions for directives."""
 
         groups = context.match.groupdict()
```

### Comparing `esbonio-1.0.0b1/esbonio/server/features/preview_manager/__init__.py` & `esbonio-1.0.0b2/esbonio/server/features/preview_manager/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import asyncio
 import logging
+import sys
 from http.server import HTTPServer
 from http.server import SimpleHTTPRequestHandler
 from typing import Any
 from typing import Dict
 from typing import Optional
 from urllib.parse import urlencode
 
 import attrs
 
 from esbonio.server import EsbonioLanguageServer
 from esbonio.server import Uri
 from esbonio.server.feature import LanguageFeature
+from esbonio.server.features.project_manager import ProjectManager
 from esbonio.server.features.sphinx_manager import SphinxClient
 from esbonio.server.features.sphinx_manager import SphinxManager
 
 from .webview import WebviewServer
 from .webview import make_ws_server
 
 
@@ -75,27 +77,48 @@
     show_line_markers: bool = attrs.field(default=False)
     """If set, render the source line markers in the preview"""
 
 
 class PreviewManager(LanguageFeature):
     """Language feature for managing previews."""
 
-    def __init__(self, server: EsbonioLanguageServer, sphinx: SphinxManager):
+    def __init__(
+        self,
+        server: EsbonioLanguageServer,
+        sphinx: SphinxManager,
+        projects: ProjectManager,
+    ):
         super().__init__(server)
         self.sphinx = sphinx
         self.sphinx.add_listener("build", self.on_build)
 
+        self.projects = projects
+
         logger = server.logger.getChild("PreviewServer")
         self._request_handler_factory = RequestHandlerFactory(logger)
         self._http_server: Optional[HTTPServer] = None
         self._http_future: Optional[asyncio.Future] = None
 
         self._ws_server: Optional[WebviewServer] = None
         self._ws_task: Optional[asyncio.Task] = None
 
+    def shutdown(self, params: None):
+        """Called when the client instructs the server to ``shutdown``."""
+        args = {}
+        if sys.version_info.minor > 8:
+            args["msg"] = "Server is shutting down."
+
+        if self._http_server:
+            self.logger.debug("Shutting down preview HTTP server")
+            self._http_server.shutdown()
+
+        if self._ws_task:
+            self.logger.debug("Shutting down preview WebSocket server")
+            self._ws_task.cancel(**args)
+
     @property
     def preview_active(self) -> bool:
         """Return true if the preview is active.
 
         i.e. there is a HTTP server hosting the build result."""
         return self._http_server is not None
 
@@ -180,26 +203,21 @@
         self._ws_server.scroll(line)
 
     async def preview_file(self, params):
         # Always check the fully resolved uri.
         src_uri = Uri.parse(params["uri"]).resolve()
         self.logger.debug("Previewing file: '%s'", src_uri)
 
-        client = await self.sphinx.get_client(src_uri)
-        if client is None:
+        if (client := await self.sphinx.get_client(src_uri)) is None:
             return None
 
-        if client.builder not in {"html", "dirhtml"}:
-            self.logger.error(
-                "Previews for the '%s' builder are not currently supported",
-                client.builder,
-            )
+        if (project := self.projects.get_project(src_uri)) is None:
             return None
 
-        if (build_path := await client.get_build_path(src_uri)) is None:
+        if (build_path := await project.get_build_path(src_uri)) is None:
             self.logger.debug(
                 "Unable to preview file '%s', not included in build output.", src_uri
             )
             return None
 
         config = await self.get_preview_config()
         server = await self.get_http_server(config)
@@ -218,16 +236,18 @@
             query=urlencode(query_params),
         )
 
         self.logger.info("Preview available at: %s", uri.as_string(encode=False))
         return {"uri": uri.as_string(encode=False)}
 
 
-def esbonio_setup(server: EsbonioLanguageServer, sphinx: SphinxManager):
-    manager = PreviewManager(server, sphinx)
+def esbonio_setup(
+    server: EsbonioLanguageServer, sphinx: SphinxManager, projects: ProjectManager
+):
+    manager = PreviewManager(server, sphinx, projects)
     server.add_feature(manager)
 
     @server.feature("view/scroll")
     async def on_scroll(ls: EsbonioLanguageServer, params):
         await manager.scroll_view(params.line)
 
     @server.command("esbonio.server.previewFile")
```

### Comparing `esbonio-1.0.0b1/esbonio/server/features/preview_manager/webview.py` & `esbonio-1.0.0b2/esbonio/server/features/preview_manager/webview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """This module implements the websocket server used to communicate with preivew
  windows."""
+
 import asyncio
 import json
 import logging
 import socket
 from typing import Optional
 
 from pygls.protocol import JsonRPCProtocol
```

### Comparing `esbonio-1.0.0b1/esbonio/server/features/sphinx_manager/client_subprocess.py` & `esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/client_subprocess.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 """Subprocess implementation of the ``SphinxClient`` protocol."""
+
 from __future__ import annotations
 
 import asyncio
-import json
 import logging
 import os
+import pathlib
 import subprocess
+import sys
 import typing
+from uuid import uuid4
 
-import aiosqlite
 from pygls.client import JsonRPCClient
 from pygls.protocol import JsonRPCProtocol
 
 import esbonio.sphinx_agent.types as types
+from esbonio.server import EventSource
 from esbonio.server import Uri
 
+from .client import ClientState
 from .config import SphinxConfig
 
 if typing.TYPE_CHECKING:
     from typing import Any
     from typing import Dict
     from typing import List
     from typing import Optional
-    from typing import Tuple
 
     from .client import SphinxClient
     from .manager import SphinxManager
 
 
+sphinx_logger = logging.getLogger("sphinx")
+
+
 class SphinxAgentProtocol(JsonRPCProtocol):
     """Describes the protocol spoken between the client below and the sphinx agent."""
 
     def get_message_type(self, method: str) -> Any | None:
         return types.METHOD_TO_MESSAGE_TYPE.get(method, None)
 
     def get_result_type(self, method: str) -> Any | None:
@@ -43,86 +49,122 @@
     a separate subprocess.
 
     See :mod:`esbonio.sphinx_agent` for the implementation of the server component.
     """
 
     def __init__(
         self,
+        config: SphinxConfig,
         logger: Optional[logging.Logger] = None,
         protocol_cls=SphinxAgentProtocol,
         *args,
         **kwargs,
     ):
         super().__init__(protocol_cls=protocol_cls, *args, **kwargs)  # type: ignore[misc]
+
+        self.id = str(uuid4())
+        """The client's id."""
+
+        self.config = config
+        """Configuration values."""
+
         self.logger = logger or logging.getLogger(__name__)
+        """The logger instance to use."""
 
         self.sphinx_info: Optional[types.SphinxInfo] = None
+        """Information about the Sphinx application the client is connected to."""
 
-        self._connection: Optional[aiosqlite.Connection] = None
-        self._building = False
+        self.state: Optional[ClientState] = None
+        """The current state of the client."""
 
-    @property
-    def converter(self):
-        return self.protocol._converter
+        self.exception: Optional[Exception] = None
+        """The most recently encountered exception (if any)"""
 
-    @property
-    def id(self) -> Optional[str]:
-        """The id of the Sphinx instance."""
-        if self.sphinx_info is None:
-            return None
+        self._events = EventSource(self.logger)
+        """The sphinx client can emit events."""
+
+        self._startup_task: Optional[asyncio.Task] = None
+        """The startup task."""
+
+        self._stderr_forwarder: Optional[asyncio.Task] = None
+        """A task that forwards the server's stderr to the test process."""
+
+    def __repr__(self):
+        if self.state is None:
+            return "SphinxClient<None>"
+
+        if self.state == ClientState.Errored:
+            return f"SphinxClient<{self.state.name}: {self.exception}>"
 
-        return self.sphinx_info.id
+        state = self.state.name
+        command = " ".join(self.config.build_command)
+        return f"SphinxClient<{state}: {command}>"
+
+    def __await__(self):
+        """Makes the client await-able"""
+        if self._startup_task is None:
+            self._startup_task = asyncio.create_task(self.start())
+
+        return self._startup_task.__await__()
 
     @property
-    def building(self) -> bool:
-        return self._building
+    def converter(self):
+        return self.protocol._converter
 
     @property
-    def builder(self) -> Optional[str]:
+    def builder(self) -> str:
         """The sphinx application's builder name"""
         if self.sphinx_info is None:
-            return None
+            raise RuntimeError("sphinx_info is None, has the client been started?")
 
         return self.sphinx_info.builder_name
 
     @property
-    def src_uri(self) -> Optional[Uri]:
+    def src_uri(self) -> Uri:
         """The src uri of the Sphinx application."""
         if self.sphinx_info is None:
-            return None
+            raise RuntimeError("sphinx_info is None, has the client been started?")
 
         return Uri.for_file(self.sphinx_info.src_dir)
 
     @property
-    def conf_uri(self) -> Optional[Uri]:
+    def conf_uri(self) -> Uri:
         """The conf uri of the Sphinx application."""
         if self.sphinx_info is None:
-            return None
+            raise RuntimeError("sphinx_info is None, has the client been started?")
 
         return Uri.for_file(self.sphinx_info.conf_dir)
 
     @property
-    def db(self) -> Optional[aiosqlite.Connection]:
+    def db(self) -> pathlib.Path:
         """Connection to the associated database."""
-        return self._connection
+        if self.sphinx_info is None:
+            raise RuntimeError("sphinx_info is None, has the client been started?")
+
+        return pathlib.Path(self.sphinx_info.dbpath)
 
     @property
-    def build_uri(self) -> Optional[Uri]:
+    def build_uri(self) -> Uri:
         """The build uri of the Sphinx application."""
         if self.sphinx_info is None:
-            return None
+            raise RuntimeError("sphinx_info is None, has the client been started?")
 
         return Uri.for_file(self.sphinx_info.build_dir)
 
+    def add_listener(self, event: str, handler):
+        self._events.add_listener(event, handler)
+
     async def server_exit(self, server: asyncio.subprocess.Process):
         """Called when the sphinx agent process exits."""
 
         #   0: all good
         # -15: terminated
         if server.returncode not in {0, -15}:
+            self.exception = RuntimeError(server.returncode)
+            self._set_state(ClientState.Errored)
             self.logger.error(
                 f"sphinx-agent process exited with code: {server.returncode}"
             )
 
             if server.stderr is not None:
                 stderr = await server.stderr.read()
                 self.logger.error("Stderr:\n%s", stderr.decode("utf8"))
@@ -131,73 +173,79 @@
         # Cancel any pending futures.
         for id_, fut in self.protocol._request_futures.items():
             message = "Cancelled" if fut.cancel() else "Unable to cancel"
             self.logger.debug(
                 "%s future '%s' for pending request '%s'", message, fut, id_
             )
 
-    async def start(self, config: SphinxConfig):
-        """Start the client."""
+        if self.state != ClientState.Errored:
+            self._set_state(ClientState.Exited)
 
-        if len(config.python_command) == 0:
-            raise ValueError("No python environment configured")
+    async def start_io(self, cmd: str, *args, **kwargs):
+        await super().start_io(cmd, *args, **kwargs)
 
-        command = []
+        # Forward the server's stderr to this process' stderr
+        if self._server and self._server.stderr:
+            self._stderr_forwarder = asyncio.create_task(forward_stderr(self._server))
 
-        if config.enable_dev_tools and (
-            lsp_devtools := self._get_lsp_devtools_command()
-        ):
-            command.extend([lsp_devtools, "agent", "--"])
+    async def start(self) -> SphinxClient:
+        """Start the client."""
 
-        command.extend([*config.python_command, "-m", "sphinx_agent"])
-        env = get_sphinx_env(config)
+        # Only try starting once.
+        if self.state is not None:
+            return self
 
-        self.logger.debug("Starting sphinx agent: %s", " ".join(command))
-        await self.start_io(*command, env=env, cwd=config.cwd)
+        try:
+            self._set_state(ClientState.Starting)
+            command = get_start_command(self.config, self.logger)
+            env = get_sphinx_env(self.config)
+
+            self.logger.debug("Starting sphinx agent: %s", " ".join(command))
+            await self.start_io(*command, env=env, cwd=self.config.cwd)
+
+            params = types.CreateApplicationParams(
+                command=self.config.build_command,
+                enable_sync_scrolling=self.config.enable_sync_scrolling,
+            )
 
-    def _get_lsp_devtools_command(self) -> Optional[str]:
-        # Assumes that the user has `lsp-devtools` available on their PATH
-        # TODO: Windows support
-        result = subprocess.run(["command", "-v", "lsp-devtools"], capture_output=True)
-        if result.returncode == 0:
-            lsp_devtools = result.stdout.decode("utf8").strip()
-            return lsp_devtools
+            self.sphinx_info = await self.protocol.send_request_async(
+                "sphinx/createApp", params
+            )
 
-        stderr = result.stderr.decode("utf8").strip()
-        self.logger.debug("Unable to locate lsp-devtools command", stderr)
-        return None
+            self._set_state(ClientState.Running)
+            return self
+        except Exception as exc:
+            self.logger.debug("Unable to start SphinxClient: %s", exc, exc_info=True)
+
+            self.exception = exc
+            self._set_state(ClientState.Errored)
+
+            return self
+
+    def _set_state(self, new_state: ClientState):
+        """Change the state of the client."""
+        old_state, self.state = self.state, new_state
+
+        self.logger.debug("SphinxClient[%s]: %s -> %s", self.id, old_state, new_state)
+        self._events.trigger("state-change", self, old_state, new_state)
 
     async def stop(self):
         """Stop the client."""
 
-        self.protocol.notify("exit", None)
-        if self._connection:
-            await self._connection.close()
+        if self.state in {ClientState.Running, ClientState.Building}:
+            self.protocol.notify("exit", None)
 
         # Give the agent a little time to close.
-        # await asyncio.sleep(0.5)
-        await super().stop()
-
-    async def create_application(self, config: SphinxConfig) -> types.SphinxInfo:
-        """Create a sphinx application object."""
-
-        params = types.CreateApplicationParams(
-            command=config.build_command,
-            enable_sync_scrolling=config.enable_sync_scrolling,
-        )
-
-        sphinx_info = await self.protocol.send_request_async("sphinx/createApp", params)
-        self.sphinx_info = sphinx_info
+        await asyncio.sleep(0.5)
 
-        try:
-            self._connection = await aiosqlite.connect(sphinx_info.dbpath)
-        except Exception:
-            self.logger.error("Unable to connect to database", exc_info=True)
+        if self._stderr_forwarder:
+            self._stderr_forwarder.cancel()
 
-        return sphinx_info
+        self.logger.debug(self._async_tasks)
+        await super().stop()
 
     async def build(
         self,
         *,
         filenames: Optional[List[str]] = None,
         force_all: bool = False,
         content_overrides: Optional[Dict[str, str]] = None,
@@ -214,192 +262,106 @@
         try:
             result = await self.protocol.send_request_async("sphinx/build", params)
         finally:
             self._building = False
 
         return result
 
-    async def get_src_uris(self) -> List[Uri]:
-        """Return all known source uris."""
-
-        if self.db is None:
-            return []
-
-        query = "SELECT uri FROM files"
-        async with self.db.execute(query) as cursor:
-            results = await cursor.fetchall()
-            return [Uri.parse(s[0]) for s in results]
-
-    async def get_build_path(self, src_uri: Uri) -> Optional[str]:
-        """Get the build path associated with the given ``src_uri``."""
-
-        if self.db is None:
-            return None
-
-        query = "SELECT urlpath FROM files WHERE uri = ?"
-        async with self.db.execute(query, (str(src_uri.resolve()),)) as cursor:
-            if (result := await cursor.fetchone()) is None:
-                return None
-
-            return result[0]
-
-    async def get_config_value(self, name: str) -> Optional[Any]:
-        """Return the requested configuration value, if available."""
-        if self.db is None:
-            return None
-
-        query = "SELECT value FROM config WHERE name = ?"
-        cursor = await self.db.execute(query, (name,))
 
-        if (row := await cursor.fetchone()) is None:
-            return None
+async def forward_stderr(server: asyncio.subprocess.Process):
+    if server.stderr is None:
+        return
+
+    # EOF is signalled with an empty bytestring
+    while (line := await server.stderr.readline()) != b"":
+        sphinx_logger.info(line.decode())
 
-        (value,) = row
-        return json.loads(value)
-
-    async def get_directives(self) -> List[Tuple[str, Optional[str]]]:
-        """Get the directives known to Sphinx."""
-        if self.db is None:
-            return []
-
-        query = "SELECT name, implementation FROM directives"
-        cursor = await self.db.execute(query)
-        return await cursor.fetchall()  # type: ignore[return-value]
-
-    async def get_document_symbols(self, src_uri: Uri) -> List[types.Symbol]:
-        """Get the symbols for the given file."""
-        if self.db is None:
-            return []
-
-        query = (
-            "SELECT id, name, kind, detail, range, parent_id, order_id "
-            "FROM symbols WHERE uri = ?"
-        )
-        cursor = await self.db.execute(query, (str(src_uri.resolve()),))
-        return await cursor.fetchall()  # type: ignore[return-value]
-
-    async def find_symbols(self, **kwargs) -> List[types.Symbol]:
-        """Find symbols which match the given criteria."""
-        if self.db is None:
-            return []
-
-        base_query = (
-            "SELECT id, name, kind, detail, range, parent_id, order_id FROM symbols"
-        )
-        where: List[str] = []
-        parameters: List[Any] = []
-
-        for param, value in kwargs.items():
-            where.append(f"{param} = ?")
-            parameters.append(value)
-
-        if where:
-            conditions = " AND ".join(where)
-            query = " ".join([base_query, "WHERE", conditions])
-        else:
-            query = base_query
 
-        cursor = await self.db.execute(query, tuple(parameters))
-        return await cursor.fetchall()  # type: ignore[return-value]
-
-    async def get_workspace_symbols(
-        self, query: str
-    ) -> List[Tuple[str, str, int, str, str, str]]:
-        """Return all the workspace symbols matching the given query string"""
-
-        if self.db is None:
-            return []
-
-        sql_query = """\
-SELECT
-    child.uri,
-    child.name,
-    child.kind,
-    child.detail,
-    child.range,
-    COALESCE(parent.name, '') AS container_name
-FROM
-    symbols child
-LEFT JOIN
-    symbols parent ON (child.parent_id = parent.id AND child.uri = parent.uri)
-WHERE
-    child.name like ? or child.detail like ?;"""
-
-        query_str = f"%{query}%"
-        cursor = await self.db.execute(sql_query, (query_str, query_str))
-        return await cursor.fetchall()  # type: ignore[return-value]
-
-    async def get_diagnostics(self) -> Dict[Uri, List[Dict[str, Any]]]:
-        """Get diagnostics for the project."""
-        if self.db is None:
-            return {}
-
-        cursor = await self.db.execute("SELECT * FROM diagnostics")
-        results: Dict[Uri, List[Dict[str, Any]]] = {}
-
-        for uri_str, item in await cursor.fetchall():
-            uri = Uri.parse(uri_str)
-            diagnostic = json.loads(item)
-            results.setdefault(uri, []).append(diagnostic)
-
-        return results
-
-
-def make_subprocess_sphinx_client(manager: SphinxManager) -> SphinxClient:
+def make_subprocess_sphinx_client(
+    manager: SphinxManager, config: SphinxConfig
+) -> SphinxClient:
     """Factory function for creating a ``SubprocessSphinxClient`` instance.
 
     Parameters
     ----------
     manager
        The manager instance creating the client
 
+    config
+       The Sphinx configuration
+
     Returns
     -------
     SphinxClient
        The configured client
     """
-    client = SubprocessSphinxClient(logger=manager.logger)
+    client = SubprocessSphinxClient(config, logger=manager.logger)
 
     @client.feature("window/logMessage")
     def _on_msg(ls: SubprocessSphinxClient, params):
-        manager.server.show_message_log(params.message)
+        sphinx_logger.info(params.message)
 
     @client.feature("$/progress")
     def _on_progress(ls: SubprocessSphinxClient, params):
         manager.report_progress(ls, params)
 
     return client
 
 
-def make_test_sphinx_client() -> SubprocessSphinxClient:
+def make_test_sphinx_client(config: SphinxConfig) -> SubprocessSphinxClient:
     """Factory function for creating a ``SubprocessSphinxClient`` instance
     to use for testing."""
     logger = logging.getLogger("sphinx_client")
     logger.setLevel(logging.INFO)
 
-    client = SubprocessSphinxClient()
+    client = SubprocessSphinxClient(config)
 
     @client.feature("window/logMessage")
     def _(params):
-        logger.info("%s", params.message)
+        print(params.message, file=sys.stderr)
 
     @client.feature("$/progress")
     def _on_progress(params):
         logger.info("%s", params)
 
     return client
 
 
 def get_sphinx_env(config: SphinxConfig) -> Dict[str, str]:
     """Return the set of environment variables to use with the Sphinx process."""
 
     env = {
+        "PYTHONUNBUFFERED": "1",
         "PYTHONPATH": os.pathsep.join([str(p) for p in config.python_path]),
     }
     for envname, value in os.environ.items():
         # Don't pass any vars we've explictly set.
         if envname in env:
             continue
 
         env[envname] = value
 
     return env
+
+
+def get_start_command(config: SphinxConfig, logger: logging.Logger):
+    """Return the command to use to start the sphinx agent."""
+
+    command = []
+
+    if len(config.python_command) == 0:
+        raise ValueError("No python environment configured")
+
+    if config.enable_dev_tools:
+        # Assumes that the user has `lsp-devtools` available on their PATH
+        # TODO: Windows support
+        result = subprocess.run(["command", "-v", "lsp-devtools"], capture_output=True)
+        if result.returncode == 0:
+            lsp_devtools = result.stdout.decode("utf8").strip()
+            command.extend([lsp_devtools, "agent", "--"])
+
+        else:
+            stderr = result.stderr.decode("utf8").strip()
+            logger.debug("Unable to locate lsp-devtools command", stderr)
+
+    command.extend([*config.python_command, "-m", "sphinx_agent"])
+    return command
```

### Comparing `esbonio-1.0.0b1/esbonio/server/features/sphinx_manager/config.py` & `esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -137,37 +137,39 @@
            The working directory to launch the sphinx agent in.
            If ``None``, the working directory could not be determined.
         """
 
         if self.cwd:
             return self.cwd
 
-        for folder_uri in workspace.folders.keys():
-            folder_uri = Uri.parse(folder_uri)
-            if folder_uri and str(uri).startswith(str(folder_uri)):
-                break
-        else:
-            folder_uri = Uri.parse(workspace.root_uri)
-
-        if folder_uri is None or (cwd := folder_uri.fs_path) is None:
-            logger.error("Unable to determine working directory from '%s'", folder_uri)
-            return None
+        candidates = [Uri.parse(f) for f in workspace.folders.keys()]
 
-        return cwd
+        if workspace.root_uri is not None:
+            if (root_uri := Uri.parse(workspace.root_uri)) not in candidates:
+                candidates.append(root_uri)
+
+        for folder in candidates:
+            if str(uri).startswith(str(folder)):
+                if (cwd := folder.fs_path) is None:
+                    logger.error(
+                        "Unable to determine working directory from '%s'", folder
+                    )
+                    return None
+
+                return cwd
+
+        return None
 
     def _resolve_python_path(self, logger: logging.Logger) -> List[pathlib.Path]:
         """Return the list of paths to put on the sphinx agent's ``PYTHONPATH``
 
         Using the ``PYTHONPATH`` environment variable, we can inject additional Python
         packages into the user's Python environment. This method will locate the
         installation path of the sphinx agent and return it.
 
-        Additionally if the ``enable_dev_tools`` flag is set, this will attempt to
-        locate the ``lsp_devtools`` package
-
         Parameters
         ----------
         logger
            The logger instance to use
 
         Returns
         -------
```

### Comparing `esbonio-1.0.0b1/esbonio/server/features/sphinx_manager/manager.py` & `esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,126 @@
 from __future__ import annotations
 
 import asyncio
-import inspect
+import traceback
 import typing
 import uuid
-from typing import Callable
-from typing import Dict
-from typing import Optional
+from functools import partial
 
+import attrs
 import lsprotocol.types as lsp
 
-import esbonio.sphinx_agent.types as types
-from esbonio.server import LanguageFeature
+from esbonio import server
 from esbonio.server import Uri
+from esbonio.sphinx_agent import types
 
+from .client import ClientState
 from .config import SphinxConfig
 
 if typing.TYPE_CHECKING:
+    from typing import Callable
+    from typing import Dict
+    from typing import Optional
+
+    from esbonio.server.features.project_manager import ProjectManager
+
     from .client import SphinxClient
 
+    SphinxClientFactory = Callable[["SphinxManager", "SphinxConfig"], "SphinxClient"]
+
+
+@attrs.define
+class ClientCreatedNotification:
+    """The payload of a ``sphinx/clientCreated`` notification"""
+
+    id: str
+    """The client's id"""
+
+    scope: str
+    """The scope at which the client was created."""
+
+    config: SphinxConfig
+    """The final configuration."""
+
+
+@attrs.define
+class AppCreatedNotification:
+    """The payload of a ``sphinx/appCreated`` notification"""
+
+    id: str
+    """The client's id"""
+
+    application: types.SphinxInfo
+    """Details about the created application."""
+
+
+@attrs.define
+class ClientErroredNotification:
+    """The payload of a ``sphinx/clientErrored`` notification"""
 
-SphinxClientFactory = Callable[["SphinxManager"], "SphinxClient"]
+    id: str
+    """The client's id"""
 
+    error: str
+    """Short description of the error."""
 
-class SphinxManager(LanguageFeature):
+    detail: str
+    """Detailed description of the error."""
+
+
+@attrs.define
+class ClientDestroyedNotification:
+    """The payload of ``sphinx/clientDestroyed`` notification."""
+
+    id: str
+    """The client's id"""
+
+
+class SphinxManager(server.LanguageFeature):
     """Responsible for managing Sphinx application instances."""
 
-    def __init__(self, client_factory: SphinxClientFactory, *args, **kwargs):
+    def __init__(
+        self,
+        client_factory: SphinxClientFactory,
+        project_manager: ProjectManager,
+        *args,
+        **kwargs,
+    ):
         super().__init__(*args, **kwargs)
 
         self.client_factory = client_factory
         """Used to create new Sphinx client instances."""
 
-        self.clients: Dict[Uri, SphinxClient] = {}
+        self.project_manager = project_manager
+        """The project manager instance to use."""
+
+        self.clients: Dict[str, Optional[SphinxClient]] = {
+            # Prevent any clients from being created in the global scope.
+            "": None,
+        }
         """Holds currently active Sphinx clients."""
 
-        self.handlers: Dict[str, set] = {}
-        """Collection of handlers for various events."""
+        self._events = server.EventSource(self.logger)
+        """The SphinxManager can emit events."""
 
         self._pending_builds: Dict[str, asyncio.Task] = {}
         """Holds tasks that will trigger a build after a given delay if not cancelled."""
 
-        self._client_creating: Optional[asyncio.Task] = None
-        """If set, indicates we're in the process of setting up a new client."""
-
         self._progress_tokens: Dict[str, str] = {}
         """Holds work done progress tokens."""
 
     def add_listener(self, event: str, handler):
-        self.handlers.setdefault(event, set()).add(handler)
+        self._events.add_listener(event, handler)
 
     async def document_change(self, params: lsp.DidChangeTextDocumentParams):
         if (uri := Uri.parse(params.text_document.uri)) is None:
             return
 
         client = await self.get_client(uri)
-        if client is None or client.id is None:
+        if client is None:
             return
 
         # Cancel any existing pending builds
         if (task := self._pending_builds.pop(client.id, None)) is not None:
             task.cancel()
 
         self._pending_builds[client.id] = asyncio.create_task(
@@ -73,181 +134,199 @@
             await self.get_client(uri)
 
     async def document_save(self, params: lsp.DidSaveTextDocumentParams):
         if (uri := Uri.parse(params.text_document.uri)) is None:
             return
 
         client = await self.get_client(uri)
-        if client is None or client.id is None:
+        if client is None:
             return
 
         # Cancel any existing pending builds
         if (task := self._pending_builds.pop(client.id, None)) is not None:
             task.cancel()
 
         await self.trigger_build(uri)
 
+    async def shutdown(self, params: None):
+        """Called when the server is instructed to ``shutdown``."""
+
+        # Stop any existing clients.
+        tasks = []
+        for client in self.clients.values():
+            if client:
+                self.logger.debug("Stopping SphinxClient: %s", client)
+                tasks.append(asyncio.create_task(client.stop()))
+
+        await asyncio.gather(*tasks)
+
     async def trigger_build_after(self, uri: Uri, app_id: str, delay: float):
         """Trigger a build for the given uri after the given delay."""
         await asyncio.sleep(delay)
 
         self._pending_builds.pop(app_id)
         self.logger.debug("Triggering build")
         await self.trigger_build(uri)
 
     async def trigger_build(self, uri: Uri):
         """Trigger a build for the relevant Sphinx application for the given uri."""
+
         client = await self.get_client(uri)
-        if client is None or client.building:
+        if client is None or client.state != ClientState.Running:
+            return
+
+        if (project := self.project_manager.get_project(uri)) is None:
             return
 
         # Pass through any unsaved content to the Sphinx agent.
         content_overrides: Dict[str, str] = {}
-        known_src_uris = await client.get_src_uris()
+        known_src_uris = await project.get_src_uris()
 
         for src_uri in known_src_uris:
             doc = self.server.workspace.get_document(str(src_uri))
             doc_version = doc.version or 0
             saved_version = getattr(doc, "saved_version", 0)
 
-            if saved_version < doc_version and (fs_path := src_uri.fs_path) is not None:
-                content_overrides[fs_path] = doc.source
+            if saved_version < doc_version:
+                content_overrides[str(src_uri)] = doc.source
 
         await self.start_progress(client)
 
         try:
             result = await client.build(content_overrides=content_overrides)
         except Exception as exc:
             self.server.show_message(f"{exc}", lsp.MessageType.Error)
             return
         finally:
             self.stop_progress(client)
 
         # Notify listeners.
-        for listener in self.handlers.get("build", set()):
-            try:
-                # TODO: Concurrent awaiting?
-                res = listener(client, result)
-                if inspect.isawaitable(res):
-                    await res
-            except Exception:
-                name = f"{listener}"
-                self.logger.error("Error in build handler '%s'", name, exc_info=True)
+        self._events.trigger("build", client, result)
 
     async def get_client(self, uri: Uri) -> Optional[SphinxClient]:
         """Given a uri, return the relevant sphinx client instance for it."""
 
-        # Wait until the new client is created - it might be the one we're looking for!
-        if self._client_creating:
-            await self._client_creating
-
-        # Always check the fully resolved uri.
-        resolved_uri = uri.resolve()
-
-        for src_uri, client in self.clients.items():
-            if resolved_uri in (await client.get_src_uris()):
-                return client
-
-            # For now assume a single client instance per srcdir.
-            # This *should* prevent us from spwaning endless client instances
-            # when given a file located near a valid Sphinx project - but not actually
-            # part of it.
-            in_src_dir = str(resolved_uri).startswith(str(src_uri))
-            if in_src_dir:
-                # Of course, we can only tell if a uri truly is not in a project
-                # when the build file map is populated!
-                # if len(client.build_file_map) == 0:
-                return client
-
-        # Create a new client instance.
-        self._client_creating = asyncio.create_task(self._create_client(uri))
-        try:
-            return await self._client_creating
-        finally:
-            # Be sure to unset the task when it resolves
-            self._client_creating = None
-
-    async def _create_client(self, uri: Uri) -> Optional[SphinxClient]:
-        """Create a new sphinx client instance."""
-        # TODO: Replace with config subscription
-        await self.server.ready
-        config = self.server.configuration.get(
-            "esbonio.sphinx", SphinxConfig, scope=uri
-        )
-        if config is None:
+        scope = self.server.configuration.scope_for(uri)
+        if scope not in self.clients:
+            self.logger.debug("No client found, creating new subscription")
+            self.server.configuration.subscribe(
+                "esbonio.sphinx",
+                SphinxConfig,
+                self._create_or_replace_client,
+                scope=uri,
+            )
+            # The first few callers in a given scope will miss out, but that shouldn't matter
+            # too much
             return None
 
-        resolved = config.resolve(uri, self.server.workspace, self.logger)
-        if resolved is None:
+        if (client := self.clients[scope]) is None:
+            self.logger.debug("No applicable client for uri: %s", uri)
             return None
 
-        client = self.client_factory(self)
+        return await client
 
-        try:
-            await client.start(resolved)
-        except Exception as exc:
-            message = "Unable to start sphinx-agent"
-            self.logger.error(message, exc_info=True)
-            self.server.show_message(f"{message}: {exc}", lsp.MessageType.Error)
+    async def _create_or_replace_client(
+        self, event: server.ConfigChangeEvent[SphinxConfig]
+    ):
+        """Create or replace thesphinx client instance for the given config."""
 
-            return None
+        config = event.value
 
-        try:
-            sphinx_info = await client.create_application(resolved)
-        except Exception as exc:
-            message = "Unable to create sphinx application"
-            self.logger.error(message, exc_info=True)
-            self.server.show_message(f"{message}: {exc}", lsp.MessageType.Error)
+        # Do not try and create clients in the global scope
+        if event.scope == "":
+            return
 
-            await client.stop()
-            return None
+        # If there was a previous client, stop it.
+        if (previous_client := self.clients.pop(event.scope, None)) is not None:
+            self.server.lsp.notify(
+                "sphinx/clientDestroyed",
+                ClientDestroyedNotification(id=previous_client.id),
+            )
+            self.server.run_task(previous_client.stop())
 
-        if client.src_uri is None:
-            self.logger.error("No src uri!")
-            await client.stop()
-            return None
+        resolved = config.resolve(
+            Uri.parse(event.scope), self.server.workspace, self.logger
+        )
+        if resolved is None:
+            self.clients[event.scope] = None
+            return
+
+        self.clients[event.scope] = client = self.client_factory(self, resolved)
+        client.add_listener("state-change", partial(self._on_state_change, event.scope))
+
+        self.server.lsp.notify(
+            "sphinx/clientCreated",
+            ClientCreatedNotification(id=client.id, scope=event.scope, config=resolved),
+        )
+        self.logger.debug("Client created for scope %s", event.scope)
+
+        # Start the client
+        await client
 
-        self.server.lsp.notify("sphinx/appCreated", sphinx_info)
-        self.clients[client.src_uri] = client
-        return client
+    def _on_state_change(
+        self,
+        scope: str,
+        client: SphinxClient,
+        old_state: ClientState,
+        new_state: ClientState,
+    ):
+        """React to state changes in the client."""
+
+        if old_state == ClientState.Starting and new_state == ClientState.Running:
+            if (sphinx_info := client.sphinx_info) is not None:
+                self.project_manager.register_project(scope, client.db)
+                self.server.lsp.notify(
+                    "sphinx/appCreated",
+                    AppCreatedNotification(id=client.id, application=sphinx_info),
+                )
+
+        if new_state == ClientState.Errored:
+            error = ""
+            detail = ""
+
+            if (exc := getattr(client, "exception", None)) is not None:
+                error = f"{type(exc).__name__}: {exc}"
+                detail = "".join(
+                    traceback.format_exception(type(exc), exc, exc.__traceback__)
+                )
+
+            self.server.lsp.show_message(error, lsp.MessageType.Error)
+            self.server.lsp.notify(
+                "sphinx/clientErrored",
+                ClientErroredNotification(id=client.id, error=error, detail=detail),
+            )
 
     async def start_progress(self, client: SphinxClient):
         """Start reporting work done progress for the given client."""
 
-        if client.id is None:
-            return
-
         token = str(uuid.uuid4())
-        self.logger.error("Starting progress: '%s'", token)
+        self.logger.debug("Starting progress: '%s'", token)
 
         try:
             await self.server.progress.create_async(token)
         except Exception as exc:
             self.logger.debug("Unable to create progress token: %s", exc)
             return
 
         self._progress_tokens[client.id] = token
         self.server.progress.begin(
             token,
             lsp.WorkDoneProgressBegin(title="sphinx-build", cancellable=False),
         )
 
     def stop_progress(self, client: SphinxClient):
-        if client.id is None:
-            return
-
         if (token := self._progress_tokens.pop(client.id, None)) is None:
             return
 
         self.server.progress.end(token, lsp.WorkDoneProgressEnd(message="Finished"))
 
     def report_progress(self, client: SphinxClient, progress: types.ProgressParams):
         """Report progress done for the given client."""
 
-        if client.id is None:
+        if client.state not in {ClientState.Running, ClientState.Building}:
             return
 
         if (token := self._progress_tokens.get(client.id, None)) is None:
             return
 
         self.server.progress.report(
             token,
```

### Comparing `esbonio-1.0.0b1/esbonio/server/features/sphinx_support/directives.py` & `esbonio-1.0.0b2/esbonio/server/features/sphinx_support/directives.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,51 +2,51 @@
 
 import typing
 
 from lsprotocol import types
 
 from esbonio import server
 from esbonio.server.features import directives
-from esbonio.server.features.sphinx_manager import SphinxManager
+from esbonio.server.features.project_manager import ProjectManager
 
 if typing.TYPE_CHECKING:
     from typing import List
     from typing import Optional
 
 
 class SphinxDirectives(directives.DirectiveProvider):
     """Support for directives in a sphinx project."""
 
-    def __init__(self, manager: SphinxManager):
+    def __init__(self, manager: ProjectManager):
         self.manager = manager
 
     async def suggest_directives(
         self, context: server.CompletionContext
     ) -> Optional[List[directives.Directive]]:
         """Given a completion context, suggest directives that may be used."""
 
-        if (client := await self.manager.get_client(context.uri)) is None:
+        if (project := self.manager.get_project(context.uri)) is None:
             return None
 
         # Does the document have a default domain set?
-        results = await client.find_symbols(
+        results = await project.find_symbols(
             uri=str(context.uri.resolve()),
             kind=types.SymbolKind.Class.value,
             detail="default-domain",
         )
         if len(results) > 0:
             default_domain = results[0][1]
         else:
             default_domain = None
 
-        primary_domain = await client.get_config_value("primary_domain")
+        primary_domain = await project.get_config_value("primary_domain")
         active_domain = default_domain or primary_domain or "py"
 
         result: List[directives.Directive] = []
-        for name, implementation in await client.get_directives():
+        for name, implementation in await project.get_directives():
             # std: directives can be used unqualified
             if name.startswith("std:"):
                 short_name = name.replace("std:", "")
                 result.append(
                     directives.Directive(name=short_name, implementation=implementation)
                 )
 
@@ -61,12 +61,12 @@
                 directives.Directive(name=name, implementation=implementation)
             )
 
         return result
 
 
 def esbonio_setup(
-    sphinx_manager: SphinxManager,
+    project_manager: ProjectManager,
     directive_feature: directives.DirectiveFeature,
 ):
-    provider = SphinxDirectives(sphinx_manager)
+    provider = SphinxDirectives(project_manager)
     directive_feature.add_provider(provider)
```

### Comparing `esbonio-1.0.0b1/esbonio/server/features/sphinx_support/symbols.py` & `esbonio-1.0.0b2/esbonio/server/features/sphinx_support/symbols.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 from typing import Optional
 
 from lsprotocol import types
 
 from esbonio.server import EsbonioLanguageServer
 from esbonio.server import LanguageFeature
 from esbonio.server import Uri
-from esbonio.server.features.sphinx_manager import SphinxManager
+from esbonio.server.features.project_manager import ProjectManager
 
 
 class SphinxSymbols(LanguageFeature):
     """Add support for ``textDocument/documentSymbol`` requests"""
 
-    def __init__(self, server: EsbonioLanguageServer, manager: SphinxManager):
+    def __init__(self, server: EsbonioLanguageServer, manager: ProjectManager):
         super().__init__(server)
         self.manager = manager
 
     async def document_symbol(
         self, params: types.DocumentSymbolParams
     ) -> Optional[List[types.DocumentSymbol]]:
         """Called when a document symbols request is received."""
 
         uri = Uri.parse(params.text_document.uri)
-        if (client := await self.manager.get_client(uri)) is None:
+        if (project := self.manager.get_project(uri)) is None:
             return None
 
-        symbols = await client.get_document_symbols(uri)
+        symbols = await project.get_document_symbols(uri)
         if len(symbols) == 0:
             return None
 
         root: List[types.DocumentSymbol] = []
         index: Dict[int, types.DocumentSymbol] = {}
 
         for id_, name, kind, detail, range_json, parent_id, _ in symbols:
@@ -60,17 +60,17 @@
 
     async def workspace_symbol(
         self, params: types.WorkspaceSymbolParams
     ) -> Optional[List[types.WorkspaceSymbol]]:
         """Called when a workspace symbol request is received."""
 
         tasks = []
-        for client in self.manager.clients.values():
+        for project in self.manager.projects.values():
             tasks.append(
-                asyncio.create_task(client.get_workspace_symbols(params.query))
+                asyncio.create_task(project.get_workspace_symbols(params.query))
             )
 
         symbols = await asyncio.gather(*tasks)
         result: List[types.WorkspaceSymbol] = []
 
         for batch in symbols:
             for uri_str, name, kind, detail, range_json, container in batch:
@@ -90,10 +90,10 @@
                         container_name=container,
                     )
                 )
 
         return result
 
 
-def esbonio_setup(server: EsbonioLanguageServer, sphinx_manager: SphinxManager):
-    symbols = SphinxSymbols(server, sphinx_manager)
+def esbonio_setup(server: EsbonioLanguageServer, project_manager: ProjectManager):
+    symbols = SphinxSymbols(server, project_manager)
     server.add_feature(symbols)
```

### Comparing `esbonio-1.0.0b1/esbonio/sphinx_agent/__init__.py` & `esbonio-1.0.0b2/esbonio/sphinx_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/esbonio/sphinx_agent/config.py` & `esbonio-1.0.0b2/esbonio/sphinx_agent/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import dataclasses
 import inspect
 import pathlib
+import sys
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
 from typing import Optional
 from typing import Union
 from unittest import mock
@@ -148,13 +149,13 @@
             "confoverrides": self.config_overrides,
             "doctreedir": str(doctree_dir),
             "freshenv": self.force_full_build,
             "keep_going": self.keep_going,
             "outdir": str(build_dir),
             "parallel": self.parallel,
             "srcdir": str(src_dir),
-            "status": None,
+            "status": sys.stderr,
             "tags": self.tags,
             "verbosity": self.verbosity,
-            "warning": None,
+            "warning": sys.stderr,
             "warningiserror": self.warning_is_error,
         }
```

### Comparing `esbonio-1.0.0b1/esbonio/sphinx_agent/database.py` & `esbonio-1.0.0b2/esbonio/sphinx_agent/database.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/esbonio/sphinx_agent/log.py` & `esbonio-1.0.0b2/esbonio/sphinx_agent/log.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,46 @@
+from __future__ import annotations
+
 import inspect
 import logging
 import os
 import pathlib
 import sys
-from types import ModuleType
-from typing import Any
-from typing import Dict
-from typing import List
-from typing import Optional
-from typing import Set
-from typing import Tuple
-from typing import Union
-
-from sphinx.util.logging import OnceFilter
-from sphinx.util.logging import SphinxLogRecord
-from sphinx.util.logging import WarningLogRecordTranslator
+import typing
 
 from . import types
+from .types import Uri
 from .util import logger
-from .util import send_message
+
+if typing.TYPE_CHECKING:
+    from types import ModuleType
+    from typing import Any
+    from typing import Dict
+    from typing import List
+    from typing import Optional
+    from typing import Set
+    from typing import Tuple
+    from typing import Union
+
 
 DIAGNOSTIC_SEVERITY = {
     logging.ERROR: types.DiagnosticSeverity.Error,
     logging.INFO: types.DiagnosticSeverity.Information,
     logging.WARNING: types.DiagnosticSeverity.Warning,
 }
 
 
-class SphinxLogHandler(logging.Handler):
+class DiagnosticFilter(logging.Filter):
     """A logging handler that can extract errors from Sphinx's build output."""
 
     def __init__(self, app, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.app = app
-        self.translator = WarningLogRecordTranslator(app)
-        self.only_once = OnceFilter()
-        self.diagnostics: Dict[str, Set[types.Diagnostic]] = {}
+        self.diagnostics: Dict[Uri, Set[types.Diagnostic]] = {}
 
     def get_location(self, location: str) -> Tuple[str, Optional[int]]:
         if not location:
             conf = pathlib.Path(self.app.confdir, "conf.py")
             return (str(conf), None)
 
         lineno = None
@@ -101,35 +101,24 @@
             # Correct off by one error for docstrings that don't start with a newline.
             nl = (obj.__doc__ or "").startswith("\n")
             return line + int(offset) - (not nl)
         except Exception:
             logger.debug("Unable to determine diagnostic location\n%s", exc_info=True)
             return None
 
-    def emit(self, record: logging.LogRecord) -> None:
+    def filter(self, record: logging.LogRecord) -> bool:
         conditions = [
             "sphinx" not in record.name,
             record.levelno not in {logging.WARNING, logging.ERROR},
         ]
 
         if any(conditions):
-            # Log the record as normal
-            self.do_emit(record)
-            return
-
-        # Let sphinx extract location info for warning/error messages
-        self.translator.filter(record)  # type: ignore
-
-        # Only process errors/warnings once.
-        # Note: This isn't a silver bullet as it only catches messages that are explicitly
-        #       marked as to be logged only once e.g. logger.warning(..., once=True).
-        if not self.only_once.filter(record):
-            return
+            return True
 
-        loc = record.location if isinstance(record, SphinxLogRecord) else ""
+        loc = getattr(record, "location", "")
         doc, lineno = self.get_location(loc)
         line = lineno or 1
 
         try:
             # Not every message contains a string...
             if not isinstance(record.msg, str):
                 message = str(record.msg)
@@ -151,13 +140,9 @@
             ),
             message=message,
             severity=DIAGNOSTIC_SEVERITY.get(
                 record.levelno, types.DiagnosticSeverity.Warning
             ),
         )
 
-        self.diagnostics.setdefault(doc, set()).add(diagnostic)
-        self.do_emit(record)
-
-    def do_emit(self, record):
-        params = types.LogMessageParams(message=self.format(record).strip(), type=4)
-        send_message(types.LogMessage(params=params))
+        self.diagnostics.setdefault(Uri.for_file(doc), set()).add(diagnostic)
+        return True
```

### Comparing `esbonio-1.0.0b1/esbonio/sphinx_agent/patches.py` & `esbonio-1.0.0b2/esbonio/sphinx_agent/patches.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/esbonio/sphinx_agent/server.py` & `esbonio-1.0.0b2/esbonio/sphinx_agent/server.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/esbonio/sphinx_agent/types.py` & `esbonio-1.0.0b2/esbonio/sphinx_agent/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Type definitions for the sphinx agent.
 
 This is the *only* file shared between the agent itself and the parent language server.
 For this reason this file *cannot* import anything from Sphinx.
 """
+
 import dataclasses
 import enum
 import os
 import pathlib
 import re
 from typing import Callable
 from typing import Dict
@@ -211,14 +212,49 @@
             raise ValueError("Paths with an authority must start with a slash '/'")
 
         if self.path and self.path.startswith("//") and (not self.authority):
             raise ValueError(
                 "Paths without an authority cannot start with two slashes '//'"
             )
 
+    def __eq__(self, other):
+        if type(other) is not type(self):
+            return False
+
+        if self.scheme != other.scheme:
+            return False
+
+        if self.authority != other.authority:
+            return False
+
+        if self.query != other.query:
+            return False
+
+        if self.fragment != other.fragment:
+            return False
+
+        if IS_WIN and self.scheme == "file":
+            # Filepaths on windows are case in-sensitive
+            if self.path.lower() != other.path.lower():
+                return False
+
+        elif self.path != other.path:
+            return False
+
+        return True
+
+    def __hash__(self):
+        if IS_WIN and self.scheme == "file":
+            # Filepaths on windows are case in-sensitive
+            path = self.path.lower()
+        else:
+            path = self.path
+
+        return hash((self.scheme, self.authority, path, self.query, self.fragment))
+
     def __fspath__(self):
         """Return the file system representation of this uri.
 
         This makes Uri instances compatible with any function that expects an
         ``os.PathLike`` object!
         """
         # TODO: Should we raise an exception if scheme != "file"?
@@ -529,17 +565,14 @@
     jsonrpc: str = dataclasses.field(default="2.0")
 
 
 @dataclasses.dataclass
 class SphinxInfo:
     """Represents information about an instance of the Sphinx application."""
 
-    id: str
-    """A unique id representing a particular Sphinx application instance."""
-
     version: str
     """The version of Sphinx being used."""
 
     conf_dir: str
     """The folder containing the project's conf.py"""
 
     build_dir: str
```

### Comparing `esbonio-1.0.0b1/esbonio/sphinx_agent/util.py` & `esbonio-1.0.0b2/esbonio/sphinx_agent/util.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/esbonio/sphinx_agent/handlers/__init__.py` & `esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 import inspect
 import logging
 import os.path
 import pathlib
 import sys
 import traceback
 import typing
-from functools import partial
-from typing import IO
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
-from uuid import uuid4
 
 import sphinx.application
 from sphinx import __version__ as __sphinx_version__
-from sphinx.util import console
-from sphinx.util import logging as sphinx_logging_module
 from sphinx.util.logging import NAMESPACE as SPHINX_LOG_NAMESPACE
-from sphinx.util.logging import VERBOSITY_MAP
 
 from .. import types
 from ..app import Sphinx
 from ..config import SphinxConfig
-from ..log import SphinxLogHandler
 from ..transforms import LineNumberTransform
+from ..types import Uri
 from ..util import send_error
 from ..util import send_message
 
 STATIC_DIR = (pathlib.Path(__file__).parent.parent / "static").resolve()
 sphinx_logger = logging.getLogger(SPHINX_LOG_NAMESPACE)
 
 # Inject our own 'core' extensions into Sphinx
@@ -45,15 +39,15 @@
 class SphinxHandler:
     """Responsible for implementing the JSON-RPC API exposed by the Sphinx agent."""
 
     def __init__(self):
         self.app: Optional[Sphinx] = None
         """The sphinx application instance"""
 
-        self._content_overrides: Dict[pathlib.Path, str] = {}
+        self._content_overrides: Dict[Uri, str] = {}
         """Holds any additional content to inject into a build."""
 
         self._handlers: Dict[str, Tuple[Type, Callable]] = self._register_handlers()
 
     def get(self, method: str) -> Optional[Tuple[Type, Callable]]:
         """Return the handler for the given method - if possible.
 
@@ -116,17 +110,14 @@
     def create_sphinx_app(self, request: types.CreateApplicationRequest):
         """Create a new sphinx application instance."""
         sphinx_config = SphinxConfig.fromcli(request.params.command)
         if sphinx_config is None:
             raise ValueError("Invalid build command")
 
         sphinx_args = sphinx_config.to_application_args()
-
-        # Override Sphinx's logging setup with our own.
-        sphinx_logging_module.setup = partial(self.setup_logging, sphinx_config)
         self.app = Sphinx(**sphinx_args)
 
         # Connect event handlers.
         self.app.connect("env-before-read-docs", self._cb_env_before_read_docs)
         self.app.connect("source-read", self._cb_source_read, priority=0)
 
         # TODO: Sphinx 7.x has introduced a `include-read` event
@@ -134,15 +125,14 @@
 
         if request.params.enable_sync_scrolling:
             _enable_sync_scrolling(self.app)
 
         response = types.CreateApplicationResponse(
             id=request.id,
             result=types.SphinxInfo(
-                id=str(uuid4()),
                 version=__sphinx_version__,
                 conf_dir=str(self.app.confdir),
                 build_dir=str(self.app.outdir),
                 builder_name=self.app.builder.name,
                 src_dir=str(self.app.srcdir),
                 dbpath=str(self.app.esbonio.db.path),
             ),
@@ -152,65 +142,34 @@
 
     def _cb_env_before_read_docs(self, app: Sphinx, env, docnames: List[str]):
         """Used to add additional documents to the "to build" list."""
 
         is_building = set(docnames)
 
         for docname in env.found_docs - is_building:
-            filepath = pathlib.Path(env.doc2path(docname, base=True))
-            if filepath in self._content_overrides:
+            uri = Uri.for_file(env.doc2path(docname, base=True))
+            if uri in self._content_overrides:
                 docnames.append(docname)
 
     def _cb_source_read(self, app: Sphinx, docname: str, source):
         """Called whenever sphinx reads a file from disk."""
 
-        filepath = app.env.doc2path(docname, base=True)
-
-        # Override file contents if necessary
-        path = pathlib.Path(filepath)
-        if (content := self._content_overrides.get(path)) is not None:
+        uri = Uri.for_file(app.env.doc2path(docname, base=True))
+        if (content := self._content_overrides.get(uri, None)) is not None:
             source[0] = content
 
-    def setup_logging(self, config: SphinxConfig, app: Sphinx, status: IO, warning: IO):
-        """Setup Sphinx's logging so that it integrates well with the parent language
-        server."""
-
-        # Disable color escape codes in Sphinx's log messages
-        console.nocolor()
-
-        if not config.silent:
-            # Be sure to remove any old handlers
-            for handler in sphinx_logger.handlers:
-                if isinstance(handler, SphinxLogHandler):
-                    sphinx_logger.handlers.remove(handler)
-                    self.log_handler = None
-
-            app.esbonio.log = SphinxLogHandler(app)
-            sphinx_logger.addHandler(app.esbonio.log)
-
-            if config.quiet:
-                level = logging.WARNING
-            else:
-                level = VERBOSITY_MAP[app.verbosity]
-
-            sphinx_logger.setLevel(level)
-            app.esbonio.log.setLevel(level)
-
-            formatter = logging.Formatter("%(message)s")
-            app.esbonio.log.setFormatter(formatter)
-
     def build_sphinx_app(self, request: types.BuildRequest):
         """Trigger a Sphinx build."""
 
         if self.app is None:
             send_error(id=request.id, code=-32803, message="Sphinx app not initialized")
             return
 
         self._content_overrides = {
-            pathlib.Path(p): content
+            Uri.parse(p): content
             for p, content in request.params.content_overrides.items()
         }
 
         try:
             self.app.build()
 
             response = types.BuildResponse(
@@ -222,14 +181,17 @@
         except Exception as exc:
             message = "".join(traceback.format_exception_only(type(exc), exc))
             sphinx_logger.error("sphinx-build failed", exc_info=True)
             send_error(
                 id=request.id, code=-32603, message=f"sphinx-build failed: {message}"
             )
 
+        finally:
+            self.app._warncount = 0
+
     def notify_exit(self, request: types.ExitNotification):
         """Sent from the client to signal that the agent should exit."""
         sys.exit(0)
 
 
 def _enable_sync_scrolling(app: Sphinx):
     """Given a Sphinx application, configure it so that we can support syncronised
```

### Comparing `esbonio-1.0.0b1/esbonio/sphinx_agent/handlers/diagnostics.py` & `esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/diagnostics.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,28 +18,27 @@
 
 def init_db(app: Sphinx, config: Config):
     app.esbonio.db.ensure_table(DIAGNOSTICS_TABLE)
 
 
 def clear_diagnostics(app: Sphinx, docname: str, source):
     """Clear the diagnostics assocated with the given file."""
-    filepath = app.env.doc2path(docname, base=True)
-    app.esbonio.log.diagnostics.pop(filepath, None)
+    uri = Uri.for_file(app.env.doc2path(docname, base=True))
+    app.esbonio.log.diagnostics.pop(uri, None)
 
 
 def sync_diagnostics(app: Sphinx, exc: Optional[Exception]):
     app.esbonio.db.clear_table(DIAGNOSTICS_TABLE)
 
     results = []
     diagnostics = app.esbonio.log.diagnostics
 
-    for fpath, items in diagnostics.items():
-        uri = str(Uri.for_file(fpath).resolve())
+    for uri, items in diagnostics.items():
         for item in items:
-            results.append((uri, as_json(item)))
+            results.append((str(uri), as_json(item)))
 
     app.esbonio.db.insert_values(DIAGNOSTICS_TABLE, results)
 
 
 def setup(app: Sphinx):
     app.connect("config-inited", init_db)
     app.connect("source-read", clear_diagnostics)
```

### Comparing `esbonio-1.0.0b1/esbonio/sphinx_agent/handlers/files.py` & `esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/files.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/esbonio/sphinx_agent/handlers/symbols.py` & `esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,19 +294,17 @@
         self.push_symbol(name, ClassSymbol, range_, detail=detail)
 
     def depart_a_directive(self, node: nodes.Node):
         self.pop_symbol()
 
     # TODO: Enable symbols for roles
     #       However the reported line numbers can be inaccurate...
-    def visit_a_role(self, node: nodes.Node) -> None:
-        ...
+    def visit_a_role(self, node: nodes.Node) -> None: ...
 
-    def depart_a_role(self, node: nodes.Node) -> None:
-        ...
+    def depart_a_role(self, node: nodes.Node) -> None: ...
 
     # TODO: Enable symbols for definition list items
     #       However the reported line numbers appear to be inaccurate...
 
     def visit_Text(self, node: nodes.Node) -> None:
         pass
```

### Comparing `esbonio-1.0.0b1/esbonio/sphinx_agent/static/webview.js` & `esbonio-1.0.0b2/esbonio/sphinx_agent/static/webview.js`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/tests/e2e/conftest.py` & `esbonio-1.0.0b2/tests/e2e/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 ),
                 # Signal workDoneProgress/create support.
                 window=types.WindowClientCapabilities(
                     work_done_progress=True,
                 ),
             ),
             initialization_options={
-                "server": {"logLevel": "debug"},
+                "logging": {"level": "debug"},
                 "sphinx": {
                     "buildCommand": [
                         "sphinx-build",
                         "-M",
                         "html",
                         workspace_uri.fs_path,
                         str(build_dir),
```

### Comparing `esbonio-1.0.0b1/tests/e2e/test_e2e_diagnostics.py` & `esbonio-1.0.0b2/tests/e2e/test_e2e_diagnostics.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,57 +7,76 @@
 from pytest_lsp import ClientServerConfig
 from pytest_lsp import LanguageClient
 
 SERVER_CMD = ["-m", "esbonio"]
 TEST_DIR = pathlib.Path(__file__).parent.parent
 
 
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_document_diagnostic(pull_client: LanguageClient, uri_for):
-    """Ensure that we can get the diagnostics for a single document correctly."""
+@pytest.mark.asyncio(scope="session")
+async def test_rst_document_diagnostic(client: LanguageClient, uri_for):
+    """Ensure that we can get the diagnostics for a single rst document correctly."""
 
-    workspace_uri = uri_for("sphinx-default", "workspace")
-    test_uri = workspace_uri / "definitions.rst"
+    workspace_uri = uri_for("workspaces", "demo")
+    test_uri = workspace_uri / "rst" / "diagnostics.rst"
     report = await client.text_document_diagnostic_async(
         types.DocumentDiagnosticParams(
             text_document=types.TextDocumentIdentifier(uri=str(test_uri))
         )
     )
 
     assert report.kind == "full"
 
     # We will only check the diagnostic message, full details will be handled by other
     # test cases.
     messages = {d.message for d in report.items}
     assert messages == {
-        "image file not readable: _static/bad.png",
-        "unknown document: '/changelog'",
+        "image file not readable: not-an-image.png",
     }
 
     assert len(client.diagnostics) == 0, "Server should not publish diagnostics"
 
 
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_workspace_diagnostic(pull_client: LanguageClient, uri_for):
+@pytest.mark.asyncio(scope="session")
+async def test_myst_document_diagnostic(client: LanguageClient, uri_for):
+    """Ensure that we can get the diagnostics for a single myst document correctly."""
+
+    workspace_uri = uri_for("workspaces", "demo")
+    test_uri = workspace_uri / "myst" / "diagnostics.md"
+    report = await client.text_document_diagnostic_async(
+        types.DocumentDiagnosticParams(
+            text_document=types.TextDocumentIdentifier(uri=str(test_uri))
+        )
+    )
+
+    assert report.kind == "full"
+
+    # We will only check the diagnostic message, full details will be handled by other
+    # test cases.
+    messages = {d.message for d in report.items}
+    assert messages == {
+        "image file not readable: not-an-image.png",
+    }
+
+    assert len(client.diagnostics) == 0, "Server should not publish diagnostics"
+
+
+@pytest.mark.asyncio(scope="session")
+async def test_workspace_diagnostic(client: LanguageClient, uri_for):
     """Ensure that we can get diagnostics for the whole workspace correctly."""
     report = await client.workspace_diagnostic_async(
         types.WorkspaceDiagnosticParams(previous_result_ids=[])
     )
 
-    workspace_uri = uri_for("sphinx-default", "workspace")
+    workspace_uri = uri_for("workspaces", "demo")
     expected = {
-        str(workspace_uri / "definitions.rst"): {
-            "image file not readable: _static/bad.png",
-            "unknown document: '/changelog'",
+        str(workspace_uri / "rst" / "diagnostics.rst"): {
+            "image file not readable: not-an-image.png",
         },
-        str(workspace_uri / "directive_options.rst"): {
-            "image file not readable: filename.png",
-            "document isn't included in any toctree",
+        str(workspace_uri / "myst" / "diagnostics.md"): {
+            "image file not readable: not-an-image.png",
         },
     }
     assert len(report.items) == len(expected)
     for item in report.items:
         assert expected[item.uri] == {d.message for d in item.items}
 
     assert len(client.diagnostics) == 0, "Server should not publish diagnostics"
@@ -67,41 +86,42 @@
     scope="module",
     config=ClientServerConfig(
         server_command=[sys.executable, *SERVER_CMD],
     ),
 )
 async def pub_client(lsp_client: LanguageClient, uri_for, tmp_path_factory):
     """A client that does **not** support the pull-diagnostics model."""
+
     build_dir = tmp_path_factory.mktemp("build")
-    workspace_uri = uri_for("sphinx-default", "workspace")
-    test_uri = workspace_uri / "definitions.rst"
+    workspace_uri = uri_for("workspaces", "demo")
+    test_uri = workspace_uri / "rst" / "diagnostics.rst"
 
     await lsp_client.initialize_session(
         types.InitializeParams(
             capabilities=types.ClientCapabilities(
                 # Signal workDoneProgress/create support.
                 window=types.WindowClientCapabilities(
                     work_done_progress=True,
                 ),
             ),
             initialization_options={
-                "server": {"logLevel": "debug"},
+                "logging": {"level": "debug"},
                 "sphinx": {
                     "buildCommand": [
                         "sphinx-build",
                         "-M",
                         "html",
                         workspace_uri.fs_path,
                         str(build_dir),
                     ],
                     "pythonCommand": [sys.executable],
                 },
             },
             workspace_folders=[
-                types.WorkspaceFolder(uri=str(workspace_uri), name="sphinx-default"),
+                types.WorkspaceFolder(uri=str(workspace_uri), name="demo"),
             ],
         )
     )
 
     # Open a text document to trigger sphinx client creation.
     lsp_client.text_document_did_open(
         types.DidOpenTextDocumentParams(
@@ -131,27 +151,24 @@
 
     yield
 
     # Teardown
     await lsp_client.shutdown_session()
 
 
-@pytest.mark.asyncio
-@pytest.mark.skip
+@pytest.mark.asyncio(scope="module")
 async def test_publish_diagnostics(pub_client: LanguageClient, uri_for):
     """Ensure that the server publishes the diagnostics it finds"""
-    workspace_uri = uri_for("sphinx-default", "workspace")
+    workspace_uri = uri_for("workspaces", "demo")
     expected = {
-        str(workspace_uri / "definitions.rst"): {
-            "image file not readable: _static/bad.png",
-            "unknown document: '/changelog'",
+        str(workspace_uri / "rst" / "diagnostics.rst"): {
+            "image file not readable: not-an-image.png",
         },
-        str(workspace_uri / "directive_options.rst"): {
-            "image file not readable: filename.png",
-            "document isn't included in any toctree",
+        str(workspace_uri / "myst" / "diagnostics.md"): {
+            "image file not readable: not-an-image.png",
         },
     }
 
     # The server might not have published its diagnostics yet
     while len(pub_client.diagnostics) < len(expected):
         await pub_client.wait_for_notification(types.TEXT_DOCUMENT_PUBLISH_DIAGNOSTICS)
```

### Comparing `esbonio-1.0.0b1/tests/e2e/test_e2e_directives.py` & `esbonio-1.0.0b2/tests/e2e/test_e2e_directives.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/tests/e2e/test_e2e_symbols.py` & `esbonio-1.0.0b2/tests/e2e/test_e2e_symbols.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/tests/server/conftest.py` & `esbonio-1.0.0b2/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/tests/server/test_configuration.py` & `esbonio-1.0.0b2/tests/server/test_configuration.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/tests/server/test_patterns.py` & `esbonio-1.0.0b2/tests/server/test_patterns.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/tests/server/features/test_directive_completion.py` & `esbonio-1.0.0b2/tests/server/features/test_directive_completion.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/tests/sphinx-agent/conftest.py` & `esbonio-1.0.0b2/tests/sphinx-agent/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,60 @@
+import logging
 import sys
 
-import pytest_lsp
+import pytest_asyncio
 from lsprotocol.types import WorkspaceFolder
 from pygls.workspace import Workspace
-from pytest_lsp import ClientServerConfig
 
+from esbonio.server.features.project_manager import Project
+from esbonio.server.features.sphinx_manager.client import ClientState
 from esbonio.server.features.sphinx_manager.client_subprocess import (
     SubprocessSphinxClient,
 )
 from esbonio.server.features.sphinx_manager.client_subprocess import (
     make_test_sphinx_client,
 )
 from esbonio.server.features.sphinx_manager.config import SphinxConfig
 
+logger = logging.getLogger(__name__)
 
-@pytest_lsp.fixture(
-    config=ClientServerConfig(
-        server_command=[sys.executable, "-m", "esbonio.sphinx_agent"],
-        client_factory=make_test_sphinx_client,
-    ),
-)
-async def client(sphinx_client: SubprocessSphinxClient, uri_for, tmp_path_factory):
+
+@pytest_asyncio.fixture
+async def client(uri_for, tmp_path_factory):
     build_dir = tmp_path_factory.mktemp("build")
     demo_workspace = uri_for("workspaces", "demo")
     test_uri = demo_workspace / "index.rst"
 
     workspace = Workspace(
         None,
         workspace_folders=[
-            WorkspaceFolder(uri=str(demo_workspace), name="sphinx-default"),
+            WorkspaceFolder(uri=str(demo_workspace), name="demo"),
         ],
     )
     config = SphinxConfig(
+        python_command=[sys.executable],
         build_command=[
             "sphinx-build",
             "-M",
             "html",
             demo_workspace.fs_path,
             str(build_dir),
         ],
     )
-    resolved = config.resolve(test_uri, workspace, sphinx_client.logger)
+    resolved = config.resolve(test_uri, workspace, logger)
     assert resolved is not None
 
-    info = await sphinx_client.create_application(resolved)
-    assert info is not None
+    sphinx_client = await make_test_sphinx_client(resolved)
+    assert sphinx_client.state == ClientState.Running
 
     await sphinx_client.build()
-    yield
+    yield sphinx_client
+
+    await sphinx_client.stop()
+
+
+@pytest_asyncio.fixture
+async def project(client: SubprocessSphinxClient):
+    project = Project(client.db)
+
+    yield project
+    await project.close()
```

### Comparing `esbonio-1.0.0b1/tests/sphinx-agent/test_app.py` & `esbonio-1.0.0b2/tests/sphinx-agent/test_app.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/tests/sphinx-agent/test_sa_build.py` & `esbonio-1.0.0b2/tests/sphinx-agent/test_sa_build.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+import logging
 import pathlib
 import re
 import sys
 
 import pytest
-import pytest_lsp
+import pytest_asyncio
 from lsprotocol.types import WorkspaceFolder
 from pygls.exceptions import JsonRpcInternalError
 from pygls.workspace import Workspace
-from pytest_lsp import ClientServerConfig
 
+from esbonio.server.features.sphinx_manager.client import ClientState
 from esbonio.server.features.sphinx_manager.client_subprocess import (
     SubprocessSphinxClient,
 )
 from esbonio.server.features.sphinx_manager.client_subprocess import (
     make_test_sphinx_client,
 )
 from esbonio.server.features.sphinx_manager.config import SphinxConfig
 
+logger = logging.getLogger(__name__)
+
 
 @pytest.mark.asyncio
 async def test_build_includes_webview_js(client: SubprocessSphinxClient, uri_for):
     """Ensure that builds include the ``webview.js`` script."""
 
     out = client.build_uri
     src = client.src_uri
@@ -50,66 +53,59 @@
 
     # Before
     expected = "Welcome to the demo documentation"
     index_html = pathlib.Path(out / "index.html")
     assert expected in index_html.read_text()
 
     await client.build(
-        content_overrides={
-            (src / "index.rst").fs_path: "My Custom Title\n==============="
-        }
+        content_overrides={str(src / "index.rst"): "My Custom Title\n==============="}
     )
 
     # Ensure the override was applied
     expected = "My Custom Title"
     print(index_html.read_text())
     assert expected in index_html.read_text()
 
 
-@pytest_lsp.fixture(
-    scope="module",
-    config=ClientServerConfig(
-        server_command=[sys.executable, "-m", "esbonio.sphinx_agent"],
-        client_factory=make_test_sphinx_client,
-    ),
-)
-async def client_build_error(
-    sphinx_client: SubprocessSphinxClient, uri_for, tmp_path_factory
-):
+@pytest_asyncio.fixture(scope="module")
+async def client_build_error(uri_for, tmp_path_factory):
     """A sphinx client that will error when a build is triggered."""
     build_dir = tmp_path_factory.mktemp("build")
     demo_workspace = uri_for("workspaces", "demo")
     test_uri = demo_workspace / "index.rst"
 
     workspace = Workspace(
         None,
         workspace_folders=[
             WorkspaceFolder(uri=str(demo_workspace), name="demo"),
         ],
     )
 
     conf_dir = uri_for("workspaces", "demo-error-build").fs_path
     config = SphinxConfig(
+        python_command=[sys.executable],
         build_command=[
             "sphinx-build",
             "-b",
             "html",
             "-c",
             str(conf_dir),
             demo_workspace.fs_path,
             str(build_dir),
         ],
     )
-    resolved = config.resolve(test_uri, workspace, sphinx_client.logger)
+    resolved = config.resolve(test_uri, workspace, logger)
     assert resolved is not None
 
-    info = await sphinx_client.create_application(resolved)
-    assert info is not None
+    sphinx_client = await make_test_sphinx_client(resolved)
+    assert sphinx_client.state == ClientState.Running
+
+    yield sphinx_client
 
-    yield
+    await sphinx_client.stop()
 
 
 @pytest.mark.asyncio(scope="module")
 async def test_build_error(client_build_error: SubprocessSphinxClient):
     """Ensure that when a build error occurs, useful information is reported."""
 
     with pytest.raises(
```

#### html2text {}

```diff
@@ -1,44 +1,43 @@
-import pathlib import re import sys import pytest import pytest_lsp from
-lsprotocol.types import WorkspaceFolder from pygls.exceptions import
-JsonRpcInternalError from pygls.workspace import Workspace from pytest_lsp
-import ClientServerConfig from
-esbonio.server.features.sphinx_manager.client_subprocess import
+import logging import pathlib import re import sys import pytest import
+pytest_asyncio from lsprotocol.types import WorkspaceFolder from
+pygls.exceptions import JsonRpcInternalError from pygls.workspace import
+Workspace from esbonio.server.features.sphinx_manager.client import ClientState
+from esbonio.server.features.sphinx_manager.client_subprocess import
 ( SubprocessSphinxClient, ) from
 esbonio.server.features.sphinx_manager.client_subprocess import
 ( make_test_sphinx_client, ) from esbonio.server.features.sphinx_manager.config
-import SphinxConfig @pytest.mark.asyncio async def
-test_build_includes_webview_js(client: SubprocessSphinxClient, uri_for):
-"""Ensure that builds include the ``webview.js`` script.""" out =
+import SphinxConfig logger = logging.getLogger(__name__) @pytest.mark.asyncio
+async def test_build_includes_webview_js(client: SubprocessSphinxClient,
+uri_for): """Ensure that builds include the ``webview.js`` script.""" out =
 client.build_uri src = client.src_uri assert out is not None and src is not
 None # Ensure the script is included in the build output webview_js =
 pathlib.Path(out / "_static" / "webview.js") assert webview_js.exists() assert
 "editor/scroll" in webview_js.read_text() # Ensure the script is included in
 the page index_html = pathlib.Path(out / "index.html") pattern = re.compile(r'
 ') assert pattern.search(index_html.read_text()) is not None
 @pytest.mark.asyncio async def test_build_content_override(client:
 SubprocessSphinxClient, uri_for): """Ensure that we can override the contents
 of a given src file when required.""" out = client.build_uri src =
 client.src_uri assert out is not None and src is not None await client.build()
 # Before expected = "Welcome to the demo documentation" index_html =
 pathlib.Path(out / "index.html") assert expected in index_html.read_text()
-await client.build( content_overrides={ (src / "index.rst").fs_path: "My Custom
-Title\n===============" } ) # Ensure the override was applied expected = "My
+await client.build( content_overrides={str(src / "index.rst"): "My Custom
+Title\n==============="} ) # Ensure the override was applied expected = "My
 Custom Title" print(index_html.read_text()) assert expected in
-index_html.read_text() @pytest_lsp.fixture( scope="module",
-config=ClientServerConfig( server_command=[sys.executable, "-m",
-"esbonio.sphinx_agent"], client_factory=make_test_sphinx_client, ), ) async def
-client_build_error( sphinx_client: SubprocessSphinxClient, uri_for,
-tmp_path_factory ): """A sphinx client that will error when a build is
-triggered.""" build_dir = tmp_path_factory.mktemp("build") demo_workspace =
-uri_for("workspaces", "demo") test_uri = demo_workspace / "index.rst" workspace
-= Workspace( None, workspace_folders=[ WorkspaceFolder(uri=str(demo_workspace),
-name="demo"), ], ) conf_dir = uri_for("workspaces", "demo-error-build").fs_path
-config = SphinxConfig( build_command=[ "sphinx-build", "-b", "html", "-c", str
-(conf_dir), demo_workspace.fs_path, str(build_dir), ], ) resolved =
-config.resolve(test_uri, workspace, sphinx_client.logger) assert resolved is
-not None info = await sphinx_client.create_application(resolved) assert info is
-not None yield @pytest.mark.asyncio(scope="module") async def test_build_error
-(client_build_error: SubprocessSphinxClient): """Ensure that when a build error
-occurs, useful information is reported.""" with pytest.raises
-( JsonRpcInternalError, match="sphinx-build failed:.*division by zero.*" ):
-await client_build_error.build()
+index_html.read_text() @pytest_asyncio.fixture(scope="module") async def
+client_build_error(uri_for, tmp_path_factory): """A sphinx client that will
+error when a build is triggered.""" build_dir = tmp_path_factory.mktemp
+("build") demo_workspace = uri_for("workspaces", "demo") test_uri =
+demo_workspace / "index.rst" workspace = Workspace( None, workspace_folders=
+[ WorkspaceFolder(uri=str(demo_workspace), name="demo"), ], ) conf_dir =
+uri_for("workspaces", "demo-error-build").fs_path config = SphinxConfig
+( python_command=[sys.executable], build_command=[ "sphinx-build", "-b",
+"html", "-c", str(conf_dir), demo_workspace.fs_path, str(build_dir), ], )
+resolved = config.resolve(test_uri, workspace, logger) assert resolved is not
+None sphinx_client = await make_test_sphinx_client(resolved) assert
+sphinx_client.state == ClientState.Running yield sphinx_client await
+sphinx_client.stop() @pytest.mark.asyncio(scope="module") async def
+test_build_error(client_build_error: SubprocessSphinxClient): """Ensure that
+when a build error occurs, useful information is reported.""" with
+pytest.raises( JsonRpcInternalError, match="sphinx-build failed:.*division by
+zero.*" ): await client_build_error.build()
```

### Comparing `esbonio-1.0.0b1/tests/sphinx-agent/test_sa_create_app.py` & `esbonio-1.0.0b2/tests/sphinx-agent/test_sa_create_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,69 @@
+import logging
 import sys
 
 import pytest
-import pytest_lsp
 from lsprotocol.types import WorkspaceFolder
 from pygls import IS_WIN
-from pygls.exceptions import JsonRpcInternalError
 from pygls.workspace import Workspace
-from pytest_lsp import ClientServerConfig
 
+from esbonio.server.features.sphinx_manager.client import ClientState
 from esbonio.server.features.sphinx_manager.client_subprocess import (
     SubprocessSphinxClient,
 )
 from esbonio.server.features.sphinx_manager.client_subprocess import (
     make_test_sphinx_client,
 )
 from esbonio.server.features.sphinx_manager.config import SphinxConfig
 
-
-@pytest_lsp.fixture(
-    config=ClientServerConfig(
-        server_command=[sys.executable, "-m", "esbonio.sphinx_agent"],
-        client_factory=make_test_sphinx_client,
-    )
-)
-async def client(sphinx_client: SubprocessSphinxClient):
-    yield
+logger = logging.getLogger("__name__")
 
 
 @pytest.mark.asyncio
-async def test_create_application(client: SubprocessSphinxClient, uri_for):
+async def test_create_application(uri_for):
     """Ensure that we can create a Sphinx application instance correctly."""
 
     demo_workspace = uri_for("workspaces", "demo")
     test_uri = demo_workspace / "index.rst"
 
     workspace = Workspace(
         None,
         workspace_folders=[
             WorkspaceFolder(uri=str(demo_workspace), name="demo"),
         ],
     )
-    config = SphinxConfig()
-    resolved = config.resolve(test_uri, workspace, client.logger)
+    config = SphinxConfig(python_command=[sys.executable])
+    resolved = config.resolve(test_uri, workspace, logger)
     assert resolved is not None
+    client = None
 
-    info = await client.create_application(resolved)
-    assert info is not None
-    assert info.builder_name == "dirhtml"
-
-    # Paths are case insensitive on Windows
-    if IS_WIN:
-        assert info.src_dir.lower() == demo_workspace.fs_path.lower()
-        assert info.conf_dir.lower() == demo_workspace.fs_path.lower()
-        assert "cache" in info.build_dir.lower()
-    else:
-        assert info.src_dir == demo_workspace.fs_path
-        assert info.conf_dir == demo_workspace.fs_path
-        assert "cache" in info.build_dir
+    try:
+        client = await make_test_sphinx_client(resolved)
+        assert client.state == ClientState.Running
+
+        info = client.sphinx_info
+        assert info is not None
+        assert info.builder_name == "dirhtml"
+
+        # Paths are case insensitive on Windows
+        if IS_WIN:
+            assert info.src_dir.lower() == demo_workspace.fs_path.lower()
+            assert info.conf_dir.lower() == demo_workspace.fs_path.lower()
+            assert "cache" in info.build_dir.lower()
+        else:
+            assert info.src_dir == demo_workspace.fs_path
+            assert info.conf_dir == demo_workspace.fs_path
+            assert "cache" in info.build_dir
+    finally:
+        if client:
+            await client.stop()
 
 
 @pytest.mark.asyncio
-async def test_create_application_error(
-    client: SubprocessSphinxClient, uri_for, tmp_path_factory
-):
+async def test_create_application_error(uri_for, tmp_path_factory):
     """Ensure that we can handle errors during application creation."""
 
     build_dir = tmp_path_factory.mktemp("build")
     demo_workspace = uri_for("workspaces", "demo")
     test_uri = demo_workspace / "index.rst"
 
     workspace = Workspace(
@@ -74,25 +71,29 @@
         workspace_folders=[
             WorkspaceFolder(uri=str(demo_workspace), name="demo"),
         ],
     )
 
     conf_dir = uri_for("workspaces", "demo-error").fs_path
     config = SphinxConfig(
+        python_command=[sys.executable],
         build_command=[
             "sphinx-build",
             "-b",
             "html",
             "-c",
             conf_dir,
             demo_workspace.fs_path,
             str(build_dir),
-        ]
+        ],
     )
-    resolved = config.resolve(test_uri, workspace, client.logger)
+    resolved = config.resolve(test_uri, workspace, logger)
     assert resolved is not None
 
-    with pytest.raises(
-        JsonRpcInternalError,
-        match="There is a programmable error in your configuration file:",
-    ):
-        await client.create_application(resolved)
+    try:
+        client = await SubprocessSphinxClient(resolved)
+        assert client.state == ClientState.Errored
+
+        message = "There is a programmable error in your configuration file:"
+        assert message in str(client.exception)
+    finally:
+        await client.stop()
```

### Comparing `esbonio-1.0.0b1/tests/sphinx-agent/test_sa_unit.py` & `esbonio-1.0.0b2/tests/sphinx-agent/test_sa_unit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,40 @@
+from __future__ import annotations
+
 import logging
 import os
 import pathlib
 import sys
-from typing import Any
-from typing import Dict
-from typing import List
-from typing import Optional
-from typing import Tuple
+import typing
 from unittest import mock
 
 import pytest
-from lsprotocol.types import WorkspaceFolder
-from pygls.workspace import Workspace
 
-from esbonio.server import Uri
-from esbonio.server.features.sphinx_manager.config import (
-    SphinxConfig as SphinxAgentConfig,
-)
 from esbonio.sphinx_agent.config import SphinxConfig
-from esbonio.sphinx_agent.log import SphinxLogHandler
+from esbonio.sphinx_agent.log import DiagnosticFilter
+
+if typing.TYPE_CHECKING:
+    from typing import Any
+    from typing import Dict
+    from typing import List
+    from typing import Optional
+    from typing import Tuple
+
 
 logger = logging.getLogger(__name__)
 
 
 def application_args(**kwargs) -> Dict[str, Any]:
     defaults = {
         "confoverrides": {},
         "freshenv": False,
         "keep_going": False,
         "parallel": 1,
-        "status": None,
         "tags": [],
         "verbosity": 0,
-        "warning": None,
         "warningiserror": False,
     }
 
     for arg in {"srcdir", "outdir", "confdir", "doctreedir"}:
         if arg in kwargs:
             kwargs[arg] = str(pathlib.Path(kwargs[arg]).resolve())
 
@@ -428,92 +426,28 @@
             ),
         ),
     ],
 )
 def test_cli_arg_handling(args: List[str], expected: Dict[str, Any]):
     """Ensure that we can convert ``sphinx-build`` to the correct Sphinx application
     options."""
-
     config = SphinxConfig.fromcli(args)
     assert config is not None
-    assert expected == config.to_application_args()
 
+    actual = config.to_application_args()
 
-@pytest.mark.parametrize(
-    "config, uri, workspace, expected",
-    [
-        # If everything is specified, resolve should be a no-op
-        (
-            SphinxAgentConfig(
-                python_command=[sys.executable],
-                build_command=["sphinx-build", "-M", "html", "src", "dest"],
-                cwd="/path/to/workspace",
-                python_path=["/path/to/site-packages/esbonio/"],
-            ),
-            "file::///path/to/file.rst",
-            Workspace(None),
-            SphinxAgentConfig(
-                python_command=[sys.executable],
-                build_command=["sphinx-build", "-M", "html", "src", "dest"],
-                cwd="/path/to/workspace",
-                python_path=["/path/to/site-packages/esbonio/"],
-            ),
-        ),
-        # If no cwd given, we should try to pick one based on the given workspace
-        (
-            SphinxAgentConfig(
-                python_command=[sys.executable],
-                build_command=["sphinx-build", "-M", "html", "src", "dest"],
-                python_path=["/path/to/site-packages/esbonio/"],
-            ),
-            "file::///path/to/file.rst",
-            Workspace("file:///path/to/workspace/root"),
-            SphinxAgentConfig(
-                python_command=[sys.executable],
-                build_command=["sphinx-build", "-M", "html", "src", "dest"],
-                cwd=os.path.join(".", "path", "to", "workspace", "root")[1:],
-                python_path=["/path/to/site-packages/esbonio/"],
-            ),
-        ),
-        (
-            SphinxAgentConfig(
-                python_command=[sys.executable],
-                build_command=["sphinx-build", "-M", "html", "src", "dest"],
-                python_path=["/path/to/site-packages/esbonio/"],
-            ),
-            "file:///path/to/workspace-b/file.rst",
-            Workspace(
-                "file:///path/to/workspace/root",
-                workspace_folders=[
-                    WorkspaceFolder(
-                        uri="file:///path/to/workspace-a", name="Workspace A"
-                    ),
-                    WorkspaceFolder(
-                        uri="file:///path/to/workspace-b", name="Workspace B"
-                    ),
-                ],
-            ),
-            SphinxAgentConfig(
-                python_command=[sys.executable],
-                build_command=["sphinx-build", "-M", "html", "src", "dest"],
-                cwd=os.path.join(".", "path", "to", "workspace-b")[1:],
-                python_path=["/path/to/site-packages/esbonio/"],
-            ),
-        ),
-    ],
-)
-def test_resolve_sphinx_config(
-    config: SphinxAgentConfig,
-    uri: str,
-    workspace: Workspace,
-    expected: SphinxAgentConfig,
-):
-    """Ensure that we can resolve the client side config for the SphinxAgent
-    correctly."""
-    assert expected == config.resolve(Uri.parse(uri), workspace, logger)
+    # pytest overrides stderr on windows, so if we were to put `sys.stderr` in the
+    # `expected` dict this test would fail as `sys.stderr` inside a test function has a
+    # different value.
+    #
+    # So, let's test for it here instead
+    assert actual.pop("status") == sys.stderr
+    assert actual.pop("warning") == sys.stderr
+
+    assert expected == actual
 
 
 ROOT = pathlib.Path(__file__).parent.parent / "sphinx-extensions" / "workspace"
 PY_PATH = ROOT / "code" / "diagnostics.py"
 CONF_PATH = ROOT / "sphinx-extensions" / "conf.py"
 RST_PATH = ROOT / "sphinx-extensions" / "index.rst"
 INC_PATH = ROOT / "sphinx-extensions" / "_include_me.txt"
@@ -525,28 +459,28 @@
     [
         ("", (str(CONF_PATH), None)),
         (f"{RST_PATH}", (str(RST_PATH), None)),
         (f"{RST_PATH}:", (str(RST_PATH), None)),
         (f"{RST_PATH}:3", (str(RST_PATH), 3)),
         (f"{REL_INC_PATH}:12", (str(INC_PATH), 12)),
         (
-            f"{PY_PATH}:docstring of esbonio.sphinx_agent.log.SphinxLogHandler:3",
+            f"{PY_PATH}:docstring of esbonio.sphinx_agent.log.DiagnosticFilter:3",
             (str(PY_PATH), 22),
         ),
         (f"internal padding after {RST_PATH}:34", (str(RST_PATH), 34)),
         (f"internal padding before {RST_PATH}:34", (str(RST_PATH), 34)),
     ],
 )
 def test_get_diagnostic_location(location: str, expected: Tuple[str, Optional[int]]):
     """Ensure we can correctly determine a dianostic's location based on the string we
     get from sphinx."""
 
     app = mock.Mock()
     app.confdir = str(ROOT / "sphinx-extensions")
 
-    handler = SphinxLogHandler(app)
+    handler = DiagnosticFilter(app)
 
-    mockpath = f"{SphinxLogHandler.__module__}.inspect.getsourcelines"
+    mockpath = f"{DiagnosticFilter.__module__}.inspect.getsourcelines"
     with mock.patch(mockpath, return_value=([""], 20)):
         actual = handler.get_location(location)
 
     assert actual == expected
```

### Comparing `esbonio-1.0.0b1/tests/sphinx-agent/test_sa_uri_class.py` & `esbonio-1.0.0b2/tests/sphinx-agent/test_sa_uri_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Test cases originally based on:
 # https://github.com/microsoft/vscode/blob/5653420433692dc4269ad39adbc143e3438af179/src/vs/base/test/common/uri.test.ts
 import os.path
 import pathlib
+from typing import Any
 from typing import Dict
 
 import pytest
 
 from esbonio.sphinx_agent.types import IS_WIN
 from esbonio.sphinx_agent.types import Uri
 
@@ -27,14 +28,80 @@
     keys etc."""
 
     uri = Uri.for_file("file.txt")
     assert hash(uri) != 0
 
 
 @pytest.mark.parametrize(
+    "a,b,expected",
+    [
+        (Uri.parse("file:///a.txt"), 1, False),
+        (Uri.create(scheme="file"), Uri.create(scheme="file"), True),
+        (Uri.create(scheme="file"), Uri.create(scheme="http"), False),
+        (
+            Uri.create(scheme="file", query="a"),
+            Uri.create(scheme="file", query="a"),
+            True,
+        ),
+        (
+            Uri.create(scheme="file", query="a"),
+            Uri.create(scheme="file", query="b"),
+            False,
+        ),
+        (
+            Uri.create(scheme="file", authority="a"),
+            Uri.create(scheme="file", authority="a"),
+            True,
+        ),
+        (
+            Uri.create(scheme="file", authority="a"),
+            Uri.create(scheme="file", authority="b"),
+            False,
+        ),
+        (
+            Uri.create(scheme="file", fragment="a"),
+            Uri.create(scheme="file", fragment="a"),
+            True,
+        ),
+        (
+            Uri.create(scheme="file", fragment="a"),
+            Uri.create(scheme="file", fragment="b"),
+            False,
+        ),
+        (
+            Uri.create(scheme="http", path="a/b"),
+            Uri.create(scheme="http", path="a/b"),
+            True,
+        ),
+        (
+            Uri.create(scheme="http", path="a/b"),
+            Uri.create(scheme="http", path="a/B"),
+            False,
+        ),
+        pytest.param(
+            Uri.create(scheme="file", path="a/b"),
+            Uri.create(scheme="file", path="a/B"),
+            False,
+            marks=pytest.mark.skipif(IS_WIN, reason="N/A for Windows"),
+        ),
+        pytest.param(
+            # Filepaths on Windows are case insensitive
+            Uri.create(scheme="file", path="a/b"),
+            Uri.create(scheme="file", path="a/B"),
+            True,
+            marks=pytest.mark.skipif(not IS_WIN, reason="Windows only"),
+        ),
+    ],
+)
+def test_uri_eq(a: Uri, b: Any, expected: bool):
+    """Ensure that we have implemented ``__eq__`` for Uris correctly."""
+    assert (a == b) is expected
+
+
+@pytest.mark.parametrize(
     "path, expected",
     [
         ("c:/win/path", "file:///c%3A/win/path"),
         ("C:/win/path", "file:///c%3A/win/path"),
         ("c:/win/path/", "file:///c%3A/win/path/"),
         ("/c:/win/path", "file:///c%3A/win/path"),
         pytest.param(
```

### Comparing `esbonio-1.0.0b1/tests/sphinx-agent/handlers/test_database.py` & `esbonio-1.0.0b2/tests/sphinx-agent/handlers/test_database.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 import pytest
 
+from esbonio.server.features.project_manager import Project
 from esbonio.server.features.sphinx_manager.client_subprocess import (
     SubprocessSphinxClient,
 )
 
 
 def anuri(base, *args):
     uri = base
     for a in args:
         uri /= a
 
     return str(uri.resolve())
 
 
 @pytest.mark.asyncio
-async def test_files_table(client: SubprocessSphinxClient):
+async def test_files_table(client: SubprocessSphinxClient, project: Project):
     """Ensure that we can correctly index all the files in the Sphinx project."""
 
     src = client.src_uri
-    assert src is not None
 
-    assert client.db is not None
-    cursor = await client.db.execute("SELECT * FROM files")
+    db = await project.get_db()
+    cursor = await db.execute("SELECT * FROM files")
     results = await cursor.fetchall()
     actual = {r for r in results if "badfile" not in r[1]}
 
     expected = {
         (anuri(src, "index.rst"), "index", "index.html"),
         (anuri(src, "rst", "directives.rst"), "rst/directives", "rst/directives.html"),
+        (
+            anuri(src, "rst", "diagnostics.rst"),
+            "rst/diagnostics",
+            "rst/diagnostics.html",
+        ),
         (anuri(src, "rst", "symbols.rst"), "rst/symbols", "rst/symbols.html"),
         (
             anuri(src, "myst", "directives.md"),
             "myst/directives",
             "myst/directives.html",
         ),
+        (
+            anuri(src, "myst", "diagnostics.md"),
+            "myst/diagnostics",
+            "myst/diagnostics.html",
+        ),
         (anuri(src, "myst", "symbols.md"), "myst/symbols", "myst/symbols.html"),
         (anuri(src, "demo_rst.rst"), "demo_rst", "demo_rst.html"),
         (anuri(src, "demo_myst.md"), "demo_myst", "demo_myst.html"),
     }
 
     assert expected == actual
```

### Comparing `esbonio-1.0.0b1/tests/sphinx-agent/handlers/test_diagnostics.py` & `esbonio-1.0.0b2/tests/sphinx-agent/handlers/test_diagnostics.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Dict
 from typing import List
 
 import pytest
 from pygls.protocol import default_converter
 
 from esbonio.server import Uri
+from esbonio.server.features.project_manager import Project
 from esbonio.server.features.sphinx_manager.client_subprocess import (
     SubprocessSphinxClient,
 )
 from esbonio.sphinx_agent import types
 
 
 def check_diagnostics(
@@ -25,74 +26,61 @@
         actual_diags = [converter.structure(d, types.Diagnostic) for d in actual[k]]
 
         # Order of results is not important
         assert set(actual_diags) == set(ex_diags)
 
 
 @pytest.mark.asyncio
-@pytest.mark.skip
-async def test_diagnostics(client: SubprocessSphinxClient, uri_for):
+async def test_diagnostics(client: SubprocessSphinxClient, project: Project, uri_for):
     """Ensure that the sphinx agent reports diagnostics collected during the build, and
     that they are correctly reset when fixed."""
-    definitions_uri = uri_for("sphinx-default/workspace/definitions.rst")
-    options_uri = uri_for("sphinx-default/workspace/directive_options.rst")
+    rst_diagnostics_uri = uri_for("workspaces/demo/rst/diagnostics.rst")
+    myst_diagnostics_uri = uri_for("workspaces/demo/myst/diagnostics.md")
 
     expected = {
-        definitions_uri: [
+        rst_diagnostics_uri: [
             types.Diagnostic(
-                message="image file not readable: _static/bad.png",
+                message="image file not readable: not-an-image.png",
                 severity=types.DiagnosticSeverity.Warning,
                 range=types.Range(
-                    start=types.Position(line=28, character=0),
-                    end=types.Position(line=29, character=0),
-                ),
-            ),
-            types.Diagnostic(
-                message="unknown document: '/changelog'",
-                severity=types.DiagnosticSeverity.Warning,
-                range=types.Range(
-                    start=types.Position(line=13, character=0),
-                    end=types.Position(line=14, character=0),
+                    start=types.Position(line=5, character=0),
+                    end=types.Position(line=6, character=0),
                 ),
             ),
         ],
-        options_uri: [
-            types.Diagnostic(
-                message="image file not readable: filename.png",
-                severity=types.DiagnosticSeverity.Warning,
-                range=types.Range(
-                    start=types.Position(line=0, character=0),
-                    end=types.Position(line=1, character=0),
-                ),
-            ),
+        myst_diagnostics_uri: [
             types.Diagnostic(
-                message="document isn't included in any toctree",
+                message="image file not readable: not-an-image.png",
                 severity=types.DiagnosticSeverity.Warning,
                 range=types.Range(
                     start=types.Position(line=0, character=0),
                     end=types.Position(line=1, character=0),
                 ),
             ),
         ],
     }
 
-    actual = await client.get_diagnostics()
+    actual = await project.get_diagnostics()
     check_diagnostics(expected, actual)
 
     await client.build(
-        content_overrides={definitions_uri.fs_path: "My Custom Title\n==============="}
+        content_overrides={
+            str(
+                rst_diagnostics_uri
+            ): "My Custom Title\n===============\n\nThere are no images here"
+        }
     )
 
-    actual = await client.get_diagnostics()
-    check_diagnostics({options_uri: expected[options_uri]}, actual)
+    actual = await project.get_diagnostics()
+    check_diagnostics({myst_diagnostics_uri: expected[myst_diagnostics_uri]}, actual)
 
     # The original diagnostics should be reported when the issues are re-introduced.
     #
     # Note: We have to "override" the contents of the file with the original text to
     #       trick Sphinx into re-building the file.
     await client.build(
         content_overrides={
-            definitions_uri.fs_path: pathlib.Path(definitions_uri).read_text()
+            str(rst_diagnostics_uri): pathlib.Path(rst_diagnostics_uri).read_text()
         }
     )
-    actual = await client.get_diagnostics()
+    actual = await project.get_diagnostics()
     check_diagnostics(expected, actual)
```

### Comparing `esbonio-1.0.0b1/tests/workspaces/demo/LICENSE` & `esbonio-1.0.0b2/tests/workspaces/demo/LICENSE`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/tests/workspaces/demo/README.md` & `esbonio-1.0.0b2/tests/workspaces/demo/README.md`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/tests/workspaces/demo/conf.py` & `esbonio-1.0.0b2/tests/workspaces/demo/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 html_theme = "furo"
 html_title = "Esbonio Demo"
 html_theme_options = {
     "source_repository": "https://github.com/swyddfa/esbonio",
     "source_branch": "develop",
     "source_directory": "lib/esbonio/tests/workspaces/demo/",
 }
-html_static_path = ["_static"]
 
 
 def lsp_role(name, rawtext, text, lineno, inliner, options={}, content=[]):
     """Link to sections within the lsp specification."""
 
     anchor = text.replace("/", "_")
     ref = f"https://microsoft.github.io/language-server-protocol/specifications/lsp/3.17/specification/#{anchor}"
```

### Comparing `esbonio-1.0.0b1/tests/workspaces/demo/index.rst` & `esbonio-1.0.0b2/tests/workspaces/demo/index.rst`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/tests/workspaces/demo/myst/symbols.md` & `esbonio-1.0.0b2/tests/workspaces/demo/myst/symbols.md`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/tests/workspaces/demo/rst/symbols.rst` & `esbonio-1.0.0b2/tests/workspaces/demo/rst/symbols.rst`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/tests/workspaces/demo-error/conf.py` & `esbonio-1.0.0b2/tests/workspaces/demo-error/conf.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/tests/workspaces/demo-error-build/conf.py` & `esbonio-1.0.0b2/tests/workspaces/demo-error-build/conf.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/LICENSE` & `esbonio-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b1/README.md` & `esbonio-1.0.0b2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,12 +38,12 @@
 
 ![Implementations Demo](https://github.com/swyddfa/esbonio/raw/release/resources/images/implementation-demo.gif)
 
 ## Installation
 
 It's recommended to install the language server with [`pipx`](https://pipx.pypa.io/stable/)
 
-Be sure to check out the [Getting Started](https://docs.esbon.io/latest/en/lsp/getting-started.html) guide for details on integrating the server with your editor of choice.
+Be sure to check out the [Getting Started](https://docs.esbon.io/en/latest/lsp/getting-started.html) guide for details on integrating the server with your editor of choice.
 
 ```
 $ pipx install esbonio
 ```
```

### Comparing `esbonio-1.0.0b1/pyproject.toml` & `esbonio-1.0.0b2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 [project.urls]
 "Bug Tracker" = "https://github.com/swyddfa/esbonio/issues"
 "Documentation" = "https://swyddfa.github.io/esbonio/"
 "Source Code" = "https://github.com/swyddfa/esbonio"
 
 [project.scripts]
 esbonio = "esbonio.server.cli:main"
-esbonio-sphinx = "esbonio.lsp.sphinx.cli:main"
 
 [project.optional-dependencies]
 typecheck = ["mypy", "pytest-lsp>=0.3.1", "types-docutils", "types-pygments"]
 dev = ["black", "flake8", "pre-commit", "tox"]
 
 [tool.coverage.run]
 parallel = true
@@ -63,24 +62,27 @@
 force_single_line = true
 known_first_party = ["esbonio"]
 profile = "black"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-glob='*.txt'"
 asyncio_mode = "auto"
-filterwarnings = [
-    "ignore:'contextfunction' is renamed to 'pass_context',*:DeprecationWarning",
-    "ignore:'environmentfilter' is renamed to 'pass_environment',*:DeprecationWarning",
-]
 
 [tool.mypy]
 mypy_path = "$MYPY_CONFIG_FILE_DIR"
 explicit_package_bases = true
 check_untyped_defs = true
 
+[tool.pyright]
+venv = ".env"
+include = ["esbonio"]
+
+pythonVersion = "3.8"
+pythonPlatform = "All"
+
 [tool.towncrier]
 filename = "CHANGES.md"
 directory = "changes/"
 title_format = "## v{version} - {project_date}"
 issue_format = "[#{issue}](https://github.com/swyddfa/esbonio/issues/{issue})"
 underlines = ["", "", ""]
```

### Comparing `esbonio-1.0.0b1/PKG-INFO` & `esbonio-1.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: esbonio
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A language server for sphinx/docutils based documentation projects.
 Project-URL: Bug Tracker, https://github.com/swyddfa/esbonio/issues
 Project-URL: Documentation, https://swyddfa.github.io/esbonio/
 Project-URL: Source Code, https://github.com/swyddfa/esbonio
 Author-email: Alex Carney <alcarneyme@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -79,12 +79,12 @@
 
 ![Implementations Demo](https://github.com/swyddfa/esbonio/raw/release/resources/images/implementation-demo.gif)
 
 ## Installation
 
 It's recommended to install the language server with [`pipx`](https://pipx.pypa.io/stable/)
 
-Be sure to check out the [Getting Started](https://docs.esbon.io/latest/en/lsp/getting-started.html) guide for details on integrating the server with your editor of choice.
+Be sure to check out the [Getting Started](https://docs.esbon.io/en/latest/lsp/getting-started.html) guide for details on integrating the server with your editor of choice.
 
 ```
 $ pipx install esbonio
 ```
```

