# Comparing `tmp/EclipsingBinaries-4.0.8.tar.gz` & `tmp/eclipsingbinaries-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-4.0.8.tar", last modified: Fri Apr  5 18:41:31 2024, max compression
+gzip compressed data, was "eclipsingbinaries-4.1.0.tar", last modified: Sat Apr 20 03:10:47 2024, max compression
```

## Comparing `EclipsingBinaries-4.0.8.tar` & `eclipsingbinaries-4.1.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:31.387123 EclipsingBinaries-4.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:31.367123 EclipsingBinaries-4.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:31.371123 EclipsingBinaries-4.0.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:31.371123 EclipsingBinaries-4.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/.github/workflows/ci_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)   112224 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:31.375123 EclipsingBinaries-4.0.8/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (127)    24730 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    22282 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (127)    31253 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/color_light_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:31.383123 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/APASS_Catalog_ex.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/Gaia_output.txt
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/O-C_paper_table.txt
--rw-r--r--   0 runner    (1001) docker     (127)    85904 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/OConnell_plot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/OConnell_table.txt
--rw-r--r--   0 runner    (1001) docker     (127)    48237 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/O_C_ex.png
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:41:15.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:31.383123 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/calibration_images/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/calibration_images/purpose.txt
--rw-r--r--   0 runner    (1001) docker     (127)   135237 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/color_light_curve_ex.png
--rw-r--r--   0 runner    (1001) docker     (127)    35357 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/example_OC_table.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/example_regression.txt
--rw-r--r--   0 runner    (1001) docker     (127)   118184 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/gui_color_light.png
--rw-r--r--   0 runner    (1001) docker     (127)   109712 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/light_curve_ex.png
--rw-r--r--   0 runner    (1001) docker     (127)   136591 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/min_program_demo.png
--rw-r--r--   0 runner    (1001) docker     (127)   131114 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/overlay_example.png
--rw-r--r--   0 runner    (1001) docker     (127)    31361 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/test_B.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25814 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/test_R.txt
--rw-r--r--   0 runner    (1001) docker     (127)    30132 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/test_V.txt
--rw-r--r--   0 runner    (1001) docker     (127)    39669 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/examples/test_minimums.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25259 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    16127 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/multi_aperture_photometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/tess_ccd_info.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/tesscut.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:31.383123 EclipsingBinaries-4.0.8/EclipsingBinaries/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/tests/test_IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/tests/test_OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/tests/test_apass.py
--rw-r--r--   0 runner    (1001) docker     (127)    81825 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:31.387123 EclipsingBinaries-4.0.8/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-05 18:41:27.000000 EclipsingBinaries-4.0.8/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-05 18:41:31.000000 EclipsingBinaries-4.0.8/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:41:27.000000 EclipsingBinaries-4.0.8/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-05 18:41:27.000000 EclipsingBinaries-4.0.8/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:41:27.000000 EclipsingBinaries-4.0.8/EclipsingBinaries.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-05 18:41:27.000000 EclipsingBinaries-4.0.8/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 18:41:27.000000 EclipsingBinaries-4.0.8/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-05 18:41:31.387123 EclipsingBinaries-4.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:31.383123 EclipsingBinaries-4.0.8/changelog/
--rw-r--r--   0 runner    (1001) docker     (127)   222548 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/changelog/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/changelog/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:31.383123 EclipsingBinaries-4.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/docs/EB.rst
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:31.371123 EclipsingBinaries-4.0.8/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:31.387123 EclipsingBinaries-4.0.8/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/docs/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)    24030 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/docs/toolbox.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-05 18:41:31.387123 EclipsingBinaries-4.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-05 18:41:19.000000 EclipsingBinaries-4.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:10:47.585421 eclipsingbinaries-4.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:10:47.569421 eclipsingbinaries-4.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:10:47.573421 eclipsingbinaries-4.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:10:47.573421 eclipsingbinaries-4.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/.github/workflows/ci_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   112224 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:10:47.577421 eclipsingbinaries-4.1.0/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (127)    25998 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22282 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31253 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/color_light_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:10:47.581421 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/APASS_Catalog_ex.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/Gaia_output.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/O-C_paper_table.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    85904 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/OConnell_plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/OConnell_table.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    48237 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/O_C_ex.png
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 03:10:31.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:10:47.581421 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/calibration_images/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/calibration_images/purpose.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   135237 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/color_light_curve_ex.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35357 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/example_OC_table.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/example_regression.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   118184 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/gui_color_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)   109712 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/light_curve_ex.png
+-rw-r--r--   0 runner    (1001) docker     (127)   136591 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/min_program_demo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   131114 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/overlay_example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31361 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/test_B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25814 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/test_R.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    30132 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/test_V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    39669 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/examples/test_minimums.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25329 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16127 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/multi_aperture_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/tess_ccd_info.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/tesscut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:10:47.581421 eclipsingbinaries-4.1.0/EclipsingBinaries/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/tests/test_IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/tests/test_OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/tests/test_apass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54298 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:10:47.585421 eclipsingbinaries-4.1.0/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-20 03:10:43.000000 eclipsingbinaries-4.1.0/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-20 03:10:47.000000 eclipsingbinaries-4.1.0/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 03:10:43.000000 eclipsingbinaries-4.1.0/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-20 03:10:43.000000 eclipsingbinaries-4.1.0/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 03:10:43.000000 eclipsingbinaries-4.1.0/EclipsingBinaries.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-20 03:10:43.000000 eclipsingbinaries-4.1.0/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-20 03:10:43.000000 eclipsingbinaries-4.1.0/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-20 03:10:47.585421 eclipsingbinaries-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:10:47.581421 eclipsingbinaries-4.1.0/changelog/
+-rw-r--r--   0 runner    (1001) docker     (127)   222548 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/changelog/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/changelog/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:10:47.585421 eclipsingbinaries-4.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/docs/EB.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:10:47.569421 eclipsingbinaries-4.1.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:10:47.585421 eclipsingbinaries-4.1.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/docs/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    24030 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/docs/toolbox.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-20 03:10:47.585421 eclipsingbinaries-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-20 03:10:35.000000 eclipsingbinaries-4.1.0/tox.ini
```

### Comparing `EclipsingBinaries-4.0.8/.github/ISSUE_TEMPLATE/bug_report.md` & `eclipsingbinaries-4.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/.github/ISSUE_TEMPLATE/feature_request.md` & `eclipsingbinaries-4.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/.github/workflows/ci_tests.yml` & `eclipsingbinaries-4.1.0/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/.github/workflows/python-publish.yml` & `eclipsingbinaries-4.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/CHANGELOG.md` & `eclipsingbinaries-4.1.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/CODE_OF_CONDUCT.md` & `eclipsingbinaries-4.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/IRAF_Reduction.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/IRAF_Reduction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Author: Kyle Koeller
 Created: 11/08/2022
