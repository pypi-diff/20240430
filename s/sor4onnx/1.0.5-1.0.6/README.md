# Comparing `tmp/sor4onnx-1.0.5.tar.gz` & `tmp/sor4onnx-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sor4onnx-1.0.5.tar", last modified: Sat Sep 24 04:47:59 2022, max compression
+gzip compressed data, was "sor4onnx-1.0.6.tar", last modified: Tue Apr 30 06:35:06 2024, max compression
```

## Comparing `sor4onnx-1.0.5.tar` & `sor4onnx-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 04:47:59.407190 sor4onnx-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-24 04:47:52.000000 sor4onnx-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6456 2022-09-24 04:47:59.407190 sor4onnx-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6123 2022-09-24 04:47:52.000000 sor4onnx-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-24 04:47:59.407190 sor4onnx-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-09-24 04:47:52.000000 sor4onnx-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 04:47:59.403190 sor4onnx-1.0.5/sor4onnx/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-24 04:47:52.000000 sor4onnx-1.0.5/sor4onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-24 04:47:52.000000 sor4onnx-1.0.5/sor4onnx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11241 2022-09-24 04:47:52.000000 sor4onnx-1.0.5/sor4onnx/onnx_opname_renamer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 04:47:59.407190 sor4onnx-1.0.5/sor4onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6456 2022-09-24 04:47:59.000000 sor4onnx-1.0.5/sor4onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-09-24 04:47:59.000000 sor4onnx-1.0.5/sor4onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-24 04:47:59.000000 sor4onnx-1.0.5/sor4onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-24 04:47:59.000000 sor4onnx-1.0.5/sor4onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-24 04:47:59.000000 sor4onnx-1.0.5/sor4onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:06.283565 sor4onnx-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 06:35:00.000000 sor4onnx-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-04-30 06:35:06.279565 sor4onnx-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-04-30 06:35:00.000000 sor4onnx-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:35:06.283565 sor4onnx-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-30 06:35:00.000000 sor4onnx-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:06.279565 sor4onnx-1.0.6/sor4onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-30 06:35:00.000000 sor4onnx-1.0.6/sor4onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 06:35:00.000000 sor4onnx-1.0.6/sor4onnx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11486 2024-04-30 06:35:00.000000 sor4onnx-1.0.6/sor4onnx/onnx_opname_renamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:06.279565 sor4onnx-1.0.6/sor4onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-04-30 06:35:06.000000 sor4onnx-1.0.6/sor4onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-30 06:35:06.000000 sor4onnx-1.0.6/sor4onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:35:06.000000 sor4onnx-1.0.6/sor4onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 06:35:06.000000 sor4onnx-1.0.6/sor4onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 06:35:06.000000 sor4onnx-1.0.6/sor4onnx.egg-info/top_level.txt
```

### Comparing `sor4onnx-1.0.5/LICENSE` & `sor4onnx-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sor4onnx-1.0.5/PKG-INFO` & `sor4onnx-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sor4onnx
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simple OP Renamer for ONNX.
 Home-page: https://github.com/PINTO0309/sor4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

### Comparing `sor4onnx-1.0.5/README.md` & `sor4onnx-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sor4onnx-1.0.5/setup.py` & `sor4onnx-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `sor4onnx-1.0.5/sor4onnx/onnx_opname_renamer.py` & `sor4onnx-1.0.6/sor4onnx/onnx_opname_renamer.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,19 @@
         )
         sys.exit(1)
 
     # Loading Graphs
     # onnx_graph If specified, onnx_graph is processed first
     if not onnx_graph:
         onnx_graph = onnx.load(input_onnx_file_path)
+
+    # domain, ir_version
+    domain: str = onnx_graph.domain
+    ir_version: int = onnx_graph.ir_version
+
     graph = gs.import_onnx(onnx_graph)
     graph.cleanup().toposort()
 
     if mode in ['full', 'inputs']:
         for graph_input in graph.inputs:
             if search_mode == 'exact_match':
                 if graph_input.name == old_new[0]:
@@ -210,17 +215,17 @@
             supplementation_idx += 1
 
     graph.cleanup().toposort()
 
     # Shape Estimation
     renamed_graph = None
     try:
-        renamed_graph = onnx.shape_inference.infer_shapes(gs.export_onnx(graph))
+        renamed_graph = onnx.shape_inference.infer_shapes(gs.export_onnx(graph, do_type_check=False, **{'domain': domain, 'ir_version': ir_version}))
     except:
-        renamed_graph = gs.export_onnx(graph)
+        renamed_graph = gs.export_onnx(graph, do_type_check=False, **{'domain': domain, 'ir_version': ir_version})
         if not non_verbose:
             print(
                 f'{Color.YELLOW}WARNING:{Color.RESET} '+
                 'The input shape of the next OP does not match the output shape. '+
                 'Be sure to open the .onnx file to verify the certainty of the geometry.'
             )
```

### Comparing `sor4onnx-1.0.5/sor4onnx.egg-info/PKG-INFO` & `sor4onnx-1.0.6/sor4onnx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sor4onnx
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simple OP Renamer for ONNX.
 Home-page: https://github.com/PINTO0309/sor4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

