# Comparing `tmp/PyCOMUS-1.0.3.tar.gz` & `tmp/pycomus-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyCOMUS-1.0.3.tar", last modified: Fri Mar 15 07:33:09 2024, max compression
+gzip compressed data, was "pycomus-1.0.4.tar", last modified: Tue Apr 30 01:53:54 2024, max compression
```

## Comparing `PyCOMUS-1.0.3.tar` & `pycomus-1.0.4.tar`

### file list

```diff
@@ -1,48 +1,74 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 07:33:09.000000 PyCOMUS-1.0.3/
--rw-rw-rw-   0        0        0     5139 2024-03-15 07:33:09.000000 PyCOMUS-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-15 07:33:09.000000 PyCOMUS-1.0.3/pycomus/
-drwxrwxrwx   0        0        0        0 2024-03-15 07:33:09.000000 PyCOMUS-1.0.3/pycomus/ComusDis/
--rw-rw-rw-   0        0        0    19455 2024-03-01 01:35:51.000000 PyCOMUS-1.0.3/pycomus/ComusDis/CmsDis.py
--rw-rw-rw-   0        0        0    25336 2024-02-29 08:19:33.000000 PyCOMUS-1.0.3/pycomus/ComusDis/CmsGridPars.py
--rw-rw-rw-   0        0        0     5299 2024-03-15 03:52:33.000000 PyCOMUS-1.0.3/pycomus/ComusDis/CmsMd.py
--rw-rw-rw-   0        0        0     6489 2024-03-04 03:25:51.000000 PyCOMUS-1.0.3/pycomus/ComusDis/CmsOutPars.py
--rw-rw-rw-   0        0        0    11621 2024-03-15 02:36:58.000000 PyCOMUS-1.0.3/pycomus/ComusDis/CmsPars.py
--rw-rw-rw-   0        0        0     5151 2024-03-05 09:18:02.000000 PyCOMUS-1.0.3/pycomus/ComusDis/CmsTime.py
--rw-rw-rw-   0        0        0      389 2024-02-07 03:08:10.000000 PyCOMUS-1.0.3/pycomus/ComusDis/GridCell.py
--rw-rw-rw-   0        0        0      670 2024-02-05 03:51:34.000000 PyCOMUS-1.0.3/pycomus/ComusDis/GridLyr.py
--rw-rw-rw-   0        0        0      226 2024-02-01 04:28:53.000000 PyCOMUS-1.0.3/pycomus/ComusDis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 07:33:09.000000 PyCOMUS-1.0.3/pycomus/Package/
--rw-rw-rw-   0        0        0     7269 2024-03-04 02:31:48.000000 PyCOMUS-1.0.3/pycomus/Package/CDRN.py
--rw-rw-rw-   0        0        0     9716 2024-03-04 02:32:27.000000 PyCOMUS-1.0.3/pycomus/Package/CEVT.py
--rw-rw-rw-   0        0        0     7700 2024-03-04 02:33:24.000000 PyCOMUS-1.0.3/pycomus/Package/CGHB.py
--rw-rw-rw-   0        0        0     5764 2024-03-01 01:57:45.000000 PyCOMUS-1.0.3/pycomus/Package/CHFB.py
--rw-rw-rw-   0        0        0     5570 2024-03-01 02:01:43.000000 PyCOMUS-1.0.3/pycomus/Package/CIBS.py
--rw-rw-rw-   0        0        0    20378 2024-03-01 02:04:12.000000 PyCOMUS-1.0.3/pycomus/Package/CLAK.py
--rw-rw-rw-   0        0        0     6160 2024-03-04 02:30:44.000000 PyCOMUS-1.0.3/pycomus/Package/CRCH.py
--rw-rw-rw-   0        0        0     4917 2024-03-01 02:09:30.000000 PyCOMUS-1.0.3/pycomus/Package/CREG.py
--rw-rw-rw-   0        0        0    14829 2024-03-01 02:10:26.000000 PyCOMUS-1.0.3/pycomus/Package/CRES.py
--rw-rw-rw-   0        0        0     9156 2024-03-04 02:34:00.000000 PyCOMUS-1.0.3/pycomus/Package/CRIV.py
--rw-rw-rw-   0        0        0     6745 2024-03-04 02:14:54.000000 PyCOMUS-1.0.3/pycomus/Package/CSHB.py
--rw-rw-rw-   0        0        0    42493 2024-03-15 06:34:52.000000 PyCOMUS-1.0.3/pycomus/Package/CSTR.py
--rw-rw-rw-   0        0        0    21610 2024-03-01 07:34:13.000000 PyCOMUS-1.0.3/pycomus/Package/CSUB.py
--rw-rw-rw-   0        0        0     7151 2024-03-04 02:34:26.000000 PyCOMUS-1.0.3/pycomus/Package/CWEL.py
--rw-rw-rw-   0        0        0      392 2024-02-22 01:12:55.000000 PyCOMUS-1.0.3/pycomus/Package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 07:33:09.000000 PyCOMUS-1.0.3/pycomus/Utils/
--rw-rw-rw-   0        0        0     9456 2024-02-29 07:14:22.000000 PyCOMUS-1.0.3/pycomus/Utils/BoundaryCheck.py
--rw-rw-rw-   0        0        0     1813 2024-03-04 03:24:27.000000 PyCOMUS-1.0.3/pycomus/Utils/CONSTANTS.py
--rw-rw-rw-   0        0        0    19768 2024-03-15 02:33:52.000000 PyCOMUS-1.0.3/pycomus/Utils/LinuxCheckParams.so
--rw-rw-rw-   0        0        0  2516512 2024-03-15 01:34:26.000000 PyCOMUS-1.0.3/pycomus/Utils/LinuxComus.so
--rw-rw-rw-   0        0        0     4181 2024-03-06 02:35:53.000000 PyCOMUS-1.0.3/pycomus/Utils/Map.py
--rw-rw-rw-   0        0        0    11877 2024-03-06 02:09:33.000000 PyCOMUS-1.0.3/pycomus/Utils/ReadData.py
--rw-rw-rw-   0        0        0    13824 2024-02-05 02:25:25.000000 PyCOMUS-1.0.3/pycomus/Utils/WinCheckParams.dll
--rw-rw-rw-   0        0        0   757760 2024-03-14 09:00:49.000000 PyCOMUS-1.0.3/pycomus/Utils/WinComus.dll
--rw-rw-rw-   0        0        0       61 2024-03-05 07:43:35.000000 PyCOMUS-1.0.3/pycomus/Utils/__init__.py
--rw-rw-rw-   0        0        0      172 2024-02-01 02:11:48.000000 PyCOMUS-1.0.3/pycomus/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 07:33:09.000000 PyCOMUS-1.0.3/PyCOMUS.egg-info/
--rw-rw-rw-   0        0        0        1 2024-03-15 07:33:08.000000 PyCOMUS-1.0.3/PyCOMUS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     5139 2024-03-15 07:33:08.000000 PyCOMUS-1.0.3/PyCOMUS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1037 2024-03-15 07:33:08.000000 PyCOMUS-1.0.3/PyCOMUS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2024-03-15 07:33:08.000000 PyCOMUS-1.0.3/PyCOMUS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4616 2024-03-06 05:50:45.000000 PyCOMUS-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-03-15 07:33:09.000000 PyCOMUS-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      948 2024-03-15 07:32:57.000000 PyCOMUS-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.870367 pycomus-1.0.4/
+-rw-rw-rw-   0        0        0     5166 2024-04-30 01:53:54.869351 pycomus-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.868322 pycomus-1.0.4/PyCOMUS.egg-info/
+-rw-rw-rw-   0        0        0     5166 2024-04-30 01:53:54.000000 pycomus-1.0.4/PyCOMUS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1919 2024-04-30 01:53:54.000000 pycomus-1.0.4/PyCOMUS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 01:53:54.000000 pycomus-1.0.4/PyCOMUS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-30 01:53:54.000000 pycomus-1.0.4/PyCOMUS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4684 2024-04-18 01:48:26.000000 pycomus-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.316623 pycomus-1.0.4/RestfulApi/
+drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.318170 pycomus-1.0.4/RestfulApi/ComusApi/
+drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.354480 pycomus-1.0.4/RestfulApi/ComusApi/ComusApi/
+-rw-rw-rw-   0        0        0        0 2024-03-18 00:44:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusApi/__init__.py
+-rw-rw-rw-   0        0        0      409 2024-03-18 00:44:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusApi/asgi.py
+-rw-rw-rw-   0        0        0     3930 2024-03-18 03:23:34.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusApi/settings.py
+-rw-rw-rw-   0        0        0      825 2024-03-18 00:54:12.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusApi/urls.py
+-rw-rw-rw-   0        0        0      409 2024-03-18 00:44:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusApi/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.402192 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/
+-rw-rw-rw-   0        0        0        0 2024-03-18 00:44:50.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-18 00:44:50.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/admin.py
+-rw-rw-rw-   0        0        0      154 2024-03-18 07:41:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.408379 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/migrations/
+-rw-rw-rw-   0        0        0     2954 2024-03-18 07:41:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      413 2024-03-18 07:41:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/migrations/0002_alter_comusctrlparsmodel_comus_dis_uuid.py
+-rw-rw-rw-   0        0        0     1512 2024-03-18 07:41:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/migrations/0003_comusoutparsmodel.py
+-rw-rw-rw-   0        0        0        0 2024-03-18 00:44:50.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2658 2024-03-18 08:09:54.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/models.py
+-rw-rw-rw-   0        0        0     6044 2024-03-18 07:47:07.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/serializers.py
+-rw-rw-rw-   0        0        0       63 2024-03-18 00:44:50.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/tests.py
+-rw-rw-rw-   0        0        0      386 2024-03-18 07:32:07.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/urls.py
+-rw-rw-rw-   0        0        0     5789 2024-03-18 08:07:45.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/views.py
+-rw-rw-rw-   0        0        0        0 2024-03-18 03:39:00.000000 pycomus-1.0.4/RestfulApi/ComusApi/__init__.py
+-rw-rw-rw-   0        0        0      686 2024-03-18 00:44:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/manage.py
+-rw-rw-rw-   0        0        0        0 2024-03-18 03:39:00.000000 pycomus-1.0.4/RestfulApi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.408892 pycomus-1.0.4/pycomus/
+drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.466366 pycomus-1.0.4/pycomus/ComusDis/
+-rw-rw-rw-   0        0        0     1813 2024-03-04 03:24:27.000000 pycomus-1.0.4/pycomus/ComusDis/CONSTANTS.py
+-rw-rw-rw-   0        0        0    21568 2024-04-30 01:45:25.000000 pycomus-1.0.4/pycomus/ComusDis/CmsDis.py
+-rw-rw-rw-   0        0        0    26311 2024-04-29 01:57:32.000000 pycomus-1.0.4/pycomus/ComusDis/CmsGridPars.py
+-rw-rw-rw-   0        0        0     4842 2024-04-29 01:49:54.000000 pycomus-1.0.4/pycomus/ComusDis/CmsMd.py
+-rw-rw-rw-   0        0        0     6648 2024-04-29 01:49:54.000000 pycomus-1.0.4/pycomus/ComusDis/CmsOutPars.py
+-rw-rw-rw-   0        0        0    12197 2024-04-29 01:49:54.000000 pycomus-1.0.4/pycomus/ComusDis/CmsPars.py
+-rw-rw-rw-   0        0        0     5597 2024-04-29 01:59:01.000000 pycomus-1.0.4/pycomus/ComusDis/CmsTime.py
+-rw-rw-rw-   0        0        0      389 2024-02-07 03:08:10.000000 pycomus-1.0.4/pycomus/ComusDis/GridCell.py
+-rw-rw-rw-   0        0        0      670 2024-02-05 03:51:34.000000 pycomus-1.0.4/pycomus/ComusDis/GridLyr.py
+-rw-rw-rw-   0        0        0      221 2024-04-30 01:49:26.000000 pycomus-1.0.4/pycomus/ComusDis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.672317 pycomus-1.0.4/pycomus/Package/
+-rw-rw-rw-   0        0        0     7972 2024-04-29 02:07:48.000000 pycomus-1.0.4/pycomus/Package/CDRN.py
+-rw-rw-rw-   0        0        0    10485 2024-04-29 02:07:52.000000 pycomus-1.0.4/pycomus/Package/CEVT.py
+-rw-rw-rw-   0        0        0     8343 2024-04-29 02:08:21.000000 pycomus-1.0.4/pycomus/Package/CGHB.py
+-rw-rw-rw-   0        0        0     6240 2024-04-29 02:09:29.000000 pycomus-1.0.4/pycomus/Package/CHFB.py
+-rw-rw-rw-   0        0        0     6132 2024-04-29 02:12:07.000000 pycomus-1.0.4/pycomus/Package/CIBS.py
+-rw-rw-rw-   0        0        0    21602 2024-04-29 02:32:25.000000 pycomus-1.0.4/pycomus/Package/CLAK.py
+-rw-rw-rw-   0        0        0     6632 2024-04-29 02:17:59.000000 pycomus-1.0.4/pycomus/Package/CRCH.py
+-rw-rw-rw-   0        0        0     5371 2024-04-29 02:19:25.000000 pycomus-1.0.4/pycomus/Package/CREG.py
+-rw-rw-rw-   0        0        0    15899 2024-04-29 02:33:20.000000 pycomus-1.0.4/pycomus/Package/CRES.py
+-rw-rw-rw-   0        0        0     9861 2024-04-29 02:40:00.000000 pycomus-1.0.4/pycomus/Package/CRIV.py
+-rw-rw-rw-   0        0        0     7323 2024-04-29 02:43:07.000000 pycomus-1.0.4/pycomus/Package/CSHB.py
+-rw-rw-rw-   0        0        0    46089 2024-04-29 02:57:18.000000 pycomus-1.0.4/pycomus/Package/CSTR.py
+-rw-rw-rw-   0        0        0    23849 2024-04-29 03:05:02.000000 pycomus-1.0.4/pycomus/Package/CSUB.py
+-rw-rw-rw-   0        0        0     7702 2024-04-29 03:06:22.000000 pycomus-1.0.4/pycomus/Package/CWEL.py
+-rw-rw-rw-   0        0        0      392 2024-02-22 01:12:55.000000 pycomus-1.0.4/pycomus/Package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.867289 pycomus-1.0.4/pycomus/Utils/
+-rw-rw-rw-   0        0        0     9516 2024-04-18 01:34:14.000000 pycomus-1.0.4/pycomus/Utils/BoundaryCheck.py
+-rw-rw-rw-   0        0        0     1813 2024-03-04 03:24:27.000000 pycomus-1.0.4/pycomus/Utils/CONSTANTS.py
+-rw-rw-rw-   0        0        0    19768 2024-03-15 02:33:52.000000 pycomus-1.0.4/pycomus/Utils/LinuxCheckParams.so
+-rw-rw-rw-   0        0        0  2516512 2024-03-15 01:34:26.000000 pycomus-1.0.4/pycomus/Utils/LinuxComus.so
+-rw-rw-rw-   0        0        0     5703 2024-04-29 03:23:40.000000 pycomus-1.0.4/pycomus/Utils/Map.py
+-rw-rw-rw-   0        0        0    15272 2024-04-29 03:45:14.000000 pycomus-1.0.4/pycomus/Utils/ReadData.py
+-rw-rw-rw-   0        0        0    13824 2024-02-05 02:25:25.000000 pycomus-1.0.4/pycomus/Utils/WinCheckParams.dll
+-rw-rw-rw-   0        0        0   757760 2024-03-14 09:00:49.000000 pycomus-1.0.4/pycomus/Utils/WinComus.dll
+-rw-rw-rw-   0        0        0       61 2024-03-05 07:43:35.000000 pycomus-1.0.4/pycomus/Utils/__init__.py
+-rw-rw-rw-   0        0        0      172 2024-02-01 02:11:48.000000 pycomus-1.0.4/pycomus/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-30 01:53:54.870378 pycomus-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      948 2024-04-30 01:51:51.000000 pycomus-1.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyCOMUS-1.0.3/pycomus/ComusDis/CmsDis.py` & `pycomus-1.0.4/pycomus/ComusDis/CmsDis.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,52 +3,82 @@
 # Version: 1.0.0
 # Author: Zhenjiang Wu
 # Description: Set COMUS Model LPF Or BCF Layer Property.
 # --------------------------------------------------------------
 import os
 from typing import List, Union, Tuple
 
-import pycomus
-from pycomus.ComusDis.GridCell import GridCell
-from pycomus.ComusDis.GridLyr import LpfLayers, BcfLayers
-from pycomus.Utils.CONSTANTS import LPF_LYR_FILE_NAME, BCF_LYR_FILE_NAME, LPF_LYR_PKG_NAME, BCF_LYR_PKG_NAME, \
+from GridCell import GridCell
+from GridLyr import LpfLayers, BcfLayers
+from CONSTANTS import LPF_LYR_FILE_NAME, BCF_LYR_FILE_NAME, LPF_LYR_PKG_NAME, BCF_LYR_PKG_NAME, \
     GRID_SPACE_FILE_NAME, CON_PKG_NAME
 
 
 class ComusDis:
+    """
+    Base Class
+    """
+
     def __init__(self, model, num_lyr: int = 1, num_row: int = 1, num_col: int = 1,
-                 x_coord: float = 0, y_coord: float = 0, row_space: Union[float, int, List[float]] = 1,
+                 x_coord: Union[float, int] = 0, y_coord: Union[float, int] = 0,
+                 row_space: Union[float, int, List[float]] = 1,
                  col_space: Union[float, int, List[float]] = 1):
-        if num_row < 1:
-            raise ValueError("num_row should be greater than 0!")
-        if num_col < 1:
-            raise ValueError("num_col should be greater than 0!")
-        if num_lyr < 1:
-            raise ValueError("num_lyr should be greater than 0!")
-        self.num_lyr: int = num_lyr
-        self.num_row: int = num_row
-        self.num_col: int = num_col
-        self.x_coord: float = x_coord
-        self.y_coord: float = y_coord
+
+        # Check layer,row,col
+        if isinstance(num_lyr, int):
+            self.num_lyr: int = num_lyr
+            if num_lyr < 1:
+                raise ValueError("num_lyr should be greater than 0!")
+        else:
+            raise ValueError("num_lyr should be int")
+
+        if isinstance(num_row, int):
+            self.num_row: int = num_row
+            if num_row < 1:
+                raise ValueError("num_row should be greater than 0!")
+        else:
+            raise ValueError("num_row should be int")
+
+        if isinstance(num_col, int):
+            self.num_col: int = num_col
+            if num_col < 1:
+                raise ValueError("num_col should be greater than 0!")
+        else:
+            raise ValueError("num_col should be int")
+
+        # Check x_coord and y_coord
+        if isinstance(x_coord, (float, int)):
+            self.x_coord: Union[float, int] = x_coord
+        else:
+            raise ValueError("x_coord should be an integer or a float.")
+
+        if isinstance(y_coord, (float, int)):
+            self.y_coord: Union[float, int] = y_coord
+        else:
+            raise ValueError("y_coord should be an integer or a float.")
+
+        # Check row_space and col_space
         if isinstance(row_space, (float, int)):
             self.row_space: List[Union[int, float]] = [row_space] * num_row
         elif isinstance(row_space, list) and num_row != len(row_space):
             raise ValueError("row_space grid spacing length should be the same as num_row!")
         else:
             self.row_space: List[Union[int, float]] = row_space