-Last Edited: 06/17/2023
+Last Edited: 04/19/2024
 
 This program is meant to automatically do the data reduction of the raw images from the
 Ball State University Observatory (BSUO) and SARA data. The new calibrated images are placed into a new folder as to
 not overwrite the original images.
 """
 # import sys
 from pathlib import Path
@@ -28,23 +28,23 @@
 # "The warning raised when the contents of the FITS header have been modified to be standards compliant."
 warnings.filterwarnings("ignore", category=wcs.FITSFixedWarning)
 
 # global variables for combining, to either play with or set depending on the run
 sigma_clip_low_thresh = None
 sigma_clip_high_thresh = 3
 sigclip = 5  # sigclip for cosmic ray removal
-rdnoise = 10.83  # * u.electron  # gathered from fits headers manually
-gain = 1.43  # * u.electron / u.adu  # gathered from fits headers manually
+# rdnoise = 10.83  # * u.electron  # gathered from fits headers manually
+# gain = 1.43  # * u.electron / u.adu  # gathered from fits headers manually
 overwrite = True  # if the user wants to overwrite already existing files or not, by default it is set to True
-mem_limit = 1600e6  # maximum memory limit 4.5 Gb is the recommended which is 450e6 (i.e. 8.0 Gb would be 800e6)
+# mem_limit = 1600e6  # maximum memory limit 4.5 Gb is the recommended which is 450e6 (i.e. 8.0 Gb would be 800e6)
 dark_bool = "True"
-location = "bsuo"
+# location = "bsuo"
 
 
-def main(path="", calibrated="", pipeline=False, location="", dark_bool=True):
+def main(path="", calibrated="", pipeline=False, location="", dark_bool=True, gain=1.43, rdnoise=10.83, mem_limit=450e6):
     """
     This function calls all other functions in order of the calibration.
 
     :param path: the path to the raw images
     :param calibrated: the path to the calibrated images
     :param pipeline: if the user wants to use the pipeline or not
     :param location: the location of the telescope
@@ -71,19 +71,19 @@
                 break
             except FileNotFoundError:
                 print("Files were not found. Please try again.\n")
                 path = input("Please enter a file path or folder name (if this code is in the same main folder): ")
                 calibrated = input("Please enter a name for a new calibrated folder to not overwrite the original images: ")
 
         if location.lower() == "kpno":
-            kpno()
+            gain, rdnoise = kpno()
         elif location.lower() == "ctio":
-            ctio()
-        elif lapalma():
-            lapalma()
+            gain, rdnoise = ctio()
+        elif location.lower() == "lapalma":
+            gain, rdnoise = lapalma()
         elif location.lower() == "bsuo":
             pass
         else:
             print("\nDo you want to load default options like gain and read noise? The defaults are for BSUO")
             while True:
                 default_ans = input("To load defaults type 'Default' otherwise type 'New' to enter values: ")
                 # default_ans = "default"
@@ -94,21 +94,21 @@
                     break
                 else:
                     print("Please either enter 'Default' or 'New'.\n")
 
         calibrated_data.mkdir(exist_ok=True)
         files = ccdp.ImageFileCollection(images_path)
 
-        zero, overscan_region, trim_region = bias(files, calibrated_data, path, pipeline)
+        zero, overscan_region, trim_region = bias(files, calibrated_data, path, pipeline, mem_limit, gain)
         if not dark_bool:
             master_dark = None
         else:
-            master_dark = dark(files, zero, calibrated_data, overscan_region, trim_region)
+            master_dark = dark(files, zero, calibrated_data, overscan_region, trim_region, gain, rdnoise, mem_limit)
 
-        flat(files, zero, master_dark, calibrated_data, overscan_region, trim_region)
+        flat(files, zero, master_dark, calibrated_data, overscan_region, trim_region, gain, rdnoise, mem_limit)
         science_images(files, calibrated_data, zero, master_dark, trim_region, overscan_region)
     else:
         # checks whether the file paths from above are real
         while True:
             try:
                 images_path = Path(path)
                 calibrated_data = Path(calibrated)
