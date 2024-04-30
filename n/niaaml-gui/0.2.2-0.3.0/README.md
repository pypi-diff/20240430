# Comparing `tmp/niaaml_gui-0.2.2.tar.gz` & `tmp/niaaml_gui-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niaaml_gui-0.2.2.tar", max compression
+gzip compressed data, was "niaaml_gui-0.3.0.tar", max compression
```

## Comparing `niaaml_gui-0.2.2.tar` & `niaaml_gui-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1069 2024-03-20 08:01:35.256839 niaaml_gui-0.2.2/LICENSE
--rw-r--r--   0        0        0     7005 2024-03-20 08:01:35.256839 niaaml_gui-0.2.2/README.md
--rw-r--r--   0        0        0      322 2024-03-20 08:01:35.256839 niaaml_gui-0.2.2/niaaml_gui/__init__.py
--rw-r--r--   0        0        0     2032 2024-03-20 08:01:35.256839 niaaml_gui-0.2.2/niaaml_gui/main.py
--rw-r--r--   0        0        0     1215 2024-03-20 08:01:35.256839 niaaml_gui-0.2.2/niaaml_gui/process_window_data.py
--rw-r--r--   0        0        0      291 2024-03-20 08:01:35.256839 niaaml_gui-0.2.2/niaaml_gui/progress_bar.py
--rw-r--r--   0        0        0      281 2024-03-20 08:01:35.256839 niaaml_gui-0.2.2/niaaml_gui/widgets/__init__.py
--rw-r--r--   0        0        0     1499 2024-03-20 08:01:35.256839 niaaml_gui-0.2.2/niaaml_gui/widgets/base_main_widget.py
--rw-r--r--   0        0        0      770 2024-03-20 08:01:35.256839 niaaml_gui-0.2.2/niaaml_gui/widgets/list_widget_custom.py
--rw-r--r--   0        0        0    15554 2024-03-20 08:01:35.256839 niaaml_gui-0.2.2/niaaml_gui/widgets/optimization_widget.py
--rw-r--r--   0        0        0     3489 2024-03-20 08:01:35.256839 niaaml_gui-0.2.2/niaaml_gui/widgets/use_pipeline_widget.py
--rw-r--r--   0        0        0      223 2024-03-20 08:01:35.257839 niaaml_gui-0.2.2/niaaml_gui/windows/__init__.py
--rw-r--r--   0        0        0     3525 2024-03-20 08:01:35.257839 niaaml_gui-0.2.2/niaaml_gui/windows/csv_editor_window.py
--rw-r--r--   0        0        0     3427 2024-03-20 08:01:35.257839 niaaml_gui-0.2.2/niaaml_gui/windows/process_window.py
--rw-r--r--   0        0        0      173 2024-03-20 08:01:35.257839 niaaml_gui-0.2.2/niaaml_gui/windows/threads/__init__.py
--rw-r--r--   0        0        0     1999 2024-03-20 08:01:35.257839 niaaml_gui-0.2.2/niaaml_gui/windows/threads/optimize_thread.py
--rw-r--r--   0        0        0      593 2024-03-20 08:01:35.257839 niaaml_gui-0.2.2/niaaml_gui/windows/threads/run_thread.py
--rw-r--r--   0        0        0      860 2024-03-20 08:01:35.258839 niaaml_gui-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     7920 1970-01-01 00:00:00.000000 niaaml_gui-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-30 18:39:11.971898 niaaml_gui-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7131 2024-04-30 18:39:11.971898 niaaml_gui-0.3.0/README.md
+-rw-r--r--   0        0        0      322 2024-04-30 18:39:11.971898 niaaml_gui-0.3.0/niaaml_gui/__init__.py
+-rw-r--r--   0        0        0     2199 2024-04-30 18:39:11.971898 niaaml_gui-0.3.0/niaaml_gui/main.py
+-rw-r--r--   0        0        0     1215 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/process_window_data.py
+-rw-r--r--   0        0        0      291 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/progress_bar.py
+-rw-r--r--   0        0        0      971 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/styles.qss
+-rw-r--r--   0        0        0      281 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/widgets/__init__.py
+-rw-r--r--   0        0        0     1499 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/widgets/base_main_widget.py
+-rw-r--r--   0        0        0      770 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/widgets/list_widget_custom.py
+-rw-r--r--   0        0        0    15746 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/widgets/optimization_widget.py
+-rw-r--r--   0        0        0     3489 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/widgets/use_pipeline_widget.py
+-rw-r--r--   0        0        0      223 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/windows/__init__.py
+-rw-r--r--   0        0        0     3544 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/windows/csv_editor_window.py
+-rw-r--r--   0        0        0     3427 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/windows/process_window.py
+-rw-r--r--   0        0        0      173 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/windows/threads/__init__.py
+-rw-r--r--   0        0        0     1999 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/windows/threads/optimize_thread.py
+-rw-r--r--   0        0        0      593 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/windows/threads/run_thread.py
+-rw-r--r--   0        0        0      862 2024-04-30 18:39:11.973898 niaaml_gui-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8048 1970-01-01 00:00:00.000000 niaaml_gui-0.3.0/PKG-INFO
```

### Comparing `niaaml_gui-0.2.2/LICENSE` & `niaaml_gui-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.2.2/README.md` & `niaaml_gui-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/niaaml-gui.svg)
 [![GitHub license](https://img.shields.io/github/license/lukapecnik/NiaAML-GUI.svg)](https://github.com/flukapecnik/NiaAML-GUI/blob/master/LICENSE)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/lukapecnik/NiaAML-GUI.svg)
 [![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/lukapecnik/NiaAML-GUI.svg)](http://isitmaintained.com/project/lukapecnik/NiaAML-GUI "Average time to resolve an issue")
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/lukapecnik/NiaAML-GUI.svg)](http://isitmaintained.com/project/lukapecnik/NiaAML-GUI "Percentage of issues still open")
 ![GitHub contributors](https://img.shields.io/github/contributors/lukapecnik/NiaAML-GUI.svg)
 [![Fedora package](https://img.shields.io/fedora/v/NiaAML-GUI?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/NiaAML-GUI)
+[![Packaging status](https://repology.org/badge/tiny-repos/niaaml-gui.svg)](https://repology.org/project/niaaml-gui/versions)
 
 ---
 
 This is a basic graphical user interface intended for users of the [NiaAML](https://github.com/lukapecnik/NiaAML) Python package.
 
 * **Python versions:** 3.9.x, 3.10.x, 3.11.x
```

### Comparing `niaaml_gui-0.2.2/niaaml_gui/main.py` & `niaaml_gui-0.3.0/niaaml_gui/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+import os
 from PyQt6.QtWidgets import QMainWindow, QMessageBox, QApplication
 from PyQt6.QtGui import QAction
 from PyQt6.QtCore import QSize
 from niaaml_gui.widgets import OptimizationWidget, UsePipelineWidget
 
 
 class MainAppWindow(QMainWindow):
@@ -44,14 +45,19 @@
     def __setUsePipelineView(self):
         self.setCentralWidget(UsePipelineWidget(self))
 
 
 def run():
     app = QApplication(sys.argv)
     app.setStyle("Fusion")
+
+    with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'styles.qss'), 'r') as f:
+        style = f.read()
+        app.setStyleSheet(style)
+
     mainWin = MainAppWindow()
     mainWin.show()
     sys.exit(app.exec())
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `niaaml_gui-0.2.2/niaaml_gui/process_window_data.py` & `niaaml_gui-0.3.0/niaaml_gui/process_window_data.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.2.2/niaaml_gui/widgets/base_main_widget.py` & `niaaml_gui-0.3.0/niaaml_gui/widgets/base_main_widget.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.2.2/niaaml_gui/widgets/list_widget_custom.py` & `niaaml_gui-0.3.0/niaaml_gui/widgets/list_widget_custom.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.2.2/niaaml_gui/widgets/optimization_widget.py` & `niaaml_gui-0.3.0/niaaml_gui/widgets/optimization_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     QVBoxLayout,
     QGridLayout,
     QTabWidget,
     QFileDialog,
     QCheckBox,
 )
 from PyQt6.QtGui import QRegularExpressionValidator
-from PyQt6.QtCore import QRegularExpression
+from PyQt6.QtCore import QRegularExpression, Qt
 from niapy.util.factory import _algorithm_options
 from niaaml_gui.widgets.list_widget_custom import ListWidgetCustom
 from niaaml_gui.widgets.base_main_widget import BaseMainWidget
 from niaaml_gui.windows import ProcessWindow
 from niaaml_gui.process_window_data import ProcessWindowData
 from niaaml.classifiers import ClassifierFactory
 from niaaml.preprocessing.feature_selection import FeatureSelectionAlgorithmFactory
@@ -55,30 +55,31 @@
         self.__niaamlClassifiersList.sort()
         self.__is_v1 = is_v1
         super().__init__(parent, *args, **kwargs)
 
         fileLayout = QHBoxLayout(self._parent)
 
         selectFileBar = QHBoxLayout(self._parent)
-        selectFileBar.setSpacing(0)
+        selectFileBar.setSpacing(5)
         selectFileBar.setContentsMargins(0, 5, 5, 5)
         fNameLine = QLineEdit(self._parent)
         fNameLine.setObjectName("csvFile")
         fNameLine.setPlaceholderText("Select a CSV dataset file...")
         fNameLine.setReadOnly(True)
         font = fNameLine.font()
         font.setPointSize(12)
         fNameLine.setFont(font)
         selectFileBar.addWidget(fNameLine)
         editBtn = self._createButton(
-            None, self._editCSVFile, "editCSVButton", qta.icon("fa5.edit")
+            None, self._editCSVFile, "editCSVButton", qta.icon("fa5.edit", color_off='white')
         )
         editBtn.setEnabled(False)
         selectFileBar.addWidget(editBtn)
-        selectFileBar.addWidget(self._createButton("Select file", self._openCSVFile))
+        selectFileBar.addWidget(self._createButton(None, self._openCSVFile,
+                                                   icon=qta.icon("fa5.file", color_off='white')))
 
         checkBox = QCheckBox("CSV has header")
         checkBox.setObjectName("csv")
         checkBox.setFont(font)
 
         fileLayout.addItem(selectFileBar)
         fileLayout.addWidget(checkBox)
@@ -167,16 +168,17 @@
         foNameLine.setPlaceholderText("Select pipeline output folder...")
         foNameLine.setReadOnly(True)
         font = foNameLine.font()
         font.setPointSize(12)
         foNameLine.setFont(font)
         selectOutputFolderBar.addWidget(foNameLine)
         selectOutputFolderBar.addWidget(
-            self._createButton("Select folder", self.__selectDirectory)
+            self._createButton(None, self.__selectDirectory, icon=qta.icon('fa5.folder', color_off='white'))
         )
+        selectOutputFolderBar.setSpacing(5)
 
         settingsBox.addItem(optAlgos)
         if not self.__is_v1:
             settingsBox.addItem(optAlgosInner)
         settingsBox.addItem(popSize)
         if not self.__is_v1:
             settingsBox.addItem(popSizeInner)
@@ -223,15 +225,15 @@
         for k in items:
             cb.addItem(k)
         comboBox.addWidget(label)
         comboBox.addWidget(cb)
         return comboBox
 
     def __createTextInput(self, label, name, validator=None):
-        textBox = QVBoxLayout()
+        textBox = QHBoxLayout()
         textBox.setSpacing(5)
         label = QLabel(label, self._parent)
         font = label.font()
         font.setPointSize(12)
         label.setFont(font)
         tb = QLineEdit(self._parent)
         tb.setObjectName(name)
```

### Comparing `niaaml_gui-0.2.2/niaaml_gui/widgets/use_pipeline_widget.py` & `niaaml_gui-0.3.0/niaaml_gui/widgets/use_pipeline_widget.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.2.2/niaaml_gui/windows/csv_editor_window.py` & `niaaml_gui-0.3.0/niaaml_gui/windows/csv_editor_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             return
 
         centralWidget = QWidget(self)
         layout = QVBoxLayout(centralWidget)
 
         toolBar = QHBoxLayout(centralWidget)
         toolBar.setAlignment(Qt.AlignmentFlag.AlignLeft)
-        saveBtn = self.__createButton(None, self.__save, None, qta.icon("fa5.save"))
+        saveBtn = self.__createButton(None, self.__save, None, qta.icon("fa5.save", color_off='white'))
         toolBar.addWidget(saveBtn)
 
         layout.addItem(toolBar)
         layout.addWidget(self.__table)
 
         centralWidget.setLayout(layout)
         self.setCentralWidget(centralWidget)
```

### Comparing `niaaml_gui-0.2.2/niaaml_gui/windows/process_window.py` & `niaaml_gui-0.3.0/niaaml_gui/windows/process_window.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.2.2/niaaml_gui/windows/threads/optimize_thread.py` & `niaaml_gui-0.3.0/niaaml_gui/windows/threads/optimize_thread.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.2.2/niaaml_gui/windows/threads/run_thread.py` & `niaaml_gui-0.3.0/niaaml_gui/windows/threads/run_thread.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.2.2/pyproject.toml` & `niaaml_gui-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "NiaAML-GUI"
-version = "0.2.2"
+version = "0.3.0"
 description = "GUI for NiaAML Python package"
 license = "MIT"
 authors = ["Luka Pečnik <lukapecnik96@gmail.com>"]
 keywords = ['classification', 'NiaPy', 'NiaAML', 'scikit-learn', 'nature-inspired algorithms', 'feature selection', 'preprocessing']
-homepage = "https://github.com/lukapecnik/NiaAML-GUI"
-repository = "https://github.com/lukapecnik/NiaAML-GUI"
+homepage = "https://github.com/firefly-cpp/NiaAML-GUI"
+repository = "https://github.com/firefly-cpp/NiaAML-GUI"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 niapy = "^2.0.5"
 QtAwesome = "^1.2.3"
 niaaml = "^1.2.0"
```

### Comparing `niaaml_gui-0.2.2/PKG-INFO` & `niaaml_gui-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: niaaml-gui
-Version: 0.2.2
+Version: 0.3.0
 Summary: GUI for NiaAML Python package
-Home-page: https://github.com/lukapecnik/NiaAML-GUI
+Home-page: https://github.com/firefly-cpp/NiaAML-GUI
 License: MIT
 Keywords: classification,NiaPy,NiaAML,scikit-learn,nature-inspired algorithms,feature selection,preprocessing
 Author: Luka Pečnik
 Author-email: lukapecnik96@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: QtAwesome (>=1.2.3,<2.0.0)
 Requires-Dist: niaaml (>=1.2.0,<2.0.0)
 Requires-Dist: niapy (>=2.0.5,<3.0.0)
 Requires-Dist: pyqt6 (>=6.6.0,<7.0.0)
 Requires-Dist: scikit-learn (>=1.3.2,<2.0.0)
-Project-URL: Repository, https://github.com/lukapecnik/NiaAML-GUI
+Project-URL: Repository, https://github.com/firefly-cpp/NiaAML-GUI
 Description-Content-Type: text/markdown
 
 # NiaAML-GUI
 
 ---
 
 [![PyPI Version](https://img.shields.io/pypi/v/niaaml-gui.svg)](https://pypi.python.org/pypi/niaaml-gui)
@@ -30,14 +30,15 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/niaaml-gui.svg)
 [![GitHub license](https://img.shields.io/github/license/lukapecnik/NiaAML-GUI.svg)](https://github.com/flukapecnik/NiaAML-GUI/blob/master/LICENSE)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/lukapecnik/NiaAML-GUI.svg)
 [![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/lukapecnik/NiaAML-GUI.svg)](http://isitmaintained.com/project/lukapecnik/NiaAML-GUI "Average time to resolve an issue")
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/lukapecnik/NiaAML-GUI.svg)](http://isitmaintained.com/project/lukapecnik/NiaAML-GUI "Percentage of issues still open")
 ![GitHub contributors](https://img.shields.io/github/contributors/lukapecnik/NiaAML-GUI.svg)
 [![Fedora package](https://img.shields.io/fedora/v/NiaAML-GUI?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/NiaAML-GUI)
+[![Packaging status](https://repology.org/badge/tiny-repos/niaaml-gui.svg)](https://repology.org/project/niaaml-gui/versions)
 
 ---
 
 This is a basic graphical user interface intended for users of the [NiaAML](https://github.com/lukapecnik/NiaAML) Python package.
 
 * **Python versions:** 3.9.x, 3.10.x, 3.11.x
```

