# Comparing `tmp/cubed-xarray-0.0.5.tar.gz` & `tmp/cubed-xarray-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubed-xarray-0.0.5.tar", last modified: Wed Mar 20 15:25:49 2024, max compression
+gzip compressed data, was "cubed-xarray-0.0.6.tar", last modified: Tue Apr 30 08:26:07 2024, max compression
```

## Comparing `cubed-xarray-0.0.5.tar` & `cubed-xarray-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-20 15:25:49.974500 cubed-xarray-0.0.5/
--rw-r--r--   0 tom        (501) staff       (20)     1799 2024-03-01 17:48:00.000000 cubed-xarray-0.0.5/.gitignore
--rw-r--r--   0 tom        (501) staff       (20)    11357 2024-03-01 17:48:00.000000 cubed-xarray-0.0.5/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)     3769 2024-03-20 15:25:49.974418 cubed-xarray-0.0.5/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     2689 2024-03-04 16:24:28.000000 cubed-xarray-0.0.5/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-20 15:25:49.973160 cubed-xarray-0.0.5/cubed_xarray/
--rw-r--r--   0 tom        (501) staff       (20)      243 2024-03-01 17:48:00.000000 cubed-xarray-0.0.5/cubed_xarray/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     6416 2024-03-04 16:19:21.000000 cubed-xarray-0.0.5/cubed_xarray/cubedmanager.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-20 15:25:49.974145 cubed-xarray-0.0.5/cubed_xarray/tests/
--rw-r--r--   0 tom        (501) staff       (20)        0 2024-03-01 17:48:00.000000 cubed-xarray-0.0.5/cubed_xarray/tests/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      727 2024-03-04 16:18:59.000000 cubed-xarray-0.0.5/cubed_xarray/tests/test_wrapping.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-20 15:25:49.973904 cubed-xarray-0.0.5/cubed_xarray.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     3769 2024-03-20 15:25:49.000000 cubed-xarray-0.0.5/cubed_xarray.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      418 2024-03-20 15:25:49.000000 cubed-xarray-0.0.5/cubed_xarray.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2024-03-20 15:25:49.000000 cubed-xarray-0.0.5/cubed_xarray.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)       70 2024-03-20 15:25:49.000000 cubed-xarray-0.0.5/cubed_xarray.egg-info/entry_points.txt
--rw-r--r--   0 tom        (501) staff       (20)       43 2024-03-20 15:25:49.000000 cubed-xarray-0.0.5/cubed_xarray.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       13 2024-03-20 15:25:49.000000 cubed-xarray-0.0.5/cubed_xarray.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)     1578 2024-03-20 15:09:11.000000 cubed-xarray-0.0.5/pyproject.toml
--rw-r--r--   0 tom        (501) staff       (20)       44 2024-03-04 16:18:59.000000 cubed-xarray-0.0.5/requirements.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2024-03-20 15:25:49.974682 cubed-xarray-0.0.5/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)       93 2024-03-01 17:48:00.000000 cubed-xarray-0.0.5/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-30 08:26:07.524094 cubed-xarray-0.0.6/
+-rw-r--r--   0 tom        (501) staff       (20)     1799 2023-05-10 10:10:03.000000 cubed-xarray-0.0.6/.gitignore
+-rw-r--r--   0 tom        (501) staff       (20)    11357 2023-05-10 10:10:03.000000 cubed-xarray-0.0.6/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)     3682 2024-04-30 08:26:07.524406 cubed-xarray-0.0.6/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     2690 2024-04-30 08:23:23.000000 cubed-xarray-0.0.6/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-30 08:26:07.522651 cubed-xarray-0.0.6/cubed_xarray/
+-rw-r--r--   0 tom        (501) staff       (20)      243 2023-05-10 10:10:03.000000 cubed-xarray-0.0.6/cubed_xarray/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     6160 2024-04-30 08:21:19.000000 cubed-xarray-0.0.6/cubed_xarray/cubedmanager.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-30 08:26:07.523872 cubed-xarray-0.0.6/cubed_xarray/tests/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-05-10 10:10:03.000000 cubed-xarray-0.0.6/cubed_xarray/tests/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      727 2024-04-04 12:43:55.000000 cubed-xarray-0.0.6/cubed_xarray/tests/test_wrapping.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-30 08:26:07.523599 cubed-xarray-0.0.6/cubed_xarray.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     3682 2024-04-30 08:26:07.000000 cubed-xarray-0.0.6/cubed_xarray.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      418 2024-04-30 08:26:07.000000 cubed-xarray-0.0.6/cubed_xarray.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2024-04-30 08:26:07.000000 cubed-xarray-0.0.6/cubed_xarray.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)       70 2024-04-30 08:26:07.000000 cubed-xarray-0.0.6/cubed_xarray.egg-info/entry_points.txt
+-rw-r--r--   0 tom        (501) staff       (20)       44 2024-04-30 08:26:07.000000 cubed-xarray-0.0.6/cubed_xarray.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       13 2024-04-30 08:26:07.000000 cubed-xarray-0.0.6/cubed_xarray.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)     1579 2024-04-30 08:23:29.000000 cubed-xarray-0.0.6/pyproject.toml
+-rw-r--r--   0 tom        (501) staff       (20)       45 2024-04-30 08:21:19.000000 cubed-xarray-0.0.6/requirements.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2024-04-30 08:26:07.524630 cubed-xarray-0.0.6/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)       93 2023-05-10 10:10:03.000000 cubed-xarray-0.0.6/setup.py
```

### Comparing `cubed-xarray-0.0.5/.gitignore` & `cubed-xarray-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `cubed-xarray-0.0.5/LICENSE` & `cubed-xarray-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cubed-xarray-0.0.5/PKG-INFO` & `cubed-xarray-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubed-xarray
-Version: 0.0.5
+Version: 0.0.6
 Summary: Interface for using cubed with xarray for parallel computation.
 Author-email: Tom Nicholas <tomnicholas1@googlemail.com>
 License: Apache-2
 Project-URL: homepage, https://github.com/xarray-contrib/cubed-xarray
 Project-URL: documentation, https://github.com/xarray-contrib/cubed-xarray#readme
 Project-URL: repository, https://github.com/xarray-contrib/cubed-xarray
 Classifier: Development Status :: 3 - Alpha
@@ -16,27 +16,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.17
-Requires-Dist: xarray>=2024.02.0
-Requires-Dist: cubed>=0.6.3
 
 Note: this is a proof-of-concept, and many things are incomplete, untested, or don't work.
 
 # cubed-xarray
 
 Interface for using [cubed](https://github.com/cubed-dev/cubed) with [xarray](https://github.com/pydata/xarray).
 
 ## Requirements
 
-- Cubed version >=0.6.3
+- Cubed version >=0.14.2
 - Xarray version >=2024.02.0
 
 ## Installation
 
 Install via pip 
 
 `pip install cubed-xarray`
```

