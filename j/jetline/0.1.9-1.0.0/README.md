# Comparing `tmp/jetline-0.1.9.tar.gz` & `tmp/jetline-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetline-0.1.9.tar", last modified: Sun Apr 28 16:50:12 2024, max compression
+gzip compressed data, was "jetline-1.0.0.tar", last modified: Tue Apr 30 11:50:27 2024, max compression
```

## Comparing `jetline-0.1.9.tar` & `jetline-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,53 @@
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:50:12.632384 jetline-0.1.9/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:50:12.632123 jetline-0.1.9/PKG-INFO
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1103 2024-04-25 16:42:38.000000 jetline-0.1.9/README.md
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:50:12.622449 jetline-0.1.9/jetline/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.9/jetline/__init__.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:50:12.625436 jetline-0.1.9/jetline/commands/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.9/jetline/commands/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1997 2024-04-28 08:26:04.000000 jetline-0.1.9/jetline/commands/_helper.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     4122 2024-04-26 06:00:11.000000 jetline-0.1.9/jetline/commands/create_pipe.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)    10211 2024-04-28 16:43:19.000000 jetline-0.1.9/jetline/commands/create_viz.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     2086 2024-04-25 16:41:25.000000 jetline-0.1.9/jetline/commands/info.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     2912 2024-04-28 15:45:14.000000 jetline-0.1.9/jetline/commands/installer.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1485 2024-04-27 07:23:16.000000 jetline-0.1.9/jetline/commands/run_pipeline.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)    10251 2024-04-27 08:48:48.000000 jetline-0.1.9/jetline/commands/to_exe.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:50:12.627537 jetline-0.1.9/jetline/data/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.9/jetline/data/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     5221 2024-04-28 16:10:21.000000 jetline-0.1.9/jetline/data/data.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      362 2024-04-27 08:37:20.000000 jetline-0.1.9/jetline/data/helper.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      127 2024-04-26 05:52:47.000000 jetline-0.1.9/jetline/logging.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:50:12.628619 jetline-0.1.9/jetline/pipeline/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.9/jetline/pipeline/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1686 2024-04-28 16:49:06.000000 jetline-0.1.9/jetline/pipeline/node.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     6042 2024-04-28 16:49:35.000000 jetline-0.1.9/jetline/pipeline/pipeline.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:50:12.630662 jetline-0.1.9/jetline/templates/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.9/jetline/templates/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      271 2024-04-28 16:45:03.000000 jetline-0.1.9/jetline/templates/data.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      504 2024-04-27 07:36:36.000000 jetline-0.1.9/jetline/templates/main.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      292 2024-04-27 08:19:53.000000 jetline-0.1.9/jetline/templates/nodes.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      533 2024-04-28 16:45:49.000000 jetline-0.1.9/jetline/templates/pipeline.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:50:12.631616 jetline-0.1.9/jetline.egg-info/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:50:12.000000 jetline-0.1.9/jetline.egg-info/PKG-INFO
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      771 2024-04-28 16:50:12.000000 jetline-0.1.9/jetline.egg-info/SOURCES.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        1 2024-04-28 16:50:12.000000 jetline-0.1.9/jetline.egg-info/dependency_links.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      308 2024-04-28 16:50:12.000000 jetline-0.1.9/jetline.egg-info/entry_points.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      117 2024-04-28 16:50:12.000000 jetline-0.1.9/jetline.egg-info/requires.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        8 2024-04-28 16:50:12.000000 jetline-0.1.9/jetline.egg-info/top_level.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)       38 2024-04-28 16:50:12.632563 jetline-0.1.9/setup.cfg
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1630 2024-04-28 16:50:02.000000 jetline-0.1.9/setup.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-30 11:50:27.257475 jetline-1.0.0/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)       49 2024-04-29 07:25:58.000000 jetline-1.0.0/MANIFEST.in
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1020 2024-04-30 11:50:27.257238 jetline-1.0.0/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1103 2024-04-25 16:42:38.000000 jetline-1.0.0/README.md
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-30 11:50:27.244569 jetline-1.0.0/jetline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-1.0.0/jetline/__init__.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-30 11:50:27.248237 jetline-1.0.0/jetline/commands/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-1.0.0/jetline/commands/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1997 2024-04-28 08:26:04.000000 jetline-1.0.0/jetline/commands/_helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2076 2024-04-29 14:56:50.000000 jetline-1.0.0/jetline/commands/create_pipe.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     9278 2024-04-30 07:54:31.000000 jetline-1.0.0/jetline/commands/create_viz.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2086 2024-04-25 16:41:25.000000 jetline-1.0.0/jetline/commands/info.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2084 2024-04-30 06:16:09.000000 jetline-1.0.0/jetline/commands/installer.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1156 2024-04-29 16:35:07.000000 jetline-1.0.0/jetline/commands/run_pipeline.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)    10251 2024-04-27 08:48:48.000000 jetline-1.0.0/jetline/commands/to_exe.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-30 11:50:27.249011 jetline-1.0.0/jetline/data/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-1.0.0/jetline/data/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     5190 2024-04-29 16:32:58.000000 jetline-1.0.0/jetline/data/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      362 2024-04-27 08:37:20.000000 jetline-1.0.0/jetline/data/helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)       54 2024-04-29 16:32:58.000000 jetline-1.0.0/jetline/logging.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-30 11:50:27.250003 jetline-1.0.0/jetline/pipeline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-1.0.0/jetline/pipeline/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1688 2024-04-29 16:33:03.000000 jetline-1.0.0/jetline/pipeline/node.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     7081 2024-04-29 16:32:58.000000 jetline-1.0.0/jetline/pipeline/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-30 11:50:27.251416 jetline-1.0.0/jetline/templates/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-1.0.0/jetline/templates/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      355 2024-04-30 06:27:29.000000 jetline-1.0.0/jetline/templates/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      682 2024-04-30 06:19:23.000000 jetline-1.0.0/jetline/templates/main.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      153 2024-04-30 06:27:29.000000 jetline-1.0.0/jetline/templates/nodes.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      483 2024-04-30 08:53:46.000000 jetline-1.0.0/jetline/templates/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-30 11:50:27.251698 jetline-1.0.0/jetline/visualization/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-29 06:48:26.000000 jetline-1.0.0/jetline/visualization/__init__.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-30 11:50:27.252010 jetline-1.0.0/jetline/visualization/server/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-29 06:51:18.000000 jetline-1.0.0/jetline/visualization/server/__init__.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-30 11:50:27.252780 jetline-1.0.0/jetline/visualization/server/dist/
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-30 11:50:27.254964 jetline-1.0.0/jetline/visualization/server/dist/assets/
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-30 11:50:27.256583 jetline-1.0.0/jetline/visualization/server/dist/assets/assets/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)   503049 2024-04-29 09:25:46.000000 jetline-1.0.0/jetline/visualization/server/dist/assets/assets/index-BCqVGvry.js
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)    14745 2024-04-29 09:25:46.000000 jetline-1.0.0/jetline/visualization/server/dist/assets/assets/index-BUXWNTAg.css
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)   503049 2024-04-29 09:02:51.000000 jetline-1.0.0/jetline/visualization/server/dist/assets/index-BCqVGvry.js
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)    14745 2024-04-29 09:02:51.000000 jetline-1.0.0/jetline/visualization/server/dist/assets/index-BUXWNTAg.css
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      454 2024-04-29 09:25:46.000000 jetline-1.0.0/jetline/visualization/server/dist/index.html
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1497 2024-04-29 09:25:46.000000 jetline-1.0.0/jetline/visualization/server/dist/vite.svg
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1485 2024-04-29 07:35:13.000000 jetline-1.0.0/jetline/visualization/server/server.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-30 11:50:27.256918 jetline-1.0.0/jetline.egg-info/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1020 2024-04-30 11:50:27.000000 jetline-1.0.0/jetline.egg-info/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1237 2024-04-30 11:50:27.000000 jetline-1.0.0/jetline.egg-info/SOURCES.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        1 2024-04-30 11:50:27.000000 jetline-1.0.0/jetline.egg-info/dependency_links.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      308 2024-04-30 11:50:27.000000 jetline-1.0.0/jetline.egg-info/entry_points.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      117 2024-04-30 11:50:27.000000 jetline-1.0.0/jetline.egg-info/requires.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        8 2024-04-30 11:50:27.000000 jetline-1.0.0/jetline.egg-info/top_level.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)       38 2024-04-30 11:50:27.257524 jetline-1.0.0/setup.cfg
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1609 2024-04-30 11:50:20.000000 jetline-1.0.0/setup.py
```

### Comparing `jetline-0.1.9/PKG-INFO` & `jetline-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: jetline
-Version: 0.1.9
+Version: 1.0.0
 Summary: Automated Pipeline Builder
 Home-page: https://github.com/your_username/jetline
 Author: Johannes Kanthak
 Author-email: johannes.kanthak@kdc-solutions.de
 License: MIT
