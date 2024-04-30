# Comparing `tmp/turbodbc-4.8.0.tar.gz` & `tmp/turbodbc-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbodbc-4.8.0.tar", last modified: Tue Nov 14 09:12:08 2023, max compression
+gzip compressed data, was "turbodbc-4.9.0.tar", last modified: Sun Nov 19 10:23:45 2023, max compression
```

## Comparing `turbodbc-4.8.0.tar` & `turbodbc-4.9.0.tar`

### file list

```diff
@@ -1,221 +1,222 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.421791 turbodbc-4.8.0/
--rw-r--r--   0 root         (0) root         (0)    20818 2020-04-16 12:00:00.000000 turbodbc-4.8.0/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)     1087 2020-04-16 12:00:00.000000 turbodbc-4.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       96 2020-04-16 12:00:00.000000 turbodbc-4.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3579 2023-11-14 09:12:08.421791 turbodbc-4.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2523 2020-04-16 12:00:00.000000 turbodbc-4.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.369790 turbodbc-4.8.0/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.373791 turbodbc-4.8.0/include/cpp_odbc/
--rw-r--r--   0 root         (0) root         (0)      957 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/column_description.h
--rw-r--r--   0 root         (0) root         (0)     2554 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/connection.h
--rw-r--r--   0 root         (0) root         (0)      893 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/cpp_odbc.h
--rw-r--r--   0 root         (0) root         (0)      512 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/credentials.h
--rw-r--r--   0 root         (0) root         (0)     1377 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/environment.h
--rw-r--r--   0 root         (0) root         (0)      551 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/error.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.373791 turbodbc-4.8.0/include/cpp_odbc/level1/
--rw-r--r--   0 root         (0) root         (0)    11658 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level1/api.h
--rw-r--r--   0 root         (0) root         (0)      506 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level1/level1.h
--rw-r--r--   0 root         (0) root         (0)     4792 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level1/unixodbc_backend.h
--rw-r--r--   0 root         (0) root         (0)     4810 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level1/unixodbc_backend_debug.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.377791 turbodbc-4.8.0/include/cpp_odbc/level2/
--rw-r--r--   0 root         (0) root         (0)    19100 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level2/api.h
--rw-r--r--   0 root         (0) root         (0)      636 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level2/diagnostic_record.h
--rw-r--r--   0 root         (0) root         (0)     1286 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level2/fixed_length_string_buffer.h
--rw-r--r--   0 root         (0) root         (0)     2498 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level2/handles.h
--rw-r--r--   0 root         (0) root         (0)      838 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level2/input_string_buffer.h
--rw-r--r--   0 root         (0) root         (0)      855 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level2/input_u16string_buffer.h
--rw-r--r--   0 root         (0) root         (0)     4565 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level2/level1_connector.h
--rw-r--r--   0 root         (0) root         (0)      736 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level2/level2.h
--rw-r--r--   0 root         (0) root         (0)     1435 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level2/string_buffer.h
--rw-r--r--   0 root         (0) root         (0)     1513 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level2/u16string_buffer.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.377791 turbodbc-4.8.0/include/cpp_odbc/level3/
--rw-r--r--   0 root         (0) root         (0)      588 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level3/level3.h
--rw-r--r--   0 root         (0) root         (0)     1909 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level3/raii_connection.h
--rw-r--r--   0 root         (0) root         (0)     1323 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level3/raii_environment.h
--rw-r--r--   0 root         (0) root         (0)     2606 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/level3/raii_statement.h
--rw-r--r--   0 root         (0) root         (0)      562 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/make_environment.h
--rw-r--r--   0 root         (0) root         (0)     3045 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/multi_value_buffer.h
--rw-r--r--   0 root         (0) root         (0)     7841 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/cpp_odbc/statement.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.381790 turbodbc-4.8.0/include/turbodbc/
--rw-r--r--   0 root         (0) root         (0)     1443 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/buffer_size.h
--rw-r--r--   0 root         (0) root         (0)     1241 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/column.h
--rw-r--r--   0 root         (0) root         (0)      217 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/column_info.h
--rw-r--r--   0 root         (0) root         (0)     1602 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/command.h
--rw-r--r--   0 root         (0) root         (0)      842 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/configuration.h
--rw-r--r--   0 root         (0) root         (0)      486 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/connect.h
--rw-r--r--   0 root         (0) root         (0)     1427 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/connection.h
--rw-r--r--   0 root         (0) root         (0)     1093 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/cursor.h
--rw-r--r--   0 root         (0) root         (0)     1640 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/description.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.381790 turbodbc-4.8.0/include/turbodbc/descriptions/
--rw-r--r--   0 root         (0) root         (0)      552 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/descriptions/boolean_description.h
--rw-r--r--   0 root         (0) root         (0)      537 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/descriptions/date_description.h
--rw-r--r--   0 root         (0) root         (0)      615 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/descriptions/floating_point_description.h
--rw-r--r--   0 root         (0) root         (0)      552 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/descriptions/integer_description.h
--rw-r--r--   0 root         (0) root         (0)      693 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/descriptions/string_description.h
--rw-r--r--   0 root         (0) root         (0)      562 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/descriptions/timestamp_description.h
--rw-r--r--   0 root         (0) root         (0)      698 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/descriptions/unicode_description.h
--rw-r--r--   0 root         (0) root         (0)      404 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/descriptions.h
--rw-r--r--   0 root         (0) root         (0)      230 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/errors.h
--rw-r--r--   0 root         (0) root         (0)      746 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/field.h
--rw-r--r--   0 root         (0) root         (0)      711 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/field_translator.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.381790 turbodbc-4.8.0/include/turbodbc/field_translators/
--rw-r--r--   0 root         (0) root         (0)      372 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/field_translators/boolean_translator.h
--rw-r--r--   0 root         (0) root         (0)      354 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/field_translators/date_translator.h
--rw-r--r--   0 root         (0) root         (0)      386 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/field_translators/float64_translator.h
--rw-r--r--   0 root         (0) root         (0)      373 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/field_translators/int64_translator.h
--rw-r--r--   0 root         (0) root         (0)      368 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/field_translators/string_translator.h
--rw-r--r--   0 root         (0) root         (0)      374 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/field_translators/timestamp_translator.h
--rw-r--r--   0 root         (0) root         (0)      364 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/field_translators.h
--rw-r--r--   0 root         (0) root         (0)     1019 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/make_description.h
--rw-r--r--   0 root         (0) root         (0)      316 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/make_field_translator.h
--rw-r--r--   0 root         (0) root         (0)     1761 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/parameter.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.385791 turbodbc-4.8.0/include/turbodbc/parameter_sets/
--rw-r--r--   0 root         (0) root         (0)     2469 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/parameter_sets/bound_parameter_set.h
--rw-r--r--   0 root         (0) root         (0)      745 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/parameter_sets/field_parameter_set.h
--rw-r--r--   0 root         (0) root         (0)      704 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/parameter_sets/set_field.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.385791 turbodbc-4.8.0/include/turbodbc/result_sets/
--rw-r--r--   0 root         (0) root         (0)     1254 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/result_sets/bound_result_set.h
--rw-r--r--   0 root         (0) root         (0)     2327 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/result_sets/double_buffered_result_set.h
--rw-r--r--   0 root         (0) root         (0)      971 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/result_sets/field_result_set.h
--rw-r--r--   0 root         (0) root         (0)     1256 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/result_sets/result_set.h
--rw-r--r--   0 root         (0) root         (0)     1028 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/result_sets/row_based_result_set.h
--rw-r--r--   0 root         (0) root         (0)      157 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/string_helpers.h
--rw-r--r--   0 root         (0) root         (0)     1190 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/time_helpers.h
--rw-r--r--   0 root         (0) root         (0)      459 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc/type_code.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.385791 turbodbc-4.8.0/include/turbodbc_arrow/
--rw-r--r--   0 root         (0) root         (0)     1674 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc_arrow/arrow_result_set.h
--rw-r--r--   0 root         (0) root         (0)      297 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc_arrow/set_arrow_parameters.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.385791 turbodbc-4.8.0/include/turbodbc_numpy/
--rw-r--r--   0 root         (0) root         (0)      556 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc_numpy/binary_column.h
--rw-r--r--   0 root         (0) root         (0)      683 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc_numpy/datetime_column.h
--rw-r--r--   0 root         (0) root         (0)      378 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc_numpy/make_numpy_array.h
--rw-r--r--   0 root         (0) root         (0)      698 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc_numpy/masked_column.h
--rw-r--r--   0 root         (0) root         (0)      459 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc_numpy/ndarrayobject.h
--rw-r--r--   0 root         (0) root         (0)      756 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc_numpy/numpy_result_set.h
--rw-r--r--   0 root         (0) root         (0)      260 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc_numpy/numpy_type.h
--rw-r--r--   0 root         (0) root         (0)      299 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc_numpy/set_numpy_parameters.h
--rw-r--r--   0 root         (0) root         (0)      508 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc_numpy/string_column.h
--rw-r--r--   0 root         (0) root         (0)      511 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc_numpy/unicode_column.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.385791 turbodbc-4.8.0/include/turbodbc_python/
--rw-r--r--   0 root         (0) root         (0)      454 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc_python/determine_parameter_type.h
--rw-r--r--   0 root         (0) root         (0)      685 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc_python/python_parameter_set.h
--rw-r--r--   0 root         (0) root         (0)      885 2020-04-16 12:00:00.000000 turbodbc-4.8.0/include/turbodbc_python/python_result_set.h
--rw-r--r--   0 root         (0) root         (0)      155 2023-11-14 09:12:08.421791 turbodbc-4.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    10193 2020-04-16 12:00:00.000000 turbodbc-4.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.369790 turbodbc-4.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.389791 turbodbc-4.8.0/src/cpp_odbc/
--rw-r--r--   0 root         (0) root         (0)     2694 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/column_description.cpp
--rw-r--r--   0 root         (0) root         (0)      802 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/connection.cpp
--rw-r--r--   0 root         (0) root         (0)      190 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/cpp_odbc.cpp
--rw-r--r--   0 root         (0) root         (0)      411 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/environment.cpp
--rw-r--r--   0 root         (0) root         (0)      744 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/error.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.389791 turbodbc-4.8.0/src/cpp_odbc/level1/
--rw-r--r--   0 root         (0) root         (0)     7405 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level1/api.cpp
--rw-r--r--   0 root         (0) root         (0)      193 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level1/level1.cpp
--rw-r--r--   0 root         (0) root         (0)     7663 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level1/unixodbc_backend.cpp
--rw-r--r--   0 root         (0) root         (0)    12404 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level1/unixodbc_backend_debug.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.389791 turbodbc-4.8.0/src/cpp_odbc/level2/
--rw-r--r--   0 root         (0) root         (0)     5853 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level2/api.cpp
--rw-r--r--   0 root         (0) root         (0)     1265 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level2/handles.cpp
--rw-r--r--   0 root         (0) root         (0)      419 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level2/input_string_buffer.cpp
--rw-r--r--   0 root         (0) root         (0)      457 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level2/input_u16string_buffer.cpp
--rw-r--r--   0 root         (0) root         (0)    16753 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level2/level1_connector.cpp
--rw-r--r--   0 root         (0) root         (0)      193 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level2/level2.cpp
--rw-r--r--   0 root         (0) root         (0)      595 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level2/string_buffer.cpp
--rw-r--r--   0 root         (0) root         (0)      621 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level2/u16string_buffer.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.393791 turbodbc-4.8.0/src/cpp_odbc/level3/
--rw-r--r--   0 root         (0) root         (0)      193 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level3/level3.cpp
--rw-r--r--   0 root         (0) root         (0)     3649 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level3/raii_connection.cpp
--rw-r--r--   0 root         (0) root         (0)     1623 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level3/raii_environment.cpp
--rw-r--r--   0 root         (0) root         (0)     3845 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/level3/raii_statement.cpp
--rw-r--r--   0 root         (0) root         (0)      949 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/make_environment.cpp
--rw-r--r--   0 root         (0) root         (0)     1816 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/multi_value_buffer.cpp
--rw-r--r--   0 root         (0) root         (0)     2787 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/cpp_odbc/statement.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.397791 turbodbc-4.8.0/src/turbodbc/
--rw-r--r--   0 root         (0) root         (0)     1218 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/buffer_size.cpp
--rw-r--r--   0 root         (0) root         (0)      963 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/column.cpp
--rw-r--r--   0 root         (0) root         (0)     1805 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/command.cpp
--rw-r--r--   0 root         (0) root         (0)      901 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/configuration.cpp
--rw-r--r--   0 root         (0) root         (0)      298 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/connect.cpp
--rw-r--r--   0 root         (0) root         (0)     1136 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/connection.cpp
--rw-r--r--   0 root         (0) root         (0)     1941 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/cursor.cpp
--rw-r--r--   0 root         (0) root         (0)      830 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/description.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.401791 turbodbc-4.8.0/src/turbodbc/descriptions/
--rw-r--r--   0 root         (0) root         (0)      783 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/descriptions/boolean_description.cpp
--rw-r--r--   0 root         (0) root         (0)      784 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/descriptions/date_description.cpp
--rw-r--r--   0 root         (0) root         (0)      899 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/descriptions/floating_point_description.cpp
--rw-r--r--   0 root         (0) root         (0)      810 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/descriptions/integer_description.cpp
--rw-r--r--   0 root         (0) root         (0)      915 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/descriptions/string_description.cpp
--rw-r--r--   0 root         (0) root         (0)      864 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/descriptions/timestamp_description.cpp
--rw-r--r--   0 root         (0) root         (0)      993 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/descriptions/unicode_description.cpp
--rw-r--r--   0 root         (0) root         (0)      211 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/errors.cpp
--rw-r--r--   0 root         (0) root         (0)      393 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/field_translator.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.401791 turbodbc-4.8.0/src/turbodbc/field_translators/
--rw-r--r--   0 root         (0) root         (0)      380 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/field_translators/boolean_translator.cpp
--rw-r--r--   0 root         (0) root         (0)      483 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/field_translators/date_translator.cpp
--rw-r--r--   0 root         (0) root         (0)      414 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/field_translators/float64_translator.cpp
--rw-r--r--   0 root         (0) root         (0)      403 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/field_translators/int64_translator.cpp
--rw-r--r--   0 root         (0) root         (0)      389 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/field_translators/string_translator.cpp
--rw-r--r--   0 root         (0) root         (0)      761 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/field_translators/timestamp_translator.cpp
--rw-r--r--   0 root         (0) root         (0)     7166 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/make_description.cpp
--rw-r--r--   0 root         (0) root         (0)      972 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/make_field_translator.cpp
--rw-r--r--   0 root         (0) root         (0)     1820 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/parameter.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.405791 turbodbc-4.8.0/src/turbodbc/parameter_sets/
--rw-r--r--   0 root         (0) root         (0)     4834 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/parameter_sets/bound_parameter_set.cpp
--rw-r--r--   0 root         (0) root         (0)     2680 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/parameter_sets/field_parameter_set.cpp
--rw-r--r--   0 root         (0) root         (0)     3552 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/parameter_sets/set_field.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.405791 turbodbc-4.8.0/src/turbodbc/result_sets/
--rw-r--r--   0 root         (0) root         (0)     3054 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/result_sets/bound_result_set.cpp
--rw-r--r--   0 root         (0) root         (0)     2929 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/result_sets/double_buffered_result_set.cpp
--rw-r--r--   0 root         (0) root         (0)      856 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/result_sets/field_result_set.cpp
--rw-r--r--   0 root         (0) root         (0)      481 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/result_sets/result_set.cpp
--rw-r--r--   0 root         (0) root         (0)      985 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/result_sets/row_based_result_set.cpp
--rw-r--r--   0 root         (0) root         (0)      436 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/string_helpers.cpp
--rw-r--r--   0 root         (0) root         (0)     3200 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc/time_helpers.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.405791 turbodbc-4.8.0/src/turbodbc_arrow/
--rw-r--r--   0 root         (0) root         (0)    15431 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_arrow/arrow_result_set.cpp
--rw-r--r--   0 root         (0) root         (0)     1113 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_arrow/python_bindings.cpp
--rw-r--r--   0 root         (0) root         (0)    19064 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_arrow/set_arrow_parameters.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.409791 turbodbc-4.8.0/src/turbodbc_numpy/
--rw-r--r--   0 root         (0) root         (0)     1907 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_numpy/binary_column.cpp
--rw-r--r--   0 root         (0) root         (0)     2492 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_numpy/datetime_column.cpp
--rw-r--r--   0 root         (0) root         (0)     2304 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_numpy/make_numpy_array.cpp
--rw-r--r--   0 root         (0) root         (0)      431 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_numpy/masked_column.cpp
--rw-r--r--   0 root         (0) root         (0)     2434 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_numpy/numpy_result_set.cpp
--rw-r--r--   0 root         (0) root         (0)      327 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_numpy/numpy_type.cpp
--rw-r--r--   0 root         (0) root         (0)     1396 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_numpy/python_bindings.cpp
--rw-r--r--   0 root         (0) root         (0)    15127 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_numpy/set_numpy_parameters.cpp
--rw-r--r--   0 root         (0) root         (0)     1077 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_numpy/string_column.cpp
--rw-r--r--   0 root         (0) root         (0)     1092 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_numpy/unicode_column.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.409791 turbodbc-4.8.0/src/turbodbc_python/
--rw-r--r--   0 root         (0) root         (0)     4027 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_python/determine_parameter_type.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.413791 turbodbc-4.8.0/src/turbodbc_python/python_bindings/
--rw-r--r--   0 root         (0) root         (0)      675 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_python/python_bindings/buffer_size.cpp
--rw-r--r--   0 root         (0) root         (0)      505 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_python/python_bindings/column_info.cpp
--rw-r--r--   0 root         (0) root         (0)      259 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_python/python_bindings/connect.cpp
--rw-r--r--   0 root         (0) root         (0)      776 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_python/python_bindings/connection.cpp
--rw-r--r--   0 root         (0) root         (0)      757 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_python/python_bindings/cursor.cpp
--rw-r--r--   0 root         (0) root         (0)      340 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_python/python_bindings/error.cpp
--rw-r--r--   0 root         (0) root         (0)     1155 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_python/python_bindings/module.cpp
--rw-r--r--   0 root         (0) root         (0)     2786 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_python/python_bindings/options.cpp
--rw-r--r--   0 root         (0) root         (0)      568 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_python/python_bindings/python_parameter_set.cpp
--rw-r--r--   0 root         (0) root         (0)      913 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_python/python_bindings/python_result_set.cpp
--rw-r--r--   0 root         (0) root         (0)     3004 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_python/python_parameter_set.cpp
--rw-r--r--   0 root         (0) root         (0)     3469 2020-04-16 12:00:00.000000 turbodbc-4.8.0/src/turbodbc_python/python_result_set.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.417791 turbodbc-4.8.0/turbodbc/
--rw-r--r--   0 root         (0) root         (0)      826 2020-04-16 12:00:00.000000 turbodbc-4.8.0/turbodbc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      154 2020-04-16 12:00:00.000000 turbodbc-4.8.0/turbodbc/api_constants.py
--rw-r--r--   0 root         (0) root         (0)      247 2020-04-16 12:00:00.000000 turbodbc-4.8.0/turbodbc/arrow_support.py
--rw-r--r--   0 root         (0) root         (0)     1949 2020-04-16 12:00:00.000000 turbodbc-4.8.0/turbodbc/connect.py
--rw-r--r--   0 root         (0) root         (0)     1871 2020-04-16 12:00:00.000000 turbodbc-4.8.0/turbodbc/connection.py
--rw-r--r--   0 root         (0) root         (0)      286 2020-04-16 12:00:00.000000 turbodbc-4.8.0/turbodbc/constructors.py
--rw-r--r--   0 root         (0) root         (0)    15873 2020-04-16 12:00:00.000000 turbodbc-4.8.0/turbodbc/cursor.py
--rw-r--r--   0 root         (0) root         (0)      761 2020-04-16 12:00:00.000000 turbodbc-4.8.0/turbodbc/data_types.py
--rw-r--r--   0 root         (0) root         (0)      990 2020-04-16 12:00:00.000000 turbodbc-4.8.0/turbodbc/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     6269 2020-04-16 12:00:00.000000 turbodbc-4.8.0/turbodbc/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 09:12:08.421791 turbodbc-4.8.0/turbodbc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3579 2023-11-14 09:12:08.000000 turbodbc-4.8.0/turbodbc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7302 2023-11-14 09:12:08.000000 turbodbc-4.8.0/turbodbc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-14 09:12:08.000000 turbodbc-4.8.0/turbodbc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-11-14 09:12:08.000000 turbodbc-4.8.0/turbodbc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       83 2023-11-14 09:12:08.000000 turbodbc-4.8.0/turbodbc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.173557 turbodbc-4.9.0/
+-rw-r--r--   0 root         (0) root         (0)    20903 2020-04-16 12:00:00.000000 turbodbc-4.9.0/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)     1087 2020-04-16 12:00:00.000000 turbodbc-4.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       96 2020-04-16 12:00:00.000000 turbodbc-4.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-11-19 10:23:45.173557 turbodbc-4.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2523 2020-04-16 12:00:00.000000 turbodbc-4.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.121557 turbodbc-4.9.0/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.125557 turbodbc-4.9.0/include/cpp_odbc/
+-rw-r--r--   0 root         (0) root         (0)      957 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/column_description.h
+-rw-r--r--   0 root         (0) root         (0)     2554 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/connection.h
+-rw-r--r--   0 root         (0) root         (0)      893 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/cpp_odbc.h
+-rw-r--r--   0 root         (0) root         (0)      512 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/credentials.h
+-rw-r--r--   0 root         (0) root         (0)     1377 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/environment.h
+-rw-r--r--   0 root         (0) root         (0)      551 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/error.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.129557 turbodbc-4.9.0/include/cpp_odbc/level1/
+-rw-r--r--   0 root         (0) root         (0)    11658 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level1/api.h
+-rw-r--r--   0 root         (0) root         (0)      506 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level1/level1.h
+-rw-r--r--   0 root         (0) root         (0)     4792 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level1/unixodbc_backend.h
+-rw-r--r--   0 root         (0) root         (0)     4810 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level1/unixodbc_backend_debug.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.129557 turbodbc-4.9.0/include/cpp_odbc/level2/
+-rw-r--r--   0 root         (0) root         (0)    19100 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level2/api.h
+-rw-r--r--   0 root         (0) root         (0)      636 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level2/diagnostic_record.h
+-rw-r--r--   0 root         (0) root         (0)     1286 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level2/fixed_length_string_buffer.h
+-rw-r--r--   0 root         (0) root         (0)     2498 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level2/handles.h
+-rw-r--r--   0 root         (0) root         (0)      838 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level2/input_string_buffer.h
+-rw-r--r--   0 root         (0) root         (0)      855 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level2/input_u16string_buffer.h
+-rw-r--r--   0 root         (0) root         (0)     4565 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level2/level1_connector.h
+-rw-r--r--   0 root         (0) root         (0)      736 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level2/level2.h
+-rw-r--r--   0 root         (0) root         (0)     1435 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level2/string_buffer.h
+-rw-r--r--   0 root         (0) root         (0)     1513 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level2/u16string_buffer.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.129557 turbodbc-4.9.0/include/cpp_odbc/level3/
+-rw-r--r--   0 root         (0) root         (0)      588 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level3/level3.h
+-rw-r--r--   0 root         (0) root         (0)     1909 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level3/raii_connection.h
+-rw-r--r--   0 root         (0) root         (0)     1323 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level3/raii_environment.h
+-rw-r--r--   0 root         (0) root         (0)     2606 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/level3/raii_statement.h
+-rw-r--r--   0 root         (0) root         (0)      562 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/make_environment.h
+-rw-r--r--   0 root         (0) root         (0)     3045 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/multi_value_buffer.h
+-rw-r--r--   0 root         (0) root         (0)     7841 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/cpp_odbc/statement.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.137557 turbodbc-4.9.0/include/turbodbc/
+-rw-r--r--   0 root         (0) root         (0)     1443 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/buffer_size.h
+-rw-r--r--   0 root         (0) root         (0)     1241 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/column.h
+-rw-r--r--   0 root         (0) root         (0)      217 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/column_info.h
+-rw-r--r--   0 root         (0) root         (0)     1602 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/command.h
+-rw-r--r--   0 root         (0) root         (0)      842 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/configuration.h
+-rw-r--r--   0 root         (0) root         (0)      486 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/connect.h
+-rw-r--r--   0 root         (0) root         (0)     1427 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/connection.h
+-rw-r--r--   0 root         (0) root         (0)     1093 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/cursor.h
+-rw-r--r--   0 root         (0) root         (0)     1640 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/description.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.137557 turbodbc-4.9.0/include/turbodbc/descriptions/
+-rw-r--r--   0 root         (0) root         (0)      552 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/descriptions/boolean_description.h
+-rw-r--r--   0 root         (0) root         (0)      537 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/descriptions/date_description.h
+-rw-r--r--   0 root         (0) root         (0)      615 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/descriptions/floating_point_description.h
+-rw-r--r--   0 root         (0) root         (0)      552 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/descriptions/integer_description.h
+-rw-r--r--   0 root         (0) root         (0)      693 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/descriptions/string_description.h
+-rw-r--r--   0 root         (0) root         (0)      562 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/descriptions/timestamp_description.h
+-rw-r--r--   0 root         (0) root         (0)      698 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/descriptions/unicode_description.h
+-rw-r--r--   0 root         (0) root         (0)      404 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/descriptions.h
+-rw-r--r--   0 root         (0) root         (0)      230 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/errors.h
+-rw-r--r--   0 root         (0) root         (0)      746 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/field.h
+-rw-r--r--   0 root         (0) root         (0)      711 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/field_translator.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.141557 turbodbc-4.9.0/include/turbodbc/field_translators/
+-rw-r--r--   0 root         (0) root         (0)      372 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/field_translators/boolean_translator.h
+-rw-r--r--   0 root         (0) root         (0)      354 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/field_translators/date_translator.h
+-rw-r--r--   0 root         (0) root         (0)      386 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/field_translators/float64_translator.h
+-rw-r--r--   0 root         (0) root         (0)      373 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/field_translators/int64_translator.h
+-rw-r--r--   0 root         (0) root         (0)      368 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/field_translators/string_translator.h
+-rw-r--r--   0 root         (0) root         (0)      374 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/field_translators/timestamp_translator.h
+-rw-r--r--   0 root         (0) root         (0)      364 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/field_translators.h
+-rw-r--r--   0 root         (0) root         (0)     1019 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/make_description.h
+-rw-r--r--   0 root         (0) root         (0)      316 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/make_field_translator.h
+-rw-r--r--   0 root         (0) root         (0)     1761 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/parameter.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.141557 turbodbc-4.9.0/include/turbodbc/parameter_sets/
+-rw-r--r--   0 root         (0) root         (0)     2469 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/parameter_sets/bound_parameter_set.h
+-rw-r--r--   0 root         (0) root         (0)      745 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/parameter_sets/field_parameter_set.h
+-rw-r--r--   0 root         (0) root         (0)      704 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/parameter_sets/set_field.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.141557 turbodbc-4.9.0/include/turbodbc/result_sets/
+-rw-r--r--   0 root         (0) root         (0)     1254 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/result_sets/bound_result_set.h
+-rw-r--r--   0 root         (0) root         (0)     2327 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/result_sets/double_buffered_result_set.h
+-rw-r--r--   0 root         (0) root         (0)      971 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/result_sets/field_result_set.h
+-rw-r--r--   0 root         (0) root         (0)     1256 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/result_sets/result_set.h
+-rw-r--r--   0 root         (0) root         (0)     1028 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/result_sets/row_based_result_set.h
+-rw-r--r--   0 root         (0) root         (0)      157 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/string_helpers.h
+-rw-r--r--   0 root         (0) root         (0)     1190 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/time_helpers.h
+-rw-r--r--   0 root         (0) root         (0)      459 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc/type_code.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.141557 turbodbc-4.9.0/include/turbodbc_arrow/
+-rw-r--r--   0 root         (0) root         (0)     1674 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc_arrow/arrow_result_set.h
+-rw-r--r--   0 root         (0) root         (0)      297 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc_arrow/set_arrow_parameters.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.145557 turbodbc-4.9.0/include/turbodbc_numpy/
+-rw-r--r--   0 root         (0) root         (0)      556 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc_numpy/binary_column.h
+-rw-r--r--   0 root         (0) root         (0)      683 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc_numpy/datetime_column.h
+-rw-r--r--   0 root         (0) root         (0)      378 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc_numpy/make_numpy_array.h
+-rw-r--r--   0 root         (0) root         (0)      698 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc_numpy/masked_column.h
+-rw-r--r--   0 root         (0) root         (0)      459 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc_numpy/ndarrayobject.h
+-rw-r--r--   0 root         (0) root         (0)      756 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc_numpy/numpy_result_set.h
+-rw-r--r--   0 root         (0) root         (0)      260 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc_numpy/numpy_type.h
+-rw-r--r--   0 root         (0) root         (0)      299 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc_numpy/set_numpy_parameters.h
+-rw-r--r--   0 root         (0) root         (0)      508 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc_numpy/string_column.h
+-rw-r--r--   0 root         (0) root         (0)      511 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc_numpy/unicode_column.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.145557 turbodbc-4.9.0/include/turbodbc_python/
+-rw-r--r--   0 root         (0) root         (0)      454 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc_python/determine_parameter_type.h
+-rw-r--r--   0 root         (0) root         (0)      685 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc_python/python_parameter_set.h
+-rw-r--r--   0 root         (0) root         (0)      885 2020-04-16 12:00:00.000000 turbodbc-4.9.0/include/turbodbc_python/python_result_set.h
+-rw-r--r--   0 root         (0) root         (0)      682 2020-04-16 12:00:00.000000 turbodbc-4.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      155 2023-11-19 10:23:45.173557 turbodbc-4.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    10193 2020-04-16 12:00:00.000000 turbodbc-4.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.121557 turbodbc-4.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.145557 turbodbc-4.9.0/src/cpp_odbc/
+-rw-r--r--   0 root         (0) root         (0)     2694 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/column_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      802 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/connection.cpp
+-rw-r--r--   0 root         (0) root         (0)      190 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/cpp_odbc.cpp
+-rw-r--r--   0 root         (0) root         (0)      411 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/environment.cpp
+-rw-r--r--   0 root         (0) root         (0)      744 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/error.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.149557 turbodbc-4.9.0/src/cpp_odbc/level1/
+-rw-r--r--   0 root         (0) root         (0)     7405 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level1/api.cpp
+-rw-r--r--   0 root         (0) root         (0)      193 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level1/level1.cpp
+-rw-r--r--   0 root         (0) root         (0)     7663 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level1/unixodbc_backend.cpp
+-rw-r--r--   0 root         (0) root         (0)    12404 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level1/unixodbc_backend_debug.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.149557 turbodbc-4.9.0/src/cpp_odbc/level2/
+-rw-r--r--   0 root         (0) root         (0)     5853 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level2/api.cpp
+-rw-r--r--   0 root         (0) root         (0)     1265 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level2/handles.cpp
+-rw-r--r--   0 root         (0) root         (0)      419 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level2/input_string_buffer.cpp
+-rw-r--r--   0 root         (0) root         (0)      457 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level2/input_u16string_buffer.cpp
+-rw-r--r--   0 root         (0) root         (0)    16753 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level2/level1_connector.cpp
+-rw-r--r--   0 root         (0) root         (0)      193 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level2/level2.cpp
+-rw-r--r--   0 root         (0) root         (0)      595 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level2/string_buffer.cpp
+-rw-r--r--   0 root         (0) root         (0)      621 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level2/u16string_buffer.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.149557 turbodbc-4.9.0/src/cpp_odbc/level3/
+-rw-r--r--   0 root         (0) root         (0)      193 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level3/level3.cpp
+-rw-r--r--   0 root         (0) root         (0)     3649 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level3/raii_connection.cpp
+-rw-r--r--   0 root         (0) root         (0)     1623 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level3/raii_environment.cpp
+-rw-r--r--   0 root         (0) root         (0)     3845 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/level3/raii_statement.cpp
+-rw-r--r--   0 root         (0) root         (0)      949 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/make_environment.cpp
+-rw-r--r--   0 root         (0) root         (0)     1816 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/multi_value_buffer.cpp
+-rw-r--r--   0 root         (0) root         (0)     2787 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/cpp_odbc/statement.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.153557 turbodbc-4.9.0/src/turbodbc/
+-rw-r--r--   0 root         (0) root         (0)     1218 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/buffer_size.cpp
+-rw-r--r--   0 root         (0) root         (0)      963 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/column.cpp
+-rw-r--r--   0 root         (0) root         (0)     1805 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/command.cpp
+-rw-r--r--   0 root         (0) root         (0)      901 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/configuration.cpp
+-rw-r--r--   0 root         (0) root         (0)      298 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/connect.cpp
+-rw-r--r--   0 root         (0) root         (0)     1136 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/connection.cpp
+-rw-r--r--   0 root         (0) root         (0)     1941 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/cursor.cpp
+-rw-r--r--   0 root         (0) root         (0)      830 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/description.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.157557 turbodbc-4.9.0/src/turbodbc/descriptions/
+-rw-r--r--   0 root         (0) root         (0)      783 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/descriptions/boolean_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      784 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/descriptions/date_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      899 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/descriptions/floating_point_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      810 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/descriptions/integer_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      915 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/descriptions/string_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      864 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/descriptions/timestamp_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      993 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/descriptions/unicode_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      211 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/errors.cpp
+-rw-r--r--   0 root         (0) root         (0)      393 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/field_translator.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.157557 turbodbc-4.9.0/src/turbodbc/field_translators/
+-rw-r--r--   0 root         (0) root         (0)      380 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/field_translators/boolean_translator.cpp
+-rw-r--r--   0 root         (0) root         (0)      483 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/field_translators/date_translator.cpp
+-rw-r--r--   0 root         (0) root         (0)      414 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/field_translators/float64_translator.cpp
+-rw-r--r--   0 root         (0) root         (0)      403 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/field_translators/int64_translator.cpp
+-rw-r--r--   0 root         (0) root         (0)      389 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/field_translators/string_translator.cpp
+-rw-r--r--   0 root         (0) root         (0)      761 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/field_translators/timestamp_translator.cpp
+-rw-r--r--   0 root         (0) root         (0)     7166 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/make_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      972 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/make_field_translator.cpp
+-rw-r--r--   0 root         (0) root         (0)     1820 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/parameter.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.157557 turbodbc-4.9.0/src/turbodbc/parameter_sets/
+-rw-r--r--   0 root         (0) root         (0)     4834 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/parameter_sets/bound_parameter_set.cpp
+-rw-r--r--   0 root         (0) root         (0)     2680 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/parameter_sets/field_parameter_set.cpp
+-rw-r--r--   0 root         (0) root         (0)     3552 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/parameter_sets/set_field.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.161557 turbodbc-4.9.0/src/turbodbc/result_sets/
+-rw-r--r--   0 root         (0) root         (0)     3054 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/result_sets/bound_result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)     2929 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/result_sets/double_buffered_result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)      856 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/result_sets/field_result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)      481 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/result_sets/result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)      985 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/result_sets/row_based_result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)      436 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/string_helpers.cpp
+-rw-r--r--   0 root         (0) root         (0)     3200 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc/time_helpers.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.161557 turbodbc-4.9.0/src/turbodbc_arrow/
+-rw-r--r--   0 root         (0) root         (0)    15431 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_arrow/arrow_result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)     1113 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_arrow/python_bindings.cpp
+-rw-r--r--   0 root         (0) root         (0)    19064 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_arrow/set_arrow_parameters.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.165557 turbodbc-4.9.0/src/turbodbc_numpy/
+-rw-r--r--   0 root         (0) root         (0)     1907 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_numpy/binary_column.cpp
+-rw-r--r--   0 root         (0) root         (0)     2492 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_numpy/datetime_column.cpp
+-rw-r--r--   0 root         (0) root         (0)     2304 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_numpy/make_numpy_array.cpp
+-rw-r--r--   0 root         (0) root         (0)      431 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_numpy/masked_column.cpp
+-rw-r--r--   0 root         (0) root         (0)     2434 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_numpy/numpy_result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)      327 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_numpy/numpy_type.cpp
+-rw-r--r--   0 root         (0) root         (0)     1396 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_numpy/python_bindings.cpp
+-rw-r--r--   0 root         (0) root         (0)    15127 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_numpy/set_numpy_parameters.cpp
+-rw-r--r--   0 root         (0) root         (0)     1077 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_numpy/string_column.cpp
+-rw-r--r--   0 root         (0) root         (0)     1092 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_numpy/unicode_column.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.165557 turbodbc-4.9.0/src/turbodbc_python/
+-rw-r--r--   0 root         (0) root         (0)     4027 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_python/determine_parameter_type.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.165557 turbodbc-4.9.0/src/turbodbc_python/python_bindings/
+-rw-r--r--   0 root         (0) root         (0)      675 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_python/python_bindings/buffer_size.cpp
+-rw-r--r--   0 root         (0) root         (0)      505 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_python/python_bindings/column_info.cpp
+-rw-r--r--   0 root         (0) root         (0)      259 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_python/python_bindings/connect.cpp
+-rw-r--r--   0 root         (0) root         (0)      776 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_python/python_bindings/connection.cpp
+-rw-r--r--   0 root         (0) root         (0)      757 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_python/python_bindings/cursor.cpp
+-rw-r--r--   0 root         (0) root         (0)      340 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_python/python_bindings/error.cpp
+-rw-r--r--   0 root         (0) root         (0)     1155 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_python/python_bindings/module.cpp
+-rw-r--r--   0 root         (0) root         (0)     2786 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_python/python_bindings/options.cpp
+-rw-r--r--   0 root         (0) root         (0)      568 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_python/python_bindings/python_parameter_set.cpp
+-rw-r--r--   0 root         (0) root         (0)      913 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_python/python_bindings/python_result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)     3004 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_python/python_parameter_set.cpp
+-rw-r--r--   0 root         (0) root         (0)     3469 2020-04-16 12:00:00.000000 turbodbc-4.9.0/src/turbodbc_python/python_result_set.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.169557 turbodbc-4.9.0/turbodbc/
+-rw-r--r--   0 root         (0) root         (0)      826 2020-04-16 12:00:00.000000 turbodbc-4.9.0/turbodbc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      154 2020-04-16 12:00:00.000000 turbodbc-4.9.0/turbodbc/api_constants.py
+-rw-r--r--   0 root         (0) root         (0)      247 2020-04-16 12:00:00.000000 turbodbc-4.9.0/turbodbc/arrow_support.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2020-04-16 12:00:00.000000 turbodbc-4.9.0/turbodbc/connect.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2020-04-16 12:00:00.000000 turbodbc-4.9.0/turbodbc/connection.py
+-rw-r--r--   0 root         (0) root         (0)      286 2020-04-16 12:00:00.000000 turbodbc-4.9.0/turbodbc/constructors.py
+-rw-r--r--   0 root         (0) root         (0)    15873 2020-04-16 12:00:00.000000 turbodbc-4.9.0/turbodbc/cursor.py
+-rw-r--r--   0 root         (0) root         (0)      761 2020-04-16 12:00:00.000000 turbodbc-4.9.0/turbodbc/data_types.py
+-rw-r--r--   0 root         (0) root         (0)      990 2020-04-16 12:00:00.000000 turbodbc-4.9.0/turbodbc/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     6269 2020-04-16 12:00:00.000000 turbodbc-4.9.0/turbodbc/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-19 10:23:45.169557 turbodbc-4.9.0/turbodbc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-11-19 10:23:45.000000 turbodbc-4.9.0/turbodbc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7317 2023-11-19 10:23:45.000000 turbodbc-4.9.0/turbodbc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-11-19 10:23:45.000000 turbodbc-4.9.0/turbodbc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-11-19 10:23:45.000000 turbodbc-4.9.0/turbodbc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-11-19 10:23:45.000000 turbodbc-4.9.0/turbodbc.egg-info/top_level.txt
```

### Comparing `turbodbc-4.8.0/CHANGELOG.rst` & `turbodbc-4.9.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Version history / changelog
 ===========================
 
 From version 2.0.0, turbodbc adapts semantic versioning.
 
