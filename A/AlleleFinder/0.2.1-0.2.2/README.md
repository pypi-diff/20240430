# Comparing `tmp/allelefinder-0.2.1.tar.gz` & `tmp/allelefinder-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allelefinder-0.2.1.tar", last modified: Tue Apr 30 13:59:01 2024, max compression
+gzip compressed data, was "allelefinder-0.2.2.tar", last modified: Tue Apr 30 14:11:40 2024, max compression
```

## Comparing `allelefinder-0.2.1.tar` & `allelefinder-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:59:01.329594 allelefinder-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:59:01.329594 allelefinder-0.2.1/AlleleFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-30 13:59:01.000000 allelefinder-0.2.1/AlleleFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-30 13:59:01.000000 allelefinder-0.2.1/AlleleFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:59:01.000000 allelefinder-0.2.1/AlleleFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-30 13:59:01.000000 allelefinder-0.2.1/AlleleFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 13:59:01.000000 allelefinder-0.2.1/AlleleFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-30 13:58:53.000000 allelefinder-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 13:58:53.000000 allelefinder-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-30 13:59:01.329594 allelefinder-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-30 13:58:53.000000 allelefinder-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:59:01.325594 allelefinder-0.2.1/allele_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:58:53.000000 allelefinder-0.2.1/allele_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26836 2024-04-30 13:58:53.000000 allelefinder-0.2.1/allele_tools/allele_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    38776 2024-04-30 13:58:53.000000 allelefinder-0.2.1/allele_tools/allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-04-30 13:58:53.000000 allelefinder-0.2.1/allele_tools/allele_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)   121713 2024-04-30 13:58:53.000000 allelefinder-0.2.1/allele_tools/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-04-30 13:58:53.000000 allelefinder-0.2.1/allele_tools/profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    53101 2024-04-30 13:58:53.000000 allelefinder-0.2.1/allele_tools/stec.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 13:58:53.000000 allelefinder-0.2.1/allele_tools/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-30 13:58:53.000000 allelefinder-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:59:01.329594 allelefinder-0.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2048 2024-04-30 13:58:53.000000 allelefinder-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:59:01.329594 allelefinder-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:58:53.000000 allelefinder-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-04-30 13:58:53.000000 allelefinder-0.2.1/tests/test_0_profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-04-30 13:58:53.000000 allelefinder-0.2.1/tests/test_1_allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-04-30 13:58:53.000000 allelefinder-0.2.1/tests/test_2_allele_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-30 13:58:53.000000 allelefinder-0.2.1/tests/test_3_stec_profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-30 13:58:53.000000 allelefinder-0.2.1/tests/test_4_stec_allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-30 13:58:53.000000 allelefinder-0.2.1/tests/test_5_stec_allele_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-30 13:58:53.000000 allelefinder-0.2.1/tests/test_6_stec_aa_allele_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-30 13:58:53.000000 allelefinder-0.2.1/tests/test_7_stec_allele_split.py
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-30 13:58:53.000000 allelefinder-0.2.1/tests/test_8_stec_allele_concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-30 13:58:53.000000 allelefinder-0.2.1/tests/test_9_stec_allele_translate_find.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:11:40.934442 allelefinder-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:11:40.934442 allelefinder-0.2.2/AlleleFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-30 14:11:40.000000 allelefinder-0.2.2/AlleleFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-30 14:11:40.000000 allelefinder-0.2.2/AlleleFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:11:40.000000 allelefinder-0.2.2/AlleleFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-30 14:11:40.000000 allelefinder-0.2.2/AlleleFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 14:11:40.000000 allelefinder-0.2.2/AlleleFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-30 14:11:29.000000 allelefinder-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 14:11:29.000000 allelefinder-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-30 14:11:40.934442 allelefinder-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-30 14:11:29.000000 allelefinder-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:11:40.934442 allelefinder-0.2.2/allele_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:11:29.000000 allelefinder-0.2.2/allele_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26836 2024-04-30 14:11:29.000000 allelefinder-0.2.2/allele_tools/allele_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38776 2024-04-30 14:11:29.000000 allelefinder-0.2.2/allele_tools/allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-04-30 14:11:29.000000 allelefinder-0.2.2/allele_tools/allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121713 2024-04-30 14:11:29.000000 allelefinder-0.2.2/allele_tools/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-04-30 14:11:29.000000 allelefinder-0.2.2/allele_tools/profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53101 2024-04-30 14:11:29.000000 allelefinder-0.2.2/allele_tools/stec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 14:11:29.000000 allelefinder-0.2.2/allele_tools/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-30 14:11:29.000000 allelefinder-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:11:40.934442 allelefinder-0.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2048 2024-04-30 14:11:29.000000 allelefinder-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:11:40.934442 allelefinder-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:11:29.000000 allelefinder-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-04-30 14:11:29.000000 allelefinder-0.2.2/tests/test_0_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-04-30 14:11:29.000000 allelefinder-0.2.2/tests/test_1_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-04-30 14:11:29.000000 allelefinder-0.2.2/tests/test_2_allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-30 14:11:29.000000 allelefinder-0.2.2/tests/test_3_stec_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-30 14:11:29.000000 allelefinder-0.2.2/tests/test_4_stec_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-30 14:11:29.000000 allelefinder-0.2.2/tests/test_5_stec_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-30 14:11:29.000000 allelefinder-0.2.2/tests/test_6_stec_aa_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-30 14:11:29.000000 allelefinder-0.2.2/tests/test_7_stec_allele_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-30 14:11:29.000000 allelefinder-0.2.2/tests/test_8_stec_allele_concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-30 14:11:29.000000 allelefinder-0.2.2/tests/test_9_stec_allele_translate_find.py
```

### Comparing `allelefinder-0.2.1/AlleleFinder.egg-info/PKG-INFO` & `allelefinder-0.2.2/AlleleFinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlleleFinder
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/OLC-Bioinformatics/AlleleFinder
 Author: Adam Koziol
 Author-email: adam.koziol@inspection.gc.ca
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `allelefinder-0.2.1/AlleleFinder.egg-info/SOURCES.txt` & `allelefinder-0.2.2/AlleleFinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/LICENSE` & `allelefinder-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/PKG-INFO` & `allelefinder-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlleleFinder
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/OLC-Bioinformatics/AlleleFinder
 Author: Adam Koziol
 Author-email: adam.koziol@inspection.gc.ca
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `allelefinder-0.2.1/README.md` & `allelefinder-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/allele_tools/allele_profiler.py` & `allelefinder-0.2.2/allele_tools/allele_profiler.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/allele_tools/allele_translate_reduce.py` & `allelefinder-0.2.2/allele_tools/allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/allele_tools/allele_updater.py` & `allelefinder-0.2.2/allele_tools/allele_updater.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/allele_tools/methods.py` & `allelefinder-0.2.2/allele_tools/methods.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/allele_tools/profile_reduce.py` & `allelefinder-0.2.2/allele_tools/profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/allele_tools/stec.py` & `allelefinder-0.2.2/allele_tools/stec.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/setup.py` & `allelefinder-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/tests/test_0_profile_reduce.py` & `allelefinder-0.2.2/tests/test_0_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/tests/test_1_allele_translate_reduce.py` & `allelefinder-0.2.2/tests/test_1_allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/tests/test_2_allele_updater.py` & `allelefinder-0.2.2/tests/test_2_allele_updater.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/tests/test_3_stec_profile_reduce.py` & `allelefinder-0.2.2/tests/test_3_stec_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/tests/test_4_stec_allele_translate_reduce.py` & `allelefinder-0.2.2/tests/test_4_stec_allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/tests/test_5_stec_allele_find.py` & `allelefinder-0.2.2/tests/test_5_stec_allele_find.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/tests/test_6_stec_aa_allele_find.py` & `allelefinder-0.2.2/tests/test_6_stec_aa_allele_find.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/tests/test_7_stec_allele_split.py` & `allelefinder-0.2.2/tests/test_7_stec_allele_split.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/tests/test_8_stec_allele_concatenate.py` & `allelefinder-0.2.2/tests/test_8_stec_allele_concatenate.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.1/tests/test_9_stec_allele_translate_find.py` & `allelefinder-0.2.2/tests/test_9_stec_allele_translate_find.py`

 * *Files identical despite different names*

