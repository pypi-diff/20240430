# Comparing `tmp/py50-1.0.0.tar.gz` & `tmp/py50-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py50-1.0.0.tar", max compression
+gzip compressed data, was "py50-1.0.1.tar", max compression
```

## Comparing `py50-1.0.0.tar` & `py50-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-11-15 10:28:16.943898 py50-1.0.0/LICENSE
--rw-r--r--   0        0        0     4542 2024-04-29 03:50:21.000706 py50-1.0.0/README_pypi.md
--rw-r--r--   0        0        0     6148 2024-02-12 06:00:11.583727 py50-1.0.0/py50/.DS_Store
--rw-r--r--   0        0        0      177 2024-04-17 01:25:24.147050 py50-1.0.0/py50/__init__.py
--rw-r--r--   0        0        0    20268 2024-04-26 14:38:41.720572 py50-1.0.0/py50/calculator.py
--rw-r--r--   0        0        0     8604 2024-01-29 16:09:38.892265 py50-1.0.0/py50/plot_settings.py
--rw-r--r--   0        0        0    43456 2024-04-20 15:15:35.300736 py50-1.0.0/py50/plotcurve.py
--rw-r--r--   0        0        0    88711 2024-04-29 03:02:08.739556 py50-1.0.0/py50/stats.py
--rw-r--r--   0        0        0     6413 2024-04-20 14:15:03.007112 py50-1.0.0/py50/utils.py
--rw-r--r--   0        0        0      515 2024-04-29 01:15:06.686222 py50-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5335 1970-01-01 00:00:00.000000 py50-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-11-15 10:28:16.943898 py50-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4542 2024-04-29 03:50:21.000706 py50-1.0.1/README_pypi.md
+-rw-r--r--   0        0        0     6148 2024-02-12 06:00:11.583727 py50-1.0.1/py50/.DS_Store
+-rw-r--r--   0        0        0      177 2024-04-17 01:25:24.147050 py50-1.0.1/py50/__init__.py
+-rw-r--r--   0        0        0    20268 2024-04-26 14:38:41.720572 py50-1.0.1/py50/calculator.py
+-rw-r--r--   0        0        0     8604 2024-01-29 16:09:38.892265 py50-1.0.1/py50/plot_settings.py
+-rw-r--r--   0        0        0    43460 2024-04-30 01:26:56.191290 py50-1.0.1/py50/plotcurve.py
+-rw-r--r--   0        0        0    88711 2024-04-29 03:02:08.739556 py50-1.0.1/py50/stats.py
+-rw-r--r--   0        0        0     6413 2024-04-20 14:15:03.007112 py50-1.0.1/py50/utils.py
+-rw-r--r--   0        0        0      564 2024-04-30 05:43:59.343236 py50-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5410 1970-01-01 00:00:00.000000 py50-1.0.1/PKG-INFO
```

### Comparing `py50-1.0.0/LICENSE` & `py50-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py50-1.0.0/README_pypi.md` & `py50-1.0.1/README_pypi.md`

 * *Files identical despite different names*

### Comparing `py50-1.0.0/py50/.DS_Store` & `py50-1.0.1/py50/.DS_Store`

 * *Files identical despite different names*

### Comparing `py50-1.0.0/py50/calculator.py` & `py50-1.0.1/py50/calculator.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.0/py50/plot_settings.py` & `py50-1.0.1/py50/plot_settings.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.0/py50/plotcurve.py` & `py50-1.0.1/py50/plotcurve.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,54 +93,54 @@
         :param xlabel: str
             Title of the X-axis
         :param ylabel: str
             Title of the Y-axis
         :param axis_fontsize: int
             Modify axis label font size
         :param conc_unit: str
-            Input unit of concentration. Can accept nanomolar (nM) and micromolar (uM or µM). If the \
-        units are different, for example in the DataFrame units are in nM, but the units for the graph are µM, the \
-        units from the DataFrame will be converted to match the conc_unit input. The final plot will scale based on \
-        the conc_unit input. By default, it will assume input concentration will be in nM.
+            Input unit of concentration. Can accept nanomolar (nM) and micromolar (uM or µM). If the units are
+            different, for example in the DataFrame units are in nM, but the units for the graph are µM, the units from
+            the DataFrame will be converted to match the conc_unit input. The final plot will scale based on the
+            conc_unit input. By default, it will assume input concentration will be in nM.
         :param xscale: int
             Set the scale of the X-axis as logarithmic or linear. It is logarithmic by default.
         :param xscale_ticks: tuple
             Set the scale of the X-axis
         :param ymax: int
             Give a set maximum limit for the Y-Axis
         :param ymin: int
             Give a set minimum limit for the Y-Axis
         :param line_color: str.
