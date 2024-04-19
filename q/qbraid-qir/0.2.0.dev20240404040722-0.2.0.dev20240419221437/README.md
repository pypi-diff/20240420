# Comparing `tmp/qbraid-qir-0.2.0.dev20240404040722.tar.gz` & `tmp/qbraid_qir-0.2.0.dev20240419221437.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-qir-0.2.0.dev20240404040722.tar", last modified: Thu Apr  4 04:07:24 2024, max compression
+gzip compressed data, was "qbraid_qir-0.2.0.dev20240419221437.tar", last modified: Fri Apr 19 22:14:39 2024, max compression
```

## Comparing `qbraid-qir-0.2.0.dev20240404040722.tar` & `qbraid_qir-0.2.0.dev20240419221437.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.717945 qbraid-qir-0.2.0.dev20240404040722/
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    49026 2024-04-04 04:07:24.717945 qbraid-qir-0.2.0.dev20240404040722/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.709945 qbraid-qir-0.2.0.dev20240404040722/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.709945 qbraid-qir-0.2.0.dev20240404040722/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.709945 qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/
--rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/cirq.png
--rw-r--r--   0 runner    (1001) docker     (127)    32358 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/qbraid.png
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/qir.png
--rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/qosf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.709945 qbraid-qir-0.2.0.dev20240404040722/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/api/qbraid_qir.cirq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/api/qbraid_qir.qasm3.rst
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/api/qbraid_qir.rst
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/api/qbraid_qir.runner.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.713945 qbraid-qir-0.2.0.dev20240404040722/docs/userguide/
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/userguide/cirq_qir.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/userguide/qasm3_qir.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/userguide/qasm3_supported.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.713945 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 04:07:22.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.713945 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/opsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/passes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.713945 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/oq3_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)    30831 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.717945 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/runner/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/runner/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/runner/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/runner/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.717945 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    49026 2024-04-04 04:07:24.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-04 04:07:24.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:07:24.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-04 04:07:24.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 04:07:24.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:07:24.717945 qbraid-qir-0.2.0.dev20240404040722/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.717945 qbraid-qir-0.2.0.dev20240404040722/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5254 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.912293 qbraid_qir-0.2.0.dev20240419221437/
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    49311 2024-04-19 22:14:39.912293 qbraid_qir-0.2.0.dev20240419221437/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.904293 qbraid_qir-0.2.0.dev20240419221437/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.904293 qbraid_qir-0.2.0.dev20240419221437/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.904293 qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/cirq.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32358 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/qbraid.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/qir.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/qosf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.904293 qbraid_qir-0.2.0.dev20240419221437/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/api/qbraid_qir.cirq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/api/qbraid_qir.qasm3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/api/qbraid_qir.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/api/qbraid_qir.runner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.904293 qbraid_qir-0.2.0.dev20240419221437/docs/userguide/
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/userguide/cirq_qir.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/userguide/qasm3_qir.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/userguide/qasm3_supported.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.904293 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 22:14:37.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.908293 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/opsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.908293 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/oq3_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34547 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.908293 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.908293 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49311 2024-04-19 22:14:39.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-19 22:14:39.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:14:39.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 22:14:39.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 22:14:39.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 22:14:39.912293 qbraid_qir-0.2.0.dev20240419221437/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.908293 qbraid_qir-0.2.0.dev20240419221437/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5254 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/tools/verify_headers.py
```

### Comparing `qbraid-qir-0.2.0.dev20240404040722/CODE_OF_CONDUCT.md` & `qbraid_qir-0.2.0.dev20240419221437/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/CONTRIBUTING.md` & `qbraid_qir-0.2.0.dev20240419221437/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/LICENSE` & `qbraid_qir-0.2.0.dev20240419221437/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/PKG-INFO` & `qbraid_qir-0.2.0.dev20240419221437/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-qir
-Version: 0.2.0.dev20240404040722
+Version: 0.2.0.dev20240419221437
 Summary: qBraid-SDK extension providing support for QIR conversions.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,61 +686,64 @@
 Keywords: qbraid,quantum,qir,llvm,cirq,openqasm
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyqir~=0.10.0
 Requires-Dist: numpy
 Provides-Extra: cirq
 Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "cirq"
 Provides-Extra: qasm3
 Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0; extra == "qasm3"
 Provides-Extra: test
-Requires-Dist: qbraid~=0.5.3; extra == "test"
+Requires-Dist: qbraid<0.7.0,>=0.5.3; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: lint
 Requires-Dist: black[jupyter]; extra == "lint"
 Requires-Dist: isort; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.2.6; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints<2.1,>=1.24; extra == "docs"
 Requires-Dist: sphinx-rtd-theme~=2.0.0; extra == "docs"
