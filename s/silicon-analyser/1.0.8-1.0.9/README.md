# Comparing `tmp/silicon_analyser-1.0.8.tar.gz` & `tmp/silicon_analyser-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silicon_analyser-1.0.8.tar", last modified: Thu Apr 18 18:34:42 2024, max compression
+gzip compressed data, was "silicon_analyser-1.0.9.tar", last modified: Sat Apr 20 10:28:21 2024, max compression
```

## Comparing `silicon_analyser-1.0.8.tar` & `silicon_analyser-1.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/
--rw-rw-rw-   0        0        0     1087 2024-04-18 18:34:42.000000 silicon_analyser-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     3334 2024-04-18 18:34:42.000000 silicon_analyser-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2530 2024-04-16 18:45:45.000000 silicon_analyser-1.0.8/README.md
--rw-rw-rw-   0        0        0     1154 2024-04-18 18:33:46.000000 silicon_analyser-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 18:34:42.000000 silicon_analyser-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser/
-drwxrwxrwx   0        0        0        0 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser/dialogs/
--rw-rw-rw-   0        0        0     3487 2024-04-13 14:15:10.000000 silicon_analyser-1.0.8/silicon_analyser/dialogs/compute_stats.py
--rw-rw-rw-   0        0        0     1508 2024-04-06 18:45:56.000000 silicon_analyser-1.0.8/silicon_analyser/dialogs/compute_stats.ui
--rw-rw-rw-   0        0        0     3340 2024-04-14 09:21:04.000000 silicon_analyser-1.0.8/silicon_analyser/dialogs/pixel_image.py
--rw-rw-rw-   0        0        0     3752 2024-04-14 09:20:00.000000 silicon_analyser-1.0.8/silicon_analyser/dialogs/pixel_image.ui
--rw-rw-rw-   0        0        0     3883 2024-04-16 18:29:36.000000 silicon_analyser-1.0.8/silicon_analyser/grid.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser/helper/
-drwxrwxrwx   0        0        0        0 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser/helper/abstract/
--rw-rw-rw-   0        0        0     2406 2024-04-16 16:39:34.000000 silicon_analyser-1.0.8/silicon_analyser/helper/abstract/abstractimage.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 17:24:06.000000 silicon_analyser-1.0.8/silicon_analyser/helper/abstract/abstractmywindow.py
--rw-rw-rw-   0        0        0     1024 2024-04-13 06:54:26.000000 silicon_analyser-1.0.8/silicon_analyser/helper/abstract/abstracttreehelper.py
--rw-rw-rw-   0        0        0      719 2024-04-13 07:29:28.000000 silicon_analyser-1.0.8/silicon_analyser/helper/addgridbtn.py
--rw-rw-rw-   0        0        0      696 2024-04-08 17:17:53.000000 silicon_analyser-1.0.8/silicon_analyser/helper/addlabelbtn.py
--rw-rw-rw-   0        0        0     1768 2024-04-18 18:06:25.000000 silicon_analyser-1.0.8/silicon_analyser/helper/ai.py
--rw-rw-rw-   0        0        0    16999 2024-04-18 18:21:52.000000 silicon_analyser-1.0.8/silicon_analyser/helper/computebtn.py
--rw-rw-rw-   0        0        0    21170 2024-04-17 15:20:05.000000 silicon_analyser-1.0.8/silicon_analyser/helper/fullimage.py
--rw-rw-rw-   0        0        0     1532 2024-04-13 13:40:26.000000 silicon_analyser-1.0.8/silicon_analyser/helper/minimap.py
--rw-rw-rw-   0        0        0     3989 2024-04-16 18:29:06.000000 silicon_analyser-1.0.8/silicon_analyser/helper/properties.py
--rw-rw-rw-   0        0        0    20657 2024-04-16 18:12:59.000000 silicon_analyser-1.0.8/silicon_analyser/helper/tree.py
--rw-rw-rw-   0        0        0      263 2024-04-08 17:15:10.000000 silicon_analyser-1.0.8/silicon_analyser/main.py
--rw-rw-rw-   0        0        0     7687 2024-04-18 18:24:48.000000 silicon_analyser-1.0.8/silicon_analyser/main_window.ui
--rw-rw-rw-   0        0        0    10412 2024-04-18 17:28:35.000000 silicon_analyser-1.0.8/silicon_analyser/mywindow.py
--rw-rw-rw-   0        0        0      134 2024-04-07 08:11:27.000000 silicon_analyser-1.0.8/silicon_analyser/rect.py
--rw-rw-rw-   0        0        0     2305 2024-04-16 18:10:57.000000 silicon_analyser-1.0.8/silicon_analyser/savefiles.py
--rw-rw-rw-   0        0        0     1365 2024-04-13 14:16:41.000000 silicon_analyser-1.0.8/silicon_analyser/treeitem.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser.egg-info/
--rw-rw-rw-   0        0        0     3334 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1078 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 10:28:20.000000 silicon_analyser-1.0.9/
+-rw-rw-rw-   0        0        0     1087 2024-04-07 16:13:23.000000 silicon_analyser-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3334 2024-04-20 10:28:21.000000 silicon_analyser-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2530 2024-04-16 18:45:45.000000 silicon_analyser-1.0.9/README.md
+-rw-rw-rw-   0        0        0     1154 2024-04-20 08:43:03.000000 silicon_analyser-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-20 10:28:21.000000 silicon_analyser-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 10:28:20.000000 silicon_analyser-1.0.9/silicon_analyser/
+drwxrwxrwx   0        0        0        0 2024-04-20 10:28:20.000000 silicon_analyser-1.0.9/silicon_analyser/dialogs/
+-rw-rw-rw-   0        0        0     3487 2024-04-13 14:15:10.000000 silicon_analyser-1.0.9/silicon_analyser/dialogs/compute_stats.py
+-rw-rw-rw-   0        0        0     1508 2024-04-06 18:45:56.000000 silicon_analyser-1.0.9/silicon_analyser/dialogs/compute_stats.ui
+-rw-rw-rw-   0        0        0     3340 2024-04-14 09:21:04.000000 silicon_analyser-1.0.9/silicon_analyser/dialogs/pixel_image.py
+-rw-rw-rw-   0        0        0     3752 2024-04-14 09:20:00.000000 silicon_analyser-1.0.9/silicon_analyser/dialogs/pixel_image.ui
+-rw-rw-rw-   0        0        0     5000 2024-04-20 10:25:34.000000 silicon_analyser-1.0.9/silicon_analyser/grid.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:28:20.000000 silicon_analyser-1.0.9/silicon_analyser/helper/
+drwxrwxrwx   0        0        0        0 2024-04-20 10:28:20.000000 silicon_analyser-1.0.9/silicon_analyser/helper/abstract/
+-rw-rw-rw-   0        0        0     2406 2024-04-16 16:39:34.000000 silicon_analyser-1.0.9/silicon_analyser/helper/abstract/abstractimage.py
+-rw-rw-rw-   0        0        0     3006 2024-04-20 08:48:27.000000 silicon_analyser-1.0.9/silicon_analyser/helper/abstract/abstractmywindow.py
+-rw-rw-rw-   0        0        0     1024 2024-04-13 06:54:26.000000 silicon_analyser-1.0.9/silicon_analyser/helper/abstract/abstracttreehelper.py
+-rw-rw-rw-   0        0        0      719 2024-04-13 07:29:28.000000 silicon_analyser-1.0.9/silicon_analyser/helper/addgridbtn.py
+-rw-rw-rw-   0        0        0      696 2024-04-08 17:17:53.000000 silicon_analyser-1.0.9/silicon_analyser/helper/addlabelbtn.py
+-rw-rw-rw-   0        0        0     1768 2024-04-18 18:06:25.000000 silicon_analyser-1.0.9/silicon_analyser/helper/ai.py
+-rw-rw-rw-   0        0        0    16999 2024-04-18 18:21:52.000000 silicon_analyser-1.0.9/silicon_analyser/helper/computebtn.py
+-rw-rw-rw-   0        0        0    21317 2024-04-20 09:50:09.000000 silicon_analyser-1.0.9/silicon_analyser/helper/fullimage.py
+-rw-rw-rw-   0        0        0     1532 2024-04-13 13:40:26.000000 silicon_analyser-1.0.9/silicon_analyser/helper/minimap.py
+-rw-rw-rw-   0        0        0     4051 2024-04-20 08:17:04.000000 silicon_analyser-1.0.9/silicon_analyser/helper/properties.py
+-rw-rw-rw-   0        0        0    23389 2024-04-20 09:11:28.000000 silicon_analyser-1.0.9/silicon_analyser/helper/tree.py
+-rw-rw-rw-   0        0        0      263 2024-04-08 17:15:10.000000 silicon_analyser-1.0.9/silicon_analyser/main.py
+-rw-rw-rw-   0        0        0     8314 2024-04-20 08:47:52.000000 silicon_analyser-1.0.9/silicon_analyser/main_window.ui
+-rw-rw-rw-   0        0        0    10537 2024-04-20 08:48:09.000000 silicon_analyser-1.0.9/silicon_analyser/mywindow.py
+-rw-rw-rw-   0        0        0      134 2024-04-07 08:11:27.000000 silicon_analyser-1.0.9/silicon_analyser/rect.py
+-rw-rw-rw-   0        0        0     2305 2024-04-16 18:10:57.000000 silicon_analyser-1.0.9/silicon_analyser/savefiles.py
+-rw-rw-rw-   0        0        0     1365 2024-04-13 14:16:41.000000 silicon_analyser-1.0.9/silicon_analyser/treeitem.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:28:20.000000 silicon_analyser-1.0.9/silicon_analyser.egg-info/
+-rw-rw-rw-   0        0        0     3334 2024-04-20 10:28:21.000000 silicon_analyser-1.0.9/silicon_analyser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1078 2024-04-20 10:28:21.000000 silicon_analyser-1.0.9/silicon_analyser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 10:28:21.000000 silicon_analyser-1.0.9/silicon_analyser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-20 10:28:21.000000 silicon_analyser-1.0.9/silicon_analyser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2024-04-20 10:28:21.000000 silicon_analyser-1.0.9/silicon_analyser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-20 10:28:21.000000 silicon_analyser-1.0.9/silicon_analyser.egg-info/top_level.txt
```

### Comparing `silicon_analyser-1.0.8/LICENSE` & `silicon_analyser-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.8/PKG-INFO` & `silicon_analyser-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silicon-analyser
-Version: 1.0.8
+Version: 1.0.9
 Summary: helps to analyse integrated circuit die images (for example from siliconpr0n.org) with the help of ai.
 Author-email: CrazyT <crazyt2019+sa@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/SiliconAnalyser
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/SiliconAnalyser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `silicon_analyser-1.0.8/README.md` & `silicon_analyser-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.8/pyproject.toml` & `silicon_analyser-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "silicon-analyser"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="CrazyT", email="crazyt2019+sa@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `silicon_analyser-1.0.8/silicon_analyser/dialogs/compute_stats.py` & `silicon_analyser-1.0.9/silicon_analyser/dialogs/compute_stats.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.8/silicon_analyser/dialogs/compute_stats.ui` & `silicon_analyser-1.0.9/silicon_analyser/dialogs/compute_stats.ui`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.8/silicon_analyser/dialogs/pixel_image.py` & `silicon_analyser-1.0.9/silicon_analyser/dialogs/pixel_image.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.8/silicon_analyser/dialogs/pixel_image.ui` & `silicon_analyser-1.0.9/silicon_analyser/dialogs/pixel_image.ui`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.8/silicon_analyser/grid.py` & `silicon_analyser-1.0.9/silicon_analyser/grid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from functools import lru_cache
+
+
 class Grid:
     _rects: dict[str,list[list[int]]]
     _rectsActive: dict[str,bool]
     def __init__(self, name, x, y, cols, rows, width, height):
         self.name = name
         self.x = x
         self.y = y
