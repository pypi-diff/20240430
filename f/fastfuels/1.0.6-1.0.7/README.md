# Comparing `tmp/fastfuels-1.0.6.tar.gz` & `tmp/fastfuels-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastfuels-1.0.6.tar", last modified: Fri Apr 26 02:26:07 2024, max compression
+gzip compressed data, was "fastfuels-1.0.7.tar", last modified: Tue Apr 30 18:22:31 2024, max compression
```

## Comparing `fastfuels-1.0.6.tar` & `fastfuels-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lucaswells   (501) staff       (20)        0 2024-04-26 02:26:07.660703 fastfuels-1.0.6/
--rw-r--r--   0 lucaswells   (501) staff       (20)    34502 2024-04-26 02:21:14.000000 fastfuels-1.0.6/LICENSE.txt
--rw-r--r--   0 lucaswells   (501) staff       (20)     3373 2024-04-26 02:26:07.660616 fastfuels-1.0.6/PKG-INFO
--rw-r--r--   0 lucaswells   (501) staff       (20)     2377 2024-04-26 02:21:14.000000 fastfuels-1.0.6/README.md
-drwxr-xr-x   0 lucaswells   (501) staff       (20)        0 2024-04-26 02:26:07.659285 fastfuels-1.0.6/fastfuels/
--rw-r--r--   0 lucaswells   (501) staff       (20)       23 2024-04-26 02:21:14.000000 fastfuels-1.0.6/fastfuels/__init__.py
--rw-r--r--   0 lucaswells   (501) staff       (20)    35612 2024-04-26 02:21:14.000000 fastfuels-1.0.6/fastfuels/core.py
--rwxr-xr-x   0 lucaswells   (501) staff       (20)     5042 2024-04-26 02:21:14.000000 fastfuels-1.0.6/fastfuels/fastfuels_create_index.py
-drwxr-xr-x   0 lucaswells   (501) staff       (20)        0 2024-04-26 02:26:07.660329 fastfuels-1.0.6/fastfuels.egg-info/
--rw-r--r--   0 lucaswells   (501) staff       (20)     3373 2024-04-26 02:26:07.000000 fastfuels-1.0.6/fastfuels.egg-info/PKG-INFO
--rw-r--r--   0 lucaswells   (501) staff       (20)      280 2024-04-26 02:26:07.000000 fastfuels-1.0.6/fastfuels.egg-info/SOURCES.txt
--rw-r--r--   0 lucaswells   (501) staff       (20)        1 2024-04-26 02:26:07.000000 fastfuels-1.0.6/fastfuels.egg-info/dependency_links.txt
--rw-r--r--   0 lucaswells   (501) staff       (20)      130 2024-04-26 02:26:07.000000 fastfuels-1.0.6/fastfuels.egg-info/requires.txt
--rw-r--r--   0 lucaswells   (501) staff       (20)       10 2024-04-26 02:26:07.000000 fastfuels-1.0.6/fastfuels.egg-info/top_level.txt
--rw-r--r--   0 lucaswells   (501) staff       (20)       79 2024-04-26 02:26:07.660947 fastfuels-1.0.6/setup.cfg
--rw-r--r--   0 lucaswells   (501) staff       (20)     1766 2024-04-26 02:24:03.000000 fastfuels-1.0.6/setup.py
+drwxr-xr-x   0 lucaswells   (501) staff       (20)        0 2024-04-30 18:22:31.266558 fastfuels-1.0.7/
+-rw-r--r--   0 lucaswells   (501) staff       (20)    34502 2024-04-26 02:21:14.000000 fastfuels-1.0.7/LICENSE.txt
+-rw-r--r--   0 lucaswells   (501) staff       (20)     3372 2024-04-30 18:22:31.266474 fastfuels-1.0.7/PKG-INFO
+-rw-r--r--   0 lucaswells   (501) staff       (20)     2377 2024-04-26 02:21:14.000000 fastfuels-1.0.7/README.md
+drwxr-xr-x   0 lucaswells   (501) staff       (20)        0 2024-04-30 18:22:31.265156 fastfuels-1.0.7/fastfuels/
+-rw-r--r--   0 lucaswells   (501) staff       (20)       23 2024-04-26 02:21:14.000000 fastfuels-1.0.7/fastfuels/__init__.py
+-rw-r--r--   0 lucaswells   (501) staff       (20)    35612 2024-04-26 02:21:14.000000 fastfuels-1.0.7/fastfuels/core.py
+-rwxr-xr-x   0 lucaswells   (501) staff       (20)     5042 2024-04-26 02:21:14.000000 fastfuels-1.0.7/fastfuels/fastfuels_create_index.py
+drwxr-xr-x   0 lucaswells   (501) staff       (20)        0 2024-04-30 18:22:31.266145 fastfuels-1.0.7/fastfuels.egg-info/
+-rw-r--r--   0 lucaswells   (501) staff       (20)     3372 2024-04-30 18:22:31.000000 fastfuels-1.0.7/fastfuels.egg-info/PKG-INFO
+-rw-r--r--   0 lucaswells   (501) staff       (20)      280 2024-04-30 18:22:31.000000 fastfuels-1.0.7/fastfuels.egg-info/SOURCES.txt
+-rw-r--r--   0 lucaswells   (501) staff       (20)        1 2024-04-30 18:22:31.000000 fastfuels-1.0.7/fastfuels.egg-info/dependency_links.txt
+-rw-r--r--   0 lucaswells   (501) staff       (20)      129 2024-04-30 18:22:31.000000 fastfuels-1.0.7/fastfuels.egg-info/requires.txt
+-rw-r--r--   0 lucaswells   (501) staff       (20)       10 2024-04-30 18:22:31.000000 fastfuels-1.0.7/fastfuels.egg-info/top_level.txt
+-rw-r--r--   0 lucaswells   (501) staff       (20)       79 2024-04-30 18:22:31.266816 fastfuels-1.0.7/setup.cfg
+-rw-r--r--   0 lucaswells   (501) staff       (20)     1765 2024-04-30 18:19:59.000000 fastfuels-1.0.7/setup.py
```

### Comparing `fastfuels-1.0.6/LICENSE.txt` & `fastfuels-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastfuels-1.0.6/PKG-INFO` & `fastfuels-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfuels
-Version: 1.0.6
+Version: 1.0.7
 Summary: 3D fuelscapes for the contiguous US
 Home-page: https://github.com/teamholtz/FastFuels-Python
 Author: Holtz Technology and Development Services LLC
 Author-email: lucas@holtztds.com
 License: GNU GPLv3
 Keywords: fire model,fuelscape,wildfire
 Classifier: Development Status :: 3 - Alpha
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: colorcet==2.0.6
-Requires-Dist: fsspec==2021.11.0
+Requires-Dist: fsspec==2024.2.0
 Requires-Dist: msgpack==1.0.2
 Requires-Dist: numpy==1.23.0
 Requires-Dist: pyvista==0.28.1
 Requires-Dist: s3fs==2024.2.0
 Requires-Dist: scipy==1.11.4
 Requires-Dist: shapely<2
 Requires-Dist: zarr==2.8.3