-Requires-Dist: docutils<0.21; extra == "docs"
+Requires-Dist: docutils<0.22; extra == "docs"
 
 <img width="full" alt="qbraid-qir-header" src="https://github.com/qBraid/qbraid-qir/assets/46977852/39f921ae-c4bf-442a-b059-6b21abd2ae50">
 
 <p align='center'>
   <a href='https://github.com/qBraid/qbraid-qir/actions/workflows/main.yml'>
       <img src='https://github.com/qBraid/qbraid-qir/actions/workflows/main.yml/badge.svg' alt='CI'>
   </a>
-  <a href="https://codecov.io/gh/qBraid/qbraid-qir" >
+  <!-- <a href="https://codecov.io/gh/qBraid/qbraid-qir" >
     <img src="https://codecov.io/gh/qBraid/qbraid-qir/graph/badge.svg?token=GUQ3EN8DGI"/>
-  </a>
+  </a> -->
   <a href='https://docs.qbraid.com/projects/qir/en/latest/?badge=latest'>
     <img src='https://readthedocs.com/projects/qbraid-qbraid-qir/badge/?version=latest&token=7656ee72b7a66dec6d78dda911ce808676dca55c3e86702d5e97191badfdf19c' alt='Documentation Status'/>
   </a>
   <a href="https://pypi.org/project/qbraid-qir/">
     <img src="https://img.shields.io/pypi/v/qbraid-qir.svg?color=blue" alt="PyPI version"/>
   </a>
   <a href="https://pypi.org/project/qbraid-qir/">
     <img src="https://img.shields.io/pypi/pyversions/qbraid-qir.svg?color=blue" alt="PyPI version"/>
   </a>
+  <a href="https://pepy.tech/project/qbraid-qir">
+    <img src="https://static.pepy.tech/badge/qbraid-qir" alt="Downloads"/>
+  </a>
   <a href='https://www.gnu.org/licenses/gpl-3.0.html'>
     <img src='https://img.shields.io/github/license/qBraid/qbraid.svg' alt='License'/>
   </a>
   <a href='https://discord.gg/TPBU2sa8Et'>
     <img src='https://img.shields.io/discord/771898982564626445.svg?color=pink' alt='Discord'/>
   </a>
 </p>
