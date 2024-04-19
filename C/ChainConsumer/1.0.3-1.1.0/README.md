# Comparing `tmp/chainconsumer-1.0.3.tar.gz` & `tmp/chainconsumer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainconsumer-1.0.3.tar", max compression
+gzip compressed data, was "chainconsumer-1.1.0.tar", max compression
```

## Comparing `chainconsumer-1.0.3.tar` & `chainconsumer-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1080 2024-01-22 22:49:57.965280 chainconsumer-1.0.3/LICENSE
--rw-r--r--   0        0        0    13699 2024-01-22 22:49:57.965280 chainconsumer-1.0.3/README.md
--rw-r--r--   0        0        0     2303 2024-01-22 22:50:19.525241 chainconsumer-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      450 2024-01-22 22:49:57.969280 chainconsumer-1.0.3/src/chainconsumer/__init__.py
--rw-r--r--   0        0        0    18896 2024-01-22 22:49:57.969280 chainconsumer-1.0.3/src/chainconsumer/analysis.py
--rw-r--r--   0        0        0      461 2024-01-22 22:49:57.969280 chainconsumer-1.0.3/src/chainconsumer/base.py
--rw-r--r--   0        0        0    17349 2024-01-22 22:49:57.969280 chainconsumer-1.0.3/src/chainconsumer/chain.py
--rw-r--r--   0        0        0     6402 2024-01-22 22:49:57.969280 chainconsumer-1.0.3/src/chainconsumer/chainconsumer.py
--rw-r--r--   0        0        0     5946 2024-01-22 22:49:57.969280 chainconsumer-1.0.3/src/chainconsumer/color_finder.py
--rw-r--r--   0        0        0     8613 2024-01-22 22:49:57.969280 chainconsumer-1.0.3/src/chainconsumer/comparisons.py
--rw-r--r--   0        0        0     6738 2024-01-22 22:49:57.969280 chainconsumer-1.0.3/src/chainconsumer/diagnostic.py
--rw-r--r--   0        0        0      920 2024-01-22 22:49:57.969280 chainconsumer-1.0.3/src/chainconsumer/examples.py
--rw-r--r--   0        0        0     4381 2024-01-22 22:49:57.969280 chainconsumer-1.0.3/src/chainconsumer/helpers.py
--rw-r--r--   0        0        0     3319 2024-01-22 22:49:57.973280 chainconsumer-1.0.3/src/chainconsumer/kde.py
--rw-r--r--   0        0        0       60 2024-01-22 22:49:57.973280 chainconsumer-1.0.3/src/chainconsumer/log.py
--rw-r--r--   0        0        0    42462 2024-01-22 22:49:57.973280 chainconsumer-1.0.3/src/chainconsumer/plotter.py
--rw-r--r--   0        0        0      272 2024-01-22 22:49:57.973280 chainconsumer-1.0.3/src/chainconsumer/plotting/__init__.py
--rw-r--r--   0        0        0     3722 2024-01-22 22:49:57.973280 chainconsumer-1.0.3/src/chainconsumer/plotting/config.py
--rw-r--r--   0        0        0     5494 2024-01-22 22:49:57.973280 chainconsumer-1.0.3/src/chainconsumer/plotting/contours.py
--rw-r--r--   0        0        0      544 2024-01-22 22:49:57.973280 chainconsumer-1.0.3/src/chainconsumer/plotting/truth.py
--rw-r--r--   0        0        0     1916 2024-01-22 22:49:57.973280 chainconsumer-1.0.3/src/chainconsumer/plotting/watermark.py
--rw-r--r--   0        0        0        0 2024-01-22 22:49:57.973280 chainconsumer-1.0.3/src/chainconsumer/py.typed
--rw-r--r--   0        0        0      910 2024-01-22 22:49:57.973280 chainconsumer-1.0.3/src/chainconsumer/statistics.py
--rw-r--r--   0        0        0     1414 2024-01-22 22:49:57.973280 chainconsumer-1.0.3/src/chainconsumer/truth.py
--rw-r--r--   0        0        0    14418 1970-01-01 00:00:00.000000 chainconsumer-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-19 08:30:27.842604 chainconsumer-1.1.0/LICENSE
+-rw-r--r--   0        0        0    14114 2024-04-19 08:30:27.842604 chainconsumer-1.1.0/README.md
+-rw-r--r--   0        0        0     2327 2024-04-19 08:30:47.098739 chainconsumer-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      450 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/__init__.py
+-rw-r--r--   0        0        0    18896 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/analysis.py
+-rw-r--r--   0        0        0      461 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/base.py
+-rw-r--r--   0        0        0    19365 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/chain.py
+-rw-r--r--   0        0        0     6402 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/chainconsumer.py
+-rw-r--r--   0        0        0     5946 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/color_finder.py
+-rw-r--r--   0        0        0     8613 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/comparisons.py
+-rw-r--r--   0        0        0     6738 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/diagnostic.py
+-rw-r--r--   0        0        0      920 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/examples.py
+-rw-r--r--   0        0        0     4386 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/helpers.py
+-rw-r--r--   0        0        0     3319 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/kde.py
+-rw-r--r--   0        0        0       60 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/log.py
+-rw-r--r--   0        0        0    42742 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/plotter.py
+-rw-r--r--   0        0        0      272 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/plotting/__init__.py
+-rw-r--r--   0        0        0     3722 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/plotting/config.py
+-rw-r--r--   0        0        0     5494 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/plotting/contours.py
+-rw-r--r--   0        0        0      544 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/plotting/truth.py
+-rw-r--r--   0        0        0     1916 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/plotting/watermark.py
+-rw-r--r--   0        0        0        0 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/py.typed
+-rw-r--r--   0        0        0      910 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/statistics.py
+-rw-r--r--   0        0        0     1414 2024-04-19 08:30:27.850604 chainconsumer-1.1.0/src/chainconsumer/truth.py
+-rw-r--r--   0        0        0    14833 1970-01-01 00:00:00.000000 chainconsumer-1.1.0/PKG-INFO
```

### Comparing `chainconsumer-1.0.3/LICENSE` & `chainconsumer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chainconsumer-1.0.3/README.md` & `chainconsumer-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,22 @@
 The common error states that `dvipng: not found`, and as per [StackOverflow](http://stackoverflow.com/a/32915992/3339667)
 post, it can be solved by explicitly install the `matplotlib` dependency `dvipng` via `sudo apt-get install dvipng`.
 
 If you are running on HPC or clusters where you can't install things yourself, users may run into issues where LaTeX or other optional dependencies aren't installed. In this case, set `usetex=False` in `configure` to request matplotlib not try to use TeX. If this does not work, also set `serif=False`, which has helped some uses.
 
 ### Update History
 
+##### 1.1.0
+* Updating numpyro and arviz translators so you can specify variable names (`var_names`) to include or exclude.
+* Adding `histogram_relative_height` property to chains to control histogram height.
+* Adding `show_label_in_legend` so you can decide to give a chain a label but not have it pollute the legend.
+
+##### 1.0.3
+* Bug fix not using labels instead of column names for parameter title summaries.
+
 ##### 1.0.2
 * Bug fix for chain divisions.
 
 ##### 1.0.1
 * Bug fix for the truth labels.
 
 ##### 1.0.0
```

### Comparing `chainconsumer-1.0.3/pyproject.toml` & `chainconsumer-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.poetry]
 authors = ["Samuel Hinton <samuelreay@gmail.com>"]
 description = "ChainConsumer: Consumer your MCMC chains"
 name = "ChainConsumer"
 packages = [{include = "chainconsumer", from = "src"}]
 readme = "README.md"
