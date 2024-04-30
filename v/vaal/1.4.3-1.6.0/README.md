# Comparing `tmp/vaal-1.4.3-py3-none-any.whl.zip` & `tmp/vaal-1.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12025 bytes, number of entries: 9
--rw-rw-r--  2.0 unx      464 b- defN 23-Aug-16 19:33 deepview/vaal/__init__.py
--rw-rw-r--  2.0 unx     1829 b- defN 23-Aug-16 19:33 deepview/vaal/camera.py
--rw-rw-r--  2.0 unx    13008 b- defN 23-Aug-16 19:33 deepview/vaal/context.py
--rw-rw-r--  2.0 unx     9004 b- defN 23-Aug-16 19:33 deepview/vaal/library.py
--rw-rw-r--  2.0 unx    11710 b- defN 23-Aug-16 19:37 vaal-1.4.3.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      229 b- defN 23-Aug-16 19:37 vaal-1.4.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Aug-16 19:37 vaal-1.4.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Aug-16 19:37 vaal-1.4.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      698 b- defN 23-Aug-16 19:37 vaal-1.4.3.dist-info/RECORD
-9 files, 37043 bytes uncompressed, 10831 bytes compressed:  70.8%
+Zip file size: 11955 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      453 b- defN 24-Apr-30 18:02 deepview/vaal/__init__.py
+-rw-rw-r--  2.0 unx     1829 b- defN 24-Apr-30 18:02 deepview/vaal/camera.py
+-rw-rw-r--  2.0 unx    13009 b- defN 24-Apr-30 18:02 deepview/vaal/context.py
+-rw-rw-r--  2.0 unx     8877 b- defN 24-Apr-30 18:02 deepview/vaal/library.py
+-rw-rw-r--  2.0 unx    11710 b- defN 24-Apr-30 18:06 vaal-1.6.0.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      229 b- defN 24-Apr-30 18:06 vaal-1.6.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-30 18:06 vaal-1.6.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 24-Apr-30 18:06 vaal-1.6.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      698 b- defN 24-Apr-30 18:06 vaal-1.6.0.dist-info/RECORD
+9 files, 36906 bytes uncompressed, 10761 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: deepview/vaal/context.py
 Comment: 
 
 Filename: deepview/vaal/library.py
 Comment: 
 
-Filename: vaal-1.4.3.dist-info/LICENSE.txt
+Filename: vaal-1.6.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: vaal-1.4.3.dist-info/METADATA
+Filename: vaal-1.6.0.dist-info/METADATA
 Comment: 
 
-Filename: vaal-1.4.3.dist-info/WHEEL
+Filename: vaal-1.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: vaal-1.4.3.dist-info/top_level.txt
+Filename: vaal-1.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: vaal-1.4.3.dist-info/RECORD
+Filename: vaal-1.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deepview/vaal/__init__.py

```diff
@@ -2,10 +2,10 @@
 #
 # Unauthorized copying of this file, via any medium is strictly prohibited
 # Proprietary and confidential.
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
-from .library import lib, version, strerror, load_library, ImageProc, ModelType
+from .library import lib, version, strerror, load_library, ImageProc
 from .context import Context
 from .camera import Camera, CameraType
```

## deepview/vaal/context.py

```diff
@@ -6,26 +6,26 @@
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
 from ctypes import \
     cast, c_void_p, c_int, c_int32, c_uint32, c_float, c_size_t, \
     create_string_buffer, byref
 from deepview.vaal.library import VAALBox, VAALKeypoint, VAALEuler, \
-    lib, strerror, Type, ModelType
+    lib, strerror, Type
 from enum import Enum
 
 
 class Context:
     """
     DeepView VAAL Context is used to manage DeepViewRT models with VisionPack.
     """
 
-    def __init__(self, engine="npu", model_type=ModelType.NONE):
-        if model_type != ModelType.NONE:
-            c_model_type = c_uint32(model_type.value)
+    def __init__(self, engine="npu", model_type=None):
+        if model_type != None and isinstance(model_type, str):
+            c_model_type = model_type.encode('utf-8')
             self._handle = lib.vaal_model_probe(
                 engine.encode('utf-8'), c_model_type)
         else:
             self._handle = lib.vaal_context_create(engine.encode('utf-8'))
 
     def __del__(self):
         if self._handle is not None:
```

## deepview/vaal/library.py

```diff
@@ -38,22 +38,14 @@
     WHITENING = 2
     SIGNED_NORM = 4
     IMAGENET = 8
     MIRROR = 0x1000
     FLIP = 0x2000
 
 
-class ModelType(Enum):
-    NONE = 0
-    PEOPLE_DETECTION = 10
-    FACE_DETECTION = 20
-    HEAD_POSE = 30
-    HUMAN_POSE = 40
-
-
 class VAALBox(Structure):
     _fields_ = [('xmin', c_float),
                 ('ymin', c_float),
                 ('xmax', c_float),
                 ('ymax', c_float),
                 ('score', c_float),
                 ('label', c_int)]
@@ -309,15 +301,15 @@
     lib.vaal_output_count.argtypes = [c_void_p]
     lib.vaal_output_count.restype = c_int
 
     lib.vaal_output_name.argtypes = [c_void_p, c_int]
     lib.vaal_output_name.restype = c_char_p
 
     # model.c Implementations
-    lib.vaal_model_probe.argtypes = [c_char_p, c_uint32]
+    lib.vaal_model_probe.argtypes = [c_char_p, c_char_p]
     lib.vaal_model_probe.restype = c_void_p
 
     lib.vaal_model_path.argtypes = None
     lib.vaal_model_path.restype = c_char_p
 
 
 if 'lib' not in locals():
```

## Comparing `vaal-1.4.3.dist-info/LICENSE.txt` & `vaal-1.6.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

