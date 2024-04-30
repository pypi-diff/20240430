# Comparing `tmp/figurify-0.0.9.tar.gz` & `tmp/figurify-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figurify-0.0.9.tar", last modified: Tue Apr 30 13:10:57 2024, max compression
+gzip compressed data, was "figurify-0.1.0.tar", last modified: Tue Apr 30 13:37:54 2024, max compression
```

## Comparing `figurify-0.0.9.tar` & `figurify-0.1.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-30 13:10:57.943938 figurify-0.0.9/
--rw-r--r--   0 julian    (1000) julian    (1000)     1068 2024-04-28 15:07:49.000000 figurify-0.0.9/LICENSE
--rw-r--r--   0 julian    (1000) julian    (1000)       60 2024-04-29 12:55:00.000000 figurify-0.0.9/MANIFEST.in
--rw-r--r--   0 julian    (1000) julian    (1000)    11470 2024-04-30 13:10:57.943938 figurify-0.0.9/PKG-INFO
--rw-r--r--   0 julian    (1000) julian    (1000)     1945 2024-04-29 16:03:47.000000 figurify-0.0.9/README.md
--rw-r--r--   0 julian    (1000) julian    (1000)        5 2024-04-30 13:08:22.000000 figurify-0.0.9/VERSION.txt
--rw-r--r--   0 julian    (1000) julian    (1000)    11005 2024-04-29 16:31:38.000000 figurify-0.0.9/documentation.md
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-30 13:10:57.933938 figurify-0.0.9/figurify/
--rw-r--r--   0 julian    (1000) julian    (1000)      177 2024-04-30 13:07:42.000000 figurify-0.0.9/figurify/__init__.py
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-30 13:10:57.937272 figurify-0.0.9/figurify/figure_physics/
--rw-r--r--   0 julian    (1000) julian    (1000)      546 2024-04-30 12:59:44.000000 figurify-0.0.9/figurify/figure_physics/__init__.py
--rw-r--r--   0 julian    (1000) julian    (1000)      732 2024-04-29 13:55:51.000000 figurify-0.0.9/figurify/figure_physics/dynamics.py
--rw-r--r--   0 julian    (1000) julian    (1000)      672 2024-04-29 13:57:52.000000 figurify-0.0.9/figurify/figure_physics/energy.py
--rw-r--r--   0 julian    (1000) julian    (1000)      669 2024-04-29 14:02:07.000000 figurify-0.0.9/figurify/figure_physics/forces.py
--rw-r--r--   0 julian    (1000) julian    (1000)      571 2024-04-29 14:05:26.000000 figurify-0.0.9/figurify/figure_physics/gravity.py
--rw-r--r--   0 julian    (1000) julian    (1000)      637 2024-04-29 14:08:46.000000 figurify-0.0.9/figurify/figure_physics/kinematics.py
--rw-r--r--   0 julian    (1000) julian    (1000)      410 2024-04-29 14:10:30.000000 figurify-0.0.9/figurify/figure_physics/momentum.py
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-30 13:10:57.940605 figurify-0.0.9/figurify/geometric_solids/
--rw-r--r--   0 julian    (1000) julian    (1000)      730 2024-04-30 13:06:08.000000 figurify-0.0.9/figurify/geometric_solids/__init__.py
--rw-r--r--   0 julian    (1000) julian    (1000)      767 2024-04-29 13:12:25.000000 figurify-0.0.9/figurify/geometric_solids/cone.py
--rw-r--r--   0 julian    (1000) julian    (1000)      692 2024-04-29 13:15:21.000000 figurify-0.0.9/figurify/geometric_solids/cube.py
--rw-r--r--   0 julian    (1000) julian    (1000)      974 2024-04-29 13:16:41.000000 figurify-0.0.9/figurify/geometric_solids/cuboid.py
--rw-r--r--   0 julian    (1000) julian    (1000)      798 2024-04-29 13:19:50.000000 figurify-0.0.9/figurify/geometric_solids/cylinder.py
--rw-r--r--   0 julian    (1000) julian    (1000)      975 2024-04-29 13:25:48.000000 figurify-0.0.9/figurify/geometric_solids/prism.py
--rw-r--r--   0 julian    (1000) julian    (1000)     1425 2024-04-29 13:28:22.000000 figurify-0.0.9/figurify/geometric_solids/pyramid.py
--rw-r--r--   0 julian    (1000) julian    (1000)      845 2024-04-29 13:32:52.000000 figurify-0.0.9/figurify/geometric_solids/sphere.py
--rw-r--r--   0 julian    (1000) julian    (1000)      943 2024-04-29 13:36:11.000000 figurify-0.0.9/figurify/geometric_solids/torus.py
--rw-r--r--   0 julian    (1000) julian    (1000)      824 2024-04-28 06:24:04.000000 figurify-0.0.9/figurify/material_properties.py
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-30 13:10:57.940605 figurify-0.0.9/figurify/plane_metrics/
--rw-r--r--   0 julian    (1000) julian    (1000)      736 2024-04-30 13:02:31.000000 figurify-0.0.9/figurify/plane_metrics/__init__.py
--rw-r--r--   0 julian    (1000) julian    (1000)      784 2024-04-27 08:24:04.000000 figurify-0.0.9/figurify/plane_metrics/circle.py
--rw-r--r--   0 julian    (1000) julian    (1000)     1394 2024-04-27 08:18:08.000000 figurify-0.0.9/figurify/plane_metrics/ellipse.py
--rw-r--r--   0 julian    (1000) julian    (1000)     1104 2024-04-27 08:01:55.000000 figurify-0.0.9/figurify/plane_metrics/parallelogram.py
--rw-r--r--   0 julian    (1000) julian    (1000)      415 2024-04-27 08:28:31.000000 figurify-0.0.9/figurify/plane_metrics/polygon.py
--rw-r--r--   0 julian    (1000) julian    (1000)      890 2024-04-29 13:44:00.000000 figurify-0.0.9/figurify/plane_metrics/quadrilateral.py
--rw-r--r--   0 julian    (1000) julian    (1000)      597 2024-04-29 13:46:59.000000 figurify-0.0.9/figurify/plane_metrics/rectangle.py
--rw-r--r--   0 julian    (1000) julian    (1000)     1465 2024-04-27 08:26:22.000000 figurify-0.0.9/figurify/plane_metrics/trapezoid.py
--rw-r--r--   0 julian    (1000) julian    (1000)      889 2024-04-29 13:48:54.000000 figurify-0.0.9/figurify/plane_metrics/triangle.py
--rw-r--r--   0 julian    (1000) julian    (1000)     2114 2024-04-28 06:52:47.000000 figurify-0.0.9/figurify/units.py
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-30 13:10:57.933938 figurify-0.0.9/figurify.egg-info/
--rw-r--r--   0 julian    (1000) julian    (1000)    11470 2024-04-30 13:10:57.000000 figurify-0.0.9/figurify.egg-info/PKG-INFO
--rw-r--r--   0 julian    (1000) julian    (1000)     1161 2024-04-30 13:10:57.000000 figurify-0.0.9/figurify.egg-info/SOURCES.txt
--rw-r--r--   0 julian    (1000) julian    (1000)        1 2024-04-30 13:10:57.000000 figurify-0.0.9/figurify.egg-info/dependency_links.txt
--rw-r--r--   0 julian    (1000) julian    (1000)        9 2024-04-30 13:10:57.000000 figurify-0.0.9/figurify.egg-info/top_level.txt
--rw-r--r--   0 julian    (1000) julian    (1000)       38 2024-04-30 13:10:57.943938 figurify-0.0.9/setup.cfg
--rw-r--r--   0 julian    (1000) julian    (1000)      762 2024-04-29 17:52:07.000000 figurify-0.0.9/setup.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-30 13:37:54.707309 figurify-0.1.0/
+-rw-r--r--   0 julian    (1000) julian    (1000)     1068 2024-04-28 15:07:49.000000 figurify-0.1.0/LICENSE
+-rw-r--r--   0 julian    (1000) julian    (1000)       60 2024-04-29 12:55:00.000000 figurify-0.1.0/MANIFEST.in
+-rw-r--r--   0 julian    (1000) julian    (1000)    11442 2024-04-30 13:37:54.707309 figurify-0.1.0/PKG-INFO
+-rw-r--r--   0 julian    (1000) julian    (1000)     1953 2024-04-30 13:35:24.000000 figurify-0.1.0/README.md
+-rw-r--r--   0 julian    (1000) julian    (1000)        5 2024-04-30 13:37:41.000000 figurify-0.1.0/VERSION.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)    10977 2024-04-30 13:35:24.000000 figurify-0.1.0/documentation.md
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-30 13:37:54.700642 figurify-0.1.0/figurify/
+-rw-r--r--   0 julian    (1000) julian    (1000)      177 2024-04-30 13:20:06.000000 figurify-0.1.0/figurify/__init__.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-30 13:37:54.703976 figurify-0.1.0/figurify/figure_physics/
+-rw-r--r--   0 julian    (1000) julian    (1000)      546 2024-04-30 13:20:06.000000 figurify-0.1.0/figurify/figure_physics/__init__.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      732 2024-04-29 13:55:51.000000 figurify-0.1.0/figurify/figure_physics/dynamics.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      672 2024-04-29 13:57:52.000000 figurify-0.1.0/figurify/figure_physics/energy.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      669 2024-04-29 14:02:07.000000 figurify-0.1.0/figurify/figure_physics/forces.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      571 2024-04-29 14:05:26.000000 figurify-0.1.0/figurify/figure_physics/gravity.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      637 2024-04-29 14:08:46.000000 figurify-0.1.0/figurify/figure_physics/kinematics.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      410 2024-04-29 14:10:30.000000 figurify-0.1.0/figurify/figure_physics/momentum.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-30 13:37:54.703976 figurify-0.1.0/figurify/geometric_solids/
+-rw-r--r--   0 julian    (1000) julian    (1000)      730 2024-04-30 13:20:06.000000 figurify-0.1.0/figurify/geometric_solids/__init__.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      767 2024-04-29 13:12:25.000000 figurify-0.1.0/figurify/geometric_solids/cone.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      692 2024-04-29 13:15:21.000000 figurify-0.1.0/figurify/geometric_solids/cube.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      974 2024-04-29 13:16:41.000000 figurify-0.1.0/figurify/geometric_solids/cuboid.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      798 2024-04-29 13:19:50.000000 figurify-0.1.0/figurify/geometric_solids/cylinder.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      975 2024-04-29 13:25:48.000000 figurify-0.1.0/figurify/geometric_solids/prism.py
+-rw-r--r--   0 julian    (1000) julian    (1000)     1425 2024-04-29 13:28:22.000000 figurify-0.1.0/figurify/geometric_solids/pyramid.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      845 2024-04-29 13:32:52.000000 figurify-0.1.0/figurify/geometric_solids/sphere.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      943 2024-04-29 13:36:11.000000 figurify-0.1.0/figurify/geometric_solids/torus.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      824 2024-04-28 06:24:04.000000 figurify-0.1.0/figurify/material_properties.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-30 13:37:54.707309 figurify-0.1.0/figurify/plane_metrics/
+-rw-r--r--   0 julian    (1000) julian    (1000)      736 2024-04-30 13:20:06.000000 figurify-0.1.0/figurify/plane_metrics/__init__.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      784 2024-04-27 08:24:04.000000 figurify-0.1.0/figurify/plane_metrics/circle.py
+-rw-r--r--   0 julian    (1000) julian    (1000)     1394 2024-04-27 08:18:08.000000 figurify-0.1.0/figurify/plane_metrics/ellipse.py
+-rw-r--r--   0 julian    (1000) julian    (1000)     1104 2024-04-27 08:01:55.000000 figurify-0.1.0/figurify/plane_metrics/parallelogram.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      415 2024-04-27 08:28:31.000000 figurify-0.1.0/figurify/plane_metrics/polygon.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      890 2024-04-29 13:44:00.000000 figurify-0.1.0/figurify/plane_metrics/quadrilateral.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      597 2024-04-29 13:46:59.000000 figurify-0.1.0/figurify/plane_metrics/rectangle.py
+-rw-r--r--   0 julian    (1000) julian    (1000)     1465 2024-04-27 08:26:22.000000 figurify-0.1.0/figurify/plane_metrics/trapezoid.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      889 2024-04-29 13:48:54.000000 figurify-0.1.0/figurify/plane_metrics/triangle.py
+-rw-r--r--   0 julian    (1000) julian    (1000)     2114 2024-04-28 06:52:47.000000 figurify-0.1.0/figurify/units.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-30 13:37:54.700642 figurify-0.1.0/figurify.egg-info/
+-rw-r--r--   0 julian    (1000) julian    (1000)    11442 2024-04-30 13:37:54.000000 figurify-0.1.0/figurify.egg-info/PKG-INFO
+-rw-r--r--   0 julian    (1000) julian    (1000)     1161 2024-04-30 13:37:54.000000 figurify-0.1.0/figurify.egg-info/SOURCES.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)        1 2024-04-30 13:37:54.000000 figurify-0.1.0/figurify.egg-info/dependency_links.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)        9 2024-04-30 13:37:54.000000 figurify-0.1.0/figurify.egg-info/top_level.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)       38 2024-04-30 13:37:54.707309 figurify-0.1.0/setup.cfg
+-rw-r--r--   0 julian    (1000) julian    (1000)      762 2024-04-29 17:52:07.000000 figurify-0.1.0/setup.py
```

### Comparing `figurify-0.0.9/LICENSE` & `figurify-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/PKG-INFO` & `figurify-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: figurify
-Version: 0.0.9
+Version: 0.1.0
 Summary: With figurify you can calculate figures, surfaces and physics.
 Author: Julian Hess
 Project-URL: Source, https://github.com/julian-hess/Figurify.git
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Figurify
-
 # Short explanation
 
