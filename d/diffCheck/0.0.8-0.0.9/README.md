# Comparing `tmp/diffCheck-0.0.8.tar.gz` & `tmp/diffCheck-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffCheck-0.0.8.tar", last modified: Mon Apr 15 09:10:11 2024, max compression
+gzip compressed data, was "diffCheck-0.0.9.tar", last modified: Mon Apr 15 11:46:32 2024, max compression
```

## Comparing `diffCheck-0.0.8.tar` & `diffCheck-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 09:10:11.764436 diffCheck-0.0.8/
--rw-rw-rw-   0        0        0      806 2024-04-15 09:10:11.763834 diffCheck-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      164 2024-04-12 08:02:49.000000 diffCheck-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 09:10:11.754010 diffCheck-0.0.8/diffCheck/
--rw-rw-rw-   0        0        0       21 2024-04-15 09:09:27.000000 diffCheck-0.0.8/diffCheck/__init__.py
--rw-rw-rw-   0        0        0     9419 2024-04-15 09:09:03.000000 diffCheck-0.0.8/diffCheck/df_geometries.py
--rw-rw-rw-   0        0        0     7965 2024-04-15 09:09:08.000000 diffCheck-0.0.8/diffCheck/df_joint_detector.py
--rw-rw-rw-   0        0        0     4700 2024-04-12 15:50:57.000000 diffCheck-0.0.8/diffCheck/df_transformations.py
--rw-rw-rw-   0        0        0     4174 2024-04-12 15:49:55.000000 diffCheck-0.0.8/diffCheck/df_util.py
--rw-rw-rw-   0        0        0      997 2024-04-15 09:07:29.000000 diffCheck-0.0.8/diffCheck/diffCheck_app.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:10:11.762274 diffCheck-0.0.8/diffCheck.egg-info/
--rw-rw-rw-   0        0        0      806 2024-04-15 09:10:11.000000 diffCheck-0.0.8/diffCheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-15 09:10:11.000000 diffCheck-0.0.8/diffCheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 09:10:11.000000 diffCheck-0.0.8/diffCheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-15 09:10:11.000000 diffCheck-0.0.8/diffCheck.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-15 09:10:11.000000 diffCheck-0.0.8/diffCheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 09:10:11.764971 diffCheck-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      824 2024-04-15 09:09:27.000000 diffCheck-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:46:32.838950 diffCheck-0.0.9/
+-rw-rw-rw-   0        0        0      806 2024-04-15 11:46:32.838950 diffCheck-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2024-04-12 08:02:49.000000 diffCheck-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 11:46:32.826760 diffCheck-0.0.9/diffCheck/
+-rw-rw-rw-   0        0        0       21 2024-04-15 11:46:16.000000 diffCheck-0.0.9/diffCheck/__init__.py
+-rw-rw-rw-   0        0        0     9419 2024-04-15 11:32:00.000000 diffCheck-0.0.9/diffCheck/df_geometries.py
+-rw-rw-rw-   0        0        0     7965 2024-04-15 09:38:27.000000 diffCheck-0.0.9/diffCheck/df_joint_detector.py
+-rw-rw-rw-   0        0        0     4634 2024-04-15 11:45:20.000000 diffCheck-0.0.9/diffCheck/df_transformations.py
+-rw-rw-rw-   0        0        0     4174 2024-04-12 15:49:55.000000 diffCheck-0.0.9/diffCheck/df_util.py
+-rw-rw-rw-   0        0        0     1059 2024-04-15 11:33:07.000000 diffCheck-0.0.9/diffCheck/diffCheck_app.py
+-rw-rw-rw-   0        0        0       69 2024-04-15 11:33:58.000000 diffCheck-0.0.9/diffCheck/newmodule.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:46:32.836760 diffCheck-0.0.9/diffCheck.egg-info/
+-rw-rw-rw-   0        0        0      806 2024-04-15 11:46:32.000000 diffCheck-0.0.9/diffCheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2024-04-15 11:46:32.000000 diffCheck-0.0.9/diffCheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 11:46:32.000000 diffCheck-0.0.9/diffCheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-15 11:46:32.000000 diffCheck-0.0.9/diffCheck.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-15 11:46:32.000000 diffCheck-0.0.9/diffCheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 11:46:32.838950 diffCheck-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      824 2024-04-15 11:46:20.000000 diffCheck-0.0.9/setup.py
```

### Comparing `diffCheck-0.0.8/PKG-INFO` & `diffCheck-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffCheck
-Version: 0.0.8
+Version: 0.0.9
 Summary: DiffCheck is a package to check the differences between two timber structures
 Home-page: https://github.com/diffCheckOrg/diffCheck
 Author: Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand
 Author-email: andrea.settimi@epfl.ch
 License: UNKNOWN
 Description: # DiffCheck Grasshopper Plugin
