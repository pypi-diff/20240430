# Comparing `tmp/tif_to_zarr-0.3.tar.gz` & `tmp/tif_to_zarr-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tif_to_zarr-0.3.tar", last modified: Mon Apr 29 21:39:14 2024, max compression
+gzip compressed data, was "tif_to_zarr-0.4.tar", last modified: Tue Apr 30 17:37:09 2024, max compression
```

## Comparing `tif_to_zarr-0.3.tar` & `tif_to_zarr-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 zubovy   (65918) cellmap   (1127)        0 2024-04-29 21:39:14.091232 tif_to_zarr-0.3/
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1518 2024-04-29 20:35:53.000000 tif_to_zarr-0.3/LICENSE
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1322 2024-04-29 21:39:14.091232 tif_to_zarr-0.3/PKG-INFO
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)      924 2024-04-29 20:13:11.000000 tif_to_zarr-0.3/README.md
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)      516 2024-04-29 20:13:11.000000 tif_to_zarr-0.3/pyproject.toml
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)       38 2024-04-29 21:39:14.091232 tif_to_zarr-0.3/setup.cfg
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)      698 2024-04-29 21:39:04.000000 tif_to_zarr-0.3/setup.py
-drwxr-xr-x   0 zubovy   (65918) cellmap   (1127)        0 2024-04-29 21:39:14.091232 tif_to_zarr-0.3/tif_to_zarr.egg-info/
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1322 2024-04-29 21:39:14.000000 tif_to_zarr-0.3/tif_to_zarr.egg-info/PKG-INFO
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)      215 2024-04-29 21:39:14.000000 tif_to_zarr-0.3/tif_to_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)        1 2024-04-29 21:39:14.000000 tif_to_zarr-0.3/tif_to_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)       37 2024-04-29 21:39:14.000000 tif_to_zarr-0.3/tif_to_zarr.egg-info/requires.txt
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)        1 2024-04-29 21:39:14.000000 tif_to_zarr-0.3/tif_to_zarr.egg-info/top_level.txt
+drwxr-xr-x   0 zubovy   (65918) cellmap   (1127)        0 2024-04-30 17:37:09.177664 tif_to_zarr-0.4/
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1518 2024-04-29 20:35:53.000000 tif_to_zarr-0.4/LICENSE
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1184 2024-04-30 17:37:09.177664 tif_to_zarr-0.4/PKG-INFO
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)      924 2024-04-29 20:13:11.000000 tif_to_zarr-0.4/README.md
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)      516 2024-04-29 20:13:11.000000 tif_to_zarr-0.4/pyproject.toml
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)       38 2024-04-30 17:37:09.177664 tif_to_zarr-0.4/setup.cfg
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)      698 2024-04-30 17:36:53.000000 tif_to_zarr-0.4/setup.py
+drwxr-xr-x   0 zubovy   (65918) cellmap   (1127)        0 2024-04-30 17:37:09.177664 tif_to_zarr-0.4/tif_to_zarr.egg-info/
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1184 2024-04-30 17:37:09.000000 tif_to_zarr-0.4/tif_to_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)      215 2024-04-30 17:37:09.000000 tif_to_zarr-0.4/tif_to_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)        1 2024-04-30 17:37:09.000000 tif_to_zarr-0.4/tif_to_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)       37 2024-04-30 17:37:09.000000 tif_to_zarr-0.4/tif_to_zarr.egg-info/requires.txt
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)        1 2024-04-30 17:37:09.000000 tif_to_zarr-0.4/tif_to_zarr.egg-info/top_level.txt
```

### Comparing `tif_to_zarr-0.3/LICENSE` & `tif_to_zarr-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tif_to_zarr-0.3/PKG-INFO` & `tif_to_zarr-0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: tif_to_zarr
-Version: 0.3
+Version: 0.4
 Summary: Simple package to convert small tif files to zarr format.
 Home-page: https://github.com/yuriyzubov/tif-to-zarr.git
 Author: Yurii Zubov
