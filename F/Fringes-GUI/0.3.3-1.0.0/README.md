# Comparing `tmp/fringes_gui-0.3.3.tar.gz` & `tmp/fringes_gui-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fringes_gui-0.3.3.tar", max compression
+gzip compressed data, was "fringes_gui-1.0.0.tar", max compression
```

## Comparing `fringes_gui-0.3.3.tar` & `fringes_gui-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      422 2023-05-24 16:56:44.238389 fringes_gui-0.3.3/fringes_gui/__init__.py
--rw-r--r--   0        0        0    16181 2023-09-14 19:50:10.724086 fringes_gui-0.3.3/fringes_gui/gui.py
--rw-r--r--   0        0        0    27333 2023-10-19 16:46:05.251420 fringes_gui-0.3.3/fringes_gui/logic.py
--rw-r--r--   0        0        0      129 2023-07-26 08:44:30.374279 fringes_gui-0.3.3/fringes_gui/main.py
--rw-r--r--   0        0        0     1607 2023-10-19 14:18:15.424000 fringes_gui-0.3.3/fringes_gui/numba-blue-icon-rgb.svg
--rw-r--r--   0        0        0    28645 2023-09-13 16:10:06.087656 fringes_gui-0.3.3/fringes_gui/params.py
--rw-r--r--   0        0        0    32917 2023-10-19 16:37:51.124685 fringes_gui-0.3.3/fringes_gui/setters.py
--rw-r--r--   0        0        0   250284 2023-04-01 09:49:27.000000 fringes_gui-0.3.3/fringes_gui/spirals.png
--rw-r--r--   0        0        0     1004 2023-10-19 16:49:50.159246 fringes_gui-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1277 2023-09-13 09:34:01.210814 fringes_gui-0.3.3/README.md
--rw-r--r--   0        0        0     2140 1970-01-01 00:00:00.000000 fringes_gui-0.3.3/setup.py
--rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 fringes_gui-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      795 2024-04-20 16:22:10.414097 fringes_gui-1.0.0/fringes_gui/__init__.py
+-rw-r--r--   0        0        0    16278 2024-04-20 16:26:29.615288 fringes_gui-1.0.0/fringes_gui/gui.py
+-rw-r--r--   0        0        0    32094 2024-04-20 16:26:29.623157 fringes_gui-1.0.0/fringes_gui/logic.py
+-rw-r--r--   0        0        0      129 2024-03-28 12:32:14.400050 fringes_gui-1.0.0/fringes_gui/main.py
+-rw-r--r--   0        0        0     1607 2024-04-20 16:22:10.434257 fringes_gui-1.0.0/fringes_gui/numba-blue-icon-rgb.svg
+-rw-r--r--   0        0        0    29338 2024-04-20 16:22:10.440709 fringes_gui-1.0.0/fringes_gui/params.py
+-rw-r--r--   0        0        0      312 2024-04-20 16:22:10.447172 fringes_gui-1.0.0/fringes_gui/readme.txt
+-rw-r--r--   0        0        0    33684 2024-04-20 16:22:10.453467 fringes_gui-1.0.0/fringes_gui/setters.py
+-rw-r--r--   0        0        0     2832 2024-04-20 16:22:10.408001 fringes_gui-1.0.0/fringes_gui/Xi.svg
+-rw-r--r--   0        0        0    21278 2024-04-20 16:22:10.396966 fringes_gui-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     1241 2024-04-20 16:26:29.635685 fringes_gui-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2664 2024-04-20 16:26:29.608905 fringes_gui-1.0.0/README.md
+-rw-r--r--   0        0        0     3918 1970-01-01 00:00:00.000000 fringes_gui-1.0.0/PKG-INFO
```

### Comparing `fringes_gui-0.3.3/fringes_gui/gui.py` & `fringes_gui-1.0.0/fringes_gui/gui.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,72 @@
 import os
 import ctypes
-import logging as lg
+import logging
 import hashlib
 
 import numpy as np
-import fringes as frng
+import toml
 import pyqtgraph as pg
 from PyQt6.QtWidgets import QApplication, QMainWindow, QPlainTextEdit
 from pyqtgraph.Qt import QtGui, QtWidgets
 from pyqtgraph.dockarea import *
+import fringes as frng
 
 import fringes_gui
 from fringes_gui.setters import set_functionality
 
-# import pyqtgraph.examples
-# pyqtgraph.examples.run()
+logger = logging.getLogger(__name__)
 
 
 class FringesGUI(QApplication):
     """Simple graphical user interface for the 'fringes' package."""
 
     def __init__(self):
         super(FringesGUI, self).__init__([])
 
-        myappid = "Fringes-GUI"  # arbitrary string
-        if fringes_gui.__version__:
-            myappid += f" {fringes_gui.__version__}"
+        pg.setConfigOptions(imageAxisOrder="row-major")  # useCupy slows the GUI down; useNUmba shows no effect
+        _meta = toml.load(os.path.join(os.path.dirname(__file__), "..", "pyproject.toml"))
+        name = _meta["tool"]["poetry"]["name"]
+        myappid = name + f" {fringes_gui.__version__}"  # arbitrary string
         ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
 
-        pg.setConfigOptions(imageAxisOrder="row-major", useNumba=True)  # useCupy
-
-        self.fringes = frng.Fringes(X=1920, Y=1200)
-        self.fringes.logger.setLevel("INFO")  # should be the same as in logic.py
+        # fringes
+        self.fringes = frng.Fringes()  # (X=1920, Y=1200)
+        # fixme: in params, directions are abbreviated, in defaults not; therefore next line:
+        self.fringes2 = frng.Fringes()  # (X=1920, Y=1200)
         self.fringes.load(os.path.join(os.path.expanduser("~"), ".fringes.yaml"))
         self.key = ""
-        try:
-            self.visibility = "Expert" if hashlib.sha256(os.getlogin().encode("utf-8")).hexdigest() == '095d9cc941ca4d5a84fe0a707391c05549faa500406b3a43a26f20fa7a1bcb25' else "Beginner"
-        except:
+        if (
+            hashlib.sha256(os.getlogin().encode("utf-8")).hexdigest()
+            == "095d9cc941ca4d5a84fe0a707391c05549faa500406b3a43a26f20fa7a1bcb25"
+        ):
+            self.visibility = "Expert"
+        else:
             self.visibility = "Beginner"
-        self.digits = 8  # todo: len(str(self.fringes._Pmax))  # 4 (digits) + 1 (point) + 3 (decimals) = 8 == current length of Pmax?
+        self.digits = 8  # todo: len(str(self.fringes._Pmax)) =?= 4 (digits) + 1 (point) + 3 (decimals) = 8
         self.sub = str.maketrans("1234567890", "₁₂₃₄₅₆₇₈₉₀")
         self.sup = str.maketrans("₁₂₃₄₅₆₇₈₉₀", "1234567890")
 
         # define window
         self.win = QMainWindow()
         self.area = DockArea()
         self.win.setCentralWidget(self.area)
-
-        self.win.setGeometry(QtGui.QGuiApplication.primaryScreen().availableGeometry())  # move to primary screen
-        # if Screen.count == 1 and self.desktop.availableGeometry(idx).width() / self.desktop.availableGeometry(idx).height() >= 21 / 9:
-        #     self.win.resize(self.desktop.availableGeometry().width() // 2, self.desktop.availableGeometry().height())
-        #     # self.win.move(0, 0)  # move to the left
-        #     self.win.move(self.desktop.availableGeometry().width() // 2, 0)  # move to the right
-        # else:
-        #     self.win.showMaximized()  # self.win.showFullScreen()
-
-        self.win.showMaximized()  # self.win.showFullScreen()
-
-        self.win.setWindowIcon(QtGui.QIcon(os.path.join(os.path.dirname(__file__), "spirals.png")))
-
+        self.win.setWindowIcon(QtGui.QIcon(os.path.join(os.path.dirname(__file__), "Xi.svg")))
         self.win.setWindowTitle(myappid)
