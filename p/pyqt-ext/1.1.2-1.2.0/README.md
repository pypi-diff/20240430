# Comparing `tmp/pyqt_ext-1.1.2.tar.gz` & `tmp/pyqt_ext-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt_ext-1.1.2.tar", last modified: Thu Jan 11 16:23:26 2024, max compression
+gzip compressed data, was "pyqt_ext-1.2.0.tar", last modified: Tue Apr 30 21:46:12 2024, max compression
```

## Comparing `pyqt_ext-1.1.2.tar` & `pyqt_ext-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,22 @@
--rw-r--r--   0        0        0     1077 2023-12-29 18:05:58.186297 pyqt_ext-1.1.2/LICENSE
--rw-r--r--   0        0        0     1071 2023-12-29 18:05:58.186597 pyqt_ext-1.1.2/README.md
--rw-r--r--   0        0        0     1123 2024-01-11 16:23:26.710411 pyqt_ext-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     5927 2024-01-11 15:25:47.320130 pyqt_ext-1.1.2/src/pyqt_ext/PyQtAbstractTreeItem.py
--rw-r--r--   0        0        0     8694 2023-12-29 18:05:58.187881 pyqt_ext-1.1.2/src/pyqt_ext/PyQtAbstractTreeModel.py
--rw-r--r--   0        0        0     4916 2024-01-10 15:55:55.085904 pyqt_ext-1.1.2/src/pyqt_ext/PyQtAbstractTreeView.py
--rw-r--r--   0        0        0     4698 2024-01-11 15:24:57.952367 pyqt_ext-1.1.2/src/pyqt_ext/PyQtChart.py
--rw-r--r--   0        0        0     1349 2024-01-10 15:55:55.086619 pyqt_ext-1.1.2/src/pyqt_ext/PyQtColorButton.py
--rw-r--r--   0        0        0     4479 2023-12-29 18:05:58.188474 pyqt_ext-1.1.2/src/pyqt_ext/PyQtKeyValueTreeItem.py
--rw-r--r--   0        0        0     2395 2024-01-10 15:55:55.087013 pyqt_ext-1.1.2/src/pyqt_ext/PyQtKeyValueTreeModel.py
--rw-r--r--   0        0        0     3889 2023-12-29 18:05:58.188956 pyqt_ext-1.1.2/src/pyqt_ext/PyQtKeyValueTreeView.py
--rw-r--r--   0        0        0    14367 2024-01-11 14:48:06.075458 pyqt_ext-1.1.2/src/pyqt_ext/PyQtMultiValueSpinBox.py
--rw-r--r--   0        0        0    12445 2023-12-29 18:05:58.189551 pyqt_ext-1.1.2/src/pyqt_ext/PyQtXYDataStyle.py
--rw-r--r--   0        0        0      557 2024-01-11 16:16:02.314967 pyqt_ext-1.1.2/src/pyqt_ext/__init__.py
--rw-r--r--   0        0        0        0 2023-12-29 18:05:58.189891 pyqt_ext-1.1.2/tests/__init__.py
--rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 pyqt_ext-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-01-29 19:11:38.968151 pyqt_ext-1.2.0/LICENSE
+-rw-r--r--   0        0        0      576 2024-03-01 20:13:41.411647 pyqt_ext-1.2.0/README.md
+-rw-r--r--   0        0        0     1123 2024-04-30 21:46:12.129666 pyqt_ext-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-26 18:05:49.614382 pyqt_ext-1.2.0/src/pyqt_ext/__init__.py
+-rw-r--r--   0        0        0    15661 2024-04-30 21:40:30.459705 pyqt_ext-1.2.0/src/pyqt_ext/graph/GraphStyle.py
+-rw-r--r--   0        0        0       81 2024-02-26 18:05:49.615491 pyqt_ext-1.2.0/src/pyqt_ext/graph/__init__.py
+-rw-r--r--   0        0        0     4933 2024-02-26 18:05:49.616028 pyqt_ext-1.2.0/src/pyqt_ext/tmp/Chart.py
+-rw-r--r--   0        0        0    14436 2024-04-23 20:40:53.301852 pyqt_ext-1.2.0/src/pyqt_ext/tree/AbstractTreeItem.py
+-rw-r--r--   0        0        0    14629 2024-04-22 17:42:52.732350 pyqt_ext-1.2.0/src/pyqt_ext/tree/AbstractTreeModel.py
+-rw-r--r--   0        0        0     6553 2024-03-04 20:57:48.587337 pyqt_ext-1.2.0/src/pyqt_ext/tree/KeyValueTreeItem.py
+-rw-r--r--   0        0        0     2896 2024-02-26 18:33:33.713144 pyqt_ext-1.2.0/src/pyqt_ext/tree/KeyValueTreeModel.py
+-rw-r--r--   0        0        0     3501 2024-03-04 20:57:48.587786 pyqt_ext-1.2.0/src/pyqt_ext/tree/KeyValueTreeView.py
+-rw-r--r--   0        0        0    11058 2024-04-30 14:22:19.549036 pyqt_ext-1.2.0/src/pyqt_ext/tree/TreeView.py
+-rw-r--r--   0        0        0      392 2024-02-26 18:05:49.619082 pyqt_ext-1.2.0/src/pyqt_ext/tree/__init__.py
+-rw-r--r--   0        0        0     1624 2024-04-25 15:58:28.549088 pyqt_ext-1.2.0/src/pyqt_ext/utils/Color.py
+-rw-r--r--   0        0        0       64 2024-02-26 18:05:49.619812 pyqt_ext-1.2.0/src/pyqt_ext/utils/__init__.py
+-rw-r--r--   0        0        0     5452 2024-04-23 18:11:10.293878 pyqt_ext-1.2.0/src/pyqt_ext/widgets/CollapsibleSection.py
+-rw-r--r--   0        0        0     2415 2024-02-29 22:56:53.609934 pyqt_ext-1.2.0/src/pyqt_ext/widgets/ColorButton.py
+-rw-r--r--   0        0        0    11883 2024-04-30 18:28:21.131390 pyqt_ext-1.2.0/src/pyqt_ext/widgets/MultiValueSpinBox.py
+-rw-r--r--   0        0        0      184 2024-03-05 15:06:04.507342 pyqt_ext-1.2.0/src/pyqt_ext/widgets/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-29 19:11:38.971696 pyqt_ext-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 pyqt_ext-1.2.0/PKG-INFO
```

### Comparing `pyqt_ext-1.1.2/LICENSE` & `pyqt_ext-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.1.2/pyproject.toml` & `pyqt_ext-1.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -23,22 +23,22 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
 ]
