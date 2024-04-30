# Comparing `tmp/pyqtgraph_ext-1.0.2.tar.gz` & `tmp/pyqtgraph_ext-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqtgraph_ext-1.0.2.tar", last modified: Thu Jan 11 16:23:48 2024, max compression
+gzip compressed data, was "pyqtgraph_ext-1.2.0.tar", last modified: Tue Apr 30 21:46:36 2024, max compression
```

## Comparing `pyqtgraph_ext-1.0.2.tar` & `pyqtgraph_ext-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     1077 2023-12-29 18:16:11.357234 pyqtgraph_ext-1.0.2/LICENSE
--rw-r--r--   0        0        0      824 2024-01-10 15:56:04.639598 pyqtgraph_ext-1.0.2/README.md
--rw-r--r--   0        0        0     1202 2024-01-11 16:23:48.586046 pyqtgraph_ext-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     6769 2024-01-11 05:01:30.451307 pyqtgraph_ext-1.0.2/src/pyqtgraph_ext/PyQtGraphAxisRegion.py
--rw-r--r--   0        0        0     1425 2024-01-11 04:23:48.406206 pyqtgraph_ext-1.0.2/src/pyqtgraph_ext/PyQtGraphFigure.py
--rw-r--r--   0        0        0      880 2024-01-11 04:20:28.741224 pyqtgraph_ext-1.0.2/src/pyqtgraph_ext/PyQtGraphPlot.py
--rw-r--r--   0        0        0     2073 2024-01-11 04:27:24.311567 pyqtgraph_ext-1.0.2/src/pyqtgraph_ext/PyQtGraphPlotGrid.py
--rw-r--r--   0        0        0     6570 2024-01-11 04:45:11.680611 pyqtgraph_ext-1.0.2/src/pyqtgraph_ext/PyQtGraphView.py
--rw-r--r--   0        0        0     6409 2024-01-11 04:24:02.958184 pyqtgraph_ext-1.0.2/src/pyqtgraph_ext/PyQtGraphXYData.py
--rw-r--r--   0        0        0      409 2024-01-11 04:35:53.811219 pyqtgraph_ext-1.0.2/src/pyqtgraph_ext/__init__.py
--rw-r--r--   0        0        0        0 2023-12-29 18:16:11.359389 pyqtgraph_ext-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1922 1970-01-01 00:00:00.000000 pyqtgraph_ext-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-01-29 19:12:56.810546 pyqtgraph_ext-1.2.0/LICENSE
+-rw-r--r--   0        0        0      760 2024-04-24 22:10:53.577243 pyqtgraph_ext-1.2.0/README.md
+-rw-r--r--   0        0        0     1202 2024-04-30 21:46:36.453400 pyqtgraph_ext-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9304 2024-04-30 14:22:23.759075 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/AxisRegion.py
+-rw-r--r--   0        0        0     6764 2024-04-30 14:22:23.759456 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/AxisRegionTreeItem.py
+-rw-r--r--   0        0        0     2579 2024-04-30 14:22:23.759796 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/AxisRegionTreeModel.py
+-rw-r--r--   0        0        0    17198 2024-04-30 14:22:23.760185 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/AxisRegionTreeView.py
+-rw-r--r--   0        0        0     1577 2024-02-19 16:35:28.155322 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/Figure.py
+-rw-r--r--   0        0        0     6567 2024-04-26 20:37:41.001643 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/Graph.py
+-rw-r--r--   0        0        0      830 2024-04-26 15:12:20.979202 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/Plot.py
+-rw-r--r--   0        0        0     6117 2024-04-24 22:09:55.723207 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/PlotGrid.py
+-rw-r--r--   0        0        0     6555 2024-04-24 22:10:53.578129 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/View.py
+-rw-r--r--   0        0        0      573 2024-04-30 14:22:23.760679 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-29 19:12:56.812918 pyqtgraph_ext-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1858 1970-01-01 00:00:00.000000 pyqtgraph_ext-1.2.0/PKG-INFO
```

### Comparing `pyqtgraph_ext-1.0.2/LICENSE` & `pyqtgraph_ext-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtgraph_ext-1.0.2/pyproject.toml` & `pyqtgraph_ext-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,22 +26,22 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
 ]
