# Comparing `tmp/combine_pvalues_discrete-1.2.2.tar.gz` & `tmp/combine_pvalues_discrete-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combine_pvalues_discrete-1.2.2.tar", last modified: Tue Feb 20 12:44:49 2024, max compression
+gzip compressed data, was "combine_pvalues_discrete-1.2.3.tar", last modified: Sat Apr 20 09:45:52 2024, max compression
```

## Comparing `combine_pvalues_discrete-1.2.2.tar` & `combine_pvalues_discrete-1.2.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:44:49.166308 combine_pvalues_discrete-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:44:49.158308 combine_pvalues_discrete-1.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:44:49.162308 combine_pvalues_discrete-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/.github/workflows/paper.yml
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-02-20 12:44:49.166308 combine_pvalues_discrete-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/codemeta.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:44:49.162308 combine_pvalues_discrete-1.2.2/combine_pvalues_discrete/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/combine_pvalues_discrete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20308 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/combine_pvalues_discrete/ctr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/combine_pvalues_discrete/pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/combine_pvalues_discrete/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-20 12:44:49.000000 combine_pvalues_discrete-1.2.2/combine_pvalues_discrete/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:44:49.166308 combine_pvalues_discrete-1.2.2/combine_pvalues_discrete.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-02-20 12:44:49.000000 combine_pvalues_discrete-1.2.2/combine_pvalues_discrete.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-20 12:44:49.000000 combine_pvalues_discrete-1.2.2/combine_pvalues_discrete.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 12:44:49.000000 combine_pvalues_discrete-1.2.2/combine_pvalues_discrete.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-20 12:44:49.000000 combine_pvalues_discrete-1.2.2/combine_pvalues_discrete.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-20 12:44:49.000000 combine_pvalues_discrete-1.2.2/combine_pvalues_discrete.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:44:49.162308 combine_pvalues_discrete-1.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:44:49.166308 combine_pvalues_discrete-1.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/examples/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/examples/mwu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/examples/simple_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/paper.bib
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/paper.md
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-20 12:44:49.166308 combine_pvalues_discrete-1.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      917 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:44:49.166308 combine_pvalues_discrete-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     9319 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/tests/test_ctr.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/tests/test_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/tests/test_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/tests/test_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-02-20 12:44:35.000000 combine_pvalues_discrete-1.2.2/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:45:52.711185 combine_pvalues_discrete-1.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:45:52.699185 combine_pvalues_discrete-1.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:45:52.703185 combine_pvalues_discrete-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/.github/workflows/paper.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-20 09:45:52.711185 combine_pvalues_discrete-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/codemeta.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:45:52.703185 combine_pvalues_discrete-1.2.3/combine_pvalues_discrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/combine_pvalues_discrete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22059 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/combine_pvalues_discrete/ctr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/combine_pvalues_discrete/pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/combine_pvalues_discrete/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-20 09:45:52.000000 combine_pvalues_discrete-1.2.3/combine_pvalues_discrete/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:45:52.707185 combine_pvalues_discrete-1.2.3/combine_pvalues_discrete.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-20 09:45:52.000000 combine_pvalues_discrete-1.2.3/combine_pvalues_discrete.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-20 09:45:52.000000 combine_pvalues_discrete-1.2.3/combine_pvalues_discrete.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:45:52.000000 combine_pvalues_discrete-1.2.3/combine_pvalues_discrete.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-20 09:45:52.000000 combine_pvalues_discrete-1.2.3/combine_pvalues_discrete.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 09:45:52.000000 combine_pvalues_discrete-1.2.3/combine_pvalues_discrete.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:45:52.707185 combine_pvalues_discrete-1.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:45:52.707185 combine_pvalues_discrete-1.2.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/examples/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/examples/mwu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/examples/simple_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/paper.md
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-20 09:45:52.711185 combine_pvalues_discrete-1.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      917 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:45:52.707185 combine_pvalues_discrete-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/tests/test_ctr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/tests/test_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/tests/test_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/tests/test_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-20 09:45:43.000000 combine_pvalues_discrete-1.2.3/tests/test_tools.py
```

### Comparing `combine_pvalues_discrete-1.2.2/.github/workflows/publish.yml` & `combine_pvalues_discrete-1.2.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/.github/workflows/test.yml` & `combine_pvalues_discrete-1.2.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/.gitignore` & `combine_pvalues_discrete-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/LICENSE` & `combine_pvalues_discrete-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/PKG-INFO` & `combine_pvalues_discrete-1.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combine_pvalues_discrete
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python toolbox for combining p values from tests with a discrete statistics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
@@ -15,18 +15,25 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: statsmodels; extra == "test"
 Requires-Dist: pytest-rng; extra == "test"
 
 A Python module for combining *p* values of discrete tests.
 
