# Comparing `tmp/aiidalab_widgets_base-2.2.0a0.tar.gz` & `tmp/aiidalab_widgets_base-2.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiidalab_widgets_base-2.2.0a0.tar", last modified: Fri Mar  1 15:54:23 2024, max compression
+gzip compressed data, was "aiidalab_widgets_base-2.2.0a1.tar", last modified: Wed Apr 10 20:18:52 2024, max compression
```

## Comparing `aiidalab_widgets_base-2.2.0a0.tar` & `aiidalab_widgets_base-2.2.0a1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:54:23.465280 aiidalab_widgets_base-2.2.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-03-01 15:54:23.465280 aiidalab_widgets_base-2.2.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:54:23.457280 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    70960 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/computational_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:54:23.461280 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15851 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11302 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/elns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13093 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    29519 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/process.py
--rw-r--r--   0 runner    (1001) docker     (127)    59992 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:54:23.461280 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    59232 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/viewers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:54:23.461280 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-03-01 15:54:23.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-01 15:54:23.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 15:54:23.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 15:54:23.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-01 15:54:23.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-01 15:54:23.000000 aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-01 15:54:23.465280 aiidalab_widgets_base-2.2.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:54:23.461280 aiidalab_widgets_base-2.2.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/tests/test_bug_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    30474 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/tests/test_computational_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/tests/test_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/tests/test_elns.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/tests/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/tests/test_viewers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-03-01 15:54:19.000000 aiidalab_widgets_base-2.2.0a0/tests/test_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:18:52.520245 aiidalab_widgets_base-2.2.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-10 20:18:52.520245 aiidalab_widgets_base-2.2.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:18:52.512245 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70960 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/computational_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:18:52.516245 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15852 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11302 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/elns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29520 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59993 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:18:52.516245 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59471 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:18:52.516245 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-10 20:18:52.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-10 20:18:52.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:18:52.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:18:52.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-10 20:18:52.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 20:18:52.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-10 20:18:52.520245 aiidalab_widgets_base-2.2.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:18:52.516245 aiidalab_widgets_base-2.2.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30474 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_computational_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_elns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_wizard.py
```

### Comparing `aiidalab_widgets_base-2.2.0a0/LICENSE.txt` & `aiidalab_widgets_base-2.2.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a0/PKG-INFO` & `aiidalab_widgets_base-2.2.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiidalab_widgets_base
-Version: 2.2.0a0
+Version: 2.2.0a1
 Summary: Reusable widgets for AiiDAlab applications.
 Home-page: https://github.com/aiidalab/aiidalab-widgets-base
 Author: The AiiDAlab team
 Author-email: aiidalab@materialscloud.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
```

### Comparing `aiidalab_widgets_base-2.2.0a0/README.md` & `aiidalab_widgets_base-2.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/__init__.py` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Reusable widgets for AiiDAlab applications."""
+
 from aiida.manage import get_profile
 
 _WARNING_TEMPLATE = """
 <div style="background-color: #f7f7f7; border: 2px solid #e0e0e0; padding: 20px; border-radius: 5px;">
     <p style="font-size: 16px; font-weight: bold; color: #ff5733;">Warning:</p>
     <p style="font-size: 14px;">The default profile '<span style="font-style: italic;">{profile}</span>' was loaded automatically. This behavior will be removed in the <span style="font-style: italic;">{version}</span>. Please load the profile manually before loading modules from aiidalab-widgets-base by adding the following code at the beginning cell of the notebook:</p>
     <pre style="background-color: #f0f0f0; padding: 10px; border: 1px solid #ccc; font-family: 'Courier New', monospace;">
@@ -112,8 +113,8 @@
     "SubmitButtonWidget",
     "WizardAppWidget",
     "WizardAppWidgetStep",
     "register_viewer_widget",
     "viewer",
 ]
 
-__version__ = "2.2.0a0"
+__version__ = "2.2.0a1"
```

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/bug_report.py` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/bug_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Provide more user friendly error messages and automated reporting.
 
 Authors:
 
     * Carl Simon Adorf <simon.adorf@epfl.ch>
 """
+
 from __future__ import annotations
 
 import base64
 import json
 import platform
 import re
 import sys
```

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/computational_resources.py` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/computational_resources.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/data/__init__.py` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""Useful functions that provide access to some data. """
+"""Useful functions that provide access to some data."""
+
 import ipywidgets as ipw
 import numpy as np
 from ase import Atom, Atoms
 
 # The first atom is anchoring, so the new bond will be connecting it
 # The direction of the new bond is (-1, -1, -1).
 FUNCTIONAL_GROUPS = {
```

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/databases.py` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/databases.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Widgets that allow to query online databases."""
+
 import re
 
 import ase
 import ipywidgets as ipw
 import requests
 import traitlets as tl
