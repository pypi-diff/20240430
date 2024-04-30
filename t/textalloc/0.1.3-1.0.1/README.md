# Comparing `tmp/textalloc-0.1.3.tar.gz` & `tmp/textalloc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textalloc-0.1.3.tar", last modified: Sun Apr 28 19:51:21 2024, max compression
+gzip compressed data, was "textalloc-1.0.1.tar", last modified: Tue Apr 30 21:14:03 2024, max compression
```

## Comparing `textalloc-0.1.3.tar` & `textalloc-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-28 19:51:20.992719 textalloc-0.1.3/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     1077 2023-02-14 19:18:58.000000 textalloc-0.1.3/LICENSE
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     8360 2024-04-28 19:51:20.983723 textalloc-0.1.3/PKG-INFO
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     7697 2024-04-28 19:24:07.000000 textalloc-0.1.3/README.md
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      741 2024-04-28 19:47:07.000000 textalloc-0.1.3/pyproject.toml
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       38 2024-04-28 19:51:20.993718 textalloc-0.1.3/setup.cfg
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-28 19:51:20.694720 textalloc-0.1.3/src/
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-28 19:51:20.830718 textalloc-0.1.3/src/textalloc/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    16374 2024-04-28 19:46:31.000000 textalloc-0.1.3/src/textalloc/__init__.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6539 2024-02-20 19:23:50.000000 textalloc-0.1.3/src/textalloc/candidates.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9795 2024-04-28 19:46:34.000000 textalloc-0.1.3/src/textalloc/non_overlapping_boxes.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    10042 2024-02-20 19:25:04.000000 textalloc-0.1.3/src/textalloc/overlap_functions.py
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-28 19:51:20.972718 textalloc-0.1.3/src/textalloc.egg-info/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     8360 2024-04-28 19:51:20.000000 textalloc-0.1.3/src/textalloc.egg-info/PKG-INFO
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      344 2024-04-28 19:51:20.000000 textalloc-0.1.3/src/textalloc.egg-info/SOURCES.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        1 2024-04-28 19:51:20.000000 textalloc-0.1.3/src/textalloc.egg-info/dependency_links.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       49 2024-04-28 19:51:20.000000 textalloc-0.1.3/src/textalloc.egg-info/requires.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       10 2024-04-28 19:51:20.000000 textalloc-0.1.3/src/textalloc.egg-info/top_level.txt
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:14:03.794313 textalloc-1.0.1/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     1077 2023-02-14 19:18:58.000000 textalloc-1.0.1/LICENSE
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9452 2024-04-30 21:14:03.794313 textalloc-1.0.1/PKG-INFO
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     8788 2024-04-30 21:07:51.000000 textalloc-1.0.1/README.md
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      741 2024-04-30 21:13:50.000000 textalloc-1.0.1/pyproject.toml
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       38 2024-04-30 21:14:03.794313 textalloc-1.0.1/setup.cfg
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:14:03.377790 textalloc-1.0.1/src/
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:14:03.561073 textalloc-1.0.1/src/textalloc/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    14205 2024-04-30 20:51:26.000000 textalloc-1.0.1/src/textalloc/__init__.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6539 2024-02-20 19:23:50.000000 textalloc-1.0.1/src/textalloc/candidates.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9803 2024-04-30 19:38:17.000000 textalloc-1.0.1/src/textalloc/non_overlapping_boxes.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    10042 2024-02-20 19:25:04.000000 textalloc-1.0.1/src/textalloc/overlap_functions.py
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:14:03.777628 textalloc-1.0.1/src/textalloc.egg-info/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9452 2024-04-30 21:14:03.000000 textalloc-1.0.1/src/textalloc.egg-info/PKG-INFO
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      344 2024-04-30 21:14:03.000000 textalloc-1.0.1/src/textalloc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        1 2024-04-30 21:14:03.000000 textalloc-1.0.1/src/textalloc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       49 2024-04-30 21:14:03.000000 textalloc-1.0.1/src/textalloc.egg-info/requires.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       10 2024-04-30 21:14:03.000000 textalloc-1.0.1/src/textalloc.egg-info/top_level.txt
```

### Comparing `textalloc-0.1.3/LICENSE` & `textalloc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `textalloc-0.1.3/PKG-INFO` & `textalloc-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textalloc
-Version: 0.1.3
+Version: 1.0.1
 Summary: Efficient Text Allocation in matplotlib using NumPy Broadcasting
 Author-email: Christoffer Kjellson <c.kjellson@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ckjellson/textalloc
 Project-URL: Bug Tracker, https://github.com/ckjellson/textalloc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -118,26 +118,21 @@
 textcolor: (Union[str, List[str]]), default "k"
     Color code of the text.
 seed: (int), default 0
     Seeds order of text allocations.
 direction: (str), default None
     Sets the preferred direction of the boxes with options:
     (south, north, east, west, northeast, northwest, southeast, southwest).
-x_logscale_base: (int), default None
-    Base of x-axis log-scale, required if the scaling of the x-axis is "log"
-y_logscale_base: (int), default None
-    Base of y-axis log-scale, required if the scaling of the y-axis is "log"
 avoid_label_lines_overlap: (bool), default False
     If set to True, avoids overlap for drawn lines to text labels.
-src_crs: (object), default None
-    Default crs of data, required when using transform in kwargs.
-    For example one can set src_crs=cartopy.crs.TransverseMercator() which is
-    default in matplotlib if using transform=cartopy.crs.PlateCarree().
-plot_kwargs (dict, optional): kwargs for the plt.plot of the lines if draw_lines is True.
-**kwargs: (), kwargs for the plt.text() call.
+plot_kwargs: (dict), default None
+    kwargs for the plt.plot of the lines if draw_lines is True.
+**kwargs: ()
+    kwargs for the plt.text() call.
+    If transform is used, it only needs to be provided here, i.e. not also in plot_kwargs.
 ```
 # Implementation and speed
 
 The implementation aims to plot as many text-boxes as possible in the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
 1. Generate a large number of candidate boxes near the original point with size that matches the fontsize.