@@ -67,54 +70,84 @@
         self._rectsActive[text] = True
     
     def rectDeactive(self, text):
         self._rectsActive[text] = False
         
     def addTopRow(self):
         self.y -= int(self.height/self.rows)
+        self.height += int(self.height/self.rows)
         self.rows += 1
         for label in self._rects:
             for i in range(0,len(self._rects[label])):
                 col, row = self._rects[label][i]
                 self._rects[label][i] = [col, row+1]
+
+    def addBottomRow(self):
+        self.height += int(self.height/self.rows)
+        self.rows += 1
+        
+    def removeTopRow(self):
+        for label in self._rects:
+            delEntries = []
+            for i in range(0,len(self._rects[label])):
+                col, row = self._rects[label][i]
+                if row - 1 < 0:
+                    delEntries.append(i)
+                else:
+                    self._rects[label][i] = [col, row-1]
+            delEntries = sorted(delEntries, reverse=True)
+            for i in delEntries:
+                del self._rects[label][i]
+        self.y += int(self.height/self.rows)
+        self.height -= int(self.height/self.rows)
+        self.rows -= 1
+
+    def removeBottomRow(self):
+        self.height -= int(self.height/self.rows)
+        self.rows -= 1
     
     def setRect(self, col, row, label):
+        self.isRectSet.cache_clear()
+        self.rectLabel.cache_clear()
         #print(f"setRect {col} {row} {label}")
         r = [col, row]
         if label not in self._rects:
             self._rects[label] = []
         for lbl in self._rects.keys():
             if r in self._rects[lbl]:
                 self._rects[lbl].remove(r)
         self._rects[label].append(r)
         
     def unsetRect(self, col, row, label):
