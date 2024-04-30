# Comparing `tmp/tif_to_zarr-0.2.tar.gz` & `tmp/tif_to_zarr-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tif_to_zarr-0.2.tar", last modified: Mon Apr 29 21:35:17 2024, max compression
+gzip compressed data, was "tif_to_zarr-0.3.tar", last modified: Mon Apr 29 21:39:14 2024, max compression
```

## Comparing `tif_to_zarr-0.2.tar` & `tif_to_zarr-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 zubovy   (65918) cellmap   (1127)        0 2024-04-29 21:35:17.568539 tif_to_zarr-0.2/
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1518 2024-04-29 20:35:53.000000 tif_to_zarr-0.2/LICENSE
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1319 2024-04-29 21:35:17.568539 tif_to_zarr-0.2/PKG-INFO
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)      924 2024-04-29 20:13:11.000000 tif_to_zarr-0.2/README.md
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)      516 2024-04-29 20:13:11.000000 tif_to_zarr-0.2/pyproject.toml
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)       38 2024-04-29 21:35:17.568539 tif_to_zarr-0.2/setup.cfg
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)      717 2024-04-29 21:35:14.000000 tif_to_zarr-0.2/setup.py
-drwxr-xr-x   0 zubovy   (65918) cellmap   (1127)        0 2024-04-29 21:35:17.568539 tif_to_zarr-0.2/tif_to_zarr.egg-info/
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1319 2024-04-29 21:35:17.000000 tif_to_zarr-0.2/tif_to_zarr.egg-info/PKG-INFO
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)      215 2024-04-29 21:35:17.000000 tif_to_zarr-0.2/tif_to_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)        1 2024-04-29 21:35:17.000000 tif_to_zarr-0.2/tif_to_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)       45 2024-04-29 21:35:17.000000 tif_to_zarr-0.2/tif_to_zarr.egg-info/requires.txt
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)        1 2024-04-29 21:35:17.000000 tif_to_zarr-0.2/tif_to_zarr.egg-info/top_level.txt
+drwxr-xr-x   0 zubovy   (65918) cellmap   (1127)        0 2024-04-29 21:39:14.091232 tif_to_zarr-0.3/
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1518 2024-04-29 20:35:53.000000 tif_to_zarr-0.3/LICENSE
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1322 2024-04-29 21:39:14.091232 tif_to_zarr-0.3/PKG-INFO
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)      924 2024-04-29 20:13:11.000000 tif_to_zarr-0.3/README.md
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)      516 2024-04-29 20:13:11.000000 tif_to_zarr-0.3/pyproject.toml
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)       38 2024-04-29 21:39:14.091232 tif_to_zarr-0.3/setup.cfg
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)      698 2024-04-29 21:39:04.000000 tif_to_zarr-0.3/setup.py
+drwxr-xr-x   0 zubovy   (65918) cellmap   (1127)        0 2024-04-29 21:39:14.091232 tif_to_zarr-0.3/tif_to_zarr.egg-info/
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1322 2024-04-29 21:39:14.000000 tif_to_zarr-0.3/tif_to_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)      215 2024-04-29 21:39:14.000000 tif_to_zarr-0.3/tif_to_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)        1 2024-04-29 21:39:14.000000 tif_to_zarr-0.3/tif_to_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)       37 2024-04-29 21:39:14.000000 tif_to_zarr-0.3/tif_to_zarr.egg-info/requires.txt
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)        1 2024-04-29 21:39:14.000000 tif_to_zarr-0.3/tif_to_zarr.egg-info/top_level.txt
```

### Comparing `tif_to_zarr-0.2/LICENSE` & `tif_to_zarr-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tif_to_zarr-0.2/PKG-INFO` & `tif_to_zarr-0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: tif_to_zarr
-Version: 0.2
-Summary: Simple package to convert small tif files to zarr format.
-Home-page: https://github.com/yuriyzubov/tif-to-zarr.git
-Author: Yurii Zubov
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: imagecodecs
-Requires-Dist: click
-Requires-Dist: zarr
-Requires-Dist: dask
-Requires-Dist: tifffile
-Requires-Dist: logging
-
 This script could be used for conversion of a .tiff file to .zarr format with OME-NGFF multiscales metadata structure.
 #### How to run
 1. open command line terminal
 2. install poetry tool for dependency management and packaging: https://pypi.org/project/poetry/
 3. switch to the tif_to_zarr directory:
     ``cd PATH_TO_DIRECTORY/tif_to_zarr``
 4. install python dependencies:
