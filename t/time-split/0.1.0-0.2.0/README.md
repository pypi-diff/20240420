# Comparing `tmp/time_split-0.1.0.tar.gz` & `tmp/time_split-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_split-0.1.0.tar", max compression
+gzip compressed data, was "time_split-0.2.0.tar", max compression
```

## Comparing `time_split-0.1.0.tar` & `time_split-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     1077 2024-04-14 10:48:07.136003 time_split-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     3234 2024-04-14 10:48:07.136003 time_split-0.1.0/README.md
--rw-r--r--   0        0        0     4755 2024-04-14 10:48:07.140003 time_split-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      352 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/__init__.py
--rw-r--r--   0        0        0      134 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/_backend/__init__.py
--rw-r--r--   0        0        0     2204 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/_backend/_available.py
--rw-r--r--   0        0        0      487 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/_backend/_datetime_index_like.py
--rw-r--r--   0        0        0     4930 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/_backend/_limits.py
--rw-r--r--   0        0        0     2643 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/_backend/_schedule.py
--rw-r--r--   0        0        0     3744 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/_backend/_span.py
--rw-r--r--   0        0        0     5654 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/_backend/_splitter.py
--rw-r--r--   0        0        0     1506 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/_docstrings.py
--rw-r--r--   0        0        0      261 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/_frontend/__init__.py
--rw-r--r--   0        0        0    11885 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/_frontend/_plot.py
--rw-r--r--   0        0        0     5087 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/_frontend/_progress.py
--rw-r--r--   0        0        0     1099 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/_frontend/_split.py
--rw-r--r--   0        0        0     3001 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/_frontend/_to_string.py
--rw-r--r--   0        0        0     2163 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/_frontend/_weight.py
--rw-r--r--   0        0        0      420 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/_support.py
--rw-r--r--   0        0        0       62 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/integration/__init__.py
--rw-r--r--   0        0        0      953 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/integration/_log_progress.py
--rw-r--r--   0        0        0     1808 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/integration/pandas/__init__.py
--rw-r--r--   0        0        0     2800 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/integration/pandas/_impl.py
--rw-r--r--   0        0        0     2424 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/integration/polars/__init__.py
--rw-r--r--   0        0        0     1890 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/integration/polars/_impl.py
--rw-r--r--   0        0        0      131 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/integration/sklearn/__init__.py
--rw-r--r--   0        0        0     5721 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/integration/sklearn/_impl.py
--rw-r--r--   0        0        0     2550 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/integration/split_data.py
--rw-r--r--   0        0        0        0 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/py.typed
--rw-r--r--   0        0        0     6331 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/settings.py
--rw-r--r--   0        0        0      556 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/support/__init__.py
--rw-r--r--   0        0        0     2002 2024-04-14 10:48:07.140003 time_split-0.1.0/src/time_split/types.py
--rw-r--r--   0        0        0     4569 1970-01-01 00:00:00.000000 time_split-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-20 10:53:49.431216 time_split-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     3248 2024-04-20 10:53:49.431216 time_split-0.2.0/README.md
+-rw-r--r--   0        0        0     4772 2024-04-20 10:53:49.435217 time_split-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      342 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/__init__.py
+-rw-r--r--   0        0        0      351 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/_backend/__init__.py
+-rw-r--r--   0        0        0      496 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/_backend/_datetime_index_like.py
+-rw-r--r--   0        0        0     4930 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/_backend/_limits.py
+-rw-r--r--   0        0        0     2220 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/_backend/_process_available.py
+-rw-r--r--   0        0        0     2666 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/_backend/_schedule.py
+-rw-r--r--   0        0        0     3744 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/_backend/_span.py
+-rw-r--r--   0        0        0     5712 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/_backend/_splitter.py
+-rw-r--r--   0        0        0     1560 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/_docstrings.py
+-rw-r--r--   0        0        0      261 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/_frontend/__init__.py
+-rw-r--r--   0        0        0    11750 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/_frontend/_plot.py
+-rw-r--r--   0        0        0     5087 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/_frontend/_progress.py
+-rw-r--r--   0        0        0     1089 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/_frontend/_split.py
+-rw-r--r--   0        0        0     3001 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/_frontend/_to_string.py
+-rw-r--r--   0        0        0     2163 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/_frontend/_weight.py
+-rw-r--r--   0        0        0      420 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/_support.py
+-rw-r--r--   0        0        0       62 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/integration/__init__.py
+-rw-r--r--   0        0        0      953 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/integration/_log_progress.py
+-rw-r--r--   0        0        0     1808 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/integration/pandas/__init__.py
+-rw-r--r--   0        0        0     2800 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/integration/pandas/_impl.py
+-rw-r--r--   0        0        0     2424 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/integration/polars/__init__.py
+-rw-r--r--   0        0        0     1890 2024-04-20 10:53:49.435217 time_split-0.2.0/src/time_split/integration/polars/_impl.py
+-rw-r--r--   0        0        0      131 2024-04-20 10:53:49.439216 time_split-0.2.0/src/time_split/integration/sklearn/__init__.py
+-rw-r--r--   0        0        0     5711 2024-04-20 10:53:49.439216 time_split-0.2.0/src/time_split/integration/sklearn/_impl.py
+-rw-r--r--   0        0        0     3001 2024-04-20 10:53:49.439216 time_split-0.2.0/src/time_split/integration/split_data.py
+-rw-r--r--   0        0        0        0 2024-04-20 10:53:49.439216 time_split-0.2.0/src/time_split/py.typed
+-rw-r--r--   0        0        0     6331 2024-04-20 10:53:49.439216 time_split-0.2.0/src/time_split/settings.py
+-rw-r--r--   0        0        0      652 2024-04-20 10:53:49.439216 time_split-0.2.0/src/time_split/support/__init__.py
+-rw-r--r--   0        0        0      250 2024-04-20 10:53:49.439216 time_split-0.2.0/src/time_split/support/types.py
+-rw-r--r--   0        0        0     2194 2024-04-20 10:53:49.439216 time_split-0.2.0/src/time_split/types.py
+-rw-r--r--   0        0        0     4600 1970-01-01 00:00:00.000000 time_split-0.2.0/PKG-INFO
```

### Comparing `time_split-0.1.0/LICENSE.md` & `time_split-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `time_split-0.1.0/README.md` & `time_split-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Time Split  <!-- omit in toc -->
-Flexible k-fold validation splits for heterogeneous data.
+Time-based k-fold validation splits for heterogeneous data.
 
 -----------------
 [![PyPI - Version](https://img.shields.io/pypi/v/time-split.svg)](https://pypi.python.org/pypi/time-split)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/time-split.svg)](https://pypi.python.org/pypi/time-split)
 [![Tests](https://github.com/rsundqvist/time-split/workflows/tests/badge.svg)](https://github.com/rsundqvist/time-split/actions?workflow=tests)
 [![Codecov](https://codecov.io/gh/rsundqvist/time-split/branch/master/graph/badge.svg)](https://codecov.io/gh/rsundqvist/time-split)
 [![Read the Docs](https://readthedocs.org/projects/time-split/badge/)](https://time-split.readthedocs.io/)
@@ -11,20 +11,20 @@
 
 <div align="center">
   <img alt="Plotted folds on a two-by-two grid." 
        title="Examples" height="300" width="1200" 
   src="https://raw.githubusercontent.com/rsundqvist/time-split/master/docs/2x2-examples.jpg"><br>
 </div>
 
-Plotted folds on a two-by-two grid. See the
+Folds plotted on a two-by-two grid. See the
 [examples](https://time-split.readthedocs.io/en/stable/auto_examples/index.html) page for more.
 
 ## What is it?
-A library for creating cross-validation splits of _heterogeneous_ data, such as raw transaction data with strong
-non-stationary characteristics.
+A library for creating time-based cross-validation splits of _heterogeneous_ data, such as raw transaction data with 
+strong non-stationary characteristics.
 
 ## Highlighted Features
 - [Splitting schedules](https://time-split.readthedocs.io/en/stable/guide/schedules.html) based on a fixed interval, 
   a CRON-expression, or a pre-defined list.
 - [Data selection](https://time-split.readthedocs.io/en/stable/guide/spans.html) based on a timedelta, or the splitting 
   schedule itself.
 - Automatically extract and [normalize](https://time-split.readthedocs.io/en/stable/guide/flex.html) data limits for
```

