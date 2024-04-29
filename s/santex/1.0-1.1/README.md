# Comparing `tmp/santex-1.0.tar.gz` & `tmp/santex-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "santex-1.0.tar", last modified: Thu Apr 18 11:35:01 2024, max compression
+gzip compressed data, was "santex-1.1.tar", last modified: Mon Apr 29 22:45:23 2024, max compression
```

## Comparing `santex-1.0.tar` & `santex-1.1.tar`

### file list

```diff
@@ -1,50 +1,48 @@
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-18 11:35:01.214076 santex-1.0/
--rw-r--r--   0 usin8611   (502) staff       (20)     2830 2024-04-18 11:35:01.213558 santex-1.0/PKG-INFO
--rw-r--r--   0 usin8611   (502) staff       (20)     1565 2024-04-18 08:00:38.000000 santex-1.0/README.md
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-18 11:35:01.189883 santex-1.0/santex/
--rw-r--r--   0 usin8611   (502) staff       (20)      203 2024-04-18 07:52:49.000000 santex-1.0/santex/__init__.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-18 11:35:01.197694 santex-1.0/santex/anisotropy/
--rw-r--r--   0 usin8611   (502) staff       (20)       80 2024-03-20 02:12:45.000000 santex-1.0/santex/anisotropy/__init__.py
--rw-r--r--   0 usin8611   (502) staff       (20)    19250 2024-04-18 08:00:33.000000 santex-1.0/santex/anisotropy/anisotropy.py
--rw-r--r--   0 usin8611   (502) staff       (20)     1245 2024-03-29 03:12:40.000000 santex-1.0/santex/anisotropy/calcMeltVolume.py
--rw-r--r--   0 usin8611   (502) staff       (20)     2345 2024-04-18 01:13:19.000000 santex-1.0/santex/anisotropy/map.py
--rw-r--r--   0 usin8611   (502) staff       (20)     9124 2024-04-18 08:00:34.000000 santex-1.0/santex/anisotropy/melt.py
--rw-r--r--   0 usin8611   (502) staff       (20)      770 2024-03-20 02:12:45.000000 santex-1.0/santex/anisotropy/modalAnisotropy.py
--rw-r--r--   0 usin8611   (502) staff       (20)     2530 2024-04-18 01:13:34.000000 santex-1.0/santex/anisotropy/plot_seismic_velocity.py
--rw-r--r--   0 usin8611   (502) staff       (20)     2966 2024-04-18 08:00:36.000000 santex-1.0/santex/anisotropy/plot_vel_grid.py
--rw-r--r--   0 usin8611   (502) staff       (20)     1760 2024-03-20 02:12:45.000000 santex-1.0/santex/anisotropy/utils.py
--rw-r--r--   0 usin8611   (502) staff       (20)     9719 2024-03-20 02:12:45.000000 santex-1.0/santex/anisotropy/vtkplotter.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-18 11:35:01.205469 santex-1.0/santex/ebsd/
--rw-r--r--   0 usin8611   (502) staff       (20)       50 2024-03-20 02:12:45.000000 santex-1.0/santex/ebsd/__init__.py
--rw-r--r--   0 usin8611   (502) staff       (20)     4195 2024-04-18 07:02:34.000000 santex-1.0/santex/ebsd/calcGrainBoundary.py
--rw-r--r--   0 usin8611   (502) staff       (20)     3511 2024-03-20 02:12:45.000000 santex-1.0/santex/ebsd/calcGrainBoundary2.py
--rwxr-xr-x   0 usin8611   (502) staff       (20)     2489 2024-04-17 07:55:00.000000 santex-1.0/santex/ebsd/ctf_parser.py
--rw-r--r--   0 usin8611   (502) staff       (20)    20897 2024-04-18 07:15:43.000000 santex-1.0/santex/ebsd/ebsd.py
--rw-r--r--   0 usin8611   (502) staff       (20)     4989 2024-04-18 07:05:23.000000 santex-1.0/santex/ebsd/ebsdrotation.py
--rw-r--r--   0 usin8611   (502) staff       (20)      937 2024-04-02 06:06:56.000000 santex-1.0/santex/ebsd/melt.py
--rw-r--r--   0 usin8611   (502) staff       (20)    41037 2024-04-17 08:55:46.000000 santex-1.0/santex/ebsd/odf.py
--rw-r--r--   0 usin8611   (502) staff       (20)     6636 2024-04-18 07:05:44.000000 santex-1.0/santex/ebsd/rotateEBSD.py
--rw-r--r--   0 usin8611   (502) staff       (20)      551 2024-03-20 02:12:45.000000 santex-1.0/santex/ebsd/saveEBSD.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-18 11:35:01.206572 santex-1.0/santex/isotropy/
--rw-r--r--   0 usin8611   (502) staff       (20)       30 2024-03-20 02:12:45.000000 santex-1.0/santex/isotropy/__init__.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-18 11:35:01.207280 santex-1.0/santex/isotropy/data/
--rw-r--r--   0 usin8611   (502) staff       (20)    36992 2024-03-25 22:00:33.000000 santex-1.0/santex/isotropy/data/materials.json
--rw-r--r--   0 usin8611   (502) staff       (20)    12960 2024-03-28 06:43:14.000000 santex-1.0/santex/isotropy/isotropy.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-18 11:35:01.208736 santex-1.0/santex/material/
--rw-r--r--   0 usin8611   (502) staff       (20)       30 2024-03-20 02:12:45.000000 santex-1.0/santex/material/__init__.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-18 11:35:01.211498 santex-1.0/santex/material/data/
--rw-r--r--   0 usin8611   (502) staff       (20)    23272 2024-04-02 06:42:52.000000 santex-1.0/santex/material/data/derivatives_P.json
--rw-r--r--   0 usin8611   (502) staff       (20)    23300 2024-04-02 06:40:16.000000 santex-1.0/santex/material/data/derivatives_T.json
--rw-r--r--   0 usin8611   (502) staff       (20)    23072 2024-04-02 06:20:18.000000 santex-1.0/santex/material/data/materials_database.json
--rw-r--r--   0 usin8611   (502) staff       (20)    11525 2024-04-17 07:56:01.000000 santex-1.0/santex/material/material.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-18 11:35:01.213005 santex-1.0/santex/tensor/
--rw-r--r--   0 usin8611   (502) staff       (20)       26 2024-03-20 02:12:45.000000 santex-1.0/santex/tensor/__init__.py
--rw-r--r--   0 usin8611   (502) staff       (20)     3221 2024-03-20 02:12:45.000000 santex-1.0/santex/tensor/tensor.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-18 11:35:01.191979 santex-1.0/santex.egg-info/
--rw-r--r--   0 usin8611   (502) staff       (20)     2830 2024-04-18 11:35:01.000000 santex-1.0/santex.egg-info/PKG-INFO
--rw-r--r--   0 usin8611   (502) staff       (20)     1086 2024-04-18 11:35:01.000000 santex-1.0/santex.egg-info/SOURCES.txt
--rw-r--r--   0 usin8611   (502) staff       (20)        1 2024-04-18 11:35:01.000000 santex-1.0/santex.egg-info/dependency_links.txt
--rw-r--r--   0 usin8611   (502) staff       (20)       74 2024-04-18 11:35:01.000000 santex-1.0/santex.egg-info/requires.txt
--rw-r--r--   0 usin8611   (502) staff       (20)        7 2024-04-18 11:35:01.000000 santex-1.0/santex.egg-info/top_level.txt
--rw-r--r--   0 usin8611   (502) staff       (20)       38 2024-04-18 11:35:01.214130 santex-1.0/setup.cfg
--rw-r--r--   0 usin8611   (502) staff       (20)     1731 2024-04-18 11:34:43.000000 santex-1.0/setup.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-29 22:45:23.264203 santex-1.1/
+-rw-r--r--   0 usin8611   (502) staff       (20)    35149 2024-04-29 22:40:04.000000 santex-1.1/LICENSE
+-rw-r--r--   0 usin8611   (502) staff       (20)     2895 2024-04-29 22:45:23.263671 santex-1.1/PKG-INFO
+-rw-r--r--   0 usin8611   (502) staff       (20)     1625 2024-04-26 05:21:45.000000 santex-1.1/README.md
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-29 22:45:23.246825 santex-1.1/santex/
+-rw-r--r--   0 usin8611   (502) staff       (20)      203 2024-04-18 07:52:49.000000 santex-1.1/santex/__init__.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-29 22:45:23.253640 santex-1.1/santex/anisotropy/
+-rw-r--r--   0 usin8611   (502) staff       (20)       80 2024-03-20 02:12:45.000000 santex-1.1/santex/anisotropy/__init__.py
+-rw-r--r--   0 usin8611   (502) staff       (20)    20787 2024-04-26 03:15:28.000000 santex-1.1/santex/anisotropy/anisotropy.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     1949 2024-04-26 02:39:07.000000 santex-1.1/santex/anisotropy/map.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     8343 2024-04-26 03:25:54.000000 santex-1.1/santex/anisotropy/melt.py
+-rw-r--r--   0 usin8611   (502) staff       (20)      790 2024-04-26 01:57:52.000000 santex-1.1/santex/anisotropy/modalAnisotropy.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     3002 2024-04-26 03:55:11.000000 santex-1.1/santex/anisotropy/plot_seismic_velocity.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     3701 2024-04-26 02:06:53.000000 santex-1.1/santex/anisotropy/plot_vel_grid.py
+-rw-r--r--   0 usin8611   (502) staff       (20)      696 2024-04-26 03:15:41.000000 santex-1.1/santex/anisotropy/utils.py
+-rw-r--r--   0 usin8611   (502) staff       (20)    10990 2024-04-26 03:17:55.000000 santex-1.1/santex/anisotropy/vtkplotter.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-29 22:45:23.257893 santex-1.1/santex/ebsd/
+-rw-r--r--   0 usin8611   (502) staff       (20)       51 2024-04-26 03:57:28.000000 santex-1.1/santex/ebsd/__init__.py
+-rwxr-xr-x   0 usin8611   (502) staff       (20)     2236 2024-04-26 03:22:43.000000 santex-1.1/santex/ebsd/_ctf_parser.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     3180 2024-04-24 21:53:17.000000 santex-1.1/santex/ebsd/calcGrainBoundary.py
+-rw-r--r--   0 usin8611   (502) staff       (20)    30796 2024-04-29 17:18:09.000000 santex-1.1/santex/ebsd/ebsd.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     1077 2024-04-26 03:55:11.000000 santex-1.1/santex/ebsd/melt_tensor.py
+-rw-r--r--   0 usin8611   (502) staff       (20)    40972 2024-04-26 02:15:21.000000 santex-1.1/santex/ebsd/odf.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     5000 2024-04-26 03:55:11.000000 santex-1.1/santex/ebsd/rotateEBSD.py
+-rw-r--r--   0 usin8611   (502) staff       (20)      551 2024-03-20 02:12:45.000000 santex-1.1/santex/ebsd/saveEBSD.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-29 22:45:23.258902 santex-1.1/santex/isotropy/
+-rw-r--r--   0 usin8611   (502) staff       (20)       30 2024-03-20 02:12:45.000000 santex-1.1/santex/isotropy/__init__.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-29 22:45:23.259388 santex-1.1/santex/isotropy/data/
+-rw-r--r--   0 usin8611   (502) staff       (20)    36992 2024-03-25 22:00:33.000000 santex-1.1/santex/isotropy/data/materials.json
+-rw-r--r--   0 usin8611   (502) staff       (20)    14900 2024-04-26 03:55:11.000000 santex-1.1/santex/isotropy/isotropy.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-29 22:45:23.260278 santex-1.1/santex/material/
+-rw-r--r--   0 usin8611   (502) staff       (20)       30 2024-03-20 02:12:45.000000 santex-1.1/santex/material/__init__.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-29 22:45:23.261966 santex-1.1/santex/material/data/
+-rw-r--r--   0 usin8611   (502) staff       (20)    36654 2024-04-29 16:14:37.000000 santex-1.1/santex/material/data/derivatives_P.json
+-rw-r--r--   0 usin8611   (502) staff       (20)    36845 2024-04-29 16:07:01.000000 santex-1.1/santex/material/data/derivatives_T.json
+-rw-r--r--   0 usin8611   (502) staff       (20)    23072 2024-04-02 06:20:18.000000 santex-1.1/santex/material/data/materials_database.json
+-rw-r--r--   0 usin8611   (502) staff       (20)    16915 2024-04-29 00:44:37.000000 santex-1.1/santex/material/material.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-29 22:45:23.263085 santex-1.1/santex/tensor/
+-rw-r--r--   0 usin8611   (502) staff       (20)       26 2024-03-20 02:12:45.000000 santex-1.1/santex/tensor/__init__.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     3445 2024-04-26 03:55:11.000000 santex-1.1/santex/tensor/tensor.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-29 22:45:23.248676 santex-1.1/santex.egg-info/
+-rw-r--r--   0 usin8611   (502) staff       (20)     2895 2024-04-29 22:45:23.000000 santex-1.1/santex.egg-info/PKG-INFO
+-rw-r--r--   0 usin8611   (502) staff       (20)     1004 2024-04-29 22:45:23.000000 santex-1.1/santex.egg-info/SOURCES.txt
+-rw-r--r--   0 usin8611   (502) staff       (20)        1 2024-04-29 22:45:23.000000 santex-1.1/santex.egg-info/dependency_links.txt
+-rw-r--r--   0 usin8611   (502) staff       (20)       91 2024-04-29 22:45:23.000000 santex-1.1/santex.egg-info/requires.txt
+-rw-r--r--   0 usin8611   (502) staff       (20)        7 2024-04-29 22:45:23.000000 santex-1.1/santex.egg-info/top_level.txt
+-rw-r--r--   0 usin8611   (502) staff       (20)       38 2024-04-29 22:45:23.264260 santex-1.1/setup.cfg
+-rw-r--r--   0 usin8611   (502) staff       (20)     1710 2024-04-29 22:45:20.000000 santex-1.1/setup.py
```

### Comparing `santex-1.0/PKG-INFO` & `santex-1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 Metadata-Version: 2.1
 Name: santex
