# Comparing `tmp/silicon_analyser-1.1.0.tar.gz` & `tmp/silicon_analyser-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silicon_analyser-1.1.0.tar", last modified: Sat Apr 20 16:59:42 2024, max compression
+gzip compressed data, was "silicon_analyser-1.1.1.tar", last modified: Tue Apr 30 13:02:55 2024, max compression
```

## Comparing `silicon_analyser-1.1.0.tar` & `silicon_analyser-1.1.1.tar`

### file list

```diff
@@ -1,39 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 16:59:41.000000 silicon_analyser-1.1.0/
--rw-rw-rw-   0        0        0     1087 2024-04-07 16:13:23.000000 silicon_analyser-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     3379 2024-04-20 16:59:42.000000 silicon_analyser-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2575 2024-04-20 10:31:11.000000 silicon_analyser-1.1.0/README.md
--rw-rw-rw-   0        0        0     1154 2024-04-20 11:22:18.000000 silicon_analyser-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-20 16:59:42.000000 silicon_analyser-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-20 16:59:41.000000 silicon_analyser-1.1.0/silicon_analyser/
-drwxrwxrwx   0        0        0        0 2024-04-20 16:59:41.000000 silicon_analyser-1.1.0/silicon_analyser/dialogs/
--rw-rw-rw-   0        0        0     3487 2024-04-13 14:15:10.000000 silicon_analyser-1.1.0/silicon_analyser/dialogs/compute_stats.py
--rw-rw-rw-   0        0        0     1508 2024-04-06 18:45:56.000000 silicon_analyser-1.1.0/silicon_analyser/dialogs/compute_stats.ui
--rw-rw-rw-   0        0        0     3340 2024-04-14 09:21:04.000000 silicon_analyser-1.1.0/silicon_analyser/dialogs/pixel_image.py
--rw-rw-rw-   0        0        0     3752 2024-04-14 09:20:00.000000 silicon_analyser-1.1.0/silicon_analyser/dialogs/pixel_image.ui
--rw-rw-rw-   0        0        0     5152 2024-04-20 10:50:22.000000 silicon_analyser-1.1.0/silicon_analyser/grid.py
-drwxrwxrwx   0        0        0        0 2024-04-20 16:59:41.000000 silicon_analyser-1.1.0/silicon_analyser/helper/
-drwxrwxrwx   0        0        0        0 2024-04-20 16:59:41.000000 silicon_analyser-1.1.0/silicon_analyser/helper/abstract/
--rw-rw-rw-   0        0        0     2563 2024-04-20 14:08:21.000000 silicon_analyser-1.1.0/silicon_analyser/helper/abstract/abstractimage.py
--rw-rw-rw-   0        0        0     3006 2024-04-20 08:48:27.000000 silicon_analyser-1.1.0/silicon_analyser/helper/abstract/abstractmywindow.py
--rw-rw-rw-   0        0        0     1024 2024-04-13 06:54:26.000000 silicon_analyser-1.1.0/silicon_analyser/helper/abstract/abstracttreehelper.py
--rw-rw-rw-   0        0        0      719 2024-04-13 07:29:28.000000 silicon_analyser-1.1.0/silicon_analyser/helper/addgridbtn.py
--rw-rw-rw-   0        0        0      696 2024-04-08 17:17:53.000000 silicon_analyser-1.1.0/silicon_analyser/helper/addlabelbtn.py
--rw-rw-rw-   0        0        0     1874 2024-04-20 16:34:45.000000 silicon_analyser-1.1.0/silicon_analyser/helper/ai.py
--rw-rw-rw-   0        0        0    17433 2024-04-20 16:23:43.000000 silicon_analyser-1.1.0/silicon_analyser/helper/computebtn.py
--rw-rw-rw-   0        0        0    21550 2024-04-20 16:28:29.000000 silicon_analyser-1.1.0/silicon_analyser/helper/fullimage.py
--rw-rw-rw-   0        0        0     1581 2024-04-20 14:51:25.000000 silicon_analyser-1.1.0/silicon_analyser/helper/minimap.py
--rw-rw-rw-   0        0        0     4051 2024-04-20 08:17:04.000000 silicon_analyser-1.1.0/silicon_analyser/helper/properties.py
--rw-rw-rw-   0        0        0    23821 2024-04-20 10:45:19.000000 silicon_analyser-1.1.0/silicon_analyser/helper/tree.py
--rw-rw-rw-   0        0        0      263 2024-04-08 17:15:10.000000 silicon_analyser-1.1.0/silicon_analyser/main.py
--rw-rw-rw-   0        0        0     8314 2024-04-20 08:47:52.000000 silicon_analyser-1.1.0/silicon_analyser/main_window.ui
--rw-rw-rw-   0        0        0    10672 2024-04-20 14:43:13.000000 silicon_analyser-1.1.0/silicon_analyser/mywindow.py
--rw-rw-rw-   0        0        0      134 2024-04-07 08:11:27.000000 silicon_analyser-1.1.0/silicon_analyser/rect.py
--rw-rw-rw-   0        0        0     2305 2024-04-16 18:10:57.000000 silicon_analyser-1.1.0/silicon_analyser/savefiles.py
--rw-rw-rw-   0        0        0     1365 2024-04-13 14:16:41.000000 silicon_analyser-1.1.0/silicon_analyser/treeitem.py
-drwxrwxrwx   0        0        0        0 2024-04-20 16:59:41.000000 silicon_analyser-1.1.0/silicon_analyser.egg-info/
--rw-rw-rw-   0        0        0     3379 2024-04-20 16:59:41.000000 silicon_analyser-1.1.0/silicon_analyser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1078 2024-04-20 16:59:41.000000 silicon_analyser-1.1.0/silicon_analyser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 16:59:41.000000 silicon_analyser-1.1.0/silicon_analyser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-20 16:59:41.000000 silicon_analyser-1.1.0/silicon_analyser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2024-04-20 16:59:41.000000 silicon_analyser-1.1.0/silicon_analyser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-20 16:59:41.000000 silicon_analyser-1.1.0/silicon_analyser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 13:02:55.000000 silicon_analyser-1.1.1/
+-rw-rw-rw-   0        0        0     1087 2024-04-07 16:13:23.000000 silicon_analyser-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4311 2024-04-30 13:02:55.000000 silicon_analyser-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2024-04-30 09:20:21.000000 silicon_analyser-1.1.1/README.md
+-rw-rw-rw-   0        0        0     1154 2024-04-26 16:18:30.000000 silicon_analyser-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 13:02:55.000000 silicon_analyser-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 13:02:55.000000 silicon_analyser-1.1.1/silicon_analyser/
+drwxrwxrwx   0        0        0        0 2024-04-30 13:02:55.000000 silicon_analyser-1.1.1/silicon_analyser/dialogs/
+-rw-rw-rw-   0        0        0     3498 2024-04-22 16:35:39.000000 silicon_analyser-1.1.1/silicon_analyser/dialogs/compute_stats.py
+-rw-rw-rw-   0        0        0     1508 2024-04-06 18:45:56.000000 silicon_analyser-1.1.1/silicon_analyser/dialogs/compute_stats.ui
+-rw-rw-rw-   0        0        0     3340 2024-04-14 09:21:04.000000 silicon_analyser-1.1.1/silicon_analyser/dialogs/pixel_image.py
+-rw-rw-rw-   0        0        0     3752 2024-04-14 09:20:00.000000 silicon_analyser-1.1.1/silicon_analyser/dialogs/pixel_image.ui
+-rw-rw-rw-   0        0        0     7101 2024-04-30 09:09:19.000000 silicon_analyser-1.1.1/silicon_analyser/grid.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:02:55.000000 silicon_analyser-1.1.1/silicon_analyser/helper/
+drwxrwxrwx   0        0        0        0 2024-04-30 13:02:55.000000 silicon_analyser-1.1.1/silicon_analyser/helper/abstract/
+-rw-rw-rw-   0        0        0     1216 2024-04-28 14:03:52.000000 silicon_analyser-1.1.1/silicon_analyser/helper/abstract/abstractcomputationmethod.py
+-rw-rw-rw-   0        0        0     3343 2024-04-28 10:31:38.000000 silicon_analyser-1.1.1/silicon_analyser/helper/abstract/abstractimage.py
+-rw-rw-rw-   0        0        0     5105 2024-04-30 08:42:30.000000 silicon_analyser-1.1.1/silicon_analyser/helper/abstract/abstractmywindow.py
+-rw-rw-rw-   0        0        0     1228 2024-04-28 10:31:28.000000 silicon_analyser-1.1.1/silicon_analyser/helper/abstract/abstracttreehelper.py
+-rw-rw-rw-   0        0        0      822 2024-04-28 15:33:17.000000 silicon_analyser-1.1.1/silicon_analyser/helper/addgridbtn.py
+-rw-rw-rw-   0        0        0      807 2024-04-28 15:33:35.000000 silicon_analyser-1.1.1/silicon_analyser/helper/addlabelbtn.py
+-rw-rw-rw-   0        0        0     8164 2024-04-29 07:22:01.000000 silicon_analyser-1.1.1/silicon_analyser/helper/ai.py
+-rw-rw-rw-   0        0        0    10439 2024-04-29 18:39:51.000000 silicon_analyser-1.1.1/silicon_analyser/helper/autocomputebtn.py
+-rw-rw-rw-   0        0        0      253 2024-04-27 07:10:56.000000 silicon_analyser-1.1.1/silicon_analyser/helper/common.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:02:55.000000 silicon_analyser-1.1.1/silicon_analyser/helper/computation_methods/
+-rw-rw-rw-   0        0        0     2256 2024-04-28 14:03:19.000000 silicon_analyser-1.1.1/silicon_analyser/helper/computation_methods/decision_tree.py
+-rw-rw-rw-   0        0        0     6071 2024-04-29 07:45:09.000000 silicon_analyser-1.1.1/silicon_analyser/helper/computation_methods/neural_network.py
+-rw-rw-rw-   0        0        0     6431 2024-04-30 09:33:38.000000 silicon_analyser-1.1.1/silicon_analyser/helper/computebtn.py
+-rw-rw-rw-   0        0        0    22053 2024-04-29 17:36:07.000000 silicon_analyser-1.1.1/silicon_analyser/helper/fullimage.py
+-rw-rw-rw-   0        0        0     1656 2024-04-28 10:50:37.000000 silicon_analyser-1.1.1/silicon_analyser/helper/minimap.py
+-rw-rw-rw-   0        0        0     4067 2024-04-29 17:34:25.000000 silicon_analyser-1.1.1/silicon_analyser/helper/properties.py
+-rw-rw-rw-   0        0        0    28973 2024-04-30 09:03:39.000000 silicon_analyser-1.1.1/silicon_analyser/helper/tree.py
+-rw-rw-rw-   0        0        0      411 2024-04-28 11:15:06.000000 silicon_analyser-1.1.1/silicon_analyser/main.py
+-rw-rw-rw-   0        0        0    10105 2024-04-30 09:14:05.000000 silicon_analyser-1.1.1/silicon_analyser/main_window.ui
+-rw-rw-rw-   0        0        0    13963 2024-04-30 08:42:06.000000 silicon_analyser-1.1.1/silicon_analyser/mywindow.py
+-rw-rw-rw-   0        0        0      134 2024-04-07 08:11:27.000000 silicon_analyser-1.1.1/silicon_analyser/rect.py
+-rw-rw-rw-   0        0        0     3460 2024-04-29 18:27:14.000000 silicon_analyser-1.1.1/silicon_analyser/savefiles.py
+-rw-rw-rw-   0        0        0     1450 2024-04-27 08:35:13.000000 silicon_analyser-1.1.1/silicon_analyser/treeitem.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:02:55.000000 silicon_analyser-1.1.1/silicon_analyser.egg-info/
+-rw-rw-rw-   0        0        0     4311 2024-04-30 13:02:55.000000 silicon_analyser-1.1.1/silicon_analyser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1339 2024-04-30 13:02:55.000000 silicon_analyser-1.1.1/silicon_analyser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 13:02:55.000000 silicon_analyser-1.1.1/silicon_analyser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-30 13:02:55.000000 silicon_analyser-1.1.1/silicon_analyser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2024-04-30 13:02:55.000000 silicon_analyser-1.1.1/silicon_analyser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-30 13:02:55.000000 silicon_analyser-1.1.1/silicon_analyser.egg-info/top_level.txt
```

### Comparing `silicon_analyser-1.1.0/LICENSE` & `silicon_analyser-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.1.0/PKG-INFO` & `silicon_analyser-1.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,29 @@
-Metadata-Version: 2.1
-Name: silicon-analyser
-Version: 1.1.0
-Summary: helps to analyse integrated circuit die images (for example from siliconpr0n.org) with the help of ai.
-Author-email: CrazyT <crazyt2019+sa@gmail.com>
-Project-URL: Homepage, https://github.com/TheCrazyT/SiliconAnalyser
-Project-URL: Bug Tracker, https://github.com/TheCrazyT/SiliconAnalyser/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch
-Requires-Dist: numpy
-Requires-Dist: pillow
-Requires-Dist: keras
-Requires-Dist: PyQt5
-Requires-Dist: pyqtgraph
-Requires-Dist: scikit-learn
-Requires-Dist: packaging
-
 # Installation
 
 Install from source:
 
 `pip install --upgrade .`
 
 Install from pip:
 
 `pip install --upgrade silicon-analyser`
 
 # Information
 