+* Read the `paper <https://doi.org/10.21105/joss.06096>`_ for a short overview; read the `documentation <https://combine-p-values-discrete.rtfd.io>`_ for more.
 * Install with:
 
   * ``pip install combine-pvalues-discrete``
   * ``pip3 install git+git://github.com/BPSB/combine-p-values-discrete``
   * or similar.
 
-* Install requirements for testing with `pip install ".[test]"` (or similar). Run the test with `pytest` (or similar) in the source directory. Run `pytest -m "not slow"` to exclude some particularly time-consuming tests.
-* `Documentation <https://combine-p-values-discrete.rtfd.io>`_
+* Install requirements for testing with ``pip install ".[test]"`` (or similar). Run the test with ``pytest`` (or similar) in the source directory. Run ``pytest -m "not slow"`` to exclude some particularly time-consuming tests.
 * `Issue Tracker <https://github.com/BPSB/combine-p-values-discrete/issues>`_ – Please use this if you need any help with this module, in particular if you are facing any bugs or require features (in particular support for tests).
 * Contributions are welcome. Feel free to discuss them on the issue tracker or just file a pull request.
-* DOI for citing: `10.5281/zenodo.8338798 <https://dx.doi.org/10.5281/zenodo.8338798>`_
+* Cite the `paper <https://doi.org/10.21105/joss.06096>`_ to give credit or shift blame. If you want to cite specific versions, you can find them on `Zenodo <https://dx.doi.org/10.5281/zenodo.8338798>`_.
+
+.. image:: https://joss.theoj.org/papers/10.21105/joss.06096/status.svg
+  :target: https://doi.org/10.21105/joss.06096
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10684537.svg
+  :target: https://doi.org/10.5281/zenodo.10684537
+
```

### Comparing `combine_pvalues_discrete-1.2.2/combine_pvalues_discrete/ctr.py` & `combine_pvalues_discrete-1.2.3/combine_pvalues_discrete/ctr.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 from itertools import permutations
 
 from .tools import sign_test, counted_p, Combined_P_Value, is_empty, searchsorted_closest, has_ties
 from .pdist import PDist
 
 from scipy.special import erfinv, factorial
 from scipy.stats import rankdata, spearmanr, pearsonr, kendalltau, fisher_exact, boschloo_exact, wilcoxon
-from scipy.stats._morestats import _get_wilcoxon_distr
+from scipy.stats._hypotests import _get_wilcoxon_distr
 from scipy.stats._mannwhitneyu import _mwu_state, mannwhitneyu
-from scipy.stats._stats_py import _ttest_finish
 from scipy.stats._mstats_basic import _kendall_p_exact
 from scipy.stats.distributions import hypergeom
 
 def assert_one_sided(alternative):
 	if alternative.lower() == "two-sided":
 		raise NotImplementedError("The two-sided test is not supported (and makes little sense for combining test results).")
 	elif alternative not in ["less","greater"]:
@@ -32,58 +31,73 @@
 	p
 		The *p* value yielded by the test for the investigated sub-dataset.
 	
 	all_ps
 		An iterable containing all possible *p* values of the test for datasets with the same size as the dataset for this individual test.
 		If `None` or empty, all *p* values will be considered possible, i.e., the test will be assumed to be continuous.
 	
+	dof
+		Number of degrees of freedom that affect the test’s outcome; only relevant for automatic weighting (see the `weights` argument of `combine`).
+	
 	Examples
 	--------
 	.. code-block:: python3
 	
 		p = 0.1
 		possible_ps = [0.1,0.5,1]
