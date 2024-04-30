# Comparing `tmp/echordlib-1.0.0.tar.gz` & `tmp/echordlib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echordlib-1.0.0.tar", max compression
+gzip compressed data, was "echordlib-1.0.1.tar", max compression
```

## Comparing `echordlib-1.0.0.tar` & `echordlib-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     8320 2024-01-04 14:15:24.020014 echordlib-1.0.0/eCHORDlib/BM3D_GUI_pg_v1.py
--rw-r--r--   0        0        0     4703 2024-01-03 16:21:02.207191 echordlib-1.0.0/eCHORDlib/BM3D_v1.ui
--rw-r--r--   0        0        0     6800 2024-01-04 14:11:33.518145 echordlib-1.0.0/eCHORDlib/Fct_profil_modification.py
--rw-r--r--   0        0        0     7000 2024-01-05 08:52:49.000000 echordlib-1.0.0/eCHORDlib/general_functions.py
--rw-r--r--   0        0        0    52039 2024-01-03 16:21:02.286329 echordlib-1.0.0/eCHORDlib/indexation_tiff_sur_GPU_v19_lib.py
--rw-r--r--   0        0        0    23205 2024-01-05 10:34:22.000000 echordlib-1.0.0/eCHORDlib/indexation_tiff_sur_GPU_v20_lib.py
--rw-r--r--   0        0        0    10223 2024-01-27 11:57:10.555640 echordlib-1.0.0/eCHORDlib/IPF_V1.py
--rw-r--r--   0        0        0     9385 2024-01-04 14:23:57.312065 echordlib-1.0.0/eCHORDlib/NLMD_GUI_pg_v1.py
--rw-r--r--   0        0        0     6432 2024-01-03 16:21:02.276670 echordlib-1.0.0/eCHORDlib/NLMD_v1.ui
--rw-r--r--   0        0        0     4772 2024-01-03 16:21:02.286329 echordlib-1.0.0/eCHORDlib/remOutliers_v3.ui
--rw-r--r--   0        0        0     8128 2024-01-04 14:23:07.119006 echordlib-1.0.0/eCHORDlib/remOutliersGUI_pg_v2.py
--rw-r--r--   0        0        0     2891 2024-01-03 16:21:02.286329 echordlib-1.0.0/eCHORDlib/requirements.txt
--rw-r--r--   0        0        0    24069 2024-01-03 16:21:02.276670 echordlib-1.0.0/eCHORDlib/Rotations.py
--rw-r--r--   0        0        0     2907 2024-01-03 16:21:02.286329 echordlib-1.0.0/eCHORDlib/stackViewer_v2.ui
--rw-r--r--   0        0        0     4789 2024-01-04 14:22:05.549792 echordlib-1.0.0/eCHORDlib/stackViewerGUI_pg_v2.py
--rw-r--r--   0        0        0     6608 2024-01-04 08:16:59.256806 echordlib-1.0.0/eCHORDlib/Symetry.py
--rw-r--r--   0        0        0      371 2024-01-03 16:21:02.286329 echordlib-1.0.0/eCHORDlib/test_general_functions.py
--rw-r--r--   0        0        0     8193 2024-01-04 14:20:57.879336 echordlib-1.0.0/eCHORDlib/VSNR_GUI_pg_v1.py
--rw-r--r--   0        0        0     3899 2024-01-03 16:21:02.276670 echordlib-1.0.0/eCHORDlib/VSNR_v1.ui
--rw-r--r--   0        0        0     4541 2024-01-05 09:41:12.000000 echordlib-1.0.0/eCHORDlib/Xallo.py
--rw-r--r--   0        0        0      967 2024-04-29 16:55:43.458819 echordlib-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-29 15:25:25.847033 echordlib-1.0.0/README.md
--rw-r--r--   0        0        0     1417 1970-01-01 00:00:00.000000 echordlib-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     8320 2024-01-04 14:15:24.020014 echordlib-1.0.1/eCHORDlib/BM3D_GUI_pg_v1.py
+-rw-r--r--   0        0        0     4703 2024-01-03 16:21:02.207191 echordlib-1.0.1/eCHORDlib/BM3D_v1.ui
+-rw-r--r--   0        0        0     6800 2024-01-04 14:11:33.518145 echordlib-1.0.1/eCHORDlib/Fct_profil_modification.py
+-rw-r--r--   0        0        0     7000 2024-01-05 08:52:49.000000 echordlib-1.0.1/eCHORDlib/general_functions.py
+-rw-r--r--   0        0        0    52039 2024-01-03 16:21:02.286329 echordlib-1.0.1/eCHORDlib/indexation_tiff_sur_GPU_v19_lib.py
+-rw-r--r--   0        0        0    23205 2024-01-05 10:34:22.000000 echordlib-1.0.1/eCHORDlib/indexation_tiff_sur_GPU_v20_lib.py
+-rw-r--r--   0        0        0    10223 2024-01-27 11:57:10.555640 echordlib-1.0.1/eCHORDlib/IPF_V1.py
+-rw-r--r--   0        0        0     9385 2024-01-04 14:23:57.312065 echordlib-1.0.1/eCHORDlib/NLMD_GUI_pg_v1.py
+-rw-r--r--   0        0        0     6432 2024-01-03 16:21:02.276670 echordlib-1.0.1/eCHORDlib/NLMD_v1.ui
+-rw-r--r--   0        0        0     4772 2024-01-03 16:21:02.286329 echordlib-1.0.1/eCHORDlib/remOutliers_v3.ui
+-rw-r--r--   0        0        0     8128 2024-01-04 14:23:07.119006 echordlib-1.0.1/eCHORDlib/remOutliersGUI_pg_v2.py
+-rw-r--r--   0        0        0     2891 2024-01-03 16:21:02.286329 echordlib-1.0.1/eCHORDlib/requirements.txt
+-rw-r--r--   0        0        0    24069 2024-01-03 16:21:02.276670 echordlib-1.0.1/eCHORDlib/Rotations.py
+-rw-r--r--   0        0        0     2907 2024-01-03 16:21:02.286329 echordlib-1.0.1/eCHORDlib/stackViewer_v2.ui
+-rw-r--r--   0        0        0     4789 2024-01-04 14:22:05.549792 echordlib-1.0.1/eCHORDlib/stackViewerGUI_pg_v2.py
+-rw-r--r--   0        0        0     6608 2024-01-04 08:16:59.256806 echordlib-1.0.1/eCHORDlib/Symetry.py
+-rw-r--r--   0        0        0      371 2024-01-03 16:21:02.286329 echordlib-1.0.1/eCHORDlib/test_general_functions.py
+-rw-r--r--   0        0        0     8193 2024-01-04 14:20:57.879336 echordlib-1.0.1/eCHORDlib/VSNR_GUI_pg_v1.py
+-rw-r--r--   0        0        0     3899 2024-01-03 16:21:02.276670 echordlib-1.0.1/eCHORDlib/VSNR_v1.ui
+-rw-r--r--   0        0        0     4541 2024-01-05 09:41:12.000000 echordlib-1.0.1/eCHORDlib/Xallo.py
+-rw-r--r--   0        0        0    35823 2024-04-30 10:31:26.630118 echordlib-1.0.1/LICENSE
+-rw-r--r--   0        0        0      967 2024-04-30 10:34:42.772770 echordlib-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-29 15:25:25.847033 echordlib-1.0.1/README.md
+-rw-r--r--   0        0        0     1417 1970-01-01 00:00:00.000000 echordlib-1.0.1/PKG-INFO
```

### Comparing `echordlib-1.0.0/eCHORDlib/BM3D_GUI_pg_v1.py` & `echordlib-1.0.1/eCHORDlib/BM3D_GUI_pg_v1.py`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/BM3D_v1.ui` & `echordlib-1.0.1/eCHORDlib/BM3D_v1.ui`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/Fct_profil_modification.py` & `echordlib-1.0.1/eCHORDlib/Fct_profil_modification.py`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/general_functions.py` & `echordlib-1.0.1/eCHORDlib/general_functions.py`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/indexation_tiff_sur_GPU_v19_lib.py` & `echordlib-1.0.1/eCHORDlib/indexation_tiff_sur_GPU_v19_lib.py`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/indexation_tiff_sur_GPU_v20_lib.py` & `echordlib-1.0.1/eCHORDlib/indexation_tiff_sur_GPU_v20_lib.py`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/IPF_V1.py` & `echordlib-1.0.1/eCHORDlib/IPF_V1.py`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/NLMD_GUI_pg_v1.py` & `echordlib-1.0.1/eCHORDlib/NLMD_GUI_pg_v1.py`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/NLMD_v1.ui` & `echordlib-1.0.1/eCHORDlib/NLMD_v1.ui`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/remOutliers_v3.ui` & `echordlib-1.0.1/eCHORDlib/remOutliers_v3.ui`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/remOutliersGUI_pg_v2.py` & `echordlib-1.0.1/eCHORDlib/remOutliersGUI_pg_v2.py`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/requirements.txt` & `echordlib-1.0.1/eCHORDlib/requirements.txt`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/Rotations.py` & `echordlib-1.0.1/eCHORDlib/Rotations.py`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/stackViewer_v2.ui` & `echordlib-1.0.1/eCHORDlib/stackViewer_v2.ui`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/stackViewerGUI_pg_v2.py` & `echordlib-1.0.1/eCHORDlib/stackViewerGUI_pg_v2.py`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/Symetry.py` & `echordlib-1.0.1/eCHORDlib/Symetry.py`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/VSNR_GUI_pg_v1.py` & `echordlib-1.0.1/eCHORDlib/VSNR_GUI_pg_v1.py`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/VSNR_v1.ui` & `echordlib-1.0.1/eCHORDlib/VSNR_v1.ui`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/eCHORDlib/Xallo.py` & `echordlib-1.0.1/eCHORDlib/Xallo.py`

 * *Files identical despite different names*

### Comparing `echordlib-1.0.0/pyproject.toml` & `echordlib-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "echordlib"
-version = "1.0.0"
+version = "1.0.1"
 description = "mandatory library for CHORD framework (image tratment, indexing and visualization)"
 authors = ["Langlois Cyril, Gabriel L'Hôte, Clément Lafond, Joël Lachambre"]
 license = "CeCILL"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `echordlib-1.0.0/PKG-INFO` & `echordlib-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echordlib
-Version: 1.0.0
+Version: 1.0.1
 Summary: mandatory library for CHORD framework (image tratment, indexing and visualization)
 License: CeCILL
 Author: Langlois Cyril, Gabriel L'Hôte, Clément Lafond, Joël Lachambre
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

