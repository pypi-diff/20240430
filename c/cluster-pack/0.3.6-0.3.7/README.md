# Comparing `tmp/cluster_pack-0.3.6-py3-none-any.whl.zip` & `tmp/cluster_pack-0.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 33491 bytes, number of entries: 18
--rw-rw-r--  2.0 unx      334 b- defN 24-Mar-15 14:14 cluster_pack/__init__.py
--rw-rw-r--  2.0 unx    18462 b- defN 24-Mar-15 14:14 cluster_pack/_version.py
--rw-rw-r--  2.0 unx     5126 b- defN 24-Mar-15 14:14 cluster_pack/conda.py
--rw-rw-r--  2.0 unx     8259 b- defN 24-Mar-15 14:14 cluster_pack/filesystem.py
--rw-rw-r--  2.0 unx    19623 b- defN 24-Mar-15 14:14 cluster_pack/packaging.py
--rw-rw-r--  2.0 unx      652 b- defN 24-Mar-15 14:14 cluster_pack/process.py
--rw-rw-r--  2.0 unx    18169 b- defN 24-Mar-15 14:14 cluster_pack/uploader.py
--rw-rw-r--  2.0 unx      123 b- defN 24-Mar-15 14:14 cluster_pack/skein/__init__.py
--rw-rw-r--  2.0 unx      567 b- defN 24-Mar-15 14:14 cluster_pack/skein/_execute_fun.py
--rw-rw-r--  2.0 unx     5610 b- defN 24-Mar-15 14:14 cluster_pack/skein/skein_config_builder.py
--rw-rw-r--  2.0 unx    10587 b- defN 24-Mar-15 14:14 cluster_pack/skein/skein_launcher.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Mar-15 14:14 cluster_pack/spark/__init__.py
--rw-rw-r--  2.0 unx     3066 b- defN 24-Mar-15 14:14 cluster_pack/spark/spark_config_builder.py
--rw-rw-r--  2.0 unx    11336 b- defN 24-Mar-15 14:14 cluster_pack-0.3.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3772 b- defN 24-Mar-15 14:14 cluster_pack-0.3.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-15 14:14 cluster_pack-0.3.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 24-Mar-15 14:14 cluster_pack-0.3.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1531 b- defN 24-Mar-15 14:14 cluster_pack-0.3.6.dist-info/RECORD
-18 files, 107322 bytes uncompressed, 30971 bytes compressed:  71.1%
+Zip file size: 33492 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      334 b- defN 24-Apr-30 14:02 cluster_pack/__init__.py
+-rw-r--r--  2.0 unx    18462 b- defN 24-Apr-30 14:02 cluster_pack/_version.py
+-rw-r--r--  2.0 unx     5126 b- defN 24-Apr-30 14:02 cluster_pack/conda.py
+-rw-r--r--  2.0 unx     8259 b- defN 24-Apr-30 14:02 cluster_pack/filesystem.py
+-rw-r--r--  2.0 unx    19623 b- defN 24-Apr-30 14:02 cluster_pack/packaging.py
+-rw-r--r--  2.0 unx      652 b- defN 24-Apr-30 14:02 cluster_pack/process.py
+-rw-r--r--  2.0 unx    18169 b- defN 24-Apr-30 14:02 cluster_pack/uploader.py
+-rw-r--r--  2.0 unx      123 b- defN 24-Apr-30 14:02 cluster_pack/skein/__init__.py
+-rw-r--r--  2.0 unx      567 b- defN 24-Apr-30 14:02 cluster_pack/skein/_execute_fun.py
+-rw-r--r--  2.0 unx     5610 b- defN 24-Apr-30 14:02 cluster_pack/skein/skein_config_builder.py
+-rw-r--r--  2.0 unx    10587 b- defN 24-Apr-30 14:02 cluster_pack/skein/skein_launcher.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-30 14:02 cluster_pack/spark/__init__.py
+-rw-r--r--  2.0 unx     3066 b- defN 24-Apr-30 14:02 cluster_pack/spark/spark_config_builder.py
+-rw-r--r--  2.0 unx    11336 b- defN 24-Apr-30 14:02 cluster_pack-0.3.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3764 b- defN 24-Apr-30 14:02 cluster_pack-0.3.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 14:02 cluster_pack-0.3.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-30 14:02 cluster_pack-0.3.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1531 b- defN 24-Apr-30 14:02 cluster_pack-0.3.7.dist-info/RECORD
+18 files, 107314 bytes uncompressed, 30972 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: cluster_pack/spark/__init__.py
 Comment: 
 
 Filename: cluster_pack/spark/spark_config_builder.py
 Comment: 
 
-Filename: cluster_pack-0.3.6.dist-info/LICENSE
+Filename: cluster_pack-0.3.7.dist-info/LICENSE
 Comment: 
 
-Filename: cluster_pack-0.3.6.dist-info/METADATA
+Filename: cluster_pack-0.3.7.dist-info/METADATA
 Comment: 
 
-Filename: cluster_pack-0.3.6.dist-info/WHEEL
+Filename: cluster_pack-0.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: cluster_pack-0.3.6.dist-info/top_level.txt
+Filename: cluster_pack-0.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: cluster_pack-0.3.6.dist-info/RECORD
+Filename: cluster_pack-0.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cluster_pack-0.3.6.dist-info/LICENSE` & `cluster_pack-0.3.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cluster_pack-0.3.6.dist-info/METADATA` & `cluster_pack-0.3.7.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluster-pack
-Version: 0.3.6
+Version: 0.3.7
 Summary: A library on top of either pex or conda-packto make your Python code easily available on a cluster
 Home-page: https://github.com/criteo/cluster-pack
 Maintainer: Criteo
 Maintainer-email: github@criteo.com
 License: UNKNOWN
 Keywords: hadoop distributed cluster S3 HDFS
 Platform: UNKNOWN
@@ -18,20 +18,19 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: cloudpickle
-Requires-Dist: pex ==2.1.137
+Requires-Dist: pex (==2.1.137)
 Requires-Dist: conda-pack
-Requires-Dist: pip >=18.1
-Requires-Dist: pyarrow
+Requires-Dist: pip (>=18.1)
+Requires-Dist: pyarrow (<16.0.0)
 Requires-Dist: fire
 Requires-Dist: types-setuptools
 Requires-Dist: wheel-filename
 
 # cluster-pack
 
 cluster-pack is a library on top of either [pex][pex] or [conda-pack][conda-pack] to make your Python code easily available on a cluster.
```