-		ctr = CTR(p,possible_ps)
+		dof = 7
+		ctr = CTR(p,possible_ps,dof)
 	
 	"""
-	def __init__(self,p,all_ps=None):
+	def __init__(self,p,all_ps=None,dof=None):
 		if p==0: raise ValueError("p value cannot be zero.")
 		if np.isnan(p): raise ValueError("p value must not be NaN.")
 		
 		if not is_empty(all_ps) and p not in all_ps:
 			all_ps = np.asarray(all_ps)
 			closest = all_ps[np.argmin(np.abs(all_ps-p))]
 			if (closest-p)/p > 1e-10:
 				raise ValueError(f"p value {p} must be in `all_ps`.")
 			else:
 				p = closest
 		
 		self.p = p
 		self.nulldist = PDist(all_ps)
 		self.q = self.nulldist.complement(self.p)
+		self.dof = dof
 	
 	def __repr__(self):
-		return f"CombinableTestResult(\n\t p-value: {self.p},\n\t nulldist: {self.nulldist}\n )"
+		return f"""CombinableTestResult(
+		\t p-value: {self.p},
+		\t nulldist: {self.nulldist}
+		\t degrees of freedom: {self.dof}
+		\t )"""
 	
 	def __eq__(self,other):
 		return self._approx(other,atol=0)
 	
 	def _approx(self,other,atol=1e-14):
 		"""
 		Whether this result is identical to another with in an absolute tolerance `atol` between *p* values.
 		"""
-		return abs(self.p-other.p)<=atol and self.nulldist.approx(other.nulldist,atol)
+		return (
+				abs(self.p-other.p) <= atol and
+				self.nulldist.approx(other.nulldist,atol) and
+				self.dof == other.dof
+			)
 	
 	@classmethod
 	def mann_whitney_u( cls, x, y, **kwargs ):
 		"""
 		Creates an object representing the result of a single Mann–Whitney *U* test (using SciPy’s `mannwhitneyu`).
 		
 		Ties are not supported yet because I expect them not to occur in the scenarios that require test combinations (but I may be wrong about this) and they make things much more complicated.
 		
+		For automatic weighting, the number of degrees of freedom is taken to be `len(x) + len(y) - 1`. Note how this aligns with the sign test and Wilcoxon’s signed rank test when either `x` or `y` has size 1.
+		
 		Parameters
 		----------
 		x,y
 			The two iterables of samples to compare.
 		
 		kwargs
 			Further keyword arguments to be passed on to SciPy’s `mannwhitneyu`, such as `alternative`.
@@ -108,22 +122,24 @@
 		
 		n,m = len(x),len(y)
 		
 		if kwargs.pop("method","exact") != "exact":
 			warn('Can only use `method="exact"`.')
 		
 		p = mannwhitneyu(x,y,method="exact",**kwargs).pvalue
-		possible_ps = [ _mwu_state.cdf( U,n,m ) for U in range(n*m+1) ]
-		return cls( p, possible_ps )
+		possible_ps = [ _mwu_state.cdf(U,n,m) for U in range(n*m+1) ]
+		return cls( p, possible_ps, n+m-1 )
 	
 	@classmethod
 	def sign_test( cls, x, y=0, alternative="less" ):
 		"""
 		Creates an object representing the result of a single sign test.
 		
+		For automatic weighting, the number of pairs is taken as the number of degrees of freedom.
+		
 		Parameters
 		----------
 		x,y
 			The two arrays of paired samples to compare. If `y` is a number, a one-sample sign test is performed with `y` as the median. With `y` as an iterable, the two-sample test is performed.
 		
 		alternative: "less" or "greater"
 		
@@ -137,21 +153,24 @@
 		"""
 		
 		assert_one_sided(alternative)
 		
 		p,m,_ = sign_test(x,y,alternative)
 		
 		all_ps = list( np.cumsum([math.comb(m,i)/2**m for i in range(m)]) ) + [1]
-		return cls( p, all_ps )
+		
+		return cls( p, all_ps, m )
 	
 	@classmethod
 	def wilcoxon_signed_rank( cls, x, y=None, alternative="less" ):
 		"""
 		Creates an object representing the result of a single Wilcoxon signed-rank test.
 		
+		For automatic weighting, the number of pairs is taken as the number of degrees of freedom.
+		
 		Parameters
 		----------
 		x,y
 			The two arrays of paired samples to compare. If `y` is `None`, the one-sample test is performed, otherwise the two-sample one.
 		
 		alternative: "less" or "greater"
 		
@@ -170,22 +189,24 @@
 		if has_ties(np.abs(d)) or np.any(d==0):
 			raise NotImplementedError("Ties and zeros are not yet implemented.")
 		
 		n = len(x)
 		all_ps = np.cumsum( _get_wilcoxon_distr(n) )
 		p = wilcoxon(x,y,alternative=alternative,mode="exact").pvalue
 		
-		return cls( p, all_ps )
+		return cls( p, all_ps, n )
 	
 	@classmethod
 	def spearmanr( cls, x, y, alternative="greater", n_thresh=9 ):
 		"""
 		Creates an object representing the result of a single Spearman’s ρ test.
 		If the size of `x` and `y`, *n,* is smaller than `n_thresh`, *p* values are exactly determined using a permutation test. Otherwise *p* values are computed using SciPy’s `spearmanr` assuming a uniform distribution of *p* values and ensuring :math:`p≥\\frac{1}{n!}`.
 		