-version = "v1.0.3"
+version = "v1.1.0"
 
 [tool.poetry-version-plugin]
 source = "git-tag"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 numpy = "^1.23.0"
@@ -26,17 +26,17 @@
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
 numpyro = ">=0.13.2, <1"
 emcee = "^3.1.4"
 arviz = ">=0.16.1, <1"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = ">=3.3.3"
-ruff = ">=0.1.4, <1"
-mypy = "^1.4.1"
+pre-commit = ">=3.7.0"
+ruff = ">=0.3.7, <1"
+mypy = "^1.9.0"
 pandas-stubs = "^2.1.1.230928"
 
 
 [tool.poetry.group.docs.dependencies]
 Markdown = "^3.3.7"
 mkdocs = "^1.1.2"
 mkdocs-material = "^9.1.19"
@@ -44,25 +44,28 @@
 mdx-include = ">=1.4.1"
 mkdocstrings-python = ">=0.8.3"
 mkdocs-gallery = ">=0.7.8"
 
 
 [tool.ruff]
 src = ["src"]
-select = ["E", "F", "I", "N", "W", "D207", "D208", "D300", "UP", "YTT", "ASYNC", "DTZ", "G10", "G101", "G201", "G202", "INP001", "PIE", "T20", "SIM", "PTH", "PD", "PLE", "PLR", "PLW", "TRY", "NPY", "RUF"]
-ignore = ["PD010", "PD901", "PLR2004", "UP017", "PLR0915", "TRY003", "INP001", "PLR0912", "PLR0913", "TRY300", "E712"]
 line-length = 120
 target-version = "py310"
 
