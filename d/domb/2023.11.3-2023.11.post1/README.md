# Comparing `tmp/domb-2023.11.3.tar.gz` & `tmp/domb-2023.11.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domb-2023.11.3.tar", last modified: Thu Nov 23 18:15:13 2023, max compression
+gzip compressed data, was "domb-2023.11.post1.tar", last modified: Tue Nov 21 16:17:08 2023, max compression
```

## Comparing `domb-2023.11.3.tar` & `domb-2023.11.post1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.644053 domb-2023.11.3/
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     1081 2023-11-22 08:56:42.000000 domb-2023.11.3/LICENSE
--rw-r--r--   0 wisstock  (1000) wisstock  (1000)     6495 2023-11-23 18:15:13.644053 domb-2023.11.3/PKG-INFO
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     4218 2023-11-23 16:49:29.000000 domb-2023.11.3/README.md
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     1475 2023-11-23 18:13:47.000000 domb-2023.11.3/pyproject.toml
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)       38 2023-11-23 18:15:13.644053 domb-2023.11.3/setup.cfg
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.640053 domb-2023.11.3/src/
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.640053 domb-2023.11.3/src/domb/
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)        0 2023-08-01 13:48:59.000000 domb-2023.11.3/src/domb/__init__.py
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.640053 domb-2023.11.3/src/domb/fret/
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)        0 2023-08-01 13:48:59.000000 domb-2023.11.3/src/domb/fret/__init__.py
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.644053 domb-2023.11.3/src/domb/fret/b_fret/
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)        0 2023-08-01 13:48:17.000000 domb-2023.11.3/src/domb/fret/b_fret/__init__.py
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.640053 domb-2023.11.3/src/domb/fret/b_fret/example/
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.640053 domb-2023.11.3/src/domb/fret/b_fret/example/gauss_noise/
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.644053 domb-2023.11.3/src/domb/fret/b_fret/example/gauss_noise/sinusoids/
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     2399 2023-09-13 14:45:12.000000 domb-2023.11.3/src/domb/fret/b_fret/example/gauss_noise/sinusoids/define_analysis_params.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     1815 2023-09-13 14:45:12.000000 domb-2023.11.3/src/domb/fret/b_fret/example/gauss_noise/sinusoids/define_model_functions.py
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.644053 domb-2023.11.3/src/domb/fret/b_fret/example/gauss_noise/steps/
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     2399 2023-09-13 14:45:12.000000 domb-2023.11.3/src/domb/fret/b_fret/example/gauss_noise/steps/define_analysis_params.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     1815 2023-09-13 14:45:12.000000 domb-2023.11.3/src/domb/fret/b_fret/example/gauss_noise/steps/define_model_functions.py
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.640053 domb-2023.11.3/src/domb/fret/b_fret/example/non_gauss_noise/
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.644053 domb-2023.11.3/src/domb/fret/b_fret/example/non_gauss_noise/sinusoids/
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     2403 2023-09-13 14:45:12.000000 domb-2023.11.3/src/domb/fret/b_fret/example/non_gauss_noise/sinusoids/define_analysis_params.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     2447 2023-09-13 14:45:12.000000 domb-2023.11.3/src/domb/fret/b_fret/example/non_gauss_noise/sinusoids/define_model_functions.py
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.644053 domb-2023.11.3/src/domb/fret/b_fret/example/non_gauss_noise/steps/
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     2403 2023-09-13 14:45:12.000000 domb-2023.11.3/src/domb/fret/b_fret/example/non_gauss_noise/steps/define_analysis_params.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     2447 2023-09-13 14:45:12.000000 domb-2023.11.3/src/domb/fret/b_fret/example/non_gauss_noise/steps/define_model_functions.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     3234 2023-09-13 14:45:12.000000 domb-2023.11.3/src/domb/fret/b_fret/main.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    16408 2023-09-13 14:45:12.000000 domb-2023.11.3/src/domb/fret/b_fret/param_dist_funcs.py
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.644053 domb-2023.11.3/src/domb/fret/b_fret/scripts/
--rwxrwxr-x   0 wisstock  (1000) wisstock  (1000)      317 2023-09-13 14:45:12.000000 domb-2023.11.3/src/domb/fret/b_fret/scripts/sample_run_script.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    12257 2023-09-13 14:45:12.000000 domb-2023.11.3/src/domb/fret/b_fret/state_dist_funcs.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     7768 2023-09-13 14:45:12.000000 domb-2023.11.3/src/domb/fret/b_fret/utils.py
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.644053 domb-2023.11.3/src/domb/fret/e_fret/
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)        0 2023-08-01 13:48:17.000000 domb-2023.11.3/src/domb/fret/e_fret/__init__.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    29379 2023-09-06 15:08:38.000000 domb-2023.11.3/src/domb/fret/e_fret/coef_calc.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     6162 2023-11-21 14:51:22.000000 domb-2023.11.3/src/domb/fret/e_fret/e_app.py
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.644053 domb-2023.11.3/src/domb/red_green/
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)      144 2023-10-17 15:51:56.000000 domb-2023.11.3/src/domb/red_green/__init__.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    21192 2023-11-21 14:51:02.000000 domb-2023.11.3/src/domb/red_green/wt_vs_mut.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    14788 2023-11-21 14:50:23.000000 domb-2023.11.3/src/domb/red_green/wt_vs_mut_multistim.py
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.644053 domb-2023.11.3/src/domb/reg_type/
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)       54 2023-10-17 15:55:54.000000 domb-2023.11.3/src/domb/reg_type/__init__.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    13089 2023-11-21 12:15:56.000000 domb-2023.11.3/src/domb/reg_type/wf_x2_m2.py
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.644053 domb-2023.11.3/src/domb/utils/
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)        0 2023-10-24 10:27:51.000000 domb-2023.11.3/src/domb/utils/__init__.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    15813 2023-11-21 14:49:20.000000 domb-2023.11.3/src/domb/utils/masking.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    29187 2023-08-26 11:06:16.000000 domb-2023.11.3/src/domb/utils/oiffile.py
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     9504 2023-11-21 14:49:54.000000 domb-2023.11.3/src/domb/utils/plot.py
-drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-23 18:15:13.644053 domb-2023.11.3/src/domb.egg-info/
--rw-r--r--   0 wisstock  (1000) wisstock  (1000)     6495 2023-11-23 18:15:13.000000 domb-2023.11.3/src/domb.egg-info/PKG-INFO
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     1442 2023-11-23 18:15:13.000000 domb-2023.11.3/src/domb.egg-info/SOURCES.txt
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)        1 2023-11-23 18:15:13.000000 domb-2023.11.3/src/domb.egg-info/dependency_links.txt
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)       72 2023-11-23 18:15:13.000000 domb-2023.11.3/src/domb.egg-info/requires.txt
--rw-rw-r--   0 wisstock  (1000) wisstock  (1000)        5 2023-11-23 18:15:13.000000 domb-2023.11.3/src/domb.egg-info/top_level.txt
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.510131 domb-2023.11.post1/
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     1146 2023-08-02 07:26:57.000000 domb-2023.11.post1/LICENSE
+-rw-r--r--   0 wisstock  (1000) wisstock  (1000)     6006 2023-11-21 16:17:08.506132 domb-2023.11.post1/PKG-INFO
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     3868 2023-11-21 14:38:29.000000 domb-2023.11.post1/README.md
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)      843 2023-11-21 11:43:56.000000 domb-2023.11.post1/pyproject.toml
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)       38 2023-11-21 16:17:08.510131 domb-2023.11.post1/setup.cfg
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.502132 domb-2023.11.post1/src/
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.502132 domb-2023.11.post1/src/domb/
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)        0 2023-08-01 13:48:59.000000 domb-2023.11.post1/src/domb/__init__.py
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.506132 domb-2023.11.post1/src/domb/fret/
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)        0 2023-08-01 13:48:59.000000 domb-2023.11.post1/src/domb/fret/__init__.py
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.506132 domb-2023.11.post1/src/domb/fret/b_fret/
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)        0 2023-08-01 13:48:17.000000 domb-2023.11.post1/src/domb/fret/b_fret/__init__.py
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.502132 domb-2023.11.post1/src/domb/fret/b_fret/example/
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.502132 domb-2023.11.post1/src/domb/fret/b_fret/example/gauss_noise/
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.506132 domb-2023.11.post1/src/domb/fret/b_fret/example/gauss_noise/sinusoids/
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     2399 2023-09-13 14:45:12.000000 domb-2023.11.post1/src/domb/fret/b_fret/example/gauss_noise/sinusoids/define_analysis_params.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     1815 2023-09-13 14:45:12.000000 domb-2023.11.post1/src/domb/fret/b_fret/example/gauss_noise/sinusoids/define_model_functions.py
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.506132 domb-2023.11.post1/src/domb/fret/b_fret/example/gauss_noise/steps/
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     2399 2023-09-13 14:45:12.000000 domb-2023.11.post1/src/domb/fret/b_fret/example/gauss_noise/steps/define_analysis_params.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     1815 2023-09-13 14:45:12.000000 domb-2023.11.post1/src/domb/fret/b_fret/example/gauss_noise/steps/define_model_functions.py
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.502132 domb-2023.11.post1/src/domb/fret/b_fret/example/non_gauss_noise/
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.506132 domb-2023.11.post1/src/domb/fret/b_fret/example/non_gauss_noise/sinusoids/
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     2403 2023-09-13 14:45:12.000000 domb-2023.11.post1/src/domb/fret/b_fret/example/non_gauss_noise/sinusoids/define_analysis_params.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     2447 2023-09-13 14:45:12.000000 domb-2023.11.post1/src/domb/fret/b_fret/example/non_gauss_noise/sinusoids/define_model_functions.py
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.506132 domb-2023.11.post1/src/domb/fret/b_fret/example/non_gauss_noise/steps/
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     2403 2023-09-13 14:45:12.000000 domb-2023.11.post1/src/domb/fret/b_fret/example/non_gauss_noise/steps/define_analysis_params.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     2447 2023-09-13 14:45:12.000000 domb-2023.11.post1/src/domb/fret/b_fret/example/non_gauss_noise/steps/define_model_functions.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     3234 2023-09-13 14:45:12.000000 domb-2023.11.post1/src/domb/fret/b_fret/main.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    16408 2023-09-13 14:45:12.000000 domb-2023.11.post1/src/domb/fret/b_fret/param_dist_funcs.py
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.506132 domb-2023.11.post1/src/domb/fret/b_fret/scripts/
+-rwxrwxr-x   0 wisstock  (1000) wisstock  (1000)      317 2023-09-13 14:45:12.000000 domb-2023.11.post1/src/domb/fret/b_fret/scripts/sample_run_script.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    12257 2023-09-13 14:45:12.000000 domb-2023.11.post1/src/domb/fret/b_fret/state_dist_funcs.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     7768 2023-09-13 14:45:12.000000 domb-2023.11.post1/src/domb/fret/b_fret/utils.py
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.506132 domb-2023.11.post1/src/domb/fret/e_fret/
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)        0 2023-08-01 13:48:17.000000 domb-2023.11.post1/src/domb/fret/e_fret/__init__.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    29379 2023-09-06 15:08:38.000000 domb-2023.11.post1/src/domb/fret/e_fret/coef_calc.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     6162 2023-11-21 14:51:22.000000 domb-2023.11.post1/src/domb/fret/e_fret/e_app.py
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.506132 domb-2023.11.post1/src/domb/red_green/
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)      144 2023-10-17 15:51:56.000000 domb-2023.11.post1/src/domb/red_green/__init__.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    21192 2023-11-21 14:51:02.000000 domb-2023.11.post1/src/domb/red_green/wt_vs_mut.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    14788 2023-11-21 14:50:23.000000 domb-2023.11.post1/src/domb/red_green/wt_vs_mut_multistim.py
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.506132 domb-2023.11.post1/src/domb/reg_type/
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)       54 2023-10-17 15:55:54.000000 domb-2023.11.post1/src/domb/reg_type/__init__.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    13089 2023-11-21 12:15:56.000000 domb-2023.11.post1/src/domb/reg_type/wf_x2_m2.py
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.506132 domb-2023.11.post1/src/domb/utils/
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)        0 2023-10-24 10:27:51.000000 domb-2023.11.post1/src/domb/utils/__init__.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    15813 2023-11-21 14:49:20.000000 domb-2023.11.post1/src/domb/utils/masking.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)    29187 2023-08-26 11:06:16.000000 domb-2023.11.post1/src/domb/utils/oiffile.py
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     9504 2023-11-21 14:49:54.000000 domb-2023.11.post1/src/domb/utils/plot.py
+drwxrwxr-x   0 wisstock  (1000) wisstock  (1000)        0 2023-11-21 16:17:08.506132 domb-2023.11.post1/src/domb.egg-info/
+-rw-r--r--   0 wisstock  (1000) wisstock  (1000)     6006 2023-11-21 16:17:08.000000 domb-2023.11.post1/src/domb.egg-info/PKG-INFO
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)     1442 2023-11-21 16:17:08.000000 domb-2023.11.post1/src/domb.egg-info/SOURCES.txt
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)        1 2023-11-21 16:17:08.000000 domb-2023.11.post1/src/domb.egg-info/dependency_links.txt
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)      224 2023-11-21 16:17:08.000000 domb-2023.11.post1/src/domb.egg-info/requires.txt
+-rw-rw-r--   0 wisstock  (1000) wisstock  (1000)        5 2023-11-21 16:17:08.000000 domb-2023.11.post1/src/domb.egg-info/top_level.txt
```

### Comparing `domb-2023.11.3/LICENSE` & `domb-2023.11.post1/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-Copyright (c) 2023 Borys Olifirov <omnia.fatum@gmail.com>
+DoMB tools: Python toolkit of Department of Molecular Biophysics
+
+Copyright © 2023 Borys Olifirov <omnia.fatum@gmail.com>
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `domb-2023.11.3/PKG-INFO` & `domb-2023.11.post1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: domb
-Version: 2023.11.3
-Summary: DoMB Tools: Python Toolkit of Department of Molecular Biophysics
+Version: 2023.11.post1
+Summary: DoMB tools: Python Toolkit of Department of Molecular Biophysics
 Author-email: Borys Olifirov <omnia.fatum@gmail.com>
-License: Copyright (c) 2023 Borys Olifirov <omnia.fatum@gmail.com>
+License: DoMB tools: Python toolkit of Department of Molecular Biophysics
+        
+        Copyright © 2023 Borys Olifirov <omnia.fatum@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
         distribute, sublicense, and/or sell copies of the Software, and to
         permit persons to whom the Software is furnished to do so, subject to
@@ -19,52 +21,45 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
         EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
         MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
         NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
         LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
         OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
         WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Project-URL: Documentation, https://domb.bio/
+Project-URL: documentation, https://domb.bio/
 Project-URL: Repository, https://github.com/wisstock/DoMB_tools
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: IPython
-Classifier: Framework :: Jupyter
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: scikit-image
-Requires-Dist: scikit-learn
-Requires-Dist: scikit-posthocs
-Requires-Dist: scipy
+Requires-Dist: autograd>=1.6
+Requires-Dist: ipykernel>=6.19
+Requires-Dist: jupyter>=1.0
+Requires-Dist: matplotlib>=3.7
+Requires-Dist: mkdocstrings[python]>=0.18
+Requires-Dist: numpy>=1.25
+Requires-Dist: opencv-python>=4.5
+Requires-Dist: pandas>=1.5
+Requires-Dist: pathos>=0.3
+Requires-Dist: plotly>=5.15
+Requires-Dist: scikit-image>=0.19
+Requires-Dist: scikit-learn>=1.0
+Requires-Dist: scikit-posthocs>=0.7
+Requires-Dist: scipy>=0.12
 
-DoMB Tools
+DoMB tools
 ==========
-## Python Toolkit of Department of Molecular Biophysics
 
-![PyPI - Version](https://img.shields.io/pypi/v/domb)
-![PyPI - License](https://img.shields.io/pypi/l/domb)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/domb)
-![Website](https://img.shields.io/website?up_message=domb.bio&up_color=%23038C93&url=https%3A%2F%2Fdomb.bio%2F)
+__Python Toolkit of Department of Molecular Biophysics__
 
 # Description
-__Registration types__ integrate acquired data (images, electrophysiological recordings, metadata) into unified data structures. Attributes within this structure support subsequent analysis through functions in the _modules_.
+__Registrations types__ combine acquired data (images, electrophysiological recordings, metadata) into unified data structures. Attributes within this structure support subsequent analysis through _modules_ functions.
 
-__Modules__ provide distinct data analysis approaches with predefined pipelines. These pipelines transform inputs into approach-specific illustrations and organized pre-processed images, optimized for further quantitative analysis. Modules require specific _registration types_ as inputs.
+__Modules__ offer distinct data analysis approaches with predefined pipelines. These pipelines transform inputs into approach-specific illustrations and organized pre-processed images, optimized for further quantitative analysis. Modules require specific _registration types_ as inputs.
 
-__Utilities__ offer reusable functions for multidimensional image processing, advanced visualization, and uploading data in specific formats (OIF/OIB, HEKA, etc.).
+__Utilities__ provide reusable functions for multidimensional image processing, advanced visualization, and specific data format (OIF/OIB, HEKA) uploading.
 
 
 # Structure Overview
 ```
 └── domb
     ├── reg_type                  # data types for different registration designs
     │   └── wf_x2_m2.py             #  widefield, 2 excitation wavelengths, 2 emission channels