+        if not all(x > 0 for x in self.row_space):
+            raise ValueError("row_space should be greater than 0")
+
         if isinstance(col_space, (float, int)):
             self.col_space: List[Union[int, float]] = [col_space] * num_col
         elif isinstance(col_space, list) and num_col != len(col_space):
             raise ValueError("col_space grid spacing length should be the same as num_col!")
         else:
             self.col_space: List[Union[int, float]] = col_space
-        if not all(x > 0 for x in self.row_space):
-            raise ValueError("row_space should be greater than 0")
         if not all(x > 0 for x in self.col_space):
             raise ValueError("col_space should be greater than 0")
+
         self._model = model
 
     @classmethod
     def _load_control_params(cls, ctrl_params_file: str) -> Tuple:
         with open(ctrl_params_file, 'r') as file:
             lines: List[str] = file.readlines()
         if len(lines) != 2:
@@ -87,78 +117,94 @@
                 raise ValueError("Row space or col space should be greater than 0")
             if data[0] == "R":
                 col_space.append(float(data[2]))
             else:
                 row_space.append(float(data[2]))
         return row_space, col_space
 
-    def __str__(self):
-        return f"Mesh Grid And Layer:\n    Number of layers : {self.num_lyr}\n    Number of rows : {self.num_row}\n    Number of cols : {self.num_col}  \n" \
-               f"    RowSpace : {self.row_space}  \n    ColSpace : {self.col_space}  \n    XCoord : {self.x_coord}\n    " \
-               f"YCoord : {self.y_coord}"
-
     def write_file(self, folder_path):
         with open(os.path.join(folder_path, GRID_SPACE_FILE_NAME), "w") as file:
             file.write("ATTI  NUMID  DELT\n")
             index: int = 1
             for rowSpace in self.row_space:
                 file.write(f"C  {index}  {rowSpace}\n")
                 index += 1
             index: int = 1
             for colSpace in self.col_space:
                 file.write(f"R  {index}  {colSpace}\n")
                 index += 1
 
+    def __str__(self):
+        return f"Grid And Layer:\n    Number of layers : {self.num_lyr}\n    Number of rows : {self.num_row}\n    Number of cols : {self.num_col}  \n" \
+               f"    RowSpace : {self.row_space}  \n    ColSpace : {self.col_space}  \n    XCoord : {self.x_coord}\n    " \
+               f"YCoord : {self.y_coord}"
+
 
 class ComusDisLpf(ComusDis):
-    def __init__(self, model, num_lyr: int = 1, num_row: int = 1, num_col: int = 1,
+    """
+    COMUS Layer Property Flow Package Class(LPF).
+
+    Attributes:
+    -----------
+    model : pycomus.ComusModel
+        COMUS Model Object
+    num_lyr : int
+        Number of layers
+    num_row : int
+        Number of rows
+    num_col : int
+        Number of columns
+    row_space : Union[float, int, List[float]]
+        A float, int, or List representing row spacing
+    col_space : Union[float, int, List[float]]
+        A float, int, or List representing column spacing
+    x_coord : float
+        Top left corner X coordinate
+    y_coord : float
+        Top left corner Y coordinate
+    lyr_type : List[int]
+        The data in lyr_type should be in [0: Confined, 1: Convertible]
+    lyr_cbd : List[int]
+        The data in lyr_cbd should be in [0: Quasi Three Dimensions-Disable, 1: Quasi Three Dimensions-Enable]
+    lyr_ibs : List[int]
+        The data in lyr_ibs should be in [0: IBS-Disable, 1: IBS-Enable]
+
+    Methods:
+    --------
+    __init__(self, model, num_lyr: int = 1, num_row: int = 1, num_col: int = 1,
                  row_space: Union[float, int, List[float]] = 1, col_space: Union[float, int, List[float]] = 1,
                  x_coord: float = 0, y_coord: float = 0, lyr_type: List[int] = None, lyr_cbd: List[int] = None,
-                 lyr_ibs: List[int] = None):
-        """
-        COMUS Layer Property Flow Package Class(LPF).
+                 lyr_ibs: List[int] = None)
+        Instantiate an instance of ComusDisLpf.
 
-        Parameters:
-        ----------------------------
-        model: pycomus.ComusModel
-            COMUS Model Object
-        num_lyr: int
-            Number of layers
-        num_row: int
-            Number of rows
-        num_col: int
-            Number of columns
-        row_space: Union[float, int, List[float]]
-            A float, int, or List representing row spacing
-        col_space: Union[float, int, List[float]]
-            A float, int, or List representing column spacing
-        x_coord: float
-            Top left corner X coordinate
-        y_coord: float
-            Top left corner Y coordinate
-        lyr_type: List[int]
-            The data in lyr_type should be in [0: Confined, 1: Convertible]
-        lyr_cbd: List[int]
-            The data in lyr_cbd should be in [0: Quasi Three Dimensions-Disable, 1: Quasi Three Dimensions-Enable]
-        lyr_ibs: List[int]
-            The data in lyr_ibs should be in [0: IBS-Disable, 1: IBS-Enable]
+    load(cls, model, ctrl_params_file: str, grd_space_file: str, lpf_lyr_file: str)
+         Load parameters from a LpfLyr.in file and create a ComusDisLpf instance.
 
-        Returns:
-        --------
-        instance: pycomus.ComusDisLpf
-            COMUS LPF Layer Params Object.
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusDisLpf`
+        module to the specified path as <LpfLyr.in>.
 
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> modelDis = pycomus.ComusDisLpf(model1, 1, 20, 20, row_space=1, col_space=1, lyr_type=[1 for _ in range(1)], y_coord=1)
-        """
+    Returns:
+    --------
+    instance: pycomus.ComusDisLpf
+        COMUS LPF Layer Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> modelDis = pycomus.ComusDisLpf(model1, 1, 20, 20, row_space=1, col_space=1, lyr_type=[1 for _ in range(1)], y_coord=1)
+    """
+
+    def __init__(self, model, num_lyr: int = 1, num_row: int = 1, num_col: int = 1,
+                 row_space: Union[float, int, List[float]] = 1, col_space: Union[float, int, List[float]] = 1,
+                 x_coord: float = 0, y_coord: float = 0, lyr_type: List[int] = None, lyr_cbd: List[int] = None,
+                 lyr_ibs: List[int] = None):
         super().__init__(model, num_lyr, num_row, num_col, x_coord, y_coord, row_space, col_space)
-        cms_pars: pycomus.ComusConPars = model.package[CON_PKG_NAME]
+        cms_pars = model.package[CON_PKG_NAME]
         if cms_pars.intblkm == 1:
             raise ValueError("In BCF format has been selected, it is not possible to add layers in LPF format.")
         if not lyr_type:
             lyr_type: List[int] = [0] * num_lyr
         if not lyr_cbd:
             lyr_cbd: List[int] = [0] * num_lyr
         if not lyr_ibs:
@@ -211,15 +257,15 @@
         Example:
         --------
         >>> import pycomus
         >>> model1 = pycomus.ComusModel(model_name="test")
         >>> modelDis = pycomus.ComusDisLpf.load(model1, "./InputFiles/CtrlPar.in", "./InputFiles/GrdSpace.in", "./InputFiles/LpfLyr.in")
         """
         # Check INTBLKM
-        cms_pars: pycomus.ComusConPars = model.package[CON_PKG_NAME]
+        cms_pars = model.package[CON_PKG_NAME]
         if cms_pars.intblkm == 1:
             raise ValueError("In BCF format has been selected, it is not possible to add layers in LPF format.")
 
         # Check Control Params
         num_lyr, num_row, num_col, x_coord, y_coord = ComusDis._load_control_params(ctrl_params_file)
 
         # Check Grid Space Params
@@ -259,58 +305,75 @@
             for i in range(self.num_lyr):
                 file.write(
                     f"{self._model.layers[i].lyr_id}  {self._model.layers[i].lyr_type}  -1  0  "
                     f"{self._model.layers[i].lyr_cbd}  {self._model.layers[i].lyr_ibs}\n")
 
 
 class ComusDisBcf(ComusDis):
-    def __init__(self, model, num_lyr: int = 1, num_row: int = 1, num_col: int = 1,
+    """
+    COMUS Grid And Layer Property Flow Package Class(BCF).
+
+    Attributes:
+    ----------------------------
+    model: pycomus.ComusModel
+        COMUS model object
+    num_lyr: int
+        Number of layers
+    num_row: int
+        Number of rows
+    num_col: int
+        Number of cols
+    row_space: Union[float, int, List[float]]
+        A float or List data that represents row spacing
+    col_space: Union[float, int, List[float]]
+        A float or List data that represents col spacing
+    x_coord: float, optional
+        Top left corner X coordinate, by default 0
+    y_coord: float, optional
+        Top left corner Y coordinate, by default 0
+    lyr_type: List[int]
+        The data in lyr_type should be in [0:Confined,1:Unconfined,2:Limited Convertible,3:Full Convertible]
+    lyr_trpy: List[float], optional
+        ky/kx, by default None
+    lyr_ibs: List[int], optional
+        The data in lyr_ibs should be in [0:IBS-Disable,1:IBS-Enable]!, by default None
+
+    Methods:
+    --------
+    __init__(self, model, num_lyr: int = 1, num_row: int = 1, num_col: int = 1,
                  row_space: Union[float, int, List[float]] = 1,
                  col_space: Union[float, int, List[float]] = 1,
                  x_coord: float = 0, y_coord: float = 0,
-                 lyr_type: List[int] = None, lyr_trpy: List[float] = None, lyr_ibs: List[int] = None) -> None:
-        """
-        COMUS Grid And Layer Property Flow Package Class(BCF).
+                 lyr_type: List[int] = None, lyr_trpy: List[float] = None, lyr_ibs: List[int] = None)
+        Instantiate an instance of ComusDisBcf.
 
-        Parameters:
-        ----------------------------
-        model: pycomus.ComusModel
-            COMUS model object
-        num_lyr: int
-            Number of layers
-        num_row: int
-            Number of rows
-        num_col: int
-            Number of cols
-        row_space: Union[float, int, List[float]]
-            A float or List data that represents row spacing
-        col_space: Union[float, int, List[float]]
-            A float or List data that represents col spacing
-        x_coord: float, optional
-            Top left corner X coordinate, by default 0
-        y_coord: float, optional
-            Top left corner Y coordinate, by default 0
-        lyr_type: List[int]
-            The data in lyr_type should be in [0:Confined,1:Unconfined,2:Limited Convertible,3:Full Convertible]
-        lyr_trpy: List[float], optional
-            ky/kx, by default None
-        lyr_ibs: List[int], optional
-            The data in lyr_ibs should be in [0:IBS-Disable,1:IBS-Enable]!, by default None
+    load(cls, model, ctrl_params_file: str, grd_space_file: str, bcf_lyr_file: str)
+         Load parameters from a LpfLyr.in file and create a ComusDisLpf instance.
 
-        Returns:
-        --------
-        instance: pycomus.ComusDisBcf
-            COMUS BCF Layer Params Object.
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusDisBcf`
+        module to the specified path as <BcfLyr.in>.
+
+    Returns:
+    --------
+    instance: pycomus.ComusDisBcf
+        COMUS BCF Layer Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> modelDis = pycomus.ComusDisBcf(model1, 1, 20, 20, row_space=1, col_space=1, lyr_type=[1 for _ in range(1)], y_coord=1)
+    """
 
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> modelDis = pycomus.ComusDisBcf(model1, 1, 20, 20, row_space=1, col_space=1, lyr_type=[1 for _ in range(1)], y_coord=1)
-        """
+    def __init__(self, model, num_lyr: int = 1, num_row: int = 1, num_col: int = 1,
+                 row_space: Union[float, int, List[float]] = 1,
+                 col_space: Union[float, int, List[float]] = 1,
+                 x_coord: float = 0, y_coord: float = 0,
+                 lyr_type: List[int] = None, lyr_trpy: List[float] = None, lyr_ibs: List[int] = None) -> None:
         super().__init__(model, num_lyr, num_row, num_col, x_coord, y_coord, row_space, col_space)
         cms_pars = model.package[CON_PKG_NAME]
         if cms_pars.intblkm == 2:
             raise ValueError("In LPF format has been selected, it is not possible to add layers in BCF format.")
         if not lyr_type:
             lyr_type = [0] * num_lyr
         if not lyr_trpy:
@@ -338,15 +401,15 @@
         self.lyr_type = lyr_type
         self.lyr_trpy = lyr_trpy
         self.lyr_ibs = lyr_ibs
 
     @classmethod
     def load(cls, model, ctrl_params_file: str, grd_space_file: str, bcf_lyr_file: str):
         """
-        Load parameters from a LpfLyr.in file and create a ComusDisLpf instance.
+        Load parameters from a BcfLyr.in file and create a ComusDisBcf instance.
 
         Parameters:
         ----------------------------
         model: pycomus.ComusModel
             COMUS Model Object.
         ctrl_params_file: str
             Control Params File(CtrlPar.in)
```

### Comparing `PyCOMUS-1.0.3/pycomus/ComusDis/CmsGridPars.py` & `pycomus-1.0.4/pycomus/ComusDis/CmsGridPars.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,77 +11,94 @@
 
 from pycomus.ComusDis.GridCell import GridCell
 from pycomus.Utils.CONSTANTS import BCF_GRID_FILE_NAME, LPF_GRID_FILE_NAME, GRID_PKG_NAME, BCF_LYR_PKG_NAME, \
     LPF_LYR_PKG_NAME, CON_PKG_NAME
 
 
 class ComusGridPars:
+    """
+    Set COMUS Model GridCell Parameter Attributes.
+
+    Attributes:
+    ----------------------------
+    model:
+        COMUS Model Object.
+    top:
+        A value of 0 indicates an inactive cell; 1 indicates a variable head cell; -1 indicates a constant head cell.
+    bot:
+        Represents the elevation of the bottom boundary of the grid cell (in length units).
+    ibound:
+        Represents the elevation of the top boundary of the grid cell (in length units).
+    shead:
+        The initial head value for the grid cell (L).
+    kx:
+        Permeability coefficient kx in the X-direction.
+    transm:
+        This represents the transmissivity of the grid cell in the row direction.
+    vcont:
+        The vertical hydraulic conductivity of the grid cell (1/T), also known as the leakage coefficient.
+    sc1:
+        Grid cell type 1 storage coefficient (-).
+    sc2:
+        Grid cell type 2 storage coefficient (-).
+    wet_dry:
+        The absolute value is the threshold by which the head in the adjacent cell must exceed the bottom elevation of the current cell to trigger wetting.
+    ky:
+        Permeability coefficient ky in the Y-direction.
+    kz:
+        Permeability coefficient kz in the Z-direction.
+    vkcb:
+        It represents the vertical hydraulic conductivity of the low-permeability medium at the bottom of the grid cell (L/T).
+    tkcb:
+        It denotes the thickness of the low-permeability medium at the bottom of the grid cell (L).
+
+    Methods:
+    --------
+    __init__(self, model, top: Union[float, int, np.ndarray] = None, bot: Union[float, int, np.ndarray] = None,
+        ibound: Union[int, np.ndarray] = None, shead: Union[float, int, np.ndarray] = None,
+        kx: Union[float, int, np.ndarray] = None, transm: Union[float, int, np.ndarray] = None,
+        vcont: Union[float, int, np.ndarray] = None, sc1: Union[float, int, np.ndarray] = None,
+        sc2: Union[float, int, np.ndarray] = None, wet_dry: Union[float, int, np.ndarray] = None,
+        ky: Union[float, int, np.ndarray] = None, kz: Union[float, int, np.ndarray] = None,
+        vkcb: Union[float, int, np.ndarray] = None, tkcb: Union[float, int, np.ndarray] = None)
+        Set COMUS Model GridCell Parameter Attributes.
+
+    load(cls, model, grid_params_file: str)
+         Load parameters from a BcfGrd.in or LpfGrd.in file and create a ComusGridPars instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusGridPars`
+        module to the specified path as <BcfGrd.in> or <LpfGrd.in>.
+
+    Returns:
+    --------
+    controlParams: pycomus.ComusGridPars
+        COMUS Grid Attribute Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="OneDimFlowSim")
+    >>> modelGridPar = pycomus.ComusGridPars(model1, top=50, bot=0, ibound=1, kx=1, shead=20)
+    """
     def __init__(self, model, top: Union[float, int, np.ndarray] = None, bot: Union[float, int, np.ndarray] = None,
                  ibound: Union[int, np.ndarray] = None, shead: Union[float, int, np.ndarray] = None,
                  kx: Union[float, int, np.ndarray] = None, transm: Union[float, int, np.ndarray] = None,
                  vcont: Union[float, int, np.ndarray] = None, sc1: Union[float, int, np.ndarray] = None,
                  sc2: Union[float, int, np.ndarray] = None, wet_dry: Union[float, int, np.ndarray] = None,
                  ky: Union[float, int, np.ndarray] = None, kz: Union[float, int, np.ndarray] = None,
                  vkcb: Union[float, int, np.ndarray] = None, tkcb: Union[float, int, np.ndarray] = None):
-        """
-        Set COMUS Model GridCell Parameter Attributes.
-
-        Parameters:
-        ----------------------------
-        model:
-            COMUS Model Object.
-        top:
-            A value of 0 indicates an inactive cell; 1 indicates a variable head cell; -1 indicates a constant head cell.
-        bot:
-            Represents the elevation of the bottom boundary of the grid cell (in length units).
-        ibound:
-            Represents the elevation of the top boundary of the grid cell (in length units).
-        shead:
-            The initial head value for the grid cell (L).
-        kx:
-            Permeability coefficient kx in the X-direction.
-        transm:
-            This represents the transmissivity of the grid cell in the row direction.
-        vcont:
-            The vertical hydraulic conductivity of the grid cell (1/T), also known as the leakage coefficient.
-        sc1:
-            Grid cell type 1 storage coefficient (-).
-        sc2:
-            Grid cell type 2 storage coefficient (-).
-        wet_dry:
-            The absolute value is the threshold by which the head in the adjacent cell must exceed the bottom elevation of the current cell to trigger wetting.
-        ky:
-            Permeability coefficient ky in the Y-direction.
-        kz:
-            Permeability coefficient kz in the Z-direction.
-        vkcb:
-            It represents the vertical hydraulic conductivity of the low-permeability medium at the bottom of the grid cell (L/T).
-        tkcb:
-            It denotes the thickness of the low-permeability medium at the bottom of the grid cell (L).
-
-        Returns:
-        --------
-        controlParams: pycomus.ComusGridPars
-            COMUS Grid Attribute Params Object.
-
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="OneDimFlowSim")
-        >>> modelGridPar = pycomus.ComusGridPars(model1, top=50, bot=0, ibound=1, kx=1, shead=20)
-        """
         cms_pars, cms_dis = self.__Check(model)
         self._model = model
         self._num_lyr = cms_dis.num_lyr
         self._num_row = cms_dis.num_row
         self._num_col = cms_dis.num_col
         self._intblkm = cms_pars.intblkm
         self._sim_type = cms_pars.sim_type
         self._lyr_type = [model.layers[i].lyr_type for i in range(self._num_lyr)]
-        model.package[GRID_PKG_NAME] = self
 
         # top Check
         if isinstance(top, np.ndarray):
             if top.size == 0:
                 top = 1
         elif not top:
             top = 1
@@ -298,14 +315,15 @@
                 if isinstance(sc2, float) or isinstance(sc2, int):
                     self.sc2 = np.full((self._num_lyr, self._num_row, self._num_col), sc2)
                 elif isinstance(sc2, np.ndarray) and sc2.shape == (self._num_lyr, self._num_row, self._num_col):
                     self.sc2 = sc2
                 else:
                     self.__ShowErrorMsg("sc2")
             self.__SetLpfPars()
+        model.package[GRID_PKG_NAME] = self
 
     @classmethod
     def load(cls, model, grid_params_file: str):
         """
         Load parameters from a BcfGrd.in or LpfGrd.in file and create a ComusGridPars instance.
 
         Parameters:
```