@@ -119,87 +119,85 @@
                 calibrated = input(
                     "Please enter a name for a new calibrated folder to not overwrite the original images: ")
 
         if location.lower() == "kpno":
             kpno()
         elif location.lower() == "ctio":
             ctio()
-        elif lapalma():
+        elif location.lower() == "lapalma":
             lapalma()
         elif location.lower() == "bsuo":
             pass
 
         calibrated_data.mkdir(exist_ok=True)
         files = ccdp.ImageFileCollection(images_path)
 
-        zero, overscan_region, trim_region = bias(files, calibrated_data, path, pipeline)
+        zero, overscan_region, trim_region = bias(files, calibrated_data, path, pipeline, mem_limit, gain)
         if not dark_bool:
             master_dark = None
         else:
-            master_dark = dark(files, zero, calibrated_data, overscan_region, trim_region)
+            master_dark = dark(files, zero, calibrated_data, overscan_region, trim_region, gain, rdnoise, mem_limit)
 
-        flat(files, zero, master_dark, calibrated_data, overscan_region, trim_region)
+        flat(files, zero, master_dark, calibrated_data, overscan_region, trim_region, gain, rdnoise, mem_limit)
         science_images(files, calibrated_data, zero, master_dark, trim_region, overscan_region)
 
 # more observatory sites can be found here: https://github.com/astropy/astropy-data/blob/gh-pages/coordinates/sites.json
 def kpno():
     """
     Kitt Peak National Observatory default values
 
-    :return: None
+    :return: Camera characteristics
     """
-    global gain
-    global rdnoise
     global dark_bool
-
+    
     gain = 2.3
     rdnoise = 6.0
     dark_bool = True
 
+    return gain, rdnoise
+
 
 def ctio():
     """
     Cerro Tololo Inter-American Observatory default values
 
-    :return: None
+    :return: Camera characteristics
     """
-    global gain
-    global rdnoise
     global dark_bool
 
     gain = 2.0
     rdnoise = 9.7
     dark_bool = True
 
+    return gain, rdnoise
+
 
 def lapalma():
     """
     La Palma default values
 
-    :return: None
+    :return: Camera characteristics
     """
-    global gain
-    global rdnoise
     global dark_bool
 
     gain = 1.0
     rdnoise = 6.3
     dark_bool = True
 
+    return gain, rdnoise
+
 
 def new_default():
     """
     Generates new values that the user can enter
 
     :return: newly entered default values
     """
     global sigma_clip_high_thresh
     global sigma_clip_low_thresh
-    global gain
-    global rdnoise
     global sigclip
     global dark_bool
     global location
 
     sigma_clip_low_thresh = (input("\nEnter a sigma clip low threshold, default is 'None': "))
     if sigma_clip_low_thresh.lower() == "none":
         sigma_clip_low_thresh = None
@@ -212,27 +210,32 @@
     dark_bool = input("Are you using Dark Frames, default is True (enter 'True' or 'False'): ")
     if dark_bool.lower == "false":
         dark_bool = False
     elif dark_bool.lower == "true":
         dark_bool = True
     location = input("What is your observation location, default is bsuo (ctio, kpno, lapalma")
 
+    return gain, rdnoise, dark_bool
 
-def reduce(ccd, overscan_region, trim_region, num, zero, combined_dark, good_flat):
+
+def reduce(ccd, overscan_region, trim_region, num, zero, combined_dark, good_flat, gain=gain, rdnoise=rdnoise):
     """
     This function takes the information for each section of the reduction process into a singular function for
     limits in duplication of the code.
 
     :param ccd: individual image
     :param overscan_region: the overscan region of the image
     :param trim_region: region of the image to trim
     :param num: tells the program what stage of the process it is in
     :param zero: master bias
     :param combined_dark: master dark
     :param good_flat: master flat
+    :param gain: gain of the camera
+    :param rdnoise: readout noise of the camera
+
     :return: depends on the stage of process, but will return a final image for each process
     """
 
     # subtract overscan, trims image, and gain corrects
     if overscan_region.lower() == "none":
         pass
     else:
@@ -285,22 +288,24 @@
 
         # cosmic ray reject above 5 sigmas and gain_apply is set to false because it changes the units of the image
         # new_reduced = ccdp.cosmicray_lacosmic(reduced, gain_apply=False, readnoise=rdnoise, gain=gain, sigclip=sigclip)
 
         return reduced
 
 