+Version 4.9.0
+-------------
+
+* Fix pip wheel missing pyproject.toml - support pep517
+
 Version 4.8.0
 -------------
 
 * Support ``pyarrow=14``
 
-
 Version 4.7.0
 -------------
 
 * Support ``pyarrow=13``
 
 Version 4.6.0
 --------------
```

### Comparing `turbodbc-4.8.0/LICENSE` & `turbodbc-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/PKG-INFO` & `turbodbc-4.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbodbc
-Version: 4.8.0
+Version: 4.9.0
 Summary: turbodbc is a Python DB API 2.0 compatible ODBC driver
 Home-page: https://github.com/blue-yonder/turbodbc
 Author: Michael Koenig
 Author-email: michael.koenig@blue-yonder.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `turbodbc-4.8.0/README.md` & `turbodbc-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/column_description.h` & `turbodbc-4.9.0/include/cpp_odbc/column_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/connection.h` & `turbodbc-4.9.0/include/cpp_odbc/connection.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/cpp_odbc.h` & `turbodbc-4.9.0/include/cpp_odbc/cpp_odbc.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/credentials.h` & `turbodbc-4.9.0/include/cpp_odbc/credentials.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/environment.h` & `turbodbc-4.9.0/include/cpp_odbc/environment.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/error.h` & `turbodbc-4.9.0/include/cpp_odbc/error.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level1/api.h` & `turbodbc-4.9.0/include/cpp_odbc/level1/api.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level1/unixodbc_backend.h` & `turbodbc-4.9.0/include/cpp_odbc/level1/unixodbc_backend.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level1/unixodbc_backend_debug.h` & `turbodbc-4.9.0/include/cpp_odbc/level1/unixodbc_backend_debug.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level2/api.h` & `turbodbc-4.9.0/include/cpp_odbc/level2/api.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level2/diagnostic_record.h` & `turbodbc-4.9.0/include/cpp_odbc/level2/diagnostic_record.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level2/fixed_length_string_buffer.h` & `turbodbc-4.9.0/include/cpp_odbc/level2/fixed_length_string_buffer.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level2/handles.h` & `turbodbc-4.9.0/include/cpp_odbc/level2/handles.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level2/input_string_buffer.h` & `turbodbc-4.9.0/include/cpp_odbc/level2/input_string_buffer.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level2/input_u16string_buffer.h` & `turbodbc-4.9.0/include/cpp_odbc/level2/input_u16string_buffer.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level2/level1_connector.h` & `turbodbc-4.9.0/include/cpp_odbc/level2/level1_connector.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level2/level2.h` & `turbodbc-4.9.0/include/cpp_odbc/level2/level2.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level2/string_buffer.h` & `turbodbc-4.9.0/include/cpp_odbc/level2/string_buffer.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level2/u16string_buffer.h` & `turbodbc-4.9.0/include/cpp_odbc/level2/u16string_buffer.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level3/level3.h` & `turbodbc-4.9.0/include/cpp_odbc/level3/level3.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level3/raii_connection.h` & `turbodbc-4.9.0/include/cpp_odbc/level3/raii_connection.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level3/raii_environment.h` & `turbodbc-4.9.0/include/cpp_odbc/level3/raii_environment.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/level3/raii_statement.h` & `turbodbc-4.9.0/include/cpp_odbc/level3/raii_statement.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/make_environment.h` & `turbodbc-4.9.0/include/cpp_odbc/make_environment.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/multi_value_buffer.h` & `turbodbc-4.9.0/include/cpp_odbc/multi_value_buffer.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/cpp_odbc/statement.h` & `turbodbc-4.9.0/include/cpp_odbc/statement.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/buffer_size.h` & `turbodbc-4.9.0/include/turbodbc/buffer_size.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/column.h` & `turbodbc-4.9.0/include/turbodbc/column.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/command.h` & `turbodbc-4.9.0/include/turbodbc/command.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/configuration.h` & `turbodbc-4.9.0/include/turbodbc/configuration.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/connection.h` & `turbodbc-4.9.0/include/turbodbc/connection.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/cursor.h` & `turbodbc-4.9.0/include/turbodbc/cursor.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/description.h` & `turbodbc-4.9.0/include/turbodbc/description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/descriptions/boolean_description.h` & `turbodbc-4.9.0/include/turbodbc/descriptions/boolean_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/descriptions/date_description.h` & `turbodbc-4.9.0/include/turbodbc/descriptions/date_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/descriptions/floating_point_description.h` & `turbodbc-4.9.0/include/turbodbc/descriptions/floating_point_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/descriptions/integer_description.h` & `turbodbc-4.9.0/include/turbodbc/descriptions/integer_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/descriptions/string_description.h` & `turbodbc-4.9.0/include/turbodbc/descriptions/string_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/descriptions/timestamp_description.h` & `turbodbc-4.9.0/include/turbodbc/descriptions/timestamp_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/descriptions/unicode_description.h` & `turbodbc-4.9.0/include/turbodbc/descriptions/unicode_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/field.h` & `turbodbc-4.9.0/include/turbodbc/field.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/field_translator.h` & `turbodbc-4.9.0/include/turbodbc/field_translator.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/make_description.h` & `turbodbc-4.9.0/include/turbodbc/make_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/parameter.h` & `turbodbc-4.9.0/include/turbodbc/parameter.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/parameter_sets/bound_parameter_set.h` & `turbodbc-4.9.0/include/turbodbc/parameter_sets/bound_parameter_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/parameter_sets/field_parameter_set.h` & `turbodbc-4.9.0/include/turbodbc/parameter_sets/field_parameter_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/parameter_sets/set_field.h` & `turbodbc-4.9.0/include/turbodbc/parameter_sets/set_field.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/result_sets/bound_result_set.h` & `turbodbc-4.9.0/include/turbodbc/result_sets/bound_result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/result_sets/double_buffered_result_set.h` & `turbodbc-4.9.0/include/turbodbc/result_sets/double_buffered_result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/result_sets/field_result_set.h` & `turbodbc-4.9.0/include/turbodbc/result_sets/field_result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/result_sets/result_set.h` & `turbodbc-4.9.0/include/turbodbc/result_sets/result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/result_sets/row_based_result_set.h` & `turbodbc-4.9.0/include/turbodbc/result_sets/row_based_result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc/time_helpers.h` & `turbodbc-4.9.0/include/turbodbc/time_helpers.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc_arrow/arrow_result_set.h` & `turbodbc-4.9.0/include/turbodbc_arrow/arrow_result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc_numpy/binary_column.h` & `turbodbc-4.9.0/include/turbodbc_numpy/binary_column.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc_numpy/datetime_column.h` & `turbodbc-4.9.0/include/turbodbc_numpy/datetime_column.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc_numpy/masked_column.h` & `turbodbc-4.9.0/include/turbodbc_numpy/masked_column.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc_numpy/numpy_result_set.h` & `turbodbc-4.9.0/include/turbodbc_numpy/numpy_result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc_python/python_parameter_set.h` & `turbodbc-4.9.0/include/turbodbc_python/python_parameter_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/include/turbodbc_python/python_result_set.h` & `turbodbc-4.9.0/include/turbodbc_python/python_result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/setup.py` & `turbodbc-4.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="turbodbc",
-    version="4.8.0",
+    version="4.9.0",
     description="turbodbc is a Python DB API 2.0 compatible ODBC driver",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/blue-yonder/turbodbc",
     author="Michael Koenig",
     author_email="michael.koenig@blue-yonder.com",
```

