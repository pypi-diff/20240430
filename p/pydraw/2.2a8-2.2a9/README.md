# Comparing `tmp/pydraw-2.2a8-py3-none-any.whl.zip` & `tmp/pydraw-2.2a9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 121331 bytes, number of entries: 33
+Zip file size: 121325 bytes, number of entries: 33
 -rw-r--r--  2.0 unx      284 b- defN 24-Jan-17 03:41 pydraw/__init__.py
 -rw-r--r--  2.0 unx    16481 b- defN 23-Jan-02 18:04 pydraw/color.py
 -rw-r--r--  2.0 unx    11292 b- defN 23-Nov-15 03:50 pydraw/compound.py
 -rw-r--r--  2.0 unx      136 b- defN 22-Dec-20 05:27 pydraw/errors.py
 -rw-r--r--  2.0 unx     6647 b- defN 22-Dec-20 05:27 pydraw/location.py
 -rw-r--r--  2.0 unx   205312 b- defN 23-Jun-04 19:34 pydraw/objects.py
 -rw-r--r--  2.0 unx    26065 b- defN 22-Nov-03 15:19 pydraw/overload.py
@@ -23,13 +23,13 @@
 -rw-r--r--  2.0 unx     2746 b- defN 22-Dec-20 05:27 tests/objects_test.py
 -rw-r--r--  2.0 unx      449 b- defN 22-Nov-03 15:19 tests/overload_test.py
 -rw-r--r--  2.0 unx     1741 b- defN 22-Dec-20 05:27 tests/polygon_test.py
 -rw-r--r--  2.0 unx     1412 b- defN 22-Nov-03 15:19 tests/scene_test.py
 -rw-r--r--  2.0 unx     1255 b- defN 22-Dec-20 05:27 tests/screen_test.py
 -rw-r--r--  2.0 unx       51 b- defN 22-Nov-03 15:19 tests/text_test.py
 -rw-r--r--  2.0 unx     3775 b- defN 22-Dec-20 05:27 tests/tutorial.py
--rw-r--r--  2.0 unx    35148 b- defN 24-Jan-17 04:01 pydraw-2.2a8.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    10836 b- defN 24-Jan-17 04:01 pydraw-2.2a8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-17 04:01 pydraw-2.2a8.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Jan-17 04:01 pydraw-2.2a8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2488 b- defN 24-Jan-17 04:01 pydraw-2.2a8.dist-info/RECORD
-33 files, 527057 bytes uncompressed, 117471 bytes compressed:  77.7%
+-rw-r--r--  2.0 unx    35148 b- defN 24-Jan-17 04:15 pydraw-2.2a9.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    10811 b- defN 24-Jan-17 04:15 pydraw-2.2a9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jan-17 04:15 pydraw-2.2a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Jan-17 04:15 pydraw-2.2a9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2488 b- defN 24-Jan-17 04:15 pydraw-2.2a9.dist-info/RECORD
+33 files, 527032 bytes uncompressed, 117465 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -78,23 +78,23 @@
 
 Filename: tests/text_test.py
 Comment: 
 
 Filename: tests/tutorial.py
 Comment: 
 
-Filename: pydraw-2.2a8.dist-info/LICENSE.md
+Filename: pydraw-2.2a9.dist-info/LICENSE.md
 Comment: 
 
-Filename: pydraw-2.2a8.dist-info/METADATA
+Filename: pydraw-2.2a9.dist-info/METADATA
 Comment: 
 
-Filename: pydraw-2.2a8.dist-info/WHEEL
+Filename: pydraw-2.2a9.dist-info/WHEEL
 Comment: 
 
-Filename: pydraw-2.2a8.dist-info/top_level.txt
+Filename: pydraw-2.2a9.dist-info/top_level.txt
 Comment: 
 
-Filename: pydraw-2.2a8.dist-info/RECORD
+Filename: pydraw-2.2a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pydraw-2.2a8.dist-info/LICENSE.md` & `pydraw-2.2a9.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `pydraw-2.2a8.dist-info/METADATA` & `pydraw-2.2a9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pydraw
-Version: 2.2a8
+Version: 2.2a9
 Summary: A package designed to make graphics with Python simple and easy!
 Home-page: https://github.com/pydraw/pydraw
 Author: Noah Coetsee
 Author-email: noah@noahcoetsee.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: pillow
-Requires-Dist: pygobject
 
 ![pyDraw](https://pydraw.graphics/logo.png)
 
 ![version](https://img.shields.io/pypi/v/pydraw)
 
 This is a simple graphics library designed to make graphics
 and input simple and synchronized.
```

## Comparing `pydraw-2.2a8.dist-info/RECORD` & `pydraw-2.2a9.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -22,12 +22,12 @@
 tests/objects_test.py,sha256=hKoluSq7GxO-o9vM19o4D9whaYIZGeq_8FzgCdfC6ss,2746
 tests/overload_test.py,sha256=2pPWpu0EPXQIDamJwaa4EA2IaFpPXnFci1HwM42AiDo,449
 tests/polygon_test.py,sha256=kj0WyyC3qGE-Wk8tTovbJyRAeugKhMchO7-OQE7-35w,1741
 tests/scene_test.py,sha256=wJ_tWueyo6FWzd6thho-Tsgi8NQ6-lFOabxdQB0Z8_I,1412
 tests/screen_test.py,sha256=zx18pkJFV8fIojJzSuSSQmEO_j3sF3h02IZfiztlzvQ,1255
 tests/text_test.py,sha256=mFdYV5W4hKh02fuP4giujf9J8FFYvqQMgV8L0gnyMzs,51
 tests/tutorial.py,sha256=16sSb2Dlx08jysR5z_fV9ASK0an0e2U493Edh8uRzKg,3775
-pydraw-2.2a8.dist-info/LICENSE.md,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
-pydraw-2.2a8.dist-info/METADATA,sha256=ZtvMV8f0NYIIAr9-cIEqD8AjoEsHHWmHJ2ke3iNEktU,10836
-pydraw-2.2a8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-pydraw-2.2a8.dist-info/top_level.txt,sha256=CstEtkSWciqMigRl_I_q9ri8CYlp5tRC7jqtkG43Dlo,13
-pydraw-2.2a8.dist-info/RECORD,,
+pydraw-2.2a9.dist-info/LICENSE.md,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
+pydraw-2.2a9.dist-info/METADATA,sha256=n-iNKUhIlabHliL7SZ6JvK03AENHHmkJIDWPXo88eGw,10811
+pydraw-2.2a9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+pydraw-2.2a9.dist-info/top_level.txt,sha256=CstEtkSWciqMigRl_I_q9ri8CYlp5tRC7jqtkG43Dlo,13
+pydraw-2.2a9.dist-info/RECORD,,
```

