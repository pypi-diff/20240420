# Comparing `tmp/mpl-markers-0.0.6.tar.gz` & `tmp/mpl_markers-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl-markers-0.0.6.tar", last modified: Wed Apr  3 02:58:30 2024, max compression
+gzip compressed data, was "mpl_markers-0.0.7.tar", last modified: Sat Apr 20 16:13:13 2024, max compression
```

## Comparing `mpl-markers-0.0.6.tar` & `mpl_markers-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 02:58:30.913511 mpl-markers-0.0.6/
--rw-rw-rw-   0        0        0     1058 2023-07-19 22:42:52.000000 mpl-markers-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0       34 2023-07-19 22:42:52.000000 mpl-markers-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4079 2024-04-03 02:58:30.908862 mpl-markers-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3251 2024-04-03 00:29:44.000000 mpl-markers-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 02:58:30.873389 mpl-markers-0.0.6/mpl_markers/
--rw-rw-rw-   0        0        0       23 2024-01-29 04:35:13.000000 mpl-markers-0.0.6/mpl_markers/__init__.py
--rw-rw-rw-   0        0        0    35833 2024-04-03 02:50:33.000000 mpl-markers-0.0.6/mpl_markers/artists.py
--rw-rw-rw-   0        0        0     3904 2024-01-29 04:35:13.000000 mpl-markers-0.0.6/mpl_markers/interactive.py
--rw-rw-rw-   0        0        0    24949 2024-04-03 02:48:42.000000 mpl-markers-0.0.6/mpl_markers/markers.py
-drwxrwxrwx   0        0        0        0 2024-04-03 02:58:30.901860 mpl-markers-0.0.6/mpl_markers/style/
--rw-rw-rw-   0        0        0      936 2023-07-19 22:42:52.000000 mpl-markers-0.0.6/mpl_markers/style/default.json
--rw-rw-rw-   0        0        0     3735 2024-03-31 04:01:33.000000 mpl-markers-0.0.6/mpl_markers/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 02:58:30.905862 mpl-markers-0.0.6/mpl_markers.egg-info/
--rw-rw-rw-   0        0        0     4079 2024-04-03 02:58:30.000000 mpl-markers-0.0.6/mpl_markers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      402 2024-04-03 02:58:30.000000 mpl-markers-0.0.6/mpl_markers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 02:58:30.000000 mpl-markers-0.0.6/mpl_markers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-03 02:58:30.000000 mpl-markers-0.0.6/mpl_markers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-03 02:58:30.000000 mpl-markers-0.0.6/mpl_markers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      837 2024-04-03 02:57:28.000000 mpl-markers-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 02:58:30.913511 mpl-markers-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0       55 2024-01-29 04:35:13.000000 mpl-markers-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 02:58:30.903861 mpl-markers-0.0.6/tests/
--rw-rw-rw-   0        0        0     8240 2024-04-03 02:49:01.000000 mpl-markers-0.0.6/tests/test_markers.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:13:13.116762 mpl_markers-0.0.7/
+-rw-rw-rw-   0        0        0     1058 2023-07-19 22:42:52.000000 mpl_markers-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       34 2023-07-19 22:42:52.000000 mpl_markers-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4208 2024-04-20 16:13:13.116762 mpl_markers-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3379 2024-04-20 16:06:21.000000 mpl_markers-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 16:13:13.085512 mpl_markers-0.0.7/mpl_markers/
+-rw-rw-rw-   0        0        0       23 2024-01-29 04:35:13.000000 mpl_markers-0.0.7/mpl_markers/__init__.py
+-rw-rw-rw-   0        0        0    33814 2024-04-20 15:58:16.000000 mpl_markers-0.0.7/mpl_markers/artists.py
+-rw-rw-rw-   0        0        0     3904 2024-04-20 15:29:51.000000 mpl_markers-0.0.7/mpl_markers/interactive.py
+-rw-rw-rw-   0        0        0    28047 2024-04-20 15:58:16.000000 mpl_markers-0.0.7/mpl_markers/markers.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:13:13.101138 mpl_markers-0.0.7/mpl_markers/style/
+-rw-rw-rw-   0        0        0     1175 2024-04-20 15:04:31.000000 mpl_markers-0.0.7/mpl_markers/style/default.json
+-rw-rw-rw-   0        0        0     3735 2024-03-31 04:01:33.000000 mpl_markers-0.0.7/mpl_markers/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:13:13.116762 mpl_markers-0.0.7/mpl_markers.egg-info/
+-rw-rw-rw-   0        0        0     4208 2024-04-20 16:13:13.000000 mpl_markers-0.0.7/mpl_markers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      402 2024-04-20 16:13:13.000000 mpl_markers-0.0.7/mpl_markers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 16:13:13.000000 mpl_markers-0.0.7/mpl_markers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-20 16:13:13.000000 mpl_markers-0.0.7/mpl_markers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-20 16:13:13.000000 mpl_markers-0.0.7/mpl_markers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      837 2024-04-20 16:12:39.000000 mpl_markers-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-20 16:13:13.116762 mpl_markers-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0       55 2024-01-29 04:35:13.000000 mpl_markers-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:13:13.101138 mpl_markers-0.0.7/tests/
+-rw-rw-rw-   0        0        0     8240 2024-04-20 15:37:20.000000 mpl_markers-0.0.7/tests/test_markers.py
```

### Comparing `mpl-markers-0.0.6/LICENSE.txt` & `mpl_markers-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mpl-markers-0.0.6/PKG-INFO` & `mpl_markers-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl-markers
-Version: 0.0.6
+Version: 0.0.7
 Summary: interactive marker support for matplotlib
 Author-email: Rick Lyon <rlyon14@gmail.com>
 Project-URL: repository, https://github.com/ricklyon/mpl_markers
 Keywords: matplotlib,markers,interactive
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -31,30 +31,31 @@
 ## Usage
 
 ```python
 import mpl_markers as mplm
 ```
 
 ### Line Markers
