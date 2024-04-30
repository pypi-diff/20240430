# Comparing `tmp/astromartini-2.0.8.tar.gz` & `tmp/astromartini-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromartini-2.0.8.tar", last modified: Sun Mar 24 12:49:31 2024, max compression
+gzip compressed data, was "astromartini-2.0.9.tar", last modified: Wed Mar 27 13:07:22 2024, max compression
```

## Comparing `astromartini-2.0.8.tar` & `astromartini-2.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 12:49:31.709078 astromartini-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-03-24 12:49:08.000000 astromartini-2.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-24 12:49:08.000000 astromartini-2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13003 2024-03-24 12:49:31.709078 astromartini-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-03-24 12:49:08.000000 astromartini-2.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 12:49:31.709078 astromartini-2.0.8/astromartini.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13003 2024-03-24 12:49:31.000000 astromartini-2.0.8/astromartini.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-24 12:49:31.000000 astromartini-2.0.8/astromartini.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 12:49:31.000000 astromartini-2.0.8/astromartini.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-24 12:49:31.000000 astromartini-2.0.8/astromartini.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-24 12:49:31.000000 astromartini-2.0.8/astromartini.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 12:49:31.705078 astromartini-2.0.8/martini/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/_demo.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/beams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/beams.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16064 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/datacube.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/datacube.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    44766 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/martini.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/martini.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/noise.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 12:49:31.705078 astromartini-2.0.8/martini/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sources/_L_align.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sources/_L_align.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sources/_cartesian_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sources/_cartesian_translation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sources/_illustris_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sources/colibre_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sources/eagle_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sources/magneticum_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sources/simba_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sources/so_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    20261 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sources/sph_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sources/sph_source.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sources/swiftgalaxy_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    14494 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sources/tng_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    14654 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/spectral_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/spectral_models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    58654 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sph_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-03-24 12:49:08.000000 astromartini-2.0.8/martini/sph_kernels.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-24 12:49:08.000000 astromartini-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 12:49:31.709078 astromartini-2.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 12:49:31.709078 astromartini-2.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-24 12:49:08.000000 astromartini-2.0.8/tests/test_beams.py
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-03-24 12:49:08.000000 astromartini-2.0.8/tests/test_datacube.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-24 12:49:08.000000 astromartini-2.0.8/tests/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-24 12:49:08.000000 astromartini-2.0.8/tests/test_fits_compliant.py
--rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-03-24 12:49:08.000000 astromartini-2.0.8/tests/test_martini.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-03-24 12:49:08.000000 astromartini-2.0.8/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    18930 2024-03-24 12:49:08.000000 astromartini-2.0.8/tests/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-03-24 12:49:08.000000 astromartini-2.0.8/tests/test_spectral_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12775 2024-03-24 12:49:08.000000 astromartini-2.0.8/tests/test_sph_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-03-24 12:49:08.000000 astromartini-2.0.8/tests/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:07:22.039995 astromartini-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-03-27 13:06:55.000000 astromartini-2.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-27 13:06:55.000000 astromartini-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13003 2024-03-27 13:07:22.039995 astromartini-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-03-27 13:06:55.000000 astromartini-2.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:07:22.035995 astromartini-2.0.9/astromartini.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13003 2024-03-27 13:07:22.000000 astromartini-2.0.9/astromartini.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-27 13:07:22.000000 astromartini-2.0.9/astromartini.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 13:07:22.000000 astromartini-2.0.9/astromartini.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-27 13:07:22.000000 astromartini-2.0.9/astromartini.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-27 13:07:22.000000 astromartini-2.0.9/astromartini.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:07:22.031995 astromartini-2.0.9/martini/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/_demo.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/beams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/beams.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16064 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/datacube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/datacube.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    44766 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/martini.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/martini.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/noise.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:07:22.035995 astromartini-2.0.9/martini/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sources/_L_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sources/_L_align.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sources/_cartesian_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sources/_cartesian_translation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sources/_illustris_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sources/colibre_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sources/eagle_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sources/magneticum_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sources/simba_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sources/so_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20261 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sources/sph_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sources/sph_source.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sources/swiftgalaxy_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14494 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sources/tng_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14654 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/spectral_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/spectral_models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    58654 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sph_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-03-27 13:06:55.000000 astromartini-2.0.9/martini/sph_kernels.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-27 13:06:55.000000 astromartini-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 13:07:22.039995 astromartini-2.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:07:22.035995 astromartini-2.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-27 13:06:55.000000 astromartini-2.0.9/tests/test_beams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-03-27 13:06:55.000000 astromartini-2.0.9/tests/test_datacube.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-27 13:06:55.000000 astromartini-2.0.9/tests/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-27 13:06:55.000000 astromartini-2.0.9/tests/test_fits_compliant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15304 2024-03-27 13:06:55.000000 astromartini-2.0.9/tests/test_martini.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-03-27 13:06:55.000000 astromartini-2.0.9/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18930 2024-03-27 13:06:55.000000 astromartini-2.0.9/tests/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-03-27 13:06:55.000000 astromartini-2.0.9/tests/test_spectral_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12728 2024-03-27 13:06:55.000000 astromartini-2.0.9/tests/test_sph_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-03-27 13:06:55.000000 astromartini-2.0.9/tests/test_write.py
```

### Comparing `astromartini-2.0.8/LICENSE.md` & `astromartini-2.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/PKG-INFO` & `astromartini-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromartini
-Version: 2.0.8
+Version: 2.0.9
 Summary: Synthetic datacube creation from simulations.
 Author-email: Kyle Oman <kyle.a.oman@durham.ac.uk>
 Project-URL: Homepage, https://github.com/kyleaoman/martini
 Project-URL: Bug Tracker, https://github.com/kyleaoman/martini/issues
 Project-URL: Documentation, https://martini.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `astromartini-2.0.8/README.rst` & `astromartini-2.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/astromartini.egg-info/PKG-INFO` & `astromartini-2.0.9/astromartini.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromartini
