# Comparing `tmp/rgbloom-1.8.tar.gz` & `tmp/rgbloom-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgbloom-1.8.tar", last modified: Thu Apr 25 14:27:12 2024, max compression
+gzip compressed data, was "rgbloom-1.9.tar", last modified: Tue Apr 30 11:17:39 2024, max compression
```

## Comparing `rgbloom-1.8.tar` & `rgbloom-1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-25 14:27:12.110639 rgbloom-1.8/
--rw-r--r--   0 cardiel    (501) staff       (20)    35149 2022-11-06 08:36:25.000000 rgbloom-1.8/LICENSE
--rw-r--r--   0 cardiel    (501) staff       (20)    14558 2024-04-25 14:27:12.110436 rgbloom-1.8/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)    13559 2023-09-27 17:14:08.000000 rgbloom-1.8/README.md
--rw-r--r--   0 cardiel    (501) staff       (20)      100 2022-11-06 08:38:35.000000 rgbloom-1.8/pyproject.toml
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-25 14:27:12.103166 rgbloom-1.8/rgbloom/
--rw-r--r--   0 cardiel    (501) staff       (20)       51 2022-11-06 08:39:16.000000 rgbloom-1.8/rgbloom/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)     6597 2023-05-24 13:46:56.000000 rgbloom-1.8/rgbloom/__main__.py
--rw-r--r--   0 cardiel    (501) staff       (20)      439 2023-05-25 06:38:09.000000 rgbloom-1.8/rgbloom/choices_mag_plot.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-25 14:27:12.108018 rgbloom-1.8/rgbloom/core/
--rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.8/rgbloom/core/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)     2735 2024-04-25 14:25:02.000000 rgbloom-1.8/rgbloom/core/step1.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1844 2022-11-06 08:39:16.000000 rgbloom-1.8/rgbloom/core/step2.py
--rw-r--r--   0 cardiel    (501) staff       (20)     3128 2023-03-21 17:40:50.000000 rgbloom-1.8/rgbloom/core/step3.py
--rw-r--r--   0 cardiel    (501) staff       (20)     2560 2022-11-06 08:39:16.000000 rgbloom-1.8/rgbloom/core/step4.py
--rw-r--r--   0 cardiel    (501) staff       (20)     3007 2023-03-21 17:42:15.000000 rgbloom-1.8/rgbloom/core/step5.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-25 14:27:12.109166 rgbloom-1.8/rgbloom/gui/
--rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.8/rgbloom/gui/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)    13610 2023-05-25 08:32:56.000000 rgbloom-1.8/rgbloom/gui/step6.py
--rw-r--r--   0 cardiel    (501) staff       (20)      497 2022-11-06 08:39:16.000000 rgbloom-1.8/rgbloom/gui/style.py
--rw-r--r--   0 cardiel    (501) staff       (20)      171 2024-04-25 14:25:02.000000 rgbloom-1.8/rgbloom/version.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-25 14:27:12.109742 rgbloom-1.8/rgbloom.egg-info/
--rw-r--r--   0 cardiel    (501) staff       (20)    14558 2024-04-25 14:27:12.000000 rgbloom-1.8/rgbloom.egg-info/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)      527 2024-04-25 14:27:12.000000 rgbloom-1.8/rgbloom.egg-info/SOURCES.txt
--rw-r--r--   0 cardiel    (501) staff       (20)        1 2024-04-25 14:27:12.000000 rgbloom-1.8/rgbloom.egg-info/dependency_links.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       50 2024-04-25 14:27:12.000000 rgbloom-1.8/rgbloom.egg-info/entry_points.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       80 2024-04-25 14:27:12.000000 rgbloom-1.8/rgbloom.egg-info/requires.txt
--rw-r--r--   0 cardiel    (501) staff       (20)        8 2024-04-25 14:27:12.000000 rgbloom-1.8/rgbloom.egg-info/top_level.txt
--rw-r--r--   0 cardiel    (501) staff       (20)     1040 2024-04-25 14:27:12.111186 rgbloom-1.8/setup.cfg
--rw-r--r--   0 cardiel    (501) staff       (20)       68 2022-11-06 08:39:44.000000 rgbloom-1.8/setup.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-30 11:17:39.000890 rgbloom-1.9/
+-rw-r--r--   0 cardiel    (501) staff       (20)    35149 2022-11-06 08:36:25.000000 rgbloom-1.9/LICENSE
+-rw-r--r--   0 cardiel    (501) staff       (20)    14562 2024-04-30 11:17:39.000764 rgbloom-1.9/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)    13563 2024-04-30 11:16:01.000000 rgbloom-1.9/README.md
+-rw-r--r--   0 cardiel    (501) staff       (20)      100 2022-11-06 08:38:35.000000 rgbloom-1.9/pyproject.toml
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-30 11:17:38.998294 rgbloom-1.9/rgbloom/
+-rw-r--r--   0 cardiel    (501) staff       (20)       51 2022-11-06 08:39:16.000000 rgbloom-1.9/rgbloom/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     6597 2023-05-24 13:46:56.000000 rgbloom-1.9/rgbloom/__main__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      439 2023-05-25 06:38:09.000000 rgbloom-1.9/rgbloom/choices_mag_plot.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-30 11:17:38.999733 rgbloom-1.9/rgbloom/core/
+-rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.9/rgbloom/core/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2735 2024-04-25 14:25:02.000000 rgbloom-1.9/rgbloom/core/step1.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1844 2022-11-06 08:39:16.000000 rgbloom-1.9/rgbloom/core/step2.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     3128 2023-03-21 17:40:50.000000 rgbloom-1.9/rgbloom/core/step3.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2567 2024-04-30 11:16:01.000000 rgbloom-1.9/rgbloom/core/step4.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     3008 2024-04-30 11:16:01.000000 rgbloom-1.9/rgbloom/core/step5.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-30 11:17:39.000106 rgbloom-1.9/rgbloom/gui/
+-rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.9/rgbloom/gui/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)    13611 2024-04-30 11:16:01.000000 rgbloom-1.9/rgbloom/gui/step6.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      497 2022-11-06 08:39:16.000000 rgbloom-1.9/rgbloom/gui/style.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      171 2024-04-30 11:16:01.000000 rgbloom-1.9/rgbloom/version.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-30 11:17:39.000433 rgbloom-1.9/rgbloom.egg-info/
+-rw-r--r--   0 cardiel    (501) staff       (20)    14562 2024-04-30 11:17:38.000000 rgbloom-1.9/rgbloom.egg-info/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)      527 2024-04-30 11:17:38.000000 rgbloom-1.9/rgbloom.egg-info/SOURCES.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)        1 2024-04-30 11:17:38.000000 rgbloom-1.9/rgbloom.egg-info/dependency_links.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       50 2024-04-30 11:17:38.000000 rgbloom-1.9/rgbloom.egg-info/entry_points.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       80 2024-04-30 11:17:38.000000 rgbloom-1.9/rgbloom.egg-info/requires.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)        8 2024-04-30 11:17:38.000000 rgbloom-1.9/rgbloom.egg-info/top_level.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)     1040 2024-04-30 11:17:39.001172 rgbloom-1.9/setup.cfg
+-rw-r--r--   0 cardiel    (501) staff       (20)       68 2022-11-06 08:39:44.000000 rgbloom-1.9/setup.py
```

### Comparing `rgbloom-1.8/LICENSE` & `rgbloom-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rgbloom-1.8/PKG-INFO` & `rgbloom-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgbloom
-Version: 1.8
+Version: 1.9
 Summary: RGB from Gaia EDR3
 Home-page: https://github.com/guaix-ucm/rgbloom
 Author: Nicolás Cardiel
 Author-email: cardiel@ucm.es
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -108,15 +108,15 @@
 specific location unless you want to delete these files to free up disk space.
 
 The execution of this example should led to the following output in the
 terminal (except for the absolute path where the auxiliary downloaded files 
 are stored):
 
 ```
-        Welcome to rgbloom version 1.7
+        Welcome to rgbloom version 1.9
         ==============================
 
 Downloading data from 'http://nartex.fis.ucm.es/~ncl/rgbphot/gaiaDR3/reference_healpix8.csv' to file '/Users/cardiel/Library/Caches/pooch/635cd722cf61b23bd8eee20635e4d580-reference_healpix8.csv'.
 <STEP1> Starting cone search in Gaia DR3... (please wait)
   INFO: Query finished. [astroquery.utils.tap.core]
         --> 310 objects found
         --> 23 objects classified as VARIABLE
@@ -124,18 +124,18 @@
 <STEP3> Retrieving objects from the 200M sample in the enclosing HEALPIx level-8 tables
 Downloading data from 'http://nartex.fis.ucm.es/~ncl/rgbphot/gaiaDR3/RGBsynthetic_NOVARIABLES/sortida_XpContinuousMeanSpectrum_006602-007952_RGB_NOVARIABLES_final.csv.gz' to file '/Users/cardiel/Library/Caches/pooch/2d94d5acfcb380d6dff1eaa207caa086-sortida_XpContinuousMeanSpectrum_006602-007952_RGB_NOVARIABLES_final.csv.gz'.
         * Required file: /Users/cardiel/Library/Caches/pooch/2d94d5acfcb380d6dff1eaa207caa086-sortida_XpContinuousMeanSpectrum_006602-007952_RGB_NOVARIABLES_final.csv.gz
           md5:f9cf7ed0f84eecda13ef6a408d291b96
         --> Number of objects: 100553
         --> Total number of objects: 100553
 <STEP4> Cross-matching DR3 with 200M sample
-        --> Number of objects in the 200M subsample............: 100553
-        --> Number of objects in DR3 query.....................: 310
-        --> Number of DR3 objects within the 200M sample.......: 248
-        --> Number of DR3 objects no present in the 200M sample: 62
+        --> Number of objects in the 200M subsample.............: 100553
+        --> Number of objects in DR3 query......................: 310
+        --> Number of DR3 objects within the 200M sample........: 248
+        --> Number of DR3 objects not present in the 200M sample: 62
 <STEP5> Saving output CSV files
         --> file rgbloom_200m.csv saved
         --> file rgbloom_no200m.csv saved
 <STEP6> Generating PDF plot
 End of program
 ```