-Add a marker attached to plotted data lines:
+Add a marker attached to matplotlib data lines:
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
 
 plt.style.use('ggplot')
 plt.rc('font', size=7)
 
 fig, ax = plt.subplots(1,1)
 x1 = np.linspace(-2*np.pi, 2*np.pi, 1000)
 
 ax.plot(x1, np.sin(x1)*np.cos(x1)**2)
 
-mplm.data_marker(x=0)
+mplm.line_marker(x=0)
 ```
-The marker can be dragged to any location along the data line, or moved incrementally with the left/right arrow keys.
+In GUI backends (i.e. Qt5Agg), the marker can be dragged to any location along the data line, or moved incrementally with the left/right arrow keys. Interactive markers are not supported for static inline figures 
+generated in Jupyter Notebooks.
 
 ![example1](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example1.gif)
 
 ### Axis Markers
 Add an axis marker that moves freely on the canvas:
 ```python
 ax.xaxis.set_major_formatter(lambda x, pos: '{:.2f}$\pi$'.format(x/np.pi))
@@ -78,15 +79,15 @@
 z = np.sin(2*x)**2 + np.cos(3*y)**2
 
 fig, ax = plt.subplots(1, 1)
 m = ax.pcolormesh(x, y, z, vmin=0, vmax=2)
 plt.colorbar(m)
 
 # add a data marker at a single x/y point on the plot. x/y is in data coordinates.
-mplm.data_marker(x=0.75, y=0.25)
+mplm.mesh_marker(x=0.75, y=0)
 ```
 ![example3](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example3.gif)
 
 ## Styling
 The marker style is controlled by the `mpl_markers/style/default.json` file:
 
 ```json
@@ -135,18 +136,18 @@
 }
 
 ```
 To use custom styles, pass in a dictionary of artist settings when creating the marker that matches the keys in this file.
 For example, this line will change the color of the dotted vertical line to red.
 
 ```python
-mplm.data_marker(x=0, xline=dict(color='red', linestyle="dashed", alpha=0.5))
+mplm.line_marker(x=0, xline=dict(color='red', linestyle="dashed", alpha=0.5))
 ```
 
 To turn on/off any of the artists, pass in `True/False` for the artist key,
 ```python
-mplm.data_marker(x=0, xlabel=True, xline=False)
+mplm.line_marker(x=0, xlabel=True, xline=False)
 ```
 
 ## License
 
 mpl-markers is licensed under the MIT License.
```

### Comparing `mpl-markers-0.0.6/README.md` & `mpl_markers-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,30 +11,31 @@
 ## Usage
 
 ```python
 import mpl_markers as mplm
 ```
 
 ### Line Markers
-Add a marker attached to plotted data lines:
+Add a marker attached to matplotlib data lines:
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
 
 plt.style.use('ggplot')
 plt.rc('font', size=7)
 
 fig, ax = plt.subplots(1,1)
 x1 = np.linspace(-2*np.pi, 2*np.pi, 1000)
 
 ax.plot(x1, np.sin(x1)*np.cos(x1)**2)
 
-mplm.data_marker(x=0)
+mplm.line_marker(x=0)
 ```
-The marker can be dragged to any location along the data line, or moved incrementally with the left/right arrow keys.
+In GUI backends (i.e. Qt5Agg), the marker can be dragged to any location along the data line, or moved incrementally with the left/right arrow keys. Interactive markers are not supported for static inline figures 
+generated in Jupyter Notebooks.
 
 ![example1](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example1.gif)
 
 ### Axis Markers
 Add an axis marker that moves freely on the canvas:
 ```python
 ax.xaxis.set_major_formatter(lambda x, pos: '{:.2f}$\pi$'.format(x/np.pi))
@@ -58,15 +59,15 @@
 z = np.sin(2*x)**2 + np.cos(3*y)**2
 
 fig, ax = plt.subplots(1, 1)
 m = ax.pcolormesh(x, y, z, vmin=0, vmax=2)
 plt.colorbar(m)
 
 # add a data marker at a single x/y point on the plot. x/y is in data coordinates.
-mplm.data_marker(x=0.75, y=0.25)
+mplm.mesh_marker(x=0.75, y=0)
 ```
 ![example3](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example3.gif)
 
 ## Styling
 The marker style is controlled by the `mpl_markers/style/default.json` file:
 
 ```json
@@ -115,18 +116,18 @@
 }
 
 ```
 To use custom styles, pass in a dictionary of artist settings when creating the marker that matches the keys in this file.
 For example, this line will change the color of the dotted vertical line to red.
 
 ```python
-mplm.data_marker(x=0, xline=dict(color='red', linestyle="dashed", alpha=0.5))
+mplm.line_marker(x=0, xline=dict(color='red', linestyle="dashed", alpha=0.5))
 ```
 
 To turn on/off any of the artists, pass in `True/False` for the artist key,
 ```python
-mplm.data_marker(x=0, xlabel=True, xline=False)
+mplm.line_marker(x=0, xlabel=True, xline=False)
 ```
 
 ## License
 
 mpl-markers is licensed under the MIT License.
```

