# Comparing `tmp/meni-0.1.2.tar.gz` & `tmp/meni-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meni-0.1.2.tar", max compression
+gzip compressed data, was "meni-0.1.5.tar", max compression
```

## Comparing `meni-0.1.2.tar` & `meni-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1490 2024-03-19 20:22:26.653713 meni-0.1.2/LICENSE
--rw-r--r--   0        0        0     2046 2024-04-18 18:18:05.428346 meni-0.1.2/README.md
--rw-r--r--   0        0        0      150 2024-04-18 03:56:58.735096 meni-0.1.2/meni/__init__.py
--rw-r--r--   0        0        0      872 2024-04-28 23:42:55.444189 meni-0.1.2/meni/__main__.py
--rw-r--r--   0        0        0     2439 2024-04-27 03:58:58.344925 meni-0.1.2/meni/app.py
--rw-r--r--   0        0        0    10717 2024-04-27 04:00:10.714310 meni-0.1.2/meni/model/model.py
--rw-r--r--   0        0        0     4699 2024-04-27 04:02:08.300488 meni-0.1.2/meni/rc_assets.py
--rw-r--r--   0        0        0     4766 2024-04-27 03:59:03.609027 meni-0.1.2/meni/theme.py
--rw-r--r--   0        0        0     3017 2024-04-27 03:59:57.822066 meni-0.1.2/meni/ui/common.py
--rw-r--r--   0        0        0    12600 2024-04-27 03:59:43.493793 meni-0.1.2/meni/ui/docks/browser.py
--rw-r--r--   0        0        0     3580 2024-04-27 03:59:45.393829 meni-0.1.2/meni/ui/docks/collectionproperties.py
--rw-r--r--   0        0        0     3279 2024-04-27 03:59:46.609852 meni-0.1.2/meni/ui/docks/fileproperties.py
--rw-r--r--   0        0        0     4363 2024-04-27 03:59:47.845876 meni-0.1.2/meni/ui/docks/viewer.py
--rw-r--r--   0        0        0     7768 2024-04-27 03:59:58.830085 meni-0.1.2/meni/ui/filestable.py
--rw-r--r--   0        0        0     4817 2024-04-27 04:00:00.386114 meni-0.1.2/meni/ui/flowlayout.py
--rw-r--r--   0        0        0     2019 2024-04-27 03:59:49.117900 meni-0.1.2/meni/ui/menus/filecontextmenu.py
--rw-r--r--   0        0        0      799 2024-04-27 03:59:51.205940 meni-0.1.2/meni/ui/menus/menusettings.py
--rw-r--r--   0        0        0     3168 2024-04-27 15:05:41.987610 meni-0.1.2/meni/ui/propertyrowwithapply.py
--rw-r--r--   0        0        0     1219 2024-04-27 04:00:04.394190 meni-0.1.2/meni/ui/searchinput.py
--rw-r--r--   0        0        0     1341 2024-04-27 04:00:05.746216 meni-0.1.2/meni/ui/tagrow.py
--rw-r--r--   0        0        0     7500 2024-04-27 03:59:53.969992 meni-0.1.2/meni/ui/windows/importdialog.py
--rw-r--r--   0        0        0     7901 2024-04-27 03:59:55.014012 meni-0.1.2/meni/ui/windows/mainwindow.py
--rw-r--r--   0        0        0     4683 2024-04-27 03:59:56.626043 meni-0.1.2/meni/ui/windows/welcome.py
--rw-r--r--   0        0        0     1148 2024-04-27 03:59:06.161076 meni-0.1.2/meni/utils.py
--rw-r--r--   0        0        0      880 2024-04-27 03:59:08.129114 meni-0.1.2/meni/worker.py
--rw-r--r--   0        0        0     1178 2024-04-28 23:47:15.739864 meni-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 meni-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1490 2024-03-19 20:22:26.653713 meni-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2046 2024-04-18 18:18:05.428346 meni-0.1.5/README.md
+-rw-r--r--   0        0        0       61 2024-04-29 16:56:27.214798 meni-0.1.5/meni/__init__.py
+-rw-r--r--   0        0        0     1374 2024-04-30 13:33:44.850293 meni-0.1.5/meni/__main__.py
+-rw-r--r--   0        0        0     2439 2024-04-27 03:58:58.344925 meni-0.1.5/meni/app.py
+-rw-r--r--   0        0        0    10717 2024-04-27 04:00:10.714310 meni-0.1.5/meni/model/model.py
+-rw-r--r--   0        0        0     4699 2024-04-30 13:32:13.989462 meni-0.1.5/meni/rc_assets.py
+-rw-r--r--   0        0        0     4766 2024-04-27 03:59:03.609027 meni-0.1.5/meni/theme.py
+-rw-r--r--   0        0        0     3017 2024-04-27 03:59:57.822066 meni-0.1.5/meni/ui/common.py
+-rw-r--r--   0        0        0    12600 2024-04-27 03:59:43.493793 meni-0.1.5/meni/ui/docks/browser.py
+-rw-r--r--   0        0        0     3580 2024-04-27 03:59:45.393829 meni-0.1.5/meni/ui/docks/collectionproperties.py
+-rw-r--r--   0        0        0     3279 2024-04-27 03:59:46.609852 meni-0.1.5/meni/ui/docks/fileproperties.py
+-rw-r--r--   0        0        0     4363 2024-04-27 03:59:47.845876 meni-0.1.5/meni/ui/docks/viewer.py
+-rw-r--r--   0        0        0     7768 2024-04-27 03:59:58.830085 meni-0.1.5/meni/ui/filestable.py
+-rw-r--r--   0        0        0     4817 2024-04-27 04:00:00.386114 meni-0.1.5/meni/ui/flowlayout.py
+-rw-r--r--   0        0        0     2019 2024-04-27 03:59:49.117900 meni-0.1.5/meni/ui/menus/filecontextmenu.py
+-rw-r--r--   0        0        0      799 2024-04-27 03:59:51.205940 meni-0.1.5/meni/ui/menus/menusettings.py
+-rw-r--r--   0        0        0     3168 2024-04-27 15:05:41.987610 meni-0.1.5/meni/ui/propertyrowwithapply.py
+-rw-r--r--   0        0        0     1219 2024-04-27 04:00:04.394190 meni-0.1.5/meni/ui/searchinput.py
+-rw-r--r--   0        0        0     1341 2024-04-27 04:00:05.746216 meni-0.1.5/meni/ui/tagrow.py
+-rw-r--r--   0        0        0     7500 2024-04-27 03:59:53.969992 meni-0.1.5/meni/ui/windows/importdialog.py
+-rw-r--r--   0        0        0     7975 2024-04-29 16:58:33.476370 meni-0.1.5/meni/ui/windows/mainwindow.py
+-rw-r--r--   0        0        0     4645 2024-04-30 13:32:58.805870 meni-0.1.5/meni/ui/windows/welcome.py
+-rw-r--r--   0        0        0     1148 2024-04-27 03:59:06.161076 meni-0.1.5/meni/utils.py
+-rw-r--r--   0        0        0      880 2024-04-27 03:59:08.129114 meni-0.1.5/meni/worker.py
+-rw-r--r--   0        0        0     1178 2024-04-30 13:34:38.258789 meni-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 meni-0.1.5/PKG-INFO
```

### Comparing `meni-0.1.2/LICENSE` & `meni-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/README.md` & `meni-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/__main__.py` & `meni-0.1.5/meni/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,42 @@
+import importlib.metadata
 from PySide6 import QtWidgets, QtCore
 from qt_material import apply_stylesheet
 from meni.ui.windows.mainwindow import MainWindow
 from meni.ui.windows.welcome import WelcomeWindow
 from meni.app import AppMeni
 import sys
 import argparse