-Version: 1.0
+Version: 1.1
 Summary: SAnTeX is a Python library which calculates seismic anisotropy from full elastic tensor of rocks from modal mineral composition, crystallographic orientation, and a crystal stiffness tensor catalogue that accounts for the dependency of elasticity with pressure and temperature. SAnTex facilitates the processing and cleaning of EBSD data and calculation of Orientation Distribution Function (ODF) and Inverse pole figure (IPF)
 Home-page: https://github.com/utpal-singh/SAnTex
 Author: Utpal Singh
 Author-email: utpal_singh@yahoo.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Keywords: python,seismic,seismic anisotropy,EBSD,Texture,Crystallography
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: joblib
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: vtk
 Requires-Dist: tqdm
 Requires-Dist: tabulate
 Requires-Dist: scikit-learn
 Requires-Dist: plotly
 Requires-Dist: orix
+Requires-Dist: sphinx_rtd_theme
 
 # SAnTex: Seismic Anisotropy from Texture
 
-SAnTeX is a Python library which calculates the full elastic tensor of rocks from modal mineral composition, crystallographic orientation, and a crystal stiffness tensor catalogue that accounts for the dependency of elasticity with pressure and temperature.
+SAnTex is a Python library which calculates the full elastic tensor of rocks from modal mineral composition, crystallographic orientation, and a crystal stiffness tensor catalogue that accounts for the dependency of elasticity with pressure and temperature.
 
 ## Features
 
 - **Pre-processing and cleaning of EBSD data**: SAnTex facilitates the processing and cleaning of EBSD data.  To enhance data completeness, SAnTex  offers the option to fill not-indexed pixels or indexed pixels removed during the cleaning process, using machine learning techniques.
 - **Tensor operations**: Tensor conversions between Voigt matrix and full stiffness tensors, as well as rotations based on euler angles.
 - **Material analysis**: SAnTex provides a catalogue of minerals, users can load the catalogue and can either utilise them to load stiffness tensors for their EBSD phases or make a modal rock and can calculate seismic anisotropy for the modal rock.
 - **Seismic Anisotropy**: SAnTex performs calculations of seismic anisotropy at a range of pressure and temperature conditions.  It also offers visualisation capabilities, allowing users to view the calculated seismic anisotropy in 2D and 3D plots. 
 - **Isotropic velocities**: Calculates isotropic seismic wave velocities (Vp, Vs and vbulk), isothermal bulk modulus, and density at elevated temperatures and pressures (Hacker & Abers, 2004). 
 
 
 ## Installation
 
-You can install SAnTeX using pip:
+You can install SAnTex using pip from your terminal:
 
 ```bash
 git clone https://github.com/utpal-singh/SAnTex.git
-cd sage
+cd santex
 pip install .
+```
 
+
+or
+
+```bash
+pip install santex
+```
```

### Comparing `santex-1.0/README.md` & `santex-1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 # SAnTex: Seismic Anisotropy from Texture
 
-SAnTeX is a Python library which calculates the full elastic tensor of rocks from modal mineral composition, crystallographic orientation, and a crystal stiffness tensor catalogue that accounts for the dependency of elasticity with pressure and temperature.
+SAnTex is a Python library which calculates the full elastic tensor of rocks from modal mineral composition, crystallographic orientation, and a crystal stiffness tensor catalogue that accounts for the dependency of elasticity with pressure and temperature.
 
 ## Features
 
 - **Pre-processing and cleaning of EBSD data**: SAnTex facilitates the processing and cleaning of EBSD data.  To enhance data completeness, SAnTex  offers the option to fill not-indexed pixels or indexed pixels removed during the cleaning process, using machine learning techniques.
 - **Tensor operations**: Tensor conversions between Voigt matrix and full stiffness tensors, as well as rotations based on euler angles.
 - **Material analysis**: SAnTex provides a catalogue of minerals, users can load the catalogue and can either utilise them to load stiffness tensors for their EBSD phases or make a modal rock and can calculate seismic anisotropy for the modal rock.
 - **Seismic Anisotropy**: SAnTex performs calculations of seismic anisotropy at a range of pressure and temperature conditions.  It also offers visualisation capabilities, allowing users to view the calculated seismic anisotropy in 2D and 3D plots. 
 - **Isotropic velocities**: Calculates isotropic seismic wave velocities (Vp, Vs and vbulk), isothermal bulk modulus, and density at elevated temperatures and pressures (Hacker & Abers, 2004). 
 
 
 ## Installation
 
-You can install SAnTeX using pip:
+You can install SAnTex using pip from your terminal:
 
 ```bash
 git clone https://github.com/utpal-singh/SAnTex.git
-cd sage
+cd santex
 pip install .
+```
 
+
+or
+
+```bash
+pip install santex
+```
```

### Comparing `santex-1.0/santex/anisotropy/anisotropy.py` & `santex-1.1/santex/anisotropy/anisotropy.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from .vtkplotter import Plotter
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 from .plot_vel_grid import plot_velocity_grid
+from .utils import christoffel_tensor, wave_property
 
 from .. import Material
 from .. import EBSD
 
 from scipy.interpolate import griddata
 import math
 
@@ -80,21 +81,15 @@
             ValueError: If an error occurs during the calculation.
 
         Example direction:
             n = np.array([1, 0, 0])
         
         """
         try:
-            tik = np.zeros((3, 3))
-
-            for i in range(3):
-                for k in range(3):
-                    tik[i, k] = np.tensordot(self.cijkl[i, :, k, :], np.outer(n, n))
-
-            return tik
+            return christoffel_tensor(self.cijkl, n)
         except Exception as e:
             raise ValueError("Error in calculating the Christoffel tensor:", e)
 
     def wave_property(self, tik):
         """
         Calculates the wave properties (wave moduli and polarization directions) given the Christoffel tensor Tik.
 
@@ -104,21 +99,15 @@
         Returns:
             tuple: A tuple containing the wave moduli and polarization directions.
 
         Raises:
             ValueError: If an error occurs during the calculation.
         """
         try:
-            eigenvalues, eigenvectors = np.linalg.eig(tik)
-            indices = np.argsort(eigenvalues)[::-1]
-
-            wave_moduli = [eigenvalues[i] for i in indices]
-            polarization_directions = [eigenvectors[:, i] / np.linalg.norm(eigenvectors[:, i]) for i in indices]
-
-            return tuple(wave_moduli), tuple(polarization_directions)
+            return wave_property(tik)
         except Exception as e:
             raise ValueError("Error in calculating wave properties:", e)
 
     def phase_velocity(self):
         """
         Calculates the phase velocities (P-wave velocity, S1-wave velocity, and S2-wave velocity) for different
         directions using the Christoffel tensor and wave properties.
@@ -264,34 +253,34 @@
             }
         
     def plot_velocities(self, pressure_range, temperature_range, return_type, is_ebsd = False, phase = None, grid = [5, 5], filename = None, *args):
         """
         Plots velocities based on specified ranges and return types.
 
             Parameters:
-                pressure_range (tuple): The range of pressures for which velocities will be plotted.
-                temperature_range (tuple): The range of temperatures for which velocities will be plotted.
+                pressure_range (tuple): The range of pressures for which velocities will be plotted. Example: [2, 4].
+                temperature_range (tuple): The range of temperatures for which velocities will be plotted. Example: [1000, 2000]
                 return_type (str): The type of velocity to plot. Options: 'maxvp', 'minvp', 'maxvs1', 'minvs1', 'maxvs2', 'minvs2'.
                 is_ebsd (bool): Whether the data comes from electron backscatter diffraction (EBSD). Default is False.
-                phase (str or None): The phase of the material. Only required if is_ebsd is True.
+                phase (str or None): The phase of the material. Example, phase = 'Forsterite'
                 grid (list): The grid dimensions for the plot. Default is [5, 5].
-                filename (str or None): The filename to save the plot. Required if is_ebsd is True.
-                *args: can be [01, 2, 3]
+                filename (str or None): The filename of the EBSD data. Required if is_ebsd is True.
+                *args: can be [1, 2, 3]
 
             Raises:
                 ValueError: If required parameters are not provided or if an error occurs during plotting.
 
             Notes:
                 - If is_ebsd is True, phase and filename must be provided.
                 - The plot type and appearance can be customized using *args.
 
             Example Usage:
                 anisotropy.plot_velocities((0, 100), (500, 1000), 'maxvp', is_ebsd=True, phase='phase1', filename='velocity_plot.png', 'ro-')
         """
-        plot_velocity_grid(pressure_range, temperature_range, return_type, is_ebsd = False, phase = phase, grid = [5, 5], filename = None, *args)
+        return plot_velocity_grid(pressure_range=pressure_range, temperature_range=temperature_range, return_type=return_type, is_ebsd=is_ebsd, phase = phase, grid = grid, filename = filename, *args)
 
 
 
     def plot(self, colormap="RdBu_r", step = 180, savefig = False, figname = None, dpi = 300):
         """
         Plots various anisotropic maps based on the Christoffel tensor.
 
@@ -382,14 +371,31 @@
             if savefig:
                 plt.savefig(f"{figname}", dpi = dpi)
         except Exception as e:
             print(f"An error occurred: {e}")
 
 
     def plotly(self):
+        """
+        Generates a Plotly figure to visualize material properties based on calculations using Christoffel and wave tensors.
+
+        This method creates a Plotly figure with subplots for various properties such as VP/VS1, VP, VS1, VS2, AVpVs1, and AVpVs2.
+        The figure is generated by iterating over specified ranges of angles and calculating properties like wave moduli, VP, VS1, VS2,
+        VP/VS1 ratios, and AVpVs1/AVpVs2 ratios. The resulting data points are plotted on scatter plots with a color scale representing
+        different property values.
+
+        Raises:
+            ValueError: If an error occurs during the plotting process.
+
+        Notes:
+            - Requires the existence of the `christoffel_tensor` and `wave_property` methods in the class instance to calculate material properties.
+
+        Example Usage:
+            plotter = anisotropy_instance.plotly()
+        """
         try:
             fig = go.Figure()
 
             step = math.pi / 180
 
             fig = make_subplots(rows=2, cols=3, subplot_titles=("VP/VS1", "VP", "VS1", "VS2", "AVpVs1", "AVpVs2"))
 
@@ -447,21 +453,48 @@
             fig.show()
         except Exception as e:
             raise ValueError("Error in plotting:", e)
 
 
             
     def plotter_vs_splitting(self, density, voigt_stiffness):
+        """
+        Plots the Vs splitting based on density and Voigt stiffness.
 
