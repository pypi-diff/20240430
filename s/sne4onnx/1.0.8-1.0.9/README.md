# Comparing `tmp/sne4onnx-1.0.8.tar.gz` & `tmp/sne4onnx-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sne4onnx-1.0.8.tar", last modified: Wed May 25 06:31:10 2022, max compression
+gzip compressed data, was "sne4onnx-1.0.9.tar", last modified: Tue Jun  7 14:47:00 2022, max compression
```

## Comparing `sne4onnx-1.0.8.tar` & `sne4onnx-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 06:31:10.569312 sne4onnx-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-05-25 06:31:02.000000 sne4onnx-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6888 2022-05-25 06:31:10.569312 sne4onnx-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6352 2022-05-25 06:31:02.000000 sne4onnx-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-25 06:31:10.569312 sne4onnx-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-05-25 06:31:02.000000 sne4onnx-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 06:31:10.565312 sne4onnx-1.0.8/sne4onnx/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-25 06:31:02.000000 sne4onnx-1.0.8/sne4onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-05-25 06:31:02.000000 sne4onnx-1.0.8/sne4onnx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6565 2022-05-25 06:31:02.000000 sne4onnx-1.0.8/sne4onnx/onnx_network_extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 06:31:10.569312 sne4onnx-1.0.8/sne4onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6888 2022-05-25 06:31:10.000000 sne4onnx-1.0.8/sne4onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-05-25 06:31:10.000000 sne4onnx-1.0.8/sne4onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-25 06:31:10.000000 sne4onnx-1.0.8/sne4onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-25 06:31:10.000000 sne4onnx-1.0.8/sne4onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-25 06:31:10.000000 sne4onnx-1.0.8/sne4onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 14:47:00.945129 sne4onnx-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-06-07 14:46:48.000000 sne4onnx-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     6888 2022-06-07 14:47:00.945129 sne4onnx-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6352 2022-06-07 14:46:48.000000 sne4onnx-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 14:47:00.945129 sne4onnx-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-06-07 14:46:48.000000 sne4onnx-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 14:47:00.945129 sne4onnx-1.0.9/sne4onnx/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-06-07 14:46:48.000000 sne4onnx-1.0.9/sne4onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-07 14:46:48.000000 sne4onnx-1.0.9/sne4onnx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6770 2022-06-07 14:46:48.000000 sne4onnx-1.0.9/sne4onnx/onnx_network_extraction.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 14:47:00.945129 sne4onnx-1.0.9/sne4onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6888 2022-06-07 14:47:00.000000 sne4onnx-1.0.9/sne4onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-06-07 14:47:00.000000 sne4onnx-1.0.9/sne4onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 14:47:00.000000 sne4onnx-1.0.9/sne4onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-06-07 14:47:00.000000 sne4onnx-1.0.9/sne4onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-07 14:47:00.000000 sne4onnx-1.0.9/sne4onnx.egg-info/top_level.txt
```

### Comparing `sne4onnx-1.0.8/LICENSE` & `sne4onnx-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sne4onnx-1.0.8/PKG-INFO` & `sne4onnx-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sne4onnx
-Version: 1.0.8
+Version: 1.0.9
 Summary: A very simple tool for situations where optimization with onnx-simplifier would exceed the Protocol Buffers upper file size limit of 2GB, or simply to separate onnx files to any size you want. Simple Network Extraction for ONNX.
 Home-page: https://github.com/PINTO0309/sne4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

### Comparing `sne4onnx-1.0.8/README.md` & `sne4onnx-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sne4onnx-1.0.8/setup.py` & `sne4onnx-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `sne4onnx-1.0.8/sne4onnx/onnx_network_extraction.py` & `sne4onnx-1.0.9/sne4onnx/onnx_network_extraction.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,28 +121,30 @@
     ]
 
     # Init graph INPUT/OUTPUT
     graph.inputs.clear()
     graph.outputs.clear()
 
     # Update graph INPUT/OUTPUT
-    graph.inputs = [
-        graph_node_input \
-            for graph_node in graph_node_inputs \
-                for graph_node_input in graph_node.inputs \
-                    if graph_node_input.shape
-    ]
+    input_tmp = []
+    for graph_node in graph_node_inputs:
+        for graph_node_input in graph_node.inputs:
+            # if graph_node_input.shape and graph_node_input.name not in [i.name for i in input_tmp]:
+            if graph_node_input.shape and graph_node_input not in [i for i in input_tmp]:
+                input_tmp.append(graph_node_input)
+    graph.inputs = input_tmp
+
     graph.outputs = [
         graph_node_output \
             for graph_node in graph_node_outputs \
                 for graph_node_output in graph_node.outputs
     ]
 
     # Cleanup
-    graph.cleanup().toposort()
+    graph.cleanup(remove_unused_graph_inputs=True).toposort()
 
     # Shape Estimation
     extracted_graph = None
     try:
         extracted_graph = onnx.shape_inference.infer_shapes(gs.export_onnx(graph))
     except Exception as e:
         extracted_graph = gs.export_onnx(graph)
```

### Comparing `sne4onnx-1.0.8/sne4onnx.egg-info/PKG-INFO` & `sne4onnx-1.0.9/sne4onnx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sne4onnx
-Version: 1.0.8
+Version: 1.0.9
 Summary: A very simple tool for situations where optimization with onnx-simplifier would exceed the Protocol Buffers upper file size limit of 2GB, or simply to separate onnx files to any size you want. Simple Network Extraction for ONNX.
 Home-page: https://github.com/PINTO0309/sne4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