-version = "1.0.2"
+version = "1.2.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
-homepage = "https://github.com/marcel-goldschen-ohm/PyQtGraph-ext"
-repository = "https://github.com/marcel-goldschen-ohm/PyQtGraph-ext"
+homepage = "https://github.com/marcel-goldschen-ohm/pyqtgraph-ext"
+repository = "https://github.com/marcel-goldschen-ohm/pyqtgraph-ext"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `pyqtgraph_ext-1.0.2/src/pyqtgraph_ext/PyQtGraphFigure.py` & `pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/Figure.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,22 +27,24 @@
             # See https://bugreports.qt.io/browse/QTBUG-103935
             for view in self.scene().views():
                 view.viewport().setAttribute(Qt.WidgetAttribute.WA_AcceptTouchEvents, False)
 
 
 def test_live():
     import numpy as np
-    from pyqtgraph_ext import XYData
+    from pyqtgraph_ext import Graph
     app = QApplication()
     plot = Figure()
+    view = plot.getViewBox()
     for i in range(3):
-        line = XYData(y=np.random.randn(10), lineWidth=2)
+        line = Graph(y=np.random.randn(10), pen=pg.mkPen(color=view.nextColor(), width=3))
         plot.addItem(line)
-    line = XYData(y=np.random.randn(10))
-    plot.addItem(line)
     plot.setWindowTitle('pyqtgraph-tools')
     plot.show()
+    # from pyqtgraph_ext import XAxisRegion
+    # view.startDrawingItemsOfType(XAxisRegion)
+    # QTimer.singleShot(1000, lambda: view.stopDrawingItems())
     app.exec()
 
 
 if __name__ == '__main__':
     test_live()
```

### Comparing `pyqtgraph_ext-1.0.2/src/pyqtgraph_ext/PyQtGraphView.py` & `pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/View.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 
 from __future__ import annotations
 from qtpy.QtCore import *
 from qtpy.QtGui import *
 from qtpy.QtWidgets import *
 import pyqtgraph as pg
-from pyqtgraph_ext import AxisRegion, XAxisRegion, YAxisRegion, XYData
+from pyqtgraph_ext import XAxisRegion, YAxisRegion
 
 
 class View(pg.ViewBox):
     """ ViewBox with context menu for drawing ROIs and events. """
 
     sigStartedDrawingItems = Signal()
     sigItemAdded = Signal(QGraphicsObject)  # emits the newly added QGraphicsObject item
@@ -53,18 +53,18 @@
     
     def colorIndex(self):
         return self._colorIndex
     
     def setColorIndex(self, colorIndex):
         self._colorIndex = colorIndex
     
-    def addItem(self, item):
-        if isinstance(item, XYData):
-            item.setColor(self.nextColor())
-        pg.ViewBox.addItem(self, item)
+    # def addItem(self, item):
+    #     if isinstance(item, Graph):
+    #         item.setColor(self.nextColor())
+    #     pg.ViewBox.addItem(self, item)
     
     # def initContextMenu(self):
     #     self._ROIsMenu = QMenu("ROIs")
     #     self._ROIsMenu.addAction('Draw X-Axis ROIs (right-click to stop)', lambda: self.startDrawingItemsOfType(XAxisRegion))
     #     # self._ROIsMenu.addAction('Draw Y-Axis ROIs (right-click to stop)', lambda: self.startDrawingItemsOfType(YAxisRegionItem))
     #     self._ROIsMenu.addSeparator()
     #     self._ROIsMenu.addAction("Show All", lambda: self.setVisibilityForItemsOfType(AxisRegion, True))
@@ -153,19 +153,19 @@
         self._drawingItemsOfType = None
         self._itemBeingDrawn = None
         self.sigFinishedDrawingItems.emit()
 
 
 def test_live():
     import numpy as np
-    from pyqtgraph_ext import Figure, XYData
+    from pyqtgraph_ext import Figure, Graph
     app = QApplication()
     axes = View()
     plot = Figure(viewBox=axes)
-    line = XYData(y=np.random.randn(1000))
+    line = Graph(y=np.random.randn(1000))
     plot.addItem(line)
     plot.setWindowTitle('pyqtgraph-tools')
     plot.show()
     app.exec()
 
 
 if __name__ == '__main__':
