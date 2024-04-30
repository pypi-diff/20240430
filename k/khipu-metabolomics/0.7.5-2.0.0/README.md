# Comparing `tmp/khipu-metabolomics-0.7.5.tar.gz` & `tmp/khipu_metabolomics-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khipu-metabolomics-0.7.5.tar", last modified: Mon Oct  2 02:47:02 2023, max compression
+gzip compressed data, was "khipu_metabolomics-2.0.0.tar", last modified: Tue Apr 30 00:39:17 2024, max compression
```

## Comparing `khipu-metabolomics-0.7.5.tar` & `khipu_metabolomics-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 lish     (195676001) 1088672553        0 2023-10-02 02:47:02.273798 khipu-metabolomics-0.7.5/
--rw-r--r--   0 lish     (195676001) 1088672553      360 2023-09-29 14:47:06.000000 khipu-metabolomics-0.7.5/LICENSE
--rw-r--r--   0 lish     (195676001) 1088672553       38 2023-09-18 15:05:27.000000 khipu-metabolomics-0.7.5/MANIFEST.in
--rw-r--r--   0 lish     (195676001) 1088672553     8636 2023-10-02 02:47:02.273208 khipu-metabolomics-0.7.5/PKG-INFO
--rw-r--r--   0 lish     (195676001) 1088672553     7722 2023-09-29 14:47:06.000000 khipu-metabolomics-0.7.5/README.md
-drwxr-xr-x   0 lish     (195676001) 1088672553        0 2023-10-02 02:47:02.267746 khipu-metabolomics-0.7.5/khipu/
--rw-r--r--   0 lish     (195676001) 1088672553       22 2023-10-02 02:43:38.000000 khipu-metabolomics-0.7.5/khipu/__init__.py
--rw-r--r--   0 lish     (195676001) 1088672553       24 2023-09-29 14:47:06.000000 khipu-metabolomics-0.7.5/khipu/command_line.py
--rw-r--r--   0 lish     (195676001) 1088672553     3913 2023-09-29 14:47:06.000000 khipu-metabolomics-0.7.5/khipu/epdsConstructor.py
--rw-r--r--   0 lish     (195676001) 1088672553    13705 2023-09-29 14:47:06.000000 khipu-metabolomics-0.7.5/khipu/extended.py
--rw-r--r--   0 lish     (195676001) 1088672553     5531 2023-10-02 02:43:08.000000 khipu-metabolomics-0.7.5/khipu/formula_filter.py
--rw-r--r--   0 lish     (195676001) 1088672553     1474 2023-09-29 14:47:06.000000 khipu-metabolomics-0.7.5/khipu/main.py
--rw-r--r--   0 lish     (195676001) 1088672553    30719 2023-09-29 14:47:06.000000 khipu-metabolomics-0.7.5/khipu/model.py
--rw-r--r--   0 lish     (195676001) 1088672553     3383 2023-09-29 15:48:17.000000 khipu-metabolomics-0.7.5/khipu/plot.py
--rw-r--r--   0 lish     (195676001) 1088672553     4360 2023-09-29 14:47:06.000000 khipu-metabolomics-0.7.5/khipu/test.py
--rw-r--r--   0 lish     (195676001) 1088672553  7428142 2023-10-02 02:04:57.000000 khipu-metabolomics-0.7.5/khipu/tree_formulas.py
--rw-r--r--   0 lish     (195676001) 1088672553    22536 2023-09-29 14:47:06.000000 khipu-metabolomics-0.7.5/khipu/utils.py
-drwxr-xr-x   0 lish     (195676001) 1088672553        0 2023-10-02 02:47:02.272643 khipu-metabolomics-0.7.5/khipu_metabolomics.egg-info/
--rw-r--r--   0 lish     (195676001) 1088672553     8636 2023-10-02 02:47:02.000000 khipu-metabolomics-0.7.5/khipu_metabolomics.egg-info/PKG-INFO
--rw-r--r--   0 lish     (195676001) 1088672553      511 2023-10-02 02:47:02.000000 khipu-metabolomics-0.7.5/khipu_metabolomics.egg-info/SOURCES.txt
--rw-r--r--   0 lish     (195676001) 1088672553        1 2023-10-02 02:47:02.000000 khipu-metabolomics-0.7.5/khipu_metabolomics.egg-info/dependency_links.txt
--rw-r--r--   0 lish     (195676001) 1088672553       50 2023-10-02 02:47:02.000000 khipu-metabolomics-0.7.5/khipu_metabolomics.egg-info/entry_points.txt
--rw-r--r--   0 lish     (195676001) 1088672553       27 2023-10-02 02:47:02.000000 khipu-metabolomics-0.7.5/khipu_metabolomics.egg-info/requires.txt
--rw-r--r--   0 lish     (195676001) 1088672553        6 2023-10-02 02:47:02.000000 khipu-metabolomics-0.7.5/khipu_metabolomics.egg-info/top_level.txt
--rw-r--r--   0 lish     (195676001) 1088672553       67 2023-09-29 14:47:06.000000 khipu-metabolomics-0.7.5/requirements.txt
--rw-r--r--   0 lish     (195676001) 1088672553       38 2023-10-02 02:47:02.273842 khipu-metabolomics-0.7.5/setup.cfg
--rw-r--r--   0 lish     (195676001) 1088672553     1412 2023-09-29 14:47:06.000000 khipu-metabolomics-0.7.5/setup.py
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-30 00:39:17.481614 khipu_metabolomics-2.0.0/
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)      360 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.0/LICENSE
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       38 2023-09-18 15:05:27.000000 khipu_metabolomics-2.0.0/MANIFEST.in
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     9717 2024-04-30 00:39:17.480933 khipu_metabolomics-2.0.0/PKG-INFO
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     8803 2024-04-30 00:36:50.000000 khipu_metabolomics-2.0.0/README.md
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-30 00:39:17.463256 khipu_metabolomics-2.0.0/khipu/
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       68 2024-04-30 00:31:29.000000 khipu_metabolomics-2.0.0/khipu/__init__.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    18736 2024-04-30 00:21:47.000000 khipu_metabolomics-2.0.0/khipu/analysis.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       24 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.0/khipu/command_line.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     3913 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.0/khipu/epdsConstructor.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    13754 2024-04-25 13:06:56.000000 khipu_metabolomics-2.0.0/khipu/extended.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     5531 2023-10-02 02:43:08.000000 khipu_metabolomics-2.0.0/khipu/formula_filter.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    11636 2024-04-30 00:21:47.000000 khipu_metabolomics-2.0.0/khipu/isotopes.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     1607 2024-04-25 13:06:56.000000 khipu_metabolomics-2.0.0/khipu/main.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    30719 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.0/khipu/model.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     3383 2023-09-29 15:48:17.000000 khipu_metabolomics-2.0.0/khipu/plot.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     4360 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.0/khipu/test.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)  7428142 2023-10-02 02:04:57.000000 khipu_metabolomics-2.0.0/khipu/tree_formulas.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    24528 2024-04-25 13:06:56.000000 khipu_metabolomics-2.0.0/khipu/utils.py
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-30 00:39:17.480309 khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     9717 2024-04-30 00:39:17.000000 khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/PKG-INFO
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)      547 2024-04-30 00:39:17.000000 khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/SOURCES.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        1 2024-04-30 00:39:17.000000 khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/dependency_links.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       50 2024-04-30 00:39:17.000000 khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/entry_points.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       27 2024-04-30 00:39:17.000000 khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/requires.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        6 2024-04-30 00:39:17.000000 khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/top_level.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       67 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.0/requirements.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       38 2024-04-30 00:39:17.481685 khipu_metabolomics-2.0.0/setup.cfg
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     1412 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.0/setup.py
```

### Comparing `khipu-metabolomics-0.7.5/PKG-INFO` & `khipu_metabolomics-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khipu-metabolomics
-Version: 0.7.5
+Version: 2.0.0
 Summary: Common utilities for interpreting mass spectrometry data
 Home-page: https://github.com/shuzhao-li/khipu
 Author: Shuzhao Li
 Author-email: shuzhao.li@gmail.com
 License: BSD
 Keywords: chemistry,bioinformatics,mass spectrometry
 Classifier: Development Status :: 4 - Beta