+        Parameters:
+            density (float): The density of the material.
+            voigt_stiffness (float): The Voigt stiffness of the material.
+        """
         Plotter.plot_vs_splitting(voigt_stiffness, density)
 
     def plotter_vp(self, density, voigt_stiffness):
+        """
+        Plots the Vp based on density and Voigt stiffness.
+
+        Parameters:
+            density (float): The density of the material.
+            voigt_stiffness (float): The Voigt stiffness of the material.
+        """
 
         Plotter.plot_vp(voigt_stiffness, density)
 
     def plotter_vs1(self, density, voigt_stiffness):
+        """
+        Plots the Vs1 based on density and Voigt stiffness.
+
+        Parameters:
+            density (float): The density of the material.
+            voigt_stiffness (float): The Voigt stiffness of the material.
+        """
 
         Plotter.plot_vp(voigt_stiffness, density)
 
     def plotter_vs2(self, density, voigt_stiffness):
+        """
+        Plots the Vs2 based on density and Voigt stiffness.
+
+        Parameters:
+            density (float): The density of the material.
+            voigt_stiffness (float): The Voigt stiffness of the material.
+        """
 
         Plotter.plot_vp(voigt_stiffness, density)
```

### Comparing `santex-1.0/santex/anisotropy/map.py` & `santex-1.1/santex/anisotropy/map.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,14 +43,9 @@
     
     ax.plot(lon_points, lat_points, 'ro', markersize=5, transform=ccrs.Geodetic(), label='Data Points')
     
     plt.legend()
     plt.title("Interpolated Data Map")
     plt.show()
 
-lon_points = np.array([138.58, 138.60, 138.62, 138.64, 138.66, 138.68, 138.70, 138.72, 138.74, 138.76])
-lat_points = np.array([-34.92, -34.93, -34.94, -34.95, -34.96, -34.97, -34.98, -34.99, -35.00, -35.01])
-values = np.random.randint(100, 500, size=10)  # Random sample values for demonstration
-
-interp_box = (138.5, -35.0, 139.0, -34.5)  # Defined as (left_lon, bottom_lat, right_lon, top_lat)
```

### Comparing `santex-1.0/santex/anisotropy/melt.py` & `santex-1.1/santex/anisotropy/melt.py`

 * *Files 6% similar despite different names*

```diff
@@ -163,31 +163,10 @@
 
     for i in range(len(fraction)):
         cij_average += fraction[i] * cij[i]
     return cij_average, rho_average
 
 
 
-if __name__ == "__main__":
-    weight_per = [40, 1.84, 13.7, 2.7, 9.57, 6.67, 11.5, 2.68, 0.25, 10]
-    dens, component_density = calc_melt_density(weight_per, 500, 1273)
-    print(dens)
-    print(component_density)
-    rock = ["Forsterite", "Diopside", "Enstatite"]
-    fraction = [0.2, 0.5, 0.3]
-    cij_average, rho_average = modalRock(rock, fraction, 2, 1000)
-    print(cij_average)
-    print(rho_average)
-
-    cij_average, rho_average = modalRock(rock, fraction, 2, 1000, 0.05, weight_per)
-    print(cij_average)
-    print(rho_average)
-
-    oxide_dict = {'sio2': 40, 'tio2': 1.84, 'feo': 9.57, 'mgo': 6.67, 'cao': 11.5, 'na2o': 2.68, 'k2o': 0.25, 'h2o': 10}
-    dens, component_density = calc_melt_density(oxide_dict, 500, 1500)
-    print(dens)
-    print(component_density)
-
-
```

### Comparing `santex-1.0/santex/anisotropy/modalAnisotropy.py` & `santex-1.1/santex/anisotropy/modalAnisotropy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from ..material import Material
 from ..anisotropy import Anisotropy
 
+import numpy as np
+
 def modalAnisotropy(material, fraction, pressure, temperature):
     voigtMatrixTotal = []
     density = []
     for i in range(len(material)):
         material_instance = Material()
         phase = 'Diopside'
         voigtMatrix = material_instance.voigthighPT(material[i], PRESSURE = pressure, TEMP = temperature)
```

### Comparing `santex-1.0/santex/anisotropy/plot_seismic_velocity.py` & `santex-1.1/santex/anisotropy/plot_seismic_velocity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,23 @@
 import numpy as np
 import math
-
 import matplotlib.pyplot as plt
-from mpl_toolkits import mplot3d
-
-def christoffel_tensor(cijkl, n):
-    tik = np.zeros((3, 3))
-
-    for i in range(3):
-        for k in range(3):
-            for j in range(3):
-                for l in range(3):
-                    tik[i][k] += cijkl[i][j][k][l] * n[j] * n[l]
-
-    return tik
-
-
-def wave_property(tik):
-    eigenvalues, eigenvectors = np.linalg.eig(tik)
-    indices = np.argsort(eigenvalues)[::-1]
-    wave_moduli = []
-    polarization_directions = []
-
-    for i in indices:
-        wave_moduli.append(eigenvalues[i])
-        polarization_directions.append(eigenvectors[:, i] / np.linalg.norm(eigenvectors[:, i]))
-    return tuple(wave_moduli), tuple(polarization_directions)
-
+from .utils import christoffel_tensor, wave_property
 
 def phase_velocity(cijkl, rho):
+    """
+    Calculate phase velocities for various propagation directions.
+
+    Parameters:
+    - cijkl (array): The fourth-rank stiffness tensor for the material.
+    - rho (float): Density of the material.
+
+    Returns:
+    - tuple: Tuples containing phase velocities for P-wave (vp), S-wave with higher velocity (vs1), and S-wave with lower velocity (vs2).
+    """
     vp = []
     vs1 = []
     vs2 = []
     step = math.pi / 180
 
     for theta in np.arange(0, math.pi + step, step):
         for phi in np.arange(0, 2 * math.pi + step, step):
@@ -42,38 +27,55 @@
             tik = christoffel_tensor(cijkl, n)
             wave_moduli, polarization_directions = wave_property(tik)
             vp.append(math.sqrt(wave_moduli[0] / rho))
             vs1.append(math.sqrt(wave_moduli[1] / rho))
             vs2.append(math.sqrt(wave_moduli[2] / rho))
     return tuple(vp), tuple(vs1), tuple(vs2)
 
-
-def plot_vp_2d(cijkl, rho):
+def plot_vp_2d(cijkl, rho, save_plot=False, filename=None, dpi=300, cmap='RdBu'):
+    """
+    Plot phase velocities in a 2D stereographic projection.
+
+    Parameters:
+    - cijkl (array): The fourth-rank stiffness tensor for the material.
+    - rho (float): Density of the material.
+    - save_plot (bool): Whether to save the plot or not. Default is False.
+    - filename (str): Name of the file to save the plot. Required if save_plot is True.
+    - dpi (int): Dots per inch for saving the plot. Default is 300.
+    - cmap (str or Colormap): The colormap to be used for the scatter plot. Default is 'RdBu'.
+
+    Returns:
+    - None
+    """
     fig = plt.figure()
     ax = fig.add_subplot(111)
     step = math.pi / 180
     x = []
     y = []
     c = []
 
     for theta in np.arange(0, math.pi / 2 + step, step):
         for phi in np.arange(0, 2 * math.pi + step, step):
             n = np.array([math.sin(theta) * math.cos(phi), math.sin(theta) * math.sin(phi), math.cos(theta)])
-            # print(n)
             tik = christoffel_tensor(cijkl, n)
             wave_moduli, polarization_directions = wave_property(tik)
             vp = math.sqrt(wave_moduli[0] / rho)
-            # print(vp)
             x.append(n[0] / (1 + n[2]))
             y.append(n[1] / (1 + n[2]))
             c.append(vp)
 
-    sc = ax.scatter(x, y, c=c, cmap='RdBu')
+    sc = ax.scatter(x, y, c=c, cmap=cmap)
     ax.set_xlabel('x')
     ax.set_ylabel('y')
     ax.set_title('vp in 2d stereographic projection plots with velocity represented by colour')
     cb = plt.colorbar(sc)
     cb.set_label('vp')
     cb.ax.set_yticklabels(['{:.1f}'.format(v) for v in cb.get_ticks()])
-    plt.show()
+
+    if save_plot:
+        if filename is None:
+            raise ValueError("Filename must be provided when saving the plot.")
+        plt.savefig(filename, dpi=dpi)
+    else:
+        plt.show()
```

### Comparing `santex-1.0/santex/anisotropy/plot_vel_grid.py` & `santex-1.1/santex/anisotropy/plot_vel_grid.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
-from santex import Material
 import matplotlib.pyplot as plt
 
-def plot_velocity_grid(pressure_range, temperature_range, return_type, is_ebsd = False, phase = None, grid = [5, 5], filename = None, *args):
+def plot_velocity_grid(pressure_range, temperature_range, return_type, is_ebsd = False, phase = None, grid = [5, 5], filename = None,fig_name=None, save_plot=False, dpi=300, *args):
     from santex import Anisotropy
+    from santex import EBSD
+    from santex import Material
     """
     Generates a grid of velocity values based on specified pressure and temperature ranges.
 
     Parameters:
         pressure_range (tuple): A tuple containing the minimum and maximum pressure values (in GPa).
         temperature_range (tuple): A tuple containing the minimum and maximum temperature values (in Kelvin).
         return_type (str): The type of velocity values to return. Allowed values are 'maxvp', 'minv', 'maxvs1', 'minvs1', 'maxvs2', 'minvs2'.