### Comparing `time_split-0.1.0/pyproject.toml` & `time_split-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "time-split"
-version = "0.1.0"
-description = "My personal little ML engineering library."
+version = "0.2.0"
+description = "Time-based k-fold validation splits for heterogeneous data."
 authors = ["Richard Sundqvist <richard.sundqvist@live.se>"]
 
 readme = "README.md"
 homepage = "https://github.com/rsundqvist/time-split"
 repository = "https://github.com/rsundqvist/time-split"
 documentation = "https://time-split.readthedocs.io"
 classifiers = [
```

### Comparing `time_split-0.1.0/src/time_split/_backend/_available.py` & `time_split-0.2.0/src/time_split/_backend/_process_available.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 from .._support import handle_dask
 from ..types import DatetimeIterable, Flex
 from ._datetime_index_like import DatetimeIndexLike
 from ._limits import LimitsTuple, expand_limits
 
 
-class AvailableMetadata(NamedTuple):
-    """Output of :func:`process_available`."""
+class ProcessAvailableResult(NamedTuple):
+    """Output of :func:`.process_available`."""
 
     available_as_index: DatetimeIndexLike | None
     limits: LimitsTuple
     expanded_limits: LimitsTuple
 
 
-def process_available(available: DatetimeIterable, *, flex: Flex) -> AvailableMetadata:
+def process_available(available: DatetimeIterable, *, flex: Flex) -> ProcessAvailableResult:
     """Process a user-given `available` argument.
 
     Args:
         available: Available data from user. May be ``None``
         flex: Flex-argument. Determines how much (if at all) to expand limits.
 
     Returns:
@@ -46,12 +46,12 @@
 
     if not (isinstance(min_dt, Timestamp) and isinstance(max_dt, Timestamp)):
         # Enforce pandas types; we might have a numpy.datetime64
         # (croniter 1.4.1 + numpy 1.25.2): croniter cannot handle numpy.datetime64
         limits = Timestamp(min_dt), Timestamp(max_dt)
 
     expanded_limits = expand_limits(limits, flex=flex)
-    return AvailableMetadata(available_retval, limits=limits, expanded_limits=expanded_limits)
+    return ProcessAvailableResult(available_retval, limits=limits, expanded_limits=expanded_limits)
 
 
 def _compute_data_limits(available: DatetimeIndexLike) -> LimitsTuple:
     return handle_dask(available.min()), handle_dask(available.max())
```

### Comparing `time_split-0.1.0/src/time_split/_backend/_limits.py` & `time_split-0.2.0/src/time_split/_backend/_limits.py`

 * *Files identical despite different names*

### Comparing `time_split-0.1.0/src/time_split/_backend/_schedule.py` & `time_split-0.2.0/src/time_split/_backend/_schedule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import NamedTuple, cast, get_args
 
 from pandas import DatetimeIndex, NaT, Timedelta, Timestamp, date_range
 
 from ..types import DatetimeIterable, Flex, Schedule, TimedeltaTypes
-from ._available import AvailableMetadata, process_available
 from ._limits import LimitsTuple
+from ._process_available import ProcessAvailableResult, process_available
 
 NO_LIMITS = cast(LimitsTuple, (NaT, NaT))
 
 
 class MaterializedSchedule(NamedTuple):
     """An explicit schedule."""
 
     schedule: DatetimeIndex
-    available_metadata: AvailableMetadata
+    available_metadata: ProcessAvailableResult
 
 
 def materialize_schedule(
     schedule: Schedule, flex: Flex, *, available: DatetimeIterable | None = None
 ) -> MaterializedSchedule:
     """Materialize user schedule based on available data."""
     if available is None:
         try:
             return MaterializedSchedule(
                 DatetimeIndex(schedule),
-                available_metadata=AvailableMetadata(None, NO_LIMITS, NO_LIMITS),
+                available_metadata=ProcessAvailableResult(None, NO_LIMITS, NO_LIMITS),
             )
         except TypeError as e:
             raise ValueError("Schedule must be explicit when not bounded by an available range.") from e
 
     available_metadata = process_available(available, flex=flex)
     min_dt, max_dt = available_metadata.expanded_limits
```

### Comparing `time_split-0.1.0/src/time_split/_backend/_span.py` & `time_split-0.2.0/src/time_split/_backend/_span.py`

 * *Files identical despite different names*

### Comparing `time_split-0.1.0/src/time_split/_backend/_splitter.py` & `time_split-0.2.0/src/time_split/_backend/_splitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 from ._span import OffsetCalculator, to_strict_span
 
 LOGGER = logging.getLogger("time_split")
 
 
 @dataclass(frozen=True)
 class DatetimeIndexSplitter:
-    """Backend interface for splitting user data."""
+    """Backend interface for splitting user data. See the :ref:`Parameter overview` page."""
 
     schedule: Schedule
     before: Span
     after: Span
     step: int
-    n_splits: int | None
+    n_splits: int
     flex: Flex
 
     def get_splits(self, available: DatetimeIterable | None = None) -> DatetimeSplits:
         """Compute a split of given user data."""
         ms = self._materialize_schedule(available)
         self._log_expansion(ms.available_metadata.limits, expanded=ms.available_metadata.expanded_limits)
         return self._make_bounds_list(ms)
@@ -111,18 +111,18 @@
 
         """
         if self.step != 1:
             step = abs(self.step)
             splits = [s for i, s in enumerate(reversed(splits)) if i % step == 0]
             splits.reverse()
 
-        if self.n_splits:
+        if self.n_splits > 0:
             splits = splits[-self.n_splits :]
 
-        if self.step < 0:
+        if self.step < 0:  # Poorly documented - might not work as expected?
             splits.reverse()
 
         return splits
 
     def _log_expansion(self, original: LimitsTuple, *, expanded: LimitsTuple) -> None:
         if original == expanded:
             return
@@ -143,16 +143,16 @@
             f"Available data limits have been expanded (since flex={self.flex!r}):\n"
             f"  start: {stringify(original[0], new=expanded[0])}\n"
             f"    end: {stringify(original[1], new=expanded[1])}"
         )
 
     def __post_init__(self) -> None:
         # Verify n_splits