-version = "1.1.2"
+version = "1.2.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
-homepage = "https://github.com/marcel-goldschen-ohm/PyQt-ext"
-repository = "https://github.com/marcel-goldschen-ohm/PyQt-ext"
+homepage = "https://github.com/marcel-goldschen-ohm/pyqt-ext"
+repository = "https://github.com/marcel-goldschen-ohm/pyqt-ext"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `pyqt_ext-1.1.2/src/pyqt_ext/PyQtAbstractTreeItem.py` & `pyqt_ext-1.2.0/src/pyqt_ext/tree/KeyValueTreeItem.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,180 +1,217 @@
-""" Base class for a tree of items to be used as a data interface with QAbstractItemModel.
+""" Data interface for a tree of key-value pairs.
 """
 
 from __future__ import annotations
+from pyqt_ext.tree import AbstractTreeItem
 
-from qtpy.QtCore import *
-from qtpy.QtGui import *
-from qtpy.QtWidgets import *
 
-
-class AbstractTreeItem():
-    """ Base class for a tree of items to be used as a data interface with QAbstractItemModel.
-    
-    !!! This only implements the tree structure. You must define any data variables in a derived class.
-
-    In a class derived from this base class:
-        1. Add attributes to store/interface with your data.
-        2. Reimplement data(), set_data(), and __repr__() methods.
-    """
+class KeyValueTreeItem(AbstractTreeItem):
     
-    def __init__(self, parent: AbstractTreeItem | None = None):
-        self.parent: AbstractTreeItem = parent
-        self.children: list[AbstractTreeItem] = []
-    
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        next_item: AbstractTreeItem = self.next_depth_first()
-        if next_item is None:
-            raise StopIteration
-        return next_item
+    def __init__(self, key: str | None, value, parent: KeyValueTreeItem | None = None) -> None:
+        self._key: str | None = key
+        self._value = value
+        AbstractTreeItem.__init__(self, parent=parent)
+
+        # recursively build subtree if value is itself a container with key,value access
+        if isinstance(value, dict):
+            for key in value:
+                KeyValueTreeItem(key, value[key], parent=self)
+        elif isinstance(value, list):
+            for i in range(len(value)):
+                # list keys are not explicitly set, they will default to the list index
+                KeyValueTreeItem(None, value[i], parent=self)
     
-    # !!! not implemented
     def __repr__(self):
-        # raise NotImplementedError
-        return str(id(self))  # for debugging
-    
-    def row(self) -> int:
-        return self.sibling_index()
-    
-    def root(self) -> AbstractTreeItem:
-        item: AbstractTreeItem = self
-        while item.parent is not None:
-            item = item.parent
-        return item
-    
-    def first_child(self) -> AbstractTreeItem | None:
-        if self.children:
-            return self.children[0]
-
-    def last_child(self) -> AbstractTreeItem | None:
-        if self.children:
-            return self.children[-1]
-
-    def first_sibling(self) -> AbstractTreeItem:
-        if self.parent is not None:
-            return self.parent.first_child()
-        return self
-
-    def last_sibling(self) -> AbstractTreeItem:
+        if self.is_container():
+            return f'{self.key}'
+        return f'{self.key}: {self.value}'
+    
+    @property
+    def key(self) -> str | int:
+        # if parent is a list, the key is the index of this item in the list
         if self.parent is not None:
-            return self.parent.last_child()
-        return self
-
-    def siblings(self) -> list[AbstractTreeItem]:
+            if self.parent.is_list():
+                return self.sibling_index
+        # otherwise, return the local key
+        return self._key
+    
+    @key.setter
+    def key(self, key: str) -> None:
+        # update parent dict
         if self.parent is not None:
-            return self.parent.children
-        return [self]
-    
-    def next_sibling(self) -> AbstractTreeItem | None:
-        siblings: list[AbstractTreeItem] = self.siblings()
-        if siblings:
-            i: int = siblings.index(self)
-            if i+1 < len(siblings):
-                return siblings[i+1]
-
-    def prev_sibling(self) -> AbstractTreeItem | None:
-        siblings: list[AbstractTreeItem] = self.siblings()
-        if siblings:
-            i: int = siblings.index(self)
-            if i-1 >= 0:
-                return siblings[i-1]
-
-    def last_depth_first(self) -> AbstractTreeItem:
-        item: AbstractTreeItem = self
-        while item.children:
-            item = item.last_child()
-        return item
-
-    def next_depth_first(self) -> AbstractTreeItem | None:
-        if self.children:
-            return self.first_child()
-        next_sibling: AbstractTreeItem = self.next_sibling()
-        if next_sibling is not None:
-            return next_sibling
-        item: AbstractTreeItem = self.parent
-        while item is not None:
-            next_sibling: AbstractTreeItem = item.next_sibling()
-            if next_sibling is not None:
-                return next_sibling
-            item = item.parent
-
-    def prev_depth_first(self) -> AbstractTreeItem | None:
-        prev_sibling: AbstractTreeItem = self.prev_sibling()
-        if prev_sibling is not None:
-            return prev_sibling.last_depth_first()
+            if self.parent.is_dict():
+                # only allow string keys for dict
+                key = str(key)
+                # remove old key from parent dict
+                if (self.key is not None) and (self.key in self.parent.value):
+                    self.parent.value.pop(self.key)
+                # make sure key is unique
+                if key in self.parent.value:
+                    key = unique_name(key, list(self.parent.value.keys()))
+                # add new key to parent dict
+                self.parent.value[key] = self.value
+            elif self.parent.is_list():
+                # cannot edit list index
+                return
+        # update local key
+        self._key = key
+    
+    @property
+    def value(self):
+        return self._value
+    
+    @value.setter
+    def value(self, value) -> None:
+        # update parent dict or list
         if self.parent is not None:
-            return self.parent
+            if self.parent.is_dict() or self.parent.is_list():
+                self.parent.value[self.key] = value
+        # update local value
+        self._value = value
+    
+    @AbstractTreeItem.parent.setter
+    def parent(self, parent: KeyValueTreeItem | None) -> None:
+        if self.parent is parent:
+            return
+        if (parent is not None) and (not parent.is_container()):
+            raise ValueError('Parent must be a container (dict or list).')
+        old_parent: KeyValueTreeItem | None = self.parent
+
+        # update item tree
+        AbstractTreeItem.parent.fset(self, parent)
+
+        # remove value from old parent container
+        if old_parent is not None:
+            if old_parent.is_dict():
+                for key, value in old_parent.value.items():
+                    if (value is self.value) or (value == self.value):
+                        old_parent.value.pop(key)
+                        break
+            elif old_parent.is_list():
+                if self.value in old_parent.value:
+                    old_parent.value.remove(self.value)
+        
+        # insert value into new parent container
+        if parent is not None:
+            if parent.is_dict():
+                if self.value not in parent.value.values():
+                    # resetting key will insert value into parent dict
+                    self.key = str(self.key)
+                    # if key in parent.value:
+                    #     key = unique_name(key, list(parent.value.keys()))
+                    # self._key = key
+                    # parent.value[self.key] = self.value
+            elif parent.is_list():
+                if self.value not in parent.value:
+                    parent.value.append(self.value)
+    
+    @AbstractTreeItem.name.getter
+    def name(self) -> str:
+        return str(self.key)
+    
+    def is_dict(self):
+        return isinstance(self.value, dict)
     
-    def sibling_index(self) -> int:
-        if self.parent is None:
-            return 0
-        return self.parent.children.index(self)
-    
-    def depth(self) -> int:
-        depth: int = 0
-        item: AbstractTreeItem = self
-        while item.parent is not None:
-            depth += 1
-            item = item.parent
-        return depth
-    
-    def subtree_max_depth(self) -> int:
-        root_depth: int = self.depth()
-        max_depth: int = 0
-        item: AbstractTreeItem = self.next_depth_first()
-        while item is not None:
-            depth: int = item.depth()
-            if depth - root_depth > max_depth:
-                max_depth = depth - root_depth
-            item = item.next_depth_first()
-        return max_depth
-    
-    def dump(self, indent: int = 0):
-        print(' ' * indent + self.__repr__())
-        for child in self.children:
-            child.dump(indent + 4)
-    
-    # !!! not implemented
-    def data(self, column: int):
-        # raise NotImplementedError
-        return self.__repr__()  # for debugging
+    def is_list(self):
+        return isinstance(self.value, list)
     
-    # !!! not implemented
-    def set_data(self, column: int, value) -> bool:
-        # raise NotImplementedError
-        return False
+    def is_container(self):
+        return self.is_dict() or self.is_list()
     
-    def remove_children(self, position: int, count: int) -> bool:
-        if position < 0 or position + count > len(self.children):
+    def insert_child(self, index: int, item: KeyValueTreeItem) -> bool:
+        if not AbstractTreeItem.insert_child(self, index, item):
             return False
-        for row in range(count):
-            item: AbstractTreeItem = self.children.pop(position)
-            item.parent = None
+        if self.is_list():
+            pos = self.value.index(item.value)
+            if pos != index:
+                self.value.insert(index, self.value.pop(pos))
         return True
     
-    def insert_children(self, position: int, items: list[AbstractTreeItem]) -> bool:
-        if position < 0 or position > len(self.children):
-            return False
-        for i, item in enumerate(items):
-            item.parent = self
-            self.children.insert(position + i, item)
-        return True
+    def get_data(self, column: int):
+        if column == 0:
+            return self.key
+        elif column == 1:
+            if self.is_container():
+                return
+            return self.value
     
-    def append_children(self, items: list[AbstractTreeItem]) -> bool:
-        position: int = len(self.children)
-        return self.insert_children(position, items)
+    def set_data(self, column: int, value) -> bool:
+        if column == 0:
+            self.key = value
+            return True
+        elif column == 1:
+            if self.is_container():
+                return False
+            self.value = value
+            return True
+        return False
+
+
+def unique_name(name: str, names: list[str]) -> str:
+    if name not in names:
+        return name
+    i: int = 1
+    uname = f'{name}_{i}'
+    while uname in names:
+        i += 1
+        uname = f'{name}_{i}'
+    return uname
 
 
 def test_tree():
-    root = AbstractTreeItem()
-    root.insert_children(0, [AbstractTreeItem(), AbstractTreeItem(), AbstractTreeItem()])
-    root.children[-1].insert_children(0, [AbstractTreeItem(), AbstractTreeItem(), AbstractTreeItem()])
-    root.children[-1].children[0].insert_children(0, [AbstractTreeItem(), AbstractTreeItem()])
-    root.dump()
+    data = {
+        'a': 1,
+        'b': [4, 8, 9, 5, 7, 99],
+        'c': {
+            'me': 'hi',
+            3: 67,
+            'd': {
+                'e': 3,
+                'f': 'ya!',
+                'g': 5,
+            },
+        },
+    }
+    root = KeyValueTreeItem('/', data)
+    print(root)
+
+    root.remove_child(root['/a'])
+    print('remove /a')
+    print(root)
+
+    d = root['c/d']
+    f = root['c/d/f']
+    d.remove_child(f)
+    print('remove /c/d/f')
+    print(root)
+
+    d.parent = root
+    print('move /c/d to /d')
+    print(root)
+
+    root.insert_child(1, d)
+    print('move /d to 2nd child of /')
+    print(root)
+
+    b = root['b']
+    b.insert_child(2, d)
+    print('move /d to 3rd child of /b')
+    print(root)
+
+    b.remove_child(b['1'])
+    print('remove /b/1')
+    print(root)
+
+    c = root['c']
+    c.children[1].value = 'bye'
+    print('/c/me:hi -> /c/me:bye')
+    print(root)
+    print(c)
+
+    c.insert_child(0, b['1'])
+    print('move /b/1 to first child of /c')
+    print(root)
 
 
 if __name__ == '__main__':
     test_tree()
```