@@ -30,34 +31,49 @@
     give filename is is_ebsd is True
     """
 
     if is_ebsd is False:
         cij = []
         density = []
 
-
         pressure_grid = np.linspace(pressure_range[0], pressure_range[1], grid[0])
         temperature_grid = np.linspace(temperature_range[0], temperature_range[1], grid[1])
-        
         vp_matrix = np.zeros((grid[0], grid[1]))
         
         for i, p in enumerate(pressure_grid):
             for j, t in enumerate(temperature_grid):
                 material = Material()
                 cij_highpt = material.voigthighPT(phase, p, t)*10**9
                 density_highpt = material.load_density(phase, p, t)
                 anisotropy = Anisotropy(cij_highpt, density_highpt)
                 vp_matrix[i, j] = anisotropy.anisotropy_values(return_values=return_type)
+        pressure_mesh, temperature_mesh = np.meshgrid(pressure_grid, temperature_grid)
+        plt.figure(figsize=(8, 6))
+        plt.pcolormesh(pressure_mesh, temperature_mesh, vp_matrix, shading='auto', cmap='viridis')
+        plt.colorbar(label=f'{return_type}')
+        plt.xlabel('Pressure')
+        plt.ylabel('Temperature')
+        plt.title(f'{return_type} vs. Pressure and Temperature')
+        # plt.grid(True)
+        plt.tight_layout()
+        if save_plot:
+            if fig_name is None:
+                raise ValueError("Filename must be provided when saving the plot.")
+            plt.savefig(fig_name, dpi=dpi)
+        else:
+            plt.show()
 
         return vp_matrix
 
     if is_ebsd is True:
         euler_angles = []
         df = ebsd.get_ebsd_data()
         for i in args:
             ebsd = EBSD(filename)
             euler_angles.append(ebsd.get_euler_angles(phase=i, data = df))
 
         average_tensor, average_density = ebsd.getAnisotropyForEBSD(cij, euler_angles, density)
         anis = Anisotropy(average_tensor*10**9, average_density)
+    
+
```

### Comparing `santex-1.0/santex/anisotropy/vtkplotter.py` & `santex-1.1/santex/anisotropy/vtkplotter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 import numpy as np
 from vtk import (
     vtkStructuredGrid, vtkPoints, vtkFloatArray,
     vtkStructuredGridGeometryFilter, vtkPolyDataMapper,
     vtkActor, vtkRenderer, vtkRenderWindow,
     vtkRenderWindowInteractor
 )
-# from .anisotropy import Anisotropy
-# from cijkl_3dplots import christoffel_tensor, wave_property
-# import tensor_conversion
-
-from .utils import christoffel_tensor, wave_property, tensor_to_voigt, voigt_to_tensor
+from ..tensor.tensor import Tensor
+from .utils import christoffel_tensor, wave_property
 
+tensor = Tensor()
 class Plotter:
+    """
+    A class for plotting seismic wave velocities in 3D using VTK.
+
+    Attributes:
+    - None
+    """
     @classmethod
     def plot_vs_splitting(cls, c, rho):
-        cijkl = voigt_to_tensor(c)
+        """
+        Plot the difference between S-wave velocities (vs1 - vs2) in 3D using VTK.
+
+        Parameters:
+        - c (array): The fourth-rank stiffness tensor in Voigt notation.
+        - rho (float): Density of the material.
+
+        Returns:
+        - None
+        """
+        cijkl = tensor.voigt_to_tensor(c)
 
         theta = np.linspace(0, np.pi, 100)
         phi = np.linspace(0, 2 * np.pi, 100)
         theta, phi = np.meshgrid(theta, phi)
 
         x = np.sin(theta) * np.cos(phi)
         y = np.sin(theta) * np.sin(phi)
@@ -75,15 +89,25 @@
         interactor.SetRenderWindow(render_window)
 
         interactor.Initialize()
         interactor.Start()
 
     @classmethod
     def plot_vp(cls, c, rho):
-        cijkl = voigt_to_tensor(c)
+        """
+        Plot the P-wave velocities (vp) in 3D using VTK.
+
+        Parameters:
+        - c (array): The fourth-rank stiffness tensor in Voigt notation.
+        - rho (float): Density of the material.
+
+        Returns:
+        - None
+        """
+        cijkl = tensor.voigt_to_tensor(c)
 
         theta = np.linspace(0, np.pi, 100)
         phi = np.linspace(0, 2 * np.pi, 100)
         theta, phi = np.meshgrid(theta, phi)
 
         x = np.sin(theta) * np.cos(phi)
         y = np.sin(theta) * np.sin(phi)
@@ -140,15 +164,25 @@
         interactor.SetRenderWindow(render_window)
 
         interactor.Initialize()
         interactor.Start()
 
     @classmethod
     def plot_vs1(cls, c, rho):
-        cijkl = voigt_to_tensor(c)
+        """
+        Plot the S-wave velocities with higher velocity (vs1) in 3D using VTK.
+
+        Parameters:
+        - c (array): The fourth-rank stiffness tensor in Voigt notation.
+        - rho (float): Density of the material.
+
+        Returns:
+        - None
+        """
+        cijkl = tensor.voigt_to_tensor(c)
 
         theta = np.linspace(0, np.pi, 100)
         phi = np.linspace(0, 2 * np.pi, 100)
         theta, phi = np.meshgrid(theta, phi)
 
         x = np.sin(theta) * np.cos(phi)
         y = np.sin(theta) * np.sin(phi)
@@ -204,15 +238,39 @@
         interactor = vtkRenderWindowInteractor()
         interactor.SetRenderWindow(render_window)
 
         interactor.Initialize()
         interactor.Start()
     @classmethod
     def plot_vp(cls, c, rho):
-        cijkl = voigt_to_tensor(c)
+
+        """
+        Plot the P-wave velocities (vp) in 3D using VTK.
+
+        This method calculates and visualizes the P-wave velocities (vp) for a given fourth-rank stiffness tensor (c)
+        and material density (rho) using the Visualization Toolkit (VTK).
+
+        Parameters:
+        - c (array): The fourth-rank stiffness tensor in Voigt notation.
+        - rho (float): Density of the material.
+
+        Returns:
+        - None
+
+        Usage Example:
+        >>> c = np.array([[323.70, 66.40, 71.60, 0.000, 0.000, 0.000],
+        ...               [66.40, 197.60, 75.60, 0.000, 0.000, 0.000],
+        ...               [71.60, 75.60, 235.10, 0.000, 0.000, 0.000],
+        ...               [0.000, 0.000, 0.000, 64.62, 0.000, 0.000],
+        ...               [0.000, 0.000, 0.000, 0.000, 78.05, 0.000],
+        ...               [0.000, 0.000, 0.000, 0.000, 0.000, 79.04]]) * 1e9
+        >>> Plotter.plot_vp(c, 3310)
+        """
+
+        cijkl = tensor.voigt_to_tensor(c)
 
         theta = np.linspace(0, np.pi, 100)
         phi = np.linspace(0, 2 * np.pi, 100)
         theta, phi = np.meshgrid(theta, phi)
 
         x = np.sin(theta) * np.cos(phi)
         y = np.sin(theta) * np.sin(phi)
@@ -266,21 +324,7 @@
         render_window.AddRenderer(renderer)
 
         interactor = vtkRenderWindowInteractor()
         interactor.SetRenderWindow(render_window)
 
         interactor.Initialize()
         interactor.Start()
-
-
-
-if __name__ == "__main__":
-    density = 3310
-    c = np.array([[323.70, 66.40, 71.60, 0.000, 0.000, 0.000],
-                [66.40, 197.60, 75.60, 0.000, 0.000, 0.000],
-                [71.60, 75.60, 235.10, 0.000, 0.000, 0.000],
-                [0.000, 0.000, 0.000, 64.62, 0.000, 0.000],
-                [0.000, 0.000, 0.000, 0.000, 78.05, 0.000],
-                [0.000, 0.000, 0.000, 0.000, 0.000, 79.04]]) * 1e9
-    # cijkl = tensor_conversion.voigt_to_tensor(c)
-
-    Plotter.plot_wave_velocities(c, density)
```

### Comparing `santex-1.0/santex/ebsd/calcGrainBoundary.py` & `santex-1.1/santex/ebsd/calcGrainBoundary.py`

 * *Files 17% similar despite different names*

```diff
@@ -94,28 +94,7 @@
         progress = (processed_rows / total_rows) * 100
         print(f"Progress: {progress:.2f}%\r", end='')
 
     Parallel(n_jobs=-1, prefer="threads")(delayed(process_row)(row) for _, row in df.iterrows())
 
     return grain_indices
 
-# # Sample phase names
-# phase_names = ['nothn', 'Forsterite', 'Enstatite Opx AV77', 'Diopside CaMgSi2O6',  
-#                'Anorthite', 'Hornblende', 'Chromite', 'Pyrope']
-
-# # Assume df contains the dataframe with columns Phase, Euler1, Euler2, Euler3
-# # Replace df with your actual dataframe
-
-# # Assign rows to grains in parallel
-# threshold = 20 # Misorientation threshold
-# grain_indices = assign_to_grains_parallel(df[['Euler1', 'Euler2', 'Euler3']], threshold)
-
-# # Add grain indices to the dataframe
-# df['Grain'] = pd.Series(grain_indices)
-
-# # Display grains with their respective phase names
-# for grain_idx, group in df.groupby('Grain'):
-#     phase_counts = group['Phase'].value_counts()
-#     dominant_phase = phase_counts.idxmax()
-#     print(f"Grain {grain_idx}: Dominant Phase - {phase_names[dominant_phase]}, Size - {len(group)}")
-
-# # Now you have grains organized based on similar Euler angles with a maximum misorientation of 10 degrees, using parallel processing with progress indication.
```

### Comparing `santex-1.0/santex/ebsd/ctf_parser.py` & `santex-1.1/santex/ebsd/_ctf_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,25 +41,15 @@
         return self.nphases, self.mag, self.coverage, self.device, self.kv, self.tilt_angle, self.phases
             
 
     def get_data(self):
         with open(self._filename, 'r') as file:
             lines = file.readlines()
 
-    # print(lines[:15])
         header_start = lines.index('JobMode\tGrid\n')
-        # print(header_start)
         data_start = lines.index('Phase\tX\tY\tBands\tError\tEuler1\tEuler2\tEuler3\tMAD\tBC\tBS\n')
-        # print(data_start)
-
         header_data = pd.read_csv(self._filename, delimiter='\t', skiprows=header_start+1, nrows=7, names=["info", "value"])
-        # print(header_data)
-
         data = pd.read_csv(self._filename, delimiter='\t', skiprows=data_start)
-        # print(data)
-        # print(data)
-        # header_info = pd.read_csv(filename, sep="\t", nrows=data_start)
-        # print(data)
         return data, header_data
 
     def get_phases_numbers(self):
         return self.get_data
```

### Comparing `santex-1.0/santex/ebsd/ebsd.py` & `santex-1.1/santex/ebsd/ebsd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # sage/ebsd/ebsd.py
 
-from .ctf_parser import Ctf
+from ._ctf_parser import Ctf
 import matplotlib.pyplot as plt 
 from tabulate import tabulate
 import os
 
 import numpy as np 
 import pandas as pd 
-from sklearn.neighbors import KNeighborsClassifier 
-from joblib import Parallel, delayed 
 from ..tensor import Tensor
 from scipy.spatial.transform import Rotation
 
 from .calcGrainBoundary import assign_to_grains_parallel
 import plotly.express as px
 
-from .melt import calcMelttensor
+from .melt_tensor import calcMelttensor
 from .rotateEBSD import apply_custom_rotation_to_dataframe, apply_custom_rotation_to_dataframe_noxy
 
 # from .ebsdrotation import apply_custom_rotation_to_dataframe as rotebsd
-from .ebsdrotation import plot as plotrotebsd
 from .odf import ipf, odf, pdf
 
 class EBSD:
     """
     Class for handling Electron Backscatter Diffraction (EBSD) data.
     """
 
@@ -60,23 +57,30 @@
             data, header_data = self.ctf.get_data()
         phase_df = data[data['Phase'] == phase]
         euler_angles = phase_df[['Euler1', 'Euler2', 'Euler3']]
         euler_angles = euler_angles.reset_index(drop=True)
         return euler_angles
         
 
-    def plot(self, data=None, rotation_angle=0, inside_plane=True, mirror=False):
+    def plot(self, data=None, rotation_angle=0, inside_plane=True, mirror=False, save_image=False, image_filename=None, 
+             dpi=300, cmap='viridis', phase_colors=None, legend_location = "upper right"):
         """
         Plots the EBSD map with colors based on phase. Allows for rotation and optional mirroring of the data.
 
         Parameters:
             data (pandas.DataFrame, optional): DataFrame containing EBSD data. If not provided, uses stored data.
             rotation_angle (int, optional): Angle by which to rotate the EBSD data (in degrees). Accepts 0, 90, 180, 270.
             inside_plane (bool, optional): If True, rotates the EBSD data inside the plane. If False, rotates outside the plane. Default is True.
             mirror (bool, optional): If True, mirrors the EBSD data horizontally before rotating. Default is False.
+            save_image (bool, optional): If True, saves the plot as an image. Default is False.
+            image_filename (str, optional): Filename to use when saving the image. Required if save_image is True.
+            dpi (int, optional): Dots per inch for the saved image. Default is 300.
+            cmap (str, optional): Colormap to use for plotting. Default is 'viridis'.
+            phase_colors (dict, optional): Custom colors for each phase. Should be in the format {phase_number: color}.
+            legend_location (str, optional): Location of the legend. Options are 'upper right', 'upper left', 'lower right', 'lower left'. Default is 'upper right'.
 
         Returns:
             None
         """
         if data is None:
             data, _ = self.ctf.get_data()
 
@@ -92,32 +96,41 @@
             else:
                 rotation_matrix = np.array([[np.cos(theta), np.sin(theta)], [-np.sin(theta), np.cos(theta)]])
             xy = np.column_stack((data['X'], data['Y']))
             xy_rotated = np.dot(xy, rotation_matrix)
             data['X'], data['Y'] = xy_rotated[:, 0], xy_rotated[:, 1]
         
         # Filter data based on phase
-        df_new = data[data['Phase'].isin([0, 1, 2, 3])]
+        df_new = data
         
         # Define custom colormap for phases
-        phases_colors = {0: 'black', 1: 'green', 2: 'yellow', 3:'blue'}
-        
+        if phase_colors is None:
+            phase_colors = {0: 'black', 1: 'green', 2: 'blue', 3: 'red'}  # Default colors if not specified
+
+        phase_labels = [f'Phase {phase}' for phase in sorted(phase_colors.keys())]
+        phase_color_list = [phase_colors[phase] for phase in df_new['Phase']]
+
         # Plot
         fig, ax = plt.subplots(figsize=(16, 9))  # Adjust the figsize as per your requirement
-        ax.scatter(df_new['X'], df_new['Y'], c=df_new['Phase'].map(phases_colors), s=1)  # Set s=1 for one point per pixel
+        scatter = ax.scatter(df_new['X'], df_new['Y'], c=df_new['Phase'], cmap=cmap, s=1)
         ax.set_xlabel('X')
         ax.set_ylabel('Y')
         ax.set_title('EBSD Map with Color Based on Phase')
         
         ax.set_aspect('equal')  # Set aspect ratio to 'equal' to ensure equal scaling along both axes
 
-        plt.show()
-
+        # Create legend for phase colors
+        handles, _ = scatter.legend_elements()
+        legend = ax.legend(handles, phase_labels, title="Phases", loc=legend_location)
+        ax.add_artist(legend)
 
+        if save_image and image_filename:
+            plt.savefig(image_filename, dpi=dpi)  # Save the plot as an image with user-specified filename and DPI
 
+        plt.show()
 
     def get_index_of_phases(self, phases_list):
         """
         Get the index of phases based on their names.
 
         Parameters:
             phases_list (list): A list of phase names.
@@ -167,23 +180,23 @@
         """
         phases_info_ =  self.ctf.phases_info()[6]
         return phases_info_
     
     def get_euler_angles_by_phase(self, phase):
         """
         Retrieves Euler angles by phase names.
-        Not yet implemented.
 
         Parameters:
             phase (str): Phase name.
 
         Returns:
-            None
+            pandas.dataframe: euler angles of phase by name
         """
-        pass
+        phase_index = self.get_index_of_phases(phase)
+        return self.get_euler_angles(phase_index)
 
     def get_phases_numbers(self):
         """
         Retrieves phase numbers.
 
         Returns:
             list: List containing phase numbers.
@@ -269,19 +282,16 @@
         
         data = [(index, phase, percentage) for index, (phase, percentage) in enumerate(phase_percentages.items())]
         
         headers = ["Index", "Phase", "Percentage"]
 
         self.phases_data = data
         
-        table = tabulate(data, headers=headers, tablefmt="grid")
-        return table
-
+        return data
 
-    
     def filterByPhase(self, phase_list, data=None):
         """
         Filters EBSD data by phase.
 
         Parameters:
             phase_list (list): List of phase names.
             data (pandas.DataFrame, optional): DataFrame containing EBSD data. Defaults to None.
@@ -290,21 +300,34 @@
             pandas.DataFrame: Filtered DataFrame.
         """
         if data is None:
             data = self.ctf.get_data()[0]
         indexes = []
         for phase in phase_list:
             phase_items = list(self.phases())
-            index = phase_items.index(phase)
+            index = next(index for index, mineral, value in phase_items if mineral == phase)
             indexes.append(index)
         for index in indexes:
             data = data[data['Phase'] != index]
         return data
     
     def getAnisotropyForEBSD(self, cij, euler_angles, density, melt=0):