-def bias(files, calibrated_data, path, pipeline):
+def bias(files, calibrated_data, path, pipeline, mem_limit, gain):
     """
     Calibrates the bias images
 
     :param path: the raw images folder path
     :param files: file location where all raw images are
     :param calibrated_data: file location where the new images go
     :param pipeline: true or false for pipeline usage
+    :param mem_limit: maximum memory chunk usage
+    :param gain: gain of the camera
 
     :return: the combined bias image and the trim and overscan regions
     """
 
     # plots one of the flat image mean count values across all columns to find the trim and overscan regions
     if not pipeline:
         print("\n\nThe flat image that you enter next should be inside the " + "\033[1m" + "\033[93m" + "FIRST" +
@@ -329,23 +334,24 @@
         print()
     else:
         overscan_region = "[2073:2115, :]"
         trim_region = "[20:2060, 12:2057]"
 
     print("\nStarting overscan on bias.\n")
     for ccd, file_name in files.ccds(imagetyp='BIAS', return_fname=True, ccd_kwargs={'unit': 'adu'}):
-        new_ccd = reduce(ccd, overscan_region, trim_region, 0, zero=None, combined_dark=None, good_flat=None)
+        new_ccd = reduce(ccd, overscan_region, trim_region, 0, zero=None, combined_dark=None, good_flat=None, gain=gain, rdnoise=rdnoise)
 
         list_of_words = file_name.split(".")
         new_fname = "{}.fits".format(list_of_words[0])
 
         # Save the result
         new_ccd.write(calibrated_data / new_fname, overwrite=overwrite)
 
-        add_header(calibrated_data, new_fname, "BIAS", "None", None, None, None, trim_region, overscan_region)
+        add_header(calibrated_data, new_fname, "BIAS", "None", None, None, None,
+                   trim_region, overscan_region, gain, rdnoise)
 
         # output that an image is finished for updates to the user
         print("Finished overscan correction for " + str(new_fname))
 
     print("\nFinished overscan correcting bias frames.")
     # combine all the output bias images into a master bias
     reduced_images = ccdp.ImageFileCollection(calibrated_data)
@@ -359,15 +365,16 @@
                                  mem_limit=mem_limit
                                  )
 
     fname = "zero.fits"
     combined_bias.meta['combined'] = True
     combined_bias.write(calibrated_data / fname, overwrite=overwrite)
 
-    add_header(calibrated_data, fname, "BIAS", "None", None, None, None, trim_region, overscan_region)
+    add_header(calibrated_data, fname, "BIAS", "None", None, None, None,
+               trim_region, overscan_region, gain, rdnoise)
 
     print("\nFinished creating zero.fits\n")
 
     return combined_bias, overscan_region, trim_region
 
 
 def bias_plot(ccd):
@@ -386,38 +393,43 @@
     plt.xlim(-50, 2130)
     plt.xlabel('pixel number')
     plt.ylabel('Counts')
     # plt.title('Count Values for Row 1000')
     # plt.show()
 
 
-def dark(files, zero, calibrated_path, overscan_region, trim_region):
+def dark(files, zero, calibrated_path, overscan_region, trim_region, gain, rdnoise, mem_limit):
     """
     Calibrates the dark frames.
 
     :param files: file location of raw images
     :param zero: master bias image
     :param calibrated_path: file location for the new images
     :param trim_region: trim region for images
     :param overscan_region: overscan region for images
+    :param mem_limit: maximum memory chunk usage
+    :param gain: gain of the camera
+    :param rdnoise: readout noise of the camera
+
     :return: combined master dark
     """
     print("Starting dark calibration.\n")
     # calibrating a combining the dark frames
     for ccd, file_name in files.ccds(imagetyp='DARK', ccd_kwargs={'unit': 'adu'}, return_fname=True):
-        sub_ccd = reduce(ccd, overscan_region, trim_region, 1, zero, combined_dark=None, good_flat=None)
+        sub_ccd = reduce(ccd, overscan_region, trim_region, 1, zero, combined_dark=None, good_flat=None, gain=gain, rdnoise=rdnoise)
 
         # new file name that uses the number from the original image
         list_of_words = file_name.split(".")
         new_fname = "{}.fits".format(list_of_words[0])
 
         # Save the result
         sub_ccd.write(calibrated_path / new_fname, overwrite=overwrite)
 
-        add_header(calibrated_path, new_fname, "DARK", "None", None, None, None, trim_region, overscan_region)
+        add_header(calibrated_path, new_fname, "DARK", "None", None, None, None,
+                   trim_region, overscan_region, gain, rdnoise)
 
         print("Finished overscan correction and bias subtraction for " + str(new_fname))
 
     print("\nFinished overscan correcting and bias subtracting all dark frames.")
     print("\nStarting combining dark frames.\n")
     time.sleep(10)
     reduced_images = ccdp.ImageFileCollection(calibrated_path)
@@ -431,46 +443,52 @@
                                  rdnoise=rdnoise * u.electron, gain=gain * u.electron / u.adu, mem_limit=mem_limit
                                  )
 
     fname = "master_dark.fits"
     combined_dark.meta['combined'] = True
     combined_dark.write(calibrated_path / fname, overwrite=overwrite)
 
-    add_header(calibrated_path, fname, "DARK", "None", None, None, None, trim_region, overscan_region)
+    add_header(calibrated_path, fname, "DARK", "None", None, None, None,
+               trim_region, overscan_region, gain, rdnoise)
 
     print("Finished creating a master dark.\n")
     return combined_dark
 
 
-def flat(files, zero, combined_dark, calibrated_path, overscan_region, trim_region):
+def flat(files, zero, combined_dark, calibrated_path, overscan_region, trim_region, gain, rdnoise, mem_limit):
     """
     Calibrate flat images.
 
     :param files: file location for raw images
     :param zero: combined bias image
     :param combined_dark: combined bias image
     :param calibrated_path: file location for new images
     :param trim_region: trim region for images
     :param overscan_region: overscan region for images
+    :param mem_limit: maximum memory chunk usage
+    :param gain: gain of the camera
+    :param rdnoise: readout noise of the camera
+
     :return: master flat files in each filter
     """
     print("Starting flat calibration.\n")
 
     # calibrating and combining the flat frames
     for ccd, file_name in files.ccds(imagetyp='FLAT', return_fname=True, ccd_kwargs={'unit': 'adu'}):
