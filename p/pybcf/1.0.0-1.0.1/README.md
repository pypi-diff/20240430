# Comparing `tmp/pybcf-1.0.0.tar.gz` & `tmp/pybcf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybcf-1.0.0.tar", last modified: Mon Apr 29 22:04:15 2024, max compression
+gzip compressed data, was "pybcf-1.0.1.tar", last modified: Mon Apr 29 22:49:19 2024, max compression
```

## Comparing `pybcf-1.0.0.tar` & `pybcf-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:15.859987 pybcf-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-29 22:04:08.000000 pybcf-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-29 22:04:08.000000 pybcf-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-29 22:04:15.859987 pybcf-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-29 22:04:08.000000 pybcf-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 22:04:08.000000 pybcf-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 22:04:15.859987 pybcf-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-29 22:04:08.000000 pybcf-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:15.851987 pybcf-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-29 22:04:08.000000 pybcf-1.0.0/src/bcf.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-29 22:04:08.000000 pybcf-1.0.0/src/bcf.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:15.851987 pybcf-1.0.0/src/gzstream/
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-29 22:04:14.000000 pybcf-1.0.0/src/gzstream/gzstream.C
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-29 22:04:08.000000 pybcf-1.0.0/src/header.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-29 22:04:08.000000 pybcf-1.0.0/src/header.h
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-29 22:04:08.000000 pybcf-1.0.0/src/index.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-29 22:04:08.000000 pybcf-1.0.0/src/index.h
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-29 22:04:08.000000 pybcf-1.0.0/src/info.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-29 22:04:08.000000 pybcf-1.0.0/src/info.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:15.851987 pybcf-1.0.0/src/pybcf/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-29 22:04:08.000000 pybcf-1.0.0/src/pybcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1377881 2024-04-29 22:04:15.000000 pybcf-1.0.0/src/pybcf/reader.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:15.855987 pybcf-1.0.0/src/pybcf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-29 22:04:15.000000 pybcf-1.0.0/src/pybcf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-29 22:04:15.000000 pybcf-1.0.0/src/pybcf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:04:15.000000 pybcf-1.0.0/src/pybcf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-29 22:04:15.000000 pybcf-1.0.0/src/pybcf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 22:04:15.000000 pybcf-1.0.0/src/pybcf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-29 22:04:08.000000 pybcf-1.0.0/src/sample_data.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-29 22:04:08.000000 pybcf-1.0.0/src/sample_data.h
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-29 22:04:08.000000 pybcf-1.0.0/src/types.h
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-29 22:04:08.000000 pybcf-1.0.0/src/variant.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-29 22:04:08.000000 pybcf-1.0.0/src/variant.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:15.855987 pybcf-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-29 22:04:08.000000 pybcf-1.0.0/test/test_pybcf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:49:19.534052 pybcf-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-29 22:49:12.000000 pybcf-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-29 22:49:12.000000 pybcf-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-29 22:49:19.534052 pybcf-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-29 22:49:12.000000 pybcf-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 22:49:12.000000 pybcf-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 22:49:19.534052 pybcf-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-29 22:49:12.000000 pybcf-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:49:19.530052 pybcf-1.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-29 22:49:12.000000 pybcf-1.0.1/src/bcf.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-29 22:49:12.000000 pybcf-1.0.1/src/bcf.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:49:19.530052 pybcf-1.0.1/src/gzstream/
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-29 22:49:18.000000 pybcf-1.0.1/src/gzstream/gzstream.C
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-29 22:49:12.000000 pybcf-1.0.1/src/header.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-29 22:49:12.000000 pybcf-1.0.1/src/header.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-29 22:49:12.000000 pybcf-1.0.1/src/index.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-29 22:49:12.000000 pybcf-1.0.1/src/index.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-29 22:49:12.000000 pybcf-1.0.1/src/info.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-29 22:49:12.000000 pybcf-1.0.1/src/info.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:49:19.534052 pybcf-1.0.1/src/pybcf/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-29 22:49:12.000000 pybcf-1.0.1/src/pybcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1377881 2024-04-29 22:49:19.000000 pybcf-1.0.1/src/pybcf/reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-04-29 22:49:12.000000 pybcf-1.0.1/src/pybcf/reader.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:49:19.534052 pybcf-1.0.1/src/pybcf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-29 22:49:19.000000 pybcf-1.0.1/src/pybcf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-29 22:49:19.000000 pybcf-1.0.1/src/pybcf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:49:19.000000 pybcf-1.0.1/src/pybcf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-29 22:49:19.000000 pybcf-1.0.1/src/pybcf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 22:49:19.000000 pybcf-1.0.1/src/pybcf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-29 22:49:12.000000 pybcf-1.0.1/src/sample_data.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-29 22:49:12.000000 pybcf-1.0.1/src/sample_data.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-29 22:49:12.000000 pybcf-1.0.1/src/types.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-29 22:49:12.000000 pybcf-1.0.1/src/variant.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-29 22:49:12.000000 pybcf-1.0.1/src/variant.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:49:19.534052 pybcf-1.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-29 22:49:12.000000 pybcf-1.0.1/test/test_pybcf.py
```

### Comparing `pybcf-1.0.0/LICENSE.txt` & `pybcf-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/PKG-INFO` & `pybcf-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybcf
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for loading data from bcf files
 Home-page: https://github.com/jeremymcrae/pybcf
 Author: Jeremy McRae
 Author-email: jmcrae@illumina.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `pybcf-1.0.0/README.md` & `pybcf-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/setup.py` & `pybcf-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         language='c++'),
     ])
 
 setup(name='pybcf',
     description='Package for loading data from bcf files',
     long_description=io.open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
-    version='1.0.0',
+    version='1.0.1',
     author='Jeremy McRae',
     author_email='jmcrae@illumina.com',
     license="MIT",
     url='https://github.com/jeremymcrae/pybcf',
     packages=['pybcf'],
     package_dir={'': 'src'},
     install_requires=[
```

### Comparing `pybcf-1.0.0/src/bcf.cpp` & `pybcf-1.0.1/src/bcf.cpp`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/src/gzstream/gzstream.C` & `pybcf-1.0.1/src/gzstream/gzstream.C`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/src/header.cpp` & `pybcf-1.0.1/src/header.cpp`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/src/header.h` & `pybcf-1.0.1/src/header.h`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/src/index.cpp` & `pybcf-1.0.1/src/index.cpp`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/src/index.h` & `pybcf-1.0.1/src/index.h`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/src/info.cpp` & `pybcf-1.0.1/src/info.cpp`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/src/info.h` & `pybcf-1.0.1/src/info.h`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/src/pybcf/reader.cpp` & `pybcf-1.0.1/src/pybcf/reader.cpp`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/src/pybcf.egg-info/PKG-INFO` & `pybcf-1.0.1/src/pybcf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybcf
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for loading data from bcf files
 Home-page: https://github.com/jeremymcrae/pybcf
 Author: Jeremy McRae
 Author-email: jmcrae@illumina.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `pybcf-1.0.0/src/sample_data.cpp` & `pybcf-1.0.1/src/sample_data.cpp`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/src/sample_data.h` & `pybcf-1.0.1/src/sample_data.h`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/src/types.h` & `pybcf-1.0.1/src/types.h`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/src/variant.cpp` & `pybcf-1.0.1/src/variant.cpp`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/src/variant.h` & `pybcf-1.0.1/src/variant.h`

 * *Files identical despite different names*

### Comparing `pybcf-1.0.0/test/test_pybcf.py` & `pybcf-1.0.1/test/test_pybcf.py`

 * *Files identical despite different names*