```

### Comparing `tif_to_zarr-0.2/README.md` & `tif_to_zarr-0.3/tif_to_zarr.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,24 @@
-This script could be used for conversion of a .tiff file to .zarr format with OME-NGFF multiscales metadata structure.
-#### How to run
-1. open command line terminal
-2. install poetry tool for dependency management and packaging: https://pypi.org/project/poetry/
-3. switch to the tif_to_zarr directory:
-    ``cd PATH_TO_DIRECTORY/tif_to_zarr``
-4. install python dependencies:
-    ``poetry install``
-5. run script using cli:
-    ``poetry run python src/tif_to_zarr.py --src=PATH_TO_SOURCE_DIRECTORY/input_file.tif --dest=PATH_TO_DEST_DIRECTORY/output_file.zarr``
-6. to convert a tiff file to zarr with custom metadata values, you can run smthg similar to this:
-``poetry run python3 src/tif_to_zarr.py --src=path_to_source_tif  --dest=path_to_output_zarr -a x z y -t 1.0 2.0 3.0 -s 4.0 5.0 6.0 -u nanometer nanometer nanometer``
-7. To get the list of options, you may run this:
-``poetry run python3 src/tif_to_zarr.py --help``
+Metadata-Version: 2.1
+Name: tif-to-zarr
+Version: 0.3
+Summary: Simple package to convert small tif files to zarr format.
+Home-page: https://github.com/yuriyzubov/tif-to-zarr.git
+Author: Yurii Zubov
+License: UNKNOWN
+Description: This script could be used for conversion of a .tiff file to .zarr format with OME-NGFF multiscales metadata structure.
+        #### How to run
+        1. open command line terminal
+        2. install poetry tool for dependency management and packaging: https://pypi.org/project/poetry/
+        3. switch to the tif_to_zarr directory:
+            ``cd PATH_TO_DIRECTORY/tif_to_zarr``
+        4. install python dependencies:
+            ``poetry install``
+        5. run script using cli:
+            ``poetry run python src/tif_to_zarr.py --src=PATH_TO_SOURCE_DIRECTORY/input_file.tif --dest=PATH_TO_DEST_DIRECTORY/output_file.zarr``
+        6. to convert a tiff file to zarr with custom metadata values, you can run smthg similar to this:
+        ``poetry run python3 src/tif_to_zarr.py --src=path_to_source_tif  --dest=path_to_output_zarr -a x z y -t 1.0 2.0 3.0 -s 4.0 5.0 6.0 -u nanometer nanometer nanometer``
+        7. To get the list of options, you may run this:
+        ``poetry run python3 src/tif_to_zarr.py --help``
+        
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `tif_to_zarr-0.2/pyproject.toml` & `tif_to_zarr-0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tif_to_zarr-0.2/setup.py` & `tif_to_zarr-0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 
 with open(path.join(working_directory, 'README.md'),
           encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='tif_to_zarr',
-    version=0.2,
+    version=0.3,
     url='https://github.com/yuriyzubov/tif-to-zarr.git',
     author='Yurii Zubov',
     description='Simple package to convert small tif files to zarr format.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'imagecodecs',
         'click',
         'zarr',
         'dask', 
         'tifffile',
-        'logging',
         ],
 )
```