```

### Comparing `rgbloom-1.8/README.md` & `rgbloom-1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 specific location unless you want to delete these files to free up disk space.
 
 The execution of this example should led to the following output in the
 terminal (except for the absolute path where the auxiliary downloaded files 
 are stored):
 
 ```
-        Welcome to rgbloom version 1.7
+        Welcome to rgbloom version 1.9
         ==============================
 
 Downloading data from 'http://nartex.fis.ucm.es/~ncl/rgbphot/gaiaDR3/reference_healpix8.csv' to file '/Users/cardiel/Library/Caches/pooch/635cd722cf61b23bd8eee20635e4d580-reference_healpix8.csv'.
 <STEP1> Starting cone search in Gaia DR3... (please wait)
   INFO: Query finished. [astroquery.utils.tap.core]
         --> 310 objects found
         --> 23 objects classified as VARIABLE
@@ -94,18 +94,18 @@
 <STEP3> Retrieving objects from the 200M sample in the enclosing HEALPIx level-8 tables
 Downloading data from 'http://nartex.fis.ucm.es/~ncl/rgbphot/gaiaDR3/RGBsynthetic_NOVARIABLES/sortida_XpContinuousMeanSpectrum_006602-007952_RGB_NOVARIABLES_final.csv.gz' to file '/Users/cardiel/Library/Caches/pooch/2d94d5acfcb380d6dff1eaa207caa086-sortida_XpContinuousMeanSpectrum_006602-007952_RGB_NOVARIABLES_final.csv.gz'.
         * Required file: /Users/cardiel/Library/Caches/pooch/2d94d5acfcb380d6dff1eaa207caa086-sortida_XpContinuousMeanSpectrum_006602-007952_RGB_NOVARIABLES_final.csv.gz
           md5:f9cf7ed0f84eecda13ef6a408d291b96
         --> Number of objects: 100553
         --> Total number of objects: 100553
 <STEP4> Cross-matching DR3 with 200M sample
-        --> Number of objects in the 200M subsample............: 100553
-        --> Number of objects in DR3 query.....................: 310
-        --> Number of DR3 objects within the 200M sample.......: 248
-        --> Number of DR3 objects no present in the 200M sample: 62
+        --> Number of objects in the 200M subsample.............: 100553
+        --> Number of objects in DR3 query......................: 310
+        --> Number of DR3 objects within the 200M sample........: 248
+        --> Number of DR3 objects not present in the 200M sample: 62
 <STEP5> Saving output CSV files
         --> file rgbloom_200m.csv saved
         --> file rgbloom_no200m.csv saved
 <STEP6> Generating PDF plot
 End of program
 ```