@@ -854,14 +857,16 @@
 """
 
 module = qasm3_to_qir(program, name="my-program")
 
 ir = str(module)
 ```
 
+[Currently Supported Operations](https://docs.google.com/spreadsheets/d/1Jgo2_usAnCmV5OLK1RvaGzd7vdjKZKxoBvlTI3g1_lE/edit?usp=sharing)
+
 ### Add QIR node to qBraid conversion graph
 
 ```python
 from qbraid_qir.cirq import cirq_to_qir
 from qbraid.transpiler import Conversion, ConversionGraph
 
 graph = ConversionGraph()
```

### Comparing `qbraid-qir-0.2.0.dev20240404040722/README.md` & `qbraid_qir-0.2.0.dev20240419221437/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 <img width="full" alt="qbraid-qir-header" src="https://github.com/qBraid/qbraid-qir/assets/46977852/39f921ae-c4bf-442a-b059-6b21abd2ae50">
 
 <p align='center'>
   <a href='https://github.com/qBraid/qbraid-qir/actions/workflows/main.yml'>
       <img src='https://github.com/qBraid/qbraid-qir/actions/workflows/main.yml/badge.svg' alt='CI'>
   </a>
-  <a href="https://codecov.io/gh/qBraid/qbraid-qir" >
+  <!-- <a href="https://codecov.io/gh/qBraid/qbraid-qir" >
     <img src="https://codecov.io/gh/qBraid/qbraid-qir/graph/badge.svg?token=GUQ3EN8DGI"/>
-  </a>
+  </a> -->
   <a href='https://docs.qbraid.com/projects/qir/en/latest/?badge=latest'>
     <img src='https://readthedocs.com/projects/qbraid-qbraid-qir/badge/?version=latest&token=7656ee72b7a66dec6d78dda911ce808676dca55c3e86702d5e97191badfdf19c' alt='Documentation Status'/>
   </a>
   <a href="https://pypi.org/project/qbraid-qir/">
     <img src="https://img.shields.io/pypi/v/qbraid-qir.svg?color=blue" alt="PyPI version"/>
   </a>
   <a href="https://pypi.org/project/qbraid-qir/">
     <img src="https://img.shields.io/pypi/pyversions/qbraid-qir.svg?color=blue" alt="PyPI version"/>
   </a>
+  <a href="https://pepy.tech/project/qbraid-qir">
+    <img src="https://static.pepy.tech/badge/qbraid-qir" alt="Downloads"/>
+  </a>
   <a href='https://www.gnu.org/licenses/gpl-3.0.html'>
     <img src='https://img.shields.io/github/license/qBraid/qbraid.svg' alt='License'/>
   </a>
   <a href='https://discord.gg/TPBU2sa8Et'>
     <img src='https://img.shields.io/discord/771898982564626445.svg?color=pink' alt='Discord'/>
   </a>
 </p>
@@ -133,14 +136,16 @@
 """
 
 module = qasm3_to_qir(program, name="my-program")
 
 ir = str(module)
 ```
 
+[Currently Supported Operations](https://docs.google.com/spreadsheets/d/1Jgo2_usAnCmV5OLK1RvaGzd7vdjKZKxoBvlTI3g1_lE/edit?usp=sharing)
+
 ### Add QIR node to qBraid conversion graph
 
 ```python
 from qbraid_qir.cirq import cirq_to_qir
 from qbraid.transpiler import Conversion, ConversionGraph
 
 graph = ConversionGraph()
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 [qbraid-qir-header]
-_[_C_I_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_q_B_r_a_i_d_/_q_b_r_a_i_d_-_q_i_r_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_G_U_Q_3_E_N_8_D_G_I_]
-     _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_D_i_s_c_o_r_d_]
+  _[_C_I_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]_[_L_i_c_e_n_s_e_]
+                                   _[_D_i_s_c_o_r_d_]
 qBraid-SDK extension providing support for QIR conversions. [[https://qbraid-
 static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png]](https://
 account.qbraid.com?gitHubUrl=https://github.com/qBraid/qbraid-qir.git) ##
 Motivation [qir]This project aims to make [QIR](https://www.qir-alliance.org/
 ) representations accessible via the qBraid-SDK [transpiler](#architecture-
 diagram), and by doing so, open the door to language-specific conversions from
 any and all high-level quantum languages [supported](https://docs.qbraid.com/
@@ -30,32 +30,33 @@
 examples ### Cirq conversions ```python import cirq from qbraid_qir.cirq import
 cirq_to_qir q0, q1 = cirq.LineQubit.range(2) circuit = cirq.Circuit( cirq.H
 (q0), cirq.CNOT(q0, q1), cirq.measure(q0, q1) ) module = cirq_to_qir(circuit,
 name="my-circuit") ir = str(module) ``` ### OpenQASM 3 conversions ```python
 from qbraid_qir.qasm3 import qasm3_to_qir program = """ OPENQASM 3; include
 "stdgates.inc"; qubit[2] q; bit[2] c; h q[0]; cx q[0], q[1]; measure q[0] -> c
 [0]; measure q[1] -> c[1]; """ module = qasm3_to_qir(program, name="my-
-program") ir = str(module) ``` ### Add QIR node to qBraid conversion graph
-```python from qbraid_qir.cirq import cirq_to_qir from qbraid.transpiler import
-Conversion, ConversionGraph graph = ConversionGraph() conversion = Conversion
-("cirq", "qir", cirq_to_qir) graph.add_conversion(conversion) graph.plot() ```
-## Architecture diagram qBraid-SDK transpiler hub-and-spokes [architecture]
-(https://docs.qbraid.com/en/latest/sdk/transpiler.html#architecture) with
-qbraid-qir integration (left) mapped to language specific conversion step in
-QIR abstraction [layers](https://www.qir-alliance.org/qir-book/concepts/why-do-
-we-need.html) (right). [architecture]## Contributing - Interested in
-contributing code, or making a PR? See [CONTRIBUTING.md](CONTRIBUTING.md) - For
-feature requests and bug reports: [Submit an issue](https://github.com/qBraid/
-qbraid-qir/issues) - For discussions, and specific questions about the qBraid-
-SDK, qBraid-QIR, or other topics, [join our discord community](https://
-discord.gg/TPBU2sa8Et) - For questions that are more suited for a forum, post
-to [Quantum Computing Stack Exchange](https://
-quantumcomputing.stackexchange.com/) with the [`qbraid`](https://
-quantumcomputing.stackexchange.com/questions/tagged/qbraid) tag. - By
-participating, you are expected to uphold our [code of conduct]
+program") ir = str(module) ``` [Currently Supported Operations](https://
+docs.google.com/spreadsheets/d/1Jgo2_usAnCmV5OLK1RvaGzd7vdjKZKxoBvlTI3g1_lE/
+edit?usp=sharing) ### Add QIR node to qBraid conversion graph ```python from
+qbraid_qir.cirq import cirq_to_qir from qbraid.transpiler import Conversion,
+ConversionGraph graph = ConversionGraph() conversion = Conversion("cirq",
+"qir", cirq_to_qir) graph.add_conversion(conversion) graph.plot() ``` ##
+Architecture diagram qBraid-SDK transpiler hub-and-spokes [architecture](https:
+//docs.qbraid.com/en/latest/sdk/transpiler.html#architecture) with qbraid-qir
+integration (left) mapped to language specific conversion step in QIR
+abstraction [layers](https://www.qir-alliance.org/qir-book/concepts/why-do-we-
+need.html) (right). [architecture]## Contributing - Interested in contributing
+code, or making a PR? See [CONTRIBUTING.md](CONTRIBUTING.md) - For feature
+requests and bug reports: [Submit an issue](https://github.com/qBraid/qbraid-
+qir/issues) - For discussions, and specific questions about the qBraid-SDK,
+qBraid-QIR, or other topics, [join our discord community](https://discord.gg/
+TPBU2sa8Et) - For questions that are more suited for a forum, post to [Quantum
+Computing Stack Exchange](https://quantumcomputing.stackexchange.com/) with the
+[`qbraid`](https://quantumcomputing.stackexchange.com/questions/tagged/qbraid)
+tag. - By participating, you are expected to uphold our [code of conduct]
 (CODE_OF_CONDUCT). ## Citation If you use qBraid-QIR in your research, we
 kindly request that you cite it appropriately. The BibTeX entry below is
 aligned with the latest stable release. For the most up-to-date citation
 details, please refer to [CITATION.cff](CITATION.cff). ```tex @software
 {Kushnir_qBraid-QIR_Python_package_2024, author = {Kushnir, Samuel and Gupta,
 Harshit and Jain, Rohan and Parakh, Priyansh and Hill, Ryan James}, license =
 {GPL-3.0}, month = mar, title = {{qBraid-QIR: Python package for QIR
```

### Comparing `qbraid-qir-0.2.0.dev20240404040722/docs/_static/favicon.ico` & `qbraid_qir-0.2.0.dev20240419221437/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/docs/_static/logo.png` & `qbraid_qir-0.2.0.dev20240419221437/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/cirq.png` & `qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/cirq.png`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/qbraid.png` & `qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/qbraid.png`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/qir.png` & `qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/qir.png`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/qosf.png` & `qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/qosf.png`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/docs/conf.py` & `qbraid_qir-0.2.0.dev20240419221437/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/docs/index.rst` & `qbraid_qir-0.2.0.dev20240419221437/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/docs/userguide/cirq_qir.rst` & `qbraid_qir-0.2.0.dev20240419221437/docs/userguide/cirq_qir.rst`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/docs/userguide/qasm3_qir.rst` & `qbraid_qir-0.2.0.dev20240419221437/docs/userguide/qasm3_qir.rst`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/docs/userguide/qasm3_supported.rst` & `qbraid_qir-0.2.0.dev20240419221437/docs/userguide/qasm3_supported.rst`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/pyproject.toml` & `qbraid_qir-0.2.0.dev20240419221437/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,37 +13,37 @@
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Physics"
 ]
 dependencies = ["pyqir~=0.10.0", "numpy"]
-requires-python = ">= 3.8"
+requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://github.com/qBraid/qbraid-qir"
 Documentation = "https://docs.qbraid.com/projects/qir/en/stable/"
 "Bug Tracker" = "https://github.com/qBraid/qbraid-qir/issues"
 Discord = "https://discord.gg/TPBU2sa8Et"
 "Launch on Lab" = "https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qbraid-qir.git"
 
 [project.optional-dependencies]
 cirq = ["cirq-core>=1.3.0,<1.4.0"]
 qasm3 = ["openqasm3[parser]>=0.4.0,<0.6.0"]
-test = ["qbraid~=0.5.3", "pytest", "pytest-cov"]
+test = ["qbraid>=0.5.3,<0.7.0", "pytest", "pytest-cov"]
 lint = ["black[jupyter]", "isort", "pylint"]
-docs = ["sphinx~=7.2.6", "sphinx-autodoc-typehints>=1.24,<2.1", "sphinx-rtd-theme~=2.0.0", "docutils<0.21"]
+docs = ["sphinx~=7.2.6", "sphinx-autodoc-typehints>=1.24,<2.1", "sphinx-rtd-theme~=2.0.0", "docutils<0.22"]
 
 [tool.setuptools.dynamic]
 version = {attr = "qbraid_qir.__version__"}
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 100
 disable = "C0103, C0115, C0116, I1101, R0903, W0212, W0511"
@@ -72,8 +72,8 @@
 
 [tool.coverage.run]
 parallel = true
 source = ["qbraid_qir"]
 omit = [
   "**/qbraid_qir/runner/simulator.py",
   "**/qbraid_qir/__init__.py"
-]
+]
```

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/__init__.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/__init__.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/convert.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/convert.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/elements.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/elements.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/exceptions.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/opsets.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/opsets.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/passes.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/passes.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/visitor.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/visitor.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/exceptions.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/__init__.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/convert.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/convert.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/elements.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,19 @@
     """
 
     GLOBAL = "global"
     IF = "if"
     LOOP = "loop"
 
 
+class InversionOp(Enum):
+    NO_OP = 1
+    INVERT_ROTATION = 2
+
+
 class _ProgramElement(metaclass=ABCMeta):
     @classmethod
     def from_element_list(cls, elements):
         return [cls(elem) for elem in elements]
 
     @abstractmethod
     def accept(self, visitor):
```

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/exceptions.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/visitor.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/visitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,40 +26,47 @@
     AliasStatement,
     BinaryExpression,
     BooleanLiteral,
     BranchingStatement,
     ClassicalDeclaration,
     DurationLiteral,
     FloatLiteral,
+    GateModifierName,
     Identifier,
     ImaginaryLiteral,
     Include,
     IndexedIdentifier,
     IndexExpression,
     IntegerLiteral,
     IODeclaration,
     QuantumBarrier,
     QuantumGate,
     QuantumGateDefinition,
+    QuantumGateModifier,
     QuantumMeasurementStatement,
     QuantumReset,
     QubitDeclaration,
     RangeDefinition,
     Span,
     Statement,
     SubroutineDefinition,
     UnaryExpression,
 )
 from pyqir import BasicBlock, Builder, Constant
 from pyqir import IntType as qirIntType
 from pyqir import PointerType
 
-from .elements import Context, Qasm3Module, Scope
+from .elements import Context, InversionOp, Qasm3Module, Scope
 from .exceptions import Qasm3ConversionError
-from .oq3_maps import map_qasm_op_to_pyqir_callable, qasm3_constants_map, qasm3_expression_op_map
+from .oq3_maps import (
+    map_qasm_inv_op_to_pyqir_callable,
+    map_qasm_op_to_pyqir_callable,
+    qasm3_constants_map,
+    qasm3_expression_op_map,
+)
 
 _log = logging.getLogger(name=__name__)
 
 
 class ProgramElementVisitor(metaclass=ABCMeta):
     @abstractmethod
     def visit_register(self, register):
@@ -428,48 +435,67 @@
         """
         gate_name = definition.name.name
         if gate_name in self._custom_gates:
             self._print_err_location(definition.span)
             raise Qasm3ConversionError(f"Duplicate gate definition for {gate_name}")
         self._custom_gates[gate_name] = definition
 
-    def _visit_basic_gate_operation(self, operation: QuantumGate) -> None:
+    def _visit_basic_gate_operation(self, operation: QuantumGate, inverse: bool = False) -> None:
         """Visit a gate operation element.
 
         Args:
             operation (QuantumGate): The gate operation to visit.
+            inverse (bool): Whether the operation is an inverse operation. Defaults to False.
+
+                          - if inverse is True, we apply check for different cases in the
+                            map_qasm_inv_op_to_pyqir_callable method.
+
+                          - Only rotation and S / T gates are affected by this inversion. For S/T
+                            gates we map them to Sdg / Tdg and vice versa.
+
+                          - For rotation gates, we map to the same gates but invert the rotation
+                            angles.
 
         Returns:
             None
+
+        Raises:
+            Qasm3ConversionError: If the number of qubits is invalid.
+
         """
 
         _log.debug("Visiting basic gate operation '%s'", str(operation))
         op_name: str = operation.name.name
         op_qubits = self._get_op_qubits(operation)
-        qir_func, op_qubit_count = map_qasm_op_to_pyqir_callable(op_name)
+        inverse_action = None
+        if not inverse:
+            qir_func, op_qubit_count = map_qasm_op_to_pyqir_callable(op_name)
+        else:
+            # in basic gates, inverse action only affects the rotation gates
+            qir_func, op_qubit_count, inverse_action = map_qasm_inv_op_to_pyqir_callable(op_name)
+
         op_parameters = None
 
         if len(op_qubits) % op_qubit_count != 0:
             self._print_err_location(operation.span)
             raise Qasm3ConversionError(
                 f"Invalid number of qubits {len(op_qubits)} for operation {operation.name.name}"
             )
 
         if self._is_parametric_gate(operation):
             op_parameters = self._get_op_parameters(operation)
+            if inverse_action == InversionOp.INVERT_ROTATION:
+                op_parameters = [-1 * param for param in op_parameters]
 
-        if op_parameters is not None:
-            for i in range(0, len(op_qubits), op_qubit_count):
-                qubit_subset = op_qubits[i : i + op_qubit_count]
+        for i in range(0, len(op_qubits), op_qubit_count):
+            # we apply the gate on the qubit subset linearly
+            qubit_subset = op_qubits[i : i + op_qubit_count]
+            if op_parameters is not None:
                 qir_func(self._builder, *op_parameters, *qubit_subset)
-        else:
-            # we have a linear application of the gate
-            # first act on the first op_qubit_count qubits, then the next op_qubit_count and so on
-            for i in range(0, len(op_qubits), op_qubit_count):
-                qubit_subset = op_qubits[i : i + op_qubit_count]
+            else:
                 qir_func(self._builder, *qubit_subset)
 
     def _transform_gate_qubits(self, gate_op: QuantumGate, qubit_map: dict) -> None:
         """Transform the qubits of a gate operation with a qubit map.
 
         Args:
             gate_op (QuantumGate): The gate operation to transform.
@@ -498,82 +524,142 @@
             None
         """
         for i, param in enumerate(gate_op.arguments):
             if isinstance(param, Identifier):
                 gate_op.arguments[i] = param_map[param.name]
             # TODO : update the arg value in expressions not just SINGLE identifiers
 
-    def _visit_custom_gate_operation(self, operation: QuantumGate) -> None:
+    def _validate_gate_call(
+        self, operation: QuantumGate, gate_definition: QuantumGateDefinition, qubits_in_op
+    ) -> None:
+        if len(operation.arguments) != len(gate_definition.arguments):
+            self._print_err_location(operation.span)
+            raise Qasm3ConversionError(
+                f"""Parameter count mismatch for gate {operation.name.name}. Expected \
+{len(gate_definition.arguments)} but got {len(operation.arguments)} in operation"""
+            )
+
+        if qubits_in_op != len(gate_definition.qubits):
+            self._print_err_location(operation.span)
+            raise Qasm3ConversionError(
+                f"""Qubit count mismatch for gate {operation.name.name}. Expected \
+{len(gate_definition.qubits)} but got {qubits_in_op} in operation"""
+            )
+
+    def _visit_custom_gate_operation(self, operation: QuantumGate, inverse: bool = False) -> None:
         """Visit a custom gate operation element recursively.
 
         Args:
             operation (QuantumGate): The gate operation to visit.
+            inverse (bool): Whether the operation is an inverse operation. Defaults to False.
+
+                            If True, the gate operation is applied in reverse order and the
+                            inverse modifier is appended to each gate call.
+                            See https://openqasm.com/language/gates.html#inverse-modifier
+                            for more clarity.
 
         Returns:
             None
         """
         _log.debug("Visiting custom gate operation '%s'", str(operation))
         gate_name: str = operation.name.name
         gate_definition: QuantumGateDefinition = self._custom_gates[gate_name]
-
-        if len(operation.arguments) != len(gate_definition.arguments):
-            self._print_err_location(operation.span)
-            raise Qasm3ConversionError(
-                f"""Parameter count mismatch for gate {gate_name}. Expected \
-{len(gate_definition.arguments)} but got {len(operation.arguments)} in operation"""
-            )
-
         op_qubits = self._get_op_qubits(operation, qir_form=False)
 
-        if len(op_qubits) != len(gate_definition.qubits):
-            self._print_err_location(operation.span)
-            raise Qasm3ConversionError(
-                f"""Qubit count mismatch for gate {gate_name}. Expected \
-{len(gate_definition.qubits)} but got {len(op_qubits)} in operation"""
-            )
-
+        self._validate_gate_call(operation, gate_definition, len(op_qubits))
         # we need this because the gates applied inside a gate definition use the
         # VARIABLE names and not the qubits
 
         # so we need to update the arguments of these gate applications with the actual
         # qubit identifiers and then RECURSIVELY call the visit_generic_gate_operation
         qubit_map = {
             formal_arg.name: actual_arg
             for formal_arg, actual_arg in zip(gate_definition.qubits, op_qubits)
         }
         param_map = {
             formal_arg.name: actual_arg
             for formal_arg, actual_arg in zip(gate_definition.arguments, operation.arguments)
         }
-        for gate_op in gate_definition.body:
+
+        gate_definition_ops = copy.deepcopy(gate_definition.body)
+        if inverse:
+            gate_definition_ops.reverse()
+
+        for gate_op in gate_definition_ops:
+            if gate_op.name.name == gate_name:
+                self._print_err_location(gate_op.span)
+                raise Qasm3ConversionError(
+                    f"Recursive definitions not allowed for gate {gate_name}"
+                )
+
             # necessary to avoid modifying the original gate definition
             # in case the gate is reapplied
             gate_op_copy = copy.deepcopy(gate_op)
             if isinstance(gate_op, QuantumGate):
                 self._transform_gate_params(gate_op_copy, param_map)
                 self._transform_gate_qubits(gate_op_copy, qubit_map)
+                # need to trickle the inverse down to the child!
+                if inverse:
+                    # span doesn't matter as we don't analyse it
+                    gate_op_copy.modifiers.append(QuantumGateModifier(GateModifierName.inv, None))
                 self._visit_generic_gate_operation(gate_op_copy)
             else:
                 # TODO: add control flow support
                 self._print_err_location(gate_op.span)
                 raise Qasm3ConversionError(f"Unsupported gate definition statement {gate_op}")
 
+    def _collapse_gate_modifiers(self, operation: QuantumGate) -> Tuple[Any, Any]:
+        """Collapse the gate modifiers of a gate operation.
+           Some analysis is required to get this result.
+           The basic idea is that any power operation is multiplied and inversions are toggled.
+           The placement of the inverse operation does not matter.
+
+        Args:
+            operation (QuantumGate): The gate operation to collapse modifiers for.
+
+        Returns:
+            Tuple[Any, Any]: The power and inverse values of the gate operation.
+        """
+        power_value, inverse_value = 1, False
+
+        for modifier in operation.modifiers:
+            modifier_name = modifier.modifier
+            if modifier_name == GateModifierName.pow and modifier.argument is not None:
+                current_power = self._evaluate_expression(modifier.argument)
+                if current_power < 0:
+                    inverse_value = not inverse_value
+                power_value = power_value * abs(current_power)
+            elif modifier_name == GateModifierName.inv:
+                inverse_value = not inverse_value
+            elif modifier_name in [GateModifierName.ctrl, GateModifierName.negctrl]:
+                self._print_err_location(operation.span)
+                raise NotImplementedError(
+                    "Controlled modifier gates not yet supported in gate operation"
+                )
+        return (power_value, inverse_value)
+
     def _visit_generic_gate_operation(self, operation: QuantumGate) -> None:
         """Visit a gate operation element.
 
         Args:
             operation (QuantumGate): The gate operation to visit.
 
         Returns:
             None
         """
-        if operation.name.name in self._custom_gates:
-            self._visit_custom_gate_operation(operation)
-        else:
-            self._visit_basic_gate_operation(operation)
+
+        power_value, inverse_value = self._collapse_gate_modifiers(operation)
+
+        # Applying the inverse first and then the power is same as
+        # apply the power first and then inverting the gate
+        for _ in range(power_value):
+            if operation.name.name in self._custom_gates:
+                self._visit_custom_gate_operation(operation, inverse_value)
+            else:
+                self._visit_basic_gate_operation(operation, inverse_value)
 
     def _visit_classical_operation(self, statement: ClassicalDeclaration) -> None:
         """Visit a classical operation element.
 
         Args:
             statement (ClassicalType): The classical operation to visit.
 
@@ -614,29 +700,24 @@
 
         if isinstance(expression, BooleanLiteral):
             return expression.value
         if isinstance(expression, (IntegerLiteral, FloatLiteral)):
             return expression.value
         if isinstance(expression, UnaryExpression):
             op = expression.op.name
-            if op == "!":
-                return not self._evaluate_expression(expression.expression)
             if op == "-":
-                return -1 * self._evaluate_expression(expression.expression)
+                op = "UMINUS"
+            operand = self._evaluate_expression(expression.expression)
             if op == "~":
-                value = self._evaluate_expression(expression.expression)
-                if not isinstance(value, int):
+                if not isinstance(operand, int):
                     self._print_err_location(expression.span)
                     raise Qasm3ConversionError(
-                        f"Unsupported expression type {type(value)} in ~ operation"
+                        f"Unsupported expression type {type(operand)} in ~ operation"
                     )
-                return ~value
-            raise Qasm3ConversionError(
-                f"Unsupported UnaryExpression operation: {op}. Expected one of ['!', '-', '~']"
-            )
+            return qasm3_expression_op_map(op, operand)
         if isinstance(expression, BinaryExpression):
             lhs = self._evaluate_expression(expression.lhs)
             op = expression.op.name
             rhs = self._evaluate_expression(expression.rhs)
             return qasm3_expression_op_map(op, lhs, rhs)
 
         self._print_err_location(expression.span)
```

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/runner/__init__.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/runner/exceptions.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/runner/result.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/runner/simulator.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/simulator.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/serialization.py` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/serialization.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/PKG-INFO` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-qir
-Version: 0.2.0.dev20240404040722
+Version: 0.2.0.dev20240419221437
 Summary: qBraid-SDK extension providing support for QIR conversions.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,61 +686,64 @@
 Keywords: qbraid,quantum,qir,llvm,cirq,openqasm
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyqir~=0.10.0
 Requires-Dist: numpy
 Provides-Extra: cirq
 Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "cirq"
 Provides-Extra: qasm3
 Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0; extra == "qasm3"
 Provides-Extra: test
-Requires-Dist: qbraid~=0.5.3; extra == "test"
+Requires-Dist: qbraid<0.7.0,>=0.5.3; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: lint
 Requires-Dist: black[jupyter]; extra == "lint"
 Requires-Dist: isort; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.2.6; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints<2.1,>=1.24; extra == "docs"
 Requires-Dist: sphinx-rtd-theme~=2.0.0; extra == "docs"
-Requires-Dist: docutils<0.21; extra == "docs"
+Requires-Dist: docutils<0.22; extra == "docs"
 
 <img width="full" alt="qbraid-qir-header" src="https://github.com/qBraid/qbraid-qir/assets/46977852/39f921ae-c4bf-442a-b059-6b21abd2ae50">
 
 <p align='center'>
   <a href='https://github.com/qBraid/qbraid-qir/actions/workflows/main.yml'>
       <img src='https://github.com/qBraid/qbraid-qir/actions/workflows/main.yml/badge.svg' alt='CI'>
   </a>
-  <a href="https://codecov.io/gh/qBraid/qbraid-qir" >
+  <!-- <a href="https://codecov.io/gh/qBraid/qbraid-qir" >
     <img src="https://codecov.io/gh/qBraid/qbraid-qir/graph/badge.svg?token=GUQ3EN8DGI"/>
-  </a>
+  </a> -->
   <a href='https://docs.qbraid.com/projects/qir/en/latest/?badge=latest'>
     <img src='https://readthedocs.com/projects/qbraid-qbraid-qir/badge/?version=latest&token=7656ee72b7a66dec6d78dda911ce808676dca55c3e86702d5e97191badfdf19c' alt='Documentation Status'/>
   </a>
   <a href="https://pypi.org/project/qbraid-qir/">
     <img src="https://img.shields.io/pypi/v/qbraid-qir.svg?color=blue" alt="PyPI version"/>
   </a>
   <a href="https://pypi.org/project/qbraid-qir/">
     <img src="https://img.shields.io/pypi/pyversions/qbraid-qir.svg?color=blue" alt="PyPI version"/>
   </a>
+  <a href="https://pepy.tech/project/qbraid-qir">
+    <img src="https://static.pepy.tech/badge/qbraid-qir" alt="Downloads"/>
+  </a>
   <a href='https://www.gnu.org/licenses/gpl-3.0.html'>
     <img src='https://img.shields.io/github/license/qBraid/qbraid.svg' alt='License'/>
   </a>
   <a href='https://discord.gg/TPBU2sa8Et'>
     <img src='https://img.shields.io/discord/771898982564626445.svg?color=pink' alt='Discord'/>
   </a>
 </p>
@@ -854,14 +857,16 @@
 """
 
 module = qasm3_to_qir(program, name="my-program")
 
 ir = str(module)
 ```
 
+[Currently Supported Operations](https://docs.google.com/spreadsheets/d/1Jgo2_usAnCmV5OLK1RvaGzd7vdjKZKxoBvlTI3g1_lE/edit?usp=sharing)
+
 ### Add QIR node to qBraid conversion graph
 
 ```python
 from qbraid_qir.cirq import cirq_to_qir
 from qbraid.transpiler import Conversion, ConversionGraph
 
 graph = ConversionGraph()
```

### Comparing `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/SOURCES.txt` & `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240404040722/tools/verify_headers.py` & `qbraid_qir-0.2.0.dev20240419221437/tools/verify_headers.py`

 * *Files identical despite different names*

