# Comparing `tmp/gemsembler-0.6.4.tar.gz` & `tmp/gemsembler-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemsembler-0.6.4.tar", last modified: Wed Apr 17 14:50:27 2024, max compression
+gzip compressed data, was "gemsembler-0.6.5.tar", last modified: Tue Apr 30 11:34:24 2024, max compression
```

## Comparing `gemsembler-0.6.4.tar` & `gemsembler-0.6.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.782412 gemsembler-0.6.4/
--rw-rw-rw-   0 root         (0) root         (0)     1083 2024-04-17 14:50:14.000000 gemsembler-0.6.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-17 14:50:14.000000 gemsembler-0.6.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4287 2024-04-17 14:50:27.782412 gemsembler-0.6.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-04-17 14:50:14.000000 gemsembler-0.6.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-17 14:50:14.000000 gemsembler-0.6.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 14:50:27.782412 gemsembler-0.6.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.772412 gemsembler-0.6.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.775412 gemsembler-0.6.4/src/gemsembler/
--rw-rw-rw-   0 root         (0) root         (0)     1785 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     7898 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/anticreation.py
--rw-rw-rw-   0 root         (0) root         (0)    19906 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/comparison.py
--rw-rw-rw-   0 root         (0) root         (0)    14845 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)    52270 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/creation.py
--rw-rw-rw-   0 root         (0) root         (0)     4300 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/curation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.776412 gemsembler-0.6.4/src/gemsembler/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.778412 gemsembler-0.6.4/src/gemsembler/data/BU/
--rw-rw-rw-   0 root         (0) root         (0)   180894 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/BU/BU_agora.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   303843 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/BU/BU_carveme_hom.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   381510 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/BU/BU_gapseq.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)    83221 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/BU/BU_modelSEED.sbml.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/BU/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.781412 gemsembler-0.6.4/src/gemsembler/data/LP/
--rw-rw-rw-   0 root         (0) root         (0)   153653 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/LP_CA1.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   157673 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/LP_CA2.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)    82710 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/LP_MS2.sbml.gz
--rw-rw-rw-   0 root         (0) root         (0)   885760 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/LP_WCFS1.fasta.gz
--rw-rw-rw-   0 root         (0) root         (0)   151435 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   124883 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   547669 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/LP_protein_fasta.faa.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10388 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/dbs.py
--rw-rw-rw-   0 root         (0) root         (0)    19185 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/downstream.py
--rw-rw-rw-   0 root         (0) root         (0)    35714 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/drawing.py
--rw-rw-rw-   0 root         (0) root         (0)    24476 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/gathering.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/general.py
--rw-rw-rw-   0 root         (0) root         (0)    13452 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/genes.py
--rw-rw-rw-   0 root         (0) root         (0)    22859 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/pathsfinding.py
--rw-rw-rw-   0 root         (0) root         (0)     4557 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/periplasmic.py
--rw-rw-rw-   0 root         (0) root         (0)    10165 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/selection.py
--rw-rw-rw-   0 root         (0) root         (0)    31443 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/structural.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.782412 gemsembler-0.6.4/src/gemsembler.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4287 2024-04-17 14:50:27.000000 gemsembler-0.6.4/src/gemsembler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1435 2024-04-17 14:50:27.000000 gemsembler-0.6.4/src/gemsembler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 14:50:27.000000 gemsembler-0.6.4/src/gemsembler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-17 14:50:27.000000 gemsembler-0.6.4/src/gemsembler.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      121 2024-04-17 14:50:27.000000 gemsembler-0.6.4/src/gemsembler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-17 14:50:27.000000 gemsembler-0.6.4/src/gemsembler.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.782412 gemsembler-0.6.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)    12691 2024-04-17 14:50:14.000000 gemsembler-0.6.4/tests/test_conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-17 14:50:14.000000 gemsembler-0.6.4/tests/test_curation.py
--rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-17 14:50:14.000000 gemsembler-0.6.4/tests/test_dbs.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2024-04-17 14:50:14.000000 gemsembler-0.6.4/tests/test_gathering.py
--rw-rw-rw-   0 root         (0) root         (0)     2357 2024-04-17 14:50:14.000000 gemsembler-0.6.4/tests/test_selection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.572217 gemsembler-0.6.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2024-04-30 11:34:12.000000 gemsembler-0.6.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-30 11:34:12.000000 gemsembler-0.6.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5466 2024-04-30 11:34:24.572217 gemsembler-0.6.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2024-04-30 11:34:12.000000 gemsembler-0.6.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-30 11:34:12.000000 gemsembler-0.6.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 11:34:24.572217 gemsembler-0.6.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.561216 gemsembler-0.6.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.565216 gemsembler-0.6.5/src/gemsembler/
+-rw-rw-rw-   0 root         (0) root         (0)     1823 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7949 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/anticreation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19906 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/comparison.py
+-rw-rw-rw-   0 root         (0) root         (0)    14845 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)    52270 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/creation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4300 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/curation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.566216 gemsembler-0.6.5/src/gemsembler/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.567216 gemsembler-0.6.5/src/gemsembler/data/BU/
+-rw-rw-rw-   0 root         (0) root         (0)   180894 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/BU/BU_agora.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   303843 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/BU/BU_carveme_hom.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   381510 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/BU/BU_gapseq.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)    83221 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/BU/BU_modelSEED.sbml.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/BU/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.571216 gemsembler-0.6.5/src/gemsembler/data/LP/
+-rw-rw-rw-   0 root         (0) root         (0)   153653 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/LP_CA1.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   157673 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/LP_CA2.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)    82710 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/LP_MS2.sbml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   885760 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/LP_WCFS1.fasta.gz
+-rw-rw-rw-   0 root         (0) root         (0)   151435 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   124883 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   547669 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/LP_protein_fasta.faa.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10388 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/dbs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18938 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/downstream.py
+-rw-rw-rw-   0 root         (0) root         (0)    34325 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/drawing.py
+-rw-rw-rw-   0 root         (0) root         (0)    24547 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/gathering.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/general.py
+-rw-rw-rw-   0 root         (0) root         (0)    13452 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/genes.py
+-rw-rw-rw-   0 root         (0) root         (0)    22859 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/pathsfinding.py
+-rw-rw-rw-   0 root         (0) root         (0)     4557 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/periplasmic.py
+-rw-rw-rw-   0 root         (0) root         (0)    10165 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/selection.py
+-rw-rw-rw-   0 root         (0) root         (0)    31443 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/structural.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.571216 gemsembler-0.6.5/src/gemsembler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5466 2024-04-30 11:34:24.000000 gemsembler-0.6.5/src/gemsembler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1435 2024-04-30 11:34:24.000000 gemsembler-0.6.5/src/gemsembler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 11:34:24.000000 gemsembler-0.6.5/src/gemsembler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-30 11:34:24.000000 gemsembler-0.6.5/src/gemsembler.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-30 11:34:24.000000 gemsembler-0.6.5/src/gemsembler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-30 11:34:24.000000 gemsembler-0.6.5/src/gemsembler.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.571216 gemsembler-0.6.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    12691 2024-04-30 11:34:12.000000 gemsembler-0.6.5/tests/test_conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-30 11:34:12.000000 gemsembler-0.6.5/tests/test_curation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-30 11:34:12.000000 gemsembler-0.6.5/tests/test_dbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2024-04-30 11:34:12.000000 gemsembler-0.6.5/tests/test_gathering.py
+-rw-rw-rw-   0 root         (0) root         (0)     2357 2024-04-30 11:34:12.000000 gemsembler-0.6.5/tests/test_selection.py
```

### Comparing `gemsembler-0.6.4/LICENSE` & `gemsembler-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/PKG-INFO` & `gemsembler-0.6.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemsembler
-Version: 0.6.4
+Version: 0.6.5
 Summary: A tool for assembling and comparing several types of Genome-Scale Metabolic Models.
 Author-email: Elena Matveishina <elena.matveishina@embl.de>, Bartosz Bartmanski <bartosz.bartmanski@embl.de>
 License: MIT License
         
         Copyright (c) 2024 Zimmermann-Kogadeeva Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,14 +49,16 @@
 Requires-Dist: pyvis
 Requires-Dist: h5py
 Requires-Dist: platformdirs
 Requires-Dist: pyyaml
 
 # GEMsembler
 