-            Takes a list of colors. By default, it uses the CBPALETTE. List can contain name of colors or colors in hex\
-        code.
+            Takes a list of colors. By default, it uses the CBPALETTE. List can contain name of colors or colors in hex
+            code.
         :param line_width: int
             Set width of lines in plot.
         :param marker: Optional, list
             Takes a list of for point markers.
         :param legend: Optional, bool
             Denotes a figure legend.
         :param legend_loc: str
-        Determine legend location. Default is best. Matplotlib options can be found here \
+        Determine legend location. Default is best. Matplotlib options can be found here
         https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.legend.html
         :param box: Optional bool.
-            Draw a box to highlight a specific location. If box = True, then the box_color, \
-        box_intercept, and x_concentration MUST ALSO BE GIVEN.
+            Draw a box to highlight a specific location. If box = True, then the box_color, box_intercept, and
+            x_concentration MUST ALSO BE GIVEN.
         :param box_color: str
             Set color of box. Default is gray.
         :param box_intercept: int
             Set horizontal location of box. By default, it is set at 50% of the Y-axis.
         :param conc_target: int
-            Set vertical location of the box. By default, this is set to None. For example, if the \
-        box_intercept is set to 50%, then the x_concentration must be the Absolute IC50 value. If there is an input to \
-        x_concentration, it will override the box_intercept and the response data will move accordingly. Finally, the \
-        number must be in the same unit as the X-axis. i.e., if the axis is in µM, then the number for the \
-        x_concentration should be in µM and vice versa.
+            Set vertical location of the box. By default, this is set to None. For example, if the box_intercept is set
+            to 50%, then the x_concentration must be the Absolute IC50 value. If there is an input to x_concentration,
+            it will override the box_intercept and the response data will move accordingly. Finally, the number must be
+            in the same unit as the X-axis. i.e., if the axis is in µM, then the number for the x_concentration should
+            be in µM and vice versa.
         :param hline: Int or float
-            Draw a horizontal line across the graph. This line will stretch across the length of the plot. This is \
-        optional and set to 0 by default.
+            Draw a horizontal line across the graph. This line will stretch across the length of the plot. This is
+            optional and set to 0 by default.
         :param hline_color: str
             Set color of horizontal line. Default color is gray.
         :param vline: int or float
             This line will stretch across the height of the plot. This is  optional and set to 0 by default.
         :param vline_color: str
             Set color of vertical line. Default color is gray.
         :param figsize: tuple
@@ -384,49 +384,47 @@
         :param plot_title_size: int
             Modify plot title font size
         :param xlabel: str
             Title of the X-axis
         :param ylabel: str
             Title of the Y-axis
         :param conc_unit: str
-            Input will assume that the concentration will be in nM. \
-        Thus, it will be automatically converted into µM. \
-        If xscale_unit is given as nM, no conversion will be performed.
+            Input will assume that the concentration will be in nM. Thus, it will be automatically converted into µM. If
+            xscale_unit is given as nM, no conversion will be performed.
         :param xscale: str
             Set the scale of the X-axis as logarithmic or linear. It is logarithmic by default.
         :param xscale_ticks: tuple
             Set the scale of the X-axis
         :param ymax: int
             Give a set maximum limit for the Y-Axis
         :param ymin: int
             Give a set minimum limit for the Y-Axis
         :param axis_fontsize:int
             Modify axis label font size
         :param line_color: str
-        Takes a list of colors. By default, it uses the CBPALETTE. List can contain name of \
-        colors or colors in hex code.
+        Takes a list of colors. By default, it uses the CBPALETTE. List can contain name of colors or colors in hex
+        code.
         :param line_width: int
             Set width of lines in plot.
         :param marker: list
-        Takes a list for point markers. Marker options can be found here: \
-        https://matplotlib.org/stable/api/markers_api.html
+        Takes a list for point markers. Marker options can be found here: https://matplotlib.org/stable/api/markers_api.html
         :param legend: bool
             Denotes a figure legend.
         :param legend_loc: str
-            Determine legend location. Matplotlib options can be found here \
-        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.legend.html
+            Determine legend location. Matplotlib options can be found here
+            https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.legend.html
         :param box_target: str
             Draw a box to highlight a specific drug curve. Must use specific drug name.
         :param box_color: str
             Set color of box. Default color is gray.
         :param box_intercept: int
             Set horizontal location of box. By default, it is set at Absolute IC50.
         :param hline: int or float