### Comparing `pyqt_ext-1.1.2/src/pyqt_ext/PyQtChart.py` & `pyqt_ext-1.2.0/src/pyqt_ext/tmp/Chart.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,169 +1,167 @@
 """ PySide/PyQt 2-D plot.
-
-!!! THIS IS NOT WORKING YET !!!
 """
 
-from qtpy.QtCore import *
-from qtpy.QtGui import *
-from qtpy.QtWidgets import *
-from qtpy.QtCharts import *
-import numpy as np
-import platform
-
-# See https://github.com/PlotPyStack/PythonQwt/blob/master/qwt/plot_curve.py#L63
-import os
-try:
-    QT_API = os.environ["QT_API"].lower()
-except:
-    from qtpy import API_NAME
-    QT_API = API_NAME.lower()
-if QT_API == "pyside6":
-    import shiboken6 as shiboken
-    import ctypes
-
-
-class Plot(QChartView):
-    """ PySide/PyQt 2-D plot.
-    """
+# from qtpy.QtCore import *
+# from qtpy.QtGui import *
+# from qtpy.QtWidgets import *
+# from qtpy.QtCharts import *
+# import numpy as np
+# import platform
+
+# # See https://github.com/PlotPyStack/PythonQwt/blob/master/qwt/plot_curve.py#L63
+# import os
+# try:
+#     QT_API = os.environ["QT_API"].lower()
+# except:
+#     from qtpy import API_NAME
+#     QT_API = API_NAME.lower()
+# if QT_API == "pyside6":
+#     import shiboken6 as shiboken
+#     import ctypes
+
+
+# class Plot(QChartView):
+#     """ PySide/PyQt 2-D plot.
+#     """
     
-    def __init__(self, *args, **kwargs):
-        QChartView.__init__(self, *args, **kwargs)
+#     def __init__(self, *args, **kwargs):
+#         QChartView.__init__(self, *args, **kwargs)
 