@@ -25,17 +25,17 @@
 
 # khipu: generalized tree structure to annotate untargeted metabolomics and stable isotope tracing data
 
 [![Documentation Status](https://readthedocs.org/projects/khipu/badge/?version=latest)](https://khipu.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://img.shields.io/badge/DOI-doi%2F10.1021%2Facs.analchem.2c05810-blue)](https://pubs.acs.org/doi/10.1021/acs.analchem.2c05810)
 
 
-Pre-annotation tool to annotate degenerate ions in relationships to the original compound and infer neutral mass. 
+Pre-annotation tool to annotate degenerate ions in relationships to the original compound and infer neutral mass. The initial version was described in [Li and Zheng (2023). Analytical chemistry, 95(15), pp.6212-6217](https://pubs.acs.org/doi/10.1021/acs.analchem.2c05810).
 
-This applies to regular LC-MS data, but also enables easy analysis of isotope tracing and chemical labeling data.
+This applies to regular LC-MS data, but also enables easy analysis of isotope tracing and chemical labeling data. Different applications may require different parameters. A web server for isotope tracing data is now available at https://metabolomics.cloud/khipu.
 
 ![khipugram](doc/khipugram.png)
 
 ## Implementation overview
 Khipu is developed as an open source Python 3 package, and available to install from the standard PyPi repository via the pip tool. It is freely available on GitHub (https://github.com/shuzhao-li/khipu) under a BSD 3-Clause License. The graph operations are supported by the networkx library, tree visualization aided by the treelib library. Khipu uses our package mass2chem for search functions. The data model of “empirical compound” is described in the metDataModel package. The package is designed in a modular way to encourage reuse.
 
 The classes of Weavor and Khipu contain main algorithms, supported by numerous utility functions. All functions are documented in the source via docstrings. Examples of reuse are given in wrapper functions and in Jupyter notebooks. It can be run as a standalone command line tool. Users can use a feature table from any preprocessing tool as input and get annotated empirical compounds in JSON and tab delimited formats.
@@ -153,7 +153,17 @@
 
 
 ## What's "khipu"?
 Khipu is a recording device using knots, often 2-level of strings,
 historically used by people in Andean South America, includign Inca (https://en.wikipedia.org/wiki/Quipu).
 The format is similar to how we represent isotopes and adducts in our data.
 We chose "khipu" over the spelling of "quipu", to pay respect to the indigenous people.
+
+## Khipu is part of The Asari Project.
+
+- asari (Source code: https://github.com/shuzhao-li/asari, Package Repository: https://pypi.org/project/asari-metabolomics/)
+- metDataModel: data models for metabolomics (https://github.com/shuzhao-li-lab/metDataModel)
+- mass2chem: common utilities in interpreting mass spectrometry data, annotation (https://github.com/shuzhao-li-lab/mass2chem)
+- khipu: a Python library for generalized, low-level annotation of MS metabolomics (https://github.com/shuzhao-li-lab/khipu)
+- JMS: Json's Metabolite Services. Search functions, annotation and metabolic models (https://github.com/shuzhao-li-lab/JMS)
+- pcpfm pipeline (https://github.com/shuzhao-li-lab/PythonCentricPipelineForMetabolomics)
+- asari-x: the eXposome miner (to be released)
```

### Comparing `khipu-metabolomics-0.7.5/README.md` & `khipu_metabolomics-2.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # khipu: generalized tree structure to annotate untargeted metabolomics and stable isotope tracing data
 
 [![Documentation Status](https://readthedocs.org/projects/khipu/badge/?version=latest)](https://khipu.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://img.shields.io/badge/DOI-doi%2F10.1021%2Facs.analchem.2c05810-blue)](https://pubs.acs.org/doi/10.1021/acs.analchem.2c05810)
 
 
-Pre-annotation tool to annotate degenerate ions in relationships to the original compound and infer neutral mass. 
+Pre-annotation tool to annotate degenerate ions in relationships to the original compound and infer neutral mass. The initial version was described in [Li and Zheng (2023). Analytical chemistry, 95(15), pp.6212-6217](https://pubs.acs.org/doi/10.1021/acs.analchem.2c05810).
 
-This applies to regular LC-MS data, but also enables easy analysis of isotope tracing and chemical labeling data.
+This applies to regular LC-MS data, but also enables easy analysis of isotope tracing and chemical labeling data. Different applications may require different parameters. A web server for isotope tracing data is now available at https://metabolomics.cloud/khipu.
 
 ![khipugram](doc/khipugram.png)
 
 ## Implementation overview
 Khipu is developed as an open source Python 3 package, and available to install from the standard PyPi repository via the pip tool. It is freely available on GitHub (https://github.com/shuzhao-li/khipu) under a BSD 3-Clause License. The graph operations are supported by the networkx library, tree visualization aided by the treelib library. Khipu uses our package mass2chem for search functions. The data model of “empirical compound” is described in the metDataModel package. The package is designed in a modular way to encourage reuse.
 
 The classes of Weavor and Khipu contain main algorithms, supported by numerous utility functions. All functions are documented in the source via docstrings. Examples of reuse are given in wrapper functions and in Jupyter notebooks. It can be run as a standalone command line tool. Users can use a feature table from any preprocessing tool as input and get annotated empirical compounds in JSON and tab delimited formats.
@@ -128,7 +128,17 @@
 
 
 ## What's "khipu"?
 Khipu is a recording device using knots, often 2-level of strings,
 historically used by people in Andean South America, includign Inca (https://en.wikipedia.org/wiki/Quipu).
 The format is similar to how we represent isotopes and adducts in our data.
 We chose "khipu" over the spelling of "quipu", to pay respect to the indigenous people.
+
+## Khipu is part of The Asari Project.
+
+- asari (Source code: https://github.com/shuzhao-li/asari, Package Repository: https://pypi.org/project/asari-metabolomics/)
+- metDataModel: data models for metabolomics (https://github.com/shuzhao-li-lab/metDataModel)
+- mass2chem: common utilities in interpreting mass spectrometry data, annotation (https://github.com/shuzhao-li-lab/mass2chem)
+- khipu: a Python library for generalized, low-level annotation of MS metabolomics (https://github.com/shuzhao-li-lab/khipu)
+- JMS: Json's Metabolite Services. Search functions, annotation and metabolic models (https://github.com/shuzhao-li-lab/JMS)
+- pcpfm pipeline (https://github.com/shuzhao-li-lab/PythonCentricPipelineForMetabolomics)
+- asari-x: the eXposome miner (to be released)
```

### Comparing `khipu-metabolomics-0.7.5/khipu/epdsConstructor.py` & `khipu_metabolomics-2.0.0/khipu/epdsConstructor.py`

 * *Files identical despite different names*

### Comparing `khipu-metabolomics-0.7.5/khipu/extended.py` & `khipu_metabolomics-2.0.0/khipu/extended.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         adduct_patterns = adduct_search_patterns_neg
         delta_mz = -PROTON
         singleton_ion = 'M-H-'
 
     peaklist = local_read_file(infile=args.input, start_col=args.start, end_col=args.end)
     peak_dict = make_peak_dict(peaklist)
     khipu_list, all_assigned_peaks = peaklist_to_khipu_list(peaklist, 
-                    isotope_search_patterns=isotope_search_patterns, 
+                    isotope_search_patterns=isotope_search_patterns[:3] if args.regular else isotope_search_patterns, 
                     adduct_search_patterns=adduct_patterns,
                     extended_adducts=extended_adducts,
                     mz_tolerance_ppm=args.ppm,
                     rt_tolerance=args.rtol,
                     mode=args.mode,
                     charges=[1, 2, 3],
                     )
```

### Comparing `khipu-metabolomics-0.7.5/khipu/formula_filter.py` & `khipu_metabolomics-2.0.0/khipu/formula_filter.py`

 * *Files identical despite different names*

### Comparing `khipu-metabolomics-0.7.5/khipu/main.py` & `khipu_metabolomics-2.0.0/khipu/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
             help='input file as feature table')
     parser.add_argument('-s', '--start',  default=3, type=int,
             help='start column for intensity in input table')
     parser.add_argument('-e', '--end',  default=6, type=int,
             help='end column for intensity in input table')
     parser.add_argument('-o', '--output', 
             help='prefix of output files')
+    parser.add_argument('-r', '--regular', action='store_true',
+            help='toggle on if there is no isotopic labeled sample')
 
     args = parser.parse_args()
     khipu_annotate(args)
 
 
 #
 # -----------------------------------------------------------------------------
```

### Comparing `khipu-metabolomics-0.7.5/khipu/model.py` & `khipu_metabolomics-2.0.0/khipu/model.py`

 * *Files identical despite different names*

### Comparing `khipu-metabolomics-0.7.5/khipu/plot.py` & `khipu_metabolomics-2.0.0/khipu/plot.py`

 * *Files identical despite different names*

### Comparing `khipu-metabolomics-0.7.5/khipu/test.py` & `khipu_metabolomics-2.0.0/khipu/test.py`

 * *Files identical despite different names*

### Comparing `khipu-metabolomics-0.7.5/khipu/tree_formulas.py` & `khipu_metabolomics-2.0.0/khipu/tree_formulas.py`

 * *Files identical despite different names*

### Comparing `khipu-metabolomics-0.7.5/khipu/utils.py` & `khipu_metabolomics-2.0.0/khipu/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 '''
 Utility functions and m/z patterns.
 Adduct rules can be still better learned in the future.
 '''
 import json
 import numpy as np
 import networkx as nx
+import pandas as pd
 from mass2chem.search import build_centurion_tree, find_all_matches_centurion_indexed_list
+from mass2chem.formula import parse_chemformula_dict_comprehensive
 
 import logging
 logging.basicConfig(filename='khipu.log', level=logging.INFO)   #  encoding='utf-8',
 
 #
 # m/z differences corresponding to adducts and isotopes
 # Not using charge in tables, because all m/z diff is relative to other charged ions
 #
 PROTON = 1.00727646677
 electron = 0.000549
 
 # These are single-charged values. 
 # Double and Tripple charged ions are computed after the initial round, on the fly
 # avoid confusing adducts in initial search, e.g. H, H2O
+
+
+
 adduct_search_patterns = [  # initial patterns are relative to M+H+
                             (21.9820, 'Na/H'),
                             (41.026549, 'ACN'),     # Acetonitrile
                             (35.9767, 'HCl'),
                             (37.955882, 'K/H'),
                             ]
 
@@ -66,14 +71,42 @@
                             (-46.00548, '-CO2H2'),
                             (67.987424, 'NaCOOH'),
                             (83.961361, 'KCOOH'),
                             (97.96737927, 'H2SO4'),
                             (97.97689507, 'H3PO4'),
 ]
 
+ADDUCT_TO_FORMULA_DELTAS = {}
+for search_pattern in [*adduct_search_patterns, *adduct_search_patterns_neg, *extended_adducts]:
+    _, formula_offset = search_pattern
+    formula_offset = formula_offset.replace("ACN", "(C2H3N)")
+    formula_offset = formula_offset.replace("Me", "(CH3)")
+    if "/" in formula_offset:
+        gain, loss = formula_offset.split("/")
+    else:
+        gain, loss = formula_offset, None
+    if gain.startswith("-"):
+        if loss is None:
+            gain, loss = None, gain[1:]
+    if gain:
+        g_fdict = parse_chemformula_dict_comprehensive(gain)
+    else:
+        g_fdict = {}
+    if loss:
+        l_fdict = parse_chemformula_dict_comprehensive(loss)
+    else:
+        l_fdict = {}
+    net_fdict = {}
+    for key in set(list(g_fdict.keys()) + list(l_fdict.keys())):
+        net_fdict[key] = g_fdict.get(key, 0) - l_fdict.get(key, 0)
+    ADDUCT_TO_FORMULA_DELTAS[search_pattern[1]] = (g_fdict, l_fdict, net_fdict)
+ADDUCT_TO_FORMULA_DELTAS["M+H+"] = ({"H": 1}, {}, {"H": 1})
+ADDUCT_TO_FORMULA_DELTAS["M-H-"] = ({}, {"H": 1}, {"H": -1})
+
+
 relabel_dict = {
     'M+H+,Na/H': 'M+Na+',
     'M+H+,HCl': 'M+HCl+H+',
     'M+H+,K/H': 'M+K+',
     'M+H+,ACN': 'M+ACN+H+',
     'M+H+,NH3': 'M+NH4+',
     'M+H+,M+H+,Na2/H2': 'M-H+Na+Na+',
@@ -105,14 +138,31 @@
         A0 = compute_multichaged_patterns([(PROTON, 'M+H+')], charge)
         return A0 + [(x[0] + PROTON, x[1]) for x in pattern] 
     else:
         # neg base ion as M-H[-]
         A0 = compute_multichaged_patterns([(-PROTON, 'M-H-')], charge)
         return A0 + [(x[0] - PROTON, x[1]) for x in pattern]
 
+def khipu_list_to_ftable(khipu_list, field="MS1_pseudo_Spectra"):
+    ftable = []
+    for khipu in khipu_list:
+        if field == "MS1_pseudo_Spectra":
+            for peak in khipu["MS1_pseudo_Spectra"]:
+                ftable.append(peak)
+        if field == "isocor_results":
+            for formula in khipu["isocor_results"]:
+                for peak in khipu["isocor_results"][formula]:
+                    new_peak = {
+                        "formula_for_correction": formula,
+                        "adduct_for_correction": peak['modification']
+                    }
+                    for k, v in peak.items():
+                        new_peak[k] = v
+                    ftable.append(new_peak)  
+    return pd.DataFrame(ftable)               
 
 def read_features_from_text(text_table, 
                         id_col=0, mz_col=1, rtime_col=2, 
                         intensity_cols=(3, 6), delimiter="\t"):
     '''
     Read a text feature table into a list of features.
     
@@ -150,19 +200,19 @@
         if featureLines[ii].strip():
             a = featureLines[ii].split(delimiter)
             if isinstance(id_col, int):         # feature id specified
                 iid = a[id_col]
             else:
                 iid = 'row'+str(ii)
             xstart, xend = intensity_cols
-            intensities = [float(x) for x in a[xstart: xend]]
+            intensities = {x[0]:float(x[1]) for x in zip(header[xstart: xend], a[xstart: xend])}
             L.append({
                 'id': iid, 'mz': float(a[mz_col]), 'rtime': float(a[rtime_col]),
                 'intensities': intensities,
-                'representative_intensity': np.mean(intensities),
+                'representative_intensity': np.mean([float(value) for value in intensities.values()])
             })
     return L
 
 def make_peak_tag(peak):
     '''
     peak format: {'id': 'F1', 'mz': 60.0808, 'rtime': 117.7, ...,
     'intensities': [250346.0], 'representative_intensity': 250346.0}
```

### Comparing `khipu-metabolomics-0.7.5/khipu_metabolomics.egg-info/PKG-INFO` & `khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khipu-metabolomics
-Version: 0.7.5
+Version: 2.0.0
 Summary: Common utilities for interpreting mass spectrometry data
 Home-page: https://github.com/shuzhao-li/khipu
 Author: Shuzhao Li
 Author-email: shuzhao.li@gmail.com
 License: BSD
 Keywords: chemistry,bioinformatics,mass spectrometry
 Classifier: Development Status :: 4 - Beta
@@ -25,17 +25,17 @@
 
 # khipu: generalized tree structure to annotate untargeted metabolomics and stable isotope tracing data
 
 [![Documentation Status](https://readthedocs.org/projects/khipu/badge/?version=latest)](https://khipu.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://img.shields.io/badge/DOI-doi%2F10.1021%2Facs.analchem.2c05810-blue)](https://pubs.acs.org/doi/10.1021/acs.analchem.2c05810)
 
 
-Pre-annotation tool to annotate degenerate ions in relationships to the original compound and infer neutral mass. 
+Pre-annotation tool to annotate degenerate ions in relationships to the original compound and infer neutral mass. The initial version was described in [Li and Zheng (2023). Analytical chemistry, 95(15), pp.6212-6217](https://pubs.acs.org/doi/10.1021/acs.analchem.2c05810).
 
-This applies to regular LC-MS data, but also enables easy analysis of isotope tracing and chemical labeling data.
+This applies to regular LC-MS data, but also enables easy analysis of isotope tracing and chemical labeling data. Different applications may require different parameters. A web server for isotope tracing data is now available at https://metabolomics.cloud/khipu.
 
 ![khipugram](doc/khipugram.png)
 
 ## Implementation overview
 Khipu is developed as an open source Python 3 package, and available to install from the standard PyPi repository via the pip tool. It is freely available on GitHub (https://github.com/shuzhao-li/khipu) under a BSD 3-Clause License. The graph operations are supported by the networkx library, tree visualization aided by the treelib library. Khipu uses our package mass2chem for search functions. The data model of “empirical compound” is described in the metDataModel package. The package is designed in a modular way to encourage reuse.
 
 The classes of Weavor and Khipu contain main algorithms, supported by numerous utility functions. All functions are documented in the source via docstrings. Examples of reuse are given in wrapper functions and in Jupyter notebooks. It can be run as a standalone command line tool. Users can use a feature table from any preprocessing tool as input and get annotated empirical compounds in JSON and tab delimited formats.
@@ -153,7 +153,17 @@
 
 
 ## What's "khipu"?
 Khipu is a recording device using knots, often 2-level of strings,
 historically used by people in Andean South America, includign Inca (https://en.wikipedia.org/wiki/Quipu).
 The format is similar to how we represent isotopes and adducts in our data.
 We chose "khipu" over the spelling of "quipu", to pay respect to the indigenous people.
+
+## Khipu is part of The Asari Project.
+
+- asari (Source code: https://github.com/shuzhao-li/asari, Package Repository: https://pypi.org/project/asari-metabolomics/)
+- metDataModel: data models for metabolomics (https://github.com/shuzhao-li-lab/metDataModel)
+- mass2chem: common utilities in interpreting mass spectrometry data, annotation (https://github.com/shuzhao-li-lab/mass2chem)
+- khipu: a Python library for generalized, low-level annotation of MS metabolomics (https://github.com/shuzhao-li-lab/khipu)
+- JMS: Json's Metabolite Services. Search functions, annotation and metabolic models (https://github.com/shuzhao-li-lab/JMS)
+- pcpfm pipeline (https://github.com/shuzhao-li-lab/PythonCentricPipelineForMetabolomics)
+- asari-x: the eXposome miner (to be released)
```

### Comparing `khipu-metabolomics-0.7.5/setup.py` & `khipu_metabolomics-2.0.0/setup.py`

 * *Files identical despite different names*