```

### Comparing `pyqtgraph_ext-1.0.2/src/pyqtgraph_ext/PyQtGraphXYData.py` & `pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/Graph.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 """
 
 from __future__ import annotations
 from qtpy.QtCore import *
 from qtpy.QtGui import *
 from qtpy.QtWidgets import *
 import pyqtgraph as pg
-from pyqt_ext import XYDataStyleDict, editXYDataStyle
+from pyqt_ext.utils import toQColor
+from pyqt_ext.graph import GraphStyle, editGraphStyle
 
 
-class XYData(pg.PlotDataItem):
+class Graph(pg.PlotDataItem):
     """ PlotDataItem with custom context menu and style dialog. """
 
+    sigNameChanged = Signal(str)
+
     def __init__(self, *args, **kwargs):
         # default style is first MATLAB line color
         if 'pen' not in kwargs:
             kwargs['pen'] = pg.mkPen(QColor(0, 114, 189), width=1)
         if 'symbolPen' not in kwargs:
             kwargs['symbolPen'] = pg.mkPen(QColor(0, 114, 189), width=1)
         if 'symbolBrush' not in kwargs:
@@ -86,96 +89,93 @@
         return self.opts.get('Name', None)
     
     def setName(self, name):
         if name is None:
             del self.opts['Name']
         else:
             self.opts['Name'] = name
+        self.sigNameChanged.emit(self.name())
     
-    def styleDict(self) -> XYDataStyleDict:
-        style = XYDataStyleDict()
+    def graphStyle(self) -> GraphStyle:
+        style = GraphStyle()
 
         pen = pg.mkPen(self.opts['pen'])
         symbolPen = pg.mkPen(self.opts['symbolPen'])
         symbolBrush = pg.mkBrush(self.opts['symbolBrush'])
 
         style.setColor(pen.color())
         style.setLineStyle(pen.style())
         style.setLineWidth(pen.widthF())
         style.setMarker(self.opts.get('symbol', 'none'))
         style.setMarkerSize(self.opts.get('symbolSize', 10))
+        style.setMarkerEdgeStyle(symbolPen.style())
         style.setMarkerEdgeWidth(symbolPen.widthF())
-        markerEdgeColor = symbolPen.color()
-        if markerEdgeColor == pen.color():
-            markerEdgeColor = 'auto'
-        style.setMarkerEdgeColor(markerEdgeColor)
-        markerFaceColor = symbolBrush.color()
-        if markerFaceColor.alpha() == 0:
-            markerFaceColor = 'auto'
-        style.setMarkerFaceColor(markerFaceColor)
+        if symbolPen.color() != pen.color():
+            style.setMarkerEdgeColor(symbolPen.color())
+        if symbolBrush.color() != symbolPen.color():
+            style.setMarkerFaceColor(symbolBrush.color())
 
         return style
     
-    def setStyleDict(self, style: XYDataStyleDict, colorIndex=None):
+    def setGraphStyle(self, style: GraphStyle, colorIndex: int | None = None) -> int | None:
         # color
-        color: str = style.color()
-        if color == 'auto':
+        color = style.color()
+        if color is None:
             if colorIndex is not None:
                 try:
                     axes = self.getViewBox()
-                    colormap = axes._colormap
+                    colormap = axes.colormap()
                     color = colormap[colorIndex % len(colormap)]
+                    color = toQColor(color)
                     colorIndex += 1
                 except:
-                    old_style = self.styleDict()
-                    color = old_style.color()
+                    color = toQColor(self.graphStyle().color())
             else:
-                old_style = self.styleDict()
-                color = old_style.color()
-        color: QColor = XYDataStyleDict.toQColor(color)
+                color = toQColor(self.graphStyle().color())
+        else:
+            color = toQColor(color)
 
         # line
-        lineStyle: Qt.PenStyle = style.lineQtPenStyle()
+        lineStyle: str = style.lineStyle()
+        linePenStyle: Qt.PenStyle = GraphStyle.penstyles[GraphStyle.linestyles.index(lineStyle)]
         lineWidth = style.lineWidth()
-        linePen = pg.mkPen(color=color, width=lineWidth, style=lineStyle)
+        linePen = pg.mkPen(color=color, width=lineWidth, style=linePenStyle)
         self.setPen(linePen)
 
         # marker
         marker = style.marker()
         if marker == 'none':
             marker = None
         self.setSymbol(marker)
         
         markerSize = style.markerSize()
         self.setSymbolSize(markerSize)
 
+        markerEdgeStyle = style.markerEdgeStyle()
+        markerEdgePenStyle: Qt.PenStyle = GraphStyle.penstyles[GraphStyle.linestyles.index(markerEdgeStyle)]
         markerEdgeWidth = style.markerEdgeWidth()
         markerEdgeColor = style.markerEdgeColor()
-        if markerEdgeColor == 'auto':
+        if markerEdgeColor is None:
             markerEdgeColor = color
         else:
-            markerEdgeColor = style.markerEdgeQColor()
-        symbolPen = pg.mkPen(color=markerEdgeColor, width=markerEdgeWidth)
+            markerEdgeColor = toQColor(markerEdgeColor)
+        symbolPen = pg.mkPen(color=markerEdgeColor, width=markerEdgeWidth, style=markerEdgePenStyle)
         self.setSymbolPen(symbolPen)
 
         markerFaceColor = style.markerFaceColor()
-        if markerFaceColor == 'auto':
+        if markerFaceColor is None:
             markerFaceColor = markerEdgeColor
-            markerFaceColor.setAlpha(0)
         else:
-            markerFaceColor = style.markerFaceQColor()
+            markerFaceColor = toQColor(markerFaceColor)
         self.setSymbolBrush(markerFaceColor)
         
         return colorIndex
     
     def styleDialog(self):
         name = self.name()
         if name is None:
             name = self.__class__.__name__
-        style: XYDataStyleDict | None = editXYDataStyle(self.styleDict(), parent = self.getViewBox().getViewWidget(), title = name)
-        if style is not None:
-            self.setStyleDict(style)
-
-    def setColor(self, color: QColor):
-        style: XYDataStyleDict = self.styleDict()
-        style.setColor(color)
-        self.setStyleDict(style)
+        old_style: GraphStyle = self.graphStyle()
+        new_style: GraphStyle | None = editGraphStyle(old_style, parent = self.getViewBox().getViewWidget(), title = name)
+        if new_style is None:
+            return
+        self.setGraphStyle(new_style)
```