-        self._chart: QChart = QChart()
-        # self._chart.createDefaultAxes()
-        self._xaxis: QValueAxis = QValueAxis()
-        self._yaxis: QValueAxis = QValueAxis()
-        self._chart.addAxis(self._xaxis, Qt.AlignmentFlag.AlignBottom)
-        self._chart.addAxis(self._yaxis, Qt.AlignmentFlag.AlignLeft)
-        self.setChart(self._chart)
-
-        if platform.system() == 'Darwin':
-            # Fix error message due to touch events on MacOS trackpad.
-            # !!! Warning: This may break touch events on a touch screen or mobile device.
-            # See https://bugreports.qt.io/browse/QTBUG-103935
-            self.viewport().setAttribute(Qt.WidgetAttribute.WA_AcceptTouchEvents, False)
+#         self._chart: QChart = QChart()
+#         # self._chart.createDefaultAxes()
+#         self._xaxis: QValueAxis = QValueAxis()
+#         self._yaxis: QValueAxis = QValueAxis()
+#         self._chart.addAxis(self._xaxis, Qt.AlignmentFlag.AlignBottom)
+#         self._chart.addAxis(self._yaxis, Qt.AlignmentFlag.AlignLeft)
+#         self.setChart(self._chart)
+
+#         if platform.system() == 'Darwin':
+#             # Fix error message due to touch events on MacOS trackpad.
+#             # !!! Warning: This may break touch events on a touch screen or mobile device.
+#             # See https://bugreports.qt.io/browse/QTBUG-103935
+#             self.viewport().setAttribute(Qt.WidgetAttribute.WA_AcceptTouchEvents, False)
     
 
-def array2d_to_qpolygonf(xdata, ydata) -> QPolygonF:
-    """
-    See https://github.com/PlotPyStack/PythonQwt/blob/master/qwt/plot_curve.py#L63
-
-    Utility function to convert two 1D-NumPy arrays representing curve data
-    (X-axis, Y-axis data) into a single polyline (QtGui.PolygonF object).
-    This feature is compatible with PyQt5 and PySide6 (requires QtPy).
-
-    License/copyright: MIT License © Pierre Raybaut 2020-2021.
-
-    :param numpy.ndarray xdata: 1D-NumPy array
-    :param numpy.ndarray ydata: 1D-NumPy array
-    :return: Polyline
-    :rtype: QtGui.QPolygonF
-    """
-    if not (xdata.size == ydata.size == xdata.shape[0] == ydata.shape[0]):
-        raise ValueError("Arguments must be 1D NumPy arrays with same size")
-    size = xdata.size
-    if QT_API.startswith("pyside"):  # PySide (obviously...)
-        polyline = QPolygonF()
-        polyline.resize(size)
-        address = shiboken.getCppPointer(polyline.data())[0]
-        buffer = (ctypes.c_double * 2 * size).from_address(address)
-    else:  # PyQt
-        if QT_API == "pyqt6":
-            polyline = QPolygonF([QPointF(0, 0)] * size)
-        else:
-            polyline = QPolygonF(size)
-        buffer = polyline.data()
-        buffer.setsize(16 * size)  # 16 bytes per point: 8 bytes per X,Y value (float64)
-    memory = np.frombuffer(buffer, np.float64)
-    memory[: (size - 1) * 2 + 1 : 2] = np.array(xdata, dtype=np.float64, copy=False)
-    memory[1 : (size - 1) * 2 + 2 : 2] = np.array(ydata, dtype=np.float64, copy=False)
-    return polyline
-
-
-def test_live():
-    import sys
-    import time
-
-    app = QApplication(sys.argv)
-    plot = Plot()
-
-    series = QLineSeries(name='test')
-    plot._chart.addSeries(series)
-    series.attachAxis(plot._xaxis)
-    series.attachAxis(plot._yaxis)
-    series.setUseOpenGL(True)
-
-    a = time.time()
-    n = int(1e7)
-    x = np.linspace(0, 10, n)
-    y = np.random.rand(n)
-    b = time.time()
-    poly = array2d_to_qpolygonf(x, y)
-    points = QPointFList()
-    points.reserve(n)
-    for i in range(n):
-        points.append(poly[i])
-    c = time.time()
-    series.replace(points)
-    plot.show()
-    d = time.time()
-    print('data creation (sec):', b - a)
-    print('data -> line series (sec):', c - b)
-    print('line plot (sec):', d - c)
-
-    app.exec()
-
-
-def test_live_pyqtgraph():
-    import sys
-    import time
-    from pyqtgraph_ext import PlotWidget, XYDataItem
-
-    app = QApplication(sys.argv)
-    plot = PlotWidget()
-
-    a = time.time()
-    n = int(1e7)
-    x = np.linspace(0, 10, n)
-    y = np.random.rand(n)
-    b = time.time()
-    data = XYDataItem(x=x, y=y)
-    plot.addItem(data)
-    plot.show()
-    c = time.time()
-    print('data creation (sec):', b - a)
-    print('line plot (sec):', c - b)
-
-    app.exec()
-
-
-def test_live_vispy():
-    import sys
-    import time
-    from vispy import plot as vp
-
-    app = QApplication(sys.argv)
-    win = QMainWindow()
-    fig = vp.Fig()
-    win.setCentralWidget(fig.native)
-
-    a = time.time()
-    n = int(1e7)
-    x = np.linspace(0, 10, n)
-    y = np.random.rand(n)
-    b = time.time()
-    ax = fig[0,0]
-    ax.plot((x, y))
-    win.show()
-    c = time.time()
-    print('data creation (sec):', b - a)
-    print('line plot (sec):', c - b)
-
-    app.exec()
-
-
-if __name__ == '__main__':
-    # test_live()
-    # test_live_pyqtgraph()
-    test_live_vispy()
+# def array2d_to_qpolygonf(xdata, ydata) -> QPolygonF:
+#     """
+#     See https://github.com/PlotPyStack/PythonQwt/blob/master/qwt/plot_curve.py#L63
+
+#     Utility function to convert two 1D-NumPy arrays representing curve data
+#     (X-axis, Y-axis data) into a single polyline (QtGui.PolygonF object).
+#     This feature is compatible with PyQt5 and PySide6 (requires QtPy).
+
+#     License/copyright: MIT License © Pierre Raybaut 2020-2021.
+
+#     :param numpy.ndarray xdata: 1D-NumPy array
+#     :param numpy.ndarray ydata: 1D-NumPy array
+#     :return: Polyline
+#     :rtype: QtGui.QPolygonF
+#     """
+#     if not (xdata.size == ydata.size == xdata.shape[0] == ydata.shape[0]):
+#         raise ValueError("Arguments must be 1D NumPy arrays with same size")
+#     size = xdata.size
+#     if QT_API.startswith("pyside"):  # PySide (obviously...)
+#         polyline = QPolygonF()
+#         polyline.resize(size)
+#         address = shiboken.getCppPointer(polyline.data())[0]
+#         buffer = (ctypes.c_double * 2 * size).from_address(address)
+#     else:  # PyQt
+#         if QT_API == "pyqt6":
+#             polyline = QPolygonF([QPointF(0, 0)] * size)
+#         else:
+#             polyline = QPolygonF(size)
+#         buffer = polyline.data()
+#         buffer.setsize(16 * size)  # 16 bytes per point: 8 bytes per X,Y value (float64)
+#     memory = np.frombuffer(buffer, np.float64)
+#     memory[: (size - 1) * 2 + 1 : 2] = np.array(xdata, dtype=np.float64, copy=False)
+#     memory[1 : (size - 1) * 2 + 2 : 2] = np.array(ydata, dtype=np.float64, copy=False)
+#     return polyline
+
+
+# def test_live():
+#     import sys
+#     import time
+
+#     app = QApplication(sys.argv)
+#     plot = Plot()
+
+#     series = QLineSeries(name='test')
+#     plot._chart.addSeries(series)
+#     series.attachAxis(plot._xaxis)
+#     series.attachAxis(plot._yaxis)
+#     series.setUseOpenGL(True)
+
+#     a = time.time()
+#     n = int(1e7)
+#     x = np.linspace(0, 10, n)
+#     y = np.random.rand(n)
+#     b = time.time()
+#     poly = array2d_to_qpolygonf(x, y)
+#     points = QPointFList()
+#     points.reserve(n)
+#     for i in range(n):
+#         points.append(poly[i])
+#     c = time.time()
+#     series.replace(points)
+#     plot.show()
+#     d = time.time()
+#     print('data creation (sec):', b - a)
+#     print('data -> line series (sec):', c - b)
+#     print('line plot (sec):', d - c)
+
+#     app.exec()
+
+
+# def test_live_pyqtgraph():
+#     import sys
+#     import time
+#     from pyqtgraph_ext import PlotWidget, XYDataItem
+
+#     app = QApplication(sys.argv)
+#     plot = PlotWidget()
+
+#     a = time.time()
+#     n = int(1e7)
+#     x = np.linspace(0, 10, n)
+#     y = np.random.rand(n)
+#     b = time.time()
+#     data = XYDataItem(x=x, y=y)
+#     plot.addItem(data)
+#     plot.show()
+#     c = time.time()
+#     print('data creation (sec):', b - a)
+#     print('line plot (sec):', c - b)
+
+#     app.exec()
+
+
+# def test_live_vispy():
+#     import sys
+#     import time
+#     from vispy import plot as vp
+
+#     app = QApplication(sys.argv)
+#     win = QMainWindow()
+#     fig = vp.Fig()
+#     win.setCentralWidget(fig.native)
+
+#     a = time.time()
+#     n = int(1e7)
+#     x = np.linspace(0, 10, n)
+#     y = np.random.rand(n)
+#     b = time.time()
+#     ax = fig[0,0]
+#     ax.plot((x, y))
+#     win.show()
+#     c = time.time()
+#     print('data creation (sec):', b - a)
+#     print('line plot (sec):', c - b)
+
+#     app.exec()
+
+
+# if __name__ == '__main__':
+#     # test_live()
+#     # test_live_pyqtgraph()
+#     test_live_vispy()
```

### Comparing `pyqt_ext-1.1.2/src/pyqt_ext/PyQtMultiValueSpinBox.py` & `pyqt_ext-1.2.0/src/pyqt_ext/widgets/MultiValueSpinBox.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """ PySide/PyQt multi-value spin box.
 """
 
 from __future__ import annotations
-
 from qtpy.QtCore import *
 from qtpy.QtGui import *
 from qtpy.QtWidgets import *
 import re
 import numpy as np
 
 
