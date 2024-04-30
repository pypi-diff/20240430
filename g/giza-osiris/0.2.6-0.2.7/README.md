# Comparing `tmp/giza_osiris-0.2.6.tar.gz` & `tmp/giza_osiris-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giza_osiris-0.2.6.tar", max compression
+gzip compressed data, was "giza_osiris-0.2.7.tar", max compression
```

## Comparing `giza_osiris-0.2.6.tar` & `giza_osiris-0.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1074 2024-03-19 16:05:10.114800 giza_osiris-0.2.6/LICENSE
--rw-r--r--   0        0        0     1657 2024-03-19 16:05:10.114800 giza_osiris-0.2.6/README.md
--rw-r--r--   0        0        0        0 2024-03-19 16:05:10.118800 giza_osiris-0.2.6/osiris/__init__.py
--rw-r--r--   0        0        0     4253 2024-03-19 16:05:10.118800 giza_osiris-0.2.6/osiris/app.py
--rw-r--r--   0        0        0     1434 2024-03-19 16:05:10.118800 giza_osiris-0.2.6/osiris/cairo/data_converter/data_converter.py
--rw-r--r--   0        0        0     2653 2024-03-19 16:05:10.118800 giza_osiris-0.2.6/osiris/cairo/data_converter/data_statement_generator.py
--rw-r--r--   0        0        0     1773 2024-03-19 16:05:10.118800 giza_osiris-0.2.6/osiris/cairo/data_converter/tensor_creator.py
--rw-r--r--   0        0        0     3334 2024-03-19 16:05:10.118800 giza_osiris-0.2.6/osiris/cairo/file_manager/cairo_data.py
--rw-r--r--   0        0        0     2087 2024-03-19 16:05:10.118800 giza_osiris-0.2.6/osiris/cairo/file_manager/file.py
--rw-r--r--   0        0        0      948 2024-03-19 16:05:10.118800 giza_osiris-0.2.6/osiris/cairo/serde/data_structures.py
--rw-r--r--   0        0        0     4440 2024-03-19 16:05:10.118800 giza_osiris-0.2.6/osiris/cairo/serde/deserialize.py
--rw-r--r--   0        0        0      809 2024-03-19 16:05:10.118800 giza_osiris-0.2.6/osiris/cairo/serde/serialize.py
--rw-r--r--   0        0        0     1035 2024-03-19 16:05:10.118800 giza_osiris-0.2.6/osiris/cairo/serde/utils.py
--rw-r--r--   0        0        0      177 2024-03-19 16:05:10.118800 giza_osiris-0.2.6/osiris/dtypes/cairo_dtypes.py
--rw-r--r--   0        0        0      117 2024-03-19 16:05:10.118800 giza_osiris-0.2.6/osiris/dtypes/cairo_impls.py
--rw-r--r--   0        0        0      177 2024-03-19 16:05:10.118800 giza_osiris-0.2.6/osiris/dtypes/input_output_formats.py
--rw-r--r--   0        0        0     1290 2024-03-19 16:05:10.118800 giza_osiris-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 giza_osiris-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-30 16:57:38.515500 giza_osiris-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1657 2024-04-30 16:57:38.515500 giza_osiris-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/__init__.py
+-rw-r--r--   0        0        0     4777 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/app.py
+-rw-r--r--   0        0        0     1434 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/data_converter/data_converter.py
+-rw-r--r--   0        0        0     2653 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/data_converter/data_statement_generator.py
+-rw-r--r--   0        0        0     1773 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/data_converter/tensor_creator.py
+-rw-r--r--   0        0        0     3334 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/file_manager/cairo_data.py
+-rw-r--r--   0        0        0     2087 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/file_manager/file.py
+-rw-r--r--   0        0        0      948 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/serde/data_structures.py
+-rw-r--r--   0        0        0     4689 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/serde/deserialize.py
+-rw-r--r--   0        0        0      809 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/serde/serialize.py
+-rw-r--r--   0        0        0     1035 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/serde/utils.py
+-rw-r--r--   0        0        0      177 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/dtypes/cairo_dtypes.py
+-rw-r--r--   0        0        0      117 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/dtypes/cairo_impls.py
+-rw-r--r--   0        0        0      177 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/dtypes/input_output_formats.py
+-rw-r--r--   0        0        0     1290 2024-04-30 16:57:38.523500 giza_osiris-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 giza_osiris-0.2.7/PKG-INFO
```

### Comparing `giza_osiris-0.2.6/LICENSE` & `giza_osiris-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.6/README.md` & `giza_osiris-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.6/osiris/app.py` & `giza_osiris-0.2.7/osiris/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from osiris.cairo.serde.deserialize import deserializer
 from osiris.cairo.serde.serialize import serializer
 from osiris.dtypes.cairo_dtypes import Dtype
 from osiris.dtypes.input_output_formats import InputFormat, OutputFormat
 
 app = typer.Typer()
 
+
 def check_file_format(file_path):
     _, file_extension = os.path.splitext(file_path)
 
     if file_extension == '.csv':
         return InputFormat.CSV
     elif file_extension == '.parquet':
         return InputFormat.PARQUET
@@ -63,57 +64,70 @@
     if not isinstance(data, np.ndarray):
         typer.echo("🔄 Converting data to numpy...")
         return data.to_numpy()
     return data
 
 
 @app.command()