-Code will use your graphic card for acceleration.
+## Side note
+Bad project name decisions might lead people to this project.
+
+Maybe you are looking for [SiliconAnalysis](https://github.com/SiliconAnalysis/) instead?
+
+I'm sorry for that but I can't figure out any new project name (yet).
+
+## Acceleration
+
+The code will use your graphic card for acceleration.
 (but only if correct pytorch is installed, see "Additional info" below)
 
 Frameworks/Libraries used:
 * [PyQt5](https://www.riverbankcomputing.com/software/pyqt/)
 * [PyTorch](https://pytorch.org/)
 * [Keras](https://keras.io/)
 * [PyQtGraph](https://www.pyqtgraph.org/)
@@ -67,27 +54,40 @@
     * "acc" stands for "accuracy", "val" for "validation"
 * found ai-cells will be drawn green
 
 # Additional info
 
 * you might need to install cuda-specific [PyTorch](https://pytorch.org/get-started/previous-versions/#linux-and-windows-4) for accelerated computing
     * check your graphic driver version for compatible cuda version!
+* Computation (currently) only happens based on active/visible grid cells (don't be fooled by accuracy of 1 just because you have only 1 label active - just activate all and use compute)
+
+## Command line
+
+For automatically opening a file, you can pass the filepath as a filename.
+For example:
+  silicon-analyser c:\my_files\image.png
+But keep in mind, that the program currently needs to create files in its current working directory (grid.json, rect.json).
 
 # Keys
 
 * Use up/down/left/right to navigate
 * Hold shift to move faster
 * Scroll-wheel to zoom out
 * Click on minimap to get directly to a position
 * Right click on tree-items (left navigation menu) for additional options
+* Hold down middle mouse button, to move across the screen
+  * (behaviour might change in future, currently it does not behave as expected)
 
 ![image](https://raw.githubusercontent.com/TheCrazyT/SiliconAnalyser/main/docs/small_tutorial.gif)
 
 # TODO
 
+* undo option
+* maybe use a real db in background
+* some method to autofit grid
+* performance improvements
+* option for compute to continue from last training (currently starts fresh training)
 * show loading screen on start (pytorch with cuda support takes a bit to load)
-* option to calculate/classify by decision tree
-* auto-compute to calculate in background while you are selecting new cells for your labels
 * ai-model configuration
 * project management (project-file/-folder)
 * possibility to rotate grid
 * maybe store your model on a public place? (for others to use)
```

### Comparing `silicon_analyser-1.1.0/pyproject.toml` & `silicon_analyser-1.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "silicon-analyser"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="CrazyT", email="crazyt2019+sa@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `silicon_analyser-1.1.0/silicon_analyser/dialogs/compute_stats.py` & `silicon_analyser-1.1.1/silicon_analyser/dialogs/compute_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     _accuracygraph: PlotWidget
     _loss: typing.Any
     _val_loss: typing.Any
     _accuracy: typing.Any
     _val_accuracy: typing.Any
     _lblStatus: QLabel
     _btnStop: QPushButton
-    request_graph_update = pyqtSignal([dict,int])
+    request_graph_update:pyqtSignal = pyqtSignal([dict,int])
     
     def __init__(self):
         super().__init__()
         uic.loadUi(p.abspath(p.join(p.dirname(__file__), '.')) + '/compute_stats.ui', self)
         self._loss = linspace(0,0,self.width())
         self._val_loss = linspace(0,0,self.width())
         self._accuracy = linspace(0,0,self.width())
```

### Comparing `silicon_analyser-1.1.0/silicon_analyser/dialogs/compute_stats.ui` & `silicon_analyser-1.1.1/silicon_analyser/dialogs/compute_stats.ui`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.1.0/silicon_analyser/dialogs/pixel_image.py` & `silicon_analyser-1.1.1/silicon_analyser/dialogs/pixel_image.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.1.0/silicon_analyser/dialogs/pixel_image.ui` & `silicon_analyser-1.1.1/silicon_analyser/dialogs/pixel_image.ui`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.1.0/silicon_analyser/grid.py` & `silicon_analyser-1.1.1/silicon_analyser/grid.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+logger = logging.getLogger(__name__)
 from functools import lru_cache
 
 
 class Grid:
     _rects: dict[str,list[list[int]]]
     _rectsActive: dict[str,bool]
     def __init__(self, name, x, y, cols, rows, width, height):
@@ -13,15 +15,15 @@
         self.width = width
         self.height = height
         self.shearX = 0
         self.shearY = 0
         self._rects = {}
         self._rectsActive = {}
         self.recalcCell()
-        print(f"init grid:{id(self)}")
+        logger.info(f"init grid:{id(self)}")
     
     def recalcCell(self):
         self._cellWidth = self.width / self.cols
         self._cellHeight = self.height / self.rows
     
     def getCellWidth(self) -> float:
         return self._cellWidth
@@ -72,63 +74,112 @@
         self._rectsActive[text] = True
     
     def rectDeactive(self, text):
         self.isRectSet.cache_clear()
         self.rectLabel.cache_clear()
         self._rectsActive[text] = False
         
+    def addRightColumn(self):
+        self.isRectSet.cache_clear()
+        self.rectLabel.cache_clear()
+        self.width += int(self.getCellWidth())
+        self.cols += 1
+
+    def addLeftColumn(self):
+        self.isRectSet.cache_clear()
+        self.rectLabel.cache_clear()
+        self.x -= int(self.getCellWidth())
+        self.width += int(self.getCellWidth())
+        self.cols += 1
+        for label in self._rects:
+            for i in range(0,len(self._rects[label])):
+                col, row = self._rects[label][i]
+                self._rects[label][i] = [col+1, row]
+
+    def removeRightColumn(self):
+        self.isRectSet.cache_clear()
+        self.rectLabel.cache_clear()
+        self.width -= int(self.getCellWidth())
+        self.cols -= 1
+
+    def removeLeftColumn(self):
+        self.isRectSet.cache_clear()
+        self.rectLabel.cache_clear()
+        for label in self._rects:
+            delEntries = []
+            for i in range(0,len(self._rects[label])):
+                col, row = self._rects[label][i]
+                if col - 1 < 0:
+                    delEntries.append(i)
+                else:
+                    self._rects[label][i] = [col-1, row]
+            delEntries = sorted(delEntries, reverse=True)
+            for i in delEntries:
+                del self._rects[label][i]
+        self.x += int(self.getCellWidth())
+        self.width -= int(self.getCellWidth())
+        self.cols -= 1
+        
     def addTopRow(self):
-        self.y -= int(self.height/self.rows)
-        self.height += int(self.height/self.rows)
+        self.isRectSet.cache_clear()
+        self.rectLabel.cache_clear()
+        self.y -= int(self.getCellHeight())
+        self.height += int(self.getCellHeight())
         self.rows += 1
         for label in self._rects:
             for i in range(0,len(self._rects[label])):
                 col, row = self._rects[label][i]
                 self._rects[label][i] = [col, row+1]
 
     def addBottomRow(self):
-        self.height += int(self.height/self.rows)
+        self.isRectSet.cache_clear()
+        self.rectLabel.cache_clear()
+        self.height += int(self.getCellHeight())
         self.rows += 1
         
     def removeTopRow(self):
+        self.isRectSet.cache_clear()
+        self.rectLabel.cache_clear()
         for label in self._rects:
             delEntries = []
             for i in range(0,len(self._rects[label])):
                 col, row = self._rects[label][i]
                 if row - 1 < 0:
                     delEntries.append(i)
                 else:
                     self._rects[label][i] = [col, row-1]
             delEntries = sorted(delEntries, reverse=True)
             for i in delEntries:
                 del self._rects[label][i]
-        self.y += int(self.height/self.rows)
-        self.height -= int(self.height/self.rows)
+        self.y += int(self.getCellHeight())
+        self.height -= int(self.getCellHeight())
         self.rows -= 1
 
     def removeBottomRow(self):
-        self.height -= int(self.height/self.rows)
+        self.isRectSet.cache_clear()
+        self.rectLabel.cache_clear()
+        self.height -= int(self.getCellHeight())
         self.rows -= 1
     
     def setRect(self, col, row, label):
         self.isRectSet.cache_clear()
         self.rectLabel.cache_clear()
-        #print(f"setRect {col} {row} {label}")
+        #logger.info(f"setRect {col} {row} {label}")
         r = [col, row]
         if label not in self._rects:
             self._rects[label] = []
         for lbl in self._rects.keys():
             if r in self._rects[lbl]:
                 self._rects[lbl].remove(r)
         self._rects[label].append(r)
         
     def unsetRect(self, col, row, label):
         self.isRectSet.cache_clear()
         self.rectLabel.cache_clear()
-        print(f"unsetRect {col} {row}")
+        logger.info(f"unsetRect {col} {row}")
         r = [col, row]
         if r in self._rects[label]:
             self._rects[label].remove(r)
     
     @lru_cache(maxsize=None)
     def rectLabel(self, col, row) -> str|None:
         r = [col, row]
@@ -149,13 +200,17 @@
             if self._rectsActive[k] and r in self._rects[k]:
                 return True
         return False
 
     def getRects(self, key: str) -> list[list[int]]:
         return self._rects[key]
     
+    def getRectLabelsActive(self) -> dict[str,bool]:
+        return self._rectsActive
+    
 def getAllCellRects(grid: Grid):
     cellRects = []
     for cx in range(0,grid.cols):
         for cy in range(0,grid.rows):
             cellRects.append((cx,cy))
-    return cellRects
+    return cellRects
+
```

### Comparing `silicon_analyser-1.1.0/silicon_analyser/helper/abstract/abstractimage.py` & `silicon_analyser-1.1.1/silicon_analyser/helper/abstract/abstractimage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,122 @@
+import abc
 from PyQt5.QtWidgets import QLabel
+from PyQt5.QtCore import pyqtSignal
 import typing
 import numpy as np
 from silicon_analyser.grid import Grid
 from silicon_analyser.rect import Rect
 
 class AbstractImage(QLabel):
+    onRectChanged: pyqtSignal
     
+    @abc.abstractmethod
     def getImageHeight(self) -> int:
         raise NotImplementedError()
 
+    @abc.abstractmethod
     def getImageWidth(self) -> int:
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def clearAIRects(self):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def fetchData(self,x,y,ex,ey) -> np.ndarray[int,typing.Any]:
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def drawImage(self):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def fetchFullData(self) -> np.ndarray[int,typing.Any]:
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def appendRectGroup(self, text):
          raise NotImplementedError()
 
+    @abc.abstractmethod
     def appendAIRectGroup(self, text):
          raise NotImplementedError()
     
+    @abc.abstractmethod
     def appendGridRectGroup(self, grid, text):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def appendAIGridRectGroup(self, grid, text):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def activateGridRectGroup(self, grid, text):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def deactivateGridRectGroup(self, grid, text):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def activateAIGridRectGroup(self, grid, text):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def deactivateAIGridRectGroup(self, grid, text):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def activateRectGroup(self, text):
         raise NotImplementedError()
 
+    @abc.abstractmethod
     def deactivateRectGroup(self, text):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def activateAIRectGroup(self, text):
         raise NotImplementedError()
 
+    @abc.abstractmethod
     def deactivateAIRectGroup(self, text):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def appendAIRect(self,key,x,y,ex,ey):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def appendAIGrid(self, text):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def activateAIGrid(self, text):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def getRects(self) -> dict[str,Rect]:
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def getGrids(self) -> dict[str,Grid]:
          raise NotImplementedError()
     
+    @abc.abstractmethod
     def removeRectGroup(self, label):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def removeGrid(self, label):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def appendGrid(self, text):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def activateGrid(self, text):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def getAIIgnoreRects(self) -> list:
         raise NotImplementedError()
```

### Comparing `silicon_analyser-1.1.0/silicon_analyser/helper/abstract/abstracttreehelper.py` & `silicon_analyser-1.1.1/silicon_analyser/helper/abstract/abstracttreehelper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,42 @@
+import abc
 from PyQt5.QtCore import pyqtSignal
 from PyQt5.QtGui import QStandardItem
 from PyQt5.QtWidgets import QTreeView
 
 from silicon_analyser.grid import Grid
 from silicon_analyser.treeitem import TreeItem
 
 class AbstractTreeHelper(QTreeView):
     evtTreeSelectionChanged: pyqtSignal
     
+    @abc.abstractmethod
     def selectedType(self) -> str:
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def selectedLabel(self) -> str:
         raise NotImplementedError()
 
+    @abc.abstractmethod
     def getSelectedItem(self) -> QStandardItem:
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def getSelectedGrid(self):
        raise NotImplementedError()
 
+    @abc.abstractmethod
     def getSelectedAIGrid(self):
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def isItemSelected(self, rectLabel, gridName, gridItemType) -> bool:
         raise NotImplementedError()
-            
+    
+    @abc.abstractmethod
     def addTreeItem(self, text, type="auto", parent_obj=None, parent_item=None) -> tuple[Grid, TreeItem]:
         raise NotImplementedError()
     
+    @abc.abstractmethod
     def clearAIItem(self):
         raise NotImplementedError()
```

### Comparing `silicon_analyser-1.1.0/silicon_analyser/helper/addgridbtn.py` & `silicon_analyser-1.1.1/silicon_analyser/helper/addgridbtn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,23 @@
+import logging
+logger = logging.getLogger(__name__)
+
 from PyQt5.QtWidgets import QInputDialog, QPushButton
 from PyQt5.QtGui import QMouseEvent
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
 from silicon_analyser.treeitem import TreeItem
 
 class AddGridBtn(QPushButton):
     def __init__(self, text: str):
         QPushButton.__init__(self, text)
         self.clicked.connect(self.buttonClicked)
         self._gridIdx = 0
 
     def buttonClicked(self, event: QMouseEvent):
         print("AddGridBtn: buttonClicked")
-        self._myWindow.getTree().addTreeItem("grid_%d" % self._gridIdx,TreeItem.TYPE_GRID)
+        tree = self._myWindow.getTree()
+        tree.addTreeItem("grid_%d" % self._gridIdx,TreeItem.TYPE_GRID)
+        tree.expandAll()
         self._gridIdx += 1
     
     def initialize(self, myWindow: AbstractMyWindow):
         self._myWindow = myWindow
```

### Comparing `silicon_analyser-1.1.0/silicon_analyser/helper/addlabelbtn.py` & `silicon_analyser-1.1.1/silicon_analyser/helper/addlabelbtn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+import logging
+logger = logging.getLogger(__name__)
+
 from PyQt5.QtWidgets import QInputDialog, QPushButton
 from PyQt5.QtGui import QMouseEvent
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
 
 class AddLabelBtn(QPushButton):
     def __init__(self, text: str):
         QPushButton.__init__(self, text)
         self.clicked.connect(self.buttonClicked)
 
     def buttonClicked(self, event: QMouseEvent):
         print("AddLabelBtn: buttonClicked")
         text, ok = QInputDialog.getText(self, 'Label Input Dialog', 'Enter your label:')
         if ok:
-            self._myWindow.getTree().addTreeItem(text)
+            tree = self._myWindow.getTree()
+            tree.addTreeItem(text)
+            tree.expandAll()
             
     def initialize(self, myWindow: AbstractMyWindow):
         self._myWindow = myWindow
```

### Comparing `silicon_analyser-1.1.0/silicon_analyser/helper/fullimage.py` & `silicon_analyser-1.1.1/silicon_analyser/helper/fullimage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from functools import lru_cache
-from PyQt5.QtCore import Qt, QRect, QSize, QTimer
+import inspect
+import logging
+logger = logging.getLogger(__name__)
+
+from PyQt5.QtCore import Qt, QRect, QSize, QTimer, pyqtSignal
 from PyQt5.QtWidgets import QLabel, QSizePolicy
 from PyQt5.QtGui import QImage, QPixmap, QColor, QMouseEvent, QPainter, QPen, QBrush
 import typing
 import numpy as np
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
-from silicon_analyser.savefiles import triggerSaveGrids, triggerSaveRects, saveGrids, saveRects
 from silicon_analyser.grid import Grid
 from silicon_analyser.rect import Rect
 from silicon_analyser.treeitem import TreeItem
 
 class FullImage(QLabel):
     _rects: dict[str, list[Rect]]
     _aiRects: dict[str, list[Rect]]
@@ -20,14 +22,15 @@
     _aiGridsActive: dict[str, bool]
     _moveStartX: int
     _moveStartY: int
     _moveDeltaX: int
     _moveDeltaY: int
     _moveTimer: QTimer
     _saveTimer: QTimer
+    onRectChanged = pyqtSignal()
     
     def __init__(self, parent):
         QLabel.__init__(self, parent)
         self._drawRectStart = False
         self._rectStartX = 0
         self._rectStartY = 0
         self._rectEndX = 0
@@ -48,16 +51,16 @@
         self._moveStart = False
         self._saveTimer = QTimer()
         self._saveTimer.timeout.connect(self.doSave)
         self._saveTimer.setInterval(int(1000 * 10)) #save every 10 seconds
         self._saveTimer.start()
     
     def doSave(self):
-        saveRects(self._rects)
-        saveGrids(self._grids)
+        self._myWindow.getSaving().saveRects(self._rects)
+        self._myWindow.getSaving().saveGrids(self._grids)
         
     def moveUpdate(self):
         posX, posY = self._myWindow.getPos()
         posX += self._moveDeltaX
         posY += self._moveDeltaY
         self._myWindow.setPosX(posX)
         self._myWindow.setPosY(posY)
@@ -96,32 +99,34 @@
                 if x < evx and y < evy and ex > evx and ey > evy:
                     tevx = self._translateEventToPixel(evx)
                     tevy = self._translateEventToPixel(evy)
                     rx = grid.x - posX
                     ry = grid.y - posY
                     if button == Qt.MouseButton.LeftButton:
                         grid.setRect(int((tevx - rx)/(grid.getCellWidth())),int((tevy - ry)/(grid.getCellHeight())), self._myWindow.getTree().selectedLabel())
+                        self.onRectChanged.emit()
                     if button == Qt.MouseButton.RightButton:
                         grid.unsetRect(int((tevx - rx)/(grid.getCellWidth())),int((tevy - ry)/(grid.getCellHeight())), self._myWindow.getTree().selectedLabel())
+                        self.onRectChanged.emit()
                     if self._myWindow.autosave:
-                        triggerSaveGrids()
+                        self._myWindow.getSaving().triggerSaveGrids()
                     
     def mousePressEvent(self, event: QMouseEvent):
         if event.button() == Qt.MouseButton.MiddleButton:
             self._moveStart = True
             self._moveStartX = event.x()
             self._moveStartY = event.y()
             self._moveDeltaX = 0
             self._moveDeltaY = 0
         tree = self._myWindow.getTree()
         if tree.selectedType() == TreeItem.TYPE_GRID_ITEM:
             self.markGridItem(event.x(),event.y(),event.button())
             return
         if event.button() == Qt.MouseButton.LeftButton:
-            print("FullImage: mousePressEvent",self._drawRectStart)
+            logger.info(f"FullImage: mousePressEvent:{self._drawRectStart}")
             if tree.selectedType() is not None:
                 if not self._drawRectStart:
                     self._drawRectStart = True
                     self._rectStartX = self._translateEventToPixel(event.x())
                     self._rectStartY = self._translateEventToPixel(event.y())
     
     def mouseMoveEvent(self, event: QMouseEvent) -> None:
@@ -154,15 +159,15 @@
     def mouseReleaseEvent(self, event: QMouseEvent):
         if event.button() == Qt.MouseButton.MiddleButton:
             self._moveStart = False
             self._moveTimer.stop()
             
         if event.button() == Qt.MouseButton.LeftButton:
             self._drawRectStart = False
-            print("mouseReleaseEvent",self._rectStartX,self._rectStartY,self._rectEndX,self._rectEndY)
+            logger.info(f"mouseReleaseEvent:{self._rectStartX},{self._rectStartY},{self._rectEndX},{self._rectEndY}")
             selectedKey: str = self._myWindow.getTree().selectedLabel()
             if selectedKey is not None:
                 x = self._rectStartX
                 y = self._rectStartY
                 ex = self._rectEndX
                 ey = self._rectEndY
                 if selectedKey in self._rects:
@@ -172,21 +177,21 @@
                     posX, posY = self._myWindow.getPos()
                     grid.x = posX+x
                     grid.y = posY+y
                     grid.width = ex-x
                     grid.height = ey-y
                     grid.recalcCell()
                     self._grids[selectedKey] = grid
-                    print(f"grid resized: {id(grid)}")
+                    logger.info(f"grid resized: {id(grid)}")
                     self._myWindow.reloadProperyWindowByGrid(grid)
                     if self._myWindow.autosave:
-                        triggerSaveGrids()
+                        self._myWindow.getSaving().triggerSaveGrids()
                 self.drawImage()
         if event.button() == Qt.MouseButton.RightButton:
-            print("right click")
+            logger.info("right click")
             self.removeRectAt(event.x(),event.y())
     
     def removeRectGroup(self, label):
         self._rects.pop(label, None)
         self._aiRects.pop(label, None)
         self._rectActive.pop(label, None)
         self._aiRectActive.pop(label, None)
@@ -215,15 +220,15 @@
                     if ex < x:
                         x,ex = ex,x
                     if ey < y:
                         y,ey = ey,y
                     if x < evx and y < evy and ex > evx and ey > evy:
                         toRemove.append(i)
             for i in  sorted(toRemove, reverse=True):
-                print(f"remove {i}")
+                logger.info(f"remove {i}")
                 del self._rects[k][i]
         
         for k in self._aiRects.keys():
             toRemove = []
             if self._aiRectActive[k]:
                 for i in range(0,len(self._aiRects[k])):
                     rect: Rect = self._aiRects[k][i]
@@ -236,27 +241,27 @@
                     if ex<x:
                         x,ex = ex,x
                     if ey<y:
                         y,ey = ey,y
                     if x<evx and y<evy and ex>evx and ey>evy:
                         toRemove.append(i)
             for i in sorted(toRemove, reverse=True):
-                print(f"remove {i}")
+                logger.info(f"remove {i}")
                 self._aiIgnoreRects.append(self._aiRects[k][i])
                 del self._aiRects[k][i]
                 
         self.drawImage()
         if  self._myWindow.autosave:
-            triggerSaveRects()
-            triggerSaveGrids()
+            self._myWindow.getSaving().triggerSaveRects()
+            self._myWindow.getSaving().triggerSaveGrids()
 
     def appendRect(self,key,x,y,ex,ey):
         self._appendRect(key, self._rects, x, y, ex, ey)
         if self._myWindow.autosave:
-            triggerSaveRects()
+            self._myWindow.getSaving().triggerSaveRects()
 
     def _appendRect(self, key, rects, x, y, ex, ey, ignorePos = False):
         if ignorePos:
             rects[key].append(Rect(
                 x,
                 y,
                 ex,
@@ -301,18 +306,18 @@
     def _translateEventToPixel(self, v):
         return int(v/self._myWindow.getScale())
     
     def _translatePixelToScaled(self, v):
         return int(v*self._myWindow.getScale())
     
     def clearAIRects(self):
-        self._aiGridsActive = {}
-        self._aiGrids = {}
-        self._aiRects = {}
-        self._aiRectActive = {}
+        self._aiGridsActive.clear()
+        self._aiGrids.clear()
+        self._aiRects.clear()
+        self._aiRectActive.clear()
     
     # TODO: maybe deprecated, not shure yet
     def drawRectOnScaledImg(self, scaledImg: QPixmap):
         qp = QPainter(scaledImg)
         brush = QBrush(QColor(0,0,255,80))
         pen = QPen(Qt.GlobalColor.blue, 2)
         qp.setBrush(brush)
@@ -433,14 +438,18 @@
                     ey = int(self._translatePixelToScaled(ey)-sposY)
                     w = ex - x
                     h = ey - y
                     if x>=0 and y>=0 and x<=self.width() and y<=self.height():
                         qp.drawRect(x,y,w,h)
 
     def drawImage(self):
+        idx = 1
+        stack = inspect.stack()
+        logger.info(f"drawImage {stack[idx].filename},{stack[idx].lineno}")
+        #logger.info(f"drawImage")
         posX, posY = self._myWindow.getPos()
         scale = self._myWindow.getScale()
         rect = QRect(int(posX), int(posY), int(self.width()/scale), int(self.height()/scale))
         cropped = self._pixmap.copy(rect)
         scaled = cropped.scaled(QSize(int(self.width()), int(self.height())))
         self._currentImg = scaled
         self.drawRectOnScaledImg(scaled)
@@ -456,20 +465,19 @@
         return aiGrid
     
     def appendGrid(self, text):
         grid = Grid(text,0,0,20,20,20*10,20*10)
         self._grids[text] = grid
         self._myWindow.reloadProperyWindowByGrid(grid)
         if self._myWindow.autosave:
-            triggerSaveGrids()
+            self._myWindow.getSaving().triggerSaveGrids()
         return self._grids[text]
     
     def activateAIGrid(self, text):
         self._aiGridsActive[text] = True
-        self.drawImage()
 
     def activateGrid(self, text: str):
         self._gridsActive[text] = True
         self.drawImage()
 
     def deactivateGrid(self, text: str):
         self._gridsActive[text] = False
```

### Comparing `silicon_analyser-1.1.0/silicon_analyser/helper/minimap.py` & `silicon_analyser-1.1.1/silicon_analyser/helper/minimap.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+import logging
+logger = logging.getLogger(__name__)
+
 from PyQt5.QtWidgets import QLabel
 from PyQt5.QtCore import QSize, Qt
 from PyQt5.QtGui import QPixmap, QPainter, QPen, QMouseEvent
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
 
 class MiniMap(QLabel):
     def __init__(self, parent):
         QLabel.__init__(self, parent)
     
     def initialize(self, myWindow: AbstractMyWindow, pixmap: QPixmap):
         self._myWindow = myWindow
         self._pixmap = pixmap
         
     def mouseReleaseEvent(self,event: QMouseEvent):
-        print("clicked")
+        logger.info("clicked")
         sc1x = 300/self._pixmap.width()
         sc1y = 300/self._pixmap.height()
         self._myWindow.setPosX(int(event.x()/sc1x))
         self._myWindow.setPosY(int(event.y()/sc1y))
         self._myWindow.drawImgAndMinimap()
-        print(self._myWindow.getPosX(),self._myWindow.getPosY())
+        logger.info(f"{self._myWindow.getPosX()},{self._myWindow.getPosY()}")
 
     def scaleMinimapX(self):
         return 300/self._pixmap.width()
     
     def scaleMinimapY(self):
         return 300/self._pixmap.height()
```

### Comparing `silicon_analyser-1.1.0/silicon_analyser/helper/properties.py` & `silicon_analyser-1.1.1/silicon_analyser/helper/properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
+import logging
+logger = logging.getLogger(__name__)
+
 import typing
 from PyQt5.QtWidgets import QTableView
 from PyQt5.QtCore import QItemSelection, QModelIndex, Qt, QAbstractItemModel
 from PyQt5.QtGui import QStandardItem, QStandardItemModel
-from silicon_analyser.savefiles import saveGrids
 from silicon_analyser.grid import Grid
 from silicon_analyser.treeitem import TreeItem
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
 
 class PropertiesUtil:
     def __init__(self, myWindow: AbstractMyWindow,properties: QTableView):
         self._properties = properties
         self._myWindow = myWindow
         properties.model().dataChanged.connect(self.dataChanged)
     
     def dataChanged(self,*args,**kwargs):
-        print("dataChanged")
+        logger.info("dataChanged")
         valueCol: QModelIndex = args[0]
         if valueCol.column() != 1:
             return
         row = valueCol.row()
         model: QStandardItemModel = typing.cast(QStandardItemModel,self._properties.model())
         nameCol = model.item(row,0)
         name = nameCol.data(Qt.ItemDataRole.DisplayRole)
         value = valueCol.data(Qt.ItemDataRole.DisplayRole)
-        print(f"{name}: {value}")
+        logger.info(f"{name}: {value}")
         grid: Grid = self._myWindow.getTree().getSelectedGrid()
         if(name == "cols"):
             grid.cols = int(value)
             grid.recalcCell()
         if(name == "rows"):
             grid.rows = int(value)
             grid.recalcCell()
@@ -42,15 +44,15 @@
             grid.height = int(value)
             grid.recalcCell()
         if(name == "shearX"):
             grid.shearX = float(value)
         if(name == "shearY"):
             grid.shearY = float(value)
         self._myWindow.getImage().drawImage()
-        saveGrids(self._myWindow.getImage().getGrids())
+        self._myWindow.getSaving().triggerSaveGrids()
     
     def reloadPropertyWindow(self,selection: QItemSelection):
         table: QTableView = self._properties
         model = table.model()
         model.removeRows(0,model.rowCount())
         cnt = selection.count()
         if(cnt == 0):
```

### Comparing `silicon_analyser-1.1.0/silicon_analyser/helper/tree.py` & `silicon_analyser-1.1.1/silicon_analyser/helper/tree.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import logging
+logger = logging.getLogger(__name__)
+
 from PIL import Image
 import typing
 import numpy as np
 import re
 from PyQt5.QtCore import QItemSelection, pyqtSignal, QItemSelectionModel
 from PyQt5 import QtCore
 from PyQt5.QtWidgets import QTreeView, QWidget, QAction, QFileDialog, QInputDialog
@@ -16,14 +19,18 @@
 
 class Tree(AbstractTreeHelper):
     _myWindow: AbstractMyWindow
     _actionGridAddXRowsBottom: QAction
     _actionGridAddXRowsTop: QAction
     _actionGridRemoveXRowsBottom: QAction
     _actionGridRemoveXRowsTop: QAction
+    _actionGridAddXColumnsLeft: QAction
+    _actionGridAddXColumnsRight: QAction
+    _actionGridRemoveXColumnsLeft: QAction
+    _actionGridRemoveXColumnsRight: QAction
     _actionSaveModel: QAction
     _actionLoadModel: QAction
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionSaveAsCsv: QAction
     _actionViewAsPixelimage: QAction
     _actionExportCellsToImages: QAction
@@ -43,40 +50,52 @@
         self._actionSaveAsCsv = self._myWindow._actionSaveAsCsv
         self._actionViewAsPixelimage = self._myWindow._actionViewAsPixelimage
         self._actionExportCellsToImages = self._myWindow._actionExportCellsToImages
         self._actionGridAddXRowsTop = self._myWindow._actionGridAddXRowsTop
         self._actionGridAddXRowsBottom = self._myWindow._actionGridAddXRowsBottom
         self._actionGridRemoveXRowsTop = self._myWindow._actionGridRemoveXRowsTop
         self._actionGridRemoveXRowsBottom = self._myWindow._actionGridRemoveXRowsBottom
+        self._actionGridAddXColumnsLeft = self._myWindow._actionGridAddXColumnsLeft
+        self._actionGridAddXColumnsRight = self._myWindow._actionGridAddXColumnsRight
+        self._actionGridRemoveXColumnsLeft = self._myWindow._actionGridRemoveXColumnsLeft
+        self._actionGridRemoveXColumnsRight = self._myWindow._actionGridRemoveXColumnsRight
         self.addAction(self._actionGridAddXRowsTop)
         self.addAction(self._actionGridAddXRowsBottom)
         self.addAction(self._actionGridRemoveXRowsTop)
         self.addAction(self._actionGridRemoveXRowsBottom)
+        self.addAction(self._actionGridAddXColumnsLeft)
+        self.addAction(self._actionGridAddXColumnsRight)
+        self.addAction(self._actionGridRemoveXColumnsLeft)
+        self.addAction(self._actionGridRemoveXColumnsRight)
         self.addAction(self._actionSaveModel)
         self.addAction(self._actionLoadModel)
         self.addAction(self._actionRemoveGrid)
         self.addAction(self._actionRemoveLabel)
         self.addAction(self._actionSaveAsCsv)
         self.addAction(self._actionViewAsPixelimage)
         self.addAction(self._actionExportCellsToImages)
         self._actionGridAddXRowsTop.triggered.connect(self.addTopRows)
         self._actionGridAddXRowsBottom.triggered.connect(self.addBottomRows)
         self._actionGridRemoveXRowsTop.triggered.connect(self.removeTopRows)
         self._actionGridRemoveXRowsBottom.triggered.connect(self.removeBottomRows)
+        self._actionGridAddXColumnsLeft.triggered.connect(self.addLeftColumns)
+        self._actionGridAddXColumnsRight.triggered.connect(self.addRightColumns)
+        self._actionGridRemoveXColumnsLeft.triggered.connect(self.removeLeftColumns)
+        self._actionGridRemoveXColumnsRight.triggered.connect(self.removeRightColumns)
         self._actionSaveModel.triggered.connect(self.saveModel)
         self._actionLoadModel.triggered.connect(self.loadModel)
         self._actionRemoveGrid.triggered.connect(self.removeGrid)
         self._actionRemoveLabel.triggered.connect(self.removeLabel)
         self._actionSaveAsCsv.triggered.connect(self.saveAsCsv)
         self._actionViewAsPixelimage.triggered.connect(self.viewAsPixelimage)
         self._actionExportCellsToImages.triggered.connect(self.exportCellsToImages)
         self._pixelImageDlg = PixelImageDlg()
     
     def exportCellsToImages(self, *args, **kwargs):
-        print("exportCellsToImages")
+        logger.info("exportCellsToImages")
         grid: Grid|None = self.getSelectedGrid()
         if grid is None:
             return
         dlg: QFileDialog = QFileDialog()
         dlg.setLabelText(QFileDialog.DialogLabel.Accept, "Save")
         directoryPath: str = dlg.getExistingDirectory()
         if directoryPath is not None:
@@ -90,33 +109,33 @@
                   clean_label = re.sub("[^A-Za-z0-9]","_",label)
                   imgArr = np.zeros(arr.shape,np.uint8)
                   imgArr[:,:,0] = arr[:,:,2]
                   imgArr[:,:,1] = arr[:,:,1]
                   imgArr[:,:,2] = arr[:,:,0]
                   imgToSave = Image.fromarray(imgArr)
                   imgToSave.save(f"{directoryPath}/{clean_label}_{x:03}_{y:03}.png","PNG")
-        print("exportCellsToImages done")
+        logger.info("exportCellsToImages done")
 
     def viewAsPixelimage(self, *args, **kwargs):
-        print("viewAsPixelimage")
+        logger.info("viewAsPixelimage")
         grid: Grid|None
         selectedType = self.selectedType()
         if selectedType == TreeItem.TYPE_GRID_ITEM:
             grid = self.getSelectedGrid()
         elif selectedType == TreeItem.TYPE_AI_GRID_ITEM:
             grid = self.getSelectedAIGrid()
         if grid is None:
             return
         label = self.selectedLabel()
         if label is not None: 
             self._pixelImageDlg.show()
             self._pixelImageDlg.drawRects(grid.getRects(label))
     
     def saveAsCsv(self, *args, **kwargs):
-        print("saveAsCsv")
+        logger.info("saveAsCsv")
         dlg = QFileDialog()
         dlg.setLabelText(QFileDialog.DialogLabel.Accept, "Save")
         filenames = []
         filenames = dlg.getSaveFileName(caption="Save csv",filter="Comma separated values (*.csv)",initialFilter="Comma separated values (*.csv)")
         if(len(filenames) >= 1):
             grid:Grid|None
             if self.selectedType() == TreeItem.TYPE_GRID:
@@ -140,57 +159,62 @@
                                 break
                         if not labelFound:
                             cells.append(f'')
                     f.write(",".join(cells))
                     f.write("\n")
     
     def saveModel(self, *args, **kwargs):
-        print("saveModel")
+        logger.info("saveModel")
         dlg = QFileDialog()
         dlg.setLabelText(QFileDialog.DialogLabel.Accept, "Save")
         filenames = []
         filenames = dlg.getSaveFileName(caption="Save trained model",filter="Trained model (*.h5)",initialFilter="Trained model (*.h5)")
         if(len(filenames) >= 1):
+            import os
+            os.environ["KERAS_BACKEND"] = "torch"
             from keras.models import Sequential
             grid = self.getSelectedGrid()
             if grid is not None:
                 model: Sequential = self._myWindow.getModel(grid.name)
                 model.save(filenames[0])
     
     
     def recreateAiTree(self, grid:Grid):
         self.clearAIItem(grid.name)
         aiGrid, aiTreeItem = self.addTreeItem(grid.name,TreeItem.TYPE_AI_GRID)
         for l in grid.getLabels():
             self.addTreeItem(l,TreeItem.TYPE_AI_GRID_ITEM,aiGrid,aiTreeItem)
+        self.expandAll()
         return aiGrid
     
     def loadModel(self, *args, **kwargs):
-        print("loadModel")
+        logger.info("loadModel")
         myWindow: AbstractMyWindow = self._myWindow
         dlg = QFileDialog()
         dlg.setFileMode(QFileDialog.ExistingFile)
         dlg.setNameFilter("Trained model (*.h5)")
         filenames = []
         if dlg.exec_():
             filenames = dlg.selectedFiles()
         if(len(filenames) == 1):
+            import os
+            os.environ["KERAS_BACKEND"] = "torch"
             from keras.models import load_model
             from silicon_analyser.helper.ai import appendFoundCellRects
             grid: Grid|None = self.getSelectedGrid()
             if grid is not None:
                 model = load_model(filenames[0])
                 aiGrid = self.recreateAiTree(grid)
                 myWindow.setLastModel(grid.name, model)
                 img: AbstractImage = myWindow.getImage()
                 appendFoundCellRects(img, grid, aiGrid, None, None, model) # type: ignore
                 img.drawImage()
     
     def removeGrid(self, *args, **kwargs):
-        print("removeGrid")
+        logger.info("removeGrid")
         myWindow: AbstractMyWindow = self._myWindow
         grid: Grid|None = self.getSelectedGrid()
         if grid is None:
             return
         myWindow.getImage().removeGrid(grid.name)
         myWindow.getImage().drawImage()
         self.removeSelectedRow()
@@ -201,105 +225,177 @@
             index = QtCore.QPersistentModelIndex(model_index)         
             index_list.append(index)                                             
 
         for index in index_list:                                      
             self.model().removeRow(index.row(),index.parent())
 
     def removeLabel(self, *args, **kwargs):
-        print("removeLabel")
+        logger.info("removeLabel")
         myWindow: AbstractMyWindow = self._myWindow
         label = self.selectedLabel()
         if(self.selectedType() == TreeItem.TYPE_GRID_ITEM):
             grid: Grid|None = self.getSelectedGrid()
             if grid is None:
                 return
             grid.removeRectGroup(label)
         elif(self.selectedType() == TreeItem.TYPE_MANUAL):
             myWindow.getImage().removeRectGroup(label)
         myWindow.getImage().drawImage()
         self.removeSelectedRow()
 
+    def addLeftColumns(self, *args, **kwargs):
+        logger.info("addLeftColumns")
+        num,ok = QInputDialog.getInt(self,"How many columns to add?","enter a number",1)
+        if ok:
+            grid: Grid|None = self.getSelectedGrid()
+            if grid is None:
+                return
+            for _ in range(0,num):
+                grid.addLeftColumn()
+            grid.recalcCell()
+            myWindow: AbstractMyWindow = self._myWindow
+            myWindow.getImage().drawImage()
+            tree:Tree = self
+            myWindow.reloadPropertyWindow(tree.selectionModel().selection())
+
+    def addRightColumns(self, *args, **kwargs):
+        logger.info("addRightColumns")
+        num,ok = QInputDialog.getInt(self,"How many columns to add?","enter a number",1)
+        if ok:
+            grid: Grid|None = self.getSelectedGrid()
+            if grid is None:
+                return
+            for _ in range(0,num):
+                grid.addRightColumn()
+            grid.recalcCell()
+            myWindow: AbstractMyWindow = self._myWindow
+            myWindow.getImage().drawImage()
+            tree:Tree = self
+            myWindow.reloadPropertyWindow(tree.selectionModel().selection())
+                
+    def removeLeftColumns(self, *args, **kwargs):
+        logger.info("removeLeftColumns")
+        num,ok = QInputDialog.getInt(self,"How many columns to remove?","enter a number",1)
+        if ok:
+            grid: Grid|None = self.getSelectedGrid()
+            if grid is None:
+                return
+            for _ in range(0,num):
+                grid.removeLeftColumn()
+            grid.recalcCell()
+            myWindow: AbstractMyWindow = self._myWindow
+            myWindow.getImage().drawImage()
+            tree:Tree = self
+            myWindow.reloadPropertyWindow(tree.selectionModel().selection())
+
+    def removeRightColumns(self, *args, **kwargs):
+        logger.info("removeRightColumns")
+        num,ok = QInputDialog.getInt(self,"How many columns to remove?","enter a number",1)
+        if ok:
+            grid: Grid|None = self.getSelectedGrid()
+            if grid is None:
+                return
+            for _ in range(0,num):
+                grid.removeRightColumn()
+            grid.recalcCell()
+            myWindow: AbstractMyWindow = self._myWindow
+            myWindow.getImage().drawImage()
+            tree:Tree = self
+            myWindow.reloadPropertyWindow(tree.selectionModel().selection())
+
     def addTopRows(self, *args, **kwargs):
-        print("addTopRows")
+        logger.info("addTopRows")
         num,ok = QInputDialog.getInt(self,"How many rows to add?","enter a number",1)
         if ok:
             grid: Grid|None = self.getSelectedGrid()
             if grid is None:
                 return
             for _ in range(0,num):
                 grid.addTopRow()
             grid.recalcCell()
             myWindow: AbstractMyWindow = self._myWindow
             myWindow.getImage().drawImage()
             tree:Tree = self
             myWindow.reloadPropertyWindow(tree.selectionModel().selection())
 
     def addBottomRows(self, *args, **kwargs):
-        print("addBottomRows")
+        logger.info("addBottomRows")
         num,ok = QInputDialog.getInt(self,"How many rows to add?","enter a number",1)
         if ok:
             grid: Grid|None = self.getSelectedGrid()
             if grid is None:
                 return
             for _ in range(0,num):
                 grid.addBottomRow()
             grid.recalcCell()
             myWindow: AbstractMyWindow = self._myWindow
             myWindow.getImage().drawImage()
             tree:Tree = self
             myWindow.reloadPropertyWindow(tree.selectionModel().selection())
 
     def removeTopRows(self, *args, **kwargs):
-        print("addTopRows")
-        num,ok = QInputDialog.getInt(self,"How many rows to add?","enter a number",1)
+        logger.info("removeTopRows")
+        num,ok = QInputDialog.getInt(self,"How many rows to remove?","enter a number",1)
         if ok:
             grid: Grid|None = self.getSelectedGrid()
             if grid is None:
                 return
             for _ in range(0,num):
                 grid.removeTopRow()
             grid.recalcCell()
             myWindow: AbstractMyWindow = self._myWindow
             myWindow.getImage().drawImage()
             tree:Tree = self
             myWindow.reloadPropertyWindow(tree.selectionModel().selection())
 
     def removeBottomRows(self, *args, **kwargs):
-        print("addBottomRows")
-        num,ok = QInputDialog.getInt(self,"How many rows to add?","enter a number",1)
+        logger.info("removeBottomRows")
+        num,ok = QInputDialog.getInt(self,"How many rows to remove?","enter a number",1)
         if ok:
             grid: Grid|None = self.getSelectedGrid()
             if grid is None:
                 return
             for _ in range(0,num):
                 grid.removeBottomRow()
             grid.recalcCell()
             myWindow: AbstractMyWindow = self._myWindow
             myWindow.getImage().drawImage()
             tree:Tree = self
             myWindow.reloadPropertyWindow(tree.selectionModel().selection())
         
     def treeSelectionChanged(self, selection: QItemSelection):
-        print("treeSelectionChanged")
+        logger.info("treeSelectionChanged")
         myWindow: AbstractMyWindow = self._myWindow
         myWindow.reloadPropertyWindow(selection)
         tree = self
         selectedType = tree.selectedType()
         if((selectedType == TreeItem.TYPE_GRID_ITEM) or (selectedType == TreeItem.TYPE_GRID)):
             self._actionGridAddXRowsTop.setVisible(True)
             self._actionGridAddXRowsBottom.setVisible(True)
+            self._actionGridAddXColumnsLeft.setVisible(True)
+            self._actionGridAddXColumnsRight.setVisible(True)
+            self._actionGridRemoveXRowsTop.setVisible(True)
+            self._actionGridRemoveXRowsBottom.setVisible(True)
+            self._actionGridRemoveXColumnsLeft.setVisible(True)
+            self._actionGridRemoveXColumnsRight.setVisible(True)
             grid: Grid|None = self.getSelectedGrid()
             if grid is None:
                 return
             if myWindow.hasModel(grid.name):
                 self._actionSaveModel.setVisible(True)
             self._actionLoadModel.setVisible(True)
         else:
             self._actionGridAddXRowsTop.setVisible(False)
             self._actionGridAddXRowsBottom.setVisible(False)
+            self._actionGridAddXColumnsLeft.setVisible(False)
+            self._actionGridAddXColumnsRight.setVisible(False)
+            self._actionGridRemoveXRowsTop.setVisible(False)
+            self._actionGridRemoveXRowsBottom.setVisible(False)
+            self._actionGridRemoveXColumnsLeft.setVisible(False)
+            self._actionGridRemoveXColumnsRight.setVisible(False)
             self._actionSaveModel.setVisible(False)
             self._actionLoadModel.setVisible(False)
         if(selectedType == TreeItem.TYPE_GRID):
             self._actionRemoveGrid.setVisible(True)
             self._actionSaveAsCsv.setVisible(True)
             self._actionExportCellsToImages.setVisible(True)
         else:
@@ -384,19 +480,14 @@
             selectedItem = self.getSelectedItem()
             if selectedItem is not None:
                 treeItem: QStandardItem = selectedItem.parent()
         if parent_item is not None:
             treeItem: QStandardItem = parent_item
         tree: Tree = self
         treeItem.appendRow(item)
-        tree.expandAll()
-        selModel = tree.selectionModel()
-        tree.clearSelection()
-        model: QStandardItemModel = typing.cast(QStandardItemModel, tree.model())
-        selModel.select(model.indexFromItem(item), QItemSelectionModel.SelectionFlag.Select)
         item.setFlags(item.flags() | QtCore.Qt.ItemFlag.ItemIsUserCheckable |
                         QtCore.Qt.ItemFlag.ItemIsEnabled |
                         QtCore.Qt.ItemFlag.ItemIsSelectable)
         item.setCheckState(QtCore.Qt.CheckState.Checked)
         if type in [TreeItem.TYPE_AI_GRID,TreeItem.TYPE_GRID,TreeItem.TYPE_MANUAL]:
             item.onChecked = self.itemChecked
         if type == TreeItem.TYPE_GRID_ITEM:
@@ -436,20 +527,33 @@
             manual: QStandardItem = myWindow.getManualItem()
             for r in range(0,manual.rowCount()):
                 if manual.child(r).data(TreeItem.TEXT) == gridName:
                     return manual.child(r).data(TreeItem.OBJECT)
         return None if type != TreeItem.TYPE_GRID else selectedItem.data(TreeItem.OBJECT)
 
     def getSelectedAIGrid(self):
+        myWindow: AbstractMyWindow = self._myWindow
         selectedItem = self.getSelectedItem()
         if selectedItem is None:
             return
         type = selectedItem.data(TreeItem.TYPE)
         if type == TreeItem.TYPE_AI_GRID_ITEM:
             return selectedItem.parent().data(TreeItem.OBJECT)
+        if type == TreeItem.TYPE_GRID_ITEM:
+            gridName = selectedItem.parent().data(TreeItem.TEXT)
+            aiItem: QStandardItem = myWindow.getAIItem()
+            for r in range(0,aiItem.rowCount()):
+                if aiItem.child(r).data(TreeItem.TEXT) == gridName:
+                    return aiItem.child(r).data(TreeItem.OBJECT)
+        if type == TreeItem.TYPE_GRID:
+            gridName = selectedItem.data(TreeItem.TEXT)
+            aiItem: QStandardItem = myWindow.getAIItem()
+            for r in range(0,aiItem.rowCount()):
+                if aiItem.child(r).data(TreeItem.TEXT) == gridName:
+                    return aiItem.child(r).data(TreeItem.OBJECT)
         return None if type != TreeItem.TYPE_AI_GRID else selectedItem.data(TreeItem.OBJECT)
     
     def isItemSelected(self, rectLabel, gridName, gridItemType) -> bool:
         selectedItem = self.getSelectedItem()
         if selectedItem is None:
             return False
         type = selectedItem.data(TreeItem.TYPE)
@@ -492,15 +596,14 @@
         myWindow: AbstractMyWindow = self._myWindow
         img = myWindow.getImage()
         grid = treeItem.parent().data(TreeItem.OBJECT)
         if checked:
             img.activateAIGridRectGroup(grid,text)
         else:
             img.deactivateAIGridRectGroup(grid,text)
-        img.drawImage()
         
     def gridRectGroupChecked(self, treeItem: TreeItem, checked, text):
         myWindow: AbstractMyWindow = self._myWindow
         img = myWindow.getImage()
         grid = treeItem.parent().data(TreeItem.OBJECT)
         if checked:
             img.activateGridRectGroup(grid,text)
```

### Comparing `silicon_analyser-1.1.0/silicon_analyser/main_window.ui` & `silicon_analyser-1.1.1/silicon_analyser/main_window.ui`

 * *Files 14% similar despite different names*

#### Comparing `silicon_analyser-1.1.0/silicon_analyser/main_window.ui` & `silicon_analyser-1.1.1/silicon_analyser/main_window.ui`

```diff
@@ -3,134 +3,147 @@
   <class>MainWindow</class>
   <widget class="QMainWindow" name="MainWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>924</width>
-        <height>657</height>
+        <height>857</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>MainWindow</string>
     </property>
     <widget class="QWidget" name="centralwidget">
       <property name="baseSize">
         <size>
           <width>0</width>
           <height>0</height>
         </size>
       </property>
       <layout class="QGridLayout" name="gridLayout">
-        <item row="3" column="0">
-          <widget class="Tree" name="_tree">
+        <item row="6" column="0">
+          <widget class="MiniMap" name="_minimap">
+            <property name="minimumSize">
+              <size>
+                <width>300</width>
+                <height>300</height>
+              </size>
+            </property>
             <property name="maximumSize">
               <size>
                 <width>300</width>
-                <height>16777215</height>
+                <height>300</height>
               </size>
             </property>
-            <property name="focusPolicy">
-              <enum>Qt::NoFocus</enum>
+            <property name="text">
+              <string/>
             </property>
-            <property name="contextMenuPolicy">
-              <enum>Qt::ActionsContextMenu</enum>
+          </widget>
+        </item>
+        <item row="0" column="1" rowspan="7">
+          <widget class="FullImage" name="_image">
+            <property name="minimumSize">
+              <size>
+                <width>600</width>
+                <height>600</height>
+              </size>
+            </property>
+            <property name="text">
+              <string/>
             </property>
           </widget>
         </item>
-        <item row="2" column="0">
-          <widget class="ComputeBtn" name="_computeBtn">
+        <item row="1" column="0">
+          <widget class="AddLabelBtn" name="_addLabelBtn">
             <property name="maximumSize">
               <size>
                 <width>300</width>
                 <height>16777215</height>
               </size>
             </property>
             <property name="focusPolicy">
               <enum>Qt::NoFocus</enum>
             </property>
             <property name="text">
-              <string>Compute</string>
+              <string>Add label</string>
             </property>
           </widget>
         </item>
-        <item row="0" column="0">
-          <widget class="AddGridBtn" name="_addGridBtn">
+        <item row="3" column="0">
+          <widget class="ComputeBtn" name="_computeBtn">
             <property name="maximumSize">
               <size>
                 <width>300</width>
                 <height>16777215</height>
               </size>
             </property>
             <property name="focusPolicy">
               <enum>Qt::NoFocus</enum>
             </property>
             <property name="text">
-              <string>Add grid</string>
+              <string>Compute</string>
             </property>
           </widget>
         </item>
-        <item row="5" column="0">
-          <widget class="MiniMap" name="_minimap">
-            <property name="minimumSize">
-              <size>
-                <width>300</width>
-                <height>300</height>
-              </size>
-            </property>
+        <item row="0" column="0">
+          <widget class="AddGridBtn" name="_addGridBtn">
             <property name="maximumSize">
               <size>
                 <width>300</width>
-                <height>300</height>
+                <height>16777215</height>
               </size>
             </property>
+            <property name="focusPolicy">
+              <enum>Qt::NoFocus</enum>
+            </property>
             <property name="text">
-              <string/>
+              <string>Add grid</string>
             </property>
           </widget>
         </item>
-        <item row="1" column="0">
-          <widget class="AddLabelBtn" name="_addLabelBtn">
+        <item row="5" column="0">
+          <widget class="QTableView" name="_properties">
             <property name="maximumSize">
               <size>
                 <width>300</width>
                 <height>16777215</height>
               </size>
             </property>
             <property name="focusPolicy">
               <enum>Qt::NoFocus</enum>
             </property>
-            <property name="text">
-              <string>Add label</string>
-            </property>
           </widget>
         </item>
         <item row="4" column="0">
-          <widget class="QTableView" name="_properties">
+          <widget class="Tree" name="_tree">
             <property name="maximumSize">
               <size>
                 <width>300</width>
                 <height>16777215</height>
               </size>
             </property>
             <property name="focusPolicy">
               <enum>Qt::NoFocus</enum>
             </property>
+            <property name="contextMenuPolicy">
+              <enum>Qt::ActionsContextMenu</enum>
+            </property>
           </widget>
         </item>
-        <item row="0" column="1" rowspan="6">
-          <widget class="FullImage" name="_image">
-            <property name="minimumSize">
-              <size>
-                <width>600</width>
-                <height>600</height>
-              </size>
+        <item row="2" column="0">
+          <widget class="AutoComputeBtn" name="_autoComputeBtn">
+            <property name="focusPolicy">
+              <enum>Qt::NoFocus</enum>
             </property>
             <property name="text">
-              <string/>
+              <string>Activate auto compute</string>
+            </property>
+            <property name="checkable">
+              <bool>true</bool>
             </property>
           </widget>
         </item>
       </layout>
     </widget>
     <widget class="QStatusBar" name="_statusBar"/>
     <widget class="QMenuBar" name="menuBar">
@@ -153,16 +166,23 @@
       <widget class="QMenu" name="menuComputation_method">
         <property name="title">
           <string>Computation method</string>
         </property>
         <addaction name="_actionDecisionTree"/>
         <addaction name="_actionNeuralNetwork"/>
       </widget>
+      <widget class="QMenu" name="menuWeblinks">
+        <property name="title">
+          <string>Weblinks</string>
+        </property>
+        <addaction name="_actionSiliconpr0n"/>
+      </widget>
       <addaction name="menuInfo"/>
       <addaction name="menuComputation_method"/>
+      <addaction name="menuWeblinks"/>
     </widget>
     <action name="_actionSaveModel">
       <property name="text">
         <string>Save computation model</string>
       </property>
     </action>
     <action name="_actionLoadModel">
@@ -264,17 +284,56 @@
       <property name="text">
         <string>Remove X rows on top</string>
       </property>
       <property name="toolTip">
         <string>Remove X rows on top</string>
       </property>
     </action>
+    <action name="_actionSiliconpr0n">
+      <property name="text">
+        <string>https://siliconpr0n.org/</string>
+      </property>
+    </action>
+    <action name="_actionGridAddXColumnsLeft">
+      <property name="text">
+        <string>Add X columns to left</string>
+      </property>
+    </action>
+    <action name="_actionGridAddXColumnsRight">
+      <property name="text">
+        <string>Add X columns to right</string>
+      </property>
+      <property name="toolTip">
+        <string>Add X columns to right</string>
+      </property>
+    </action>
+    <action name="_actionGridRemoveXColumnsLeft">
+      <property name="text">
+        <string>Remove X columns on left</string>
+      </property>
+      <property name="toolTip">
+        <string>Remove X columns on left</string>
+      </property>
+    </action>
+    <action name="_actionGridRemoveXColumnsRight">
+      <property name="text">
+        <string>Remove X columns on right</string>
+      </property>
+      <property name="toolTip">
+        <string>Remove X columns on right</string>
+      </property>
+    </action>
   </widget>
   <customwidgets>
     <customwidget>
+      <class>AutoComputeBtn</class>
+      <extends>QPushButton</extends>
+      <header>silicon_analyser.helper.autocomputebtn</header>
+    </customwidget>
+    <customwidget>
       <class>ComputeBtn</class>
       <extends>QPushButton</extends>
       <header>silicon_analyser.helper.computebtn</header>
     </customwidget>
     <customwidget>
       <class>AddLabelBtn</class>
       <extends>QPushButton</extends>
```

### Comparing `silicon_analyser-1.1.0/silicon_analyser/mywindow.py` & `silicon_analyser-1.1.1/silicon_analyser/mywindow.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,80 @@
+import logging
+
+logger = logging.getLogger(__name__)
+
 import torch
 import importlib.metadata
 from PyQt5 import QtCore, QtGui, uic
-from PyQt5.QtCore import Qt, QItemSelection
+from PyQt5.QtCore import Qt, QItemSelection, QSemaphore
 from PyQt5.QtWidgets import QFileDialog, QMenu, QTableView, QStatusBar, QAction
 from PyQt5.QtGui import QPixmap, QStandardItem, QStandardItemModel
 from os import path as p
 import sys
 
 import silicon_analyser.savefiles
-from silicon_analyser.savefiles import loadGrids, loadRects
+from silicon_analyser.savefiles import Saving
 from silicon_analyser.helper.abstract.abstracttreehelper import AbstractTreeHelper
 from silicon_analyser.helper.abstract.abstractimage import AbstractImage
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
 from silicon_analyser.helper.minimap import MiniMap
 from silicon_analyser.helper.fullimage import FullImage
 from silicon_analyser.helper.addlabelbtn import AddLabelBtn
 from silicon_analyser.helper.computebtn import ComputeBtn
+from silicon_analyser.helper.autocomputebtn import AutoComputeBtn
 from silicon_analyser.helper.addgridbtn import AddGridBtn
 from silicon_analyser.treeitem import TreeItem
 from silicon_analyser.helper.properties import PropertiesUtil
 from silicon_analyser.grid import Grid
 from silicon_analyser.treeitem import TreeItem
 from silicon_analyser.helper.tree import Tree
 
 class MyWindow(AbstractMyWindow):
+    _mainSemaphore: QSemaphore
     _tree: Tree
     _properties: QTableView
     _addLabelBtn: AddLabelBtn
+    _autoComputeBtn: AutoComputeBtn
     _computeBtn: ComputeBtn
     _addGridBtn: AddGridBtn
     _statusBar: QStatusBar
     _minimap: MiniMap
     _image: FullImage
     _models: dict[str,object]
     _actionGridAddXRowsTop: QAction
     _actionGridAddXRowsBottom: QAction
     _actionGridRemoveXRowsTop: QAction
     _actionGridRemoveXRowsBottom: QAction
+    _actionGridAddXColumnsLeft: QAction
+    _actionGridAddXColumnsRight: QAction
+    _actionGridRemoveXColumnsLeft: QAction
+    _actionGridRemoveXColumnsRight: QAction
     _actionSaveModel: QAction
     _actionLoadModel: QAction
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionMade_by_TheCrazyT: QAction
     _actionUrl: QAction
     _actionSaveAsCsv: QAction
     _actionViewAsPixelimage: QAction
     _actionExportCellsToImages: QAction
     _actionDecisionTree: QAction
     _actionNeuralNetwork: QAction
+    _actionSiliconpr0n: QAction
 
     autosave: bool
     menuBar: QMenu
+    saving: Saving
     
     def __init__(self):
         AbstractMyWindow.__init__(self)
         path: str = p.abspath(p.join(p.dirname(__file__), '.')) + '/main_window.ui'
         uic.loadUi(path, self)
+        self._mainSemaphore = QSemaphore(1)
+        self.saving = Saving(self._mainSemaphore)
         tree: Tree = self._tree
         properties: QTableView = self._properties
                 
         self._treeModel = QStandardItemModel()
         self._propertiesModel = QStandardItemModel()
         properties.setModel(self._propertiesModel)
         self._propertiesUtil = PropertiesUtil(self,self._properties)
@@ -73,66 +88,77 @@
         self._treeAIItem.setFlags(self._treeAIItem.flags() |QtCore.Qt.ItemFlag.ItemIsUserCheckable |
                           QtCore.Qt.ItemFlag.ItemIsEnabled)
         self._treeAIItem.setCheckState(QtCore.Qt.CheckState.Unchecked)
         self._treeModel.appendRow(self._treeAIItem)
         tree.setModel(self._treeModel)
         self._models = {}
         self._actionUrl.triggered.connect(self.openMainUrl)
+        self._actionSiliconpr0n.triggered.connect(self.openSiliconpr0nUrl)
 
+        imageFile: str
         if(len(sys.argv) < 2):
             dlg = QFileDialog()
             filenames = dlg.getOpenFileName(caption="Load image",filter="Image (*.png;*.jpg;*.bmp;*.gif)",initialFilter="Image (*.png;*.jpg;*.bmp;*.gif)")
             if(len(filenames) >= 1):
-                self._pixmap = QPixmap(filenames[0])
+                imageFile = filenames[0]
         else:
-            self._pixmap = QPixmap(sys.argv[1])
+            imageFile = sys.argv[1]
+        self._pixmap = QPixmap(imageFile)
+        self.setWindowTitle(f"SiliconAnalyser - {imageFile}")
         
         computeBtn: ComputeBtn = self._computeBtn
+        autoComputeBtn: ComputeBtn = self._autoComputeBtn
         addGridBtn: AddGridBtn = self._addGridBtn
         addLabelBtn: AddLabelBtn = self._addLabelBtn
         minimap: MiniMap = self._minimap
         image: FullImage = self._image
 
         tree.initialize(self)
         computeBtn.initialize(self)
+        autoComputeBtn.initialize(self)
         addGridBtn.initialize(self)
         addLabelBtn.initialize(self)
         minimap.initialize(self, self._pixmap)
         image.initialize(self, self._pixmap)
         
-        computeBtn.setDisabled(True)
-        addLabelBtn.setDisabled(True)
+        self.disableComputeButton()
+        self.disableAutoComputeButton()
+        self.disableAddLabelButton()
         tree.evtTreeSelectionChanged.connect(self.treeSelectionChanged)
 
         self._actionDecisionTree.triggered.connect(self.decisionTreeChecked)
         self._actionNeuralNetwork.triggered.connect(self.neuralNetworkChecked)
         
+        self.getAutoComputeBtn().active.connect(self.autoComputeActive)
+        self.getAutoComputeBtn().unactive.connect(self.autoComputeUnactive)
+        
         self._posX = 0
         self._posY = 0
         
         self._scale = 1.0
         self.drawImgAndMinimap()
         
         self.autosave = False
         
         if p.isfile(silicon_analyser.savefiles.SAVE_RECTS):
             with open(silicon_analyser.savefiles.SAVE_RECTS,"r") as f:
-                rects = loadRects()
+                rects = self.saving.loadRects()
                 for k in rects.keys():
-                    self.getTree().addTreeItem(k)
+                    tree.addTreeItem(k)
                 image.loadRects(rects)
         if p.isfile(silicon_analyser.savefiles.SAVE_GRIDS):
-            grids: dict[str, Grid] = loadGrids()
+            grids: dict[str, Grid] = self.saving.loadGrids()
             for gridKey in grids.keys():
-                grid, parentTreeItem = self.getTree().addTreeItem(gridKey,TreeItem.TYPE_GRID)
+                grid, parentTreeItem = tree.addTreeItem(gridKey,TreeItem.TYPE_GRID)
                 for gridItemKey in grids[gridKey].getLabels():
-                    _, treeItem = self.getTree().addTreeItem(gridItemKey,TreeItem.TYPE_GRID_ITEM, grid, parentTreeItem)
+                    _, treeItem = tree.addTreeItem(gridItemKey,TreeItem.TYPE_GRID_ITEM, grid, parentTreeItem)
                     text = treeItem.data(TreeItem.TEXT)
                     if(not grids[gridKey]._rectsActive[text]):
-                        treeItem.setCheckState(QtCore.Qt.CheckState.Unchecked)
+                        treeItem.uncheck()
+                tree.expandAll()
             image.loadGrids(grids)
         
         image.drawImage()
         self.autosave = True
         if(torch.cuda.is_available()):
             self.setSuccessStatus("CUDA successfully initialized")
         else:
@@ -140,43 +166,74 @@
         
         menuBar: QMenu = self.menuBar    
 
         version = importlib.metadata.version("silicon-analyser")
         action = menuBar.addAction(f"Version: {version}")
         action.triggered.connect(self.openMainUrl)
         
+        self.saving.onSaving.connect(lambda : self.setStatusText("Saving ..."))
+    
+    def getMainSemaphore(self) -> QSemaphore:
+        return self._mainSemaphore
+    
+    def getSaving(self) -> Saving:
+        return self.saving
+    
+    def autoComputeActive(self):
+        self.disableComputeButton()
+        self.disableAddLabelButton()
+        self.disableAddGridButton()
+        self._actionDecisionTree.setEnabled(False)
+        self._actionNeuralNetwork.setEnabled(False)
+        
+    def autoComputeUnactive(self):
+        self.enableComputeButton()
+        self.enableAddLabelButton()
+        self.enableAddGridButton()
+        self._actionDecisionTree.setEnabled(True)
+        self._actionNeuralNetwork.setEnabled(True)
+    
+    def getAutoComputeBtn(self) -> AutoComputeBtn:
+        return self._autoComputeBtn
 
     def decisionTreeChecked(self):
         if(self._actionDecisionTree.isChecked()):
             self._actionNeuralNetwork.setChecked(False)
+            self.getAutoComputeBtn().computationMethodChanged.emit()
 
     def neuralNetworkChecked(self):
         if(self._actionNeuralNetwork.isChecked()):
             self._actionDecisionTree.setChecked(False)
+            self.getAutoComputeBtn().computationMethodChanged.emit()
         
     def treeSelectionChanged(self, selection: QItemSelection):
         tree: Tree = self._tree
         selectedType: str|None = tree.selectedType()
-        computeBtn: ComputeBtn = self._computeBtn
-        addLabelBtn: AddLabelBtn = self._addLabelBtn
-        if((selectedType == TreeItem.TYPE_GRID_ITEM)
-           or (selectedType == TreeItem.TYPE_GRID)
-           or (selectedType == TreeItem.TYPE_AI_GRID)
-           or (selectedType == TreeItem.TYPE_AI_GRID_ITEM)
-           ):
-            computeBtn.setDisabled(False)
-            addLabelBtn.setDisabled(False)
-        else:
-            computeBtn.setDisabled(True)
-            addLabelBtn.setDisabled(True)
+        if not self.getAutoComputeBtn().isChecked():
+            if((selectedType == TreeItem.TYPE_GRID_ITEM)
+            or (selectedType == TreeItem.TYPE_GRID)
+            or (selectedType == TreeItem.TYPE_AI_GRID)
+            or (selectedType == TreeItem.TYPE_AI_GRID_ITEM)
+            ):
+                self.enableComputeButton()
+                self.enableAutoComputeButton()
+                self.enableAddLabelButton()
+            else:
+                self.disableComputeButton()
+                self.disableAutoComputeButton()
+                self.disableAddLabelButton()
 
     def openMainUrl(self) -> None:
         import webbrowser
         webbrowser.open('https://github.com/TheCrazyT/SiliconAnalyser')
         
+    def openSiliconpr0nUrl(self) -> None:
+        import webbrowser
+        webbrowser.open('https://siliconpr0n.org/')
+        
     def getModel(self, name):
         if name in self._models:
             return self._models[name]
         return None
     
     def hasModel(self, name) -> bool:
         if name in self._models:
@@ -207,14 +264,15 @@
         statusBar: QStatusBar = self._statusBar
         statusBar.setStyleSheet('background-color: #ff0000')
         statusBar.showMessage(text)
             
     def setStatusText(self, text):
         statusBar: QStatusBar = self._statusBar
         statusBar.setStyleSheet('')
+        logger.info(f"status: {text}")
         statusBar.showMessage(text)
         
     def getTree(self) -> AbstractTreeHelper:
         return self._tree
     
     def getManualItem(self) -> QStandardItem:
         return self._treeManualItem
@@ -233,20 +291,20 @@
     
     def getPosY(self):
         return self._posY
     
     def setPosX(self, x):
         self._posX = x
         self._posX = max(self._posX,0)
-        self._posX = min(self._posX,self._image.getImageWidth()-self.imageWidth()/self.getScale())
+        self._posX = min(self._posX,self.getImage().getImageWidth()-self.imageWidth()/self.getScale())
     
     def setPosY(self, y):
         self._posY = y
         self._posY = max(self._posY,0)
-        self._posY = min(self._posY,self._image.getImageHeight()-self.imageHeight()/self.getScale())
+        self._posY = min(self._posY,self.getImage().getImageHeight()-self.imageHeight()/self.getScale())
     
     def drawImgAndMinimap(self):
         self.getImage().drawImage()
         self.getMinimap().drawMinimap()
     
     def reloadProperyWindowByGrid(self, grid):
         return self._propertiesUtil.reloadProperyWindowByGrid(grid)
@@ -265,15 +323,46 @@
         if keyEvent.key() == Qt.Key.Key_Up:
             self.setPosY(self.getPosY() - c)
         if keyEvent.key() == Qt.Key.Key_Down:
             self.setPosY(self.getPosY() + c)
         self.drawImgAndMinimap()
             
     def wheelEvent(self,event):
-        #print(event.angleDelta())
         if event.angleDelta().y() > 0:
             self._scale += 0.25
         else:
             self._scale -= 0.25
         self._scale = max(self._scale,0.25)
-        print(self._scale)
-        self.drawImgAndMinimap()
+        logger.info(self._scale)
+        self.drawImgAndMinimap()
+        
+    def disableComputeButton(self):
+        computeBtn: ComputeBtn = self._computeBtn
+        computeBtn.setEnabled(False)
+
+    def disableAutoComputeButton(self):
+        autoComputeBtn: AutoComputeBtn = self._autoComputeBtn
+        autoComputeBtn.setEnabled(False)
+    
+    def disableAddLabelButton(self):
+        addLabelBtn: AddLabelBtn = self._addLabelBtn
+        addLabelBtn.setEnabled(False)
+    
+    def disableAddGridButton(self):
+        addGridBtn: AddGridBtn = self._addGridBtn
+        addGridBtn.setEnabled(False)
+    
+    def enableComputeButton(self):
+        computeBtn: ComputeBtn = self._computeBtn
+        computeBtn.setEnabled(True)
+    
+    def enableAutoComputeButton(self):
+        autoComputeBtn: AutoComputeBtn = self._autoComputeBtn
+        autoComputeBtn.setEnabled(True)
+    
+    def enableAddLabelButton(self):
+        addLabelBtn: AddLabelBtn = self._addLabelBtn
+        addLabelBtn.setEnabled(True)
+    
+    def enableAddGridButton(self):
+        addGridBtn: AddGridBtn = self._addGridBtn
+        addGridBtn.setEnabled(True)
```

### Comparing `silicon_analyser-1.1.0/silicon_analyser/treeitem.py` & `silicon_analyser-1.1.1/silicon_analyser/treeitem.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,8 +40,12 @@
             if self.onChecked is not None:
                 if value == 0:
                     self.onChecked(self,False,self._text)
                 else:
                     self.onChecked(self,True,self._text)
         return super().setData(value, role)
     
+    def uncheck(self):
+        self.setCheckState(Qt.CheckState.Unchecked)
+
+
```

### Comparing `silicon_analyser-1.1.0/silicon_analyser.egg-info/PKG-INFO` & `silicon_analyser-1.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silicon-analyser
-Version: 1.1.0
+Version: 1.1.1
 Summary: helps to analyse integrated circuit die images (for example from siliconpr0n.org) with the help of ai.
 Author-email: CrazyT <crazyt2019+sa@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/SiliconAnalyser
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/SiliconAnalyser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,24 @@
 
 Install from pip:
 
 `pip install --upgrade silicon-analyser`
 
 # Information
 
-Code will use your graphic card for acceleration.
+## Side note
+Bad project name decisions might lead people to this project.
+
+Maybe you are looking for [SiliconAnalysis](https://github.com/SiliconAnalysis/) instead?
+
+I'm sorry for that but I can't figure out any new project name (yet).
+
+## Acceleration
+
+The code will use your graphic card for acceleration.
 (but only if correct pytorch is installed, see "Additional info" below)
 
 Frameworks/Libraries used:
 * [PyQt5](https://www.riverbankcomputing.com/software/pyqt/)
 * [PyTorch](https://pytorch.org/)
 * [Keras](https://keras.io/)
 * [PyQtGraph](https://www.pyqtgraph.org/)
@@ -67,27 +76,40 @@
     * "acc" stands for "accuracy", "val" for "validation"
 * found ai-cells will be drawn green
 
 # Additional info
 
 * you might need to install cuda-specific [PyTorch](https://pytorch.org/get-started/previous-versions/#linux-and-windows-4) for accelerated computing
     * check your graphic driver version for compatible cuda version!
+* Computation (currently) only happens based on active/visible grid cells (don't be fooled by accuracy of 1 just because you have only 1 label active - just activate all and use compute)
+
+## Command line
+
+For automatically opening a file, you can pass the filepath as a filename.
+For example:
+  silicon-analyser c:\my_files\image.png
+But keep in mind, that the program currently needs to create files in its current working directory (grid.json, rect.json).
 
 # Keys
 
 * Use up/down/left/right to navigate
 * Hold shift to move faster
 * Scroll-wheel to zoom out
 * Click on minimap to get directly to a position
 * Right click on tree-items (left navigation menu) for additional options
+* Hold down middle mouse button, to move across the screen
+  * (behaviour might change in future, currently it does not behave as expected)
 
 ![image](https://raw.githubusercontent.com/TheCrazyT/SiliconAnalyser/main/docs/small_tutorial.gif)
 
 # TODO
 
+* undo option
+* maybe use a real db in background
+* some method to autofit grid
+* performance improvements
+* option for compute to continue from last training (currently starts fresh training)
 * show loading screen on start (pytorch with cuda support takes a bit to load)
-* option to calculate/classify by decision tree
-* auto-compute to calculate in background while you are selecting new cells for your labels
 * ai-model configuration
 * project management (project-file/-folder)
 * possibility to rotate grid
 * maybe store your model on a public place? (for others to use)
```

### Comparing `silicon_analyser-1.1.0/silicon_analyser.egg-info/SOURCES.txt` & `silicon_analyser-1.1.1/silicon_analyser.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -17,15 +17,20 @@
 silicon_analyser/dialogs/compute_stats.py
 silicon_analyser/dialogs/compute_stats.ui
 silicon_analyser/dialogs/pixel_image.py
 silicon_analyser/dialogs/pixel_image.ui
 silicon_analyser/helper/addgridbtn.py
 silicon_analyser/helper/addlabelbtn.py
 silicon_analyser/helper/ai.py
+silicon_analyser/helper/autocomputebtn.py
+silicon_analyser/helper/common.py
 silicon_analyser/helper/computebtn.py
 silicon_analyser/helper/fullimage.py
 silicon_analyser/helper/minimap.py
 silicon_analyser/helper/properties.py
 silicon_analyser/helper/tree.py
+silicon_analyser/helper/abstract/abstractcomputationmethod.py
 silicon_analyser/helper/abstract/abstractimage.py
 silicon_analyser/helper/abstract/abstractmywindow.py
-silicon_analyser/helper/abstract/abstracttreehelper.py
+silicon_analyser/helper/abstract/abstracttreehelper.py
+silicon_analyser/helper/computation_methods/decision_tree.py
+silicon_analyser/helper/computation_methods/neural_network.py
```

