# Comparing `tmp/clump-python-0.2.7.tar.gz` & `tmp/clump-python-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clump-python-0.2.7.tar", last modified: Fri Apr 26 09:24:34 2024, max compression
+gzip compressed data, was "clump-python-0.2.8.tar", last modified: Tue Apr 30 14:33:40 2024, max compression
```

## Comparing `clump-python-0.2.7.tar` & `clump-python-0.2.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 09:24:34.818075 clump-python-0.2.7/
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 09:24:34.810075 clump-python-0.2.7/CLUMP/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8025 2024-04-26 09:21:09.000000 clump-python-0.2.7/CLUMP/ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-26 05:50:24.000000 clump-python-0.2.7/CLUMP/GenerateClump_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-26 09:22:56.000000 clump-python-0.2.7/CLUMP/GenerateClump_Favier.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-26 09:22:56.000000 clump-python-0.2.7/CLUMP/GenerateClump_Ferellec_McDowell.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.2.7/CLUMP/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 09:24:34.810075 clump-python-0.2.7/CLUMP/examples/
--rw-rw-r--   0 utku      (1000) utku      (1000)      812 2024-04-26 05:50:01.000000 clump-python-0.2.7/CLUMP/examples/Example_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      937 2024-04-26 05:49:49.000000 clump-python-0.2.7/CLUMP/examples/Example_Euclidean_3D_Extended.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      675 2024-04-26 05:50:04.000000 clump-python-0.2.7/CLUMP/examples/Example_ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      713 2024-04-26 05:50:07.000000 clump-python-0.2.7/CLUMP/examples/Example_Favier_automatic_generation.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      743 2024-04-26 05:50:11.000000 clump-python-0.2.7/CLUMP/examples/Example_Ferellec_McDowell.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 09:24:34.818075 clump-python-0.2.7/CLUMP/examples/ParticleGeometries/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8351 2024-04-17 12:23:12.000000 clump-python-0.2.7/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat
--rw-rw-r--   0 utku      (1000) utku      (1000)     4280 2024-04-17 12:23:12.000000 clump-python-0.2.7/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat
--rw-rw-r--   0 utku      (1000) utku      (1000)  1024084 2022-11-01 09:30:38.000000 clump-python-0.2.7/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)   153684 2024-04-17 12:23:12.000000 clump-python-0.2.7/CLUMP/examples/ParticleGeometries/Hexahedron.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)  2670559 2024-04-17 12:23:12.000000 clump-python-0.2.7/CLUMP/examples/ParticleGeometries/Human_femur.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)   102484 2024-04-17 12:23:12.000000 clump-python-0.2.7/CLUMP/examples/ParticleGeometries/Octahedron.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)  2880084 2024-04-23 14:41:30.000000 clump-python-0.2.7/CLUMP/examples/ParticleGeometries/Torus.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.7/CLUMP/examples/ParticleGeometries/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.7/CLUMP/examples/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 09:24:34.818075 clump-python-0.2.7/CLUMP/utils/
--rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-26 05:50:40.000000 clump-python-0.2.7/CLUMP/utils/MyRobustCrust.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     2670 2024-04-26 05:57:34.000000 clump-python-0.2.7/CLUMP/utils/ParticlePlotter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     2287 2024-04-26 05:54:26.000000 clump-python-0.2.7/CLUMP/utils/PatchNormals.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.2.7/CLUMP/utils/RigidBodyParameters.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     2293 2024-04-26 05:56:57.000000 clump-python-0.2.7/CLUMP/utils/STL_ReaderWriter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1330 2024-04-26 05:51:27.000000 clump-python-0.2.7/CLUMP/utils/VTK_Writer.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.2.7/CLUMP/utils/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.2.7/LICENSE
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-26 09:24:34.818075 clump-python-0.2.7/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     7680 2024-04-24 15:24:47.000000 clump-python-0.2.7/README.md
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 09:24:34.818075 clump-python-0.2.7/clump_python.egg-info/
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-26 09:24:34.000000 clump-python-0.2.7/clump_python.egg-info/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     1230 2024-04-26 09:24:34.000000 clump-python-0.2.7/clump_python.egg-info/SOURCES.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-26 09:24:34.000000 clump-python-0.2.7/clump_python.egg-info/dependency_links.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-26 09:24:34.000000 clump-python-0.2.7/clump_python.egg-info/requires.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-26 09:24:34.000000 clump-python-0.2.7/clump_python.egg-info/top_level.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-26 09:24:34.818075 clump-python-0.2.7/setup.cfg
--rw-rw-r--   0 utku      (1000) utku      (1000)      970 2024-04-26 09:23:24.000000 clump-python-0.2.7/setup.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-30 14:33:40.230849 clump-python-0.2.8/
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-30 14:33:40.218849 clump-python-0.2.8/CLUMP/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8025 2024-04-26 09:21:09.000000 clump-python-0.2.8/CLUMP/ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-26 05:50:24.000000 clump-python-0.2.8/CLUMP/GenerateClump_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-26 09:22:56.000000 clump-python-0.2.8/CLUMP/GenerateClump_Favier.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-26 09:22:56.000000 clump-python-0.2.8/CLUMP/GenerateClump_Ferellec_McDowell.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.2.8/CLUMP/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-30 14:33:40.218849 clump-python-0.2.8/CLUMP/examples/
+-rw-rw-r--   0 utku      (1000) utku      (1000)      812 2024-04-26 05:50:01.000000 clump-python-0.2.8/CLUMP/examples/Example_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      937 2024-04-26 05:49:49.000000 clump-python-0.2.8/CLUMP/examples/Example_Euclidean_3D_Extended.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      675 2024-04-26 05:50:04.000000 clump-python-0.2.8/CLUMP/examples/Example_ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      713 2024-04-26 05:50:07.000000 clump-python-0.2.8/CLUMP/examples/Example_Favier_automatic_generation.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      743 2024-04-26 05:50:11.000000 clump-python-0.2.8/CLUMP/examples/Example_Ferellec_McDowell.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-30 14:33:40.226849 clump-python-0.2.8/CLUMP/examples/ParticleGeometries/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8351 2024-04-17 12:23:12.000000 clump-python-0.2.8/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat
+-rw-rw-r--   0 utku      (1000) utku      (1000)     4280 2024-04-17 12:23:12.000000 clump-python-0.2.8/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat
+-rw-rw-r--   0 utku      (1000) utku      (1000)  1024084 2022-11-01 09:30:38.000000 clump-python-0.2.8/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)   153684 2024-04-17 12:23:12.000000 clump-python-0.2.8/CLUMP/examples/ParticleGeometries/Hexahedron.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)  2670559 2024-04-17 12:23:12.000000 clump-python-0.2.8/CLUMP/examples/ParticleGeometries/Human_femur.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)   102484 2024-04-17 12:23:12.000000 clump-python-0.2.8/CLUMP/examples/ParticleGeometries/Octahedron.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)  2880084 2024-04-23 14:41:30.000000 clump-python-0.2.8/CLUMP/examples/ParticleGeometries/Torus.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.8/CLUMP/examples/ParticleGeometries/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.8/CLUMP/examples/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-30 14:33:40.226849 clump-python-0.2.8/CLUMP/utils/
+-rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-26 05:50:40.000000 clump-python-0.2.8/CLUMP/utils/MyRobustCrust.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2670 2024-04-26 05:57:34.000000 clump-python-0.2.8/CLUMP/utils/ParticlePlotter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2287 2024-04-26 05:54:26.000000 clump-python-0.2.8/CLUMP/utils/PatchNormals.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.2.8/CLUMP/utils/RigidBodyParameters.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2293 2024-04-26 05:56:57.000000 clump-python-0.2.8/CLUMP/utils/STL_ReaderWriter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1330 2024-04-26 05:51:27.000000 clump-python-0.2.8/CLUMP/utils/VTK_Writer.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.2.8/CLUMP/utils/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.2.8/LICENSE
+-rw-r--r--   0 utku      (1000) utku      (1000)     6289 2024-04-30 14:33:40.230849 clump-python-0.2.8/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     5525 2024-04-30 12:04:41.000000 clump-python-0.2.8/README.md
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-30 14:33:40.230849 clump-python-0.2.8/clump_python.egg-info/
+-rw-r--r--   0 utku      (1000) utku      (1000)     6289 2024-04-30 14:33:40.000000 clump-python-0.2.8/clump_python.egg-info/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1230 2024-04-30 14:33:40.000000 clump-python-0.2.8/clump_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-30 14:33:40.000000 clump-python-0.2.8/clump_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-30 14:33:40.000000 clump-python-0.2.8/clump_python.egg-info/requires.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-30 14:33:40.000000 clump-python-0.2.8/clump_python.egg-info/top_level.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-30 14:33:40.230849 clump-python-0.2.8/setup.cfg
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1209 2024-04-30 14:20:24.000000 clump-python-0.2.8/setup.py
```

### Comparing `clump-python-0.2.7/CLUMP/ExtractSurface.py` & `clump-python-0.2.8/CLUMP/ExtractSurface.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/GenerateClump_Euclidean_3D.py` & `clump-python-0.2.8/CLUMP/GenerateClump_Euclidean_3D.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/GenerateClump_Favier.py` & `clump-python-0.2.8/CLUMP/GenerateClump_Favier.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/GenerateClump_Ferellec_McDowell.py` & `clump-python-0.2.8/CLUMP/GenerateClump_Ferellec_McDowell.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/examples/Example_Euclidean_3D.py` & `clump-python-0.2.8/CLUMP/examples/Example_Euclidean_3D.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/examples/Example_Euclidean_3D_Extended.py` & `clump-python-0.2.8/CLUMP/examples/Example_Euclidean_3D_Extended.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/examples/Example_ExtractSurface.py` & `clump-python-0.2.8/CLUMP/examples/Example_ExtractSurface.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/examples/Example_Favier_automatic_generation.py` & `clump-python-0.2.8/CLUMP/examples/Example_Favier_automatic_generation.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/examples/Example_Ferellec_McDowell.py` & `clump-python-0.2.8/CLUMP/examples/Example_Ferellec_McDowell.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat` & `clump-python-0.2.8/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat` & `clump-python-0.2.8/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl` & `clump-python-0.2.8/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/examples/ParticleGeometries/Hexahedron.stl` & `clump-python-0.2.8/CLUMP/examples/ParticleGeometries/Hexahedron.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/examples/ParticleGeometries/Human_femur.stl` & `clump-python-0.2.8/CLUMP/examples/ParticleGeometries/Human_femur.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/examples/ParticleGeometries/Octahedron.stl` & `clump-python-0.2.8/CLUMP/examples/ParticleGeometries/Octahedron.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/examples/ParticleGeometries/Torus.stl` & `clump-python-0.2.8/CLUMP/examples/ParticleGeometries/Torus.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/utils/MyRobustCrust.py` & `clump-python-0.2.8/CLUMP/utils/MyRobustCrust.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/utils/ParticlePlotter.py` & `clump-python-0.2.8/CLUMP/utils/ParticlePlotter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/utils/PatchNormals.py` & `clump-python-0.2.8/CLUMP/utils/PatchNormals.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/utils/RigidBodyParameters.py` & `clump-python-0.2.8/CLUMP/utils/RigidBodyParameters.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/utils/STL_ReaderWriter.py` & `clump-python-0.2.8/CLUMP/utils/STL_ReaderWriter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/CLUMP/utils/VTK_Writer.py` & `clump-python-0.2.8/CLUMP/utils/VTK_Writer.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/LICENSE` & `clump-python-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/clump_python.egg-info/SOURCES.txt` & `clump-python-0.2.8/clump_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.7/setup.py` & `clump-python-0.2.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-from setuptools import setup, find_packages
+from setuptools import setup
+from setuptools import find_packages
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="clump-python",
-    version="0.2.7",
+    version="0.2.8",
     packages=find_packages(),
     install_requires=[
         'matplotlib',
         'numpy',
         'numpy-stl',
         'pyvista',
         'scipy',
@@ -15,11 +20,13 @@
     package_data={
         # Include all *.stl and *.mat files found in any directory within the package
         '': ['**/*.stl', '**/*.mat'],
     },
     author="Utku Canbolat, Vasileios Angelidakis",
     author_email="utku.canbolat@fau.de",
     description="This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     license="GPL-3.0-only",
     keywords="Clump, Clump Generation, Euclidean Distance Transform, Favier, Ferellec-McDowell, Surface Extraction",
     url="https://github.com/vsangelidakis/CLUMP",
 )
```

