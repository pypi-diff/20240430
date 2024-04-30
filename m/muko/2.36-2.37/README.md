# Comparing `tmp/muko-2.36-py3-none-any.whl.zip` & `tmp/muko-2.37-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 2121054 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-01 07:17 muko/__init__.py
--rw-rw-rw-  2.0 fat   752640 b- defN 24-Apr-29 12:03 muko/cmuko.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat  1088944 b- defN 24-Apr-29 12:02 muko/cmuko.cpython-38-darwin.so
--rw-rw-rw-  2.0 fat  2082964 b- defN 24-Apr-01 07:17 muko/font/default.otf
--rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-29 12:03 muko-2.36.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1275 b- defN 24-Apr-29 12:03 muko-2.36.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-29 12:03 muko-2.36.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-29 12:03 muko-2.36.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-29 12:03 muko-2.36.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      787 b- defN 24-Apr-29 12:03 muko-2.36.dist-info/RECORD
-10 files, 3927821 bytes uncompressed, 2119728 bytes compressed:  46.0%
+Zip file size: 2121684 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat       20 b- defN 24-Mar-13 17:30 muko/__init__.py
+-rw-rw-rw-  2.0 fat   754688 b- defN 24-Apr-29 14:56 muko/cmuko.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  1088944 b- defN 24-Apr-29 14:26 muko/cmuko.cpython-38-darwin.so
+-rw-rw-rw-  2.0 fat  2082964 b- defN 24-Feb-08 07:11 muko/font/default.otf
+-rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-29 14:56 muko-2.37.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1275 b- defN 24-Apr-29 14:56 muko-2.37.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-29 14:56 muko-2.37.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-29 14:56 muko-2.37.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-29 14:56 muko-2.37.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      787 b- defN 24-Apr-29 14:56 muko-2.37.dist-info/RECORD
+10 files, 3929869 bytes uncompressed, 2120358 bytes compressed:  46.1%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: muko/cmuko.cpython-38-darwin.so
 Comment: 
 
 Filename: muko/font/default.otf
 Comment: 
 
-Filename: muko-2.36.dist-info/LICENSE
+Filename: muko-2.37.dist-info/LICENSE
 Comment: 
 
-Filename: muko-2.36.dist-info/METADATA
+Filename: muko-2.37.dist-info/METADATA
 Comment: 
 
-Filename: muko-2.36.dist-info/WHEEL
+Filename: muko-2.37.dist-info/WHEEL
 Comment: 
 
-Filename: muko-2.36.dist-info/entry_points.txt
+Filename: muko-2.37.dist-info/entry_points.txt
 Comment: 
 
-Filename: muko-2.36.dist-info/top_level.txt
+Filename: muko-2.37.dist-info/top_level.txt
 Comment: 
 
-Filename: muko-2.36.dist-info/RECORD
+Filename: muko-2.37.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `muko-2.36.dist-info/LICENSE` & `muko-2.37.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `muko-2.36.dist-info/METADATA` & `muko-2.37.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muko
-Version: 2.36
+Version: 2.37
 Summary: 加速实现AIGC、自动办公的中文编程工具
 Home-page: https://www.mikooo.cn
 Author: Milk
 Author-email: 719496375@qq.com
 License: The MIT License
 Platform: win64
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `muko-2.36.dist-info/RECORD` & `muko-2.37.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 muko/__init__.py,sha256=CCRGa1csLmHKI_CslhtoPnqhEJA3mszIsRjACQuz5iE,20
-muko/cmuko.cp38-win_amd64.pyd,sha256=rYBhAutAYnkTatiiK5kEvGZCq83HMKmznJ4-YdW_a1U,752640
+muko/cmuko.cp38-win_amd64.pyd,sha256=TRqt0JQLBlJVxBi-6WK0IW7LkyJ1vpXCp0oFKG52N8M,754688
 muko/cmuko.cpython-38-darwin.so,sha256=y7SDH7BvUIS6oztZrnPyJN-rXIKPUljFpMjRYaYfQZw,1088944
 muko/font/default.otf,sha256=ZMqD7VMsbmTwwTRN4d72gVQLIekvjl5SSCvxs8-O4GA,2082964
-muko-2.36.dist-info/LICENSE,sha256=RwagnXR-4KxFgkvsh5PWaPhlca1CH_BNf-ozi5vp0fw,1074
-muko-2.36.dist-info/METADATA,sha256=T-LWPBQ2B-JZ8LZ3uxM_-_QKcDtuilQo1lQAHYw_eTQ,1275
-muko-2.36.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-muko-2.36.dist-info/entry_points.txt,sha256=eqGnTHtEVMYwfXVk1Z9MhC8O2N8wuqAbr0lisLmrkxs,20
-muko-2.36.dist-info/top_level.txt,sha256=fp2J4q9iyOPhu1UrXQqzVFSagtatDPDXHXAFWfVJk2M,5
-muko-2.36.dist-info/RECORD,,
+muko-2.37.dist-info/LICENSE,sha256=RwagnXR-4KxFgkvsh5PWaPhlca1CH_BNf-ozi5vp0fw,1074
+muko-2.37.dist-info/METADATA,sha256=EFy5QuRtPEu4X-XyDmn5xJ88prGYl0JrbNPCOctZXvc,1275
+muko-2.37.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+muko-2.37.dist-info/entry_points.txt,sha256=eqGnTHtEVMYwfXVk1Z9MhC8O2N8wuqAbr0lisLmrkxs,20
+muko-2.37.dist-info/top_level.txt,sha256=fp2J4q9iyOPhu1UrXQqzVFSagtatDPDXHXAFWfVJk2M,5
+muko-2.37.dist-info/RECORD,,
```