```

### Comparing `fastfuels-1.0.6/README.md` & `fastfuels-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fastfuels-1.0.6/fastfuels/core.py` & `fastfuels-1.0.7/fastfuels/core.py`

 * *Files identical despite different names*

### Comparing `fastfuels-1.0.6/fastfuels/fastfuels_create_index.py` & `fastfuels-1.0.7/fastfuels/fastfuels_create_index.py`

 * *Files identical despite different names*

### Comparing `fastfuels-1.0.6/fastfuels.egg-info/PKG-INFO` & `fastfuels-1.0.7/fastfuels.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfuels
-Version: 1.0.6
+Version: 1.0.7
 Summary: 3D fuelscapes for the contiguous US
 Home-page: https://github.com/teamholtz/FastFuels-Python
 Author: Holtz Technology and Development Services LLC
 Author-email: lucas@holtztds.com
 License: GNU GPLv3
 Keywords: fire model,fuelscape,wildfire
 Classifier: Development Status :: 3 - Alpha
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: colorcet==2.0.6
-Requires-Dist: fsspec==2021.11.0
+Requires-Dist: fsspec==2024.2.0
 Requires-Dist: msgpack==1.0.2
 Requires-Dist: numpy==1.23.0
 Requires-Dist: pyvista==0.28.1
 Requires-Dist: s3fs==2024.2.0
 Requires-Dist: scipy==1.11.4
 Requires-Dist: shapely<2
 Requires-Dist: zarr==2.8.3
```

### Comparing `fastfuels-1.0.6/setup.py` & `fastfuels-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     author='Holtz Technology and Development Services LLC',
     author_email='lucas@holtztds.com',
     url='https://github.com/teamholtz/FastFuels-Python',
     keywords=['fire model', 'fuelscape', 'wildfire'],
     install_requires=[
         # pinning all dependencies to avoid version mismatch
         'colorcet==2.0.6',
-        'fsspec==2021.11.0',
+        'fsspec==2024.2.0',
         # numcodecs no longer includes msgpack?
         'msgpack==1.0.2',
         # use numpy 1.23 to avoid TypeError: 'numpy._DTypeMeta' object is not subscriptable
         'numpy==1.23.0',
         'pyvista==0.28.1',
         's3fs==2024.2.0',
         # use newer scipy for numpy 1.23
```