-Keywords: pipeline automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `jetline-0.1.9/README.md` & `jetline-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `jetline-0.1.9/jetline/commands/_helper.py` & `jetline-1.0.0/jetline/commands/_helper.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.9/jetline/commands/create_viz.py` & `jetline-1.0.0/jetline/commands/create_viz.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import os
 import ast
 import astor
 import toml
 import re
 import json
+import shutil
+import subprocess
+import sys
 
 
 def get_project_infos():
     """Fetches the project name and path based on project settings in a TOML file."""
     current_dir = os.getcwd()
     toml_file_path = os.path.join(current_dir, "project.toml")
 
@@ -20,38 +23,23 @@
                 return None, None
             place_path = os.path.join(current_dir, place)
             return project_name, place_path, current_dir
     except Exception:
         raise ValueError("Project name or place is missing in the TOML file.")
 
 
-def extract_pipeline_order(current_directory):
-    """
-    Extracts the PIPELINE_ORDER list from the content of the main file.
-
-    :param current_directory: The directory of the main file.
-    :return: The extracted PIPELINE_ORDER list or None if not found.
-    """
-    main_path = os.path.join(current_directory, 'main.py')
-    with open(main_path, 'r') as file:
-        main_content = file.read()
-
-    pipeline_order_match = re.search(r'PIPELINE_ORDER\s*=\s*\[([^\]]+)\]', main_content)
-    if pipeline_order_match:
-        return pipeline_order_match.group(1).replace("'", "").replace('"', "").split(',')
-    return None
-
 def extract_class_name(class_code):
     # Suchen Sie nach dem ersten Auftreten von 'name =' im Klassencode
     match = re.search(r"name\s*=\s*[\"']([^\"']+)[\"']", class_code)
     if match:
         # Extrahieren Sie den Namen aus dem Regex-Match
         class_name = match.group(1)
         return class_name
 