-License: UNKNOWN
-Description: This script could be used for conversion of a .tiff file to .zarr format with OME-NGFF multiscales metadata structure.
-        #### How to run
-        1. open command line terminal
-        2. install poetry tool for dependency management and packaging: https://pypi.org/project/poetry/
-        3. switch to the tif_to_zarr directory:
-            ``cd PATH_TO_DIRECTORY/tif_to_zarr``
-        4. install python dependencies:
-            ``poetry install``
-        5. run script using cli:
-            ``poetry run python src/tif_to_zarr.py --src=PATH_TO_SOURCE_DIRECTORY/input_file.tif --dest=PATH_TO_DEST_DIRECTORY/output_file.zarr``
-        6. to convert a tiff file to zarr with custom metadata values, you can run smthg similar to this:
-        ``poetry run python3 src/tif_to_zarr.py --src=path_to_source_tif  --dest=path_to_output_zarr -a x z y -t 1.0 2.0 3.0 -s 4.0 5.0 6.0 -u nanometer nanometer nanometer``
-        7. To get the list of options, you may run this:
-        ``poetry run python3 src/tif_to_zarr.py --help``
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+This script could be used for conversion of a .tiff file to .zarr format with OME-NGFF multiscales metadata structure.
+#### How to run
+1. open command line terminal
+2. install poetry tool for dependency management and packaging: https://pypi.org/project/poetry/
+3. switch to the tif_to_zarr directory:
+    ``cd PATH_TO_DIRECTORY/tif_to_zarr``
+4. install python dependencies:
+    ``poetry install``
+5. run script using cli:
+    ``poetry run python src/tif_to_zarr.py --src=PATH_TO_SOURCE_DIRECTORY/input_file.tif --dest=PATH_TO_DEST_DIRECTORY/output_file.zarr``
+6. to convert a tiff file to zarr with custom metadata values, you can run smthg similar to this:
+``poetry run python3 src/tif_to_zarr.py --src=path_to_source_tif  --dest=path_to_output_zarr -a x z y -t 1.0 2.0 3.0 -s 4.0 5.0 6.0 -u nanometer nanometer nanometer``
+7. To get the list of options, you may run this:
+``poetry run python3 src/tif_to_zarr.py --help``
```

### Comparing `tif_to_zarr-0.3/README.md` & `tif_to_zarr-0.4/README.md`

 * *Files identical despite different names*

### Comparing `tif_to_zarr-0.3/pyproject.toml` & `tif_to_zarr-0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tif_to_zarr-0.3/setup.py` & `tif_to_zarr-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open(path.join(working_directory, 'README.md'),
           encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='tif_to_zarr',
-    version=0.3,
+    version=0.4,
     url='https://github.com/yuriyzubov/tif-to-zarr.git',
     author='Yurii Zubov',
     description='Simple package to convert small tif files to zarr format.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

### Comparing `tif_to_zarr-0.3/tif_to_zarr.egg-info/PKG-INFO` & `tif_to_zarr-0.4/tif_to_zarr.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: tif-to-zarr
-Version: 0.3
+Version: 0.4
 Summary: Simple package to convert small tif files to zarr format.
 Home-page: https://github.com/yuriyzubov/tif-to-zarr.git
 Author: Yurii Zubov
-License: UNKNOWN
-Description: This script could be used for conversion of a .tiff file to .zarr format with OME-NGFF multiscales metadata structure.
-        #### How to run
-        1. open command line terminal
-        2. install poetry tool for dependency management and packaging: https://pypi.org/project/poetry/
-        3. switch to the tif_to_zarr directory:
-            ``cd PATH_TO_DIRECTORY/tif_to_zarr``
-        4. install python dependencies:
-            ``poetry install``
-        5. run script using cli:
-            ``poetry run python src/tif_to_zarr.py --src=PATH_TO_SOURCE_DIRECTORY/input_file.tif --dest=PATH_TO_DEST_DIRECTORY/output_file.zarr``
-        6. to convert a tiff file to zarr with custom metadata values, you can run smthg similar to this:
-        ``poetry run python3 src/tif_to_zarr.py --src=path_to_source_tif  --dest=path_to_output_zarr -a x z y -t 1.0 2.0 3.0 -s 4.0 5.0 6.0 -u nanometer nanometer nanometer``
-        7. To get the list of options, you may run this:
-        ``poetry run python3 src/tif_to_zarr.py --help``
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+This script could be used for conversion of a .tiff file to .zarr format with OME-NGFF multiscales metadata structure.
+#### How to run
+1. open command line terminal
+2. install poetry tool for dependency management and packaging: https://pypi.org/project/poetry/
+3. switch to the tif_to_zarr directory:
+    ``cd PATH_TO_DIRECTORY/tif_to_zarr``
+4. install python dependencies:
+    ``poetry install``
+5. run script using cli:
+    ``poetry run python src/tif_to_zarr.py --src=PATH_TO_SOURCE_DIRECTORY/input_file.tif --dest=PATH_TO_DEST_DIRECTORY/output_file.zarr``
+6. to convert a tiff file to zarr with custom metadata values, you can run smthg similar to this:
+``poetry run python3 src/tif_to_zarr.py --src=path_to_source_tif  --dest=path_to_output_zarr -a x z y -t 1.0 2.0 3.0 -s 4.0 5.0 6.0 -u nanometer nanometer nanometer``
+7. To get the list of options, you may run this:
+``poetry run python3 src/tif_to_zarr.py --help``
```