+import os
+import importlib
 
 
 def main():
     parser = argparse.ArgumentParser(description="Meni: Library manager for 3D models and assets.")
     parser.add_argument("-l", "--library", help="Path to the library directory.")
+    parser.add_argument("-w", "--wayland", help="Support for wayland (set QT_QPA_PLATFORM=xcb)", action="store_true")
+    parser.add_argument("-v", "--version", action="version", version=f"meni {importlib.metadata.version('meni')}")
+    parser.add_argument("--welcome", help="Show welcome screen", action="store_true")
     args = parser.parse_args()
 
+    if args.wayland:
+        os.environ["QT_QPA_PLATFORM"] = "xcb"
+
     app = AppMeni(sys.argv, library=args.library)
 
     # app.setStyleSheet(qdarkstyle.load_stylesheet_pyside6())
 
     # setup stylesheet
     # apply_stylesheet(app, theme="dark_teal.xml")
     # extra = {"density_scale": "-3"}
     # apply_stylesheet(app, "dark_teal.xml", invert_secondary=False, extra=extra, save_as="stylesheet.css")
 
-    app.startup()
+    if args.welcome:
+        app.show_welcome()
+    else:
+        app.startup()
 
     app.exec()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `meni-0.1.2/meni/app.py` & `meni-0.1.5/meni/app.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/model/model.py` & `meni-0.1.5/meni/model/model.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/rc_assets.py` & `meni-0.1.5/meni/rc_assets.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/theme.py` & `meni-0.1.5/meni/theme.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/ui/common.py` & `meni-0.1.5/meni/ui/common.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/ui/docks/browser.py` & `meni-0.1.5/meni/ui/docks/browser.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/ui/docks/collectionproperties.py` & `meni-0.1.5/meni/ui/docks/collectionproperties.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/ui/docks/fileproperties.py` & `meni-0.1.5/meni/ui/docks/fileproperties.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/ui/docks/viewer.py` & `meni-0.1.5/meni/ui/docks/viewer.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/ui/filestable.py` & `meni-0.1.5/meni/ui/filestable.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/ui/flowlayout.py` & `meni-0.1.5/meni/ui/flowlayout.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/ui/menus/filecontextmenu.py` & `meni-0.1.5/meni/ui/menus/filecontextmenu.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/ui/menus/menusettings.py` & `meni-0.1.5/meni/ui/menus/menusettings.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/ui/propertyrowwithapply.py` & `meni-0.1.5/meni/ui/propertyrowwithapply.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/ui/searchinput.py` & `meni-0.1.5/meni/ui/searchinput.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/ui/tagrow.py` & `meni-0.1.5/meni/ui/tagrow.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/ui/windows/importdialog.py` & `meni-0.1.5/meni/ui/windows/importdialog.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/ui/windows/mainwindow.py` & `meni-0.1.5/meni/ui/windows/mainwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from meni.ui.menus.menusettings import MenuSettings
 from meni.ui.docks.collectionproperties import CollectionPropertiesDock
 from meni.ui.docks.fileproperties import FilePropertiesDock
 from meni.ui.docks.viewer import ViewerDock
 from meni.ui.docks.browser import BrowserDock
 from meni.ui.common import DockTitleBar
 import qtawesome as qta
+import importlib
 
 
 class MainWindow(QtWidgets.QMainWindow):
     def __init__(self):
         super().__init__()
 
         self.app = QtCore.QCoreApplication.instance()
@@ -170,15 +171,16 @@
     def on_open_library_folder(self):
         folder = QtWidgets.QFileDialog.getExistingDirectory(None, "Select a folder")
         if folder:
             self.app.current_library = folder
             self.app.metadata.changed.emit()
 
     def on_about(self):
+        version = importlib.metadata.version("meni")
         QtWidgets.QMessageBox.about(
             self,
             "About Meni",
             f"""
             <h1>Meni</h1>
-            <p>Version: 0.1.0</p>
+            <p>Version: {version}</p>
             """,
         )
```