+        """
+        Calculates average density and tensor for EBSD data
+
+        Parameters:
+        cij: array, stiffness tensor of phase
+        euler_angles: list, euler angles of phases in list
+        density: float, density of phases
+        melt: float, fraction of melt available
+
+        Returns:
+        - average_tensor: array, average tensor calculated
+        - density: float, average density
+        """
         if melt:
             tensor = Tensor()
             tensor_list = []
             for voigt in cij:
                 tensor_list.append(tensor.voigt_to_tensor(voigt))
 
             rotated_tensor_list = []
@@ -323,15 +346,15 @@
             density_averaged = (np.sum(np.multiply(density,len_euler)))/(np.sum(len_euler))
 
             tensor_sum = np.sum(rotated_tensor_list, axis=0)
             tensor_sum= tensor_sum/sum(len_euler)
 
             tensor_sum = (1 - melt*0.01)*tensor_sum + melt*0.01*calcMelttensor
 
-            return tensor_sum, len_euler, density_averaged
+            return tensor_sum, density_averaged
 
         tensor = Tensor()
         tensor_list = []
         for voigt in cij:
             tensor_list.append(tensor.voigt_to_tensor(voigt))
             
         tensor = Tensor()
@@ -374,21 +397,26 @@
         Returns:
         quaternion : numpy.ndarray
             Quaternion as [w, x, y, z].
         """
         r = Rotation.from_euler('ZXZ', [phi, phi1, phi2], degrees=True)
         return r.as_quat()
     
-    def calcGrains(self, df, threshold, phase_names, downsampling_factor=20):
+    def calcGrains(self, df, phase_names, threshold = 10, downsampling_factor=20):
         """
-        this is the df from df = ebsdfile.get_ebsd_data(), 
-        threshold will be the threshold angle in degrees, phase_name will be a 
-        list of phases present and that can be obtained from self.phases_names
-        by default threshold is set to 10 degrees, but can be modified as threshold = 20 and
-        so on and so forth
+        Calculated the grains in the ebsd data
+
+        Parameters:
+        - df: EBSD dataframe, this is the df we get from from df = ebsdfile.get_ebsd_data(), 
+        - threshold: float, threshold will be the threshold angle in degrees, threshold mean orientation angle, by default threshold is set to 10 degrees, but can be modified as threshold = 20 and so on and so forth
+        - phase_names: list, phase_name will be a list of phases present and that can be obtained from self.phases_names
+        - downsampling factor: int, specify downsampling factor for faster computation, default is 20
+
+        Returns:
+        - df: EBSD dataframe with grains calculated
         """
         if df is None:
             df = self.get_ebsd_data()
 
         if phase_names is None:
             phase_names = self.phases_names()['phase'].tolist()
             phase_names.insert(0, "na")
@@ -412,15 +440,22 @@
             print(f"Grain {grain_idx}: Dominant Phase - {phase_names[dominant_phase]}, Size - {len(group)}")
 
         self.plotGrains(df)
         return df
     
     def filterByGrainSize(self, df, phases_names, min_grain_size = 100):
         """
-        df is the input from calcGrainsdf, with grain column appended
+        Filters ebsd by grain size
+
+        Parameters:
+        - df: EBSD dataframe, which is the input from calcGrainsdf, with grain column appended
+        - min_grain_size: int, desired minimum grain size, default is 100
+
+        Returns:
+        - df_filtered: Filtered EBSD dataframe
         """
 
         if df is None:
             df = self.calcGrains()
 
         if phases_names == None:
             phases_names = self.phases_names()['phase'].tolist()
@@ -438,40 +473,80 @@
             dominant_phase = phase_counts.idxmax()
             print(f"Grain {grain_idx}: Dominant Phase - {phases_names[dominant_phase]}, Size - {len(group)}")
 
         self.plotGrains(df_filtered)
 
         return df_filtered
     
-    def plotGrains(self, df):
-        fig = px.scatter(df, x='X', y='Y', color='Phase', color_continuous_scale='viridis')
+    def plotGrains(self, df, color_continuous_scale='viridis', save_name=None, dpi=None):
+        """
+        Create a 2D scatter plot with phase coloring.
 
-        # Customize marker size (2 pixel here)
-        fig.update_traces(marker=dict(size=2))
+        Parameters:
+        - df (DataFrame): The EBSD DataFrame containing the data to plot.
+        - color_continuous_scale (str): The color scale to use for continuous colors, default is viridis.
+        - save_name (str): The name to use when saving the figure as a PNG file. If None, the figure will be displayed but not saved.
+        - dpi (int): The DPI (dots per inch) to use when saving the figure. If None, the default DPI will be used.
 
-        # Customize the layout
+        Returns:
+        - None
+        """
+        fig = px.scatter(df, x='X', y='Y', color='Phase', color_continuous_scale=color_continuous_scale)
+        fig.update_traces(marker=dict(size=2))
         fig.update_layout(
             title="2D Scatter Plot with Phase",
             xaxis_title="X",
             yaxis_title="Y",
             coloraxis_colorbar_title="Phase",
             showlegend=True
         )
-
-        fig.show()
+        if save_name:
+            if not save_name.endswith('.png'):
+                save_name += '.png'  # Ensure the file has a .png extension
+            if dpi:
+                fig.write_image(save_name, format='png', scale=dpi)
+            else:
+                fig.write_image(save_name, format='png')
+            print(f"Figure saved as {os.path.abspath(save_name)}")
+        else:
+            fig.show()
 
     def rotateEBSD(self, ebsd_df, angles, keepXY = True):
 
+        """
+        Rotate EBSD with a certain angles
+
+        Parameters:
+        - ebsd_df: ebsd pandas dataframe
+        - angles: angles to be rotated (phi1, phi2, phi3), eg: [20, 30, 40]
+        - keepXY: bool, Specify if you want to keep X and Y constant. Default is True
+
+        Returns:
+        - Rotated EBSD dataframe 
+        
+        """
+
         if keepXY == False:
             return apply_custom_rotation_to_dataframe_noxy(ebsd_df, angles)
         else:
             return apply_custom_rotation_to_dataframe(ebsd_df, angles)
     
 
     def plot_rotate_ebsd(self, sample_ref = ["x2east", "zOutOfPlane"], ebsd_df = None, keepXY = False):
+        """
+        Plots the rotated ebsd and returns the rotated ebsd dataframe
+
+        Parameters:
+        - sample_ref: sample reference, eg: ["x2east", "zOutOfPlane"], ["x2west", "zOutOfPlane"], ["x2north", "zOutOfPlane"], ["x2south", "zOutOfPlane"], ["x2east", "zIntoPlane"], default is ["x2east", "zOutOfPlane"]
+        - ebsd_df: the ebsd pandas dataframe
+        - keepXY: bool, Specify if you want to keep X and Y constant. Default is False
+
+        Returns:
+        - rotated_ebsd_df : rotated ebsd dataframe
+        """
         if ebsd_df is None:
             ebsd_df = self.get_ebsd_data()
 
         if sample_ref == ["x2east", "zOutOfPlane"]:
             angle = (0, 0, 0)
 
         if sample_ref == ["x2west", "zOutOfPlane"]:
@@ -499,24 +574,44 @@
             rotated_ebsd_df = apply_custom_rotation_to_dataframe_noxy(ebsd_df, angle)
         else:
             rotated_ebsd_df = apply_custom_rotation_to_dataframe(ebsd_df, angle)
 
         return rotated_ebsd_df
     
     def filterMAD(self, df, value=0.7):
+        """
+        Filters the ebsd dataframe with MAD greater than a certain threshold
+
+        Parameters:
+        - df: pandas EBSD dataframe
+        - value: value of the threshold for MAD (default is 0.7)
+
+        Returns:
+        - df: EBSD filtered dataframe
+        """
         return df[df['MAD']<value]
     
+    def filterByPhaseNumberList(self, df, phase_list):
+        """
+        Filters the EBSD dataframe given a list of phases
+        """
+        if df is None:
+            df = self.ctf.get_data()[0]
+
+        df_filtered = df[~df['Phase'].isin(phase_list)]
+        return df_filtered
+    
     def odf(self, df, phase=1, crystal_symmetry='D2', random_val=True, miller=[1, 0, 0], hemisphere = 'both', 
             axes_labels=["Xs", "Ys"], alpha = 0.01, figure = None, vector_labels = None, reproject=False, show_hemisphere_label = None,
             grid = None, grid_resolution = None, return_figure = None):
         """
             Calculate the Orientation Distribution Function (ODF) for a given EBSD dataset and optionally visualize it.
 
             Parameters:
-            - df: pandas DataFrame
+            - df: pandas EBSD DataFrame
                 The DataFrame containing EBSD (Electron Backscatter Diffraction) data.
             - phase: int, optional
                 The phase number for which ODF needs to be calculated (default is 1).
             - crystal_symmetry: str, optional
                 The crystal symmetry of the material, e.g., 'D2' for cubic symmetry (default is 'D2').
             - random_val: bool, optional
                 If True, randomly generate orientation values for incomplete data (default is True).
@@ -555,13 +650,92 @@
             - figure: matplotlib Figure or None
                 If return_figure is True, the Figure object containing the ODF plot; otherwise, None.
             """
         odf(df=df, phase=phase, crystal_symmetry=crystal_symmetry, random_val=random_val, miller=miller, hemisphere = hemisphere, 
             axes_labels=axes_labels, alpha = alpha, figure = figure, vector_labels = vector_labels, reproject=reproject, show_hemisphere_label = show_hemisphere_label,
             grid = grid, grid_resolution = grid_resolution, return_figure = return_figure)
 
-    def pdf(self, ebsd_df):
-        pdf(df = ebsd_df)
+    def pdf(self, df, phase=1, crystal_symmetry='D2', random_val=True, miller=[0, 1, 0], hemisphere = 'both', sigma = 4,
+        axes_labels=["Xs", "Ys"], figure = None, show_hemisphere_label = None,
+        grid = None, grid_resolution = None, return_figure = None, log = False, colorbar=True, weights = None):
+
+        """
+            Calculate the Orientation Distribution Function (ODF) for a given EBSD dataset and optionally visualize it.
+
+            Parameters:
+            - df: pandas DataFrame
+                The DataFrame containing EBSD (Electron Backscatter Diffraction) data.
+            - phase: int, optional
+                The phase number for which ODF needs to be calculated (default is 1).
+            - crystal_symmetry: str, optional
+                The crystal symmetry of the material, e.g., 'D2' for cubic symmetry (default is 'D2').
+            - random_val: bool, optional
+                If True, randomly generate orientation values for incomplete data (default is True).
+            - miller: list of int, optional
+                The Miller indices representing the crystallographic plane to calculate ODF for (default is [1, 0, 0]).
+            - projection: str, optional
+                The type of projection to use for visualization (default is 'stereographic').
+            - figure: matplotlib Figure or None, optional
+                If provided, the ODF plot will be added to this Figure; otherwise, a new Figure will be created.
+            - axes_labels: list of str or None, optional
+                Labels for the X and Y axes of the ODF plot (default is None).
+            - vector_labels: list of str or None, optional
+                Labels for the vectors in the ODF plot (default is None, which results in auto-generated labels).
+            - hemisphere: str, upper or lower or both, optional
+                Specify the hemisphere for ODF calculation and visualization (default is None).
+            - reproject: bool, optional
+                If True, reproject data into a specified coordinate system (default is False).
+            - show_hemisphere_label: bool or None, optional
+                Specify whether to show the hemisphere label on the plot (default is None).
+            - grid: bool or None, optional
+                Specify whether to display a grid on the ODF plot (default is None).
+            - grid_resolution: tuple of float or None, optional
+                Resolution of the grid (default is None).
+            - figure_kwargs: dict or None, optional
+                Additional keyword arguments for configuring the matplotlib Figure (default is None).
+            - reproject_scatter_kwargs: dict or None, optional
+                Additional keyword arguments for configuring scatter plot during reprojection (default is None).
+            - text_kwargs: dict or None, optional
+                Additional keyword arguments for configuring text elements in the plot (default is None).
+            - return_figure: bool, optional
+                If True, return the matplotlib Figure object along with the ODF data (default is False).
+
+            Returns:
+            - odf_result: pandas DataFrame
+                DataFrame containing the calculated Orientation Distribution Function (ODF) values.
+            - figure: matplotlib Figure or None
+                If return_figure is True, the Figure object containing the ODF plot; otherwise, None.
+            """
+
+        pdf(df = df, phase=phase, crystal_symmetry=crystal_symmetry, random_val=random_val, miller=miller, sigma=sigma, hemisphere=hemisphere, axes_labels=axes_labels, figure = figure, show_hemisphere_label = show_hemisphere_label,
+        grid = grid, grid_resolution = grid_resolution, return_figure = return_figure, log = log, colorbar=colorbar, weights = weights)
+
+    def ipf(self, df, phase=1, vector_sample=[0, 0, 1], random_val=True,
+            vector_title='Z', projection='ipf', crystal_symmetry='D2'):
+        
+        """
+            Generate and visualize an Inverse Pole Figure (IPF) from EBSD data.
+
+            Parameters:
+            - df: pandas DataFrame
+                The DataFrame containing EBSD (Electron Backscatter Diffraction) data.
+            - phase: int, optional
+                The phase number for which IPF needs to be generated (default is 1).
+            - vector_sample: list of int, optional
+                The sample vector used for IPF generation (default is [0, 0, 1]).
+            - random_val: bool, optional
+                If True, randomly select orientation values for IPF generation (default is True).
+            - vector_title: str, optional
+                The title for the vector used in IPF visualization (default is 'Z').
+            - projection: str, optional
+                The type of projection for IPF visualization (default is 'ipf').
+            - crystal_symmetry: str, optional
+                The crystal symmetry of the material (default is 'D2').
+
+            Returns:
+            - fig: matplotlib Figure
+                The generated matplotlib Figure object containing the IPF visualization.
+        """
 
-    def ipf(self, ebsd_df):
-        self.pdf(ebsd_df=ebsd_df)
-        ipf(df = ebsd_df)
+        self.pdf(df = df, phase=phase, random_val=random_val, crystal_symmetry=crystal_symmetry)
+        ipf(df = df, phase=phase, vector_sample=vector_sample, random_val=random_val,
+            vector_title=vector_title, projection=projection, crystal_symmetry=crystal_symmetry)
```

### Comparing `santex-1.0/santex/ebsd/ebsdrotation.py` & `santex-1.1/santex/ebsd/rotateEBSD.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 from scipy.spatial.transform import Rotation
 from joblib import Parallel, delayed
-import pandas as pd
 from tqdm import tqdm
 
 def bunge_euler_rotation(phi1, Phi, phi2, angles):
     """
     Calculates the resultant Bunge Euler angles after applying a custom rotation.
 
     Args:
