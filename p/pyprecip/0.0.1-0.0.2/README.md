# Comparing `tmp/pyprecip-0.0.1-py2.py3-none-any.whl.zip` & `tmp/pyprecip-0.0.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,13 @@
-Zip file size: 2461 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-07 06:08 pyprecip/__init__.py
+Zip file size: 6556 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-30 06:07 pyprecip/__init__.py
 -rw-rw-rw-  2.0 fat      117 b- defN 24-Apr-07 08:21 pyprecip/main.py
--rw-rw-rw-  2.0 fat     1094 b- defN 24-Apr-07 12:10 pyprecip-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      631 b- defN 24-Apr-07 12:10 pyprecip-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-07 12:10 pyprecip-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-07 12:10 pyprecip-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      536 b- defN 24-Apr-07 12:10 pyprecip-0.0.1.dist-info/RECORD
-7 files, 2497 bytes uncompressed, 1507 bytes compressed:  39.6%
+-rw-rw-rw-  2.0 fat       49 b- defN 24-Apr-30 06:53 pyprecip/reading/__init__.py
+-rw-rw-rw-  2.0 fat     5136 b- defN 24-Apr-30 06:13 pyprecip/reading/read_api.py
+-rw-rw-rw-  2.0 fat     5184 b- defN 24-Apr-30 05:02 pyprecip/reading/read_file.py
+-rw-rw-rw-  2.0 fat      118 b- defN 24-Apr-30 07:59 pyprecip/reading/test.py
+-rw-rw-rw-  2.0 fat     1094 b- defN 24-Apr-30 08:20 pyprecip-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      834 b- defN 24-Apr-30 08:20 pyprecip-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-30 08:20 pyprecip-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-30 08:20 pyprecip-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      870 b- defN 24-Apr-30 08:20 pyprecip-0.0.2.dist-info/RECORD
+11 files, 13521 bytes uncompressed, 5080 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -1,22 +1,34 @@
 Filename: pyprecip/__init__.py
 Comment: 
 
 Filename: pyprecip/main.py
 Comment: 
 
-Filename: pyprecip-0.0.1.dist-info/LICENSE
+Filename: pyprecip/reading/__init__.py
 Comment: 
 
-Filename: pyprecip-0.0.1.dist-info/METADATA
+Filename: pyprecip/reading/read_api.py
 Comment: 
 
-Filename: pyprecip-0.0.1.dist-info/WHEEL
+Filename: pyprecip/reading/read_file.py
 Comment: 
 
-Filename: pyprecip-0.0.1.dist-info/top_level.txt
+Filename: pyprecip/reading/test.py
 Comment: 
 
-Filename: pyprecip-0.0.1.dist-info/RECORD
+Filename: pyprecip-0.0.2.dist-info/LICENSE
+Comment: 
+
+Filename: pyprecip-0.0.2.dist-info/METADATA
+Comment: 
+
+Filename: pyprecip-0.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: pyprecip-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: pyprecip-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyprecip-0.0.1.dist-info/LICENSE` & `pyprecip-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyprecip-0.0.1.dist-info/METADATA` & `pyprecip-0.0.2.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprecip
-Version: 0.0.1
+Version: 0.0.2
 Summary: A climate data processing library.
 Home-page: https://github.com/ma0513207162/pyprecip
 Author: hasang
 Author-email: ma0513207162@163.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -12,13 +12,13 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7.0
 License-File: LICENSE
 
-# Example Package
-A climate data processing library.
+# pyprecip 科学计算
 
+pyprecip 是一个专注于气候数据处理的 Python 库，旨在为用户提供方便、高效的气候数据处理和分析工具。该库致力于处理各种气候数据，并特别关注于降水数据的处理和分析。
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `pyprecip-0.0.1.dist-info/RECORD` & `pyprecip-0.0.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,11 @@
 pyprecip/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyprecip/main.py,sha256=GRip5D32taF3_EL5Q1N_Gm7UfMlU8Ttwf-IzBK4DcOw,117
-pyprecip-0.0.1.dist-info/LICENSE,sha256=5VmicU9G7tYoRg6lG2pOTlnQR-ZNyyd1g9odyyrLYzU,1094
-pyprecip-0.0.1.dist-info/METADATA,sha256=iuGqJgQhmitayyA4ZMmt-5JPHHPqImcdogqtY-3IuW0,631
-pyprecip-0.0.1.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-pyprecip-0.0.1.dist-info/top_level.txt,sha256=TUBZn-IeYiCoBF5Mx6vzAEZDD083ijzLBA20d56im24,9
-pyprecip-0.0.1.dist-info/RECORD,,
+pyprecip/reading/__init__.py,sha256=K9CT7ocsU1xsezZOn1ZLJ9TKNFsrldfI8tM9MZkWBoI,49
+pyprecip/reading/read_api.py,sha256=Z7aDWF5YcDNK3a74IH4O9CmKxiHqGDvzQOZ-FzzTlmA,5136
+pyprecip/reading/read_file.py,sha256=kzgiwv8RZY4f77_bUWc2g_coBwvTQViHuWV9cAoBNTE,5184
+pyprecip/reading/test.py,sha256=OzdvigY0aC0DJ8sXokj8dOP7RqA8R77WKbALZ53wdaU,118
+pyprecip-0.0.2.dist-info/LICENSE,sha256=5VmicU9G7tYoRg6lG2pOTlnQR-ZNyyd1g9odyyrLYzU,1094
+pyprecip-0.0.2.dist-info/METADATA,sha256=mi4A5VO5HgA7_TvF7FFaVr-I2hjIeT66I_dOFT7DpTw,834
+pyprecip-0.0.2.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+pyprecip-0.0.2.dist-info/top_level.txt,sha256=TUBZn-IeYiCoBF5Mx6vzAEZDD083ijzLBA20d56im24,9
+pyprecip-0.0.2.dist-info/RECORD,,
```