-Version: 2.0.8
+Version: 2.0.9
 Summary: Synthetic datacube creation from simulations.
 Author-email: Kyle Oman <kyle.a.oman@durham.ac.uk>
 Project-URL: Homepage, https://github.com/kyleaoman/martini
 Project-URL: Bug Tracker, https://github.com/kyleaoman/martini/issues
 Project-URL: Documentation, https://martini.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `astromartini-2.0.8/astromartini.egg-info/SOURCES.txt` & `astromartini-2.0.9/astromartini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/__init__.py` & `astromartini-2.0.9/martini/__init__.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/_demo.py` & `astromartini-2.0.9/martini/_demo.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/beams.py` & `astromartini-2.0.9/martini/beams.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/beams.pyi` & `astromartini-2.0.9/martini/beams.pyi`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/datacube.py` & `astromartini-2.0.9/martini/datacube.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/datacube.pyi` & `astromartini-2.0.9/martini/datacube.pyi`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/martini.py` & `astromartini-2.0.9/martini/martini.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/martini.pyi` & `astromartini-2.0.9/martini/martini.pyi`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/noise.py` & `astromartini-2.0.9/martini/noise.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,24 +49,24 @@
 
     Provides a `generate` method producing a cube of Gaussian noise.
 
     Parameters
     ----------
     rms : Quantity, with dimensions of flux density per beam
         Desired root mean square amplitude of the noise field after convolution with the