### Comparing `cubed-xarray-0.0.5/README.md` & `cubed-xarray-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # cubed-xarray
 
 Interface for using [cubed](https://github.com/cubed-dev/cubed) with [xarray](https://github.com/pydata/xarray).
 
 ## Requirements
 
-- Cubed version >=0.6.3
+- Cubed version >=0.14.2
 - Xarray version >=2024.02.0
 
 ## Installation
 
 Install via pip 
 
 `pip install cubed-xarray`
```

### Comparing `cubed-xarray-0.0.5/cubed_xarray/cubedmanager.py` & `cubed-xarray-0.0.6/cubed_xarray/cubedmanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     ) -> "CubedArray":
         from cubed.core.ops import reduction
 
         return reduction(
             arr,
             func=func,
             combine_func=combine_func,
-            aggegrate_func=aggregate_func,  # TODO fix the typo in argument name in cubed
+            aggregate_func=aggregate_func,
             axis=axis,
             dtype=dtype,
             keepdims=keepdims,
         )
 
     def map_blocks(
         self,
@@ -100,19 +100,14 @@
         chunks: tuple[int, ...] | None = None,
         drop_axis: int | Sequence[int] | None = None,
         new_axis: int | Sequence[int] | None = None,
         **kwargs,
     ):
         from cubed.core.ops import map_blocks
 
-        if drop_axis is None:
-            # TODO should fix this upstream in cubed to match dask
-            # see https://github.com/pydata/xarray/pull/7019#discussion_r1196729489
-            drop_axis = []
-
         return map_blocks(
             func,
             *args,
             dtype=dtype,
             chunks=chunks,
             drop_axis=drop_axis,
             new_axis=new_axis,
```

### Comparing `cubed-xarray-0.0.5/cubed_xarray/tests/test_wrapping.py` & `cubed-xarray-0.0.6/cubed_xarray/tests/test_wrapping.py`

 * *Files identical despite different names*

### Comparing `cubed-xarray-0.0.5/cubed_xarray.egg-info/PKG-INFO` & `cubed-xarray-0.0.6/cubed_xarray.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubed-xarray
-Version: 0.0.5
+Version: 0.0.6
 Summary: Interface for using cubed with xarray for parallel computation.
 Author-email: Tom Nicholas <tomnicholas1@googlemail.com>
 License: Apache-2
 Project-URL: homepage, https://github.com/xarray-contrib/cubed-xarray
 Project-URL: documentation, https://github.com/xarray-contrib/cubed-xarray#readme
 Project-URL: repository, https://github.com/xarray-contrib/cubed-xarray
 Classifier: Development Status :: 3 - Alpha
@@ -16,27 +16,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.17
-Requires-Dist: xarray>=2024.02.0
-Requires-Dist: cubed>=0.6.3
 
 Note: this is a proof-of-concept, and many things are incomplete, untested, or don't work.
 
 # cubed-xarray
 
 Interface for using [cubed](https://github.com/cubed-dev/cubed) with [xarray](https://github.com/pydata/xarray).
 
 ## Requirements
 
-- Cubed version >=0.6.3
+- Cubed version >=0.14.2
 - Xarray version >=2024.02.0
 
 ## Installation
 
 Install via pip 
 
 `pip install cubed-xarray`
```

### Comparing `cubed-xarray-0.0.5/pyproject.toml` & `cubed-xarray-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cubed-xarray"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     {name = "Tom Nicholas", email = "tomnicholas1@googlemail.com"}
 ]
 description = "Interface for using cubed with xarray for parallel computation."
 license = {text = "Apache-2"}
 readme = "README.md"
 classifiers = [
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "numpy >= 1.17",
     "xarray >= 2024.02.0",
-    "cubed >= 0.6.3",
+    "cubed >= 0.14.2",
 ]
 
 [project.urls]
 homepage = "https://github.com/xarray-contrib/cubed-xarray"
 documentation = "https://github.com/xarray-contrib/cubed-xarray#readme"
 repository = "https://github.com/xarray-contrib/cubed-xarray"
```