+        self.isRectSet.cache_clear()
+        self.rectLabel.cache_clear()
         print(f"unsetRect {col} {row}")
         r = [col, row]
         if r in self._rects[label]:
             self._rects[label].remove(r)
     
+    @lru_cache(maxsize=None)
     def rectLabel(self, col, row) -> str|None:
         r = [col, row]
         keys = self._rects.keys()
         for k in keys:
             if self._rectsActive[k]:
                 if r in self._rects[k]:
                     return k
     
-    def isRectSet(self, col ,row, key = None) -> bool:
+    @lru_cache(maxsize=None)
+    def isRectSet(self, col , row, key = None) -> bool:
         r = [col, row]
         if key is None:
             keys = self._rects.keys()
         else:
             keys = [key]
         for k in keys:
-            if self._rectsActive[k]:
-                if r in self._rects[k]:
-                    return True
+            if self._rectsActive[k] and r in self._rects[k]:
+                return True
         return False
 
     def getRects(self, key: str) -> list[list[int]]:
         return self._rects[key]
     
 def getAllCellRects(grid: Grid):
     cellRects = []
```

### Comparing `silicon_analyser-1.0.8/silicon_analyser/helper/abstract/abstractimage.py` & `silicon_analyser-1.0.9/silicon_analyser/helper/abstract/abstractimage.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.8/silicon_analyser/helper/abstract/abstractmywindow.py` & `silicon_analyser-1.0.9/silicon_analyser/helper/abstract/abstractmywindow.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 from PyQt5.QtWidgets import QMainWindow, QPushButton, QAction
 from PyQt5.QtGui import QStandardItem
 
 from silicon_analyser.helper.abstract.abstractimage import AbstractImage
 from silicon_analyser.helper.abstract.abstracttreehelper import AbstractTreeHelper
 
 class AbstractMyWindow(QMainWindow):