+		For automatic weighting, the number of degrees of freedom is taken to be one less than the number of pairs.
+		
 		Parameters
 		----------
 		x,y
 			The two arrays of samples to correlate.
 		
 		alternative: "greater" or "less"
 		
@@ -201,15 +222,15 @@
 			ctr = CTR.spearmanr(dataset_A,dataset_B,alternative="greater")
 		"""
 		n = len(x)
 		
 		if n>n_thresh:
 			p = spearmanr(x,y,alternative=alternative).pvalue
 			p = np.clip( p, 1/factorial(n), 1 )
-			return cls(p)
+			return cls(p,dof=n-1)
 		
 		# Working with n³·cov(2R(x),2R(y)) because it is integer. As a statistics, it is equivalent to Spearman’s ρ.
 		x_r = np.fix(2*rankdata(x)).astype(int)
 		y_r = np.fix(2*rankdata(y)).astype(int)
 		x_normed = n*x_r - np.sum(x_r)
 		y_normed = n*y_r - np.sum(y_r)
 		
@@ -224,22 +245,24 @@
 		assert_one_sided(alternative)
 		
 		k = len(possible_covs)
 		# Using the last of duplicate covs by updating dictionary in the right order:
 		cov_to_p = dict( zip( possible_covs, np.linspace(1/k,1,k) ) )
 		
 		orig_p = cov_to_p[orig_cov]
-		return cls( orig_p, list(cov_to_p.values()) )
+		return cls( orig_p, list(cov_to_p.values()), n-1 )
 	
 	@classmethod
 	def kendalltau( cls, x, y, **kwargs ):
 		"""
 		Creates an object representing the result of a single Kendall’s τ test using SciPy’s `kendalltau` to compute *p* values.
 		
-		NaNs and ties are not supported.
+		NaNs and ties are not supported yet.
+		
+		For automatic weighting, the number of degrees of freedom is taken to be one less than the number of pairs.
 		
 		Parameters
 		----------
 		x,y
 			The two arrays of samples to correlate.
 		
 		alternative: "greater" or "less"
@@ -263,20 +286,22 @@
 		tot = math.comb(n,2)
 		
 		possible_ps = [
 			_kendall_p_exact(n,dis,"greater")
 			for dis in range(0,math.comb(n,2)+1)
 		]
 		
-		return cls(p,possible_ps)
+		return cls(p,possible_ps,n-1)
 	
 	@classmethod
 	def fisher_exact( cls, C, alternative="less" ):
 		"""
-		Creates an object representing the result of Fisher’s exact test for a single contingency table C. This is unrelated to Fisher’s method of combining *p* values. Note that most scientific applications do not meet the restrictive conditions of this test and Boschloo’s exact test is more appropriate.
+		Creates an object representing the result of Fisher’s exact test for a single contingency table `C`. This is unrelated to Fisher’s method of combining *p* values. Note that, for most scientific applications, the restrictive conditions of this test are not met and Boschloo’s exact test is more appropriate.
+		
+		For automatic weighting, the sum over `C` is taken as the number of degrees of freedom.
 		
 		Parameters
 		----------
 		C: 2×2 array or nested iterable
 			The contingency table.
 		
 		alternative: "less" or "greater"
@@ -298,20 +323,22 @@
 		n ,_  = np.sum(C,axis=0)
 		
 		possible_ps = [
 				hypergeom.cdf( x, n1+n2, n1, n )
 				for x in range( max(0,n-n2), min(n,n1)+1 )
 			]
 		
-		return cls( p, possible_ps )
+		return cls( p, possible_ps, np.sum(C) )
 	
 	@classmethod
 	def boschloo_exact( cls, C, alternative="less", n=32, atol=1e-10 ):
 		"""
-		Creates an object representing the result of Boschloo’s exact for a single contingency table C using SciPy’s implementation.
+		Creates an object representing the result of Boschloo’s exact for a single contingency table `C` using SciPy’s implementation.
+		
+		For automatic weighting, the sum over `C` is taken as the number of degrees of freedom.
 		
 		Parameters
 		----------
 		C: 2×2 array or nested iterable
 			The contingency table.
 		
 		alternative: "less" or "greater"