-## Explanation
-
 Figurify is a Python library that allows you to perform various calculations related to geometric figures. With Figurify, you can quickly and easily calculate properties such as perimeter, area, angles, and more for various geometric shapes.
 
 ## Installation
 
 You can easily install Figurify using pip:
 
     pip install figurify
```

### Comparing `figurify-0.0.9/README.md` & `figurify-0.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## Explanation
 
-Figurify is a Python library that allows you to perform various calculations related to geometric figures. With Figurify, you can quickly and easily calculate properties such as perimeter, area, angles, and more for various geometric shapes.
+**Figurify** is a **Python library** that allows you to perform various calculations related to geometric figures. With Figurify, you can quickly and easily calculate properties such as perimeter, area, angles, and more for various geometric shapes.
 
 ## Installation
 
 You can easily install Figurify using pip:
 
     pip install figurify
```

### Comparing `figurify-0.0.9/documentation.md` & `figurify-0.1.0/documentation.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-# Figurify
-
 # Short explanation
 
-## Explanation
-
 Figurify is a Python library that allows you to perform various calculations related to geometric figures. With Figurify, you can quickly and easily calculate properties such as perimeter, area, angles, and more for various geometric shapes.
 
 ## Installation
 
 You can easily install Figurify using pip:
 
     pip install figurify