+
 def extract_classes_with_parent(current_dir):
     """
     Extracts all classes with a given parent class from a file.
     """
     nodes = []
     file_path = os.path.join(current_dir, "data.py")
     with open(file_path, "r") as f:
@@ -123,14 +111,15 @@
     node_file_path = os.path.join(folder_path, "nodes.py")
     if os.path.exists(node_file_path):
         with open(node_file_path, "r") as file:
             tree = ast.parse(file.read(), filename=node_file_path)
             for node_def in tree.body:
                 if isinstance(node_def, ast.FunctionDef):
                     node_name = node_def.name
+
                     node_description = ast.get_docstring(node_def) or ''
                     node_code = ast.unparse(node_def)
                     nodes_dict[node_name] = {
                         "id": node_name,
                         "data": {
                             "title": node_name,
                             "description": node_description,
@@ -142,41 +131,45 @@
                         "position": {
                             "x": '',
                             "y": '',
                         }
                     }
 
             for i, func_name in enumerate(function_names):
+
                 node_name = func_name.split('.')[-1]
                 if node_name in nodes_dict:
                     sorted_nodes[i] = nodes_dict[node_name]
                     if i < len(inputs):
                         sorted_nodes[i]["data"]["inputs"] = format_node_parameters(inputs[i])
 
                     if i < len(outputs):
                         sorted_nodes[i]["data"]["outputs"] = format_node_parameters(outputs[i])
 
             for i, position_data in enumerate(viz):
-                x = int(position_data.split(",")[0].split(":")[1].strip())
-
-                y = int(position_data.split(",")[1].split(":")[1].strip())
-                source = position_data.split(",")[2].split(":")[1].strip().replace("'", "").replace('"', '')
+                node_name = function_names[i].split('.')[-1]
 
-                sorted_nodes[i]["position"]["x"] = x
-                sorted_nodes[i]["position"]["y"] = y
-
-                edge_id = f"{source}->{node_name}"
-                edges.append({
-                    "id": edge_id,
-                    "source": source,
-                    "target": node_name,
-                    "animated": True,
-                    "type": "default",
-                    "style": "edgeStyle"
-                })
+                position_dict = eval("{" + position_data + "}")
+                x = position_dict['x']
+                y = position_dict['y']
+                sources = position_dict['sources']
+
+                for source in sources:
+                    sorted_nodes[i]["position"]["x"] = x
+                    sorted_nodes[i]["position"]["y"] = y
+
+                    edge_id = f"{source}->{node_name}"
+                    edges.append({
+                        "id": edge_id,
+                        "source": source,
+                        "target": node_name,
+                        "animated": True,
+                        "type": "default",
+                        "style": "edgeStyle"
+                    })
 
             return sorted_nodes, edges
 
     return [], []
 
 
 def extract_register_functions_from_pipeline(pipeline_file_path):
@@ -190,18 +183,16 @@
                 break  # Stop after finding the first 'register' function
     return register_functions
 
 
 def extract_data_from_pipelines(current_dir, place_path):
     nodes = []
     edges = []
-    pipeline_order = extract_pipeline_order(current_dir)
+
     pipeline_folders = [folder for folder in os.listdir(place_path) if os.path.isdir(os.path.join(place_path, folder))]
-    pipeline_folders = sorted(pipeline_folders,
-                              key=lambda x: pipeline_order.index(x) if x in pipeline_order else len(pipeline_order))
 
     for folder in pipeline_folders:
         folder_path = os.path.join(current_dir, place_path, folder)
         pipeline_file_path = os.path.join(folder_path, "pipeline.py")
         if os.path.exists(pipeline_file_path):
             register_function = extract_register_functions_from_pipeline(pipeline_file_path)
 
@@ -235,44 +226,39 @@
             edge["target"] = name_to_number[target_id]
 
         new_edges.append(edge)
 
     return new_nodes, new_edges
 
 
-import os
-import shutil
-
-
 def main():
+    subprocess.run("lsof -ti:8000 | xargs kill", shell=True)
     nodes = []
     project_name, place_path, current_dir = get_project_infos()
     nodes += extract_classes_with_parent(current_dir)
 
     new_nodes, edges = extract_data_from_pipelines(current_dir, place_path)
 
     nodes.extend(new_nodes)
 
     new_nodes, new_edges = convert_to_numbered_ids(nodes, edges)
 
-
-    # generate viz folder
-
+    # create folder
     viz_folder = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'visualization', 'server'))
