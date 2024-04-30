# Comparing `tmp/mpl_ascii-0.2.0.tar.gz` & `tmp/mpl_ascii-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_ascii-0.2.0.tar", last modified: Sun Apr 28 12:46:46 2024, max compression
+gzip compressed data, was "mpl_ascii-0.3.0.tar", last modified: Tue Apr 30 17:43:44 2024, max compression
```

## Comparing `mpl_ascii-0.2.0.tar` & `mpl_ascii-0.3.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 12:46:46.504310 mpl_ascii-0.2.0/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 12:46:46.492310 mpl_ascii-0.2.0/.github/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 12:46:46.496310 mpl_ascii-0.2.0/.github/workflows/
--rw-rw-r--   0 chris     (1000) chris     (1000)      992 2024-04-25 17:23:19.000000 mpl_ascii-0.2.0/.github/workflows/python-package.yml
--rw-rw-r--   0 chris     (1000) chris     (1000)     3107 2024-04-25 16:48:20.000000 mpl_ascii-0.2.0/.gitignore
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2024-04-25 16:42:37.000000 mpl_ascii-0.2.0/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)     1472 2024-04-27 12:42:39.000000 mpl_ascii-0.2.0/Makefile
--rw-r--r--   0 chris     (1000) chris     (1000)    20434 2024-04-28 12:46:46.504310 mpl_ascii-0.2.0/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)    20125 2024-04-28 08:08:12.000000 mpl_ascii-0.2.0/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 12:46:46.500310 mpl_ascii-0.2.0/examples/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1306 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/bar_chart.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      827 2024-04-28 08:03:54.000000 mpl_ascii-0.2.0/examples/bar_color.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      903 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/bar_label_1.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1011 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/bar_label_2.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1084 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/bar_label_3.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      675 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/bar_label_4.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      669 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/bar_label_5.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1012 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/bar_stacked.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1036 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/barh.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      736 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/categorical_variables.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1069 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/cohere.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      998 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/cohere_single_plot.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1286 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/csd_demo.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      747 2024-04-28 08:04:51.000000 mpl_ascii-0.2.0/examples/double_plot.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1124 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/hist_best_fit_line.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1019 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/hist_simple.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1665 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/hist_simple_colors.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1188 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/lines_multi_color.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1218 2024-04-28 08:05:08.000000 mpl_ascii-0.2.0/examples/scatter_multi_color.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      627 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/simple_plot.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 12:46:46.500310 mpl_ascii-0.2.0/mpl_ascii/
--rw-rw-r--   0 chris     (1000) chris     (1000)     8963 2024-04-28 12:43:13.000000 mpl_ascii-0.2.0/mpl_ascii/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      856 2024-04-25 16:43:43.000000 mpl_ascii-0.2.0/mpl_ascii/ascii_canvas.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1629 2024-04-25 16:43:43.000000 mpl_ascii-0.2.0/mpl_ascii/color_map.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3987 2024-04-25 16:43:43.000000 mpl_ascii-0.2.0/mpl_ascii/draw.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1340 2024-04-25 16:43:43.000000 mpl_ascii-0.2.0/mpl_ascii/overlay.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      274 2024-04-25 16:43:43.000000 mpl_ascii-0.2.0/mpl_ascii/tools.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 12:46:46.504310 mpl_ascii-0.2.0/mpl_ascii.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)    20434 2024-04-28 12:46:46.000000 mpl_ascii-0.2.0/mpl_ascii.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      945 2024-04-28 12:46:46.000000 mpl_ascii-0.2.0/mpl_ascii.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-04-28 12:46:46.000000 mpl_ascii-0.2.0/mpl_ascii.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       18 2024-04-28 12:46:46.000000 mpl_ascii-0.2.0/mpl_ascii.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       10 2024-04-28 12:46:46.000000 mpl_ascii-0.2.0/mpl_ascii.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      429 2024-04-28 12:44:22.000000 mpl_ascii-0.2.0/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)      144 2024-04-25 18:43:05.000000 mpl_ascii-0.2.0/requirements.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-04-28 12:46:46.504310 mpl_ascii-0.2.0/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 12:46:46.504310 mpl_ascii-0.2.0/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2024-04-25 16:45:15.000000 mpl_ascii-0.2.0/tests/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4510 2024-04-25 16:45:15.000000 mpl_ascii-0.2.0/tests/test_overlay.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-30 17:43:44.744003 mpl_ascii-0.3.0/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-30 17:43:44.736003 mpl_ascii-0.3.0/.github/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-30 17:43:44.736003 mpl_ascii-0.3.0/.github/workflows/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      992 2024-04-25 17:23:19.000000 mpl_ascii-0.3.0/.github/workflows/python-package.yml
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3107 2024-04-25 16:48:20.000000 mpl_ascii-0.3.0/.gitignore
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2024-04-25 16:42:37.000000 mpl_ascii-0.3.0/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1472 2024-04-27 12:42:39.000000 mpl_ascii-0.3.0/Makefile
+-rw-r--r--   0 chris     (1000) chris     (1000)     5590 2024-04-30 17:43:44.744003 mpl_ascii-0.3.0/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5253 2024-04-30 17:38:47.000000 mpl_ascii-0.3.0/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-30 17:43:44.744003 mpl_ascii-0.3.0/examples/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1306 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/bar_chart.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      827 2024-04-28 08:03:54.000000 mpl_ascii-0.3.0/examples/bar_color.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      903 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/bar_label_1.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1011 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/bar_label_2.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1084 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/bar_label_3.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      675 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/bar_label_4.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      669 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/bar_label_5.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1012 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/bar_stacked.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1036 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/barh.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      736 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/categorical_variables.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1069 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/cohere.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      998 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/cohere_single_plot.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1286 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/csd_demo.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      747 2024-04-28 08:04:51.000000 mpl_ascii-0.3.0/examples/double_plot.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1124 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/hist_best_fit_line.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1019 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/hist_simple.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1665 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/hist_simple_colors.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1188 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/lines_multi_color.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1218 2024-04-28 08:05:08.000000 mpl_ascii-0.3.0/examples/scatter_multi_color.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      627 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/simple_plot.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-30 17:43:44.744003 mpl_ascii-0.3.0/mpl_ascii/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3413 2024-04-30 16:42:51.000000 mpl_ascii-0.3.0/mpl_ascii/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1239 2024-04-30 16:43:02.000000 mpl_ascii-0.3.0/mpl_ascii/ascii_canvas.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2055 2024-04-30 16:45:38.000000 mpl_ascii-0.3.0/mpl_ascii/color_map.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9879 2024-04-30 16:42:27.000000 mpl_ascii-0.3.0/mpl_ascii/draw.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1342 2024-04-30 16:37:32.000000 mpl_ascii-0.3.0/mpl_ascii/overlay.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      274 2024-04-25 16:43:43.000000 mpl_ascii-0.3.0/mpl_ascii/tools.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-30 17:43:44.744003 mpl_ascii-0.3.0/mpl_ascii.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     5590 2024-04-30 17:43:44.000000 mpl_ascii-0.3.0/mpl_ascii.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      945 2024-04-30 17:43:44.000000 mpl_ascii-0.3.0/mpl_ascii.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-04-30 17:43:44.000000 mpl_ascii-0.3.0/mpl_ascii.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       31 2024-04-30 17:43:44.000000 mpl_ascii-0.3.0/mpl_ascii.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       10 2024-04-30 17:43:44.000000 mpl_ascii-0.3.0/mpl_ascii.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      445 2024-04-30 17:39:29.000000 mpl_ascii-0.3.0/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)      144 2024-04-25 18:43:05.000000 mpl_ascii-0.3.0/requirements.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-04-30 17:43:44.744003 mpl_ascii-0.3.0/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-30 17:43:44.744003 mpl_ascii-0.3.0/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2024-04-25 16:45:15.000000 mpl_ascii-0.3.0/tests/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4510 2024-04-30 16:36:55.000000 mpl_ascii-0.3.0/tests/test_overlay.py
```

### Comparing `mpl_ascii-0.2.0/.github/workflows/python-package.yml` & `mpl_ascii-0.3.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/.gitignore` & `mpl_ascii-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/LICENSE` & `mpl_ascii-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/Makefile` & `mpl_ascii-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/bar_chart.py` & `mpl_ascii-0.3.0/examples/bar_chart.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/bar_color.py` & `mpl_ascii-0.3.0/examples/bar_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/bar_label_1.py` & `mpl_ascii-0.3.0/examples/bar_label_1.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/bar_label_2.py` & `mpl_ascii-0.3.0/examples/bar_label_2.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/bar_label_3.py` & `mpl_ascii-0.3.0/examples/bar_label_3.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/bar_label_4.py` & `mpl_ascii-0.3.0/examples/bar_label_4.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/bar_label_5.py` & `mpl_ascii-0.3.0/examples/bar_label_5.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/bar_stacked.py` & `mpl_ascii-0.3.0/examples/bar_stacked.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/barh.py` & `mpl_ascii-0.3.0/examples/barh.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/categorical_variables.py` & `mpl_ascii-0.3.0/examples/categorical_variables.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/cohere.py` & `mpl_ascii-0.3.0/examples/cohere.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/cohere_single_plot.py` & `mpl_ascii-0.3.0/examples/cohere_single_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/csd_demo.py` & `mpl_ascii-0.3.0/examples/csd_demo.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/double_plot.py` & `mpl_ascii-0.3.0/examples/double_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/hist_best_fit_line.py` & `mpl_ascii-0.3.0/examples/hist_best_fit_line.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/hist_simple.py` & `mpl_ascii-0.3.0/examples/hist_simple.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/hist_simple_colors.py` & `mpl_ascii-0.3.0/examples/hist_simple_colors.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/lines_multi_color.py` & `mpl_ascii-0.3.0/examples/lines_multi_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/scatter_multi_color.py` & `mpl_ascii-0.3.0/examples/scatter_multi_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/examples/simple_plot.py` & `mpl_ascii-0.3.0/examples/simple_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/mpl_ascii/__init__.py` & `mpl_ascii-0.3.0/mpl_ascii/draw.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,241 +1,301 @@
-from matplotlib._pylab_helpers import Gcf
-
-from matplotlib.backends.backend_agg import (
-    FigureManagerBase,
-    RendererAgg,
-    FigureCanvasAgg,
-)
+import math
 from matplotlib.collections import PathCollection
 from matplotlib.container import BarContainer