@@ -351,15 +378,15 @@
 		i = 1
 		while i<len(possible_ps):
 			if possible_ps[i-1]+atol > possible_ps[i]:
 				del possible_ps[i]
 			else:
 				i += 1
 		
-		return cls( p, possible_ps )
+		return cls( p, possible_ps, np.sum(C) )
 
 combining_statistics = {
 	("fisher"          ,"normal"  ): lambda p:  np.sum( np.log(p)     , axis=0 ),
 	("pearson"         ,"normal"  ): lambda q: -np.sum( np.log(q)     , axis=0 ),
 	("mudholkar_george","normal"  ): lambda p,q:np.sum( np.log(p/q)   , axis=0 ),
 	("stouffer"        ,"normal"  ): lambda p:  np.sum( erfinv(2*p-1) , axis=0 ),
 	("tippett"         ,"normal"  ): lambda p:  np.min( p             , axis=0 ),
@@ -448,16 +475,18 @@
 		The direction of the (common) trend that your compound null hypothesis is testing against.
 		Mind that this is not about the sidedness of the individual tests: Those should always be one-sided.
 		
 		* If "less", the compound research hypothesis is that the subtests exhibit a trend towards a low *p* value.
 		* If "greater", the compound research hypothesis is that the subtests exhibit a trend towards high *p* values (close to 1). In this case, the method of choice will be applied to the complements of the *p* values (see `complements`).
 		* If "two-sided", the compound research hypothesis is that the subtests exhibit either of the two above trends. Beware that this is not necessarily the same as just doubling the *p* value of the respective one-sided test, since for some combining methods, a compound dataset may exhibit **both** trends.
 	
-	weights: iterable of numbers
+	weights: iterable of numbers or "dof"
 		Weights for individual results. Does not work for minimum-based methods (Tippett and Simes).
+		
+		If `"dof"`, each test will be weighted with its degrees of freedom, i.e., the number of samples that can independently affect the test’s result. As there is some potential for ambiguity as to what the degrees of freedom of a given test are, please check that they are what you expect by looking at the tests’ documentations or the attribute `dof` of a CombinableTestResult. This particularly applies when combining different tests.
 	
 	n_samples
 		Number of samples used for Monte Carlo simulation. High numbers increase the accuracy, but also the runtime and memory requirements.
 	
 	rtol: non-negative float
 	atol: non-negative float
 		Values of the statistics closer than specified by `atol` and `rtol` are regarded as identical (as in `numpy.isclose`). A small value (such as the default) may improve the results if numerical noise makes values different.
@@ -530,14 +559,16 @@
 				target[:] = ctr.nulldist.sample(which=x,**sampling_kwargs)
 	
 	data_orig = {
 			x : np.array([getattr(ctr,x) for ctr in ctrs])
 			for x in ["p","q"]
 		}
 	
+	if isinstance(weights,str) and weights == "dof":
+		weights = [ ctr.dof for ctr in ctrs ]
 	if weights is not None:
 		data_null["w"] = data_orig["w"] = np.asarray(weights)
 	
 	err_kwargs = {"divide":"ignore","invalid":"ignore"} if (method in statistics_with_inf) else {}
 	with np.errstate(**err_kwargs):
 		orig_stat  = apply_statistics(statistic,data_orig,alternative=alternative)
 		null_stats = apply_statistics(statistic,data_null,alternative=alternative)
@@ -577,14 +608,16 @@
 		statistic = get_statistic(method,weights)
 		
 		data_orig = {
 				x : np.array([getattr(ctr,x) for ctr in ctrs])
 				for x in ["p","q"]
 			}
 		
+		if isinstance(weights,str) and weights == "dof":
+			weights = [ ctr.dof for ctr in ctrs ]
 		if weights is not None:
 			data_orig["w"] = np.asarray(weights)
 		
 		err_kwargs = {"divide":"ignore","invalid":"ignore"} if (method in statistics_with_inf) else {}
 		with np.errstate(**err_kwargs):
 			stats = {
 				case: apply_statistics(statistic,data_orig,alternative=case)
```

### Comparing `combine_pvalues_discrete-1.2.2/combine_pvalues_discrete/pdist.py` & `combine_pvalues_discrete-1.2.3/combine_pvalues_discrete/pdist.py`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/combine_pvalues_discrete/tools.py` & `combine_pvalues_discrete-1.2.3/combine_pvalues_discrete/tools.py`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/combine_pvalues_discrete.egg-info/PKG-INFO` & `combine_pvalues_discrete-1.2.3/combine_pvalues_discrete.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combine_pvalues_discrete
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python toolbox for combining p values from tests with a discrete statistics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
@@ -15,18 +15,25 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: statsmodels; extra == "test"
 Requires-Dist: pytest-rng; extra == "test"
 
 A Python module for combining *p* values of discrete tests.
 
+* Read the `paper <https://doi.org/10.21105/joss.06096>`_ for a short overview; read the `documentation <https://combine-p-values-discrete.rtfd.io>`_ for more.
 * Install with:
 
   * ``pip install combine-pvalues-discrete``
   * ``pip3 install git+git://github.com/BPSB/combine-p-values-discrete``
   * or similar.
 
-* Install requirements for testing with `pip install ".[test]"` (or similar). Run the test with `pytest` (or similar) in the source directory. Run `pytest -m "not slow"` to exclude some particularly time-consuming tests.
-* `Documentation <https://combine-p-values-discrete.rtfd.io>`_
+* Install requirements for testing with ``pip install ".[test]"`` (or similar). Run the test with ``pytest`` (or similar) in the source directory. Run ``pytest -m "not slow"`` to exclude some particularly time-consuming tests.
 * `Issue Tracker <https://github.com/BPSB/combine-p-values-discrete/issues>`_ – Please use this if you need any help with this module, in particular if you are facing any bugs or require features (in particular support for tests).
 * Contributions are welcome. Feel free to discuss them on the issue tracker or just file a pull request.
-* DOI for citing: `10.5281/zenodo.8338798 <https://dx.doi.org/10.5281/zenodo.8338798>`_
+* Cite the `paper <https://doi.org/10.21105/joss.06096>`_ to give credit or shift blame. If you want to cite specific versions, you can find them on `Zenodo <https://dx.doi.org/10.5281/zenodo.8338798>`_.
+
+.. image:: https://joss.theoj.org/papers/10.21105/joss.06096/status.svg
+  :target: https://doi.org/10.21105/joss.06096
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10684537.svg
+  :target: https://doi.org/10.5281/zenodo.10684537
+
```

### Comparing `combine_pvalues_discrete-1.2.2/combine_pvalues_discrete.egg-info/SOURCES.txt` & `combine_pvalues_discrete-1.2.3/combine_pvalues_discrete.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/docs/Makefile` & `combine_pvalues_discrete-1.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/docs/conf.py` & `combine_pvalues_discrete-1.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/docs/index.rst` & `combine_pvalues_discrete-1.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/examples/comparison.py` & `combine_pvalues_discrete-1.2.3/examples/comparison.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,27 +95,27 @@
 Obtaining a precision comparable to `combine` would require an excessive amount of time.
 
 Once more with weights
 ``````````````````````
 
 So far, we have treated the *p* values for each sub-dataset equally.
 However, the different sub-datasets differ considerably in size and thus meaningfulness, e.g., the first contains seven data points while the last only contains two.
-We can account for this by weighing the sub-datasets with their numbers of data points:
+We can account for this by weighting the sub-datasets with their degrees of freedom (number of samples minus one), which are stored with the test results for this purpose:
 
 .. literalinclude:: ../examples/comparison.py
 	:start-after: example-st\u0061rt
 	:dedent: 1
-	:lines: 69-71
+	:lines: 69-70
 
 And like above, we can check this result by comparing to an explicit, computationally expensive simulation of the null hypothesis:
 
 .. literalinclude:: ../examples/comparison.py
 	:start-after: example-st\u0061rt
 	:dedent: 1
-	:lines: 73-85
+	:lines: 72-85
 
 """
 
 if __name__ == "__main__":
 	# example-start
 	data = [# control group  , treatment group
 	        ( [20,44,14,68]  , [73,22,80]    ), # Breed 1
@@ -181,22 +181,22 @@
 	n = 10000
 	null_statistic = [ fisher_statistic(null_sample(data)) for _ in range(n) ]
 	count = np.sum( null_statistic >= data_statistic )
 	p_from_simulation = (count+1)/(n+1)
 	print(p_from_simulation)
 	# 0.0016998300169983002
 	
-	weights = np.array([len(C)+len(T) for C,T in data])
-	print( combine(ctrs,method="fisher",weights=weights) )
-	# Combined_P_Value(pvalue=0.001098999890100011, std=1.0477080696699578e-05)
+	print( combine(ctrs,method="fisher",weights="dof") )
+	# Combined_P_Value(pvalue=0.0011117998888200112, std=1.0537855099673787e-05)
 	
 	def weighted_fisher_statistic(dataset,weights):
 		pvalues = [ mannwhitneyu(C,T,alternative="less").pvalue for C,T in dataset ]
 		return -2*weights.dot(np.log(pvalues))
 	
+	weights = np.array([len(C)+len(T)-1 for C,T in data])
 	weighted_data_statistic = weighted_fisher_statistic(data,weights)
 	weighted_null_statistic = [
 			weighted_fisher_statistic(null_sample(data),weights)
 			for _ in range(n)
 		]
 	weighted_count = np.sum( weighted_null_statistic >= weighted_data_statistic )
 	weighted_p_from_simulation = (weighted_count+1)/(n+1)
```

### Comparing `combine_pvalues_discrete-1.2.2/examples/mwu.py` & `combine_pvalues_discrete-1.2.3/examples/mwu.py`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/examples/simple_example.py` & `combine_pvalues_discrete-1.2.3/examples/simple_example.py`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/paper.bib` & `combine_pvalues_discrete-1.2.3/paper.bib`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/paper.md` & `combine_pvalues_discrete-1.2.3/paper.md`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/setup.py` & `combine_pvalues_discrete-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/tests/test_ctr.py` & `combine_pvalues_discrete-1.2.3/tests/test_ctr.py`

 * *Files 3% similar despite different names*

```diff
@@ -321,7 +321,33 @@
 			alternative = "less",
 		)
 	result_A =   combine(ctrs_A,method=method_A,**kwargs).pvalue
 	result_B = 1-combine(ctrs_B,method=method_B,**kwargs).pvalue
 	
 	assert_matching_p_values( result_A, result_B, n=n_samples, compare=True )
 
+def test_automatic_weights(rng):
+	weights = []
+	ctrs = []
+	for _ in range(10):
+		size_x,size_y = rng.randint(1,10,size=2)
+		x = rng.random(size_x)
+		y = rng.random(size_y)
+		ctrs.append( CTR.mann_whitney_u(x,y,alternative="less") )
+		weights.append( size_x + size_y - 1 )
+	
+	seed = rng.randint(2**32)
+	automatic = combine(
+			ctrs,
+			weights = "dof",
+			RNG = np.random.RandomState(seed),
+			n_samples = n_samples
+		)
+	manual = combine(
+			ctrs,
+			weights = weights,
+			RNG = np.random.RandomState(seed),
+			n_samples = n_samples
+		)
+	assert automatic==manual
+
+
```

### Comparing `combine_pvalues_discrete-1.2.2/tests/test_direction.py` & `combine_pvalues_discrete-1.2.3/tests/test_direction.py`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/tests/test_pdist.py` & `combine_pvalues_discrete-1.2.3/tests/test_pdist.py`

 * *Files identical despite different names*

### Comparing `combine_pvalues_discrete-1.2.2/tests/test_tests.py` & `combine_pvalues_discrete-1.2.3/tests/test_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 
 n_samples = 100000
 
 def test_simple_mwu():
 	assert (
 		CTR.mann_whitney_u([0],[1],alternative="less")
 		==
-		CTR( 0.5, [0.5,1.0] )
+		CTR( 0.5, [0.5,1.0], 1 )
 	)
 
 def test_simple_signtest():
 	assert (
 		CTR.sign_test([0],[1],alternative="less")
 		==
-		CTR( 0.5, [0.5,1.0] )
+		CTR( 0.5, [0.5,1.0], 1 )
 	)
 
 @mark.parametrize("n",range(3,10))
 def test_simple_wilcoxon(n,rng):
 	data = np.arange(1,n+1)*rng.choice([-1,1],n)
 	
 	wilcoxon_kwargs = dict(alternative="less",mode="exact")
@@ -42,34 +42,38 @@
 			wilcoxon( np.arange(1,n+1)*signs, **wilcoxon_kwargs ).pvalue
 			for signs in product([-1,1],repeat=n)
 		})
 	
 	assert (
 		CTR.wilcoxon_signed_rank(data,alternative="less")
 		==
-		CTR( control_p, control_all_ps )
+		CTR( control_p, control_all_ps, n )
 	)
 
 @mark.parametrize(
 		"  x    ,    y   ,    alt   ,   p  ,      all_ps         ",
 	[
 		([1,3,2], [4,5,0], "less"   ,  5/6 , [ 1/6, 1/2, 5/6, 1 ]),
 		([1,3,2], [4,5,0], "greater",  1/2 , [ 1/6, 1/2, 5/6, 1 ]),
 		([1,2,2], [3,3,5], "less"   ,   1  , [ 1/3,           1 ]),
 		([1,2,2], [3,3,5], "greater",  2/3 , [ 2/3,           1 ]),
 	])
 def test_simple_spearman(x,y,alt,p,all_ps):
-	assert CTR.spearmanr( x, y, alternative=alt )._approx( CTR(p,all_ps) )
+	result = CTR.spearmanr( x, y, alternative=alt )
+	control = CTR(p,all_ps,len(x)-1)
+	assert result._approx(control)
 
 @mark.parametrize("alt",["less","greater"])
 def test_spearman_large_dataset(rng,alt):
-	x,y = rng.normal(size=(2,100))
+	n = 100
+	x,y = rng.normal(size=(2,n))
 	ctr = CTR.spearmanr(x,y,alternative=alt)
 	assert ctr.p == spearmanr(x,y,alternative=alt).pvalue
 	assert ctr.nulldist.continuous
+	assert ctr.dof == n-1
 
 def test_spearman_large_perfect_dataset():
 	n = 100
 	ctr = CTR.spearmanr(range(n),range(n),alternative="greater")
 	assert ctr.p >= 1/math.factorial(n)
 
 @mark.parametrize("n",range(2,9))
@@ -120,40 +124,42 @@
 @mark.parametrize(
 		"    x    ,     y    ,    alt   ,    p   ,                all_ps                 ",
 	[
 		([1,3,2,4], [4,5,0,6], "less"   ,  23/24 , [ 1/24, 1/6, 3/8, 5/8, 5/6, 23/24, 1 ]),
 		([1,3,2,4], [4,5,0,6], "greater",   1/6  , [ 1/24, 1/6, 3/8, 5/8, 5/6, 23/24, 1 ]),
 	])
 def test_simple_kendall(x,y,alt,p,all_ps):
-	result = CTR.kendalltau( x, y, alternative=alt )
+	result = CTR.kendalltau(x,y,alternative=alt)
 	control_p = kendalltau(x,y,alternative=alt).pvalue
-	assert result._approx( CTR(p,all_ps) )
+	n = len(x)
+	assert result._approx( CTR(p,all_ps,n-1) )
 	assert np.isclose( result.p, control_p )
 
 @mark.parametrize(
 		"      C      ,   alt    ,    p    ,            all_ps            ",
 	[
 		([[2,3],[4,0]], "less"   ,   5/42  , [  5/42 , 25/42 ,  20/21 , 1 ]),
 		([[2,3],[4,0]], "greater",    1    , [  1/21 , 17/42 ,  37/42 , 1 ]),
 		([[1,7],[2,7]], "less"   ,  93/170 , [ 21/170, 93/170,  78/85 , 1 ]),
 		([[1,7],[2,7]], "greater", 149/170 , [  7/85 , 77/170, 149/170, 1 ]),
 	])
 def test_simple_fisher_exact(C,alt,p,all_ps):
 	result = CTR.fisher_exact( C, alternative=alt )
 	control_p = fisher_exact(C,alternative=alt)[1]
-	assert result._approx( CTR(p,all_ps) )
+	assert result._approx( CTR(p,all_ps,np.sum(C)) )
 	assert np.isclose( result.p, control_p )
 
 def test_simple_boschloo():
 	C = [[1,2],[3,0]]
 	result = CTR.boschloo_exact( C, alternative="less" )
 	control_p = boschloo_exact(C,alternative="less" ).pvalue
 	assert np.isclose( result.p, control_p )
 	all_ps = [ 1/64, 0.079305, 0.273032, 11/32, 0.57860, 49/64, 1 ]
-	assert result._approx( CTR(0.079305,all_ps), atol=1e-5 )
+	control = CTR(0.079305,all_ps,np.sum(C))
+	assert result._approx(control,atol=1e-5)
 
 # -----------------
 
 # What follows are extensive simulations checking the null distributions of the combined p values as well as comparing the combined p values with those obtained by extensive null models. We first prepare utility functions for two tests (sign test and MWU test). We use Fisher’s method, hence the sums of logarithms of p values (logp_sum).
 
 def mwu_combine( data, **kwargs ):
 	ctrs = [ CTR.mann_whitney_u(X,Y,alternative="less") for X,Y in data ]
```

### Comparing `combine_pvalues_discrete-1.2.2/tests/test_tools.py` & `combine_pvalues_discrete-1.2.3/tests/test_tools.py`

 * *Files identical despite different names*

