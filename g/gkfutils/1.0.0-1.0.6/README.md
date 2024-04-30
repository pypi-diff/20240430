# Comparing `tmp/gkfutils-1.0.0-py3-none-any.whl.zip` & `tmp/gkfutils-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,17 @@
-Zip file size: 31273 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      265 b- defN 22-Jun-11 15:21 gkfutils/__init__.py
--rw-rw-rw-  2.0 fat       89 b- defN 22-Jun-11 15:21 gkfutils/__main__.py
--rw-rw-rw-  2.0 fat    48774 b- defN 22-May-17 09:16 gkfutils/det.py
--rw-rw-rw-  2.0 fat     1176 b- defN 22-May-13 05:57 gkfutils/pcl.py
--rw-rw-rw-  2.0 fat    15310 b- defN 22-May-13 06:00 gkfutils/seg.py
--rw-rw-rw-  2.0 fat    28091 b- defN 22-May-13 06:00 gkfutils/utils.py
--rw-rw-rw-  2.0 fat       53 b- defN 22-Jun-11 15:24 gkfutils-1.0.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 22-Jun-11 15:24 gkfutils-1.0.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 22-Jun-11 15:24 gkfutils-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      640 b- defN 22-Jun-11 15:24 gkfutils-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      851 b- defN 22-Jun-11 15:24 gkfutils-1.0.0.dist-info/RECORD
-11 files, 95355 bytes uncompressed, 29865 bytes compressed:  68.7%
+Zip file size: 183582 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx      152 b- defN 24-Apr-03 09:05 gkfutils/__init__.py
+-rw-rw-r--  2.0 unx       89 b- defN 24-Mar-20 06:17 gkfutils/__main__.py
+-rw-rw-r--  2.0 unx      118 b- defN 24-Apr-03 09:10 gkfutils/main_gkfutils_test.py
+-rw-rw-r--  2.0 unx   332579 b- defN 24-Apr-29 02:52 gkfutils/main_test.py
+-rw-rw-r--  2.0 unx       21 b- defN 24-Apr-03 09:04 gkfutils/cv/__init__.py
+-rw-rw-r--  2.0 unx   630568 b- defN 24-Apr-22 01:39 gkfutils/cv/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-29 03:51 gkfutils/nlp/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-29 03:51 gkfutils/radar/__init__.py
+-rw-rw-r--  2.0 unx       20 b- defN 24-Apr-03 09:04 gkfutils/utils/__init__.py
+-rw-rw-r--  2.0 unx    67842 b- defN 24-Apr-25 06:26 gkfutils/utils/utils.py
+-rw-rw-r--  2.0 unx     1073 b- defN 24-Apr-30 07:01 gkfutils-1.0.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      370 b- defN 24-Apr-30 07:01 gkfutils-1.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-30 07:01 gkfutils-1.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 24-Apr-30 07:01 gkfutils-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1183 b- defN 24-Apr-30 07:01 gkfutils-1.0.6.dist-info/RECORD
+15 files, 1034116 bytes uncompressed, 181626 bytes compressed:  82.4%
```

## zipnote {}

```diff
@@ -1,34 +1,46 @@
 Filename: gkfutils/__init__.py
 Comment: 
 
 Filename: gkfutils/__main__.py
 Comment: 
 
-Filename: gkfutils/det.py
+Filename: gkfutils/main_gkfutils_test.py
 Comment: 
 
-Filename: gkfutils/pcl.py
+Filename: gkfutils/main_test.py
 Comment: 
 
-Filename: gkfutils/seg.py
+Filename: gkfutils/cv/__init__.py
 Comment: 
 
-Filename: gkfutils/utils.py
+Filename: gkfutils/cv/utils.py
 Comment: 
 
-Filename: gkfutils-1.0.0.dist-info/entry_points.txt
+Filename: gkfutils/nlp/__init__.py
 Comment: 
 
-Filename: gkfutils-1.0.0.dist-info/top_level.txt
+Filename: gkfutils/radar/__init__.py
 Comment: 
 
-Filename: gkfutils-1.0.0.dist-info/WHEEL
+Filename: gkfutils/utils/__init__.py
 Comment: 
 
-Filename: gkfutils-1.0.0.dist-info/METADATA
+Filename: gkfutils/utils/utils.py
 Comment: 
 
-Filename: gkfutils-1.0.0.dist-info/RECORD
+Filename: gkfutils-1.0.6.dist-info/LICENSE
+Comment: 
+
+Filename: gkfutils-1.0.6.dist-info/METADATA
+Comment: 
+
+Filename: gkfutils-1.0.6.dist-info/WHEEL
+Comment: 
+
+Filename: gkfutils-1.0.6.dist-info/top_level.txt
+Comment: 
+
+Filename: gkfutils-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gkfutils/__init__.py

```diff
@@ -1,14 +1,8 @@
 # -*- coding:utf-8 -*-
-
-from .det import *
-from .pcl import *
-from .seg import *
-from .utils import *
-from gkfutils import det
-from gkfutils import pcl
-from gkfutils import seg
-from gkfutils import utils
-
+from . import cv
+from . import nlp
+from . import radar
+from . import utils
 
 __appname__ = "gkfutils"
-__version__ = "1.0.0"
+__version__ = "1.0.6"
```

