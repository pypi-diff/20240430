# Comparing `tmp/untie-0.0.4.tar.gz` & `tmp/untie-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "untie-0.0.4.tar", last modified: Sun Apr 28 06:00:53 2024, max compression
+gzip compressed data, was "untie-0.0.5.tar", last modified: Tue Apr 30 18:00:18 2024, max compression
```

## Comparing `untie-0.0.4.tar` & `untie-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-28 06:00:53.850843 untie-0.0.4/
--rw-rw-r--   0 marco     (1000) marco     (1000)       60 2024-04-27 17:01:18.000000 untie-0.0.4/AUTHORS.md
--rw-rw-r--   0 marco     (1000) marco     (1000)      812 2024-04-27 17:01:18.000000 untie-0.0.4/LICENSE.md
--rw-r--r--   0 marco     (1000) marco     (1000)       72 2024-04-27 20:31:19.000000 untie-0.0.4/MANIFEST.in
--rw-r--r--   0 marco     (1000) marco     (1000)     1850 2024-04-28 06:00:53.850843 untie-0.0.4/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      177 2024-04-27 17:01:18.000000 untie-0.0.4/README.md
--rw-rw-r--   0 marco     (1000) marco     (1000)        6 2024-04-28 05:58:18.000000 untie-0.0.4/VERSION
--rw-rw-r--   0 marco     (1000) marco     (1000)       81 2024-04-27 17:01:18.000000 untie-0.0.4/pyproject.toml
--rw-rw-r--   0 marco     (1000) marco     (1000)     1085 2024-04-28 06:00:53.854843 untie-0.0.4/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)     1527 2024-04-28 05:56:42.000000 untie-0.0.4/setup.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-28 06:00:53.850843 untie-0.0.4/src/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-28 06:00:53.850843 untie-0.0.4/src/untie/
--rw-rw-r--   0 marco     (1000) marco     (1000)     2079 2024-04-27 20:10:25.000000 untie-0.0.4/src/untie/TIE_classes.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    27696 2024-04-27 20:10:25.000000 untie-0.0.4/src/untie/TIE_core.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    17933 2024-04-27 20:10:25.000000 untie-0.0.4/src/untie/TIE_general.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    12556 2024-04-27 20:10:25.000000 untie-0.0.4/src/untie/TIE_load.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    33933 2024-04-27 20:10:25.000000 untie-0.0.4/src/untie/TIE_visual.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      107 2024-04-27 20:10:25.000000 untie-0.0.4/src/untie/__init__.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-28 06:00:53.850843 untie-0.0.4/src/untie.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     1850 2024-04-28 06:00:53.000000 untie-0.0.4/src/untie.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      421 2024-04-28 06:00:53.000000 untie-0.0.4/src/untie.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-28 06:00:53.000000 untie-0.0.4/src/untie.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-27 17:32:53.000000 untie-0.0.4/src/untie.egg-info/not-zip-safe
--rw-rw-r--   0 marco     (1000) marco     (1000)      180 2024-04-28 06:00:53.000000 untie-0.0.4/src/untie.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        6 2024-04-28 06:00:53.000000 untie-0.0.4/src/untie.egg-info/top_level.txt
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-30 18:00:18.226529 untie-0.0.5/
+-rw-rw-r--   0 marco     (1000) marco     (1000)       60 2024-04-27 17:01:18.000000 untie-0.0.5/AUTHORS.md
+-rw-rw-r--   0 marco     (1000) marco     (1000)      812 2024-04-27 17:01:18.000000 untie-0.0.5/LICENSE.md
+-rw-rw-r--   0 marco     (1000) marco     (1000)       72 2024-04-30 17:55:03.000000 untie-0.0.5/MANIFEST.in
+-rw-r--r--   0 marco     (1000) marco     (1000)     1850 2024-04-30 18:00:18.226529 untie-0.0.5/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      177 2024-04-27 17:01:18.000000 untie-0.0.5/README.md
+-rw-rw-r--   0 marco     (1000) marco     (1000)        6 2024-04-30 17:58:06.000000 untie-0.0.5/VERSION
+-rw-rw-r--   0 marco     (1000) marco     (1000)       81 2024-04-27 17:01:18.000000 untie-0.0.5/pyproject.toml
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1085 2024-04-30 18:00:18.230529 untie-0.0.5/setup.cfg
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1527 2024-04-30 17:55:03.000000 untie-0.0.5/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-30 18:00:18.222528 untie-0.0.5/src/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-30 18:00:18.226529 untie-0.0.5/src/untie/
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2079 2024-04-30 17:55:03.000000 untie-0.0.5/src/untie/TIE_classes.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    27700 2024-04-30 17:56:35.000000 untie-0.0.5/src/untie/TIE_core.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    17933 2024-04-30 17:55:03.000000 untie-0.0.5/src/untie/TIE_general.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    12560 2024-04-30 17:56:05.000000 untie-0.0.5/src/untie/TIE_load.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    33937 2024-04-30 17:55:37.000000 untie-0.0.5/src/untie/TIE_visual.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      107 2024-04-30 17:55:03.000000 untie-0.0.5/src/untie/__init__.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-30 18:00:18.226529 untie-0.0.5/src/untie.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1850 2024-04-30 18:00:18.000000 untie-0.0.5/src/untie.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      421 2024-04-30 18:00:18.000000 untie-0.0.5/src/untie.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-30 18:00:18.000000 untie-0.0.5/src/untie.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-27 17:32:53.000000 untie-0.0.5/src/untie.egg-info/not-zip-safe
+-rw-rw-r--   0 marco     (1000) marco     (1000)      180 2024-04-30 18:00:18.000000 untie-0.0.5/src/untie.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        6 2024-04-30 18:00:18.000000 untie-0.0.5/src/untie.egg-info/top_level.txt
```

### Comparing `untie-0.0.4/LICENSE.md` & `untie-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `untie-0.0.4/PKG-INFO` & `untie-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untie
-Version: 0.0.4
+Version: 0.0.5
 Summary: Trace Information Extraction (TIE) library
 Home-page: https://github.com/swisstopo/lg-tie-lib
 Author: Anna Rauch
 Author-email: contact@infogrip.ch
 Maintainer: Marc Monnerat
 Maintainer-email: marc.monnerat@swisstopo.ch
 License: BSD 3-Clause License
```

