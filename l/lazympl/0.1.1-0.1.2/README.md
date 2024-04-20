# Comparing `tmp/lazympl-0.1.1.tar.gz` & `tmp/lazympl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazympl-0.1.1.tar", last modified: Thu Apr 18 10:49:12 2024, max compression
+gzip compressed data, was "lazympl-0.1.2.tar", last modified: Sat Apr 20 18:27:12 2024, max compression
```

## Comparing `lazympl-0.1.1.tar` & `lazympl-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:49:12.784703 lazympl-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:49:12.780703 lazympl-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:49:12.780703 lazympl-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-18 10:49:07.000000 lazympl-0.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-18 10:49:07.000000 lazympl-0.1.1/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 10:49:07.000000 lazympl-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 10:49:07.000000 lazympl-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-18 10:49:12.784703 lazympl-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 10:49:07.000000 lazympl-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-18 10:49:07.000000 lazympl-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 10:49:12.784703 lazympl-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:49:12.780703 lazympl-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:49:12.784703 lazympl-0.1.1/src/lazympl/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 10:49:07.000000 lazympl-0.1.1/src/lazympl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 10:49:12.000000 lazympl-0.1.1/src/lazympl/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-18 10:49:07.000000 lazympl-0.1.1/src/lazympl/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-18 10:49:07.000000 lazympl-0.1.1/src/lazympl/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:49:07.000000 lazympl-0.1.1/src/lazympl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:49:12.784703 lazympl-0.1.1/src/lazympl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-18 10:49:12.000000 lazympl-0.1.1/src/lazympl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-18 10:49:12.000000 lazympl-0.1.1/src/lazympl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:49:12.000000 lazympl-0.1.1/src/lazympl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 10:49:12.000000 lazympl-0.1.1/src/lazympl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 10:49:12.000000 lazympl-0.1.1/src/lazympl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-18 10:49:07.000000 lazympl-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:12.222035 lazympl-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:12.218035 lazympl-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:12.222035 lazympl-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-20 18:27:06.000000 lazympl-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-20 18:27:06.000000 lazympl-0.1.2/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-20 18:27:06.000000 lazympl-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-20 18:27:06.000000 lazympl-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-20 18:27:12.222035 lazympl-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-20 18:27:06.000000 lazympl-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-20 18:27:06.000000 lazympl-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:27:12.222035 lazympl-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:12.218035 lazympl-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:12.222035 lazympl-0.1.2/src/lazympl/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-20 18:27:06.000000 lazympl-0.1.2/src/lazympl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-20 18:27:12.000000 lazympl-0.1.2/src/lazympl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-20 18:27:06.000000 lazympl-0.1.2/src/lazympl/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-20 18:27:06.000000 lazympl-0.1.2/src/lazympl/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:06.000000 lazympl-0.1.2/src/lazympl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:12.222035 lazympl-0.1.2/src/lazympl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-20 18:27:12.000000 lazympl-0.1.2/src/lazympl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-20 18:27:12.000000 lazympl-0.1.2/src/lazympl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:27:12.000000 lazympl-0.1.2/src/lazympl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-20 18:27:12.000000 lazympl-0.1.2/src/lazympl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 18:27:12.000000 lazympl-0.1.2/src/lazympl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-20 18:27:06.000000 lazympl-0.1.2/tox.ini
```

### Comparing `lazympl-0.1.1/.github/workflows/release.yml` & `lazympl-0.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `lazympl-0.1.1/.github/workflows/tox.yml` & `lazympl-0.1.2/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `lazympl-0.1.1/LICENSE` & `lazympl-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lazympl-0.1.1/PKG-INFO` & `lazympl-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazympl
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lazy wrappers around matplotlib
 Author: Thomas Guillet
 Author-email: Adrien Morison <adrien.morison@gmail.com>
 Maintainer-email: Adrien Morison <adrien.morison@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Adrien Morison, Thomas Guillet