@@ -19,17 +18,22 @@
     """
 
     indicesChanged = Signal()
 
     def __init__(self, *args, **kwargs):
         QAbstractSpinBox.__init__(self, *args, **kwargs)
 
-        self._indices: np.ndarray[int] = np.array([0], dtype=int)
+        # possible values to select from
         self._indexed_values: np.ndarray = np.arange(100)
 
+        # indices of selected values in self._indexed_values
+        # i.e., selected values are self._indexed_values[self._indices]
+        self._indices: np.ndarray[int] = np.array([0], dtype=int)
+
+        # initialize with default values
         self.setIndices(self._indices)
 
         self.setSizePolicy(QSizePolicy.Expanding, self.sizePolicy().verticalPolicy())
 
         self.editingFinished.connect(self.onTextEdited)
 
         self.setToolTip('index/slice (+Shift: page up/down)')
@@ -106,79 +110,39 @@
         return indices
     
     def valuesFromText(self, text: str, validate: bool = False) -> list:
         text = text.strip()
         if text == '':
             return np.array([0])
         if text == ':':
-            return np.arange(len(self._indexed_values))
+            return self._indexed_values
         fields = re.split(r'[,\s]+', text)
         values = []
         dtype = self._indexed_values.dtype.type
         for field in fields:
             try:
                 field = field.strip()
                 if field == '':
                     continue
                 if field == ':':
-                    return np.arange(len(self._indexed_values))
-                if ':' in field:
-                    slice_args = [dtype(arg) if len(arg.strip()) else None for arg in field.split(':')]
-                    if np.issubdtype(self._indexed_values.dtype, np.integer):
-                        slice_obj = slice(*slice_args)
-                        slice_indices = list(range(*slice_obj.indices(len(self._indexed_values))))
-                        values.extend(slice_indices)
-                    elif np.issubdtype(self._indexed_values.dtype, np.floating):
-                        if len(slice_args) == 1:
-                            first = slice_args[0]
-                            i: int = np.searchsorted(self._indexed_values, first, side='left')
-                            values.extend(self._indexed_values[i:].tolist())
-                        elif len(slice_args) == 2:
-                            first = slice_args[0]
-                            last = slice_args[1]
-                            i: int = np.searchsorted(self._indexed_values, first, side='left')
-                            j: int = i + 1 + np.searchsorted(self._indexed_values[i+1:], last, side='right')
-                            if j > i:
-                                values.extend(self._indexed_values[i:j].tolist())
+                    return self._indexed_values
+                if ':' in field or '-' in field:
+                    # first:last or first-last inclusive
+                    delimeter = ':' if ':' in field else '-'
+                    first, last = [dtype(arg) if len(arg.strip()) else None for arg in field.split(delimeter)]
+                    if first is None:
+                        start_index: int = 0
                     else:
-                        # do not assume values are ordered if not integer or floating point
-                        if len(slice_args) == 1:
-                            first = slice_args[0]
-                            try:
-                                i: int = np.where(self._indexed_values == first)[0][0]
-                                values.extend(self._indexed_values[i:].tolist())
-                            except:
-                                pass
-                        elif len(slice_args) == 2:
-                            first = slice_args[0]
-                            last = slice_args[1]
-                            try:
-                                i: int = np.where(self._indexed_values == first)[0][0]
-                                j: int = i + 1 + np.where(self._indexed_values[i+1:] == last)[0][0] + 1
-                                values.extend(self._indexed_values[i:j].tolist())
-                            except:
-                                pass
-                elif '-' in field:
-                    first, last = field.split('-')
-                    first, last = dtype(first), dtype(last)
-                    if np.issubdtype(self._indexed_values.dtype, np.integer):
-                        values.extend(list(range(int(first), int(last) + 1)))
-                    elif np.issubdtype(self._indexed_values.dtype, np.floating):
-                        i: int = np.searchsorted(self._indexed_values, first, side='left')
-                        j: int = i + 1 + np.searchsorted(self._indexed_values[i+1:], last, side='right')
-                        if j > i:
-                            values.extend(self._indexed_values[i:j].tolist())
+                        start_index: int = self.indicesFromValues([first])[0]
+                    if last is None:
+                        stop_index: int = len(self._indexed_values)
                     else:
-                        # do not assume values are ordered if not integer or floating point
-                        try:
-                            i: int = np.where(self._indexed_values == first)[0][0]
-                            j: int = i + 1 + np.where(self._indexed_values[i+1:] == last)[0][0] + 1
-                            values.extend(self._indexed_values[i:j].tolist())
-                        except:
-                            pass
+                        stop_index: int = self.indicesFromValues([last])[0] + 1
+                    if stop_index > start_index:
+                        values.extend(self._indexed_values[start_index:stop_index].tolist())
                 else:
                     value = dtype(field)
                     values.append(value)
             except:
                 if validate:
                     raise ValueError(f'Invalid text: {field}')
                 else:
@@ -271,16 +235,15 @@
         #     self.values_from_text(self.lineEdit().text(), validate=True)
         # except:
         #     return QValidator.Intermediate, text, pos
         return QValidator.Acceptable, text, pos
 
     
 def test_live():
-    import sys
-    app = QApplication(sys.argv)
+    app = QApplication()
 
     def print_indices_and_values(spinbox: MultiValueSpinBox):
         print('indices:', spinbox.indices())
         print('selected_values:', spinbox.selectedValues())
 
     ui = QWidget()
     vbox = QVBoxLayout(ui)
@@ -322,13 +285,12 @@
     spinbox.setIndexedValues(['cat','mouse','dog','house','car','truck'])
     spinbox.indicesChanged.connect(lambda obj=spinbox: print_indices_and_values(obj))
     vbox.addWidget(QLabel('cat, mouse, dog, house, car, truck'))
     vbox.addWidget(spinbox)
     vbox.addStretch()
 
     ui.show()
-    status = app.exec()
-    sys.exit(status)
+    app.exec()
 
 
 if __name__ == '__main__':
     test_live()
```

### Comparing `pyqt_ext-1.1.2/src/pyqt_ext/PyQtXYDataStyle.py` & `pyqt_ext-1.2.0/src/pyqt_ext/graph/GraphStyle.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,302 +1,388 @@
-""" Widget for editing the style of (x,y) data.
+""" Widget for editing the style of graph data.
 
 Style is stored in hashable dict.
 """
 
 from __future__ import annotations
 from qtpy.QtCore import *
 from qtpy.QtGui import *
 from qtpy.QtWidgets import *
