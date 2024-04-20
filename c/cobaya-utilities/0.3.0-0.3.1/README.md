# Comparing `tmp/cobaya_utilities-0.3.0.tar.gz` & `tmp/cobaya_utilities-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobaya_utilities-0.3.0.tar", last modified: Tue Apr  9 04:34:46 2024, max compression
+gzip compressed data, was "cobaya_utilities-0.3.1.tar", last modified: Sat Apr 20 16:27:06 2024, max compression
```

## Comparing `cobaya_utilities-0.3.0.tar` & `cobaya_utilities-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:34:46.158883 cobaya_utilities-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-09 04:34:46.158883 cobaya_utilities-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:34:46.158883 cobaya_utilities-0.3.0/cobaya_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/cobaya_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-09 04:34:46.158883 cobaya_utilities-0.3.0/cobaya_utilities/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/cobaya_utilities/fisher.py
--rw-r--r--   0 runner    (1001) docker     (127)    22174 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/cobaya_utilities/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    25686 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/cobaya_utilities/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/cobaya_utilities/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:34:46.158883 cobaya_utilities-0.3.0/cobaya_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-09 04:34:46.000000 cobaya_utilities-0.3.0/cobaya_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-09 04:34:46.000000 cobaya_utilities-0.3.0/cobaya_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:34:46.000000 cobaya_utilities-0.3.0/cobaya_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-09 04:34:46.000000 cobaya_utilities-0.3.0/cobaya_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 04:34:46.000000 cobaya_utilities-0.3.0/cobaya_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 04:34:46.158883 cobaya_utilities-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    83635 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:27:06.627515 cobaya_utilities-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-20 16:27:06.627515 cobaya_utilities-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:27:06.611515 cobaya_utilities-0.3.1/binder/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/binder/apt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/binder/runtime.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:27:06.611515 cobaya_utilities-0.3.1/cobaya_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/cobaya_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-20 16:27:06.000000 cobaya_utilities-0.3.1/cobaya_utilities/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/cobaya_utilities/fisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22176 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/cobaya_utilities/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:27:06.611515 cobaya_utilities-0.3.1/cobaya_utilities/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:27:06.611515 cobaya_utilities-0.3.1/cobaya_utilities/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:27:06.623515 cobaya_utilities-0.3.1/cobaya_utilities/tests/data/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)   315656 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/cobaya_utilities/tests/data/chains/mcmc.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/cobaya_utilities/tests/data/chains/mcmc.covmat
+-rw-r--r--   0 runner    (1001) docker     (127)  6631707 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/cobaya_utilities/tests/data/chains/mcmc.log
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/cobaya_utilities/tests/data/chains/mcmc.progress
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/cobaya_utilities/tests/data/chains/mcmc.updated.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/cobaya_utilities/tests/data/fisher_ref.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/cobaya_utilities/tests/test_fisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/cobaya_utilities/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/cobaya_utilities/tests/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25686 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/cobaya_utilities/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/cobaya_utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:27:06.627515 cobaya_utilities-0.3.1/cobaya_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-20 16:27:06.000000 cobaya_utilities-0.3.1/cobaya_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-20 16:27:06.000000 cobaya_utilities-0.3.1/cobaya_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 16:27:06.000000 cobaya_utilities-0.3.1/cobaya_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-20 16:27:06.000000 cobaya_utilities-0.3.1/cobaya_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-20 16:27:06.000000 cobaya_utilities-0.3.1/cobaya_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:27:06.623515 cobaya_utilities-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:27:06.627515 cobaya_utilities-0.3.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)  2114694 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/docs/tutorials/chains.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:27:06.627515 cobaya_utilities-0.3.1/docs/tutorials/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)   853687 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/docs/tutorials/figures/print_chains_size.png
+-rw-r--r--   0 runner    (1001) docker     (127)   191224 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/docs/tutorials/fisher.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-20 16:26:57.000000 cobaya_utilities-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 16:27:06.627515 cobaya_utilities-0.3.1/setup.cfg
```

### Comparing `cobaya_utilities-0.3.0/PKG-INFO` & `cobaya_utilities-0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 Metadata-Version: 2.1
 Name: cobaya_utilities
-Version: 0.3.0
+Version: 0.3.1
 Summary: A set of functions to deal with MCMC output from cobaya
-Home-page: https://github.com/xgarrido/cobaya_utilities.git
 Author: Xavier Garrido