@@ -208,7 +203,57 @@
                 textcolor="b")
 plt.show()
 ```
 
 plt.text|textalloc (0.7s)
 :-------------------------:|:-------------------------:
 ![](images/bar_before.png)|![](images/bar_after.png)
+
+# Plotting on images and using transforms
+
+textalloc now also supports plotting on images and using transforms. Below is an eample of using the PlateCarree transform to plot on top of a downloaded OSM-map (thank you @nebukadnezar for the example).
+
+```
+import numpy as np
+import matplotlib.pyplot as plt
+import cartopy.crs as ccrs
+import cartopy.io.img_tiles as cimgt
+import textalloc as ta
+
+np.random.seed(1)
+x = np.random.rand(100)
+x += 150.5
+y = np.random.rand(100)
+y -= 34.5
+
+dpi = 72
+fig = plt.figure(figsize=(800/dpi, 800/dpi), dpi=dpi)
+
+zoom = 10
+sitelon = np.mean(x)
+sitelat = np.mean(y)
+radius = (np.max(x) - np.min(x) ) / 1.5
+ll_lon = sitelon - radius * (1/np.cos(np.radians(sitelat)))
+ll_lat = sitelat - radius
+ur_lon = sitelon + radius * (1/np.cos(np.radians(sitelat)))
+ur_lat = sitelat + radius
+extent = [ll_lon, ur_lon, ll_lat, ur_lat]
+
+request = cimgt.OSM(desired_tile_form="L")
+ax = plt.axes(projection=request.crs)
+ax.set_extent(extent)
+ax.add_image(request, zoom, alpha=0.5, cmap='gray')
+ax.scatter(x, y, c='b', transform=ccrs.PlateCarree())
+
+text_list = [f'Text{i}' for i in range(len(x))]
+ta.allocate_text(fig,ax,x,y,
+                text_list,
+                x_scatter=x, y_scatter=y,
+                textsize=10,
+                draw_lines=True,
+                linewidth=0.5,
+                draw_all=False,
+                transform=ccrs.PlateCarree(),
+                avoid_label_lines_overlap=True)
+plt.show()
+```
+![](images/cartopy.png)
```

### Comparing `textalloc-0.1.3/README.md` & `textalloc-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -100,26 +100,21 @@
 textcolor: (Union[str, List[str]]), default "k"
     Color code of the text.
 seed: (int), default 0
     Seeds order of text allocations.
 direction: (str), default None
     Sets the preferred direction of the boxes with options:
     (south, north, east, west, northeast, northwest, southeast, southwest).