+<img src="gemsembler_long.gif" alt="drawing" width="150"/>
+
 GEMsembler tool for assembling and comparing several types of Genome-Scale Metabolic
 Models. 
 
 **THIS IS A BETA VERSION! BUGS CAN BE EXPECTED**
 
 ## Installation
 
@@ -74,14 +76,50 @@
 (modelseed), gapseq (gapseq) and models downloaded from AGORA VMH database
 (agora) are supported. Custom type is coming soon. Genomes, from which the
 models are built will allow to convert and assemble genes as well.
 First, we import gemsembler and get the path to data files:
 ```
 from gemsembler import GatheredModels, lp_example, get_model_of_interest
 ```
+lp_example is a list with input models and related inforamtion such as model type, corresponding genome and so on.
+```
+lp_example = [
+    dict(
+        model_id="curated_LP",
+        path_to_model=files(LP) / "LP_iLP728_revision_data_met_C_c.xml.gz",
+        model_type="carveme",
+        path_to_genome=files(LP) / "LP_protein_fasta.faa.gz",
+    ),
+    dict(
+        model_id="cauniv_LP",
+        path_to_model=files(LP) / "LP_CA1.xml.gz",
+        model_type="carveme",
+        path_to_genome=files(LP) / "LP_protein_fasta.faa.gz",
+    ),
+    dict(
+        model_id="cagram_LP",
+        path_to_model=files(LP) / "LP_CA2.xml.gz",
+        model_type="carveme",
+        path_to_genome=files(LP) / "LP_protein_fasta.faa.gz",
+    ),
+    dict(
+        model_id="msgram_LP",
+        path_to_model=files(LP) / "LP_MS2.sbml.gz",
+        model_type="modelseed",
+        path_to_genome=files(LP) / "LP_protein_fasta.faa.gz",
+    ),
+    dict(
+        model_id="agora_LP",
+        path_to_model=files(LP) / "LP_WCFS1_agora.xml.gz",
+        model_type="agora",
+        path_to_genome=files(LP) / "LP_WCFS1.fasta.gz",
+    ),
+]
+```
+
 First stage is the creation of gathered models, a class, that performs
 conversion and contains results of all stages:
 ```
 gathered = GatheredModels()
 for model in lp_example:
     gathered.add_model(**model)
 gathered.run()
```