-    _actionGridAddRowTop: QAction
     _actionSaveModel: QAction
     _actionLoadModel: QAction
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionSaveAsCsv: QAction
     _actionViewAsPixelimage: QAction
     _actionExportCellsToImages: QAction
     _actionDecisionTree: QAction
     _actionNeuralNetwork: QAction
+    _actionGridAddXRowsBottom: QAction
+    _actionGridAddXRowsTop: QAction
+    _actionGridRemoveXRowsTop: QAction
+    _actionGridRemoveXRowsBottom: QAction
     autosave: bool
     def __init__(self):
         QMainWindow.__init__(self)
         
     def getManualItem(self) -> QStandardItem:
         raise NotImplementedError()
```

### Comparing `silicon_analyser-1.0.8/silicon_analyser/helper/abstract/abstracttreehelper.py` & `silicon_analyser-1.0.9/silicon_analyser/helper/abstract/abstracttreehelper.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.8/silicon_analyser/helper/addgridbtn.py` & `silicon_analyser-1.0.9/silicon_analyser/helper/addgridbtn.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.8/silicon_analyser/helper/addlabelbtn.py` & `silicon_analyser-1.0.9/silicon_analyser/helper/addlabelbtn.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.8/silicon_analyser/helper/ai.py` & `silicon_analyser-1.0.9/silicon_analyser/helper/ai.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.8/silicon_analyser/helper/computebtn.py` & `silicon_analyser-1.0.9/silicon_analyser/helper/computebtn.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.8/silicon_analyser/helper/fullimage.py` & `silicon_analyser-1.0.9/silicon_analyser/helper/fullimage.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,18 +91,20 @@
                 if ex<x:
                     x,ex = ex,x
                 if ey<y:
                     y,ey = ey,y
                 if x < evx and y < evy and ex > evx and ey > evy:
                     tevx = self._translateEventToPixel(evx)
                     tevy = self._translateEventToPixel(evy)
+                    rx = grid.x - posX
+                    ry = grid.y - posY
                     if button == Qt.MouseButton.LeftButton:
-                        grid.setRect(int((tevx - (grid.x - posX))/(grid.width/grid.cols)),int((tevy - (grid.y - posY))/(grid.height/grid.rows)), self._myWindow.getTree().selectedLabel())
+                        grid.setRect(int((tevx - rx)/(grid.getCellWidth())),int((tevy - ry)/(grid.getCellHeight())), self._myWindow.getTree().selectedLabel())
                     if button == Qt.MouseButton.RightButton:
-                        grid.unsetRect(int((tevx - (grid.x - posX))/(grid.width/grid.cols)),int((tevy - (grid.y - posY))/(grid.height/grid.rows)), self._myWindow.getTree().selectedLabel())
+                        grid.unsetRect(int((tevx - rx)/(grid.getCellWidth())),int((tevy - ry)/(grid.getCellHeight())), self._myWindow.getTree().selectedLabel())
                     if self._myWindow.autosave:
                         triggerSaveGrids()
                     
     def mousePressEvent(self, event: QMouseEvent):
         if event.button() == Qt.MouseButton.MiddleButton:
             self._moveStart = True
             self._moveStartX = event.x()
@@ -363,29 +365,32 @@
         endRow = int(min(endRow, grid.rows))
         
         return (startCol, startRow, endCol, endRow)
         
     def getGrids(self) -> dict[str,Grid]:
         return self._grids
         
-    def _drawGridOnScaledImg(self, grids, gridsActive, qp:QPainter, gridItemType:str, rectSetColor:QColor = QColor(0,255,255,40), rectSetActiveColor:QColor = QColor(0,255,255,127), rectUnsetColor:QColor = QColor(0,0,255,20)):
+    def _drawGridOnScaledImg(self, grids: dict[str,Grid], gridsActive: dict[str,bool], qp:QPainter, gridItemType:str, rectSetColor:QColor = QColor(0,255,255,40), rectSetActiveColor:QColor = QColor(0,255,255,127), rectUnsetColor:QColor = QColor(0,0,255,20)):
+        activeBrush = QBrush(rectSetActiveColor)
+        nonActiveBrush = QBrush(rectSetColor)
+        unsetBrush = QBrush(rectUnsetColor)
         posX, posY = self._myWindow.getPos()
         scale = self._myWindow.getScale()
         sposX, sposY = posX*scale, posY*scale
         for k in grids.keys():
             if gridsActive[k]:
                 grid: Grid = grids[k]
                 cellWidth = grid.getCellWidth()
                 cellHeight = grid.getCellHeight()
                 startCol, startRow, endCol, endRow = self.calcGridCellsVisibleRange(grid)
                 for row in range(startRow,endRow):
-                    if not self._drawGridOnScaledImgRow(qp, gridItemType, rectSetColor, rectSetActiveColor, rectUnsetColor, sposX, sposY, grid, cellWidth, cellHeight, startCol, endCol, row):
+                    if not self._drawGridOnScaledImgRow(qp, gridItemType, activeBrush, nonActiveBrush, unsetBrush, sposX, sposY, grid, cellWidth, cellHeight, startCol, endCol, row):
                         break
 
-    def _drawGridOnScaledImgRow(self, qp:QPainter, gridItemType:str, rectSetColor:QColor, rectSetActiveColor:QColor, rectUnsetColor:QColor, sposX:float, sposY:float, grid:Grid, cellWidth:float, cellHeight:float, startCol:int, endCol:int, row:int):
+    def _drawGridOnScaledImgRow(self, qp:QPainter, gridItemType:str, activeBrush:QBrush, nonActiveBrush:QBrush, unsetBrush:QBrush, sposX:float, sposY:float, grid:Grid, cellWidth:float, cellHeight:float, startCol:int, endCol:int, row:int):
         oy = grid.absY(row, 0)
         y = int(self._translatePixelToScaled(oy)-sposY)
         if y >= self.height():
             return False
         for col in range(startCol,endCol):
             oy = grid.absY(row, col)
             y = int(self._translatePixelToScaled(oy)-sposY)
@@ -399,20 +404,20 @@
             ey = int(self._translatePixelToScaled(ey)-sposY)
             w = ex - x
             h = ey - y
             if x>=0 and y>=0 and x<=self.width() and y<=self.height():
                 if grid.isRectSet(col,row):
                     rectLabel = grid.rectLabel(col, row)
                     if self._myWindow.getTree().isItemSelected(rectLabel, grid.name, gridItemType):
-                        brush = QBrush(rectSetActiveColor)
+                        brush = activeBrush
                     else:
-                        brush = QBrush(rectSetColor)
+                        brush = nonActiveBrush
                     qp.setBrush(brush)
                 else:
-                    brush = QBrush(rectUnsetColor)
+                    brush = unsetBrush
                     qp.setBrush(brush)
                 qp.drawRect(x,y,w,h)
         return True
 
     # TODO: maybe deprecated, not shure yet                        
     def _drawRectOnScaledImg(self, rects, rectActive, qp:QPainter):
         posX, posY = self._myWindow.getPos()