-        final_ccd = reduce(ccd, overscan_region, trim_region, 2, zero, combined_dark, good_flat=None)
+        final_ccd = reduce(ccd, overscan_region, trim_region, 2, zero, combined_dark, good_flat=None, gain=gain, rdnoise=rdnoise)
 
         # new file name with the filter and number from the original file
         list_of_words = file_name.split(".")
         new_fname = "{}.fits".format(list_of_words[0])
 
         # Save the result
         final_ccd.write(calibrated_path / new_fname, overwrite=overwrite)
 
-        add_header(calibrated_path, new_fname, "FLAT", "None", None, None, None, trim_region, overscan_region)
+        add_header(calibrated_path, new_fname, "FLAT", "None", None, None, None,
+                   trim_region, overscan_region, gain, rdnoise)
 
         print("Finished overscan correction, bias subtraction, and dark subtraction for " + str(new_fname))
 
     print("\nFinished overscan, bias subtracting, and dark subtracting of flat frames.\n")
     print("Starting flat combination.\n")
     time.sleep(10)
 
@@ -487,15 +505,16 @@
                                       )
 
         combined_flats.meta['combined'] = True
         flat_file_name = 'master_flat_{}.fits'.format(filt.replace("Empty/", ""))
 
         combined_flats.write(calibrated_path / flat_file_name, overwrite=overwrite)
 
-        add_header(calibrated_path, flat_file_name, "FLAT", "None", None, None, None, trim_region, overscan_region)
+        add_header(calibrated_path, flat_file_name, "FLAT", "None", None, None, None,
+                   trim_region, overscan_region, gain, rdnoise)
 
         print("Finished combining flat " + str(flat_file_name))
 
     print("\nFinished creating the master flats by filter.\n")
 
 
 def science_images(files, calibrated_data, zero, combined_dark, trim_region, overscan_region):
@@ -506,45 +525,48 @@
     ifc_reduced = ccdp.ImageFileCollection(calibrated_data)
     combined_flats = {ccd.header['filter']: ccd for ccd in ifc_reduced.ccds(imagetyp=flat_imagetyp, combined=True)}
 
     print("Starting reduction of science images.\n")
 
     for light, file_name in files.ccds(imagetyp=science_imagetyp, return_fname=True, ccd_kwargs={'unit': 'adu'}):
         good_flat = combined_flats[light.header['filter']]
-        reduced = reduce(light, overscan_region, trim_region, 3, zero, combined_dark, good_flat)
+        reduced = reduce(light, overscan_region, trim_region, 3, zero, combined_dark, good_flat, gain=gain, rdnoise=rdnoise)
 
         list_of_words = file_name.split(".")
         new_fname = "{}.fits".format(list_of_words[0])
 
         all_reds.append(reduced)
         reduced.write(calibrated_data / new_fname, overwrite=overwrite)
 
         hjd = light.header["JD-HELIO"]
         ra = light.header["RA"]
         dec = light.header["DEC"]
 
-        add_header(calibrated_data, new_fname, science_imagetyp, "None", hjd, ra, dec, trim_region, overscan_region)
+        add_header(calibrated_data, new_fname, science_imagetyp, "None", hjd, ra, dec, trim_region, overscan_region, gain, rdnoise)
 
         print("Finished calibration of " + str(new_fname))
     print("\nFinished calibrating all science images.")
 
 
-def add_header(pathway, fname, imagetyp, filter_name, hjd, ra, dec, trim_region, overscan_region):
+def add_header(pathway, fname, imagetyp, filter_name, hjd, ra, dec, trim_region, overscan_region, gain, rdnoise):
     """
     Adds values to the header of each image reduced
 
     :param overscan_region: BIASSEC for the header
     :param trim_region: DATASEC for the header
     :param dec: declination of target object
     :param ra: right ascension of target object
     :param hjd: time of mid-exposure for each image
     :param pathway: pathway to the new file
     :param fname: file name
     :param imagetyp: image type (bias, flat, dark, light)
     :param filter_name: filter type (B, V, R)
+    :param gain: gain of the camera
+    :param rdnoise: readout noise of the camera
+
     :return: None
     """
     # bias_image = get_pkg_data_filename(pathway + "\\" + fname)
     image_name = pathway / fname
     fits.setval(image_name, "GAIN", value=gain, comment="Units of e-/ADU")
     fits.setval(image_name, "RDNOISE", value=rdnoise, comment="UNits of e-")
     fits.setval(image_name, "OBSERVAT", value=location, comment="Obs. Loc.")
```

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/Night_Filters.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/OC_plot.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/OConnell.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/apass.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/apass.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/color_light_curve.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/color_light_curve.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/APASS_Catalog_ex.txt` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/APASS_Catalog_ex.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/O-C_paper_table.txt` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/O-C_paper_table.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/OConnell_plot.png` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/OConnell_plot.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/OConnell_table.txt` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/OConnell_table.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/O_C_ex.png` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/O_C_ex.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/color_light_curve_ex.png` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/color_light_curve_ex.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/example_OC_table.txt` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/example_OC_table.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/example_regression.txt` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/example_regression.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/gui_color_light.png` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/gui_color_light.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/light_curve_ex.png` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/light_curve_ex.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/min_program_demo.png` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/min_program_demo.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/overlay_example.png` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/overlay_example.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/test_B.txt` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/test_B.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/test_R.txt` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/test_R.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/test_V.txt` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/test_V.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/examples/test_minimums.txt` & `eclipsingbinaries-4.1.0/EclipsingBinaries/examples/test_minimums.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/find_min.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/find_min.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created:  07/03/2021
 Original Author: Alec Neal
 
 Last Edits Done By: Kyle Koeller
