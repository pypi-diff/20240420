# Comparing `tmp/ypricemagic-3.4.8.tar.gz` & `tmp/ypricemagic-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypricemagic-3.4.8.tar", last modified: Sun Apr 14 23:50:43 2024, max compression
+gzip compressed data, was "ypricemagic-3.4.9.tar", last modified: Mon Apr 15 21:58:27 2024, max compression
```

## Comparing `ypricemagic-3.4.8.tar` & `ypricemagic-3.4.9.tar`

### file list

```diff
@@ -1,205 +1,205 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.768445 ypricemagic-3.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.744445 ypricemagic-3.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.748445 ypricemagic-3.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/.github/workflows/deploy-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-14 23:50:43.768445 ypricemagic-3.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.752445 ypricemagic-3.4.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.744445 ypricemagic-3.4.8/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.744445 ypricemagic-3.4.8/docs/_build/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.752445 ypricemagic-3.4.8/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/_build/html/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.752445 ypricemagic-3.4.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/scripts/debug-curve.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/scripts/debug-price.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-14 23:50:43.768445 ypricemagic-3.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.752445 ypricemagic-3.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.752445 ypricemagic-3.4.8/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/classes/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/classes/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.752445 ypricemagic-3.4.8/tests/prices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.756445 ypricemagic-3.4.8/tests/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/dex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/dex/test_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/dex/test_uniswap.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/dex/test_velodrome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.756445 ypricemagic-3.4.8/tests/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/lending/test_aave.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/lending/test_compound.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.756445 ypricemagic-3.4.8/tests/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/stable_swap/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/test_chainlink.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/test_gearbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/test_popsicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/test_yearn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.756445 ypricemagic-3.4.8/tests/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/tokenized_fund/test_piedao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.756445 ypricemagic-3.4.8/tests/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/prices/utils/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.756445 ypricemagic-3.4.8/y/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.756445 ypricemagic-3.4.8/y/_db/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.760445 ypricemagic-3.4.8/y/_db/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/utils/_ep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/utils/bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/utils/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/utils/price.py
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/utils/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/utils/traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/_db/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.760445 ypricemagic-3.4.8/y/classes/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/classes/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/classes/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24922 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.760445 ypricemagic-3.4.8/y/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.760445 ypricemagic-3.4.8/y/interfaces/balancer/
--rw-r--r--   0 runner    (1001) docker     (127)    23102 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/interfaces/balancer/WeightedPool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/interfaces/balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.760445 ypricemagic-3.4.8/y/interfaces/compound/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/interfaces/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32517 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/interfaces/compound/unitroller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.760445 ypricemagic-3.4.8/y/interfaces/curve/
--rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/interfaces/curve/CurveRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/interfaces/curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/interfaces/multicall2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.760445 ypricemagic-3.4.8/y/interfaces/uniswap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/interfaces/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/interfaces/uniswap/factoryv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/interfaces/uniswap/quoterv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/interfaces/uniswap/velov2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.760445 ypricemagic-3.4.8/y/prices/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/band.py
--rw-r--r--   0 runner    (1001) docker     (127)    20384 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/chainlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/convex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.764445 ypricemagic-3.4.8/y/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.764445 ypricemagic-3.4.8/y/prices/dex/balancer/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/dex/balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/dex/balancer/balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/dex/balancer/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13914 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/dex/balancer/v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/dex/genericamm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/dex/mooniswap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/dex/solidly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.764445 ypricemagic-3.4.8/y/prices/dex/uniswap/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/dex/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/dex/uniswap/uniswap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/dex/uniswap/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    31162 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/dex/uniswap/v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/dex/uniswap/v2_forks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/dex/uniswap/v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/dex/velodrome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.764445 ypricemagic-3.4.8/y/prices/eth_derivs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/eth_derivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/eth_derivs/creth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/eth_derivs/wsteth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/gearbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.764445 ypricemagic-3.4.8/y/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/lending/aave.py
--rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/lending/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/lending/ib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14526 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/popsicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/rkp3r.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/solidex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.764445 ypricemagic-3.4.8/y/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/stable_swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/stable_swap/belt.py
--rw-r--r--   0 runner    (1001) docker     (127)    24089 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/stable_swap/curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/stable_swap/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/stable_swap/froyo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/stable_swap/mstablefeederpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/stable_swap/saddle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.764445 ypricemagic-3.4.8/y/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/tokenized_fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/tokenized_fund/basketdao.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/tokenized_fund/gelato.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/tokenized_fund/piedao.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/tokenized_fund/tokensets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.768445 ypricemagic-3.4.8/y/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/utils/buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/utils/sense_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/utils/ypriceapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/prices/yearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.768445 ypricemagic-3.4.8/y/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/utils/dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (127)    15215 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/utils/fakes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/utils/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/utils/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/y/utils/raw_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.768445 ypricemagic-3.4.8/ypricemagic/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/ypricemagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-14 23:50:33.000000 ypricemagic-3.4.8/ypricemagic/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:50:43.768445 ypricemagic-3.4.8/ypricemagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-14 23:50:43.000000 ypricemagic-3.4.8/ypricemagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-14 23:50:43.000000 ypricemagic-3.4.8/ypricemagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:50:43.000000 ypricemagic-3.4.8/ypricemagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-14 23:50:43.000000 ypricemagic-3.4.8/ypricemagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-14 23:50:43.000000 ypricemagic-3.4.8/ypricemagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.377562 ypricemagic-3.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.381562 ypricemagic-3.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.381562 ypricemagic-3.4.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.377562 ypricemagic-3.4.9/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.377562 ypricemagic-3.4.9/docs/_build/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/scripts/debug-curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/scripts/debug-price.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/classes/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/classes/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/tests/prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/tests/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/dex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/dex/test_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/dex/test_uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/dex/test_velodrome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/tests/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/lending/test_aave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/lending/test_compound.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/tests/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/stable_swap/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/test_chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/test_gearbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/test_popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/test_yearn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/tests/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/tokenized_fund/test_piedao.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.389562 ypricemagic-3.4.9/tests/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/utils/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.389562 ypricemagic-3.4.9/y/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.389562 ypricemagic-3.4.9/y/_db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.389562 ypricemagic-3.4.9/y/_db/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/_ep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.393562 ypricemagic-3.4.9/y/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/classes/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/classes/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24922 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.393562 ypricemagic-3.4.9/y/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.393562 ypricemagic-3.4.9/y/interfaces/balancer/
+-rw-r--r--   0 runner    (1001) docker     (127)    23102 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/balancer/WeightedPool.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.393562 ypricemagic-3.4.9/y/interfaces/compound/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32517 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/compound/unitroller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.393562 ypricemagic-3.4.9/y/interfaces/curve/
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/curve/CurveRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/multicall2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.393562 ypricemagic-3.4.9/y/interfaces/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/uniswap/factoryv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/uniswap/quoterv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/uniswap/velov2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.393562 ypricemagic-3.4.9/y/prices/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/band.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20384 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/convex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.397562 ypricemagic-3.4.9/y/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.397562 ypricemagic-3.4.9/y/prices/dex/balancer/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/balancer/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/balancer/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13914 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/balancer/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/genericamm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/mooniswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/solidly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.397562 ypricemagic-3.4.9/y/prices/dex/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/uniswap/uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/uniswap/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31162 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/uniswap/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/uniswap/v2_forks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/uniswap/v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/velodrome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.397562 ypricemagic-3.4.9/y/prices/eth_derivs/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/eth_derivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/eth_derivs/creth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/eth_derivs/wsteth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/gearbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.397562 ypricemagic-3.4.9/y/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/lending/aave.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/lending/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/lending/ib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14526 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/rkp3r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/solidex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.397562 ypricemagic-3.4.9/y/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/stable_swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/stable_swap/belt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24138 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/stable_swap/curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/stable_swap/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/stable_swap/froyo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/stable_swap/mstablefeederpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/stable_swap/saddle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/y/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/tokenized_fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/tokenized_fund/basketdao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/tokenized_fund/gelato.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/tokenized_fund/piedao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/tokenized_fund/tokensets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/y/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/utils/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/utils/sense_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/utils/ypriceapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/yearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/y/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15215 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/raw_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/ypricemagic/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/ypricemagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/ypricemagic/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/ypricemagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-15 21:58:27.000000 ypricemagic-3.4.9/ypricemagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-15 21:58:27.000000 ypricemagic-3.4.9/ypricemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:58:27.000000 ypricemagic-3.4.9/ypricemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 21:58:27.000000 ypricemagic-3.4.9/ypricemagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 21:58:27.000000 ypricemagic-3.4.9/ypricemagic.egg-info/top_level.txt
```

### Comparing `ypricemagic-3.4.8/.github/workflows/codeql-analysis.yml` & `ypricemagic-3.4.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/.github/workflows/deploy-docs.yml` & `ypricemagic-3.4.9/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/.github/workflows/pytest.yaml` & `ypricemagic-3.4.9/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/.github/workflows/release.yaml` & `ypricemagic-3.4.9/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/CONTRIBUTING.md` & `ypricemagic-3.4.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/LICENSE.txt` & `ypricemagic-3.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/Makefile` & `ypricemagic-3.4.9/Makefile`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/PKG-INFO` & `ypricemagic-3.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ypricemagic
-Version: 3.4.8
+Version: 3.4.9
 Summary: Use this tool to extract historical on-chain price data from an archive node. Shoutout to @bantg and @nymmrx for their awesome work on yearn-exporter that made this library possible.
 Home-page: https://github.com/BobTheBuidler/ypricemagic
 Author: BobTheBuidler
 Author-email: bobthebuidlerdefi@gmail.com
 License: MIT
 License-File: LICENSE.txt
 Requires-Dist: bobs_lazy_logging==0.0.4
```