```

### Comparing `silicon_analyser-1.0.8/silicon_analyser/helper/minimap.py` & `silicon_analyser-1.0.9/silicon_analyser/helper/minimap.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.8/silicon_analyser/helper/properties.py` & `silicon_analyser-1.0.9/silicon_analyser/helper/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,18 @@
         nameCol = model.item(row,0)
         name = nameCol.data(Qt.ItemDataRole.DisplayRole)
         value = valueCol.data(Qt.ItemDataRole.DisplayRole)
         print(f"{name}: {value}")
         grid: Grid = self._myWindow.getTree().getSelectedGrid()
         if(name == "cols"):
             grid.cols = int(value)
+            grid.recalcCell()
         if(name == "rows"):
             grid.rows = int(value)
+            grid.recalcCell()
         if(name == "x"):
             grid.x = int(value)
         if(name == "y"):
             grid.y = int(value)
         if(name == "width"):
             grid.width = int(value)
             grid.recalcCell()
```

### Comparing `silicon_analyser-1.0.8/silicon_analyser/helper/tree.py` & `silicon_analyser-1.0.9/silicon_analyser/helper/tree.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from PIL import Image
 import typing
 import numpy as np
 import re
 from PyQt5.QtCore import QItemSelection, pyqtSignal, QItemSelectionModel
 from PyQt5 import QtCore
-from PyQt5.QtWidgets import QTreeView, QWidget, QAction, QFileDialog
+from PyQt5.QtWidgets import QTreeView, QWidget, QAction, QFileDialog, QInputDialog
 from PyQt5.QtGui import QStandardItem, QStandardItemModel
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
 from silicon_analyser.grid import Grid
 from silicon_analyser.helper.abstract.abstracttreehelper import AbstractTreeHelper
 from silicon_analyser.helper.abstract.abstractimage import AbstractImage
 from silicon_analyser.treeitem import TreeItem
 from silicon_analyser.grid import Grid
 from silicon_analyser.dialogs.pixel_image import PixelImageDlg
 
 class Tree(AbstractTreeHelper):
     _myWindow: AbstractMyWindow
-    _actionGridAddRowTop: QAction
+    _actionGridAddXRowsBottom: QAction
+    _actionGridAddXRowsTop: QAction
+    _actionGridRemoveXRowsBottom: QAction
+    _actionGridRemoveXRowsTop: QAction
     _actionSaveModel: QAction
     _actionLoadModel: QAction
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionSaveAsCsv: QAction
     _actionViewAsPixelimage: QAction
     _actionExportCellsToImages: QAction
@@ -29,31 +32,40 @@
 
     def __init__(self, parent: QWidget | None = ...) -> None: # type: ignore
         super().__init__(parent)
     
     def initialize(self, myWindow: AbstractMyWindow):
         self._myWindow = myWindow
         self.selectionModel().selectionChanged.connect(self.treeSelectionChanged)
-        self._actionGridAddRowTop = self._myWindow._actionGridAddRowTop
         self._actionSaveModel = self._myWindow._actionSaveModel
         self._actionLoadModel = self._myWindow._actionLoadModel
         self._actionRemoveGrid = self._myWindow._actionRemoveGrid
         self._actionRemoveLabel = self._myWindow._actionRemoveLabel
         self._actionSaveAsCsv = self._myWindow._actionSaveAsCsv
         self._actionViewAsPixelimage = self._myWindow._actionViewAsPixelimage
         self._actionExportCellsToImages = self._myWindow._actionExportCellsToImages
-        self.addAction(self._actionGridAddRowTop)
+        self._actionGridAddXRowsTop = self._myWindow._actionGridAddXRowsTop
+        self._actionGridAddXRowsBottom = self._myWindow._actionGridAddXRowsBottom
+        self._actionGridRemoveXRowsTop = self._myWindow._actionGridRemoveXRowsTop
+        self._actionGridRemoveXRowsBottom = self._myWindow._actionGridRemoveXRowsBottom
+        self.addAction(self._actionGridAddXRowsTop)
+        self.addAction(self._actionGridAddXRowsBottom)
+        self.addAction(self._actionGridRemoveXRowsTop)
+        self.addAction(self._actionGridRemoveXRowsBottom)
         self.addAction(self._actionSaveModel)
         self.addAction(self._actionLoadModel)
         self.addAction(self._actionRemoveGrid)
         self.addAction(self._actionRemoveLabel)
         self.addAction(self._actionSaveAsCsv)
         self.addAction(self._actionViewAsPixelimage)
         self.addAction(self._actionExportCellsToImages)
