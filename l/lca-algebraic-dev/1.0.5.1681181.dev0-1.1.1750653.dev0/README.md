# Comparing `tmp/lca_algebraic_dev-1.0.5.1681181.dev0.tar.gz` & `tmp/lca_algebraic_dev-1.1.1750653.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lca_algebraic_dev-1.0.5.1681181.dev0.tar", last modified: Wed Mar 13 10:41:18 2024, max compression
+gzip compressed data, was "lca_algebraic_dev-1.1.1750653.dev0.tar", last modified: Tue Apr 30 15:33:02 2024, max compression
```

## Comparing `lca_algebraic_dev-1.0.5.1681181.dev0.tar` & `lca_algebraic_dev-1.1.1750653.dev0.tar`

### file list

```diff
@@ -1,48 +1,39 @@
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-03-13 10:41:18.113882 lca_algebraic_dev-1.0.5.1681181.dev0/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      174 2024-02-27 10:51:22.000000 lca_algebraic_dev-1.0.5.1681181.dev0/.gitignore
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1331 2020-03-30 15:19:57.000000 lca_algebraic_dev-1.0.5.1681181.dev0/LICENSE
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      989 2024-02-26 17:11:56.000000 lca_algebraic_dev-1.0.5.1681181.dev0/Makefile
--rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)     4649 2024-03-13 10:41:18.113882 lca_algebraic_dev-1.0.5.1681181.dev0/PKG-INFO
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3904 2022-08-03 18:27:03.000000 lca_algebraic_dev-1.0.5.1681181.dev0/README.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     5452 2024-02-27 10:51:22.000000 lca_algebraic_dev-1.0.5.1681181.dev0/RELEASE_NOTES.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        5 2024-02-20 17:07:28.000000 lca_algebraic_dev-1.0.5.1681181.dev0/VERSION
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-03-13 10:41:18.109882 lca_algebraic_dev-1.0.5.1681181.dev0/conda-recipe/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      799 2024-02-20 17:07:28.000000 lca_algebraic_dev-1.0.5.1681181.dev0/conda-recipe/meta.yaml
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-03-13 10:41:18.109882 lca_algebraic_dev-1.0.5.1681181.dev0/doc/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    17897 2021-06-23 09:18:46.000000 lca_algebraic_dev-1.0.5.1681181.dev0/doc/base_utils.html
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)   156146 2020-03-24 15:08:44.000000 lca_algebraic_dev-1.0.5.1681181.dev0/doc/doc.html
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    88740 2021-06-23 09:18:46.000000 lca_algebraic_dev-1.0.5.1681181.dev0/doc/helpers.html
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    12016 2022-08-03 18:27:03.000000 lca_algebraic_dev-1.0.5.1681181.dev0/doc/index.html
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    10282 2021-06-23 09:18:46.000000 lca_algebraic_dev-1.0.5.1681181.dev0/doc/io.html
--rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)    29363 2020-03-24 15:08:44.000000 lca_algebraic_dev-1.0.5.1681181.dev0/doc/lca-algebraic.odp
--rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)   206268 2020-03-24 15:08:44.000000 lca_algebraic_dev-1.0.5.1681181.dev0/doc/lca-algebraic.png
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    49312 2021-06-23 09:18:46.000000 lca_algebraic_dev-1.0.5.1681181.dev0/doc/lca.html
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)   100461 2022-08-03 18:27:03.000000 lca_algebraic_dev-1.0.5.1681181.dev0/doc/params.html
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    76217 2022-08-03 18:27:03.000000 lca_algebraic_dev-1.0.5.1681181.dev0/doc/stats.html
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)   752624 2024-02-28 15:35:03.000000 lca_algebraic_dev-1.0.5.1681181.dev0/example-notebook.ipynb
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-03-13 10:41:18.109882 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1036 2024-02-28 15:35:03.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/__init__.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2224 2024-02-27 17:53:50.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/axis_dict.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     5317 2024-02-28 15:35:03.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/base_utils.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2557 2024-02-28 15:35:03.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/cache.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1276 2024-02-27 10:51:22.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/db.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    30720 2024-02-28 15:35:03.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/helpers.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1931 2024-02-20 17:07:28.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/io.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    28351 2024-03-13 10:22:52.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/lca.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      368 2024-02-20 17:07:28.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/log.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    35341 2024-02-28 15:35:03.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/params.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    37514 2024-02-27 17:53:50.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/stats.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-03-13 10:41:18.113882 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic_dev.egg-info/
--rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)     4649 2024-03-13 10:41:18.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic_dev.egg-info/PKG-INFO
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      837 2024-03-13 10:41:18.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        1 2024-03-13 10:41:18.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       99 2024-03-13 10:41:18.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic_dev.egg-info/requires.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       14 2024-03-13 10:41:18.000000 lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic_dev.egg-info/top_level.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      144 2024-02-28 15:35:03.000000 lca_algebraic_dev-1.0.5.1681181.dev0/requirements.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      332 2024-03-13 10:41:18.113882 lca_algebraic_dev-1.0.5.1681181.dev0/setup.cfg
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2017 2024-02-28 15:35:03.000000 lca_algebraic_dev-1.0.5.1681181.dev0/setup.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-03-13 10:41:18.109882 lca_algebraic_dev-1.0.5.1681181.dev0/test/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2021-06-23 08:53:38.000000 lca_algebraic_dev-1.0.5.1681181.dev0/test/__init__.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-03-13 10:41:18.113882 lca_algebraic_dev-1.0.5.1681181.dev0/test/fixtures/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1491 2024-02-28 15:35:03.000000 lca_algebraic_dev-1.0.5.1681181.dev0/test/fixtures/__init__.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      777 2024-02-27 17:53:50.000000 lca_algebraic_dev-1.0.5.1681181.dev0/test/test_axis_dict.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-04-30 15:33:02.531867 lca_algebraic_dev-1.1.1750653.dev0/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      199 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/.gitignore
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1331 2020-03-30 15:19:57.000000 lca_algebraic_dev-1.1.1750653.dev0/LICENSE
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      693 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/Makefile
+-rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)     2916 2024-04-30 15:33:02.531867 lca_algebraic_dev-1.1.1750653.dev0/PKG-INFO
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2118 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/README.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     5451 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/RELEASE_NOTES.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        3 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/VERSION
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-04-30 15:33:02.527867 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1147 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/__init__.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    26296 2024-04-30 11:37:51.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/activity.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2224 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/axis_dict.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4736 2024-04-29 09:36:57.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/base_utils.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3015 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/cache.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     6009 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/database.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3600 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/interpolation.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2043 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/io.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    28054 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/lca.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      547 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/log.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1760 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/methods.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    41317 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/params.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      103 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/settings.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    39547 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/stats.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     7874 2024-04-29 10:45:25.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/units.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-04-30 15:33:02.531867 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic_dev.egg-info/
+-rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)     2916 2024-04-30 15:33:02.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      757 2024-04-30 15:33:02.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        1 2024-04-30 15:33:02.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      122 2024-04-30 15:33:02.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic_dev.egg-info/requires.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       14 2024-04-30 15:33:02.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic_dev.egg-info/top_level.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      167 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/requirements.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      338 2024-04-30 15:33:02.531867 lca_algebraic_dev-1.1.1750653.dev0/setup.cfg
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2062 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/setup.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-04-30 15:33:02.531867 lca_algebraic_dev-1.1.1750653.dev0/test/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2021-06-23 08:53:38.000000 lca_algebraic_dev-1.1.1750653.dev0/test/__init__.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-04-30 15:33:02.531867 lca_algebraic_dev-1.1.1750653.dev0/test/fixtures/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1016 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/test/fixtures/__init__.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      777 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/test/test_axis_dict.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3877 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/test/test_units.py
```

### Comparing `lca_algebraic_dev-1.0.5.1681181.dev0/LICENSE` & `lca_algebraic_dev-1.1.1750653.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.0.5.1681181.dev0/RELEASE_NOTES.md` & `lca_algebraic_dev-1.1.1750653.dev0/RELEASE_NOTES.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 1.1 
+# 1.1
 
 * Fixed bug in ActivityExtended#getExchanges introduced by merge #14
 * Added linear interpolation between activities with function `interpolate_activities`
 * Rename multiLCaAlgebraic => compute_impacts
 * Added breakdown of impacts by arbitrary attribute with the parameter `axis` of `compute_impacts`
 * Added `functional_unit` in compute_impacts : You are not obliged to define a custom activity anymore 
 * findActivities() is now case insensitive by default
```

### Comparing `lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/__init__.py` & `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 #
 # This file defines several utility functions above brightway2 to be used by notebooks
 #
 
+from .activity import *
 from .base_utils import *
-from .db import *
-from .helpers import *
+from .database import *
+from .interpolation import *
 from .io import *
 from .lca import *
 from .log import *
+from .methods import *
 from .params import *
+from .settings import Settings
 from .stats import *
+from .units import *
 
 # Backport the test of pypardiso from bw2calc to emit a warning
 try:
     from pypardiso import factorized, spsolve
 except ImportError:
     from scipy.sparse.linalg import factorized, spsolve
     from scipy.sparse.linalg._dsolve import linsolve
```

### Comparing `lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/axis_dict.py` & `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/axis_dict.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/base_utils.py` & `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/base_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,22 @@
 from contextlib import AbstractContextManager
 from inspect import isfunction
-from sys import stderr
-from typing import Dict, Iterable
+from typing import Dict, Iterable, Union
 
 import brightway2 as bw
 import ipywidgets as widgets
 import numpy as np
 import pandas as pd
 from bw2data.backends.peewee import Activity
 from IPython.display import display
 from six import raise_from
+from sympy import Basic
+from sympy.physics.units import Quantity
 
-DEBUG = False
-LANG = "fr"
-UNIT_OVERRIDE = dict()
-
-
-def set_debug(value=True):
-    """Activate debug logs"""
-    global DEBUG
-    DEBUG = value
-
-
-def set_lang(lang):
-    """Set language"""
-    global LANG
-    LANG = lang
-
-
-def debug(*args, **kwargs):
-    if DEBUG:
-        print(*args, **kwargs)
-
-
-def error(*args, **kwargs):
-    """Print message on stderr"""
-    print(*args, **kwargs, file=stderr)
+_user_functions = dict()
 
 
 def _isOutputExch(exc):
     return exc.get("type") == "production"
 
 
 def _isnumber(value):
@@ -52,21 +29,14 @@
 def _getDb(dbname) -> bw.Database:
     """Pool of Database instances"""
     if dbname not in dbs:
         dbs[dbname] = bw.Database(dbname)
     return dbs[dbname]
 
 
-def interpolate(x, x1, x2, y1, y2):
-    """Build an expression for linear interpolation between two points.
-    If x is not within [x1, x2] the corresponding bound Y values are returned"""
-    x = Min(Max(x, x1), x2)
-    return y1 + (y2 - y1) * (x - x1) / (x2 - x1)
-
-
 def Max(a, b):
     """Max define as algrebraic forumal with 'abs' for proper computation on vectors"""
     return (a + b + abs(a - b)) / 2
 
 
 def Min(a, b):
     """Max define as algrebraic forumal with 'abs' for proper computation on vectors"""
@@ -77,20 +47,14 @@
     """Generate pretty name for activity + basic information"""
     name = _actName(act)
     amount = act.getOutputAmount()
 
     return "%s (%f %s)" % (name, amount, act["unit"])
 
 
-def _method_unit(method):
-    if method in UNIT_OVERRIDE:
-        return UNIT_OVERRIDE[method]
-    return bw.Method(method).metadata["unit"]
-
-
 def _actName(act: Activity):
     """Generate pretty name for activity, appending location if not 'GLO'"""
     res = act["name"]
     if "location" in act and act["location"] != "GLO":
         res += "[%s]" % act["location"]
     return res
 
@@ -204,7 +168,15 @@
 
 def one(it: Iterable):
     """Expect a list with single value a returns it"""
     it = list(it)
     if len(it) != 1:
         raise Exception(f"Expected a single value but got {len(it)}")
     return it[0]
+
+
+ValueOrExpression = Union[float, Basic, Quantity]
+
+
+def getActByCode(db_name, code):
+    """Get activity by code"""
+    return _getDb(db_name).get(code)
```

### Comparing `lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/cache.py` & `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,56 @@
 import os
 import pickle
 from os import path
 
 import brightway2 as bw
 
 from .log import logger
+from .settings import Settings
 
 LCIA_CACHE = "lcia"
 EXPR_CACHE = "expr"
 
 
-class CacheSettings:
-    enabled = True
+# Overide the behaviour for pickling sympy.UndefineFunction
+class Pickler(pickle.Pickler):
+    from sympy.core.function import UndefinedFunction
+
+    def reducer_override(self, obj):
+        # FIXME: maybe too gready, we may check if obj is an instance of
+        #        registered functions instead.
+        if obj.__class__ is Pickler.UndefinedFunction:
+            return type, (obj.__name__, obj.__bases__, dict(obj.__dict__))
+        return NotImplemented
 
 
 def last_db_update():
     """Get the last update of current database project"""
     filename = path.join(bw.projects.dir, "lci", "databases.db")
 
     return path.getmtime(filename)
 
 
 def disable_cache():
-    CacheSettings.enabled = False
+    Settings.cache_enabled = False
 
 
 class _Caches:
     "Singleton instance holding caches"
     caches = dict()
 
 
 class _CacheDict:
     """A smart cache that get cleared whenever database changes, and dumped to file whenever we exit from it"""
 
     def __init__(self, name):
         self.name = name
 
         # No cache ? => LOCAL DICT
-        if not CacheSettings.enabled:
+        if not Settings.cache_enabled:
             self.data = dict()
             return
 
         filename = _CacheDict.filename(self.name)
         if path.exists(filename):
             if last_db_update() > path.getmtime(filename):
                 logger.info(f"Db changed recently, clearing cache {self.name}")
@@ -64,17 +73,17 @@
         self.data = _Caches.caches[name]
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         # Save data on exit
-        if CacheSettings.enabled and self.data:
+        if Settings.cache_enabled and self.data:
             with open(_CacheDict.filename(self.name), "wb") as pickleFile:
-                self.data = pickle.dump(self.data, pickleFile)
+                self.data = Pickler(pickleFile).dump(self.data)
 
     @classmethod
     def filename(cls, name):
         return path.join(bw.projects.dir, f"lca_algebraic_cache-{name}.pickle")
 
 
 class LCIACache(_CacheDict):