-Last Edited: 06/15/2023
+Last Edited: 04/19/2024
 """
 
 # from vseq_updated import calc, FT, io, plot  # testing purposes
 from .vseq_updated import calc, FT, io, plot
 from os import environ, path
 import matplotlib.pyplot as plt
 import numpy as np
@@ -75,15 +75,15 @@
         plot_obs(filter_files, day=day, lb=last_lb, rb=last_rb, order=order, resolution=resolution, npairs=npairs,
                  para_range=None, norm_method="norm")
     return bestroot
 
 
 def calc_S(fracHJD, flux, guess_min, npairs=None):
     # if interp == None:
-    interp = scipy.interpolate.interp1d(fracHJD, flux)
+    interp = scipy.interpolate.interp1d(fracHJD, flux, fill_value="extrapolate")
     max_range = min([guess_min - min(fracHJD), max(fracHJD) - guess_min])
     N = 0  # represents the total number of obs. in the range
     for time in fracHJD:
         if guess_min - max_range < time < guess_min + max_range:
             N += 1
     """
     K is the number of "paired" observations, and is a general measure
@@ -99,14 +99,15 @@
     # klist=np.arange(1,K+1,1)
     if npairs is None:
         npairs = 20
 
     # thing=100 # better signal with +10 but cheating?
     step = max_range / npairs
     klist = np.arange(1, npairs + 1, 1)
+    # print(guess_min)
     S = sum((interp(guess_min - klist * step) - interp(guess_min + klist * step)) ** 2)
 
     return S, K
 
 
 def KvW(fracHJD, flux, discard=0.1, resolution=100, para_range=None, plot=False,
         need_error=False, ax=None, npairs=20, entire_S=False):
@@ -188,15 +189,15 @@
             ax.set_ylim(min(paraS) - Srange * 0.07, max(paraS) + Srange * 0.07)
             ax.set_xlim(min(paraHJD) - HJDrange * 0.025, max(paraHJD) + HJDrange * 0.025)
 
         ax.plot(guesses, np.array(Slist), 'ok', ms=5)
         polyx, polyy = calc.poly.polylist(coef, min(paraHJD), max(paraHJD), 100)
         ax.plot(polyx, polyy, 'b', lw=1)
         # plt.plot(paraHJD,results,'b',lw=1,label=r'${S}^{\prime}$')
-        ax.axvline(T_kw, color='b', label=r'$T_{\rm KW}=' + str(round(T_kw, 6)) + '$', linewidth=1, ls='--')
+        ax.axvline(T_kw, color='b', label=r"$T_{\rm KW}=" + str(round(T_kw, 6)) + '$', linewidth=1, ls='--')
         # ax.axvline(best_min[1], color='gray', label=r'$T_{\rm BF}=' + str(round(best_min[1], 6)) + '$', linewidth=1,
         #            ls='-.')
 
         ax.set_ylabel(r'$S$', fontsize=fontsize, usetex=False)
         ax.legend(fontsize=7, loc='upper left', bbox_to_anchor=[0.1, 1.03], frameon=False).set_draggable(True)
         xt, yt = percent_to_xy((0.6, 0.8), paraHJD, ax.get_ylim())
         # strcoef = (coef / a).round(5)
@@ -330,15 +331,15 @@
         plt.rcParams.update(parameters)
 
         [Splot, MIN], fig = plot.multiplot(figsize=(5, 4), height_ratios=[1, 4], sharex=False, sharey=False,
                                                 hspace=0)
         MIN.errorbar(fracHJD, all_flux[day], all_fluxerr[day], fmt='ok', ms=3, capsize=3, elinewidth=0.6, ecolor='gray',
                      capthick=0.6)  # ,'ok',ms=3)
 
-        fig.canvas.mpl_connect('key_press_event', lambda event: press(event, Z))
+        fig.canvas.mpl_connect('key_press_event', lambda event: press(event, Z, filter_files))
         # fig.canvas.get_tk_widget().focus_force()
 
         HJD_inbounds, flux_inbounds, fluxerr_inbounds = [], [], []
         for n in range(len(all_HJD[day])):
             if lb < fracHJD[n] < rb:
                 HJD_inbounds.append(fracHJD[n])
                 flux_inbounds.append(all_flux[day][n])
@@ -407,17 +408,17 @@
         Splot.xaxis.tick_top()
 
         print('============================')
         print('T_KW:     ' + str(intday + t_kw))
         # totalerr = np.sqrt(sigt_kw ** 2 + kweeer ** 2)
         if sigt_kw != float(sigt_kw):
             MIN.axvline(t_kw, color='blue',
-                        label=r' $T_{\rm KW}=' + str(round(intday * 0 + t_kw, 6)) + '\pm$' + 'ERROR')
+                        label=r'$T_{\mathrm{KW}}=' + str(round(intday * 0 + t_kw, 6)) + '\pm$' + 'ERROR')
         else:
