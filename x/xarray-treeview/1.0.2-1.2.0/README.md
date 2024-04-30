# Comparing `tmp/xarray_treeview-1.0.2.tar.gz` & `tmp/xarray_treeview-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_treeview-1.0.2.tar", last modified: Thu Jan 11 16:24:37 2024, max compression
+gzip compressed data, was "xarray_treeview-1.2.0.tar", last modified: Tue Apr 30 21:47:09 2024, max compression
```

## Comparing `xarray_treeview-1.0.2.tar` & `xarray_treeview-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-01-11 16:04:45.274505 xarray_treeview-1.0.2/LICENSE
--rw-r--r--   0        0        0      194 2024-01-11 16:04:45.274689 xarray_treeview-1.0.2/README.md
--rw-r--r--   0        0        0     1256 2024-01-11 16:24:37.955186 xarray_treeview-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4168 2024-01-11 16:07:12.989573 xarray_treeview-1.0.2/src/xarray_treeview/PyQtXarrayTreeItem.py
--rw-r--r--   0        0        0     5554 2024-01-11 16:06:48.414176 xarray_treeview-1.0.2/src/xarray_treeview/PyQtXarrayTreeModel.py
--rw-r--r--   0        0        0     9528 2024-01-11 16:15:33.714988 xarray_treeview-1.0.2/src/xarray_treeview/PyQtXarrayTreeView.py
--rw-r--r--   0        0        0      187 2024-01-11 16:07:55.230839 xarray_treeview-1.0.2/src/xarray_treeview/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 16:04:45.276303 xarray_treeview-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 xarray_treeview-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-01-11 16:04:45.274505 xarray_treeview-1.2.0/LICENSE
+-rw-r--r--   0        0        0      210 2024-01-29 19:36:00.736104 xarray_treeview-1.2.0/README.md
+-rw-r--r--   0        0        0     1256 2024-04-30 21:47:09.910923 xarray_treeview-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7671 2024-04-24 22:17:08.019833 xarray_treeview-1.2.0/src/xarray_treeview/XarrayTreeItem.py
+-rw-r--r--   0        0        0     5999 2024-03-08 22:47:30.993487 xarray_treeview-1.2.0/src/xarray_treeview/XarrayTreeModel.py
+-rw-r--r--   0        0        0    10664 2024-04-26 15:47:20.923676 xarray_treeview-1.2.0/src/xarray_treeview/XarrayTreeView.py
+-rw-r--r--   0        0        0      195 2024-02-08 22:49:32.523681 xarray_treeview-1.2.0/src/xarray_treeview/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 16:04:45.276303 xarray_treeview-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 xarray_treeview-1.2.0/PKG-INFO
```

### Comparing `xarray_treeview-1.0.2/LICENSE` & `xarray_treeview-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray_treeview-1.0.2/pyproject.toml` & `xarray_treeview-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
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
 homepage = "https://github.com/marcel-goldschen-ohm/xarray-treeview"
 repository = "https://github.com/marcel-goldschen-ohm/xarray-treeview"