```

### Comparing `lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/helpers.py` & `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/activity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,149 +1,44 @@
-import functools
-import inspect
 import re
-import types
 from collections import defaultdict
 from copy import deepcopy
-from itertools import chain
+from types import FunctionType
 from typing import Dict, Tuple, Union
 
+import brightway2 as bw
 import pandas as pd
-from bw2data.backends.peewee import ExchangeDataset
+from bw2data.backends.peewee import Activity, ExchangeDataset
 from bw2data.backends.peewee.utils import dict_as_exchangedataset
-from bw2data.meta import databases as dbmeta
-from sympy import Basic, Expr, Piecewise, simplify, symbols
+from pint import DimensionalityError, Quantity
+from sympy import Basic, simplify, symbols
 
-from .base_utils import (
-    Activity,
-    _actDesc,
-    _actName,
-    _getDb,
-    _isOutputExch,
-    bw,
-    error,
-    interpolate,
-    one,
+from lca_algebraic.base_utils import _actName, _getDb, _isOutputExch
+from lca_algebraic.database import (
+    _find_biosphere_db,
+    _isForeground,
+    _listTechBackgroundDbs,
+    with_db_context,
 )
-from .params import (
+from lca_algebraic.params import (
     DbContext,
-    EnumParam,
     ParamDef,
     _complete_and_expand_params,
     _getAmountOrFormula,
     _param_registry,
 )
 
-BIOSPHERE_PREFIX = "biosphere"
-
-_metaCache = defaultdict(lambda: {})
-
-# param_manager = ParameterManager()
-
-
-def _setMeta(dbname, key, value):
-    """Set meta param on DB"""
-    _metaCache[dbname][key] = value
-
-    data = dbmeta[dbname]
-    data[key] = value
-    dbmeta[dbname] = data
-    dbmeta.flush()
-
-
-def _getMeta(db_name, key):
-    if key in _metaCache[db_name]:
-        return _metaCache[db_name][key]
-
-    val = dbmeta[db_name].get(key)
-    _metaCache[db_name][key] = val
-    return val
-
-
-FOREGROUND_KEY = "fg"
-
-
-def _isForeground(db_name):
-    """Check is db is marked as foreground DB : which means activities may be parametrized / should be developped."""
-    return _getMeta(db_name, FOREGROUND_KEY)
-
-
-def setForeground(db_name):
-    """Set a db as being a foreground database, meaning it is parametrized and lca_algebraic should develop its activities"""
-    return _setMeta(db_name, FOREGROUND_KEY, True)
-
-
-def setBackground(db_name):
-    """Set a db as being a foreground database, meaning it should be considred as static"""
-    return _setMeta(db_name, FOREGROUND_KEY, False)
-
-
-def _listTechBackgroundDbs():
-    """List all background databases technosphere (non biosphere) batabases"""
-    return list(name for name in bw.databases if not _isForeground(name) and BIOSPHERE_PREFIX not in name)
-
-
-def _find_biosphere_db():
-    """List all background databases technosphere (non biosphere) batabases"""
-    return one(name for name in bw.databases if BIOSPHERE_PREFIX in name)
-
-
-old_amount = symbols(
-    "old_amount"
-)  # Can be used in expression of amount for updateExchanges, in order to reference the previous value
-NumOrExpression = Union[float, Basic]
-
-
-def list_databases():
-    """List of databases and their status"""
-    data = list(
-        dict(
-            name=name,
-            backend=_getMeta(name, "backend"),
-            nb_activities=len(bw.Database(name)),
-            type="biosphere" if BIOSPHERE_PREFIX in name else "foreground" if _isForeground(name) else "background",
-        )
-        for name in bw.databases
-    )
-
-    res = pd.DataFrame(data)
-    return res.set_index("name")
-
-
-def with_db_context(func=None, arg="self"):
-    """Internal decorator wrapping function into DbContext, using its first parameters (either Activity, Db or Db name)"""
-
-    if func is None:
-        return functools.partial(with_db_context, arg=arg)
-
-    param_specs = inspect.signature(func).parameters
-
-    if arg not in param_specs:
-        raise Exception("No param %s in signature of %s" % (arg, func))
-
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs):
-        # Transform all parameters (positionnal and named) to named ones
-        all_param = {k: args[n] if n < len(args) else v.default for n, (k, v) in enumerate(param_specs.items()) if k != "kwargs"}
-        all_param.update(kwargs)
-
-        val = all_param[arg]
-        if hasattr(val, "key"):
-            # value is an activity
-            dbname = val.key[0]
-        elif isinstance(val, str):
-            # Value is directly a  db_name
-            dbname = val
-        else:
-            raise Exception("Param %s is neither an Activity or a db_name : %s" % (arg, val))
-
-        with DbContext(dbname):
-            return func(*args, **kwargs)
-
-    return wrapper
+from .base_utils import ValueOrExpression, getActByCode
+from .log import logger, warn
+from .settings import Settings
+from .units import is_dimensionless, is_equivalent, parse_db_unit
+from .units import unit_registry as u
+
+# Can be used in expression of amount for updateExchanges, in order to reference the previous value
+old_amount = symbols("old_amount")
+old_amount_with_unit = symbols("old_amount") * u.old_unit
 
 
 def _exch_name(exch):
     return exch["name"] if "name" in exch else str(exch.input)
 
 
 class ActivityExtended(Activity):
@@ -162,29 +57,35 @@
 
             input = bw.get_activity(exc.input.key)
             amount = _getAmountOrFormula(exc)
             res.append((exc["name"], input, amount))
         return res
 
     @with_db_context
-    def getExchange(self, name=None, input=None, single=True):
+    def getExchange(self, name: str = None, input: Activity = None, single=True):
         """Get exchange by name or input
 
         Parameters
         ----------
-        name : name of the exchange. Name can be suffixed with '#LOCATION' to distinguish several exchanges with same name. \
+        name :
+            name of the exchange. Name can be suffixed with '#LOCATION' to distinguish several exchanges with same name. \
             It can also be suffised by '*' to match an exchange starting with this name. Location can be a negative match '!'
-            Exampple : "Wood*#!RoW" matches any exchange with name  containing Wood, and location not "RoW"
+            Example  "Wood*#!RoW" matches any exchange with name  containing Wood, and location not "RoW"
+
+        input :
+            input activity
 
-        single :True if a single match is expected. Otherwize, a list of result is returned
+        single :
+            True if a single match is expected. Otherwize, a list of result is returned
 
         Returns
         -------
-            Single exchange or list of exchanges (if _single is False or "name" contains a '*')
-            raise Exception if not matching exchange found
+        Single exchange or list of exchanges (if _single is False or "name" contains a '*')
+        raise Exception if not matching exchange found
+
         """
 
         def single_match(name, exch):
             # Name can be "Elecricity#RER"
             if "#" in name:
                 name, loc = name.split("#")
                 negative = False
@@ -208,15 +109,15 @@
                     return any(single_match(iname, exch) for iname in name)
                 else:
                     return single_match(name, exch)
 
             if input:
                 return input == exch["input"]
 
-        exchs = list(exch for exch in self.exchangesNp() if match(exch))
+        exchs = list(exch for exch in self.non_production_exchanges() if match(exch))
         if len(exchs) == 0:
             raise Exception("Found no exchange matching name : %s" % name)
 
         if single and len(exchs) != 1:
             raise Exception("Expected 1 exchange with name '%s' found %d" % (name, len(exchs)))
         if single:
             return exchs[0]
@@ -233,120 +134,190 @@
 
         Parameters
         ----------
         updates : Dict of "<exchange name>" => <new value>
 
             <exchange name> can be suffixed with '#LOCATION' to distinguish several exchanges with same name. \
             It can also be suffixed by '*' to match an exchange starting with this name. Location can be a negative match '!'
-            Exampple : "Wood*#!RoW" matches any exchange with name  containing Wood, and location not "RoW"
+            Example : "Wood*#!RoW" matches any exchange with name  containing Wood, and location not "RoW"
 
             <New Value>  : either single value (float or SympPy expression) for updating only amount, \
                 or activity for updating only input,
             or dict of attributes, for updating both at once, or any other attribute.
             The amount can reference the symbol 'old_amount' that will be replaced with the current amount of the exchange.
         """
 
         # Update exchanges
-        for name, attrs in updates.items():
-            exchs = self.getExchange(name, single="*" not in name)
-            if not isinstance(exchs, list):
-                exchs = [exchs]
+        for ex_name, updates in updates.items():
+            # Build input & amount
+            if updates is not None and not isinstance(updates, dict):
+                if isinstance(updates, Activity):
+                    updates = dict(input=updates)
+                else:
+                    updates = dict(amount=updates)
 
-            for exch in exchs:
-                if attrs is None:
+            # Find echzanges matching name
+            matching_exchanges = self.getExchange(ex_name, single="*" not in ex_name)
+            if not isinstance(matching_exchanges, list):
+                matching_exchanges = [matching_exchanges]
+
+            # Loop on matching echanges to update
+            for exch in matching_exchanges:
+                # Delete exchange
+                if updates is None:
                     exch.delete()
                     exch.save()
                     continue
+                else:
+                    self._update_exchange(exch, updates)
 
-                # Single value ? => amount
-                if not isinstance(attrs, dict):
-                    if isinstance(attrs, Activity):
-                        attrs = dict(input=attrs)
-                    else:
-                        attrs = dict(amount=attrs)
-
-                if "amount" in attrs:
-                    attrs.update(_amountToFormula(attrs["amount"], exch["amount"]))
+    def deleteExchanges(self, name, single=True):
+        """Remove matching exchanges
 
-                exch.update(attrs)
-                exch.save()
+        Parameters
+        ----------
+        name:
+            Name of the exchange to delete. Can contain wildcards. See #getExchange for more details.
 
-    def deleteExchanges(self, name, single=True):
-        """Remove matching exchanges"""
+        single:
+            If true (default) expect to only delete a single exchange
+        """
         exchs = self.getExchange(name, single=single)
         if not isinstance(exchs, list):
             exchs = [exchs]
         if len(exchs) == 0:
             raise Exception("No exchange found for '%s'" % name)
         for ex in exchs:
             ex.delete()
             ex.save()
         self.save()
 
     @with_db_context
-    def substituteWithDefault(
-        self,
-        exchange_name: str,
-        switch_act: Activity,
-        paramSwitch: EnumParam,
-        amount=None,
-    ):
-        """Substitutes one exchange with a switch on other activities,
-        or fallback to the current one as default (parameter set to None)
-        For this purpose, we create a new exchange referencing the activity switch,
-        and we multiply current activity by '<param_name>_default',
-        making it null as soon as one enum value is set.
-
-        This is useful for changing electricty mix, leaving the default one if needed
-
-        Parameters
-        ----------
-        act : Activity to update
-        exchange_name : Name of the exchange to update
-        switch_act : Activity to substitue as input
-        amount : Amount of the input (uses previous amount by default)
-        """
-
-        current_exch = self.getExchange(exchange_name)
-
-        prev_amount = amount if amount else _getAmountOrFormula(current_exch)
-
-        self.addExchanges({switch_act: prev_amount})
-        self.updateExchanges({exchange_name: paramSwitch.symbol(None) * prev_amount})
-
-    @with_db_context
-    def addExchanges(self, exchanges: Dict[Activity, Union[NumOrExpression, dict]] = dict()):
+    def addExchanges(self, exchanges: Dict[Activity, Union[ValueOrExpression, dict]] = dict()):
         """Add exchanges to an existing activity, with a compact syntax :
 
         Parameters
         ----------
-        exchanges : Dict of activity => amount or activity => attributes_dict. \
+        exchanges :
+            Dict of activity => amount or activity => attributes_dict. \
             Amount being either a fixed value or Sympy expression (arithmetic expression of Sympy symbols)
         """
 
         with DbContext(self.key[0]):
-            for sub_act, attrs in exchanges.items():
-                if isinstance(attrs, dict):
-                    amount = attrs.pop("amount")
-                else:
-                    amount = attrs
-                    attrs = dict()
+            for sub_act, updates in exchanges.items():
+                if not isinstance(updates, dict):
+                    updates = dict(amount=updates)
 
                 exch = self.new_exchange(
                     input=sub_act.key,
                     name=sub_act["name"],
                     unit=sub_act["unit"] if "unit" in sub_act else None,
                     type="production" if self == sub_act else "technosphere" if sub_act.get("type") == "process" else "biosphere",
                 )
 
-                exch.update(attrs)
-                exch.update(_amountToFormula(amount))
-                exch.save()
+                self._update_exchange(exch, updates)
+
             self.save()
 
+    def _transform_unit(self, amount: ValueOrExpression, exchange_unit: str):
+        if not Settings.units_enabled:
+            return amount
+
+        # Parse unit
+        if exchange_unit is None:
+            logger.warn("Missing unit for target activity; Assuming dimensionless")
+            exchange_unit = u.dimensionless
+        else:
+            exchange_unit = parse_db_unit(exchange_unit)
+
+        if not isinstance(amount, Quantity):
+            if not is_dimensionless(exchange_unit) and not self.isSwitch() and amount != 0:
+                raise Exception(
+                    f"Unit '{exchange_unit}' expected, and dimensionless amount provided in a non-switch Activity: {amount}"
+                )
+            else:
+                return amount
+
+        # Help the compiler
+        amount: Quantity
+
+        act_unit = parse_db_unit(self["unit"])
+
+        if self.isSwitch() and (exchange_unit != act_unit):
+            raise Exception(f"Units should be the same in a switch activity {exchange_unit} != {act_unit}")
+
+        # Using 'old_amount' ? => replace with requested unit
+        if amount.units == u.old_unit:
+            amount = u.Quantity(amount.magnitude, exchange_unit)
+
+        # We try to transform either to the exchange unit, or ex_unit/act_unit
+        for target_unit in [exchange_unit, exchange_unit / act_unit]:
+            # We'll catch error at the end if none of the target units worked
+            if not is_equivalent(target_unit, amount.units):
+                continue
+
+            # Try to convert
+            new_amount = amount.to(target_unit).magnitude
+
+            # Auto scale disabld ?
+            if not _equals(amount.magnitude, new_amount) and not u.auto_scale:
+                raise Exception(f"auto_scale is disabled. '{amount}' should be explicity transformed to {target_unit}")
+
+            return new_amount
+
+        # At this point, no convertion worked :
+        raise DimensionalityError(
+            amount.units,
+            exchange_unit,
+            f"Unit of amount '{amount}' is not compatible with physical unit of exchange '{exchange_unit}' or the "
+            f"unit of exchange divided by the unit of the activity : '{exchange_unit / act_unit}'",
+        )
+
+    def _amount_to_formula(self, amount: ValueOrExpression, exchange: ExchangeDataset):
+        res = dict()
+        if isinstance(amount, Basic):
+            current_amount = exchange.get("amount", None)
+            if current_amount is not None:
+                amount = amount.subs(old_amount, current_amount)
+
+            # Check the expression does not reference undefined params
+            all_symbols = list([key for param in _param_registry().values() for key, val in param.expandParams().items()])
+            for symbol in amount.free_symbols:
+                if not str(symbol) in all_symbols:
+                    raise Exception("Symbol '%s' not found in params : %s" % (symbol, all_symbols))
+
+            res["formula"] = str(amount)
+            res["amount"] = 0
+        elif isinstance(amount, float) or isinstance(amount, int):
+            res["amount"] = amount
+        else:
+            raise Exception(
+                "Amount should be either a constant number or a Sympy expression (expression of ParamDef). Was : %s"
+                % type(amount)
+            )
+        return res
+
+    def _update_exchange(self, exchange: ExchangeDataset, updates):
+        """Update a single exchange. Take care of setting amount / formula accordingly"""
+        amount = updates.pop("amount") if "amount" in updates else None
+
+        if amount is not None:
+            # Update units
+            amount = self._transform_unit(amount, exchange["unit"])
+
+            # Extract formula if two separate field "amount" and "formula"
+            # Update the list of updates
+            updates.update(self._amount_to_formula(amount, exchange))
+
+        exchange.update(updates)
+        exchange.save()
+
+    def isSwitch(self):
+        return self.get("switch", False)
+
     @with_db_context
     def getAmount(self, *args, sum=False, **kargs):
         """
         Get the amount of one or several exchanges, selected by name or input. See #getExchange()
         """
         exchs = self.getExchange(*args, single=not sum, **kargs)
         if sum:
@@ -365,42 +336,30 @@
 
         for exch in self.exchanges():
             if (exch["input"] == exch["output"]) and (exch["type"] == "production"):
                 res = exch["amount"]
                 break
         return res
 
-    def exchangesNp(self):
+    def non_production_exchanges(self):
         """List of exchange, except production (output) one."""
         for exch in self.exchanges():
             if exch["input"] != exch["output"]:
                 yield exch
 
     def updateMeta(self, **kwargs):
-        """Update any property. Useful to update axis"""
+        """Update any property. Useful to update axes"""
         for key, val in kwargs.items():
             self._data[key] = val
         self.save()
 
 
-# Backport new methods to vanilla Activity class in order to benefit from it for all existing instances
-for name, item in ActivityExtended.__dict__.items():
-    if isinstance(item, types.FunctionType):
-        setattr(Activity, name, item)
-
-
-def getActByCode(db_name, code):
-    """Get activity by code"""
-    return _getDb(db_name).get(code)
-
-
 def findActivity(
     name=None,
     loc=None,
-    in_name=None,
     code=None,
     categories=None,
     category=None,
     db_name=None,
     single=True,
     case_sensitive=False,
     unit=None,
@@ -408,25 +367,26 @@
 ) -> ActivityExtended:
     """
         Find activity by name & location
         Uses index for fast fetching
 
     :param name: Name of the activity. Can contain '*' for searching partial chain
     :param loc: optional location
-    :param in_name: Same as using name="something*"
     :param code: Unique code. If provided alone, returns the activity for this code
     :param categories: Optional : exact list of catagories
     :param category: Optional : single category that should be part of the list of categories of the selected activities
     :param db_name: Name of the database
     :param single: If False, returns a list of matching activities. If True (default) fails if more than one activity fits.
     :param case_sensitive: If True (default) ignore the case
     :param unit: If provided, only match activities with provided unit
     :return: Either a single activity (if single is True) or a list of activities, possibly empty.
     """
 
+    in_name = None
+
     if name and "*" in name:
         in_name = name.replace("*", "")
         name = None
 
     if not case_sensitive:
         if name:
             name = name.lower()
@@ -489,207 +449,148 @@
 def findBioAct(name=None, loc=None, **kwargs):
     """Alias for findActivity(name, ... db_name=BIOSPHERE3_DB_NAME). See doc for #findActivity"""
     return findActivity(name=name, loc=loc, db_name=_find_biosphere_db(), **kwargs)
 
 
 def findTechAct(name=None, loc=None, single=True, **kwargs):
     """
-    Search activities in technosphere. This function try to guess which database is your background database.
+    Search activities in technosphere. This function tries to guess which database is your background database.
+    If you have more than one background technosphere, you should use findActivity() and specify the **db_name** directly.
     See also doc for #findActivity"""
     dbs = _listTechBackgroundDbs()
     if len(dbs) > 1:
         raise Exception(
             "There is more than one technosphere background DB (%s) please use findActivity(..., db_name=YOUR_DB)" % str(dbs)
         )
 
     return findActivity(name=name, loc=loc, db_name=dbs[0], single=single, **kwargs)
 
 
-def _amountToFormula(amount: Union[float, str, Basic], currentAmount=None):
-    """Transform amount in exchange to either simple amount or formula"""
-    res = dict()
-    if isinstance(amount, Basic):
-        if currentAmount is not None:
-            amount = amount.subs(old_amount, currentAmount)
-
-        # Check the expression does not reference undefined params
-        all_symbols = list([key for param in _param_registry().values() for key, val in param.expandParams().items()])
-        for symbol in amount.free_symbols:
-            if not str(symbol) in all_symbols:
-                raise Exception("Symbol '%s' not found in params : %s" % (symbol, all_symbols))
-
-        res["formula"] = str(amount)
-        res["amount"] = 0
-    elif isinstance(amount, float) or isinstance(amount, int):
-        res["amount"] = amount
-    else:
-        raise Exception(
-            "Amount should be either a constant number or a Sympy expression (expression of ParamDef). Was : %s" % type(amount)
-        )
-    return res
+def _equals(val1: ValueOrExpression, val2: ValueOrExpression):
+    """Compare float of Sympy values"""
+    if val1 == val2:
+        return True
+    if isinstance(val1, Basic) != isinstance(val2, Basic):
+        return False
+    return simplify(val1 / val2) == 1.0
 
 
 def _newAct(db_name, code):
     if not _isForeground(db_name):
-        error(
+        warn(
             "WARNING: You are creating activity in background DB. You should only do it in your foreground / user DB : ",
             db_name,
         )
 
     db = _getDb(db_name)
     # Already present : delete it ?
     for act in db:
         if act["code"] == code:
-            error("Activity '%s' was already in '%s'. Overwriting it" % (code, db_name))
+            warn("Activity '%s' was already in '%s'. Overwriting it" % (code, db_name))
             act.delete()
 
     return db.new_activity(code)
 
 
 def newActivity(
     db_name,
     name,
     unit,
     exchanges: Dict[Activity, Union[float, str]] = dict(),
     amount=1,
     code=None,
     type="process",
+    switchActivity=False,
     **argv,
-):
+) -> ActivityExtended:
     """Creates a new activity
 
     Parameters
     ----------
-    name : Name of the new activity
-    db_name : Destination DB : ACV DB by default
-    unit: Unit of the process
-
-    code: Unique code in the Db. Optional. If not provided, Name is used
-    exchanges : Dict of activity => amount. If amount is a string, is it considered as a formula with parameters
-    argv : extra params passed as properties of the new activity
-    amount: Production amount. 1 by default
+    name :
+        Name of the new activity
+    db_name :
+        Destination DB : ACV DB by default
+    unit:
+        Unit of the process
+
+    code:
+        Unique code in the Db. Optional. If not provided, the name is used
+
+    exchanges :
+        Dict of activity => amount. See the doc for @addExchanges()
+
+    argv :
+        Any extra params passed as properties of the new activity
+
+    switch:
+        Activities marked as *switch* are expected to be linear combination of activities of same unit.
+        This option changes how physical units are checked.
+
+    amount:
+        Production amount. 1 by default
     """
 
     code = code if code else name
 
     act = _newAct(db_name, code)
     act["name"] = name
     act["type"] = type
     act["unit"] = unit
+    if switchActivity:
+        act["switch"] = True
+
     act.update(argv)
 
     # Add single production exchange
     if type == "process":
         ex = act.new_exchange(
             input=act.key,
             name=act["name"],
             unit=act["unit"],
             type="production",
-            amount=1,
+            amount=amount,
         )
         ex.save()
 
         act["reference product"] = act["name"]
         act.save()
 
     # Add exchanges
     act.addExchanges(exchanges)
 
     return act
 
 
-def _segments_to_piecewise(param, segments):
-    conds = []
-    for start, end, val in segments:
-        cond = True
-        if start is not None:
-            cond = cond & (param >= start)
-        if end is not None:
-            cond = cond & (param < end)
-        conds.append((val, simplify(cond)))
-
-    return Piecewise(*conds, (0, True))
+def copyActivity(db_name, activity: ActivityExtended, code=None, withExchanges=True, **kwargs) -> ActivityExtended:
+    """Copy an activity and its exchanges into another database. You usually want to copy activities from your background to
+    your foreground DB to update them, keeping your background DB clean.
 
+    Parameters
+    ----------
+    db_name:
+        Name of the target database
+    activity:
+        Source activity
+    code:
+        Code of the target activity. Also used as its name
 
-def interpolate_activities(
-    db_name,
-    act_name,
-    param: ParamDef,
-    act_per_value: Dict,
-    add_zero=False,
-):
-    """
-     Creates a linear virtual activity being a linear interpolation between several activities,
-     based on the values of a given parameter.
 
-     This is useful to produce a continuous parametrized activity based on the scale of the system,
-     given that you have dicrete activities coresponding to
-     discrete values of the parameter.
-
-    :param db_name: Name of user DB (string)
-    :param act_name: Name of the new activity
-    :param param: Parameter to use [ParamDef]
-    :param act_per_value : Dictionnary of value => activitiy [Dict]
-    :param add_zero: If True add the "Zero" point to the data. Usefull for linear interoplation of a single activity / point
-    :return: the new activity
+    Returns
+    -------
+        The new activity. note that is is flagged with the custom property **inherited_from**, providing the full key of the
+        initial activity.
     """
 
-    # Add "Zero" to the list
-    act_per_value = act_per_value.copy()
-
-    if add_zero:
-        act_per_value[0.0] = None
-
-    # List of segments : triplet of (start, end, expression)
-    segments = defaultdict(list)
-
-    # Transform to sorted list of value => activity
-    sorted_points = sorted(act_per_value.items(), key=lambda item: item[0])
-    for i, (curr_val, curr_act) in enumerate(sorted_points):
-        if i >= len(sorted_points) - 1:
-            continue
-
-        # Next val and act
-        next_val, next_act = sorted_points[i + 1]
-
-        # Boundaries of segment : none if first / last point
-        start = curr_val if i > 0 else None
-        end = next_val if i < (len(sorted_points) - 2) else None
-
-        # Add segment for current activity
-        segments[curr_act].append(
-            [start, end, (param - next_val) / (curr_val - next_val)]
-        )  # Will equal 1 at current point and 0 at next point
-
-        # Add segment for next activity
-        segments[next_act].append(
-            [start, end, (param - curr_val) / (next_val - curr_val)]
-        )  # Will equal 0 at current point and 1 at next point
-
-    # Transform segments into piecewize expressions
-    exchanges = {act: _segments_to_piecewise(param, segs) for act, segs in segments.items() if act is not None}
-
-    # Find unit
-    units = list(act["unit"] for act in exchanges.keys())
-    same_unit = all(x == units[0] for x in units)
-
-    if not same_unit:
-        error("Warning : units of activities should be the same : %s" % str(units))
-
-    # Create act
-    new_act = newActivity(db_name=db_name, name=act_name, unit=units[0], exchanges=exchanges)
-
-    return new_act
-
-
-def copyActivity(db_name, activity: ActivityExtended, code=None, withExchanges=True, **kwargs) -> ActivityExtended:
-    """Copy activity into a new DB"""
-
     res = _newAct(db_name, code)
 
+    # Same code if not provided
+    if code is None:
+        code = activity.key[1]
+
     for key, value in activity.items():
         if key not in ["database", "code"]:
             res[key] = value
     for k, v in kwargs.items():
         res._data[k] = v
     res._data["code"] = code
     res["name"] = code
@@ -705,33 +606,35 @@
             if exc["input"] == exc["output"]:
                 data["input"] = res.key
             ExchangeDataset.create(**dict_as_exchangedataset(data))
 
     return res
 
 
-ValueOrExpression = Union[int, float, Expr]
-
 ActivityOrActivityAmount = Union[Activity, Tuple[Activity, float]]
 
 
 def newSwitchAct(dbname, name, paramDef: ParamDef, acts_dict: Dict[str, ActivityOrActivityAmount]):
-    """Create a new parametrized, virtual activity, made of a map of other activities, controlled by an enum parameter.
+    """Creates a new parametrized, virtual activity, made of a map of other activities, controlled by an enum parameter.
     This enables to implement a "Switch" with brightway parameters
     Internally, this will create a linear sum of other activities controlled by <param_name>_<enum_value> : 0 or 1
 
     By default, all activities have associated amount of 1.
     You can provide other amounts by providing a tuple of (activity, amount).
 
     Parameters
     ----------
-    dbname: name of the target DB
-    name: Name of the new activity
-    paramDef : parameter definition of type enum
-    acts_dict : dict of "enumValue" => activity or "enumValue" => (activity, amount)
+    dbname:
+        name of the target DB
+    name:
+        Name of the new activity
+    paramDef :
+        parameter definition of type enum
+    acts_dict :
+        dict of "enumValue" => activity or "enumValue" => (activity, amount)
 
     Examples
     --------
 
     >>> newSwitchAct(MYDB, "switchAct", switchParam, {
     >>>    "val1" : act1 # Amount is 1
     >>>    "val2" : (act2, 0.4) # Different amount
@@ -747,41 +650,47 @@
     for key, act in acts_dict.items():
         amount = 1
         if isinstance(act, (list, tuple)):
             act, amount = act
         exch[act] += amount * paramDef.symbol(key)
         unit = act["unit"]
 
-    res = newActivity(dbname, name, unit=unit, exchanges=exch)
+    res = newActivity(dbname, name, unit=unit, exchanges=exch, switch=True)
 
     return res
 
 
-def switchValue(param: EnumParam, **values: Dict[str, ValueOrExpression]):
-    """Defines different formulas for each value of an eum"""
+def _actDesc(act: ActivityExtended):
+    """Generate pretty name for activity + basic information"""
+    name = _actName(act)
+    amount = act.getOutputAmount()
 
-    res = 0
-    for key, val in values.items():
-        res += param.symbol(key) * val
-    return res
+    return "%s (%f %s)" % (name, amount, act["unit"])
 
 
-def printAct(*args, **params):
+def printAct(*activities, **params):
     """
     Print activities and their exchanges.
     If parameter values are provided, formulas will be evaluated accordingly.
-    If impact is provided it will be computed.
 
-    :return A Dataframe.
+    Parameters
+    ----------
+    activities:
+        One or two activities. If two activities are provided, differences are highlighted.
+
+    params:
+        If provided, the formulas are evaluated accordingly and the result amount is shown instead of formula
+
+    Returns
+    -------
+        A Dataframe is returned, containing all information, exchange by exchange
     """
     tables = []
     names = []
 
-    activities = args
-
     for act in activities:
         with DbContext(act.key[0]):
             inputs_by_ex_name = dict()
             df = pd.DataFrame(index=["input", "amount", "unit"])
             data = dict()
             for i, exc in enumerate(act.exchanges()):
                 # Don't show production
@@ -847,79 +756,11 @@
             return res
 
         full = full.style.apply(same_amount, axis=1)
 
     return full
 
 
-def newInterpolatedAct(
-    dbname: str,
-    name: str,
-    act1: ActivityExtended,
-    act2: ActivityExtended,
-    x1,
-    x2,
-    x,
-    alpha1=1,
-    alpha2=1,
-    **kwargs,
-):
-    """Creates a new activity made of interpolation of two similar activities.
-    For each exchange :
-    amount = alpha1 * a1 + (x - X1) * (alpha2 * a2 - alpha1 * a1) / (x2 - x1)
-
-    Parameters
-    ----------
-    name : Name of new activity
-    act1 : Activity 1
-    act2 : Activity 2
-    x1 : X for act1
-    x2 : X for act 2
-    x : Should be a parameter symbol
-    alpha1 : Ratio for act1 (Default value = 1)
-    alpha2 : Ratio for act2 (Default value = 1)
-    kwargs : Any other param will be added as attributes of new activity
-    """
-    res = copyActivity(dbname, act1, name, withExchanges=False, **kwargs)
-
-    exch1_by_input = dict({exch["input"]: exch for exch in act1.exchangesNp()})
-    exch2_by_input = dict({exch["input"]: exch for exch in act2.exchangesNp()})
-
-    inputs = set(chain(exch1_by_input.keys(), exch2_by_input.keys()))
-
-    for input in inputs:
-        exch1 = exch1_by_input.get(input)
-        exch2 = exch2_by_input.get(input)
-        exch = exch1 if exch1 else exch2
-
-        amount1 = exch1["amount"] if exch1 else 0
-        amount2 = exch2["amount"] if exch2 else 0
-
-        if exch1 and exch2 and exch1["name"] != exch2["name"]:
-            raise Exception("Input %s refer two different names : %s, %s" % (input, exch1["name"], exch2["name"]))
-
-        amount = interpolate(x, x1, x2, amount1 * alpha1, amount2 * alpha2)
-        act = getActByCode(*input)
-        res.addExchanges({act: dict(amount=amount, name=exch["name"])})
-    return res
-
-
-def findMethods(search=None, mainCat=None):
-    """
-    Find impact method. Search in all methods against a list of match strings.
-    Each parameter can be either an exact match match, or case insenstive search, if suffixed by '*'
-
-    Parameters
-    ----------
-    search : String to search
-    mainCat : if specified, limits the research for method[0] == mainCat.
-    """
-    res = []
-    search = search.lower()
-    for method in bw.methods:
-        text = str(method).lower()
-        match = search in text
-        if mainCat:
-            match = match and (mainCat == method[0])
-        if match:
-            res.append(method)
-    return res
+# Backport new methods to vanilla Activity class in order to benefit from it for all existing instances
+for name, item in ActivityExtended.__dict__.items():
+    if isinstance(item, FunctionType):
+        setattr(Activity, name, item)
```

### Comparing `lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/io.py` & `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 import brightway2 as bw
 from bw2data.parameters import DatabaseParameter, ProjectParameter
 from bw2io import BW2Package
 
-from lca_algebraic.base_utils import error
+from lca_algebraic.log import warn
 from lca_algebraic.params import _listParams, loadParams
 
 __all__ = ["export_db", "import_db"]
 
 
-def param_data(param):
+def _param_data(param):
     """Return param data except id"""
     res = {key: val for key, val in param.__data__.items() if key != "id"}
     data = res.pop("data")
     res.update(data)
 
     return res
 
 
 def export_db(db_name, filename):
-    """Export Db and linked parameters"""
+    """This function exports a database to the **BW2Package** format, including the definition of parameters"""
     db = bw.Database(db_name)
     db_params = DatabaseParameter.select().where(DatabaseParameter.database == db_name)
 
     # Export Db params
-    db.metadata["database_parameters"] = [param_data(param) for param in db_params]
+    db.metadata["database_parameters"] = [_param_data(param) for param in db_params]
 
     # List of all project params used in this dataset
     used_project_params = list(param.name for param in _listParams(db_name) if param.dbname is None)
 
     if len(used_project_params) > 0:
-        error(
+        warn(
             "Warning : this DB uses project parameters that are exported as well "
             "and might override project params at import time : ",
             used_project_params,
         )
 
         proj_params = list(ProjectParameter.get(ProjectParameter.name == name) for name in used_project_params)
 
-        db.metadata["project_parameters"] = [param_data(param) for param in proj_params]
+        db.metadata["project_parameters"] = [_param_data(param) for param in proj_params]
 
     BW2Package._write_file(filename, [BW2Package._prepare_obj(db, False)])
 
 
 def import_db(filename):
-    """Export Db and linked parameters"""
+    """Import Db from BW2Package with linked parameters (as produced by **export_db**)"""
 
     db = BW2Package.import_file(filename)[0]
     if "database_parameters" in db.metadata:
         params = db.metadata["database_parameters"]
         bw.parameters.new_database_parameters(params, db.name)
 
     if "project_parameters" in db.metadata:
```

### Comparing `lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/lca.py` & `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/lca.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,89 @@
-import builtins
 import concurrent.futures
+import re
 from collections import OrderedDict
 from dataclasses import dataclass
-from typing import List
-from warnings import warn
+from types import FunctionType
+from typing import Dict, List, Optional, Union
 
+import brightway2 as bw
 import numpy as np
 import pandas as pd
 from peewee import DoesNotExist
-from sympy import Symbol, lambdify, parse_expr
+from pint import Quantity, Unit
+from sympy import Basic, Symbol, lambdify, parse_expr, simplify, symbols
+from sympy.printing.numpy import NumPyPrinter
+from typing_extensions import deprecated
 
-from . import TabbedDataframe
+from . import newActivity
+from .activity import ActivityExtended
 from .axis_dict import AxisDict
-from .base_utils import _actName, _getDb, _method_unit
-from .cache import ExprCache, LCIACache
-from .helpers import (
-    BIOSPHERE_PREFIX,
-    Activity,
-    ActivityExtended,
-    Basic,
-    DbContext,
-    Dict,
-    _actDesc,
-    _getAmountOrFormula,
-    _isForeground,
-    bw,
-    error,
-    newActivity,
-    re,
-    simplify,
-    symbols,
-    types,
-    with_db_context,
+from .base_utils import (
+    TabbedDataframe,
+    ValueOrExpression,
+    _actName,
+    _getDb,
+    _user_functions,
 )
-from .log import logger
+from .cache import ExprCache, LCIACache
+from .database import BIOSPHERE_PREFIX, DbContext, _isForeground, with_db_context
+from .log import logger, warn
+from .methods import method_name, method_unit
 from .params import (
     FixedParamMode,
     _complete_params,
     _compute_param_length,
     _expand_param_names,
     _expand_params,
     _expanded_names_to_names,
     _fixed_params,
+    _getAmountOrFormula,
     _param_registry,
     _toSymbolDict,
     all_params,
-    compute_expr_value,
     freezeParams,
 )
 
 
-def _impact_labels():
-    """Dictionnary of custom impact names
-    Dict of "method tuple" => string
-    """
-    # Prevent reset upon auto reload in jupyter notebook
-    if "_impact_labels" not in builtins.__dict__:
-        builtins._impact_labels = dict()
-
-    return builtins._impact_labels
-
+def register_user_function(sym, func):
+    """Register a custom function with is python implementation
+    Parameters
+    ----------
+    sym : the sympy function expression
+    func : the implementation of the function
 
-def set_custom_impact_labels(impact_labels: Dict):
-    """Global function to override name of impact method in graphs"""
-    _impact_labels().update(impact_labels)
+    Examples
+    --------
+    >>> def func_add(*args):
+            returm sum(*args)
+    >>>
+    >>> func_add_sym = register_user_function(sympy.Function('func_add', real=True, imaginary=False), func_add)
+    >>> e = sympy.Symbol('a') * func_add_sym(sympy.Symbol('b'), sympy.Symbol('c'))
+    >>> sympy.srepr(e)
+    "Mul(Symbol('a'), Function('func_add')(Symbol('b'), Symbol('c')))"
+    """
+    global _user_functions
+    _user_functions[sym.name] = (sym, func)
+    return sym
+
+
+def user_function(sym):
+    """Function decorator to register user function
+
+    Usage
+    -----
+    >>> @user_function(sympy.Function('func_add', real=True, imaginary=False))
+    >>> def func_add(*args):
+            returm sum(*args)
+    >>>
+    >>> e = sympy.Symbol('a') * func_add(sympy.Symbol('b'), sympy.Symbol('c'))
+    >>> sympy.srepr(e)
+    "Mul(Symbol('a'), Function('func_add')(Symbol('b'), Symbol('c')))"
+    """
+    return lambda func: register_user_function(sym, func)
 
 
 def _multiLCA(activities, methods):
     """Simple wrapper around brightway API"""
     bw.calculation_setups["process"] = {"inv": activities, "ia": methods}
     lca = bw.MultiLCA("process")
     cols = [_actName(act) for act_amount in activities for act, amount in act_amount.items()]
@@ -207,16 +223,23 @@
     else:
         # Static value
         return set()
 
 
 def _lambdify(expr: Basic, expanded_params):
     """Lambdify, handling manually the case of SymDict (for impacts by axis)"""
+
+    printer = NumPyPrinter(
+        {"fully_qualified_modules": False, "inline": True, "allow_unknown_functions": True, "user_functions": dict()}
+    )
+
+    modules = [{x[0].name: x[1] for x in _user_functions.values()}, "numpy"]
+
     if isinstance(expr, Basic):
-        lambd = lambdify(expanded_params, expr, "numpy")
+        lambd = lambdify(expanded_params, expr, modules, printer=printer, cse=LambdaWithParamNames._use_sympy_cse)
 
         def func(*arg, **kwargs):
             res = lambd(*arg, **kwargs)
             if isinstance(res, dict):
                 # Transform key symbols into Str
                 return {str(k): v for k, v in res.items()}
             else:
@@ -228,47 +251,45 @@
         # Not an expression : return static func
         def static_func(*args, **kargs):
             return expr
 
         return static_func
 
 
-def compute_param_formulas(param_values: Dict, required_params: List[str]):
-    # Compute the values params computed from formulas (and not specified in input)
-    pass
-
-
 @dataclass
 class ValueContext:
     """Represents a result value, with all parameters values used in context"""
 
     value: float
     context: Dict[str, float]
 
 
 class LambdaWithParamNames:
     """
     This class represents a compiled (lambdified) expression together
     with the list of requirement parameters and the source expression
     """
 
+    _use_sympy_cse = False
+
     def __init__(self, exprOrDict, expanded_params=None, params=None, sobols=None):
         """Computes a lamdda function from expression and list of expected parameters.
         you can provide either the list pf expanded parameters (full vars for enums) for the 'user' param names
         """
 
         if isinstance(exprOrDict, dict):
             # Come from JSON serialization
             obj = exprOrDict
             # LIst of required params for this lambda
             self.params: List[str] = obj["params"]
 
             # Full names
             self.expanded_params = _expand_param_names(self.params)
-            self.expr = parse_expr(obj["expr"])
+            local_dict = {x[0].name: x[0] for x in _user_functions.values()}
+            self.expr = parse_expr(obj["expr"], local_dict=local_dict)
             self.lambd = _lambdify(self.expr, self.expanded_params)
             self.sobols = obj["sobols"]
 
         else:
             self.expr = exprOrDict
             self.params = params
 
@@ -317,55 +338,61 @@
 
         return ValueContext(value=value, context=completed_params)
 
     def serialize(self):
         expr = str(self.expr)
         return dict(params=self.params, expr=expr, sobols=self.sobols)
 
+    @staticmethod
+    def use_sympy_cse(b=True):
+        LambdaWithParamNames._use_sympy_cse = b
+
     def __repr__(self):
         return repr(self.expr)
 
     def _repr_latex_(self):
         return self.expr._repr_latex_()
 
 
-def _preMultiLCAAlgebric(model: ActivityExtended, methods, alpha=1, axis=None):
+def lambdify_expr(expr):
+    return LambdaWithParamNames(expr, params=[param.name for param in _param_registry().values()])
+
+
+def _preMultiLCAAlgebric(model: ActivityExtended, methods, alpha: ValueOrExpression = 1, axis=None):
     """
     This method transforms an activity into a set of functions ready to compute LCA very fast on a set on methods.
     You may use is and pass the result to postMultiLCAAlgebric for fast computation on a model that does not change.
 
     This method is used by multiLCAAlgebric
     """
+
+    # Using units ? Only keep the magnitude, drop the units
+    if isinstance(alpha, Quantity):
+        alpha = alpha.magnitude
+
     with DbContext(model):
         exprs = _modelToExpr(model, methods, alpha=alpha, axis=axis)
 
         # Lambdify (compile) expressions
         return [LambdaWithParamNames(expr) for expr in exprs]
 
 
-def method_name(method):
-    """Return name of method, taking into account custom label set via set_custom_impact_labels(...)"""
-    if method in _impact_labels():
-        return _impact_labels()[method]
-    return method[1] + " - " + method[2]
-
-
 def _slugify(str):
     return re.sub("[^0-9a-zA-Z]+", "_", str)
 
 
 @dataclass
 class ResultsWithParams:
     """Holds bith the result with context parameters"""
 
     dataframe: pd.DataFrame
     params: Dict
 
 
-def _postMultiLCAAlgebric(methods, lambdas: List[LambdaWithParamNames], with_params=False, **params):
+def _postMultiLCAAlgebric(methods, lambdas: List[LambdaWithParamNames], with_params=False, unit: Unit = None, **params):
     """
     Compute LCA for a given set of parameters and pre-compiled lambda functions.
     This function is used by **multiLCAAlgebric**
 
     Parameters
     ----------
     methodAndLambdas : Output of preMultiLCAAlgebric
@@ -411,15 +438,15 @@
     # Use multithread for that
     with concurrent.futures.ThreadPoolExecutor() as exec:
         for imethod, value in exec.map(process, enumerate(lambdas)):
             res[imethod, :] = value
 
     result = pd.DataFrame(
         res,
-        index=[method_name(method) + "[%s]" % _method_unit(method) for method in methods],
+        index=[method_name(method) + "[%s]" % method_unit(method, fu_unit=unit) for method in methods],
     ).transpose()
 
     if with_params:
         return ResultsWithParams(dataframe=result, params=context_params)
     else:
         return result
 
@@ -429,21 +456,21 @@
     res = params.copy()
 
     expected_params_names = _expanded_names_to_names(expected_names)
     for expected_name in expected_params_names:
         if expected_name not in params:
             default = _param_registry()[expected_name].default
             res[expected_name] = default
-            error("Missing parameter %s, replaced by default value %s" % (expected_name, default))
+            warn("Missing parameter %s, replaced by default value %s" % (expected_name, default))
 
     for key, value in params.items():
         if key not in expected_params_names:
             del res[key]
             if model:
-                error("Param %s not required for model %s" % (key, model))
+                warn("Param %s not required for model %s" % (key, model))
     return res
 
 
 def compute_value(formula, **params):
     """Compute actual value for a given formula, with possible parameters (or default ones)"""
     if isinstance(formula, float) or isinstance(formula, int):
         return formula
@@ -451,14 +478,15 @@
     lambd = LambdaWithParamNames(formula)
 
     value_context = lambd.compute(**params)
 
     return value_context.value
 
 
+@deprecated("multiLCAAlgebric is deprecated, use compute_impacts instead")
 def multiLCAAlgebric(*args, **kwargs):
     """deprecated. `compute_impacts()` instead"""
     warn("multiLCAAlgebric is deprecated, use compute_impacts instead")
     return compute_impacts(*args, **kwargs)
 
 
 def _params_dataframe(param_values: Dict[str, float]):
@@ -491,14 +519,17 @@
         records.append(record)
 
     df = pd.DataFrame.from_records(records).set_index(["group", "name"]).sort_index()
 
     return df
 
 
+SingleOrMultipleFloat = Union[float, List[float], np.ndarray]
+
+
 def compute_impacts(
     models,
     methods,
     axis=None,
     functional_unit=1,
     return_params=False,
     description=None,
@@ -515,22 +546,59 @@
     ----------
     models :
         Single model or
         List of model or
         List of (model, alpha)
         or Dict of model:amount
         In case of several models, you cannot use list of parameters
-    methods : List of methods / impacts to consider
-    params : You should provide named values of all the parameters declared in the model. \
-             Values can be single value or list of samples, all of the same size
-    axis: Designates the name of an attribute of user activities to split impacts by their value. \
-        This is useful to get impact by phase or sub modules
-    functional_unit: quantity (static or Sypy formula) by which to divide impacts
-    return_params: If true, also returns the value of all parameters in as tabbed DataFrame
-    description: Optional description/metadata to be added in output when using "return params" Dataframe
+
+    methods :
+        List of methods / impacts to consider
+
+    axis:
+        Designates the name of a custom attribute of foreground activities.
+        You may set this attribute using the method `myActivity.updateMeta(your_custom_attr="some_value")`
+
+        The impacts will be ventilated by this attribute.
+        This is useful to get impact by phase or sub-modules.
+
+    params:
+        Any other argument passed to this function is considered as a value of a parameter of the model :
+        Values can be either single float values, list or ndarray of values.
+        In the later case, all parameters should have the same number of values.
+        Paremeters that are not provided will have their default value set.
+
+    functional_unit:
+        Quantity (static or Sympy formula) by which to divide impacts. Optional, 1 by default.
+
+    return_params:
+        If true, also returns the value of all parameters in as tabbed DataFrame
+
+    description:
+        Optional description/metadata to be added in output when using "return params" Dataframe
+
+    Returns
+    -------
+    A dataframe with the results. If *return_params* is true, it returns `TabbedDataframe`,
+    including all parameters values, that can be saved as a multi sheet excel file.
+
+    Examples
+    --------
+    >>> compute_impacts(
+    >>>    mainAct1, # The root activity of the foreground model
+    >>>    [climate_change], # climate_change is the key (tuple) of the impact method
+    >>>    functional_unit=energy_expression, # energy expression is a Sympy expression computing the energy in kWh
+    >>>    axis="phase", # Split results by phase
+    >>>    return_params=True, # Return all parameter values
+    >>>
+    >>>    # Parameter values
+    >>>    p1=2.0,
+    >>>    p2=3.0)
+
+
     """
     dfs = dict()
 
     if isinstance(models, list):
 
         def to_tuple(item):
             if isinstance(item, tuple):
@@ -541,33 +609,40 @@
         models = dict(to_tuple(item) for item in models)
     elif not isinstance(models, dict):
         models = {models: 1}
 
     # Gather all param values (even default and computed)
     params_all = dict()
 
+    # Single method provided ?
+    if isinstance(methods, tuple):
+        methods = [methods]
+
     for model, alpha in models.items():
         if type(model) is tuple:
             model, alpha = model
 
         alpha = float(alpha)
 
         dbname = model.key[0]
         with DbContext(dbname):
             # Check no params are passed for FixedParams
             for key in params:
                 if key in _fixed_params():
-                    error("Param '%s' is marked as FIXED, but passed in parameters : ignored" % key)
+                    warn("Param '%s' is marked as FIXED, but passed in parameters : ignored" % key)
 
             if functional_unit != 1:
                 alpha = alpha / functional_unit
 
             lambdas = _preMultiLCAAlgebric(model, methods, alpha=alpha, axis=axis)
 
-            res = _postMultiLCAAlgebric(methods, lambdas, with_params=return_params, **params)
+            unit: Optional[Unit] = functional_unit.units if isinstance(functional_unit, Quantity) else None
+
+            res = _postMultiLCAAlgebric(methods, lambdas, with_params=return_params, unit=unit, **params)
+
             if return_params:
                 df = res.dataframe
                 params_all.update(res.params)
             else:
                 df = res
 
             model_name = _actName(model)
@@ -690,15 +765,15 @@
     else:
         res = expr
 
     return AxisDict({axis_tag: res})
 
 
 @with_db_context(arg="act")
-def actToExpression(act: Activity, axis=None):
+def actToExpression(act: ActivityExtended, axis=None):
     """Computes a symbolic expression of the model, referencing background activities and model parameters as symbols
 
     Returns
     -------
         (sympy_expr, dict of symbol => activity)
     """
 
@@ -734,15 +809,15 @@
         if not _isForeground(act["database"]):
             # We reached a background DB ? => stop developping and create reference to activity
             return act_to_symbol(act)
 
         for exch in act.exchanges():
             formula = _getAmountOrFormula(exch)
 
-            if isinstance(formula, types.FunctionType):
+            if isinstance(formula, FunctionType):
                 # Some amounts in EIDB are functions ... we ignore them
                 continue
 
             #  Production exchange
             if exch["input"] == exch["output"]:
                 continue
 
@@ -776,109 +851,17 @@
 
         return res
 
     expr = actToExpressionRec(act)
 
     if isinstance(expr, float):
         expr = simplify(expr)
+
     else:
         # Replace fixed params with their default value
         expr = _replace_fixed_params(expr, _fixed_params().values())
 
     return (expr, _reverse_dict(act_symbols))
 
 
 def _reverse_dict(dic):
     return {v: k for k, v in dic.items()}
-
-
-def exploreImpacts(impact, *activities: ActivityExtended, **params):
-    """
-    Advanced version of #printAct()
-
-    Displays all exchanges of one or several activities and their impacts.
-    If parameter values are provided, formulas will be evaluated accordingly.
-    If two activities are provided, they will be shown side by side and compared.
-    """
-    tables = []
-    names = []
-
-    diffOnly = params.pop("diffOnly", False)
-    withImpactPerUnit = params.pop("withImpactPerUnit", False)
-
-    for main_act in activities:
-        inputs_by_ex_name = dict()
-        data = dict()
-
-        for i, (name, input, amount) in enumerate(main_act.listExchanges()):
-            # Params provided ? Evaluate formulas
-            if len(params) > 0 and isinstance(amount, Basic):
-                amount = compute_expr_value(amount, params)
-
-            i = 1
-            ex_name = name
-            while ex_name in data:
-                ex_name = "%s#%d" % (name, i)
-                i += 1
-
-            inputs_by_ex_name[ex_name] = _createTechProxyForBio(input.key, main_act.key[0])
-
-            input_name = _actName(input)
-
-            if _isForeground(input.key[0]):
-                input_name += "{user-db}"
-
-            data[ex_name] = dict(input=input_name, amount=amount)
-
-        # Provide impact calculation if impact provided
-        all_acts = list(set(inputs_by_ex_name.values()))
-        res = multiLCAAlgebric(all_acts, [impact], **params)
-        impacts = res[res.columns.tolist()[0]].to_list()
-
-        impact_by_act = {act: value for act, value in zip(all_acts, impacts)}
-
-        # Add impacts to data
-        for key, vals in data.items():
-            amount = vals["amount"]
-            act = inputs_by_ex_name[key]
-            impact = impact_by_act[act]
-
-            if withImpactPerUnit:
-                vals["impact_per_unit"] = impact
-            vals["impact"] = amount * impact
-
-        # To dataframe
-        df = pd.DataFrame(data)
-
-        tables.append(df.T)
-        names.append(_actDesc(main_act))
-
-    full = pd.concat(tables, axis=1, keys=names, sort=True)
-
-    # Highlight differences in case two activites are provided
-    if len(activities) == 2:
-        YELLOW = "background-color:NavajoWhite"
-        diff_cols = ["amount", "input", "impact"]
-        cols1 = dict()
-        cols2 = dict()
-        for col_name in diff_cols:
-            cols1[col_name] = full.columns.get_loc((names[0], col_name))
-            cols2[col_name] = full.columns.get_loc((names[1], col_name))
-
-        if diffOnly:
-
-            def isDiff(row):
-                return row[cols1["impact"]] != row[cols2["impact"]]
-
-            full = full.loc[isDiff]
-
-        def same_amount(row):
-            res = [""] * len(row)
-            for col_name in diff_cols:
-                if row[cols1[col_name]] != row[cols2[col_name]]:
-                    res[cols1[col_name]] = YELLOW
-                    res[cols2[col_name]] = YELLOW
-            return res
-
-        full = full.style.apply(same_amount, axis=1)
-
-    return full
```

### Comparing `lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/params.py` & `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/params.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,75 +2,40 @@
 from collections import defaultdict
 from enum import Enum
 from typing import Any, Dict, List, Union
 
 import brightway2 as bw
 import numpy as np
 import pandas as pd
-from bw2data.backends import LCIBackend
 from bw2data.backends.peewee import ExchangeDataset
 from bw2data.parameters import (
     ActivityParameter,
     DatabaseParameter,
     Group,
     ProjectParameter,
 )
-from bw2data.proxies import ActivityProxyBase
 from IPython.core.display import HTML
+from pint import Quantity
 from scipy.stats import beta, lognorm, norm, triang, truncnorm
 from sympy import Basic, Expr, Symbol, lambdify, parse_expr
 from tabulate import tabulate
 
-from lca_algebraic.base_utils import ExceptionContext
+from lca_algebraic.base_utils import ExceptionContext, ValueOrExpression
 from lca_algebraic.log import logger
 
-from .base_utils import LANG, _snake2camel, as_np_array, error
+from .base_utils import _snake2camel, _user_functions, as_np_array
+from .database import DbContext
+from .log import warn
+from .settings import Settings
+from .units import unit_registry as u
 
 DEFAULT_PARAM_GROUP = "acv"
 UNCERTAINTY_TYPE = "uncertainty type"
 
 
-class DbContext:
-    """
-    Context class specifying the current foreground DB in use. in internal
-    Used internally to distinguish database parameters with same names
-
-    usage :
-    with DbContext("db") :
-        <some code>
-
-    """
-
-    stack = []
-
-    @staticmethod
-    def current_db():
-        if len(DbContext.stack) == 0:
-            return None
-        return DbContext.stack[-1]
-
-    def __init__(self, db: Union[str, ActivityProxyBase, LCIBackend]):
-        if db is None:
-            self.db = None
-        elif isinstance(db, ActivityProxyBase):
-            self.db = db.key[0]
-        elif isinstance(db, str):
-            self.db = db
-        else:
-            self.db = db.name
-
-    def __enter__(self):
-        if self.db is not None:
-            DbContext.stack.append(self.db)
-
-    def __exit__(self, exc_type, exc_value, exc_traceback):
-        if self.db is not None:
-            DbContext.stack.pop()
-
-
 class ParamType:
     """Type of parameters"""
 
     ENUM = "enum"
     """ Enum Parameter """
 
     BOOL = "bool"
@@ -145,19 +110,21 @@
     """ Use the median of the distribution of the parameter """
 
     MEAN = "mean"
     """ Use the mean of the distribution of the parameter """
 
 
 class ParamDef(Symbol):
-    """Generic definition of a parameter, with name, bound, type, distribution
+    """
+    Generic definition of a parameter, with name, bound, type, distribution
     This definition will serve both to generate brightway2 parameters and to evaluate.
-
     This class inherits sympy Symbol, making it possible to use in standard arithmetic python
     while keeping it as a symbolic expression (delayed evaluation).
+
+    Don't instantiate it directly. Use the function **newXXXParam() instead.
     """
 
     def __new__(cls, name, *karg, **kargs):
         # We use dbname as an "assumption" so that two symbols with same name are not equal if from separate DBs
         assumptions = dict()
         assumptions["real"] = True
 
@@ -172,30 +139,28 @@
         type: str,
         default,
         min=None,
         max=None,
         unit="",
         description="",
         label=None,
-        label_fr=None,
         group=None,
         distrib: DistributionType = None,
         dbname=None,
         formula=None,
         **kwargs,
     ):
         self.name = name
         self.type = type
         self.default = default
         self.description = description
         self.min = min
         self.max = max
         self.unit = unit
         self.label = label
-        self.label_fr = label_fr
         self.group = group
         self.distrib = distrib
         self.dbname = dbname
         self.formula = formula
 
         # if (self.dbname == None) :
         #    error("Warning : param '%s' linked to root project instead of a specific DB" % self.name)
@@ -212,28 +177,29 @@
 
         elif distrib in [DistributionType.NORMAL, DistributionType.LOGNORMAL]:
             if "std" not in kwargs:
                 raise Exception("Standard deviation is mandatory for normal / lognormal distribution")
             self.std = kwargs["std"]
 
             if distrib == DistributionType.LOGNORMAL and self.min is not None:
-                error(
+                warn(
                     "Warning : LogNormal does not support min/max boundaries for parameter : ",
                     self.name,
                 )
 
         elif distrib == DistributionType.BETA:
             if "a" not in kwargs or "b" not in kwargs or "std" not in kwargs:
                 raise Exception("Beta distribution requires params 'a' 'b' and 'std' (used as scale)")
             self.a = kwargs["a"]
             self.b = kwargs["b"]
             self.std = kwargs["std"]
 
     def stat_value(self, mode: FixedParamMode):
-        """Compute a fixed value for this parameter, according to the requested FixedParamMode"""
+        """Computes a fixed value for this parameter, either median or mean, according to the requested FixedParamMode and its
+        statistical distribution."""
         if mode == FixedParamMode.DEFAULT:
             return self.default
         else:
             # Compute statistical value for replacement
             rnd = np.random.rand(1000)
             x = self.rand(rnd)
 
@@ -241,29 +207,34 @@
                 return np.mean(x)
             elif mode == FixedParamMode.MEDIAN:
                 return np.median(x)
             else:
                 raise Exception("Unkown mode " + mode)
 
     def get_label(self):
-        if LANG == "fr " and self.label_fr is not None:
-            return self.label_fr
-        elif self.label is not None:
+        if self.label is not None:
             return self.label
         else:
             return self.name.replace("_", " ")
 
     def range(self, n):
         """Return N uniform values of this parameter, within its range of definition"""
         step = (self.max - self.min) / (n - 1)
         return list(i * step + self.min for i in range(0, n))
 
     def rand(self, alpha):
         """Transforms a random number between 0 and 1 to valid value according
-        to the distribution of probability of the parameter"""
+        to the distribution of probability of the parameter
+
+        Parameters
+        ----------
+
+        alpha:
+            Can be a *float* or numpy array of floats, between 0 and 1.
+        """
 
         if self.distrib == DistributionType.FIXED:
             return self.default
 
         elif self.distrib == DistributionType.LINEAR:
             if self.min is None or self.max is None:
                 raise Exception("Missing min/max for : " + self.name)
@@ -305,48 +276,53 @@
 
     def __eq__(self, other):
         if isinstance(other, ParamDef):
             return self.name == other.name and getattr(self, "dbname", None) == getattr(other, "dbname", None)
         else:
             return Symbol.__eq__(self, other)
 
-    # Expand parameter (useful for enum param)
     def expandParams(self, value=None) -> Dict[str, float]:
+        """Abstract function to represent a parameter as a dict : useful to be consistent with Enum params"""
         if value is None:
             value = self.default
         return {self.name: value}
 
-    # Useful for enum param, having several names
     def names(self, use_label=False):
+        """Generic method usefull to be consistent with Enum parameters"""
         if use_label:
             return [self.get_label()]
         else:
             return [self.name]
 
+    def with_unit(self):
+        """Returns the symbol together with its unit, as a Pint Quantity"""
+        return u.Quantity(self, self.unit)
+
     def __repr__(self):
         return self.name
 
 
 class BooleanDef(ParamDef):
-    """Parameter with discrete value 0 or 1"""
+    """Parameter with discrete value 0 or 1. Use **newBoolParam()** to instantiate it."""
 
     def __init__(self, name, **argv):
         if "min" not in argv:
             argv = dict(argv, min=None, max=None)
         super(BooleanDef, self).__init__(name, ParamType.BOOL, **argv)
 
     def range(self, n):
         return [0, 1]
 
     def rand(self, alpha):
         return np.around(alpha)
 
 
 class EnumParam(ParamDef):
-    """Enum param is a facility wrapping a choice / switch as many boolean parameters.
+    """
+    Enum param is a facility wrapping a choice / switch as many boolean parameters.
     It is not itself a Sympy symbol. use #symbol("value") to access it.
     Statistics weight can be attached to values by providing a dict.
     """
 
     def __init__(self, name, values: Union[List[str], Dict[str, float]], **argv):
         if "min" not in argv:
             argv = dict(argv, min=None, max=None)
@@ -383,21 +359,21 @@
             var_name = "%s_%s" % (
                 self.name,
                 enum_val if enum_val is not None else "default",
             )
             res[var_name] = 1.0 if enum_val == currValue else 0.0
         return res
 
-    def symbol(self, enumValue):
-        """Return the invididual symbol for a given enum value : <paramName>_<paramValue>"""
-        if enumValue is None:
+    def symbol(self, choice):
+        """Returns the invididual Sympy symbol for a given choice : <paramName>_<choice>"""
+        if choice is None:
             return Symbol(self.name + "_default")
-        if enumValue not in self.values:
-            raise Exception("enumValue should be one of %s. Was %s" % (str(self.values), enumValue))
-        return Symbol(self.name + "_" + enumValue)
+        if choice not in self.values:
+            raise Exception("enumValue should be one of %s. Was %s" % (str(self.values), choice))
+        return Symbol(self.name + "_" + choice)
 
     def names(self, use_label=False):
         if use_label:
             base_name = self.get_label()
         else:
             base_name = self.name
         return ["%s_%s" % (base_name, value) for value in (self.values + ["default"])]
@@ -432,20 +408,22 @@
 
 def newParamDef(name, type, dbname=None, save=True, **kwargs):
     """
     Creates a parameter and register it into a global registry and as a brightway parameter.
 
     Parameters
     ----------
-
-    type : Type of the parameter (From ParamType)
-    save : Boolean, persist this into Brightway2 project (True by default)
-    dbname : Optional name of db. If None, the parameter is a project parameter
-    other arguments : Refer to the documentation of BooleanDef ParamDef and EnumParam
-
+    type :
+        Type of the parameter (From ParamType)
+    save :
+        Boolean, persist this into Brightway2 project (True by default)
+    dbname :
+        Optional name of db. If None, the parameter is a project parameter
+    other arguments :
+        Refer to the documentation of BooleanDef ParamDef and EnumParam
     """
     if type == ParamType.ENUM:
         param = EnumParam(name, dbname=dbname, **kwargs)
     elif type == ParamType.BOOL:
         param = BooleanDef(name, dbname=dbname, **kwargs)
     else:
         param = ParamDef(name, dbname=dbname, type=type, **kwargs)
@@ -463,18 +441,24 @@
     UNCERTAINTY_TYPE: _UncertaintyType.DISCRETE,
     "minimum": 0,
     "maximum": 2,  # upper bound + 1
 }
 
 
 def persistParams():
-    """Persist parameters into Brightway project, as per :
-    https://stats-arrays.readthedocs.io/en/latest/
     """
+    Persist parameters into Brightway project, as per : https://stats-arrays.readthedocs.io/en/latest/.
 
+    This is important only in case you want t o:
+    - Use parameters outside lca_algebraic (Activity Browser for instance)
+    - Use *loadParams()* to init your parameters instead of deleting them and creating them programmaically each time.
+
+    This function is automatically run when creating new parameters. However, it should be called manually after **updating**
+    manually some properties of a parameter.
+    """
     for param in _param_registry().all():
         _persistParam(param)
 
 
 def _persistParam(param):
     """Persist parameter into Brightway project"""
     out = []
@@ -521,15 +505,15 @@
 
             elif param.distrib == DistributionType.BETA:
                 bwParam["scale"] = param.std
                 bwParam["loc"] = param.a
                 bwParam["shape"] = param.b
 
         else:
-            error("Param type not supported", param.type)
+            warn("Param type not supported", param.type)
 
         out.append(bwParam)
 
     if param.dbname:
         bw.parameters.new_database_parameters(out, param.dbname)
     else:
         bw.parameters.new_project_parameters(out)
@@ -550,29 +534,39 @@
     }
 
 
 def loadParams(global_variable=True, dbname=None):
     """
     Load parameters from Brightway database, as per : https://stats-arrays.readthedocs.io/en/latest/
 
+    The recommended way is to delete parameters at the start of your session and to define them programmically each time.
+
+    However, it can be useful if your parameters come from an import or where defined in **Activity Browser**.
+
     Parameters
     ----------
-    global_variable If true, loaded parameters are made available as global variable.
-    dbname : None. By default load all project and database parameters. If provided, only load DB params
+    global_variable:
+        If true, loaded parameters are made available as global variable.
+    dbname:
+        If provided, load only database parameters for the given db
+
+    Returns
+    -------
+    A dictionary of parameters
     """
 
     enumParams = defaultdict(lambda: dict())
 
     def register(param):
         _param_registry()[param.name] = param
 
         # Make it available as global var
         if global_variable:
             if param.name in builtins.__dict__:
-                error("Variable '%s' was already defined : overidding it with param." % param.name)
+                warn("Variable '%s' was already defined : overidding it with param." % param.name)
             builtins.__dict__[param.name] = param
 
     select = DatabaseParameter.select()
     if dbname:
         select = select.where(DatabaseParameter.database == dbname)
 
     params = list(select)
@@ -602,23 +596,23 @@
                 enumParams[enum_name][enum_value] = data
                 continue
 
             elif data["maximum"] == 2:
                 del args["max"], args["min"]
                 param = newBoolParam(name, save=False, **args)
             else:
-                error(
+                warn(
                     "Non boolean discrete values (max != 2) are not supported for param :",
                     name,
                 )
                 continue
         else:
             # Float parameter
             if type is None or type == _UncertaintyType.UNDEFINED:
-                error("'Uncertainty type' of param %s not provided. Assuming UNIFORM")
+                warn("'Uncertainty type' of param %s not provided. Assuming UNIFORM")
                 type = _UncertaintyType.UNIFORM
 
             # Uncertainty type to distribution type
             args["distrib"] = _DistributionTypeMapReverse[type]
 
             if type == _UncertaintyType.TRIANGLE:
                 args["default"] = data["loc"]
@@ -649,41 +643,213 @@
 
         # Default enum value is the one with amount=1
         defaults = list(key for key, data in param_values.items() if data.get("amount") == 1)
         if len(defaults) == 1:
             default = defaults[0]
         else:
             default = None
-            error("No default enum value found for ", param_name, defaults)
+            warn("No default enum value found for ", param_name, defaults)
 
-        param = newEnumParam(param_name, default, save=False, **args)
+        param = newEnumParam(name=param_name, default=default, save=False, **args)
 
         # Save it in shared dict
         register(param)
 
     # Parse formulas
     for param in _param_registry().all():
         with DbContext(param.dbname):
             if isinstance(param.formula, str):
                 param.formula = _parse_formula(param.formula)
 
+    return _param_registry()
+
+
+def newFloatParam(
+    name,
+    default,
+    min: float = None,
+    max: float = None,
+    unit: str = None,
+    description: str = None,
+    label: str = None,
+    group: str = None,
+    distrib: DistributionType = DistributionType.LINEAR,
+    formula=None,
+    save=True,
+    **kwargs,
+) -> Union[ParamDef, Quantity]:
+    """
+    Creates a float (decimal) parameter.
+
+    Parameters
+    ----------
+    name:
+        Name of the parameter
+    default:
+        Default value
+    min:
+        Minimum value
+    max:
+        Maximum value
+    unit:
+        Unit of the parameter
+    description:
+        Long description (optional)
+    label:
+        Extended name (optional)
+    group:
+        Name of the group (optional). Used to organize parameters.
+    distrib:
+        Type of the distribution (optional) Linear (uniform) by default
+    formula:
+        Sympy expression. Optional. If provided the default value of this parameter (if not provided at runtime) will be computed
+        from other parameter values.
+    kwargs:
+        Extra parameters required for advanced distribution types.
+
+
+    Examples
+    --------
+
+    The following code defines a float parameter *p1* of unit *kg*, with a triangle distribution.
+
+    >>> p1 = newFloatParam("p1", min=1.0, max=3.0, default=2.0, distrib=DistributionType.TRIANGLE, unit="kg")
+
+    Returns
+    -------
+    The newly created parameter
+
+    """
+
+    if Settings.units_enabled and unit is None:
+        raise Exception("Unit mode activated : unit is mandatory for parameters")
+
+    param = newParamDef(
+        name=name,
+        type=ParamType.FLOAT,
+        default=default,
+        min=min,
+        max=max,
+        unit=unit,
+        description=description,
+        label=label,
+        group=group,
+        distrib=distrib,
+        formula=formula,
+        save=save,
+        **kwargs,
+    )
+
+    # If units are enables, wrap float params with their unit
+    if Settings.units_enabled:
+        return param.with_unit()
+    else:
+        return param
+
+
+def newBoolParam(name, default, description: str = None, label: str = None, group: str = None, formula=None, save=True, **kwargs):
+    """
+    Creates a boolean parameter.
+
+    Parameters
+    ----------
+    name:
+        Name of the parameter
+    default:
+        Default value
+    description:
+        Long description (optional)
+    label:
+        Extended name (optional)
+    group:
+        Name of the group (optional). Used to organize parameters.
+    formula:
+        Sympy expression. Optional. If provided the default value of this parameter (if not provided at runtime) will be computed
+        from other parameter values.
+
 
-def newFloatParam(name, default, dbname=None, **kwargs):
-    """Create a FLOAT parameter. See the documentation of arguments for #newParamDef()."""
-    return newParamDef(name, ParamType.FLOAT, dbname=dbname, default=default, **kwargs)
+    Examples
+    --------
 
+    >>> p1 = newBoolParam("p1", default=0, group="param group")
 
-def newBoolParam(name, default, dbname=None, **kwargs):
-    """Create a BOOL parameter. See the documentation of arguments for #newParamDef()."""
-    return newParamDef(name, ParamType.BOOL, dbname=dbname, default=default, **kwargs)
+    Returns
+    -------
+    The newly created parameter
+
+    """
+    return newParamDef(
+        name,
+        ParamType.BOOL,
+        default=default,
+        description=description,
+        label=label,
+        group=group,
+        formula=formula,
+        save=save,
+        **kwargs,
+    )
+
+
+def newEnumParam(
+    name: str,
+    default: str,
+    values: Union[List[str], Dict[str, float]],
+    description: str = None,
+    label: str = None,
+    group: str = None,
+    save=True,
+    **kwargs,
+):
+    """
+    Creates an enum parameter : a set of mutually exclusive boolean choices.
+    Enum parameters themselves are *not* Sympy symbols. Each of the choice is represented internally
+    as a boolean sympy symbol, that can be accessed via **param.symbol("choice_name")**
+
+    Parameters
+    ----------
+
+    name:
+        Name of the parameter
+    default:
+        Default
+    values:
+        Possible choices. The values can be provided as a list of strings, in which case every choice is equiprobable.
+        They can also be provided as a python dictionnary of "choice" => value. The proability to be picked is then the
+        pro-rata of the value.
+    description:
+        Long description (optional)
+    label:
+        Extended name (optional)
+    group:
+        Name of the group (optional). Used to organize parameters.
+
+    Examples
+    --------
 
+    *p1* is an enum param with equiprobable choices "choice_a", "choice_b" and "choice_c"
 
-def newEnumParam(name, default, values: Union[List[str], Dict[str, float]], dbname=None, **kwargs):
-    """Create a ENUM parameter. See the documentation of arguments for #newParamDef()."""
-    return newParamDef(name, ParamType.ENUM, dbname=dbname, default=default, values=values, **kwargs)
+    >>> p1 = newEnumParam("p1", default="choice_a", values=["choice_a", "choice_b", "choice_c"])
+
+    *p2* is an anum param with "choice_a" and "choice_b" of probability 25% and "choice_c" of probability 50%.
+
+    >>> p2 = newEnumParam("p2", default="choice_a", values={"choice_a":1, "choice_b":1, "choice_c":2})
+
+    """
+    return newParamDef(
+        name,
+        ParamType.ENUM,
+        default=default,
+        values=values,
+        description=description,
+        label=label,
+        group=group,
+        save=save,
+        **kwargs,
+    )
 
 
 def _variable_params(param_names=None):
     if param_names is None:
         param_names = _param_registry().keys()
     params = {key: _param_registry()[key] for key in param_names}
     return {key: param for key, param in params.items() if param.distrib != DistributionType.FIXED}
@@ -742,17 +908,15 @@
             raise Exception(f"Parameter {key} not found :. Valid parameters : {self.keys()}")
 
     def as_dict(self):
         return dict(self.items())
 
     def __setitem__(self, key, param: ParamDef):
         if param.dbname in self.params[key]:
-            error(
-                "[ParamRegistry] Param %s was already defined in '%s' : overriding." % (param.name, param.dbname or "<project>")
-            )
+            warn("[ParamRegistry] Param %s was already defined in '%s' : overriding." % (param.name, param.dbname or "<project>"))
 
         self.params[key][param.dbname] = param
 
     def __contains__(self, key):
         return key in self.params
 
     def values(self):
@@ -789,15 +953,15 @@
     if "param_registry" not in builtins.__dict__:
         builtins.param_registry = ParamRegistry()
 
     return builtins.param_registry
 
 
 def all_params() -> Dict[str, ParamDef]:
-    """Return the dict of all parameters defined in ParamRegistry"""
+    """Return the dict of all parameters defined in memory"""
     return {param.name: param for param in _param_registry().all()}
 
 
 def _toSymbolDict(params: Dict[str, Any]):
     """Replace names with actual params as key when possible"""
     all_params = _param_registry().as_dict()
     return {all_params[name] if name in all_params else Symbol(name): val for name, val in params.items()}
@@ -876,16 +1040,23 @@
     if asSymbols:
         params = _toSymbolDict(params)
 
     return params
 
 
 def resetParams(db_name=None):
-    """Clear parameters in live memory (registry) and on disk.
-    Clear either all params (project and all db params) or db params from a single database (if db_name provided)"""
+    """
+    Clear parameters in live memory (registry) and on disk.
+    Clear either all params (project and all db params) or db params from a single database (if db_name provided).
+
+    This is a good practice in your code to start fresh, cleaning your foreground database and parameters and redefine all
+    programmatically at the start. This ensures the state of the projet / database is always in sync your code and your session
+    / in memory.
+
+    """
     _param_registry().clear(db_name)
 
     if db_name is None:
         ProjectParameter.delete().execute()
         ActivityParameter.delete().execute()
         DatabaseParameter.delete().execute()
     else:
@@ -906,15 +1077,21 @@
     elif name_type == NameType.LABEL:
         return param.get_label()
     else:
         return _snake2camel(param.name)
 
 
 def list_parameters(name_type=NameType.NAME, as_dataframe=False):
-    """Print a pretty list of all defined parameters"""
+    """Prints a pretty list of all defined parameters
+
+    Parameters
+    ----------
+    as_dataframe:
+        If true, a pandas *Dataframe* is returned. Otherwise, an HTML table is generated.
+    """
     params = [
         dict(
             group=param.group or "",
             name=_param_name(param, name_type),
             label=param.get_label(),
             default=param.default,
             min=param.min,
@@ -954,19 +1131,34 @@
     # Filter only required params
     values = {name: val for name, val in values.items() if name in free_symbols}
 
     return lambd(**values)
     # return expr.evalf(subs=_completeParamValues(param_values, required_params=required_params))
 
 
-def freezeParams(db_name, **params):
+def freezeParams(db_name, **params: Dict[str, float]):
     """
-    Freeze parameters values in all exchanges amounts of a DB.
+    Freezes amounts in all exchanges for a given set of parameter values.
     The formulas are computed and the 'amount' attributes are set with the result.
-    This enables parametric datasets to be used by standard, non parametric tools of Brightway2.
+
+    This enables parametric datasets to be used by standard, non-parametric tools of Brightway2 (like Activities browser).
+
+    Parameters
+    ----------
+    db_name :
+        Name of the database for freeze (your foreground db usually)
+
+    params:
+        All other parameters of this function are threated as the values of *lca_algebraic* parameters
+
+    Examples
+    --------
+
+    >>> freezeParams("USER_DB", p1=0.1, p2=3.0)
+
     """
 
     db = bw.Database(db_name)
 
     with DbContext(db):
         for act in db:
             for exc in act.exchanges():
@@ -1033,19 +1225,53 @@
     if len(missing) > 0:
         raise Exception("Unkown params : %s" % missing)
 
     return {param.name for param in res.values()}
 
 
 def _parse_formula(formula):
-    return parse_expr(formula, local_dict=_param_registry().as_dict())
+    local_dict = {x[0].name: x[0] for x in _user_functions.values()}
+    return parse_expr(formula, local_dict=local_dict | _param_registry().as_dict())
 
 
 def _getAmountOrFormula(ex: ExchangeDataset) -> Union[Basic, float]:
     """Return either a fixed float value or an expression for the amount of this exchange"""
     if "formula" in ex:
         try:
             return _parse_formula(ex["formula"])
         except Exception:
-            error("Error while parsing formula '%s' : backing to amount" % ex["formula"])
+            warn("Error while parsing formula '%s' : backing to amount" % ex["formula"])
 
     return ex["amount"]
+
+
+def switchValue(param: EnumParam, **values: Dict[str, ValueOrExpression]):
+    """
+
+    Helper method defining an expression that returns a different value / formula for each possible choice of an anum param.
+
+    Parameters
+    ----------
+    param: EnumParam
+        The enum param
+
+    values: Dict[str, ValueOrExpression]
+        Each param should correspond to a valid choice of the num parameter.
+
+
+    Examples
+    --------
+
+    Given the enum parameter *p1* :
+
+    >>> p1 = newEnumParam("p1", values=["choice1", "choice2", "choice3"])
+
+    The following code defines an expression worth 0.1 for *choice1*, 0.2 for *choice2*  and *4 x p2* for *choice3*
+
+    >>> amount = switchValue(p1, choice1=0.1, choice2=0.2, choice3=4*p2)
+
+    """
+
+    res = 0
+    for key, val in values.items():
+        res += param.symbol(key) * val
+    return res
```

### Comparing `lca_algebraic_dev-1.0.5.1681181.dev0/lca_algebraic/stats.py` & `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,62 @@
 import math
 import random
 import warnings
 from collections import defaultdict
 from time import time
-from typing import List, Tuple, Type
+from typing import Dict, List, Tuple, Type
 
 import numpy as np
 import seaborn as sns
+from bw2data.backends.peewee import Activity
 from IPython.display import display
 from ipywidgets import interact
 from matplotlib import pyplot as plt
 from matplotlib.lines import Line2D
 from SALib.analyze import sobol as analyse_sobol
 from SALib.sample import sobol, sobol_sequence
-from sympy import Abs, Add, AtomicExpr, Eq, Expr, Float, Mul, Number, Piecewise, Sum
+from sympy import (
+    Abs,
+    Add,
+    AtomicExpr,
+    Eq,
+    Expr,
+    Float,
+    Mul,
+    Number,
+    Piecewise,
+    Sum,
+    simplify,
+    symbols,
+)
 from sympy.core.operations import AssocOp
 
-from .base_utils import _display_tabs, _method_unit, displayWithExportButton, r_squared
+from .base_utils import (
+    ValueOrExpression,
+    _display_tabs,
+    displayWithExportButton,
+    r_squared,
+)
+from .database import DbContext, with_db_context
 from .lca import (
-    Activity,
-    DbContext,
-    Dict,
     LambdaWithParamNames,
     Symbol,
     _expanded_names_to_names,
     _filter_param_values,
     _modelToExpr,
     _postMultiLCAAlgebric,
     _preMultiLCAAlgebric,
     _replace_fixed_params,
     compute_impacts,
     concurrent,
-    error,
     lambdify,
-    method_name,
     pd,
-    simplify,
-    symbols,
-    with_db_context,
 )
+from .log import warn
+from .methods import method_name, method_unit
 from .params import (
     FixedParamMode,
     NameType,
     ParamDef,
     ParamType,
     _complete_and_expand_params,
     _param_name,
@@ -85,22 +99,37 @@
         required_param_names.update(_expanded_names_to_names(lamb.expanded_params))
     var_params = _variable_params(required_param_names)
     return sorted(var_params.values(), key=lambda p: (p.group if p.group else "", p.name))
 
 
 @with_db_context(arg="model")
 def oat_matrix(
-    model,
+    model: Activity,
     impacts,
-    functional_unit=1,
+    functional_unit: ValueOrExpression = 1,
     n=10,
     title="Impact variability (% of mean)",
     name_type=NameType.LABEL,
 ):
-    """Generates a heatmap of the incertitude of the model, varying input parameters one a a time."""
+    """
+
+    This function generates a heat map of relative the variance of impacts
+    for each parameter varying along its min/max values.
+
+    Parameters
+    ----------
+    model:
+        Root activity of the inventory
+
+    impacts:
+        Impact variabilityList of impact methods keys (tuples)
+
+    functional_unit:
+        Float value of expression by which to divide each impact.
+    """
 
     # Compile model into lambda functions for fast LCA
     lambdas = _preMultiLCAAlgebric(model, impacts, alpha=1 / functional_unit)
 
     # Sort params by category
     sorted_params = _extract_var_params(lambdas)
 
@@ -123,56 +152,41 @@
         change,
         index=[_param_name(param, name_type) for param in sorted_params],
         columns=[method_name(imp) for imp in impacts],
     )
     _heatmap(change.transpose(), title, 100, ints=True)
 
 
-def oat_dasboard(
-    modelOrLambdas,
+def _oat_dasboard(
+    model,
     impacts,
-    varying_param: ParamDef,
+    varying_param: ParamDef = None,
     n=10,
     all_param_names=None,
     figsize=(15, 15),
     figspace=(0.5, 0.5),
     sharex=True,
     cols=3,
-    func_unit="kWh",
+    func_unit_name="kWh",
 ):
-    """
-    Analyse the evolution of impacts for a single parameter. The other parameters are set to their default values.
-    The result heatmap shows percentage of variation relative to median value.
-
-    Parameters
-    ----------
-    model : activity, or lambdas as precomputed by preMultiLCAAlgebric, for faster computation
-    impacts : set of methods
-    param: parameter to analyse
-    n: number of samples of the parameter
-    figsize: Size of figure fro graphs : (15, 15 by default)
-    figspace: Space between figures for graphs : (0.5, 0.5) by default
-    sharex: Shared X axes ? True by default
-    """
-
     if all_param_names is None:
         all_param_names = _param_registry().keys()
 
     params = {name: _param_registry()[name].default for name in all_param_names}
 
     # Compute range of values for given param
     params[varying_param.name] = varying_param.range(n)
 
     # print("Params: ", params)
 
-    if isinstance(modelOrLambdas, Activity):
-        with DbContext(modelOrLambdas):
-            df = compute_impacts(modelOrLambdas, impacts, **params)
+    if isinstance(model, Activity):
+        with DbContext(model):
+            df = compute_impacts(model, impacts, **params)
     else:
-        df = _postMultiLCAAlgebric(impacts, modelOrLambdas, **params)
+        df = _postMultiLCAAlgebric(impacts, model, **params)
 
     # Add X values in the table
     pname = varying_param.name
     if varying_param.unit:
         pname = "%s [%s]" % (pname, varying_param.unit)
     df.insert(0, pname, varying_param.range(n))
     df = df.set_index(pname)
@@ -198,15 +212,15 @@
                 kind="line" if varying_param.type == ParamType.FLOAT else "bar",
             )
 
             axes = axes.flatten()
 
             for ax, impact in zip(axes, impacts):
                 ax.set_ylim(ymin=0)
-                unit = _method_unit(impact) + " / " + func_unit
+                unit = method_unit(impact) + " / " + func_unit_name
                 ax.set_ylabel(unit, fontsize=15)
                 ax.set_xlabel(pname, fontsize=15)
 
             plt.show(fig)
 
     def change():
         ch = (df.max() - df.min()) / df.median() * 100
@@ -217,29 +231,58 @@
         plt.tight_layout()
         plt.show(fig)
 
     _display_tabs({"Graphs": graph, "Data": table, "Variation": change})
 
 
 @with_db_context(arg="model")
-def oat_dashboard_interact(model, methods, functional_unit=1, **kwparams):
-    """Interactive dashboard, with a dropdown for selecting parameter
+def oat_dashboard(model, impacts, functional_unit: ValueOrExpression = 1, func_unit_name="kWh", **kwparams):
+    """
+    This function runs a "one at a time" analysis on the selected param.
+
+    It makes each parameter vary on its min:max range, while keeping other parameters at their default values.
+
+    It returns an interactive dashboard.
 
     Parameters
     ----------
-    figsize: Size of figure fro graphs : (15, 15 by default)
-    figspace: Space between figures for graphs : (0.5, 0.5) by default
-    sharex: Shared X axes ? True by default
+
+    model :
+        Root activity of the inventory
+
+    methods :
+        List of methods keys (tuple)
+
+    functional_unit:
+        Value of sympy expression by which to divide the impacts
+
+    func_unit_name:
+        Name of the physical unit of the functional unit, for display
+
+    figsize:
+        Size of figure fro graphs : (15, 15 by default)
+    figspace:
+        Space between figures for graphs : (0.5, 0.5) by default
+    sharex:
+        Shared X axes ? True by default
+
+    Returns
+    -------
+
+    An interactive dashboard with selection of a parameter and graphs of impacts.
+
     """
 
-    lambdas = _preMultiLCAAlgebric(model, methods, alpha=1 / functional_unit)
+    lambdas = _preMultiLCAAlgebric(model, impacts, alpha=1 / functional_unit)
 
     def process_func(param):
         with DbContext(model):
-            oat_dasboard(lambdas, methods, _param_registry()[param], **kwparams)
+            _oat_dasboard(
+                model=lambdas, impacts=impacts, varying_param=_param_registry()[param], func_unit_name=func_unit_name, **kwparams
+            )
 
     param_list = _expanded_names_to_names(lambdas[0].expanded_params)
     param_list = list(_variable_params(param_list).keys())
 
     interact(process_func, param=param_list)
 
 
@@ -355,15 +398,15 @@
             s2_conf_ = np.nan_to_num(res["S2_conf"])
             s2[:, :, imethod] = s2_ + np.transpose(s2_)
             s2_conf[:, :, imethod] = s2_conf_ + np.transpose(s2_conf_)
             st[:, imethod] = res["ST"]
             st_conf[:, imethod] = res["ST_conf"]
 
         except Exception as e:
-            error("Sobol failed on %s" % imethod[2], e)
+            warn("Sobol failed on %s" % imethod[2], e)
 
     return SobolResults(s1, s2, st, s1_conf, s2_conf, st_conf)
 
 
 def _incer_stochastic_matrix(methods, param_names, Y, sob, name_type=NameType.LABEL):
     """Internal method computing matrix of parameter importance"""
 
@@ -448,15 +491,15 @@
         median = np.median(data)
         std = np.std(data)
         mean = np.mean(data)
 
         ax.violinplot(data, showmedians=True)
         ax.title.set_text(method_name(method))
         ax.set_ylim(ymin=0)
-        ax.set_ylabel(_method_unit(method))
+        ax.set_ylabel(method_unit(method))
         ax.set_xticklabels([])
 
         # Add text
         textstr = "\n".join(
             (
                 r"$\mu=%.3g$" % (mean,),
                 r"$\mathrm{median}=%.3g$" % (median,),
@@ -558,24 +601,54 @@
     )
 
     df = pd.DataFrame(data, index=rows, columns=[method_name(method) for method in methods])
     displayWithExportButton(df)
 
 
 @with_db_context(arg="model")
-def incer_stochastic_dashboard(model, methods, n=DEFAULT_N, var_params=None, functional_unit=1, **kwparams):
-    """Generates a dashboard with several statistics : matrix of parameter incertitude, violin diagrams, ...
+def incer_stochastic_dashboard(
+    model: Activity, methods, n=DEFAULT_N, var_params=None, functional_unit=ValueOrExpression, **kwparams
+):
+    """
+    This function runs a monte carlo & Sobol analysis (GSA) on a parametric model and displays a dashboard with results.
 
-    parameters
+    Parameters
     ----------
-    var_params: Optional list of parameters to vary.
-    By default use all the parameters with distribution not FIXED
-    figsize: Size of figure for violin plots : (15, 15) by default
-    figspace: Space between violin graphs (0.5, 0.5) by default
-    sharex: Share X axe for violin graph : True by default
+    model:
+        The root activity of your inventory
+
+    methods:
+        List of impact methods keys (tuples)
+
+    var_params:
+        Optional list of parameters to vary.
+        By default, all the parameters that are not marked as *FIXED* will be varyed.
+
+    functional_unit:
+        Float value or Sympy expression by which to divide the impacts
+
+    figsize:
+        Size of figure for violin plots : (15, 15) by default
+
+    figspace:
+        Space between violin graphs (0.5, 0.5) by default
+
+    sharex:
+        Share X axe for violin graph : True by default
+
+
+    Returns
+    -------
+    An interactive dashboard with 4 tabs :
+
+    * Violin graphs with distributions of impacts
+    * Bar graph with relative variance of impacts
+    * A heatmap amtrix of Sobol indices for each paramter x impact method
+    * A detailed table with all values
+
     """
 
     problem, _, Y = _stochastics(model, methods, n, var_params=var_params, functional_unit=functional_unit)
 
     param_names = problem["names"]
 
     print("Processing Sobol indices ...")
@@ -723,41 +796,79 @@
     res = exp.replace(lambda x: isinstance(x, Abs), lambda x: replaceAbs(x))
 
     return res, nb_match
 
 
 @with_db_context(arg="model")
 def sobol_simplify_model(
-    model,
+    model: Activity,
     methods,
     min_ratio=0.8,
+    functional_unit=1,
     n=DEFAULT_N * 2,
     var_params=None,
     fixed_mode=FixedParamMode.MEDIAN,
     num_digits=3,
     simple_sums=True,
-    functional_unit=1,
     simple_products=True,
 ) -> List[LambdaWithParamNames]:
     """
     Computes Sobol indices and selects main parameters for explaining sensibility of at least 'min_ratio',
     Then generates simplified models for those parameters.
 
-    parameters
+    The other parameters are replaced by their mean or median values.
+
+    Also the term contributing to less than 1% of variation in sums and products are removed.
+
+    Decimal numbers are rounded to 3 digits.
+
+    Parameters
     ----------
-    min_ratio: [0, 1] minimum amount of first order variation (sum of S1) to explain
-    var_params: Optional list of parameters to vary.
-    fixed_mode : What to replace minor parameters with : MEDIAN by default
-    simple_sums: If true (default) remove terms in sums that are lower than 1%
+    model:
+        Root activity of the inventory
 
-    returns
-    _______
+    methods:
+        List of impact methods to consider
 
-    List of LambdaWithParamNames, one per impact : with wraps the simplified expression together with the
-    list of required parameters and a fast complied lambda function for fast evaluation.
+    min_ratio:
+        [0, 1] minimum amount of first order variation (sum of S1) to explain; 0.8 (80%) by default.
+
+    var_params:
+        Optional list of parameters to vary. If not provided, all parameters vary.
+
+    fixed_mode :
+        What to replace minor parameters with : MEDIAN by default
+
+    simple_sums:
+        If true (default) remove terms in sums that are lower than 1%
+
+    simple_products:
+        If true (default) remove terms in products that contribute to less than 1% to variation
+
+    num_digits:
+        Number of decimal places to round decimal number to (default 3)
+
+    Returns
+    -------
+    List of *LambdaWithParamNames*, one per impact.
+    The class *LambdaWithParamNames* wraps the simplified expression together with the
+    list of required parameters and compiled lambda functions for fast evaluation.
+
+    The core simplified expresion may be access with **res[i].expr**
+
+
+    Examples
+    --------
+
+    >>> res = sobol_simplify_model(
+    >>>     model=total_inventory,
+    >>>     methods=[climate_change],
+    >>>     functional_unit=total_energy) # Holds a sympy expression computing the total energy
+
+    >>> print(res[0].expr) # Dispalt the simplified expression
     """
 
     # Default var param names
     if var_params is None:
         var_params = _variable_params().values()
 
     var_param_names = list([param.name for param in var_params])
@@ -1015,66 +1126,65 @@
     ax.set_xlabel(unit, dict(fontsize=14))
     ax.set_yticks([])
     ax.set_title(title, dict(fontsize=16))
 
     return dict(median=median, std=std, p=pvals, mean=mean, var=variability)
 
 
-def distrib(*args, **kwargs):
-    """
-    Show distributions together with statistical outcomes
-
-    Synonym of #graphs()
-
-    parameters
-    ----------
-    model: normalized model
-    methods: List of impacts
-    Y: output of processing. If None, monte carlo will be processed again
-    nb_cols : number of colons to display graphs on
-    invert : list of methods for which result should be inverted (1/X). None by default
-    scales : Dict of method => scale, for multiplying results. To be used with unit overrides
-    unit_overrides : Dict of method => string for overriding unit, in respect to custom scales
-    height: Height of graph : 10 inches be default
-    width : Width of graphs : 15 inches by default
-    """
-    return graphs(*args, **kwargs)
-
-
-@with_db_context(arg="model")
-def graphs(
+def distrib(
     model,
     methods,
     functional_unit=1,
+    func_unit_name="",
     Y=None,
     nb_cols=1,
     axes=None,
     title=None,
     invert=None,
     scales=None,  # Dict of method => scale
     unit_overrides=None,
     height=10,
     width=15,
-    func_unit="kWh",
     **kwargs,
 ):
     """
     Show distributions together with statistical outcomes
 
+    Synonym of #graphs()
+
     parameters
     ----------
-    model: normalized model
-    methods: List of impacts
-    Y: output of processing. If None, monte carlo will be processed again
-    nb_cols : number of colons to display graphs on
-    invert : list of methods for which result should be inverted (1/X). None by default
-    scales : Dict of method => scale, for multiplying results. To be used with unit overrides
-    unit_overrides : Dict of method => string for overriding unit, in respect to custom scales
-    height: Height of graph : 10 inches be default
-    width : Width of graphs : 15 inches by default
+    model:
+        Root activity of the onventory
+
+    methods:
+        List of impact methods keys (tuples)
+
+    functional_unit:
+        Value of expression by which to divide the impacts
+
+    func_unit_name:
+        Physical unit name of the fonctional unit
+
+    nb_cols :
+        number of colons to display graphs on
+
+    invert :
+        list of methods for which result should be inverted (1/X). None by default
+
+    scales :
+        Dict of method => scale, for multiplying results. To be used with unit overrides
+
+    unit_overrides :
+        Dict of method => string for overriding unit, in respect to custom scales
+
+    height:
+        Height of graph : 10 inches be default
+    width :
+        Width of graphs : 15 inches by default
     """
 
     if Y is None:
         _, _, Y = _stochastics(model, methods, n=DEFAULT_N * 16, functional_unit=functional_unit)
 
     if axes is None:
         nb_rows = math.ceil(len(methods) / nb_cols)
@@ -1098,57 +1208,77 @@
             data = data * scales[method]
 
         graph_title = title if title else method_name(method)
 
         if unit_overrides and method in unit_overrides:
             unit = unit_overrides[method]
         else:
-            unit = _method_unit(method)
+            unit = method_unit(method)
 
-        unit += " / " + func_unit
+        unit += " / " + func_unit_name
 
         stats = _graph(data, unit, graph_title, ax=ax, **kwargs)
 
         res[graph_title + (" [%s]" % unit)] = stats
 
     for i in range(0, -len(methods) % nb_cols):
         ax = axes.flatten()[-(i + 1)]
         ax.axis("off")
 
     return pd.DataFrame(res)
 
 
 @with_db_context(arg="model")
 def compare_simplified(
-    model,
+    model: Activity,
     methods,
     simpl_lambdas,
     functional_unit=1,
+    func_unit_name="",
     scales=None,  # Dict of method => scale
     unit_overrides=None,
     nb_cols=2,
     height=10,
     width=15,
     textboxright=0.6,
     r2_height=0.65,
-    func_unit="kWh",
     residuals=False,
     **kwargs,
 ):
     """
-    Compare distribution of simplified model with full model
+    Compare distribution of simplified model with full model.
+
+    This functions runs the same monte caarlo random sample as input and feed it to oboth simplified models and full
+    model. It displays graphs and metrics comparing the two.
 
     Parameters
     ----------
-    model: Model
-    residuals : If true, draw heat map of residuals, instead of distributions
-    methods : Impact methods
-    simpl_lambdas : Simplified lambdas, as returned by sobol_simplify_model(...)
-    nb_cols: number of columns for displaying graphs
-    percentiles: List of percentiles to compute [5, 95] by default
+    model:
+        Root activity of the inventory
+
+    methods :
+        List of impact methods
+
+    functional_unit:
+        Float value or sympy expression by whicxh to devide the impacts
+
+    func_unit_name:
+        Name of the physical functional unit
+
+    simpl_lambdas :
+        Simplified lambdas, as returned by **sobol_simplify_model(...)**
+
+    residuals :
+        If true, draw heat map of residuals, rather than distributions
+
+    nb_cols:
+        number of columns for displaying graphs
+
+    percentiles:
+        List of percentiles to compute [5, 95] by default
     """
 
     # Raw model
     lambdas = _preMultiLCAAlgebric(model, methods, alpha=1 / functional_unit)
 
     nb_rows = math.ceil(len(methods) / nb_cols)
     fig, axes = plt.subplots(nb_rows, nb_cols, figsize=(width, height * nb_rows))
@@ -1179,17 +1309,17 @@
         if scales and method in scales:
             d1 = d1 * scales[method]
             d2 = d2 * scales[method]
 
         if unit_overrides and method in unit_overrides:
             unit = unit_overrides[method]
         else:
-            unit = _method_unit(method)
+            unit = method_unit(method)
 
-        unit += " / " + func_unit
+        unit += " / " + func_unit_name
 
         if residuals:
             hb = ax.hexbin(d1, d2, gridsize=(200, 200), mincnt=1)
             cb = fig.colorbar(hb, ax=ax)
 
             xmin, xmax = ax.get_xlim()
             ymin, ymax = ax.get_ylim()
```

### Comparing `lca_algebraic_dev-1.0.5.1681181.dev0/setup.py` & `lca_algebraic_dev-1.1.1750653.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,9 +65,11 @@
         "seaborn",
         "sympy",
         "matplotlib",
         "deprecation",
         "brightway2",
         "pypardiso",
         "SALib",
+        "pint",
+        "typing-extensions",
     ],
 )
```

### Comparing `lca_algebraic_dev-1.0.5.1681181.dev0/test/test_axis_dict.py` & `lca_algebraic_dev-1.1.1750653.dev0/test/test_axis_dict.py`

 * *Files identical despite different names*