+        geo = QtGui.QGuiApplication.primaryScreen().availableGeometry()
+        W = geo.width()
+        H = geo.height()
+        S = len(QtGui.QGuiApplication.screens())
+        if S == 1 and W / H > 2:
+            self.win.resize(W // 2, H)
+            # self.win.move(0, 0)  # move to the left
+            self.win.move(W // 2, 0)  # move to the right
+        else:
+            self.win.setGeometry(geo)  # move to primary screen
+            self.win.showMaximized()
 
         # set style
         # self.setStyleSheet(open("QTDark.stylesheet").read())
 
         # import qdarkstyle
         # self.setStyleSheet(qdarkstyle.load_stylesheet(qt_api='pyqt6'))
 
@@ -72,17 +75,14 @@
 
         # import qtmodern.styles
         # import qtmodern.windows
         # qtmodern.styles.dark(self)
         # self.win = qtmodern.windows.ModernWindow(self.win)  # todo: moving window with win+arrow keys doesn't work
         # pg.setConfigOptions(background=42/255)
 
-        # Create docks, place them into the window one at a time.
-        from pyqtgraph.dockarea.Dock import DockLabel
-
         def updateStylePatched(
             self,
         ):  # from https://gist.github.com/matmr/72487a03da95b99db6ae
             r = "3px"
             if self.dim:
                 fg = "#fff"  # gray
                 bg = "##6CC0A8"  # green brighter
@@ -127,14 +127,16 @@
                     fg,
                     r,
                     r,
                     border,
                 )
                 self.setStyleSheet(self.hStyle)
 
+        # Create docks, place them into the window one at a time.
+        from pyqtgraph.dockarea.Dock import DockLabel
         DockLabel.updateStyle = updateStylePatched
 
         self.dock_attributes = Dock("Attributes", size=(15, 99))
         self.dock_methods = Dock("Methods", size=(15, 1))
         self.dock_viewer = Dock("Viewer", size=(70, 100))
         self.dock_data = Dock("Data", size=(15, 50))
         self.dock_log = Dock("Log", size=(15, 50))
@@ -144,16 +146,16 @@
         self.area.addDock(self.dock_methods, "bottom", self.dock_attributes)
         self.area.addDock(self.dock_data, "right", self.dock_viewer)
         self.area.addDock(self.dock_log, "bottom", self.dock_data)
 
         # Add widgets into each dock.
 
         # General settings
-        self.immerse = False
-        self.immerse_key = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+Shift+i"), self.win)
+        self.full_screen = False
+        self.full_screen_key = QtGui.QShortcut(QtGui.QKeySequence("F11"), self.win)
 
         self.tree = pg.parametertree.ParameterTree()
         self.dock_attributes.addWidget(self.tree)
 
         # Control
         self.undo_key = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+Z"), self.win)
         self.redo_key = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+Y"), self.win)
@@ -162,29 +164,33 @@
         self.reset_button.setToolTip("Press 'Ctrl+R'.")
         self.reset_key = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+R"), self.win)
         self.encode_checkbox = QtWidgets.QCheckBox()
         self.encode_label = QtWidgets.QLabel("      Encode on parameter change")
         self.decode_checkbox = QtWidgets.QCheckBox()
         self.decode_label = QtWidgets.QLabel("      Decode on parameter change")
         self.default_key = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+Shift+D"), self.win)
-        self.coordinates_key = QtGui.QShortcut(QtGui.QKeySequence("G"), self.win)
+        self.coordinates_key = QtGui.QShortcut(QtGui.QKeySequence("X"), self.win)
         self.encode_button = QtWidgets.QPushButton("Encode")
         self.encode_button.setToolTip("Press 'E'.")
-        self.encode_button.setStyleSheet("" if self.encodeOK else "QPushButton{color: red}")
+        self.encode_button.setStyleSheet("" if not self.fringes._ambiguous else "QPushButton{color: red}")
         self.encode_key = QtGui.QShortcut(QtGui.QKeySequence("E"), self.win)
         self.decode_button = QtWidgets.QPushButton("Decode")
         self.decode_button.setEnabled(False)
         self.decode_button.setToolTip("Press 'D'.")
         self.decode_key = QtGui.QShortcut(QtGui.QKeySequence("D"), self.win)
         self.decode_key.setEnabled(False)
-        self.remap_button = QtWidgets.QPushButton("Remap")
-        self.remap_button.setEnabled(False)
-        self.remap_button.setToolTip("Press 'R'.")
-        self.remap_key = QtGui.QShortcut(QtGui.QKeySequence("R"), self.win)
-        self.remap_key.setEnabled(False)
+        self.register_key = QtGui.QShortcut(QtGui.QKeySequence("R"), self.win)
+        self.source_button = QtWidgets.QPushButton("Source")
+        self.source_button.setEnabled(False)
+        self.source_button.setToolTip("Press 'S'.")
+        self.source_key = QtGui.QShortcut(QtGui.QKeySequence("S"), self.win)
+        self.source_key.setEnabled(False)
+        self.bright_key = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+B"), self.win)
+        self.bright_inverse_key = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+Shift+B"), self.win)
+        self.dark_key = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+D"), self.win)
         self.curvature_button = QtWidgets.QPushButton("Curvature")
         self.curvature_button.setEnabled(False)
         self.curvature_button.setToolTip("Press 'C'.")
         self.curvature_key = QtGui.QShortcut(QtGui.QKeySequence("C"), self.win)
         self.curvature_key.setEnabled(False)
         self.height_button = QtWidgets.QPushButton("Height")
         self.height_button.setEnabled(False)
@@ -194,70 +200,63 @@
         self.dock_methods.addWidget(self.reset_button, 0, 0, 1, 2)
         # self.dock_methods.addWidget(self.encode_label, 1, 0, 1, 2)
         # self.dock_methods.addWidget(self.encode_checkbox, 1, 0, 1, 2)
         # self.dock_methods.addWidget(self.decode_label, 2, 0, 1, 2)
         # self.dock_methods.addWidget(self.decode_checkbox, 2, 0, 1, 2)
         self.dock_methods.addWidget(self.encode_button, 3, 0)
         self.dock_methods.addWidget(self.decode_button, 3, 1)
-        self.dock_methods.addWidget(self.remap_button, 4, 0, 1, 2)
+        self.dock_methods.addWidget(self.source_button, 4, 0, 1, 2)
         self.dock_methods.addWidget(self.curvature_button, 5, 0)
         self.dock_methods.addWidget(self.height_button, 5, 1)
 
         # Viewer
-        self.zoomback_key = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+0"), self.win)  # todo
+        self.zoomback_key = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+0"), self.win)
 
         self.plot = pg.PlotItem()
         self.plot.setLabel(axis="left", text="y-axis")
         self.plot.setLabel(axis="bottom", text="x-axis")  # todo: set label 'T-axis'
+        # todo: plot.setTitle according to datum
         self.imv = pg.ImageView(view=self.plot)
         # self.imv.ui.histogram.hide()
         # self.imv.ui.roiBtn.hide()
         # self.imv.ui.menuBtn.hide()
         self.dock_viewer.addWidget(self.imv)
 
-        self.info = QtWidgets.QLabel()
-        self.dock_viewer.addWidget(self.info)
-
         # Data
         # self.data_tree = pg.DataTreeWidget()
 
         class TableView(QtWidgets.QTableWidget):
             def __init__(self, *args):
                 QtWidgets.QTableWidget.__init__(self, *args)
                 self.resizeRowsToContents()
                 self.resizeColumnsToContents()
-                # self.setSelectionBehavior(QtWidgets.QTableView.selectRow)
+                # self.setSelectionBehavior(QtWidgets.QTableView.selectRow)  # todo
                 # self.setSelectionMode(QtWidgets.QTableView.SingleSelection)
                 self.setColumnCount(3)
                 self.setRowCount(0)
                 self.setHorizontalHeaderLabels(["Name", "Video-Shape", "Type"])
 
             def setData(self, data={}):
                 self.setRowCount(len(data))
                 for i, row in enumerate(sorted(data)):
                     for j, v in enumerate(row):
                         newitem = QtWidgets.QTableWidgetItem(v)
                         self.setItem(i, j, newitem)
 
-                # self.resizeRowsToContents()
                 self.resizeColumnsToContents()
 
-        # self.display_selector = QtWidgets.QComboBox()
-        # self.display_selector.setPlaceholderText("Nothing")
-        # self.con = Container(self.display_selector)
         class Container:
             @property
             def info(self):
                 info = [
                     [str(k), str(v.shape), str(v.dtype)] for k, v in self.__dict__.items() if isinstance(v, np.ndarray)
                 ]
                 return info
 
         self.con = Container()
-        # self.dock_data.addWidget(self.display_selector, 0, 0)
 
         self.data_table = TableView()
         self.dock_data.addWidget(self.data_table, 1, 0, 1, 2)
         self.load_button = QtWidgets.QPushButton("Load")
         self.load_button.setToolTip("Press 'Ctrl+L'.")
         self.load_key = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+L"), self.win)
         self.save_button = QtWidgets.QPushButton("Save")
@@ -273,33 +272,40 @@
         self.clear_key = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+Shift+C"), self.win)
         self.clear_key.setEnabled(self.dataOK)
         self.dock_data.addWidget(self.load_button, 2, 0)
         self.dock_data.addWidget(self.save_button, 2, 1)
         self.dock_data.addWidget(self.clear_button, 3, 0)
         self.dock_data.addWidget(self.set_button, 3, 1)
 
-        # self.model = QtWidgets.QFileSystemModel()
-        # self.model.setRootPath(self.data.dest)
-        # self.view = QtWidgets.QTreeView()
-        # self.view.setModel(self.model)
-        # self.view.setCurrentIndex(self.model.index(self.data.dest))
-        # self.view.setExpanded(self.model.index(self.data.dest), True)
-        # self.dock_data.addWidget(self.view, row=3, col=0)
-
-        # Log
-        class QPlainTextEditLogger(lg.Handler):
+        # logging
+        class QPlainTextEditLogger(logging.Handler):
             def emit(self, record):
                 self.widget.appendPlainText(self.format(record))
 
         self.log_widget = QPlainTextEdit()
         self.dock_log.addWidget(self.log_widget)
+
+        formatter = logging.Formatter("%(asctime)s %(levelname)-8s %(name)s.%(funcName)s(): %(message)s")
+
+        self.glogger = fringes_gui.logger  # parent logger
+        self.glogger.setLevel("INFO")
+
+        self.flogger = logging.getLogger("fringes")
+        self.flogger.setLevel("INFO")
+
+        stream_handler = logging.StreamHandler()
+        stream_handler.setFormatter(formatter)
+        self.glogger.addHandler(stream_handler)
+        self.flogger.addHandler(stream_handler)
+
         handler = QPlainTextEditLogger()
-        handler.setFormatter(self.fringes.logger.handlers[0].formatter)
+        handler.setFormatter(formatter)
         handler.widget = self.log_widget
-        self.fringes.logger.addHandler(handler)
+        self.glogger.addHandler(handler)
+        self.flogger.addHandler(handler)
 
         set_functionality(self)
 
     def show(self):
         """Display the Application."""
         pg.exec()
         # if (sys.flags.interactive != 1) or not hasattr(QtCore, "PYQT_VERSION"):
@@ -325,20 +331,20 @@
         b = not self.fringes.SDM
         c = not self.fringes.WDM
         return a and b and c
 
     @property
     def resetOK(self):
         """True if params equal defalts."""
-        return self.fringes.params != frng.Fringes().params or self.visibility != "Expert"
+        return self.fringes.params != self.fringes2.params or self.visibility != "Expert"
 
-    @property
-    def encodeOK(self):
-        """True if unambiguous measurement range >= length."""
-        return not self.fringes._ambiguous
+    # @property
+    # def encodeOK(self):
+    #     """True if unambiguous measurement range >= length."""
+    #     return not self.fringes._ambiguous
 
     @property
     def dataOK(self):
         """Return True if at least one attribute of Container class is an ndarray object."""
         return any(isinstance(obj, np.ndarray) for obj in self.con.__dict__.values())
 
     @property
@@ -350,22 +356,20 @@
     @property
     def decodeOK(self):
         """Return true if data present can be decoded."""
         I = (
             getattr(self.con, self.key)
             if hasattr(self.con, self.key)
             # else self.con.raw if hasattr(self.con, "raw")
-            else self.con.fringes
-            if hasattr(self.con, "fringes")
-            else None
+            else self.con.fringes if hasattr(self.con, "fringes") else None
         )
         return I is not None and hasattr(I, "ndim") and frng.vshape(I).shape[0] == self.fringes.T
 
     @property
-    def remapOK(self):
+    def sourceOK(self):
         """Returns True if modulation and registration is available."""
         return hasattr(self.con, "registration")
 
     @property
     def curvatureOK(self):
         return (
             hasattr(self.con, "registration")
```

### Comparing `fringes_gui-0.3.3/fringes_gui/logic.py` & `fringes_gui-1.0.0/fringes_gui/logic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-import numpy as np
+import logging
+import functools
 import os
+
+# os.environ["OPENCV_IO_ENABLE_OPENEXR"] = "1"  # todo: exr, in put this line in __init__?
 import glob
+import ast
 
-# os.environ["OPENCV_IO_ENABLE_OPENEXR"]="1"
-import functools
+import numpy as np
 
 from pyqtgraph.Qt import QtWidgets, QtGui
 from PyQt6.QtWidgets import QFileDialog, QMessageBox
 import pyqtgraph as pg
 import cv2
-import json
 import h5py
 import asdf
 import fringes as frng
 
+logger = logging.getLogger(__name__)
 
 config = frng.Fringes._loader
 
 image = {  # https://docs.opencv.org/4.x/d4/da8/group__imgcodecs.html#ga288b8b3da0892bd651fce07b3bbd3a56
     ".bmp": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),
     # ".dip": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),  # i.e. ".bmp"
     # ".jpeg": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),
@@ -32,15 +35,15 @@
     # ".pxm": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),
     # ".pnm": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),
     # ".pfm": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),
     # ".sr": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),
     # ".ras": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),
     ".tiff": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),
     ".tif": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),