-    print(viz_folder)
-    # Kopieren Sie den gesamten Inhalt des viz_folder in das current_dir
+
     destination_folder = os.path.join(current_dir, "visualization")
+
     if os.path.exists(destination_folder) and os.path.isdir(destination_folder):
         shutil.rmtree(destination_folder)
 
-    # Kopieren Sie das Verzeichnis visualization und dessen gesamten Inhalt in das current_dir
     if os.path.exists(viz_folder) and os.path.isdir(viz_folder):
         shutil.copytree(viz_folder, destination_folder)
 
-    # add json to distvisualization/dist/viz-data.json"
-    output_file_path = os.path.join(current_dir, "visualization", "dist", "viz-data.json" )
-    with open(output_file_path, "w") as outfile:
-        json.dump({"nodes": new_nodes, "edges": new_edges}, outfile, indent=4)
+    with open("visualization/dist/viz-data.json", "w") as f:
+        f.write(json.dumps({"nodes": new_nodes, "edges": new_edges}, indent=4))
+
+    os.chdir(destination_folder)
+    subprocess.Popen([sys.executable, 'server.py'])
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jetline-0.1.9/jetline/commands/info.py` & `jetline-1.0.0/jetline/commands/info.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.9/jetline/commands/installer.py` & `jetline-1.0.0/jetline/commands/installer.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,35 +41,14 @@
     shutil.copy(os.path.join(templates_folder, 'main.py'), project_folder)
 
     pipeline_folder = os.path.join(project_folder, pipeline_name)
     os.makedirs(pipeline_folder, exist_ok=True)
 
     shutil.copy(os.path.join(templates_folder, 'data.py'), project_folder)
 
