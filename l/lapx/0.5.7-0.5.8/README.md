# Comparing `tmp/lapx-0.5.7.tar.gz` & `tmp/lapx-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapx-0.5.7.tar", last modified: Thu Mar 21 01:36:43 2024, max compression
+gzip compressed data, was "lapx-0.5.8.tar", last modified: Mon Apr 29 23:23:20 2024, max compression
```

## Comparing `lapx-0.5.7.tar` & `lapx-0.5.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 01:36:43.417023 lapx-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-21 01:36:30.000000 lapx-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-21 01:36:30.000000 lapx-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-03-21 01:36:43.417023 lapx-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-03-21 01:36:30.000000 lapx-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 01:36:43.413023 lapx-0.5.7/_lapjv_src/
--rw-r--r--   0 runner    (1001) docker     (127)   568004 2024-03-21 01:36:43.000000 lapx-0.5.7/_lapjv_src/_lapjv.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-03-21 01:36:30.000000 lapx-0.5.7/_lapjv_src/_lapjv.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-03-21 01:36:30.000000 lapx-0.5.7/_lapjv_src/lapjv.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-21 01:36:30.000000 lapx-0.5.7/_lapjv_src/lapjv.h
--rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-03-21 01:36:30.000000 lapx-0.5.7/_lapjv_src/lapmod.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 01:36:43.413023 lapx-0.5.7/lap/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-21 01:36:30.000000 lapx-0.5.7/lap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-03-21 01:36:30.000000 lapx-0.5.7/lap/lapmod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 01:36:43.417023 lapx-0.5.7/lap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 01:36:30.000000 lapx-0.5.7/lap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1415310 2024-03-21 01:36:30.000000 lapx-0.5.7/lap/tests/cost_eps.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-03-21 01:36:30.000000 lapx-0.5.7/lap/tests/test_arr_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-03-21 01:36:30.000000 lapx-0.5.7/lap/tests/test_lapjv.py
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-03-21 01:36:30.000000 lapx-0.5.7/lap/tests/test_lapmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-03-21 01:36:30.000000 lapx-0.5.7/lap/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 01:36:43.417023 lapx-0.5.7/lapx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-03-21 01:36:43.000000 lapx-0.5.7/lapx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-21 01:36:43.000000 lapx-0.5.7/lapx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 01:36:43.000000 lapx-0.5.7/lapx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-21 01:36:43.000000 lapx-0.5.7/lapx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-21 01:36:43.000000 lapx-0.5.7/lapx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-21 01:36:30.000000 lapx-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-21 01:36:30.000000 lapx-0.5.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 01:36:43.417023 lapx-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-03-21 01:36:30.000000 lapx-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:23:20.365656 lapx-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-29 23:23:09.000000 lapx-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-29 23:23:09.000000 lapx-0.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-29 23:23:20.365656 lapx-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-29 23:23:09.000000 lapx-0.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:23:20.357656 lapx-0.5.8/_lapjv_src/
+-rw-r--r--   0 runner    (1001) docker     (127)   569034 2024-04-29 23:23:20.000000 lapx-0.5.8/_lapjv_src/_lapjv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-29 23:23:09.000000 lapx-0.5.8/_lapjv_src/_lapjv.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-04-29 23:23:09.000000 lapx-0.5.8/_lapjv_src/lapjv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-29 23:23:09.000000 lapx-0.5.8/_lapjv_src/lapjv.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-04-29 23:23:09.000000 lapx-0.5.8/_lapjv_src/lapmod.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:23:20.361656 lapx-0.5.8/lap/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/lapmod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:23:20.361656 lapx-0.5.8/lap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1415310 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/tests/cost_eps.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/tests/test_arr_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/tests/test_lapjv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/tests/test_lapmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:23:20.361656 lapx-0.5.8/lapx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-29 23:23:20.000000 lapx-0.5.8/lapx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-29 23:23:20.000000 lapx-0.5.8/lapx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 23:23:20.000000 lapx-0.5.8/lapx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-29 23:23:20.000000 lapx-0.5.8/lapx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-29 23:23:20.000000 lapx-0.5.8/lapx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-29 23:23:09.000000 lapx-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-29 23:23:09.000000 lapx-0.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 23:23:20.365656 lapx-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-29 23:23:09.000000 lapx-0.5.8/setup.py
```

### Comparing `lapx-0.5.7/LICENSE` & `lapx-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lapx-0.5.7/PKG-INFO` & `lapx-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lapx
-Version: 0.5.7
+Version: 0.5.8
 Summary: Linear Assignment Problem solver (LAPJV/LAPMOD).
 Home-page: https://github.com/rathaROG/lapx
 Author: rathaROG
 License: BSD-2-Clause
 Keywords: Linear Assignment,LAPJV,LAPMOD,lap
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -25,14 +25,15 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Cython>=0.29.32
 Requires-Dist: numpy>=1.21.6
 
 [![Test Simple](https://github.com/rathaROG/lapx/actions/workflows/test_simple.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/test_simple.yaml)
 [![Benchmark](https://github.com/rathaROG/lapx/actions/workflows/benchmark.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/benchmark.yaml)
```

### Comparing `lapx-0.5.7/README.md` & `lapx-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `lapx-0.5.7/_lapjv_src/_lapjv.cpp` & `lapx-0.5.8/_lapjv_src/_lapjv.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -20,18 +20,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -115,14 +115,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -176,14 +178,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -237,60 +241,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -373,14 +400,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -1526,177 +1556,177 @@
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1725,42 +1755,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2107,22 +2137,16 @@
 static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info);
 static Py_ssize_t __Pyx_minusones[] = { -1, -1, -1, -1, -1, -1, -1, -1 };
 static Py_ssize_t __Pyx_zeros[] = { 0, 0, 0, 0, 0, 0, 0, 0 };
 
 /* BufferFallbackError.proto */
 static void __Pyx_RaiseBufferFallbackError(void);
 
-/* PyIntBinop.proto */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
-#else
-#define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
-    (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
-#endif
-
+#define __Pyx_BufPtrCContig2d(type, buf, i0, s0, i1, s1) ((type)((char*)buf + i0 * s0) + i1)
+#define __Pyx_BufPtrCContig1d(type, buf, i0, s0) ((type)buf + i0)
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
 #if !CYTHON_VECTORCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
 #endif
@@ -2159,16 +2183,14 @@
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
 /* PyObjectFastCall.proto */
 #define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
 
-#define __Pyx_BufPtrCContig2d(type, buf, i0, s0, i1, s1) ((type)((char*)buf + i0 * s0) + i1)
-#define __Pyx_BufPtrCContig1d(type, buf, i0, s0) ((type)buf + i0)
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
@@ -2194,30 +2216,30 @@
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key);
 #else
 #define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
@@ -2539,23 +2561,23 @@
 /* CIntFromPy.proto */
 static CYTHON_INLINE uint_t __Pyx_PyInt_As_uint_t(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE enum fp_t __Pyx_PyInt_As_enum__fp_t(PyObject *);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value);
-
-/* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint_t(uint_t value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value);
+
+/* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int_t(int_t value);
 
 /* FormatTypeName.proto */
 #if CYTHON_COMPILING_IN_LIMITED_API
@@ -2651,15 +2673,14 @@
 static const char __pyx_k__7[] = "*";
 static const char __pyx_k_cc[] = "cc";
 static const char __pyx_k_ii[] = "ii";
 static const char __pyx_k_kk[] = "kk";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k__12[] = "?";
 static const char __pyx_k_inf[] = "inf";
-static const char __pyx_k_max[] = "max";
 static const char __pyx_k_nan[] = "nan";
 static const char __pyx_k_opt[] = "opt";
 static const char __pyx_k_ret[] = "ret";
 static const char __pyx_k_sum[] = "sum";
 static const char __pyx_k_x_c[] = "x_c";
 static const char __pyx_k_y_c[] = "y_c";
 static const char __pyx_k_FP_1[] = "FP_1_";
@@ -2675,14 +2696,15 @@
 static const char __pyx_k_LARGE[] = "LARGE_";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_empty[] = "empty";
 static const char __pyx_k_int32[] = "int32";
 static const char __pyx_k_lapjv[] = "lapjv";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
+static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_arange[] = "arange";
 static const char __pyx_k_cost_c[] = "cost_c";
 static const char __pyx_k_double[] = "double";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_lapmod[] = "_lapmod";
 static const char __pyx_k_n_cols[] = "n_cols";
 static const char __pyx_k_n_rows[] = "n_rows";
@@ -2829,15 +2851,14 @@
   PyObject *__pyx_n_s_kk;
   PyObject *__pyx_n_s_kk_c;
   PyObject *__pyx_n_s_lapjv;
   PyObject *__pyx_n_s_lapjv_2;
   PyObject *__pyx_kp_s_lapjv_src__lapjv_pyx;
   PyObject *__pyx_n_s_lapmod;
   PyObject *__pyx_n_s_main;
-  PyObject *__pyx_n_s_max;
   PyObject *__pyx_n_s_n;
   PyObject *__pyx_n_s_n_cols;
   PyObject *__pyx_n_s_n_rows;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_nan;
   PyObject *__pyx_n_s_nonzero;
   PyObject *__pyx_n_s_np;
@@ -2850,16 +2871,16 @@
   PyObject *__pyx_n_s_return_cost;
   PyObject *__pyx_n_s_spec;
   PyObject *__pyx_n_s_sum;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_uint32;
   PyObject *__pyx_n_s_x_c;
   PyObject *__pyx_n_s_y_c;
+  PyObject *__pyx_n_s_zeros;
   PyObject *__pyx_int_0;
-  PyObject *__pyx_int_1;
   PyObject *__pyx_int_neg_1;
   PyObject *__pyx_tuple_;
   PyObject *__pyx_slice__5;
   PyObject *__pyx_tuple__2;
   PyObject *__pyx_tuple__3;
   PyObject *__pyx_tuple__4;
   PyObject *__pyx_tuple__6;
@@ -2968,15 +2989,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_kk);
   Py_CLEAR(clear_module_state->__pyx_n_s_kk_c);
   Py_CLEAR(clear_module_state->__pyx_n_s_lapjv);
   Py_CLEAR(clear_module_state->__pyx_n_s_lapjv_2);
   Py_CLEAR(clear_module_state->__pyx_kp_s_lapjv_src__lapjv_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_lapmod);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
-  Py_CLEAR(clear_module_state->__pyx_n_s_max);
   Py_CLEAR(clear_module_state->__pyx_n_s_n);
   Py_CLEAR(clear_module_state->__pyx_n_s_n_cols);
   Py_CLEAR(clear_module_state->__pyx_n_s_n_rows);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_nan);
   Py_CLEAR(clear_module_state->__pyx_n_s_nonzero);
   Py_CLEAR(clear_module_state->__pyx_n_s_np);
@@ -2989,16 +3009,16 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_return_cost);
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
   Py_CLEAR(clear_module_state->__pyx_n_s_sum);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_uint32);
   Py_CLEAR(clear_module_state->__pyx_n_s_x_c);
   Py_CLEAR(clear_module_state->__pyx_n_s_y_c);
+  Py_CLEAR(clear_module_state->__pyx_n_s_zeros);
   Py_CLEAR(clear_module_state->__pyx_int_0);
-  Py_CLEAR(clear_module_state->__pyx_int_1);
   Py_CLEAR(clear_module_state->__pyx_int_neg_1);
   Py_CLEAR(clear_module_state->__pyx_tuple_);
   Py_CLEAR(clear_module_state->__pyx_slice__5);
   Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_tuple__3);
   Py_CLEAR(clear_module_state->__pyx_tuple__4);
   Py_CLEAR(clear_module_state->__pyx_tuple__6);
@@ -3085,15 +3105,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_kk);
   Py_VISIT(traverse_module_state->__pyx_n_s_kk_c);
   Py_VISIT(traverse_module_state->__pyx_n_s_lapjv);
   Py_VISIT(traverse_module_state->__pyx_n_s_lapjv_2);
   Py_VISIT(traverse_module_state->__pyx_kp_s_lapjv_src__lapjv_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_lapmod);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
-  Py_VISIT(traverse_module_state->__pyx_n_s_max);
   Py_VISIT(traverse_module_state->__pyx_n_s_n);
   Py_VISIT(traverse_module_state->__pyx_n_s_n_cols);
   Py_VISIT(traverse_module_state->__pyx_n_s_n_rows);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_nan);
   Py_VISIT(traverse_module_state->__pyx_n_s_nonzero);
   Py_VISIT(traverse_module_state->__pyx_n_s_np);
@@ -3106,16 +3125,16 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_return_cost);
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
   Py_VISIT(traverse_module_state->__pyx_n_s_sum);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_uint32);
   Py_VISIT(traverse_module_state->__pyx_n_s_x_c);
   Py_VISIT(traverse_module_state->__pyx_n_s_y_c);
+  Py_VISIT(traverse_module_state->__pyx_n_s_zeros);
   Py_VISIT(traverse_module_state->__pyx_int_0);
-  Py_VISIT(traverse_module_state->__pyx_int_1);
   Py_VISIT(traverse_module_state->__pyx_int_neg_1);
   Py_VISIT(traverse_module_state->__pyx_tuple_);
   Py_VISIT(traverse_module_state->__pyx_slice__5);
   Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_tuple__3);
   Py_VISIT(traverse_module_state->__pyx_tuple__4);
   Py_VISIT(traverse_module_state->__pyx_tuple__6);
@@ -3234,15 +3253,14 @@
 #define __pyx_n_s_kk __pyx_mstate_global->__pyx_n_s_kk
 #define __pyx_n_s_kk_c __pyx_mstate_global->__pyx_n_s_kk_c
 #define __pyx_n_s_lapjv __pyx_mstate_global->__pyx_n_s_lapjv
 #define __pyx_n_s_lapjv_2 __pyx_mstate_global->__pyx_n_s_lapjv_2
 #define __pyx_kp_s_lapjv_src__lapjv_pyx __pyx_mstate_global->__pyx_kp_s_lapjv_src__lapjv_pyx
 #define __pyx_n_s_lapmod __pyx_mstate_global->__pyx_n_s_lapmod
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
-#define __pyx_n_s_max __pyx_mstate_global->__pyx_n_s_max
 #define __pyx_n_s_n __pyx_mstate_global->__pyx_n_s_n
 #define __pyx_n_s_n_cols __pyx_mstate_global->__pyx_n_s_n_cols
 #define __pyx_n_s_n_rows __pyx_mstate_global->__pyx_n_s_n_rows
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_nan __pyx_mstate_global->__pyx_n_s_nan
 #define __pyx_n_s_nonzero __pyx_mstate_global->__pyx_n_s_nonzero
 #define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
@@ -3255,276 +3273,276 @@
 #define __pyx_n_s_return_cost __pyx_mstate_global->__pyx_n_s_return_cost
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
 #define __pyx_n_s_sum __pyx_mstate_global->__pyx_n_s_sum
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_uint32 __pyx_mstate_global->__pyx_n_s_uint32
 #define __pyx_n_s_x_c __pyx_mstate_global->__pyx_n_s_x_c
 #define __pyx_n_s_y_c __pyx_mstate_global->__pyx_n_s_y_c
+#define __pyx_n_s_zeros __pyx_mstate_global->__pyx_n_s_zeros
 #define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
-#define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
 #define __pyx_int_neg_1 __pyx_mstate_global->__pyx_int_neg_1
 #define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
 #define __pyx_slice__5 __pyx_mstate_global->__pyx_slice__5
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
 #define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
 #define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
 #define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
 /* #### Code section: module_code ### */
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3533,29 +3551,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3566,15 +3584,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3583,29 +3601,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3616,15 +3634,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3633,29 +3651,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3666,15 +3684,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3683,29 +3701,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3716,15 +3734,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3733,29 +3751,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3766,217 +3784,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3992,15 +4010,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4008,68 +4026,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4077,15 +4095,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4100,15 +4118,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4124,15 +4142,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4140,68 +4158,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4209,15 +4227,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4232,15 +4250,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4256,15 +4274,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4272,68 +4290,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4341,15 +4359,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4364,184 +4382,184 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "_lapjv.pyx":41
- * 
+/* "_lapjv.pyx":42
+ * # https://github.com/rathaROG/lapx/pull/7
  * 
  * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
  * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
  */
 
 static PyObject *__pyx_pf_6_lapjv_4__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
@@ -4553,69 +4571,69 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 1);
   __Pyx_XDECREF(__pyx_r);
 
-  /* "_lapjv.pyx":43
+  /* "_lapjv.pyx":44
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def lapjv(cnp.ndarray cost not None, char extend_cost=False,             # <<<<<<<<<<<<<<
  *           double cost_limit=np.inf, char return_cost=True):
  *     """Solve linear assignment problem using Jonker-Volgenant algorithm.
  */
-  __pyx_t_1 = __Pyx_PyBool_FromLong(((int)0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(((int)0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "_lapjv.pyx":41
- * 
+  /* "_lapjv.pyx":42
+ * # https://github.com/rathaROG/lapx/pull/7
  * 
  * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
  * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
  */
-  __pyx_t_2 = PyFloat_FromDouble(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_cost_limit); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_cost_limit); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "_lapjv.pyx":44
+  /* "_lapjv.pyx":45
  * @cython.wraparound(False)
  * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
  *           double cost_limit=np.inf, char return_cost=True):             # <<<<<<<<<<<<<<
  *     """Solve linear assignment problem using Jonker-Volgenant algorithm.
  * 
  */
-  __pyx_t_3 = __Pyx_PyBool_FromLong(((int)1)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBool_FromLong(((int)1)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "_lapjv.pyx":41
- * 
+  /* "_lapjv.pyx":42
+ * # https://github.com/rathaROG/lapx/pull/7
  * 
  * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
  * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
  */
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3)) __PYX_ERR(0, 41, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 41, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 42, __pyx_L1_error);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, Py_None)) __PYX_ERR(0, 41, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, Py_None)) __PYX_ERR(0, 42, __pyx_L1_error);
   __pyx_t_4 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4691,41 +4709,41 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cost)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 41, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 42, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_extend_cost);
           if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 41, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 42, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cost_limit);
           if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 41, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 42, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_return_cost);
           if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 41, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 42, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lapjv") < 0)) __PYX_ERR(0, 41, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lapjv") < 0)) __PYX_ERR(0, 42, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -4734,46 +4752,46 @@
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_cost = ((PyArrayObject *)values[0]);
     if (values[1]) {
-      __pyx_v_extend_cost = __Pyx_PyInt_As_char(values[1]); if (unlikely((__pyx_v_extend_cost == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
+      __pyx_v_extend_cost = __Pyx_PyInt_As_char(values[1]); if (unlikely((__pyx_v_extend_cost == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 44, __pyx_L3_error)
     } else {
       __pyx_v_extend_cost = ((char)((int)0));
     }
     if (values[2]) {
-      __pyx_v_cost_limit = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_cost_limit == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 44, __pyx_L3_error)
+      __pyx_v_cost_limit = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_cost_limit == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
     } else {
       __pyx_v_cost_limit = __pyx_dynamic_args->__pyx_arg_cost_limit;
     }
     if (values[3]) {
-      __pyx_v_return_cost = __Pyx_PyInt_As_char(values[3]); if (unlikely((__pyx_v_return_cost == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 44, __pyx_L3_error)
+      __pyx_v_return_cost = __Pyx_PyInt_As_char(values[3]); if (unlikely((__pyx_v_return_cost == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
     } else {
       __pyx_v_return_cost = ((char)((int)1));
     }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("lapjv", 0, 1, 4, __pyx_nargs); __PYX_ERR(0, 41, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("lapjv", 0, 1, 4, __pyx_nargs); __PYX_ERR(0, 42, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("_lapjv.lapjv", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cost), __pyx_ptype_5numpy_ndarray, 0, "cost", 0))) __PYX_ERR(0, 43, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cost), __pyx_ptype_5numpy_ndarray, 0, "cost", 0))) __PYX_ERR(0, 44, __pyx_L1_error)
   __pyx_r = __pyx_pf_6_lapjv_lapjv(__pyx_self, __pyx_v_cost, __pyx_v_extend_cost, __pyx_v_cost_limit, __pyx_v_return_cost);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4814,26 +4832,27 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyArrayObject *__pyx_t_8 = NULL;
   npy_intp *__pyx_t_9;
-  int __pyx_t_10;
-  PyArrayObject *__pyx_t_11 = NULL;
+  PyArrayObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
-  PyObject *__pyx_t_14 = NULL;
+  uint_t __pyx_t_14;
   uint_t __pyx_t_15;
   uint_t __pyx_t_16;
   Py_ssize_t __pyx_t_17;
   Py_ssize_t __pyx_t_18;
   PyArrayObject *__pyx_t_19 = NULL;
   PyArrayObject *__pyx_t_20 = NULL;
   double __pyx_t_21;
+  int __pyx_t_22;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lapjv", 1);
   __pyx_pybuffer_cost_c.pybuffer.buf = NULL;
   __pyx_pybuffer_cost_c.refcount = 0;
   __pyx_pybuffernd_cost_c.data = NULL;
@@ -4847,1098 +4866,1197 @@
   __pyx_pybuffernd_x_c.data = NULL;
   __pyx_pybuffernd_x_c.rcbuffer = &__pyx_pybuffer_x_c;
   __pyx_pybuffer_y_c.pybuffer.buf = NULL;
   __pyx_pybuffer_y_c.refcount = 0;
   __pyx_pybuffernd_y_c.data = NULL;
   __pyx_pybuffernd_y_c.rcbuffer = &__pyx_pybuffer_y_c;
 
-  /* "_lapjv.pyx":74
+  /* "_lapjv.pyx":75
  *     All such entries are set to -1.
  *     """
  *     if cost.ndim != 2:             # <<<<<<<<<<<<<<
  *         raise ValueError('2-dimensional array expected')
  *     cdef cnp.ndarray[cnp.double_t, ndim=2, mode='c'] cost_c = \
  */
-  __pyx_t_1 = __pyx_f_5numpy_7ndarray_4ndim_ndim(__pyx_v_cost); if (unlikely(__pyx_t_1 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5numpy_7ndarray_4ndim_ndim(__pyx_v_cost); if (unlikely(__pyx_t_1 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(0, 75, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 2);
   if (unlikely(__pyx_t_2)) {
 
-    /* "_lapjv.pyx":75
+    /* "_lapjv.pyx":76
  *     """
  *     if cost.ndim != 2:
  *         raise ValueError('2-dimensional array expected')             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[cnp.double_t, ndim=2, mode='c'] cost_c = \
  *         np.ascontiguousarray(cost, dtype=np.double)
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 75, __pyx_L1_error)
+    __PYX_ERR(0, 76, __pyx_L1_error)
 
-    /* "_lapjv.pyx":74
+    /* "_lapjv.pyx":75
  *     All such entries are set to -1.
  *     """
  *     if cost.ndim != 2:             # <<<<<<<<<<<<<<
  *         raise ValueError('2-dimensional array expected')
  *     cdef cnp.ndarray[cnp.double_t, ndim=2, mode='c'] cost_c = \
  */
   }
 
-  /* "_lapjv.pyx":77
+  /* "_lapjv.pyx":78
  *         raise ValueError('2-dimensional array expected')
  *     cdef cnp.ndarray[cnp.double_t, ndim=2, mode='c'] cost_c = \
  *         np.ascontiguousarray(cost, dtype=np.double)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[cnp.double_t, ndim=2, mode='c'] cost_c_extended
  *     cdef uint_t n_rows = cost_c.shape[0]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF((PyObject *)__pyx_v_cost);
   __Pyx_GIVEREF((PyObject *)__pyx_v_cost);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_cost))) __PYX_ERR(0, 77, __pyx_L1_error);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 77, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_cost))) __PYX_ERR(0, 78, __pyx_L1_error);
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_double); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_double); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 77, __pyx_L1_error)
+  if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 78, __pyx_L1_error)
   __pyx_t_8 = ((PyArrayObject *)__pyx_t_7);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_cost_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 76, __pyx_L1_error)
+      __PYX_ERR(0, 77, __pyx_L1_error)
     } else {__pyx_pybuffernd_cost_c.diminfo[0].strides = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_cost_c.diminfo[0].shape = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_cost_c.diminfo[1].strides = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_cost_c.diminfo[1].shape = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_8 = 0;
   __pyx_v_cost_c = ((PyArrayObject *)__pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "_lapjv.pyx":79
+  /* "_lapjv.pyx":80
  *         np.ascontiguousarray(cost, dtype=np.double)
  *     cdef cnp.ndarray[cnp.double_t, ndim=2, mode='c'] cost_c_extended
  *     cdef uint_t n_rows = cost_c.shape[0]             # <<<<<<<<<<<<<<
  *     cdef uint_t n_cols = cost_c.shape[1]
  *     cdef uint_t n = 0
  */
-  __pyx_t_9 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_cost_c)); if (unlikely(__pyx_t_9 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_9 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_cost_c)); if (unlikely(__pyx_t_9 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 80, __pyx_L1_error)
   __pyx_v_n_rows = (__pyx_t_9[0]);
 
-  /* "_lapjv.pyx":80
+  /* "_lapjv.pyx":81
  *     cdef cnp.ndarray[cnp.double_t, ndim=2, mode='c'] cost_c_extended
  *     cdef uint_t n_rows = cost_c.shape[0]
  *     cdef uint_t n_cols = cost_c.shape[1]             # <<<<<<<<<<<<<<
  *     cdef uint_t n = 0
  *     if n_rows == n_cols:
  */
-  __pyx_t_9 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_cost_c)); if (unlikely(__pyx_t_9 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_9 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_cost_c)); if (unlikely(__pyx_t_9 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L1_error)
   __pyx_v_n_cols = (__pyx_t_9[1]);
 
-  /* "_lapjv.pyx":81
+  /* "_lapjv.pyx":82
  *     cdef uint_t n_rows = cost_c.shape[0]
  *     cdef uint_t n_cols = cost_c.shape[1]
  *     cdef uint_t n = 0             # <<<<<<<<<<<<<<
  *     if n_rows == n_cols:
  *         n = n_rows
  */
   __pyx_v_n = 0;
 
-  /* "_lapjv.pyx":82
+  /* "_lapjv.pyx":83
  *     cdef uint_t n_cols = cost_c.shape[1]
  *     cdef uint_t n = 0
  *     if n_rows == n_cols:             # <<<<<<<<<<<<<<
  *         n = n_rows
  *     else:
  */
   __pyx_t_2 = (__pyx_v_n_rows == __pyx_v_n_cols);
   if (__pyx_t_2) {
 
-    /* "_lapjv.pyx":83
+    /* "_lapjv.pyx":84
  *     cdef uint_t n = 0
  *     if n_rows == n_cols:
  *         n = n_rows             # <<<<<<<<<<<<<<
  *     else:
  *         if not extend_cost:
  */
     __pyx_v_n = __pyx_v_n_rows;
 
-    /* "_lapjv.pyx":82
+    /* "_lapjv.pyx":83
  *     cdef uint_t n_cols = cost_c.shape[1]
  *     cdef uint_t n = 0
  *     if n_rows == n_cols:             # <<<<<<<<<<<<<<
  *         n = n_rows
  *     else:
  */
     goto __pyx_L4;
   }
 
-  /* "_lapjv.pyx":85
+  /* "_lapjv.pyx":86
  *         n = n_rows
  *     else:
  *         if not extend_cost:             # <<<<<<<<<<<<<<
  *             raise ValueError(
  *                     'Square cost array expected. If cost is intentionally '
  */
   /*else*/ {
     __pyx_t_2 = (!(__pyx_v_extend_cost != 0));
     if (unlikely(__pyx_t_2)) {
 
-      /* "_lapjv.pyx":86
+      /* "_lapjv.pyx":87
  *     else:
  *         if not extend_cost:
  *             raise ValueError(             # <<<<<<<<<<<<<<
  *                     'Square cost array expected. If cost is intentionally '
  *                     'non-square, pass extend_cost=True.')
  */
-      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 86, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 87, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_Raise(__pyx_t_7, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __PYX_ERR(0, 86, __pyx_L1_error)
+      __PYX_ERR(0, 87, __pyx_L1_error)
 
-      /* "_lapjv.pyx":85
+      /* "_lapjv.pyx":86
  *         n = n_rows
  *     else:
  *         if not extend_cost:             # <<<<<<<<<<<<<<
  *             raise ValueError(
  *                     'Square cost array expected. If cost is intentionally '
  */
     }
   }
   __pyx_L4:;
 
-  /* "_lapjv.pyx":89
+  /* "_lapjv.pyx":90
  *                     'Square cost array expected. If cost is intentionally '
  *                     'non-square, pass extend_cost=True.')
- *     if extend_cost or cost_limit < np.inf:             # <<<<<<<<<<<<<<
+ *     if cost_limit < np.inf:             # <<<<<<<<<<<<<<
  *         n = n_rows + n_cols
  *         cost_c_extended = np.empty((n, n), dtype=np.double)
  */
-  __pyx_t_10 = (__pyx_v_extend_cost != 0);
-  if (!__pyx_t_10) {
-  } else {
-    __pyx_t_2 = __pyx_t_10;
-    goto __pyx_L7_bool_binop_done;
-  }
-  __pyx_t_7 = PyFloat_FromDouble(__pyx_v_cost_limit); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_7 = PyFloat_FromDouble(__pyx_v_cost_limit); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_inf); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_inf); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyObject_RichCompare(__pyx_t_7, __pyx_t_3, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_5 = PyObject_RichCompare(__pyx_t_7, __pyx_t_3, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely((__pyx_t_10 < 0))) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_2 = __pyx_t_10;
-  __pyx_L7_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "_lapjv.pyx":90
+    /* "_lapjv.pyx":91
  *                     'non-square, pass extend_cost=True.')
- *     if extend_cost or cost_limit < np.inf:
+ *     if cost_limit < np.inf:
  *         n = n_rows + n_cols             # <<<<<<<<<<<<<<
  *         cost_c_extended = np.empty((n, n), dtype=np.double)
- *         if cost_limit < np.inf:
+ *         cost_c_extended[:] = cost_limit / 2.
  */
     __pyx_v_n = (__pyx_v_n_rows + __pyx_v_n_cols);
 
-    /* "_lapjv.pyx":91
- *     if extend_cost or cost_limit < np.inf:
+    /* "_lapjv.pyx":92
+ *     if cost_limit < np.inf:
  *         n = n_rows + n_cols
  *         cost_c_extended = np.empty((n, n), dtype=np.double)             # <<<<<<<<<<<<<<
- *         if cost_limit < np.inf:
- *             cost_c_extended[:] = cost_limit / 2.
+ *         cost_c_extended[:] = cost_limit / 2.
+ *         cost_c_extended[n_rows:, n_cols:] = 0
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_7);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7)) __PYX_ERR(0, 91, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7)) __PYX_ERR(0, 92, __pyx_L1_error);
     __pyx_t_5 = 0;
     __pyx_t_7 = 0;
-    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_4);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_double); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_double); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 91, __pyx_L1_error)
-    __pyx_t_11 = ((PyArrayObject *)__pyx_t_6);
+    if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 92, __pyx_L1_error)
+    __pyx_t_10 = ((PyArrayObject *)__pyx_t_6);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer);
-      __pyx_t_1 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer, (PyObject*)__pyx_t_11, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
+      __pyx_t_1 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer, (PyObject*)__pyx_t_10, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
       if (unlikely(__pyx_t_1 < 0)) {
-        PyErr_Fetch(&__pyx_t_12, &__pyx_t_13, &__pyx_t_14);
+        PyErr_Fetch(&__pyx_t_11, &__pyx_t_12, &__pyx_t_13);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer, (PyObject*)__pyx_v_cost_c_extended, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_14);
+          Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_13);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_12, __pyx_t_13, __pyx_t_14);
+          PyErr_Restore(__pyx_t_11, __pyx_t_12, __pyx_t_13);
         }
-        __pyx_t_12 = __pyx_t_13 = __pyx_t_14 = 0;
+        __pyx_t_11 = __pyx_t_12 = __pyx_t_13 = 0;
       }
       __pyx_pybuffernd_cost_c_extended.diminfo[0].strides = __pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_cost_c_extended.diminfo[0].shape = __pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_cost_c_extended.diminfo[1].strides = __pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_cost_c_extended.diminfo[1].shape = __pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer.shape[1];
-      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 91, __pyx_L1_error)
+      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 92, __pyx_L1_error)
     }
-    __pyx_t_11 = 0;
+    __pyx_t_10 = 0;
     __pyx_v_cost_c_extended = ((PyArrayObject *)__pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "_lapjv.pyx":92
+    /* "_lapjv.pyx":93
  *         n = n_rows + n_cols
  *         cost_c_extended = np.empty((n, n), dtype=np.double)
- *         if cost_limit < np.inf:             # <<<<<<<<<<<<<<
- *             cost_c_extended[:] = cost_limit / 2.
- *         else:
+ *         cost_c_extended[:] = cost_limit / 2.             # <<<<<<<<<<<<<<
+ *         cost_c_extended[n_rows:, n_cols:] = 0
+ *         cost_c_extended[:n_rows, :n_cols] = cost_c
  */
-    __pyx_t_6 = PyFloat_FromDouble(__pyx_v_cost_limit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
+    __pyx_t_6 = PyFloat_FromDouble((__pyx_v_cost_limit / 2.)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_inf); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyObject_RichCompare(__pyx_t_6, __pyx_t_7, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
+    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_slice__5, __pyx_t_6) < 0))) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (__pyx_t_2) {
 
-      /* "_lapjv.pyx":93
+    /* "_lapjv.pyx":94
  *         cost_c_extended = np.empty((n, n), dtype=np.double)
- *         if cost_limit < np.inf:
- *             cost_c_extended[:] = cost_limit / 2.             # <<<<<<<<<<<<<<
- *         else:
- *             cost_c_extended[:] = cost_c.max() + 1
+ *         cost_c_extended[:] = cost_limit / 2.
+ *         cost_c_extended[n_rows:, n_cols:] = 0             # <<<<<<<<<<<<<<
+ *         cost_c_extended[:n_rows, :n_cols] = cost_c
+ *         cost_c = cost_c_extended
  */
-      __pyx_t_4 = PyFloat_FromDouble((__pyx_v_cost_limit / 2.)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_slice__5, __pyx_t_4) < 0))) __PYX_ERR(0, 93, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_4 = PySlice_New(__pyx_t_6, Py_None, Py_None); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = PySlice_New(__pyx_t_6, Py_None, Py_None); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_4);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_7);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_7)) __PYX_ERR(0, 94, __pyx_L1_error);
+    __pyx_t_4 = 0;
+    __pyx_t_7 = 0;
+    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_t_6, __pyx_int_0) < 0))) __PYX_ERR(0, 94, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "_lapjv.pyx":92
- *         n = n_rows + n_cols
- *         cost_c_extended = np.empty((n, n), dtype=np.double)
- *         if cost_limit < np.inf:             # <<<<<<<<<<<<<<
- *             cost_c_extended[:] = cost_limit / 2.
- *         else:
+    /* "_lapjv.pyx":95
+ *         cost_c_extended[:] = cost_limit / 2.
+ *         cost_c_extended[n_rows:, n_cols:] = 0
+ *         cost_c_extended[:n_rows, :n_cols] = cost_c             # <<<<<<<<<<<<<<
+ *         cost_c = cost_c_extended
+ *     elif extend_cost:
  */
-      goto __pyx_L9;
-    }
+    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = PySlice_New(Py_None, __pyx_t_6, Py_None); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_4 = PySlice_New(Py_None, __pyx_t_6, Py_None); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_7);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7)) __PYX_ERR(0, 95, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_4);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error);
+    __pyx_t_7 = 0;
+    __pyx_t_4 = 0;
+    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_t_6, ((PyObject *)__pyx_v_cost_c)) < 0))) __PYX_ERR(0, 95, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "_lapjv.pyx":95
- *             cost_c_extended[:] = cost_limit / 2.
- *         else:
- *             cost_c_extended[:] = cost_c.max() + 1             # <<<<<<<<<<<<<<
+    /* "_lapjv.pyx":96
  *         cost_c_extended[n_rows:, n_cols:] = 0
  *         cost_c_extended[:n_rows, :n_cols] = cost_c
+ *         cost_c = cost_c_extended             # <<<<<<<<<<<<<<
+ *     elif extend_cost:
+ *         n = max(n_rows, n_cols)
  */
-    /*else*/ {
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_cost_c), __pyx_n_s_max); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 95, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_6 = NULL;
-      __pyx_t_1 = 0;
-      #if CYTHON_UNPACK_METHODS
-      if (likely(PyMethod_Check(__pyx_t_7))) {
-        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
-        if (likely(__pyx_t_6)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-          __Pyx_INCREF(__pyx_t_6);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_7, function);
-          __pyx_t_1 = 1;
+    {
+      __Pyx_BufFmt_StackElem __pyx_stack[1];
+      __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_cost_c.rcbuffer->pybuffer);
+      __pyx_t_1 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_v_cost_c_extended), &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
+      if (unlikely(__pyx_t_1 < 0)) {
+        PyErr_Fetch(&__pyx_t_13, &__pyx_t_12, &__pyx_t_11);
+        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c.rcbuffer->pybuffer, (PyObject*)__pyx_v_cost_c, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack) == -1)) {
+          Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_11);
+          __Pyx_RaiseBufferFallbackError();
+        } else {
+          PyErr_Restore(__pyx_t_13, __pyx_t_12, __pyx_t_11);
         }
+        __pyx_t_13 = __pyx_t_12 = __pyx_t_11 = 0;
       }
-      #endif
-      {
-        PyObject *__pyx_callargs[2] = {__pyx_t_6, NULL};
-        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_1, 0+__pyx_t_1);
-        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      }
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 95, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_slice__5, __pyx_t_7) < 0))) __PYX_ERR(0, 95, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __pyx_pybuffernd_cost_c.diminfo[0].strides = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_cost_c.diminfo[0].shape = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_cost_c.diminfo[1].strides = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_cost_c.diminfo[1].shape = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.shape[1];
+      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 96, __pyx_L1_error)
     }
-    __pyx_L9:;
+    __Pyx_INCREF((PyObject *)__pyx_v_cost_c_extended);
+    __Pyx_DECREF_SET(__pyx_v_cost_c, ((PyArrayObject *)__pyx_v_cost_c_extended));
 
-    /* "_lapjv.pyx":96
- *         else:
- *             cost_c_extended[:] = cost_c.max() + 1
- *         cost_c_extended[n_rows:, n_cols:] = 0             # <<<<<<<<<<<<<<
+    /* "_lapjv.pyx":90
+ *                     'Square cost array expected. If cost is intentionally '
+ *                     'non-square, pass extend_cost=True.')
+ *     if cost_limit < np.inf:             # <<<<<<<<<<<<<<
+ *         n = n_rows + n_cols
+ *         cost_c_extended = np.empty((n, n), dtype=np.double)
+ */
+    goto __pyx_L6;
+  }
+
+  /* "_lapjv.pyx":97
  *         cost_c_extended[:n_rows, :n_cols] = cost_c
  *         cost_c = cost_c_extended
+ *     elif extend_cost:             # <<<<<<<<<<<<<<
+ *         n = max(n_rows, n_cols)
+ *         cost_c_extended = np.zeros((n, n), dtype=np.double)
  */
-    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 96, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = PySlice_New(__pyx_t_7, Py_None, Py_None); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_2 = (__pyx_v_extend_cost != 0);
+  if (__pyx_t_2) {
+
+    /* "_lapjv.pyx":98
+ *         cost_c = cost_c_extended
+ *     elif extend_cost:
+ *         n = max(n_rows, n_cols)             # <<<<<<<<<<<<<<
+ *         cost_c_extended = np.zeros((n, n), dtype=np.double)
+ *         cost_c_extended[:n_rows, :n_cols] = cost_c
+ */
+    __pyx_t_14 = __pyx_v_n_cols;
+    __pyx_t_15 = __pyx_v_n_rows;
+    __pyx_t_2 = (__pyx_t_14 > __pyx_t_15);
+    if (__pyx_t_2) {
+      __pyx_t_16 = __pyx_t_14;
+    } else {
+      __pyx_t_16 = __pyx_t_15;
+    }
+    __pyx_v_n = __pyx_t_16;
+
+    /* "_lapjv.pyx":99
+ *     elif extend_cost:
+ *         n = max(n_rows, n_cols)
+ *         cost_c_extended = np.zeros((n, n), dtype=np.double)             # <<<<<<<<<<<<<<
+ *         cost_c_extended[:n_rows, :n_cols] = cost_c
+ *         cost_c = cost_c_extended
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 96, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_6 = PySlice_New(__pyx_t_7, Py_None, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 99, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 99, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_GIVEREF(__pyx_t_4);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4)) __PYX_ERR(0, 96, __pyx_L1_error);
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_6);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_6)) __PYX_ERR(0, 96, __pyx_L1_error);
-    __pyx_t_4 = 0;
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6)) __PYX_ERR(0, 99, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_7);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_7)) __PYX_ERR(0, 99, __pyx_L1_error);
     __pyx_t_6 = 0;
-    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_t_7, __pyx_int_0) < 0))) __PYX_ERR(0, 96, __pyx_L1_error)
+    __pyx_t_7 = 0;
+    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_GIVEREF(__pyx_t_3);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error);
+    __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 99, __pyx_L1_error)
+    __pyx_t_10 = ((PyArrayObject *)__pyx_t_5);
+    {
+      __Pyx_BufFmt_StackElem __pyx_stack[1];
+      __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer);
+      __pyx_t_1 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer, (PyObject*)__pyx_t_10, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
+      if (unlikely(__pyx_t_1 < 0)) {
+        PyErr_Fetch(&__pyx_t_11, &__pyx_t_12, &__pyx_t_13);
+        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer, (PyObject*)__pyx_v_cost_c_extended, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack) == -1)) {
+          Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_13);
+          __Pyx_RaiseBufferFallbackError();
+        } else {
+          PyErr_Restore(__pyx_t_11, __pyx_t_12, __pyx_t_13);
+        }
+        __pyx_t_11 = __pyx_t_12 = __pyx_t_13 = 0;
+      }
+      __pyx_pybuffernd_cost_c_extended.diminfo[0].strides = __pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_cost_c_extended.diminfo[0].shape = __pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_cost_c_extended.diminfo[1].strides = __pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_cost_c_extended.diminfo[1].shape = __pyx_pybuffernd_cost_c_extended.rcbuffer->pybuffer.shape[1];
+      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 99, __pyx_L1_error)
+    }
+    __pyx_t_10 = 0;
+    __pyx_v_cost_c_extended = ((PyArrayObject *)__pyx_t_5);
+    __pyx_t_5 = 0;
 
-    /* "_lapjv.pyx":97
- *             cost_c_extended[:] = cost_c.max() + 1
- *         cost_c_extended[n_rows:, n_cols:] = 0
+    /* "_lapjv.pyx":100
+ *         n = max(n_rows, n_cols)
+ *         cost_c_extended = np.zeros((n, n), dtype=np.double)
  *         cost_c_extended[:n_rows, :n_cols] = cost_c             # <<<<<<<<<<<<<<
  *         cost_c = cost_c_extended
  * 
  */
-    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 97, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_6 = PySlice_New(Py_None, __pyx_t_7, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 97, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 97, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = PySlice_New(Py_None, __pyx_t_7, Py_None); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_3 = PySlice_New(Py_None, __pyx_t_5, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_7 = PySlice_New(Py_None, __pyx_t_5, Py_None); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_GIVEREF(__pyx_t_6);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_6)) __PYX_ERR(0, 97, __pyx_L1_error);
-    __Pyx_GIVEREF(__pyx_t_4);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error);
-    __pyx_t_6 = 0;
-    __pyx_t_4 = 0;
-    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_t_7, ((PyObject *)__pyx_v_cost_c)) < 0))) __PYX_ERR(0, 97, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_3);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_7);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_7)) __PYX_ERR(0, 100, __pyx_L1_error);
+    __pyx_t_3 = 0;
+    __pyx_t_7 = 0;
+    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_cost_c_extended), __pyx_t_5, ((PyObject *)__pyx_v_cost_c)) < 0))) __PYX_ERR(0, 100, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "_lapjv.pyx":98
- *         cost_c_extended[n_rows:, n_cols:] = 0
+    /* "_lapjv.pyx":101
+ *         cost_c_extended = np.zeros((n, n), dtype=np.double)
  *         cost_c_extended[:n_rows, :n_cols] = cost_c
  *         cost_c = cost_c_extended             # <<<<<<<<<<<<<<
  * 
  *     cdef double **cost_ptr
  */
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_cost_c.rcbuffer->pybuffer);
       __pyx_t_1 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_v_cost_c_extended), &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
       if (unlikely(__pyx_t_1 < 0)) {
-        PyErr_Fetch(&__pyx_t_14, &__pyx_t_13, &__pyx_t_12);
+        PyErr_Fetch(&__pyx_t_13, &__pyx_t_12, &__pyx_t_11);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cost_c.rcbuffer->pybuffer, (PyObject*)__pyx_v_cost_c, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_14); Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_12);
+          Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_11);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_14, __pyx_t_13, __pyx_t_12);
+          PyErr_Restore(__pyx_t_13, __pyx_t_12, __pyx_t_11);
         }
-        __pyx_t_14 = __pyx_t_13 = __pyx_t_12 = 0;
+        __pyx_t_13 = __pyx_t_12 = __pyx_t_11 = 0;
       }
       __pyx_pybuffernd_cost_c.diminfo[0].strides = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_cost_c.diminfo[0].shape = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_cost_c.diminfo[1].strides = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_cost_c.diminfo[1].shape = __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.shape[1];
-      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 98, __pyx_L1_error)
+      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 101, __pyx_L1_error)
     }
     __Pyx_INCREF((PyObject *)__pyx_v_cost_c_extended);
     __Pyx_DECREF_SET(__pyx_v_cost_c, ((PyArrayObject *)__pyx_v_cost_c_extended));
 
-    /* "_lapjv.pyx":89
- *                     'Square cost array expected. If cost is intentionally '
- *                     'non-square, pass extend_cost=True.')
- *     if extend_cost or cost_limit < np.inf:             # <<<<<<<<<<<<<<
- *         n = n_rows + n_cols
- *         cost_c_extended = np.empty((n, n), dtype=np.double)
+    /* "_lapjv.pyx":97
+ *         cost_c_extended[:n_rows, :n_cols] = cost_c
+ *         cost_c = cost_c_extended
+ *     elif extend_cost:             # <<<<<<<<<<<<<<
+ *         n = max(n_rows, n_cols)
+ *         cost_c_extended = np.zeros((n, n), dtype=np.double)
  */
   }
+  __pyx_L6:;
 
-  /* "_lapjv.pyx":101
+  /* "_lapjv.pyx":104
  * 
  *     cdef double **cost_ptr
  *     cost_ptr = <double **> malloc(n * sizeof(double *))             # <<<<<<<<<<<<<<
  *     cdef int i
  *     for i in range(n):
  */
   __pyx_v_cost_ptr = ((double **)malloc((__pyx_v_n * (sizeof(double *)))));
 
-  /* "_lapjv.pyx":103
+  /* "_lapjv.pyx":106
  *     cost_ptr = <double **> malloc(n * sizeof(double *))
  *     cdef int i
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         cost_ptr[i] = &cost_c[i, 0]
  * 
  */
-  __pyx_t_15 = __pyx_v_n;
-  __pyx_t_16 = __pyx_t_15;
-  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_16; __pyx_t_1+=1) {
+  __pyx_t_16 = __pyx_v_n;
+  __pyx_t_14 = __pyx_t_16;
+  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_14; __pyx_t_1+=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "_lapjv.pyx":104
+    /* "_lapjv.pyx":107
  *     cdef int i
  *     for i in range(n):
  *         cost_ptr[i] = &cost_c[i, 0]             # <<<<<<<<<<<<<<
  * 
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] x_c = \
  */
     __pyx_t_17 = __pyx_v_i;
     __pyx_t_18 = 0;
     (__pyx_v_cost_ptr[__pyx_v_i]) = (&(*__Pyx_BufPtrCContig2d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_cost_c.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_cost_c.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_cost_c.diminfo[1].strides)));
   }
 
-  /* "_lapjv.pyx":107
+  /* "_lapjv.pyx":110
  * 
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] x_c = \
  *         np.empty((n,), dtype=np.int32)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] y_c = \
  *         np.empty((n,), dtype=np.int32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GIVEREF(__pyx_t_7);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7)) __PYX_ERR(0, 107, __pyx_L1_error);
-  __pyx_t_7 = 0;
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GIVEREF(__pyx_t_6);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_6)) __PYX_ERR(0, 107, __pyx_L1_error);
-  __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5)) __PYX_ERR(0, 110, __pyx_L1_error);
+  __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 107, __pyx_L1_error)
-  __pyx_t_19 = ((PyArrayObject *)__pyx_t_5);
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_19 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_19, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_x_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_x_c.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 106, __pyx_L1_error)
+      __PYX_ERR(0, 109, __pyx_L1_error)
     } else {__pyx_pybuffernd_x_c.diminfo[0].strides = __pyx_pybuffernd_x_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_x_c.diminfo[0].shape = __pyx_pybuffernd_x_c.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_19 = 0;
-  __pyx_v_x_c = ((PyArrayObject *)__pyx_t_5);
-  __pyx_t_5 = 0;
+  __pyx_v_x_c = ((PyArrayObject *)__pyx_t_6);
+  __pyx_t_6 = 0;
 
-  /* "_lapjv.pyx":109
+  /* "_lapjv.pyx":112
  *         np.empty((n,), dtype=np.int32)
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] y_c = \
  *         np.empty((n,), dtype=np.int32)             # <<<<<<<<<<<<<<
  * 
  *     cdef int ret = lapjv_internal(n, cost_ptr, &x_c[0], &y_c[0])
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GIVEREF(__pyx_t_6);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6)) __PYX_ERR(0, 112, __pyx_L1_error);
+  __pyx_t_6 = 0;
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5)) __PYX_ERR(0, 109, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5)) __PYX_ERR(0, 112, __pyx_L1_error);
   __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GIVEREF(__pyx_t_7);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error);
-  __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 109, __pyx_L1_error)
-  __pyx_t_20 = ((PyArrayObject *)__pyx_t_3);
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_20 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_20, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_y_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_y_c.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 108, __pyx_L1_error)
+      __PYX_ERR(0, 111, __pyx_L1_error)
     } else {__pyx_pybuffernd_y_c.diminfo[0].strides = __pyx_pybuffernd_y_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_y_c.diminfo[0].shape = __pyx_pybuffernd_y_c.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_20 = 0;
-  __pyx_v_y_c = ((PyArrayObject *)__pyx_t_3);
-  __pyx_t_3 = 0;
+  __pyx_v_y_c = ((PyArrayObject *)__pyx_t_4);
+  __pyx_t_4 = 0;
 
-  /* "_lapjv.pyx":111
+  /* "_lapjv.pyx":114
  *         np.empty((n,), dtype=np.int32)
  * 
  *     cdef int ret = lapjv_internal(n, cost_ptr, &x_c[0], &y_c[0])             # <<<<<<<<<<<<<<
  *     free(cost_ptr)
  *     if ret != 0:
  */
   __pyx_t_18 = 0;
   __pyx_t_17 = 0;
   __pyx_v_ret = lapjv_internal(__pyx_v_n, __pyx_v_cost_ptr, (&(*__Pyx_BufPtrCContig1d(int_t *, __pyx_pybuffernd_x_c.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_x_c.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(int_t *, __pyx_pybuffernd_y_c.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_y_c.diminfo[0].strides))));
 
-  /* "_lapjv.pyx":112
+  /* "_lapjv.pyx":115
  * 
  *     cdef int ret = lapjv_internal(n, cost_ptr, &x_c[0], &y_c[0])
  *     free(cost_ptr)             # <<<<<<<<<<<<<<
  *     if ret != 0:
  *         if ret == -1:
  */
   free(__pyx_v_cost_ptr);
 
-  /* "_lapjv.pyx":113
+  /* "_lapjv.pyx":116
  *     cdef int ret = lapjv_internal(n, cost_ptr, &x_c[0], &y_c[0])
  *     free(cost_ptr)
  *     if ret != 0:             # <<<<<<<<<<<<<<
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')
  */
   __pyx_t_2 = (__pyx_v_ret != 0);
   if (__pyx_t_2) {
 
-    /* "_lapjv.pyx":114
+    /* "_lapjv.pyx":117
  *     free(cost_ptr)
  *     if ret != 0:
  *         if ret == -1:             # <<<<<<<<<<<<<<
  *             raise MemoryError('Out of memory.')
  *         raise RuntimeError('Unknown error (lapjv_internal returned %d).' % ret)
  */
     __pyx_t_2 = (__pyx_v_ret == -1L);
     if (unlikely(__pyx_t_2)) {
 
-      /* "_lapjv.pyx":115
+      /* "_lapjv.pyx":118
  *     if ret != 0:
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')             # <<<<<<<<<<<<<<
  *         raise RuntimeError('Unknown error (lapjv_internal returned %d).' % ret)
  * 
  */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 115, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(0, 115, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_Raise(__pyx_t_4, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __PYX_ERR(0, 118, __pyx_L1_error)
 
-      /* "_lapjv.pyx":114
+      /* "_lapjv.pyx":117
  *     free(cost_ptr)
  *     if ret != 0:
  *         if ret == -1:             # <<<<<<<<<<<<<<
  *             raise MemoryError('Out of memory.')
  *         raise RuntimeError('Unknown error (lapjv_internal returned %d).' % ret)
  */
     }
 
-    /* "_lapjv.pyx":116
+    /* "_lapjv.pyx":119
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')
  *         raise RuntimeError('Unknown error (lapjv_internal returned %d).' % ret)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_ret); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = PyUnicode_Format(__pyx_kp_u_Unknown_error_lapjv_internal_ret, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 116, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 116, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_ret); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = PyUnicode_Format(__pyx_kp_u_Unknown_error_lapjv_internal_ret, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 119, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __PYX_ERR(0, 119, __pyx_L1_error)
 
-    /* "_lapjv.pyx":113
+    /* "_lapjv.pyx":116
  *     cdef int ret = lapjv_internal(n, cost_ptr, &x_c[0], &y_c[0])
  *     free(cost_ptr)
  *     if ret != 0:             # <<<<<<<<<<<<<<
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')
  */
   }
 
-  /* "_lapjv.pyx":119
+  /* "_lapjv.pyx":122
  * 
  * 
  *     cdef double opt = np.nan             # <<<<<<<<<<<<<<
- *     if n != n_rows:
+ *     if cost_limit < np.inf or extend_cost:
  *         x_c[x_c >= n_cols] = -1
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_nan); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_7); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_nan); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 122, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_opt = __pyx_t_21;
 
-  /* "_lapjv.pyx":120
+  /* "_lapjv.pyx":123
  * 
  *     cdef double opt = np.nan
- *     if n != n_rows:             # <<<<<<<<<<<<<<
+ *     if cost_limit < np.inf or extend_cost:             # <<<<<<<<<<<<<<
  *         x_c[x_c >= n_cols] = -1
  *         y_c[y_c >= n_rows] = -1
  */
-  __pyx_t_2 = (__pyx_v_n != __pyx_v_n_rows);
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_cost_limit); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_inf); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_5, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_22 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_22 < 0))) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (!__pyx_t_22) {
+  } else {
+    __pyx_t_2 = __pyx_t_22;
+    goto __pyx_L12_bool_binop_done;
+  }
+  __pyx_t_22 = (__pyx_v_extend_cost != 0);
+  __pyx_t_2 = __pyx_t_22;
+  __pyx_L12_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "_lapjv.pyx":121
+    /* "_lapjv.pyx":124
  *     cdef double opt = np.nan
- *     if n != n_rows:
+ *     if cost_limit < np.inf or extend_cost:
  *         x_c[x_c >= n_cols] = -1             # <<<<<<<<<<<<<<
  *         y_c[y_c >= n_rows] = -1
  *         x_c = x_c[:n_rows]
  */
-    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 121, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_3 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_t_7, Py_GE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_x_c), __pyx_t_3, __pyx_int_neg_1) < 0))) __PYX_ERR(0, 121, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_6 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_t_4, Py_GE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_x_c), __pyx_t_6, __pyx_int_neg_1) < 0))) __PYX_ERR(0, 124, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "_lapjv.pyx":122
- *     if n != n_rows:
+    /* "_lapjv.pyx":125
+ *     if cost_limit < np.inf or extend_cost:
  *         x_c[x_c >= n_cols] = -1
  *         y_c[y_c >= n_rows] = -1             # <<<<<<<<<<<<<<
  *         x_c = x_c[:n_rows]
  *         y_c = y_c[:n_cols]
  */
-    __pyx_t_3 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 122, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = PyObject_RichCompare(((PyObject *)__pyx_v_y_c), __pyx_t_3, Py_GE); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 122, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_y_c), __pyx_t_7, __pyx_int_neg_1) < 0))) __PYX_ERR(0, 122, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_4 = PyObject_RichCompare(((PyObject *)__pyx_v_y_c), __pyx_t_6, Py_GE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_y_c), __pyx_t_4, __pyx_int_neg_1) < 0))) __PYX_ERR(0, 125, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "_lapjv.pyx":123
+    /* "_lapjv.pyx":126
  *         x_c[x_c >= n_cols] = -1
  *         y_c[y_c >= n_rows] = -1
  *         x_c = x_c[:n_rows]             # <<<<<<<<<<<<<<
  *         y_c = y_c[:n_cols]
  *         if return_cost:
  */
-    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 123, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_3 = PySlice_New(Py_None, __pyx_t_7, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_x_c), __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 123, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 123, __pyx_L1_error)
-    __pyx_t_19 = ((PyArrayObject *)__pyx_t_7);
+    __pyx_t_4 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_6 = PySlice_New(Py_None, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_x_c), __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 126, __pyx_L1_error)
+    __pyx_t_19 = ((PyArrayObject *)__pyx_t_4);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_x_c.rcbuffer->pybuffer);
       __pyx_t_1 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_19, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_1 < 0)) {
-        PyErr_Fetch(&__pyx_t_12, &__pyx_t_13, &__pyx_t_14);
+        PyErr_Fetch(&__pyx_t_11, &__pyx_t_12, &__pyx_t_13);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_c.rcbuffer->pybuffer, (PyObject*)__pyx_v_x_c, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_14);
+          Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_13);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_12, __pyx_t_13, __pyx_t_14);
+          PyErr_Restore(__pyx_t_11, __pyx_t_12, __pyx_t_13);
         }
-        __pyx_t_12 = __pyx_t_13 = __pyx_t_14 = 0;
+        __pyx_t_11 = __pyx_t_12 = __pyx_t_13 = 0;
       }
       __pyx_pybuffernd_x_c.diminfo[0].strides = __pyx_pybuffernd_x_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_x_c.diminfo[0].shape = __pyx_pybuffernd_x_c.rcbuffer->pybuffer.shape[0];
-      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 123, __pyx_L1_error)
+      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 126, __pyx_L1_error)
     }
     __pyx_t_19 = 0;
-    __Pyx_DECREF_SET(__pyx_v_x_c, ((PyArrayObject *)__pyx_t_7));
-    __pyx_t_7 = 0;
+    __Pyx_DECREF_SET(__pyx_v_x_c, ((PyArrayObject *)__pyx_t_4));
+    __pyx_t_4 = 0;
 
-    /* "_lapjv.pyx":124
+    /* "_lapjv.pyx":127
  *         y_c[y_c >= n_rows] = -1
  *         x_c = x_c[:n_rows]
  *         y_c = y_c[:n_cols]             # <<<<<<<<<<<<<<
  *         if return_cost:
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  */
-    __pyx_t_7 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 124, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_3 = PySlice_New(Py_None, __pyx_t_7, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 124, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_y_c), __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 124, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 124, __pyx_L1_error)
-    __pyx_t_20 = ((PyArrayObject *)__pyx_t_7);
+    __pyx_t_4 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_6 = PySlice_New(Py_None, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_y_c), __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 127, __pyx_L1_error)
+    __pyx_t_20 = ((PyArrayObject *)__pyx_t_4);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_y_c.rcbuffer->pybuffer);
       __pyx_t_1 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_20, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_1 < 0)) {
-        PyErr_Fetch(&__pyx_t_14, &__pyx_t_13, &__pyx_t_12);
+        PyErr_Fetch(&__pyx_t_13, &__pyx_t_12, &__pyx_t_11);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_c.rcbuffer->pybuffer, (PyObject*)__pyx_v_y_c, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_14); Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_12);
+          Py_XDECREF(__pyx_t_13); Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_11);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_14, __pyx_t_13, __pyx_t_12);
+          PyErr_Restore(__pyx_t_13, __pyx_t_12, __pyx_t_11);
         }
-        __pyx_t_14 = __pyx_t_13 = __pyx_t_12 = 0;
+        __pyx_t_13 = __pyx_t_12 = __pyx_t_11 = 0;
       }
       __pyx_pybuffernd_y_c.diminfo[0].strides = __pyx_pybuffernd_y_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_y_c.diminfo[0].shape = __pyx_pybuffernd_y_c.rcbuffer->pybuffer.shape[0];
-      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 124, __pyx_L1_error)
+      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 127, __pyx_L1_error)
     }
     __pyx_t_20 = 0;
-    __Pyx_DECREF_SET(__pyx_v_y_c, ((PyArrayObject *)__pyx_t_7));
-    __pyx_t_7 = 0;
+    __Pyx_DECREF_SET(__pyx_v_y_c, ((PyArrayObject *)__pyx_t_4));
+    __pyx_t_4 = 0;
 
-    /* "_lapjv.pyx":125
+    /* "_lapjv.pyx":128
  *         x_c = x_c[:n_rows]
  *         y_c = y_c[:n_cols]
  *         if return_cost:             # <<<<<<<<<<<<<<
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  *     elif return_cost:
  */
     __pyx_t_2 = (__pyx_v_return_cost != 0);
     if (__pyx_t_2) {
 
-      /* "_lapjv.pyx":126
+      /* "_lapjv.pyx":129
  *         y_c = y_c[:n_cols]
  *         if return_cost:
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()             # <<<<<<<<<<<<<<
  *     elif return_cost:
  *         opt = cost_c[np.arange(n_rows), x_c].sum()
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 126, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 129, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_nonzero); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 126, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_nonzero); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_int_neg_1, Py_NE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 126, __pyx_L1_error)
-      __pyx_t_4 = NULL;
+      __pyx_t_5 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_int_neg_1, Py_NE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __pyx_t_7 = NULL;
       __pyx_t_1 = 0;
       #if CYTHON_UNPACK_METHODS
-      if (unlikely(PyMethod_Check(__pyx_t_6))) {
-        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
-        if (likely(__pyx_t_4)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-          __Pyx_INCREF(__pyx_t_4);
+      if (unlikely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(__pyx_t_7)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_6, function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
           __pyx_t_1 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_5};
-        __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
-        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
+        __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+        __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 129, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
-      __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_3, 0, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 126, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_int_neg_1, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
-      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_x_c), __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 126, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_6, 0, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_GIVEREF(__pyx_t_6);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6)) __PYX_ERR(0, 126, __pyx_L1_error);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_6 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_int_neg_1, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_x_c), __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_GIVEREF(__pyx_t_3);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error);
       __Pyx_GIVEREF(__pyx_t_5);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_5)) __PYX_ERR(0, 126, __pyx_L1_error);
-      __pyx_t_6 = 0;
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_5)) __PYX_ERR(0, 129, __pyx_L1_error);
+      __pyx_t_3 = 0;
       __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_cost_c), __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 126, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_cost_c), __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 129, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_sum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_sum); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_5 = NULL;
       __pyx_t_1 = 0;
       #if CYTHON_UNPACK_METHODS
-      if (likely(PyMethod_Check(__pyx_t_3))) {
-        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(PyMethod_Check(__pyx_t_6))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_5)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __Pyx_DECREF_SET(__pyx_t_6, function);
           __pyx_t_1 = 1;
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
-        __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_1, 0+__pyx_t_1);
+        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_1, 0+__pyx_t_1);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 126, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
-      __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_7); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 126, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 129, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_v_opt = __pyx_t_21;
 
-      /* "_lapjv.pyx":125
+      /* "_lapjv.pyx":128
  *         x_c = x_c[:n_rows]
  *         y_c = y_c[:n_cols]
  *         if return_cost:             # <<<<<<<<<<<<<<
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  *     elif return_cost:
  */
     }
 
-    /* "_lapjv.pyx":120
+    /* "_lapjv.pyx":123
  * 
  *     cdef double opt = np.nan
- *     if n != n_rows:             # <<<<<<<<<<<<<<
+ *     if cost_limit < np.inf or extend_cost:             # <<<<<<<<<<<<<<
  *         x_c[x_c >= n_cols] = -1
  *         y_c[y_c >= n_rows] = -1
  */
-    goto __pyx_L14;
+    goto __pyx_L11;
   }
 
-  /* "_lapjv.pyx":127
+  /* "_lapjv.pyx":130
  *         if return_cost:
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  *     elif return_cost:             # <<<<<<<<<<<<<<
  *         opt = cost_c[np.arange(n_rows), x_c].sum()
  * 
  */
   __pyx_t_2 = (__pyx_v_return_cost != 0);
   if (__pyx_t_2) {
 
-    /* "_lapjv.pyx":128
+    /* "_lapjv.pyx":131
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  *     elif return_cost:
  *         opt = cost_c[np.arange(n_rows), x_c].sum()             # <<<<<<<<<<<<<<
  * 
  *     if return_cost:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_arange); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 128, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = NULL;
+    __pyx_t_7 = NULL;
     __pyx_t_1 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (unlikely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_4);
+    if (unlikely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_7)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_1 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_5};
-      __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
+      __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 128, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_3);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error);
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_6);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6)) __PYX_ERR(0, 131, __pyx_L1_error);
     __Pyx_INCREF((PyObject *)__pyx_v_x_c);
     __Pyx_GIVEREF((PyObject *)__pyx_v_x_c);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 128, __pyx_L1_error);
-    __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_cost_c), __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sum); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 128, __pyx_L1_error)
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 131, __pyx_L1_error);
+    __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_cost_c), __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = NULL;
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_sum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = NULL;
     __pyx_t_1 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_3);
+    if (likely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_1 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
-      __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_1, 0+__pyx_t_1);
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 128, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      PyObject *__pyx_callargs[2] = {__pyx_t_6, NULL};
+      __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_1, 0+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_7); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 128, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_opt = __pyx_t_21;
 
-    /* "_lapjv.pyx":127
+    /* "_lapjv.pyx":130
  *         if return_cost:
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  *     elif return_cost:             # <<<<<<<<<<<<<<
  *         opt = cost_c[np.arange(n_rows), x_c].sum()
  * 
  */
   }
-  __pyx_L14:;
+  __pyx_L11:;
 
-  /* "_lapjv.pyx":130
+  /* "_lapjv.pyx":133
  *         opt = cost_c[np.arange(n_rows), x_c].sum()
  * 
  *     if return_cost:             # <<<<<<<<<<<<<<
  *         return opt, x_c, y_c
  *     else:
  */
   __pyx_t_2 = (__pyx_v_return_cost != 0);
   if (__pyx_t_2) {
 
-    /* "_lapjv.pyx":131
+    /* "_lapjv.pyx":134
  * 
  *     if return_cost:
  *         return opt, x_c, y_c             # <<<<<<<<<<<<<<
  *     else:
  *         return x_c, y_c
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_7 = PyFloat_FromDouble(__pyx_v_opt); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 131, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 131, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_7);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7)) __PYX_ERR(0, 131, __pyx_L1_error);
+    __pyx_t_4 = PyFloat_FromDouble(__pyx_v_opt); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 134, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 134, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_4);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 134, __pyx_L1_error);
     __Pyx_INCREF((PyObject *)__pyx_v_x_c);
     __Pyx_GIVEREF((PyObject *)__pyx_v_x_c);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 131, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 134, __pyx_L1_error);
     __Pyx_INCREF((PyObject *)__pyx_v_y_c);
     __Pyx_GIVEREF((PyObject *)__pyx_v_y_c);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 2, ((PyObject *)__pyx_v_y_c))) __PYX_ERR(0, 131, __pyx_L1_error);
-    __pyx_t_7 = 0;
-    __pyx_r = __pyx_t_6;
-    __pyx_t_6 = 0;
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 2, ((PyObject *)__pyx_v_y_c))) __PYX_ERR(0, 134, __pyx_L1_error);
+    __pyx_t_4 = 0;
+    __pyx_r = __pyx_t_3;
+    __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "_lapjv.pyx":130
+    /* "_lapjv.pyx":133
  *         opt = cost_c[np.arange(n_rows), x_c].sum()
  * 
  *     if return_cost:             # <<<<<<<<<<<<<<
  *         return opt, x_c, y_c
  *     else:
  */
   }
 
-  /* "_lapjv.pyx":133
+  /* "_lapjv.pyx":136
  *         return opt, x_c, y_c
  *     else:
  *         return x_c, y_c             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 133, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF((PyObject *)__pyx_v_x_c);
     __Pyx_GIVEREF((PyObject *)__pyx_v_x_c);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 133, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 136, __pyx_L1_error);
     __Pyx_INCREF((PyObject *)__pyx_v_y_c);
     __Pyx_GIVEREF((PyObject *)__pyx_v_y_c);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)__pyx_v_y_c))) __PYX_ERR(0, 133, __pyx_L1_error);
-    __pyx_r = __pyx_t_6;
-    __pyx_t_6 = 0;
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, ((PyObject *)__pyx_v_y_c))) __PYX_ERR(0, 136, __pyx_L1_error);
+    __pyx_r = __pyx_t_3;
+    __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "_lapjv.pyx":41
- * 
+  /* "_lapjv.pyx":42
+ * # https://github.com/rathaROG/lapx/pull/7
  * 
  * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
  * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
  */
 
   /* function exit code */
@@ -5971,46 +6089,46 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_x_c);
   __Pyx_XDECREF((PyObject *)__pyx_v_y_c);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_lapjv.pyx":136
+/* "_lapjv.pyx":139
  * 
  * 
  * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
- * def _lapmod(
+ * def _lapmod(const uint_t n,
  */
 
 static PyObject *__pyx_pf_6_lapjv_6__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum__fp_t(__Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_fp_version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__fp_t(__Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_fp_version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error);
   __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, Py_None)) __PYX_ERR(0, 136, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, Py_None)) __PYX_ERR(0, 139, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6087,99 +6205,99 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cc)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 1); __PYX_ERR(0, 136, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 1); __PYX_ERR(0, 139, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ii)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 2); __PYX_ERR(0, 136, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 2); __PYX_ERR(0, 139, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kk)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 3); __PYX_ERR(0, 136, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 3); __PYX_ERR(0, 139, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fp_version);
           if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_lapmod") < 0)) __PYX_ERR(0, 136, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_lapmod") < 0)) __PYX_ERR(0, 139, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_n = __Pyx_PyInt_As_uint_t(values[0]); if (unlikely((__pyx_v_n == ((uint_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
+    __pyx_v_n = __Pyx_PyInt_As_uint_t(values[0]); if (unlikely((__pyx_v_n == ((uint_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 141, __pyx_L3_error)
     __pyx_v_cc = ((PyArrayObject *)values[1]);
     __pyx_v_ii = ((PyArrayObject *)values[2]);
     __pyx_v_kk = ((PyArrayObject *)values[3]);
     if (values[4]) {
-      __pyx_v_fp_version = ((enum fp_t)__Pyx_PyInt_As_enum__fp_t(values[4])); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 143, __pyx_L3_error)
+      __pyx_v_fp_version = ((enum fp_t)__Pyx_PyInt_As_enum__fp_t(values[4])); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 145, __pyx_L3_error)
     } else {
       __pyx_v_fp_version = __pyx_dynamic_args->__pyx_arg_fp_version;
     }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, __pyx_nargs); __PYX_ERR(0, 136, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, __pyx_nargs); __PYX_ERR(0, 139, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("_lapjv._lapmod", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cc), __pyx_ptype_5numpy_ndarray, 0, "cc", 0))) __PYX_ERR(0, 140, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ii), __pyx_ptype_5numpy_ndarray, 0, "ii", 0))) __PYX_ERR(0, 141, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kk), __pyx_ptype_5numpy_ndarray, 0, "kk", 0))) __PYX_ERR(0, 142, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cc), __pyx_ptype_5numpy_ndarray, 0, "cc", 0))) __PYX_ERR(0, 142, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ii), __pyx_ptype_5numpy_ndarray, 0, "ii", 0))) __PYX_ERR(0, 143, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kk), __pyx_ptype_5numpy_ndarray, 0, "kk", 0))) __PYX_ERR(0, 144, __pyx_L1_error)
   __pyx_r = __pyx_pf_6_lapjv_2_lapmod(__pyx_self, __pyx_v_n, __pyx_v_cc, __pyx_v_ii, __pyx_v_kk, __pyx_v_fp_version);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -6249,377 +6367,377 @@
   __pyx_pybuffernd_x_c.data = NULL;
   __pyx_pybuffernd_x_c.rcbuffer = &__pyx_pybuffer_x_c;
   __pyx_pybuffer_y_c.pybuffer.buf = NULL;
   __pyx_pybuffer_y_c.refcount = 0;
   __pyx_pybuffernd_y_c.data = NULL;
   __pyx_pybuffernd_y_c.rcbuffer = &__pyx_pybuffer_y_c;
 
-  /* "_lapjv.pyx":146
+  /* "_lapjv.pyx":148
  *     """Internal function called from lapmod(..., fast=True)."""
  *     cdef cnp.ndarray[cnp.double_t, ndim=1, mode='c'] cc_c = \
  *         np.ascontiguousarray(cc, dtype=np.double)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[uint_t, ndim=1, mode='c'] ii_c = \
  *         np.ascontiguousarray(ii, dtype=np.uint32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF((PyObject *)__pyx_v_cc);
   __Pyx_GIVEREF((PyObject *)__pyx_v_cc);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_cc))) __PYX_ERR(0, 146, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_cc))) __PYX_ERR(0, 148, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 146, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 148, __pyx_L1_error)
   __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cc_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_cc_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_cc_c.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 145, __pyx_L1_error)
+      __PYX_ERR(0, 147, __pyx_L1_error)
     } else {__pyx_pybuffernd_cc_c.diminfo[0].strides = __pyx_pybuffernd_cc_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_cc_c.diminfo[0].shape = __pyx_pybuffernd_cc_c.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_6 = 0;
   __pyx_v_cc_c = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "_lapjv.pyx":148
+  /* "_lapjv.pyx":150
  *         np.ascontiguousarray(cc, dtype=np.double)
  *     cdef cnp.ndarray[uint_t, ndim=1, mode='c'] ii_c = \
  *         np.ascontiguousarray(ii, dtype=np.uint32)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[uint_t, ndim=1, mode='c'] kk_c = \
  *         np.ascontiguousarray(kk, dtype=np.uint32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF((PyObject *)__pyx_v_ii);
   __Pyx_GIVEREF((PyObject *)__pyx_v_ii);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)__pyx_v_ii))) __PYX_ERR(0, 148, __pyx_L1_error);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)__pyx_v_ii))) __PYX_ERR(0, 150, __pyx_L1_error);
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 148, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 150, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ii_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn_uint_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_ii_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_ii_c.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 147, __pyx_L1_error)
+      __PYX_ERR(0, 149, __pyx_L1_error)
     } else {__pyx_pybuffernd_ii_c.diminfo[0].strides = __pyx_pybuffernd_ii_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_ii_c.diminfo[0].shape = __pyx_pybuffernd_ii_c.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_ii_c = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "_lapjv.pyx":150
+  /* "_lapjv.pyx":152
  *         np.ascontiguousarray(ii, dtype=np.uint32)
  *     cdef cnp.ndarray[uint_t, ndim=1, mode='c'] kk_c = \
  *         np.ascontiguousarray(kk, dtype=np.uint32)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] x_c = \
  *         np.empty((n,), dtype=np.int32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF((PyObject *)__pyx_v_kk);
   __Pyx_GIVEREF((PyObject *)__pyx_v_kk);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)__pyx_v_kk))) __PYX_ERR(0, 150, __pyx_L1_error);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)__pyx_v_kk))) __PYX_ERR(0, 152, __pyx_L1_error);
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 150, __pyx_L1_error)
+  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 152, __pyx_L1_error)
   __pyx_t_8 = ((PyArrayObject *)__pyx_t_2);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_kk_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn_uint_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_kk_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_kk_c.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 149, __pyx_L1_error)
+      __PYX_ERR(0, 151, __pyx_L1_error)
     } else {__pyx_pybuffernd_kk_c.diminfo[0].strides = __pyx_pybuffernd_kk_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_kk_c.diminfo[0].shape = __pyx_pybuffernd_kk_c.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_8 = 0;
   __pyx_v_kk_c = ((PyArrayObject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "_lapjv.pyx":152
+  /* "_lapjv.pyx":154
  *         np.ascontiguousarray(kk, dtype=np.uint32)
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] x_c = \
  *         np.empty((n,), dtype=np.int32)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] y_c = \
  *         np.empty((n,), dtype=np.int32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error);
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4)) __PYX_ERR(0, 152, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 152, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 154, __pyx_L1_error)
   __pyx_t_9 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_x_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_x_c.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 151, __pyx_L1_error)
+      __PYX_ERR(0, 153, __pyx_L1_error)
     } else {__pyx_pybuffernd_x_c.diminfo[0].strides = __pyx_pybuffernd_x_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_x_c.diminfo[0].shape = __pyx_pybuffernd_x_c.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_9 = 0;
   __pyx_v_x_c = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "_lapjv.pyx":154
+  /* "_lapjv.pyx":156
  *         np.empty((n,), dtype=np.int32)
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] y_c = \
  *         np.empty((n,), dtype=np.int32)             # <<<<<<<<<<<<<<
  * 
- *     cdef int_t ret = lapmod_internal(
+ *     cdef int_t ret = lapmod_internal(n, &cc_c[0], &ii_c[0], &kk_c[0],
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error);
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 154, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 156, __pyx_L1_error)
   __pyx_t_10 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_10, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_y_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_y_c.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 153, __pyx_L1_error)
+      __PYX_ERR(0, 155, __pyx_L1_error)
     } else {__pyx_pybuffernd_y_c.diminfo[0].strides = __pyx_pybuffernd_y_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_y_c.diminfo[0].shape = __pyx_pybuffernd_y_c.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_10 = 0;
   __pyx_v_y_c = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "_lapjv.pyx":157
+  /* "_lapjv.pyx":158
+ *         np.empty((n,), dtype=np.int32)
  * 
- *     cdef int_t ret = lapmod_internal(
- *                 n, &cc_c[0], &ii_c[0], &kk_c[0],             # <<<<<<<<<<<<<<
- *                 &x_c[0], &y_c[0], fp_version)
+ *     cdef int_t ret = lapmod_internal(n, &cc_c[0], &ii_c[0], &kk_c[0],             # <<<<<<<<<<<<<<
+ *                                      &x_c[0], &y_c[0], fp_version)
  *     if ret != 0:
  */
   __pyx_t_11 = 0;
   __pyx_t_12 = 0;
   __pyx_t_13 = 0;
 
-  /* "_lapjv.pyx":158
- *     cdef int_t ret = lapmod_internal(
- *                 n, &cc_c[0], &ii_c[0], &kk_c[0],
- *                 &x_c[0], &y_c[0], fp_version)             # <<<<<<<<<<<<<<
+  /* "_lapjv.pyx":159
+ * 
+ *     cdef int_t ret = lapmod_internal(n, &cc_c[0], &ii_c[0], &kk_c[0],
+ *                                      &x_c[0], &y_c[0], fp_version)             # <<<<<<<<<<<<<<
  *     if ret != 0:
  *         if ret == -1:
  */
   __pyx_t_14 = 0;
   __pyx_t_15 = 0;
 
-  /* "_lapjv.pyx":156
+  /* "_lapjv.pyx":158
  *         np.empty((n,), dtype=np.int32)
  * 
- *     cdef int_t ret = lapmod_internal(             # <<<<<<<<<<<<<<
- *                 n, &cc_c[0], &ii_c[0], &kk_c[0],
- *                 &x_c[0], &y_c[0], fp_version)
+ *     cdef int_t ret = lapmod_internal(n, &cc_c[0], &ii_c[0], &kk_c[0],             # <<<<<<<<<<<<<<
+ *                                      &x_c[0], &y_c[0], fp_version)
+ *     if ret != 0:
  */
   __pyx_v_ret = lapmod_internal(__pyx_v_n, (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_cc_c.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_cc_c.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(uint_t *, __pyx_pybuffernd_ii_c.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_ii_c.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(uint_t *, __pyx_pybuffernd_kk_c.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_kk_c.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(int_t *, __pyx_pybuffernd_x_c.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_x_c.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(int_t *, __pyx_pybuffernd_y_c.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_y_c.diminfo[0].strides))), __pyx_v_fp_version);
 
-  /* "_lapjv.pyx":159
- *                 n, &cc_c[0], &ii_c[0], &kk_c[0],
- *                 &x_c[0], &y_c[0], fp_version)
+  /* "_lapjv.pyx":160
+ *     cdef int_t ret = lapmod_internal(n, &cc_c[0], &ii_c[0], &kk_c[0],
+ *                                      &x_c[0], &y_c[0], fp_version)
  *     if ret != 0:             # <<<<<<<<<<<<<<
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')
  */
   __pyx_t_16 = (__pyx_v_ret != 0);
   if (__pyx_t_16) {
 
-    /* "_lapjv.pyx":160
- *                 &x_c[0], &y_c[0], fp_version)
+    /* "_lapjv.pyx":161
+ *                                      &x_c[0], &y_c[0], fp_version)
  *     if ret != 0:
  *         if ret == -1:             # <<<<<<<<<<<<<<
  *             raise MemoryError('Out of memory.')
  *         raise RuntimeError('Unknown error (lapmod_internal returned %d).' % ret)
  */
     __pyx_t_16 = (__pyx_v_ret == -1L);
     if (unlikely(__pyx_t_16)) {
 
-      /* "_lapjv.pyx":161
+      /* "_lapjv.pyx":162
  *     if ret != 0:
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')             # <<<<<<<<<<<<<<
  *         raise RuntimeError('Unknown error (lapmod_internal returned %d).' % ret)
  * 
  */
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(0, 161, __pyx_L1_error)
+      __PYX_ERR(0, 162, __pyx_L1_error)
 
-      /* "_lapjv.pyx":160
- *                 &x_c[0], &y_c[0], fp_version)
+      /* "_lapjv.pyx":161
+ *                                      &x_c[0], &y_c[0], fp_version)
  *     if ret != 0:
  *         if ret == -1:             # <<<<<<<<<<<<<<
  *             raise MemoryError('Out of memory.')
  *         raise RuntimeError('Unknown error (lapmod_internal returned %d).' % ret)
  */
     }
 
-    /* "_lapjv.pyx":162
+    /* "_lapjv.pyx":163
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')
  *         raise RuntimeError('Unknown error (lapmod_internal returned %d).' % ret)             # <<<<<<<<<<<<<<
  * 
  *     return x_c, y_c
  */
-    __pyx_t_1 = __Pyx_PyInt_From_int_t(__pyx_v_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int_t(__pyx_v_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyUnicode_Format(__pyx_kp_u_Unknown_error_lapmod_internal_re, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_2 = PyUnicode_Format(__pyx_kp_u_Unknown_error_lapmod_internal_re, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 162, __pyx_L1_error)
+    __PYX_ERR(0, 163, __pyx_L1_error)
 
-    /* "_lapjv.pyx":159
- *                 n, &cc_c[0], &ii_c[0], &kk_c[0],
- *                 &x_c[0], &y_c[0], fp_version)
+    /* "_lapjv.pyx":160
+ *     cdef int_t ret = lapmod_internal(n, &cc_c[0], &ii_c[0], &kk_c[0],
+ *                                      &x_c[0], &y_c[0], fp_version)
  *     if ret != 0:             # <<<<<<<<<<<<<<
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')
  */
   }
 
-  /* "_lapjv.pyx":164
+  /* "_lapjv.pyx":165
  *         raise RuntimeError('Unknown error (lapmod_internal returned %d).' % ret)
  * 
  *     return x_c, y_c             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF((PyObject *)__pyx_v_x_c);
   __Pyx_GIVEREF((PyObject *)__pyx_v_x_c);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 164, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 165, __pyx_L1_error);
   __Pyx_INCREF((PyObject *)__pyx_v_y_c);
   __Pyx_GIVEREF((PyObject *)__pyx_v_y_c);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)__pyx_v_y_c))) __PYX_ERR(0, 164, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)__pyx_v_y_c))) __PYX_ERR(0, 165, __pyx_L1_error);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_lapjv.pyx":136
+  /* "_lapjv.pyx":139
  * 
  * 
  * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
- * def _lapmod(
+ * def _lapmod(const uint_t n,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -6714,15 +6832,14 @@
     {&__pyx_n_s_kk, __pyx_k_kk, sizeof(__pyx_k_kk), 0, 0, 1, 1},
     {&__pyx_n_s_kk_c, __pyx_k_kk_c, sizeof(__pyx_k_kk_c), 0, 0, 1, 1},
     {&__pyx_n_s_lapjv, __pyx_k_lapjv, sizeof(__pyx_k_lapjv), 0, 0, 1, 1},
     {&__pyx_n_s_lapjv_2, __pyx_k_lapjv_2, sizeof(__pyx_k_lapjv_2), 0, 0, 1, 1},
     {&__pyx_kp_s_lapjv_src__lapjv_pyx, __pyx_k_lapjv_src__lapjv_pyx, sizeof(__pyx_k_lapjv_src__lapjv_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_lapmod, __pyx_k_lapmod, sizeof(__pyx_k_lapmod), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-    {&__pyx_n_s_max, __pyx_k_max, sizeof(__pyx_k_max), 0, 0, 1, 1},
     {&__pyx_n_s_n, __pyx_k_n, sizeof(__pyx_k_n), 0, 0, 1, 1},
     {&__pyx_n_s_n_cols, __pyx_k_n_cols, sizeof(__pyx_k_n_cols), 0, 0, 1, 1},
     {&__pyx_n_s_n_rows, __pyx_k_n_rows, sizeof(__pyx_k_n_rows), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_nan, __pyx_k_nan, sizeof(__pyx_k_nan), 0, 0, 1, 1},
     {&__pyx_n_s_nonzero, __pyx_k_nonzero, sizeof(__pyx_k_nonzero), 0, 0, 1, 1},
     {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
@@ -6735,136 +6852,136 @@
     {&__pyx_n_s_return_cost, __pyx_k_return_cost, sizeof(__pyx_k_return_cost), 0, 0, 1, 1},
     {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
     {&__pyx_n_s_sum, __pyx_k_sum, sizeof(__pyx_k_sum), 0, 0, 1, 1},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_uint32, __pyx_k_uint32, sizeof(__pyx_k_uint32), 0, 0, 1, 1},
     {&__pyx_n_s_x_c, __pyx_k_x_c, sizeof(__pyx_k_x_c), 0, 0, 1, 1},
     {&__pyx_n_s_y_c, __pyx_k_y_c, sizeof(__pyx_k_y_c), 0, 0, 1, 1},
+    {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 75, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 103, __pyx_L1_error)
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 115, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 119, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 984, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-39kcshgg/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "_lapjv.pyx":75
+  /* "_lapjv.pyx":76
  *     """
  *     if cost.ndim != 2:
  *         raise ValueError('2-dimensional array expected')             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[cnp.double_t, ndim=2, mode='c'] cost_c = \
  *         np.ascontiguousarray(cost, dtype=np.double)
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_2_dimensional_array_expected); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_2_dimensional_array_expected); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "_lapjv.pyx":86
+  /* "_lapjv.pyx":87
  *     else:
  *         if not extend_cost:
  *             raise ValueError(             # <<<<<<<<<<<<<<
  *                     'Square cost array expected. If cost is intentionally '
  *                     'non-square, pass extend_cost=True.')
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Square_cost_array_expected_If_co); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Square_cost_array_expected_If_co); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "_lapjv.pyx":93
+ *         n = n_rows + n_cols
  *         cost_c_extended = np.empty((n, n), dtype=np.double)
- *         if cost_limit < np.inf:
- *             cost_c_extended[:] = cost_limit / 2.             # <<<<<<<<<<<<<<
- *         else:
- *             cost_c_extended[:] = cost_c.max() + 1
+ *         cost_c_extended[:] = cost_limit / 2.             # <<<<<<<<<<<<<<
+ *         cost_c_extended[n_rows:, n_cols:] = 0
+ *         cost_c_extended[:n_rows, :n_cols] = cost_c
  */
   __pyx_slice__5 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__5)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__5);
   __Pyx_GIVEREF(__pyx_slice__5);
 
-  /* "_lapjv.pyx":115
+  /* "_lapjv.pyx":118
  *     if ret != 0:
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')             # <<<<<<<<<<<<<<
  *         raise RuntimeError('Unknown error (lapjv_internal returned %d).' % ret)
  * 
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_Out_of_memory); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_Out_of_memory); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "_lapjv.pyx":41
- * 
+  /* "_lapjv.pyx":42
+ * # https://github.com/rathaROG/lapx/pull/7
  * 
  * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
  * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
  */
-  __pyx_tuple__8 = PyTuple_Pack(15, __pyx_n_s_cost, __pyx_n_s_extend_cost, __pyx_n_s_cost_limit, __pyx_n_s_return_cost, __pyx_n_s_cost_c, __pyx_n_s_cost_c_extended, __pyx_n_s_n_rows, __pyx_n_s_n_cols, __pyx_n_s_n, __pyx_n_s_cost_ptr, __pyx_n_s_i, __pyx_n_s_x_c, __pyx_n_s_y_c, __pyx_n_s_ret, __pyx_n_s_opt); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(15, __pyx_n_s_cost, __pyx_n_s_extend_cost, __pyx_n_s_cost_limit, __pyx_n_s_return_cost, __pyx_n_s_cost_c, __pyx_n_s_cost_c_extended, __pyx_n_s_n_rows, __pyx_n_s_n_cols, __pyx_n_s_n, __pyx_n_s_cost_ptr, __pyx_n_s_i, __pyx_n_s_x_c, __pyx_n_s_y_c, __pyx_n_s_ret, __pyx_n_s_opt); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lapjv_src__lapjv_pyx, __pyx_n_s_lapjv, 41, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lapjv_src__lapjv_pyx, __pyx_n_s_lapjv, 42, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 42, __pyx_L1_error)
 
-  /* "_lapjv.pyx":136
+  /* "_lapjv.pyx":139
  * 
  * 
  * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
- * def _lapmod(
+ * def _lapmod(const uint_t n,
  */
-  __pyx_tuple__10 = PyTuple_Pack(11, __pyx_n_s_n, __pyx_n_s_cc, __pyx_n_s_ii, __pyx_n_s_kk, __pyx_n_s_fp_version, __pyx_n_s_cc_c, __pyx_n_s_ii_c, __pyx_n_s_kk_c, __pyx_n_s_x_c, __pyx_n_s_y_c, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(11, __pyx_n_s_n, __pyx_n_s_cc, __pyx_n_s_ii, __pyx_n_s_kk, __pyx_n_s_fp_version, __pyx_n_s_cc_c, __pyx_n_s_ii_c, __pyx_n_s_kk_c, __pyx_n_s_x_c, __pyx_n_s_y_c, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lapjv_src__lapjv_pyx, __pyx_n_s_lapmod, 136, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lapjv_src__lapjv_pyx, __pyx_n_s_lapmod, 139, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
   if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: init_globals ### */
 
@@ -6940,41 +7057,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -7285,113 +7402,113 @@
  * cimport cython
  */
   __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_numpy, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_lapjv.pyx":35
- *             fp_t fp_version)
+  /* "_lapjv.pyx":33
+ *                         fp_t fp_version)
  * 
  * LARGE_ = LARGE             # <<<<<<<<<<<<<<
  * FP_1_ = FP_1
  * FP_2_ = FP_2
  */
-  __pyx_t_2 = __Pyx_PyInt_From_int(LARGE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(LARGE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LARGE, __pyx_t_2) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LARGE, __pyx_t_2) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_lapjv.pyx":36
+  /* "_lapjv.pyx":34
  * 
  * LARGE_ = LARGE
  * FP_1_ = FP_1             # <<<<<<<<<<<<<<
  * FP_2_ = FP_2
  * FP_DYNAMIC_ = FP_DYNAMIC
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum__fp_t(FP_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__fp_t(FP_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FP_1, __pyx_t_2) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FP_1, __pyx_t_2) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_lapjv.pyx":37
+  /* "_lapjv.pyx":35
  * LARGE_ = LARGE
  * FP_1_ = FP_1
  * FP_2_ = FP_2             # <<<<<<<<<<<<<<
  * FP_DYNAMIC_ = FP_DYNAMIC
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum__fp_t(FP_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__fp_t(FP_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FP_2, __pyx_t_2) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FP_2, __pyx_t_2) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_lapjv.pyx":38
+  /* "_lapjv.pyx":36
  * FP_1_ = FP_1
  * FP_2_ = FP_2
  * FP_DYNAMIC_ = FP_DYNAMIC             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum__fp_t(FP_DYNAMIC); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__fp_t(FP_DYNAMIC); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FP_DYNAMIC, __pyx_t_2) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FP_DYNAMIC, __pyx_t_2) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_lapjv.pyx":41
- * 
+  /* "_lapjv.pyx":42
+ * # https://github.com/rathaROG/lapx/pull/7
  * 
  * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
  * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_lapjv_1lapjv, 0, __pyx_n_s_lapjv, NULL, __pyx_n_s_lapjv_2, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_lapjv_1lapjv, 0, __pyx_n_s_lapjv, NULL, __pyx_n_s_lapjv_2, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults), 0)) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults), 0)) __PYX_ERR(0, 42, __pyx_L1_error)
 
-  /* "_lapjv.pyx":44
+  /* "_lapjv.pyx":45
  * @cython.wraparound(False)
  * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
  *           double cost_limit=np.inf, char return_cost=True):             # <<<<<<<<<<<<<<
  *     """Solve linear assignment problem using Jonker-Volgenant algorithm.
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_inf); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_inf); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_2)->__pyx_arg_cost_limit = __pyx_t_5;
   __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_6_lapjv_4__defaults__);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lapjv, __pyx_t_2) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lapjv, __pyx_t_2) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_lapjv.pyx":136
+  /* "_lapjv.pyx":139
  * 
  * 
  * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
- * def _lapmod(
+ * def _lapmod(const uint_t n,
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_lapjv_3_lapmod, 0, __pyx_n_s_lapmod, NULL, __pyx_n_s_lapjv_2, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_lapjv_3_lapmod, 0, __pyx_n_s_lapmod, NULL, __pyx_n_s_lapjv_2, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults1), 0)) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults1), 0)) __PYX_ERR(0, 139, __pyx_L1_error)
 
-  /* "_lapjv.pyx":143
- *         cnp.ndarray ii not None,
- *         cnp.ndarray kk not None,
- *         fp_t fp_version=FP_DYNAMIC):             # <<<<<<<<<<<<<<
+  /* "_lapjv.pyx":145
+ *             cnp.ndarray ii not None,
+ *             cnp.ndarray kk not None,
+ *             fp_t fp_version=FP_DYNAMIC):             # <<<<<<<<<<<<<<
  *     """Internal function called from lapmod(..., fast=True)."""
  *     cdef cnp.ndarray[cnp.double_t, ndim=1, mode='c'] cc_c = \
  */
   __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_t_2)->__pyx_arg_fp_version = FP_DYNAMIC;
   __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_6_lapjv_6__defaults__);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lapmod, __pyx_t_2) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lapmod, __pyx_t_2) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_lapjv.pyx":1
  * # Tomas Kazmar, 2012-2017, BSD 2-clause license, see LICENSE.             # <<<<<<<<<<<<<<
  * 
  * # Updated 2023/06/22 by rathaROG
  */
@@ -9099,147 +9216,14 @@
 
 /* BufferFallbackError */
   static void __Pyx_RaiseBufferFallbackError(void) {
   PyErr_SetString(PyExc_ValueError,
      "Buffer acquisition failed on assignment; and then reacquiring the old buffer failed too!");
 }
 
-/* PyIntBinop */
-  #if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check) {
-    CYTHON_MAYBE_UNUSED_VAR(intval);
-    CYTHON_MAYBE_UNUSED_VAR(inplace);
-    CYTHON_UNUSED_VAR(zerodivision_check);
-    #if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_CheckExact(op1))) {
-        const long b = intval;
-        long x;
-        long a = PyInt_AS_LONG(op1);
-        
-            x = (long)((unsigned long)a + (unsigned long)b);
-            if (likely((x^a) >= 0 || (x^b) >= 0))
-                return PyInt_FromLong(x);
-            return PyLong_Type.tp_as_number->nb_add(op1, op2);
-    }
-    #endif
-    #if CYTHON_USE_PYLONG_INTERNALS
-    if (likely(PyLong_CheckExact(op1))) {
-        const long b = intval;
-        long a, x;
-#ifdef HAVE_LONG_LONG
-        const PY_LONG_LONG llb = intval;
-        PY_LONG_LONG lla, llx;
-#endif
-        if (unlikely(__Pyx_PyLong_IsZero(op1))) {
-            return __Pyx_NewRef(op2);
-        }
-        if (likely(__Pyx_PyLong_IsCompact(op1))) {
-            a = __Pyx_PyLong_CompactValue(op1);
-        } else {
-            const digit* digits = __Pyx_PyLong_Digits(op1);
-            const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(op1);
-            switch (size) {
-                case -2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
-                        lla = -(PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        a = (long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
-                        lla = (PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        a = -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
-                        lla = -(PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        a = (long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
-                        lla = (PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                        a = -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
-                        lla = -(PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                        a = (long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
-                        lla = (PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                default: return PyLong_Type.tp_as_number->nb_add(op1, op2);
-            }
-        }
-                x = a + b;
-            return PyLong_FromLong(x);
-#ifdef HAVE_LONG_LONG
-        long_long:
-                llx = lla + llb;
-            return PyLong_FromLongLong(llx);
-#endif
-        
-        
-    }
-    #endif
-    if (PyFloat_CheckExact(op1)) {
-        const long b = intval;
-#if CYTHON_COMPILING_IN_LIMITED_API
-        double a = __pyx_PyFloat_AsDouble(op1);
-#else
-        double a = PyFloat_AS_DOUBLE(op1);
-#endif
-            double result;
-            
-            PyFPE_START_PROTECT("add", return NULL)
-            result = ((double)a) + (double)b;
-            PyFPE_END_PROTECT(result)
-            return PyFloat_FromDouble(result);
-    }
-    return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
-}
-#endif
-
 /* PyFunctionFastCall */
   #if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject **fastlocals;
@@ -9610,18 +9594,18 @@
         return __Pyx_PyObject_GetIndex(obj, key);
     }
     return __Pyx_PyObject_GetItem_Slow(obj, key);
 }
 #endif
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -9667,23 +9651,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -12651,78 +12635,14 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to enum fp_t");
     return (enum fp_t) -1;
 }
 
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const char neg_one = (char) -1, const_zero = (char) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(char) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(char) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(char) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(char) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(char) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
-        return _PyLong_FromByteArray(bytes, sizeof(char),
-                                     little, !is_unsigned);
-#else
-        PyObject *from_bytes, *result = NULL;
-        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
-        if (!from_bytes) return NULL;
-        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(char));
-        if (!py_bytes) goto limited_bad;
-        order_str = PyUnicode_FromString(little ? "little" : "big");
-        if (!order_str) goto limited_bad;
-        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
-        if (!arg_tuple) goto limited_bad;
-        if (!is_unsigned) {
-            kwds = PyDict_New();
-            if (!kwds) goto limited_bad;
-            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
-        }
-        result = PyObject_Call(from_bytes, arg_tuple, kwds);
-        limited_bad:
-        Py_XDECREF(kwds);
-        Py_XDECREF(arg_tuple);
-        Py_XDECREF(order_str);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(from_bytes);
-        return result;
-#endif
-    }
-}
-
-/* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint_t(uint_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const uint_t neg_one = (uint_t) -1, const_zero = (uint_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
@@ -13052,14 +12972,78 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const char neg_one = (char) -1, const_zero = (char) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(char) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(char) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(char) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(char) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(char) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
+        return _PyLong_FromByteArray(bytes, sizeof(char),
+                                     little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(char));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
+    }
+}
+
+/* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
```

### Comparing `lapx-0.5.7/_lapjv_src/_lapjv.pyx` & `lapx-0.5.8/_lapjv_src/_lapjv.pyx`

 * *Files 7% similar despite different names*

```diff
@@ -14,34 +14,35 @@
     ctypedef signed int int_t
     ctypedef unsigned int uint_t
     cdef int LARGE
     cdef enum fp_t:
         FP_1
         FP_2
         FP_DYNAMIC
-    int lapjv_internal(
-            const uint_t n,
-            double *cost[],
-            int_t *x,
-            int_t *y)
-    int lapmod_internal(
-            const uint_t n,
-            double *cc,
-            uint_t *ii,
-            uint_t *kk,
-            int_t *x,
-            int_t *y,
-            fp_t fp_version)
+    int lapjv_internal(const uint_t n,
+                       double *cost[],
+                       int_t *x,
+                       int_t *y)
+    int lapmod_internal(const uint_t n,
+                        double *cc,
+                        uint_t *ii,
+                        uint_t *kk,
+                        int_t *x,
+                        int_t *y,
+                        fp_t fp_version)
 
 LARGE_ = LARGE
 FP_1_ = FP_1
 FP_2_ = FP_2
 FP_DYNAMIC_ = FP_DYNAMIC
 
 
+# Improved efficiency by raphaelreme
+# https://github.com/rathaROG/lapx/pull/7
+
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def lapjv(cnp.ndarray cost not None, char extend_cost=False,
           double cost_limit=np.inf, char return_cost=True):
     """Solve linear assignment problem using Jonker-Volgenant algorithm.
 
     Parameters
@@ -82,24 +83,26 @@
     if n_rows == n_cols:
         n = n_rows
     else:
         if not extend_cost:
             raise ValueError(
                     'Square cost array expected. If cost is intentionally '
                     'non-square, pass extend_cost=True.')
-    if extend_cost or cost_limit < np.inf:
+    if cost_limit < np.inf:
         n = n_rows + n_cols
         cost_c_extended = np.empty((n, n), dtype=np.double)
-        if cost_limit < np.inf:
-            cost_c_extended[:] = cost_limit / 2.
-        else:
-            cost_c_extended[:] = cost_c.max() + 1
+        cost_c_extended[:] = cost_limit / 2.
         cost_c_extended[n_rows:, n_cols:] = 0
         cost_c_extended[:n_rows, :n_cols] = cost_c
         cost_c = cost_c_extended
+    elif extend_cost:
+        n = max(n_rows, n_cols)
+        cost_c_extended = np.zeros((n, n), dtype=np.double)
+        cost_c_extended[:n_rows, :n_cols] = cost_c
+        cost_c = cost_c_extended
 
     cdef double **cost_ptr
     cost_ptr = <double **> malloc(n * sizeof(double *))
     cdef int i
     for i in range(n):
         cost_ptr[i] = &cost_c[i, 0]
 
@@ -113,15 +116,15 @@
     if ret != 0:
         if ret == -1:
             raise MemoryError('Out of memory.')
         raise RuntimeError('Unknown error (lapjv_internal returned %d).' % ret)
 
 
     cdef double opt = np.nan
-    if n != n_rows:
+    if cost_limit < np.inf or extend_cost:
         x_c[x_c >= n_cols] = -1
         y_c[y_c >= n_rows] = -1
         x_c = x_c[:n_rows]
         y_c = y_c[:n_cols]
         if return_cost:
             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
     elif return_cost:
@@ -131,34 +134,32 @@
         return opt, x_c, y_c
     else:
         return x_c, y_c
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def _lapmod(
-        const uint_t n,
-        cnp.ndarray cc not None,
-        cnp.ndarray ii not None,
-        cnp.ndarray kk not None,
-        fp_t fp_version=FP_DYNAMIC):
+def _lapmod(const uint_t n,
+            cnp.ndarray cc not None,
+            cnp.ndarray ii not None,
+            cnp.ndarray kk not None,
+            fp_t fp_version=FP_DYNAMIC):
     """Internal function called from lapmod(..., fast=True)."""
     cdef cnp.ndarray[cnp.double_t, ndim=1, mode='c'] cc_c = \
         np.ascontiguousarray(cc, dtype=np.double)
     cdef cnp.ndarray[uint_t, ndim=1, mode='c'] ii_c = \
         np.ascontiguousarray(ii, dtype=np.uint32)
     cdef cnp.ndarray[uint_t, ndim=1, mode='c'] kk_c = \
         np.ascontiguousarray(kk, dtype=np.uint32)
     cdef cnp.ndarray[int_t, ndim=1, mode='c'] x_c = \
         np.empty((n,), dtype=np.int32)
     cdef cnp.ndarray[int_t, ndim=1, mode='c'] y_c = \
         np.empty((n,), dtype=np.int32)
 
-    cdef int_t ret = lapmod_internal(
-                n, &cc_c[0], &ii_c[0], &kk_c[0],
-                &x_c[0], &y_c[0], fp_version)
+    cdef int_t ret = lapmod_internal(n, &cc_c[0], &ii_c[0], &kk_c[0], 
+                                     &x_c[0], &y_c[0], fp_version)
     if ret != 0:
         if ret == -1:
             raise MemoryError('Out of memory.')
         raise RuntimeError('Unknown error (lapmod_internal returned %d).' % ret)
 
     return x_c, y_c
```

### Comparing `lapx-0.5.7/_lapjv_src/lapjv.cpp` & `lapx-0.5.8/_lapjv_src/lapjv.cpp`

 * *Files identical despite different names*

### Comparing `lapx-0.5.7/_lapjv_src/lapjv.h` & `lapx-0.5.8/_lapjv_src/lapjv.h`

 * *Files identical despite different names*

### Comparing `lapx-0.5.7/_lapjv_src/lapmod.cpp` & `lapx-0.5.8/_lapjv_src/lapmod.cpp`

 * *Files identical despite different names*

### Comparing `lapx-0.5.7/lap/__init__.py` & `lapx-0.5.8/lap/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 lapjv
     Find optimal (minimum-cost) assignment for a dense cost matrix.
 lapmod
     Find optimal (minimum-cost) assignment for a sparse cost matrix.
 """
 
-__version__ = '0.5.7'
+__version__ = '0.5.8'
 
 from ._lapjv import (
     lapjv,
     LARGE_ as LARGE,
     FP_1_ as FP_1,
     FP_2_ as FP_2,
     FP_DYNAMIC_ as FP_DYNAMIC
```

### Comparing `lapx-0.5.7/lap/lapmod.py` & `lapx-0.5.8/lap/lapmod.py`

 * *Files identical despite different names*

### Comparing `lapx-0.5.7/lap/tests/cost_eps.csv.gz` & `lapx-0.5.8/lap/tests/cost_eps.csv.gz`

 * *Files identical despite different names*

### Comparing `lapx-0.5.7/lap/tests/test_arr_loop.py` & `lapx-0.5.8/lap/tests/test_arr_loop.py`

 * *Files identical despite different names*

### Comparing `lapx-0.5.7/lap/tests/test_lapjv.py` & `lapx-0.5.8/lap/tests/test_lapjv.py`

 * *Files identical despite different names*

### Comparing `lapx-0.5.7/lap/tests/test_lapmod.py` & `lapx-0.5.8/lap/tests/test_lapmod.py`

 * *Files identical despite different names*

### Comparing `lapx-0.5.7/lap/tests/test_utils.py` & `lapx-0.5.8/lap/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lapx-0.5.7/lapx.egg-info/PKG-INFO` & `lapx-0.5.8/lapx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lapx
-Version: 0.5.7
+Version: 0.5.8
 Summary: Linear Assignment Problem solver (LAPJV/LAPMOD).
 Home-page: https://github.com/rathaROG/lapx
 Author: rathaROG
 License: BSD-2-Clause
 Keywords: Linear Assignment,LAPJV,LAPMOD,lap
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -25,14 +25,15 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Cython>=0.29.32
 Requires-Dist: numpy>=1.21.6
 
 [![Test Simple](https://github.com/rathaROG/lapx/actions/workflows/test_simple.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/test_simple.yaml)
 [![Benchmark](https://github.com/rathaROG/lapx/actions/workflows/benchmark.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/benchmark.yaml)
```

### Comparing `lapx-0.5.7/setup.py` & `lapx-0.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,16 +99,17 @@
         long_description_content_type="text/markdown",
         author="rathaROG",
         url="https://github.com/rathaROG/lapx",
         license=LICENSE,
         packages=packages,
         package_data=package_data,
         include_package_data=True,
-        keywords=['Linear Assignment', 'LAPJV', 'LAPMOD', 'lap'],
         install_requires=read_requirements(),
+        keywords=['Linear Assignment', 'LAPJV', 'LAPMOD', 'lap'],
+        python_requires=">=3.7",
         classifiers=['Development Status :: 4 - Beta',
                      'Environment :: Console',
                      'Intended Audience :: Developers',
                      'Intended Audience :: Education',
                      'Intended Audience :: Science/Research',
                      'License :: OSI Approved :: BSD License',
                      'Programming Language :: Python :: 3',
```

