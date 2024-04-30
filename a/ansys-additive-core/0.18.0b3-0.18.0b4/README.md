# Comparing `tmp/ansys_additive_core-0.18.0b3.tar.gz` & `tmp/ansys_additive_core-0.18.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_additive_core-0.18.0b3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_additive_core-0.18.0b4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_additive_core-0.18.0b3.tar` & `ansys_additive_core-0.18.0b4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1097 2024-03-20 23:04:31.830836 ansys_additive_core-0.18.0b3/LICENSE
--rw-r--r--   0        0        0     3904 2024-03-20 23:04:31.830836 ansys_additive_core-0.18.0b3/README.rst
--rw-r--r--   0        0        0     3666 2024-03-20 23:04:31.830836 ansys_additive_core-0.18.0b3/pyproject.toml
--rw-r--r--   0        0        0     3136 2024-03-20 23:04:31.830836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/__init__.py
--rw-r--r--   0        0        0    25352 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/additive.py
--rw-r--r--   0        0        0     1764 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/conversions.py
--rw-r--r--   0        0        0     3062 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/download.py
--rw-r--r--   0        0        0     1437 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/examples/__init__.py
--rw-r--r--   0        0        0     9864 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/examples/downloads.py
--rw-r--r--   0        0        0     1314 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/exceptions.py
--rw-r--r--   0        0        0     5315 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/geometry_file.py
--rw-r--r--   0        0        0     9103 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/logger.py
--rw-r--r--   0        0        0    13089 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/machine.py
--rw-r--r--   0        0        0    33644 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/material.py
--rw-r--r--   0        0        0     8255 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/material_tuning.py
--rw-r--r--   0        0        0    25863 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/microstructure.py
--rw-r--r--   0        0        0    17395 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/microstructure_3d.py
--rw-r--r--   0        0        0     1393 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/misc.py
--rw-r--r--   0        0        0     1629 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/__init__.py
--rw-r--r--   0        0        0     6296 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/constants.py
--rw-r--r--   0        0        0     1485 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/display/__init__.py
--rw-r--r--   0        0        0     3318 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/display/_common_controls.py
--rw-r--r--   0        0        0     8111 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/display/ave_grain_size_plot.py
--rw-r--r--   0        0        0    10178 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/display/porosity_contour_plot.py
--rw-r--r--   0        0        0     8770 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/display/porosity_eval_plot.py
--rw-r--r--   0        0        0     6387 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/display/show_table.py
--rw-r--r--   0        0        0     8617 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/display/single_bead_eval_plot.py
--rw-r--r--   0        0        0     9582 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/parametric_runner.py
--rw-r--r--   0        0        0    92580 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/parametric_study.py
--rw-r--r--   0        0        0     3252 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/parametric_utils.py
--rw-r--r--   0        0        0     6943 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/porosity.py
--rw-r--r--   0        0        0     3337 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/progress_logger.py
--rw-r--r--   0        0        0     1373 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/server_connection/__init__.py
--rw-r--r--   0        0        0     1711 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/server_connection/constants.py
--rw-r--r--   0        0        0     5563 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/server_connection/local_server.py
--rw-r--r--   0        0        0     2627 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/server_connection/network_utils.py
--rw-r--r--   0        0        0     8078 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/server_connection/server_connection.py
--rw-r--r--   0        0        0     2739 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/simulation.py
--rw-r--r--   0        0        0     8059 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/single_bead.py
--rw-r--r--   0        0        0    10190 2024-03-20 23:04:31.834836 ansys_additive_core-0.18.0b3/src/ansys/additive/core/thermal_history.py
--rw-r--r--   0        0        0     7485 1970-01-01 00:00:00.000000 ansys_additive_core-0.18.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/LICENSE
+-rw-r--r--   0        0        0     3904 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/README.rst
+-rw-r--r--   0        0        0     3679 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/pyproject.toml
+-rw-r--r--   0        0        0     3136 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/__init__.py
+-rw-r--r--   0        0        0    26598 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/additive.py
+-rw-r--r--   0        0        0     1764 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/conversions.py
+-rw-r--r--   0        0        0     3224 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/download.py
+-rw-r--r--   0        0        0     1437 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/examples/__init__.py
+-rw-r--r--   0        0        0     9864 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/examples/downloads.py
+-rw-r--r--   0        0        0     1314 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/exceptions.py
+-rw-r--r--   0        0        0     5315 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/geometry_file.py
+-rw-r--r--   0        0        0     9107 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/logger.py
+-rw-r--r--   0        0        0    13089 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/machine.py
+-rw-r--r--   0        0        0    33644 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/material.py
+-rw-r--r--   0        0        0     8255 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/material_tuning.py
+-rw-r--r--   0        0        0    25863 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/microstructure.py
+-rw-r--r--   0        0        0    17413 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/microstructure_3d.py
+-rw-r--r--   0        0        0     1393 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/misc.py
+-rw-r--r--   0        0        0     1629 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/__init__.py
+-rw-r--r--   0        0        0     6296 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/constants.py
+-rw-r--r--   0        0        0     1485 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/__init__.py
+-rw-r--r--   0        0        0     3318 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/_common_controls.py
+-rw-r--r--   0        0        0     8111 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/ave_grain_size_plot.py
+-rw-r--r--   0        0        0    10178 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/porosity_contour_plot.py
+-rw-r--r--   0        0        0     8770 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/porosity_eval_plot.py
+-rw-r--r--   0        0        0     6387 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/show_table.py
+-rw-r--r--   0        0        0     8617 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/single_bead_eval_plot.py
+-rw-r--r--   0        0        0    10207 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/parametric_runner.py
+-rw-r--r--   0        0        0    93178 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/parametric_study.py
+-rw-r--r--   0        0        0     3252 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/parametric_utils.py
+-rw-r--r--   0        0        0     6943 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/porosity.py
+-rw-r--r--   0        0        0     4835 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/progress_handler.py
+-rw-r--r--   0        0        0     1373 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/__init__.py
+-rw-r--r--   0        0        0     1711 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/constants.py
+-rw-r--r--   0        0        0     5563 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/local_server.py
+-rw-r--r--   0        0        0     2627 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/network_utils.py
+-rw-r--r--   0        0        0     8078 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/server_connection.py
+-rw-r--r--   0        0        0     2739 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/simulation.py
+-rw-r--r--   0        0        0     8059 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/single_bead.py
+-rw-r--r--   0        0        0    10190 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/thermal_history.py
+-rw-r--r--   0        0        0     7566 1970-01-01 00:00:00.000000 ansys_additive_core-0.18.0b4/PKG-INFO
```

### Comparing `ansys_additive_core-0.18.0b3/LICENSE` & `ansys_additive_core-0.18.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/README.rst` & `ansys_additive_core-0.18.0b4/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/pyproject.toml` & `ansys_additive_core-0.18.0b4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-additive-core"
-version = "0.18.0b3"
+version = "0.18.0b4"
 description = "A Python client for the Ansys Additive service"
 readme = "README.rst"
 requires-python = ">=3.9,<4"
 license = { file = "LICENSE" }
 authors = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 maintainers = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 classifiers = [
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
 dependencies = [
-    "ansys-api-additive==1.6.7",
+    "ansys-api-additive==1.7.2",
     "ansys-platform-instancemanagement>=1.1.1",
     "dill>=0.3.7",
     "google-api-python-client>=1.7.11",
     "googleapis-common-protos>=1.52.0",
     "grpcio>=1.35.0",
     "grpcio-health-checking>=1.45.0",
     "importlib-metadata>=4.0",
@@ -37,55 +37,56 @@
     "pandas>=1.3.2",
     "panel>=1.2.1",
     "platformdirs>=3.8.0",
     "plotly>=5.16.1",
     "protobuf>=3.20.2,<5",
     "six>=1.16.0",
     "tqdm>=4.45.0",
+    "pydantic>=2.6.3",
 ]
 
 [project.optional-dependencies]
 tests = [
     "ansys-platform-instancemanagement==1.1.2",
     "dill==0.3.8",
-    "google-api-python-client==2.120.0",
-    "googleapis-common-protos==1.62.0",
+    "google-api-python-client==2.122.0",
+    "googleapis-common-protos==1.63.0",
     "grpcio==1.60.0",
     "grpcio-health-checking==1.48.2",
     "numpy==1.26.4",
-    "pandas==2.2.1",
-    "panel==1.3.8",
-    "platformdirs==4.2.0",
-    "plotly==5.19.0",
+    "pandas==2.2.2",
+    "panel==1.4.2",
+    "platformdirs==4.2.1",
+    "plotly==5.21.0",
     "protobuf==4.25.3",
     "six==1.16.0",
     "tqdm==4.66.2",
-    # Test specific dependencies
-    "pytest==8.1.0",
-    "pytest-cov==4.0.0",
+    "pydantic==2.7.1",
+    "pytest==8.2.0",
+    "pytest-cov==5.0.0",
 ]
 
 doc = [
-    "ansys-sphinx-theme==0.14.0",
-    "enum-tools==0.11.0",
+    "ansys-sphinx-theme==0.15.2",
+    "enum-tools==0.12.0",
     "jupyter_sphinx==0.5.3",
-    "matplotlib==3.8.3",
-    "numpydoc==1.6.0",
-    "panel==1.3.8",
+    "matplotlib==3.8.4",
+    "numpydoc==1.7.0",
+    "panel==1.4.2",
     "phantomjs==1.4.1",
     "pypandoc==1.13",
-    "pyvista==0.43.3",
-    "selenium==4.18.1",
-    "sphinx==7.2.6",
+    "pyvista==0.43.6",
+    "selenium==4.20.0",
+    "sphinx==7.3.7",
     "sphinx-autoapi==3.0.0",
     #"sphinx-autoapi @ git+https://github.com/ansys/sphinx-autoapi@feat/single-page-stable",
-    "sphinx-autodoc-typehints==2.0.0",
+    "sphinx-autodoc-typehints==2.1.0",
     "sphinx-copybutton==0.5.2",
     "sphinx-design==0.5.0",
-    "sphinx-gallery==0.15.0",
+    "sphinx-gallery==0.16.0",
     "sphinx-jinja==2.0.2",
     "sphinx-notfound-page==1.0.0",
     "sphinx-toolbox==3.5.0",
     "sphinxemoji==0.3.1",
 ]
 
 [project.urls]
```

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/__init__.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/additive.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/additive.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,30 +28,35 @@
 from datetime import datetime
 import hashlib
 import logging
 import os
 import zipfile
 
 from ansys.api.additive import __version__ as api_version
-from ansys.api.additive.v0.additive_domain_pb2 import ProgressState
 from ansys.api.additive.v0.additive_materials_pb2 import GetMaterialRequest
 from ansys.api.additive.v0.additive_simulation_pb2 import UploadFileRequest
 from google.protobuf.empty_pb2 import Empty
 import grpc
 
 from ansys.additive.core import USER_DATA_PATH, __version__
 from ansys.additive.core.download import download_file
 from ansys.additive.core.exceptions import BetaFeatureNotEnabledError
+from ansys.additive.core.logger import LOG
 from ansys.additive.core.material import AdditiveMaterial
 from ansys.additive.core.material_tuning import MaterialTuningInput, MaterialTuningSummary
 from ansys.additive.core.microstructure import MicrostructureInput, MicrostructureSummary
 from ansys.additive.core.microstructure_3d import Microstructure3DInput, Microstructure3DSummary
 import ansys.additive.core.misc as misc
 from ansys.additive.core.porosity import PorosityInput, PorositySummary
-from ansys.additive.core.progress_logger import ProgressLogger
+from ansys.additive.core.progress_handler import (
+    DefaultSingleSimulationProgressHandler,
+    IProgressHandler,
+    Progress,
+    ProgressState,
+)
 from ansys.additive.core.server_connection import DEFAULT_PRODUCT_VERSION, ServerConnection
 from ansys.additive.core.simulation import SimulationError
 from ansys.additive.core.single_bead import SingleBeadInput, SingleBeadSummary
 from ansys.additive.core.thermal_history import ThermalHistoryInput, ThermalHistorySummary
 
 
 class Additive:
@@ -157,15 +162,15 @@
         self._nsims_per_server = nsims_per_server
         self._enable_beta_features = enable_beta_features
 
         # Setup data directory
         self._user_data_path = USER_DATA_PATH
         if not os.path.exists(self._user_data_path):  # pragma: no cover
             os.makedirs(self._user_data_path)
-        print("user data path: " + self._user_data_path)
+        LOG.info("user data path: " + self._user_data_path)
 
     @staticmethod
     def _create_logger(log_file, log_level) -> logging.Logger:
         """Instantiate the logger."""
         format = "%(asctime)s %(message)s"
         datefmt = "%Y-%m-%d %H:%M:%S"
         numeric_level = getattr(logging, log_level.upper(), None)
@@ -260,14 +265,15 @@
             SingleBeadInput
             | PorosityInput
             | MicrostructureInput
             | ThermalHistoryInput
             | Microstructure3DInput
             | list
         ),
+        progress_handler: IProgressHandler | None = None,
     ) -> (
         SingleBeadSummary
         | PorositySummary
         | MicrostructureSummary
         | ThermalHistorySummary
         | Microstructure3DSummary
         | SimulationError
@@ -275,71 +281,78 @@
     ):
         """Execute additive simulations.
 
         Parameters
         ----------
         inputs: SingleBeadInput, PorosityInput, MicrostructureInput, ThermalHistoryInput,
         Microstructure3DInput, list
-            Parameters to use for simulations. A list of inputs may be provided to execute multiple
+            Parameters to use for simulations. A list of inputs may be provided to run multiple
             simulations.
+        progress_handler: IProgressHandler, None, default: None
+            Handler for progress updates. If ``None``, and ``inputs`` contains a single
+            simulation input, a default progress handler will be assigned.
 
         Returns
         -------
         SingleBeadSummary, PorositySummary, MicrostructureSummary, ThermalHistorySummary,
         Microstructure3DSummary, SimulationError, list
             One or more summaries of simulation results. If a list of inputs is provided, a
             list is returned.
         """
         self._check_for_duplicate_id(inputs)
 
         if not isinstance(inputs, list):
-            return self._simulate(inputs, self._servers[0], show_progress=True)
+            if not progress_handler:
+                progress_handler = DefaultSingleSimulationProgressHandler()
+            return self._simulate(inputs, self._servers[0], progress_handler)
+
+        if len(inputs) == 0:
+            raise ValueError("No simulation inputs provided")
 
         summaries = []
-        print(
-            f"{datetime.now().strftime('%Y-%m-%d %H:%M:%S')} Completed 0 of {len(inputs)} simulations",
+        LOG.info(
+            f"{datetime.now().strftime('%Y-%m-%d %H:%M:%S')} Starting {len(inputs)} simulations",
             end="",
         )
         threads = min(len(inputs), len(self._servers) * self._nsims_per_server)
         with concurrent.futures.ThreadPoolExecutor(threads) as executor:
             futures = []
             for i, input in enumerate(inputs):
                 server_id = i % len(self._servers)
                 futures.append(
                     executor.submit(
                         self._simulate,
                         input=input,
                         server=self._servers[server_id],
-                        show_progress=False,
+                        progress_handler=progress_handler,
                     )
                 )
             for future in concurrent.futures.as_completed(futures):
                 summary = future.result()
                 if isinstance(summary, SimulationError):
-                    print(f"\nError: {summary.message}")
+                    LOG.error(f"\nError: {summary.message}")
                 summaries.append(summary)
                 timestamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-                print(
+                LOG.info(
                     f"\r{timestamp} Completed {len(summaries)} of {len(inputs)} simulations",
                     end="",
                 )
-        print("")
         return summaries
 
     def _simulate(
         self,
         input: (
             SingleBeadInput
             | PorosityInput
             | MicrostructureInput
             | ThermalHistoryInput
             | Microstructure3DInput
         ),
         server: ServerConnection,
-        show_progress: bool = False,
+        progress_handler: IProgressHandler | None = None,
     ) -> (
         SingleBeadSummary
         | PorositySummary
         | MicrostructureSummary
         | ThermalHistorySummary
         | Microstructure3DSummary
         | SimulationError
@@ -351,48 +364,47 @@
         input: SingleBeadInput, PorosityInput, MicrostructureInput, ThermalHistoryInput,
         Microstructure3DInput
             Parameters to use for simulation.
 
         server: ServerConnection
             Server to use for the simulation.
 
-        show_progress: bool, False
-            Whether to send progress updates to the user interface.
+        progress_handler: IProgressHandler, None, default: None
+            Handler for progress updates. If ``None``, no progress updates are provided.
 
         Returns
         -------
         SingleBeadSummary, PorositySummary, MicrostructureSummary, ThermalHistorySummary,
         Microstructure3DSummary, SimulationError
         """
-        logger = None
-        if show_progress:
-            logger = ProgressLogger("Simulation")  # pragma: no cover
-
         if input.material == AdditiveMaterial():
             raise ValueError("A material is not assigned to the simulation input")
 
         if isinstance(input, Microstructure3DInput) and self.enable_beta_features is False:
             raise BetaFeatureNotEnabledError(
                 "3D microstructure simulations require beta features to be enabled.\n"
                 + "Set enable_beta_features=True when creating the Additive client."
             )
 
         try:
             request = None
             if isinstance(input, ThermalHistoryInput):
-                return self._simulate_thermal_history(input, USER_DATA_PATH, server, logger)
+                return self._simulate_thermal_history(
+                    input, USER_DATA_PATH, server, progress_handler
+                )
             else:
                 request = input._to_simulation_request()
 
             for response in server.simulation_stub.Simulate(request):
                 if response.HasField("progress"):
-                    if logger:
-                        logger.log_progress(response.progress)  # pragma: no cover
-                    if response.progress.state == ProgressState.PROGRESS_STATE_ERROR:
-                        raise Exception(response.progress.message)
+                    progress = Progress.from_proto_msg(input.id, response.progress)
+                    if progress_handler:
+                        progress_handler.update(progress)
+                    if progress.state == ProgressState.ERROR:
+                        raise Exception(progress.message)
                 if response.HasField("melt_pool"):
                     return SingleBeadSummary(input, response.melt_pool)
                 if response.HasField("porosity_result"):
                     return PorositySummary(input, response.porosity_result)
                 if response.HasField("microstructure_result"):
                     return MicrostructureSummary(
                         input, response.microstructure_result, self._user_data_path
@@ -460,15 +472,18 @@
         material = AdditiveMaterial()
         material._load_parameters(parameters_file)
         material._load_thermal_properties(thermal_lookup_file)
         material._load_characteristic_width(characteristic_width_lookup_file)
         return material
 
     def tune_material(
-        self, input: MaterialTuningInput, out_dir: str = USER_DATA_PATH
+        self,
+        input: MaterialTuningInput,
+        out_dir: str = USER_DATA_PATH,
+        progress_handler: IProgressHandler = None,
     ) -> MaterialTuningSummary:
         """Tune a custom material for use with additive simulations.
 
         This method performs the same function as the Material Tuning Tool
         described in
         `Find Simulation Parameters to Match Simulation to Experiments
         <https://ansyshelp.ansys.com/account/secured?returnurl=/Views/Secured/corp/v232/en/add_beta/add_print_udm_tool_match_sim_to_exp.html>`_.
@@ -477,14 +492,18 @@
         `Chapter 2: Material Tuning Tool (Beta) to Create User Defined Materials
         <https://ansyshelp.ansys.com/account/secured?returnurl=/Views/Secured/corp/v232/en/add_beta/add_science_BETA_material_tuning_tool.html>`_.
 
         Parameters
         ----------
         input: MaterialTuningInput
             Input parameters for material tuning.
+        out_dir: str, default: USER_DATA_PATH
+            Folder path for output files.
+        progress_handler: IProgressHandler, None, default: None
+            Handler for progress updates. If ``None``, no progress updates are provided.
 
         Returns
         -------
         MaterialTuningSummary
             Summary of material tuning.
         """  # noqa: E501
         if input.id == "":
@@ -497,25 +516,28 @@
                 f"Directory {out_dir} already exists. Delete or choose a different output directory."
             )
 
         request = input._to_request()
 
         for response in self._servers[0].materials_stub.TuneMaterial(request):
             if response.HasField("progress"):
-                if response.progress.state == ProgressState.PROGRESS_STATE_ERROR:
-                    raise Exception(response.progress.message)
+                progress = Progress.from_proto_msg(input.id, response.progress)
+                if progress.state == ProgressState.ERROR:
+                    raise Exception(progress.message)
                 else:
-                    for m in response.progress.message.splitlines():
+                    for m in progress.message.splitlines():
                         if (
                             "License successfully" in m
                             or "Starting ThermalSolver" in m
                             or "threads for solver" in m
                         ):
                             continue
-                        print(m)
+                        LOG.info(m)
+                        if progress_handler:
+                            progress_handler.update(progress)
             if response.HasField("result"):
                 return MaterialTuningSummary(input, response.result, out_dir)
 
     def __file_upload_reader(
         self, file_name: str, chunk_size=2 * 1024**2
     ) -> Iterator[UploadFileRequest]:
         """Read a file and return an iterator of UploadFileRequests."""
@@ -534,56 +556,56 @@
                 )
 
     def _simulate_thermal_history(
         self,
         input: ThermalHistoryInput,
         out_dir: str,
         server: ServerConnection,
-        logger: ProgressLogger | None = None,
+        progress_handler: IProgressHandler | None = None,
     ) -> ThermalHistorySummary:
-        """Execute a thermal history simulation.
+        """Run a thermal history simulation.
 
-        Parameters
-        ----------
-        input: ThermalHistoryInput
-            Simulation input parameters.
-        out_dir: str
-            Folder path for output files.
-        server: ServerConnection
-            Server to use for the simulation.
-        logger: ProgressLogger
-            Log message handler.
-
-        Returns
-        -------
-        :class:`ThermalHistorySummary`
+                Parameters
+                ----------
+                input: ThermalHistoryInput
+                    Simulation input parameters.
+                out_dir: str
+                    Folder path for output files.
+                server: ServerConnection
+                    Server to use for the simulation.
+                progress_handler: IPorgressHandler, None, default: None
+                    Handler for progress updates. If ``None``, no progress updates are provided.
+        .
+
+                Returns
+                -------
+                :class:`ThermalHistorySummary`
         """
         if input.geometry is None or input.geometry.path == "":
             raise ValueError("The geometry path is not defined in the simulation input")
 
         remote_geometry_path = ""
         for response in server.simulation_stub.UploadFile(
             self.__file_upload_reader(input.geometry.path)
         ):
             remote_geometry_path = response.remote_file_name
-            if logger:
-                logger.log_progress(response.progress)  # pragma: no cover
-            if response.progress.state == ProgressState.PROGRESS_STATE_ERROR:
-                raise Exception(response.progress.message)
+            progress = Progress.from_proto_msg(input.id, response.progress)
+            if progress_handler:
+                progress_handler.update(progress)
+            if progress.state == ProgressState.ERROR:
+                raise Exception(progress.message)
 
         request = input._to_simulation_request(remote_geometry_path=remote_geometry_path)
         for response in server.simulation_stub.Simulate(request):
             if response.HasField("progress"):
-                if logger:
-                    logger.log_progress(response.progress)  # pragma: no cover
-                if (
-                    response.progress.state == ProgressState.PROGRESS_STATE_ERROR
-                    and "WARN" not in response.progress.message
-                ):
-                    raise Exception(response.progress.message)
+                progress = Progress.from_proto_msg(input.id, response.progress)
+                if progress_handler:
+                    progress_handler.update(progress)
+                if progress.state == ProgressState.ERROR and "WARN" not in progress.message:
+                    raise Exception(progress.message)
             if response.HasField("thermal_history_result"):
                 path = os.path.join(out_dir, input.id, "coax_ave_output")
                 local_zip = download_file(
                     server.simulation_stub,
                     response.thermal_history_result.coax_ave_zip_file,
                     path,
                 )
```

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/conversions.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/conversions.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/download.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/download.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,33 +22,33 @@
 """Provides a function for downloading files from the server to the client."""
 import hashlib
 import os
 
 from ansys.api.additive.v0.additive_simulation_pb2 import DownloadFileRequest
 from ansys.api.additive.v0.additive_simulation_pb2_grpc import SimulationServiceStub
 
-from ansys.additive.core.progress_logger import Progress, ProgressLogger, ProgressState
+from ansys.additive.core.progress_handler import IProgressHandler, Progress, ProgressState
 
 
 def download_file(
     stub: SimulationServiceStub,
     remote_file_name: str,
     local_folder: str,
-    logger: ProgressLogger = None,
+    progress_handler: IProgressHandler = None,
 ) -> str:
     """Download a file from the server to the localhost.
 
     Parameters
     ----------
     remote_file_name: str
         Path to file on the server.
     local_folder: str
         Folder on your localhost to write your file to.
-    logger: ProgressLogger
-        Log message handler.
+    progress_handler: ProgressLogger, None, default: None
+        Progress update handler. If ``None``, no progress will be provided.
 
     Returns
     -------
     str
         Local path of downloaded file.
     """
 
@@ -56,22 +56,25 @@
         os.makedirs(local_folder)
 
     dest = os.path.join(local_folder, os.path.basename(remote_file_name))
     request = DownloadFileRequest(remote_file_name=remote_file_name)
 
     with open(dest, "wb") as f:
         for response in stub.DownloadFile(request):
-            if logger:
-                logger.log_progress(response.progress)  # pragma: no cover
+            if progress_handler:
+                progress_handler.update(
+                    Progress.from_proto_msg(response.progress)
+                )  # pragma: no cover
             if len(response.content) > 0:
                 md5 = hashlib.md5(response.content).hexdigest()
                 if md5 != response.content_md5:
-                    if logger:  # pragma: no cover
-                        logger.log_progress(
+                    msg = "Download error, MD5 sums did not match"
+                    if progress_handler:  # pragma: no cover
+                        progress_handler.update(
                             Progress(
-                                state=ProgressState.PROGRESS_STATE_ERROR,
-                                message="Download error, MD5 sums did not match",
+                                state=ProgressState.ERROR,
+                                message=msg,
                             )
                         )
-                    raise ValueError("Download error, MD5 sums did not match")
+                    raise ValueError(msg)
                 f.write(response.content)
     return dest
```

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/examples/__init__.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/examples/downloads.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/exceptions.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/geometry_file.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/geometry_file.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/logger.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 You can rename this logger to avoid conflicts with other loggers (if any):
 
 .. code:: python
 
    from ansys.additive.core import LOG as logger
 
-The default logging level of ``LOG`` is ``ERROR``.
+The default logging level of ``LOG`` is ``WARNING``.
 You can change this level and output lower-level messages with
 this code:
 
 .. code:: python
 
    LOG.logger.setLevel("DEBUG")
    LOG.file_handler.setLevel("DEBUG")  # If present.
@@ -279,8 +279,8 @@
     return logger
 
 
 # ===============================================================
 # Finally define logger
 # ===============================================================
 
-LOG = Logger(level=logging.ERROR, to_file=False, to_stdout=True)
+LOG = Logger(level=logging.WARNING, to_file=False, to_stdout=True)
```

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/machine.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/machine.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/material.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/material.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/material_tuning.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/material_tuning.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/microstructure.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/microstructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     """Minimum melt pool depth (m)."""
     MAX_MELT_POOL_DEPTH = 8e-4
     """Maximum melt pool depth (m)."""
     DEFAULT_RANDOM_SEED = 0
     """The default random seed, which indicates that a random seed was not provided."""
     MIN_RANDOM_SEED = 1
     """Minimum random seed."""
-    MAX_RANDOM_SEED = 2**31 - 1
+    MAX_RANDOM_SEED = 2**32 - 1
     """Maximum random seed."""
 
     def __init__(
         self,
         id: str = "",
         *,
         sample_min_x: float = DEFAULT_POSITION_COORDINATE,
```

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/microstructure_3d.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/microstructure_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,16 +394,16 @@
         """
         return self._input
 
     @property
     def grain_3d_vtk(self) -> str:
         """Path to the VTK file containing the 3D grain structure data.
 
-        The VTK file contains these scalar data sets" ``GrainNumber``, ``Phi0``,
-        ``Phi1``, ``Phi2``, and ``Temperatures``.
+        The VTK file contains these scalar data sets" ``GrainNumber``, ``Phi0_(deg)``,
+        ``Phi1_(deg)``, ``Phi2_(deg)``, and ``Temperatures``.
         """
         return self._grain_3d_vtk
 
     @property
     def xy_average_grain_size(self) -> float:
         """Average grain size (µm) for the XY plane."""
         return self._2d_result._xy_average_grain_size
```

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/misc.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/__init__.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/constants.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/display/__init__.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/display/_common_controls.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/_common_controls.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/display/ave_grain_size_plot.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/ave_grain_size_plot.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/display/porosity_contour_plot.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/porosity_contour_plot.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/display/porosity_eval_plot.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/porosity_eval_plot.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/display/show_table.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/show_table.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/display/single_bead_eval_plot.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/single_bead_eval_plot.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/parametric_runner.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/parametric_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 """Provides a class to run parametric study simulations."""
 from __future__ import annotations
 
 import numpy as np
 import pandas as pd
 
 from ansys.additive.core import (
+    LOG,
     Additive,
     AdditiveMachine,
     AdditiveMaterial,
     MachineConstants,
     MicrostructureInput,
     MicrostructureSummary,
     PorosityInput,
@@ -119,40 +120,52 @@
                 inputs.append(ParametricRunner._create_microstructure_input(row, material, machine))
             else:  # pragma: no cover
                 print(
                     f"Invalid simulation type: {row[ColumnNames.TYPE]} for {row[ColumnNames.ID]}, skipping"
                 )
                 continue
 
+        if len(inputs) == 0:
+            LOG.warning("None of the input simulations meet the criteria selected")
+            return []
+
         summaries = additive.simulate(inputs)
 
         # TODO: Return the summaries one at a time, possibly as an iterator,
         # so that the data frame can be updated as each simulation completes.
         return summaries
 
     @staticmethod
     def _create_machine(row: pd.Series) -> AdditiveMachine:
         return AdditiveMachine(
             laser_power=row[ColumnNames.LASER_POWER],
             scan_speed=row[ColumnNames.SCAN_SPEED],
             layer_thickness=row[ColumnNames.LAYER_THICKNESS],
             beam_diameter=row[ColumnNames.BEAM_DIAMETER],
             heater_temperature=row[ColumnNames.HEATER_TEMPERATURE],
-            starting_layer_angle=row[ColumnNames.START_ANGLE]
-            if not np.isnan(row[ColumnNames.START_ANGLE])
-            else MachineConstants.DEFAULT_STARTING_LAYER_ANGLE,
-            layer_rotation_angle=row[ColumnNames.ROTATION_ANGLE]
-            if not np.isnan(row[ColumnNames.ROTATION_ANGLE])
-            else MachineConstants.DEFAULT_LAYER_ROTATION_ANGLE,
-            hatch_spacing=row[ColumnNames.HATCH_SPACING]
-            if not np.isnan(row[ColumnNames.HATCH_SPACING])
-            else MachineConstants.DEFAULT_HATCH_SPACING,
-            slicing_stripe_width=row[ColumnNames.STRIPE_WIDTH]
-            if not np.isnan(row[ColumnNames.STRIPE_WIDTH])
-            else MachineConstants.DEFAULT_SLICING_STRIPE_WIDTH,
+            starting_layer_angle=(
+                row[ColumnNames.START_ANGLE]
+                if not np.isnan(row[ColumnNames.START_ANGLE])
+                else MachineConstants.DEFAULT_STARTING_LAYER_ANGLE
+            ),
+            layer_rotation_angle=(
+                row[ColumnNames.ROTATION_ANGLE]
+                if not np.isnan(row[ColumnNames.ROTATION_ANGLE])
+                else MachineConstants.DEFAULT_LAYER_ROTATION_ANGLE
+            ),
+            hatch_spacing=(
+                row[ColumnNames.HATCH_SPACING]
+                if not np.isnan(row[ColumnNames.HATCH_SPACING])
+                else MachineConstants.DEFAULT_HATCH_SPACING
+            ),
+            slicing_stripe_width=(
+                row[ColumnNames.STRIPE_WIDTH]
+                if not np.isnan(row[ColumnNames.STRIPE_WIDTH])
+                else MachineConstants.DEFAULT_SLICING_STRIPE_WIDTH
+            ),
         )
 
     @staticmethod
     def _create_single_bead_input(
         row: pd.Series, material: AdditiveMaterial, machine: AdditiveMachine
     ) -> SingleBeadInput:
         return SingleBeadInput(
@@ -191,32 +204,48 @@
             material=material,
             machine=machine,
             sample_size_x=row[ColumnNames.MICRO_SIZE_X],
             sample_size_y=row[ColumnNames.MICRO_SIZE_Y],
             sample_size_z=row[ColumnNames.MICRO_SIZE_Z],
             sensor_dimension=row[ColumnNames.MICRO_SENSOR_DIM],
             use_provided_thermal_parameters=use_provided_thermal_param,
-            sample_min_x=row[ColumnNames.MICRO_MIN_X]
-            if not np.isnan(row[ColumnNames.MICRO_MIN_X])
-            else MicrostructureInput.DEFAULT_POSITION_COORDINATE,
-            sample_min_y=row[ColumnNames.MICRO_MIN_Y]
-            if not np.isnan(row[ColumnNames.MICRO_MIN_Y])
-            else MicrostructureInput.DEFAULT_POSITION_COORDINATE,
-            sample_min_z=row[ColumnNames.MICRO_MIN_Z]
-            if not np.isnan(row[ColumnNames.MICRO_MIN_Z])
-            else MicrostructureInput.DEFAULT_POSITION_COORDINATE,
-            cooling_rate=row[ColumnNames.COOLING_RATE]
-            if not np.isnan(row[ColumnNames.COOLING_RATE])
-            else MicrostructureInput.DEFAULT_COOLING_RATE,
-            thermal_gradient=row[ColumnNames.THERMAL_GRADIENT]
-            if not np.isnan(row[ColumnNames.THERMAL_GRADIENT])
-            else MicrostructureInput.DEFAULT_THERMAL_GRADIENT,
-            melt_pool_width=row[ColumnNames.MICRO_MELT_POOL_WIDTH]
-            if not np.isnan(row[ColumnNames.MICRO_MELT_POOL_WIDTH])
-            else MicrostructureInput.DEFAULT_MELT_POOL_WIDTH,
-            melt_pool_depth=row[ColumnNames.MICRO_MELT_POOL_DEPTH]
-            if not np.isnan(row[ColumnNames.MICRO_MELT_POOL_DEPTH])
-            else MicrostructureInput.DEFAULT_MELT_POOL_DEPTH,
-            random_seed=row[ColumnNames.RANDOM_SEED]
-            if not np.isnan(row[ColumnNames.RANDOM_SEED])
-            else MicrostructureInput.DEFAULT_RANDOM_SEED,
+            sample_min_x=(
+                row[ColumnNames.MICRO_MIN_X]
+                if not np.isnan(row[ColumnNames.MICRO_MIN_X])
+                else MicrostructureInput.DEFAULT_POSITION_COORDINATE
+            ),
+            sample_min_y=(
+                row[ColumnNames.MICRO_MIN_Y]
+                if not np.isnan(row[ColumnNames.MICRO_MIN_Y])
+                else MicrostructureInput.DEFAULT_POSITION_COORDINATE
+            ),
+            sample_min_z=(
+                row[ColumnNames.MICRO_MIN_Z]
+                if not np.isnan(row[ColumnNames.MICRO_MIN_Z])
+                else MicrostructureInput.DEFAULT_POSITION_COORDINATE
+            ),
+            cooling_rate=(
+                row[ColumnNames.COOLING_RATE]
+                if not np.isnan(row[ColumnNames.COOLING_RATE])
+                else MicrostructureInput.DEFAULT_COOLING_RATE
+            ),
+            thermal_gradient=(
+                row[ColumnNames.THERMAL_GRADIENT]
+                if not np.isnan(row[ColumnNames.THERMAL_GRADIENT])
+                else MicrostructureInput.DEFAULT_THERMAL_GRADIENT
+            ),
+            melt_pool_width=(
+                row[ColumnNames.MICRO_MELT_POOL_WIDTH]
+                if not np.isnan(row[ColumnNames.MICRO_MELT_POOL_WIDTH])
+                else MicrostructureInput.DEFAULT_MELT_POOL_WIDTH
+            ),
+            melt_pool_depth=(
+                row[ColumnNames.MICRO_MELT_POOL_DEPTH]
+                if not np.isnan(row[ColumnNames.MICRO_MELT_POOL_DEPTH])
+                else MicrostructureInput.DEFAULT_MELT_POOL_DEPTH
+            ),
+            random_seed=(
+                row[ColumnNames.RANDOM_SEED]
+                if not np.isnan(row[ColumnNames.RANDOM_SEED])
+                else MicrostructureInput.DEFAULT_RANDOM_SEED
+            ),
         )
```

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/parametric_study.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/parametric_study.py`

 * *Files 0% similar despite different names*

```diff
@@ -5752,36 +5752,73 @@
 00016770: 525f 4449 4d5d 2c0a 2020 2020 2020 2020  R_DIM],.        
 00016780: 2020 2020 2020 2020 7573 655f 7072 6f76          use_prov
 00016790: 6964 6564 5f74 6865 726d 616c 5f70 6172  ided_thermal_par
 000167a0: 616d 6574 6572 733d 7465 7374 5f75 7365  ameters=test_use
 000167b0: 5f70 726f 7669 6465 645f 7468 6572 6d61  _provided_therma
 000167c0: 6c5f 7061 7261 6d65 7465 7273 2c0a 2020  l_parameters,.  
 000167d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000167e0: 6f6c 696e 675f 7261 7465 3d74 6573 745f  oling_rate=test_
-000167f0: 636f 6f6c 696e 675f 7261 7465 2c0a 2020  cooling_rate,.  
-00016800: 2020 2020 2020 2020 2020 2020 2020 7468                th
-00016810: 6572 6d61 6c5f 6772 6164 6965 6e74 3d74  ermal_gradient=t
-00016820: 6573 745f 7468 6572 6d61 6c5f 6772 6164  est_thermal_grad
-00016830: 6965 6e74 2c0a 2020 2020 2020 2020 2020  ient,.          
-00016840: 2020 2020 2020 6d65 6c74 5f70 6f6f 6c5f        melt_pool_
-00016850: 7769 6474 683d 7465 7374 5f6d 656c 745f  width=test_melt_
-00016860: 706f 6f6c 5f77 6964 7468 2c0a 2020 2020  pool_width,.    
-00016870: 2020 2020 2020 2020 2020 2020 6d65 6c74              melt
-00016880: 5f70 6f6f 6c5f 6465 7074 683d 7465 7374  _pool_depth=test
-00016890: 5f6d 656c 745f 706f 6f6c 5f64 6570 7468  _melt_pool_depth
-000168a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000168b0: 2020 7261 6e64 6f6d 5f73 6565 643d 7465    random_seed=te
-000168c0: 7374 5f72 616e 646f 6d5f 7365 6564 2c0a  st_random_seed,.
-000168d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168e0: 6d61 6368 696e 653d 6d61 6368 696e 652c  machine=machine,
-000168f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016900: 206d 6174 6572 6961 6c3d 6d61 7465 7269   material=materi
-00016910: 616c 2c0a 2020 2020 2020 2020 2020 2020  al,.            
-00016920: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00016930: 7475 726e 2028 5472 7565 2c20 2222 290a  turn (True, "").
-00016940: 2020 2020 2020 2020 6578 6365 7074 2056          except V
-00016950: 616c 7565 4572 726f 7220 6173 2065 3a0a  alueError as e:.
-00016960: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00016970: 726e 2028 4661 6c73 652c 2028 6622 496e  rn (False, (f"In
-00016980: 7661 6c69 6420 7061 7261 6d65 7465 7220  valid parameter 
-00016990: 636f 6d62 696e 6174 696f 6e3a 207b 657d  combination: {e}
-000169a0: 2229 290a                                ")).
+000167e0: 6f6c 696e 675f 7261 7465 3d4d 6963 726f  oling_rate=Micro
+000167f0: 7374 7275 6374 7572 6549 6e70 7574 2e44  structureInput.D
+00016800: 4546 4155 4c54 5f43 4f4f 4c49 4e47 5f52  EFAULT_COOLING_R
+00016810: 4154 450a 2020 2020 2020 2020 2020 2020  ATE.            
+00016820: 2020 2020 6966 2028 7465 7374 5f63 6f6f      if (test_coo
+00016830: 6c69 6e67 5f72 6174 6520 6973 204e 6f6e  ling_rate is Non
+00016840: 6520 6f72 206d 6174 682e 6973 6e61 6e28  e or math.isnan(
+00016850: 7465 7374 5f63 6f6f 6c69 6e67 5f72 6174  test_cooling_rat
+00016860: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
+00016870: 2020 2020 656c 7365 2074 6573 745f 636f      else test_co
+00016880: 6f6c 696e 675f 7261 7465 2c0a 2020 2020  oling_rate,.    
+00016890: 2020 2020 2020 2020 2020 2020 7468 6572              ther
+000168a0: 6d61 6c5f 6772 6164 6965 6e74 3d4d 6963  mal_gradient=Mic
+000168b0: 726f 7374 7275 6374 7572 6549 6e70 7574  rostructureInput
+000168c0: 2e44 4546 4155 4c54 5f54 4845 524d 414c  .DEFAULT_THERMAL
+000168d0: 5f47 5241 4449 454e 540a 2020 2020 2020  _GRADIENT.      
+000168e0: 2020 2020 2020 2020 2020 6966 2028 7465            if (te
+000168f0: 7374 5f74 6865 726d 616c 5f67 7261 6469  st_thermal_gradi
+00016900: 656e 7420 6973 204e 6f6e 6520 6f72 206d  ent is None or m
+00016910: 6174 682e 6973 6e61 6e28 7465 7374 5f74  ath.isnan(test_t
+00016920: 6865 726d 616c 5f67 7261 6469 656e 7429  hermal_gradient)
+00016930: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00016940: 2020 656c 7365 2074 6573 745f 7468 6572    else test_ther
+00016950: 6d61 6c5f 6772 6164 6965 6e74 2c0a 2020  mal_gradient,.  
+00016960: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00016970: 6c74 5f70 6f6f 6c5f 7769 6474 683d 4d69  lt_pool_width=Mi
+00016980: 6372 6f73 7472 7563 7475 7265 496e 7075  crostructureInpu
+00016990: 742e 4445 4641 554c 545f 4d45 4c54 5f50  t.DEFAULT_MELT_P
+000169a0: 4f4f 4c5f 5749 4454 480a 2020 2020 2020  OOL_WIDTH.      
+000169b0: 2020 2020 2020 2020 2020 6966 2028 7465            if (te
+000169c0: 7374 5f6d 656c 745f 706f 6f6c 5f77 6964  st_melt_pool_wid
+000169d0: 7468 2069 7320 4e6f 6e65 206f 7220 6d61  th is None or ma
+000169e0: 7468 2e69 736e 616e 2874 6573 745f 6d65  th.isnan(test_me
+000169f0: 6c74 5f70 6f6f 6c5f 7769 6474 6829 290a  lt_pool_width)).
+00016a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a10: 656c 7365 2074 6573 745f 6d65 6c74 5f70  else test_melt_p
+00016a20: 6f6f 6c5f 7769 6474 682c 0a20 2020 2020  ool_width,.     
+00016a30: 2020 2020 2020 2020 2020 206d 656c 745f             melt_
+00016a40: 706f 6f6c 5f64 6570 7468 3d4d 6963 726f  pool_depth=Micro
+00016a50: 7374 7275 6374 7572 6549 6e70 7574 2e44  structureInput.D
+00016a60: 4546 4155 4c54 5f4d 454c 545f 504f 4f4c  EFAULT_MELT_POOL
+00016a70: 5f44 4550 5448 0a20 2020 2020 2020 2020  _DEPTH.         
+00016a80: 2020 2020 2020 2069 6620 2874 6573 745f         if (test_
+00016a90: 6d65 6c74 5f70 6f6f 6c5f 6465 7074 6820  melt_pool_depth 
+00016aa0: 6973 204e 6f6e 6520 6f72 206d 6174 682e  is None or math.
+00016ab0: 6973 6e61 6e28 7465 7374 5f6d 656c 745f  isnan(test_melt_
+00016ac0: 706f 6f6c 5f64 6570 7468 2929 0a20 2020  pool_depth)).   
+00016ad0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00016ae0: 6520 7465 7374 5f6d 656c 745f 706f 6f6c  e test_melt_pool
+00016af0: 5f64 6570 7468 2c0a 2020 2020 2020 2020  _depth,.        
+00016b00: 2020 2020 2020 2020 7261 6e64 6f6d 5f73          random_s
+00016b10: 6565 643d 7465 7374 5f72 616e 646f 6d5f  eed=test_random_
+00016b20: 7365 6564 2c0a 2020 2020 2020 2020 2020  seed,.          
+00016b30: 2020 2020 2020 6d61 6368 696e 653d 6d61        machine=ma
+00016b40: 6368 696e 652c 0a20 2020 2020 2020 2020  chine,.         
+00016b50: 2020 2020 2020 206d 6174 6572 6961 6c3d         material=
+00016b60: 6d61 7465 7269 616c 2c0a 2020 2020 2020  material,.      
+00016b70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00016b80: 2020 2020 7265 7475 726e 2028 5472 7565      return (True
+00016b90: 2c20 2222 290a 2020 2020 2020 2020 6578  , "").        ex
+00016ba0: 6365 7074 2056 616c 7565 4572 726f 7220  cept ValueError 
+00016bb0: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00016bc0: 2020 7265 7475 726e 2028 4661 6c73 652c    return (False,
+00016bd0: 2028 6622 496e 7661 6c69 6420 7061 7261   (f"Invalid para
+00016be0: 6d65 7465 7220 636f 6d62 696e 6174 696f  meter combinatio
+00016bf0: 6e3a 207b 657d 2229 290a                 n: {e}")).
```

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/parametric_study/parametric_utils.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/parametric_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/porosity.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/porosity.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/progress_logger.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/progress_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,62 +15,117 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-"""Provides logging and progress."""
+"""Provides progress updates."""
 
-import logging
+from abc import ABC, abstractmethod
+from enum import IntEnum
 from os import getenv
 
-from ansys.api.additive.v0.additive_domain_pb2 import Progress, ProgressState
+from ansys.api.additive.v0.additive_domain_pb2 import Progress as ProgressMsg
+from ansys.api.additive.v0.additive_domain_pb2 import ProgressState as ProgressMsgState
+from pydantic import BaseModel
 from tqdm import tqdm
 
 
-class ProgressLogger:
-    """Provides for logging and progress reporting."""
+class ProgressState(IntEnum):
+    """Simulation progress status."""
 
-    def __init__(self, name: str = None) -> None:
-        """Initialize a ``ProgressLogger`` object.
+    WAITING = ProgressMsgState.PROGRESS_STATE_WAITING
+    """Waiting for the simulation to start."""
+    RUNNING = ProgressMsgState.PROGRESS_STATE_EXECUTING
+    """Simulation is running."""
+    COMPLETED = ProgressMsgState.PROGRESS_STATE_COMPLETED
+    """Simulation has completed."""
+    ERROR = ProgressMsgState.PROGRESS_STATE_ERROR
+    """Simulation has errored."""
+
+
+class Progress(BaseModel):
+    """Progress information."""
+
+    sim_id: str
+    state: ProgressState
+    percent_complete: int
+    message: str
+    context: str
+
+    @classmethod
+    def from_proto_msg(cls, sim_id: str, progress: ProgressMsg):
+        """Create a ``Progress`` object from a progress protobuf message."""
+        return cls(
+            sim_id=sim_id,
+            state=ProgressState(progress.state),
+            percent_complete=progress.percent_complete,
+            message=progress.message,
+            context=progress.context,
+        )
+
+    def __str__(self):
+        return f"{self.id}: {self.state.name} - {self.percent_complete}% - {self.context} - {self.message}"
+
+
+class IProgressHandler(ABC):
+    """Interface for simulation progress updates."""
+
+    @abstractmethod
+    def update(self, progress: Progress):
+        """Update progress.
 
         Parameters
         ----------
-        name: str
-            Name of the logger.
+        progress : Progress
+            Progress information.
         """
-        self._log = logging.getLogger(name)
+        raise NotImplementedError
+
+
+class DefaultSingleSimulationProgressHandler(IProgressHandler):
+    """Creates a progress bar for a single simulation.
+
+    Parameters
+    ----------
+    sim_id : str
+        Simulation ID.
+    """
+
+    def __init__(self):
+        """Initialize progress handler."""
         self._last_percent_complete = 0
         self._last_context = "Initializing"
 
-    def log_progress(self, progress: Progress):
-        """Report progress and possibly emit a log message.
+    def update(self, progress: Progress):
+        """Update the progress bar.
 
         Parameters
         ----------
         progress: Progress
             Latest progress.
         """
+        # Don't send  progress when generating docs
         if getenv("GENERATING_DOCS"):
-            # Don't send  progress when generating docs
             return
+
+        # Skip SOLVERINFO messages
+        if progress.message and "SOLVERINFO" in progress.message:
+            return
+
         if not hasattr(self, "_pbar"):
             self._pbar = tqdm(
                 total=100,
                 colour="green",
                 desc=self._last_context,
                 dynamic_ncols=True,
             )
 
-        if progress.message and "SOLVERINFO" in progress.message:
-            self._log.debug(progress.message)
-            return
-
-        if progress.state == ProgressState.PROGRESS_STATE_ERROR:
+        if progress.state == ProgressState.ERROR:
             self._pbar.write(progress.message)
             return
 
         if progress.context and progress.context != self._last_context:
             if "Solving Layer" not in progress.context or progress.context == "Solving Layer 1":
                 self._pbar.reset(total=100)
                 self._pbar.set_description(progress.context)
```

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/server_connection/__init__.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/server_connection/constants.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/server_connection/local_server.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/local_server.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/server_connection/network_utils.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/network_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/server_connection/server_connection.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/server_connection.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/simulation.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/simulation.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/single_bead.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/single_bead.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/src/ansys/additive/core/thermal_history.py` & `ansys_additive_core-0.18.0b4/src/ansys/additive/core/thermal_history.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b3/PKG-INFO` & `ansys_additive_core-0.18.0b4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ansys-additive-core
-Version: 0.18.0b3
+Version: 0.18.0b4
 Summary: A Python client for the Ansys Additive service
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Manufacturing
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ansys-api-additive==1.6.7
+Requires-Dist: ansys-api-additive==1.7.2
 Requires-Dist: ansys-platform-instancemanagement>=1.1.1
 Requires-Dist: dill>=0.3.7
 Requires-Dist: google-api-python-client>=1.7.11
 Requires-Dist: googleapis-common-protos>=1.52.0
 Requires-Dist: grpcio>=1.35.0
 Requires-Dist: grpcio-health-checking>=1.45.0
 Requires-Dist: importlib-metadata>=4.0
@@ -27,50 +27,52 @@
 Requires-Dist: pandas>=1.3.2
 Requires-Dist: panel>=1.2.1
 Requires-Dist: platformdirs>=3.8.0
 Requires-Dist: plotly>=5.16.1
 Requires-Dist: protobuf>=3.20.2,<5
 Requires-Dist: six>=1.16.0
 Requires-Dist: tqdm>=4.45.0
-Requires-Dist: ansys-sphinx-theme==0.14.0 ; extra == "doc"
-Requires-Dist: enum-tools==0.11.0 ; extra == "doc"
+Requires-Dist: pydantic>=2.6.3
+Requires-Dist: ansys-sphinx-theme==0.15.2 ; extra == "doc"
+Requires-Dist: enum-tools==0.12.0 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.5.3 ; extra == "doc"
-Requires-Dist: matplotlib==3.8.3 ; extra == "doc"
-Requires-Dist: numpydoc==1.6.0 ; extra == "doc"
-Requires-Dist: panel==1.3.8 ; extra == "doc"
+Requires-Dist: matplotlib==3.8.4 ; extra == "doc"
+Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
+Requires-Dist: panel==1.4.2 ; extra == "doc"
 Requires-Dist: phantomjs==1.4.1 ; extra == "doc"
 Requires-Dist: pypandoc==1.13 ; extra == "doc"
-Requires-Dist: pyvista==0.43.3 ; extra == "doc"
-Requires-Dist: selenium==4.18.1 ; extra == "doc"
-Requires-Dist: sphinx==7.2.6 ; extra == "doc"
+Requires-Dist: pyvista==0.43.6 ; extra == "doc"
+Requires-Dist: selenium==4.20.0 ; extra == "doc"
+Requires-Dist: sphinx==7.3.7 ; extra == "doc"
 Requires-Dist: sphinx-autoapi==3.0.0 ; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints==2.0.0 ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints==2.1.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-design==0.5.0 ; extra == "doc"
-Requires-Dist: sphinx-gallery==0.15.0 ; extra == "doc"
+Requires-Dist: sphinx-gallery==0.16.0 ; extra == "doc"
 Requires-Dist: sphinx-jinja==2.0.2 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==1.0.0 ; extra == "doc"
 Requires-Dist: sphinx-toolbox==3.5.0 ; extra == "doc"
 Requires-Dist: sphinxemoji==0.3.1 ; extra == "doc"
 Requires-Dist: ansys-platform-instancemanagement==1.1.2 ; extra == "tests"
 Requires-Dist: dill==0.3.8 ; extra == "tests"
-Requires-Dist: google-api-python-client==2.120.0 ; extra == "tests"
-Requires-Dist: googleapis-common-protos==1.62.0 ; extra == "tests"
+Requires-Dist: google-api-python-client==2.122.0 ; extra == "tests"
+Requires-Dist: googleapis-common-protos==1.63.0 ; extra == "tests"
 Requires-Dist: grpcio==1.60.0 ; extra == "tests"
 Requires-Dist: grpcio-health-checking==1.48.2 ; extra == "tests"
 Requires-Dist: numpy==1.26.4 ; extra == "tests"
-Requires-Dist: pandas==2.2.1 ; extra == "tests"
-Requires-Dist: panel==1.3.8 ; extra == "tests"
-Requires-Dist: platformdirs==4.2.0 ; extra == "tests"
-Requires-Dist: plotly==5.19.0 ; extra == "tests"
+Requires-Dist: pandas==2.2.2 ; extra == "tests"
+Requires-Dist: panel==1.4.2 ; extra == "tests"
+Requires-Dist: platformdirs==4.2.1 ; extra == "tests"
+Requires-Dist: plotly==5.21.0 ; extra == "tests"
 Requires-Dist: protobuf==4.25.3 ; extra == "tests"
 Requires-Dist: six==1.16.0 ; extra == "tests"
 Requires-Dist: tqdm==4.66.2 ; extra == "tests"
-Requires-Dist: pytest==8.1.0 ; extra == "tests"
-Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
+Requires-Dist: pydantic==2.7.1 ; extra == "tests"
+Requires-Dist: pytest==8.2.0 ; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
 Project-URL: Discussions, https://github.com/ansys/pyadditive/discussions
 Project-URL: Documentation, https://additive.docs.pyansys.com
 Project-URL: Issues, https://github.com/ansys/pyadditive/issues
 Project-URL: Releases, https://github.com/ansys/pyadditive/releases
 Project-URL: Source, https://github.com/ansys/pyadditive
 Provides-Extra: doc
 Provides-Extra: tests
```

