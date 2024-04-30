# Comparing `tmp/bam-filter-1.4.6.tar.gz` & `tmp/bam-filter-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bam-filter-1.4.6.tar", last modified: Tue Apr 30 13:07:24 2024, max compression
+gzip compressed data, was "bam-filter-1.4.7.tar", last modified: Tue Apr 30 13:41:52 2024, max compression
```

## Comparing `bam-filter-1.4.6.tar` & `bam-filter-1.4.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:07:24.536532 bam-filter-1.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-30 13:07:20.000000 bam-filter-1.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 13:07:20.000000 bam-filter-1.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-30 13:07:24.536532 bam-filter-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21540 2024-04-30 13:07:20.000000 bam-filter-1.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:07:24.536532 bam-filter-1.4.6/bam_filter/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-30 13:07:24.536532 bam-filter-1.4.6/bam_filter/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    23868 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/lca.py
--rw-r--r--   0 runner    (1001) docker     (127)    40437 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/reassign.py
--rw-r--r--   0 runner    (1001) docker     (127)    50203 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/sam_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    44025 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:07:24.536532 bam-filter-1.4.6/bam_filter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-30 13:07:24.000000 bam-filter-1.4.6/bam_filter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-30 13:07:24.000000 bam-filter-1.4.6/bam_filter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:07:24.000000 bam-filter-1.4.6/bam_filter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 13:07:24.000000 bam-filter-1.4.6/bam_filter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-30 13:07:24.000000 bam-filter-1.4.6/bam_filter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 13:07:24.000000 bam-filter-1.4.6/bam_filter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-30 13:07:24.536532 bam-filter-1.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 13:07:20.000000 bam-filter-1.4.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    70238 2024-04-30 13:07:20.000000 bam-filter-1.4.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:41:52.132058 bam-filter-1.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-30 13:41:45.000000 bam-filter-1.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 13:41:45.000000 bam-filter-1.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-30 13:41:52.132058 bam-filter-1.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21540 2024-04-30 13:41:45.000000 bam-filter-1.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:41:52.136058 bam-filter-1.4.7/bam_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 13:41:45.000000 bam-filter-1.4.7/bam_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-30 13:41:45.000000 bam-filter-1.4.7/bam_filter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-30 13:41:52.136058 bam-filter-1.4.7/bam_filter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-30 13:41:45.000000 bam-filter-1.4.7/bam_filter/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-30 13:41:45.000000 bam-filter-1.4.7/bam_filter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23868 2024-04-30 13:41:45.000000 bam-filter-1.4.7/bam_filter/lca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40453 2024-04-30 13:41:45.000000 bam-filter-1.4.7/bam_filter/reassign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50219 2024-04-30 13:41:45.000000 bam-filter-1.4.7/bam_filter/sam_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44025 2024-04-30 13:41:45.000000 bam-filter-1.4.7/bam_filter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:41:52.132058 bam-filter-1.4.7/bam_filter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-30 13:41:52.000000 bam-filter-1.4.7/bam_filter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-30 13:41:52.000000 bam-filter-1.4.7/bam_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:41:52.000000 bam-filter-1.4.7/bam_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 13:41:52.000000 bam-filter-1.4.7/bam_filter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-30 13:41:52.000000 bam-filter-1.4.7/bam_filter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 13:41:52.000000 bam-filter-1.4.7/bam_filter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-30 13:41:52.136058 bam-filter-1.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 13:41:45.000000 bam-filter-1.4.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70238 2024-04-30 13:41:45.000000 bam-filter-1.4.7/versioneer.py
```

### Comparing `bam-filter-1.4.6/LICENSE` & `bam-filter-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.6/README.md` & `bam-filter-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.6/bam_filter/__main__.py` & `bam-filter-1.4.7/bam_filter/__main__.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.6/bam_filter/entropy.py` & `bam-filter-1.4.7/bam_filter/entropy.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.6/bam_filter/filter.py` & `bam-filter-1.4.7/bam_filter/filter.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.6/bam_filter/lca.py` & `bam-filter-1.4.7/bam_filter/lca.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.6/bam_filter/reassign.py` & `bam-filter-1.4.7/bam_filter/reassign.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import gc
 from collections import defaultdict
 import os
 import concurrent.futures
 import math
 import warnings
 from bam_filter.sam_utils import check_bam_file
+import shutil
 
 # import cProfile as prof
 # import pstats
 
 log = logging.getLogger("my_logger")
 
 
@@ -424,15 +425,15 @@
                 str(threads),
                 out_bam,
             )
 
         os.remove(out_files["bam_reassigned_tmp"])
     else:
         logging.info("Skipping BAM file sorting...")
-        os.rename(out_files["bam_reassigned_tmp"], out_bam)
+        shutil.move(out_files["bam_reassigned_tmp"], out_bam)
 
 
 # def calculate_alignment_score(identity, read_length):
 #     return (identity / math.log(read_length)) * math.sqrt(read_length)
 
 # Values from:
 # https://www.ncbi.nlm.nih.gov/IEB/ToolBox/CPP_DOC/lxr/source/src/algo/blast/core/blast_stat.c
```

### Comparing `bam-filter-1.4.6/bam_filter/sam_utils.py` & `bam-filter-1.4.7/bam_filter/sam_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import random
 from bam_filter.entropy import entropy, norm_entropy, gini_coeff, norm_gini_coeff
 from collections import defaultdict
 import pyranges as pr
 from pathlib import Path
 import concurrent.futures
 import gc
+import shutil
 
 # import cProfile as profile
 # import pstats
 
 # import pstats
 
 import matplotlib.pyplot as plt
@@ -1336,15 +1337,15 @@
                             str(threads),
                             out_files["bam_filtered"],
                         )
 
                 os.remove(out_files["bam_filtered_tmp"])
             else:
                 logging.info("Skipping BAM file sorting...")
-                os.rename(out_files["bam_filtered_tmp"], out_files["bam_filtered"])
+                shutil.move(out_files["bam_filtered_tmp"], out_files["bam_filtered"])
         else:
             logging.info("Skipping filtering BAM file creation...")
     else:
         logging.info("No references meet the filter conditions.")
         # Path(out_files["bam_filtered"]).touch()
         create_empty_bam(out_files["bam_filtered"])
         Path(out_files["stats_filtered"]).touch()
```

### Comparing `bam-filter-1.4.6/bam_filter/utils.py` & `bam-filter-1.4.7/bam_filter/utils.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.6/setup.cfg` & `bam-filter-1.4.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.6/setup.py` & `bam-filter-1.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.6/versioneer.py` & `bam-filter-1.4.7/versioneer.py`

 * *Files identical despite different names*