-        if self.n_splits is not None and self.n_splits < 1:
-            raise ValueError(f"Expected n_splits >= 1, but got n_splits={self.n_splits!r}.")
+        if self.n_splits < 0:
+            raise ValueError(f"Expected n_splits >= 0, but got n_splits={self.n_splits!r}.")
 
         # Verify before/after
         to_strict_span(self.before, name="before")
         to_strict_span(self.after, name="after")
 
         if self.step == 0:
             raise ValueError(f"Bad argument step={self.step}; must be a non-zero integer.")
```

### Comparing `time_split-0.1.0/src/time_split/_docstrings.py` & `time_split-0.2.0/src/time_split/_docstrings.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 _OFFSET = "pandas :ref:`offset alias <pandas:timeseries.offset_aliases>`"
 _SPAN = (
     f"Range {{arg}} `schedule` timestamps. Either a {_OFFSET}, an integer (`schedule`-based offsets), "
     f"or `'all'` (requires `available` data)."
 )
 _DOCSTRINGS = {
-    "schedule": f"A collection of timestamps, a {_OFFSET}, or a cron expression.",
+    "schedule": f"A :attr:`~time_split.types.DatetimeIterable`, {_OFFSET}, or `cron <https://pypi.org/project/croniter/>`_ expression.",
     "before": _SPAN.format(arg="before"),
     "after": _SPAN.format(arg="after"),
     "step": "Select a subset of folds, preferring folds later in the schedule.",
     "n_splits": "Maximum number of folds, preferring folds later in the schedule.",
     "available": "Binds `schedule` to a range.",
     "flex": f'A {_OFFSET} used to expand `available` data to its likely `"true"` limits. Pass ``False`` to disable.',
     "USER_GUIDE": (
```

### Comparing `time_split-0.1.0/src/time_split/_frontend/_plot.py` & `time_split-0.2.0/src/time_split/_frontend/_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import asdict, dataclass
+from dataclasses import asdict, dataclass, replace
 from typing import TYPE_CHECKING, Any, Literal
 
 import pandas as pd
 from pandas import Timestamp
 from rics.misc import format_kwargs, get_public_module
 from rics.performance import format_seconds
 
@@ -58,15 +58,15 @@
 @docs
 def plot(
     schedule: Schedule,
     *,
     before: Span = "7d",
     after: Span = 1,
     step: int = 1,
-    n_splits: int | None = None,
+    n_splits: int = 0,
     available: DatetimeIterable | None = None,
     flex: Flex = "auto",
     # Split plot args
     bar_labels: str | Rows | list[tuple[str, str]] | bool = True,
     show_removed: bool = False,
     row_count_bin: str | pd.Series | None = None,
     ax: "Axes | None" = None,
@@ -279,18 +279,15 @@
     show_removed: bool,
 ) -> PlotData:
     splits, ms = splitter.get_plot_data(available)
     available = ms.available_metadata.available_as_index
 
     if show_removed:
         kept_splits = set(splits)
-        kwargs = asdict(splitter)  # Can't use dataclasses.replace: 3.10+ only
-        kwargs["n_splits"] = None
-        kwargs["step"] = 1
-        splits = DatetimeIndexSplitter(**kwargs).get_plot_data(available)[0]
+        splits = replace(splitter, n_splits=0, step=1).get_plot_data(available)[0]
         if splitter.step < 0:
             splits.reverse()
         removed = set(splits) - set(kept_splits)
     else:
         removed = set()
 
     row_counts = _compute_row_counts(available, row_count_bin=row_count_bin)
```

### Comparing `time_split-0.1.0/src/time_split/_frontend/_progress.py` & `time_split-0.2.0/src/time_split/_frontend/_progress.py`

 * *Files identical despite different names*

### Comparing `time_split-0.1.0/src/time_split/_frontend/_split.py` & `time_split-0.2.0/src/time_split/_frontend/_split.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @docs
 def split(
     schedule: Schedule,
     *,
     before: Span = "7d",
     after: Span = 1,
     step: int = 1,
-    n_splits: int | None = None,
+    n_splits: int = 0,
     available: DatetimeIterable | None = None,
     flex: Flex = "auto",
 ) -> DatetimeSplits:
     """Create time-based cross-validation splits.
 
     To visualize the folds, pass the same arguments to the :func:`.plot`-function.
```

### Comparing `time_split-0.1.0/src/time_split/_frontend/_to_string.py` & `time_split-0.2.0/src/time_split/_frontend/_to_string.py`

 * *Files identical despite different names*

### Comparing `time_split-0.1.0/src/time_split/_frontend/_weight.py` & `time_split-0.2.0/src/time_split/_frontend/_weight.py`

 * *Files identical despite different names*

### Comparing `time_split-0.1.0/src/time_split/integration/_log_progress.py` & `time_split-0.2.0/src/time_split/integration/_log_progress.py`

 * *Files identical despite different names*

### Comparing `time_split-0.1.0/src/time_split/integration/pandas/__init__.py` & `time_split-0.2.0/src/time_split/integration/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `time_split-0.1.0/src/time_split/integration/pandas/_impl.py` & `time_split-0.2.0/src/time_split/integration/pandas/_impl.py`

 * *Files identical despite different names*

### Comparing `time_split-0.1.0/src/time_split/integration/polars/__init__.py` & `time_split-0.2.0/src/time_split/integration/polars/__init__.py`

 * *Files identical despite different names*

### Comparing `time_split-0.1.0/src/time_split/integration/polars/_impl.py` & `time_split-0.2.0/src/time_split/integration/polars/_impl.py`

 * *Files identical despite different names*

### Comparing `time_split-0.1.0/src/time_split/integration/sklearn/_impl.py` & `time_split-0.2.0/src/time_split/integration/sklearn/_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     def __init__(
         self,
         schedule: Schedule,
         *,
         before: Span = "7d",
         after: Span = 1,
-        n_splits: int | None = None,
+        n_splits: int = 0,
         flex: Flex = "auto",
         step: int = 1,
         log_progress: LogProgressArg = False,
         verify_xy: bool = True,
     ) -> None:
         super().__init__()
         self._splitter = DatetimeIndexSplitter(
```

### Comparing `time_split-0.1.0/src/time_split/integration/split_data.py` & `time_split-0.2.0/src/time_split/integration/split_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,46 +2,61 @@
 
 Users may implement splitting of any data type by implementing suitable ``as_available`` and ``select`` functions.
 """
 
 import typing as _t
 from datetime import datetime as _datetime
 
-from .. import _frontend, types
+from .. import _frontend
+from .. import types as _tst
 from .._docstrings import docs as _docs
 from . import _log_progress
 
+if _t.TYPE_CHECKING:
+    import pandas
+
 DataT = _t.TypeVar("DataT")
 """Type of data to split."""
 
-DataAsAvailableFn = _t.Callable[[DataT], types.DatetimeIterable]
+DataAsAvailableFn = _t.Callable[[DataT], _tst.DatetimeIterable]
 """A callable ``(data: DataT) -> DatetimeIterable``."""
 DataSelectFn = _t.Callable[[DataT, _datetime, _datetime], DataT]
 """A callable ``(data: DataT, left_inclusive: datetime, end_exclusive: datetime) -> DataT)``."""
 
 
 class DatetimeSplit(_t.NamedTuple, _t.Generic[DataT]):
     """Time-based split of a generic data type."""
 
     data: DataT
-    """Data before ``bounds.mid``."""
+    """Data before the simulated :attr:`training_date`.
+
+    Bounded by `bounds.start <= time(future_data) < bounds.mid`.
+    """
     future_data: DataT
-    """Data after ``bounds.mid``."""
-    bounds: types.DatetimeSplitBounds
+    """Data after the simulated :attr:`training_date`.
+
+    Bounded by `bounds.mid <= time(future_data) < bounds.end`.
+    """
+    bounds: _tst.DatetimeSplitBounds
     """The underlying bounds that produced this split."""
 
+    @property
+    def training_date(self) -> "pandas.Timestamp":
+        """Returns the simulated training date (alias of :attr:`self.bounds.mid <.DatetimeSplitBounds.mid>`)."""
+        return self.bounds.mid
+
 
 @_docs
 def split_data(
     data: DataT,
     *,
     log_progress: _log_progress.LogProgressArg = False,
     as_available: DataAsAvailableFn[DataT],
     select: DataSelectFn[DataT],
-    **kwargs: _t.Unpack[types.DatetimeIndexSplitterKwargs],
+    **kwargs: _t.Unpack[_tst.DatetimeIndexSplitterKwargs],
 ) -> _t.Iterable[DatetimeSplit[DataT]]:
     """Base implementation for splitting integrated `data` types.
 
     The required ``as_available`` and ``select`` callables provided perform the actual integration.
 
     Args:
         data: The data to split.
```

### Comparing `time_split-0.1.0/src/time_split/settings.py` & `time_split-0.2.0/src/time_split/settings.py`

 * *Files identical despite different names*

### Comparing `time_split-0.1.0/src/time_split/types.py` & `time_split-0.2.0/src/time_split/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 
     start: _pd.Timestamp
     """Left (inclusive) limit of the `data` range."""
     mid: _pd.Timestamp
     """Schedule timestamp.
 
     Right (exclusive) limit of the `data` range, left (inclusive) limit of the `future_data` range.
+
+    When using :mod:`.integration` functions, These are available as :attr:`.DatetimeSplit.data` and
+    :attr:`.DatetimeSplit.future_data`, respectively.
     """
     end: _pd.Timestamp
     """Right (exclusive) limit of the `future_data` range."""
 
 
 DatetimeSplits = list[DatetimeSplitBounds]
 """A list of bounds."""
@@ -45,17 +48,17 @@
     data: int
     future_data: int
 
 
 class DatetimeIndexSplitterKwargs(_t.TypedDict, total=False):
     """Keyword arguments for creating a ``DatetimeIndexSplitter``.
 
-    The ``DatetimeIndexSplitter`` is the backing type for all splitting logic. It is not exposed directly to users. See
-    :func:`.split` or one of the related functions for user-facing APIs.
+    The :class:`time_split.support.DatetimeIndexSplitter` is the backend implementation for the splitting logic. In most
+    cases, it should not be used directly. See func:`.split` or one of the related functions for user-facing APIs.
     """
 
     schedule: _t.Required[Schedule]
     before: Span
     after: Span
     step: int
-    n_splits: int | None
+    n_splits: int
     flex: Flex
```

### Comparing `time_split-0.1.0/PKG-INFO` & `time_split-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: time-split
-Version: 0.1.0
-Summary: My personal little ML engineering library.
+Version: 0.2.0
+Summary: Time-based k-fold validation splits for heterogeneous data.
 Home-page: https://github.com/rsundqvist/time-split
 Author: Richard Sundqvist
 Author-email: richard.sundqvist@live.se
 Requires-Python: >=3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -26,15 +26,15 @@
 Project-URL: Bug Tracker, https://github.com/rsundqvist/time-split/issues
 Project-URL: Changelog, https://github.com/rsundqvist/time-split/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://time-split.readthedocs.io
 Project-URL: Repository, https://github.com/rsundqvist/time-split
 Description-Content-Type: text/markdown
 
 # Time Split  <!-- omit in toc -->
-Flexible k-fold validation splits for heterogeneous data.
+Time-based k-fold validation splits for heterogeneous data.
 
 -----------------
 [![PyPI - Version](https://img.shields.io/pypi/v/time-split.svg)](https://pypi.python.org/pypi/time-split)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/time-split.svg)](https://pypi.python.org/pypi/time-split)
 [![Tests](https://github.com/rsundqvist/time-split/workflows/tests/badge.svg)](https://github.com/rsundqvist/time-split/actions?workflow=tests)
 [![Codecov](https://codecov.io/gh/rsundqvist/time-split/branch/master/graph/badge.svg)](https://codecov.io/gh/rsundqvist/time-split)
 [![Read the Docs](https://readthedocs.org/projects/time-split/badge/)](https://time-split.readthedocs.io/)
@@ -42,20 +42,20 @@
 
 <div align="center">
   <img alt="Plotted folds on a two-by-two grid." 
        title="Examples" height="300" width="1200" 
   src="https://raw.githubusercontent.com/rsundqvist/time-split/master/docs/2x2-examples.jpg"><br>
 </div>
 
-Plotted folds on a two-by-two grid. See the
+Folds plotted on a two-by-two grid. See the
 [examples](https://time-split.readthedocs.io/en/stable/auto_examples/index.html) page for more.
 
 ## What is it?
-A library for creating cross-validation splits of _heterogeneous_ data, such as raw transaction data with strong
-non-stationary characteristics.
+A library for creating time-based cross-validation splits of _heterogeneous_ data, such as raw transaction data with 
+strong non-stationary characteristics.
 
 ## Highlighted Features
 - [Splitting schedules](https://time-split.readthedocs.io/en/stable/guide/schedules.html) based on a fixed interval, 
   a CRON-expression, or a pre-defined list.
 - [Data selection](https://time-split.readthedocs.io/en/stable/guide/spans.html) based on a timedelta, or the splitting 
   schedule itself.
 - Automatically extract and [normalize](https://time-split.readthedocs.io/en/stable/guide/flex.html) data limits for
```