```

### Comparing `lazympl-0.1.1/pyproject.toml` & `lazympl-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lazympl-0.1.1/src/lazympl/figure.py` & `lazympl-0.1.2/src/lazympl/figure.py`

 * *Files identical despite different names*

### Comparing `lazympl-0.1.1/src/lazympl/plot.py` & `lazympl-0.1.2/src/lazympl/plot.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,48 @@
 from __future__ import annotations
 
+import warnings
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing import Callable, Sequence
+    from typing import Callable, Optional, Sequence
 
     import matplotlib.axes as mpla
 
     from .figure import Figure
 
 
 class Plot(ABC):
     @abstractmethod
     def draw_on(self, ax: mpla.Axes) -> None:
         """Draw plot onto provided axes."""
 
+    def __add__(self, plot: Plot) -> Plot:
+        return AddPlot(left=self, right=plot)
+
+
+@dataclass(frozen=True)
+class AddPlot(Plot):
+    left: Plot
+    right: Plot
+
+    def draw_on(self, ax: mpla.Axes) -> None:
+        self.left.draw_on(ax)
+        self.right.draw_on(ax)
+
+
+@dataclass(frozen=True)
+class NullPlot(Plot):
+    """A Plot that doesn't draw anything on the given Axes."""
+
+    def draw_on(self, ax: mpla.Axes) -> None:
+        pass
+
 
 @dataclass(frozen=True)
 class FigureTeePlot(Plot):
     plot: Plot
     make_figure: Callable[[Plot], Figure]
     file_name: str
     dpi: int = 200
@@ -61,27 +83,53 @@
     def draw_on(self, ax: mpla.Axes) -> None:
         if self.condition:
             self.plot_if.draw_on(ax)
         else:
             self.plot_else.draw_on(ax)
 
 
+@dataclass(frozen=True)
+class Decorations(Plot):
+    xlabel: Optional[str] = None
+    ylabel: Optional[str] = None
+    title: Optional[str] = None
+
+    def draw_on(self, ax: mpla.Axes) -> None:
+        if self.xlabel is not None:
+            ax.set_xlabel(self.xlabel)
+        if self.ylabel is not None:
+            ax.set_ylabel(self.ylabel)
+        if self.title is not None:
+            ax.set_title(self.title)
+
+
 @dataclass(frozen=True, eq=False)
 class WithAxisLabels(Plot):
     plot: Plot
     xlabel: str
     ylabel: str
 
+    def __post_init__(self) -> None:
+        warnings.warn(
+            "WithAxisLabels is deprecated, use Decorations instead",
+            FutureWarning,
+            stacklevel=2,
+        )
+
     def draw_on(self, ax: mpla.Axes) -> None:
-        self.plot.draw_on(ax)
-        ax.set_xlabel(self.xlabel)
-        ax.set_ylabel(self.ylabel)
+        (self.plot + Decorations(xlabel=self.xlabel, ylabel=self.ylabel)).draw_on(ax)
 
 
 @dataclass(frozen=True, eq=False)
 class WithPlotTitle(Plot):
     plot: Plot
     title: str
 
+    def __post_init__(self) -> None:
+        warnings.warn(
+            "WithPlotTitle is deprecated, use Decorations instead",
+            FutureWarning,
+            stacklevel=2,
+        )
+
     def draw_on(self, ax: mpla.Axes) -> None:
-        self.plot.draw_on(ax)
-        ax.set_title(self.title)
+        (self.plot + Decorations(title=self.title)).draw_on(ax)
```

### Comparing `lazympl-0.1.1/src/lazympl.egg-info/PKG-INFO` & `lazympl-0.1.2/src/lazympl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazympl
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lazy wrappers around matplotlib
 Author: Thomas Guillet
 Author-email: Adrien Morison <adrien.morison@gmail.com>
 Maintainer-email: Adrien Morison <adrien.morison@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Adrien Morison, Thomas Guillet
```

