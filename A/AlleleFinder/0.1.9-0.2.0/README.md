# Comparing `tmp/allelefinder-0.1.9.tar.gz` & `tmp/allelefinder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allelefinder-0.1.9.tar", last modified: Mon Apr 29 19:28:27 2024, max compression
+gzip compressed data, was "allelefinder-0.2.0.tar", last modified: Mon Apr 29 20:02:18 2024, max compression
```

## Comparing `allelefinder-0.1.9.tar` & `allelefinder-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:28:27.264323 allelefinder-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:28:27.264323 allelefinder-0.1.9/AlleleFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-29 19:28:27.000000 allelefinder-0.1.9/AlleleFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-29 19:28:27.000000 allelefinder-0.1.9/AlleleFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:28:27.000000 allelefinder-0.1.9/AlleleFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-29 19:28:27.000000 allelefinder-0.1.9/AlleleFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 19:28:27.000000 allelefinder-0.1.9/AlleleFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-29 19:28:19.000000 allelefinder-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 19:28:19.000000 allelefinder-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-29 19:28:27.264323 allelefinder-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-29 19:28:19.000000 allelefinder-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:28:27.264323 allelefinder-0.1.9/allele_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26836 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/allele_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    38776 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/allele_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)   121713 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    53101 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/stec.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-29 19:28:19.000000 allelefinder-0.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:28:27.264323 allelefinder-0.1.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2048 2024-04-29 19:28:19.000000 allelefinder-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:28:27.264323 allelefinder-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_0_profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_1_allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_2_allele_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_3_stec_profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_4_stec_allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_5_stec_allele_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_6_stec_aa_allele_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_7_stec_allele_split.py
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_8_stec_allele_concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_9_stec_allele_translate_find.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:02:18.442148 allelefinder-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:02:18.442148 allelefinder-0.2.0/AlleleFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-29 20:02:18.000000 allelefinder-0.2.0/AlleleFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-29 20:02:18.000000 allelefinder-0.2.0/AlleleFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:02:18.000000 allelefinder-0.2.0/AlleleFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-29 20:02:18.000000 allelefinder-0.2.0/AlleleFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 20:02:18.000000 allelefinder-0.2.0/AlleleFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-29 20:02:10.000000 allelefinder-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 20:02:10.000000 allelefinder-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-29 20:02:18.442148 allelefinder-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-29 20:02:10.000000 allelefinder-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:02:18.438148 allelefinder-0.2.0/allele_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 20:02:10.000000 allelefinder-0.2.0/allele_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26836 2024-04-29 20:02:10.000000 allelefinder-0.2.0/allele_tools/allele_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38776 2024-04-29 20:02:10.000000 allelefinder-0.2.0/allele_tools/allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-04-29 20:02:10.000000 allelefinder-0.2.0/allele_tools/allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121713 2024-04-29 20:02:10.000000 allelefinder-0.2.0/allele_tools/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-04-29 20:02:10.000000 allelefinder-0.2.0/allele_tools/profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53101 2024-04-29 20:02:10.000000 allelefinder-0.2.0/allele_tools/stec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 20:02:10.000000 allelefinder-0.2.0/allele_tools/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-29 20:02:10.000000 allelefinder-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 20:02:18.442148 allelefinder-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2048 2024-04-29 20:02:10.000000 allelefinder-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:02:18.442148 allelefinder-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 20:02:10.000000 allelefinder-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-04-29 20:02:10.000000 allelefinder-0.2.0/tests/test_0_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-04-29 20:02:10.000000 allelefinder-0.2.0/tests/test_1_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-04-29 20:02:10.000000 allelefinder-0.2.0/tests/test_2_allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-29 20:02:10.000000 allelefinder-0.2.0/tests/test_3_stec_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-29 20:02:10.000000 allelefinder-0.2.0/tests/test_4_stec_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-29 20:02:10.000000 allelefinder-0.2.0/tests/test_5_stec_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-29 20:02:10.000000 allelefinder-0.2.0/tests/test_6_stec_aa_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-29 20:02:10.000000 allelefinder-0.2.0/tests/test_7_stec_allele_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-29 20:02:10.000000 allelefinder-0.2.0/tests/test_8_stec_allele_concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-29 20:02:10.000000 allelefinder-0.2.0/tests/test_9_stec_allele_translate_find.py
```

### Comparing `allelefinder-0.1.9/AlleleFinder.egg-info/PKG-INFO` & `allelefinder-0.2.0/AlleleFinder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlleleFinder
-Version: 0.1.9
+Version: 0.2.0
 Home-page: https://github.com/OLC-Bioinformatics/AlleleFinder
 Author: Adam Koziol
 Author-email: adam.koziol@inspection.gc.ca
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,15 +27,16 @@
 Requires-Dist: xlsxwriter==3.0.2
 
 # AlleleFinder
 
 [![CircleCI](https://circleci.com/gh/OLC-Bioinformatics/AlleleFinder/tree/main.svg?style=shield)](https://circleci.com/gh/OLC-LOC-Bioinformatics/AlleleFinder/tree/main)
 [![codecov](https://codecov.io/gh/OLC-Bioinformatics/AlleleFinder/branch/main/graph/badge.svg?token=Z6SSEJV9GU)](https://codecov.io/gh/OLC-Bioinformatics/AlleleFinder)
 [![Anaconda-Server Badge](https://img.shields.io/badge/install%20with-conda-brightgreen)](https://anaconda.org/olcbioinformatics/allelefinder)
-[![GitHub version](https://badge.fury.io/gh/olc-bioinformatics%2Fallelefinder.svg)](https://badge.fury.io/gh/olc-bioinformatics%2Fallelefinder)
+[![GitHub Release](https://img.shields.io/github/v/release/OLC-Bioinformatics/AlleleFinder?display_name=release&label=version&color=%20dark%20green
+)](https://github.com/OLC-Bioinformatics/AlleleFinder/releases)
 [![GitHub issues](https://img.shields.io/github/issues/OLC-Bioinformatics/AlleleFinder)](https://github.com/OLC-LOC-Bioinformatics/AlleleFinder/issues)
 [![Documentation Status](https://readthedocs.org/projects/pip/badge/?version=stable)](https://OLC-Bioinformatics.github.io/AlleleFinder/?badge=stable)
 [![license](https://img.shields.io/badge/license-MIT-brightgreen)](https://github.com/OLC-Bioinformatics/AlleleFinder/blob/main/LICENSE)
 
 ## Overview
 
 AlleleFinder is a Python-based suite of tools designed for the discovery, sequence typing, and profiling of _stx_ alleles in Shiga toxin-producing _Escherichia coli_ (STEC). It provides a comprehensive solution for researchers and professionals working in the field of bacterial genomics.
```

### Comparing `allelefinder-0.1.9/AlleleFinder.egg-info/SOURCES.txt` & `allelefinder-0.2.0/AlleleFinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/LICENSE` & `allelefinder-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/PKG-INFO` & `allelefinder-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlleleFinder
-Version: 0.1.9
+Version: 0.2.0
 Home-page: https://github.com/OLC-Bioinformatics/AlleleFinder
 Author: Adam Koziol
 Author-email: adam.koziol@inspection.gc.ca
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,15 +27,16 @@
 Requires-Dist: xlsxwriter==3.0.2
 
 # AlleleFinder
 
 [![CircleCI](https://circleci.com/gh/OLC-Bioinformatics/AlleleFinder/tree/main.svg?style=shield)](https://circleci.com/gh/OLC-LOC-Bioinformatics/AlleleFinder/tree/main)
 [![codecov](https://codecov.io/gh/OLC-Bioinformatics/AlleleFinder/branch/main/graph/badge.svg?token=Z6SSEJV9GU)](https://codecov.io/gh/OLC-Bioinformatics/AlleleFinder)
 [![Anaconda-Server Badge](https://img.shields.io/badge/install%20with-conda-brightgreen)](https://anaconda.org/olcbioinformatics/allelefinder)
-[![GitHub version](https://badge.fury.io/gh/olc-bioinformatics%2Fallelefinder.svg)](https://badge.fury.io/gh/olc-bioinformatics%2Fallelefinder)
+[![GitHub Release](https://img.shields.io/github/v/release/OLC-Bioinformatics/AlleleFinder?display_name=release&label=version&color=%20dark%20green
+)](https://github.com/OLC-Bioinformatics/AlleleFinder/releases)
 [![GitHub issues](https://img.shields.io/github/issues/OLC-Bioinformatics/AlleleFinder)](https://github.com/OLC-LOC-Bioinformatics/AlleleFinder/issues)
 [![Documentation Status](https://readthedocs.org/projects/pip/badge/?version=stable)](https://OLC-Bioinformatics.github.io/AlleleFinder/?badge=stable)
 [![license](https://img.shields.io/badge/license-MIT-brightgreen)](https://github.com/OLC-Bioinformatics/AlleleFinder/blob/main/LICENSE)
 
 ## Overview
 
 AlleleFinder is a Python-based suite of tools designed for the discovery, sequence typing, and profiling of _stx_ alleles in Shiga toxin-producing _Escherichia coli_ (STEC). It provides a comprehensive solution for researchers and professionals working in the field of bacterial genomics.
```

### Comparing `allelefinder-0.1.9/README.md` & `allelefinder-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # AlleleFinder
 
 [![CircleCI](https://circleci.com/gh/OLC-Bioinformatics/AlleleFinder/tree/main.svg?style=shield)](https://circleci.com/gh/OLC-LOC-Bioinformatics/AlleleFinder/tree/main)
 [![codecov](https://codecov.io/gh/OLC-Bioinformatics/AlleleFinder/branch/main/graph/badge.svg?token=Z6SSEJV9GU)](https://codecov.io/gh/OLC-Bioinformatics/AlleleFinder)
 [![Anaconda-Server Badge](https://img.shields.io/badge/install%20with-conda-brightgreen)](https://anaconda.org/olcbioinformatics/allelefinder)
-[![GitHub version](https://badge.fury.io/gh/olc-bioinformatics%2Fallelefinder.svg)](https://badge.fury.io/gh/olc-bioinformatics%2Fallelefinder)
+[![GitHub Release](https://img.shields.io/github/v/release/OLC-Bioinformatics/AlleleFinder?display_name=release&label=version&color=%20dark%20green
+)](https://github.com/OLC-Bioinformatics/AlleleFinder/releases)
 [![GitHub issues](https://img.shields.io/github/issues/OLC-Bioinformatics/AlleleFinder)](https://github.com/OLC-LOC-Bioinformatics/AlleleFinder/issues)
 [![Documentation Status](https://readthedocs.org/projects/pip/badge/?version=stable)](https://OLC-Bioinformatics.github.io/AlleleFinder/?badge=stable)
 [![license](https://img.shields.io/badge/license-MIT-brightgreen)](https://github.com/OLC-Bioinformatics/AlleleFinder/blob/main/LICENSE)
 
 ## Overview
 
 AlleleFinder is a Python-based suite of tools designed for the discovery, sequence typing, and profiling of _stx_ alleles in Shiga toxin-producing _Escherichia coli_ (STEC). It provides a comprehensive solution for researchers and professionals working in the field of bacterial genomics.
```

### Comparing `allelefinder-0.1.9/allele_tools/allele_profiler.py` & `allelefinder-0.2.0/allele_tools/allele_profiler.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/allele_tools/allele_translate_reduce.py` & `allelefinder-0.2.0/allele_tools/allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/allele_tools/allele_updater.py` & `allelefinder-0.2.0/allele_tools/allele_updater.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/allele_tools/methods.py` & `allelefinder-0.2.0/allele_tools/methods.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/allele_tools/profile_reduce.py` & `allelefinder-0.2.0/allele_tools/profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/allele_tools/stec.py` & `allelefinder-0.2.0/allele_tools/stec.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/setup.py` & `allelefinder-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/tests/test_0_profile_reduce.py` & `allelefinder-0.2.0/tests/test_0_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/tests/test_1_allele_translate_reduce.py` & `allelefinder-0.2.0/tests/test_1_allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/tests/test_2_allele_updater.py` & `allelefinder-0.2.0/tests/test_2_allele_updater.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/tests/test_3_stec_profile_reduce.py` & `allelefinder-0.2.0/tests/test_3_stec_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/tests/test_4_stec_allele_translate_reduce.py` & `allelefinder-0.2.0/tests/test_4_stec_allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/tests/test_5_stec_allele_find.py` & `allelefinder-0.2.0/tests/test_5_stec_allele_find.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/tests/test_6_stec_aa_allele_find.py` & `allelefinder-0.2.0/tests/test_6_stec_aa_allele_find.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/tests/test_7_stec_allele_split.py` & `allelefinder-0.2.0/tests/test_7_stec_allele_split.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/tests/test_8_stec_allele_concatenate.py` & `allelefinder-0.2.0/tests/test_8_stec_allele_concatenate.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.9/tests/test_9_stec_allele_translate_find.py` & `allelefinder-0.2.0/tests/test_9_stec_allele_translate_find.py`

 * *Files identical despite different names*