-        beam.
+        beam. (Default: 1.0 * U.Jy * U.beam ** -1)
 
     seed : int or None
         Seed for random number generator. If None, results will be unpredictable,
         if an integer is given results will be repeatable. (Default: None)
     """
 
     def __init__(
         self,
-        rms=1.0 * U.Jy * U.beam**-2,
+        rms=1.0 * U.Jy * U.beam**-1,
         seed=None,
     ):
         self.target_rms = rms
 
         super().__init__(seed=seed)
 
         return
```

### Comparing `astromartini-2.0.8/martini/noise.pyi` & `astromartini-2.0.9/martini/noise.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     def __init__(self, seed: T.Optional[int] = ...) -> None: ...
     @abstractmethod
     def generate(self, datacube: DataCube, beam: _BaseBeam): ...
     def reset_rng(self) -> None: ...
 
 class GaussianNoise(_BaseNoise):
-    rms: U.Quantity[U.Jy * U.arcsec**-2]
+    rms: U.Quantity[U.Jy * U.beam**-1]
 
     def __init__(
-        self, rms: U.Quantity[U.Jy * U.arcsec**-2] = ..., seed: T.Optional[int] = ...
+        self, rms: U.Quantity[U.Jy * U.beam**-1] = ..., seed: T.Optional[int] = ...
     ) -> None: ...
     def generate(
         self, datacube: DataCube, beam: _BaseBeam
     ) -> U.Quantity[U.Jy * U.arcsec**-2]: ...
```

### Comparing `astromartini-2.0.8/martini/sources/_L_align.py` & `astromartini-2.0.9/martini/sources/_L_align.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/sources/_cartesian_translation.py` & `astromartini-2.0.9/martini/sources/_cartesian_translation.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/sources/_illustris_tools.py` & `astromartini-2.0.9/martini/sources/_illustris_tools.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/sources/colibre_source.py` & `astromartini-2.0.9/martini/sources/colibre_source.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/sources/eagle_source.py` & `astromartini-2.0.9/martini/sources/eagle_source.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/sources/magneticum_source.py` & `astromartini-2.0.9/martini/sources/magneticum_source.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/sources/simba_source.py` & `astromartini-2.0.9/martini/sources/simba_source.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/sources/so_source.py` & `astromartini-2.0.9/martini/sources/so_source.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/sources/sph_source.py` & `astromartini-2.0.9/martini/sources/sph_source.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/sources/sph_source.pyi` & `astromartini-2.0.9/martini/sources/sph_source.pyi`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/sources/swiftgalaxy_source.py` & `astromartini-2.0.9/martini/sources/swiftgalaxy_source.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/sources/tng_source.py` & `astromartini-2.0.9/martini/sources/tng_source.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/spectral_models.py` & `astromartini-2.0.9/martini/spectral_models.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/spectral_models.pyi` & `astromartini-2.0.9/martini/spectral_models.pyi`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/sph_kernels.py` & `astromartini-2.0.9/martini/sph_kernels.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/martini/sph_kernels.pyi` & `astromartini-2.0.9/martini/sph_kernels.pyi`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/pyproject.toml` & `astromartini-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "astromartini"
-version = "2.0.8"
+version = "2.0.9"
 authors = [
     { name="Kyle Oman", email="kyle.a.oman@durham.ac.uk" },
 ]
 description="Synthetic datacube creation from simulations."
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `astromartini-2.0.8/tests/test_beams.py` & `astromartini-2.0.9/tests/test_beams.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/tests/test_datacube.py` & `astromartini-2.0.9/tests/test_datacube.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/tests/test_demo.py` & `astromartini-2.0.9/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/tests/test_fits_compliant.py` & `astromartini-2.0.9/tests/test_fits_compliant.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/tests/test_martini.py` & `astromartini-2.0.9/tests/test_martini.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,17 @@
         assert m.datacube._array.shape == expected_shape
 
     def test_preview(self, m_init):
         """
         Simply check that the preview visualisation runs without error.
         """
         # with default arguments
-        m_init.preview()
+        with pytest.warns(UserWarning, match="singular"):
+            # warning: single-particle source is used, so axis limits try to be equal
+            m_init.preview()
         # with non-default arguments
         m_init.preview(
             max_points=1000,
             fig=2,
             lim="datacube",
             vlim="datacube",
             point_scaling="fixed",
```

### Comparing `astromartini-2.0.8/tests/test_noise.py` & `astromartini-2.0.9/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/tests/test_sources.py` & `astromartini-2.0.9/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/tests/test_spectral_models.py` & `astromartini-2.0.9/tests/test_spectral_models.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.8/tests/test_sph_kernels.py` & `astromartini-2.0.9/tests/test_sph_kernels.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,14 @@
     CubicSplineKernel,
     GaussianKernel,
     QuarticSplineKernel,
 )
 adaptive_kernels = recommended_kernels + (_AdaptiveKernel,)
 all_kernels = simple_kernels + adaptive_kernels
 
-for k in all_kernels:
-    k.noFWHMwarn = True
-
 
 def total_kernel_weight(k, h, ngrid=50):
     r = np.arange(0, ngrid)
     dr = (r[1] - r[0]) * U.pix
     xgrid, ygrid = np.meshgrid(np.r_[r[1:][::-1], r], np.r_[r[1:][::-1], r])
     dij = np.vstack((xgrid.flatten(), ygrid.flatten()))
     k.sm_lengths = np.ones(dij.shape[1]) * h * U.pix
```

### Comparing `astromartini-2.0.8/tests/test_write.py` & `astromartini-2.0.9/tests/test_write.py`

 * *Files identical despite different names*