### Comparing `PyCOMUS-1.0.3/pycomus/ComusDis/CmsOutPars.py` & `pycomus-1.0.4/pycomus/ComusDis/CmsOutPars.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,85 +7,89 @@
 import os
 from typing import Dict, List
 
 from pycomus.Utils.CONSTANTS import OUT_PKG_NAME, OUT_FILE_NAME
 
 
 class ComusOutputPars:
-    def __init__(self, model, gdw_bd: int = 1, lyr_bd: int = 1, cell_bd: int = 1, cell_hh: int = 1,
+    """
+    Set COMUS Model Output Params Attributes.
+        0: No output;
+
+        1: Output for each simulation time step within a period;
+
+        2: Output for each period.
+
+
+    Attributes:
+    ----------------------------
+    model: pycomus.ComusModel
+        COMUS Model Object
+    gdw_bd: int
+        Groundwater system balance output control option.
+    lyr_bd: int
+        Layer balance output control option.
+    cell_bd: int
+        Grid cell balance output control option.
+    cell_hh: int
+        Grid cell head output control option.
+    cell_dd: int
+        Grid cell draw down output control option.
+    cell_flo: int
+        Inter-cell flow output control option.
+    lak_bd: int
+        Lake balance output control option.
+    segm_bd: int
+        Stream channel balance output control option.
+    rech_bd: int
+        Stream segment balance output control option.
+    ibs: int
+        Interbed simulation results output control option.
+    sub: int
+        Grid cell land subsidence simulation results output control option.
+    ndb: int
+        For no-delay interbed simulation results output control option.
+    db: int
+        For delayed interbed simulation results output control option.
+    reg_bd: int
+        Regional water balance output control option.
+
+    Methods:
+    --------
+    __init__(self, model, gdw_bd: int = 1, lyr_bd: int = 1, cell_bd: int = 1, cell_hh: int = 1,
                  cell_dd: int = 1, cell_flo: int = 1, lak_bd: int = 1, segm_bd: int = 1, rech_bd: int = 1,
-                 ibs: int = 1, sub: int = 1, ndb: int = 1, db: int = 1, reg_bd: int = 1):
-        """
+                 ibs: int = 1, sub: int = 1, ndb: int = 1, db: int = 1, reg_bd: int = 1)
         Set COMUS Model Output Params Attributes.
-            0: No output;
-
-            1: Output for each simulation time step within a period;
-
-            2: Output for each period.
 
+    load(cls, model, output_params_file: str)
+        Load parameters from a load OutOpt.in file and create a ComusOutputPars instance.
 
-        Parameters:
-        ----------------------------
-        model:
-            COMUS Model Object
-        gdw_bd: int
-            Groundwater system balance output control option.
-        lyr_bd: int
-            Layer balance output control option.
-        cell_bd: int
-            Grid cell balance output control option.
-        cell_hh: int
-            Grid cell head output control option.
-        cell_dd: int
-            Grid cell draw down output control option.
-        cell_flo: int
-            Inter-cell flow output control option.
-        lak_bd: int
-            Lake balance output control option.
-        segm_bd: int
-            Stream channel balance output control option.
-        rech_bd: int
-            Stream segment balance output control option.
-        ibs: int
-            Interbed simulation results output control option.
-        sub: int
-            Grid cell land subsidence simulation results output control option.
-        ndb: int
-            For no-delay interbed simulation results output control option.
-        db: int
-            For delayed interbed simulation results output control option.
-        reg_bd: int
-            Regional water balance output control option.
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusOutputPars`
+        module to the specified path as <OutOpt.in>.
 
-        Returns:
-        --------
-        instance: pycomus.ComusConPars
-            COMUS Control Params Object.
+    Returns:
+    --------
+    instance: pycomus.ComusConPars
+        COMUS Control Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="OneDimFlowSim")
+    >>> outParams = pycomus.ComusOutputPars(model1, 2, 2, 2, 2, 2, 2)
+    """
 
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="OneDimFlowSim")
-        >>> outParams = pycomus.ComusOutputPars(model1, 2, 2, 2, 2, 2, 2)
-        """
+    def __init__(self, model, gdw_bd: int = 1, lyr_bd: int = 1, cell_bd: int = 1, cell_hh: int = 1,
+                 cell_dd: int = 1, cell_flo: int = 1, lak_bd: int = 1, segm_bd: int = 1, rech_bd: int = 1,
+                 ibs: int = 1, sub: int = 1, ndb: int = 1, db: int = 1, reg_bd: int = 1):
         self.__params: Dict = {
-            'gdw_bd': gdw_bd,
-            'lyr_bd': lyr_bd,
-            'cell_bd': cell_bd,
-            'cell_hh': cell_hh,
-            'cell_dd': cell_dd,
-            'cell_flo': cell_flo,
-            'lak_bd': lak_bd,
-            'segm_bd': segm_bd,
-            'rech_bd': rech_bd,
-            'ibs': ibs,
-            'sub': sub,
-            'ndb': ndb,
-            'db': db,
-            'reg_bd': reg_bd,
+            'gdw_bd': gdw_bd, 'lyr_bd': lyr_bd, 'cell_bd': cell_bd, 'cell_hh': cell_hh, 'cell_dd': cell_dd,
+            'cell_flo': cell_flo, 'lak_bd': lak_bd, 'segm_bd': segm_bd, 'rech_bd': rech_bd, 'ibs': ibs,
+            'sub': sub, 'ndb': ndb, 'db': db, 'reg_bd': reg_bd
         }
         self._model = model
 
         for param_name, param_value in self.__params.items():
             if param_value not in {0, 1, 2}:
                 raise ValueError(f'"{param_name}" parameter is invalid. It should be between 0 and 2. Please check!')
 
@@ -135,29 +139,18 @@
         if len(lines[0].strip().split()) != 14:
             raise ValueError("The Output Params file should have 14 fields.")
 
         data: List[str] = lines[1].strip().split()
         if len(data) != 14:
             raise ValueError("The Output Params data line should have 14 values.")
 
-        instance = cls(model,
-                       gdw_bd=int(data[0]),
-                       lyr_bd=int(data[1]),
-                       cell_bd=int(data[2]),
-                       cell_hh=int(data[3]),
-                       cell_dd=int(data[4]),
-                       cell_flo=int(data[5]),
-                       lak_bd=int(data[6]),
-                       segm_bd=int(data[7]),
-                       rech_bd=int(data[8]),
-                       ibs=int(data[9]),
-                       sub=int(data[10]),
-                       ndb=int(data[11]),
-                       db=int(data[12]),
-                       reg_bd=int(data[13]))
+        instance = cls(model, gdw_bd=int(data[0]), lyr_bd=int(data[1]), cell_bd=int(data[2]), cell_hh=int(data[3]),
+                       cell_dd=int(data[4]), cell_flo=int(data[5]), lak_bd=int(data[6]), segm_bd=int(data[7]),
+                       rech_bd=int(data[8]), ibs=int(data[9]), sub=int(data[10]), ndb=int(data[11]),
+                       db=int(data[12]), reg_bd=int(data[13]))
         return instance
 
     def write_file(self, folder_path: str):
         """
         Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusOutputPars`
         module to the specified path as <OutOpt.in>.
```

### Comparing `PyCOMUS-1.0.3/pycomus/ComusDis/CmsPars.py` & `pycomus-1.0.4/pycomus/ComusDis/CmsPars.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,92 +10,111 @@
 import sys
 from typing import List
 
 from pycomus.Utils.CONSTANTS import CON_PKG_NAME, CON_FILE_NAME, BCF_LYR_PKG_NAME, LPF_LYR_PKG_NAME
 
 
 class ComusConPars:
+    """
+    Set COMUS Model Control Params Attributes.
 
-    def __init__(self, model, dim_unit: str = "m", time_unit: str = "day", sim_mtd: int = 1,
+    Attributes:
+    --------
+    model:
+        COMUS Model Object
+    dim_unit: str
+        The unit of spatial measurement (Length)
+    time_unit: str
+        The unit of spatial measurement (Time)
+    sim_mtd: int
+        The simulation method option. 1 for the ACC method; 2 for the original MODFLOW method.
+    sim_type: int
+        The simulation type option. 1 for steady-flow simulation; 2 for transient-flow simulation.
+    acc_lambda: float
+        It is the resistance coefficient in the additional term on the right side of the grid cell differential equation.
+    intblkm: int
+        Option for the input format of layer type and grid cell data. 1 for BCF format; 2 for LPF format.
+    solve: int
+        The option for the method of solving the matrix equation (1 for SIP; 2 for PCG).
+    max_iter: int
+        The maximum number of iterations for matrix solving.
+    damp: float
+        Iterative calculation damping factor (-), usually set to 1.0 (valid range: 0.0001~1.0).
+    h_close: float
+        The accuracy threshold for water level calculation (L).
+    r_close: float
+        Valid only when solve=2 (Preconditioned Conjugate Gradient Method).
+    relax: int
+        Option to enable the deep relaxation iterative algorithm.
+    theta: float
+        It is the reduction coefficient for the dynamic relaxation factor when oscillations occur during iterative calculations (-).
+    gamma: float
+        It is the increase coefficient for the dynamic relaxation factor.
+    akappa: float
+        It is the unit increase value for the dynamic relaxation factor.
+    n_iter: int
+        It is the number of consecutive non-oscillatory iterations required to increase the dynamic relaxation factor.
+    hno_flo: float
+        The water head value for invalid computational cells (L).
+    ch_flg: int
+        Option to calculate the flow between two adjacent fixed head cells.
+    wd_flg: int
+        An option indicating whether to simulate the conversion between dry and wet cells.
+    wet_fct: float
+        A multiplier for the trial thickness of the aquifer layer when a cell is reWetted.
+    newt_iter: int
+        The number of iterations between attempts to convert a cell from dry to wet.
+    hd_wet: int
+        An option for the algorithm to calculate the trial aquifer thickness when a cell is reWetted.
+    reg_sta: int
+        An option to enable the functionality for sub-regional water balance statistics.
+    mul_td: int
+        An option to enable multi-threaded parallel computation.
+    num_td: int
+        This parameter specifies the number of threads to use for parallel computation.
+
+    Methods:
+    --------
+    __init__(self, model, dim_unit: str = "m", time_unit: str = "day", sim_mtd: int = 1,
                  sim_type: int = 2, acc_lambda: float = -1, intblkm: int = 1, solve: int = 2,
                  max_iter: int = 200, damp: float = 1, h_close: float = 0.0001,
                  r_close: float = 0.001, relax: int = 0, theta: float = 0.7,
                  gamma: float = 3, akappa: float = 0.001, n_iter: int = 5,
                  hno_flo: float = -1E+30, ch_flg: int = 0, wd_flg: int = 0,
                  wet_fct: float = 0.1, newt_iter: int = 1, hd_wet: int = 1,
-                 reg_sta: int = 0, mul_td: int = 0, num_td: int = -1):
-        """
+                 reg_sta: int = 0, mul_td: int = 0, num_td: int = -1)
         Set COMUS Model Control Params Attributes.
 
-        Parameters:
-        --------
-        model:
-            COMUS Model Object
-        dim_unit: str
-            The unit of spatial measurement (Length)
-        time_unit: str
-            The unit of spatial measurement (Time)
-        sim_mtd: int
-            The simulation method option. 1 for the ACC method; 2 for the original MODFLOW method.
-        sim_type: int
-            The simulation type option. 1 for steady-flow simulation; 2 for transient-flow simulation.
-        acc_lambda: float
-            It is the resistance coefficient in the additional term on the right side of the grid cell differential equation.
-        intblkm: int
-            Option for the input format of layer type and grid cell data. 1 for BCF format; 2 for LPF format.
-        solve: int
-            The option for the method of solving the matrix equation (1 for SIP; 2 for PCG).
-        max_iter: int
-            The maximum number of iterations for matrix solving.
-        damp: float
-            Iterative calculation damping factor (-), usually set to 1.0 (valid range: 0.0001~1.0).
-        h_close: float
-            The accuracy threshold for water level calculation (L).
-        r_close: float
-            Valid only when solve=2 (Preconditioned Conjugate Gradient Method).
-        relax: int
-            Option to enable the deep relaxation iterative algorithm.
-        theta: float
-            It is the reduction coefficient for the dynamic relaxation factor when oscillations occur during iterative calculations (-).
-        gamma: float
-            It is the increase coefficient for the dynamic relaxation factor.
-        akappa: float
-            It is the unit increase value for the dynamic relaxation factor.
-        n_iter: int
-            It is the number of consecutive non-oscillatory iterations required to increase the dynamic relaxation factor.
-        hno_flo: float
-            The water head value for invalid computational cells (L).
-        ch_flg: int
-            Option to calculate the flow between two adjacent fixed head cells.
-        wd_flg: int
-            An option indicating whether to simulate the conversion between dry and wet cells.
-        wet_fct: float
-            A multiplier for the trial thickness of the aquifer layer when a cell is reWetted.
-        newt_iter: int
-            The number of iterations between attempts to convert a cell from dry to wet.
-        hd_wet: int
-            An option for the algorithm to calculate the trial aquifer thickness when a cell is reWetted.
-        reg_sta: int
-            An option to enable the functionality for sub-regional water balance statistics.
-        mul_td: int
-            An option to enable multi-threaded parallel computation.
-        num_td: int
-            This parameter specifies the number of threads to use for parallel computation.
+    load(cls, model, ctrl_params_file: str)
+        Load parameters from a CtrlPar.in file and create a ComusConPars instance.
 
-        Returns:
-        --------
-        controlParams: pycomus.ComusConPars
-            COMUS Control Params Object.
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusConPars`
+        module to the specified path as <CtrlPar.in>.
 
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> controlParams = pycomus.ComusConPars(model=model1, sim_type=1, max_iter=10000)
-        """
+    Returns:
+    --------
+    controlParams: pycomus.ComusConPars
+        COMUS Control Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> controlParams = pycomus.ComusConPars(model=model1, sim_type=1, max_iter=10000)
+    """
+
+    def __init__(self, model, dim_unit: str = "m", time_unit: str = "day", sim_mtd: int = 1,
+                 sim_type: int = 2, acc_lambda: float = -1, intblkm: int = 1, solve: int = 2,
+                 max_iter: int = 200, damp: float = 1, h_close: float = 0.0001,
+                 r_close: float = 0.001, relax: int = 0, theta: float = 0.7,
+                 gamma: float = 3, akappa: float = 0.001, n_iter: int = 5,
+                 hno_flo: float = -1E+30, ch_flg: int = 0, wd_flg: int = 0,
+                 wet_fct: float = 0.1, newt_iter: int = 1, hd_wet: int = 1,
+                 reg_sta: int = 0, mul_td: int = 0, num_td: int = -1):
         self._CheckLib = None
         self._model = model
         self.dim_unit: str = dim_unit
         self.time_unit: str = time_unit
         self.sim_mtd: int = sim_mtd
         self.sim_type: int = sim_type
         self.acc_lambda: float = acc_lambda
@@ -156,71 +175,25 @@
             raise ValueError("The Control Params file header should have 30 fields.")
 
         data = lines[1].strip().split()
         if len(data) != 30:
             raise ValueError("The Control Params data line should have 30 values.")
 
         params = {
-            'dim_unit': data[3],
-            'time_unit': data[4],
-            'sim_mtd': int(data[7]),
-            'sim_type': int(data[8]),
-            'acc_lambda': float(data[9]),
-            'intblkm': int(data[10]),
-            'solve': int(data[11]),
-            'max_iter': int(data[12]),
-            'damp': float(data[13]),
-            'h_close': float(data[14]),
-            'r_close': float(data[15]),
-            'relax': int(data[16]),
-            'theta': float(data[17]),
-            'gamma': float(data[18]),
-            'akappa': float(data[19]),
-            'n_iter': int(data[20]),
-            'hno_flo': float(data[21]),
-            'ch_flg': int(data[22]),
-            'wd_flg': int(data[23]),
-            'wet_fct': float(data[24]),
-            'newt_iter': int(data[25]),
-            'hd_wet': int(data[26]),
-            'reg_sta': int(data[27]),
-            'mul_td': int(data[28]),
+            'dim_unit': data[3], 'time_unit': data[4], 'sim_mtd': int(data[7]), 'sim_type': int(data[8]),
+            'acc_lambda': float(data[9]), 'intblkm': int(data[10]), 'solve': int(data[11]), 'max_iter': int(data[12]),
+            'damp': float(data[13]), 'h_close': float(data[14]), 'r_close': float(data[15]), 'relax': int(data[16]),
+            'theta': float(data[17]), 'gamma': float(data[18]), 'akappa': float(data[19]), 'n_iter': int(data[20]),
+            'hno_flo': float(data[21]), 'ch_flg': int(data[22]), 'wd_flg': int(data[23]), 'wet_fct': float(data[24]),
+            'newt_iter': int(data[25]), 'hd_wet': int(data[26]), 'reg_sta': int(data[27]), 'mul_td': int(data[28]),
             'num_td': int(data[29]),
         }
         instance = cls(model, **params)
         return instance
 
-    def _SetDlls(self):
-        current_file_path = os.path.abspath(__file__)
-        current_dir_path = os.path.dirname(current_file_path)
-        system = platform.system()
-        if system == 'Windows':
-            dll_path = os.path.join(current_dir_path, '.././Utils', 'WinCheckParams.dll')
-        elif system == 'Linux':
-            dll_path = os.path.join(current_dir_path, '.././Utils', 'LinuxCheckParams.so')
-        else:
-            raise ValueError("Pycomus only supports Windows and Linux systems.")
-        self._CheckLib = ctypes.CDLL(dll_path)
-        self._CheckLib.CheckCtrlParData.argtypes = [ctypes.c_int, ctypes.c_int, ctypes.c_double,
-                                                    ctypes.c_int, ctypes.c_int, ctypes.c_int, ctypes.c_double,
-                                                    ctypes.c_double, ctypes.c_double, ctypes.c_int,
-                                                    ctypes.c_double, ctypes.c_double, ctypes.c_double,
-                                                    ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                                                    ctypes.c_double, ctypes.c_int, ctypes.c_int,
-                                                    ctypes.c_int, ctypes.c_int, ctypes.c_int]
-        self._CheckLib.CheckCtrlParData.restype = ctypes.c_bool
-
-    def _Check(self):
-        if not self._CheckLib.CheckCtrlParData(self.sim_mtd, self.sim_type, self.acc_lambda, self.intblkm,
-                                               self.solve, self.max_iter, self.damp, self.h_close, self.r_close,
-                                               self.relax, self.theta, self.gamma, self.akappa, self.n_iter,
-                                               self.ch_flg, self.wd_flg, self.wet_fct, self.newt_iter,
-                                               self.hd_wet, self.reg_sta, self.mul_td, self.num_td):
-            sys.exit()
-
     def write_file(self, folder_path: str):
         """
         Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusConPars`
         module to the specified path as <CtrlPar.in>.
 
         :param folder_path: Output folder path.
         """
@@ -242,7 +215,35 @@
                        self.sim_type, self.acc_lambda, self.intblkm, self.solve, self.max_iter, self.damp, self.h_close,
                        self.r_close, self.relax, self.theta, self.gamma, self.akappa, self.n_iter, self.hno_flo,
                        self.ch_flg, self.wd_flg, self.wet_fct, self.newt_iter, self.hd_wet, self.reg_sta, self.mul_td,
                        self.num_td]
         with open(os.path.join(folder_path, CON_FILE_NAME), "w") as file:
             file.write(header_line + "\n")
             file.write('    '.join(map(str, conParsData)))
+
+    def _SetDlls(self):
+        current_file_path = os.path.abspath(__file__)
+        current_dir_path = os.path.dirname(current_file_path)
+        system = platform.system()
+        if system == 'Windows':
+            dll_path = os.path.join(current_dir_path, '.././Utils', 'WinCheckParams.dll')
+        elif system == 'Linux':
+            dll_path = os.path.join(current_dir_path, '.././Utils', 'LinuxCheckParams.so')
+        else:
+            raise ValueError("Pycomus only supports Windows and Linux systems.")
+        self._CheckLib = ctypes.CDLL(dll_path)
+        self._CheckLib.CheckCtrlParData.argtypes = [ctypes.c_int, ctypes.c_int, ctypes.c_double,
+                                                    ctypes.c_int, ctypes.c_int, ctypes.c_int, ctypes.c_double,
+                                                    ctypes.c_double, ctypes.c_double, ctypes.c_int,
+                                                    ctypes.c_double, ctypes.c_double, ctypes.c_double,
+                                                    ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                                                    ctypes.c_double, ctypes.c_int, ctypes.c_int,
+                                                    ctypes.c_int, ctypes.c_int, ctypes.c_int]
+        self._CheckLib.CheckCtrlParData.restype = ctypes.c_bool
+
+    def _Check(self):
+        if not self._CheckLib.CheckCtrlParData(self.sim_mtd, self.sim_type, self.acc_lambda, self.intblkm,
+                                               self.solve, self.max_iter, self.damp, self.h_close, self.r_close,
+                                               self.relax, self.theta, self.gamma, self.akappa, self.n_iter,
+                                               self.ch_flg, self.wd_flg, self.wet_fct, self.newt_iter,
+                                               self.hd_wet, self.reg_sta, self.mul_td, self.num_td):
+            sys.exit()
```

### Comparing `PyCOMUS-1.0.3/pycomus/ComusDis/CmsTime.py` & `pycomus-1.0.4/pycomus/ComusDis/CmsTime.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,37 +7,50 @@
 import os
 from typing import List, Tuple, Union
 
 from pycomus.Utils.CONSTANTS import PERIOD_FILE_NAME, PERIOD_PKG_NAME
 
 
 class ComusPeriod:
-    def __init__(self, model, period: Union[Tuple, List[Tuple]]):
-        """
+    """
+    Set COMUS Model Period Attributes.
+
+    Attributes:
+    ----------------------------
+    model: pycomus.ComusModel
+        COMUS Model Object.
+    period: Union[Tuple, List[Tuple]]
+        It can be a Tuple or a List[Tuple], and each Tuple should contain three elements, which are PERLEN, NSTEP
+         and MULTR, and each element should be greater than 0.
+
+    Methods:
+    --------
+    __init__(self, model, period: Union[Tuple, List[Tuple]])
         Set COMUS Model Period Attributes.
 
-        Parameters:
-        ----------------------------
-        model:
-            COMUS Model Object.
-        period:
-            It can be a Tuple or a List[Tuple], and each Tuple should contain three elements, which are PERLEN, NSTEP,
-             and MULTR, and each element should be greater than 0.
-
-        Returns:
-        --------
-        controlParams: pycomus.ComusPeriod
-            COMUS Period Attributes Object.
-
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> period1 = pycomus.ComusPeriod(model1, [(1, 1, 1)])
-        """
+    load(cls, model, period_file: str)
+        Load parameters from a PerAttr.in file and create a ComusPeriod instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusPeriod`
+        module to the specified path as <PerAttr.in>.
+
+    Returns:
+    --------
+    controlParams: pycomus.ComusPeriod
+        COMUS Period Attributes Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> period1 = pycomus.ComusPeriod(model1, [(1, 1, 1)])
+    """
+
+    def __init__(self, model, period: Union[Tuple, List[Tuple]]):
         self.period: Union[Tuple, List[Tuple]] = self._validate_period(period)
         self._model = model
         model.package[PERIOD_PKG_NAME] = self
 
     @staticmethod
     def _validate_period(period: Union[Tuple, List[Tuple]]) -> Union[Tuple, List[Tuple]]:
         if isinstance(period, tuple):
```