-    example_pipeline_folder = os.path.join(pipeline_folder, 'example_pipeline')
-    os.makedirs(example_pipeline_folder, exist_ok=True)
-
-    init_file_example = os.path.join(example_pipeline_folder, "__init__.py")
-    Path(init_file_example).touch()
-
-    shutil.copy(os.path.join(templates_folder, 'pipeline.py'), example_pipeline_folder)
-
-    def replace_text_in_file(file_path, old_text, new_text):
-        with open(file_path, 'r') as file:
-            file_content = file.read()
-
-        file_content = file_content.replace(old_text, new_text)
-
-        with open(file_path, 'w') as file:
-            file.write(file_content)
-
-    replace_text_in_file(os.path.join(example_pipeline_folder, 'pipeline.py'), '__PIPE__', 'example_pipeline')
-
-    shutil.copy(os.path.join(templates_folder, 'nodes.py'), example_pipeline_folder)
-
     click.echo(
         click.style("✅ Project setup complete at ", fg='green', bold=True) + click.style(project_folder, fg='white'))
 
     click.echo(
         click.style(f"\nRun {Fore.YELLOW}cd {project_name}{Style.RESET_ALL} to navigate to the project directory.",
                     fg='cyan'))
```

### Comparing `jetline-0.1.9/jetline/commands/to_exe.py` & `jetline-1.0.0/jetline/commands/to_exe.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.9/jetline/data/data.py` & `jetline-1.0.0/jetline/data/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                         spec.loader.exec_module(data_module)
 
                         for name, obj in inspect.getmembers(data_module):
                             if inspect.isclass(obj) and isinstance(obj, type) and obj != data_module.Data:
                                 data_classes.append(obj)
 
                         for data_class in data_classes:
-                            logger.info(f"Found: {data_class.__name__}, Description: {data_class.__doc__}")
+                            logger.info(f"Found: {data_class.__name__}")
 
                     except Exception as e:
                         logger.error(f"Error loading data classes from file {data_file}: {e}")
                         exit(1)
 
         return data_classes
 
@@ -127,17 +127,17 @@
 
     def update_jetline_data(self, name, new_value):
         """
         Update jetline data to the data dictionary.
         """
         if name in self.data:
             self.data[name]['value'] = new_value
-            logger.info(f"Data object '{name}' successfully updated.")
+            logger.success(f"Data object '{name}' successfully updated.")
         else:
-            logger.info(f"Data object '{name}' not found. Cannot be updated.")
+            logger.error(f"Data object '{name}' not found. Cannot be updated.")
 
     def get_jetline_data(self, name):
         """
         Retrieve the data associated with the given name from the self.data dictionary.
         """
         data_info = self.data.get(name)
         if data_info:
```

### Comparing `jetline-0.1.9/jetline/pipeline/node.py` & `jetline-1.0.0/jetline/pipeline/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 class Node:
     """
     Node
 
     Represents a node in a graph that performs a specific function on input data.
 
     Attributes:
```

### Comparing `jetline-0.1.9/jetline/pipeline/pipeline.py` & `jetline-1.0.0/jetline/pipeline/pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 import toml
 import inspect
 from jetline.data.data import DataManager
 from jetline.logging import logger
 import os
 import sys
-
+import concurrent.futures
 
 class Pipeline:
     def __init__(self, nodes=None, data_manager=None):
         """
         Initialize the Pipeline with a list of nodes and a data manager.
         """
         self.nodes = {node.function: node for node in nodes} if nodes else {}
@@ -128,39 +128,56 @@
                             pipeline_definition = pipeline_register_function(self.data_manager)
                             if isinstance(pipeline_definition, Pipeline):
                                 self.pipelines[pipeline_name] = pipeline_definition
                             else:
                                 raise ValueError(
                                     f"The register function in {pipeline_module_path} must return a Pipeline instance.")
 
-    def run(self, pipeline_order):
+    def run(self, pipeline_orders):
         """
-        Run method to execute pipelines in a specific order.
+        Run method to execute pipelines in multiple orders simultaneously.
 
         Parameters:
         - self: The object instance.
-        - pipeline_order (list): The order in which the pipelines should be executed.
+        - pipeline_orders (list of lists): List of lists where each inner list contains the pipelines to be executed simultaneously.
 
         Returns:
         - results (dict): A dictionary with the results of each pipeline execution.
 
         Raises:
         - ValueError: If any of the pipelines in the specified order are not found.
 
         Example usage:
