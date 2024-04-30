# Comparing `tmp/tflite_runtime_nightly-2.17.0.dev20240426-cp39-cp39-manylinux_2_34_armv7l.whl.zip` & `tmp/tflite_runtime_nightly-2.17.0.dev20240428-cp39-cp39-manylinux_2_34_armv7l.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1914728 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 24-Apr-27 05:15 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  5241996 b- defN 24-Apr-27 05:20 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    39490 b- defN 24-Apr-27 05:15 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 24-Apr-27 05:15 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 24-Apr-27 05:15 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1439 b- defN 24-Apr-27 05:20 tflite_runtime_nightly-2.17.0.dev20240426.dist-info/METADATA
--rw-rw-r--  2.0 unx      112 b- defN 24-Apr-27 05:20 tflite_runtime_nightly-2.17.0.dev20240426.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-27 05:20 tflite_runtime_nightly-2.17.0.dev20240426.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 24-Apr-27 05:20 tflite_runtime_nightly-2.17.0.dev20240426.dist-info/RECORD
-9 files, 5287600 bytes uncompressed, 1913182 bytes compressed:  63.8%
+Zip file size: 1914729 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       80 b- defN 24-Apr-29 05:18 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  5241996 b- defN 24-Apr-29 05:23 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    39490 b- defN 24-Apr-29 05:18 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 24-Apr-29 05:18 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 24-Apr-29 05:18 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1439 b- defN 24-Apr-29 05:23 tflite_runtime_nightly-2.17.0.dev20240428.dist-info/METADATA
+-rw-rw-r--  2.0 unx      112 b- defN 24-Apr-29 05:23 tflite_runtime_nightly-2.17.0.dev20240428.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-29 05:23 tflite_runtime_nightly-2.17.0.dev20240428.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 24-Apr-29 05:23 tflite_runtime_nightly-2.17.0.dev20240428.dist-info/RECORD
+9 files, 5287600 bytes uncompressed, 1913183 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.17.0.dev20240426.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.17.0.dev20240428.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.17.0.dev20240426.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.17.0.dev20240428.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.17.0.dev20240426.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.17.0.dev20240428.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.17.0.dev20240426.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.17.0.dev20240428.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.17.0dev20240426'
-__git_version__ = '0.6.0-163429-gf0dfc040579'
+__version__ = '2.17.0dev20240428'
+__git_version__ = '0.6.0-163448-g57f87057403'
```

## Comparing `tflite_runtime_nightly-2.17.0.dev20240426.dist-info/METADATA` & `tflite_runtime_nightly-2.17.0.dev20240428.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.17.0.dev20240426
+Version: 2.17.0.dev20240428
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `tflite_runtime_nightly-2.17.0.dev20240426.dist-info/RECORD` & `tflite_runtime_nightly-2.17.0.dev20240428.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tflite_runtime/__init__.py,sha256=F4ECtYt_-rYfM0DRft6DHgS7wXDJCIQKHnS_TZoumIU,80
+tflite_runtime/__init__.py,sha256=7sI3cBJ9GnwWVx386It6TDedG-ZqDmpLJ4iRDGpie4Q,80
 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so,sha256=6PbonVafcw6aQxR74B8o0i99kZNmsoAtK0ERP6bKB8M,5241996
 tflite_runtime/interpreter.py,sha256=Uvz3AcX8AUJ1xbrtmbaT8tmSIHQdELGHG4W5HWJpOCE,39490
 tflite_runtime/metrics_interface.py,sha256=dVu6SmbnQUntPgE5o6BxHVMyemwli-7F6tDfVMGrlYI,1542
 tflite_runtime/metrics_portable.py,sha256=YBiMNokP9JtoQaUcCRRY1T_iFSZGeWCjr6L0iUR6eY8,2048
-tflite_runtime_nightly-2.17.0.dev20240426.dist-info/METADATA,sha256=0piYXZPnQL0lvX5Vj4dJ7JzXgoDgrW4VSHnU80hJIWQ,1439
-tflite_runtime_nightly-2.17.0.dev20240426.dist-info/WHEEL,sha256=H_X0hyYwShjvxJpY03pCHdk9VYSkMJ-2tTyHKuG1QxU,112
-tflite_runtime_nightly-2.17.0.dev20240426.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
-tflite_runtime_nightly-2.17.0.dev20240426.dist-info/RECORD,,
+tflite_runtime_nightly-2.17.0.dev20240428.dist-info/METADATA,sha256=O4XRXHmqCNKxdgl56OkmVBzbX396AFcMn95vLktcvq0,1439
+tflite_runtime_nightly-2.17.0.dev20240428.dist-info/WHEEL,sha256=H_X0hyYwShjvxJpY03pCHdk9VYSkMJ-2tTyHKuG1QxU,112
+tflite_runtime_nightly-2.17.0.dev20240428.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
+tflite_runtime_nightly-2.17.0.dev20240428.dist-info/RECORD,,
```