### Comparing `mpl-markers-0.0.6/mpl_markers/artists.py` & `mpl_markers-0.0.7/mpl_markers/artists.py`

 * *Files 6% similar despite different names*

```diff
@@ -515,100 +515,85 @@
     Places a marker label on a pcolormesh.
     """
 
     def __init__(
         self,
         axes: Axes,
         quadmesh: QuadMesh,
-        xydot: dict = None,
-        ylabel: dict = None,
-        yline: dict = None,
-        ylabel_formatter: Callable = None,
+        zlabel: dict = None,
+        zlabel_formatter: Callable = None,
     ):
         """
         Parameters:
         ----------
         axes: Axes
             axes object that marker will be drawn on.
         data_line: Line2D
             line object to attach marker to. Line does not need to belong to axes if twinx or twiny axes are used.
         dot: bool or dictionary
             If true, a default dot will be drawn. If a dictionary, the parameters will be
             passed into the Line2D constructor. False for no marker dot.
         """
 
-        self.ylabel = None
+        self.zlabel = None
         self.xydot = None
-        self.yline = None
-        self.ylabel_formatter = ylabel_formatter
-        self.xlabel_formatter = ylabel_formatter
+        self.zlabel_formatter = zlabel_formatter
         self.quadmesh = quadmesh
+        self.coords = (
+            quadmesh.get_coordinates().data[:-1, :-1]
+            + quadmesh.get_coordinates().data[1:, 1:]
+        ) / 2
 
         self._yidx = None
         self._xidx = None
         self._xd = None
         self._yd = None
-        self._coords = quadmesh._coordinates.data
-        self._xdata = self._coords[0, :-1, 0] + np.diff(self._coords[0, :, 0]) / 2
-        self._ydata = self._coords[:-1, 0, 1] + np.diff(self._coords[:, 0, 1]) / 2
 
-        if ylabel:
+        if zlabel:
             # initalize text box as the label
-            self.ylabel = MarkerLabel(
-                axes=axes, transform=None, verticalalignment="bottom", **ylabel
+            self.zlabel = MarkerLabel(
+                axes=axes, transform=None, verticalalignment="bottom", **zlabel
             )
 
         # initalize marker dot at data point
         self.xydot = MarkerLine(
             axes=axes,
-            **xydot,
             markeredgewidth=1,
             markeredgecolor="k",
             markerfacecolor="w",
+            markersize=10,
+            marker=".",
         )
         self.xydot_outer = MarkerLine(
             axes=axes,
-            # **xydot,
             markeredgewidth=1,
             markeredgecolor="k",
             markerfacecolor="w",
             markersize=20,
             marker=".",
         )
 
-        if yline:
-            self.yline = MarkerLine(axes=axes, **yline)
-
-        artists = [self.yline, self.xydot_outer, self.xydot, self.ylabel]
+        artists = [self.xydot_outer, self.xydot, self.zlabel]
 
         super().__init__(axes, artists)
         # set to arbitrary position to intialize member variables.
         self.set_position_by_index(xidx=0, yidx=0)
 
     @property
     def xd(self):
         return self._xd
 
     @property
     def yd(self):
         return self._yd
 
     def set_position_by_index(self, xidx, yidx):
-
-        self._coords = self.quadmesh._coordinates.data
-
-        # coordinates store the edges of each cell, get the midpoint
-        self._xdata = self._coords[0, :-1, 0] + np.diff(self._coords[0, :, 0]) / 2
-        self._ydata = self._coords[:-1, 0, 1] + np.diff(self._coords[:, 0, 1]) / 2
-
-        self._data = self.quadmesh.get_array().data.T
-
         # coordinates is a NxMx2 array where NxM is the shape of the meshgrid.
         # the last dimension holds the xy data coordinates of each meshgrid cell.
-        xlen, ylen = len(self._xdata), len(self._ydata)
+        xlen, ylen = self.quadmesh.get_array().shape
 
         if xidx >= xlen:
             xidx = xlen - 1
 
         if xidx < 0:
             xidx = 0
 
@@ -616,17 +601,18 @@
             yidx = ylen - 1
 
         if yidx < 0:
             yidx = 0
 
         self._xidx, self._yidx = xidx, yidx
         # index the x and y coordinates
-        self._xd, self._yd = self._xdata[xidx], self._ydata[yidx]
+        self._xd, self._yd = self.coords[xidx, yidx]
+
         # get the data value at the xy coordinates
-        self._zd = self._data[xidx, yidx]
+        self._zd = self.quadmesh.get_array()[xidx, yidx]
 
         # pad values in display coordinates (pixels)
         label_xpad = 15 * self.axes.figure.dpi / 100
 
         # hide marker if data is not finite or NaN
         if not np.isfinite(self._zd):
             self.set_hidden(True)
@@ -634,27 +620,24 @@
         else:
             self.set_hidden(False)
 
         # get label position in display coordinates. Use the line axes instead of the class axes since
         # the line may belong to another twinx/y axes and have different scaling.
         xl, yl = utils.data2display(self.axes, (self._xd, self._yd))
 
-        if self.ylabel:
+        if self.zlabel:
             # set the x position to the data point location plus a small pad (in display coordinates)
             txt = utils.yformatter(
-                self._xd, self._zd, self._xidx, self.axes, self.ylabel_formatter
+                self._xd, self._zd, self._xidx, self.axes, self.zlabel_formatter
             )
 
-            self.ylabel.set_position(
+            self.zlabel.set_position(
                 (xl, yl), txt, anchor="center left", disp=True, offset=(label_xpad, 0)
             )
 
-        if self.yline:
-            self.yline.set_data(self.axes.get_xlim(), [self._yd] * 2)
-
         if self.xydot:
             self.xydot.set_data([self._xd], [self._yd])
             self.xydot_outer.set_data([self._xd], [self._yd])
             # set the color of the dot
             z_norm = self.quadmesh.norm(self._zd)
             plt.setp(self.xydot, markerfacecolor=self.quadmesh.cmap(z_norm))
             self.xydot.set_color(self.quadmesh.cmap(z_norm))
@@ -662,18 +645,19 @@
     def set_position(self, x: float, y: float, disp: bool = False):
         """
         Returns the index of the line data for the point closest to the x,y data values, and the distance in data coordinates
         """
         if disp:
             x, y = utils.display2data(self.axes, (x, y))
 
-        self._data = self.quadmesh.get_array().data.T
+        dist = np.argmin(
+            np.sum(np.abs(self.coords - np.array([x, y])[None, None]), axis=-1)
+        )
 
-        self._xidx = np.nanargmin(np.abs(x - self._xdata))
-        self._yidx = np.nanargmin(np.abs(y - self._ydata))
+        self._xidx, self._yidx = np.unravel_index(dist, self.coords.shape[:2])
 
         # set position to the data point with the smallest error
         self.set_position_by_index(self._xidx, self._yidx)
 
 
 class DataMarker(MarkerArtist):
     """
@@ -700,15 +684,14 @@
 
         """
         self.data_labels = []
         artists = []
         self.xaxis_label = None
         self.lines = lines
         self.ylabel_artists = []
-        self.xlabel_artist = None
         self.axes = axes
         self._alias_xdata = alias_xdata
 
         # check if all lines have monotonic x-axis data
         self._monotonic_xdata = True
         for ln in lines:
             if self._monotonic_xdata:
@@ -752,16 +735,14 @@
         )
         if self.xaxis_label:
             artists += self.xaxis_label._artists[2:]
 
         # get list of all labels in the marker
         if ylabel:
             self.ylabel_artists += [lbl.ylabel for lbl in self.data_labels]
-        if self.xaxis_label:
-            self.xlabel_artist = self.xaxis_label.xlabel
 
         self._has_xlabel = self.xaxis_label and self.xaxis_label.xlabel
 
         self.set_position(0)
 
         super().__init__(axes, artists)
 
@@ -923,101 +904,77 @@
 
     def __init__(
         self,
         axes: Axes,
         quadmesh: QuadMesh,
         xlabel: dict = None,
         ylabel: dict = None,
-        xydot: dict = None,
+        zlabel: dict = None,
         xline: dict = None,
         yline: dict = None,
         xlabel_formatter: Callable = None,
         ylabel_formatter: Callable = None,
-        alias_xdata: np.ndarray = None,
+        zlabel_formatter: Callable = None,
     ):
         """
         Parameters:
         -----------
 
 
         """
         self.data_label = None
         artists = []
-        self.xaxis_label = None
+        self.axis_label = None
         self.quadmesh = quadmesh
-        self.ylabel_artists = []
-        self.xlabel_artist = None
+        self.data_label = None
         self.axes = axes
-        self._alias_xdata = alias_xdata
 
-        # check that ylines have associated labels or dots
-        if yline and not (ylabel or xydot):
-            raise TypeError("y-axis lines require labels or marker dots.")
-
-        # create single x-axes label shared by all the data markers
-        if xline or xlabel:
-            self.xaxis_label = AxisLabel(
-                axes, xlabel, False, xline, False, False, xlabel_formatter, None
+        # create single x/y-axes label
+        if xline or xlabel or yline or ylabel:
+            self.axis_label = AxisLabel(
+                axes,
+                xlabel,
+                ylabel,
+                xline,
+                yline,
+                False,
+                xlabel_formatter,
+                ylabel_formatter,
             )
 
-        # data labels for each line
-        if ylabel or xydot or yline:
-            # turn off ylabel on data markers if yline is present. The axes label will be used as the data label.
-            self.data_label = MeshLabel(
-                axes, quadmesh, xydot, ylabel, yline, ylabel_formatter
-            )
+        # label for the z data
+        self.data_label = MeshLabel(axes, quadmesh, zlabel, zlabel_formatter)
 
         # build list of all artists in the marker
-
         # line and dot artists first
-        if self.xaxis_label:
-            artists += self.xaxis_label._artists[:2]
-        artists += self.data_label._artists[:-1]
-
-        # then label artists on top
-        artists += self.data_label._artists[-1:]
-
-        if self.xaxis_label:
-            artists += self.xaxis_label._artists[2:]
+        if self.axis_label:
+            artists += self.axis_label._artists
 
-        # get list of all labels in the marker
-        if ylabel:
-            self.ylabel_artists += [self.data_label.ylabel]
-        if self.xaxis_label:
-            self.xlabel_artist = self.xaxis_label.xlabel
-
-        self._has_xlabel = self.xaxis_label and self.xaxis_label.xlabel
+        artists += self.data_label._artists
 
         self.set_position(0, 0)
 
         super().__init__(axes, artists)
 
     def set_position(self, x: float, y: float, disp: bool = False):
         """
         Parameters:
         -----------
-        mode: str -- ['x', 'y', 'xy']
-            controls if line markers are placed by the x value ('x'), the y value ('y'), or by both ('xy').
+
         """
 
         # save the arguments to update the marker position when the axes bbox changes later
         self._position_args = (x, y, disp)
 
         # set the positions for each of the data label
-        self._xlbl = None
         self.data_label.set_position(x, y, disp)
-        self._xdata, self._ydata = self.data_label._xdata, self.data_label._ydata
         self._xd, self._yd = self.data_label._xd, self.data_label._yd
 
-        if self.xaxis_label:
-
+        if self.axis_label:
             # find the label with the closest x data point to the target position and place the x-axis marker there'
-            nearest_lbl_idx = np.nanargmin(np.abs(self._xdata - x))
-            self._xlbl = self._xdata[nearest_lbl_idx]
-
-            self.xaxis_label.set_position(self._xlbl)
+            self.axis_label.set_position(self.data_label._xd, self.data_label._yd)
 
     def get_data_points(self):
         return self._xd, self._yd
 
     def update_positions(self):
         self.set_position(*self._position_args)
```

