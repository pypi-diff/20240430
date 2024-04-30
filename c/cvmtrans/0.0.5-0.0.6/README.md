# Comparing `tmp/cvmtrans-0.0.5.tar.gz` & `tmp/cvmtrans-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvmtrans-0.0.5.tar", last modified: Tue Apr 30 07:40:09 2024, max compression
+gzip compressed data, was "cvmtrans-0.0.6.tar", last modified: Tue Apr 30 07:41:45 2024, max compression
```

## Comparing `cvmtrans-0.0.5.tar` & `cvmtrans-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:40:09.702777 cvmtrans-0.0.5/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4807 2024-04-30 07:40:09.702642 cvmtrans-0.0.5/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4058 2024-04-30 07:16:28.000000 cvmtrans-0.0.5/README.md
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:40:09.701298 cvmtrans-0.0.5/cvmtrans/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      297 2024-04-30 07:40:02.000000 cvmtrans-0.0.5/cvmtrans/__init__.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8775 2024-04-08 10:09:38.000000 cvmtrans-0.0.5/cvmtrans/cvmtrans.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3719 2024-04-30 06:48:59.000000 cvmtrans-0.0.5/cvmtrans/cvmtrans_cut_tags.py
--rwx------   0 cuiqingpo   (501) staff       (20)     3539 2024-04-03 13:02:47.000000 cvmtrans-0.0.5/cvmtrans/cvmtrans_extract_reads.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      536 2024-04-03 12:21:00.000000 cvmtrans-0.0.5/cvmtrans/data_process.sh
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4417 2024-04-03 03:57:33.000000 cvmtrans-0.0.5/cvmtrans/embl_parse.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4689 2024-04-03 06:52:24.000000 cvmtrans-0.0.5/cvmtrans/embl_parse_test.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      152 2024-04-03 11:01:42.000000 cvmtrans-0.0.5/cvmtrans/gb2fa.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3216 2024-04-03 03:02:06.000000 cvmtrans-0.0.5/cvmtrans/parse_bam.py
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:40:09.702420 cvmtrans-0.0.5/cvmtrans.egg-info/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4807 2024-04-30 07:40:09.000000 cvmtrans-0.0.5/cvmtrans.egg-info/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      452 2024-04-30 07:40:09.000000 cvmtrans-0.0.5/cvmtrans.egg-info/SOURCES.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2024-04-30 07:40:09.000000 cvmtrans-0.0.5/cvmtrans.egg-info/dependency_links.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      146 2024-04-30 07:40:09.000000 cvmtrans-0.0.5/cvmtrans.egg-info/entry_points.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       40 2024-04-30 07:40:09.000000 cvmtrans-0.0.5/cvmtrans.egg-info/requires.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2024-04-30 07:40:09.000000 cvmtrans-0.0.5/cvmtrans.egg-info/top_level.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       85 2024-04-30 07:07:54.000000 cvmtrans-0.0.5/requirements.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2024-04-30 07:40:09.702827 cvmtrans-0.0.5/setup.cfg
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2260 2024-04-30 07:39:45.000000 cvmtrans-0.0.5/setup.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:41:45.762596 cvmtrans-0.0.6/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4807 2024-04-30 07:41:45.762472 cvmtrans-0.0.6/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4058 2024-04-30 07:16:28.000000 cvmtrans-0.0.6/README.md
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:41:45.761453 cvmtrans-0.0.6/cvmtrans/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      297 2024-04-30 07:41:36.000000 cvmtrans-0.0.6/cvmtrans/__init__.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8775 2024-04-08 10:09:38.000000 cvmtrans-0.0.6/cvmtrans/cvmtrans.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3719 2024-04-30 06:48:59.000000 cvmtrans-0.0.6/cvmtrans/cvmtrans_cut_tags.py
+-rwx------   0 cuiqingpo   (501) staff       (20)     3539 2024-04-03 13:02:47.000000 cvmtrans-0.0.6/cvmtrans/cvmtrans_extract_reads.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      536 2024-04-03 12:21:00.000000 cvmtrans-0.0.6/cvmtrans/data_process.sh
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4417 2024-04-03 03:57:33.000000 cvmtrans-0.0.6/cvmtrans/embl_parse.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4689 2024-04-03 06:52:24.000000 cvmtrans-0.0.6/cvmtrans/embl_parse_test.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      152 2024-04-03 11:01:42.000000 cvmtrans-0.0.6/cvmtrans/gb2fa.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3216 2024-04-03 03:02:06.000000 cvmtrans-0.0.6/cvmtrans/parse_bam.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:41:45.762269 cvmtrans-0.0.6/cvmtrans.egg-info/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4807 2024-04-30 07:41:45.000000 cvmtrans-0.0.6/cvmtrans.egg-info/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      452 2024-04-30 07:41:45.000000 cvmtrans-0.0.6/cvmtrans.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2024-04-30 07:41:45.000000 cvmtrans-0.0.6/cvmtrans.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      167 2024-04-30 07:41:45.000000 cvmtrans-0.0.6/cvmtrans.egg-info/entry_points.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       40 2024-04-30 07:41:45.000000 cvmtrans-0.0.6/cvmtrans.egg-info/requires.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2024-04-30 07:41:45.000000 cvmtrans-0.0.6/cvmtrans.egg-info/top_level.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       85 2024-04-30 07:07:54.000000 cvmtrans-0.0.6/requirements.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2024-04-30 07:41:45.762645 cvmtrans-0.0.6/setup.cfg
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2281 2024-04-30 07:41:31.000000 cvmtrans-0.0.6/setup.py
```

### Comparing `cvmtrans-0.0.5/PKG-INFO` & `cvmtrans-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvmtrans
-Version: 0.0.5
+Version: 0.0.6
 Summary: Transposon data process
 Home-page: https://github.com/hbucqp/cvmtrans
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,transposon,transposon sequecing
 Platform: any