```

### Comparing `diffCheck-0.0.8/diffCheck/df_geometries.py` & `diffCheck-0.0.9/diffCheck/df_geometries.py`

 * *Files identical despite different names*

### Comparing `diffCheck-0.0.8/diffCheck/df_joint_detector.py` & `diffCheck-0.0.9/diffCheck/df_joint_detector.py`

 * *Files identical despite different names*

### Comparing `diffCheck-0.0.8/diffCheck/df_transformations.py` & `diffCheck-0.0.9/diffCheck/df_transformations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import Rhino
 import Rhino.Geometry as rg
 import scriptcontext as sc
 
 import numpy as np
+import math
 
 
 def get_inverse_transformation(
     x_form: Rhino.Geometry.Transform,
 ) -> Rhino.Geometry.Transform:
     """
         Get the inverse of a transformation
@@ -81,15 +82,14 @@
 
     # get the plane of the biggest face
     if biggest_face.TryGetPlane()[0] is False:
         log.error("Could not find plane for longest edge. Exiting...")
         return
     plane_src = biggest_face.TryGetPlane()[1]
     plane_tgt = Rhino.Geometry.Plane.WorldXY
-    print("Found plane for longest edge: " + str(plane_src))
 
     # plane to plane transformation
     x_form_pln2pln = Rhino.Geometry.Transform.PlaneToPlane(plane_src, plane_tgt)
     brep.Transform(x_form_pln2pln)
 
     # adjust to x,y,z positive
     lowest_vertex = _get_lowest_brep_vertex(brep)
@@ -105,17 +105,18 @@
         y_val_sum += corner.Y
         x_val_sum += corner.X
 
     # check if a 90 deg rotation is needed (for the joint detector)
     x_form_transl_B = None
     x_form_rot90z = None
     if x_val_sum > y_val_sum:
-        print("Bounding box is alligned to x axis. No rotation needed.")
+        # AABB is alligned to x axis. No rotation needed
+        pass
     else:
-        print("Bounding box is not alligned to y axis. A 90 deg rotation is needed.")
+        # AABB is not alligned to y axis. A 90 deg rotation is needed.
         x_form_rot90z = Rhino.Geometry.Transform.Rotation(
             math.radians(90), rg.Vector3d.ZAxis, rg.Point3d.Origin
         )
         brep.Transform(x_form_rot90z)
         lowest_vertex = _get_lowest_brep_vertex(brep)
 
         x_form_transl_B = Rhino.Geometry.Transform.Translation(
```

### Comparing `diffCheck-0.0.8/diffCheck/df_util.py` & `diffCheck-0.0.9/diffCheck/df_util.py`

 * *Files identical despite different names*

### Comparing `diffCheck-0.0.8/diffCheck.egg-info/PKG-INFO` & `diffCheck-0.0.9/diffCheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffCheck
-Version: 0.0.8
+Version: 0.0.9
 Summary: DiffCheck is a package to check the differences between two timber structures
 Home-page: https://github.com/diffCheckOrg/diffCheck
 Author: Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand
 Author-email: andrea.settimi@epfl.ch
 License: UNKNOWN
 Description: # DiffCheck Grasshopper Plugin
```

### Comparing `diffCheck-0.0.8/setup.py` & `diffCheck-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="diffCheck",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(),
     install_requires=[
         "numpy",
         # other dependencies...
     ],
     description="DiffCheck is a package to check the differences between two timber structures",
     long_description=open("README.md").read(),
```