+[tool.ruff.lint]
+select = ["E", "F", "I", "N", "W", "D207", "D208", "D300", "UP", "YTT", "ASYNC", "DTZ", "G10", "G101", "G201", "G202", "INP001", "PIE", "T20", "SIM", "PTH", "PD", "PLE", "PLR", "PLW", "TRY", "NPY", "RUF"]
+ignore = ["PD010", "PD901", "PLR2004", "UP017", "PLR0915", "TRY003", "INP001", "PLR0912", "PLR0913", "TRY300", "E712"]
+
+
 [tool.ruff.format]
 indent-style = "space"
 quote-style = "double"
 line-ending = "auto"
 
-[tool.ruff.extend-per-file-ignores]
+[tool.ruff.lint.extend-per-file-ignores]
 "test/***" = ["INP001"]
 "__init__.py" = ["E402", "F401"]
 "examples/***" = ["T201", "NPY002"]
 "**/plot_*" = ["T201"]
 "docs/examples/***" = ["T201"]
 
 [tool.mypy]
```

### Comparing `chainconsumer-1.0.3/src/chainconsumer/analysis.py` & `chainconsumer-1.1.0/src/chainconsumer/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     center: float | None = Field(default=None)
     upper: float | None = Field(default=None)
 
     @property
     def array(self) -> np.ndarray:
         return np.array(
             [
-                self.lower if self.lower is not None else np.NaN,
-                self.center if self.center is not None else np.NaN,
-                self.upper if self.upper is not None else np.NaN,
+                self.lower if self.lower is not None else np.nan,
+                self.center if self.center is not None else np.nan,
+                self.upper if self.upper is not None else np.nan,
             ]
         )
 
     @property
     def all_none(self) -> bool:
         return self.lower is None and self.center is None and self.upper is None
