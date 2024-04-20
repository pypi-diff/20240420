# Comparing `tmp/fastdfe-1.1.5.tar.gz` & `tmp/fastdfe-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdfe-1.1.5.tar", max compression
+gzip compressed data, was "fastdfe-1.1.6.tar", max compression
```

## Comparing `fastdfe-1.1.5.tar` & `fastdfe-1.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1087 2024-03-12 11:01:01.557068 fastdfe-1.1.5/LICENSE
--rw-r--r--   0        0        0      915 2024-03-12 11:01:01.557068 fastdfe-1.1.5/README.md
--rw-r--r--   0        0        0     6100 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/__init__.py
--rw-r--r--   0        0        0    22839 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/abstract_inference.py
--rw-r--r--   0        0        0   159047 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/annotation.py
--rw-r--r--   0        0        0    55002 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/base_inference.py
--rw-r--r--   0        0        0     4953 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/bootstrap.py
--rw-r--r--   0        0        0    11527 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/config.py
--rw-r--r--   0        0        0    16167 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/discretization.py
--rw-r--r--   0        0        0    21570 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/filtration.py
--rw-r--r--   0        0        0    23736 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/io_handlers.py
--rw-r--r--   0        0        0    52090 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/joint_inference.py
--rw-r--r--   0        0        0     3903 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/json_handlers.py
--rw-r--r--   0        0        0     2556 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/likelihood.py
--rw-r--r--   0        0        0    41530 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/optimization.py
--rw-r--r--   0        0        0    30482 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/parametrization.py
--rw-r--r--   0        0        0    46334 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/parser.py
--rw-r--r--   0        0        0    13206 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/polydfe.py
--rw-r--r--   0        0        0     5274 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/polydfe_utils.py
--rw-r--r--   0        0        0      276 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/settings.py
--rw-r--r--   0        0        0    30541 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/spectrum.py
--rw-r--r--   0        0        0    32552 2024-03-12 11:01:01.573068 fastdfe-1.1.5/fastdfe/visualization.py
--rw-r--r--   0        0        0     1016 2024-03-12 11:01:01.577068 fastdfe-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     2087 1970-01-01 00:00:00.000000 fastdfe-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-04-20 09:19:01.722933 fastdfe-1.1.6/LICENSE
+-rw-r--r--   0        0        0     1154 2024-04-20 09:19:01.722933 fastdfe-1.1.6/README.md
+-rw-r--r--   0        0        0     6050 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/__init__.py
+-rw-r--r--   0        0        0    22930 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/abstract_inference.py
+-rw-r--r--   0        0        0   159257 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/annotation.py
+-rw-r--r--   0        0        0    55241 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/base_inference.py
+-rw-r--r--   0        0        0     4953 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/bootstrap.py
+-rw-r--r--   0        0        0    11527 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/config.py
+-rw-r--r--   0        0        0    16167 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/discretization.py
+-rw-r--r--   0        0        0    21750 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/filtration.py
+-rw-r--r--   0        0        0    23736 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/io_handlers.py
+-rw-r--r--   0        0        0    52126 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/joint_inference.py
+-rw-r--r--   0        0        0     3912 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/json_handlers.py
+-rw-r--r--   0        0        0     2556 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/likelihood.py
+-rw-r--r--   0        0        0    41556 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/optimization.py
+-rw-r--r--   0        0        0    30449 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/parametrization.py
+-rw-r--r--   0        0        0    46334 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/parser.py
+-rw-r--r--   0        0        0    13173 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/polydfe.py
+-rw-r--r--   0        0        0     5274 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/polydfe_utils.py
+-rw-r--r--   0        0        0      276 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/settings.py
+-rw-r--r--   0        0        0    30571 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/spectrum.py
+-rw-r--r--   0        0        0    32440 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/visualization.py
+-rw-r--r--   0        0        0     1016 2024-04-20 09:19:01.746933 fastdfe-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2326 1970-01-01 00:00:00.000000 fastdfe-1.1.6/PKG-INFO
```

### Comparing `fastdfe-1.1.5/LICENSE` & `fastdfe-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastdfe-1.1.5/README.md` & `fastdfe-1.1.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+# fastDFE  <img align="right" width="100" src="https://raw.githubusercontent.com/Sendrowski/fastDFE/master/docs/logo.png">
 [![tests](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml)
 [![codecov](https://codecov.io/gh/Sendrowski/fastDFE/branch/master/graph/badge.svg?token=0LUE8SZYBJ)](https://codecov.io/gh/Sendrowski/fastDFE)
 [![Documentation Status](https://readthedocs.org/projects/fastdfe/badge/?version=latest)](https://fastdfe.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/fastdfe.svg)](https://badge.fury.io/py/fastdfe)
+[![DOI](https://img.shields.io/badge/DOI-10.1093/molbev/msae070-blue)](https://doi.org/10.1093/molbev/msae070)
 
-fastDFE is a package for fast, flexible, and hierarchical inference of the distribution of fitness effects (DFE) from site frequency spectra (SFS). It also contains a versatile VCF-to-SFS parser with support for ancestral allele and site-degeneracy annotation.
+
+``fastdfe`` is a package for fast, flexible, and hierarchical inference of the distribution of fitness effects (DFE) from site frequency spectra (SFS). It also contains a versatile VCF-to-SFS parser with support for ancestral allele and site-degeneracy annotation.
 
 Please see the [documentation](https://fastdfe.readthedocs.io/en/latest/) for all the details.
```

### Comparing `fastdfe-1.1.5/fastdfe/__init__.py` & `fastdfe-1.1.6/fastdfe/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,40 +2,43 @@
 fastDFE package.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-03-10"
 
-__version__ = '1.1.5'
+__version__ = '1.1.6'
 
 import logging
 import sys
 import warnings
 
 import jsonpickle
-import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 
 from .json_handlers import DataframeHandler, SpectrumHandler, SpectraHandler, NumpyArrayHandler
 from .spectrum import Spectrum, Spectra
 
 # set the default figure size
-plt.rcParams['figure.figsize'] = np.array([6.4, 4.8]) * 0.8
+# plt.rcParams['figure.figsize'] = np.array([6.4, 4.8]) * 0.8
 
 # register custom handles
 jsonpickle.handlers.registry.register(pd.DataFrame, DataframeHandler)
 jsonpickle.handlers.registry.register(Spectrum, SpectrumHandler)
 jsonpickle.handlers.registry.register(Spectra, SpectraHandler)
 jsonpickle.handlers.registry.register(np.ndarray, NumpyArrayHandler)
 
 
 class TqdmLoggingHandler(logging.Handler):
+    """
+    TQDM logging handler
+    """
+
     def __init__(self, level=logging.NOTSET):
         """
         Initialize the handler.
 
         :param level:
         """
         super().__init__(level)
@@ -127,15 +130,14 @@
     GammaDiscreteParametrization, DisplacedGammaParametrization, DiscreteFractionalParametrization
 from .config import Config
 from .settings import Settings
 from .abstract_inference import Inference
 from .base_inference import BaseInference, InferenceResults
 from .joint_inference import JointInference, SharedParams
 from .optimization import Covariate
-from .visualization import Visualization
 from .spectrum import Spectrum, Spectra
 from .parser import Parser, Stratification, BaseTransitionStratification, BaseContextStratification, \
     DegeneracyStratification, TransitionTransversionStratification, AncestralBaseStratification, \
     SynonymyStratification, VEPStratification, SnpEffStratification, ContigStratification, ChunkedStratification, \
     TargetSiteCounter
 from .io_handlers import VCFHandler, FASTAHandler, GFFHandler, FileHandler
 from .annotation import Annotator, Annotation, MaximumParsimonyAncestralAnnotation, SiteInfo, \
@@ -155,15 +157,14 @@
     'Config',
     'Settings',
     'Inference',
     'BaseInference',
     'JointInference',
     'SharedParams',
     'Covariate',
-    'Visualization',
     'Spectrum',
     'Spectra',
     'Parser',
     'FileHandler',
     'VCFHandler',
     'FASTAHandler',
     'GFFHandler',
```

### Comparing `fastdfe-1.1.5/fastdfe/abstract_inference.py` & `fastdfe-1.1.6/fastdfe/abstract_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,18 @@
 import logging
 from abc import ABC, abstractmethod
 from typing import List, Optional, Literal, Tuple, Dict
 
 import jsonpickle
 import numpy as np
 import pandas as pd
-from matplotlib import pyplot as plt
 from typing_extensions import Self
 
 from .bootstrap import Bootstrap
 from .parametrization import Parametrization, _from_string
-from .visualization import Visualization
 
 logger = logging.getLogger("fastdfe")
 
 
 class Inference:
     """
     Static utility methods for inference objects.
@@ -35,19 +33,19 @@
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'discretized DFEs',
             labels: list | np.ndarray = None,
-            ax: plt.Axes = None,
+            ax: 'plt.Axes' = None,
             kwargs_legend: dict = dict(prop=dict(size=8)),
             **kwargs
 
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Visualize several discretized DFEs given by the list of inference objects.
 
         :param inferences: List of inference objects.
         :param intervals: Intervals to use for discretization.
         :param confidence_intervals: Whether to plot confidence intervals.
         :param ci_level: Confidence level for confidence intervals.
@@ -57,14 +55,16 @@
         :param title: Title of the plot.
         :param labels: Labels for the DFEs.
         :param kwargs: Additional arguments for the plot.
         :param ax: Axes to plot on. Only for Python visualization backend.
         :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`. Only for Python visualization backend.
         :return: Axes of the plot.
         """
+        from .visualization import Visualization
+
         # get data from inference objects
         values = []
         errors = []
         for i, inference in enumerate(inferences):
             val, errs = inference.get_discretized(
                 intervals=np.array(intervals),
                 confidence_intervals=confidence_intervals,
@@ -97,19 +97,19 @@
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'continuous DFEs',
             labels: list | np.ndarray = None,
             scale: Literal['lin', 'log', 'symlog'] = 'lin',
             scale_density: bool = False,
-            ax: plt.Axes = None,
+            ax: 'plt.Axes' = None,
             kwargs_legend: dict = dict(prop=dict(size=8)),
             **kwargs
 
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Visualize several DFEs given by the list of inference objects.
         By default, the PDF is plotted as is. Due to the logarithmic scale on
         the x-axis, we may get a wrong intuition on how the mass is distributed,
         however. To get a better intuition, we can optionally scale the density
         by the x-axis interval size using ``scale_density = True``. This has the
         disadvantage that the density now changes for x, so that even a constant
@@ -127,14 +127,16 @@
         :param scale: y-scale of the plot.
         :param scale_density: Whether to scale the density by the x-axis interval size.
         :param ax: Axes to plot on. Only for Python visualization backend.
         :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`. Only for Python visualization backend.
         :param kwargs: Additional arguments for the plot.
         :return: Axes of the plot.
         """
+        from .visualization import Visualization
+
         # get data from inference objects
         values = []
         errors = []
         for i, inf in enumerate(inferences):
             val, errs = inf.get_discretized(
                 intervals=intervals,
                 confidence_intervals=confidence_intervals,
@@ -158,39 +160,40 @@
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'parameter estimates',
             scale: Literal['lin', 'log', 'symlog'] = 'log',
-            ax: plt.Axes = None,
+            ax: 'plt.Axes' = None,
             kwargs_legend: dict = dict(prop=dict(size=8), loc='upper right'),
             **kwargs
 
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Visualize several discretized DFEs given by the list of inference objects.
         Note that the DFE parametrization needs to be the same for all inference objects.
 
         :param inferences: List of inference objects.
         :param labels: Unique labels for the DFEs.
         :param scale: y-scale of the plot.
-        :param legend: Whether to show a legend.
         :param confidence_intervals: Whether to plot confidence intervals.
         :param ci_level: Confidence level for confidence intervals.
         :param bootstrap_type: Type of bootstrap to use for confidence intervals.
         :param file: Path to file to save the plot to.
         :param show: Whether to show the plot.
         :param title: Title of the plot.
         :param ax: Axes to plot on. Only for Python visualization backend.
         :return: Axes of the plot.
         :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`. Only for Python visualization backend.
         :param kwargs: Additional arguments which are ignored.
         :raises ValueError: If no inference objects are given.
         """
+        from .visualization import Visualization
+
         if len(inferences) == 0:
             raise ValueError('No inference objects given.')
 
         # get sorted list of parameter names
         param_names = sorted(list(inferences[0].get_bootstrap_param_names()))
 
         # get errors and values
@@ -221,28 +224,30 @@
     def plot_inferred_parameters_boxplot(
             inferences: List['AbstractInference'],
             labels: list | np.ndarray,
             file: str = None,
             show: bool = True,
             title: str = 'parameter estimates',
             **kwargs
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Visualize several discretized DFEs given by the list of inference objects.
         Note that the DFE parametrization needs to be the same for all inference objects.
 
         :param inferences: List of inference objects.
         :param labels: Unique labels for the DFEs.
         :param file: Path to file to save the plot to.
         :param show: Whether to show the plot.
         :param title: Title of the plot.
         :param kwargs: Additional arguments for the plot.
         :return: Axes of the plot.
         :raises ValueError: If no inference objects are given or no bootstraps are found.
         """
+        from .visualization import Visualization
+
         if len(inferences) == 0:
             raise ValueError('No inference objects given.')
 
         # get sorted list of parameter names
         param_names = sorted(list(inferences[0].get_bootstrap_param_names()))
 
         if inferences[0].bootstraps is None:
@@ -517,17 +522,17 @@
             file: str = None,
             show: bool = True,
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             title: str = 'discretized DFE',
-            ax: plt.Axes = None,
+            ax: 'plt.Axes' = None,
             kwargs_legend: dict = dict(prop=dict(size=8)),
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Plot discretized DFE.
 
         :param title: Title of the plot
         :param bootstrap_type: Type of bootstrap
         :param ci_level: Confidence interval level
         :param confidence_intervals: Whether to plot confidence intervals
```

### Comparing `fastdfe-1.1.5/fastdfe/annotation.py` & `fastdfe-1.1.6/fastdfe/annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,25 +24,22 @@
 import numpy as np
 import pandas as pd
 from Bio import Phylo
 from Bio.Phylo.BaseTree import Clade, Tree
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
 from cyvcf2 import Variant, Writer, VCF
-from matplotlib import pyplot as plt
-from scipy.optimize import minimize, OptimizeResult
 from scipy.stats import hypergeom
 from tqdm import tqdm
 
 from .io_handlers import DummyVariant, MultiHandler, FASTAHandler
 from .io_handlers import GFFHandler, get_major_base, get_called_bases
 from .optimization import parallelize as parallelize_func, check_bounds
 from .settings import Settings
 from .spectrum import Spectra
-from .visualization import Visualization
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 # order of the bases important
 bases = np.array(['A', 'C', 'G', 'T'])
 
@@ -67,14 +64,17 @@
 # We count the third position of the isoleucine codon as 2-fold degenerate.
 # This is the only site that would normally have 3-fold degeneracy
 # (https://en.wikipedia.org/wiki/Codon_degeneracy)
 unique_to_degeneracy = {0: 0, 1: 2, 2: 2, 3: 4}
 
 
 class Annotation(ABC):
+    """
+    Base class for annotations.
+    """
 
     def __init__(self):
         """
         Create a new annotation instance.
         """
         #: The logger.
         self._logger = logger.getChild(self.__class__.__name__)
@@ -1253,24 +1253,26 @@
     first_node_ancestral: str = '.'
 
     #: The branch rates.
     rate_params: Dict[str, float] = field(default_factory=dict)
 
     def plot_tree(
             self,
-            ax: plt.Axes = None,
+            ax: 'plt.Axes' = None,
             show: bool = True,
     ):
         """
         Plot the tree for a site. Only Python visualization is supported.
 
         :param self: The site information.
         :param ax: Axes to plot on.
         :param show: Whether to show the plot.
         """
+        import matplotlib.pyplot as plt
+
         if ax is None:
             ax = plt.gca()
 
         if 'K' in self.rate_params:
             branch_lengths = {f'K{i}': self.rate_params['K'] for i in range(len(self.outgroup_bases) * 2 - 1)}
         else:
             branch_lengths = self.rate_params
@@ -1401,28 +1403,30 @@
 
     def plot(
             self,
             file: str = None,
             show: bool = True,
             title: str = 'polarization probabilities',
             scale: Literal['lin', 'log'] = 'lin',
-            ax: plt.Axes = None,
+            ax: 'plt.Axes' = None,
             ylabel: str = 'p'
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Visualize the polarization probabilities using a scatter plot.
 
         :param scale: y-scale of the plot.
         :param title: Plot title.
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param ax: Axes to plot on. Only for Python visualization backend.
         :param ylabel: y-axis label.
         :return: Axes object
         """
+        from .visualization import Visualization
+
         if self.probabilities is None:
             raise ValueError('Polarization probabilities have not been calculated yet.')
 
         return Visualization.plot_scatter(
             values=self.probabilities,
             file=file,
             show=show,
@@ -1507,14 +1511,15 @@
         """
         Get the polarization probabilities.
 
         :param configs: The site configurations.
         :param n_ingroups: The number of ingroups.
         :return: The polarization probabilities.
         """
+        from scipy.optimize import minimize, OptimizeResult
 
         # folded frequency bin indices
         # if the number of polymorphic bins is odd, the middle bin is fixed
         freq_indices = range(1, (n_ingroups + 1) // 2)
 
         # get the likelihood functions
         funcs = dict((i, self._get_likelihood(i, configs, n_ingroups)) for i in freq_indices)
@@ -2205,15 +2210,15 @@
         #: The log likelihoods for the different runs when optimizing the rate parameters.
         self.likelihoods: np.ndarray[float, (...,)] | None = None
 
         #: The best log likelihood when optimizing the rate parameters.
         self.likelihood: float | None = None
 
         #: Optimization result of the best run.
-        self.result: OptimizeResult | None = None
+        self.result: Optional['scipy.optimize.OptimizeResult'] = None
 
         #: The MLE parameters.
         self.params_mle: Dict[str, float] | None = None
 
         #: Mismatches between the most likely ancestral allele and the ad-hoc ancestral allele.
         # This is only computed when annotating a VCF file, and only contains the mismatches
         # for sites that were actually annotated.
@@ -2873,14 +2878,16 @@
 
     def infer(self):
         """
         Infer the ancestral allele probabilities for the data provided. This method is only supposed to be called
         manually if the data is provided directly, e.g. using :meth:`from_data`, :meth:`from_dataframe` or
         :meth:`from_est_sfs`. If the data is provided using a VCF file, this method is called automatically.
         """
+        from scipy.optimize import minimize, OptimizeResult
+
         # get the bounds
         bounds = self.model.get_bounds(self.n_outgroups)
 
         # get the likelihood function
         # this will raise an error if no data is available
         fun = self._get_likelihood()
 
@@ -3655,28 +3662,30 @@
 
     def plot_likelihoods(
             self,
             file: str = None,
             show: bool = True,
             title: str = 'rate likelihoods',
             scale: Literal['lin', 'log'] = 'lin',
-            ax: plt.Axes = None,
+            ax: 'plt.Axes' = None,
             ylabel: str = 'lnl'
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Visualize the likelihoods of the rate optimization runs using a scatter plot.
 
         :param scale: y-scale of the plot.
         :param title: Plot title.
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param ax: Axes to plot on. Only for Python visualization backend.
         :param ylabel: Label for y-axis.
         :return: Axes object
         """
+        from .visualization import Visualization
+
         return Visualization.plot_scatter(
             values=self.likelihoods,
             file=file,
             show=show,
             title=title,
             scale=scale,
             ax=ax,
```

### Comparing `fastdfe-1.1.5/fastdfe/base_inference.py` & `fastdfe-1.1.6/fastdfe/base_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,31 +14,28 @@
 import time
 from typing import List, Optional, Dict, Literal, cast, Tuple
 
 import jsonpickle
 import multiprocess as mp
 import numpy as np
 import pandas as pd
-from matplotlib import pyplot as plt
 from numpy.linalg import norm
-from scipy.optimize._optimize import OptimizeResult
 from scipy.stats import chi2
 from typing_extensions import Self
 
 from . import optimization
 from . import parametrization
 from .abstract_inference import AbstractInference, Inference
 from .config import Config
 from .discretization import Discretization
 from .json_handlers import CustomEncoder
 from .optimization import Optimization, flatten_dict, pack_params, expand_fixed, unpack_shared
 from .parametrization import Parametrization, _from_string
 from .spectrum import Spectrum, Spectra
 from .spectrum import standard_kingman
-from .visualization import Visualization
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 
 class BaseInference(AbstractInference):
     """
@@ -234,15 +231,15 @@
         #: Likelihoods of the different ML runs, controlled by ``n_runs``
         self.likelihoods: Optional[List[float]] = None
 
         #: Number of MLE runs to perform
         self.n_runs: int = n_runs
 
         #: Numerical optimization result
-        self.result: Optional[OptimizeResult] = None
+        self.result: Optional['scipy.optimize.OptimizeResult'] = None
 
         # Bootstrap options
 
         #: Whether to do bootstrapping
         self.do_bootstrap: bool = do_bootstrap
 
         #: Number of bootstraps
@@ -298,15 +295,15 @@
         #: Initial values
         self.x0 = dict(all=self.model.x0 | self._default_x0 | (x0['all'] if 'all' in x0 else {}))
 
         #: Bootstrapped MLE parameter estimates
         self.bootstraps: Optional[pd.DataFrame] = None
 
         #: Bootstrap optimization results
-        self.bootstrap_results: Optional[List[OptimizeResult]] = None
+        self.bootstrap_results: Optional[List['scipy.optimize.OptimizeResult']] = None
 
         #: L2 norm of differential between modelled and observed SFS
         self.L2_residual: Optional[float] = None
 
         #: Random number generator seed
         self.seed: int | None = int(seed) if seed is not None else None
 
@@ -494,15 +491,15 @@
 
         lk = -self.optimization.get_loss_function(self.get_counts())(params)
 
         self.optimization.x0 = x0_cached
 
         return lk
 
-    def _assign_result(self, result: OptimizeResult, params_mle: dict):
+    def _assign_result(self, result: 'scipy.optimize.OptimizeResult', params_mle: dict):
         """
         Assign optimization result and MLE parameters.
 
         :param params_mle: MLE parameters.
         :param result: Optimization result.
         """
         self.result = result
@@ -544,15 +541,15 @@
         ratio = self.get_residual(1) / self.sfs_sel.n_polymorphic
 
         if ratio > 0.1:
             self._logger.warning("The L1 residual comparing the modelled and observed SFS is rather large: "
                                  f"`norm(sfs_modelled - sfs_observed, 1) / sfs_observed` = {ratio:.3f}. "
                                  "This may indicate that the model does not fit the data well.")
 
-    def _report_result(self, result: OptimizeResult, params: dict):
+    def _report_result(self, result: 'scipy.optimize.OptimizeResult', params: dict):
         """
         Inform on optimization result.
 
         :param params: MLE parameters.
         :param result: Optimization result.
         """
         # report on optimization result
@@ -679,15 +676,15 @@
         Add estimates for alpha to the bootstraps.
         """
         self._logger.debug('Computing estimates for alpha.')
 
         # add alpha estimates
         self.bootstraps['alpha'] = self.bootstraps.apply(lambda r: self.get_alpha(dict(r)), axis=1)
 
-    def _run_bootstrap_sample(self, seed: int) -> (OptimizeResult, dict):
+    def _run_bootstrap_sample(self, seed: int) -> ('scipy.optimize.OptimizeResult', dict):
         """
         Resample the observed selected SFS and rerun the optimization procedure.
         We take the MLE params as initial params here. In case the optimization
         does not terminate normally, we retry up to :attr:`n_bootstrap_retries` times.
 
         :param seed: Seed for random number generator.
         :return: Optimization result and MLE parameters.
@@ -858,17 +855,17 @@
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             scale_density: bool = False,
             scale: Literal['lin', 'log', 'symlog'] = 'lin',
             title: str = 'DFE',
             kwargs_legend: dict = dict(prop=dict(size=8)),
-            ax: plt.Axes = None
+            ax: 'plt.Axes' = None
 
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Plot continuous DFE.
         The special constants np.inf and -np.inf are also valid interval bounds.
         By default, the PDF is plotted as is. Due to the logarithmic scale on
         the x-axis, we may get a wrong intuition on how the mass is distributed,
         however. To get a better intuition, we can optionally scale the density
         by the x-axis interval size using ``scale_density = True``. This has the
@@ -908,28 +905,30 @@
 
     @_run_if_required_wrapper
     def plot_bucket_sizes(
             self,
             file: str = None,
             show: bool = True,
             title: str = 'bucket sizes',
-            ax: plt.Axes = None
+            ax: 'plt.Axes' = None
 
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Plot mass in each bucket for the MLE DFE.
         This can be used to check if the interval bounds and spacing
         are chosen appropriately.
 
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param title: Plot title.
         :param ax: Axes to plot on. Only for Python visualization backend.
         :return: Axes object
         """
+        from .visualization import Visualization
+
         # evaluate at fixed parameters
         sizes = self.model._discretize(self.params_mle, self.discretization.bins)
 
         return Visualization.plot_buckets_sizes(
             n_intervals=self.discretization.n_intervals,
             bins=self.discretization.bins,
             sizes=sizes,
@@ -943,28 +942,30 @@
     def plot_interval_density(
             self,
             file: str = None,
             show: bool = True,
             intervals: list | np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             interval_labels: List[str] = None,
             color: str = 'C0',
-            ax: plt.Axes = None
-    ) -> plt.Axes:
+            ax: 'plt.Axes' = None
+    ) -> 'plt.Axes':
         """
         Plot density of the discretization intervals chosen. Note that although this plot looks similar, this is
         not the DFE!
 
         :param color: Color of the bars.
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param interval_labels: Labels for the intervals.
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
         :param ax: Axes to plot on. Only for Python visualization backend.
         :return: Axes object
         """
+        from .visualization import Visualization
+
         # issue warning
         if not self.discretization.linearized:
             self._logger.warning('Note that the interval density is not important if the DFE was not linearized.')
 
         return Visualization.plot_interval_density(
             density=self.discretization.get_interval_density(intervals),
             file=file,
@@ -978,20 +979,20 @@
     def plot_sfs_comparison(
             self,
             sfs_types: List[Literal['modelled', 'observed', 'selected', 'neutral']] = ['observed', 'modelled'],
             labels: List[str] = None,
             colors: List[str] = None,
             file: str = None,
             show: bool = True,
-            ax: plt.Axes = None,
+            ax: 'plt.Axes' = None,
             title: str = 'SFS comparison',
             use_subplots: bool = False,
             show_monomorphic: bool = False,
             kwargs_legend: dict = dict(prop=dict(size=8)),
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Plot SFS comparison.
 
         :param file: File to save plot to.
         :param labels: Labels for the SFS.
         :param colors: Colors for the SFS. Only for Python visualization backend.
         :param sfs_types: Types of SFS to plot.
@@ -999,14 +1000,16 @@
         :param ax: Axes to plot on. Only for Python visualization backend and if ``use_subplots`` is ``False``.
         :param title: Plot title
         :param use_subplots: Whether to use subplots. Only for Python visualization backend.
         :param show_monomorphic: Whether to show monomorphic counts
         :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`. Only for Python visualization backend.
         :return: Axes object
         """
+        from .visualization import Visualization
+
         if 'modelled' in sfs_types:
             self.run_if_required()
 
         mapping = dict(
             observed=self.sfs_sel,
             selected=self.sfs_sel,
             modelled=self.sfs_mle,
@@ -1027,16 +1030,16 @@
         )
 
     def plot_observed_sfs(
             self,
             labels: List[str] = None,
             file: str = None,
             show: bool = True,
-            ax: plt.Axes = None
-    ) -> plt.Axes:
+            ax: 'plt.Axes' = None
+    ) -> 'plt.Axes':
         """
         Plot neutral and selected SFS.
 
         :param file: File to save plot to.
         :param labels: Labels for the SFS.
         :param show: Whether to show plot.
         :param ax: Axes to plot on. Only for Python visualization backend.
@@ -1093,18 +1096,18 @@
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'parameter estimates',
             scale: Literal['lin', 'log', 'symlog'] = 'log',
-            ax: plt.Axes = None,
+            ax: 'plt.Axes' = None,
             kwargs_legend: dict = dict(prop=dict(size=8), loc='upper right'),
             **kwargs
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Visualize the inferred parameters and their confidence intervals.
 
         :param scale: y-scale of the plot.
         :param title: Plot title.
         :param confidence_intervals: Whether to show confidence intervals.
         :param bootstrap_type: Type of bootstrap to use.
@@ -1132,15 +1135,15 @@
     @_run_if_required_wrapper
     def plot_inferred_parameters_boxplot(
             self,
             file: str = None,
             show: bool = True,
             title: str = 'parameter estimates',
             **kwargs
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Visualize the inferred parameters and their confidence intervals.
 
         :param title: Plot title.
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :return: Axes object
@@ -1157,29 +1160,31 @@
     @_run_if_required_wrapper
     def plot_likelihoods(
             self,
             file: str = None,
             show: bool = True,
             title: str = 'likelihoods',
             scale: Literal['lin', 'log'] = 'lin',
-            ax: plt.Axes = None,
+            ax: 'plt.Axes' = None,
             ylabel: str = 'lnl',
             **kwargs
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Visualize the likelihoods of the optimization runs using a scatter plot.
 
         :param scale: y-scale of the plot.
         :param title: Plot title.
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param ax: Axes to plot on. Only for Python visualization backend.
         :param ylabel: Label for the y-axis.
         :return: Axes object
         """
+        from .visualization import Visualization
+
         return Visualization.plot_scatter(
             values=self.likelihoods,
             file=file,
             show=show,
             title=title,
             scale=scale,
             ax=ax,
@@ -1289,31 +1294,33 @@
             self,
             file: str = None,
             show: bool = True,
             remove_empty: bool = False,
             transpose: bool = False,
             cmap: str = None,
             title: str = 'nested model comparison',
-            ax: plt.Axes = None,
+            ax: 'plt.Axes' = None,
             do_bootstrap: bool = True,
 
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Plot the p-values of nested likelihoods.
 
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param remove_empty: Whether to remove empty rows and columns.
         :param transpose: Whether to transpose the matrix.
         :param cmap: Colormap to use.
         :param title: Plot title.
         :param ax: Axes to plot on. Only for Python visualization backend.
         :param do_bootstrap: Whether to perform bootstrapping. This is recommended to get more accurate p-values.
         :return: Axes object
         """
+        from .visualization import Visualization
+
         # get p-values and names
         P, inferences = self.compare_nested_models(do_bootstrap=do_bootstrap)
 
         # define labels
         labels_x = np.array(list(inferences.keys()))
         labels_y = np.array(list(inferences.keys()))
```

### Comparing `fastdfe-1.1.5/fastdfe/bootstrap.py` & `fastdfe-1.1.6/fastdfe/bootstrap.py`

 * *Files identical despite different names*

### Comparing `fastdfe-1.1.5/fastdfe/config.py` & `fastdfe-1.1.6/fastdfe/config.py`

 * *Files identical despite different names*

### Comparing `fastdfe-1.1.5/fastdfe/discretization.py` & `fastdfe-1.1.6/fastdfe/discretization.py`

 * *Files identical despite different names*

### Comparing `fastdfe-1.1.5/fastdfe/filtration.py` & `fastdfe-1.1.6/fastdfe/filtration.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,21 @@
 def _count_filtered(func: Callable) -> Callable:
     """
     Decorator that increases ``self.n_filtered`` by 1 if the decorated function returns False.
     """
 
     @functools.wraps(func)
     def wrapper(self, variant):
+        """
+        Wrapper function.
+
+        :param self: Self.
+        :param variant: The variant to filter.
+        :return: The result of the decorated function.
+        """
         result = func(self, variant)
         if not result:
             self.n_filtered += 1
         return result
 
     return wrapper
```

### Comparing `fastdfe-1.1.5/fastdfe/io_handlers.py` & `fastdfe-1.1.6/fastdfe/io_handlers.py`

 * *Files identical despite different names*

### Comparing `fastdfe-1.1.5/fastdfe/joint_inference.py` & `fastdfe-1.1.6/fastdfe/joint_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,27 @@
 import time
 from typing import List, Dict, Tuple, Literal, Optional, cast, Callable
 
 import jsonpickle
 import multiprocess as mp
 import numpy as np
 import pandas as pd
-from matplotlib import pyplot as plt
 from numpy.linalg import norm
-from scipy.optimize import OptimizeResult
 from tqdm import tqdm
 
 from .abstract_inference import Inference
 from .base_inference import BaseInference
 from .bootstrap import Bootstrap
 from .config import Config
 from .optimization import Optimization, SharedParams, pack_shared, expand_shared, \
     Covariate, flatten_dict, merge_dicts, correct_values, parallelize as parallelize_func, expand_fixed, \
     collapse_fixed, unpack_shared
 from .parametrization import Parametrization
 from .settings import Settings
 from .spectrum import Spectrum, Spectra
-from .visualization import Visualization
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 
 class JointInference(BaseInference):
     """
@@ -644,15 +641,15 @@
             self.bootstrap_if_required()
 
         # run joint inference without covariates
         simple = self.run_joint_without_covariates(do_bootstrap=do_bootstrap)
 
         return self.lrt(simple.likelihood, self.likelihood, len(self.covariates))
 
-    def _get_run_bootstrap_sample(self) -> Callable[[int], Tuple[OptimizeResult, dict]]:
+    def _get_run_bootstrap_sample(self) -> Callable[[int], Tuple['scipy.optimize.OptimizeResult', dict]]:
         """
         Get function which runs a single bootstrap sample.
 
         :return: Static function which runs a single bootstrap sample, taking an optional seed and returning the
             optimization result and the MLE parameters.
         """
         optimization = self.optimization
@@ -666,15 +663,15 @@
         bounds_linear = self.get_bounds_linear()
         scales = self.scales
         bounds = self.bounds
         n_retries = self.n_bootstrap_retries
         sfs_neut = dict((t, self.marginal_inferences[t].sfs_neut) for t in self.types)
         sfs_sel = dict((t, self.marginal_inferences[t].sfs_sel) for t in self.types)
 
-        def run_bootstrap_sample(seed: int) -> (OptimizeResult, dict):
+        def run_bootstrap_sample(seed: int) -> ('scipy.optimize.OptimizeResult', dict):
             """
             Resample the observed selected SFS and rerun the optimization procedure.
             We take the MLE params as initial params here.
             We make this function static to improve performance when parallelizing.
             In case the optimization does not terminate normally, we retry up to `n_retries` times.
 
             :return: Optimization result and dictionary of MLE params
@@ -959,16 +956,16 @@
             show_marginals: bool = True,
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             title: str = 'discretized DFE comparison',
             labels: List[str] = None,
             kwargs_legend: dict = dict(prop=dict(size=8)),
-            ax: plt.Axes = None
-    ) -> plt.Axes:
+            ax: 'plt.Axes' = None
+    ) -> 'plt.Axes':
         """
         Plot discretized DFE comparing the different types.
 
         :param labels: Labels for types
         :param title: Title of plot
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bars.
         :param show_marginals: Whether to also show marginal inferences
@@ -989,21 +986,21 @@
             self,
             sfs_types: List[Literal['modelled', 'observed', 'selected', 'neutral']] = ['observed', 'modelled'],
             types: List[str] = None,
             labels: List[str] = None,
             colors: List[str] = None,
             file: str = None,
             show: bool = True,
-            ax: plt.Axes = None,
+            ax: 'plt.Axes' = None,
             title: str = 'SFS comparison',
             use_subplots: bool = False,
             show_monomorphic: bool = False,
             kwargs_legend: dict = dict(prop=dict(size=8)),
 
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Plot SFS comparison.
 
         :param types: Types to plot
         :param file: File to save plot to
         :param labels: Labels for types.
         :param colors: Colors for types. Only for Python visualization backend.
@@ -1012,14 +1009,16 @@
         :param ax: Axes to plot on. Only for Python visualization backend and if ``use_subplots`` is ``False``.
         :param title: Plot title
         :param use_subplots: Whether to use subplots. Only for Python visualization backend.
         :param show_monomorphic: Whether to show monomorphic counts
         :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`. Only for Python visualization backend.
         :return: Axes object
         """
+        from .visualization import Visualization
+
         if 'modelled' in sfs_types:
             self.run_if_required()
 
         mapping = dict(
             observed='sfs_sel',
             selected='sfs_sel',
             modelled='sfs_mle',
@@ -1067,16 +1066,16 @@
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             title: str = 'DFE comparison',
             labels: List[str] = None,
             scale_density: bool = False,
             scale: Literal['lin', 'log', 'symlog'] = 'lin',
             kwargs_legend: dict = dict(prop=dict(size=8)),
-            ax: plt.Axes = None
-    ) -> plt.Axes:
+            ax: 'plt.Axes' = None
+    ) -> 'plt.Axes':
         """
         Plot discretized DFE. The special constants ``np.inf`` and ``-np.inf`` are also valid interval bounds.
         By default, the PDF is plotted as is. Due to the logarithmic scale on
         the x-axis, we may get a wrong intuition on how the mass is distributed,
         however. To get a better intuition, we can optionally scale the density
         by the x-axis interval size using ``scale_density = True``. This has the
         disadvantage that the density now changes for x, so that even a constant
@@ -1109,19 +1108,19 @@
             file: str = None,
             confidence_intervals: bool = True,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             ci_level: float = 0.05,
             show: bool = True,
             title: str = 'inferred parameters',
             labels: List[str] = None,
-            ax: plt.Axes = None,
+            ax: 'plt.Axes' = None,
             scale: Literal['lin', 'log', 'symlog'] = 'log',
             kwargs_legend: dict = dict(prop=dict(size=8), loc='upper right'),
             **kwargs: List[str]
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Plot discretized DFE comparing the different types.
 
         :param labels: Labels for types
         :param title: Title of plot
         :param bootstrap_type: Type of bootstrap
         :param ci_level: Confidence level
@@ -1141,15 +1140,15 @@
     def plot_inferred_parameters_boxplot(
             self,
             file: str = None,
             show: bool = True,
             title: str = 'inferred parameters',
             labels: List[str] = None,
             **kwargs: List[str]
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Plot discretized DFE comparing the different types.
 
         :param labels: Labels for types
         :param title: Title of plot
         :param file: File to save plot to
         :param show: Whether to show plot
@@ -1168,16 +1167,16 @@
             show: bool = True,
             title: str = None,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             show_types: bool = True,
             ci_level: float = 0.05,
             xlabel: str = "cov",
             ylabel: str = None,
-            ax: plt.Axes = None
-    ) -> plt.Axes:
+            ax: 'plt.Axes' = None
+    ) -> 'plt.Axes':
         """
         Plot the covariate given by the index.
 
         :param index: The index of the covariate.
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param title: Plot title.
@@ -1185,14 +1184,16 @@
         :param show_types: Whether to show types on second x-axis.
         :param ci_level: Confidence level.
         :param xlabel: X-axis label.
         :param ylabel: Y-axis label, defaults to the covariate parameter name.
         :param ax: Axes to plot on. Only for Python visualization backend.
         :return: Axes object.
         """
+        from .visualization import Visualization
+
         key = f"c{index}"
 
         # check if covariate exists
         if key not in self.covariates:
             raise ValueError(f"Covariate with index {index} does not exist.")
 
         # default title
```

### Comparing `fastdfe-1.1.5/fastdfe/json_handlers.py` & `fastdfe-1.1.6/fastdfe/json_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 import json
 import logging
 
 import numpy as np
 import pandas as pd
 from jsonpickle.handlers import BaseHandler
-from scipy.optimize._lbfgsb_py import LbfgsInvHessProduct
 
 from .optimization import SharedParams, Covariate
 from .parametrization import Parametrization
 from .spectrum import Spectrum, Spectra
 
 # configure logger
 logger = logging.getLogger('fastdfe')
@@ -130,14 +129,16 @@
     def default(self, obj):
         """
         Convert numpy arrays and objects to lists and primitives.
 
         :param obj: Object
         :return: Simplified object
         """
+        from scipy.optimize._lbfgsb_py import LbfgsInvHessProduct
+
         if isinstance(obj, Spectrum):
             return obj.to_list()
 
         if isinstance(obj, Spectra):
             return obj.to_dict()
 
         if isinstance(obj, np.ndarray):
```

### Comparing `fastdfe-1.1.5/fastdfe/likelihood.py` & `fastdfe-1.1.6/fastdfe/likelihood.py`

 * *Files identical despite different names*

### Comparing `fastdfe-1.1.5/fastdfe/optimization.py` & `fastdfe-1.1.6/fastdfe/optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from dataclasses import dataclass
 from typing import Callable, List, Dict, Literal, Tuple, Optional
 
 import multiprocess as mp
 import numpy as np
 from numpy.linalg import norm
 from numpy.random import Generator
-from scipy.optimize import minimize, OptimizeResult
 from scipy.stats import loguniform, uniform
 from tqdm import tqdm
 
 from .likelihood import Likelihood
 from .settings import Settings
 
 # get logger
@@ -891,15 +890,15 @@
             bounds: Dict[str, Tuple[float, float]] = {},
             n_runs: int = 1,
             debug_iterations: bool = True,
             print_info: bool = True,
             opts_mle: dict = None,
             pbar: bool = None,
             desc: str = 'Inferring DFE',
-    ) -> (OptimizeResult, dict):
+    ) -> ('scipy.optimize.OptimizeResult', dict):
         """
         Perform the optimization procedure.
 
         :param scales: Scales of the parameters
         :param bounds: Bounds of the parameters
         :param n_runs: Number of independent optimization runs out of which the best one is chosen. The first run
             will use the initial values if specified. Consider increasing this number if the optimization does not
@@ -909,14 +908,16 @@
         :param debug_iterations: Whether to print debug messages for each iteration
         :param opts_mle: Dictionary of options for the optimizer
         :param print_info: Whether to print information about the bounds
         :param pbar: Whether to show a progress bar
         :param desc: Description for the progress bar
         :return: The optimization result and the likelihoods
         """
+        from scipy.optimize import minimize, OptimizeResult
+
         # number of optimization runs
         self.n_runs = n_runs
 
         # store the scales of the parameters
         if scales:
             self.scales = scales
```

### Comparing `fastdfe-1.1.5/fastdfe/parametrization.py` & `fastdfe-1.1.6/fastdfe/parametrization.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 import logging
 from abc import abstractmethod, ABC
 from functools import wraps
 from typing import Callable, List, Union, Dict, Tuple, Literal
 
 import numpy as np
-from matplotlib import pyplot as plt
 from scipy.stats import gamma, expon
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 
 def _from_string(model: Union['Parametrization', str]) -> 'Parametrization':
@@ -163,17 +162,17 @@
     def plot(
             self,
             params: dict,
             intervals: list | np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             file: str = None,
             show: bool = True,
             title: str = 'discretized DFE',
-            ax: plt.Axes = None
+            ax: 'plt.Axes' = None
 
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Plot the discretized DFE.
 
         :param params: Parameters of the parametrization
         :param intervals: Intervals to use for discretization.
         :param file: File to save the plot to.
         :param show: Whether to show the plot.
```

### Comparing `fastdfe-1.1.5/fastdfe/parser.py` & `fastdfe-1.1.6/fastdfe/parser.py`

 * *Files identical despite different names*

### Comparing `fastdfe-1.1.5/fastdfe/polydfe.py` & `fastdfe-1.1.6/fastdfe/polydfe.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import tempfile
 import time
 from typing import Callable, List, Optional, Literal, Dict
 
 import numpy as np
 import pandas as pd
 import rpy2.robjects as ro
-from matplotlib import pyplot as plt
 from rpy2.robjects.packages import importr
 from rpy2.robjects.vectors import ListVector
 from typing_extensions import Self
 
 from .abstract_inference import AbstractInference, Inference
 from .config import Config
 from .parametrization import _from_string, Parametrization, DiscreteParametrization
@@ -336,17 +335,17 @@
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'parameter estimates',
             scale: Literal['lin', 'log', 'symlog'] = 'log',
             legend: bool = True,
-            ax: plt.Axes = None,
+            ax: 'plt.Axes' = None,
             kwargs_legend: dict = dict(prop=dict(size=8), loc='upper right'),
-    ) -> plt.Axes:
+    ) -> 'plt.Axes':
         """
         Visualize the inferred parameters and their confidence intervals.
 
         :param scale: Scale of the y-axis
         :param confidence_intervals: Whether to show confidence intervals
         :param ci_level: Confidence interval level
         :param bootstrap_type: Type of bootstrap
```

### Comparing `fastdfe-1.1.5/fastdfe/polydfe_utils.py` & `fastdfe-1.1.6/fastdfe/polydfe_utils.py`

 * *Files identical despite different names*

### Comparing `fastdfe-1.1.5/fastdfe/spectrum.py` & `fastdfe-1.1.6/fastdfe/spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 
 import logging
 from functools import cached_property
 from typing import Dict, List, Union, Iterable, Any, Literal
 
 import numpy as np
 import pandas as pd
-from matplotlib import pyplot as plt
 from scipy.stats import hypergeom
 
 from .io_handlers import download_if_url
-from .visualization import Visualization
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 
 def standard_kingman(n: int) -> 'Spectrum':
     """
@@ -400,28 +398,30 @@
             self,
             show: bool = True,
             file: str = None,
             title: str = None,
             log_scale: bool = False,
             show_monomorphic: bool = False,
             kwargs_legend: dict = dict(prop=dict(size=8)),
-            ax: plt.Axes = None
-    ) -> plt.Axes:
+            ax: 'plt.Axes' = None
+    ) -> 'plt.Axes':
         """
         Plot spectrum.
 
         :param show: Whether to show plot.
         :param file: File to save plot to.
         :param title: Title of plot.
         :param log_scale: Whether to use log scale on y-axis.
         :param show_monomorphic: Whether to show monomorphic counts.
         :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`. Only for Python visualization backend.
         :param ax: Axes to plot on. Only for Python visualization backend.
         :return: Axes
         """
+        from .visualization import Visualization
+
         return Visualization.plot_spectra(
             spectra=[self.to_list()],
             file=file,
             show=show,
             title=title,
             log_scale=log_scale,
             show_monomorphic=show_monomorphic,
@@ -876,29 +876,31 @@
             show: bool = True,
             file: str = None,
             title: str = None,
             log_scale: bool = False,
             use_subplots: bool = False,
             show_monomorphic: bool = False,
             kwargs_legend: dict = dict(prop=dict(size=8)),
-            ax: plt.Axes = None
-    ) -> plt.Axes:
+            ax: 'plt.Axes' = None
+    ) -> 'plt.Axes':
         """
         Visualize spectra.
 
         :param show: Whether to show the plot.
         :param file: File name to save the plot to.
         :param title: Plot title.
         :param log_scale: Whether to use log scale on y-axis.
         :param use_subplots: Whether to use subplots. Only for Python visualization backend.
         :param show_monomorphic: Whether to show monomorphic sites.
         :param kwargs_legend: Keyword arguments passed to :meth:`plt.legend`. Only for Python visualization backend.
         :param ax: Axes to plot on. Only for Python visualization backend and if ``use_subplots`` is ``False``.
         :return: Axes
         """
+        from .visualization import Visualization
+
         return Visualization.plot_spectra(
             spectra=list(list(v) for v in self.to_spectra().values()),
             labels=self.types,
             file=file,
             show=show,
             title=title,
             log_scale=log_scale,
```

### Comparing `fastdfe-1.1.5/fastdfe/visualization.py` & `fastdfe-1.1.6/fastdfe/visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,14 @@
 
 
 class Visualization:
     """
     Visualization class.
     """
 
-    # configure color map
-    # plt.rcParams['axes.prop_cycle'] = cycler('color', plt.get_cmap('Set2').colors)
-
     @classmethod
     def change_default_figsize(cls, factor: float | np.ndarray):
         """
         Scale default figure size.
 
         :return: Factor to scale default figure size by
         """
```

### Comparing `fastdfe-1.1.5/pyproject.toml` & `fastdfe-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastdfe"
-version = "1.1.5"
+version = "1.1.6"
 description = "Fast and flexible inference of the distribution of fitness effects (DFE), VCF-SFS parsing with ancestral allele and site-degeneracy annotation."
 authors = ["Sendrowski <sendrowski.janek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10.0,<3.13"
```

### Comparing `fastdfe-1.1.5/PKG-INFO` & `fastdfe-1.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastdfe
-Version: 1.1.5
+Version: 1.1.6
 Summary: Fast and flexible inference of the distribution of fitness effects (DFE), VCF-SFS parsing with ancestral allele and site-degeneracy annotation.
 License: MIT
 Author: Sendrowski
 Author-email: sendrowski.janek@gmail.com
 Requires-Python: >=3.10.0,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,16 +23,19 @@
 Requires-Dist: requests (>=2.28)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: seaborn (>=0.13.0,<0.14.0)
 Requires-Dist: tqdm (>=4.60.0,<5.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown
 
+# fastDFE  <img align="right" width="100" src="https://raw.githubusercontent.com/Sendrowski/fastDFE/master/docs/logo.png">
 [![tests](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml)
 [![codecov](https://codecov.io/gh/Sendrowski/fastDFE/branch/master/graph/badge.svg?token=0LUE8SZYBJ)](https://codecov.io/gh/Sendrowski/fastDFE)
 [![Documentation Status](https://readthedocs.org/projects/fastdfe/badge/?version=latest)](https://fastdfe.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/fastdfe.svg)](https://badge.fury.io/py/fastdfe)
+[![DOI](https://img.shields.io/badge/DOI-10.1093/molbev/msae070-blue)](https://doi.org/10.1093/molbev/msae070)
 
-fastDFE is a package for fast, flexible, and hierarchical inference of the distribution of fitness effects (DFE) from site frequency spectra (SFS). It also contains a versatile VCF-to-SFS parser with support for ancestral allele and site-degeneracy annotation.
+
+``fastdfe`` is a package for fast, flexible, and hierarchical inference of the distribution of fitness effects (DFE) from site frequency spectra (SFS). It also contains a versatile VCF-to-SFS parser with support for ancestral allele and site-degeneracy annotation.
 
 Please see the [documentation](https://fastdfe.readthedocs.io/en/latest/) for all the details.
```