```

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/dicts.py` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/dicts.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/elns.py` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/elns.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,23 +143,23 @@
             except IndexError:
                 info = {}
 
         self.eln.set_sample_config(**info)
 
     def send_to_eln(self, _=None):
         if self.eln and self.eln.is_connected:
-            self.message.value = f"\u29D7 Sending data to {self.eln.eln_instance}..."
+            self.message.value = f"\u29d7 Sending data to {self.eln.eln_instance}..."
             with requests_cache.disabled():
                 # Since the cache is enabled in AiiDAlab, we disable it here to get correct results.
                 self.eln.export_data()
             self.message.value = (
                 f"\u2705 The data were successfully sent to {self.eln.eln_instance}."
             )
         else:
-            self.message.value = f"""\u274C Something isn't right! We were not able to send the data to the "<strong>{self.eln.eln_instance}</strong>" ELN instance. Please follow <a href="{self.path_to_root}/aiidalab-widgets-base/notebooks/eln_configure.ipynb" target="_blank">the link</a> to update the ELN's configuration."""
+            self.message.value = f"""\u274c Something isn't right! We were not able to send the data to the "<strong>{self.eln.eln_instance}</strong>" ELN instance. Please follow <a href="{self.path_to_root}/aiidalab-widgets-base/notebooks/eln_configure.ipynb" target="_blank">the link</a> to update the ELN's configuration."""
 
     def handle_output(self, _=None):
         with self._output:
             clear_output()
             if self.modify_settings.value:
                 display(
                     ipw.HTML(
@@ -269,15 +269,15 @@
 
     def check_connection(self, _=None):
         if self.eln:
             err_message = self.eln.connect()
             if self.eln.is_connected:
                 self.my_output.value = "\u2705 Connected."
                 return
-        self.my_output.value = f"\u274C Not connected. {err_message}"
+        self.my_output.value = f"\u274c Not connected. {err_message}"
 
     def display_eln_config(self, value=None):
         """Display ELN configuration specific to the selected type of ELN."""
         try:
             eln_class = get_eln_connector(self.eln_types.value)
         except NotImplementedError as err:
             with self._output:
```

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/export.py` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Widgets to manage AiiDA export."""
+
 import os
 
 import ipywidgets as ipw
 
 
 class ExportButtonWidget(ipw.Button):
     """Export Node button."""
```

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/misc.py` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Some useful classes used acrross the repository."""
+
 import io
 import tokenize
 
 import ipywidgets as ipw
 from traitlets import Unicode
```

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/nodes.py` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Widgets to work with AiiDA nodes."""
+
 import functools
 
 import ipytree
 import ipywidgets as ipw
 import traitlets as tl
 from aiida import common, engine, orm
 from aiida.cmdline.utils.ascii_vis import calc_info
```

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/process.py` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Widgets to work with processes."""
+
 # pylint: disable=no-self-use
 # Built-in imports
 from __future__ import annotations
 
 import inspect
 import os
 import threading
```

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/structures.py` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module to provide functionality to import structures."""
+
 import datetime
 import functools
 import io
 import pathlib
 import tempfile
 
 import ase
```

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/utils/__init__.py` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Some utility functions used acrross the repository."""
+
 import threading
 from enum import Enum
 from typing import Any
 
 import ipywidgets as ipw
 import more_itertools as mit
 import numpy as np
```

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/viewers.py` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/viewers.py`

 * *Files 1% similar despite different names*

