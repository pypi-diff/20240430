# Comparing `tmp/condynsate-0.6.5.tar.gz` & `tmp/condynsate-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condynsate-0.6.5.tar", last modified: Wed Apr 17 17:08:03 2024, max compression
+gzip compressed data, was "condynsate-0.6.6.tar", last modified: Tue Apr 30 04:21:37 2024, max compression
```

## Comparing `condynsate-0.6.5.tar` & `condynsate-0.6.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 17:08:03.713805 condynsate-0.6.5/
--rw-rw-rw-   0        0        0     1092 2023-11-24 19:50:22.000000 condynsate-0.6.5/LICENSE
--rw-rw-rw-   0        0        0     4875 2024-04-17 17:08:03.711805 condynsate-0.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     2391 2024-03-21 21:05:21.000000 condynsate-0.6.5/README.md
--rw-rw-rw-   0        0        0     1439 2024-04-17 17:07:18.000000 condynsate-0.6.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 17:08:03.713805 condynsate-0.6.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 17:08:03.639212 condynsate-0.6.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 17:08:03.655216 condynsate-0.6.5/src/condynsate/
-drwxrwxrwx   0        0        0        0 2024-04-17 17:08:03.709805 condynsate-0.6.5/src/condynsate/__assets__/
--rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/arrow_ccw.stl
--rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/arrow_cw.stl
--rw-rw-rw-   0        0        0     6784 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/arrow_lin.stl
--rw-rw-rw-   0        0        0     6379 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/check.png
--rw-rw-rw-   0        0        0      684 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/cube.stl
--rw-rw-rw-   0        0        0    12684 2023-12-12 22:20:42.000000 condynsate-0.6.5/src/condynsate/__assets__/cylinder.stl
--rw-rw-rw-   0        0        0    12684 2023-12-12 22:33:34.000000 condynsate-0.6.5/src/condynsate/__assets__/cylinder_lower_origin.stl
--rw-rw-rw-   0        0        0    11484 2024-01-05 02:07:25.000000 condynsate-0.6.5/src/condynsate/__assets__/gate_med.stl
--rw-rw-rw-   0        0        0     4084 2024-01-05 02:03:45.000000 condynsate-0.6.5/src/condynsate/__assets__/gate_short.stl
--rw-rw-rw-   0        0        0    11484 2024-01-05 02:08:19.000000 condynsate-0.6.5/src/condynsate/__assets__/gate_tall.stl
--rw-rw-rw-   0        0        0      344 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/plane_big.obj
--rw-rw-rw-   0        0        0      332 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/plane_med.obj
--rw-rw-rw-   0        0        0      320 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/plane_small.obj
--rw-rw-rw-   0        0        0      384 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/pyramid.stl
--rw-rw-rw-   0        0        0    61284 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/sphere.stl
--rw-rw-rw-   0        0        0      153 2024-04-17 17:07:18.000000 condynsate-0.6.5/src/condynsate/__init__.py
--rw-rw-rw-   0        0        0    44652 2023-12-15 21:36:13.000000 condynsate-0.6.5/src/condynsate/animator.py
--rw-rw-rw-   0        0        0     8681 2024-04-17 16:50:25.000000 condynsate-0.6.5/src/condynsate/keyboard.py
--rw-rw-rw-   0        0        0   151710 2024-04-17 17:03:11.000000 condynsate-0.6.5/src/condynsate/simulator.py
--rw-rw-rw-   0        0        0    10805 2024-04-12 19:31:07.000000 condynsate-0.6.5/src/condynsate/utils.py
--rw-rw-rw-   0        0        0    22871 2024-04-15 16:06:31.000000 condynsate-0.6.5/src/condynsate/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-04-17 17:08:03.710805 condynsate-0.6.5/src/condynsate.egg-info/
--rw-rw-rw-   0        0        0     4875 2024-04-17 17:08:03.000000 condynsate-0.6.5/src/condynsate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      981 2024-04-17 17:08:03.000000 condynsate-0.6.5/src/condynsate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 17:08:03.000000 condynsate-0.6.5/src/condynsate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-17 17:08:03.000000 condynsate-0.6.5/src/condynsate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-17 17:08:03.000000 condynsate-0.6.5/src/condynsate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 04:21:37.578775 condynsate-0.6.6/
+-rw-rw-rw-   0        0        0     1092 2023-11-24 19:50:22.000000 condynsate-0.6.6/LICENSE
+-rw-rw-rw-   0        0        0     4875 2024-04-30 04:21:37.578775 condynsate-0.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2391 2024-03-21 21:05:21.000000 condynsate-0.6.6/README.md
+-rw-rw-rw-   0        0        0     1439 2024-04-30 04:20:27.000000 condynsate-0.6.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 04:21:37.578775 condynsate-0.6.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 04:21:37.512138 condynsate-0.6.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 04:21:37.516265 condynsate-0.6.6/src/condynsate/
+drwxrwxrwx   0        0        0        0 2024-04-30 04:21:37.578775 condynsate-0.6.6/src/condynsate/__assets__/
+-rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.6/src/condynsate/__assets__/arrow_ccw.stl
+-rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.6/src/condynsate/__assets__/arrow_cw.stl
+-rw-rw-rw-   0        0        0     6784 2023-11-24 19:50:22.000000 condynsate-0.6.6/src/condynsate/__assets__/arrow_lin.stl
+-rw-rw-rw-   0        0        0     6379 2023-11-24 19:50:22.000000 condynsate-0.6.6/src/condynsate/__assets__/check.png
+-rw-rw-rw-   0        0        0      684 2023-11-24 19:50:22.000000 condynsate-0.6.6/src/condynsate/__assets__/cube.stl
+-rw-rw-rw-   0        0        0    12684 2023-12-12 22:20:42.000000 condynsate-0.6.6/src/condynsate/__assets__/cylinder.stl
+-rw-rw-rw-   0        0        0    12684 2023-12-12 22:33:34.000000 condynsate-0.6.6/src/condynsate/__assets__/cylinder_lower_origin.stl
+-rw-rw-rw-   0        0        0    11484 2024-01-05 02:07:25.000000 condynsate-0.6.6/src/condynsate/__assets__/gate_med.stl
+-rw-rw-rw-   0        0        0     4084 2024-01-05 02:03:45.000000 condynsate-0.6.6/src/condynsate/__assets__/gate_short.stl
+-rw-rw-rw-   0        0        0    11484 2024-01-05 02:08:19.000000 condynsate-0.6.6/src/condynsate/__assets__/gate_tall.stl
+-rw-rw-rw-   0        0        0      344 2023-11-24 19:50:22.000000 condynsate-0.6.6/src/condynsate/__assets__/plane_big.obj
+-rw-rw-rw-   0        0        0      332 2023-11-24 19:50:22.000000 condynsate-0.6.6/src/condynsate/__assets__/plane_med.obj
+-rw-rw-rw-   0        0        0      320 2023-11-24 19:50:22.000000 condynsate-0.6.6/src/condynsate/__assets__/plane_small.obj
+-rw-rw-rw-   0        0        0      384 2023-11-24 19:50:22.000000 condynsate-0.6.6/src/condynsate/__assets__/pyramid.stl
+-rw-rw-rw-   0        0        0    61284 2023-11-24 19:50:22.000000 condynsate-0.6.6/src/condynsate/__assets__/sphere.stl
+-rw-rw-rw-   0        0        0      153 2024-04-30 04:20:27.000000 condynsate-0.6.6/src/condynsate/__init__.py
+-rw-rw-rw-   0        0        0    44652 2023-12-15 21:36:13.000000 condynsate-0.6.6/src/condynsate/animator.py
+-rw-rw-rw-   0        0        0     8681 2024-04-17 16:50:25.000000 condynsate-0.6.6/src/condynsate/keyboard.py
+-rw-rw-rw-   0        0        0   151848 2024-04-30 04:15:05.000000 condynsate-0.6.6/src/condynsate/simulator.py
+-rw-rw-rw-   0        0        0    10805 2024-04-20 00:47:25.000000 condynsate-0.6.6/src/condynsate/utils.py
+-rw-rw-rw-   0        0        0    22871 2024-04-19 23:25:43.000000 condynsate-0.6.6/src/condynsate/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-30 04:21:37.578775 condynsate-0.6.6/src/condynsate.egg-info/
+-rw-rw-rw-   0        0        0     4875 2024-04-30 04:21:37.000000 condynsate-0.6.6/src/condynsate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      981 2024-04-30 04:21:37.000000 condynsate-0.6.6/src/condynsate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 04:21:37.000000 condynsate-0.6.6/src/condynsate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-30 04:21:37.000000 condynsate-0.6.6/src/condynsate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-30 04:21:37.000000 condynsate-0.6.6/src/condynsate.egg-info/top_level.txt
```

### Comparing `condynsate-0.6.5/LICENSE` & `condynsate-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/PKG-INFO` & `condynsate-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: condynsate
-Version: 0.6.5
+Version: 0.6.6
 Summary: Simulates and visualizes articulated systems in real time
 Author-email: Grayson Schaer <gschaer2@illinois.edu>
 License: MIT License
         
         Copyright (c) 2023 Grayson Schaer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `condynsate-0.6.5/README.md` & `condynsate-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/pyproject.toml` & `condynsate-0.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "condynsate"
-version = "0.6.5"
+version = "0.6.6"
 description = "Simulates and visualizes articulated systems in real time"
 readme = "README.md"
 authors = [{ name = "Grayson Schaer", email = "gschaer2@illinois.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `condynsate-0.6.5/src/condynsate/__assets__/arrow_ccw.stl` & `condynsate-0.6.6/src/condynsate/__assets__/arrow_ccw.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/src/condynsate/__assets__/arrow_cw.stl` & `condynsate-0.6.6/src/condynsate/__assets__/arrow_cw.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/src/condynsate/__assets__/arrow_lin.stl` & `condynsate-0.6.6/src/condynsate/__assets__/arrow_lin.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/src/condynsate/__assets__/check.png` & `condynsate-0.6.6/src/condynsate/__assets__/check.png`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/src/condynsate/__assets__/cylinder.stl` & `condynsate-0.6.6/src/condynsate/__assets__/cylinder.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/src/condynsate/__assets__/cylinder_lower_origin.stl` & `condynsate-0.6.6/src/condynsate/__assets__/cylinder_lower_origin.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/src/condynsate/__assets__/gate_med.stl` & `condynsate-0.6.6/src/condynsate/__assets__/gate_med.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/src/condynsate/__assets__/gate_short.stl` & `condynsate-0.6.6/src/condynsate/__assets__/gate_short.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/src/condynsate/__assets__/gate_tall.stl` & `condynsate-0.6.6/src/condynsate/__assets__/gate_tall.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/src/condynsate/__assets__/sphere.stl` & `condynsate-0.6.6/src/condynsate/__assets__/sphere.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/src/condynsate/animator.py` & `condynsate-0.6.6/src/condynsate/animator.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/src/condynsate/keyboard.py` & `condynsate-0.6.6/src/condynsate/keyboard.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/src/condynsate/simulator.py` & `condynsate-0.6.6/src/condynsate/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,16 @@
         
         # A list of initial conditions of the URDF. URDF reset to this 
         # state when the simulator is reset
         self.initial_conds = {}
         
         # Lists that contain the visual geometrys and textures of the URDF
         # in order of link id. One per link
-        self.geometries = []
-        self.textures = []
+        self.geometries = {}
+        self.textures = {}
         
         # Structure that contains a bool to indicate if the stored
         # CoM is valid (True) or stale (needs to be recalculated) (False)
         # as well as the stored CoM
         self.center_of_mass = [False, np.array([0., 0., 0.])]
         
         # Structure that contains bools to indicate if the stored
@@ -2501,37 +2501,36 @@
                                              obj_path=paths[i],
                                              tex_path=tex_path,
                                              scale=scales[i],
                                              translate=poss[i],
                                              wxyz_quaternion=oris[i])
                 
                 # Save the texture and geometry
-                urdf_obj.geometries.append(geom)
-                urdf_obj.textures.append(tex)
+                urdf_obj.geometries[names[i]] = geom
+                urdf_obj.textures[names[i]] = tex
                 
             # If the current link is defined by an .stl file
             elif paths[i][-4:] == ".stl":
-                link_name = names[i]
                 rgb = format_RGB(colors[i][0:3],
                                   range_to_255=True)
                 opacity = colors[i][3]
                 transparent = opacity != 1.0
                 geom, tex = self.vis.add_stl(urdf_name=urdf_name,
-                                             link_name=link_name,
+                                             link_name=names[i],
                                              stl_path=paths[i],
                                              color=rgb,
                                              transparent=transparent,
                                              opacity=opacity,
                                              scale=scales[i],
                                              translate=poss[i],
                                              wxyz_quaternion=oris[i])
 
                 # Save the texture and geometry
-                urdf_obj.geometries.append(geom)
-                urdf_obj.textures.append(tex)
+                urdf_obj.geometries[names[i]] = geom
+                urdf_obj.textures[names[i]] = tex
 
     
     def _update_urdf_visual(self,
                             urdf_obj):
         """
         Updates the positions of dynamic links in the Visualizer.
 
@@ -2695,21 +2694,25 @@
         if not self.visualization:
             return    
         
         # If the link name doesn't exist, don't attempt to update it
         if not (link_name in urdf_obj.link_map):
             return
     
+        # If we don't already have the link geometry, we can't change its color
+        if not (link_name in urdf_obj.geometries):
+            return
+    
         # Get name and id data from urdf_obj
         urdf_id = urdf_obj.urdf_id
         urdf_name = str(urdf_id)
         link_id = urdf_obj.link_map[link_name]
         
         # Get the link's geometry
-        link_geometry = urdf_obj.geometries[link_id]
+        link_geometry = urdf_obj.geometries[link_name]
         
         # Ensure color is in proper format
         color = format_RGB(color, range_to_255=False)
         
         # Set the requested color
         self.vis.set_link_color(urdf_name = urdf_name,
                                 link_name = link_name,
```

### Comparing `condynsate-0.6.5/src/condynsate/utils.py` & `condynsate-0.6.6/src/condynsate/utils.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/src/condynsate/visualizer.py` & `condynsate-0.6.6/src/condynsate/visualizer.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.5/src/condynsate.egg-info/PKG-INFO` & `condynsate-0.6.6/src/condynsate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: condynsate
-Version: 0.6.5
+Version: 0.6.6
 Summary: Simulates and visualizes articulated systems in real time
 Author-email: Grayson Schaer <gschaer2@illinois.edu>
 License: MIT License
         
         Copyright (c) 2023 Grayson Schaer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `condynsate-0.6.5/src/condynsate.egg-info/SOURCES.txt` & `condynsate-0.6.6/src/condynsate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