### Comparing `untie-0.0.4/setup.cfg` & `untie-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `untie-0.0.4/setup.py` & `untie-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `untie-0.0.4/src/untie/TIE_classes.py` & `untie-0.0.5/src/untie/TIE_classes.py`

 * *Files identical despite different names*

### Comparing `untie-0.0.4/src/untie/TIE_core.py` & `untie-0.0.5/src/untie/TIE_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 This script contains a set of general functions/methods that perform the
 core-steps of the TIE-method (i.e. the actual TIE-steps)
 """
 import copy
 from typing import Dict, List, Tuple, Union
 
 import numpy as np
-from TIE import TIE_classes as TIEclass
-from TIE import TIE_general as TIEgen
+from untie import TIE_classes as TIEclass
+from untie import TIE_general as TIEgen
 
 
 def classifyTRACE(TRACES, pth=None):
     """Classify traces based on TIE parameters.
 
     Parameters
     ----------
```

### Comparing `untie-0.0.4/src/untie/TIE_general.py` & `untie-0.0.5/src/untie/TIE_general.py`

 * *Files identical despite different names*

### Comparing `untie-0.0.4/src/untie/TIE_load.py` & `untie-0.0.5/src/untie/TIE_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import tempfile
 
 from typing import Dict, List, Tuple, Union
 
 import geopandas as gpd
 import numpy as np
 import rasterio as rst
-from TIE import TIE_classes as TIEclass
-from TIE import TIE_general as TIEgen
+from untie import TIE_classes as TIEclass
+from untie import TIE_general as TIEgen
 from rasterio.mask import mask
 from rasterio.merge import merge
 from shapely.geometry import Polygon
 from shapely.geometry import box
 
 
 def adaptSHAPE2DEM(shapefile: gpd.GeoDataFrame, DEM: Dict) -> gpd.GeoDataFrame:
```

### Comparing `untie-0.0.4/src/untie/TIE_visual.py` & `untie-0.0.5/src/untie/TIE_visual.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 This script contains a set of functions/methods that are useful to
 display and visualize the TIE-results.
 """
 
 import numpy as np
 import math
 import matplotlib.pyplot as plt
-from TIE import TIE_general as TIEgen
-from TIE import TIE_classes as TIEclass
+from untie import TIE_general as TIEgen
+from untie import TIE_classes as TIEclass
 from mayavi import mlab
 import matplotlib.patches as mpatches
 
 
 def bed2cmap(BEDrst: np.ndarray, legendfile: str, leg_labels: bool = False) -> tuple:
     """
     Color Information For Bedrock.
```

### Comparing `untie-0.0.4/src/untie.egg-info/PKG-INFO` & `untie-0.0.5/src/untie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untie
-Version: 0.0.4
+Version: 0.0.5
 Summary: Trace Information Extraction (TIE) library
 Home-page: https://github.com/swisstopo/lg-tie-lib
 Author: Anna Rauch
 Author-email: contact@infogrip.ch
 Maintainer: Marc Monnerat
 Maintainer-email: marc.monnerat@swisstopo.ch
 License: BSD 3-Clause License
```

