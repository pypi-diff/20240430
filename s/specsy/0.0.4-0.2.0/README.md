# Comparing `tmp/specsy-0.0.4.tar.gz` & `tmp/specsy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/specsy-0.0.4.tar", last modified: Thu Sep 15 17:44:19 2022, max compression
+gzip compressed data, was "specsy-0.2.0.tar", last modified: Mon Apr 29 22:11:14 2024, max compression
```

## Comparing `specsy-0.0.4.tar` & `specsy-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,52 @@
-drwxrwxr-x   0 vital     (1001) vital     (1001)        0 2022-09-15 17:44:19.673838 specsy-0.0.4/
--rw-rw-r--   0 vital     (1001) vital     (1001)       17 2022-08-08 14:14:19.000000 specsy-0.0.4/MANIFEST.in
--rw-rw-r--   0 vital     (1001) vital     (1001)     1322 2022-09-15 17:44:19.673838 specsy-0.0.4/PKG-INFO
--rw-rw-r--   0 vital     (1001) vital     (1001)      866 2022-08-08 14:21:39.000000 specsy-0.0.4/README.rst
--rw-rw-r--   0 vital     (1001) vital     (1001)      444 2022-09-15 17:44:19.673838 specsy-0.0.4/setup.cfg
--rw-rw-r--   0 vital     (1001) vital     (1001)     1324 2022-09-15 02:00:42.000000 specsy-0.0.4/setup.py
-drwxrwxr-x   0 vital     (1001) vital     (1001)        0 2022-09-15 17:44:19.669838 specsy-0.0.4/src/
-drwxrwxr-x   0 vital     (1001) vital     (1001)        0 2022-09-15 17:44:19.673838 specsy-0.0.4/src/specsy/
--rw-rw-r--   0 vital     (1001) vital     (1001)      567 2022-09-07 23:31:25.000000 specsy-0.0.4/src/specsy/__init__.py
-drwxrwxr-x   0 vital     (1001) vital     (1001)        0 2022-09-15 17:44:19.673838 specsy-0.0.4/src/specsy/models/
--rw-rw-r--   0 vital     (1001) vital     (1001)        0 2022-08-08 14:46:35.000000 specsy-0.0.4/src/specsy/models/__init__.py
--rw-rw-r--   0 vital     (1001) vital     (1001)     4847 2022-09-15 16:28:07.000000 specsy-0.0.4/src/specsy/models/chemistry.py
--rw-rw-r--   0 vital     (1001) vital     (1001)    12334 2022-09-15 00:55:36.000000 specsy-0.0.4/src/specsy/models/extinction.py
--rw-rw-r--   0 vital     (1001) vital     (1001)     2447 2022-09-15 16:27:34.000000 specsy-0.0.4/src/specsy/plots.py
--rw-rw-r--   0 vital     (1001) vital     (1001)      712 2022-08-18 16:04:04.000000 specsy-0.0.4/src/specsy/tests.py
--rw-rw-r--   0 vital     (1001) vital     (1001)     2830 2022-09-08 03:27:46.000000 specsy-0.0.4/src/specsy/tools.py
--rw-rw-r--   0 vital     (1001) vital     (1001)       22 2022-08-08 14:57:14.000000 specsy-0.0.4/src/specsy/treatement.py
-drwxrwxr-x   0 vital     (1001) vital     (1001)        0 2022-09-15 17:44:19.673838 specsy-0.0.4/src/specsy.egg-info/
--rw-rw-r--   0 vital     (1001) vital     (1001)     1322 2022-09-15 17:44:19.000000 specsy-0.0.4/src/specsy.egg-info/PKG-INFO
--rw-rw-r--   0 vital     (1001) vital     (1001)      411 2022-09-15 17:44:19.000000 specsy-0.0.4/src/specsy.egg-info/SOURCES.txt
--rw-rw-r--   0 vital     (1001) vital     (1001)        1 2022-09-15 17:44:19.000000 specsy-0.0.4/src/specsy.egg-info/dependency_links.txt
--rw-rw-r--   0 vital     (1001) vital     (1001)       43 2022-09-15 17:44:19.000000 specsy-0.0.4/src/specsy.egg-info/requires.txt
--rw-rw-r--   0 vital     (1001) vital     (1001)        7 2022-09-15 17:44:19.000000 specsy-0.0.4/src/specsy.egg-info/top_level.txt
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.839356 specsy-0.2.0/
+-rw-rw-r--   0 vital     (1000) vital     (1000)       17 2024-04-29 21:50:58.000000 specsy-0.2.0/MANIFEST.in
+-rw-r--r--   0 vital     (1000) vital     (1000)     1883 2024-04-29 22:11:14.839356 specsy-0.2.0/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)      866 2024-04-29 21:50:58.000000 specsy-0.2.0/README.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1221 2024-04-29 21:50:58.000000 specsy-0.2.0/pyproject.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      431 2024-04-29 22:11:14.839356 specsy-0.2.0/setup.cfg
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1324 2024-04-29 21:50:58.000000 specsy-0.2.0/setup.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.835355 specsy-0.2.0/src/
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.835355 specsy-0.2.0/src/specsy/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      878 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)      759 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/core.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.835355 specsy-0.2.0/src/specsy/inference/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/inference/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    16792 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/inference/emission.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.835355 specsy-0.2.0/src/specsy/innate/
+-rw-rw-r--   0 vital     (1000) vital     (1000)       90 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/innate/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4246 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/innate/interpol_pytensor.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     3795 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/innate/main.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    12905 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/io.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.839356 specsy-0.2.0/src/specsy/models/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      243 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/models/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    16099 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/models/chemistry.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     5282 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/models/chemistry_inference.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17176 2024-04-29 21:57:45.000000 specsy-0.2.0/src/specsy/models/emissivity.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    22583 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/models/extinction.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/models/fluxes_line.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     8332 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/models/nebular_continuum.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.839356 specsy-0.2.0/src/specsy/operations/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/operations/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10732 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/operations/interpolation.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/operations/pytensors.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4631 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/operations/tensors.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1329 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/operations/tests.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    16155 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/plots.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.839356 specsy-0.2.0/src/specsy/resources/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      419 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/resources/Benjamin1999_OpticalDepthFunctionCoefficients.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    21375 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/resources/HI_t3_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)    44530 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/resources/HeII_t4_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)   326042 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/resources/HeI_t5_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)      451 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/resources/gordon_2003_LMC2_supershell.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      476 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/resources/gordon_2003_LMC_average.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      483 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/resources/gordon_2003_SMC_bar.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2887 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/tools.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10339 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/treatement.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.839356 specsy-0.2.0/src/specsy/workflow/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/workflow/__init__.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.835355 specsy-0.2.0/src/specsy.egg-info/
+-rw-r--r--   0 vital     (1000) vital     (1000)     1883 2024-04-29 22:11:14.000000 specsy-0.2.0/src/specsy.egg-info/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1287 2024-04-29 22:11:14.000000 specsy-0.2.0/src/specsy.egg-info/SOURCES.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-04-29 22:11:14.000000 specsy-0.2.0/src/specsy.egg-info/dependency_links.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      270 2024-04-29 22:11:14.000000 specsy-0.2.0/src/specsy.egg-info/requires.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        7 2024-04-29 22:11:14.000000 specsy-0.2.0/src/specsy.egg-info/top_level.txt
```

### Comparing `specsy-0.0.4/README.rst` & `specsy-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `specsy-0.0.4/setup.py` & `specsy-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `specsy-0.0.4/src/specsy/tools.py` & `specsy-0.2.0/src/specsy/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
 import numpy as np
 from scipy.stats import truncnorm, norm
+from lime.tools import extract_fluxes, normalize_fluxes
+
 # TODO some of these could go to lime
 
 _logger = logging.getLogger('SpecSy')
 
 # Percentile notation for uncertainty
 def percentile_latex_uncertainty(median, superscript, subscript, sig_fig=2):
     return r'${}^{{{}}}_{{{}}}$'.format(np.round(median, sig_fig), np.round(superscript, sig_fig), np.round(subscript, sig_fig))
```