-            pipeline_order = ['pipeline1', 'pipeline2', 'pipeline3']
-            results = obj.run(pipeline_order)
+            pipeline_orders = [['pipeline1', 'pipeline2'], ['pipeline3']]
+            results = obj.run(pipeline_orders)
         """
         results = {}
 
-        missing_pipelines = [pipeline_name for pipeline_name in pipeline_order if pipeline_name not in self.pipelines]
-        if missing_pipelines:
-            error_message = f"Error running pipelines: The following pipelines were not found: {', '.join(missing_pipelines)}"
-            logger.error(error_message)
-            raise ValueError(error_message)
-
-        for pipeline_name in pipeline_order:
-            pipeline = self.pipelines[pipeline_name]
-            results[pipeline_name] = pipeline.run()
-            logger.info(f"Pipeline '{pipeline_name}' executed successfully.")
-        logger.info("All Pipelines ran successfully.")
+        with (concurrent.futures.ThreadPoolExecutor() as executor):
+            futures = []
+            for order_idx, pipeline_order in enumerate(pipeline_orders, start=1):
+                missing_pipelines = [pipeline_name for pipeline_name in pipeline_order if pipeline_name not in self.pipelines]
+                if missing_pipelines:
+                    error_message = (f"Error running pipelines in order {order_idx}"
+                                     f": The following pipelines were not found: {', '.join(missing_pipelines)}")
+                    logger.error(error_message)
+                    raise ValueError(error_message)
+
+                results.setdefault(order_idx, {})
+                for pipeline_name in pipeline_order:
+                    pipeline = self.pipelines[pipeline_name]
+                    if pipeline_name not in results[order_idx]:
+                        futures.append(executor.submit(pipeline.run))
+
+            for future in concurrent.futures.as_completed(futures):
+                # Get the result of each completed future
+                result = future.result()
+                # Find the corresponding pipeline order
+                for order_idx, pipeline_order in enumerate(pipeline_orders, start=1):
+                    if result in pipeline_order:
+                        pipeline_name = result
+                        results[order_idx][pipeline_name] = result
+                        logger.success(f"Pipeline '{pipeline_name}' in order {order_idx} executed successfully.")
+
+            logger.success(f"All Pipelines ran successfully.")
         return results
+
```

### Comparing `jetline-0.1.9/jetline.egg-info/PKG-INFO` & `jetline-1.0.0/jetline.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: jetline
-Version: 0.1.9
+Version: 1.0.0
 Summary: Automated Pipeline Builder
 Home-page: https://github.com/your_username/jetline
 Author: Johannes Kanthak
 Author-email: johannes.kanthak@kdc-solutions.de
 License: MIT
-Keywords: pipeline automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `jetline-0.1.9/setup.py` & `jetline-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 from setuptools import setup, find_packages
 
-classifiers = [
-    'Development Status :: 3 - Alpha',
-    'Intended Audience :: Developers',
-    'License :: OSI Approved :: MIT License',
-    'Operating System :: OS Independent',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Topic :: Software Development :: Libraries :: Python Modules'
-]
-
-install_requires = [
-    'click==8.1.7',
-    'colorama==0.4.6',
-    'toml==0.10.2',
-    'pandas==2.2.0',
-    'openpyxl==3.1.2',
-    'coloredlogs==15.0.1',
-    'fastapi==0.110.0',
-    'vulture'
-    
-
-]
-
 setup(
     name='jetline',
-    version='0.1.9',
+    version='1.0.0',
     description='Automated Pipeline Builder',
     url='https://github.com/your_username/jetline',
     author='Johannes Kanthak',
     author_email='johannes.kanthak@kdc-solutions.de',
     license='MIT',
-    classifiers=classifiers,
-    keywords='pipeline automation',
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Topic :: Software Development :: Libraries :: Python Modules'
+    ],
     packages=find_packages(),
     include_package_data=True,
-    install_requires=install_requires,
+
+    install_requires=[
+        'click==8.1.7',
+        'colorama==0.4.6',
+        'toml==0.10.2',
+        'pandas==2.2.0',
+        'openpyxl==3.1.2',
+        'coloredlogs==15.0.1',
+        'fastapi==0.110.0',
+        'vulture'
+    ],
     entry_points={
         'console_scripts': [
             'jetline = jetline.commands.info:main',
             'jetline-setup = jetline.commands.installer:main',
             'jetline-create-pipe = jetline.commands.create_pipe:main',
             'jetline-viz = jetline.commands.create_viz:main',
             'jetline-run = jetline.commands.run_pipeline:main [args]',
```