@@ -38,15 +37,56 @@
     # Keep the angles in the range [0, 360)
     phi1_res = (phi1_res + 360) % 360
     Phi_res = (Phi_res + 360) % 360
     phi2_res = (phi2_res + 360) % 360
 
     return phi1_res, Phi_res, phi2_res
 
-def apply_custom_rotation_to_dataframe(df, angles):
+def apply_custom_rotation_to_dataframe(euler_df, angles):
+    """
+    Applies a custom rotation to each row of a DataFrame containing Bunge Euler angles.
+
+    Args:
+        euler_df (pd.DataFrame): DataFrame containing Bunge Euler angles.
+        angles (tuple): Custom rotation angles in degrees (alpha, beta, gamma).
+
+    Returns:
+        pd.DataFrame: DataFrame with updated Bunge Euler angles after rotation.
+    """
+    def bunge_euler_rotation_parallel(row):
+        """
+        Calculates the resultant Bunge Euler angles after applying a custom rotation in parallel.
+
+        Args:
+            row (pd.Series): Row of DataFrame containing Euler angles.
+
+        Returns:
+            tuple: Resultant Bunge Euler angles (phi1, Phi, phi2) in degrees in the range [0, 360).
+        """
+        # Extract Euler angles from the row
+        phi1, Phi, phi2 = row['Euler1'], row['Euler2'], row['Euler3']
+        
+        # Call the original rotation function
+        return bunge_euler_rotation(phi1, Phi, phi2, angles)
+
+    # Calculate the number of iterations
+    num_iterations = len(euler_df)
+
+    # Parallelize the process and show progress in percent
+    results = Parallel(n_jobs=-1)(
+        delayed(bunge_euler_rotation_parallel)(row)
+        for _, row in tqdm(euler_df.iterrows(), total=num_iterations)
+    )
+
+    # Update the DataFrame with the new Euler angles
+    euler_df[['Euler1', 'Euler2', 'Euler3']] = results
+
+    return euler_df
+
+def apply_custom_rotation_to_dataframe_noxy(df, angles):
     """
     Applies a custom rotation to each row of a DataFrame containing Bunge Euler angles, X, and Y coordinates.
 
     Args:
         df (pd.DataFrame): DataFrame containing Bunge Euler angles, X, and Y coordinates.
         angles (tuple): Custom rotation angles in degrees (alpha, beta, gamma).
 
@@ -85,45 +125,7 @@
         for _, row in tqdm(df.iterrows(), total=num_iterations)
     )
 
     # Update the DataFrame with the new Euler angles, X, and Y coordinates
     df[['Euler1', 'Euler2', 'Euler3', 'X', 'Y']] = results
 
     return df
-
-import matplotlib.pyplot as plt
-
-def plot(data=None, rotation_angle=0, inside_plane=True):
-    """
-    Plots the EBSD map with colors based on phase.
-
-    Parameters:
-        data (pandas.DataFrame, optional): DataFrame containing EBSD data. If not provided, uses stored data.
-        rotation_angle (int, optional): Angle by which to rotate the EBSD data (in degrees). Default is 0.
-        inside_plane (bool, optional): If True, rotates the EBSD data inside the plane. If False, rotates outside the plane. Default is True.
-
-    Returns:
-        None
-    """
-    if data is None:
-        data, _ = self.ctf.get_data()
-    
-    # Rotate EBSD data
-    if rotation_angle != 0:
-        theta = np.radians(rotation_angle)
-        if inside_plane:
-            rotation_matrix = np.array([[np.cos(theta), -np.sin(theta)], [np.sin(theta), np.cos(theta)]])
-        else:
-            rotation_matrix = np.array([[np.cos(theta), np.sin(theta)], [-np.sin(theta), np.cos(theta)]])
-        xy = np.column_stack((data['X'], data['Y']))
-        xy_rotated = np.dot(xy, rotation_matrix)
-        data['X'], data['Y'] = xy_rotated[:, 0], xy_rotated[:, 1]
-    
-    # Filter data based on phase
-    df_new = data[data['Phase'].isin([0, 1, 2])]
-    
-    # Plot
-    plt.scatter(df_new['X'], df_new['Y'], c=df_new['Phase'], cmap='viridis')
-    plt.xlabel('X')
-    plt.ylabel('Y')
-    plt.title('EBSD Map with Color Based on Phase')
-    plt.show()
```

### Comparing `santex-1.0/santex/ebsd/melt.py` & `santex-1.1/santex/ebsd/melt_tensor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 import numpy as np
 from ..tensor.tensor import Tensor
 
 
 def calcMelttensor():
-    """Reference 
+    """
+    Returns the melt stiffness tensor.
+    
+    Parameters: 
+    - None
+    
+    Returns:
+    - np.ndarray - melt stifness tensor
+    
+    Reference 
     Lee, A. L., Walker, A. M., Lloyd, G. E., & Torvela, T. (2017). 
     Modeling the impact of melt on seismic properties during mountain building. 
     Geochemistry, Geophysics, Geosystems, 18(3), 1090–1110. https://doi.org/10.1002/2016GC006705
     """
     voigt_melt = np.array([[16.1,   15.967,  15.967,   0.,      0,   0.   ],
                                 [ 15.967, 16.1,   15.967,    0.,      0,   0.   ],
                                 [ 15.967,  15.967,  16.1,    0.,     0,    0.   ],
```

### Comparing `santex-1.0/santex/ebsd/odf.py` & `santex-1.1/santex/ebsd/odf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.stats import gaussian_kde
 
 from orix.crystal_map import Phase
 from orix.quaternion import Orientation, symmetry
 from orix.vector import Miller, Vector3d
-
-import numpy as np
+import plotly.graph_objects as go
 
 import random
 
 def odf(df, phase=1, crystal_symmetry='D2', random_val=True, miller=[1, 0, 0], hemisphere = 'both', 
         axes_labels=["Xs", "Ys"], alpha = 0.01, figure = None, vector_labels = None, reproject=False, show_hemisphere_label = None,
         grid = None, grid_resolution = None, return_figure = None):
     """
@@ -208,15 +207,16 @@
 
     uvw_ = uvw_.symmetrise(unique=False)
 
     uvw_ = uvw_.reshape(1, uvw_.size)
     orientations = orientations.reshape(*orientations.shape, 1)
     r_ = ~orientations * uvw_
 
-    r_.scatter(hemisphere=hemisphere, axes_labels=axes_labels, alpha = alpha)
+    r_.scatter(hemisphere=hemisphere, axes_labels=axes_labels, alpha = alpha, figure = figure, vector_labels = vector_labels, reproject=reproject, show_hemisphere_label = show_hemisphere_label,
+        grid = grid, grid_resolution = grid_resolution, return_figure = return_figure)
     return r_
 
 def ipf(df, phase=1, vector_sample=[0, 0, 1], random_val=True,
             vector_title='Z', projection='ipf', crystal_symmetry='D2'):
     """
     Generate and visualize an Inverse Pole Figure (IPF) from EBSD data.
 
@@ -388,55 +388,50 @@
         orientations = Orientation.from_euler(np.deg2rad(euler_values), symmetry.Td)
         symmetry_ =symmetry.Td
     elif crystal_symmetry in ["cubic", "Oh", "m-3m", "m-3m", "432"]:
         orientations = Orientation.from_euler(np.deg2rad(euler_values), symmetry.Oh)
         symmetry_ =symmetry.Oh
 
     orientations = orientations.reshape(*orientations.shape, 1)
-    print(orientations)
+    # print(orientations)
     vec_sample = Vector3d(vector_sample)
-    print(vec_sample)
+    # print(vec_sample)
     vec_crystal = orientations * vec_sample
     subplot_kw = dict(projection=projection, symmetry=symmetry_)
     fig = plt.figure(figsize=(9, 8))
 
     ax0 = fig.add_subplot(221, direction=vec_sample, **subplot_kw)
     ax0.scatter(orientations, alpha=0.05)
     _ = ax0.set_title(f"Phase{phase}, {vector_title}")
 
     ax2 = fig.add_subplot(223, direction=vec_sample, **subplot_kw)
     ax2.pole_density_function(vec_crystal)
     _ = ax2.set_title(f"Phase{phase}, {vector_title}")
 
 
 def pdf(df, phase=1, crystal_symmetry='D2', random_val=True, miller=[0, 1, 0], hemisphere = 'both', sigma = 4,
-        axes_labels=["Xs", "Ys"], alpha = 0.01, figure = None, vector_labels = None, reproject=False, show_hemisphere_label = None,
-        grid = None, grid_resolution = None, return_figure = None):
+        axes_labels=["Xs", "Ys"], figure = None, show_hemisphere_label = None,
+        grid = None, grid_resolution = None, return_figure = None, log = False, colorbar=True, weights = None):
+    
     """
         Calculate the Orientation Distribution Function (ODF) for a given EBSD dataset and optionally visualize it.
 
         Parameters:
         - df: pandas DataFrame
             The DataFrame containing EBSD (Electron Backscatter Diffraction) data.
         - phase: int, optional
             The phase number for which ODF needs to be calculated (default is 1).
         - crystal_symmetry: str, optional
             The crystal symmetry of the material, e.g., 'D2' for cubic symmetry (default is 'D2').
         - random_val: bool, optional
             If True, randomly generate orientation values for incomplete data (default is True).
         - miller: list of int, optional
             The Miller indices representing the crystallographic plane to calculate ODF for (default is [1, 0, 0]).
-        - projection: str, optional
-            The type of projection to use for visualization (default is 'stereographic').
-        - figure: matplotlib Figure or None, optional
-            If provided, the ODF plot will be added to this Figure; otherwise, a new Figure will be created.
         - axes_labels: list of str or None, optional
             Labels for the X and Y axes of the ODF plot (default is None).
-        - vector_labels: list of str or None, optional
-            Labels for the vectors in the ODF plot (default is None, which results in auto-generated labels).
         - hemisphere: str, upper or lower or both, optional
             Specify the hemisphere for ODF calculation and visualization (default is None).
         - reproject: bool, optional
             If True, reproject data into a specified coordinate system (default is False).
         - show_hemisphere_label: bool or None, optional
             Specify whether to show the hemisphere label on the plot (default is None).
         - grid: bool or None, optional
@@ -605,15 +600,17 @@
         uvw_ = Miller(uvw = miller, phase=Phase(point_group=symmetry.Oh))
 
     uvw_ = uvw_.symmetrise(unique=False)
 
     uvw_ = uvw_.reshape(1, uvw_.size)
     orientations = orientations.reshape(*orientations.shape, 1)
     r_ = ~orientations * uvw_
-    r_.pole_density_function(sigma=sigma, hemisphere=hemisphere)
+    r_.pole_density_function(sigma=sigma, hemisphere=hemisphere, axes_labels=axes_labels, figure = figure, show_hemisphere_label = show_hemisphere_label,
+        grid = grid, grid_resolution = grid_resolution, return_figure = return_figure, log = log, colorbar=colorbar, weights = weights)
+
 
 def calculate_odf(euler_angles):
     """
     Calculate and plot an ODF from Bunge Euler angles.
     
     Parameters:
     - euler_angles: A Nx3 numpy array of Euler angles (phi1, Phi, phi2) in degrees.
@@ -635,17 +632,14 @@
     ax.set_xlabel('Phi1')
     ax.set_ylabel('Phi')
     ax.set_zlabel('Phi2')
     ax.set_title('ODF Representation')
     plt.show()
 
 
-import plotly.graph_objects as go
-import numpy as np
-
 def plot_orientations_3d(euler_angles):
 
     phi1, Phi, phi2 = euler_angles[:, 0], euler_angles[:, 1], euler_angles[:, 2]
     
     fig = go.Figure(data=[go.Scatter3d(
         x=phi1,
         y=Phi,
```

### Comparing `santex-1.0/santex/ebsd/saveEBSD.py` & `santex-1.1/santex/ebsd/saveEBSD.py`

 * *Files identical despite different names*

### Comparing `santex-1.0/santex/isotropy/data/materials.json` & `santex-1.1/santex/isotropy/data/materials.json`

 * *Files identical despite different names*

### Comparing `santex-1.0/santex/isotropy/isotropy.py` & `santex-1.1/santex/isotropy/isotropy.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,33 +3,55 @@
 import numpy as np
 from scipy.optimize import root_scalar
 import json
 import os
 
 class Isotropy:
     def __init__(self):
+        """
+        Initializes the Isotropy class by loading material data from a JSON file.
+
+        Raises:
+        FileNotFoundError: If the JSON file 'materials.json' is not found.
+        json.JSONDecodeError: If there is an error decoding the JSON file.
+        """
         try:
             json_file = 'materials.json'
             json_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data', json_file)
             with open(json_path, 'r') as f:
                 self.data = json.load(f)
         except (FileNotFoundError, json.JSONDecodeError) as e:
             raise FileNotFoundError(f"Error loading JSON file '{json_file}': {e}")
 
     def get_available_phases(self):
+        """
+        Prints and returns a list of available phases from the loaded material data.
+
+        Returns:
+        List: A list of available phases.
+        """
         try:
             for key in range(0,len(self.data)):
                 print('######################Available Phases######################')
                 print('Material id: ' + str(self.data[str(key)]['phase'] + '       ' + 'Material name: ' + str(self.data[str(key)]['name'])))
             return [self.data[key]['phase'] for key in self.data]
         except (KeyError, TypeError) as e:
             print(f"Error accessing data: {e}")
             return []
 
     def get_phase_constants(self, phase):
+        """
+        Retrieves phase constants for a given phase name or ID from the loaded material data.
+
+        Parameters:
+        phase (str): The name or ID of the phase.
+
+        Returns:
+        dict: Phase constants including ID, name, density, expansivity, bulk modulus, shear modulus, and more.
+        """
         try:
             phase_data = next(item for item in self.data.values() if item.get('phase') == phase or item.get('name') == phase)
             if phase_data:
                 return {
                     'id': phase_data['phase'],
                     'name': phase_data['name'],
                     'rho0': phase_data['density_298K(kg/m3)'],
@@ -160,52 +182,74 @@
                 else:
                     return density, aks, amu
         else:
             raise ValueError(f"No phase constants available for '{phase}'.")
 
 
     def calculate_velocities(self, density, aks, amu):
+        """
+        Calculates velocities (vp, vs, vbulk) based on density, adiabatic bulk modulus (aks), and shear modulus (amu).
+
+        Parameters:
+        density (float or array): Density in kg/m^3.
+        aks (float or array): Adiabatic bulk modulus in Pa.
+        amu (float or array): Shear modulus in Pa.
+
+        Returns:
+        Tuple: Velocities vp, vs, vbulk in km/s.
+        """
         try:
             vbulk = 0.001 * np.sqrt(aks / density)
             vp = 0.001 * np.sqrt((aks + 1.3333 * amu) / density)
             vs = 0.001 * np.sqrt(amu / density)
             return vbulk, vp, vs
         except (ZeroDivisionError, ValueError) as e:
             print(f"Error calculating velocities: {e}")
 
     def pressure_function(self, f, press, akk, akk_prime):
+        """
+        Helper function for pressure calculation in calculate_seismic_properties method.
+
+        Parameters:
+        f (float): Pressure factor.
+        press (float): Pressure in Pa.
+        akk (float): Adiabatic bulk modulus in Pa.
+        akk_prime (float): Derivative of bulk modulus with respect to pressure.
+
+        Returns:
+        float: Pressure difference.
+        """
         try:
             zeta = 0.75 * (4. - akk_prime)
             f1 = (1. + 2. * f) ** 2.5
             f2 = (1. - 2. * zeta * f)
             pdif = 3. * akk * f * f1 * f2 - press
             return pdif
         except ZeroDivisionError as e:
             print(f"Error in pressure function: {e}")
             
     def HashinShtrikmanBounds(self, phase_constant_list, fraction_list, temperature, pressure, fractions_matches_T = False):
     
         """
         Calculates Hashin-Shtrikman Bounds for the given parameters:
         
-        Inputs:
-        phase_constant_list: list of phase constant instances gotten from set_modal_composition function.
-        fraction_list: list of fractions of each phase.
-        temperature: temperature array or scalar in Kelvin
-        pressure: pressure array or scalar in GPa
-        
-        Outputs:
-        3 lists of medium value, upper bound and lower bound, indexed respectively: 
-        [Vbulk_medium,Vp_medium,Vs_medium], [Vbulk_upper,Vp_upper,Vs_upper], [Vbulk_lower, Vp_lower, Vs_lower]
+        Parameters:
+        - phase_constant_list: list of phase constant instances gotten from set_modal_composition function.
+        - fraction_list: list of fractions of each phase.
+        - temperature: temperature array or scalar in Kelvin
+        - pressure: pressure array or scalar in GPa
+        
+        Returns:
+        - 3 lists of medium value, upper bound and lower bound, indexed respectively: 
+            [Vbulk_medium,Vp_medium,Vs_medium], [Vbulk_upper,Vp_upper,Vs_upper], [Vbulk_lower, Vp_lower, Vs_lower]
         
         """
         aks_list = []
         amu_list = []
         
-        
         if isinstance(temperature,(int,float)):
             if isinstance(pressure,(int,float)):
                 method_calc = 'scalar'
             else:
                 raise ValueError('While temperature is a scalar, pressure is an array.')
         else:
             if len(temperature) != len(pressure):
@@ -288,23 +332,30 @@
         Vbulk_lower, Vp_lower, Vs_lower = self.calculate_velocities(density = density_mix, aks = khsm ,amu = mhsm)
         
         return [Vbulk_medium,Vp_medium,Vs_medium], [Vbulk_upper,Vp_upper,Vs_upper], [Vbulk_lower, Vp_lower, Vs_lower]
         
     def set_modal_composition(self, phase_list, fraction_list):
         
         """
+        Prepares the input for HashinShtrikmanBounds method for the entered phase_list
+        and fraction_list.
         
-        Inputs:
-        
-        phase_list - list of phase ids to be included in the rock. 
-        Example: ['fo', 'en'] -- Forsterite and Enstatite
+        Parameters:        
+        - phase_list - list of phase ids to be included in the rock. 
+            Example: ['fo', 'en'] -- Forsterite and Enstatite
         
-        fraction_list - list of fraction lists to be included in the rock
-        Example: [0.8, 0.2] -- 0.8 fo and 0.2 en
+        - fraction_list - list of fraction lists to be included in the rock
+            Example: [0.8, 0.2] -- 0.8 fo and 0.2 en
+            
+        Returns:
         
+        - phase_constant_list: 
+            list containing the phase constats that can be inputted into HashinShtrikmanBounds method.
+        - fraction_list: 
+            np.ndarray list of fractions of entered minerals.
         """
         
         if type(fraction_list) != np.ndarray:
             fraction_list = np.array(fraction_list)
             
         all_sums = np.allclose(fraction_list.sum(axis = 1), 1.0, atol = 1e-6)
```

### Comparing `santex-1.0/santex/material/data/derivatives_P.json` & `santex-1.1/santex/material/data/materials_database.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9710851202079271%*

 * *Differences: {'0': "{'C11': 306.7, 'C22': 306.7, 'C33': 306.7, 'C44': 94.9, 'C55': 94.9, 'C66': 94.9, 'C12': "*

 * *      "106.7, 'C13': 111.9, 'C23': 111.9}",*

 * * '1': "{'C11': 314.5, 'C22': 314.5, 'C33': 314.5, 'C44': 99.7, 'C55': 99.7, 'C66': 99.7, 'C12': "*

 * *      "95.6, 'C13': 95.6, 'C23': 95.6}",*

 * * '12': "{'C11': 320.5, 'C22': 196.5, 'C33': 233.5, 'C44': 64.0, 'C55': 77.0, 'C66': 78.7, 'C12': "*

 * *       "68.1, 'C13': 71.6, 'C23': 76.8}",*

 * * '13': "{'C11': 273.0, 'C22': 174.0, 'C33': 236.0, 'C44': 34.4, 'C55': 48.0, 'C66': 60.0,  […]*

```diff
@@ -1,117 +1,117 @@
 [
     {
-        "C11": 6.29,
-        "C12": 3.32,
-        "C13": 3.32,
+        "C11": 306.7,
+        "C12": 106.7,
+        "C13": 111.9,
         "C14": 0,
         "C15": 0,
         "C16": 0,
-        "C22": 6.29,
-        "C23": 3.32,
+        "C22": 306.7,
+        "C23": 111.9,
         "C24": 0,
         "C25": 0,
         "C26": 0,
-        "C33": 6.29,
+        "C33": 306.7,
         "C34": 0,
         "C35": 0,
         "C36": 0,
-        "C44": 1.84,
+        "C44": 94.9,
         "C45": 0,
         "C46": 0,
-        "C55": 1.84,
+        "C55": 94.9,
         "C56": 0,
-        "C66": 1.84,
+        "C66": 94.9,
         "Crystal Reference Frame": "X||a Y||b Z||c",
         "Crystal System": "Cubic",
         "Density(g/cm3)": 4.131,
         "Phase": "Almandine-pyrope",
         "Primary Phase": "Garnet",
         "Study": "Babuska et al. [1978]"
     },
     {
-        "C11": 6.29,
-        "C12": 3.32,
-        "C13": 3.32,
+        "C11": 314.5,
+        "C12": 95.6,
+        "C13": 95.6,
         "C14": 0,
         "C15": 0,
         "C16": 0,
-        "C22": 6.29,
-        "C23": 3.32,
+        "C22": 314.5,
+        "C23": 95.6,
         "C24": 0,
         "C25": 0,
         "C26": 0,
-        "C33": 6.29,
+        "C33": 314.5,
         "C34": 0,
         "C35": 0,
         "C36": 0,
-        "C44": 1.84,
+        "C44": 99.7,
         "C45": 0,
         "C46": 0,
-        "C55": 1.84,
+        "C55": 99.7,
         "C56": 0,
-        "C66": 1.84,
+        "C66": 99.7,
         "Crystal Reference Frame": "X||a Y||b Z||c",
         "Crystal System": "Cubic",
         "Density(g/cm3)": 3.605,
         "Phase": "Grossular",
         "Primary Phase": "Garnet",
         "Study": "Jiang et al. [2004]"
     },
     {
-        "C11": 6.29,
-        "C12": 3.32,
-        "C13": 3.32,
+        "C11": 286.4,
+        "C12": 83.0,
+        "C13": 104.9,
         "C14": 0,
         "C15": 0,
-        "C16": 0,
-        "C22": 6.29,
-        "C23": 3.32,
+        "C16": 1.4,
+        "C22": 286.4,
+        "C23": 104.9,
         "C24": 0,
         "C25": 0,
-        "C26": 0,
-        "C33": 6.29,
+        "C26": -1.4,
+        "C33": 280.1,
         "C34": 0,
         "C35": 0,
         "C36": 0,
-        "C44": 1.84,
+        "C44": 85.0,
         "C45": 0,
         "C46": 0,
-        "C55": 1.84,
+        "C55": 85.0,
         "C56": 0,
-        "C66": 1.84,
+        "C66": 93.2,
         "Crystal Reference Frame": "X||a Y||b Z||c",
         "Crystal System": "Cubic",
         "Density(g/cm3)": 3.522,
         "Phase": "Majorite",
         "Primary Phase": "Garnet",
         "Study": "Pacalo and Weidner [1997]"
     },
     {
-        "C11": 6.29,
-        "C12": 3.32,
-        "C13": 3.32,
+        "C11": 299.1,
+        "C12": 106.7,
+        "C13": 106.7,
         "C14": 0,
         "C15": 0,
         "C16": 0,
-        "C22": 6.29,
-        "C23": 3.32,
+        "C22": 299.1,
+        "C23": 106.7,
         "C24": 0,
         "C25": 0,
         "C26": 0,
-        "C33": 6.29,
+        "C33": 299.1,
         "C34": 0,
         "C35": 0,
         "C36": 0,
-        "C44": 1.84,
+        "C44": 93.7,
         "C45": 0,
         "C46": 0,
-        "C55": 1.84,
+        "C55": 93.7,
         "C56": 0,
-        "C66": 1.84,
+        "C66": 93.7,
         "Crystal Reference Frame": "X||a Y||b Z||c",
         "Crystal System": "Cubic",
         "Density(g/cm3)": 3.565,
         "Phase": "Pyrope",
         "Primary Phase": "Garnet",
         "Study": "Chai et al. [1997b]"
     },
@@ -344,99 +344,99 @@
         "Crystal System": "Hexagonal/ Trigonal",
         "Density(g/cm3)": 2.712,
         "Phase": "Calcite_2",
         "Primary Phase": "Calcite",
         "Study": "Chen et al. [2001]"
     },
     {
-        "C11": 8.47,
-        "C12": 4.67,
-        "C13": 4.84,
+        "C11": 320.5,
+        "C12": 68.1,
+        "C13": 71.6,
         "C14": 0,
         "C15": 0,
         "C16": 0,
-        "C22": 6.56,
-        "C23": 4.11,
+        "C22": 196.5,
+        "C23": 76.8,
         "C24": 0,
         "C25": 0,
         "C26": 0,
-        "C33": 6.37,
+        "C33": 233.5,
         "C34": 0,
         "C35": 0,
         "C36": 0,
-        "C44": 2.12,
+        "C44": 64.0,
         "C45": 0,
         "C46": 0,
-        "C55": 1.66,
+        "C55": 77.0,
         "C56": 0,
-        "C66": 2.37,
+        "C66": 78.7,
         "Crystal Reference Frame": "X||a Y||b Z||c",
         "Crystal System": "Orthorhombic",
         "Density(g/cm3)": 3.355,
         "Phase": "Forsterite",
         "Primary Phase": "Olivine",
         "Study": "Abramson et al. [1997]"
     },
     {
-        "C11": 7.4,
-        "C12": 4.1,
-        "C13": 3.9,
+        "C11": 273.0,
+        "C12": 104.0,
+        "C13": 97.0,
         "C14": 0,
         "C15": 0,
         "C16": 0,
-        "C22": 5.8,
-        "C23": 3.7,
+        "C22": 174.0,
+        "C23": 97.0,
         "C24": 0,
         "C25": 0,
         "C26": 0,
-        "C33": 6.1,
+        "C33": 236.0,
         "C34": 0,
         "C35": 0,
         "C36": 0,
-        "C44": 1.7,
+        "C44": 34.4,
         "C45": 0,
         "C46": 0,
-        "C55": 1.8,
+        "C55": 48.0,
         "C56": 0,
-        "C66": 2.0,
+        "C66": 60.0,
         "Crystal Reference Frame": "X||a Y||b Z||c",
         "Crystal System": "Orthorhombic",
         "Density(g/cm3)": 4.399,
         "Phase": "Fayalite",
         "Primary Phase": "Olivine",
-        "Study": "Abramson et al. [1997];"
+        "Study": "Speziale et al. [2004]"
     },
     {
-        "C11": -0.0617,
-        "C12": 6.31,
-        "C13": 0.95,
+        "C11": 226.0,
+        "C12": 66.0,
+        "C13": 64.0,
         "C14": 0,
         "C15": 0,
         "C16": 0,
-        "C22": 5.7407,
-        "C23": 3.2,
+        "C22": 216.0,
+        "C23": 83.0,
         "C24": 0,
         "C25": 0,
         "C26": 0,
-        "C33": -5.6914,
+        "C33": 262.0,
         "C34": 0,
         "C35": 0,
         "C36": 0,
-        "C44": -0.66,
+        "C44": 64.0,
         "C45": 0,
         "C46": 0,
-        "C55": -1.03,
+        "C55": 59.0,
         "C56": 0,
-        "C66": -0.79,
+        "C66": 18.0,
         "Crystal Reference Frame": "X||a Y||b Z||c",
         "Crystal System": "Orthorhombic",
         "Density(g/cm3)": 3.09,
         "Phase": "Lawsonite",
         "Primary Phase": "Olivine",
-        "Study": "Chantel et al. [2012]"
+        "Study": "Schilling et al. [2003]"
     },
     {
         "C11": 224.7,
         "C12": 72.4,
         "C13": 54.1,
         "C14": 0,
         "C15": 0,
@@ -489,35 +489,35 @@
         "Crystal System": "Orthorhombic",
         "Density(g/cm3)": 3.194,
         "Phase": "Orthoenstatite (MgSiO3)",
         "Primary Phase": "Olivine",
         "Study": "Jackson et al. [1999]"
     },
     {
-        "C11": 11.04,
-        "C12": 6.97,
-        "C13": 9.09,
+        "C11": 236.9,
+        "C12": 79.6,
+        "C13": 63.2,
         "C14": 0,
         "C15": 0,
         "C16": 0,
-        "C22": 9.19,
-        "C23": 8.73,
+        "C22": 180.5,
+        "C23": 56.8,
         "C24": 0,
         "C25": 0,
         "C26": 0,
-        "C33": 16.42,
+        "C33": 230.4,
         "C34": 0,
         "C35": 0,
         "C36": 0,
-        "C44": 2.38,
+        "C44": 84.3,
         "C45": 0,
         "C46": 0,
-        "C55": 2.92,
+        "C55": 79.4,
         "C56": 0,
-        "C66": 2.75,
+        "C66": 80.1,
         "Crystal Reference Frame": "X||a Y||b Z||c",
         "Crystal System": "Orthorhombic",
         "Density(g/cm3)": 3.306,
         "Phase": "Enstatite",
         "Primary Phase": "Olivine",
         "Study": "Chai et al. [1997a]"
     },
@@ -750,35 +750,35 @@
         "Crystal System": "Monoclinic",
         "Density(g/cm3)": 3.32,
         "Phase": "Augite",
         "Primary Phase": "Clinopyroxenes",
         "Study": "Aleksandrov et al. [1974]"
     },
     {
-        "C11": 6.71,
-        "C12": 4.59,
-        "C13": 4.37,
+        "C11": 237.8,
+        "C12": 83.5,
+        "C13": 80.0,
         "C14": 0,
-        "C15": -0.73,
+        "C15": 9.0,
         "C16": 0,
-        "C22": 5.68,
-        "C23": 4.06,
+        "C22": 183.6,
+        "C23": 59.9,
         "C24": 0,
-        "C25": -0.21,
+        "C25": 9.5,
         "C26": 0,
-        "C33": 6.78,
+        "C33": 229.5,
         "C34": 0,
-        "C35": 1.5,
+        "C35": 48.1,
         "C36": 0,
-        "C44": 1.52,
+        "C44": 76.5,
         "C45": 0,
-        "C46": -0.17,
-        "C55": 1.86,
+        "C46": 8.4,
+        "C55": 73.0,
         "C56": 0,
-        "C66": 2.56,
+        "C66": 81.6,
         "Crystal Reference Frame": "X||a* Y|| b Z||c",
         "Crystal System": "Monoclinic",
         "Density(g/cm3)": 3.327,
         "Phase": "Diopside",
         "Primary Phase": "Clinopyroxenes",
         "Study": "Collins and Brown [1998]"
     },
```

### Comparing `santex-1.0/santex.egg-info/PKG-INFO` & `santex-1.1/santex.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 Metadata-Version: 2.1
 Name: santex
-Version: 1.0
+Version: 1.1
 Summary: SAnTeX is a Python library which calculates seismic anisotropy from full elastic tensor of rocks from modal mineral composition, crystallographic orientation, and a crystal stiffness tensor catalogue that accounts for the dependency of elasticity with pressure and temperature. SAnTex facilitates the processing and cleaning of EBSD data and calculation of Orientation Distribution Function (ODF) and Inverse pole figure (IPF)
 Home-page: https://github.com/utpal-singh/SAnTex
 Author: Utpal Singh
 Author-email: utpal_singh@yahoo.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Keywords: python,seismic,seismic anisotropy,EBSD,Texture,Crystallography
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: joblib
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: vtk
 Requires-Dist: tqdm
 Requires-Dist: tabulate
 Requires-Dist: scikit-learn
 Requires-Dist: plotly
 Requires-Dist: orix
+Requires-Dist: sphinx_rtd_theme
 
 # SAnTex: Seismic Anisotropy from Texture
 
-SAnTeX is a Python library which calculates the full elastic tensor of rocks from modal mineral composition, crystallographic orientation, and a crystal stiffness tensor catalogue that accounts for the dependency of elasticity with pressure and temperature.
+SAnTex is a Python library which calculates the full elastic tensor of rocks from modal mineral composition, crystallographic orientation, and a crystal stiffness tensor catalogue that accounts for the dependency of elasticity with pressure and temperature.
 
 ## Features
 
 - **Pre-processing and cleaning of EBSD data**: SAnTex facilitates the processing and cleaning of EBSD data.  To enhance data completeness, SAnTex  offers the option to fill not-indexed pixels or indexed pixels removed during the cleaning process, using machine learning techniques.
 - **Tensor operations**: Tensor conversions between Voigt matrix and full stiffness tensors, as well as rotations based on euler angles.
 - **Material analysis**: SAnTex provides a catalogue of minerals, users can load the catalogue and can either utilise them to load stiffness tensors for their EBSD phases or make a modal rock and can calculate seismic anisotropy for the modal rock.
 - **Seismic Anisotropy**: SAnTex performs calculations of seismic anisotropy at a range of pressure and temperature conditions.  It also offers visualisation capabilities, allowing users to view the calculated seismic anisotropy in 2D and 3D plots. 
 - **Isotropic velocities**: Calculates isotropic seismic wave velocities (Vp, Vs and vbulk), isothermal bulk modulus, and density at elevated temperatures and pressures (Hacker & Abers, 2004). 
 
 
 ## Installation
 
-You can install SAnTeX using pip:
+You can install SAnTex using pip from your terminal:
 
 ```bash
 git clone https://github.com/utpal-singh/SAnTex.git
-cd sage
+cd santex
 pip install .
+```
 
+
+or
+
+```bash
+pip install santex
+```
```

### Comparing `santex-1.0/santex.egg-info/SOURCES.txt` & `santex-1.1/santex.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,30 @@
+LICENSE
 README.md
 setup.py
 santex/__init__.py
 santex.egg-info/PKG-INFO
 santex.egg-info/SOURCES.txt
 santex.egg-info/dependency_links.txt
 santex.egg-info/requires.txt
 santex.egg-info/top_level.txt
 santex/anisotropy/__init__.py
 santex/anisotropy/anisotropy.py
-santex/anisotropy/calcMeltVolume.py
 santex/anisotropy/map.py
 santex/anisotropy/melt.py
 santex/anisotropy/modalAnisotropy.py
 santex/anisotropy/plot_seismic_velocity.py
 santex/anisotropy/plot_vel_grid.py
 santex/anisotropy/utils.py
 santex/anisotropy/vtkplotter.py
 santex/ebsd/__init__.py
+santex/ebsd/_ctf_parser.py
 santex/ebsd/calcGrainBoundary.py
-santex/ebsd/calcGrainBoundary2.py
-santex/ebsd/ctf_parser.py
 santex/ebsd/ebsd.py
-santex/ebsd/ebsdrotation.py
-santex/ebsd/melt.py
+santex/ebsd/melt_tensor.py
 santex/ebsd/odf.py
 santex/ebsd/rotateEBSD.py
 santex/ebsd/saveEBSD.py
 santex/isotropy/__init__.py
 santex/isotropy/isotropy.py
 santex/isotropy/data/materials.json
 santex/material/__init__.py
```

### Comparing `santex-1.0/setup.py` & `santex-1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0'
+VERSION = '1.1'
 DESCRIPTION = "SAnTeX is a Python library which calculates seismic anisotropy from full elastic tensor of rocks from modal mineral composition, crystallographic orientation, and a crystal stiffness tensor catalogue that accounts for the dependency of elasticity with pressure and temperature. SAnTex facilitates the processing and cleaning of EBSD data and calculation of Orientation Distribution Function (ODF) and Inverse pole figure (IPF)"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='santex',
@@ -14,15 +14,14 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/utpal-singh/SAnTex",
     license='GNU Lesser General Public License v3 (LGPLv3)',
     classifiers=[
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Operating System :: OS Independent',
     ],
     packages=find_packages(),
     install_requires=[
         'joblib',
@@ -31,14 +30,15 @@
         'numpy',
         'vtk',
         'tqdm',
         'tabulate',
         'scikit-learn',
         'plotly',
         'orix',
+        'sphinx_rtd_theme',
     ],
     keywords=['python', 'seismic', 'seismic anisotropy', 'EBSD', 'Texture', "Crystallography"],
     package_data={
         'santex': [
             'isotropy/data/*',
             'material/data/*',
         ],
```