-            MIN.axvline(t_kw, color='blue', label=r' $  T_{\rm KW}=' + str(round(intday * 0 + t_kw, 6)) + '\pm' + str(
+            MIN.axvline(t_kw, color='blue', label=r'T_{\mathrm{KW}}=' + str(round(intday * 0 + t_kw, 6)) + '\pm' + str(
                 round(sigt_kw, 6)) + '$')
             print('err_kw:   ' + str(round(sigt_kw, 16)))
         print('')
         # print('T_LSQ:    ' + str(bestroot + intday))
         # print('err_form: ' + str(round(idkerror, 16)))
         # print('err_MC:   ' + str(round(root_error, 16)))
 
@@ -452,15 +453,15 @@
 
     last_lb = lb
     last_rb = rb
 
     return 'Done'
 
 
-def press(event, Z):
+def press(event, Z, filter_files):
     """
     Pressing a key will do something
 
     Parameters
     ----------
     event : matplotlib event
         The event that is triggered by pressing a key
@@ -475,33 +476,33 @@
     global lb
     global day
     if event.key == "d":
         # right boundary line
         lb = lb
         rb = event.xdata
         plt.close()
-        plot_obs(["896797_B.txt"], day=day, lb=lb, rb=rb, order=order, resolution=resolution, npairs=npairs,
+        plot_obs(filter_files, day=day, lb=lb, rb=rb, order=order, resolution=resolution, npairs=npairs,
                  para_range=None, norm_method="norm")
     elif event.key == "a":
         # left boundary line
         lb = event.xdata
         rb = rb
         plt.close()
-        plot_obs(["896797_B.txt"], day=day, lb=lb, rb=rb, order=order, resolution=resolution, npairs=npairs,
+        plot_obs(filter_files, day=day, lb=lb, rb=rb, order=order, resolution=resolution, npairs=npairs,
                  para_range=None, norm_method="norm")
     elif event.key == "w":
         # writes to a file
         pass
     elif event.key == "escape" or event.key == "q":
         # exits the program
         exit()
     elif event.key == "n":
         # goes to the next "day"
         day += 1
-        plot_obs(["896797_B.txt"], day=day, lb=lb, rb=rb, order=order, resolution=resolution, npairs=npairs,
+        plot_obs(filter_files, day=day, lb=lb, rb=rb, order=order, resolution=resolution, npairs=npairs,
                  para_range=None, norm_method="norm")
     elif event.key == "h":
         print("\nPress 'a' for right boundary, 'd' for left boundary, 'n' for the next day, 'w' to write to a file, "
               "or the 'ESC' or 'q' keys to close the figure.\n")
     else:
         print("\nPress 'a' for right boundary, 'd' for left boundary, 'n' for the next day, 'w' to write to a file, "
               "or the 'ESC' or 'q' keys to close the figure.\n")
```

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/gaia.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/menu.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/menu.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/multi_aperture_photometry.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/multi_aperture_photometry.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/pipeline.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This script checks for new files in a directory every second for the start of a data pipeline.
 
 Author: Kyle Koeller
 Created: 06/15/2023
-Last Edited: 08/21/2023
+Last Edited: 04/19/2024
 """
 
 from os import path, listdir
 from time import time, sleep
 import argparse
 
 from .apass import comparison_selector
@@ -20,24 +20,30 @@
     parser = argparse.ArgumentParser(description="Monitor a directory for new files and start a data pipeline.")
 
     # add the arguments
     parser.add_argument("input", metavar="Input File", type=str, help="The path of the folder where the images are going to.")
     parser.add_argument("output", metavar="Output File", type=str, help="The path of the folder where the reduced images "
                                                                         "and all files will go.")
     parser.add_argument("--time", metavar="Time Threshold", type=int, default=3600,
-                        help="The time threshold in seconds. If no new file is added within this time, an alert is "
+                        help="Time threshold in seconds. If no new file is added within this time, an alert is "
                              "raised. Default is 3600 seconds (1 hour).")
-    parser.add_argument("--loc", metavar="Location", type=str, default="BSUO",
-                        help="The location of the telescope (BSUO, CTIO, LaPalma, KPNO). Default is BSUO.")
+    parser.add_argument("--loc", metavar="Location", type=str, default="None",
+                        help="Location of the telescope (BSUO, CTIO, LaPalma, KPNO). Default is None.")
     parser.add_argument("--ra", type=str, default="00:00:00",
-                        help="The right ascension of the target. Default is 00:00:00.", required=True)
+                        help="Right ascension of the target. Default is 00:00:00.", required=True)
     parser.add_argument("--dec", type=str, default="00:00:00",
-                        help="The declination of the target (if negative -00:00:00). Default is 00:00:00.", required=True)
+                        help="Declination of the target (if negative -00:00:00). Default is 00:00:00.", required=True)
     parser.add_argument("--name", metavar="Object Name", type=str, default="NSVS_254037",
-                        help="The name of the target and must include '_' instead of spaces. Default is NSVS_254037.")
+                        help="Name of the target and must include '_' instead of spaces. Default is NSVS_254037.")
+    parser.add_argument("--mem", metavar="Memory Usage", type=str, default="450e6",
+                        help="Memory maximum of 4.5 Gb is recommended which is 450e6 (i.e. 8.0 Gb would be 800e6). Default is 450e6.")
+    parser.add_argument("--gain", metavar="Gain", type=float, default=1.43,
+                        help="Gain of the camera used. Default is 1.43.")
+    parser.add_argument("--rdnoise", metavar="Readout Noise", type=float, default=10.83,
+                        help="Readout noise of the camera used. Default is 10.83.")
 
     # parse the arguments
     args = parser.parse_args()
 
     def get_latest_file(folder_path):
         """
         Get the latest file in the directory
@@ -72,12 +78,12 @@
         else:
             # if a new file has been added
             print("Latest file: " + latest_file)
             start_time = time()
             current_latest_file = latest_file
 
     print("\n\nStarting data reduction.\n")
-    IRAF(path=args.input, calibrated=args.output, pipeline=True, location=args.loc)
+    IRAF(path=args.input, calibrated=args.output, pipeline=True, location=args.loc, gain=args.gain, rdnoise=args.rdnoise, mem_limit=args.mem)
     print("\n\nStarting comparison star selection.\n")
     radec_files = comparison_selector(ra=args.ra, dec=args.dec, pipeline=True, folder_path=args.output, obj_name=args.name)
     print("\n\nStarting photometry.\n")
     multiple_AP(path=args.output, pipeline=True, radec_list=radec_files, obj_name=args.name)
```

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/tess_ccd_info.txt` & `eclipsingbinaries-4.1.0/EclipsingBinaries/tess_ccd_info.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/tess_data_search.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/tess_data_search.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/tesscut.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/tesscut.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/tests/test_IRAF_Reduction.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/tests/test_IRAF_Reduction.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/tests/test_OC_plot.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/tests/test_OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries/tests/test_apass.py` & `eclipsingbinaries-4.1.0/EclipsingBinaries/tests/test_apass.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries.egg-info/PKG-INFO` & `eclipsingbinaries-4.1.0/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 4.0.8
+Version: 4.1.0
 Summary: "Binary Star Package for Ball State University's Astronomy Research Group"
 Home-page: https://eclipsingbinaries.readthedocs.io/
 Author: Kyle Koeller
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -33,15 +33,15 @@
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 
 # EclipsingBinaries
 
-A Python project for Ball State University's Variable Star Research Group. The package can currently reduce data, find comparison stars from the APASS catalog, calculate and plot O-C values, find the color index and effective temperature, O'Connell effect parameters, and download TESS data and calculate TESS magnitudes from Gaia data.
+EclipsingBinaries is a Python project for faster analysis of eclipsing binary star systems. The package can currently reduce data, find comparison stars from the APASS catalog, calculate and plot O-C values, find the color index and effective temperature, O'Connell effect parameters, and download TESS data and calculate TESS magnitudes from Gaia data.
 
 ***
 
 ## Documentation
 
 You can find the documentation at this [site](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest#) and any questions can be talked about in the discussions page or in an issue.
```

### Comparing `EclipsingBinaries-4.0.8/EclipsingBinaries.egg-info/SOURCES.txt` & `eclipsingbinaries-4.1.0/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/LICENSE` & `eclipsingbinaries-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/PKG-INFO` & `eclipsingbinaries-4.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 4.0.8
+Version: 4.1.0
 Summary: "Binary Star Package for Ball State University's Astronomy Research Group"
 Home-page: https://eclipsingbinaries.readthedocs.io/
 Author: Kyle Koeller
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -33,15 +33,15 @@
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 
 # EclipsingBinaries
 
-A Python project for Ball State University's Variable Star Research Group. The package can currently reduce data, find comparison stars from the APASS catalog, calculate and plot O-C values, find the color index and effective temperature, O'Connell effect parameters, and download TESS data and calculate TESS magnitudes from Gaia data.
+EclipsingBinaries is a Python project for faster analysis of eclipsing binary star systems. The package can currently reduce data, find comparison stars from the APASS catalog, calculate and plot O-C values, find the color index and effective temperature, O'Connell effect parameters, and download TESS data and calculate TESS magnitudes from Gaia data.
 
 ***
 
 ## Documentation
 
 You can find the documentation at this [site](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest#) and any questions can be talked about in the discussions page or in an issue.
```

### Comparing `EclipsingBinaries-4.0.8/README.md` & `eclipsingbinaries-4.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 
 # EclipsingBinaries
 
-A Python project for Ball State University's Variable Star Research Group. The package can currently reduce data, find comparison stars from the APASS catalog, calculate and plot O-C values, find the color index and effective temperature, O'Connell effect parameters, and download TESS data and calculate TESS magnitudes from Gaia data.
+EclipsingBinaries is a Python project for faster analysis of eclipsing binary star systems. The package can currently reduce data, find comparison stars from the APASS catalog, calculate and plot O-C values, find the color index and effective temperature, O'Connell effect parameters, and download TESS data and calculate TESS magnitudes from Gaia data.
 
 ***
 
 ## Documentation
 
 You can find the documentation at this [site](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest#) and any questions can be talked about in the discussions page or in an issue.
```

### Comparing `EclipsingBinaries-4.0.8/changelog/package-lock.json` & `eclipsingbinaries-4.1.0/changelog/package-lock.json`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/changelog/package.json` & `eclipsingbinaries-4.1.0/changelog/package.json`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/docs/conf.py` & `eclipsingbinaries-4.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/docs/contributing.rst` & `eclipsingbinaries-4.1.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/docs/index.rst` & `eclipsingbinaries-4.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/docs/installation.rst` & `eclipsingbinaries-4.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/docs/pipeline.rst` & `eclipsingbinaries-4.1.0/docs/pipeline.rst`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/docs/toolbox.rst` & `eclipsingbinaries-4.1.0/docs/toolbox.rst`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/setup.cfg` & `eclipsingbinaries-4.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.8/tox.ini` & `eclipsingbinaries-4.1.0/tox.ini`

 * *Files identical despite different names*