```

### Comparing `chainconsumer-1.0.3/src/chainconsumer/chain.py` & `chainconsumer-1.1.0/src/chainconsumer/chain.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 This file is where I expect most people will focus their time. It contains a general configuration class,
 which stores non-unique things that chains use. Like line styles, colours, etc.
 
 It is then extended by the `Chain` class, which contains the actual data.
 
 There are also a few helper functions and objects in here, like the `MaxPosterior` class which
 provides the log posterior and the coordinate at which it can be found for the chain."""
+
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING, Any, TypeAlias
 
 import numpy as np
 import pandas as pd
@@ -132,14 +133,23 @@
         description="The number of effective data points",
         ge=0,
     )
     power: float = Field(
         default=1.0,
         description="Raise the posterior surface to this. Useful for inflating or deflating uncertainty for debugging.",
     )
+    show_label_in_legend: bool = Field(
+        default=True,
+        description="Whether to show the label in the legend",
+    )
+    histogram_relative_height: float = Field(
+        default=1.0,
+        description="The relative height to plot the marginalised histogram. 1.0 will ensure a normalised histogram.",
+        ge=0.0,
+    )
 
     @property
     def data_columns(self) -> list[str]:
         """The columns in the dataframe which are not weights or posteriors."""
         results = []
         for c in self.samples.columns:
             if c in {self.weight_column, self.posterior_column}:
@@ -213,15 +223,15 @@
         return colors.format(v)
 
     @field_validator("samples")
     @classmethod
     def _copy_df(cls, v: pd.DataFrame) -> pd.DataFrame:
         return v.copy()
 
-    @model_validator(mode="after")
+    @model_validator(mode="after")  # type: ignore
     def _validate_model(self) -> Chain:
         assert not self.samples.empty, "Your chain is empty. This is not ideal."
 
         # If weights aren't set, add them all as one
         if self.weight_column not in self.samples:
             assert (
                 self.weight_column == "weight"
@@ -391,48 +401,62 @@
         return cls(samples=df, name=name, **kwargs)
 
     @classmethod
     def from_numpyro(
         cls,
         mcmc: numpyro.infer.MCMC,
         name: str,
+        var_names: list[str] | None = None,
         **kwargs: Any,
     ) -> Chain:
         """Constructor from numpyro samples
 
         Args:
             mcmc: The numpyro sampler
             name: The name of the chain
+            var_names: The names of the parameters to include in the chain. If the entries of var_names start with ~,
+            they are excluded from the variables. If empty, all parameters are included.
             kwargs: Any other arguments to pass to the Chain constructor.
 
         Returns:
             A ChainConsumer Chain made from numpyro samples
         """
-        df = pd.DataFrame.from_dict({key: np.ravel(value) for key, value in mcmc.get_samples().items()})
+
+        var_names = _filter_var_names(var_names, list(mcmc.get_samples().keys()))
+        df = pd.DataFrame.from_dict(
+            {key: np.ravel(value) for key, value in mcmc.get_samples().items() if key in var_names}
+        )
         return cls(samples=df, name=name, **kwargs)
 
     @classmethod
     def from_arviz(
         cls,
         arviz_id: arviz.InferenceData,
         name: str,
+        var_names: list[str] | None = None,
         **kwargs: Any,
     ) -> Chain:
         """Constructor from an arviz InferenceData object
 
         Args:
             arviz_id: The arviz inference data
             name: The name of the chain