```

### Comparing `rgbloom-1.8/rgbloom/__main__.py` & `rgbloom-1.9/rgbloom/__main__.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.8/rgbloom/core/step1.py` & `rgbloom-1.9/rgbloom/core/step1.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.8/rgbloom/core/step2.py` & `rgbloom-1.9/rgbloom/core/step2.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.8/rgbloom/core/step3.py` & `rgbloom-1.9/rgbloom/core/step3.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.8/rgbloom/core/step4.py` & `rgbloom-1.9/rgbloom/core/step4.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,35 +27,35 @@
         If True, display additional information.
 
     Returns
     -------
     r_dr3_200m : astropy Table
         Objects in both the DR3 query and the 200M sample.
     r_dr3_no200m : astropy Table
-        Objects in the DR3 query no present in the 200M sample.
+        Objects in the DR3 query not present in the 200M sample.
 
     """
     print('<STEP4> Cross-matching DR3 with 200M sample')
 
     r_200m.rename_column('sourceid', 'source_id')
 
     # objects in DR3 query also available in the 200M sample
     r_dr3_200m = join(r_dr3, r_200m, keys='source_id', join_type='inner')
 
     # all objects in DR3 query with data from the 200M sample when available,
-    # or with missing entries when no present in the 200M sample
+    # or with missing entries when not present in the 200M sample
     r_dr3_all = join(r_dr3, r_200m, keys='source_id', join_type='left')
 
-    # objects in DR3 query no present in the 200M sample
+    # objects in DR3 query not present in the 200M sample
     r_dr3_no200m = setdiff(r_dr3_all, r_dr3_200m, keys=['source_id'])
 
-    print(f'        --> Number of objects in the 200M subsample............: {len(r_200m)}')
-    print(f'        --> Number of objects in DR3 query.....................: {len(r_dr3_all)}')
-    print(f'        --> Number of DR3 objects within the 200M sample.......: {len(r_dr3_200m)}')
-    print(f'        --> Number of DR3 objects no present in the 200M sample: {len(r_dr3_no200m)}')
+    print(f'        --> Number of objects in the 200M subsample.............: {len(r_200m)}')
+    print(f'        --> Number of objects in DR3 query......................: {len(r_dr3_all)}')
+    print(f'        --> Number of DR3 objects within the 200M sample........: {len(r_dr3_200m)}')
+    print(f'        --> Number of DR3 objects not present in the 200M sample: {len(r_dr3_no200m)}')
 
     # sort tables by RA
     r_dr3_all.sort('ra')
     r_dr3_200m.sort('ra')
     r_dr3_no200m.sort('ra')
 
     # include first column with sequential number (useful for the plot)
```

### Comparing `rgbloom-1.8/rgbloom/core/step5.py` & `rgbloom-1.9/rgbloom/core/step5.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Generate output CSV files
 
     Parameters
     ----------
     r_dr3_200m : astropy Table
         Objects in both the DR3 query and the 200M sample.
     r_dr3_no200m : astropy Table
-        Objects in the DR3 query no present in the 200M sample.
+        Objects in the DR3 query not present in the 200M sample.
     basename : str
         Base name for output files.
     verbose : bool
         If True, display additional information.
 
     """
