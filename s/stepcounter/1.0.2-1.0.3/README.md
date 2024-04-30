# Comparing `tmp/stepcounter-1.0.2-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl.zip` & `tmp/stepcounter-1.0.3-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,61 +1,91 @@
-Zip file size: 75934 bytes, number of entries: 59
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:30 stepcounter.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:30 example/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:30 stepcounter-1.0.2.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:30 src/
--rw-r--r--  2.0 unx      259 b- defN 24-Apr-29 19:30 example/gcd.py
--rw-r--r--  2.0 unx     1248 b- defN 24-Apr-29 19:30 example/example.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:30 example/__init__.py
--rw-r--r--  2.0 unx      225 b- defN 24-Apr-29 19:30 stepcounter-1.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       12 b- defN 24-Apr-29 19:30 stepcounter-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    10979 b- defN 24-Apr-29 19:30 stepcounter-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      154 b- defN 24-Apr-29 19:30 stepcounter-1.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       54 b- defN 24-Apr-29 19:30 stepcounter-1.0.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx     4236 b- defN 24-Apr-29 19:30 stepcounter-1.0.2.dist-info/RECORD
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:30 src/profiler/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:30 src/parser/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:30 src/step_counting/
--rw-r--r--  2.0 unx     1274 b- defN 24-Apr-29 19:30 src/step_counter.py
--rw-r--r--  2.0 unx     1140 b- defN 24-Apr-29 19:30 src/utils.py
--rw-r--r--  2.0 unx       77 b- defN 24-Apr-29 19:30 src/__init__.py
--rw-r--r--  2.0 unx       77 b- defN 24-Apr-29 19:30 src/profiler/__init__.py
--rw-r--r--  2.0 unx     3797 b- defN 24-Apr-29 19:30 src/profiler/profiler.py
--rw-r--r--  2.0 unx      557 b- defN 24-Apr-29 19:30 src/parser/parser.py
--rw-r--r--  2.0 unx       77 b- defN 24-Apr-29 19:30 src/parser/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:30 src/step_counting/patch/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:30 src/step_counting/utils/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:30 src/step_counting/decorator/
--rw-r--r--  2.0 unx     1058 b- defN 24-Apr-29 19:30 src/step_counting/non_builtin_types.py
--rw-r--r--  2.0 unx     8269 b- defN 24-Apr-29 19:30 src/step_counting/setup_recording.py
--rw-r--r--  2.0 unx     1518 b- defN 24-Apr-29 19:30 src/step_counting/ignor.py
--rw-r--r--  2.0 unx       77 b- defN 24-Apr-29 19:30 src/step_counting/__init__.py
--rw-r--r--  2.0 unx     2421 b- defN 24-Apr-29 19:30 src/step_counting/ib111_restrictions.py
--rw-r--r--  2.0 unx      524 b- defN 24-Apr-29 19:30 src/step_counting/original_methods.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:30 src/step_counting/patch/bin/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:30 src/step_counting/patch/c_modules/
--rw-r--r--  2.0 unx    11912 b- defN 24-Apr-29 19:30 src/step_counting/patch/patching.py
--rw-r--r--  2.0 unx     2259 b- defN 24-Apr-29 19:30 src/step_counting/patch/method_switch.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:30 src/step_counting/patch/__init__.py
--rw-r--r--  2.0 unx    13845 b- defN 24-Apr-29 19:30 src/step_counting/patch/py_object.py
--rw-r--r--  2.0 unx     3617 b- defN 24-Apr-29 19:30 src/step_counting/patch/patch_imports.py
--rwxrwxr-x  2.0 unx    28176 b- defN 24-Apr-29 19:30 src/step_counting/patch/bin/patchdictionary.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x  2.0 unx    26456 b- defN 24-Apr-29 19:30 src/step_counting/patch/bin/patchlist.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x  2.0 unx    25848 b- defN 24-Apr-29 19:30 src/step_counting/patch/bin/patchtuple.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x  2.0 unx    25320 b- defN 24-Apr-29 19:30 src/step_counting/patch/bin/patchint.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x  2.0 unx    25280 b- defN 24-Apr-29 19:30 src/step_counting/patch/bin/patchstr.cpython-310-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:30 src/step_counting/patch/bin/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:30 src/step_counting/patch/c_modules/__init__.py
--rw-r--r--  2.0 unx     3068 b- defN 24-Apr-29 19:30 src/step_counting/utils/module.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:30 src/step_counting/utils/__init__.py
--rw-r--r--  2.0 unx     1882 b- defN 24-Apr-29 19:30 src/step_counting/utils/methods.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:30 src/step_counting/decorator/evaluations/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:30 src/step_counting/decorator/records/
--rw-r--r--  2.0 unx     4192 b- defN 24-Apr-29 19:30 src/step_counting/decorator/utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:30 src/step_counting/decorator/__init__.py
--rw-r--r--  2.0 unx     6204 b- defN 24-Apr-29 19:30 src/step_counting/decorator/decorators.py
--rw-r--r--  2.0 unx     3081 b- defN 24-Apr-29 19:30 src/step_counting/decorator/evaluations/complexities.py
--rw-r--r--  2.0 unx     5682 b- defN 24-Apr-29 19:30 src/step_counting/decorator/evaluations/evaluations.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:30 src/step_counting/decorator/evaluations/__init__.py
--rw-r--r--  2.0 unx     9849 b- defN 24-Apr-29 19:30 src/step_counting/decorator/records/record_classes.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:30 src/step_counting/decorator/records/__init__.py
-59 files, 234704 bytes uncompressed, 67376 bytes compressed:  71.3%
+Zip file size: 89800 bytes, number of entries: 89
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 stepcounter-1.0.3.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 stepcounter.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 example/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 src/
+-rw-r--r--  2.0 unx      225 b- defN 24-Apr-29 19:35 stepcounter-1.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       12 b- defN 24-Apr-29 19:35 stepcounter-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    10979 b- defN 24-Apr-29 19:35 stepcounter-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      154 b- defN 24-Apr-29 19:35 stepcounter-1.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       54 b- defN 24-Apr-29 19:35 stepcounter-1.0.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx     7696 b- defN 24-Apr-29 19:35 stepcounter-1.0.3.dist-info/RECORD
+-rw-r--r--  2.0 unx      259 b- defN 24-Apr-29 19:35 example/gcd.py
+-rw-r--r--  2.0 unx     1248 b- defN 24-Apr-29 19:35 example/example.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:35 example/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 src/profiler/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 src/parser/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 src/step_counting/
+-rw-r--r--  2.0 unx     1274 b- defN 24-Apr-29 19:35 src/step_counter.py
+-rw-r--r--  2.0 unx     1140 b- defN 24-Apr-29 19:35 src/utils.py
+-rw-r--r--  2.0 unx       77 b- defN 24-Apr-29 19:35 src/__init__.py
+-rw-r--r--  2.0 unx       77 b- defN 24-Apr-29 19:35 src/profiler/__init__.py
+-rw-r--r--  2.0 unx     3797 b- defN 24-Apr-29 19:35 src/profiler/profiler.py
+-rw-r--r--  2.0 unx      557 b- defN 24-Apr-29 19:35 src/parser/parser.py
+-rw-r--r--  2.0 unx       77 b- defN 24-Apr-29 19:35 src/parser/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 src/step_counting/patch/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 src/step_counting/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 src/step_counting/decorator/
+-rw-r--r--  2.0 unx     1058 b- defN 24-Apr-29 19:35 src/step_counting/non_builtin_types.py
+-rw-r--r--  2.0 unx     8269 b- defN 24-Apr-29 19:35 src/step_counting/setup_recording.py
+-rw-r--r--  2.0 unx     1518 b- defN 24-Apr-29 19:35 src/step_counting/ignor.py
+-rw-r--r--  2.0 unx       77 b- defN 24-Apr-29 19:35 src/step_counting/__init__.py
+-rw-r--r--  2.0 unx     2421 b- defN 24-Apr-29 19:35 src/step_counting/ib111_restrictions.py
+-rw-r--r--  2.0 unx      524 b- defN 24-Apr-29 19:35 src/step_counting/original_methods.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 src/step_counting/patch/bin/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 src/step_counting/patch/c_modules/
+-rw-r--r--  2.0 unx    11912 b- defN 24-Apr-29 19:35 src/step_counting/patch/patching.py
+-rw-r--r--  2.0 unx     2259 b- defN 24-Apr-29 19:35 src/step_counting/patch/method_switch.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:35 src/step_counting/patch/__init__.py
+-rw-r--r--  2.0 unx    13845 b- defN 24-Apr-29 19:35 src/step_counting/patch/py_object.py
+-rw-r--r--  2.0 unx     3617 b- defN 24-Apr-29 19:35 src/step_counting/patch/patch_imports.py
+-rwxrwxr-x  2.0 unx    28176 b- defN 24-Apr-29 19:35 src/step_counting/patch/bin/patchdictionary.cpython-310-x86_64-linux-gnu.so
+-rwxrwxr-x  2.0 unx    26456 b- defN 24-Apr-29 19:35 src/step_counting/patch/bin/patchlist.cpython-310-x86_64-linux-gnu.so
+-rwxrwxr-x  2.0 unx    25848 b- defN 24-Apr-29 19:35 src/step_counting/patch/bin/patchtuple.cpython-310-x86_64-linux-gnu.so
+-rwxrwxr-x  2.0 unx    25320 b- defN 24-Apr-29 19:35 src/step_counting/patch/bin/patchint.cpython-310-x86_64-linux-gnu.so
+-rwxrwxr-x  2.0 unx    25280 b- defN 24-Apr-29 19:35 src/step_counting/patch/bin/patchstr.cpython-310-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:35 src/step_counting/patch/bin/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:35 src/step_counting/patch/c_modules/__init__.py
+-rw-r--r--  2.0 unx     3068 b- defN 24-Apr-29 19:35 src/step_counting/utils/module.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:35 src/step_counting/utils/__init__.py
+-rw-r--r--  2.0 unx     1882 b- defN 24-Apr-29 19:35 src/step_counting/utils/methods.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 src/step_counting/decorator/evaluations/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 src/step_counting/decorator/records/
+-rw-r--r--  2.0 unx     4192 b- defN 24-Apr-29 19:35 src/step_counting/decorator/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:35 src/step_counting/decorator/__init__.py
+-rw-r--r--  2.0 unx     6204 b- defN 24-Apr-29 19:35 src/step_counting/decorator/decorators.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 src/step_counting/decorator/evaluations/builtins/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/
+-rw-r--r--  2.0 unx     3081 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/complexities.py
+-rw-r--r--  2.0 unx     5682 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/evaluations.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/__init__.py
+-rw-r--r--  2.0 unx      381 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/builtins/complex_evaluations.py
+-rw-r--r--  2.0 unx     2133 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/builtins/str_evaluations.py
+-rw-r--r--  2.0 unx     4351 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/builtins/builtins_evaluations.py
+-rw-r--r--  2.0 unx     1799 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/builtins/bytes_evaluations.py
+-rw-r--r--  2.0 unx      958 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/builtins/int_evaluations.py
+-rw-r--r--  2.0 unx     2059 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/builtins/list_evaluations.py
+-rw-r--r--  2.0 unx      451 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/builtins/tuple_evaluations.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/builtins/__init__.py
+-rw-r--r--  2.0 unx     1017 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/builtins/dict_evaluations.py
+-rw-r--r--  2.0 unx     1834 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/builtins/set_evaluations.py
+-rw-r--r--  2.0 unx      702 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/builtins/float_evaluations.py
+-rw-r--r--  2.0 unx      226 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/csv_evaluations.py
+-rw-r--r--  2.0 unx      120 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/glob_evaluations.py
+-rw-r--r--  2.0 unx      417 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/fractions_evaluation.py
+-rw-r--r--  2.0 unx     2442 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/datetime_evaluations.py
+-rw-r--r--  2.0 unx      593 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/zipfile_evaluations.py
+-rw-r--r--  2.0 unx      692 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/io_evaluations.py
+-rw-r--r--  2.0 unx      335 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/os_evaluations.py
+-rw-r--r--  2.0 unx     1001 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/httpclient_evaluations.py
+-rw-r--r--  2.0 unx      150 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/shutil_evaluations.py
+-rw-r--r--  2.0 unx      120 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/gzip_evaluation.py
+-rw-r--r--  2.0 unx      553 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/math_evaluations.py
+-rw-r--r--  2.0 unx      190 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/sys_evaluations.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/__init__.py
+-rw-r--r--  2.0 unx      188 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/json_evaluations.py
+-rw-r--r--  2.0 unx      130 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/calendar_evaluations.py
+-rw-r--r--  2.0 unx      340 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/turtle_evaluations.py
+-rw-r--r--  2.0 unx      214 b- defN 24-Apr-29 19:35 src/step_counting/decorator/evaluations/ib111/re_evaluations.py
+-rw-r--r--  2.0 unx     9849 b- defN 24-Apr-29 19:35 src/step_counting/decorator/records/record_classes.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:35 src/step_counting/decorator/records/__init__.py
+89 files, 261560 bytes uncompressed, 75052 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -1,44 +1,44 @@
-Filename: stepcounter.libs/
+Filename: stepcounter-1.0.3.dist-info/
 Comment: 
 