+            var_names: The names of the parameters to include in the chain. If the entries of var_names start with ~,
+            they are excluded from the variables. If empty, all parameters are included.
             kwargs: Any other arguments to pass to the Chain constructor.
 
         Returns:
             A ChainConsumer Chain made from the arviz chain
         """
 
-        df = arviz_id.to_dataframe(groups="posterior").drop(columns=["chain", "draw"])
+        import arviz as az
+
+        var_names = _filter_var_names(var_names, list(arviz_id.posterior.keys()))
+        reduced_id = az.extract(arviz_id, var_names=var_names, group="posterior")
+        df = reduced_id.to_dataframe().drop(columns=["chain", "draw"])
 
         return cls(samples=df, name=name, **kwargs)
 
 
 class MaxPosterior(BetterBase):
     """A class that bundles the value of the
     log posterior with the coordinate you can find it at."""
@@ -440,7 +464,35 @@
     log_posterior: float
     coordinate: dict[ColumnName, float]
 
     @property
     def vec_coordinate(self) -> np.ndarray:
         """The coordinate as a numpy array, in the order the columns were given."""
         return np.array(list(self.coordinate.values()))
+
+
+def _filter_var_names(var_names: list[str] | None, all_vars: list[str]) -> list[str]:
+    """
+    Helper function to return the var_names to allows filtering parameters names.
+    """
+
+    if var_names is None:
+        return all_vars
+
+    negations = set([var.startswith("~") for var in var_names])
+
+    if len(negations) != 1:
+        raise ValueError(
+            "all values in var_names must start with ~ to exclude a subset OR none of them to keep a subset"
+        )
+
+    if True in negations:
+        # remove the ~ from the var names
+        var_names = [var[1:] for var in var_names]
+        var_names = [var for var in all_vars if var not in var_names]
+
+        return var_names
+
+    else:
+        # keep var_names as is but check if var is in all_vars
+        var_names = [var for var in all_vars if var in var_names]
+        return var_names
```

### Comparing `chainconsumer-1.0.3/src/chainconsumer/chainconsumer.py` & `chainconsumer-1.1.0/src/chainconsumer/chainconsumer.py`

 * *Files identical despite different names*

### Comparing `chainconsumer-1.0.3/src/chainconsumer/color_finder.py` & `chainconsumer-1.1.0/src/chainconsumer/color_finder.py`

 * *Files identical despite different names*

### Comparing `chainconsumer-1.0.3/src/chainconsumer/comparisons.py` & `chainconsumer-1.1.0/src/chainconsumer/comparisons.py`

 * *Files identical despite different names*

### Comparing `chainconsumer-1.0.3/src/chainconsumer/diagnostic.py` & `chainconsumer-1.1.0/src/chainconsumer/diagnostic.py`

 * *Files identical despite different names*

### Comparing `chainconsumer-1.0.3/src/chainconsumer/examples.py` & `chainconsumer-1.1.0/src/chainconsumer/examples.py`

 * *Files identical despite different names*

### Comparing `chainconsumer-1.0.3/src/chainconsumer/helpers.py` & `chainconsumer-1.1.0/src/chainconsumer/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     return lower, upper
 
 
 def get_bins(chain: Chain) -> int:
     if chain.bins is not None:
         return chain.bins
     max_v = 35 if chain.smooth > 0 else 100
-    return max((max_v, np.floor(1.0 * np.power(chain.samples.shape[0] / chain.samples.shape[1], 0.25))))
+    return max((max_v, int(np.floor(1.0 * np.power(chain.samples.shape[0] / chain.samples.shape[1], 0.25)))))
 
 
 def get_smoothed_bins(
     smooth: int,
     bins: int,
     data: pd.Series,
     weight: np.ndarray,
```

### Comparing `chainconsumer-1.0.3/src/chainconsumer/kde.py` & `chainconsumer-1.1.0/src/chainconsumer/kde.py`

 * *Files identical despite different names*

### Comparing `chainconsumer-1.0.3/src/chainconsumer/plotter.py` & `chainconsumer-1.1.0/src/chainconsumer/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,16 @@
         # Otherwise it must be grow, which is the default
         return 3 + grow_factor * 2 * num_columns + (1 if has_cax else 0), 3 + grow_factor * 2 * num_columns
 
 
 def get_artists_from_chains(chains: list[Chain]) -> list[Artist]:
     artists: list[Artist] = []
     for chain in chains:
+        if not chain.show_label_in_legend:
+            continue
         if chain.plot_contour and not chain.plot_point:
             artists.append(
                 Line2D(
                     (0, 1),
                     (0, 0),
                     color=colors.format(chain.color),
                     ls=chain.linestyle,
@@ -237,18 +239,19 @@
 
         if show_legend:
             ax = axes[legend_location[0], legend_location[1]]
             legend_kwargs = self.config.legend_kwargs_final.copy()
             if "markerfirst" not in legend_kwargs:
                 legend_kwargs["markerfirst"] = legend_outside or not self.config.legend_artists
 
-            artists = get_artists_from_chains(base.chains)
+            chains_to_show_on_legend = [c for c in base.chains if c.show_label_in_legend]
+            artists = get_artists_from_chains(chains_to_show_on_legend)
             leg = ax.legend(handles=artists, **legend_kwargs)
             if self.config.legend_color_text:
-                for text, chain in zip(leg.get_texts(), base.chains):
+                for text, chain in zip(leg.get_texts(), chains_to_show_on_legend):
                     text.set_fontweight("medium")
                     text.set_color(colors.format(chain.color))
         fig.canvas.draw()
         for ax in axes[-1, :]:
             offset = ax.get_xaxis().get_offset_text()
             ax.set_xlabel("{} {}".format(ax.get_xlabel(), f"[{offset.get_text()}]" if offset.get_text() else ""))
             offset.set_visible(False)
@@ -909,28 +912,30 @@
     def _plot_bars(
         self, ax: Axes, column: str, chain: Chain, flip: bool = False, summary: bool = False
     ) -> float:  # pragma: no cover
         # Get values from config
         data = chain.get_data(column)
         if chain.smooth or chain.kde:
             xs, ys, _ = self.parent.analysis._get_smoothed_histogram(chain, column, pad=True)
+            ys *= chain.histogram_relative_height
             if flip:
                 ax.plot(ys, xs, color=chain.color, ls=chain.linestyle, lw=chain.linewidth, zorder=chain.zorder)
             else:
                 ax.plot(xs, ys, color=chain.color, ls=chain.linestyle, lw=chain.linewidth, zorder=chain.zorder)
         else:
             if chain.grid:
                 bins = get_grid_bins(data)
             else:
                 bins, _ = get_smoothed_bins(chain.smooth, get_bins(chain), data, chain.weights)
             hist, edges = np.histogram(data, bins=bins, density=True, weights=chain.weights)
             if chain.power is not None:
                 hist = hist**chain.power
             edge_center = 0.5 * (edges[:-1] + edges[1:])
             xs, ys = edge_center, hist
+            ys *= chain.histogram_relative_height
             ax.hist(
                 xs,
                 weights=ys,
                 bins=bins,  # type: ignore
                 histtype="step",
                 color=chain.color,  # type: ignore
                 orientation="horizontal" if flip else "vertical",
```

### Comparing `chainconsumer-1.0.3/src/chainconsumer/plotting/config.py` & `chainconsumer-1.1.0/src/chainconsumer/plotting/config.py`

 * *Files identical despite different names*

### Comparing `chainconsumer-1.0.3/src/chainconsumer/plotting/contours.py` & `chainconsumer-1.1.0/src/chainconsumer/plotting/contours.py`

 * *Files identical despite different names*

### Comparing `chainconsumer-1.0.3/src/chainconsumer/plotting/truth.py` & `chainconsumer-1.1.0/src/chainconsumer/plotting/truth.py`

 * *Files identical despite different names*

### Comparing `chainconsumer-1.0.3/src/chainconsumer/plotting/watermark.py` & `chainconsumer-1.1.0/src/chainconsumer/plotting/watermark.py`

 * *Files identical despite different names*

### Comparing `chainconsumer-1.0.3/src/chainconsumer/statistics.py` & `chainconsumer-1.1.0/src/chainconsumer/statistics.py`

 * *Files identical despite different names*

### Comparing `chainconsumer-1.0.3/src/chainconsumer/truth.py` & `chainconsumer-1.1.0/src/chainconsumer/truth.py`

 * *Files identical despite different names*

### Comparing `chainconsumer-1.0.3/PKG-INFO` & `chainconsumer-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChainConsumer
-Version: 1.0.3
+Version: 1.1.0
 Summary: ChainConsumer: Consumer your MCMC chains
 Author: Samuel Hinton
 Author-email: samuelreay@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -83,14 +83,22 @@
 The common error states that `dvipng: not found`, and as per [StackOverflow](http://stackoverflow.com/a/32915992/3339667)
 post, it can be solved by explicitly install the `matplotlib` dependency `dvipng` via `sudo apt-get install dvipng`.
 
 If you are running on HPC or clusters where you can't install things yourself, users may run into issues where LaTeX or other optional dependencies aren't installed. In this case, set `usetex=False` in `configure` to request matplotlib not try to use TeX. If this does not work, also set `serif=False`, which has helped some uses.
 
 ### Update History
 
+##### 1.1.0
+* Updating numpyro and arviz translators so you can specify variable names (`var_names`) to include or exclude.
+* Adding `histogram_relative_height` property to chains to control histogram height.
+* Adding `show_label_in_legend` so you can decide to give a chain a label but not have it pollute the legend.
+
+##### 1.0.3
+* Bug fix not using labels instead of column names for parameter title summaries.
+
 ##### 1.0.2
 * Bug fix for chain divisions.
 
 ##### 1.0.1
 * Bug fix for the truth labels.
 
 ##### 1.0.0
```