```

### Comparing `rgbloom-1.8/rgbloom/gui/step6.py` & `rgbloom-1.9/rgbloom/gui/step6.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     """Perform EDR3 query
 
     Parameters
     ----------
     r_dr3_200m : astropy Table
         Objects in both the DR3 query and the 200M sample.
     r_dr3_no200m : astropy Table
-        Objects in the DR3 query no present in the 200M sample.
+        Objects in the DR3 query not present in the 200M sample.
     ra_center : float
         Right ascension (decimal degree) corresponding to the center
         of the field of view.
     dec_center : float
         Declination (decimal degree) corresponding to the center
         of the field of view.
     search_radius : float
```

### Comparing `rgbloom-1.8/rgbloom.egg-info/PKG-INFO` & `rgbloom-1.9/rgbloom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgbloom
-Version: 1.8
+Version: 1.9
 Summary: RGB from Gaia EDR3
 Home-page: https://github.com/guaix-ucm/rgbloom
 Author: Nicolás Cardiel
 Author-email: cardiel@ucm.es
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -108,15 +108,15 @@
 specific location unless you want to delete these files to free up disk space.
 
 The execution of this example should led to the following output in the
 terminal (except for the absolute path where the auxiliary downloaded files 
 are stored):
 
 ```
-        Welcome to rgbloom version 1.7
+        Welcome to rgbloom version 1.9
         ==============================
 
 Downloading data from 'http://nartex.fis.ucm.es/~ncl/rgbphot/gaiaDR3/reference_healpix8.csv' to file '/Users/cardiel/Library/Caches/pooch/635cd722cf61b23bd8eee20635e4d580-reference_healpix8.csv'.
 <STEP1> Starting cone search in Gaia DR3... (please wait)
   INFO: Query finished. [astroquery.utils.tap.core]
         --> 310 objects found
         --> 23 objects classified as VARIABLE
@@ -124,18 +124,18 @@
 <STEP3> Retrieving objects from the 200M sample in the enclosing HEALPIx level-8 tables
 Downloading data from 'http://nartex.fis.ucm.es/~ncl/rgbphot/gaiaDR3/RGBsynthetic_NOVARIABLES/sortida_XpContinuousMeanSpectrum_006602-007952_RGB_NOVARIABLES_final.csv.gz' to file '/Users/cardiel/Library/Caches/pooch/2d94d5acfcb380d6dff1eaa207caa086-sortida_XpContinuousMeanSpectrum_006602-007952_RGB_NOVARIABLES_final.csv.gz'.
         * Required file: /Users/cardiel/Library/Caches/pooch/2d94d5acfcb380d6dff1eaa207caa086-sortida_XpContinuousMeanSpectrum_006602-007952_RGB_NOVARIABLES_final.csv.gz
           md5:f9cf7ed0f84eecda13ef6a408d291b96
         --> Number of objects: 100553
         --> Total number of objects: 100553
 <STEP4> Cross-matching DR3 with 200M sample
-        --> Number of objects in the 200M subsample............: 100553
-        --> Number of objects in DR3 query.....................: 310
-        --> Number of DR3 objects within the 200M sample.......: 248
-        --> Number of DR3 objects no present in the 200M sample: 62
+        --> Number of objects in the 200M subsample.............: 100553
+        --> Number of objects in DR3 query......................: 310
+        --> Number of DR3 objects within the 200M sample........: 248
+        --> Number of DR3 objects not present in the 200M sample: 62
 <STEP5> Saving output CSV files
         --> file rgbloom_200m.csv saved
         --> file rgbloom_no200m.csv saved
 <STEP6> Generating PDF plot
 End of program
 ```
```

### Comparing `rgbloom-1.8/rgbloom.egg-info/SOURCES.txt` & `rgbloom-1.9/rgbloom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rgbloom-1.8/setup.cfg` & `rgbloom-1.9/setup.cfg`

 * *Files identical despite different names*