-Filename: example/
+Filename: stepcounter.libs/
 Comment: 
 
-Filename: stepcounter-1.0.2.dist-info/
+Filename: example/
 Comment: 
 
 Filename: src/
 Comment: 
 
-Filename: example/gcd.py
+Filename: stepcounter-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: example/example.py
+Filename: stepcounter-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: example/__init__.py
+Filename: stepcounter-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: stepcounter-1.0.2.dist-info/WHEEL
+Filename: stepcounter-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: stepcounter-1.0.2.dist-info/top_level.txt
+Filename: stepcounter-1.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: stepcounter-1.0.2.dist-info/LICENSE
+Filename: stepcounter-1.0.3.dist-info/RECORD
 Comment: 
 
-Filename: stepcounter-1.0.2.dist-info/METADATA
+Filename: example/gcd.py
 Comment: 
 
-Filename: stepcounter-1.0.2.dist-info/entry_points.txt
+Filename: example/example.py
 Comment: 
 
-Filename: stepcounter-1.0.2.dist-info/RECORD
+Filename: example/__init__.py
 Comment: 
 
 Filename: src/profiler/
 Comment: 
 
 Filename: src/parser/
 Comment: 
@@ -156,23 +156,113 @@
 
 Filename: src/step_counting/decorator/__init__.py
 Comment: 
 
 Filename: src/step_counting/decorator/decorators.py
 Comment: 
 
+Filename: src/step_counting/decorator/evaluations/builtins/
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/
+Comment: 
+
 Filename: src/step_counting/decorator/evaluations/complexities.py
 Comment: 
 
 Filename: src/step_counting/decorator/evaluations/evaluations.py
 Comment: 
 
 Filename: src/step_counting/decorator/evaluations/__init__.py
 Comment: 
 
+Filename: src/step_counting/decorator/evaluations/builtins/complex_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/builtins/str_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/builtins/builtins_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/builtins/bytes_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/builtins/int_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/builtins/list_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/builtins/tuple_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/builtins/__init__.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/builtins/dict_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/builtins/set_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/builtins/float_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/csv_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/glob_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/fractions_evaluation.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/datetime_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/zipfile_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/io_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/os_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/httpclient_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/shutil_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/gzip_evaluation.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/math_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/sys_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/__init__.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/json_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/calendar_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/turtle_evaluations.py
+Comment: 
+
+Filename: src/step_counting/decorator/evaluations/ib111/re_evaluations.py
+Comment: 
+
 Filename: src/step_counting/decorator/records/record_classes.py
 Comment: 
 
 Filename: src/step_counting/decorator/records/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `stepcounter-1.0.2.dist-info/LICENSE` & `stepcounter-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