```

### Comparing `figurify-0.0.9/figurify/figure_physics/__init__.py` & `figurify-0.1.0/figurify/figure_physics/__init__.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/figure_physics/dynamics.py` & `figurify-0.1.0/figurify/figure_physics/dynamics.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/figure_physics/energy.py` & `figurify-0.1.0/figurify/figure_physics/energy.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/figure_physics/forces.py` & `figurify-0.1.0/figurify/figure_physics/forces.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/figure_physics/gravity.py` & `figurify-0.1.0/figurify/figure_physics/gravity.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/figure_physics/kinematics.py` & `figurify-0.1.0/figurify/figure_physics/kinematics.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/geometric_solids/__init__.py` & `figurify-0.1.0/figurify/geometric_solids/__init__.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/geometric_solids/cone.py` & `figurify-0.1.0/figurify/geometric_solids/cone.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/geometric_solids/cube.py` & `figurify-0.1.0/figurify/geometric_solids/cube.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/geometric_solids/cuboid.py` & `figurify-0.1.0/figurify/geometric_solids/cuboid.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/geometric_solids/cylinder.py` & `figurify-0.1.0/figurify/geometric_solids/cylinder.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/geometric_solids/prism.py` & `figurify-0.1.0/figurify/geometric_solids/prism.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/geometric_solids/pyramid.py` & `figurify-0.1.0/figurify/geometric_solids/pyramid.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/geometric_solids/sphere.py` & `figurify-0.1.0/figurify/geometric_solids/sphere.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/geometric_solids/torus.py` & `figurify-0.1.0/figurify/geometric_solids/torus.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/material_properties.py` & `figurify-0.1.0/figurify/material_properties.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/plane_metrics/__init__.py` & `figurify-0.1.0/figurify/plane_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/plane_metrics/circle.py` & `figurify-0.1.0/figurify/plane_metrics/circle.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/plane_metrics/ellipse.py` & `figurify-0.1.0/figurify/plane_metrics/ellipse.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/plane_metrics/parallelogram.py` & `figurify-0.1.0/figurify/plane_metrics/parallelogram.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/plane_metrics/quadrilateral.py` & `figurify-0.1.0/figurify/plane_metrics/quadrilateral.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/plane_metrics/rectangle.py` & `figurify-0.1.0/figurify/plane_metrics/rectangle.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/plane_metrics/trapezoid.py` & `figurify-0.1.0/figurify/plane_metrics/trapezoid.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/plane_metrics/triangle.py` & `figurify-0.1.0/figurify/plane_metrics/triangle.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify/units.py` & `figurify-0.1.0/figurify/units.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/figurify.egg-info/PKG-INFO` & `figurify-0.1.0/figurify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: figurify
-Version: 0.0.9
+Version: 0.1.0
 Summary: With figurify you can calculate figures, surfaces and physics.
 Author: Julian Hess
 Project-URL: Source, https://github.com/julian-hess/Figurify.git
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Figurify
-
 # Short explanation
 
-## Explanation
-
 Figurify is a Python library that allows you to perform various calculations related to geometric figures. With Figurify, you can quickly and easily calculate properties such as perimeter, area, angles, and more for various geometric shapes.
 
 ## Installation
 
 You can easily install Figurify using pip:
 
     pip install figurify
```

### Comparing `figurify-0.0.9/figurify.egg-info/SOURCES.txt` & `figurify-0.1.0/figurify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `figurify-0.0.9/setup.py` & `figurify-0.1.0/setup.py`

 * *Files identical despite different names*