### Comparing `PyCOMUS-1.0.3/pycomus/ComusDis/GridLyr.py` & `pycomus-1.0.4/pycomus/ComusDis/GridLyr.py`

 * *Files identical despite different names*

### Comparing `PyCOMUS-1.0.3/pycomus/Package/CDRN.py` & `pycomus-1.0.4/pycomus/Package/CDRN.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,55 +12,75 @@
 
 import pycomus
 from pycomus.Utils import BoundaryCheck
 from pycomus.Utils.CONSTANTS import DRN_PKG_NAME, DRN_FILE_NAME
 
 
 class ComusDrn:
-    def __init__(self, model: pycomus.ComusModel,
-                 cond: Union[int, float, Dict[int, Union[int, float, np.ndarray]]] = None,
-                 delev: Union[int, float, Dict[int, Union[int, float, np.ndarray]]] = None):
-        """
+    """
+    Initialize the COMUS Model with the Drainage(DRN) package.
+
+    Attributes:
+    ----------------------------
+    model: pycomus.ComusModel
+        The COMUS model to which the DRN package will be applied.
+    cond: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]
+        The hydraulic conductivity coefficient between the drainage ditch and the aquifer at the grid cell (L²/T).
+    delev: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]
+        The elevation of the bottom of the drainage ditch at the grid cell (L).
+
+    Methods:
+    --------
+    __init__(self, model: pycomus.ComusModel,
+                 cond: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 delev: Union[int, float, Dict[int, Union[int, float, np.ndarray]]])
         Initialize the COMUS Model with the Drainage(DRN) package.
 
-        Parameters:
-        ----------------------------
-        model: pycomus.ComusModel
-            The COMUS model to which the DRN package will be applied.
-        cond: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]
-            The hydraulic conductivity coefficient between the drainage ditch and the aquifer at the grid cell (L²/T).
-        delev: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]
-            The elevation of the bottom of the drainage ditch at the grid cell (L).
-
-        Returns:
-        --------
-        instance: pycomus.ComusDrn
-           COMUS Drainage(DRN) Params Object.
-
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> drnPkg = pycomus.Package.ComusDrn(model, Cond={0: 1}, Delev={0: 20})
+    load(cls, model, drn_params_file: str)
+         Load parameters from a DRN.in file and create a ComusDrn instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusDrn`
+        module to the specified path as <DRN.in>.
+
+    Returns:
+    --------
+    instance: pycomus.ComusDrn
+       COMUS Drainage(DRN) Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> drnPkg = pycomus.Package.ComusDrn(model1, Cond={0: 1}, Delev={0: 20})
 
-        """
+    """
+
+    def __init__(self, model: pycomus.ComusModel,
+                 cond: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 delev: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]):
         BoundaryCheck.check_bnd_queue(model)
         cms_dis = BoundaryCheck.get_cms_pars(model)
         cms_period = BoundaryCheck.get_period(model)
         self._num_lyr = cms_dis.num_lyr
         self._num_row = cms_dis.num_row
         self._num_col = cms_dis.num_col
         self._period = cms_period.period
         self._model = model
         if cond:
             self.cond = BoundaryCheck.CheckValueGtZero(cond, "Cond", self._period, self._num_lyr,
                                                        self._num_row, self._num_col)
+        else:
+            raise ValueError("Cond parameter not set!")
         if delev:
             self.delev = BoundaryCheck.CheckValueFormat(delev, "Delev", self._period, self._num_lyr,
                                                         self._num_row, self._num_col)
+        else:
+            raise ValueError("Delev parameter not set!")
+
         if cond and delev:
             if sorted(self.cond.keys()) != sorted(self.delev.keys()):
                 raise ValueError("The periods for the 'Cond' parameter and 'Delev' should be the same.")
         model.package[DRN_PKG_NAME] = self
 
     @classmethod
     def load(cls, model, drn_params_file: str):
```

### Comparing `PyCOMUS-1.0.3/pycomus/Package/CEVT.py` & `pycomus-1.0.4/pycomus/Package/CEVT.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,52 +12,68 @@
 
 import pycomus
 from pycomus.Utils import BoundaryCheck
 from pycomus.Utils.CONSTANTS import EVT_PKG_NAME, EVT_FILE_NAME
 
 
 class ComusEvt:
-    def __init__(self, model: pycomus.ComusModel, et_surf: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+    """
+    Initialize the COMUS Model with the Evapotranspiration(EVT) package.
+
+    Attributes:
+    ----------------------------
+    model: pycomus.ComusModel
+        The COMUS model to which the EVT package will be applied.
+    et_surf: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]
+        The elevation of the subsurface evaporation interface at the grid cell (L).
+    et_rate: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]
+        The potential (maximum) subsurface evaporation intensity at the grid cell (L/T).
+    et_mxd: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]
+        The limit depth for subsurface evaporation at the grid cell (L).
+    et_exp: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]
+        The subsurface evaporation exponent at the grid cell.
+    evt: int
+        Subsurface evaporation calculation option. 1: Calculate subsurface evaporation for specified layer grid cells;
+        2: Calculate subsurface evaporation for the highest layer effective
+    num_seg: int
+        The number of segments in the curve representing the change of subsurface evaporation with depth at the grid cell,
+        with a minimum of 2 segments and a maximum of 20 segments.
+
+    Methods:
+    --------
+    __init__(self, model: pycomus.ComusModel, et_surf: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
                  et_rate: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
                  et_mxd: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
                  et_exp: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
-                 evt: int = 1, num_seg: int = 10):
-        """
+                 evt: int = 1, num_seg: int = 10)
         Initialize the COMUS Model with the Evapotranspiration(EVT) package.
 
-        Parameters:
-        ----------------------------
-        model: pycomus.ComusModel
-            The COMUS model to which the EVT package will be applied.
-        et_surf: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]
-            The elevation of the subsurface evaporation interface at the grid cell (L).
-        et_rate: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]
-            The potential (maximum) subsurface evaporation intensity at the grid cell (L/T).
-        et_mxd: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]
-            The limit depth for subsurface evaporation at the grid cell (L).
-        et_exp: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]
-            The subsurface evaporation exponent at the grid cell.
-        evt: int
-            Subsurface evaporation calculation option. 1: Calculate subsurface evaporation for specified layer grid cells;
-            2: Calculate subsurface evaporation for the highest layer effective
-        num_seg: int
-            The number of segments in the curve representing the change of subsurface evaporation with depth at the grid cell,
-            with a minimum of 2 segments and a maximum of 20 segments.
-
-        Returns:
-        --------
-        instance: pycomus.ComusEvt
-           COMUS Evapotranspiration(EVT) Params Object.
-
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> evtPkg = pycomus.ComusEvt(model1, et_surf=1, et_rate=1, et_mxd=1, et_exp=1)
-        """
+    load(cls, model: pycomus.ComusModel, evt_params_file: str)
+         Load parameters from a EVT.in file and create a ComusEvt instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusEvt`
+        module to the specified path as <EVT.in>.
+
+    Returns:
+    --------
+    instance: pycomus.ComusEvt
+       COMUS Evapotranspiration(EVT) Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> evtPkg = pycomus.ComusEvt(model1, et_surf=1, et_rate=1, et_mxd=1, et_exp=1)
+    """
+    def __init__(self, model: pycomus.ComusModel, et_surf: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 et_rate: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 et_mxd: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 et_exp: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 evt: int = 1, num_seg: int = 10):
         BoundaryCheck.check_bnd_queue(model)
         cms_dis = BoundaryCheck.get_cms_pars(model)
         cms_period = BoundaryCheck.get_period(model)
         self._num_lyr = cms_dis.num_lyr
         self._num_row = cms_dis.num_row
         self._num_col = cms_dis.num_col
         self._period = cms_period.period
```

### Comparing `PyCOMUS-1.0.3/pycomus/Package/CGHB.py` & `pycomus-1.0.4/pycomus/Package/CSHB.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,169 +1,168 @@
 # --------------------------------------------------------------
-# CGHB.py
+# CSHB.py
 # Version: 1.0.0
 # Author: Zhenjiang Wu
-# Description: Set COMUS Model With GHB Package.
+# Description: Set COMUS Model With SHB Package.
 # --------------------------------------------------------------
 import os
 import sys
 from typing import Union, Dict
 
 import numpy as np
 
 import pycomus
 from pycomus.Utils import BoundaryCheck