```diff
@@ -668,22 +668,22 @@
             self.cell_b.value = "<i><b>b</b></i>: {:.4f} {:.4f} {:.4f}".format(
                 *self.cell.array[1]
             )
             self.cell_c.value = "<i><b>c</b></i>: {:.4f} {:.4f} {:.4f}".format(
                 *self.cell.array[2]
             )
 
-            self.cell_a_length.value = "|<i><b>a</b></i>|: {:.4f}".format(
-                self.cell.lengths()[0]
+            self.cell_a_length.value = (
+                f"|<i><b>a</b></i>|: {self.cell.lengths()[0]:.4f}"
             )
-            self.cell_b_length.value = "|<i><b>b</b></i>|: {:.4f}".format(
-                self.cell.lengths()[1]
+            self.cell_b_length.value = (
+                f"|<i><b>b</b></i>|: {self.cell.lengths()[1]:.4f}"
             )
-            self.cell_c_length.value = "|<i><b>c</b></i>|: {:.4f}".format(
-                self.cell.lengths()[2]
+            self.cell_c_length.value = (
+                f"|<i><b>c</b></i>|: {self.cell.lengths()[2]:.4f}"
             )
 
             self.cell_alpha.value = f"&alpha;: {self.cell.angles()[0]:.4f}"
             self.cell_beta.value = f"&beta;: {self.cell.angles()[1]:.4f}"
             self.cell_gamma.value = f"&gamma;: {self.cell.angles()[2]:.4f}"
 
             spglib_structure = ase2spglib(self.structure)
@@ -1517,28 +1517,33 @@
         if downloadable:
             self.download_btn = ipw.Button(description="Download")
             self.download_btn.on_click(self.download)
             children.append(self.download_btn)
         super().__init__(children, **kwargs)
 
     def change_file_view(self, _=None):
-        with self._folder.base.repository.open(self.files.value) as fobj:
-            self.text.value = fobj.read()
+        try:
+            with self._folder.base.repository.open(self.files.value) as fobj:
+                self.text.value = fobj.read()
+        except UnicodeDecodeError:
+            self.text.value = "[Binary file, preview not available]"
 
     def download(self, _=None):
-        """Prepare for downloading."""
+        """Download selected file."""
         from IPython.display import Javascript
 
-        payload = base64.b64encode(
-            self._folder.get_object_content(self.files.value).encode()
-        ).decode()
+        # TODO: Preparing large files for download might take a while.
+        # Can we do a streaming solution?
+        raw_bytes = self._folder.get_object_content(self.files.value, "rb")
+        base64_payload = base64.b64encode(raw_bytes).decode()
+
         javas = Javascript(
             f"""
             var link = document.createElement('a');
-            link.href = "data:;base64,{payload}"
+            link.href = "data:;base64,{base64_payload}"
             link.download = "{self.files.value}"
             document.body.appendChild(link);
             link.click();
             document.body.removeChild(link);
             """
         )
         display(javas)
```

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base/wizard.py` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """The wizard application allows the implication of a Wizard-like GUI.
 
 Authors:
 
     * Carl Simon Adorf <simon.adorf@epfl.ch>
 """
+
 import enum
 
 import ipywidgets as ipw
 import traitlets as tl
 
 
 class AtLeastTwoStepsWizardError(ValueError):
```

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base.egg-info/PKG-INFO` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiidalab_widgets_base
-Version: 2.2.0a0
+Version: 2.2.0a1
 Summary: Reusable widgets for AiiDAlab applications.
 Home-page: https://github.com/aiidalab/aiidalab-widgets-base
 Author: The AiiDAlab team
 Author-email: aiidalab@materialscloud.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
```

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base.egg-info/SOURCES.txt` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a0/aiidalab_widgets_base.egg-info/requires.txt` & `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a0/pyproject.toml` & `aiidalab_widgets_base-2.2.0a1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -13,21 +13,16 @@
     'ignore:crystal system:UserWarning:ase.io.cif',
     'ignore::DeprecationWarning:ase.atoms',
     # TODO: This comes from a transitive dependency of ipyoptimade
     # Remove this when this issue is addressed:
     # https://github.com/CasperWA/ipywidgets-extended/issues/85
     'ignore::DeprecationWarning:ipywidgets_extended',
     'ignore:metadata.*traitlets.traitlets.Unicode object:DeprecationWarning:traitlets',
-    # For some reason we get this error, perhaps because we do
-    # not unload the AiiDA profile? Let's ignore this for now.
-    # E pytest.PytestUnraisableExceptionWarning: Exception ignored in: <function Popen.__del__>
-    # E Traceback (most recent call last):
-    # E   File "/opt/conda/lib/python3.9/subprocess.py", line 1052, in __del__
-    # E     _warn("subprocess %s is still running" % self.pid,
-    # E ResourceWarning: subprocess 382685 is still running
+    # For some reason we get this error, see
+    # https://github.com/aiidalab/aiidalab-widgets-base/issues/551
     'ignore:Exception ignored in:pytest.PytestUnraisableExceptionWarning:_pytest',
     'ignore::DeprecationWarning:pytest_html',
     'ignore::DeprecationWarning:jupyter_client',
     'ignore::DeprecationWarning:selenium',
     'ignore::DeprecationWarning:pytest_selenium',
 ]
```