```

### Comparing `xarray_treeview-1.0.2/src/xarray_treeview/PyQtXarrayTreeView.py` & `xarray_treeview-1.2.0/src/xarray_treeview/XarrayTreeView.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,139 +2,124 @@
 """
 
 from __future__ import annotations
 from qtpy.QtCore import *
 from qtpy.QtGui import *
 from qtpy.QtWidgets import *
 import xarray as xr
-from xarray_tree import XarrayTreeNode
-from pyqt_ext import AbstractTreeView, KeyValueTreeItem, KeyValueTreeModel, KeyValueTreeView
+from datatree import DataTree
+from pyqt_ext.tree import TreeView, KeyValueTreeItem, KeyValueTreeModel, KeyValueTreeView
 from xarray_treeview import XarrayTreeItem, XarrayTreeModel
 
 
-class XarrayTreeView(AbstractTreeView):
+class XarrayTreeView(TreeView):
 
     def __init__(self, parent: QObject = None) -> None:
-        AbstractTreeView.__init__(self, parent)
-        # self.setSelectionMode(QAbstractItemView.MultiSelection)
-        self.setSelectionBehavior(QAbstractItemView.SelectionBehavior.SelectRows)
-
-        self.show_vars_action = QAction('Show Vars')
-        self.show_vars_action.setCheckable(True)
-        self.show_vars_action.setChecked(True)
-        self.show_vars_action.triggered.connect(self.update_model_and_view)
-
-        self.show_coords_action = QAction('Show Coords')
-        self.show_coords_action.setCheckable(True)
-        self.show_coords_action.setChecked(True)
-        self.show_coords_action.triggered.connect(self.update_model_and_view)
+        TreeView.__init__(self, parent)
 
-        # store/restore fold/selection state
-        self._state = {}
+        self.setSelectionBehavior(QAbstractItemView.SelectionBehavior.SelectRows)
 
-        # custom context menu items
-        self._custom_context_menu_actions: list[QAction] = []
+        self._showVarsAction = QAction('Show Vars')
+        self._showVarsAction.setCheckable(True)
+        self._showVarsAction.setChecked(True)
+        self._showVarsAction.triggered.connect(self.updateTree)
+
+        self._showCoordsAction = QAction('Show Coords')
+        self._showCoordsAction.setCheckable(True)
+        self._showCoordsAction.setChecked(True)
+        self._showCoordsAction.triggered.connect(self.updateTree)
     
-    def contextMenu(self, index: QModelIndex = QModelIndex()) -> QMenu:
-        menu: QMenu = AbstractTreeView.contextMenu(self, index)
-        model: XarrayTreeModel = self.model()
-        menu.addSeparator()
-        menu.addAction(self.show_vars_action)
-        menu.addAction(self.show_coords_action)
-        menu.addAction(model.show_details_column_action)
-        if not index.isValid():
-            return menu
-        item: XarrayTreeItem = model.get_item(index)
-        if self._custom_context_menu_actions:
-            menu.addSeparator()
-            for action in self._custom_context_menu_actions:
-                menu.addAction(action)
-        menu.addSeparator()
-        menu.addAction('Attrs', lambda self=self, item=item: self.edit_item_attrs(item))
-        menu.addSeparator()
-        menu.addAction('Info', lambda self=self, item=item: self.popup_item_info(item))
-        menu.addSeparator()
-        menu.addAction('Delete', lambda self=self, item=item: self.ask_to_delete_item(item))
-        return menu
+    def setModel(self, model: XarrayTreeModel):
+        root: XarrayTreeItem = model.root()
+        if root is not None:
+            options = {
+                'show_vars': self._showVarsAction.isChecked(),
+                'show_coords': self._showCoordsAction.isChecked(),
+            }
+            model.setRoot(XarrayTreeItem(node=root.node, key=None, options=options))
+        TreeView.setModel(self, model)
     
-    def update_model_and_view(self):
-        self.store_state()
+    def setTree(self, dt: DataTree):
+        self.storeState()
         options = {
-            'show_vars': self.show_vars_action.isChecked(),
-            'show_coords': self.show_coords_action.isChecked(),
+            'show_vars': self._showVarsAction.isChecked(),
+            'show_coords': self._showCoordsAction.isChecked(),
         }
+        root: XarrayTreeItem = XarrayTreeItem(dt, options=options)
         model: XarrayTreeModel = self.model()
-        model.root = XarrayTreeItem(node=model.root.node, key=None, options=options)
-        self.restore_state()
+        if model is None:
+            model = XarrayTreeModel(root)
+            self.setModel(model)
+        else:
+            model.setRoot(root)
+        self.restoreState()
     
-    def set_data(self, root_node: XarrayTreeNode):
+    def updateTree(self):
         model: XarrayTreeModel = self.model()
         if model is None:
             return
-        self.store_state()
+        root: XarrayTreeItem = model.root()
+        if root is None:
+            return
         options = {
-            'show_vars': self.show_vars_action.isChecked(),
-            'show_coords': self.show_coords_action.isChecked(),
+            'show_vars': self._showVarsAction.isChecked(),
+            'show_coords': self._showCoordsAction.isChecked(),
         }
-        model.root = XarrayTreeItem(node=root_node, key=None, options=options)
-        self.restore_state()
+        self.storeState()
+        model.setRoot(XarrayTreeItem(node=root.node, key=None, options=options))
+        self.restoreState()
+    
+    def isShowVars(self) -> bool:
+        return self._showVarsAction.isChecked()
+    
+    def setShowVars(self, show: bool):
+        self._showVarsAction.setChecked(show)
+        self.updateTree()
+    
+    def isShowCoords(self) -> bool:
+        return self._showCoordsAction.isChecked()
     
-    def store_state(self):
+    def setShowCoords(self, show: bool):
+        self._showCoordsAction.setChecked(show)
+        self.updateTree()
+    
+    def contextMenu(self, index: QModelIndex = QModelIndex()) -> QMenu:
+        menu: QMenu = TreeView.contextMenu(self, index)
         model: XarrayTreeModel = self.model()
-        if model is None:
-            return
-        selected: list[QModelIndex] = self.selectionModel().selectedIndexes()
-        item: XarrayTreeItem = model.root.next_depth_first()
-        while item is not None:
-            index: QModelIndex = model.createIndex(item.row(), 0, item)
-            path = item.path
-            self._state[path] = {
-                'expanded': self.isExpanded(index),
-                'selected': index in selected
-            }
-            item = item.next_depth_first()
+        menu.addSeparator()
+        menu.addAction(self._showVarsAction)
+        menu.addAction(self._showCoordsAction)
+        menu.addAction(model._showDetailsColumnAction)
+        if not index.isValid():
+            return menu
+        
+        item: XarrayTreeItem = model.itemFromIndex(index)
+        itemPath = item.path
+        if len(itemPath) > 50:
+            itemPath = '...' + itemPath[-47:]
+
+        itemMenu = QMenu(itemPath)
+        itemMenu.addAction('Attrs', lambda self=self, item=item: self.editItemAttrs(item))
+        itemMenu.addSeparator()
+        itemMenu.addAction('Info', lambda self=self, item=item: self.popupItemInfo(item))
+        
+        if not item.is_root():
+            itemMenu.addSeparator()
+            itemMenu.addAction('Delete', lambda self=self, item=item, label=itemPath: self.askToRemoveItem(item, label))
 
-    def restore_state(self):
-        model: XarrayTreeModel = self.model()
-        if model is None:
-            return
-        self.selectionModel().clearSelection()
-        selection: QItemSelection = QItemSelection()
-        item: XarrayTreeItem = model.root.next_depth_first()
-        while item is not None:
-            try:
-                index: QModelIndex = model.createIndex(item.row(), 0, item)
-                path = item.path
-                self.setExpanded(index, self._state[path]['expanded'])
-                if self._state[path]['selected']:
-                    selection.merge(QItemSelection(index, index), QItemSelectionModel.Select | QItemSelectionModel.Rows)
-            except KeyError:
-                self.setExpanded(index, False)
-            item = item.next_depth_first()
-        if selection.count():
-            self.selectionModel().select(selection, QItemSelectionModel.Select | QItemSelectionModel.Rows)
+        menu.insertSeparator(menu.actions()[0])
+        menu.insertMenu(menu.actions()[0], itemMenu)
+
+        return menu
     
-    def selected_items(self) -> list[XarrayTreeItem]:
-        model: XarrayTreeModel = self.model()
-        if model is None:
-            return []
-        selected: list[QModelIndex] = self.selectionModel().selectedRows()
-        items: list[XarrayTreeItem] = [model.get_item(index) for index in selected]
-        return items
-    
-    def edit_item_attrs(self, item: XarrayTreeItem):
-        ds: xr.Dataset = item.node.dataset
-        if ds is None:
-            return
+    def editItemAttrs(self, item: XarrayTreeItem):
         if item.is_node():
-            attrs = ds.attrs.copy()
-        elif item.is_var():
-            attrs = ds.data_vars[item.key].attrs.copy()
-        elif item.is_coord():
-            attrs = ds.coords[item.key].attrs.copy()
+            attrs = item.node.ds.attrs.copy()
+        elif item.is_var() or item.is_coord():
+            attrs = item.node.ds[item.key].attrs.copy()
         else:
             return
         
         root = KeyValueTreeItem('/', attrs)
         model = KeyValueTreeModel(root)
         view = KeyValueTreeView()
         view.setModel(model)
@@ -154,60 +139,114 @@
         layout.addWidget(btns)
         
         dlg.setWindowModality(Qt.ApplicationModal)
         dlg.setMinimumSize(QSize(400, 400))
         if dlg.exec() != QDialog.Accepted:
             return
         
-        attrs = model.root.to_obj()
+        attrs = model.root().value
         if item.is_node():
-            ds.attrs = attrs
-        elif item.is_var():
-            ds.data_vars[item.key].attrs = attrs
-        elif item.is_coord():
-            ds.coords[item.key].attrs = attrs
-    
-    def popup_item_info(self, item: XarrayTreeItem):
-        ds: xr.Dataset = item.node.dataset
-        if ds is None:
-            return
+            item.node.attrs = attrs
+        elif item.is_var() or item.is_coord():
+            item.node[item.key].attrs = attrs
+    
+    def popupItemInfo(self, item: XarrayTreeItem):
         if item.is_node():
-            text = str(ds)
-        elif item.is_var():
-            text = str(ds.data_vars[item.key])
-        elif item.is_coord():
-            text = str(ds.coords[item.key])
+            text = str(item.node.ds)
+        elif item.is_var() or item.is_coord():
+            text = str(item.node[item.key])
         else:
             return
         
         textEdit = QTextEdit()
         textEdit.setPlainText(text)
         textEdit.setReadOnly(True)
 
         dlg = QDialog(self)
         dlg.setWindowTitle(item.path)
         layout = QVBoxLayout(dlg)
         layout.setContentsMargins(0, 0, 0, 0)
         layout.addWidget(textEdit)
         dlg.exec()
     
-    def ask_to_delete_item(self, item: XarrayTreeItem):
-        answer = QMessageBox.question(self, 'Delete', f'Delete {item.path}?', QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No, QMessageBox.StandardButton.No)
-        if answer == QMessageBox.StandardButton.Yes:
-            model: XarrayTreeModel = self.model()
-            node: XarrayTreeNode = item.node
-            model.remove_item(item)
-            node.parent = None
-            del node
+    def dropEvent(self, event: QDropEvent):
+        src_index: QModelIndex = getattr(self, '_src_index', None)
+        if (src_index is None) or (not src_index.isValid()) or (src_index == QModelIndex()):
+            event.ignore()
+            return
+        dst_index: QModelIndex = self.indexAt(event.pos())
+        
+        model: XarrayTreeModel = self.model()
+        src_parent_index: QModelIndex = model.parent(src_index)
+        src_row = src_index.row()
+        dst_parent_index: QModelIndex = model.parent(dst_index)
+        dst_row = dst_index.row()
+
+        drop_pos = self.dropIndicatorPosition()
+        if drop_pos == QAbstractItemView.DropIndicatorPosition.OnViewport:
+            dst_parent_index = QModelIndex()
+            dst_row = model.rowCount(dst_parent_index)
+        elif drop_pos == QAbstractItemView.DropIndicatorPosition.OnItem:
+            dst_item = model.itemFromIndex(dst_index)
+            if dst_item.is_node():
+                dst_parent_index = dst_index
+                dst_row = model.rowCount(dst_parent_index)
+            elif dst_item.is_var():
+                pass # handle drops on vars?
+            elif dst_item.is_coord():
+                pass # handle drops on coords?
+        elif drop_pos == QAbstractItemView.DropIndicatorPosition.AboveItem:
+            pass
+        elif drop_pos == QAbstractItemView.DropIndicatorPosition.BelowItem:
+            dst_row += 1
+        
+        # organize child order: vars, coords, nodes
+        src_item = model.itemFromIndex(model.index(src_row, 0, src_parent_index))
+        if src_item.is_var():
+            while dst_row > 0:
+                dst_prev_item = model.itemFromIndex(model.index(dst_row - 1, 0, dst_parent_index))
+                if dst_prev_item.is_var():
+                    break
+                dst_row -= 1
+        elif src_item.is_coord():
+            while dst_row > 0:
+                dst_prev_item = model.itemFromIndex(model.index(dst_row - 1, 0, dst_parent_index))
+                if dst_prev_item.is_var() or dst_prev_item.is_coord():
+                    break
+                dst_row -= 1
+            while dst_row < model.rowCount(dst_parent_index):
+                dst_next_item = model.itemFromIndex(model.index(dst_row, 0, dst_parent_index))
+                if dst_next_item.is_coord() or dst_next_item.is_node():
+                    break
+                dst_row += 1
+        elif src_item.is_node():
+            while dst_row < model.rowCount(dst_parent_index):
+                dst_next_item = model.itemFromIndex(model.index(dst_row, 0, dst_parent_index))
+                if dst_next_item.is_node():
+                    break
+                dst_row += 1
+        
+        if event.dropAction() == Qt.DropAction.MoveAction:
+            model.moveRow(src_parent_index, src_row, dst_parent_index, dst_row)
+        else:
+            event.ignore()
+            return
+
+        # We already handled the drop event, so ignore the default implementation.
+        event.setDropAction(Qt.DropAction.IgnoreAction)
+        event.accept()
+
+        # debug
+        # print(model.root().dumps())
 
 
 def test_live():
-    import sys
     import numpy as np
-    app = QApplication(sys.argv)
+    from xarray_treeview import XarrayDndTreeModel
+    app = QApplication()
 
     raw_ds = xr.Dataset(
         data_vars={
             'current': (['series', 'sweep', 'time'], np.random.rand(3, 10, 100) * 1e-9, {'units': 'A'}),
             'voltage': (['series', 'sweep', 'time'], np.random.rand(3, 10, 100) * 10000, {'units': 'V'}),
         },
         coords={
@@ -230,30 +269,27 @@
         coords={
             'series': ('series', [1]),
             'sweep': ('sweep', [5,8]),
         },
     )
     # print('-----\n scaled_ds', scaled_ds)
     
-    root_node = XarrayTreeNode(name='/', dataset=None)
-    raw_node = XarrayTreeNode(name='raw data', dataset=raw_ds, parent=root_node)
-    baselined_node = XarrayTreeNode(name='baselined', dataset=baselined_ds, parent=raw_node)
-    scaled_node = XarrayTreeNode(name='scaled', dataset=scaled_ds, parent=baselined_node)
+    root_node = DataTree(name='root')
+    raw_node = DataTree(name='raw', data=raw_ds, parent=root_node)
+    baselined_node = DataTree(name='baselined', data=baselined_ds, parent=raw_node)
+    scaled_node = DataTree(name='scaled', data=scaled_ds, parent=baselined_node)
     # print('-----\n', root_node.to_datatree())
 
     root_item = XarrayTreeItem(root_node)
-    model = XarrayTreeModel(root_item)
+    model = XarrayDndTreeModel(root_item)
     view = XarrayTreeView()
     view.setModel(model)
     view.show()
     view.resize(QSize(600, 600))
     view.expandAll()
     view.resizeAllColumnsToContents()
 
-    # from PySide6.QtTest import *
-    # tester = QAbstractItemModelTester(model, QAbstractItemModelTester.FailureReportingMode.Fatal)
-
-    sys.exit(app.exec())
+    app.exec()
 
 
 if __name__ == '__main__':
     test_live()
```

### Comparing `xarray_treeview-1.0.2/PKG-INFO` & `xarray_treeview-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xarray-treeview
-Version: 1.0.2
+Version: 1.2.0
 Summary: PyQt/PySide model/view for tree of Xarray datasets.
-Keywords: PyQt PySide xarray tree
+Keywords: PyQt,PySide,xarray,tree
 Home-page: https://github.com/marcel-goldschen-ohm/xarray-treeview
 Author-Email: Marcel Goldschen-Ohm <goldschen-ohm@utexas.edu>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -25,14 +25,16 @@
 Requires-Dist: qtawesome>=1.3.0
 Requires-Dist: pyqt-ext>=1.1.0
 Description-Content-Type: text/markdown
 
 # xarray-treeview
 PyQt/PySide model/view for tree of Xarray datasets.
 
+:construction:
+
 # Install
 Should work with PySide6, PyQt6, or PyQt5.
 ```shell
 pip install PySide6 xarray-treeview
 ```
 
 # TODO
```