-from pycomus.Utils.CONSTANTS import GHB_PKG_NAME, GHB_FILE_NAME
+from pycomus.Utils.CONSTANTS import SHB_PKG_NAME, SHB_FILE_NAME
 
 
-class ComusGhb:
-    def __init__(self, model: pycomus.ComusModel, cond: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
-                 shead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
-                 ehead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]):
-        """
-        Initialize the COMUS Model with the General-Head Boundary(GHB) package.
-
-        Parameters:
-        ----------------------------
-        model:
-            The COMUS model to which the GHB package will be applied.
-        Cond:
-            The hydraulic conductivity coefficient between the general head and the aquifer (L²/T).
-        Shead:
-            The general head value at the beginning of the stress period (L).
-        Ehead:
-            The general head value at the end of the stress period (L).
+class ComusShb:
+    """
+    Initialize the COMUS Model with the Transient Specified-Head Boundary(SHB) package.
+
+    Parameters:
+    ----------------------------
+    model:
+        The COMUS model to which the SHB package will be applied.
+    shead:
+        The hydraulic head value of the grid cell at the beginning of the stress period (L).
+    ehead:
+        The hydraulic head value of the grid cell at the end of the stress period (L).
+
+    Methods:
+    --------
+    __init__(self, model: pycomus.ComusModel, shead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 ehead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]])
+        Initialize the COMUS Model with the Transient Specified-Head Boundary(SHB) package.
+
+    load(cls, model, shb_params_file: str)
+          Load parameters from a SHB.in file and create a ComusShb instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusShb`
+        module to the specified path as <SHB.in>.
+
+    Returns:
+    --------
+    instance: pycomus.ComusShb
+       COMUS Transient Specified-Head Boundary(SHB) Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> shbPackage = pycomus.ComusShb(model1, shead=1, ehead=2)
+    """
 
-        Returns:
-        --------
-        instance: pycomus.ComusGhb
-           COMUS General-Head Boundary(GHB) Params Object.
-
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> ghbPkg = pycomus.ComusGhb(model1, cond={0: 1}, shead=1, ehead=2)
-        """
+    def __init__(self, model: pycomus.ComusModel, shead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 ehead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]):
         BoundaryCheck.check_bnd_queue(model)
         cms_dis = BoundaryCheck.get_cms_pars(model)
         cms_period = BoundaryCheck.get_period(model)
         self._num_lyr = cms_dis.num_lyr
         self._num_row = cms_dis.num_row
         self._num_col = cms_dis.num_col
         self._period = cms_period.period
-        self.cond = BoundaryCheck.CheckValueGtZero(cond, "Cond", self._period, self._num_lyr,
-                                                   self._num_row, self._num_col)
+        self._model = model
         self.shead = BoundaryCheck.CheckValueFormat(shead, "Shead", self._period, self._num_lyr,
                                                     self._num_row, self._num_col)
         self.ehead = BoundaryCheck.CheckValueFormat(ehead, "Ehead", self._period, self._num_lyr,
                                                     self._num_row, self._num_col)
-        if sorted(self.cond.keys()) != sorted(self.shead.keys()) != sorted(self.ehead.keys()):
-            raise ValueError("The stress periods for the 'Cond' parameter,'Ehead' and 'Shead' should be the same.")
-        self._model = model
-        model.package[GHB_PKG_NAME] = self
+        if sorted(self.shead.keys()) != sorted(self.ehead.keys()):
+            raise ValueError("The stress periods for the 'Shead' parameter and 'Ehead' should be the same.")
+        model.package[SHB_PKG_NAME] = self
 
     @classmethod
-    def load(cls, model, ghb_params_file: str):
+    def load(cls, model, shb_params_file: str):
         """
-        Load parameters from a GHB.in file and create a ComusGhb instance.
+        Load parameters from a SHB.in file and create a ComusShb instance.
 
         Parameters:
         --------
         model: pycomus.ComusModel
             COMUS Model Object.
-        ghb_params_file: str
-            Grid GHB Params File Path(GHB.in).
+        shb_params_file: str
+            Grid SHB Params File Path(SHB.in).
 
         Returns:
         --------
-        instance: pycomus.ComusGhb
-            COMUS General-Head Boundary(GHB) Params Object.
+        instance: pycomus.ComusShb
+            COMUS Transient Specified-Head Boundary(SHB) Params Object.
 
         Example:
         --------
         >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> ghbPackage = pycomus.ComusGhb.load(model1, "./InputFiles/DRN.in")
+        >>> model1 = pycomus.ComusModel(model_name="OneDimFlowSim(File-Input)")
+        >>> shbPackage = pycomus.ComusShb.load(model, "./InputFiles/SHB.in")
         """
         BoundaryCheck.check_bnd_queue(model)
         cms_dis = BoundaryCheck.get_cms_pars(model)
         num_lyr = cms_dis.num_lyr
         num_row = cms_dis.num_row
         num_col = cms_dis.num_col
-        with open(ghb_params_file, 'r') as file:
+        with open(shb_params_file, 'r') as file:
             lines = file.readlines()
-        if len(lines[0].strip().split()) != 7:
-            raise ValueError("The General-Head Boundary(GHB) Period Attribute file header should have 7 fields.")
+        if len(lines[0].strip().split()) != 6:
+            raise ValueError(
+                "The Transient Specified-Head Boundary(SHB) Period Attribute file header should have 6 fields.")
         data = lines[1].strip().split()
-        if len(data) != 7:
-            raise ValueError("The General-Head Boundary(GHB) Period Attribute file data line should have 7 values.")
+        if len(data) != 6:
+            raise ValueError(
+                "The Transient Specified-Head Boundary(SHB) Period Attribute file data line should have 6 values.")
         lines = lines[1:]
-        cond = {}
         shead = {}
         ehead = {}
         for line in lines:
             line = line.strip().split()
             period = int(line[0]) - 1
             lyr = int(line[1]) - 1
             row = int(line[2]) - 1
             col = int(line[3]) - 1
-            if period not in cond:
+            if period not in shead:
                 shead[period] = np.zeros((num_lyr, num_row, num_col))
                 ehead[period] = np.zeros((num_lyr, num_row, num_col))
-                cond[period] = np.zeros((num_lyr, num_row, num_col))
             shead[period][lyr, row, col] = float(line[4])
             ehead[period][lyr, row, col] = float(line[5])
-            cond[period][lyr, row, col] = float(line[6])
-        instance = cls(model, cond=cond, shead=shead, ehead=ehead)
+        instance = cls(model, shead=shead, ehead=ehead)
         return instance
 
     def __str__(self):
-        res = f"{GHB_PKG_NAME}:\n"
-        for period, value in self.cond.items():
+        res = f"{SHB_PKG_NAME}: \n"
+        for period, value in self.shead.items():
             res += f"    Period : {period}\n        Value Shape : {value.shape}\n"
         return res
 
     def write_file(self, folder_path: str):
         """
-        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusGhb`
-        module to the specified path as <GHB.in>.
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusShb`
+        module to the specified path as <SHB.in>.
 
         :param folder_path: Output folder path.
         """
         if not self._write_file_test(folder_path):
-            os.remove(os.path.join(folder_path, GHB_FILE_NAME))
+            os.remove(os.path.join(folder_path, SHB_FILE_NAME))
             sys.exit()
 
     def _write_file_test(self, folder_path: str) -> bool:
-        flag = 0
         period_len = len(self._period)
-        with open(os.path.join(folder_path, GHB_FILE_NAME), "w") as file:
-            file.write("IPER  ILYR  IROW  ICOL  SHEAD  EHEAD  COND\n")
-            periods = sorted(self.cond.keys())
+        with open(os.path.join(folder_path, SHB_FILE_NAME), "w") as file:
+            file.write("IPER  ILYR  IROW  ICOL  SHEAD  EHEAD\n")
+            periods = sorted(self.shead.keys())
             for period in periods:
                 if not BoundaryCheck.check_period(period, period_len):
                     return False
-                cond_value = self.cond[period]
                 shead_value = self.shead[period]
                 ehead_value = self.ehead[period]
-                if not BoundaryCheck.check_dict_zero(cond_value, "Cond", self._num_lyr, self._num_row, self._num_col):
-                    return False
                 for layer in range(self._num_lyr):
-                    lyr_type: int = self._model.layers[layer].lyr_type
                     for row in range(self._num_row):
                         for col in range(self._num_col):
-                            if cond_value[layer, row, col] > 0:
-                                if lyr_type in (1, 3):
-                                    bot = self._model.layers[layer].grid_cells[row][col].bot
-                                    if shead_value[layer, row, col] <= bot or ehead_value[layer, row, col] <= bot:
-                                        print(f"The hydraulic head at grid cell ({layer},{row},{col}) cannot be lower "
-                                              f"than or equal to the bottom elevation of the grid cell.")
-                                        return False
+                            if shead_value[layer, row, col] != 0 and ehead_value[layer, row, col] != 0:
+                                ibound = self._model.layers[layer].grid_cells[row][col].ibound
+                                if ibound <= 0:
+                                    print(
+                                        f"DRN Package:The grid cell with the ID ({layer},{row},{col}) is initialized as an "
+                                        f"invalid cell or a steady-state head cell. It cannot be set as an SHB cell during the %dth stress period.")
+                                    return False
                                 file.write(
                                     f"{period + 1}  {layer + 1}  {row + 1}  {col + 1}  {shead_value[layer, row, col]}  "
-                                    f"{ehead_value[layer, row, col]}  {cond_value[layer, row, col]}\n")
-                                if period == 0:
-                                    flag += 1
-                if flag == 0 and period == 0:
-                    file.write("1  1  1  1  0  1E+100  1E+100\n")
+                                    f"{ehead_value[layer, row, col]}\n")
         return True
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PyCOMUS-1.0.3/pycomus/Package/CHFB.py` & `pycomus-1.0.4/pycomus/Package/CHFB.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,39 +9,52 @@
 
 import pycomus
 from pycomus.Utils import BoundaryCheck
 from pycomus.Utils.CONSTANTS import HFB_PKG_NAME, HFB_FILE_NAME
 
 
 class ComusHfb:
-    def __init__(self, model: pycomus.ComusModel, hfb_data: List[Tuple[int, int, int, int, int, Union[int, float]]]):
-        """
+    """
+    Initialize the COMUS Model with the Horizontal-Flow Barrier(HFB) package.
+
+    Attributes:
+    ----------------------------
+    model:
+        The COMUS model to which the HFB package will be applied.
+    hfb_data:
+        List[Tuple] type data, in which the Tuple should contain six parameters: ILYR, IROW1, ICOL1, IROW2, ICOL2, HCDW.
+
+    Methods:
+    --------
+    __init__(self, model: pycomus.ComusModel, hfb_data: List[Tuple[int, int, int, int, int, Union[int, float]]])
         Initialize the COMUS Model with the Horizontal-Flow Barrier(HFB) package.
 
-        Parameters:
-        ----------------------------
-        model:
-            The COMUS model to which the HFB package will be applied.
-        hfb_data:
-            List[Tuple] type data, in which the Tuple should contain six parameters: ILYR, IROW1, ICOL1, IROW2, ICOL2, HCDW.
-
-        Returns:
-        --------
-        instance: pycomus.ComusHfb
-           COMUS Horizontal-Flow Barrier(HFB) Params Object.
-
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> data = []
-        >>> for i in range(36):
-        >>>     data.append((i, 0, 15, 0, 16, 1e-6))
-        >>> hfbPackage = pycomus.ComusHfb(model=model1, hfb_data=data)
-        """
+    load(cls, model, hfb_params_file: str)
+         Load parameters from a HFB.in file and create a ComusHfb instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusHfb`
+        module to the specified path as <HFB.in>.
+
+    Returns:
+    --------
+    instance: pycomus.ComusHfb
+       COMUS Horizontal-Flow Barrier(HFB) Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> data = []
+    >>> for i in range(36):
+    >>>     data.append((i, 0, 15, 0, 16, 1e-6))
+    >>> hfbPackage = pycomus.ComusHfb(model=model1, hfb_data=data)
+    """
+
+    def __init__(self, model: pycomus.ComusModel, hfb_data: List[Tuple[int, int, int, int, int, Union[int, float]]]):
         BoundaryCheck.check_bnd_queue(model)
         cms_dis: Union[pycomus.ComusDisLpf, pycomus.ComusDisBcf] = BoundaryCheck.get_cms_pars(model)
         self._num_lyr: int = cms_dis.num_lyr
         self._num_row: int = cms_dis.num_row
         self._num_col: int = cms_dis.num_col
         self.hfb_data: List[Tuple[int, int, int, int, int, Union[int, float]]] = self.__CheckData(hfb_data)
         self._model: pycomus.ComusModel = model
```

### Comparing `PyCOMUS-1.0.3/pycomus/Package/CIBS.py` & `pycomus-1.0.4/pycomus/Package/CIBS.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,44 +11,59 @@
 
 import pycomus
 from pycomus.Utils import BoundaryCheck
 from pycomus.Utils.CONSTANTS import IBS_PKG_NAME, IBS_FILE_NAME
 
 
 class ComusIbs:
-    def __init__(self, model: pycomus.ComusModel, hc: Union[int, float, np.ndarray],
+    """
+    Initialize the COMUS Model with the Interbed Storage(IBS) package.
+
+    Attributes:
+    ----------------------------
+    model:
+        The COMUS model to which the IBS package will be applied.
+    hc:
+        Preconsolidation head (L) of interbedded bodies within the grid cell.
+    sfe:
+        Elastic storage coefficient (-) of interbedded bodies within the grid cell.
+    sfv:
+        Inelastic (plastic) storage coefficient (-) of interbedded bodies within the grid cell.
+    com:
+        Historical compression amount (L) of interbedded bodies within the grid cell.
+
+    Methods:
+    --------
+    __init__(self, model: pycomus.ComusModel, hc: Union[int, float, np.ndarray],
                  sfe: Union[int, float, np.ndarray], sfv: Union[int, float, np.ndarray],
-                 com: Union[int, float, np.ndarray]):
-        """
+                 com: Union[int, float, np.ndarray])
         Initialize the COMUS Model with the Interbed Storage(IBS) package.
 
-        Parameters:
-        ----------------------------
-        model:
-            The COMUS model to which the IBS package will be applied.
-        hc:
-            Preconsolidation head (L) of interbedded bodies within the grid cell.
-        sfe:
-            Elastic storage coefficient (-) of interbedded bodies within the grid cell.
-        sfv:
-            Inelastic (plastic) storage coefficient (-) of interbedded bodies within the grid cell.
-        com:
-            Historical compression amount (L) of interbedded bodies within the grid cell.
-
-        Returns:
-        --------
-        instance: pycomus.ComusIbs
-           COMUS Interbed Storage(IBS) Params Object.
-
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> ibsPackage = pycomus.ComusIbs(model1, hc=1, sfe=1, sfv=1, com=1)
-        """
+    load(cls, model, ibs_file: str)
+         Load parameters from a IBS.in file and create a ComusIbs instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusIbs`
+        module to the specified path as <IBS.in>.
+
+    Returns:
+    --------
+    instance: pycomus.ComusIbs
+       COMUS Interbed Storage(IBS) Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> ibsPackage = pycomus.ComusIbs(model1, hc=1, sfe=1, sfv=1, com=1)
+    """
+
+    def __init__(self, model: pycomus.ComusModel, hc: Union[int, float, np.ndarray],
+                 sfe: Union[int, float, np.ndarray], sfv: Union[int, float, np.ndarray],
+                 com: Union[int, float, np.ndarray]):
         BoundaryCheck.check_bnd_queue(model)
         cms_dis = BoundaryCheck.get_cms_pars(model)
         self._num_lyr = cms_dis.num_lyr
         self._num_row = cms_dis.num_row
         self._num_col = cms_dis.num_col
         self._model = model
         self.hc = BoundaryCheck.check_3d_format(hc, "HC", self._num_lyr, self._num_row, self._num_col)
```

### Comparing `PyCOMUS-1.0.3/pycomus/Package/CLAK.py` & `pycomus-1.0.4/pycomus/Package/CLAK.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,36 +11,63 @@
 import numpy as np
 
 from pycomus.Utils import BoundaryCheck
 from pycomus.Utils.CONSTANTS import LAK_PKG_NAME, LAK_CTRL_FILE_NAME, LAK_PERIOD_FILE_NAME, LAK_GRID_FILE_NAME
 
 
 class ComusLak:
-    def __init__(self, model, lake_num: int):
-        """
+    """
+    Initialize the COMUS Model with the Lake(LAK) package.
+
+    Attributes:
+    ----------------------------
+    model:
+        COMUS Model Object.
+    lake_num:
+        Number of lakes.
+
+    Methods:
+    --------
+    __init__(self, model, lake_num: int)
         Initialize the COMUS Model with the Lake(LAK) package.
 
-        Parameters:
-        ----------------------------
-        model:
-            COMUS Model Object.
-        lake_num:
-            Number of lakes.
-
-        Returns:
-        --------
-        instance: pycomus.ComusLak
-           COMUS Lake(LAK) Params Object.
-
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> lakPackage = pycomus.ComusLak(model1, lake_num=1)
-        """
+    set_control_params(self, control_params: Dict[
+        int, Tuple[int, int, int, float, float, float, float, float, int, float, float, float, float]])
+        Set Lake Control Params.
+
+    set_period_data(self, period_data: Dict[
+        int, Dict[int, Tuple[float, float, float, float, float, float, float, float]]])
+        Set Lake Period Data.
+
+    set_grid_data(self, btm: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                      lnk: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                      sc1: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                      sc2: Union[int, float, Dict[int, Union[int, float, np.ndarray]]])
+        Set Lake Grid Cell Data.
+
+    load(cls, model, ctrl_pars_file: str, period_file: str, grid_file: str)
+         Load parameters from LAK(LAKCtrl.in, LAKPer.in, LAKGrd.in) file and create a ComusLak instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusLak`
+        module to the specified path as <LAKCtrl.in>, <LAKPer.in> and <LAKGrd.in>.
+
+    Returns:
+    --------
+    instance: pycomus.ComusLak
+       COMUS Lake(LAK) Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> lakPackage = pycomus.ComusLak(model1, lake_num=1)
+    """
+
+    def __init__(self, model, lake_num: int):
         if lake_num < 1:
             raise ValueError("The number of lakes should be greater than or equal to 1.")
         BoundaryCheck.check_bnd_queue(model)
         cms_dis = BoundaryCheck.get_cms_pars(model)
         cms_period = BoundaryCheck.get_period(model)
         self._num_lyr = cms_dis.num_lyr
         self._num_row = cms_dis.num_row
@@ -48,15 +75,15 @@
         self._period = cms_period.period
         self._lake_num = lake_num
         self.lakeValue: Lak = Lak()
         self._model = model
         model.package[LAK_PKG_NAME] = self
 
     def set_control_params(self, control_params: Dict[
-            int, Tuple[int, int, int, float, float, float, float, float, int, float, float, float, float]]) -> None:
+        int, Tuple[int, int, int, float, float, float, float, float, int, float, float, float, float]]) -> None:
         """
         Set Lake Control Params.
 
         :param control_params:
             A Dict type data where the keys represent the lake IDs, and the values are Tuples containing 13
             elements: STRID, DIVSID, DIVSAT, BETA, INIHLEV, DEADHLEV, EVEXP, EVMAXD, NUMSEG, STRBED, STRWDT, STRNDC, STRSLP.
         """
@@ -102,20 +129,20 @@
             if str_id != 0:
                 if str_wdt <= 0 or str_ndc <= 0 or str_slp <= 0:
                     raise ValueError(
                         f"Lake number {lak_id} has downstream river reach units. Parameters like STRWDT, STRNDC, STRSLP, etc., must be greater than 0.0. Please verify!")
         self.lakeValue.ControlParams = control_params
 
     def set_period_data(self, period_data: Dict[
-            int, Dict[int, Tuple[float, float, float, float, float, float, float, float]]]) -> None:
+        int, Dict[int, Tuple[float, float, float, float, float, float, float, float]]]) -> None:
         """
-        Set Reservoir Period Data.
+        Set Lake Period Data.
 
         :param period_data:
-            A Dict type data where the keys represent the Period IDs, and the values are Dicts with reservoir IDs as
+            A Dict type data where the keys represent the Period IDs, and the values are Dicts with lake IDs as
             keys. Within the inner Dicts, the values are Tuples containing four elements: PCP, RNFCOF, PRHCOF,
              ET0, EVWBCOF, GEVCOF, WATDIV, WATUSE.
         """
         for period_id, periodData in period_data.items():
             if not (0 <= period_id < len(self._period)):
                 raise ValueError(
                     f"Invalid key {period_id} in period_data dictionary. Keys should be in the range 0 to {len(self._period) - 1}.")
@@ -154,15 +181,15 @@
         self.lakeValue.PeriodData = period_data
 
     def set_grid_data(self, btm: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
                       lnk: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
                       sc1: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
                       sc2: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]) -> None:
         """
-        Set Reservoir Grid Cell Data.
+        Set Lake Grid Cell Data.
 
         :param btm:
             Lake bed elevation (L) at the grid cell of the lake.
         :param lnk:
             Overland flow coefficient (1/T) between the lake bed and the aquifer.
         :param sc1:
             Storage coefficient (-) when the grid cell of the lake is under pressure condition.
```

### Comparing `PyCOMUS-1.0.3/pycomus/Package/CRCH.py` & `pycomus-1.0.4/pycomus/Package/CRCH.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,41 +12,55 @@
 
 import pycomus
 from pycomus.Utils import BoundaryCheck
 from pycomus.Utils.CONSTANTS import RCH_PKG_NAME, RCH_FILE_NAME
 
 
 class ComusRch:
-    def __init__(self, model: pycomus.ComusModel, rechr: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
-                 rech: int):
-        """
+    """
+    Set COMUS Model With Recharge(RCH) Package.
+
+    Attributes:
+    ----------------------------
+    model:
+        COMUS Model Object.
+    rechr:
+        The rate of areal recharge to the grid cell (L/T). This value must be greater than or equal to 0.
+    rech:
+        The computation option for areal recharge. The value 1 indicates that areal recharge is calculated for specified layer grid cells; 2 indicates that areal recharge is calculated for the highest active grid cells in the model.
+
+    Methods:
+    --------
+    __init__(self, model: pycomus.ComusModel, rechr: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 rech: int)
         Set COMUS Model With Recharge(RCH) Package.
 
-        Parameters:
-        ----------------------------
-        model:
-            COMUS Model Object.
-        rechr:
-            The rate of areal recharge to the grid cell (L/T). This value must be greater than or equal to 0.
-        rech:
-            The computation option for areal recharge. The value 1 indicates that areal recharge is calculated for specified layer grid cells; 2 indicates that areal recharge is calculated for the highest active grid cells in the model.
-
-        Returns:
-        --------
-        instance: pycomus.ComusRch
-           COMUS Recharge(RCH) Params Object.
-
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> recharge = np.zeros((40, 1, 100))
-        >>> recharge[0, 0, 49:52] = 0.0015
-        >>> rchPkg = pycomus.ComusRch(model1, rechr={0: recharge}, rech=1)
-        """
+    load(cls, model, rch_params_file: str)
+         Load parameters from a RCH.in file and create a ComusRch instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusRch`
+        module to the specified path as <RCH.in>.
+
+    Returns:
+    --------
+    instance: pycomus.ComusRch
+       COMUS Recharge(RCH) Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> recharge = np.zeros((40, 1, 100))
+    >>> recharge[0, 0, 49:52] = 0.0015
+    >>> rchPkg = pycomus.ComusRch(model1, rechr={0: recharge}, rech=1)
+    """
+
+    def __init__(self, model: pycomus.ComusModel, rechr: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 rech: int):
         BoundaryCheck.check_bnd_queue(model)
         cms_dis = BoundaryCheck.get_cms_pars(model)
         cms_period = BoundaryCheck.get_period(model)
         self._num_lyr = cms_dis.num_lyr
         self._num_row = cms_dis.num_row
         self._num_col = cms_dis.num_col
         self._period = cms_period.period
```

### Comparing `PyCOMUS-1.0.3/pycomus/Package/CREG.py` & `pycomus-1.0.4/pycomus/Package/CREG.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,39 +9,52 @@
 
 import pycomus
 from pycomus.Utils import BoundaryCheck
 from pycomus.Utils.CONSTANTS import REG_PKG_NAME, REG_FILE_NAME
 
 
 class ComusReg:
-    def __init__(self, model: pycomus.ComusModel, reg_data: Dict[str, Dict[str, List[Tuple[int, int, int]]]]):
-        """
+    """
+    Initialize the COMUS Model with the Region Statistics tool.
+
+    Attributes:
+    ----------------------------
+    model: pycomus.ComusModel
+        The COMUS model to which the IBS package will be applied.
+    reg_data: Dict[str, Dict[str, List[Tuple[int, int, int]]]]
+        The `reg_data` is a nested dictionary. The keys of the outer dictionary are the names of the statistical
+        schemes, and the values are dictionaries. The keys of the inner dictionary are the names of the statistical
+        partitions, and the values are a list of tuples, where each tuple represents the layer number, row number
+        , and column number.
+
+    Methods:
+    --------
+    __init__(self, model: pycomus.ComusModel, reg_data: Dict[str, Dict[str, List[Tuple[int, int, int]]]])
         Initialize the COMUS Model with the Region Statistics tool.
 
