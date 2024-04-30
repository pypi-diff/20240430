# Comparing `tmp/cvmtrans-0.0.1.tar.gz` & `tmp/cvmtrans-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvmtrans-0.0.1.tar", last modified: Tue Apr 30 07:16:33 2024, max compression
+gzip compressed data, was "cvmtrans-0.0.2.tar", last modified: Tue Apr 30 07:22:39 2024, max compression
```

## Comparing `cvmtrans-0.0.1.tar` & `cvmtrans-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:16:33.645872 cvmtrans-0.0.1/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4807 2024-04-30 07:16:33.645740 cvmtrans-0.0.1/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4058 2024-04-30 07:16:28.000000 cvmtrans-0.0.1/README.md
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:16:33.644742 cvmtrans-0.0.1/cvmtrans/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      297 2024-04-30 07:01:37.000000 cvmtrans-0.0.1/cvmtrans/__init__.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6571 2024-04-03 11:00:48.000000 cvmtrans-0.0.1/cvmtrans/cvmtrans.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3719 2024-04-30 06:48:59.000000 cvmtrans-0.0.1/cvmtrans/cvmtrans_cut_tags.py
--rwx------   0 cuiqingpo   (501) staff       (20)     3539 2024-04-03 13:02:47.000000 cvmtrans-0.0.1/cvmtrans/cvmtrans_extract_reads.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      536 2024-04-03 12:21:00.000000 cvmtrans-0.0.1/cvmtrans/data_process.sh
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4417 2024-04-03 03:57:33.000000 cvmtrans-0.0.1/cvmtrans/embl_parse.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4689 2024-04-03 06:52:24.000000 cvmtrans-0.0.1/cvmtrans/embl_parse_test.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      152 2024-04-03 11:01:42.000000 cvmtrans-0.0.1/cvmtrans/gb2fa.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3216 2024-04-03 03:02:06.000000 cvmtrans-0.0.1/cvmtrans/parse_bam.py
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:16:33.645547 cvmtrans-0.0.1/cvmtrans.egg-info/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4807 2024-04-30 07:16:33.000000 cvmtrans-0.0.1/cvmtrans.egg-info/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      452 2024-04-30 07:16:33.000000 cvmtrans-0.0.1/cvmtrans.egg-info/SOURCES.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2024-04-30 07:16:33.000000 cvmtrans-0.0.1/cvmtrans.egg-info/dependency_links.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      167 2024-04-30 07:16:33.000000 cvmtrans-0.0.1/cvmtrans.egg-info/entry_points.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       40 2024-04-30 07:16:33.000000 cvmtrans-0.0.1/cvmtrans.egg-info/requires.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2024-04-30 07:16:33.000000 cvmtrans-0.0.1/cvmtrans.egg-info/top_level.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       85 2024-04-30 07:07:54.000000 cvmtrans-0.0.1/requirements.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2024-04-30 07:16:33.645919 cvmtrans-0.0.1/setup.cfg
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2283 2024-04-30 07:09:08.000000 cvmtrans-0.0.1/setup.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:22:39.043439 cvmtrans-0.0.2/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4807 2024-04-30 07:22:39.043327 cvmtrans-0.0.2/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4058 2024-04-30 07:16:28.000000 cvmtrans-0.0.2/README.md
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:22:39.042356 cvmtrans-0.0.2/cvmtrans/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      297 2024-04-30 07:22:22.000000 cvmtrans-0.0.2/cvmtrans/__init__.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6571 2024-04-03 11:00:48.000000 cvmtrans-0.0.2/cvmtrans/cvmtrans.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3719 2024-04-30 06:48:59.000000 cvmtrans-0.0.2/cvmtrans/cvmtrans_cut_tags.py
+-rwx------   0 cuiqingpo   (501) staff       (20)     3539 2024-04-03 13:02:47.000000 cvmtrans-0.0.2/cvmtrans/cvmtrans_extract_reads.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      536 2024-04-03 12:21:00.000000 cvmtrans-0.0.2/cvmtrans/data_process.sh
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4417 2024-04-03 03:57:33.000000 cvmtrans-0.0.2/cvmtrans/embl_parse.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4689 2024-04-03 06:52:24.000000 cvmtrans-0.0.2/cvmtrans/embl_parse_test.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      152 2024-04-03 11:01:42.000000 cvmtrans-0.0.2/cvmtrans/gb2fa.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3216 2024-04-03 03:02:06.000000 cvmtrans-0.0.2/cvmtrans/parse_bam.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:22:39.043153 cvmtrans-0.0.2/cvmtrans.egg-info/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4807 2024-04-30 07:22:38.000000 cvmtrans-0.0.2/cvmtrans.egg-info/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      452 2024-04-30 07:22:38.000000 cvmtrans-0.0.2/cvmtrans.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2024-04-30 07:22:38.000000 cvmtrans-0.0.2/cvmtrans.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      190 2024-04-30 07:22:38.000000 cvmtrans-0.0.2/cvmtrans.egg-info/entry_points.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       40 2024-04-30 07:22:38.000000 cvmtrans-0.0.2/cvmtrans.egg-info/requires.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2024-04-30 07:22:38.000000 cvmtrans-0.0.2/cvmtrans.egg-info/top_level.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       85 2024-04-30 07:07:54.000000 cvmtrans-0.0.2/requirements.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2024-04-30 07:22:39.043480 cvmtrans-0.0.2/setup.cfg
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2305 2024-04-30 07:22:18.000000 cvmtrans-0.0.2/setup.py
```

### Comparing `cvmtrans-0.0.1/PKG-INFO` & `cvmtrans-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvmtrans
-Version: 0.0.1
+Version: 0.0.2
 Summary: Transposon data process
 Home-page: https://github.com/hbucqp/cvmtrans
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,transposon,transposon sequecing
 Platform: any