### Comparing `gemsembler-0.6.4/pyproject.toml` & `gemsembler-0.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gemsembler"
-version = "0.6.4"
+version = "0.6.5"
 description = "A tool for assembling and comparing several types of Genome-Scale Metabolic Models."
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     { name = "Elena Matveishina", email = "elena.matveishina@embl.de" },
     { name = "Bartosz Bartmanski", email = "bartosz.bartmanski@embl.de" }
 ]
@@ -49,15 +49,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["src"]
 
 [tool.bumpver]
-current_version = "0.6.4"
+current_version = "0.6.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `gemsembler-0.6.4/src/gemsembler/__init__.py` & `gemsembler-0.6.5/src/gemsembler/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from importlib.resources import files
-
-from .anticreation import get_model_of_interest
+from .anticreation import get_model_of_interest, get_models_with_all_confidence_levels
 from .creation import read_supermodel_from_pkl
 from .data import BU, LP
 from .gathering import GatheredModels, load_sbml_model
 
-__version__ = "0.6.4"
+__version__ = "0.6.5"
 
 lp_example = [
     dict(
         model_id="curated_LP",
         path_to_model=files(LP) / "LP_iLP728_revision_data_met_C_c.xml.gz",
         model_type="carveme",
         path_to_genome=files(LP) / "LP_protein_fasta.faa.gz",
```

### Comparing `gemsembler-0.6.4/src/gemsembler/__main__.py` & `gemsembler-0.6.5/src/gemsembler/__main__.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/anticreation.py` & `gemsembler-0.6.5/src/gemsembler/anticreation.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,17 @@
         ):
             out_reaction.lower_bound = -1000.0
             out_reaction.upper_bound = 1000.0
         else:
             out_reaction.lower_bound = r_lower_bound.get(interest_level_r)[0]
             out_reaction.upper_bound = r_upper_bound.get(interest_level_r)[0]
         for met, k in r_metabolites.get(interest_level_r).items():
-            out_met = Metabolite(met.id, name=met.name, compartment=met.id[-1])
+            out_met = Metabolite(
+                met.id, name=met.name, compartment=met.compartments["assembly"][0]
+            )
             out_reaction.add_metabolites({out_met: k})
         if r_gene_reaction_rule.get(gene_interest_level):
             out_reaction.gene_reaction_rule = r_gene_reaction_rule.get(
                 gene_interest_level
             )[0]
         else:
             out_reaction.gene_reaction_rule = ""
```

### Comparing `gemsembler-0.6.4/src/gemsembler/comparison.py` & `gemsembler-0.6.5/src/gemsembler/comparison.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/conversion.py` & `gemsembler-0.6.5/src/gemsembler/conversion.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/creation.py` & `gemsembler-0.6.5/src/gemsembler/creation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/curation.py` & `gemsembler-0.6.5/src/gemsembler/curation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/data/BU/BU_agora.xml.gz` & `gemsembler-0.6.5/src/gemsembler/data/BU/BU_agora.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/data/BU/BU_carveme_hom.xml.gz` & `gemsembler-0.6.5/src/gemsembler/data/BU/BU_carveme_hom.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/data/BU/BU_gapseq.xml.gz` & `gemsembler-0.6.5/src/gemsembler/data/BU/BU_gapseq.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/data/BU/BU_modelSEED.sbml.gz` & `gemsembler-0.6.5/src/gemsembler/data/BU/BU_modelSEED.sbml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/data/LP/LP_CA1.xml.gz` & `gemsembler-0.6.5/src/gemsembler/data/LP/LP_CA1.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/data/LP/LP_CA2.xml.gz` & `gemsembler-0.6.5/src/gemsembler/data/LP/LP_CA2.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/data/LP/LP_MS2.sbml.gz` & `gemsembler-0.6.5/src/gemsembler/data/LP/LP_MS2.sbml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/data/LP/LP_WCFS1.fasta.gz` & `gemsembler-0.6.5/src/gemsembler/data/LP/LP_WCFS1.fasta.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz` & `gemsembler-0.6.5/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz` & `gemsembler-0.6.5/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/data/LP/LP_protein_fasta.faa.gz` & `gemsembler-0.6.5/src/gemsembler/data/LP/LP_protein_fasta.faa.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/dbs.py` & `gemsembler-0.6.5/src/gemsembler/dbs.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/downstream.py` & `gemsembler-0.6.5/src/gemsembler/downstream.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import operator
 import re
 import warnings
 from collections import defaultdict
+from copy import deepcopy
 from pathlib import Path
 
 import dill
 import pandas as pd
 from cobra.flux_analysis import pfba
 from .creation import SuperModel
 from .comparison import getCoreGPR
@@ -32,49 +33,38 @@
         out_bp_production_tab.to_csv(
             f"{write_output_to_folder}/all_metabolites_production.tsv",
             sep="\t",
             index=False,
         )
     else:
         out_bp_production_tab.to_csv(
-            f"{write_output_to_folder}/all_{file_name}.tsv", sep="\t", index=False,
+            f"{write_output_to_folder}/{file_name}.tsv", sep="\t", index=False,
         )
-    out_core_bp_production_tab = out_bp_production_tab[
-        (out_bp_production_tab != "nan").all(axis=1)
-    ]
-    out_core_bp_production_tab.index = out_core_bp_production_tab["Metabolites"]
-    num = out_core_bp_production_tab[
-        out_core_bp_production_tab.columns.difference(["Metabolites"])
+    out_bp_production_tab.index = out_bp_production_tab["Metabolites"]
+    num = out_bp_production_tab[
+        out_bp_production_tab.columns.difference(["Metabolites"])
     ]
     num_no_grow = num.drop(index="overall_growth", errors="ignore")
     num_no_grow = num_no_grow.astype(
         {mod_name: "float" for mod_name in num_no_grow.columns}
     )
-    if file_name is None:
-        num_no_grow.to_csv(
-            f"{write_output_to_folder}/core_metabolites_production.tsv", sep="\t",
-        )
-    else:
-        num_no_grow.to_csv(
-            f"{write_output_to_folder}/core_{file_name}.tsv", sep="\t",
-        )
     bp_heatmap = sns.clustermap(
         num_no_grow,
         yticklabels=yticklabels,
         metric=metric,
         method=method,
         cmap=cmap,
         center=center,
         linewidths=linewidths,
         **kwargs,
     )
     if file_name is None:
-        bp_heatmap.savefig(f"{write_output_to_folder}/core_metabolites_production.png")
+        bp_heatmap.savefig(f"{write_output_to_folder}/all_metabolites_production.png")
     else:
-        bp_heatmap.savefig(f"{write_output_to_folder}/core_{file_name}.png")
+        bp_heatmap.savefig(f"{write_output_to_folder}/{file_name}.png")
 
 
 def table_reactions_confidence(
     supermodel: SuperModel,
     output_name: str,
     pathway_r=None,
     yes_range=1,
@@ -317,15 +307,15 @@
         return g, t
     else:
         return g
 
 
 def run_growth_full_flux_analysis(
     models_to_analyse: dict,
-    medium: list,
+    medium: dict,
     write_output_to_folder=None,
     file_name=None,
     draw_pfba_for_models=None,
     supermodel_for_draw_pfba=None,
     draw_met_not_int=False,
     biomass_r_id=None,
     m_compartment_suffix=None,
@@ -352,17 +342,25 @@
     stat_out = {}
     bp_synt = []
     for k, model in models_to_analyse.items():
         med_mod = {}
         for e in model.exchanges:
             if (
                 list(e.metabolites.keys())[0].id.removesuffix(m_compartment_suffix)
-                in medium
+                in medium.keys()
             ):
-                med_mod.update({e.id: 1000})
+                med_mod.update(
+                    {
+                        e.id: medium[
+                            list(e.metabolites.keys())[0].id.removesuffix(
+                                m_compartment_suffix
+                            )
+                        ]
+                    }
+                )
             else:
                 med_mod.update({e.id: 0})
         old_medium = model.medium
         model.medium = med_mod
         res = model.optimize()
         flux_res_out[k] = {"overall_fba": res}
         model_data = [res.objective_value]
@@ -371,57 +369,55 @@
         all_met = [mm.id for mm in model.metabolites]
         all_r = [rr.id for rr in model.reactions]
         bp_model = [
             react.id for react in model.reactions.get_by_id(biomass_r_id).reactants
         ]
         for bp in biomass_p:
             if bp not in all_met:
-                model_data.append("nan")
-            else:
-                demand_added = False
-                if ("DM_" + bp) not in all_r:
-                    model.add_boundary(model.metabolites.get_by_id(bp), type="demand")
-                    demand_added = True
-                model.objective = model.demands.get_by_id("DM_" + bp)
-                res_bp = model.optimize()
+                model_data.append(-0.5)
+                continue
+            demand_added = False
+            if ("DM_" + bp) not in all_r:
+                model.add_boundary(model.metabolites.get_by_id(bp), type="demand")
+                demand_added = True
+            model.objective = model.demands.get_by_id("DM_" + bp)
+            res_bp = model.optimize()
+            flux_res_out[k].update(
+                {bp.removesuffix(bp_compartment_suffix) + "_fba": res_bp}
+            )
+            if res_bp.objective_value > 0.001:
+                model_data.append(1)
+                if bp.removesuffix(bp_compartment_suffix) in medium.keys():
+                    model_med_stat = model_med_stat + 1
+                else:
+                    model_stat = model_stat + 1
+                if bp not in bp_synt:
+                    bp_synt.append(bp)
+                pfba_res = pfba(model)
                 flux_res_out[k].update(
-                    {bp.removesuffix(bp_compartment_suffix) + "_fba": res_bp}
+                    {bp.removesuffix(bp_compartment_suffix) + "_pfba": pfba_res}
                 )
-                if res_bp.objective_value > 0.001:
-                    model_data.append(1)
-                    if bp.removesuffix(bp_compartment_suffix) in medium:
-                        model_med_stat = model_med_stat + 1
-                    else:
-                        model_stat = model_stat + 1
-                    if bp not in bp_synt:
-                        bp_synt.append(bp)
-                    pfba_res = pfba(model)
-                    flux_res_out[k].update(
-                        {bp.removesuffix(bp_compartment_suffix) + "_pfba": pfba_res}
-                    )
-                    reactions = list(
-                        pfba_res.to_frame()[
-                            (pfba_res.to_frame()["fluxes"] > 0.001)
-                            | (pfba_res.to_frame()["fluxes"] < -0.001)
-                        ].index
-                    )
-                    path_pfba_out[k].update(
-                        {
-                            bp.removesuffix(bp_compartment_suffix)
-                            + "_path_pfba": reactions
-                        }
-                    )
+                reactions = list(
+                    pfba_res.to_frame()[
+                        (pfba_res.to_frame()["fluxes"] > 0.001)
+                        | (pfba_res.to_frame()["fluxes"] < -0.001)
+                    ].index
+                )
+                path_pfba_out[k].update(
+                    {bp.removesuffix(bp_compartment_suffix) + "_path_pfba": reactions}
+                )
+            else:
+                if bp in bp_model:
+                    model_data.append(0)
                 else:
-                    if bp in bp_model:
-                        model_data.append(0)
-                    else:
-                        model_data.append(0.5)
-                if demand_added:
-                    model.remove_reactions(["DM_" + bp])
+                    model_data.append(0.5)
+            if demand_added:
+                model.remove_reactions(["DM_" + bp])
         model.medium = old_medium
+        model.objective = model.reactions.get_by_id(biomass_r_id)
         out_bp_production.update({k: model_data})
         stat_out.update({k: model_stat})
         stat_out.update({"medium_" + k: model_med_stat})
     out_bp_production_tab = pd.DataFrame(out_bp_production)
     stat_out.update({"not_synthesized": len(set(biomass_p) - set(bp_synt))})
     stat_out_tab = pd.DataFrame(
         stat_out.items(),
@@ -445,15 +441,15 @@
                 "Models for which to draw pfba of biomass precursors is not provided. "
                 "So for each biomass precursor the model with "
                 "the highest confidence level will be used."
             )
         draw_pfba_results(
             path_pfba_out,
             supermodel_for_draw_pfba,
-            medium,
+            list(medium.keys()),
             write_output_to_folder,
             draw_pfba_for_models,
             draw_met_not_int,
         )
 
     return out_bp_production_tab, flux_res_out, path_pfba_out, stat_out_tab
 
@@ -526,15 +522,15 @@
                 metquest_all_res_paths[mod] = f / "shortest_paths.pkl"
     synthes_out = {"Metabolites": metabolites_ids} | {mod: [] for mod in model_list}
     for mod in model_list:
         model_stat = 0
         mq_data = dill.load(open(metquest_all_res_paths[mod], "rb"))
         for bp in metabolites_ids:
             if bp not in mq_data["paths"].keys():
-                to_append = "nan"
+                to_append = -0.5
             else:
                 if bp.removesuffix("_c") in medium:
                     to_append = 0.75
                     if bp not in met_med:
                         met_med.append(bp)
                 elif bp.removesuffix("_c") in cofactors:
                     to_append = 0.5
```

### Comparing `gemsembler-0.6.4/src/gemsembler/drawing.py` & `gemsembler-0.6.5/src/gemsembler/drawing.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,53 @@
 import re
 import networkx as nx
 import pandas as pd
 import seaborn as sns
 from .creation import NewElement, SuperModel
 from .comparison import getCoreGPR, getCoreConnections
 from pyvis.network import Network
+from copy import deepcopy
+
+MET_NOT_INT_GLOBAL = {
+    "h": 0,
+    "h2o": 0,
+    "h2": 0,
+    "oh1": 0,
+    "o2": 0,
+    "co2": 0,
+    "coa": 0,
+    "ppi": 0,
+    "pi": 0,
+    "amp": 0,
+    "adp": 0,
+    "atp": 0,
+    "cmp": 0,
+    "cdp": 0,
+    "ctp": 0,
+    "gmp": 0,
+    "gdp": 0,
+    "gtp": 0,
+    "ump": 0,
+    "udp": 0,
+    "utp": 0,
+    "nad": 0,
+    "nadh": 0,
+    "nadp": 0,
+    "nadph": 0,
+    "dadp": 0,
+    "damp": 0,
+    "nh3": 0,
+    "nh4": 0,
+    "fadh2": 0,
+    "fad": 0,
+    "ac": 0,
+    "accoa": 0,
+    "h2s": 0,
+    "HC00250": 0,
+}
 
 
 def get_color_palette(sources_number: int) -> dict:
     up = math.ceil(sources_number / 10)
     down = math.ceil(sources_number / 10)
     colors = sns.color_palette("bright").as_hex()
     out_colors = {
@@ -179,51 +218,15 @@
     size=25,
 ):
     if not output_name.endswith(".html"):
         raise ValueError(
             "Output file for the plot is of wrong format. Please use html file name."
         )
     if met_not_int is None:
-        met_not_int = {
-            "h": 0,
-            "h2o": 0,
-            "h2": 0,
-            "oh1": 0,
-            "o2": 0,
-            "co2": 0,
-            "coa": 0,
-            "ppi": 0,
-            "pi": 0,
-            "amp": 0,
-            "adp": 0,
-            "atp": 0,
-            "cmp": 0,
-            "cdp": 0,
-            "ctp": 0,
-            "gmp": 0,
-            "gdp": 0,
-            "gtp": 0,
-            "ump": 0,
-            "udp": 0,
-            "utp": 0,
-            "nad": 0,
-            "nadh": 0,
-            "nadp": 0,
-            "nadph": 0,
-            "dadp": 0,
-            "damp": 0,
-            "nh3": 0,
-            "nh4": 0,
-            "fadh2": 0,
-            "fad": 0,
-            "ac": 0,
-            "accoa": 0,
-            "h2s": 0,
-            "HC00250": 0,
-        }
+        met_not_int = deepcopy(MET_NOT_INT_GLOBAL)
     color_brewer = get_color_palette(len(supermodel.sources))
     if n_letter is None:
         n_letter = supermodel.get_short_name_len()
     g = nx.DiGraph()
     path_met = []
     for value in pathway.values():
         for v in value:
@@ -680,51 +683,15 @@
     size=25,
 ):
     if not output_name.endswith(".html"):
         raise ValueError(
             "Output file for the plot is of wrong format. Please use html file name."
         )
     if met_not_int is None:
-        met_not_int = {
-            "h": 0,
-            "h2o": 0,
-            "h2": 0,
-            "oh1": 0,
-            "o2": 0,
-            "co2": 0,
-            "coa": 0,
-            "ppi": 0,
-            "pi": 0,
-            "amp": 0,
-            "adp": 0,
-            "atp": 0,
-            "cmp": 0,
-            "cdp": 0,
-            "ctp": 0,
-            "gmp": 0,
-            "gdp": 0,
-            "gtp": 0,
-            "ump": 0,
-            "udp": 0,
-            "utp": 0,
-            "nad": 0,
-            "nadh": 0,
-            "nadp": 0,
-            "nadph": 0,
-            "dadp": 0,
-            "damp": 0,
-            "nh3": 0,
-            "nh4": 0,
-            "fadh2": 0,
-            "fad": 0,
-            "ac": 0,
-            "accoa": 0,
-            "h2s": 0,
-            "HC00250": 0,
-        }
+        met_not_int = deepcopy(MET_NOT_INT_GLOBAL)
     color_brewer = get_color_palette(len(supermodel.sources))
     if n_letter is None:
         n_letter = supermodel.get_short_name_len()
     g = nx.DiGraph()
     for r_id in path:
         r = supermodel.reactions.assembly.get(r_id)
         colname_r = define_node_features(color_brewer, "single_path_r", r, n_letter,)
@@ -953,57 +920,23 @@
     wid=1920,
     hei=1080,
     size=25,
 ):
     if metabolite_id not in supermodel.metabolites.assembly.keys():
         raise ValueError(f"{metabolite_id} is not in the supermodel")
     if met_not_int is None:
-        met_not_int = {
-            "h": 0,
-            "h2o": 0,
-            "h2": 0,
-            "oh1": 0,
-            "o2": 0,
-            "co2": 0,
-            "coa": 0,
-            "ppi": 0,
-            "pi": 0,
-            "amp": 0,
-            "adp": 0,
-            "atp": 0,
-            "cmp": 0,
-            "cdp": 0,
-            "ctp": 0,
-            "gmp": 0,
-            "gdp": 0,
-            "gtp": 0,
-            "ump": 0,
-            "udp": 0,
-            "utp": 0,
-            "nad": 0,
-            "nadh": 0,
-            "nadp": 0,
-            "nadph": 0,
-            "dadp": 0,
-            "damp": 0,
-            "nh3": 0,
-            "nh4": 0,
-            "fadh2": 0,
-            "fad": 0,
-            "ac": 0,
-            "accoa": 0,
-            "h2s": 0,
-            "HC00250": 0,
-        }
+        met_not_int = deepcopy(MET_NOT_INT_GLOBAL)
     all_r = set()
+    all_g = set()
     med_high_connect = []
-    all_m = [metabolite_id]
+    all_m = {metabolite_id}
+    dist_m = [metabolite_id]
     for i in range(neighborhood_dist):
         new_all_m = set()
-        for m_id in all_m:
+        for m_id in dist_m:
             tmp_m = re.sub("_([cep])$", "", m_id)
             if tmp_m in met_not_int.keys():
                 continue
             met = supermodel.metabolites.assembly.get(m_id)
             reactions = [r.id for r in met.reactions["assembly"]]
             if len(reactions) > highly_connected_t:
                 reactions = []
@@ -1016,16 +949,23 @@
                     [
                         m.id
                         for m in supermodel.reactions.assembly[r_id]
                         .metabolites["assembly"]
                         .keys()
                     ]
                 )
-        all_m = new_all_m
-    draw_one_synt_path(
+                all_g = all_g | set(
+                    [
+                        g.id
+                        for g in supermodel.reactions.assembly[r_id].genes["assembly"]
+                    ]
+                )
+        dist_m = new_all_m
+        all_m = all_m | new_all_m
+    graph = draw_one_synt_path(
         supermodel,
         list(all_r),
         med_high_connect,
         [re.sub("_([cep])$", "", metabolite_id)],
         output_name,
         draw_met_not_int,
         genes,
@@ -1033,7 +973,8 @@
         directed,
         met_not_int,
         n_letter,
         wid,
         hei,
         size,
     )
+    return graph, all_r, all_g, all_m
```

### Comparing `gemsembler-0.6.4/src/gemsembler/gathering.py` & `gemsembler-0.6.5/src/gemsembler/gathering.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,17 +104,15 @@
     Notes
     -----
     If all 3 parameters bellow are None then gene conversion is not done and
     genomes for model_id are not need.
     """
 
     def __init__(
-        self,
-        custom_model_type=None,
-        clear_db_cache=False,
+        self, custom_model_type=None, clear_db_cache=False,
     ):
         # If specified, clear the cached conversion tables and dictionaries
         if clear_db_cache:
             for p in user_data_path("gemsembler").iterdir():
                 p.unlink()
 
         self.__conf = {
@@ -433,14 +431,15 @@
 
     def assemble_supermodel(
         self,
         output_folder: str,
         assembly_id=None,
         path_final_genome_nt=None,
         path_final_genome_aa=None,
+        evalue_threshold=0.001,
         do_mix_conv_notconv=False,
         and_as_solid=False,
     ):
         # Check if assembly and final genome are present.
         # If not, throw a warning.
         if not assembly_id and not path_final_genome_nt and not path_final_genome_aa:
             warnings.warn(
@@ -522,15 +521,16 @@
                     warnings.warn("\nWarning! Something wrong with aa/nt in files/DB")
                 elif not model_gene_file:
                     warnings.warn("\nWarning! Something wrong with gene file")
                 else:
                     subprocess.run(
                         f"{blast_command} -query {model_gene_file} "
                         f"-db {Path(db_path, db_name)} "
-                        f"-max_target_seqs 1 -outfmt '6' -out {out_blast_file}",
+                        f"-max_target_seqs 1 -evalue {evalue_threshold} "
+                        f"-outfmt '6' -out {out_blast_file}",
                         shell=True,
                         check=True,
                         stdout=subprocess.PIPE,
                         stderr=subprocess.PIPE,
                         env=get_env(),
                     )
         # Get final tables to create new objects
```

### Comparing `gemsembler-0.6.4/src/gemsembler/genes.py` & `gemsembler-0.6.5/src/gemsembler/genes.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/pathsfinding.py` & `gemsembler-0.6.5/src/gemsembler/pathsfinding.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/periplasmic.py` & `gemsembler-0.6.5/src/gemsembler/periplasmic.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/selection.py` & `gemsembler-0.6.5/src/gemsembler/selection.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler/structural.py` & `gemsembler-0.6.5/src/gemsembler/structural.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/src/gemsembler.egg-info/PKG-INFO` & `gemsembler-0.6.5/src/gemsembler.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemsembler
-Version: 0.6.4
+Version: 0.6.5
 Summary: A tool for assembling and comparing several types of Genome-Scale Metabolic Models.
 Author-email: Elena Matveishina <elena.matveishina@embl.de>, Bartosz Bartmanski <bartosz.bartmanski@embl.de>
 License: MIT License
         
         Copyright (c) 2024 Zimmermann-Kogadeeva Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,14 +49,16 @@
 Requires-Dist: pyvis
 Requires-Dist: h5py
 Requires-Dist: platformdirs
 Requires-Dist: pyyaml
 
 # GEMsembler
 
+<img src="gemsembler_long.gif" alt="drawing" width="150"/>
+
 GEMsembler tool for assembling and comparing several types of Genome-Scale Metabolic
 Models. 
 
 **THIS IS A BETA VERSION! BUGS CAN BE EXPECTED**
 
 ## Installation
 
@@ -74,14 +76,50 @@
 (modelseed), gapseq (gapseq) and models downloaded from AGORA VMH database
 (agora) are supported. Custom type is coming soon. Genomes, from which the
 models are built will allow to convert and assemble genes as well.
 First, we import gemsembler and get the path to data files:
 ```
 from gemsembler import GatheredModels, lp_example, get_model_of_interest
 ```
+lp_example is a list with input models and related inforamtion such as model type, corresponding genome and so on.
+```
+lp_example = [
+    dict(
+        model_id="curated_LP",
+        path_to_model=files(LP) / "LP_iLP728_revision_data_met_C_c.xml.gz",
+        model_type="carveme",
+        path_to_genome=files(LP) / "LP_protein_fasta.faa.gz",
+    ),
+    dict(
+        model_id="cauniv_LP",
+        path_to_model=files(LP) / "LP_CA1.xml.gz",
+        model_type="carveme",
+        path_to_genome=files(LP) / "LP_protein_fasta.faa.gz",
+    ),
+    dict(
+        model_id="cagram_LP",
+        path_to_model=files(LP) / "LP_CA2.xml.gz",
+        model_type="carveme",
+        path_to_genome=files(LP) / "LP_protein_fasta.faa.gz",
+    ),
+    dict(
+        model_id="msgram_LP",
+        path_to_model=files(LP) / "LP_MS2.sbml.gz",
+        model_type="modelseed",
+        path_to_genome=files(LP) / "LP_protein_fasta.faa.gz",
+    ),
+    dict(
+        model_id="agora_LP",
+        path_to_model=files(LP) / "LP_WCFS1_agora.xml.gz",
+        model_type="agora",
+        path_to_genome=files(LP) / "LP_WCFS1.fasta.gz",
+    ),
+]
+```
+
 First stage is the creation of gathered models, a class, that performs
 conversion and contains results of all stages:
 ```
 gathered = GatheredModels()
 for model in lp_example:
     gathered.add_model(**model)
 gathered.run()
```

### Comparing `gemsembler-0.6.4/src/gemsembler.egg-info/SOURCES.txt` & `gemsembler-0.6.5/src/gemsembler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/tests/test_conversion.py` & `gemsembler-0.6.5/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/tests/test_curation.py` & `gemsembler-0.6.5/tests/test_curation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/tests/test_dbs.py` & `gemsembler-0.6.5/tests/test_dbs.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/tests/test_gathering.py` & `gemsembler-0.6.5/tests/test_gathering.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.4/tests/test_selection.py` & `gemsembler-0.6.5/tests/test_selection.py`

 * *Files identical despite different names*