-from matplotlib.figure import Figure
 from matplotlib.lines import Line2D
 from matplotlib.patches import Rectangle
 import numpy as np
 
 from mpl_ascii.ascii_canvas import AsciiCanvas
-from mpl_ascii.color_map import map_color_to_ascii
-from mpl_ascii.draw import draw_bar, draw_frame, draw_line, draw_x_ticks, draw_y_ticks
-from mpl_ascii.tools import linear_transform
-
-AXES_WIDTH = 150
-AXES_HEIGHT = 40
-
-class RendererAscii(RendererAgg):
-
-    def __init__(self, width, height, dpi):
-        super(RendererAscii, self).__init__(width, height, dpi)
-        self.texts = []
-        self.tick_info = []
-
-    def clear(self):
-        super(RendererAscii, self).clear()
-        self.texts = []
-        self.tick_info = []
-
-    def draw_text(self, gc, x, y, s, prop, angle, ismath=False, mtext=None):
-        super(RendererAscii, self).draw_text(
-            gc, x, y, s, prop, angle, ismath=ismath, mtext=mtext
+from mpl_ascii.color_map import ax_color_map, std_color
+from mpl_ascii.tools import linear_transform, scale_factor
+
+def draw_ax(ax, axes_height, axes_width):
+    frame_buffer_left = 1
+    frame_buffer_right = 1
+    frame_buffer_top = 1
+    frame_buffer_bottom = 1
+
+
+    frame_width = axes_width + frame_buffer_left + frame_buffer_right
+    frame_height = axes_height + frame_buffer_top + frame_buffer_bottom
+
+    color_to_ascii = ax_color_map(ax)
+
+    x_range = ax.get_xlim()
+    if x_range[1] < x_range[0]:
+        x_range = x_range[1], x_range[0]
+
+    y_range = ax.get_ylim()
+    if y_range[1] < y_range[0]:
+        y_range = y_range[1], y_range[0]
+
+    x_min, x_max = x_range
+    y_min, y_max = y_range
+
+    canvas = AsciiCanvas(np.full((axes_height, axes_width), fill_value=" "))
+
+    all_bars = []
+
+    for container in ax.containers:
+        if not isinstance(container, BarContainer):
+            continue
+        for bar in container.patches:
+            if not isinstance(bar, Rectangle):
+                continue
+            all_bars.append(bar)
+
+    for bar in all_bars:
+        char = color_to_ascii[std_color(bar.get_facecolor())]
+
+        canvas_bar = AsciiCanvas(
+                draw_bar(
+                bar.get_height(),
+                bar.get_width(),
+                axes_height,
+                axes_width,
+                x_range,
+                y_range,
+                char
+            )
+        )
+        ascii_x_bar = round(linear_transform(bar.xy[0], x_min, x_max, 0, axes_width-1))
+        ascii_y_bar = round(linear_transform(bar.xy[1], y_min, y_max, 1, axes_height))
+
+        canvas = canvas.update(canvas_bar, (axes_height - ascii_y_bar - canvas_bar.shape[0]+1, ascii_x_bar))
+
+
+    for line in ax.get_lines():
+        char = color_to_ascii[std_color(line.get_color())]
+        xy_data = line.get_xydata()
+        x_data, y_data = [dat[0] for dat in xy_data], [dat[1] for dat in xy_data]
+
+        line = AsciiCanvas(
+                draw_line(
+                width=axes_width,
+                height=axes_height,
+                x_data=x_data,
+                y_data=y_data,
+                x_range=x_range,
+                y_range=y_range,
+                char = char
+            )
         )
 
-        if mtext is not None:
-            self.texts.append(mtext)
+        canvas = canvas.update(line, (0,0))
+
+    for collection in ax.collections:
+        if not isinstance(collection, PathCollection):
+            continue
+        offsets = collection.get_offsets()
+
+        color = collection.get_facecolors()[0]
+        for point in offsets:
+            color = tuple(color)
+
+            x_new = round(linear_transform(point[0], x_min, x_max, 0, axes_width-1))
+            y_new = round(linear_transform(point[1], y_min, y_max, 1, axes_height))
+
+            canvas = canvas.update(AsciiCanvas(np.array([[color_to_ascii[std_color(color)]]])), (axes_height-y_new, x_new))
 
 
-def show():
-    for manager in Gcf.get_all_fig_managers():
-        canvas = manager.canvas
-        canvas.draw()
-        string = canvas.to_txt()
-        print(string)
 
+    # for text in ax.texts:
+    #     text_canvas = AsciiCanvas(np.array([list(text.get_text())]))
+    #     ascii_x = round(linear_transform(text.xy[0], x_min, x_max, 0, axes_width-1))
+    #     ascii_y = round(linear_transform(text.xy[1], y_min, y_max, 1, axes_height))
+    #     canvas = canvas.update(text_canvas, (axes_height - ascii_y, ascii_x))
 
-class FigureCanvasAscii(FigureCanvasAgg):
+    canvas = canvas.update(AsciiCanvas(draw_frame(frame_height, frame_width)), (-frame_buffer_left,-frame_buffer_top))
 
-    def __init__(self, figure: Figure | None = ...) -> None:
-        super().__init__(figure)
-        self.tick_info = []
+    tick_data = [tick.get_position()[0] for tick in ax.xaxis.get_ticklabels()]
+    label_data = [tick.get_text().replace("\n", "") for tick in ax.xaxis.get_ticklabels()]
+    xticks = AsciiCanvas(draw_x_ticks(axes_width, tick_data, label_data, x_range))
 
-    def get_renderer(self):
-        w, h = self.figure.bbox.size
-        key = w, h, self.figure.dpi
-        reuse_renderer = self._lastKey == key
-        if not reuse_renderer:
-            self.renderer = RendererAscii(w, h, self.figure.dpi)
-            self._lastKey = key
-        return self.renderer
+    xlabel = AsciiCanvas(np.array([list(ax.get_xlabel())]))
 
-    def to_txt(self, sep="\n", tw=240, invert=False, threshold=200):
-        self.draw()
+    xticks_and_label = xticks.update(xlabel, location=(xticks.shape[0],int(xticks.shape[1] / 2)))
 
-        figure = self.figure
+    canvas = canvas.update(xticks_and_label, location=(canvas.shape[0]-1, 1))
 
-        axes_height = AXES_HEIGHT
-        axes_width = AXES_WIDTH
+    tick_data = [tick.get_loc() for tick in ax.yaxis.get_major_ticks()]
+    label_data = [tick.label1.get_text().replace("\n", "") for tick in ax.yaxis.get_major_ticks()]
+    yticks = AsciiCanvas(draw_y_ticks(axes_height, tick_data, label_data, y_range))
 
-        frame_buffer_left = 1
-        frame_buffer_right = 1
-        frame_buffer_top = 1
-        frame_buffer_bottom = 1
+    ylabel = AsciiCanvas(np.array([list(ax.get_ylabel())]).T)
+    yticks_and_label = yticks.update(ylabel, location=(int(yticks.shape[0] / 2), -(ylabel.shape[1] + 1)))
 
+    canvas = canvas.update(yticks_and_label, location=(1, -yticks_and_label.shape[1]+1))
 
-        frame_width = axes_width + frame_buffer_left + frame_buffer_right
-        frame_height = axes_height + frame_buffer_top + frame_buffer_bottom
 
-        ascii_canvases = []
-        for ax in figure.axes:
-            color_to_ascii = map_color_to_ascii(ax)
+    ax_title = AsciiCanvas(np.array([list(ax.get_title())]))
+    canvas = canvas.update(ax_title, location=(-(ax_title.shape[0] + 1), int(canvas.shape[1] / 2)))
 
-            x_range = ax.get_xlim()
-            if x_range[1] < x_range[0]:
-                x_range = x_range[1], x_range[0]
+    legend = ax.get_legend()
+    if legend:
+        handles, text = legend.legendHandles, legend.texts
 
-            y_range = ax.get_ylim()
-            if y_range[1] < y_range[0]:
-                y_range = y_range[1], y_range[0]
+        canvas_legend = AsciiCanvas()
+        for handle, text in zip(handles, text):
+            char = " "
+            if isinstance(handle, Rectangle):
+                char = color_to_ascii[std_color(handle.get_facecolor())]
+            if isinstance(handle, Line2D):
+                char = color_to_ascii[std_color(handle.get_color())]
+            if isinstance(handle, PathCollection):
+                color = tuple(handle.get_facecolor()[0])
+                char = color_to_ascii[std_color(color)]
 
-            x_min, x_max = x_range
-            y_min, y_max = y_range
+            arr = np.array([[char] * 3 + [" "] + list(text.get_text())])
+            canvas_legend = canvas_legend.update(AsciiCanvas(arr), (canvas_legend.shape[0], 0))
 
-            canvas = AsciiCanvas(np.full((axes_height, axes_width), fill_value=" "))
+        title = legend.get_title().get_text() or "Legend"
+        title = AsciiCanvas(np.array([list(title)]))
+        canvas_legend = canvas_legend.update(title, (-2,0))
+        legend_frame = AsciiCanvas(draw_frame(canvas_legend.shape[0]+2, canvas_legend.shape[1]+4))
+        canvas_legend = legend_frame.update(canvas_legend, (1,2))
 
-            all_bars = []
+        canvas = canvas.update(canvas_legend, (canvas.shape[0] + 1, round(canvas.shape[1] / 2) ))
 
-            for container in ax.containers:
-                if not isinstance(container, BarContainer):
-                    continue
-                for bar in container.patches:
-                    if not isinstance(bar, Rectangle):
-                        continue
-                    all_bars.append(bar)
+    return canvas
 
-            for bar in all_bars:
-                char = color_to_ascii[bar.get_facecolor()]
 
-                canvas_bar = AsciiCanvas(
-                        draw_bar(
-                        bar.get_height(),
-                        bar.get_width(),
-                        axes_height,
-                        axes_width,
-                        x_range,
-                        y_range,
-                        char
-                    )
-                )
+def draw_frame(height, width):
+    frame = np.full((height, width), fill_value=" ")
+    frame[0,:] = "-"
+    frame[-1,:] = "-"
+    frame[:,0] = "|"
+    frame[:,-1] = "|"
 
-                ascii_x_bar = round(linear_transform(bar.xy[0], x_min, x_max, 0, axes_width-1))
-                ascii_y_bar = round(linear_transform(bar.xy[1], y_min, y_max, 1, axes_height))
+    frame[0,0] = "+"
+    frame[0,-1] = "+"
+    frame[-1,0] = "+"
+    frame[-1,-1] = "+"
 
-                canvas = canvas.update(canvas_bar, (axes_height - ascii_y_bar - canvas_bar.shape[0]+1, ascii_x_bar))
+    return frame
 
-            for line in ax.get_lines():
-                char = color_to_ascii[line.get_color()]
-                xy_data = line.get_xydata()
-                x_data, y_data = [dat[0] for dat in xy_data], [dat[1] for dat in xy_data]
 
-                line = AsciiCanvas(
-                        draw_line(
-                        width=axes_width,
-                        height=axes_height,
-                        x_data=x_data,
-                        y_data=y_data,
-                        x_range=x_range,
-                        y_range=y_range,
-                        char = char
-                    )
-                )
+def draw_line(height, width, x_data, y_data, x_range, y_range, char):
 
-                canvas = canvas.update(line, (0,0))
+    x_min, x_max = x_range[0], x_range[1]
+    y_min, y_max = y_range[0], y_range[1]
 
-            for collection in ax.collections:
-                if not isinstance(collection, PathCollection):
-                    continue
-                offsets = collection.get_offsets()
+    plot_x = []
+    plot_y = []
+    for x,y in zip(x_data, y_data):
+        if x < x_min or x > x_max:
+            continue
+        if y < y_min or y > y_max:
+            continue
+        plot_x.append(x)
+        plot_y.append(y)
 
-                color = collection.get_facecolors()[0]
-                for point in offsets:
-                    color = tuple(color)
 
-                    x_new = round(linear_transform(point[0], x_min, x_max, 0, axes_width-1))
-                    y_new = round(linear_transform(point[1], y_min, y_max, 1, axes_height))
+    ascii_x_data = [
+        round(linear_transform(x, x_min, x_max, 0, width-1)) for x in plot_x if (x <= x_max and x >= x_min)
+    ]
+    ascii_y_data = [
+        round(linear_transform(y, y_min, y_max, 1, height)) for y in plot_y if (y <= y_max and y >= y_min)
+    ]
 
-                    canvas = canvas.update(AsciiCanvas(np.array([[color_to_ascii[color]]])), (axes_height-y_new, x_new))
+    line_canvas_arr = np.full((height, width), fill_value=" ", dtype="object")
 
+    start_points = zip(ascii_x_data[:-1], ascii_y_data[:-1])
+    end_points = zip(ascii_x_data[1:], ascii_y_data[1:])
+    join_line_points = []
+    for start, end in zip(start_points, end_points):
+        line_points = bresenham_line(start[0], start[1], end[0], end[1])
+        if len(line_points) > 2:
+            join_line_points += line_points[1:-1]
 
+    for x, y in zip(ascii_x_data, ascii_y_data):
+        row = height - y
+        col = x
+        line_canvas_arr[row, col] = char
 
-            # for text in ax.texts:
-            #     text_canvas = AsciiCanvas(np.array([list(text.get_text())]))
-            #     ascii_x = round(linear_transform(text.xy[0], x_min, x_max, 0, axes_width-1))
-            #     ascii_y = round(linear_transform(text.xy[1], y_min, y_max, 1, axes_height))
-            #     canvas = canvas.update(text_canvas, (axes_height - ascii_y, ascii_x))
+    for x,y in join_line_points:
+        row = height - y
+        col = x
+        line_canvas_arr[row, col] = char
 
-            canvas = canvas.update(AsciiCanvas(draw_frame(frame_height, frame_width)), (-frame_buffer_left,-frame_buffer_top))
+    return line_canvas_arr
 
-            tick_data = [tick.get_position()[0] for tick in ax.xaxis.get_ticklabels()]
-            label_data = [tick.get_text().replace("\n", "") for tick in ax.xaxis.get_ticklabels()]
-            xticks = AsciiCanvas(draw_x_ticks(axes_width, tick_data, label_data, x_range))
+def draw_bar(bar_height, bar_width, ax_height, ax_width, x_range, y_range, char):
+    x_min, x_max = x_range[0], x_range[1]
+    y_min, y_max = y_range[0], y_range[1]
 
-            xlabel = AsciiCanvas(np.array([list(ax.get_xlabel())]))
+    ascii_width_bar = round(bar_width * scale_factor(x_min, x_max, 0, ax_width-1))
+    ascii_height_bar = round(bar_height * scale_factor(y_min, y_max, 1, ax_height))
 
-            xticks_and_label = xticks.update(xlabel, location=(xticks.shape[0],int(xticks.shape[1] / 2)))
+    return np.full((ascii_height_bar, ascii_width_bar), fill_value=char)
 
-            canvas = canvas.update(xticks_and_label, location=(canvas.shape[0]-1, 1))
+def draw_x_ticks(width, tick_data, tick_label_data, x_range):
+    x_min, x_max = x_range[0], x_range[1]
 
-            tick_data = [tick.get_loc() for tick in ax.yaxis.get_major_ticks()]
-            label_data = [tick.label1.get_text().replace("\n", "") for tick in ax.yaxis.get_major_ticks()]
-            yticks = AsciiCanvas(draw_y_ticks(axes_height, tick_data, label_data, y_range))
+    xticks = np.full((2, width), " ")
+    for x, label in zip(tick_data, tick_label_data):
+        x = round(linear_transform(x, x_min, x_max, 0, width-1))
+        if x < 0 or x >= width:
+            continue
+        xticks[0:1,x] = "|"
+        for i, char in enumerate(list(label)):
+            xticks[-1, x - len(label) + i+1] = char
 
-            ylabel = AsciiCanvas(np.array([list(ax.get_ylabel())]).T)
-            yticks_and_label = yticks.update(ylabel, location=(int(yticks.shape[0] / 2), -(ylabel.shape[1] + 1)))
+    return xticks
 
-            canvas = canvas.update(yticks_and_label, location=(1, -yticks_and_label.shape[1]+1))
+def draw_y_ticks(height, tick_data, tick_label_data, y_range):
+    y_min, y_max = y_range[0], y_range[1]
 
+    yticks_width = max([len(label) for label in tick_label_data]) + 2
+    yticks = np.full((height, yticks_width), " ")
 
-            ax_title = AsciiCanvas(np.array([list(ax.get_title())]))
-            canvas = canvas.update(ax_title, location=(-(ax_title.shape[0] + 1), int(canvas.shape[1] / 2)))
+    for y, label in zip(tick_data, tick_label_data):
+        y = round(linear_transform(y, y_min, y_max, 1, height))
+        if y <= 0 or y > height:
+            continue
+        row = height - y
+        yticks[row,-2:] = "-"
+        for i, char in enumerate(list(label)):
+            yticks[row, -len(label) - 2 + i] = char
 
-            legend = ax.get_legend()
-            if legend:
-                handles, text = legend.legendHandles, legend.texts
+    return yticks
 
-                canvas_legend = AsciiCanvas()
-                for handle, text in zip(handles, text):
-                    char = " "
-                    if isinstance(handle, Rectangle):
-                        char = color_to_ascii[handle.get_facecolor()]
-                    if isinstance(handle, Line2D):
-                        char = color_to_ascii[handle.get_color()]
-                    if isinstance(handle, PathCollection):
-                        color = tuple(handle.get_facecolor()[0])
-                        char = color_to_ascii[color]
 
-                    arr = np.array([[char] * 3 + [" "] + list(text.get_text())])
-                    canvas_legend = canvas_legend.update(AsciiCanvas(arr), (canvas_legend.shape[0], 0))
+def bresenham_line(x0, y0, x1, y1):
+    dx = x1 - x0
+    dy = y1 - y0
 
-                title = legend.get_title().get_text() or "Legend"
-                title = AsciiCanvas(np.array([list(title)]))
-                canvas_legend = canvas_legend.update(title, (-2,0))
-                legend_frame = AsciiCanvas(draw_frame(canvas_legend.shape[0]+2, canvas_legend.shape[1]+4))
-                canvas_legend = legend_frame.update(canvas_legend, (1,2))
+    # Determine how steep the line is
+    is_steep = abs(dy) > abs(dx)
 
-                canvas = canvas.update(canvas_legend, (canvas.shape[0] + 1, round(canvas.shape[1] / 2) ))
+    # Rotate line if it's steep
+    if is_steep:
+        x0, y0 = y0, x0
+        x1, y1 = y1, x1
 
-            ascii_canvases.append(canvas)
+    # Swap start and end points if necessary
+    if x0 > x1:
+        x0, x1 = x1, x0
+        y0, y1 = y1, y0
 
-        image_canvas = AsciiCanvas()
-        for canvas in ascii_canvases:
-            image_canvas = image_canvas.update(canvas, (image_canvas.shape[0], 0))
+    # Recalculate differences
+    dx = x1 - x0
+    dy = y1 - y0
 
-        return str(image_canvas)
+    # Calculate error
+    error = int(dx / 2.0)
+    ystep = 1 if y0 < y1 else -1
 
+    # Iterate over bounding box generating points between start and end
+    y = y0
+    points = []
+    for x in range(x0, x1 + 1):
+        coord = (y, x) if is_steep else (x, y)
+        points.append(coord)
+        error -= abs(dy)
+        if error < 0:
+            y += ystep
+            error += dx
 
-    def print_txt(self, filename, **kwargs):
-        if isinstance(filename, str):
-            with open(filename, "w") as f:
-                f.write(self.to_txt())
-        else:
-            filename.write(self.to_txt().encode())
+    return points
 
 
-FigureCanvas = FigureCanvasAscii
-FigureManager = FigureManagerBase
```

### Comparing `mpl_ascii-0.2.0/mpl_ascii/ascii_canvas.py` & `mpl_ascii-0.3.0/mpl_ascii/ascii_canvas.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,11 +27,24 @@
         res = np.where(self.array==" ", ".", self.array)
         return AsciiCanvas(res)
 
 
     def __str__(self) -> str:
         res = []
         for row in self.array:
-            res.append("".join(row.tolist()))
+            res.append("".join([str(char) for char in row.tolist()]))
+
+        res = "\n".join(res)
+        return res
+
+    def __rich__(self) -> str:
+        res = []
+        for row in self.array:
+            row_colors = []
+            for char in row:
+                if hasattr(char, "__rich__"):
+                    char = char.__rich__()
+                row_colors.append(char)
+            res.append("".join(row_colors))
 
         res = "\n".join(res)
         return res
```

### Comparing `mpl_ascii-0.2.0/mpl_ascii/overlay.py` & `mpl_ascii-0.3.0/mpl_ascii/overlay.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     max_row = max(start_row + foreground.shape[0], background.shape[0])
     max_col = max(start_col + foreground.shape[1], background.shape[1])
 
     total_rows = max_row - min_row
     total_cols = max_col - min_col
 
     # Create the resulting array filled with spaces (or appropriate background fill)
-    result = np.full((total_rows, total_cols), ' ', dtype='<U32')
+    result = np.full((total_rows, total_cols), ' ', dtype="object")
     bg_start_row = max(-min_row, 0)  # This will be 0 if start_row is >= 0
     bg_start_col = max(-min_col, 0)  # This will be 0 if start_col is >= 0
     result[bg_start_row:bg_start_row+background.shape[0],
            bg_start_col:bg_start_col+background.shape[1]] = background
 
     fg_start_row = max(start_row - min_row, 0)
     fg_start_col = max(start_col - min_col, 0)
```

### Comparing `mpl_ascii-0.2.0/mpl_ascii.egg-info/SOURCES.txt` & `mpl_ascii-0.3.0/mpl_ascii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.2.0/tests/test_overlay.py` & `mpl_ascii-0.3.0/tests/test_overlay.py`

 * *Files identical despite different names*