-    # ".exr": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),
+    # ".exr": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),  # todo exr
     # ".hdr": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),
     # ".pic": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),
 }
 
 binary = {
     ".mmap": np.load,
     ".npy": np.load,
@@ -53,18 +56,18 @@
 
 loader = {**config, **image, **binary}
 
 
 def set_logic(gui):
     """Assigns functionality to the buttons and keys in the GUI."""
 
-    def immerse():
-        gui.immerse = not gui.immerse
+    def full_screen():
+        gui.full_screen = not gui.full_screen  # toggle
 
-        if gui.immerse:
+        if gui.full_screen:
             gui.win.showFullScreen()
         else:
             gui.win.showMaximized()
 
     def undo():
         if len(gui.param_buffer) and gui.param_index >= 0:
             gui.param_index -= 1
@@ -73,19 +76,24 @@
     def redo():
         if len(gui.param_buffer) > gui.param_index + 1:
             gui.param_index += 1
             gui.tree.setParameters(gui.param_buffer[gui.param_index], showTop=False)
 
     def reset():
         with gui.params.treeChangeBlocker():
-            gui.params.param("vis").setValue("Expert")  # should be the same as in gui.py
             gui.fringes.reset()
             gui.fringes.save(os.path.join(os.path.expanduser("~"), ".fringes.yaml"))
+            if (
+                    hashlib.sha256(os.getlogin().encode("utf-8")).hexdigest()
+                    == "095d9cc941ca4d5a84fe0a707391c05549faa500406b3a43a26f20fa7a1bcb25"
+            ):
+                gui.params.param("vis").setValue("Expert")  # should be the same as in gui.py
+            else:
+                gui.params.param("vis").setValue("Beginner")  # should be the same as in gui.py
             gui.update_parameter_tree()
-            # gui.params.param("log").setValue("INFO")  # should be the same as in gui.py
 
         clear()
         gui.reset_button.setEnabled(gui.resetOK)
 
     def load():
         """Load data from given directory."""
 
@@ -117,54 +125,69 @@
                         for k, v in data.items():
                             if hasattr(v, "shape") and hasattr(v, "shape"):
                                 setattr(gui.con, k, np.array(v))
                                 if not key:
                                     key = k
 
                         if key:
-                            gui.fringes.logger.info(f"Loaded data from '{flist[0]}'.")  # only first asdf-file is loaded
+                            # gui.glogger.info(f"Loaded data from '{flist[0]}'.")  # only first asdf-file is loaded
+                            logger.info(f"Loaded data from '{flist[0]}'.")  # only first asdf-file is loaded
                             view(getattr(gui.con, key))
                     elif ext == ".asdf":
                         if "fringes-params" in data:
                             params = data["fringes-params"]
                             gui.fringes.params = params
+                            gui.update_parameter_tree()
 
                         key = ""
                         for k, v in data.items():
                             if isinstance(v, np.ndarray):
                                 setattr(gui.con, k, v)
                                 if not key:
                                     key = k
 
                         if key:
-                            gui.fringes.logger.info(f"Loaded data from '{flist[0]}'.")  # only first asdf-file is loaded
+                            # gui.glogger.info(f"Loaded data from '{flist[0]}'.")  # only first asdf-file is loaded
+                            logger.info(f"Loaded data from '{flist[0]}'.")  # only first asdf-file is loaded
                             view(getattr(gui.con, key))
                     elif ext == ".npz":
-                        for key in data.files:
-                            try:
-                                datum = frng.vshape(data[key])
-                                setattr(gui.con, key, datum)
-                            except ValueError:
-                                pass  # Object arrays cannot be loaded when allow_pickle=False
+                        if "fringes-params" in data:
+                            params = ast.literal_eval(np.array2string(data["fringes-params"])[1:-1])
+                            gui.fringes.params = params
+                            gui.update_parameter_tree()
+
+                        key = ""
+                        for k, v in data.items():
+                            if isinstance(v, np.ndarray) and k != "fringes-params":  # and v.dtype.kind != "U":
+                                try:
+                                    setattr(gui.con, k, v)
+                                    if not key:
+                                        key = k
+                                except ValueError:
+                                    # gui.glogger.error("Object arrays cannot be loaded when allow_pickle=False")
+                                    logger.error("Object arrays cannot be loaded when allow_pickle=False")
 
-                        gui.fringes.logger.info(f"Loaded data from '{flist[0]}'.")  # only first npz-file is loaded
-                        view(getattr(gui.con, data.files[0]))
+                        if key:
+                            # gui.glogger.info(f"Loaded data from '{flist[0]}'.")  # only first npz-file is loaded
+                            logger.info(f"Loaded data from '{flist[0]}'.")  # only first npz-file is loaded
+                            view(getattr(gui.con, key))
                     else:
                         root = name.rstrip("1234567890").rstrip("_")
 
                         if len(flist) > 1:
                             # data is only one datum in list of data
                             if all(os.path.splitext(f) == ".npy" for f in flist):
                                 for f in flist:
                                     path, base = os.path.split(flist[0])
                                     name, ext = os.path.splitext(base)
                                     datum = np.load(f)
                                     setattr(gui.con, name, datum)
-                                gui.fringes.logger.info(f"Loaded data from '{os.path.join(path, root + '*') + ext}'.")
-                            elif all(os.path.splitext(f) in image for f in flist):
+                                # gui.glogger.info(f"Loaded data from '{os.path.join(path, root + '*') + ext}'.")
+                                logger.info(f"Loaded data from '{os.path.join(path, root + '*') + ext}'.")
+                            elif all(os.path.splitext(f)[1] in image for f in flist):
                                 # here, data is only one image (one datum) in image stack (data)
                                 datum = data
                                 data = np.empty((len(flist),) + datum.shape, datum.dtype)
                                 data[0] = datum
 
                                 for i, f in enumerate(flist[1:]):
                                     path, base = os.path.split(f)
@@ -173,123 +196,146 @@
 
                                     if ext_ == ext and root_ == root:
                                         datum = loader[ext_](f)
 
                                         if datum.shape == data.shape[1:] and datum.dtype == data.dtype:
                                             data[i + 1] = datum
                                         else:
-                                            gui.fringes.logger.error(
-                                                "Files in list dint't match shape and dtype. " "Terminated loading data.")
+                                            # gui.glogger.error(
+                                            #     "Files in list dint't match shape and dtype. "
+                                            #     "Terminated loading data."
+                                            # )
+                                            logger.error(
+                                                "Files in list dint't match shape and dtype. "
+                                                "Terminated loading data."
+                                            )
                                             return
 
-                                gui.fringes.logger.info(f"Loaded data from '{os.path.join(path, root + '*') + ext}'.")
+                                # gui.glogger.info(f"Loaded data from '{os.path.join(path, root + '*') + ext}'.")
+                                logger.info(f"Loaded data from '{os.path.join(path, root + '*') + ext}'.")
                         else:
-                            gui.fringes.logger.info(f"Loaded data from '{flist[0]}'.")
+                            # gui.glogger.info(f"Loaded data from '{flist[0]}'.")
+                            logger.info(f"Loaded data from '{flist[0]}'.")
 
                         data = frng.vshape(data)
                         setattr(gui.con, root, data)
                         view(getattr(gui.con, root))
 
                     gui.data_table.setData(gui.con.info)
                     QtWidgets.QApplication.processEvents()  # refresh event queue
 
             gui.decode_button.setEnabled(gui.decodeOK)
             gui.decode_key.setEnabled(gui.decodeOK)
-            gui.remap_button.setEnabled(gui.remapOK)
-            gui.remap_key.setEnabled(gui.remapOK)
+            gui.source_button.setEnabled(gui.sourceOK)
+            gui.source_key.setEnabled(gui.sourceOK)
             gui.curvature_button.setEnabled(gui.curvatureOK)
             gui.curvature_key.setEnabled(gui.curvatureOK)
             gui.height_button.setEnabled(gui.heightOK)
             gui.height_key.setEnabled(gui.heightOK)
             gui.clear_button.setEnabled(gui.dataOK)
             gui.clear_key.setEnabled(gui.dataOK)
             gui.set_button.setEnabled(gui.set_dataOK)
 
     def save():
         """Save all data to current directory."""
 
+        # todo: used flag (mixed) to decide wheather to save as binary or multiple files i.e. memory efficient i.e. compressed
+
         # path = QFileDialog.getExistingDirectory(
         #     caption="Select directory",
         #     # directory=os.path.join(os.path.expanduser("~"), "Videos"),
         #     # options=QFileDialog.Option.DontUseNativeDialog,
         # )
 
         fname = QFileDialog.getSaveFileName(
             caption="Save dataset",
             filter=f"Misc {tuple('*' + key for key in ['.tif', '.npy'])};;"
-                   f"Binary {tuple('*' + key for key in ['.npz', '.asdf'])};;"
-                   f"Config {tuple('*' + key for key in config.keys())};;".replace(",", "").replace("'", "")
+            f"Binary {tuple('*' + key for key in ['.npz', '.asdf'])};;"
+            f"Config {tuple('*' + key for key in config.keys())};;".replace(",", "").replace("'", ""),
         )[0]
 
         path, base = os.path.split(fname)
         name, ext = os.path.splitext(base)
+        if not ext:
+            name, ext = ext, name
 
         if os.path.isdir(path):
             with pg.BusyCursor():
-                if ext in config and (not gui.con or ext != ".asdf"):  # config can only be asdf if there is no data in gui.con
+                if ext in config:
                     gui.fringes.save(fname)
-                    gui.fringes.logger.info(f"Saved config to '{fname}'.")
                 elif ext == ".asdf":
-                    tree = {}
-                    tree["fringes-params"] = gui.fringes.params  # params first!
+                    tree = {"fringes-params": gui.fringes.params}
                     for k, v in vars(gui.con).items():
                         tree[k] = v
 
                     # Create the ASDF file object from our data tree
                     af = asdf.AsdfFile(tree)
 
                     # Write the data to a new file
                     af.write_to(fname)
 
-                    gui.fringes.logger.info(f"Saved data to '{fname}'.")
+                    # gui.glogger.info(f"Saved data to '{fname}'.")
+                    logger.info(f"Saved data to '{fname}'.")
                 elif ext == ".npz":
-                    # todo: save params to json str to array of type str
-                    # s = json.dumps(gui.fringes.params)
-                    # a = np.array(s)
-                    # a2s = np.array2string(a)
-                    # s2 = json.loads(a2s)
-
-                    gui.fringes.save(os.path.join(path, "params.yaml"))
-
-                    tree = vars(gui.con)
+                    params = {"fringes-params": np.array(str(gui.fringes.params))}
+                    data = vars(gui.con)
+                    tree = params | data
                     np.savez(fname, **tree)
-                else:  # choose file format disk space effiently
+                else:  # choose file format so that disk space is used effiently
                     gui.fringes.save(os.path.join(path, "params.yaml"))
 
                     for k, v in gui.con.__dict__.items():
                         if isinstance(v, np.ndarray) and v.size > 0:
-                            T, Y, X, C = v.shape = frng.vshape(v).shape
-                            color_order = (
-                                (2, 1, 0, 3) if C == 4 else (2, 1, 0) if C == 3 else 0
-                            )  # compensate OpenCV color order
+                            T, Y, X, C = frng.vshape(v).shape
+
                             color_channels = (1, 3, 4)
-                            is_img_shape = v.ndim <= 2 or v.ndim == 3 and v.shape[-1] in color_channels
-                            is_vid_shape = v.ndim == 3 or v.ndim == 4 and v.shape[-1] in color_channels
+
+                            # is_txt_shape = X == Y == 1  # todo: txt file
+
+                            # limits of imread() in OpenCV
+                            # https://docs.opencv.org/4.x/d4/da8/group__imgcodecs.html#gab32ee19e22660912565f8140d0f675a8
+                            is_img_shape = (
+                                T == 1 and X <= 2**20 and Y <= 2**20 and X * Y <= 2**30 and C in color_channels
+                            )
+
+                            # max luma picture size of h264, h265, h266 video codecs as of 2022
+                            is_vid_shape = T > 1 and X * Y <= 35651584 and C in color_channels
+
                             is_img_dtype = (
-                                v.dtype in (bool, np.uint8, np.uint16)
+                                v.dtype
+                                in (bool, np.uint8, np.uint16)
                                 # or v.dtype in (np.float32,)  # here, OpenCV uses LogLuv high dynamic range encoding (4 bytes per pixel)
                                 # and np.min(v) >= 0
                                 # and np.max(v) <= 1
                             )  # todo: np.float16, np.float64
-                            is_exr_shape = False  # todo: exr_shape
-                            is_exr_dtype = v.dtype in (np.float16, np.float32, np.uint32)
+
+                            # is_exr_dtype = v.dtype in (np.float16, np.float32, np.uint32)  # todo: exr
+
+                            v.shape = T, Y, X, C
+
+                            # is_img_shape = v.ndim <= 2 or v.ndim == 3 and C in color_channels
+                            # is_vid_shape = v.ndim == 3 or v.ndim == 4 and C in color_channels
+
+                            # compensate OpenCV color order
+                            color_order = (2, 1, 0, 3) if C == 4 else (2, 1, 0) if C == 3 else 0
 
                             if is_img_dtype and is_img_shape:  # save as image
                                 fname = os.path.join(path, f"{k}.tif")
-                                cv2.imwrite(fname, v[..., color_order])
+                                cv2.imwrite(fname, v[0, ..., color_order])
                             elif is_img_dtype and is_vid_shape:  # save as image sequence
                                 for t in range(T):
                                     fname = os.path.join(path, f"{k}_{str(t + 1).zfill(len(str(T)))}.tif")
                                     cv2.imwrite(fname, v[t][..., color_order])
                             # elif is_exr_dtype:
                             #     pass  # todo
                             else:  # save as numpy array
                                 np.save(os.path.join(path, f"{k}.npy"), v)
                     else:  # executes only after the loop completes normally
-                        gui.fringes.logger.info(f"Saved data to '{path}'.")
+                        # gui.glogger.info(f"Saved data to '{path}'.")
+                        logger.info(f"Saved data to '{path}'.")
 
     def clear():
         """Clear all data from the gui_util."""
 
         view(None)
 
         gui.key = ""
@@ -301,16 +347,16 @@
 
         gui.data_table.clearContents()
         gui.data_table.setRowCount(0)
         gui.set_button.setEnabled(False)
 
         gui.decode_button.setEnabled(False)
         gui.decode_key.setEnabled(False)
-        gui.remap_button.setEnabled(False)
-        gui.remap_key.setEnabled(False)
+        gui.source_button.setEnabled(False)
+        gui.source_key.setEnabled(False)
         gui.curvature_button.setEnabled(False)
         gui.curvature_key.setEnabled(False)
         gui.height_button.setEnabled(False)
         gui.height_key.setEnabled(False)
         gui.clear_button.setEnabled(False)
         gui.clear_key.setEnabled(False)
 
@@ -319,64 +365,94 @@
 
         try:
             item = gui.data_table.currentItem().text()  # todo: select first element of selected row
 
             if hasattr(gui.con, item):
                 view(getattr(gui.con, item))
                 gui.key = item
-                gui.fringes.logger.info(f"Set data to be decoded to '{gui.key}'.")
+                # gui.glogger.info(f"Set data to be decoded to '{gui.key}'.")
+                logger.info(f"Set data to be decoded to '{gui.key}'.")
             else:
                 view(None)
                 gui.key = None
 
             gui.decode_button.setEnabled(gui.decodeOK)
             gui.decode_key.setEnabled(gui.decodeOK)
         except Exception:
             pass
 
     def coordinates():
         """Coordinates being encoded."""
         if hasattr(gui.con, "coordinates"):
             delattr(gui.con, "coordinates")
 
+        view(None)
         gui.data_table.setData(gui.con.info)
         QtWidgets.QApplication.processEvents()  # refresh event queue
 
         with pg.BusyCursor():
             gui.con.coordinates = gui.fringes.coordinates()
 
-        view(getattr(gui.con, "coordinates").astype(float))
+        view(gui.con.coordinates.astype(float))
         gui.data_table.setData(gui.con.info)
         QtWidgets.QApplication.processEvents()  # refresh event queue
 
-    def encode():
+    def encode(*args, display: bool = True):
         """Encode fringes based on the given parameters."""
         if hasattr(gui.con, "fringes"):
             delattr(gui.con, "fringes")
 
+        view(None)
         gui.data_table.setData(gui.con.info)
         QtWidgets.QApplication.processEvents()  # refresh event queue
 
         with pg.BusyCursor():
             gui.con.fringes = gui.fringes.encode()
 
-        view(getattr(gui.con, "fringes"))
-        gui.data_table.setData(gui.con.info)
-        QtWidgets.QApplication.processEvents()  # refresh event queue
+        if display:
+            view(gui.con.fringes)
+            gui.data_table.setData(gui.con.info)
+            QtWidgets.QApplication.processEvents()  # refresh event queue
 
         gui.decode_button.setEnabled(gui.decodeOK)
         gui.decode_key.setEnabled(gui.decodeOK)
         gui.clear_button.setEnabled(gui.dataOK)
         gui.clear_key.setEnabled(gui.dataOK)
         gui.set_button.setEnabled(gui.set_dataOK)
 
     gui.encode = encode
 
     def decode():
         """Decode encoded or acquired fringes."""
+
+        flist = glob.glob(os.path.join(os.path.dirname(frng.decoder.__file__), "__pycache__", "decoder*decode*.nbc"))
+        if not flist or os.path.getmtime(frng.decoder.__file__) > max(os.path.getmtime(file) for file in flist):
+            logging.warning(
+                "The 'decode()'-function has not been compiled yet. "
+                "This will take a few minutes (the time depends on your CPU and energy settings)."
+            )
+
+            dialog = QMessageBox()
+            dialog.setWindowIcon(QtGui.QIcon(os.path.join(os.path.dirname(__file__), "numba-blue-icon-rgb.svg")))
+            dialog.setWindowTitle("Info")
+            dialog.setIcon(QMessageBox.Icon.Information)
+            dialog.setText(
+                "For the compitationally expensive decoding we make use of the just-in-time compiler Numba. "
+                "During the first execution, an initial compilation is executed. "
+                "This will take a few minutes (the time depends on your CPU and energy settings). "
+                "However, for any subsequent execution, the compiled code is cached "
+                "and the code of the function runs much faster, approaching the speeds of code written in C."
+            )
+            dialog.setStandardButtons(QMessageBox.StandardButton.Ok | QMessageBox.StandardButton.Cancel)
+
+            button = dialog.exec()
+
+            if button == QMessageBox.StandardButton.Cancel:
+                return
+
         if hasattr(gui.con, "brightness"):
             delattr(gui.con, "brightness")
         if hasattr(gui.con, "modulation"):
             delattr(gui.con, "modulation")
         if hasattr(gui.con, "registration"):
             delattr(gui.con, "registration")
         if hasattr(gui.con, "phase"):
@@ -393,174 +469,210 @@
             delattr(gui.con, "visibility")
 
         # todo: generic deletion
         # for key in gui.fringes._verbose_output:
         #     if hasattr(gui.con, key):
         #         delattr(gui.con, key)
 
+        view(None)
         gui.data_table.setData(gui.con.info)
         QtWidgets.QApplication.processEvents()  # refresh event queue
 
         if hasattr(gui.con, gui.key):
             I = getattr(gui.con, gui.key)
-        # elif hasattr(gui.con, "raw"):
-        #     I = gui.con.raw
-        elif hasattr(gui.con, "fringes"):
+        else:
             I = gui.con.fringes
 
-        flist = glob.glob(os.path.join(os.path.dirname(frng.decoder.__file__), "__pycache__", "decoder*decode*.nbc"))
-        if flist and max(os.path.getmtime(file) for file in flist) < os.path.getmtime(__file__):
-            dialog = QMessageBox()
-            dialog.setWindowIcon(QtGui.QIcon(os.path.join(os.path.dirname(__file__), "numba-blue-icon-rgb.svg")))
-            dialog.setWindowTitle("Info")
-            dialog.setIcon(QMessageBox.Icon.Information)
-            dialog.setText("For the compitationally expensive decoding we make use of the just-in-time compiler Numba. During the first execution, an initial compilation is executed. This can take several tens of seconds up to single digit minutes, depending on your CPU. However, for any subsequent execution, the compiled code is cached and the code of the function runs much faster, approaching the speeds of code written in C.")
-            dialog.setStandardButtons(QMessageBox.StandardButton.Ok)
-            dialog.exec()
-
         with pg.BusyCursor():
             dec = gui.fringes.decode(I)
 
             for k, v in dec._asdict().items():
                 setattr(gui.con, k, v)
 
-            view(getattr(gui.con, "registration"))
+        view(gui.con.registration)
         gui.data_table.setData(gui.con.info)
         QtWidgets.QApplication.processEvents()  # refresh event queue
 
-        gui.remap_button.setEnabled(gui.remapOK)
-        gui.remap_key.setEnabled(gui.remapOK)
+        gui.source_button.setEnabled(gui.sourceOK)
+        gui.source_key.setEnabled(gui.sourceOK)
         gui.curvature_button.setEnabled(gui.curvatureOK)
         gui.curvature_key.setEnabled(gui.curvatureOK)
         gui.set_button.setEnabled(gui.set_dataOK)
 
     gui.decode = decode
 
-    def remap():
+    def register():
+        encode(display=False)
+        decode()
+
+    def source():
         if hasattr(gui.con, "source"):
             delattr(gui.con, "source")
 
+        view(None)
         gui.data_table.setData(gui.con.info)
         QtWidgets.QApplication.processEvents()  # refresh event queue
 
         with pg.BusyCursor():
             x = gui.con.registration
+
             if hasattr(gui.con, "modulation"):
                 B = gui.con.modulation
                 Bmin = 0
                 B[B < Bmin] = 0
             else:
                 B = None
-            mode = gui.fringes.mode  # todo
 
-            gui.con.source = gui.fringes.remap(x, B, mode=mode)
+            if hasattr(gui.con, "uncertainty"):
+                u = gui.con.uncertainty
+            else:
+                u = 0
+
+            if hasattr(gui.fringes, "mode"):
+                mode = gui.fringes.mode
+            else:
+                mode = "fast"
+
+            gui.con.source = gui.fringes.source(x, B, u, mode=mode)
+
+        view(gui.con.source)
+        gui.data_table.setData(gui.con.info)
+        QtWidgets.QApplication.processEvents()  # refresh event queue
+
+    def bright():
+        if hasattr(gui.con, "bright"):
+            delattr(gui.con, "bright")
+
+        view(None)
+        gui.data_table.setData(gui.con.info)
+        QtWidgets.QApplication.processEvents()  # refresh event queue
+
+        with pg.BusyCursor():
+            if hasattr(gui.con, "source"):
+                gui.con.bright = gui.fringes.brightfield(gui.con.source)
+
+                # gui.glogger.info("Bright-field.")
+                logger.info("Bright-field.")
+
+            view(gui.con.bright)
+            gui.data_table.setData(gui.con.info)
+            QtWidgets.QApplication.processEvents()  # refresh event queue
+
+    def bright_inverse():
+        if hasattr(gui.con, "bright_inverse"):
+            delattr(gui.con, "bright_inverse")
+
+        view(None)
+        gui.data_table.setData(gui.con.info)
+        QtWidgets.QApplication.processEvents()  # refresh event queue
+
+        with pg.BusyCursor():
+            if hasattr(gui.con, "source"):
+                gui.con.bright_inverse = gui.fringes.brightfield_inverse(gui.con.source)
+
+                # gui.glogger.info("Inverse bright-field.")
+                logger.info("Inverse bright-field.")
 
-            gui.fringes.logger.info("Remapped.")
+            view(gui.con.bright_inverse)
+            gui.data_table.setData(gui.con.info)
+            QtWidgets.QApplication.processEvents()  # refresh event queue
+
+    def dark():
+        if hasattr(gui.con, "dark"):
+            delattr(gui.con, "dark")
 
-        view(getattr(gui.con, "source"))
+        view(None)
+        view(None)
         gui.data_table.setData(gui.con.info)
         QtWidgets.QApplication.processEvents()  # refresh event queue
 
+        with pg.BusyCursor():
+            if hasattr(gui.con, "source"):
+                gui.con.dark = gui.fringes.darkfield(gui.con.source)
+
+                # gui.glogger.info("Dark-field.")
+                logger.info("Dark-field.")
+
+            view(gui.con.dark)
+            gui.data_table.setData(gui.con.info)
+            QtWidgets.QApplication.processEvents()  # refresh event queue
+
     def curvature():
         if hasattr(gui.con, "curvature"):
             delattr(gui.con, "curvature")
 
+        view(None)
         gui.data_table.setData(gui.con.info)
         QtWidgets.QApplication.processEvents()  # refresh event queue
 
         with pg.BusyCursor():
-            gui.con.curvature = frng.curvature(gui.con.registration)
+            gui.con.curvature = frng.curvature(gui.con.registration, normalize=True)
 
-            gui.fringes.logger.info("Computed curvature.")
-
-        view(getattr(gui.con, "curvature"))
+        view(gui.con.curvature)
         gui.data_table.setData(gui.con.info)
         QtWidgets.QApplication.processEvents()  # refresh event queue
 
         gui.height_button.setEnabled(True)
         gui.height_key.setEnabled(True)
 
     def height():
         if hasattr(gui.con, "height"):
             delattr(gui.con, "height")
 
-        with pg.BusyCursor():
-            gui.con.height = frng.height(gui.con.curvature)
-
-            gui.fringes.logger.info("Computed height.")
-
-        view(getattr(gui.con, "height"))
+        view(None)
         gui.data_table.setData(gui.con.info)
         QtWidgets.QApplication.processEvents()  # refresh event queue
 
+        with pg.BusyCursor():
+            gui.con.height = frng.height(gui.con.curvature)
+
+        view(gui.con.height)
         gui.data_table.setData(gui.con.info)
         QtWidgets.QApplication.processEvents()  # refresh event queue
 
-    def view(I=None, Imax=None, autoscale=False, enhance=False, cmap=None):  # todo: color map
+    def view(I=None, autoscale=False, cmap=None):  # todo: color map
         """Display image data in videoshape in the ImageView area of the GUI."""
-        try:
-            T, Y, X, C = frng.vshape(I).shape
-        except:
-            T = Y = X = C = None
-
-        if enhance and I is not None and T == 1 and 3 <= C and I.dtype == "uint8":  # improve lightfield-inspection
-            try:
-                I[..., 1] = 0
-                hsv = cv2.cvtColor(I, cv2.COLOR_RGB2HSV)
-                hsv[..., 1] = 255  # 2
-                I = cv2.cvtColor(hsv, cv2.COLOR_HSV2RGB)
-            except:
-                pass
 
         if I is None or not isinstance(I, np.ndarray) or not I.size:
             gui.imv.clear()
         elif I.ndim < 2:
-            gui.fringes.logger.error(
-                "Can't display array with less than 2 dimensions."
-            )  # todo: convert into videoshape
+            logger.error("Can't display array with less than 2 dimensions.")
         elif I.ndim > 4:
-            gui.fringes.logger.error(
-                "Can't display array with more than 4 dimensions."
-            )  # todo: convert into videoshape
+            logger.error("Can't display array with more than 4 dimensions.")
         elif I.dtype.kind in "b":  # bool
             gui.imv.setImage(I, autoLevels=False, levels=(0, 1), autoHistogramRange=False)
-            # gui.plot.setLimits(xMin=0, xMax=X, yMin=0, yMax=Y)
         elif I.dtype.kind in "ui":  # uint or int
             if autoscale:
                 gui.imv.setImage(I)
             else:
                 if I.dtype.kind == "u" or np.min(I) >= 0:
                     Imin = 0
                 else:
                     Imin = np.iinfo(I.dtype).min
 
-                if Imax is not None:
-                    Imax = int(Imax)
-                elif I.dtype.itemsize > 1:  # e.g. 16bit data may hold only 10bit or 12bit or 14bit information
+                if I.dtype.itemsize > 1:  # e.g. 16bit data may hold only 10bit or 12bit or 14bit information
                     if np.any(I > 2**10 - 1):  # 10-bit data
                         Imax = 2**10 - 1
                     elif np.any(I > 2**12 - 1):  # 12-bit data
                         Imax = 2**12 - 1
                     elif np.any(I > 2**14 - 1):  # 14-bit data
                         Imax = 2**14 - 1
                     else:
                         Imax = np.iinfo(I.dtype).max
                 else:
                     Imax = np.iinfo(I.dtype).max
 
                 gui.imv.setImage(I, autoLevels=False, levels=(Imin, Imax), autoHistogramRange=False)
-                # gui.plot.setLimits(xMin=0, xMax=X, yMin=0, yMax=Y)
         elif I.dtype.kind in "f":  # float
-            try:
-                if np.isnan(np.amax(I)):
-                    I = I.astype(np.float32)  # copy
-                    I[np.isnan(I)] = 0
-                gui.imv.setImage(I.astype(np.float32, copy=False))  # it's faster for float32 than for float64
-            except:
-                gui.fringes.logger.error("Couldn't display float data.")
+            if np.nan in I:
+                I = I.astype(np.float32)  # copy
+                I[np.isnan(I)] = 0
+                logger.info("Converted `nan` in data to `0`.")
+
+            gui.imv.setImage(I)
 
             # if cmap:  # todo: define cmaps
             #     try:
             #         from pyqtgraph.graphicsItems.GradientEditorItem import Gradients
             #
             #         # list the available colormaps
             #         print(Gradients.keys())
@@ -571,25 +683,34 @@
             #         # create colormaps from the builtins
             #         pos, color = zip(*Gradients[cmap]["ticks"])
             #         cmap = pg.ColorMap(pos, color)
             #
             #         gui.imv.setColorMap(cmap)
             #     except:
             #         pass
+        elif I.dtype.kind in "c":
+            I = np.concatenate(np.abs(I), np.angle(I), axis=0)
+
+            if Np.nan in I:
+                I = I.astype(np.float32)  # copy
+                I[np.isnan(I)] = 0
+
+                logger.info("Converted `nan` in data to `0`.")
 
-            # gui.plot.setLimits(xMin=0, xMax=X, yMin=0, yMax=Y)
+            gui.imv.setImage(I)
         else:
-            gui.fringes.logger.error("Can't display array with dtype %s." % I.dtype)
+            logger.error("Can't display array with dtype %s." % I.dtype)
 
         QtWidgets.QApplication.processEvents()  # refresh event queue
 
     gui.view = view
 
     def zoomback():
-        pass  # todo: zoom back strg + 0
+        gui.win.setGeometry(QtGui.QGuiApplication.primaryScreen().availableGeometry())
+        gui.win.showMaximized()
 
     def selection_changed():
         """Display the data which was selected."""
 
         try:
             item = gui.data_table.currentItem().text()  # todo: select first element of selected row
         except:
@@ -597,15 +718,15 @@
 
         if hasattr(gui.con, item):
             view(getattr(gui.con, item))
         else:
             view(None)
 
     # assign functionality to buttons
-    gui.immerse_key.activated.connect(immerse)
+    gui.full_screen_key.activated.connect(full_screen)
 
     gui.undo_key.activated.connect(undo)
     gui.redo_key.activated.connect(redo)
     gui.reset_button.clicked.connect(reset)
     gui.reset_key.activated.connect(reset)
 
     gui.load_button.clicked.connect(load)
@@ -620,16 +741,20 @@
     gui.data_table.itemSelectionChanged.connect(selection_changed)
 
     gui.coordinates_key.activated.connect(coordinates)
     gui.encode_button.clicked.connect(encode)
     gui.encode_key.activated.connect(encode)
     gui.decode_button.clicked.connect(decode)
     gui.decode_key.activated.connect(decode)
+    gui.register_key.activated.connect(register)
 
-    gui.remap_button.clicked.connect(remap)
-    gui.remap_key.activated.connect(remap)
+    gui.source_button.clicked.connect(source)
+    gui.source_key.activated.connect(source)
+    gui.bright_key.activated.connect(bright)
+    gui.bright_inverse_key.activated.connect(bright_inverse)
+    gui.dark_key.activated.connect(dark)
     gui.curvature_button.clicked.connect(curvature)
     gui.curvature_key.activated.connect(curvature)
     gui.height_button.clicked.connect(height)
     gui.height_key.activated.connect(height)
 
     gui.zoomback_key.activated.connect(zoomback)
```

### Comparing `fringes_gui-0.3.3/fringes_gui/numba-blue-icon-rgb.svg` & `fringes_gui-1.0.0/fringes_gui/numba-blue-icon-rgb.svg`

 * *Files identical despite different names*

### Comparing `fringes_gui-0.3.3/fringes_gui/params.py` & `fringes_gui-1.0.0/fringes_gui/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import logging as lg
+import logging
 
 import numpy as np
 
+logger = logging.getLogger(__name__)
+
 
 def set_params(gui):
     """Define the parameter tree."""
 
     vis = {
         "title": "Visibility",
         "name": "vis",
@@ -20,25 +22,25 @@
         f"for the assignment of the recommended visibility:\n"
         f"\u2B9A Beginner: Features that should be visible for all users via the GUI. This "
         f"is the default visibility. The number of features with 'Beginner' visibility "
         f"should be limited to all basic features so the GUI display is well-organized "
         f"and easy to use.\n"
         f"\u2B9A Expert: Features that require a more in-depth knowledge of the system "
         f"functionality. This is the preferred visibility level for all advanced features.\n"
-        f"\u2B9A Guru: - Guru: Advanced features that usually only people"
+        f"\u2B9A Guru: - Guru: Advanced features that usually only people "
         f"with a sound background in phase shifting can make good use of.\n"
         f"\u2B9A Experimental: New features that have not been tested yet "
         f"and the system might probably crash at some point.",
     }
     log = {
         "title": "Logging",
         "name": "log",
         "type": "list",
-        "value": lg.getLevelName(gui.fringes.logger.level),
-        "default": lg.getLevelName(gui.fringes.logger.level),
+        "value": logging.getLevelName(gui.glogger.level),
+        "default": logging.getLevelName(gui.glogger.level),
         "limits": ("DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"),
         "tip": "Logging level.",
     }
     vid = {
         "title": "Video Shape",
         "name": "vid",
         "type": "group",
@@ -190,173 +192,181 @@
                 "tip": gui.fringes.__class__.K.__doc__,
             },
             {
                 "title": "Shifts",
                 "name": "N",
                 "type": "action",
                 "tip": "Reset values to defaults.",
-                "children": [
-                    {
-                        "name": "N" + str(d).translate(gui.sub) + "," + str(k).translate(gui.sub),
-                        "type": "int",
-                        "value": gui.fringes._N[d, k],
-                        "default": gui.fringes._Nmin if gui.fringes.FDM else gui.fringes.defaults["N"][0, 0],
-                        "limits": (
-                            max(
-                                gui.fringes._Nmin,
-                                1 if gui.visibility == "Guru" else 2 if gui.visibility == "Expert" else 3,
+                "children": (
+                    [
+                        {
+                            "name": "N" + str(d).translate(gui.sub) + "," + str(k).translate(gui.sub),
+                            "type": "int",
+                            "value": gui.fringes._N[d, k],
+                            "default": gui.fringes._Nmin if gui.fringes.FDM else gui.fringes.defaults["N"][0, 0],
+                            "limits": (
+                                max(
+                                    gui.fringes._Nmin,
+                                    3,  # 1 if gui.visibility == "Guru" else 2 if gui.visibility == "Expert" else 3,
+                                ),
+                                gui.fringes._Nmax,
                             ),
-                            gui.fringes._Nmax,
-                        ),
-                        "tip": gui.fringes.__class__.N.__doc__,
-                    }
-                    for d in range(gui.fringes.D)
-                    for k in range(gui.fringes.K)
-                ]
-                if gui.visibility == "Guru" or gui.fringes.N.ndim > 1
-                else [  # todo: FDM: N_i
-                    {
-                        "name": "N" + str(k).translate(gui.sub),
-                        "type": "int",
-                        "value": gui.fringes.N[k],
-                        "default": gui.fringes._Nmin if gui.fringes.FDM else gui.fringes.defaults["N"][0, 0],
-                        "limits": (
-                            max(
-                                gui.fringes._Nmin,
-                                1 if gui.visibility == "Guru" else 2 if gui.visibility == "Expert" else 3,
+                            "tip": gui.fringes.__class__.N.__doc__,
+                        }
+                        for d in range(gui.fringes.D)
+                        for k in range(gui.fringes.K)
+                    ]
+                    if gui.visibility == "Guru" or gui.fringes.N.ndim > 1
+                    else [  # todo: FDM: N_i
+                        {
+                            "name": "N" + str(k).translate(gui.sub),
+                            "type": "int",
+                            "value": gui.fringes.N[k],
+                            "default": gui.fringes._Nmin if gui.fringes.FDM else gui.fringes.defaults["N"][0, 0],
+                            "limits": (
+                                max(
+                                    gui.fringes._Nmin,
+                                    1 if gui.visibility == "Guru" else 2 if gui.visibility == "Expert" else 3,
+                                ),
+                                gui.fringes._Nmax,
                             ),
-                            gui.fringes._Nmax,
-                        ),
-                        "tip": gui.fringes.__class__.N.__doc__,
-                    }
-                    for k in range(gui.fringes.K)
-                ],
+                            "tip": gui.fringes.__class__.N.__doc__,
+                        }
+                        for k in range(gui.fringes.K)
+                    ]
+                ),
             },
             {
                 "title": "Wavelengths",
                 "name": "l",
                 "type": "action",
                 "tip": "Set optimal wavelengths automatically.",
-                "children": [
-                    {
-                        "title": "\u03BB" + str(d).translate(gui.sub) + ", " + str(k).translate(gui.sub),
-                        "name": "l" + str(d).translate(gui.sub) + "," + str(k).translate(gui.sub),
-                        "type": "float",
-                        "value": gui.fringes._l[d, k],
-                        "default": None,  # gui.fringes.L ** (1 / (k + 1)),
-                        "limits": (gui.fringes.lmin, None),
-                        "decimals": gui.digits,
-                        "tip": gui.fringes.__class__.l.__doc__,
-                    }
-                    for d in range(gui.fringes.D)
-                    for k in range(gui.fringes.K)
-                ]
-                if gui.visibility == "Guru" or gui.fringes.l.ndim > 1
-                else [
-                    {
-                        "title": "\u03BB" + str(k).translate(gui.sub),
-                        "name": "l" + str(k).translate(gui.sub),
-                        "type": "float",
-                        "value": gui.fringes.l[k],
-                        "default": None,  # gui.fringes.L ** (1 / (k + 1)),
-                        "suffix": " px",
-                        "limits": (gui.fringes.lmin, None),
-                        "decimals": gui.digits,
-                        "tip": gui.fringes.__class__.l.__doc__,
-                    }
-                    for k in range(gui.fringes.K)
-                ],
+                "children": (
+                    [
+                        {
+                            "title": "\u03BB" + str(d).translate(gui.sub) + ", " + str(k).translate(gui.sub),
+                            "name": "l" + str(d).translate(gui.sub) + "," + str(k).translate(gui.sub),
+                            "type": "float",
+                            "value": gui.fringes._l[d, k],
+                            "default": None,  # gui.fringes.L ** (1 / (k + 1)),
+                            "limits": (gui.fringes.lmin, None),
+                            "decimals": gui.digits,
+                            "tip": gui.fringes.__class__.l.__doc__,
+                        }
+                        for d in range(gui.fringes.D)
+                        for k in range(gui.fringes.K)
+                    ]
+                    if gui.visibility == "Guru" or gui.fringes.l.ndim > 1
+                    else [
+                        {
+                            "title": "\u03BB" + str(k).translate(gui.sub),
+                            "name": "l" + str(k).translate(gui.sub),
+                            "type": "float",
+                            "value": gui.fringes.l[k],
+                            "default": None,  # gui.fringes.L ** (1 / (k + 1)),
+                            "suffix": " px",
+                            "limits": (gui.fringes.lmin, None),
+                            "decimals": gui.digits,
+                            "tip": gui.fringes.__class__.l.__doc__,
+                        }
+                        for k in range(gui.fringes.K)
+                    ]
+                ),
             },
             {
                 "title": "Periods",
                 "name": "v",
                 "type": "action",
                 "tip": "Set optimal periods automatically.",
-                "children": [
-                    {
-                        "title": "\u03BD" + str(d).translate(gui.sub) + ", " + str(k).translate(gui.sub),
-                        "name": "v" + str(d).translate(gui.sub) + "," + str(k).translate(gui.sub),
-                        "type": "float",
-                        "value": gui.fringes._v[d, k],
-                        "default": None,  # gui.fringes.L ** (1 - 1 / (k + 1)),
-                        "limits": (0, gui.fringes.vmax),
-                        "decimals": gui.digits,
-                        "tip": gui.fringes.__class__.v.__doc__,
-                    }
-                    for d in range(gui.fringes.D)
-                    for k in range(gui.fringes.K)
-                ]
-                if gui.visibility == "Guru" or gui.fringes.v.ndim > 1
-                else [
-                    {
-                        "title": "\u03BD" + str(k).translate(gui.sub),
-                        "name": "v" + str(k).translate(gui.sub),
-                        "type": "float",
-                        "value": gui.fringes.v[k],
-                        "default": None,  # gui.fringes.L ** (1 - 1 / (k + 1)),
-                        "limits": (0, gui.fringes.vmax),
-                        "decimals": gui.digits,
-                        "tip": gui.fringes.__class__.v.__doc__,
-                    }
-                    for k in range(gui.fringes.K)
-                ],
+                "children": (
+                    [
+                        {
+                            "title": "\u03BD" + str(d).translate(gui.sub) + ", " + str(k).translate(gui.sub),
+                            "name": "v" + str(d).translate(gui.sub) + "," + str(k).translate(gui.sub),
+                            "type": "float",
+                            "value": gui.fringes._v[d, k],
+                            "default": None,  # gui.fringes.L ** (1 - 1 / (k + 1)),
+                            "limits": (0, gui.fringes.vmax),
+                            "decimals": gui.digits,
+                            "tip": gui.fringes.__class__.v.__doc__,
+                        }
+                        for d in range(gui.fringes.D)
+                        for k in range(gui.fringes.K)
+                    ]
+                    if gui.visibility == "Guru" or gui.fringes.v.ndim > 1
+                    else [
+                        {
+                            "title": "\u03BD" + str(k).translate(gui.sub),
+                            "name": "v" + str(k).translate(gui.sub),
+                            "type": "float",
+                            "value": gui.fringes.v[k],
+                            "default": None,  # gui.fringes.L ** (1 - 1 / (k + 1)),
+                            "limits": (0, gui.fringes.vmax),
+                            "decimals": gui.digits,
+                            "tip": gui.fringes.__class__.v.__doc__,
+                        }
+                        for k in range(gui.fringes.K)
+                    ]
+                ),
             },
             {
                 "title": "Frequencies",
                 "name": "f",
                 "type": "action",
                 "visible": gui.visibility == "Guru",
                 "tip": "Reset values to defaults.",
-                "children": [
-                    {
-                        "name": "f" + str(d).translate(gui.sub) + "," + str(k).translate(gui.sub),
-                        "type": "float",
-                        "value": gui.fringes._f[d, k],
-                        "default": None if gui.fringes.FDM else 1,
-                        "limits": (-gui.fringes._fmax, gui.fringes._fmax),
-                        "decimals": gui.digits,
-                        "readonly": gui.fringes.FDM and gui.fringes.static,
-                        "tip": gui.fringes.__class__.f.__doc__,
-                    }
-                    for d in range(gui.fringes.D)
-                    for k in range(gui.fringes.K)
-                ]
-                if gui.visibility == "Guru" or gui.fringes.FDM or gui.fringes.f.ndim > 1
-                else [
-                    {
-                        "name": "f" + str(k).translate(gui.sub),
-                        "type": "float",
-                        "value": gui.fringes.f[k],
-                        "default": 1,
-                        "limits": (-gui.fringes._fmax, gui.fringes._fmax),
-                        "decimals": gui.digits,
-                        "tip": gui.fringes.__class__.f.__doc__,
-                    }
-                    for k in range(gui.fringes.K)
-                ],
+                "children": (
+                    [
+                        {
+                            "name": "f" + str(d).translate(gui.sub) + "," + str(k).translate(gui.sub),
+                            "type": "float",
+                            "value": gui.fringes._f[d, k],
+                            "default": None if gui.fringes.FDM else 1,
+                            "limits": (-gui.fringes._fmax, gui.fringes._fmax),
+                            "decimals": gui.digits,
+                            "readonly": gui.fringes.FDM and gui.fringes.static,
+                            "tip": gui.fringes.__class__.f.__doc__,
+                        }
+                        for d in range(gui.fringes.D)
+                        for k in range(gui.fringes.K)
+                    ]
+                    if gui.visibility == "Guru" or gui.fringes.FDM or gui.fringes.f.ndim > 1
+                    else [
+                        {
+                            "name": "f" + str(k).translate(gui.sub),
+                            "type": "float",
+                            "value": gui.fringes.f[k],
+                            "default": 1,
+                            "limits": (-gui.fringes._fmax, gui.fringes._fmax),
+                            "decimals": gui.digits,
+                            "tip": gui.fringes.__class__.f.__doc__,
+                        }
+                        for k in range(gui.fringes.K)
+                    ]
+                ),
             },
             {
                 "title": "Reverse",
                 "name": "reverse",
                 "type": "bool",
                 "value": gui.fringes.reverse,
                 "default": gui.fringes.defaults["reverse"],
                 "tip": gui.fringes.__class__.reverse.__doc__,
             },
             {
                 "title": "Offset",
-                "name": "o",
+                "name": "p0",
                 "type": "float",
-                "value": gui.fringes.o / np.pi,
-                "default": gui.fringes.defaults["o"] / np.pi,
+                "value": gui.fringes.p0 / np.pi,
+                "default": gui.fringes.defaults["p0"] / np.pi,
                 "limits": (-2, 2),
                 "step": 0.5,
                 "decimals": gui.digits,
                 "suffix": "\U0001D745",  # \U0001D70B
-                "tip": gui.fringes.__class__.o.__doc__,
+                "tip": gui.fringes.__class__.p0.__doc__,
             },
             {
                 "title": "\u03BB\u2098\u1D62\u2099",
                 "name": "lmin",
                 "type": "float",
                 "value": gui.fringes.lmin,
                 "default": gui.fringes.defaults["lmin"],
@@ -480,15 +490,15 @@
             },
             {
                 "title": "Gamma",
                 "name": "gamma",
                 "type": "float",
                 "value": gui.fringes.gamma,
                 "default": gui.fringes.defaults["gamma"],
-                "limits": (0, gui.fringes.__class__._gammamax),
+                "limits": (0.1, gui.fringes.__class__._gammamax),  # todo: gammamin
                 "step": 0.1,
                 "decimals": gui.digits,
                 "tip": gui.fringes.__class__.gamma.__doc__,
             },
         ],
     }
     col = {
```

### Comparing `fringes_gui-0.3.3/fringes_gui/setters.py` & `fringes_gui-1.0.0/fringes_gui/setters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+import logging
 import os
 from collections import deque
 
 import numpy as np
 import pyqtgraph as pg
 from pyqtgraph.Qt import QtWidgets
+import fringes as frng
 
 from .params import set_params
 from .logic import set_logic
 
+logger = logging.getLogger(__name__)
+
 
 def set_functionality(gui):
     """Give the list of parameters defined in Gui their functionality, i.e. set listeners for when they are changed."""
 
     set_params(gui)
 
     gui.params = pg.parametertree.Parameter.create(name="Settings", type="group", children=gui.params)
@@ -46,15 +50,28 @@
         key = change[0][0].opts["name"]
         val = change[0][2]
 
         if key in ["grid", "angle", "D"]:
             if hasattr(gui.con, "coordinates"):
                 delattr(gui.con, "coordinates")
 
-        if key not in ["mode", "Vmin", "verbose"] or key == "axis" and gui.fringes.D == 2:
+        if key in ["mode"]:
+            if hasattr(gui.con, "source"):
+                delattr(gui.con, "source")
+
+            if hasattr(gui.con, "bright_inverse"):
+                delattr(gui.con, "bright_inverse")
+
+            if hasattr(gui.con, "bright"):
+                delattr(gui.con, "bright")
+
+            if hasattr(gui.con, "dark"):
+                delattr(gui.con, "dark")
+
+        if key not in ["mode", "verbose"] or key == "axis" and gui.fringes.D == 2:
             if hasattr(gui.con, "fringes"):
                 delattr(gui.con, "fringes")
 
                 if hasattr(gui.con, "registration"):
                     gui.view(gui.con.registration)
                 elif hasattr(gui.con, gui.key):
                     gui.view(getattr(gui.con, gui.key))
@@ -107,20 +124,23 @@
                 gui.decode()
 
         gui.data_table.setData(gui.con.info)
         QtWidgets.QApplication.processEvents()  # refresh event queue
 
         if key == "vis":
             set_visibility(val)
-            gui.fringes.logger.debug(f"Set visibility to {gui.visibility}.")
+            # gui.glogger.debug(f"Set visibility to {gui.visibility}.")
+            logger.debug(f"Set visibility to {gui.visibility}.")
             gui.reset_button.setEnabled(gui.resetOK)
             return
         elif key == "log":
-            gui.fringes.logger.setLevel(val)
-            gui.fringes.logger.debug(f"Set logging level to '{val}'.")
+            gui.glogger.setLevel(val)
+            gui.flogger.setLevel(val)
+            # gui.glogger.debug(f"Set logging level to '{val}'.")
+            logger.debug(f"Set logging level to '{val}'.")
             return
 
         if key[0] in "Nlvfh" and (key[-1] == "ᵢ" or key[-1].translate(gui.sup).isdigit()) and 2 <= len(key) <= 4:
             key, id = key[0], key[1:]
             idx = id.translate(gui.sup).split(",")
             d = int(idx[0]) if len(idx) == 2 else 0
             k = int(idx[-1]) if idx[-1] != "ᵢ" else 0  # if idx[-1] != "" else 0
@@ -146,15 +166,15 @@
                     val_old[k] = [val.red(), val.green(), val.blue()]
             elif gui.visibility in ["Guru", "Experimental"] or gui.fringes.FDM:
                 val_old[d, k] = val
             else:
                 val_old[:, k] = val
 
             val = val_old
-        elif key == "o":
+        elif key == "p0":
             val *= np.pi
 
         setattr(gui.fringes, key, val)
         gui.fringes.save(os.path.join(os.path.expanduser("~"), ".fringes.yaml"))
 
         update_parameter_tree()
 
@@ -172,16 +192,16 @@
                 gui.params.param("sys", "angle").setValue(gui.fringes.defaults["angle"])
                 gui.params.param("sys", "angle").hide()
                 gui.fringes.N = np.maximum(gui.fringes._N, 3)
                 set_frequencies()
                 gui.params.param("set", "f").hide()
                 # gui.params.param("set", "reverse").setValue(gui.fringes.defaults["reverse"])
                 # gui.params.param("set", "reverse").hide()
-                # gui.params.param("set", "o").setValue(gui.fringes.defaults["o"] / np.pi)
-                # gui.params.param("set", "o").hide()
+                # gui.params.param("set", "p0").setValue(gui.fringes.defaults["p0"] / np.pi)
+                # gui.params.param("set", "p0").hide()
                 gui.params.param("set", "lmin").setValue(gui.fringes.defaults["lmin"])
                 gui.params.param("set", "lmin").hide()
                 gui.params.param("set", "vmax").hide()
                 gui.params.param("set", "lopt").hide()
                 gui.params.param("set", "vopt").hide()
                 gui.params.param("val").hide()
                 gui.params.param("val", "dtype").setValue(gui.fringes.defaults["dtype"])
@@ -216,15 +236,15 @@
                 gui.params.param("sys", "grid").hide()
                 gui.params.param("sys", "angle").setValue(gui.fringes.defaults["angle"])
                 gui.params.param("sys", "angle").hide()
                 gui.fringes.N = np.maximum(gui.fringes._N, 2)
                 set_frequencies()
                 gui.params.param("set", "f").hide()
                 # gui.params.param("set", "reverse").show()
-                # gui.params.param("set", "o").show()
+                # gui.params.param("set", "p0").show()
                 gui.params.param("set", "lmin").show()
                 gui.params.param("set", "vmax").hide()
                 gui.params.param("set", "lopt").hide()
                 gui.params.param("set", "vopt").hide()
                 gui.params.param("val").show()
                 gui.params.param("val", "dtype").setValue(gui.fringes.defaults["dtype"])
                 gui.params.param("val", "dtype").hide()
@@ -262,15 +282,15 @@
                     (
                         1,
                         (gui.fringes._Nmax - 1) / 2 / gui.fringes.D if gui.fringes.FDM else gui.fringes._Kmax,
                     )
                 )
                 gui.params.param("set", "f").show()
                 # gui.params.param("set", "reverse").show()
-                # gui.params.param("set", "o").show()
+                # gui.params.param("set", "p0").show()
                 gui.params.param("set", "lmin").show()
                 gui.params.param("set", "vmax").hide()
                 gui.params.param("set", "lopt").hide()
                 gui.params.param("set", "vopt").hide()
                 gui.params.param("val", "dtype").show()
                 gui.params.param("val", "Imax").show()
                 gui.params.param("col", "H").setLimits((1, gui.fringes._Hmax))
@@ -396,38 +416,40 @@
                         if gui.fringes.FDM:  # all shifts must be equal; hence create only one generic index "i"
                             if d == k == 0:
                                 gui.params.param("set", "N").addChild(
                                     {
                                         "name": "N" + "ᵢ",
                                         "type": "int",
                                         "value": gui.fringes._N[d, k],
-                                        "default": gui.fringes._Nmin
-                                        if gui.fringes.FDM
-                                        else gui.fringes.defaults["N"][0, 0],
+                                        "default": (
+                                            gui.fringes._Nmin if gui.fringes.FDM else gui.fringes.defaults["N"][0, 0]
+                                        ),
                                         "limits": (
                                             max(
                                                 gui.fringes._Nmin,
-                                                1
-                                                if gui.visibility == "Guru"
-                                                else 2
-                                                if gui.visibility == "Expert"
-                                                else 3,
+                                                (
+                                                    1
+                                                    if gui.visibility == "Guru"
+                                                    else 2 if gui.visibility == "Expert" else 3
+                                                ),
                                             ),
                                             gui.fringes._Nmax,
                                         ),
                                         "tip": gui.fringes.__class__.N.__doc__,
                                     }
                                 )
                         else:
                             gui.params.param("set", "N").addChild(
                                 {
                                     "name": "N" + id,
                                     "type": "int",
                                     "value": gui.fringes._N[d, k],
-                                    "default": gui.fringes._Nmin if gui.fringes.FDM else gui.fringes.defaults["N"][0, 0],
+                                    "default": (
+                                        gui.fringes._Nmin if gui.fringes.FDM else gui.fringes.defaults["N"][0, 0]
+                                    ),
                                     "limits": (
                                         max(
                                             gui.fringes._Nmin,
                                             1 if gui.visibility == "Guru" else 2 if gui.visibility == "Expert" else 3,
                                         ),
                                         gui.fringes._Nmax,
                                     ),
@@ -462,19 +484,19 @@
                         )
 
                         gui.params.param("set", "f").addChild(
                             {
                                 "name": "f" + id,
                                 "type": "float",
                                 "value": gui.fringes._f[d, k],
-                                "default": gui.fringes._f[d, k]
-                                if gui.fringes.FDM and gui.fringes.static
-                                else gui.fringes.D * k + k
-                                if gui.fringes.FDM
-                                else 1,
+                                "default": (
+                                    gui.fringes._f[d, k]
+                                    if gui.fringes.FDM and gui.fringes.static
+                                    else gui.fringes.D * k + k if gui.fringes.FDM else 1
+                                ),
                                 "limits": (-gui.fringes.vmax, gui.fringes.vmax),
                                 "decimals": gui.digits,
                                 "readonly": gui.fringes.FDM and gui.fringes.static,
                                 "tip": gui.fringes.__class__.f.__doc__,
                             }
                         )
                     else:  # update child params
@@ -517,15 +539,15 @@
                         gui.params.param("set", "f", "f" + id).setReadonly(gui.fringes.FDM and gui.fringes.static)
                         gui.params.param("set", "f", "f" + id).setLimits((-gui.fringes.vmax, gui.fringes.vmax))
                         gui.params.param("set", "f", "f" + id).setValue(gui.fringes._f[d, k])
                         gui.params.param("set", "f", "f" + id).setDefault(None if gui.fringes.FDM else 1)
 
             gui.params.param("set", "reverse").setValue(gui.fringes.reverse)
 
-            gui.params.param("set", "o").setValue(gui.fringes.o / np.pi)
+            gui.params.param("set", "p0").setValue(gui.fringes.p0 / np.pi)
 
             gui.params.param("set", "lmin").setValue(gui.fringes.lmin)
 
             gui.params.param("set", "vmax").setValue(gui.fringes.vmax)
 
             gui.params.param("set", "UMR").setValue(gui.fringes.UMR.min())
 
@@ -615,25 +637,24 @@
             gui.params.param("quali", "shot").setValue(gui.fringes.shot)
 
             gui.params.param("quali", "u").setValue(gui.fringes.u.max())
 
             gui.params.param("quali", "DR").setValue(gui.fringes.DRdB.max())
 
         gui.reset_button.setEnabled(gui.resetOK)
-        gui.encode_button.setStyleSheet("" if gui.encodeOK else "QPushButton{color: red}")
+        gui.encode_button.setStyleSheet("" if not gui.fringes._ambiguous else "QPushButton{color: red}")
         gui.decode_button.setEnabled(gui.decodeOK)
         gui.decode_key.setEnabled(gui.decodeOK)
-        gui.remap_button.setEnabled(gui.remapOK)
-        gui.remap_key.setEnabled(gui.remapOK)
+        gui.source_button.setEnabled(gui.sourceOK)
+        gui.source_key.setEnabled(gui.sourceOK)
         gui.curvature_button.setEnabled(gui.curvatureOK)
         gui.curvature_key.setEnabled(gui.curvatureOK)
         gui.height_button.setEnabled(gui.heightOK)
         gui.height_key.setEnabled(gui.heightOK)
 
-
     gui.update_parameter_tree = update_parameter_tree
 
     def set_shifts():
         gui.fringes.N = 4
         update_parameter_tree()
         gui.fringes.save(os.path.join(os.path.expanduser("~"), ".fringes.yaml"))
```