### Comparing `meni-0.1.2/meni/ui/windows/welcome.py` & `meni-0.1.5/meni/ui/windows/welcome.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,17 +28,15 @@
 
         self.layout = QtWidgets.QVBoxLayout(self)
         self.layout.setContentsMargins(30, 15, 30, 15)
 
         # Logo (logo.svg)
         self.logo = QtWidgets.QLabel()
         self.logo.setPixmap(
-            pxmap_from_svg(":/assets/logo.svg", color=self.app.theme.icon_color).scaled(
-                120, 120, QtCore.Qt.KeepAspectRatio, QtCore.Qt.SmoothTransformation
-            )
+            pxmap_from_svg(":logo.svg", color=self.app.theme.icon_color).scaled(120, 120, QtCore.Qt.KeepAspectRatio, QtCore.Qt.SmoothTransformation)
         )
 
         self.logo.setAlignment(QtCore.Qt.AlignCenter)
         self.layout.addWidget(self.logo, 0)
 
         # Panel
         self.panel = QtWidgets.QFrame()
```

### Comparing `meni-0.1.2/meni/utils.py` & `meni-0.1.5/meni/utils.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/meni/worker.py` & `meni-0.1.5/meni/worker.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.2/pyproject.toml` & `meni-0.1.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meni"
-version = "0.1.2"
+version = "0.1.5"
 description = "Software to manage a library of 3d files (stl)"
 authors = ["Diego Pereyra <diego@diegopereyra.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [{ include = "meni" }]
 homepage = "https://github.com/diesphink/meni"
 repository = "https://github.com/diesphink/meni"
```

### Comparing `meni-0.1.2/PKG-INFO` & `meni-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meni
-Version: 0.1.2
+Version: 0.1.5
 Summary: Software to manage a library of 3d files (stl)
 Home-page: https://github.com/diesphink/meni
 License: BSD-3-Clause
 Author: Diego Pereyra
 Author-email: diego@diegopereyra.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: meni Version: 0.1.2 Summary: Software to manage a
+Metadata-Version: 2.1 Name: meni Version: 0.1.5 Summary: Software to manage a
 library of 3d files (stl) Home-page: https://github.com/diesphink/meni License:
 BSD-3-Clause Author: Diego Pereyra Author-email: diego@diegopereyra.com
 Requires-Python: >=3.9,<3.13 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: X11 Applications :: Qt Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: End Users/Desktop Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
```