### Comparing `ypricemagic-3.4.8/README.md` & `ypricemagic-3.4.9/README.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/docs/Makefile` & `ypricemagic-3.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/docs/_build/html/_static/alabaster.css` & `ypricemagic-3.4.9/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/docs/_build/html/_static/basic.css` & `ypricemagic-3.4.9/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/docs/_build/html/_static/doctools.js` & `ypricemagic-3.4.9/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/docs/_build/html/_static/language_data.js` & `ypricemagic-3.4.9/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/docs/_build/html/_static/pygments.css` & `ypricemagic-3.4.9/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/docs/_build/html/_static/searchtools.js` & `ypricemagic-3.4.9/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/docs/_build/html/_static/sphinx_highlight.js` & `ypricemagic-3.4.9/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/docs/conf.py` & `ypricemagic-3.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/docs/make.bat` & `ypricemagic-3.4.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/scripts/debug-curve.py` & `ypricemagic-3.4.9/scripts/debug-curve.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/scripts/debug-price.py` & `ypricemagic-3.4.9/scripts/debug-price.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/setup.py` & `ypricemagic-3.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/tests/classes/test_erc20.py` & `ypricemagic-3.4.9/tests/classes/test_erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/tests/classes/test_singleton.py` & `ypricemagic-3.4.9/tests/classes/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/tests/fixtures.py` & `ypricemagic-3.4.9/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/tests/prices/dex/test_balancer.py` & `ypricemagic-3.4.9/tests/prices/dex/test_balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/tests/prices/dex/test_uniswap.py` & `ypricemagic-3.4.9/tests/prices/dex/test_uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/tests/prices/lending/test_aave.py` & `ypricemagic-3.4.9/tests/prices/lending/test_aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/tests/prices/lending/test_compound.py` & `ypricemagic-3.4.9/tests/prices/lending/test_compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/tests/prices/test_chainlink.py` & `ypricemagic-3.4.9/tests/prices/test_chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/tests/prices/test_magic.py` & `ypricemagic-3.4.9/tests/prices/test_magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/tests/prices/test_popsicle.py` & `ypricemagic-3.4.9/tests/prices/test_popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/tests/prices/test_synthetix.py` & `ypricemagic-3.4.9/tests/prices/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/tests/prices/test_yearn.py` & `ypricemagic-3.4.9/tests/prices/test_yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/tests/prices/utils/test_buckets.py` & `ypricemagic-3.4.9/tests/prices/utils/test_buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/ENVIRONMENT_VARIABLES.py` & `ypricemagic-3.4.9/y/ENVIRONMENT_VARIABLES.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/__init__.py` & `ypricemagic-3.4.9/y/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/_db/__init__.py` & `ypricemagic-3.4.9/y/_db/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/_db/common.py` & `ypricemagic-3.4.9/y/_db/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/_db/config.py` & `ypricemagic-3.4.9/y/_db/config.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/_db/decorators.py` & `ypricemagic-3.4.9/y/_db/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/_db/entities.py` & `ypricemagic-3.4.9/y/_db/entities.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/_db/exceptions.py` & `ypricemagic-3.4.9/y/_db/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/_db/structs.py` & `ypricemagic-3.4.9/y/_db/structs.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/_db/utils/_ep.py` & `ypricemagic-3.4.9/y/_db/utils/_ep.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/_db/utils/bulk.py` & `ypricemagic-3.4.9/y/_db/utils/bulk.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/_db/utils/contract.py` & `ypricemagic-3.4.9/y/_db/utils/contract.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/_db/utils/logs.py` & `ypricemagic-3.4.9/y/_db/utils/logs.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/_db/utils/price.py` & `ypricemagic-3.4.9/y/_db/utils/price.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/_db/utils/token.py` & `ypricemagic-3.4.9/y/_db/utils/token.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/_db/utils/traces.py` & `ypricemagic-3.4.9/y/_db/utils/traces.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/_db/utils/utils.py` & `ypricemagic-3.4.9/y/_db/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/classes/common.py` & `ypricemagic-3.4.9/y/classes/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/classes/singleton.py` & `ypricemagic-3.4.9/y/classes/singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/constants.py` & `ypricemagic-3.4.9/y/constants.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/contracts.py` & `ypricemagic-3.4.9/y/contracts.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/datatypes.py` & `ypricemagic-3.4.9/y/datatypes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/decorators.py` & `ypricemagic-3.4.9/y/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/erc20.py` & `ypricemagic-3.4.9/y/erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/exceptions.py` & `ypricemagic-3.4.9/y/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/interfaces/ERC20.py` & `ypricemagic-3.4.9/y/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/interfaces/balancer/WeightedPool.py` & `ypricemagic-3.4.9/y/interfaces/balancer/WeightedPool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/interfaces/compound/unitroller.py` & `ypricemagic-3.4.9/y/interfaces/compound/unitroller.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/interfaces/curve/CurveRegistry.py` & `ypricemagic-3.4.9/y/interfaces/curve/CurveRegistry.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/interfaces/multicall2.py` & `ypricemagic-3.4.9/y/interfaces/multicall2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/interfaces/uniswap/factoryv2.py` & `ypricemagic-3.4.9/y/interfaces/uniswap/factoryv2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/interfaces/uniswap/quoterv3.py` & `ypricemagic-3.4.9/y/interfaces/uniswap/quoterv3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/interfaces/uniswap/velov2.py` & `ypricemagic-3.4.9/y/interfaces/uniswap/velov2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/networks.py` & `ypricemagic-3.4.9/y/networks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/band.py` & `ypricemagic-3.4.9/y/prices/band.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/chainlink.py` & `ypricemagic-3.4.9/y/prices/chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/convex.py` & `ypricemagic-3.4.9/y/prices/convex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/dex/balancer/balancer.py` & `ypricemagic-3.4.9/y/prices/dex/balancer/balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/dex/balancer/v1.py` & `ypricemagic-3.4.9/y/prices/dex/balancer/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/dex/balancer/v2.py` & `ypricemagic-3.4.9/y/prices/dex/balancer/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/dex/genericamm.py` & `ypricemagic-3.4.9/y/prices/dex/genericamm.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/dex/mooniswap.py` & `ypricemagic-3.4.9/y/prices/dex/mooniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/dex/solidly.py` & `ypricemagic-3.4.9/y/prices/dex/solidly.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/dex/uniswap/uniswap.py` & `ypricemagic-3.4.9/y/prices/dex/uniswap/uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/dex/uniswap/v1.py` & `ypricemagic-3.4.9/y/prices/dex/uniswap/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/dex/uniswap/v2.py` & `ypricemagic-3.4.9/y/prices/dex/uniswap/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/dex/uniswap/v2_forks.py` & `ypricemagic-3.4.9/y/prices/dex/uniswap/v2_forks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/dex/uniswap/v3.py` & `ypricemagic-3.4.9/y/prices/dex/uniswap/v3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/dex/velodrome.py` & `ypricemagic-3.4.9/y/prices/dex/velodrome.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/eth_derivs/creth.py` & `ypricemagic-3.4.9/y/prices/eth_derivs/creth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/eth_derivs/wsteth.py` & `ypricemagic-3.4.9/y/prices/eth_derivs/wsteth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/gearbox.py` & `ypricemagic-3.4.9/y/prices/gearbox.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/lending/aave.py` & `ypricemagic-3.4.9/y/prices/lending/aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/lending/compound.py` & `ypricemagic-3.4.9/y/prices/lending/compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/lending/ib.py` & `ypricemagic-3.4.9/y/prices/lending/ib.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/magic.py` & `ypricemagic-3.4.9/y/prices/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/one_to_one.py` & `ypricemagic-3.4.9/y/prices/one_to_one.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/popsicle.py` & `ypricemagic-3.4.9/y/prices/popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/rkp3r.py` & `ypricemagic-3.4.9/y/prices/rkp3r.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/solidex.py` & `ypricemagic-3.4.9/y/prices/solidex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/stable_swap/belt.py` & `ypricemagic-3.4.9/y/prices/stable_swap/belt.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/stable_swap/curve.py` & `ypricemagic-3.4.9/y/prices/stable_swap/curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,14 +425,16 @@
             return await Contract.coroutine(factory)
         except StopIteration:
             return None    
     
     @a_sync.a_sync(cache_type='memory')
     async def get_price(self, token: Address, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Optional[float]:
         pool = await self.get_pool(token, sync=False)
+        if pool is None:
+            return None
         tvl = await pool.get_tvl(block=block, skip_cache=skip_cache, sync=False)
         if tvl is None:
             return None
         return tvl / await ERC20(token, asynchronous=True).total_supply_readable(block)
 
     @a_sync.a_sync(cache_type='memory')
     async def get_pool(self, token: AnyAddressType) -> CurvePool:
```

### Comparing `ypricemagic-3.4.8/y/prices/stable_swap/ellipsis.py` & `ypricemagic-3.4.9/y/prices/stable_swap/ellipsis.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/stable_swap/froyo.py` & `ypricemagic-3.4.9/y/prices/stable_swap/froyo.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/stable_swap/mstablefeederpool.py` & `ypricemagic-3.4.9/y/prices/stable_swap/mstablefeederpool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/stable_swap/saddle.py` & `ypricemagic-3.4.9/y/prices/stable_swap/saddle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/synthetix.py` & `ypricemagic-3.4.9/y/prices/synthetix.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import asyncio
 import logging
-from typing import List, Optional
+from typing import Callable, List, Optional
 
 import a_sync
 from a_sync.property import HiddenMethodDescriptor
 from brownie import chain
 from brownie.convert.datatypes import EthAddress, HexString
-try:
-    from eth_abi import encode
-except ImportError:
-    from eth_abi import encode_single as encode
 from multicall import Call
 from typing_extensions import Self
 
 from y import convert
 from y import ENVIRONMENT_VARIABLES as ENVS
 from y.contracts import Contract, has_method
 from y.datatypes import AnyAddressType, Block, UsdPrice
 from y.exceptions import UnsupportedNetwork, call_reverted
 from y.networks import Network
 
+try:
+    from eth_abi import encode
+    encode_bytes: Callable[[str], bytes] = lambda s: encode(["bytes32"], [s.encode()])
+except ImportError:
+    from eth_abi import encode_single
+    encode_bytes: Callable[[str], bytes] = lambda s: encode_single("bytes32", s.encode())
+
 logger = logging.getLogger(__name__)
 
 addresses = {
     Network.Mainnet: '0x823bE81bbF96BEc0e25CA13170F5AaCb5B79ba83',
     Network.Optimism: '0x95A6a3f44a70172E7d50a9e28c85Dfd712756B8C',
 }
 
@@ -43,15 +46,16 @@
     @a_sync.a_sync(ram_cache_maxsize=256)
     async def get_address(self, name: str, block: Block = None) -> Contract:
         """
         Get contract from Synthetix registry.
         See also https://docs.synthetix.io/addresses/
         """
         address_resolver = await self.__address_resolver__
-        address = await address_resolver.getAddress.coroutine(encode(['bytes32'], name.encode()), block_identifier=block)
+        key = encode_bytes(name)
+        address = await address_resolver.getAddress.coroutine(key, block_identifier=block)
         proxy = await Contract.coroutine(address)
         return await Contract.coroutine(await proxy.target.coroutine(block_identifier=block)) if hasattr(proxy, 'target') else proxy
 
     @a_sync.aka.cached_property
     async def synths(self) -> List[EthAddress]:
         """
         Get target addresses of all synths.
```

### Comparing `ypricemagic-3.4.8/y/prices/tokenized_fund/basketdao.py` & `ypricemagic-3.4.9/y/prices/tokenized_fund/basketdao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/tokenized_fund/gelato.py` & `ypricemagic-3.4.9/y/prices/tokenized_fund/gelato.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/tokenized_fund/piedao.py` & `ypricemagic-3.4.9/y/prices/tokenized_fund/piedao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/tokenized_fund/tokensets.py` & `ypricemagic-3.4.9/y/prices/tokenized_fund/tokensets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/utils/buckets.py` & `ypricemagic-3.4.9/y/prices/utils/buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/utils/sense_check.py` & `ypricemagic-3.4.9/y/prices/utils/sense_check.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/utils/ypriceapi.py` & `ypricemagic-3.4.9/y/prices/utils/ypriceapi.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/prices/yearn.py` & `ypricemagic-3.4.9/y/prices/yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/time.py` & `ypricemagic-3.4.9/y/time.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/utils/client.py` & `ypricemagic-3.4.9/y/utils/client.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/utils/events.py` & `ypricemagic-3.4.9/y/utils/events.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/utils/fakes.py` & `ypricemagic-3.4.9/y/utils/fakes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/utils/gather.py` & `ypricemagic-3.4.9/y/utils/gather.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/utils/logging.py` & `ypricemagic-3.4.9/y/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/utils/middleware.py` & `ypricemagic-3.4.9/y/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/utils/multicall.py` & `ypricemagic-3.4.9/y/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/y/utils/raw_calls.py` & `ypricemagic-3.4.9/y/utils/raw_calls.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/ypricemagic/magic.py` & `ypricemagic-3.4.9/ypricemagic/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.8/ypricemagic.egg-info/PKG-INFO` & `ypricemagic-3.4.9/ypricemagic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ypricemagic
-Version: 3.4.8
+Version: 3.4.9
 Summary: Use this tool to extract historical on-chain price data from an archive node. Shoutout to @bantg and @nymmrx for their awesome work on yearn-exporter that made this library possible.
 Home-page: https://github.com/BobTheBuidler/ypricemagic
 Author: BobTheBuidler
 Author-email: bobthebuidlerdefi@gmail.com
 License: MIT
 License-File: LICENSE.txt
 Requires-Dist: bobs_lazy_logging==0.0.4
```

### Comparing `ypricemagic-3.4.8/ypricemagic.egg-info/SOURCES.txt` & `ypricemagic-3.4.9/ypricemagic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