-x_logscale_base: (int), default None
-    Base of x-axis log-scale, required if the scaling of the x-axis is "log"
-y_logscale_base: (int), default None
-    Base of y-axis log-scale, required if the scaling of the y-axis is "log"
 avoid_label_lines_overlap: (bool), default False
     If set to True, avoids overlap for drawn lines to text labels.
-src_crs: (object), default None
-    Default crs of data, required when using transform in kwargs.
-    For example one can set src_crs=cartopy.crs.TransverseMercator() which is
-    default in matplotlib if using transform=cartopy.crs.PlateCarree().
-plot_kwargs (dict, optional): kwargs for the plt.plot of the lines if draw_lines is True.
-**kwargs: (), kwargs for the plt.text() call.
+plot_kwargs: (dict), default None
+    kwargs for the plt.plot of the lines if draw_lines is True.
+**kwargs: ()
+    kwargs for the plt.text() call.
+    If transform is used, it only needs to be provided here, i.e. not also in plot_kwargs.
 ```
 # Implementation and speed
 
 The implementation aims to plot as many text-boxes as possible in the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
 1. Generate a large number of candidate boxes near the original point with size that matches the fontsize.
@@ -190,7 +185,57 @@
                 textcolor="b")
 plt.show()
 ```
 
 plt.text|textalloc (0.7s)
 :-------------------------:|:-------------------------:
 ![](images/bar_before.png)|![](images/bar_after.png)
+
+# Plotting on images and using transforms
+
+textalloc now also supports plotting on images and using transforms. Below is an eample of using the PlateCarree transform to plot on top of a downloaded OSM-map (thank you @nebukadnezar for the example).
+
+```
+import numpy as np
+import matplotlib.pyplot as plt
+import cartopy.crs as ccrs
+import cartopy.io.img_tiles as cimgt
+import textalloc as ta
+
+np.random.seed(1)
+x = np.random.rand(100)
+x += 150.5
+y = np.random.rand(100)
+y -= 34.5
+
+dpi = 72
+fig = plt.figure(figsize=(800/dpi, 800/dpi), dpi=dpi)
+
+zoom = 10
+sitelon = np.mean(x)
+sitelat = np.mean(y)
+radius = (np.max(x) - np.min(x) ) / 1.5
+ll_lon = sitelon - radius * (1/np.cos(np.radians(sitelat)))
+ll_lat = sitelat - radius
+ur_lon = sitelon + radius * (1/np.cos(np.radians(sitelat)))
+ur_lat = sitelat + radius
+extent = [ll_lon, ur_lon, ll_lat, ur_lat]
+
+request = cimgt.OSM(desired_tile_form="L")
+ax = plt.axes(projection=request.crs)
+ax.set_extent(extent)
+ax.add_image(request, zoom, alpha=0.5, cmap='gray')
+ax.scatter(x, y, c='b', transform=ccrs.PlateCarree())
+
+text_list = [f'Text{i}' for i in range(len(x))]
+ta.allocate_text(fig,ax,x,y,
+                text_list,
+                x_scatter=x, y_scatter=y,
+                textsize=10,
+                draw_lines=True,
+                linewidth=0.5,
+                draw_all=False,
+                transform=ccrs.PlateCarree(),
+                avoid_label_lines_overlap=True)
+plt.show()
+```
+![](images/cartopy.png)
```

### Comparing `textalloc-0.1.3/pyproject.toml` & `textalloc-1.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "textalloc"
-version = "0.1.3"
+version = "1.0.1"
 authors = [
   { name="Christoffer Kjellson", email="c.kjellson@gmail.com" },
 ]
 license = {text = "MIT License"}
 description = "Efficient Text Allocation in matplotlib using NumPy Broadcasting"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `textalloc-0.1.3/src/textalloc/candidates.py` & `textalloc-1.0.1/src/textalloc/candidates.py`

 * *Files identical despite different names*