### Comparing `turbodbc-4.8.0/src/cpp_odbc/column_description.cpp` & `turbodbc-4.9.0/src/cpp_odbc/column_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/connection.cpp` & `turbodbc-4.9.0/src/cpp_odbc/connection.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/error.cpp` & `turbodbc-4.9.0/src/cpp_odbc/error.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/level1/api.cpp` & `turbodbc-4.9.0/src/cpp_odbc/level1/api.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/level1/unixodbc_backend.cpp` & `turbodbc-4.9.0/src/cpp_odbc/level1/unixodbc_backend.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/level1/unixodbc_backend_debug.cpp` & `turbodbc-4.9.0/src/cpp_odbc/level1/unixodbc_backend_debug.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/level2/api.cpp` & `turbodbc-4.9.0/src/cpp_odbc/level2/api.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/level2/handles.cpp` & `turbodbc-4.9.0/src/cpp_odbc/level2/handles.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/level2/level1_connector.cpp` & `turbodbc-4.9.0/src/cpp_odbc/level2/level1_connector.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/level2/string_buffer.cpp` & `turbodbc-4.9.0/src/cpp_odbc/level2/string_buffer.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/level2/u16string_buffer.cpp` & `turbodbc-4.9.0/src/cpp_odbc/level2/u16string_buffer.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/level3/raii_connection.cpp` & `turbodbc-4.9.0/src/cpp_odbc/level3/raii_connection.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/level3/raii_environment.cpp` & `turbodbc-4.9.0/src/cpp_odbc/level3/raii_environment.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/level3/raii_statement.cpp` & `turbodbc-4.9.0/src/cpp_odbc/level3/raii_statement.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/make_environment.cpp` & `turbodbc-4.9.0/src/cpp_odbc/make_environment.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/multi_value_buffer.cpp` & `turbodbc-4.9.0/src/cpp_odbc/multi_value_buffer.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/cpp_odbc/statement.cpp` & `turbodbc-4.9.0/src/cpp_odbc/statement.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/buffer_size.cpp` & `turbodbc-4.9.0/src/turbodbc/buffer_size.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/column.cpp` & `turbodbc-4.9.0/src/turbodbc/column.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/command.cpp` & `turbodbc-4.9.0/src/turbodbc/command.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/configuration.cpp` & `turbodbc-4.9.0/src/turbodbc/configuration.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/connection.cpp` & `turbodbc-4.9.0/src/turbodbc/connection.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/cursor.cpp` & `turbodbc-4.9.0/src/turbodbc/cursor.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/description.cpp` & `turbodbc-4.9.0/src/turbodbc/description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/descriptions/boolean_description.cpp` & `turbodbc-4.9.0/src/turbodbc/descriptions/boolean_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/descriptions/date_description.cpp` & `turbodbc-4.9.0/src/turbodbc/descriptions/date_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/descriptions/floating_point_description.cpp` & `turbodbc-4.9.0/src/turbodbc/descriptions/floating_point_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/descriptions/integer_description.cpp` & `turbodbc-4.9.0/src/turbodbc/descriptions/integer_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/descriptions/string_description.cpp` & `turbodbc-4.9.0/src/turbodbc/descriptions/string_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/descriptions/timestamp_description.cpp` & `turbodbc-4.9.0/src/turbodbc/descriptions/timestamp_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/descriptions/unicode_description.cpp` & `turbodbc-4.9.0/src/turbodbc/descriptions/unicode_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/field_translators/timestamp_translator.cpp` & `turbodbc-4.9.0/src/turbodbc/field_translators/timestamp_translator.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/make_description.cpp` & `turbodbc-4.9.0/src/turbodbc/make_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/make_field_translator.cpp` & `turbodbc-4.9.0/src/turbodbc/make_field_translator.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/parameter.cpp` & `turbodbc-4.9.0/src/turbodbc/parameter.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/parameter_sets/bound_parameter_set.cpp` & `turbodbc-4.9.0/src/turbodbc/parameter_sets/bound_parameter_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/parameter_sets/field_parameter_set.cpp` & `turbodbc-4.9.0/src/turbodbc/parameter_sets/field_parameter_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/parameter_sets/set_field.cpp` & `turbodbc-4.9.0/src/turbodbc/parameter_sets/set_field.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/result_sets/bound_result_set.cpp` & `turbodbc-4.9.0/src/turbodbc/result_sets/bound_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/result_sets/double_buffered_result_set.cpp` & `turbodbc-4.9.0/src/turbodbc/result_sets/double_buffered_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/result_sets/field_result_set.cpp` & `turbodbc-4.9.0/src/turbodbc/result_sets/field_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/result_sets/row_based_result_set.cpp` & `turbodbc-4.9.0/src/turbodbc/result_sets/row_based_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc/time_helpers.cpp` & `turbodbc-4.9.0/src/turbodbc/time_helpers.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_arrow/arrow_result_set.cpp` & `turbodbc-4.9.0/src/turbodbc_arrow/arrow_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_arrow/python_bindings.cpp` & `turbodbc-4.9.0/src/turbodbc_arrow/python_bindings.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_arrow/set_arrow_parameters.cpp` & `turbodbc-4.9.0/src/turbodbc_arrow/set_arrow_parameters.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_numpy/binary_column.cpp` & `turbodbc-4.9.0/src/turbodbc_numpy/binary_column.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_numpy/datetime_column.cpp` & `turbodbc-4.9.0/src/turbodbc_numpy/datetime_column.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_numpy/make_numpy_array.cpp` & `turbodbc-4.9.0/src/turbodbc_numpy/make_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_numpy/numpy_result_set.cpp` & `turbodbc-4.9.0/src/turbodbc_numpy/numpy_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_numpy/python_bindings.cpp` & `turbodbc-4.9.0/src/turbodbc_numpy/python_bindings.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_numpy/set_numpy_parameters.cpp` & `turbodbc-4.9.0/src/turbodbc_numpy/set_numpy_parameters.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_numpy/string_column.cpp` & `turbodbc-4.9.0/src/turbodbc_numpy/string_column.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_numpy/unicode_column.cpp` & `turbodbc-4.9.0/src/turbodbc_numpy/unicode_column.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_python/determine_parameter_type.cpp` & `turbodbc-4.9.0/src/turbodbc_python/determine_parameter_type.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_python/python_bindings/buffer_size.cpp` & `turbodbc-4.9.0/src/turbodbc_python/python_bindings/buffer_size.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_python/python_bindings/connection.cpp` & `turbodbc-4.9.0/src/turbodbc_python/python_bindings/connection.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_python/python_bindings/cursor.cpp` & `turbodbc-4.9.0/src/turbodbc_python/python_bindings/cursor.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_python/python_bindings/module.cpp` & `turbodbc-4.9.0/src/turbodbc_python/python_bindings/module.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_python/python_bindings/options.cpp` & `turbodbc-4.9.0/src/turbodbc_python/python_bindings/options.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_python/python_bindings/python_parameter_set.cpp` & `turbodbc-4.9.0/src/turbodbc_python/python_bindings/python_parameter_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_python/python_bindings/python_result_set.cpp` & `turbodbc-4.9.0/src/turbodbc_python/python_bindings/python_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_python/python_parameter_set.cpp` & `turbodbc-4.9.0/src/turbodbc_python/python_parameter_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/src/turbodbc_python/python_result_set.cpp` & `turbodbc-4.9.0/src/turbodbc_python/python_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/turbodbc/__init__.py` & `turbodbc-4.9.0/turbodbc/__init__.py`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/turbodbc/connect.py` & `turbodbc-4.9.0/turbodbc/connect.py`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/turbodbc/connection.py` & `turbodbc-4.9.0/turbodbc/connection.py`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/turbodbc/cursor.py` & `turbodbc-4.9.0/turbodbc/cursor.py`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/turbodbc/data_types.py` & `turbodbc-4.9.0/turbodbc/data_types.py`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/turbodbc/exceptions.py` & `turbodbc-4.9.0/turbodbc/exceptions.py`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/turbodbc/options.py` & `turbodbc-4.9.0/turbodbc/options.py`

 * *Files identical despite different names*

### Comparing `turbodbc-4.8.0/turbodbc.egg-info/PKG-INFO` & `turbodbc-4.9.0/turbodbc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbodbc
-Version: 4.8.0
+Version: 4.9.0
 Summary: turbodbc is a Python DB API 2.0 compatible ODBC driver
 Home-page: https://github.com/blue-yonder/turbodbc
 Author: Michael Koenig
 Author-email: michael.koenig@blue-yonder.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `turbodbc-4.8.0/turbodbc.egg-info/SOURCES.txt` & `turbodbc-4.9.0/turbodbc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 include/cpp_odbc/column_description.h
 include/cpp_odbc/connection.h
 include/cpp_odbc/cpp_odbc.h
 include/cpp_odbc/credentials.h
 include/cpp_odbc/environment.h
```