-        Parameters:
-        ----------------------------
-        model: pycomus.ComusModel
-            The COMUS model to which the IBS package will be applied.
-        reg_data: Dict[str, Dict[str, List[Tuple[int, int, int]]]]
-            The `reg_data` is a nested dictionary. The keys of the outer dictionary are the names of the statistical
-            schemes, and the values are dictionaries. The keys of the inner dictionary are the names of the statistical
-            partitions, and the values are a list of tuples, where each tuple represents the layer number, row number
-            , and column number.
-
-        Returns:
-        --------
-        instance: pycomus.ComusReg
-           COMUS Region Statistics Params Object.
-
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> reg_sta = pycomus.ComusReg(model,{"scheme1": {"par1": [(0,0,0), (0,0,1), (1,1,1)]}})
-        """
+    load(cls, model, reg_file: str)
+        Load parameters from a RegSta.in file and create a ComusReg instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusReg`
+        module to the specified path as <RegSta.in>.
+
+    Returns:
+    --------
+    instance: pycomus.ComusReg
+       COMUS Region Statistics Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> reg_sta = pycomus.ComusReg(model1,{"scheme1": {"par1": [(0,0,0), (0,0,1), (1,1,1)]}})
+    """
+
+    def __init__(self, model: pycomus.ComusModel, reg_data: Dict[str, Dict[str, List[Tuple[int, int, int]]]]):
 
         BoundaryCheck.check_bnd_queue(model)
         cms_dis = BoundaryCheck.get_cms_pars(model)
         cms_pars = BoundaryCheck.get_con_pars(model)
         self._num_lyr = cms_dis.num_lyr
         self._num_row = cms_dis.num_row
         self._num_col = cms_dis.num_col
```

### Comparing `PyCOMUS-1.0.3/pycomus/Package/CRES.py` & `pycomus-1.0.4/pycomus/Package/CRES.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,36 +11,60 @@
 import numpy as np
 
 from pycomus.Utils import BoundaryCheck
 from pycomus.Utils.CONSTANTS import RES_PKG_NAME, RES_CTRL_FILE_NAME, RES_PERIOD_FILE_NAME, RES_GRID_FILE_NAME
 
 
 class ComusRes:
-    def __init__(self, model, res_num: int):
-        """
+    """
+    Initialize the COMUS Model with the Reservoir(RES) package.
+
+    Attributes:
+    ----------------------------
+    model:
+        COMUS Model Object.
+    res_num:
+        Number of reservoirs.
+
+    Methods:
+    --------
+    __init__(self, model, res_num: int)
         Initialize the COMUS Model with the Reservoir(RES) package.
 
-        Parameters:
-        ----------------------------
-        model:
-            COMUS Model Object.
-        res_num:
-            Number of reservoirs.
-
-        Returns:
-        --------
-        instance: pycomus.ComusRes
-           COMUS Reservoir(RES) Params Object.
-
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> resPackage = pycomus.ComusRes(model1, res_num=1)
-        """
+    set_control_params(self, control_params: Dict[int, Tuple[float, float, int, int]])
+        Set Reservoir Control Params.
+
+    set_period_data(self, period_data: Dict[int, Dict[int, Tuple[float, float, float, float]]])
+        Set Reservoir Period Data.
+
+    set_grid_data(self, btm: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                      bvk: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                      btk: Union[int, float, Dict[int, Union[int, float, np.ndarray]]])
+        Set Reservoir Grid Cell Data.
+
+    load(cls, model, ctrl_pars_file: str, period_file: str, grid_file: str)
+         Load parameters from RES(RESCtrl.in, RESPer.in, RESGrd.in) file and create a ComusRes instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusRes`
+        module to the specified path as <RESCtrl.in>, <RESPer.in> and <RESGrd.in>.
+
+    Returns:
+    --------
+    instance: pycomus.ComusRes
+       COMUS Reservoir(RES) Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> resPackage = pycomus.ComusRes(model1, res_num=1)
+    """
+
+    def __init__(self, model, res_num: int):
         if res_num < 1:
             raise ValueError("The number of reservoirs should be greater than or equal to 1.")
         self._res_num = res_num
         BoundaryCheck.check_bnd_queue(model)
         cms_dis = BoundaryCheck.get_cms_pars(model)
         cms_period = BoundaryCheck.get_period(model)
         self._num_lyr = cms_dis.num_lyr
```

### Comparing `PyCOMUS-1.0.3/pycomus/Package/CRIV.py` & `pycomus-1.0.4/pycomus/Package/CRIV.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,45 +12,61 @@
 
 import pycomus
 from pycomus.Utils import BoundaryCheck
 from pycomus.Utils.CONSTANTS import RIV_PKG_NAME, RIV_FILE_NAME
 
 
 class ComusRiv:
-    def __init__(self, model: pycomus.ComusModel, cond: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+    """
+    Initialize the COMUS Model with the River(RIV) package.
+
+    Attributes:
+    ----------------------------
+    model:
+        The COMUS model to which the RIV package will be applied.
+    cond:
+        The hydraulic conductivity coefficient between the river and the aquifer on the grid cell (L²/T)
+    shead:
+        The river stage at the beginning of the stress period (L)
+    ehead:
+        The river stage at the end of the stress period (L)
+    riv_btm:
+        The elevation of the bottom of the low permeability medium in the riverbed on the grid cell (L).
+
+    Methods:
+    --------
+    __init__(self, model: pycomus.ComusModel, cond: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
                  shead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
                  ehead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
-                 riv_btm: Union[int, float, Dict[int, Union[int, float, np.ndarray]]], ):
-        """
+                 riv_btm: Union[int, float, Dict[int, Union[int, float, np.ndarray]]])
         Initialize the COMUS Model with the River(RIV) package.
 
-        Parameters:
-        ----------------------------
-        model:
-            The COMUS model to which the RIV package will be applied.
-        cond:
-            The hydraulic conductivity coefficient between the river and the aquifer on the grid cell (L²/T)
-        shead:
-            The river stage at the beginning of the stress period (L)
-        ehead:
-            The river stage at the end of the stress period (L)
-        riv_btm:
-            The elevation of the bottom of the low permeability medium in the riverbed on the grid cell (L).
-
-        Returns:
-        --------
-        instance: pycomus.ComusRiv
-           COMUS River(RIV) Params Object.
-
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> rivPackage = pycomus.ComusRiv(model1, cond=1, shead=1, ehead=2, riv_btm=10)
-        """
+    load(cls, model, riv_params_file: str)
+          Load parameters from a RIV.in file and create a ComusRiv instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusRiv`
+        module to the specified path as <RIV.in>.
+
+    Returns:
+    --------
+    instance: pycomus.ComusRiv
+       COMUS River(RIV) Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> rivPackage = pycomus.ComusRiv(model1, cond=1, shead=1, ehead=2, riv_btm=10)
+    """
+
+    def __init__(self, model: pycomus.ComusModel, cond: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 shead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 ehead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 riv_btm: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]):
         BoundaryCheck.check_bnd_queue(model)
         cms_dis = BoundaryCheck.get_cms_pars(model)
         cms_period = BoundaryCheck.get_period(model)
         self._num_lyr = cms_dis.num_lyr
         self._num_row = cms_dis.num_row
         self._num_col = cms_dis.num_col
         self._period = cms_period.period
```

### Comparing `PyCOMUS-1.0.3/pycomus/Package/CSHB.py` & `pycomus-1.0.4/pycomus/Package/CGHB.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,154 +1,184 @@
 # --------------------------------------------------------------
-# CSHB.py
+# CGHB.py
 # Version: 1.0.0
 # Author: Zhenjiang Wu
-# Description: Set COMUS Model With SHB Package.
+# Description: Set COMUS Model With GHB Package.
 # --------------------------------------------------------------
 import os
 import sys
 from typing import Union, Dict
 
 import numpy as np
 
 import pycomus
 from pycomus.Utils import BoundaryCheck
-from pycomus.Utils.CONSTANTS import SHB_PKG_NAME, SHB_FILE_NAME
+from pycomus.Utils.CONSTANTS import GHB_PKG_NAME, GHB_FILE_NAME
 
 
-class ComusShb:
-    def __init__(self, model: pycomus.ComusModel, shead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
-                 ehead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]):
-        """
-        Initialize the COMUS Model with the Transient Specified-Head Boundary(SHB) package.
+class ComusGhb:
+    """
+    Initialize the COMUS Model with the General-Head Boundary(GHB) package.
+
+    Attributes:
+    ----------------------------
+    model:
+        The COMUS model to which the GHB package will be applied.
+    Cond:
+        The hydraulic conductivity coefficient between the general head and the aquifer (L²/T).
+    Shead:
+        The general head value at the beginning of the stress period (L).
+    Ehead:
+        The general head value at the end of the stress period (L).
+
+    Methods:
+    --------
+    __init__(self, model: pycomus.ComusModel, cond: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 shead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 ehead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]])
+        Initialize the COMUS Model with the General-Head Boundary(GHB) package.
+
+    load(cls, model, ghb_params_file: str)
+          Load parameters from a GHB.in file and create a ComusGhb instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusGhb`
+        module to the specified path as <GHB.in>.
+
+    Returns:
+    --------
+    instance: pycomus.ComusGhb
+       COMUS General-Head Boundary(GHB) Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> ghbPkg = pycomus.ComusGhb(model1, cond={0: 1}, shead=1, ehead=2)
+    """
 
-        Parameters:
-        ----------------------------
-        model:
-            The COMUS model to which the SHB package will be applied.
-        shead:
-            The hydraulic head value of the grid cell at the beginning of the stress period (L).
-        ehead:
-            The hydraulic head value of the grid cell at the end of the stress period (L).
-
-        Returns:
-        --------
-        instance: pycomus.ComusShb
-           COMUS Transient Specified-Head Boundary(SHB) Params Object.
-
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> shbPackage = pycomus.ComusShb(model1, shead=1, ehead=2)
-        """
+    def __init__(self, model: pycomus.ComusModel, cond: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 shead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 ehead: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]):
         BoundaryCheck.check_bnd_queue(model)
         cms_dis = BoundaryCheck.get_cms_pars(model)
         cms_period = BoundaryCheck.get_period(model)
         self._num_lyr = cms_dis.num_lyr
         self._num_row = cms_dis.num_row
         self._num_col = cms_dis.num_col
         self._period = cms_period.period
-        self._model = model
+        self.cond = BoundaryCheck.CheckValueGtZero(cond, "Cond", self._period, self._num_lyr,
+                                                   self._num_row, self._num_col)
         self.shead = BoundaryCheck.CheckValueFormat(shead, "Shead", self._period, self._num_lyr,
                                                     self._num_row, self._num_col)
         self.ehead = BoundaryCheck.CheckValueFormat(ehead, "Ehead", self._period, self._num_lyr,
                                                     self._num_row, self._num_col)
-        if sorted(self.shead.keys()) != sorted(self.ehead.keys()):
-            raise ValueError("The stress periods for the 'Shead' parameter and 'Ehead' should be the same.")
-        model.package[SHB_PKG_NAME] = self
+        if sorted(self.cond.keys()) != sorted(self.shead.keys()) != sorted(self.ehead.keys()):
+            raise ValueError("The stress periods for the 'Cond' parameter,'Ehead' and 'Shead' should be the same.")
+        self._model = model
+        model.package[GHB_PKG_NAME] = self
 
     @classmethod
-    def load(cls, model, shb_params_file: str):
+    def load(cls, model, ghb_params_file: str):
         """
-        Load parameters from a SHB.in file and create a ComusShb instance.
+        Load parameters from a GHB.in file and create a ComusGhb instance.
 
         Parameters:
         --------
         model: pycomus.ComusModel
             COMUS Model Object.
-        shb_params_file: str
-            Grid SHB Params File Path(SHB.in).
+        ghb_params_file: str
+            Grid GHB Params File Path(GHB.in).
 
         Returns:
         --------
-        instance: pycomus.ComusShb
-            COMUS Transient Specified-Head Boundary(SHB) Params Object.
+        instance: pycomus.ComusGhb
+            COMUS General-Head Boundary(GHB) Params Object.
 
         Example:
         --------
         >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="OneDimFlowSim(File-Input)")
-        >>> shbPackage = pycomus.ComusShb.load(model, "./InputFiles/SHB.in")
+        >>> model1 = pycomus.ComusModel(model_name="test")
+        >>> ghbPackage = pycomus.ComusGhb.load(model1, "./InputFiles/DRN.in")
         """
         BoundaryCheck.check_bnd_queue(model)
         cms_dis = BoundaryCheck.get_cms_pars(model)
         num_lyr = cms_dis.num_lyr
         num_row = cms_dis.num_row
         num_col = cms_dis.num_col
-        with open(shb_params_file, 'r') as file:
+        with open(ghb_params_file, 'r') as file:
             lines = file.readlines()
-        if len(lines[0].strip().split()) != 6:
-            raise ValueError(
-                "The Transient Specified-Head Boundary(SHB) Period Attribute file header should have 6 fields.")
+        if len(lines[0].strip().split()) != 7:
+            raise ValueError("The General-Head Boundary(GHB) Period Attribute file header should have 7 fields.")
         data = lines[1].strip().split()
-        if len(data) != 6:
-            raise ValueError(
-                "The Transient Specified-Head Boundary(SHB) Period Attribute file data line should have 6 values.")
+        if len(data) != 7:
+            raise ValueError("The General-Head Boundary(GHB) Period Attribute file data line should have 7 values.")
         lines = lines[1:]
+        cond = {}
         shead = {}
         ehead = {}
         for line in lines:
             line = line.strip().split()
             period = int(line[0]) - 1
             lyr = int(line[1]) - 1
             row = int(line[2]) - 1
             col = int(line[3]) - 1
-            if period not in shead:
+            if period not in cond:
                 shead[period] = np.zeros((num_lyr, num_row, num_col))
                 ehead[period] = np.zeros((num_lyr, num_row, num_col))
+                cond[period] = np.zeros((num_lyr, num_row, num_col))
             shead[period][lyr, row, col] = float(line[4])
             ehead[period][lyr, row, col] = float(line[5])
-        instance = cls(model, shead=shead, ehead=ehead)
+            cond[period][lyr, row, col] = float(line[6])
+        instance = cls(model, cond=cond, shead=shead, ehead=ehead)
         return instance
 
     def __str__(self):
-        res = f"{SHB_PKG_NAME}: \n"
-        for period, value in self.shead.items():
+        res = f"{GHB_PKG_NAME}:\n"
+        for period, value in self.cond.items():
             res += f"    Period : {period}\n        Value Shape : {value.shape}\n"
         return res
 
     def write_file(self, folder_path: str):
         """
-        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusShb`
-        module to the specified path as <SHB.in>.
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusGhb`
+        module to the specified path as <GHB.in>.
 
         :param folder_path: Output folder path.
         """
         if not self._write_file_test(folder_path):
-            os.remove(os.path.join(folder_path, SHB_FILE_NAME))
+            os.remove(os.path.join(folder_path, GHB_FILE_NAME))
             sys.exit()
 
     def _write_file_test(self, folder_path: str) -> bool:
+        flag = 0
         period_len = len(self._period)
-        with open(os.path.join(folder_path, SHB_FILE_NAME), "w") as file:
-            file.write("IPER  ILYR  IROW  ICOL  SHEAD  EHEAD\n")
-            periods = sorted(self.shead.keys())
+        with open(os.path.join(folder_path, GHB_FILE_NAME), "w") as file:
+            file.write("IPER  ILYR  IROW  ICOL  SHEAD  EHEAD  COND\n")
+            periods = sorted(self.cond.keys())
             for period in periods:
                 if not BoundaryCheck.check_period(period, period_len):
                     return False
+                cond_value = self.cond[period]
                 shead_value = self.shead[period]
                 ehead_value = self.ehead[period]
+                if not BoundaryCheck.check_dict_zero(cond_value, "Cond", self._num_lyr, self._num_row, self._num_col):
+                    return False
                 for layer in range(self._num_lyr):
+                    lyr_type: int = self._model.layers[layer].lyr_type
                     for row in range(self._num_row):
                         for col in range(self._num_col):
-                            if shead_value[layer, row, col] != 0 and ehead_value[layer, row, col] != 0:
-                                ibound = self._model.layers[layer].grid_cells[row][col].ibound
-                                if ibound <= 0:
-                                    print(
-                                        f"DRN Package:The grid cell with the ID ({layer},{row},{col}) is initialized as an "
-                                        f"invalid cell or a steady-state head cell. It cannot be set as an SHB cell during the %dth stress period.")
-                                    return False
+                            if cond_value[layer, row, col] > 0:
+                                if lyr_type in (1, 3):
+                                    bot = self._model.layers[layer].grid_cells[row][col].bot
+                                    if shead_value[layer, row, col] <= bot or ehead_value[layer, row, col] <= bot:
+                                        print(f"The hydraulic head at grid cell ({layer},{row},{col}) cannot be lower "
+                                              f"than or equal to the bottom elevation of the grid cell.")
+                                        return False
                                 file.write(
                                     f"{period + 1}  {layer + 1}  {row + 1}  {col + 1}  {shead_value[layer, row, col]}  "
-                                    f"{ehead_value[layer, row, col]}\n")
+                                    f"{ehead_value[layer, row, col]}  {cond_value[layer, row, col]}\n")
+                                if period == 0:
+                                    flag += 1
+                if flag == 0 and period == 0:
+                    file.write("1  1  1  1  0  1E+100  1E+100\n")
         return True
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PyCOMUS-1.0.3/pycomus/Package/CSTR.py` & `pycomus-1.0.4/pycomus/Package/CSTR.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,25 +12,90 @@
 
 from pycomus.Utils import BoundaryCheck
 from pycomus.Utils.CONSTANTS import STR_PKG_NAME, STR_WAT_DRN_FILE_NAME, STR_WAT_USE_FILE_NAME, STR_GRID_FILE_NAME, \
     STR_PERIOD_FILE_NAME, STR_CTRL_FILE_NAME
 
 
 class ComusStr:
-    def __init__(self, model, stream_num: int):
-        """
+    """
+    Initialize the COMUS Model with the Stream(STR) package.
+
+    Attributes:
+    ----------------------------
+    model:
+       COMUS Model Object.
+    stream_num:
+       Number of streams.
+
+    Methods:
+    --------
+    __init__(self, model, stream_num: int)
         Initialize the COMUS Model with the Stream(STR) package.
 
-        Parameters:
-        ----------------------------
-        model:
-           COMUS Model Object.
-        stream_num:
-           Number of streams.
-        """
+    set_ControlData(self, control_params: Dict[int, Tuple[int, int, int, int, int, int, int, int, int]])
+        Set Stream Control Params.
+
+    set_PeriodData(self, period_data: Dict[int, Dict[
+        int, Tuple[int, float, float, float, float, float, float, float, float, float, float, float]]])
+        Set Stream Period Data.
+
+    set_GridData(self, cell_id: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                     length: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                     btm: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                     bwdt: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                     sizh1: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                     sizh2: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                     bvk: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                     btk: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                     slp: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                     ndc: Union[int, float, Dict[int, Union[int, float, np.ndarray]]])
+        Set Stream Grid Cell Data.
+
+    set_WatUseData(self, wureg_id: Union[int, np.ndarray], ratio: Union[int, float, np.ndarray])
+        Set Stream Water Use Data.
+
+    set_WatDrnData(self, delev: Union[int, np.ndarray], cond: Union[int, float, np.ndarray],
+                       segm_id: Union[int, float, np.ndarray])
+        Set Stream Water Drn Data.
+
+    load_ctrlPars_file(self, ctrlParFile)
+        Load data from <STRCtrl.in>.
+
+    load_period_file(self, period_file: str)
+        Load data from <STRPer.in>.
+
+    load_strGrid_file(self, strGridFile: str)
+        Load data from <STRGrd.in>.
+
+    load_watUse_file(self, watUseFile: str)
+        Load data from <STRWatUse.in>.
+
+    load_watDrn_file(self, watDrnFile: str)
+        Load data from <STRWatDrn.in>.
+
+    load(cls, model, ctrl_pars_file: str, period_file: str, grid_file: str, watUse_file: str, watDrn_file: str):
+        Load parameters from STR(STRCtrl.in, RESPer.in, RESGrd.in, STRWatUse.in, STRWatDrn.in) file and create a ComusStr instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusStr`
+        module to the specified path as <STRCtrl.in>, <STRPer.in>, <STRGrd.in>, <STRWatUse.in>, <STRWatDrn.in>.
+
+    Returns:
+    --------
+    instance: pycomus.ComusStr
+       COMUS Stream(STR) Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> strPackage = pycomus.ComusStr(model1, stream_num=1)
+    """
+
+    def __init__(self, model, stream_num: int):
         if stream_num < 1:
             raise ValueError("The number of streams should be greater than or equal to 1.")
         self._stream_num = stream_num
         BoundaryCheck.check_bnd_queue(model)
         cms_dis = BoundaryCheck.get_cms_pars(model)
         cms_period = BoundaryCheck.get_period(model)
         self._num_lyr = cms_dis.num_lyr
@@ -225,15 +290,15 @@
                      btm: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
                      bwdt: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
                      sizh1: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
                      sizh2: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
                      bvk: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
                      btk: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
                      slp: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
-                     ndc: Union[int, float, Dict[int, Union[int, float, np.ndarray]]], ) -> None:
+                     ndc: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]) -> None:
         """
         Set Stream Grid Cell Data.
 
         :param cell_id:
             cell_id is an integer representing the sequential upstream and downstream order of the river segment within
             its parent river unit (1 indicates that the river segment is the first segment of the river unit).
         :param length:
@@ -316,14 +381,19 @@
         delev = BoundaryCheck.check_3d_format(delev, "DELEV", self._num_lyr, self._num_row, self._num_col)
         cond = BoundaryCheck.check_3d_zero(cond, "COND", self._num_lyr, self._num_row, self._num_col)
         segm_id = BoundaryCheck.Check3DValueExistGrid(segm_id, "SEGMID", self._num_lyr, self._num_row,
                                                       self._num_col, SegIdList)
         self.streamValue.WatDrnData = {"DELEV": delev, "COND": cond, "SEGMID": segm_id}
 
     def load_ctrlPars_file(self, ctrlParFile):
+        """
+        Load data from <STRCtrl.in>.
+
+        :param ctrlParFile: Stream Control Parameters File.
+        """
         with open(ctrlParFile, 'r') as file:
             lines = file.readlines()
         if len(lines[0].strip().split()) != 10:
             raise ValueError("The Stream(STR) Control Params Attribute file header should have 10 fields.")
         data = lines[1].strip().split()
         if len(data) != 10:
             raise ValueError("The Stream(STR) Control Params Attribute file data line should have 10 values.")
@@ -336,14 +406,19 @@
                 ctrl_pars_data[stream_id] = (int(line[1]), int(line[2]), int(line[3]), int(line[4]), int(line[5]),
                                              int(line[6]), int(line[7]), int(line[8]), int(line[9]))
             else:
                 raise ValueError(f"The stream ID {stream_id} already exists. Stream IDs should be unique.")
         self.streamValue.ControlParams = ctrl_pars_data
 
     def load_period_file(self, period_file: str):
+        """
+        Load data from <STRPer.in>.
+
+        :param period_file: Stream Period Parameters File.
+        """
         with open(period_file, 'r') as file:
             lines = file.readlines()
         if len(lines[0].strip().split()) != 14:
             raise ValueError("The Stream(STR) Period Params Attribute file(STRPer.txt) header should have 14 fields.")
         if len(lines[1].strip().split()) != 14:
             raise ValueError(
                 "The Stream(STR) Period Params Attribute file(STRPer.txt) data line should have 14 values.")
@@ -358,14 +433,19 @@
             if period_id not in period_data[stream_id]:
                 period_data[stream_id][period_id] = (
                     int(line[2]), float(line[3]), float(line[4]), float(line[5]), float(line[6]), float(line[7]),
                     float(line[8]), float(line[9]), float(line[10]), float(line[11]), float(line[12]), float(line[13]))
         self.streamValue.PeriodData = period_data
 
     def load_strGrid_file(self, strGridFile: str):
+        """
+        Load data from <STRGrd.in>.
+
+        :param strGridFile: Stream Grid Cell Parameters File.
+        """
         with open(strGridFile, 'r') as file:
             CELLID = {}
             LEN = {}
             BTM = {}
             BWDT = {}
             SIZH1 = {}
             SIZH2 = {}
@@ -424,14 +504,19 @@
                     NDC[int_parts[0] - 1] = np.zeros((self._num_lyr, self._num_row, self._num_col))
                 NDC[int_parts[0] - 1][int_parts[2] - 1, int_parts[3] - 1, int_parts[4] - 1] = float_part[8]
 
             self.streamValue.GridData = {"CELLID": CELLID, "LEN": LEN, "BTM": BTM, "BWDT": BWDT, "SIZH1": SIZH1,
                                          "SIZH2": SIZH2, "BVK": BVK, "BTK": BTK, "SLP": SLP, "NDC": NDC}
 
     def load_watUse_file(self, watUseFile: str):
+        """
+        Load data from <STRWatUse.in>.
+
+        :param watUseFile: Stream Water Use Parameters File.
+        """
         with open(watUseFile, 'r') as file:
             WUREGID = np.zeros((self._num_lyr, self._num_row, self._num_col))
             RATIO = np.zeros((self._num_lyr, self._num_row, self._num_col))
             for line_num, line in enumerate(file, start=1):
                 if line_num == 1:
                     continue
                 line = line.strip()
@@ -442,14 +527,19 @@
                 int_parts = [int(part) for part in parts[:4]]
                 float_part = float(parts[4])
                 WUREGID[int_parts[1] - 1, int_parts[2] - 1, int_parts[3] - 1] = int_parts[0]
                 RATIO[int_parts[1] - 1, int_parts[2] - 1, int_parts[3] - 1] = float_part
             self.streamValue.WatUseData = {"WUREGID": WUREGID, "RATIO": RATIO}
 
     def load_watDrn_file(self, watDrnFile: str):
+        """
+        Load data from <STRWatDrn.in>.
+
+        :param watDrnFile: Stream Water Drn Parameters File.
+        """
         with open(watDrnFile, 'r') as file:
             DELEV = np.zeros((self._num_lyr, self._num_row, self._num_col))
             COND = np.zeros((self._num_lyr, self._num_row, self._num_col))
             SEGMID = np.zeros((self._num_lyr, self._num_row, self._num_col))
             for line_num, line in enumerate(file, start=1):
                 if line_num == 1:
                     continue
@@ -471,15 +561,15 @@
             return False
         sorted_keys = sorted(key_list)
         return sorted_keys == list(range(sorted_keys[0], sorted_keys[-1] + 1))
 
     @classmethod
     def load(cls, model, ctrl_pars_file: str, period_file: str, grid_file: str, watUse_file: str, watDrn_file: str):
         """
-        Load parameters from STR(STRCtrl.in, RESPer.in, RESGrd.in) file and create a ComusStr instance.
+        Load parameters from STR(STRCtrl.in, RESPer.in, RESGrd.in, STRWatUse.in, STRWatDrn.in) file and create a ComusStr instance.
 
         Parameters:
         --------
         model: pycomus.ComusModel
             COMUS Model Object.
         ctrl_pars_file: str
             STR Control Params File Path(STRCtrl.in).
```

### Comparing `PyCOMUS-1.0.3/pycomus/Package/CSUB.py` & `pycomus-1.0.4/pycomus/Package/CSUB.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,49 +12,83 @@
 import pycomus
 from pycomus.Utils import BoundaryCheck
 from pycomus.Utils.CONSTANTS import SUB_PKG_NAME, SUB_DB_GRID_FILE_NAME, SUB_NDB_GRID_FILE_NAME, SUB_DB_FILE_NAME, \
     SUB_NDB_FILE_NAME, SUB_MZ_FILE_NAME, SUB_CTRL_FILE_NAME
 
 
 class ComusSub:
-    def __init__(self, model: pycomus.ComusModel, num_ndb: int, num_db: int, num_mz: int, nn: int = 20,
+    """
+    Initialize the COMUS Model with the Subsidence(SUB) package.
+
+    Attributes:
+    ----------------------------
+    model:
+        The COMUS model to which the SUB package will be applied.
+    num_ndb:
+        Number of delayed interbedded body groups without delay.
+    num_db:
+        Number of delayed interbedded bodies.
+    num_mz:
+        Only valid when num_ndb > 0, indicating the number of media zones.
+    nn:
+        Number of discrete points on the half thickness of equivalent interbedded bodies.
+    acc:
+        Representing the simulation acceleration parameter of delayed interbedded bodies.
+    it_min:
+        The effective value should be greater than or equal to 2, typically set to 5.
+    dsh_opt:
+        Representing the option for determining the initial head values of delayed interbedded bodies.
+
+    Methods:
+    --------
+    __init__(self, model: pycomus.ComusModel, num_ndb: int, num_db: int, num_mz: int, nn: int = 20,
                  acc: float = 0.5, it_min: int = 5, dsh_opt: int = 2):
-        """
         Initialize the COMUS Model with the Subsidence(SUB) package.
 
-        Parameters:
-        ----------------------------
-        model:
-            The COMUS model to which the SUB package will be applied.
-        num_ndb:
-            Number of delayed interbedded body groups without delay.
-        num_db:
-            Number of delayed interbedded bodies.
-        num_mz:
-            Only valid when num_ndb > 0, indicating the number of media zones.
-        nn:
-            Number of discrete points on the half thickness of equivalent interbedded bodies.
-        acc:
-            Representing the simulation acceleration parameter of delayed interbedded bodies.
-        it_min:
-            The effective value should be greater than or equal to 2, typically set to 5.
-        dsh_opt:
-            Representing the option for determining the initial head values of delayed interbedded bodies.
-
-        Returns:
-        --------
-        instance: pycomus.ComusSub
-           COMUS Subsidence(SUB) Params Object.
-
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> subPackage = pycomus.ComusSub(model, 2, 2, 10)
-        """
+    set_mz_data(self, mz_data: Union[Dict[int, Tuple[float, float, float]], List[Tuple[float, float, float]]])
+        Set MZ Data.
+
+    set_ndb_lyr(self, ndb_lyr: Union[Dict[int, int], List[int]])
+        Set No Delay Interbeds Layer Property.
+
+    set_ndb_grid(self, hc: Union[int, float, np.ndarray], sfe: Union[int, float, np.ndarray],
+                     sfv: Union[int, float, np.ndarray], com: Union[int, float, np.ndarray])
+        Set No Delay Interbeds Grid Cell Property.
+
+    set_db_lyr(self, db_lyr: Union[Dict[int, int], List[int]])
+        Set Delay Interbeds Layer Property.
+
+    set_db_grid(self, rnb: Union[int, float, np.ndarray], dsh: Union[int, float, np.ndarray],
+                    dhc: Union[int, float, np.ndarray], dcom: Union[int, float, np.ndarray],
+                    dz: Union[int, float, np.ndarray], imz: Union[int, float, np.ndarray])
+        Set Delay Interbeds Grid Cell Property.
+
+    load(cls, model, ctrl_file: str, mz_file: str, ndb_lyr_file: str, ndb_grid_file: str, db_lyr_file: str,
+             db_grid_file: str)
+        Load parameters from SUB(SUBCtrl.in, SUBMZ.in, SUBNDB.in, SUBGrdNDB.in, SUBDB.in, SUBGrdDB.in) file and
+        create a ComusSub instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusSub`
+        module to the specified path as <SUBCtrl.in>, <SUBMZ.in>, <SUBNDB.in>, <SUBDB.in>, <SUBGrdNDB.in>, <SUBGrdDB.in>.
+
+    Returns:
+    --------
+    instance: pycomus.ComusSub
+       COMUS Subsidence(SUB) Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> subPackage = pycomus.ComusSub(model1, 2, 2, 10)
+    """
+
+    def __init__(self, model: pycomus.ComusModel, num_ndb: int, num_db: int, num_mz: int, nn: int = 20,
+                 acc: float = 0.5, it_min: int = 5, dsh_opt: int = 2):
 
         BoundaryCheck.check_bnd_queue(model)
         cms_dis = BoundaryCheck.get_cms_pars(model)
         cms_period = BoundaryCheck.get_period(model)
         self._num_lyr = cms_dis.num_lyr
         self._num_row = cms_dis.num_row
         self._num_col = cms_dis.num_col
@@ -83,17 +117,17 @@
         self._dsh_opt = dsh_opt
         self.subValue: LandSub = LandSub()
         self.subValue.ctrl_params = (num_ndb, num_db, num_mz, nn, acc, it_min, dsh_opt)
         model.package[SUB_PKG_NAME] = self
 
     def set_mz_data(self, mz_data: Union[Dict[int, Tuple[float, float, float]], List[Tuple[float, float, float]]]):
         """
+        Set MZ Data.
 
-        :param mz_data:
-        :return:
+        :param mz_data: Union[Dict[int, Tuple[float, float, float]], List[Tuple[float, float, float]]]
         """
         mz_data_len = len(mz_data)
         mz_dict_data: Dict = {}
         if mz_data_len != self._num_mz:
             raise ValueError(f"The length of mz_data should be consistent with num_mz({self._num_mz})!")
         if isinstance(mz_data, dict):
             if sorted(mz_data.keys()) != [i for i in range(self._num_mz)]:
@@ -111,17 +145,17 @@
             if value[0] < 0 or value[1] < 0 or value[2] < 0:
                 raise ValueError(
                     "The fields MZVK, MZSFE, and MZSFV must be greater than or equal to 0.0. Please check!")
         self.subValue.mz = mz_dict_data
 
     def set_ndb_lyr(self, ndb_lyr: Union[Dict[int, int], List[int]]):
         """
+        Set No Delay Interbeds Layer Property.
 
-        :param ndb_lyr:
-        :return:
+        :param ndb_lyr: Union[Dict[int, int], List[int]]
         """
         ndb_lyr_len: int = len(ndb_lyr)
         ndb_lyr_dict: Dict = {}
         if ndb_lyr_len != self._num_ndb:
             raise ValueError(f"The length of ndb_lyr should be consistent with num_ndb({self._num_ndb})!")
         if isinstance(ndb_lyr, Dict):
             if sorted(ndb_lyr.keys()) != [i for i in range(self._num_ndb)]:
@@ -137,20 +171,20 @@
                 raise ValueError(
                     f"The value of ndb_lyr should be greater than or equal to 0 and less than {self._num_lyr}.")
         self.subValue.ndb_lyr = ndb_lyr_dict
 
     def set_ndb_grid(self, hc: Union[int, float, np.ndarray], sfe: Union[int, float, np.ndarray],
                      sfv: Union[int, float, np.ndarray], com: Union[int, float, np.ndarray]):
         """
+        Set No Delay Interbeds Grid Cell Property.
 
-        :param hc:
-        :param sfe:
-        :param sfv:
-        :param com:
-        :return:
+        :param hc: Union[int, float, np.ndarray]
+        :param sfe: Union[int, float, np.ndarray]
+        :param sfv: Union[int, float, np.ndarray]
+        :param com: Union[int, float, np.ndarray]
         """
         if isinstance(hc, (int, float)):
             hc = np.full((self._num_ndb, self._num_row, self._num_col), hc, dtype=float)
         if isinstance(sfe, (int, float)):
             sfe = np.full((self._num_ndb, self._num_row, self._num_col), sfe, dtype=float)
         if isinstance(sfv, (int, float)):
             sfv = np.full((self._num_ndb, self._num_row, self._num_col), sfv, dtype=float)
@@ -160,17 +194,17 @@
         sfe = BoundaryCheck.check_3d_zero(sfe, "SFE", self._num_ndb, self._num_row, self._num_col)
         sfv = BoundaryCheck.check_3d_zero(sfv, "SFV", self._num_ndb, self._num_row, self._num_col)
         com = BoundaryCheck.check_3d_format(com, "COM", self._num_ndb, self._num_row, self._num_col)
         self.subValue.ndb_grid = {"HC": hc, "SFE": sfe, "SFV": sfv, "COM": com}
 
     def set_db_lyr(self, db_lyr: Union[Dict[int, int], List[int]]):
         """
+        Set Delay Interbeds Layer Property.
 
-        :param db_lyr:
-        :return:
+        :param db_lyr: Union[Dict[int, int], List[int]]
         """
         db_lyr_len: int = len(db_lyr)
         db_lyr_dict: Dict = {}
         if db_lyr_len != self._num_db:
             raise ValueError(f"The length of db_lyr should be consistent with num_db({self._num_db})!")
         if isinstance(db_lyr, Dict):
             if sorted(db_lyr.keys()) != [i for i in range(self._num_db)]:
@@ -187,22 +221,22 @@
                     f"The value of db_lyr should be greater than or equal to 0 and less than {self._num_lyr}.")
         self.subValue.db_lyr = db_lyr_dict
 
     def set_db_grid(self, rnb: Union[int, float, np.ndarray], dsh: Union[int, float, np.ndarray],
                     dhc: Union[int, float, np.ndarray], dcom: Union[int, float, np.ndarray],
                     dz: Union[int, float, np.ndarray], imz: Union[int, float, np.ndarray]):
         """
+        Set Delay Interbeds Grid Cell Property.
 
-        :param rnb:
-        :param dsh:
-        :param dhc:
-        :param dcom:
-        :param dz:
-        :param imz:
-        :return:
+        :param rnb: Union[int, float, np.ndarray]
+        :param dsh: Union[int, float, np.ndarray]
+        :param dhc: Union[int, float, np.ndarray]
+        :param dcom: Union[int, float, np.ndarray]
+        :param dz: Union[int, float, np.ndarray]
+        :param imz: Union[int, float, np.ndarray]
         """
         if isinstance(rnb, (int, float)):
             rnb = np.full((self._num_db, self._num_row, self._num_col), rnb, dtype=float)
         if isinstance(dsh, (int, float)):
             dsh = np.full((self._num_db, self._num_row, self._num_col), dsh, dtype=float)
         if isinstance(dhc, (int, float)):
             dhc = np.full((self._num_db, self._num_row, self._num_col), dhc, dtype=float)
```

### Comparing `PyCOMUS-1.0.3/pycomus/Package/CWEL.py` & `pycomus-1.0.4/pycomus/Package/CWEL.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,39 +12,54 @@
 
 import pycomus
 from pycomus.Utils import BoundaryCheck
 from pycomus.Utils.CONSTANTS import WEL_PKG_NAME, WEL_FILE_NAME
 
 
 class ComusWel:
-    def __init__(self, model: pycomus.ComusModel, wellr: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
-                 satthr: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]):
-        """
+    """
+    Initialize the COMUS Model with the Well(WEL) package.
+
+    Attributes:
+    ----------------------------
+    model:
+        The COMUS model to which the WEL package will be applied.
+    wellr:
+        The well flow rate (L³/T) for a grid cell.
+    satthr:
+        It is the saturation thickness threshold (L) for the grid cell.
+
+    Methods:
+    --------
+    __init__(self, model: pycomus.ComusModel, wellr: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 satthr: Union[int, float, Dict[int, Union[int, float, np.ndarray]]])
         Initialize the COMUS Model with the Well(WEL) package.
 