### Comparing `textalloc-0.1.3/src/textalloc/non_overlapping_boxes.py` & `textalloc-1.0.1/src/textalloc/non_overlapping_boxes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from typing import Tuple, List
-from textalloc.candidates import generate_candidates
-from textalloc.overlap_functions import (
+from src.textalloc.candidates import generate_candidates
+from src.textalloc.overlap_functions import (
     non_overlapping_with_points,
     non_overlapping_with_lines,
     non_overlapping_with_boxes,
     inside_plot,
 )
 
 try:
```

### Comparing `textalloc-0.1.3/src/textalloc/overlap_functions.py` & `textalloc-1.0.1/src/textalloc/overlap_functions.py`

 * *Files identical despite different names*

### Comparing `textalloc-0.1.3/src/textalloc.egg-info/PKG-INFO` & `textalloc-1.0.1/src/textalloc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textalloc
-Version: 0.1.3
+Version: 1.0.1
 Summary: Efficient Text Allocation in matplotlib using NumPy Broadcasting
 Author-email: Christoffer Kjellson <c.kjellson@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ckjellson/textalloc
 Project-URL: Bug Tracker, https://github.com/ckjellson/textalloc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -118,26 +118,21 @@
 textcolor: (Union[str, List[str]]), default "k"
     Color code of the text.
 seed: (int), default 0
     Seeds order of text allocations.
 direction: (str), default None
     Sets the preferred direction of the boxes with options:
     (south, north, east, west, northeast, northwest, southeast, southwest).
-x_logscale_base: (int), default None
-    Base of x-axis log-scale, required if the scaling of the x-axis is "log"
-y_logscale_base: (int), default None
-    Base of y-axis log-scale, required if the scaling of the y-axis is "log"
 avoid_label_lines_overlap: (bool), default False
     If set to True, avoids overlap for drawn lines to text labels.
-src_crs: (object), default None
-    Default crs of data, required when using transform in kwargs.
-    For example one can set src_crs=cartopy.crs.TransverseMercator() which is
-    default in matplotlib if using transform=cartopy.crs.PlateCarree().
-plot_kwargs (dict, optional): kwargs for the plt.plot of the lines if draw_lines is True.
-**kwargs: (), kwargs for the plt.text() call.
+plot_kwargs: (dict), default None
+    kwargs for the plt.plot of the lines if draw_lines is True.
+**kwargs: ()
+    kwargs for the plt.text() call.
+    If transform is used, it only needs to be provided here, i.e. not also in plot_kwargs.
 ```
 # Implementation and speed
 
 The implementation aims to plot as many text-boxes as possible in the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
 1. Generate a large number of candidate boxes near the original point with size that matches the fontsize.
@@ -208,7 +203,57 @@
                 textcolor="b")
 plt.show()
 ```
 
 plt.text|textalloc (0.7s)
 :-------------------------:|:-------------------------:
 ![](images/bar_before.png)|![](images/bar_after.png)
+
+# Plotting on images and using transforms
+
+textalloc now also supports plotting on images and using transforms. Below is an eample of using the PlateCarree transform to plot on top of a downloaded OSM-map (thank you @nebukadnezar for the example).
+
+```
+import numpy as np
+import matplotlib.pyplot as plt
+import cartopy.crs as ccrs
+import cartopy.io.img_tiles as cimgt
+import textalloc as ta
+
+np.random.seed(1)
+x = np.random.rand(100)
+x += 150.5
+y = np.random.rand(100)
+y -= 34.5
+
+dpi = 72
+fig = plt.figure(figsize=(800/dpi, 800/dpi), dpi=dpi)
+
+zoom = 10
+sitelon = np.mean(x)
+sitelat = np.mean(y)
+radius = (np.max(x) - np.min(x) ) / 1.5
+ll_lon = sitelon - radius * (1/np.cos(np.radians(sitelat)))
+ll_lat = sitelat - radius
+ur_lon = sitelon + radius * (1/np.cos(np.radians(sitelat)))
+ur_lat = sitelat + radius
+extent = [ll_lon, ur_lon, ll_lat, ur_lat]
+
+request = cimgt.OSM(desired_tile_form="L")
+ax = plt.axes(projection=request.crs)
+ax.set_extent(extent)
+ax.add_image(request, zoom, alpha=0.5, cmap='gray')
+ax.scatter(x, y, c='b', transform=ccrs.PlateCarree())
+
+text_list = [f'Text{i}' for i in range(len(x))]
+ta.allocate_text(fig,ax,x,y,
+                text_list,
+                x_scatter=x, y_scatter=y,
+                textsize=10,
+                draw_lines=True,
+                linewidth=0.5,
+                draw_all=False,
+                transform=ccrs.PlateCarree(),
+                avoid_label_lines_overlap=True)
+plt.show()
+```
+![](images/cartopy.png)
```