-Author-email: xavier.garrido@lal.in2p3.fr
+Project-URL: Homepage, https://github.com/xgarrido/cobaya_utilities
+Project-URL: Documentation, https://cobaya_utilities.readthedocs.io
+Project-URL: Source, https://github.com/xgarrido/cobaya_utilities
+Project-URL: Tracker, https://github.com/xgarrido/cobaya_utilities/issues
+Project-URL: Licensing, https://github.com/xgarrido/cobaya_utilities/blob/master/LICENCE
 Keywords: cobaya,MCMC,plot
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Education
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Education
-Requires-Python: >=3.9
+Requires-Python: >=3.9.0
 Description-Content-Type: text/x-rst
-Requires-Dist: cobaya
+Requires-Dist: cobaya>=3.4.1
 Requires-Dist: seaborn
 Requires-Dist: tqdm
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: camb; extra == "test"
+Requires-Dist: mflike; extra == "test"
+Provides-Extra: notebook
+Requires-Dist: jupyter; extra == "notebook"
+Requires-Dist: camb; extra == "notebook"
+Requires-Dist: latex2mathml; extra == "notebook"
 
 ==================
  Cobaya utilities
 ==================
 
 A set of tools to deal with MCMC chains and a complement to `cobaya
 <https://github.com/CobayaSampler/cobaya>`_ and `getdist <https://github.com/cmbant/getdist>`_.
```

### Comparing `cobaya_utilities-0.3.0/README.rst` & `cobaya_utilities-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `cobaya_utilities-0.3.0/cobaya_utilities/fisher.py` & `cobaya_utilities-0.3.1/cobaya_utilities/fisher.py`

 * *Files identical despite different names*

### Comparing `cobaya_utilities-0.3.0/cobaya_utilities/plots.py` & `cobaya_utilities-0.3.1/cobaya_utilities/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     plot_settings = GetDistPlotSettings()
     plot_settings.solid_colors = colors
     plot_settings.line_styles = colors
     plot_settings.num_plot_contours = num_plot_contours
     plot_settings.linewidth = linewidth
     plot_settings.legend_fontsize = 15
     plot_settings.legend_colored_text = True
-    plot_settings.figure_legend_loc = "best"
+    # plot_settings.figure_legend_loc = "best"
     plot_settings.scaling = False
     return plot_settings
 
 
 def triangle_plot(*args, **kwargs):
     """Overloaded triangle_plot function with additional features"""
     g = get_subplot_plotter(settings=get_default_settings())
```

### Comparing `cobaya_utilities-0.3.0/cobaya_utilities/tools.py` & `cobaya_utilities-0.3.1/cobaya_utilities/tools.py`

 * *Files identical despite different names*

### Comparing `cobaya_utilities-0.3.0/cobaya_utilities.egg-info/PKG-INFO` & `cobaya_utilities-0.3.1/cobaya_utilities.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 Metadata-Version: 2.1
 Name: cobaya_utilities
-Version: 0.3.0
+Version: 0.3.1
 Summary: A set of functions to deal with MCMC output from cobaya
-Home-page: https://github.com/xgarrido/cobaya_utilities.git
 Author: Xavier Garrido
-Author-email: xavier.garrido@lal.in2p3.fr
+Project-URL: Homepage, https://github.com/xgarrido/cobaya_utilities
+Project-URL: Documentation, https://cobaya_utilities.readthedocs.io
+Project-URL: Source, https://github.com/xgarrido/cobaya_utilities
+Project-URL: Tracker, https://github.com/xgarrido/cobaya_utilities/issues
+Project-URL: Licensing, https://github.com/xgarrido/cobaya_utilities/blob/master/LICENCE
 Keywords: cobaya,MCMC,plot
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Education
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Education
-Requires-Python: >=3.9
+Requires-Python: >=3.9.0
 Description-Content-Type: text/x-rst
-Requires-Dist: cobaya
+Requires-Dist: cobaya>=3.4.1
 Requires-Dist: seaborn
 Requires-Dist: tqdm
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: camb; extra == "test"
+Requires-Dist: mflike; extra == "test"
+Provides-Extra: notebook
+Requires-Dist: jupyter; extra == "notebook"
+Requires-Dist: camb; extra == "notebook"
+Requires-Dist: latex2mathml; extra == "notebook"
 
 ==================
  Cobaya utilities
 ==================
 
 A set of tools to deal with MCMC chains and a complement to `cobaya
 <https://github.com/CobayaSampler/cobaya>`_ and `getdist <https://github.com/cmbant/getdist>`_.
```