-        Parameters:
-        ----------------------------
-        model:
-            The COMUS model to which the WEL package will be applied.
-        wellr:
-            The well flow rate (L³/T) for a grid cell.
-        satthr:
-            It is the saturation thickness threshold (L) for the grid cell.
-
-        Returns:
-        --------
-        instance: pycomus.ComusWel
-           COMUS Well(WEL) Params Object.
-
-        Example:
-        --------
-        >>> import pycomus
-        >>> model1 = pycomus.ComusModel(model_name="test")
-        >>> welPackage = pycomus.ComusWel(model1, wellr={0: 1}, satthr=1)
-        """
+    load(cls, model, wel_params_file: str)
+         Load parameters from a WEL.in file and create a ComusWel instance.
+
+    write_file(self, folder_path: str)
+        Typically used as an internal function but can also be called directly, it outputs the `pycomus.ComusWel`
+        module to the specified path as <WEL.in>.
+
+
+    Returns:
+    --------
+    instance: pycomus.ComusWel
+       COMUS Well(WEL) Params Object.
+
+    Example:
+    --------
+    >>> import pycomus
+    >>> model1 = pycomus.ComusModel(model_name="test")
+    >>> welPackage = pycomus.ComusWel(model1, wellr={0: 1}, satthr=1)
+    """
+
+    def __init__(self, model: pycomus.ComusModel, wellr: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
+                 satthr: Union[int, float, Dict[int, Union[int, float, np.ndarray]]]):
         BoundaryCheck.check_bnd_queue(model)
         cms_dis = BoundaryCheck.get_cms_pars(model)
         cms_period = BoundaryCheck.get_period(model)
         self._num_lyr = cms_dis.num_lyr
         self._num_row = cms_dis.num_row
         self._num_col = cms_dis.num_col
         self._period = cms_period.period
```

### Comparing `PyCOMUS-1.0.3/pycomus/Utils/BoundaryCheck.py` & `pycomus-1.0.4/pycomus/Utils/BoundaryCheck.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import numpy as np
 
 from pycomus.Utils import CONSTANTS
 
 
 def CheckValueFormat(Value: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
-                     ValueName: str, period: List, NumLyr: int, NumRow: int, NumCol: int) -> Dict:
+                     ValueName: str, period: List, num_lyr: int, num_row: int, num_col: int) -> Dict:
     res = {}
     if isinstance(Value, (float, int)):
         for i in range(len(period)):
-            res[i] = np.full((NumLyr, NumRow, NumCol), Value, dtype=float)
+            res[i] = np.full((num_lyr, num_row, num_col), Value, dtype=float)
         return res
     elif isinstance(Value, Dict):
         # Check for duplicate keys
         if len(Value) != len(set(Value.keys())):
             raise ValueError("Duplicate Key found in the Value.")
 
         # Check dictionary length
@@ -23,36 +23,36 @@
 
         # Iterate through dictionary and validate values
         for key, value in Value.items():
             if not (0 <= key < len(period)):
                 raise ValueError(
                     f"Invalid key {key} in {ValueName} dictionary. Keys should be in the range 0 to {len(period) - 1}.")
             if isinstance(value, (int, float)):
-                res[key] = np.full((NumLyr, NumRow, NumCol), value, dtype=float)
+                res[key] = np.full((num_lyr, num_row, num_col), value, dtype=float)
             elif isinstance(value, np.ndarray):
-                if value.shape == (NumLyr, NumRow, NumCol):
+                if value.shape == (num_lyr, num_row, num_col):
                     res[key] = value
                 else:
                     raise ValueError(f"Invalid shape or values in the {ValueName} numpy array.")
             else:
                 raise ValueError(
                     "Invalid value type in the dictionary. Values should be int, float, or numpy.ndarray.")
         return res
     else:
         raise ValueError(f"Invalid value type for '{ValueName}'. It should be int, float, or a dictionary.")
 
 
 def CheckValueGtZero(Value: Union[int, float, Dict[int, Union[int, float, np.ndarray]]],
-                     ValueName: str, period: List, NumLyr: int, NumRow: int, NumCol: int) -> Dict:
+                     ValueName: str, period: List, num_lyr: int, num_row: int, num_col: int) -> Dict:
     res = {}
     if isinstance(Value, (float, int)):
         if Value < 0:
             raise ValueError(f"{ValueName} value must be greater than or equal to 0.")
         for i in range(len(period)):
-            res[i] = np.full((NumLyr, NumRow, NumCol), Value, dtype=float)
+            res[i] = np.full((num_lyr, num_row, num_col), Value, dtype=float)
         return res
     elif isinstance(Value, Dict):
         if len(Value) != len(set(Value.keys())):
             raise ValueError(f"Duplicate Key found in the {ValueName}.")
 
         if len(Value) < 1 or len(Value) > len(period):
             raise ValueError(f"Invalid {ValueName} dict length. It should be between 1 and {len(period)}.")
@@ -60,71 +60,71 @@
         for key, value in Value.items():
             if not (0 <= key < len(period)):
                 raise ValueError(
                     f"Invalid key {key} in {ValueName} dictionary. Keys should be in the range 0 to {len(period) - 1}.")
             if isinstance(value, (int, float)):
                 if value < 0:
                     raise ValueError(f"{ValueName} value must be greater than or equal to 0.")
-                res[key] = np.full((NumLyr, NumRow, NumCol), value, dtype=float)
+                res[key] = np.full((num_lyr, num_row, num_col), value, dtype=float)
             elif isinstance(value, np.ndarray):
-                if value.shape == (NumLyr, NumRow, NumCol):
+                if value.shape == (num_lyr, num_row, num_col):
                     if (value < 0).all():
                         raise ValueError(f"{ValueName} value must be greater than or equal to 0.")
                     res[key] = value
                 else:
                     raise ValueError(f"Invalid shape or values in the {ValueName} numpy array.")
             else:
                 raise ValueError(
                     "Invalid value type in the dictionary. Values should be int, float, or numpy.ndarray.")
         return res
     else:
         raise ValueError(f"Invalid value type for '{ValueName}'. It should be int, float, or a dictionary.")
 
 
-def Check3DValueExistGrid(Value: Union[int, float, np.ndarray], ValueName: str, NumLyr: int, NumRow: int,
-                          NumCol: int, OriginValueList: List) -> np.ndarray:
+def Check3DValueExistGrid(Value: Union[int, float, np.ndarray], ValueName: str, num_lyr: int, num_row: int,
+                          num_col: int, OriginValueList: List) -> np.ndarray:
     if isinstance(Value, (int, float)):
         if Value not in OriginValueList:
             raise ValueError(f"{ValueName} : should exist in {OriginValueList}.")
-        return np.full((NumLyr, NumRow, NumCol), Value, dtype=float)
+        return np.full((num_lyr, num_row, num_col), Value, dtype=float)
     elif isinstance(Value, np.ndarray):
-        if Value.shape == (NumLyr, NumRow, NumCol):
+        if Value.shape == (num_lyr, num_row, num_col):
             if np.all(np.isin(Value, OriginValueList)):
                 return Value
             else:
                 raise ValueError(f"{ValueName} : should exist in {OriginValueList}.")
         else:
             raise ValueError(f"{ValueName} : Invalid shape or values in the {ValueName} numpy array.")
     else:
         raise ValueError(f"Invalid value type for '{ValueName}'. It should be int, float, or a np.ndarray.")
 
 
-def check_3d_zero(Value: Union[int, float, np.ndarray], ValueName: str, NumLyr: int, NumRow: int,
-                  NumCol: int) -> np.ndarray:
+def check_3d_zero(Value: Union[int, float, np.ndarray], ValueName: str, num_lyr: int, num_row: int,
+                  num_col: int) -> np.ndarray:
     if isinstance(Value, (int, float)):
         if Value < 0:
             raise ValueError(f"{ValueName} value must be greater than or equal to 0.")
-        return np.full((NumLyr, NumRow, NumCol), Value, dtype=float)
+        return np.full((num_lyr, num_row, num_col), Value, dtype=float)
     elif isinstance(Value, np.ndarray):
-        if Value.shape == (NumLyr, NumRow, NumCol):
+        if Value.shape == (num_lyr, num_row, num_col):
             if (Value < 0).all():
                 raise ValueError(f"{ValueName} value must be greater than or equal to 0.")
             return Value
         else:
             raise ValueError(f"{ValueName} : Invalid shape or values in the {ValueName} numpy array.")
     else:
         raise ValueError(f"Invalid value type for '{ValueName}'. It should be int, float, or a np.ndarray.")
 
 
-def check_3d_format(Value: Union[int, float, np.ndarray], ValueName: str, NumLyr: int, NumRow: int,
-                    NumCol: int) -> np.ndarray:
+def check_3d_format(Value: Union[int, float, np.ndarray], ValueName: str, num_lyr: int, num_row: int,
+                    num_col: int) -> np.ndarray:
     if isinstance(Value, (int, float)):
-        return np.full((NumLyr, NumRow, NumCol), Value, dtype=float)
+        return np.full((num_lyr, num_row, num_col), Value, dtype=float)
     elif isinstance(Value, np.ndarray):
-        if Value.shape == (NumLyr, NumRow, NumCol):
+        if Value.shape == (num_lyr, num_row, num_col):
             return Value
         else:
             raise ValueError(f"{ValueName} : Invalid shape or values in the {ValueName} numpy array.")
     else:
         raise ValueError(f"Invalid value type for '{ValueName}'. It should be int, float, or a np.ndarray.")
 
 
@@ -187,17 +187,17 @@
 def check_col(tar_col: int, col: int) -> bool:
     if tar_col < 0 or tar_col >= col:
         print(f"The col should be greater than or equal to 0 and less than {col}.")
         return False
     return True
 
 
-def check_dict_zero(Value: np.ndarray, ValueName: str, NumLyr: int, NumRow: int,
-                    NumCol: int):
-    if Value.shape == (NumLyr, NumRow, NumCol):
+def check_dict_zero(Value: np.ndarray, ValueName: str, num_lyr: int, num_row: int,
+                    num_col: int):
+    if Value.shape == (num_lyr, num_row, num_col):
         if (Value < 0).all():
             print(f"{ValueName} value must be greater than or equal to 0.")
             return False
     else:
-        print(f"{ValueName} : Invalid shape in the {ValueName} numpy array(need {NumLyr},{NumRow},{NumCol}).")
+        print(f"{ValueName} : Invalid shape in the {ValueName} numpy array(need {num_lyr},{num_row},{num_col}).")
         return False
     return True
```

### Comparing `PyCOMUS-1.0.3/pycomus/Utils/CONSTANTS.py` & `pycomus-1.0.4/pycomus/ComusDis/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `PyCOMUS-1.0.3/pycomus/Utils/LinuxCheckParams.so` & `pycomus-1.0.4/pycomus/Utils/LinuxCheckParams.so`

 * *Files identical despite different names*

### Comparing `PyCOMUS-1.0.3/pycomus/Utils/LinuxComus.so` & `pycomus-1.0.4/pycomus/Utils/LinuxComus.so`

 * *Files identical despite different names*

### Comparing `PyCOMUS-1.0.3/pycomus/Utils/WinCheckParams.dll` & `pycomus-1.0.4/pycomus/Utils/WinCheckParams.dll`

 * *Files identical despite different names*

### Comparing `PyCOMUS-1.0.3/pycomus/Utils/WinComus.dll` & `pycomus-1.0.4/pycomus/Utils/WinComus.dll`

 * *Files identical despite different names*

### Comparing `PyCOMUS-1.0.3/README.md` & `pycomus-1.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,45 @@
+Metadata-Version: 2.1
+Name: PyCOMUS
+Version: 1.0.4
+Summary: A Python library for invoking the COMUS model for groundwater numerical simulation.
+Home-page: https://github.com/ZhenjiangWuHydro/PyCOMUS
+Author: Zhenjiang Wu
+Author-email: zhenjiangwu613@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # Introduction
 
 PyCOMUS is a Python interface built upon the COMUS model, capable of performing all the functions that the COMUS model offers.
 
 
 
 # Documentation
 
-```python
-# ---------------
-# Todo
-# --------------- 
-```
+[https://pycomus.readthedocs.io/en/latest/](https://pycomus.readthedocs.io/en/latest/)
 
 
 
 # Installation
 
-PyCOMUS requires **Python 3.8+** with:
+PyCOMUS requires **Python 3.0+** with:
 
 ```python
-numpy >=1.15.0,<2.0.0
-matplotlib >=1.4.0
+numpy
+matplotlib
 ```
 
 To install type:
 
 ```bash
-pip install PyCOMUS
+pip install PyCOMUS(PyPI)
 ```
 
 
 
 # Getting Started
 
 ```python
@@ -47,79 +56,79 @@
     # Control Params
     controlParams = pycomus.ComusConPars(model=model, intblkm=2, max_iter=10000, r_close=0.0001)
 
     # Output Params
     outParams = pycomus.ComusOutputPars(model)
 
     # Create Grid And Layer
-    NumLyr = 2
-    NumRow = 20
-    NumCol = 20
-    modelDis = pycomus.ComusDisLpf(model, num_lyr=NumLyr, num_row=NumRow, num_col=NumCol, row_space=50, col_space=50,
-                                   lyr_type=[1 for _ in range(NumLyr)], lyr_cbd=[1, 0], y_coord=1000)
+    num_lyr = 2
+    num_row = 20
+    num_col = 20
+    modelDis = pycomus.ComusDisLpf(model, num_lyr=num_lyr, num_row=num_row, num_col=num_col, row_space=50, col_space=50,
+                                   lyr_type=[1 for _ in range(num_lyr)], lyr_cbd=[1, 0], y_coord=1000)
 
     # Grid Attribute
-    bot = np.zeros((NumLyr, NumRow, NumCol))
+    bot = np.zeros((num_lyr, num_row, num_col))
     bot[0, :, :] = 10
-    vkcb = np.zeros((NumLyr, NumRow, NumCol))
+    vkcb = np.zeros((num_lyr, num_row, num_col))
     vkcb[0, :, :] = 0.001
-    tkcb = np.zeros((NumLyr, NumRow, NumCol))
+    tkcb = np.zeros((num_lyr, num_row, num_col))
     tkcb[0, :, :] = 0.1
     modelGridPar = pycomus.ComusGridPars(model, top=20, bot=bot, ibound=1, kx=10, ky=10, kz=5, vkcb=vkcb, tkcb=tkcb,
                                          shead=16, sc1=0.0001, sc2=0.08)
 
     # Set Period
     period = pycomus.ComusPeriod(model, [(10, 10, 1) for _ in range(2)])
 
     # Set SHB
-    shead_period1 = np.zeros((NumLyr, NumRow, NumCol))
+    shead_period1 = np.zeros((num_lyr, num_row, num_col))
     shead_period1[0, :, 19] = 16
-    shead_period2 = np.zeros((NumLyr, NumRow, NumCol))
+    shead_period2 = np.zeros((num_lyr, num_row, num_col))
     shead_period2[0, :, 19] = 17
 
-    ehead_period1 = np.zeros((NumLyr, NumRow, NumCol))
+    ehead_period1 = np.zeros((num_lyr, num_row, num_col))
     ehead_period1[0, :, 19] = 17
-    ehead_period2 = np.zeros((NumLyr, NumRow, NumCol))
+    ehead_period2 = np.zeros((num_lyr, num_row, num_col))
     ehead_period2[0, :, 19] = 18
     shbPackage = pycomus.ComusShb(model, shead={0: shead_period1, 1: shead_period2},
                                   ehead={0: ehead_period1, 1: ehead_period2})
 
     # Set WEL
-    wellr_period1 = np.zeros((NumLyr, NumRow, NumCol))
+    wellr_period1 = np.zeros((num_lyr, num_row, num_col))
     wellr_period1[1, 3, 12] = -500
     wellr_period1[1, 16, 12] = -500
-    wellr_period2 = np.zeros((NumLyr, NumRow, NumCol))
+    wellr_period2 = np.zeros((num_lyr, num_row, num_col))
     wellr_period2[1, 3, 12] = -300
     wellr_period2[1, 16, 12] = -300
-    satthr_period1 = np.zeros((NumLyr, NumRow, NumCol))
+    satthr_period1 = np.zeros((num_lyr, num_row, num_col))
     satthr_period1[1, 3, 12] = 0.1
     satthr_period1[1, 16, 12] = 0.1
     welPackage = pycomus.ComusWel(model, wellr={0: wellr_period1, 1: wellr_period2},
                                   satthr={0: satthr_period1, 1: satthr_period1})
 
     # Set EVT
-    etSurf = np.zeros((NumLyr, NumRow, NumCol))
+    etSurf = np.zeros((num_lyr, num_row, num_col))
     etSurf[0, :, :] = 20
-    etRate = np.zeros((NumLyr, NumRow, NumCol))
+    etRate = np.zeros((num_lyr, num_row, num_col))
     etRate[0, :, :] = 0.002
-    etMxd = np.zeros((NumLyr, NumRow, NumCol))
+    etMxd = np.zeros((num_lyr, num_row, num_col))
     etMxd[0, :, :] = 5
-    etExp = np.zeros((NumLyr, NumRow, NumCol))
+    etExp = np.zeros((num_lyr, num_row, num_col))
     etExp[0, :, :] = 2
     evtPackage = pycomus.ComusEvt(model, et_surf={0: etSurf, 1: etSurf}, et_rate={0: etRate, 1: etRate},
                                   et_mxd={0: etMxd, 1: etMxd}, et_exp={0: etExp, 1: etExp}, num_seg=2)
 
     # Set RIV
-    cond = np.zeros((NumLyr, NumRow, NumCol))
+    cond = np.zeros((num_lyr, num_row, num_col))
     cond[0, :, 0] = 100
-    rivBtm = np.zeros((NumLyr, NumRow, NumCol))
+    rivBtm = np.zeros((num_lyr, num_row, num_col))
     rivBtm[0, :, 0] = 15
-    shead_ehead_period1 = np.zeros((NumLyr, NumRow, NumCol))
+    shead_ehead_period1 = np.zeros((num_lyr, num_row, num_col))
     shead_ehead_period1[0, :, 0] = 16
-    shead_ehead_period2 = np.zeros((NumLyr, NumRow, NumCol))
+    shead_ehead_period2 = np.zeros((num_lyr, num_row, num_col))
     shead_ehead_period2[0, :, 0] = 18
     rivPackage = pycomus.ComusRiv(model, cond={0: cond, 1: cond},
                                   shead={0: shead_ehead_period1, 1: shead_ehead_period2},
                                   ehead={0: shead_ehead_period1, 1: shead_ehead_period2},
                                   riv_btm={0: rivBtm, 1: rivBtm})
 
     # Write Output
```

### Comparing `PyCOMUS-1.0.3/setup.py` & `pycomus-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyCOMUS",
-    version="1.0.3",
+    version="1.0.4",
     author="Zhenjiang Wu",
     author_email="zhenjiangwu613@gmail.com",
     description="A Python library for invoking the COMUS model for groundwater numerical simulation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ZhenjiangWuHydro/PyCOMUS",
     packages=setuptools.find_packages(exclude=['Example*', 'tests*', 'docs*', 'build*', 'dist*', '.idea*', '.gitignore', 'README.md','ComusModel','paper','CheckParam']),
```