-            Draw a horizontal line that will stretch across the length of the plot. This is \
-        optional and set to 0 by default.
+            Draw a horizontal line that will stretch across the length of the plot. This is optional and set to 0 by
+            default.
         :param hline_color: str
             Set color of horizontal line. Default color is gray.
         :param vline: int or float
             Draw a line that will stretch across the height of the plot. This is  optional and set to 0 by default.
         :param vline_color: str
             Set color of vertical line. Default color is gray.
         :param figsize: tuple
@@ -776,39 +774,39 @@
         :param ylabel: str
             Title of the Y-axis
         :param ymax: int
             Give a set maximum limit for the Y-Axis
         :param ymin: int
             Give a set minimum limit for the Y-Axis
         :param conc_unit: str
-            Input will assume that the concentration will be in nM. Thus, it will be automatically converted into µM. \
-        If xscale_unit is given as nM, no conversion will be performed.
+            Input will assume that the concentration will be in nM. Thus, it will be automatically converted into µM. If
+            xscale_unit is given as nM, no conversion will be performed.
         :param xscale: str
             Set the scale of the X-axis as logarithmic or linear. It is logarithmic by default.
         :param xscale_ticks: tuple
             Set the scale of the X-axis
         :param line_color: list
-            Takes a list of colors. By default, it uses the CBPALETTE. List can contain name of \
-        colors or colors in hex code.
+            Takes a list of colors. By default, it uses the CBPALETTE. List can contain name of
+            colors or colors in hex code.
         :param line_width: int
             Set width of lines in plot.
         :param box: bool
-        Draw a box to highlight a specific location. If box = True, then the box_color, and box_intercept MUST ALSO BE \
+        Draw a box to highlight a specific location. If box = True, then the box_color, and box_intercept MUST ALSO BE
         GIVEN.
         :param box_color: str
             Set color of box. Default color is gray.
         :param box_intercept: int
             Set horizontal location of box. By default, it is set at Absolute IC50.
         :param hline: int or float
-            Draw horizontal line that will stretch across the length of the plot. This is optional and set to 0 by \
+            Draw horizontal line that will stretch across the length of the plot. This is optional and set to 0 by
             default.
         :param hline_color: str
             Set color of horizontal line. Default color is gray.
         :param vline: int or float
-            Draw a line thatwill stretch across the height of the plot. This is  optional and set to 0 by default.
+            Draw a line that will stretch across the height of the plot. This is  optional and set to 0 by default.
         :param vline_color: str
             Set color of vertical line. Default color is gray.
         :param figsize: tuple
             Set figure size for subplot.
         :param output_filename: str
             File path for save location.
         :param verbose: bool
```

### Comparing `py50-1.0.0/py50/stats.py` & `py50-1.0.1/py50/stats.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.0/py50/utils.py` & `py50-1.0.1/py50/utils.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.0/pyproject.toml` & `py50-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [tool.poetry]
 name = "py50"
-version = "1.0.0"
+version = "1.0.1"
 description = "Generate Dose-Response Curves"
 documentation = "https://py50.readthedocs.io/en/latest/"
 authors = ["Tony Eight Lin <tonyelin@tmu.edu.tw>"]
 license = "GPL-3.0"
 readme = "README_pypi.md"
 packages = [{ include = "py50"}]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.13"
 pandas = "==1.5.0"
 numpy = ">=1.26.2"
 matplotlib = ">=3.8.1"
 scipy = ">=1.11.3"
 seaborn = "==0.12.2"
+scikit-posthocs = ">=0.7.0"
+pingouin = ">=0.5.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `py50-1.0.0/PKG-INFO` & `py50-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: py50
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generate Dose-Response Curves
 License: GPL-3.0
 Author: Tony Eight Lin
 Author-email: tonyelin@tmu.edu.tw
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (>=3.8.1)
 Requires-Dist: numpy (>=1.26.2)
 Requires-Dist: pandas (==1.5.0)
+Requires-Dist: pingouin (>=0.5.4)
+Requires-Dist: scikit-posthocs (>=0.7.0)
 Requires-Dist: scipy (>=1.11.3)
 Requires-Dist: seaborn (==0.12.2)
 Project-URL: Documentation, https://py50.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 
 # py50: Generate Dose-Response Curves
```