-        self._actionGridAddRowTop.triggered.connect(self.addTopRow)
+        self._actionGridAddXRowsTop.triggered.connect(self.addTopRows)
+        self._actionGridAddXRowsBottom.triggered.connect(self.addBottomRows)
+        self._actionGridRemoveXRowsTop.triggered.connect(self.removeTopRows)
+        self._actionGridRemoveXRowsBottom.triggered.connect(self.removeBottomRows)
         self._actionSaveModel.triggered.connect(self.saveModel)
         self._actionLoadModel.triggered.connect(self.loadModel)
         self._actionRemoveGrid.triggered.connect(self.removeGrid)
         self._actionRemoveLabel.triggered.connect(self.removeLabel)
         self._actionSaveAsCsv.triggered.connect(self.saveAsCsv)
         self._actionViewAsPixelimage.triggered.connect(self.viewAsPixelimage)
         self._actionExportCellsToImages.triggered.connect(self.exportCellsToImages)
@@ -202,37 +214,84 @@
                 return
             grid.removeRectGroup(label)
         elif(self.selectedType() == TreeItem.TYPE_MANUAL):
             myWindow.getImage().removeRectGroup(label)
         myWindow.getImage().drawImage()
         self.removeSelectedRow()
 
-    def addTopRow(self, *args, **kwargs):
-        print("addTopRow")
-        grid: Grid|None = self.getSelectedGrid()
-        if grid is None:
-            return
-        grid.addTopRow()
+    def addTopRows(self, *args, **kwargs):
+        print("addTopRows")
+        num,ok = QInputDialog.getInt(self,"How many rows to add?","enter a number",1)
+        if ok:
+            grid: Grid|None = self.getSelectedGrid()
+            if grid is None:
+                return
+            for _ in range(0,num):
+                grid.addTopRow()
+            grid.recalcCell()
+            myWindow: AbstractMyWindow = self._myWindow
+            myWindow.getImage().drawImage()
+
+    def addBottomRows(self, *args, **kwargs):
+        print("addBottomRows")
+        num,ok = QInputDialog.getInt(self,"How many rows to add?","enter a number",1)
+        if ok:
+            grid: Grid|None = self.getSelectedGrid()
+            if grid is None:
+                return
+            for _ in range(0,num):
+                grid.addBottomRow()
+            grid.recalcCell()
+            myWindow: AbstractMyWindow = self._myWindow
+            myWindow.getImage().drawImage()
+
+    def removeTopRows(self, *args, **kwargs):
+        print("addTopRows")
+        num,ok = QInputDialog.getInt(self,"How many rows to add?","enter a number",1)
+        if ok:
+            grid: Grid|None = self.getSelectedGrid()
+            if grid is None:
+                return
+            for _ in range(0,num):
+                grid.removeTopRow()
+            grid.recalcCell()
+            myWindow: AbstractMyWindow = self._myWindow
+            myWindow.getImage().drawImage()
+
+    def removeBottomRows(self, *args, **kwargs):
+        print("addBottomRows")
+        num,ok = QInputDialog.getInt(self,"How many rows to add?","enter a number",1)
+        if ok:
+            grid: Grid|None = self.getSelectedGrid()
+            if grid is None:
+                return
+            for _ in range(0,num):
+                grid.removeBottomRow()
+            grid.recalcCell()
+            myWindow: AbstractMyWindow = self._myWindow
+            myWindow.getImage().drawImage()
         
     def treeSelectionChanged(self, selection: QItemSelection):
         print("treeSelectionChanged")
         myWindow: AbstractMyWindow = self._myWindow
         myWindow.reloadPropertyWindow(selection)
         tree = self
         selectedType = tree.selectedType()
         if((selectedType == TreeItem.TYPE_GRID_ITEM) or (selectedType == TreeItem.TYPE_GRID)):
-            self._actionGridAddRowTop.setVisible(True)
+            self._actionGridAddXRowsTop.setVisible(True)
+            self._actionGridAddXRowsBottom.setVisible(True)
             grid: Grid|None = self.getSelectedGrid()
             if grid is None:
                 return
             if myWindow.hasModel(grid.name):
                 self._actionSaveModel.setVisible(True)
             self._actionLoadModel.setVisible(True)
         else:
-            self._actionGridAddRowTop.setVisible(False)
+            self._actionGridAddXRowsTop.setVisible(False)
+            self._actionGridAddXRowsBottom.setVisible(False)
             self._actionSaveModel.setVisible(False)
             self._actionLoadModel.setVisible(False)
         if(selectedType == TreeItem.TYPE_GRID):
             self._actionRemoveGrid.setVisible(True)
             self._actionSaveAsCsv.setVisible(True)
             self._actionExportCellsToImages.setVisible(True)
         else:
```

### Comparing `silicon_analyser-1.0.8/silicon_analyser/main_window.ui` & `silicon_analyser-1.0.9/silicon_analyser/main_window.ui`

 * *Files 7% similar despite different names*

#### Comparing `silicon_analyser-1.0.8/silicon_analyser/main_window.ui` & `silicon_analyser-1.0.9/silicon_analyser/main_window.ui`

```diff
@@ -156,22 +156,14 @@
         </property>
         <addaction name="_actionDecisionTree"/>
         <addaction name="_actionNeuralNetwork"/>
       </widget>
       <addaction name="menuInfo"/>
       <addaction name="menuComputation_method"/>
     </widget>
-    <action name="_actionGridAddRowTop">
-      <property name="text">
-        <string>Add row to top</string>
-      </property>
-      <property name="toolTip">
-        <string>Add row to top</string>
-      </property>
-    </action>
     <action name="_actionSaveModel">
       <property name="text">
         <string>Save computation model</string>
       </property>
     </action>
     <action name="_actionLoadModel">
       <property name="text">
@@ -243,14 +235,43 @@
       <property name="checked">
         <bool>true</bool>
       </property>
       <property name="text">
         <string>Neural network</string>
       </property>
     </action>
+    <action name="_actionGridAddXRowsBottom">
+      <property name="text">
+        <string>Add X rows to bottom</string>
+      </property>
+    </action>
+    <action name="_actionGridAddXRowsTop">
+      <property name="text">
+        <string>Add X rows to top</string>
+      </property>
+      <property name="toolTip">
+        <string>Add X rows to top</string>
+      </property>
+    </action>
+    <action name="_actionGridRemoveXRowsBottom">
+      <property name="text">
+        <string>Remove X rows on bottom</string>
+      </property>
+      <property name="toolTip">
+        <string>Remove X rows on bottom</string>
+      </property>
+    </action>
+    <action name="_actionGridRemoveXRowsTop">
+      <property name="text">
+        <string>Remove X rows on top</string>
+      </property>
+      <property name="toolTip">
+        <string>Remove X rows on top</string>
+      </property>
+    </action>
   </widget>
   <customwidgets>
     <customwidget>
       <class>ComputeBtn</class>
       <extends>QPushButton</extends>
       <header>silicon_analyser.helper.computebtn</header>
     </customwidget>
```

### Comparing `silicon_analyser-1.0.8/silicon_analyser/mywindow.py` & `silicon_analyser-1.0.9/silicon_analyser/mywindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,18 @@
     _addLabelBtn: AddLabelBtn
     _computeBtn: ComputeBtn
     _addGridBtn: AddGridBtn
     _statusBar: QStatusBar
     _minimap: MiniMap
     _image: FullImage
     _models: dict[str,object]
-    _actionGridAddRowTop: QAction
+    _actionGridAddXRowsTop: QAction
+    _actionGridAddXRowsBottom: QAction
+    _actionGridRemoveXRowsTop: QAction
+    _actionGridRemoveXRowsBottom: QAction
     _actionSaveModel: QAction
     _actionLoadModel: QAction
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionMade_by_TheCrazyT: QAction
     _actionUrl: QAction
     _actionSaveAsCsv: QAction
```

### Comparing `silicon_analyser-1.0.8/silicon_analyser/savefiles.py` & `silicon_analyser-1.0.9/silicon_analyser/savefiles.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.8/silicon_analyser/treeitem.py` & `silicon_analyser-1.0.9/silicon_analyser/treeitem.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.8/silicon_analyser.egg-info/PKG-INFO` & `silicon_analyser-1.0.9/silicon_analyser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silicon-analyser
-Version: 1.0.8
+Version: 1.0.9
 Summary: helps to analyse integrated circuit die images (for example from siliconpr0n.org) with the help of ai.
 Author-email: CrazyT <crazyt2019+sa@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/SiliconAnalyser
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/SiliconAnalyser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `silicon_analyser-1.0.8/silicon_analyser.egg-info/SOURCES.txt` & `silicon_analyser-1.0.9/silicon_analyser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