-def serialize(input_file: str, fp_impl: str = 'FP16x16'):
+def serialize(input_file: str, framework='ONNX_ORION'):
     """
     Serialize data from a file to a tensor representation.
 
     Args:
     input_file (str): The path to the input file.
-    fp_impl (str): Fixed-point implementation detail.
+    framework (str): Context of the framework used.
 
     Returns:
     Serialized tensor.
     """
 
     typer.echo("🚀 Starting the conversion process...")
     data = load_data(input_file)
     typer.echo("✅ Data loaded successfully!")
 
     numpy_array = convert_to_numpy(data)
     typer.echo("✅ Conversion to numpy completed!")
 
-    tensor = create_tensor_from_array(numpy_array, fp_impl)
-    typer.echo("✅ Conversion to tensor completed!")
+    match framework:
+        case 'ONNX_ORION':
+            tensor = create_tensor_from_array(numpy_array, 'FP16x16')
+            typer.echo("✅ Conversion to tensor completed!")
+        case 'XGB':
+            numpy_array *= 100000
+            tensor = numpy_array.astype(np.int64)
+        case 'LGBM':
+            numpy_array *= 100000
+            tensor = numpy_array.astype(np.int64)
+        case _:
+            tensor = create_tensor_from_array(
+                numpy_array, 'FP16x16')
+            typer.echo("✅ Conversion to tensor completed!")
 
     serialized = serializer(tensor)
     typer.echo("✅ Serialized tensor successfully! 🎉")
 
     return serialized
 
 
 @app.command()
-def deserialize(serialized: str, data_type: str):
+def deserialize(serialized: str, data_type: str, framework='ONNX_ORION'):
     """
     Deserialize a serialized string into a specific data type.
 
     Args:
     serialized (str): Serialized data in string format.
     data_type (str): The type of data to deserialize into.
+    framework (str): Context of the framework used.
 
     Returns:
     Deserialized data.
     """
     typer.echo("🚀 Starting deserialization process...")
 
-    deserialized = deserializer(serialized, data_type)
+    deserialized = deserializer(serialized, data_type, framework)
     typer.echo("✅ Deserialization completed! 🎉")
 
     return deserialized
 
 
 @app.command()
 def convert(input_file: str, output_file: str, output_format: OutputFormat = OutputFormat.NUMPY, dtype: Dtype = Dtype.I32):
```

### Comparing `giza_osiris-0.2.6/osiris/cairo/data_converter/data_converter.py` & `giza_osiris-0.2.7/osiris/cairo/data_converter/data_converter.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.6/osiris/cairo/data_converter/data_statement_generator.py` & `giza_osiris-0.2.7/osiris/cairo/data_converter/data_statement_generator.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.6/osiris/cairo/data_converter/tensor_creator.py` & `giza_osiris-0.2.7/osiris/cairo/data_converter/tensor_creator.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.6/osiris/cairo/file_manager/cairo_data.py` & `giza_osiris-0.2.7/osiris/cairo/file_manager/cairo_data.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.6/osiris/cairo/file_manager/file.py` & `giza_osiris-0.2.7/osiris/cairo/file_manager/file.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.6/osiris/cairo/serde/data_structures.py` & `giza_osiris-0.2.7/osiris/cairo/serde/data_structures.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.6/osiris/cairo/serde/deserialize.py` & `giza_osiris-0.2.7/osiris/cairo/serde/deserialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 import re
 
 import numpy as np
 
 from osiris.cairo.serde.utils import felt_to_int, from_fp
 
 
-def deserializer(serialized, dtype):
+def deserializer(serialized, dtype, framework='ONNX_ORION'):
 
     if dtype in ["u8", "u16", "u32", "u64", "u128", "i8", "i16", "i32", "i64", "i128"]:
-        return felt_to_int(int(serialized))
+
+        match framework:
+            case 'XGB':
+                return felt_to_int(int(serialized)) / 100000
+            case 'LGBM':
+                return felt_to_int(int(serialized)) / 100000
+            case _:
+                return felt_to_int(int(serialized))
 
     elif dtype.startswith("FP"):
         return deserialize_fp(serialized)
 
     elif dtype.startswith('Span<'):
         return deserialize_span(serialized, dtype)
```

### Comparing `giza_osiris-0.2.6/osiris/cairo/serde/serialize.py` & `giza_osiris-0.2.7/osiris/cairo/serde/serialize.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.6/osiris/cairo/serde/utils.py` & `giza_osiris-0.2.7/osiris/cairo/serde/utils.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.6/pyproject.toml` & `giza_osiris-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giza-osiris"
-version = "0.2.6"
+version = "0.2.7"
 description = "Osiris is a Python library designed for efficient data conversion and management, primarily transforming data into Cairo programs"
 authors = ["Fran Algaba <fran@gizatech.xyz>"]
 readme = "README.md"
 packages = [{include = "osiris"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `giza_osiris-0.2.6/PKG-INFO` & `giza_osiris-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giza-osiris
-Version: 0.2.6
+Version: 0.2.7
 Summary: Osiris is a Python library designed for efficient data conversion and management, primarily transforming data into Cairo programs
 Author: Fran Algaba
 Author-email: fran@gizatech.xyz
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