### Comparing `aiidalab_widgets_base-2.2.0a0/setup.cfg` & `aiidalab_widgets_base-2.2.0a1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 docs = 
 	sphinx
 	sphinx-design
 	pydata-sphinx-theme
 	myst-nb
 
 [bumpver]
-current_version = "v2.2.0a0"
+current_version = "v2.2.0a1"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
```

### Comparing `aiidalab_widgets_base-2.2.0a0/tests/test_bug_report.py` & `aiidalab_widgets_base-2.2.0a1/tests/test_bug_report.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a0/tests/test_computational_resources.py` & `aiidalab_widgets_base-2.2.0a1/tests/test_computational_resources.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a0/tests/test_databases.py` & `aiidalab_widgets_base-2.2.0a1/tests/test_databases.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a0/tests/test_elns.py` & `aiidalab_widgets_base-2.2.0a1/tests/test_elns.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a0/tests/test_export.py` & `aiidalab_widgets_base-2.2.0a1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a0/tests/test_nodes.py` & `aiidalab_widgets_base-2.2.0a1/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a0/tests/test_process.py` & `aiidalab_widgets_base-2.2.0a1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a0/tests/test_structures.py` & `aiidalab_widgets_base-2.2.0a1/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a0/tests/test_viewers.py` & `aiidalab_widgets_base-2.2.0a1/tests/test_viewers.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,48 +18,63 @@
     )
     viewer = viewers.StructureDataViewer()
     viewer.structure = ase_input
     assert viewer.periodicity.value == "Periodicity: xy"
 
 
 @pytest.mark.usefixtures("aiida_profile_clean")
-def test_several_data_viewers(
-    bands_data_object, folder_data_object, generate_calc_job_node
-):
+def test_several_data_viewers(bands_data_object, generate_calc_job_node):
     v = viewers.viewer(orm.Int(1))
 
     # No viewer for Int, so it should return the input
     assert isinstance(v, orm.Int)
 
     # DictViewer
     v = viewers.viewer(orm.Dict(dict={"a": 1}))
     assert isinstance(v, viewers.DictViewer)
 
     # BandsDataViewer
     v = viewers.viewer(bands_data_object)
     assert isinstance(v, viewers.BandsDataViewer)
 
-    # FolderDataViewer
-    v = viewers.viewer(folder_data_object)
-    assert isinstance(v, viewers.FolderDataViewer)
-
     # ProcessNodeViewer
     process = generate_calc_job_node(
         inputs={
             "parameters": orm.Int(1),
             "nested": {
                 "inner": orm.Int(2),
             },
         }
     )
     v = viewers.viewer(process)
     assert isinstance(v, viewers.ProcessNodeViewerWidget)
 
 
 @pytest.mark.usefixtures("aiida_profile_clean")
+def test_folder_data_viewer(folder_data_object):
+    v = viewers.viewer(folder_data_object)
+    assert isinstance(v, viewers.FolderDataViewer)
+
+    v.files.value = "test1.txt"
+    assert v.text.value == "content of test1.txt"
+
+    v.files.value = "test2.txt"
+    assert v.text.value == "content of test2.txt"
+    v.download_btn.click()
+    # NOTE: We're testing the download() method directly as well,
+    # since triggering it via self.download_btn.click() callback
+    # seems to swallow all exceptions.
+    v.download()
+
+    v.files.value = "test.bin"
+    assert v.text.value == "[Binary file, preview not available]"
+    v.download()
+
+
+@pytest.mark.usefixtures("aiida_profile_clean")
 def test_structure_data_viewer_storage(structure_data_object):
     v = viewers.viewer(structure_data_object)
     assert isinstance(v, viewers.StructureDataViewer)
 
     # Check the `_prepare_payload` function used for downloading.
     format_cases = [
         (
```

### Comparing `aiidalab_widgets_base-2.2.0a0/tests/test_wizard.py` & `aiidalab_widgets_base-2.2.0a1/tests/test_wizard.py`

 * *Files identical despite different names*