```

### Comparing `cvmtrans-0.0.1/README.md` & `cvmtrans-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.1/cvmtrans/cvmtrans.py` & `cvmtrans-0.0.2/cvmtrans/cvmtrans.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.1/cvmtrans/cvmtrans_cut_tags.py` & `cvmtrans-0.0.2/cvmtrans/cvmtrans_cut_tags.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.1/cvmtrans/cvmtrans_extract_reads.py` & `cvmtrans-0.0.2/cvmtrans/cvmtrans_extract_reads.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.1/cvmtrans/data_process.sh` & `cvmtrans-0.0.2/cvmtrans/data_process.sh`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.1/cvmtrans/embl_parse.py` & `cvmtrans-0.0.2/cvmtrans/embl_parse.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.1/cvmtrans/embl_parse_test.py` & `cvmtrans-0.0.2/cvmtrans/embl_parse_test.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.1/cvmtrans/parse_bam.py` & `cvmtrans-0.0.2/cvmtrans/parse_bam.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.1/cvmtrans.egg-info/PKG-INFO` & `cvmtrans-0.0.2/cvmtrans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvmtrans
-Version: 0.0.1
+Version: 0.0.2
 Summary: Transposon data process
 Home-page: https://github.com/hbucqp/cvmtrans
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,transposon,transposon sequecing
 Platform: any
```

### Comparing `cvmtrans-0.0.1/setup.py` & `cvmtrans-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,12 +61,12 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11'
     ],
     entry_points={
         'console_scripts': [
             'cvmtrans=cvmtrans.cvmtrans:main',
-            'cvmtrans_cut_tags=cvmtrans.cvmtrans_cut_tags:main',
-            'cvmtrans_extract_reads=cvmtrans.cvmtrans_extract_reads:main',
+            'cvmtrans_cut_tags=cvmtrans_cut_tags.cvmtrans_cut_tags:main',
+            'cvmtrans_extract_reads=cvmtrans_extract_reads.cvmtrans_extract_reads:main'
         ],
     },
 )
```