-from pyqt_ext import ColorButton
+from pyqt_ext.utils import ColorType, toQColor, toColorStr
+from pyqt_ext.widgets import ColorButton, CollapsibleSection
 
 
-ColorType = str | tuple[int | float] | list[int | float] | QColor
+class GraphStyle(dict):
+    """ Hashable style dict for graph data.
 
-
-class XYDataStyleDict(dict):
-    """ Hashable style dict for (x,y) data.
-
-    'Color': str
-    'LineStyle': str
-    'LineWidth': float
-    'Marker': str
-    'MarkerSize': float
-    'MarkerEdgeWidth': float
-    'MarkerEdgeColor': str
-    'MarkerFaceColor': str
+    'color': str
+    'linestyle': str
+    'linewidth': float
+    'marker': str
+    'markersize': float
+    'markeredgestyle': str
+    'markeredgewidth': float
+    'markeredgecolor': str
+    'markerfacecolor': str
     """
 
+    linestyles = ['none', '-', '--', ':', '-.', '-..']
+    penstyles = [Qt.PenStyle.NoPen, Qt.PenStyle.SolidLine, Qt.PenStyle.DashLine, Qt.PenStyle.DotLine, Qt.PenStyle.DashDotLine, Qt.PenStyle.DashDotDotLine]
+
     def __init__(self, *args, **kwargs):
         dict.__init__(self, *args, **kwargs)
 
-        # Qt.PenStyle.NoPen = 0
-        # Qt.PenStyle.SolidLine = 1
-        # Qt.PenStyle.DashLine = 2
-        # Qt.PenStyle.DotLine = 3
-        # Qt.PenStyle.DashDotLine = 4
-        self.penStyles = [Qt.PenStyle.NoPen, Qt.PenStyle.SolidLine, Qt.PenStyle.DashLine, Qt.PenStyle.DotLine, Qt.PenStyle.DashDotLine]
-        self.lineStyles = ['none', '-', '--', ':', '-.']
-
-        # Default markers supported by pyqtgraph.
-        # Change these to whatever you want.
-        self.markers = ['none', 'o', 't', 't1', 't2', 't3', 's', 'p', 'h', 'star', '+', 'd', 'x']
-    
-    def color(self) -> str:
-        return self.get('Color', 'auto')
+        # alternate key names
+        self._keymap = {
+            'c': 'color',
+            'ls': 'linestyle',
+            'lw': 'linewidth',
+            'symbol': 'marker',
+            's': 'marker',
+            'm': 'marker',
+            'ms': 'markersize',
+            'mes': 'markeredgestyle',
+            'mew': 'markeredgewidth',
+            'mec': 'markeredgecolor',
+            'mfc': 'markerfacecolor',
+        }
+
+        # default values
+        self._defaults = {
+            'linestyle': '-',
+            'linewidth': 1,
+            'marker': 'none',
+            'markersize': 10,
+            'markeredgestyle': '-',
+            'markeredgewidth': 1,
+        }
+    
+    
+    def __getitem__(self, key: str):
+        key = key.lower()
+        if key in self._keymap:
+            key = self._keymap[key]
+        if key in self:
+            return dict.__getitem__(self, key)
+        # key not found...
+        if key == 'markeredgewidth':
+            if 'linewidth' in self:
+                return self['linewidth']
+        elif key == 'markeredgecolor':
+            if 'color' in self:
+                return self['color']
+        elif key == 'markerfacecolor':
+            if 'markeredgecolor' in self:
+                return self['markeredgecolor']
+            elif 'color' in self:
+                return self['color']
+        if key in self._defaults:
+            return self._defaults[key]
+    
+    def __setitem__(self, key: str, value):
+        key = key.lower()
+        if key in self._keymap:
+            key = self._keymap[key]
+        if key.endswith('color'):
+            if value is not None:
+                value = toColorStr(value)
+        elif key in ['linestyle', 'markeredgestyle']:
+            if value is None:
+                value = 'none'
+            elif isinstance(value, int):
+                value = GraphStyle.linestyles[value]
+            elif isinstance(value, Qt.PenStyle):
+                value = GraphStyle.linestyles[GraphStyle.penstyles.index(value)]
+            elif isinstance(value, str):
+                if value == '.-':
+                    value = '-.'
+                elif value == '..-' or value == '.-.':
+                    value = '-..'
+        elif key == 'linewidth':
+            if value is not None:
+                value = max(0, value)
+        elif key == 'marker':
+            if value is None:
+                value = 'none'
+        elif key == 'markersize':
+            if value is not None:
+                value = max(0, value)
+        elif key == 'markeredgewidth':
+            if value is not None:
+                value = max(0, value)
+        if value is None:
+            del self[key]
+            return
+        dict.__setitem__(self, key, value)
+    
+    def __delitem__(self, key: str):
+        key = key.lower()
+        if key in self._keymap:
+            key = self._keymap[key]
+        if key in self:
+            dict.__delitem__(self, key)
     
-    def setColor(self, value: ColorType):
-        self['Color'] = XYDataStyleDict.toColorStr(value)
+    def color(self) -> str | None:
+        return self['color']
     
-    def qcolor(self) -> QColor:
-        return XYDataStyleDict.toQColor(self.color())
+    def setColor(self, value: ColorType | None):
+        self['color'] = value
     
     def lineStyle(self) -> str:
-        return self.get('LineStyle', '-')
+        return self['linestyle']
     
     def setLineStyle(self, value: str | int | Qt.PenStyle | None):
-        if value is None:
-            value = 'none'
-        elif isinstance(value, int):
-            value = self.lineStyles[value]
-        elif isinstance(value, Qt.PenStyle):
-            index = self.penStyles.index(value)
-            value = self.lineStyles[index]
-        self['LineStyle'] = value
-    
-    def lineQtPenStyle(self) -> Qt.PenStyle:
-        return Qt.PenStyle(self.lineStyles.index(self.lineStyle()))
+        self['linestyle'] = value
     
     def lineWidth(self) -> float:
-        return self.get('LineWidth', 1)
+        return self['linewidth']
     
     def setLineWidth(self, value: float):
-        self['LineWidth'] = value
+        self['linewidth'] = value
     
     def marker(self) -> str:
-        return self.get('Marker', 'none')
+        return self['marker']
     
     def setMarker(self, value: str | None):
-        if value is None:
-            value = 'none'
-        self['Marker'] = value
+        self['marker'] = value
     
     def markerSize(self) -> float:
-        return self.get('MarkerSize', 10)
+        return self['markersize']
     
     def setMarkerSize(self, value: float):
-        self['MarkerSize'] = value
+        self['markersize'] = value
+    
+    def markerEdgeStyle(self) -> str:
+        return self['markeredgestyle']
+    
+    def setMarkerEdgeStyle(self, value: str | int | Qt.PenStyle | None):
+        self['markeredgestyle'] = value
     
     def markerEdgeWidth(self) -> float:
-        return self.get('MarkerEdgeWidth', self.lineWidth())
+        return self['markeredgewidth']
     
     def setMarkerEdgeWidth(self, value: float):
-        self['MarkerEdgeWidth'] = value
+        self['markeredgewidth'] = value
     
     def markerEdgeColor(self) -> str:
-        return self.get('MarkerEdgeColor', 'auto')
-    
-    def setMarkerEdgeColor(self, value: ColorType):
-        self['MarkerEdgeColor'] = XYDataStyleDict.toColorStr(value)
+        return self['markeredgecolor']
     
-    def markerEdgeQColor(self) -> QColor:
-        return XYDataStyleDict.toQColor(self.markerEdgeColor())
+    def setMarkerEdgeColor(self, value: ColorType | None):
+        self['markeredgecolor'] = value
     
     def markerFaceColor(self) -> str:
-        return self.get('MarkerFaceColor', 'auto')
-    
-    def setMarkerFaceColor(self, value: ColorType):
-        self['MarkerFaceColor'] = XYDataStyleDict.toColorStr(value)
+        return self['markerfacecolor']
     
-    def markerFaceQColor(self) -> QColor:
-        return XYDataStyleDict.toQColor(self.markerFaceColor())
-    
-    @staticmethod
-    def toQColor(color: ColorType) -> QColor:
-        if isinstance(color, QColor):
-            return color
-        if isinstance(color, str):
-            color = color.strip()
-            if color.lower() in ['auto', 'none']:
-                return QColor('transparent')
-            elif QColor.isValidColorName(color):
-                return QColor(color)
-            else:
-                # (r,g,b) or (r,g,b,a)
-                color = color.lstrip('(').rstrip(')').split(',')
-                for i, part in enumerate(color):
-                    try:
-                        color[i] = int(part)
-                    except:
-                        color = [float(part) for part in color]
-                        break
-        # (r,g,b) or (r,g,b,a)
-        if isinstance(color[0], float):
-            return QColor.fromRgbF(*color)
-        return QColor(*color)
-    
-    @staticmethod
-    def toColorStr(color: ColorType) -> str:
-        if isinstance(color, QColor):
-            # (r,g,b,a) in [0,255]
-            return f'({color.red()}, {color.green()}, {color.blue()}, {color.alpha()})'
-        if isinstance(color, str):
-            if ',' in color:
-                # (r,g,b) or (r,g,b,a)
-                qcolor = XYDataStyleDict.toQColor(color)
-                return XYDataStyleDict.toColorStr(qcolor)
-            # TODO: sanity check?
-            return color
-        if isinstance(color, tuple) or isinstance(color, list):
-            # (r,g,b) or (r,g,b,a)
-            return '(' + ', '.join([str(part) for part in color]) + ')'
+    def setMarkerFaceColor(self, value: ColorType | None):
+        self['markerfacecolor'] = value
 
 
-class XYDataStylePanel(QWidget):
+class GraphStylePanel(QWidget):
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, styles: list[str] = None, *args, **kwargs):
         QWidget.__init__(self, *args, **kwargs)
 
-        form = QFormLayout(self)
-
-        # color
-        self.colorButton = ColorButton(QColor(0, 114, 189))
-        self.autoColorCheckBox = QCheckBox('Auto')
-        self.autoColorCheckBox.setChecked(False)
-        self.autoColorCheckBox.stateChanged.connect(lambda isChecked: self.colorButton.setVisible(not isChecked))
-        colorLayout = QHBoxLayout()
-        colorLayout.setContentsMargins(0, 0, 0, 0)
-        colorLayout.setSpacing(5)
-        colorLayout.addWidget(self.colorButton)
-        colorLayout.addWidget(self.autoColorCheckBox)
-        self.colorButton.setVisible(not self.autoColorCheckBox.isChecked())
-        form.addRow('Color', colorLayout)
+        if styles is None:
+            styles = ['color', 'linestyle', 'linewidth', 'marker', 'markersize', 'markeredgestyle', 'markeredgewidth', 'markeredgecolor', 'markerfacecolor']
+        self.styles = [style.lower() for style in styles]
+
+        vbox = QVBoxLayout(self)
+        vbox.setContentsMargins(10, 10, 10, 10)
+        vbox.setSpacing(10)
 
         # line
-        # Qt.PenStyle.NoPen = 0
-        # Qt.PenStyle.SolidLine = 1
-        # Qt.PenStyle.DashLine = 2
-        # Qt.PenStyle.DotLine = 3
-        # Qt.PenStyle.DashDotLine = 4
-        self.lineStyles = ['none', '-', '--', ':', '-.']
-        self.lineStyleComboBox = QComboBox()
-        self.lineStyleComboBox.addItems(['No Line', 'Solid Line', 'Dash Line', 'Dot Line', 'Dash Dot Line'])
-        self.lineStyleComboBox.setCurrentIndex(1)
-        form.addRow('Line Style', self.lineStyleComboBox)
+        if set(['color', 'linestyle', 'linewidth']).intersection(self.styles):
+            self.lineSection = CollapsibleSection(title='Line')
+            form = QFormLayout()
+            form.setContentsMargins(10, 10, 10, 10)
+            form.setSpacing(10)
+            if 'color' in self.styles:
+                self.colorButton = ColorButton()
+                form.addRow('Color', self.colorButton)
+            if 'linestyle' in self.styles:
+                self.lineStyleComboBox = QComboBox()
+                self._lineStyles = {
+                    'No Line': 'none',
+                    'Solid Line': '-',
+                    'Dash Line': '--',
+                    'Dot Line': ':',
+                    'Dash Dot Line': '-.',
+                    'Dash Dot Dot Line': '-..',
+                }
+                self.lineStyleComboBox.addItems(list(self._lineStyles.keys()))
+                self.lineStyleComboBox.setCurrentIndex(1)
+                form.addRow('Style', self.lineStyleComboBox)
+            if 'linewidth' in self.styles:
+                self.lineWidthSpinBox = QDoubleSpinBox()
+                self.lineWidthSpinBox.setMinimum(0)
+                self.lineWidthSpinBox.setValue(1)
+                form.addRow('Width', self.lineWidthSpinBox)
+            self.lineSection.setContentLayout(form)
+            vbox.addWidget(self.lineSection)
         
-        self.lineWidthSpinBox = QDoubleSpinBox()
-        self.lineWidthSpinBox.setMinimum(0)
-        self.lineWidthSpinBox.setValue(1)
-        form.addRow('Line Width', self.lineWidthSpinBox)
-
         # marker
-        # pyqtgraph default markers
-        self.markers = ['none', 'o', 't', 't1', 't2', 't3', 's', 'p', 'h', 'star', '+', 'd', 'x']
-        self.markerComboBox = QComboBox()
-        self.markerComboBox.addItems([
-            'None', 'Circle', 'Triangle Down', 'Triangle Up', 'Triangle Right', 'Triangle Left', 'Square', 
-            'Pentagon', 'Hexagon', 'Star', 'Plus', 'Prism', 'Cross'])
-        self.markerComboBox.setCurrentIndex(0)
-        form.addRow('Marker', self.markerComboBox)
-
-        self.markerSizeSpinBox = QDoubleSpinBox()
-        self.markerSizeSpinBox.setMinimum(0)
-        self.markerSizeSpinBox.setValue(10)
-        form.addRow('Marker Size', self.markerSizeSpinBox)
-
-        self.markerEdgeWidthSpinBox = QDoubleSpinBox()
-        self.markerEdgeWidthSpinBox.setMinimum(0)
-        self.markerEdgeWidthSpinBox.setValue(self.lineWidthSpinBox.value())
-        form.addRow('Marker Edge Width', self.markerEdgeWidthSpinBox)
-
-        self.markerEdgeColorButton = ColorButton(self.colorButton.color())
-        self.autoMarkerEdgeColorCheckBox = QCheckBox('Auto')
-        self.autoMarkerEdgeColorCheckBox.setChecked(True)
-        self.autoMarkerEdgeColorCheckBox.stateChanged.connect(lambda isChecked: self.markerEdgeColorButton.setVisible(not isChecked))
-        markerEdgeColorLayout = QHBoxLayout()
-        markerEdgeColorLayout.setContentsMargins(0, 0, 0, 0)
-        markerEdgeColorLayout.setSpacing(5)
-        markerEdgeColorLayout.addWidget(self.markerEdgeColorButton)
-        markerEdgeColorLayout.addWidget(self.autoMarkerEdgeColorCheckBox)
-        self.markerEdgeColorButton.setVisible(not self.autoMarkerEdgeColorCheckBox.isChecked())
-        form.addRow('Marker Edge Color', markerEdgeColorLayout)
-
-        self.markerFaceColorButton = ColorButton(self.markerEdgeColorButton.color())
-        self.autoMarkerFaceColorCheckBox = QCheckBox('Auto')
-        self.autoMarkerFaceColorCheckBox.setChecked(True)
-        self.autoMarkerFaceColorCheckBox.stateChanged.connect(lambda isChecked: self.markerFaceColorButton.setVisible(not isChecked))
-        markerFaceColorLayout = QHBoxLayout()
-        markerFaceColorLayout.setContentsMargins(0, 0, 0, 0)
-        markerFaceColorLayout.setSpacing(5)
-        markerFaceColorLayout.addWidget(self.markerFaceColorButton)
-        markerFaceColorLayout.addWidget(self.autoMarkerFaceColorCheckBox)
-        self.markerFaceColorButton.setVisible(not self.autoMarkerFaceColorCheckBox.isChecked())
-        form.addRow('Marker Face Color', markerFaceColorLayout)
-    
-    def styleDict(self) -> XYDataStyleDict:
-        style = XYDataStyleDict()
-        if self.autoColorCheckBox.isChecked():
-            style.setColor('auto')
-        else:
-            style.setColor(self.colorButton.color())
-        style.setLineStyle(self.lineStyles[self.lineStyleComboBox.currentIndex()])
-        style.setLineWidth(self.lineWidthSpinBox.value())
-        style.setMarker(self.markers[self.markerComboBox.currentIndex()])
-        style.setMarkerSize(self.markerSizeSpinBox.value())
-        style.setMarkerEdgeWidth(self.markerEdgeWidthSpinBox.value())
-        if self.autoMarkerEdgeColorCheckBox.isChecked():
-            style.setMarkerEdgeColor('auto')
-        else:
-            style.setMarkerEdgeColor(self.markerEdgeColorButton.color())
-        if self.autoMarkerFaceColorCheckBox.isChecked():
-            style.setMarkerFaceColor('auto')
-        else:
-            style.setMarkerFaceColor(self.markerFaceColorButton.color())
-        return style
-    
-    def setStyleDict(self, style: XYDataStyleDict):
-        # color
-        self.autoColorCheckBox.setChecked(style.color() == 'auto')
-        if self.autoColorCheckBox.isChecked():
-            self.colorButton.hide()
-        else:
-            self.colorButton.show()
-            self.colorButton.setColor(style.qcolor())
-
-        # line
-        try:
-            self.lineStyleComboBox.setCurrentIndex(self.lineStyles.index(style.lineStyle()))
-        except:
-            self.lineStyleComboBox.setCurrentIndex(1)
-        self.lineWidthSpinBox.setValue(style.lineWidth())
-
-        # marker
-        try:
-            self.markerComboBox.setCurrentIndex(self.markers.index(style.marker()))
-        except:
-            self.markerComboBox.setCurrentIndex(0)
-        self.markerSizeSpinBox.setValue(style.markerSize())
-        self.markerEdgeWidthSpinBox.setValue(style.markerEdgeWidth())
-        self.autoMarkerEdgeColorCheckBox.setChecked(style.markerEdgeColor() == 'auto')
-        if self.autoMarkerEdgeColorCheckBox.isChecked():
-            self.markerEdgeColorButton.hide()
-        else:
-            self.markerEdgeColorButton.show()
-            self.markerEdgeColorButton.setColor(style.markerEdgeQColor())
-        self.autoMarkerFaceColorCheckBox.setChecked(style.markerFaceColor() == 'auto')
-        if self.autoMarkerFaceColorCheckBox.isChecked():
-            self.markerFaceColorButton.hide()
-        else:
-            self.markerFaceColorButton.show()
-            self.markerFaceColorButton.setColor(style.markerFaceQColor())
-    
-
-def editXYDataStyle(style: XYDataStyleDict, parent: QWidget = None, title: str = None) -> XYDataStyleDict | None:
-    panel = XYDataStylePanel()
-    panel.setStyleDict(style)
+        if set(['marker', 'markersize', 'markeredgestyle', 'markeredgewidth', 'markeredgecolor', 'markerfacecolor']).intersection(self.styles):
+            self.markerSection = CollapsibleSection(title='Marker')
+            form = QFormLayout()
+            form.setContentsMargins(10, 10, 10, 10)
+            form.setSpacing(10)
+            if 'marker' in self.styles:
+                self.markerComboBox = QComboBox()
+                # pyqtgraph default markers
+                self.markerComboBox.addItems(['None', 'Circle', 'Triangle Down', 'Triangle Up', 'Triangle Right', 'Triangle Left', 'Square', 'Diamond', 'Pentagon', 'Hexagon', 'Star', 'Plus', 'Cross'])
+                self.markerComboBox.setCurrentIndex(0)
+                form.addRow('Symbol', self.markerComboBox)
+            if 'markersize' in self.styles:
+                self.markerSizeSpinBox = QDoubleSpinBox()
+                self.markerSizeSpinBox.setMinimum(0)
+                self.markerSizeSpinBox.setValue(10)
+                form.addRow('Size', self.markerSizeSpinBox)
+            if 'markeredgestyle' in self.styles:
+                self.markerEdgeStyleComboBox = QComboBox()
+                self._markerEdgeStyles = {
+                    'No Line': 'none',
+                    'Solid Line': '-',
+                    'Dash Line': '--',
+                    'Dot Line': ':',
+                    'Dash Dot Line': '-.',
+                    'Dash Dot Dot Line': '-..',
+                }
+                self.markerEdgeStyleComboBox.addItems(list(self._markerEdgeStyles.keys()))
+                self.markerEdgeStyleComboBox.setCurrentIndex(1)
+                form.addRow('Edge Style', self.markerEdgeStyleComboBox)
+            if 'markeredgewidth' in self.styles:
+                self.markerEdgeWidthSpinBox = QDoubleSpinBox()
+                self.markerEdgeWidthSpinBox.setMinimum(0)
+                self.markerEdgeWidthSpinBox.setValue(1)
+                form.addRow('Edge Width', self.markerEdgeWidthSpinBox)
+            if 'markeredgecolor' in self.styles:
+                self.markerEdgeColorButton = ColorButton()
+                form.addRow('Edge Color', self.markerEdgeColorButton)
+            if 'markerfacecolor' in self.styles:
+                self.markerFaceColorButton = ColorButton()
+                form.addRow('Face Color', self.markerFaceColorButton)
+            self.markerSection.setContentLayout(form)
+            vbox.addWidget(self.markerSection)
+        
+        # expand 1st section
+        if vbox.count() > 0:
+            vbox.itemAt(0).widget().expand()
+        
+        vbox.addStretch()
+    
+    def graphStyle(self) -> GraphStyle:
+        graphStyle = GraphStyle()
+        for style in self.styles:
+            if style == 'color':
+                color = self.colorButton.color()
+                if color is not None:
+                    graphStyle.setColor(color)
+            elif style == 'linestyle':
+                key = self.lineStyleComboBox.currentText()
+                lineStyle = self._lineStyles[key]
+                graphStyle.setLineStyle(lineStyle)
+            elif style == 'linewidth':
+                lineWidth = self.lineWidthSpinBox.value()
+                graphStyle.setLineWidth(lineWidth)
+            elif style == 'marker':
+                marker = self.markerComboBox.currentText().lower()
+                graphStyle.setMarker(marker)
+            elif style == 'markersize':
+                markerSize = self.markerSizeSpinBox.value()
+                graphStyle.setMarkerSize(markerSize)
+            elif style == 'markeredgestyle':
+                key = self.markerEdgeStyleComboBox.currentText()
+                markerEdgeStyle = self._markerEdgeStyles[key]
+                graphStyle.setMarkerEdgeStyle(markerEdgeStyle)
+            elif style == 'markeredgewidth':
+                markerEdgeWidth = self.markerEdgeWidthSpinBox.value()
+                graphStyle.setMarkerEdgeWidth(markerEdgeWidth)
+            elif style == 'markeredgecolor':
+                markerEdgeColor = self.markerEdgeColorButton.color()
+                if markerEdgeColor is not None:
+                    graphStyle.setMarkerEdgeColor(markerEdgeColor)
+            elif style == 'markerfacecolor':
+                markerFaceColor = self.markerFaceColorButton.color()
+                if markerFaceColor is not None:
+                    graphStyle.setMarkerFaceColor(markerFaceColor)
+        return graphStyle
+    
+    def setGraphStyle(self, graphStyle: GraphStyle):
+        for style in self.styles:
+            if style == 'color':
+                try:
+                    color = graphStyle.color()
+                    self.colorButton.setColor(color)
+                except Exception:
+                    pass
+            elif style == 'linestyle':
+                try:
+                    lineStyle = graphStyle.lineStyle()
+                    for key, value in self._lineStyles.items():
+                        if value.lower() == lineStyle.lower() or key.lower() == lineStyle.lower():
+                            lineStyle = key
+                            break
+                    self.lineStyleComboBox.setCurrentText(lineStyle)
+                except Exception:
+                    pass
+            elif style == 'linewidth':
+                try:
+                    lineWidth = graphStyle.lineWidth()
+                    self.lineWidthSpinBox.setValue(lineWidth)
+                except Exception:
+                    pass
+            elif style == 'marker':
+                try:
+                    marker = graphStyle.marker()
+                    for i, item in enumerate(self.markerComboBox.items()):
+                        if item.text().lower() == marker.lower():
+                            self.markerComboBox.setCurrentIndex(i)
+                            break
+                except Exception:
+                    pass
+            elif style == 'markersize':
+                try:
+                    markerSize = graphStyle.markerSize()
+                    self.markerSizeSpinBox.setValue(markerSize)
+                except Exception:
+                    pass
+            elif style == 'markeredgestyle':
+                try:
+                    markerEdgeStyle = graphStyle.markerEdgeStyle()
+                    for key, value in self._markerEdgeStyles.items():
+                        if value.lower() == markerEdgeStyle.lower() or key.lower() == markerEdgeStyle.lower():
+                            markerEdgeStyle = key
+                            break
+                    self.markerEdgeStyleComboBox.setCurrentText(markerEdgeStyle)
+                except Exception:
+                    pass
+            elif style == 'markeredgewidth':
+                try:
+                    markerEdgeWidth = graphStyle.setMarkerEdgeWidth()
+                    self.markerEdgeWidthSpinBox.setValue(markerEdgeWidth)
+                except Exception:
+                    pass
+            elif style == 'markeredgecolor':
+                try:
+                    markerEdgeColor = graphStyle.markerEdgeColor()
+                    self.markerEdgeColorButton.setColor(markerEdgeColor)
+                except Exception:
+                    pass
+            elif style == 'markerfacecolor':
+                try:
+                    markerFaceColor = graphStyle.markerFaceColor()
+                    self.markerFaceColorButton.setColor(markerFaceColor)
+                except Exception:
+                    pass
+
+
+def editGraphStyle(graphStyle: GraphStyle, styles: list[str] = None, parent: QWidget = None, title: str = None) -> GraphStyle | None:
+    panel = GraphStylePanel(styles)
+    panel.layout().setContentsMargins(0, 0, 0, 0)
+    panel.setGraphStyle(graphStyle)
 
     dlg = QDialog(parent)
     vbox = QVBoxLayout(dlg)
     vbox.addWidget(panel)
 
     btns = QDialogButtonBox()
     btns.setStandardButtons(QDialogButtonBox.Cancel | QDialogButtonBox.Ok)
@@ -305,21 +391,20 @@
     vbox.addWidget(btns)
     vbox.addStretch()
 
     if title is not None:
         dlg.setWindowTitle(title)
     dlg.setWindowModality(Qt.ApplicationModal)
     if dlg.exec() == QDialog.Accepted:
-        return panel.styleDict()
+        return panel.graphStyle()
 
 
 def test_live():
-    import sys 
-    app = QApplication(sys.argv)
-    ui = XYDataStylePanel()
+    app = QApplication()
+    ui = GraphStylePanel()
     ui.show()
-    status = app.exec()
-    sys.exit(status)
+    # QTimer.singleShot(1000, lambda: print(editGraphStyle(GraphStyle())))
+    app.exec()
 
 
 if __name__ == '__main__':
     test_live()
```