### Comparing `mpl-markers-0.0.6/mpl_markers/interactive.py` & `mpl_markers-0.0.7/mpl_markers/interactive.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     axes._marker_move = False
 
     m = utils.get_event_marker(axes, event)
     active_marker = axes.marker_active
 
     if m is None and (active_marker is None or axes.figure._marker_hold):
-        markers.data_marker(x, y, axes=axes)
+        markers.line_marker(x, y, axes=axes)
         markers.draw_all(axes)
     elif m is not None:
         markers.set_active(axes, m)
         markers.draw_all(axes)
     elif active_marker is not None:
         markers.move_active(x, y, axes=axes, call_handler=True)
         markers.draw_active(axes)
```

### Comparing `mpl-markers-0.0.6/mpl_markers/markers.py` & `mpl_markers-0.0.7/mpl_markers/markers.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,38 +10,39 @@
 import itertools
 import json
 from pathlib import Path
 
 from . import artists, interactive
 
 __all__ = (
-    "data_marker",
+    "line_marker",
+    "mesh_marker",
     "axis_marker",
     "clear",
     "remove",
     "disable_lines",
     "add_handler",
     "draw_active",
     "move_active",
     "draw_all",
     "init_axes",
 )
 
 
-def data_marker(
+def line_marker(
     x: float = None,
     y: float = None,
     xidx: int = None,
     xline: Union[dict, bool] = True,
     yline: Union[dict, bool] = False,
     xydot: Union[dict, bool] = True,
     xlabel: Union[dict, bool] = False,
     ylabel: Union[dict, bool] = True,
-    yformatter: Callable = None,
     xformatter: Callable = None,
+    yformatter: Callable = None,
     axes: Axes = None,
     lines: List[Line2D] = None,
     alias_xdata: np.ndarray = None,
     call_handler: bool = False,
 ):
     """
     Adds new marker at an x-axis data value, or at the index of the x-axis array. Sets the
@@ -70,20 +71,20 @@
         shows a dot at the data point of the marker. If dictionary, parameters are passed into Line2D
     xlabel: bool OR dictionary = False
         shows a text box of the x value of the marker at the bottom of the axes. If dictionary, parameters are passed
         into axes.text()
     ylabel: bool OR dictionary = True
         shows a text box of the y value of the marker at the data point location. If dictionary, parameters are passed
         into axes.text()
-    yformatter: Callable = None
-        function that returns a string to be placed in the data label given a x and y data coordinate
-            def yformatter(x: float, y:float, idx:int) -> str
     xformatter: Callable = None
         function that returns a string to be placed in the x-axis label given a x data coordinate
             def xformatter(x: float, idx:int) -> str
+    yformatter: Callable = None
+        function that returns a string to be placed in the data label given a x and y data coordinate
+            def yformatter(x: float, y:float, idx:int) -> str
 
     Returns:
     --------
     Marker object
     """
 
     # get current axes if user did not provide one
@@ -91,14 +92,17 @@
         axes = plt.gca()
 
     axes = init_axes(axes)
 
     # use lines kwarg if provided, otherwise use all marker lines attached to the axes
     lines = axes._marker_lines if lines is None else lines
 
+    if not len(lines):
+        return None
+
     # pull properties from default styles
     properties = {}
     for k, prop in zip(
         ["xline", "yline", "xlabel", "ylabel", "xydot"],
         [xline, yline, xlabel, ylabel, xydot],
     ):
         if prop is True:
@@ -110,51 +114,140 @@
 
     # get the x and y label formatters from the axes if not provided
     if xformatter is None and axes._marker_xformatter:
         xformatter = axes._marker_xformatter
     if yformatter is None and axes._marker_yformatter:
         yformatter = axes._marker_yformatter
 
-    collection = axes.collections[0] if len(axes.collections) else None
-    # create a marker on a meshgrid plot
-    if isinstance(collection, QuadMesh):
-        # force the x and y line to be attached to the marker, but allow customization
-        properties = dict(**properties)
-        for prop in ["xline", "yline"]:
-            if prop not in properties.keys() or not properties[prop]:
-                properties[prop] = axes._marker_style[prop]
-
-        m = artists.MeshMarker(
-            axes,
-            collection,
-            xlabel_formatter=xformatter,
-            ylabel_formatter=yformatter,
-            **properties,
-        )
+    # create marker on the existing data lines
+    m = artists.DataMarker(
+        axes,
+        lines,
+        xlabel_formatter=xformatter,
+        ylabel_formatter=yformatter,
+        alias_xdata=alias_xdata,
+        **properties,
+    )
+    if xidx is not None:
+        m._set_position_by_index(xidx)
+    else:
         m.set_position(x, y)
 
-    # create marker on the existing data lines
-    elif len(lines):
-        m = artists.DataMarker(
-            axes,
-            lines,
-            xlabel_formatter=xformatter,
-            ylabel_formatter=yformatter,
-            alias_xdata=alias_xdata,
-            **properties,
-        )
-        if xidx is not None:
-            m._set_position_by_index(xidx)
-        else:
-            m.set_position(x, y)
+    # create new marker and append to the axes marker list
+    axes.markers.append(m)
+    axes.marker_active = m
 
-    # if no suitable data found on the axes to attach a marker to, do nothing and return
-    else:
+    # call the axes handler if it exists
+    if axes._marker_handler is not None and call_handler:
+        func, params = axes._marker_handler
+        func(*axes.marker_active.get_data_points(), **params)
+
+    return m
+
+
+def mesh_marker(
+    x: float = None,
+    y: float = None,
+    xline: Union[dict, bool] = True,
+    yline: Union[dict, bool] = True,
+    xlabel: Union[dict, bool] = False,
+    ylabel: Union[dict, bool] = False,
+    zlabel: Union[dict, bool] = True,
+    xformatter: Callable = None,
+    yformatter: Callable = None,
+    zformatter: Callable = None,
+    axes: Axes = None,
+    call_handler: bool = False,
+):
+    """
+    Adds new marker on a pcolormesh plot.
+
+    Parameters
+    ----------
+    x: float
+        x-axis value (in data coordinates) of marker
+    y: float (optional)
+        y-axis value
+    axes: plt.Axes (optional)
+        Axes object to add markers to. Defaults to plt.gca()
+
+    ----------
+
+    xline: bool OR dictionary = True
+        shows a vertical line at the x value of the marker. If dictionary, parameters are passed
+        into Line2D.
+    yline: bool OR dictionary = True
+        shows a horizontal line at the y value of the marker. If dictionary, parameters are passed
+        into Line2D.
+    xlabel: bool OR dictionary = False
+        shows a text box of the x value of the marker at the bottom of the axes. If dictionary, parameters are passed
+        into axes.text()
+    ylabel: bool OR dictionary = False
+        shows a text box of the y value of the maker along the y axes. If dictionary, parameters are passed
+        into axes.text()
+    zlabel: bool OR dictionary = True
+        shows a text box of the z value of the marker at the data point location. If dictionary, parameters are passed
+        into axes.text()
+    xformatter: Callable = None
+        function that returns a string to be placed in the x-axis label given a x data coordinate
+            def xformatter(x: float, idx:int) -> str
+    yformatter: Callable = None
+        function that returns a string to be placed in the data label given a x and y data coordinate
+            def yformatter(x: float, y:float, idx:int) -> str
+    zformatter: Callable = None
+        function that returns a string to be placed in the z-axis label given a xy data coordinate
+            def xformatter(x: float, idx:int) -> str
+
+    Returns:
+    --------
+    Marker object
+    """
+
+    # get current axes if user did not provide one
+    if axes is None:
+        axes = plt.gca()
+
+    axes = init_axes(axes)
+
+    collection = axes.collections[0] if len(axes.collections) else None
+
+    if not isinstance(collection, QuadMesh):
         return None
 
+    # pull properties from default styles
+    properties = {}
+    for k, prop in zip(
+        ["xline", "yline", "xlabel", "ylabel", "zlabel"],
+        [xline, yline, xlabel, ylabel, zlabel],
+    ):
+        if prop is True:
+            properties[k] = axes._marker_style[k]
+        elif isinstance(prop, dict):
+            properties[k] = axes._marker_style[k]
+            for n, v in prop.items():
+                properties[k][n] = v
+
+    # get the x and y label formatters from the axes if not provided
+    if xformatter is None and axes._marker_xformatter:
+        xformatter = axes._marker_xformatter
+    if yformatter is None and axes._marker_yformatter:
+        yformatter = axes._marker_yformatter
+    if zformatter is None and axes._marker_yformatter:
+        zformatter = axes._marker_yformatter
+
+    m = artists.MeshMarker(
+        axes,
+        collection,
+        xlabel_formatter=xformatter,
+        ylabel_formatter=yformatter,
+        zlabel_formatter=yformatter,
+        **properties,
+    )
+    m.set_position(x, y)
+
     # create new marker and append to the axes marker list
     axes.markers.append(m)
     axes.marker_active = m
 
     # call the axes handler if it exists
     if axes._marker_handler is not None and call_handler:
         func, params = axes._marker_handler
```

### Comparing `mpl-markers-0.0.6/mpl_markers/style/default.json` & `mpl_markers-0.0.7/mpl_markers/style/default.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'zlabel'": "OrderedDict([('fontsize', 8), ('bbox', OrderedDict([('boxstyle', 'square'), "*

 * *             "('facecolor', 'white'), ('edgecolor', 'black'), ('alpha', 1), ('linewidth', "*

 * *             '1.5)]))])'}*

```diff
@@ -35,9 +35,19 @@
         },
         "fontsize": 8
     },
     "yline": {
         "color": "k",
         "linestyle": "dashed",
         "linewidth": 0.6
+    },
+    "zlabel": {
+        "bbox": {
+            "alpha": 1,
+            "boxstyle": "square",
+            "edgecolor": "black",
+            "facecolor": "white",
+            "linewidth": 1.5
+        },
+        "fontsize": 8
     }
 }
```

### Comparing `mpl-markers-0.0.6/mpl_markers/utils.py` & `mpl_markers-0.0.7/mpl_markers/utils.py`

 * *Files identical despite different names*

### Comparing `mpl-markers-0.0.6/mpl_markers.egg-info/PKG-INFO` & `mpl_markers-0.0.7/mpl_markers.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl-markers
-Version: 0.0.6
+Version: 0.0.7
 Summary: interactive marker support for matplotlib
 Author-email: Rick Lyon <rlyon14@gmail.com>
 Project-URL: repository, https://github.com/ricklyon/mpl_markers
 Keywords: matplotlib,markers,interactive
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -31,30 +31,31 @@
 ## Usage
 
 ```python
 import mpl_markers as mplm
 ```
 
 ### Line Markers
-Add a marker attached to plotted data lines:
+Add a marker attached to matplotlib data lines:
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
 
 plt.style.use('ggplot')
 plt.rc('font', size=7)
 
 fig, ax = plt.subplots(1,1)
 x1 = np.linspace(-2*np.pi, 2*np.pi, 1000)
 
 ax.plot(x1, np.sin(x1)*np.cos(x1)**2)
 
-mplm.data_marker(x=0)
+mplm.line_marker(x=0)
 ```
-The marker can be dragged to any location along the data line, or moved incrementally with the left/right arrow keys.
+In GUI backends (i.e. Qt5Agg), the marker can be dragged to any location along the data line, or moved incrementally with the left/right arrow keys. Interactive markers are not supported for static inline figures 
+generated in Jupyter Notebooks.
 
 ![example1](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example1.gif)
 
 ### Axis Markers
 Add an axis marker that moves freely on the canvas:
 ```python
 ax.xaxis.set_major_formatter(lambda x, pos: '{:.2f}$\pi$'.format(x/np.pi))
@@ -78,15 +79,15 @@
 z = np.sin(2*x)**2 + np.cos(3*y)**2
 
 fig, ax = plt.subplots(1, 1)
 m = ax.pcolormesh(x, y, z, vmin=0, vmax=2)
 plt.colorbar(m)
 
 # add a data marker at a single x/y point on the plot. x/y is in data coordinates.
-mplm.data_marker(x=0.75, y=0.25)
+mplm.mesh_marker(x=0.75, y=0)
 ```
 ![example3](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example3.gif)
 
 ## Styling
 The marker style is controlled by the `mpl_markers/style/default.json` file:
 
 ```json
@@ -135,18 +136,18 @@
 }
 
 ```
 To use custom styles, pass in a dictionary of artist settings when creating the marker that matches the keys in this file.
 For example, this line will change the color of the dotted vertical line to red.
 
 ```python
-mplm.data_marker(x=0, xline=dict(color='red', linestyle="dashed", alpha=0.5))
+mplm.line_marker(x=0, xline=dict(color='red', linestyle="dashed", alpha=0.5))
 ```
 
 To turn on/off any of the artists, pass in `True/False` for the artist key,
 ```python
-mplm.data_marker(x=0, xlabel=True, xline=False)
+mplm.line_marker(x=0, xlabel=True, xline=False)
 ```
 
 ## License
 
 mpl-markers is licensed under the MIT License.
```

### Comparing `mpl-markers-0.0.6/pyproject.toml` & `mpl_markers-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpl-markers"
-version = "0.0.6"
+version = "0.0.7"
 description = "interactive marker support for matplotlib"
 readme = "README.md"
 authors = [{ name = "Rick Lyon", email = "rlyon14@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mpl-markers-0.0.6/tests/test_markers.py` & `mpl_markers-0.0.7/tests/test_markers.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,16 @@
         d1 = np.sin(x1)
         d1[400:500] = np.nan
 
         ax.plot(x1, d1, label="sin(x)")
         ax.plot(x1, np.cos(x1), label="cos(x)")
         ax.legend(loc="lower left")
 
-        m = mplm.data_marker(x=-1)
-        mplm.data_marker(x=1, xline=False)
+        m = mplm.line_marker(x=-1)
+        mplm.line_marker(x=1, xline=False)
 
         self.assertLess(np.max(m._xd + 1), 1e-3)
 
         self.assertFalse(np.isfinite(m._yd[0]))
         self.assertTrue(m.data_labels[0].ylabel._hidden)
         self.assertFalse(m.data_labels[1].ylabel._hidden)
 
@@ -36,15 +36,15 @@
         x1 = np.linspace(-2 * np.pi, 2 * np.pi, 1000)
         x2 = np.linspace(-3 * np.pi, 3 * np.pi, 400)
 
         ax.plot(x1, np.sin(x1), label="sin(x)")
         ax.plot(x2, np.cos(x2), label="cos(x)")
 
         angle = 2.5 * np.pi
-        m = mplm.data_marker(x=angle)
+        m = mplm.line_marker(x=angle)
         m_x, m_y = m.get_data_points()
 
         plt.show()
 
     # @unittest.skip
     def test_non_monotonic(self):
         fig, (ax1) = plt.subplots(1, 1)
@@ -57,15 +57,15 @@
         d2 = np.exp(1j * x2) / 2
         ax1.plot(np.real(d), np.imag(d))
         ax1.plot(np.real(d2), np.imag(d2))
 
         # set marker to angle. The xdata for the marker is the real component of d, so to set the angle we need to specify the index
         angle = np.pi / 2
         m_idx = np.argmin(np.abs(x1 - angle))
-        m = mplm.data_marker(
+        m = mplm.line_marker(
             x=0
         )  # , ylabel_formatter=lambda x, y, idx, **kwargs: '{:.2f}$\pi$'.format(x1[idx]/np.pi))
 
         m_x, m_y = m.get_data_points()
 
         plt.show()
 
@@ -88,19 +88,19 @@
 
         def yfmt(x, y, idx):
             return "{:.3f}$\pi$".format(y)
 
         def xfmt(x, y, idx):
             return "{:.3f}$\pi$".format(x)
 
-        mplm.data_marker(
+        mplm.line_marker(
             x=angle1, yline=True, alias_xdata=x1_pi, yformatter=yfmt, xformatter=xfmt
         )
 
-        mplm.data_marker(
+        mplm.line_marker(
             x=angle2,
             yline=True,
             alias_xdata=x1_pi,
             yformatter="{:.3f}$\pi$",
             xformatter="{:.3f}$\pi$",
         )
 
@@ -110,15 +110,15 @@
     def test_marker_properties(self):
         fig, ax = plt.subplots(1, 1)
         ax.set_title("test_marker_properties")
         x2 = np.linspace(-3 * np.pi, 3 * np.pi, 400)
 
         ax.plot(x2, np.cos(x2), label="cos(x)")
 
-        m = mplm.data_marker(
+        m = mplm.line_marker(
             x=0,
             xlabel=True,
             ylabel=dict(fontfamily="monospace", rotation=-10, color="teal", fontsize=8),
             xline=dict(linewidth=2, color="teal", alpha=0.2),
         )
 
         plt.show()
@@ -145,44 +145,44 @@
 
         def link_ax2(xd, yd, **kwargs):
             mplm.move_active(x=xd[0], axes=ax1)
 
         mplm.init_axes(ax1, xlabel=dict(fontsize=6, color="black"), handler=link_ax1)
         mplm.init_axes(ax2, xlabel=dict(fontsize=6, color="black"), handler=link_ax2)
 
-        m1 = mplm.data_marker(x=1, axes=ax1, xlabel=True)
-        m2 = mplm.data_marker(x=0, axes=ax2, xlabel=True)
+        m1 = mplm.line_marker(x=1, axes=ax1, xlabel=True)
+        m2 = mplm.line_marker(x=0, axes=ax2, xlabel=True)
 
         # move ax1 marker and make sure they stay synced
         mplm.move_active(x=2, call_handler=True, axes=ax1)
         plt.show()
 
     # @unittest.skip
     def test_polar(self):
         fig, (ax1) = plt.subplots(1, 1, subplot_kw={"projection": "polar"})
         ax1.set_title("test_polar")
         x2 = np.linspace(-np.pi, np.pi, 1000)
 
         ax1.plot(x2, np.cos(x2) ** 2)
         ax1.plot(x2, np.cos(x2))
 
-        m = mplm.data_marker(x=np.pi / 3)
+        m = mplm.line_marker(x=np.pi / 3)
 
         m_x, m_y = m.get_data_points()
         plt.show()
 
     def test_polar2(self):
         fig, axes = plt.subplots(1, 1, subplot_kw=dict(polar=True))
 
         theta = np.linspace(-180, 180, 200)
         theta_rad = np.deg2rad(theta)
 
         axes.plot(theta_rad, np.abs(np.sin(theta_rad)))
 
-        m = mplm.data_marker(x=-np.pi / 2)
+        m = mplm.line_marker(x=-np.pi / 2)
         plt.show()
 
     # @unittest.skip
     def test_axis_markers(sef):
         fig, ax = plt.subplots(1, 1)
         ax.set_title("test_axis_markers")
         x1 = np.linspace(-2 * np.pi, 2 * np.pi, 1000)
@@ -222,30 +222,30 @@
 
         ax.plot(x1, np.cos(x1), label="cdos(x)")
         ax.plot(x1, np.sin(x1), label="sin(x)")
         ax.legend(loc="lower left")
 
         plt.margins(x=0)
 
-        m1 = mplm.data_marker(x=-2 * np.pi)
+        m1 = mplm.line_marker(x=-2 * np.pi)
 
         self.assertEqual(ax.get_xlim(), (np.pi, 2 * np.pi))
 
         plt.show()
 
     def test_svg_pdf(self):
         fig, (ax1, ax2) = plt.subplots(2, 1)
         ax1.set_title("test_svg_pdf")
         x1 = np.linspace(-2 * np.pi, 2 * np.pi, 1000)
 
         ax1.plot(x1, np.cos(x1), label="cos(x)")
         ax2.plot(x1, np.sin(x1), label="cos(x)")
         ax1.legend(loc="lower left")
 
-        m1 = mplm.data_marker(x=-1.5 * np.pi, axes=ax1)
+        m1 = mplm.line_marker(x=-1.5 * np.pi, axes=ax1)
         m2 = mplm.axis_marker(y=0.5, axes=ax1)
 
         dir_ = Path(__file__).parent
         fig.savefig(dir_ / "mpl_test.pdf")
         fig.savefig(dir_ / "mpl_test.svg")
         plt.show()
 
@@ -258,13 +258,13 @@
         # plot the data with pcolormesh
         fig = plt.figure()
         ax = fig.subplots(1, 1)
         m = ax.pcolormesh(x, y, z, vmin=0, vmax=2)
         # fig.colorbar()
 
         # add a data marker at a single x/y point on the plot. x/y is in data coordinates.
-        mplm.data_marker(x=0.75, y=0.25)
+        mplm.mesh_marker(x=0.75, y=0.25)
         plt.show()
 
 
 if __name__ == "__main__":
     unittest.main()
```