@@ -91,32 +86,32 @@
 ```
 conda create -y -n domb -c conda-forge python=3.9
 conda acticate domb
 ```
 
 ### From pip
 ```
-python -m pip install domb
+pip install domb
 ```
 
 ### From GitHub
 Clone the repo:
 ```
-git clone -b master git@github.com:wisstock/domb-tools.git
+git clone -b master git@github.com:wisstock/DoMB_tools.git
 ```
 
-To install the package, simply navigate to the repository folder and install with pip: 
+To install the package, simply navigate to the repository folder and run: 
 ```
 cd DoMB_tools
-python -m pip install .
+pip install .
 ```
 
 But if you're planning to make changes and work on the source code actively, you might want to consider using the editable mode:
 ```
-python -m pip install -e .
+pip install -e .
 ```
 
 # Borrowed modules
 ### OIF File
 _Copyright © 2012-2022 [Christoph Gohlke](https://www.cgohlke.com/)_
 
 Oiffile is a Python library to read image and metadata from Olympus Image
```

### Comparing `domb-2023.11.3/README.md` & `domb-2023.11.post1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-DoMB Tools
+DoMB tools
 ==========
-## Python Toolkit of Department of Molecular Biophysics
 
-![PyPI - Version](https://img.shields.io/pypi/v/domb)
-![PyPI - License](https://img.shields.io/pypi/l/domb)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/domb)
-![Website](https://img.shields.io/website?up_message=domb.bio&up_color=%23038C93&url=https%3A%2F%2Fdomb.bio%2F)
+__Python Toolkit of Department of Molecular Biophysics__
 
 # Description
-__Registration types__ integrate acquired data (images, electrophysiological recordings, metadata) into unified data structures. Attributes within this structure support subsequent analysis through functions in the _modules_.
+__Registrations types__ combine acquired data (images, electrophysiological recordings, metadata) into unified data structures. Attributes within this structure support subsequent analysis through _modules_ functions.
 
-__Modules__ provide distinct data analysis approaches with predefined pipelines. These pipelines transform inputs into approach-specific illustrations and organized pre-processed images, optimized for further quantitative analysis. Modules require specific _registration types_ as inputs.
+__Modules__ offer distinct data analysis approaches with predefined pipelines. These pipelines transform inputs into approach-specific illustrations and organized pre-processed images, optimized for further quantitative analysis. Modules require specific _registration types_ as inputs.
 
-__Utilities__ offer reusable functions for multidimensional image processing, advanced visualization, and uploading data in specific formats (OIF/OIB, HEKA, etc.).
+__Utilities__ provide reusable functions for multidimensional image processing, advanced visualization, and specific data format (OIF/OIB, HEKA) uploading.
 
 
 # Structure Overview
 ```
 └── domb
     ├── reg_type                  # data types for different registration designs
     │   └── wf_x2_m2.py             #  widefield, 2 excitation wavelengths, 2 emission channels
@@ -43,32 +39,32 @@
 ```
 conda create -y -n domb -c conda-forge python=3.9
 conda acticate domb
 ```
 
 ### From pip
 ```
-python -m pip install domb
+pip install domb
 ```
 
 ### From GitHub
 Clone the repo:
 ```
-git clone -b master git@github.com:wisstock/domb-tools.git
+git clone -b master git@github.com:wisstock/DoMB_tools.git
 ```
 
-To install the package, simply navigate to the repository folder and install with pip: 
+To install the package, simply navigate to the repository folder and run: 
 ```
 cd DoMB_tools
-python -m pip install .
+pip install .
 ```
 
 But if you're planning to make changes and work on the source code actively, you might want to consider using the editable mode:
 ```
-python -m pip install -e .
+pip install -e .
 ```
 
 # Borrowed modules
 ### OIF File
 _Copyright © 2012-2022 [Christoph Gohlke](https://www.cgohlke.com/)_
 
 Oiffile is a Python library to read image and metadata from Olympus Image
```

### Comparing `domb-2023.11.3/src/domb/fret/b_fret/example/gauss_noise/sinusoids/define_analysis_params.py` & `domb-2023.11.post1/src/domb/fret/b_fret/example/gauss_noise/sinusoids/define_analysis_params.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/fret/b_fret/example/gauss_noise/sinusoids/define_model_functions.py` & `domb-2023.11.post1/src/domb/fret/b_fret/example/gauss_noise/sinusoids/define_model_functions.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/fret/b_fret/example/gauss_noise/steps/define_analysis_params.py` & `domb-2023.11.post1/src/domb/fret/b_fret/example/gauss_noise/steps/define_analysis_params.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/fret/b_fret/example/gauss_noise/steps/define_model_functions.py` & `domb-2023.11.post1/src/domb/fret/b_fret/example/gauss_noise/steps/define_model_functions.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/fret/b_fret/example/non_gauss_noise/sinusoids/define_analysis_params.py` & `domb-2023.11.post1/src/domb/fret/b_fret/example/non_gauss_noise/sinusoids/define_analysis_params.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/fret/b_fret/example/non_gauss_noise/sinusoids/define_model_functions.py` & `domb-2023.11.post1/src/domb/fret/b_fret/example/non_gauss_noise/sinusoids/define_model_functions.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/fret/b_fret/example/non_gauss_noise/steps/define_analysis_params.py` & `domb-2023.11.post1/src/domb/fret/b_fret/example/non_gauss_noise/steps/define_analysis_params.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/fret/b_fret/example/non_gauss_noise/steps/define_model_functions.py` & `domb-2023.11.post1/src/domb/fret/b_fret/example/non_gauss_noise/steps/define_model_functions.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/fret/b_fret/main.py` & `domb-2023.11.post1/src/domb/fret/b_fret/main.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/fret/b_fret/param_dist_funcs.py` & `domb-2023.11.post1/src/domb/fret/b_fret/param_dist_funcs.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/fret/b_fret/state_dist_funcs.py` & `domb-2023.11.post1/src/domb/fret/b_fret/state_dist_funcs.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/fret/b_fret/utils.py` & `domb-2023.11.post1/src/domb/fret/b_fret/utils.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/fret/e_fret/coef_calc.py` & `domb-2023.11.post1/src/domb/fret/e_fret/coef_calc.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/fret/e_fret/e_app.py` & `domb-2023.11.post1/src/domb/fret/e_fret/e_app.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/red_green/wt_vs_mut.py` & `domb-2023.11.post1/src/domb/red_green/wt_vs_mut.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/red_green/wt_vs_mut_multistim.py` & `domb-2023.11.post1/src/domb/red_green/wt_vs_mut_multistim.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/reg_type/wf_x2_m2.py` & `domb-2023.11.post1/src/domb/reg_type/wf_x2_m2.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/utils/masking.py` & `domb-2023.11.post1/src/domb/utils/masking.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/utils/oiffile.py` & `domb-2023.11.post1/src/domb/utils/oiffile.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb/utils/plot.py` & `domb-2023.11.post1/src/domb/utils/plot.py`

 * *Files identical despite different names*

### Comparing `domb-2023.11.3/src/domb.egg-info/PKG-INFO` & `domb-2023.11.post1/src/domb.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: domb
-Version: 2023.11.3
-Summary: DoMB Tools: Python Toolkit of Department of Molecular Biophysics
+Version: 2023.11.post1
+Summary: DoMB tools: Python Toolkit of Department of Molecular Biophysics
 Author-email: Borys Olifirov <omnia.fatum@gmail.com>
-License: Copyright (c) 2023 Borys Olifirov <omnia.fatum@gmail.com>
+License: DoMB tools: Python toolkit of Department of Molecular Biophysics
+        
+        Copyright © 2023 Borys Olifirov <omnia.fatum@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
         distribute, sublicense, and/or sell copies of the Software, and to
         permit persons to whom the Software is furnished to do so, subject to
@@ -19,52 +21,45 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
         EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
         MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
         NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
         LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
         OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
         WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Project-URL: Documentation, https://domb.bio/
+Project-URL: documentation, https://domb.bio/
 Project-URL: Repository, https://github.com/wisstock/DoMB_tools
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: IPython
-Classifier: Framework :: Jupyter
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: scikit-image
-Requires-Dist: scikit-learn
-Requires-Dist: scikit-posthocs
-Requires-Dist: scipy
+Requires-Dist: autograd>=1.6
+Requires-Dist: ipykernel>=6.19
+Requires-Dist: jupyter>=1.0
+Requires-Dist: matplotlib>=3.7
+Requires-Dist: mkdocstrings[python]>=0.18
+Requires-Dist: numpy>=1.25
+Requires-Dist: opencv-python>=4.5
+Requires-Dist: pandas>=1.5
+Requires-Dist: pathos>=0.3
+Requires-Dist: plotly>=5.15
+Requires-Dist: scikit-image>=0.19
+Requires-Dist: scikit-learn>=1.0
+Requires-Dist: scikit-posthocs>=0.7
+Requires-Dist: scipy>=0.12
 
-DoMB Tools
+DoMB tools
 ==========
-## Python Toolkit of Department of Molecular Biophysics
 
-![PyPI - Version](https://img.shields.io/pypi/v/domb)
-![PyPI - License](https://img.shields.io/pypi/l/domb)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/domb)
-![Website](https://img.shields.io/website?up_message=domb.bio&up_color=%23038C93&url=https%3A%2F%2Fdomb.bio%2F)
+__Python Toolkit of Department of Molecular Biophysics__
 
 # Description
-__Registration types__ integrate acquired data (images, electrophysiological recordings, metadata) into unified data structures. Attributes within this structure support subsequent analysis through functions in the _modules_.
+__Registrations types__ combine acquired data (images, electrophysiological recordings, metadata) into unified data structures. Attributes within this structure support subsequent analysis through _modules_ functions.
 
-__Modules__ provide distinct data analysis approaches with predefined pipelines. These pipelines transform inputs into approach-specific illustrations and organized pre-processed images, optimized for further quantitative analysis. Modules require specific _registration types_ as inputs.
+__Modules__ offer distinct data analysis approaches with predefined pipelines. These pipelines transform inputs into approach-specific illustrations and organized pre-processed images, optimized for further quantitative analysis. Modules require specific _registration types_ as inputs.
 
-__Utilities__ offer reusable functions for multidimensional image processing, advanced visualization, and uploading data in specific formats (OIF/OIB, HEKA, etc.).
+__Utilities__ provide reusable functions for multidimensional image processing, advanced visualization, and specific data format (OIF/OIB, HEKA) uploading.
 
 
 # Structure Overview
 ```
 └── domb
     ├── reg_type                  # data types for different registration designs
     │   └── wf_x2_m2.py             #  widefield, 2 excitation wavelengths, 2 emission channels
@@ -91,32 +86,32 @@
 ```
 conda create -y -n domb -c conda-forge python=3.9
 conda acticate domb
 ```
 
 ### From pip
 ```
-python -m pip install domb
+pip install domb
 ```
 
 ### From GitHub
 Clone the repo:
 ```
-git clone -b master git@github.com:wisstock/domb-tools.git
+git clone -b master git@github.com:wisstock/DoMB_tools.git
 ```
 
-To install the package, simply navigate to the repository folder and install with pip: 
+To install the package, simply navigate to the repository folder and run: 
 ```
 cd DoMB_tools
-python -m pip install .
+pip install .
 ```
 
 But if you're planning to make changes and work on the source code actively, you might want to consider using the editable mode:
 ```
-python -m pip install -e .
+pip install -e .
 ```
 
 # Borrowed modules
 ### OIF File
 _Copyright © 2012-2022 [Christoph Gohlke](https://www.cgohlke.com/)_
 
 Oiffile is a Python library to read image and metadata from Olympus Image
```

### Comparing `domb-2023.11.3/src/domb.egg-info/SOURCES.txt` & `domb-2023.11.post1/src/domb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