```

### Comparing `cvmtrans-0.0.5/README.md` & `cvmtrans-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.5/cvmtrans/cvmtrans.py` & `cvmtrans-0.0.6/cvmtrans/cvmtrans.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.5/cvmtrans/cvmtrans_cut_tags.py` & `cvmtrans-0.0.6/cvmtrans/cvmtrans_cut_tags.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.5/cvmtrans/cvmtrans_extract_reads.py` & `cvmtrans-0.0.6/cvmtrans/cvmtrans_extract_reads.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.5/cvmtrans/data_process.sh` & `cvmtrans-0.0.6/cvmtrans/data_process.sh`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.5/cvmtrans/embl_parse.py` & `cvmtrans-0.0.6/cvmtrans/embl_parse.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.5/cvmtrans/embl_parse_test.py` & `cvmtrans-0.0.6/cvmtrans/embl_parse_test.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.5/cvmtrans/parse_bam.py` & `cvmtrans-0.0.6/cvmtrans/parse_bam.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.5/cvmtrans.egg-info/PKG-INFO` & `cvmtrans-0.0.6/cvmtrans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvmtrans
-Version: 0.0.5
+Version: 0.0.6
 Summary: Transposon data process
 Home-page: https://github.com/hbucqp/cvmtrans
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,transposon,transposon sequecing
 Platform: any
```

### Comparing `cvmtrans-0.0.5/setup.py` & `cvmtrans-0.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,12 +61,12 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11'
     ],
     entry_points={
         'console_scripts': [
             'cvmtrans=cvmtrans.cvmtrans:main',
-            'cvmtrans2=cvmtrans.cvmtrans_cut_tags:main',
-            'cvmtrans1=cvmtrans.cvmtrans_extract_reads:main'
+            'cvmtrans_cut_tags=cvmtrans.cvmtrans_cut_tags:main',
+            'cvmtrans_extract_reads=cvmtrans.cvmtrans_extract_reads:main'
         ]
     },
 )
```

