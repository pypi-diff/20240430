# Comparing `tmp/tiny_dag-0.0.6.tar.gz` & `tmp/tiny_dag-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_dag-0.0.6.tar", last modified: Mon Apr 29 16:00:42 2024, max compression
+gzip compressed data, was "tiny_dag-0.0.7.tar", last modified: Tue Apr 30 05:36:29 2024, max compression
```

## Comparing `tiny_dag-0.0.6.tar` & `tiny_dag-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-29 16:00:42.380548 tiny_dag-0.0.6/
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     1072 2024-04-27 07:53:55.000000 tiny_dag-0.0.6/LICENSE
--rw-r--r--   0 ossi      (1000) ossi      (1000)     1638 2024-04-29 16:00:42.380548 tiny_dag-0.0.6/PKG-INFO
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     1100 2024-04-29 14:48:03.000000 tiny_dag-0.0.6/README.md
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      104 2024-04-27 09:26:48.000000 tiny_dag-0.0.6/pyproject.toml
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      668 2024-04-29 16:00:42.380548 tiny_dag-0.0.6/setup.cfg
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-29 16:00:42.376548 tiny_dag-0.0.6/src/
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-29 16:00:42.380548 tiny_dag-0.0.6/src/tiny_dag.egg-info/
--rw-r--r--   0 ossi      (1000) ossi      (1000)     1638 2024-04-29 16:00:42.000000 tiny_dag-0.0.6/src/tiny_dag.egg-info/PKG-INFO
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      286 2024-04-29 16:00:42.000000 tiny_dag-0.0.6/src/tiny_dag.egg-info/SOURCES.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        1 2024-04-29 16:00:42.000000 tiny_dag-0.0.6/src/tiny_dag.egg-info/dependency_links.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        9 2024-04-29 16:00:42.000000 tiny_dag-0.0.6/src/tiny_dag.egg-info/requires.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        8 2024-04-29 16:00:42.000000 tiny_dag-0.0.6/src/tiny_dag.egg-info/top_level.txt
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-29 16:00:42.380548 tiny_dag-0.0.6/src/tinydag/
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        0 2024-04-27 07:53:55.000000 tiny_dag-0.0.6/src/tinydag/__init__.py
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     7033 2024-04-29 15:49:11.000000 tiny_dag-0.0.6/src/tinydag/graph.py
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     1526 2024-04-29 15:59:05.000000 tiny_dag-0.0.6/src/tinydag/node.py
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-30 05:36:29.989566 tiny_dag-0.0.7/
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     1072 2024-04-27 07:53:55.000000 tiny_dag-0.0.7/LICENSE
+-rw-r--r--   0 ossi      (1000) ossi      (1000)     1638 2024-04-30 05:36:29.989566 tiny_dag-0.0.7/PKG-INFO
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     1100 2024-04-29 14:48:03.000000 tiny_dag-0.0.7/README.md
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      104 2024-04-27 09:26:48.000000 tiny_dag-0.0.7/pyproject.toml
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      668 2024-04-30 05:36:29.989566 tiny_dag-0.0.7/setup.cfg
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-30 05:36:29.989566 tiny_dag-0.0.7/src/
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-30 05:36:29.989566 tiny_dag-0.0.7/src/tiny_dag.egg-info/
+-rw-r--r--   0 ossi      (1000) ossi      (1000)     1638 2024-04-30 05:36:29.000000 tiny_dag-0.0.7/src/tiny_dag.egg-info/PKG-INFO
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      312 2024-04-30 05:36:29.000000 tiny_dag-0.0.7/src/tiny_dag.egg-info/SOURCES.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        1 2024-04-30 05:36:29.000000 tiny_dag-0.0.7/src/tiny_dag.egg-info/dependency_links.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        9 2024-04-30 05:36:29.000000 tiny_dag-0.0.7/src/tiny_dag.egg-info/requires.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        8 2024-04-30 05:36:29.000000 tiny_dag-0.0.7/src/tiny_dag.egg-info/top_level.txt
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-30 05:36:29.989566 tiny_dag-0.0.7/src/tinydag/
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        0 2024-04-27 07:53:55.000000 tiny_dag-0.0.7/src/tinydag/__init__.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)       92 2024-04-30 05:29:51.000000 tiny_dag-0.0.7/src/tinydag/exceptions.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     7738 2024-04-30 00:57:56.000000 tiny_dag-0.0.7/src/tinydag/graph.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     1526 2024-04-30 05:29:47.000000 tiny_dag-0.0.7/src/tinydag/node.py
```

### Comparing `tiny_dag-0.0.6/LICENSE` & `tiny_dag-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_dag-0.0.6/PKG-INFO` & `tiny_dag-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny-dag
-Version: 0.0.6
+Version: 0.0.7
 Summary: Minimal DAG implementation with Python
 Home-page: https://github.com/omyllymaki/tiny-dag
 Author: Ossi Myllymäki
 Author-email: omyllymaki@gmail.com
 Project-URL: Bug Tracker, https://github.com/omyllymaki/tiny-dag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tiny_dag-0.0.6/README.md` & `tiny_dag-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tiny_dag-0.0.6/setup.cfg` & `tiny_dag-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tiny-dag
-version = 0.0.6
+version = 0.0.7
 author = Ossi Myllymäki
 author_email = omyllymaki@gmail.com
 description = Minimal DAG implementation with Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/omyllymaki/tiny-dag
 project_urls =
```

### Comparing `tiny_dag-0.0.6/src/tiny_dag.egg-info/PKG-INFO` & `tiny_dag-0.0.7/src/tiny_dag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny-dag
-Version: 0.0.6
+Version: 0.0.7
 Summary: Minimal DAG implementation with Python
 Home-page: https://github.com/omyllymaki/tiny-dag
 Author: Ossi Myllymäki
 Author-email: omyllymaki@gmail.com
 Project-URL: Bug Tracker, https://github.com/omyllymaki/tiny-dag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tiny_dag-0.0.6/src/tinydag/graph.py` & `tiny_dag-0.0.7/src/tinydag/graph.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 import logging
 import time
 from copy import copy
 from typing import List, Callable, Union, Optional, Any
 
+from tinydag.exceptions import InvalidGraphError, MissingInputError
 from tinydag.node import Node
 
 logger = logging.getLogger(__name__)
 
 try:
     import graphviz as graphviz
     from graphviz import Digraph
 except ImportError:
     logger.warning("Cannot import graphviz")
 
 
-class GraphError(Exception):
-    pass
-
-
 class Graph:
     """
     Minimal implementation of computational (directed, acyclic) graph.
 
     User provides the graph structure (nodes) and input data for the graph. Every node waits until input data for that
     node is ready. Eventually, the graph executes every node in the graph and returns output of every node as the
     result.
@@ -51,21 +48,28 @@
 
     def __init__(self,
                  nodes: List[Node],
                  wrappers: Optional[List[Callable]] = None) -> None:
         """
         :param nodes: List of nodes defining the graph.
         :param wrappers: Optional wrapper functions that will be used to wrap all the node functions.
-
-        :raises GraphError if the node names are not unique.
+        :raises InvalidGraphError if the node names are not unique.
         """
-
-        self._check_nodes(nodes)
+        self._check_node_names_are_unique(nodes)
         self.nodes = nodes
         self.wrappers = wrappers
+        self.required_user_inputs = self._get_required_user_inputs()
+        logger.debug(f"Required user input: {self.required_user_inputs}")
+
+    def _get_required_user_inputs(self):
+        node_output_names = [node.output_name for node in self.nodes]
+        required_inputs = []
+        for node in self.nodes:
+            required_inputs += node.inputs
+        return list(set(required_inputs) - set(node_output_names))
 
     def render(self,
                path: str = "graph.gv",
                view: bool = True) -> Optional["Digraph"]:
         """
         Render graph. This will only work if graphviz is available.
         :param path: Path to save fig.
@@ -82,34 +86,39 @@
                     dot.edge(node_input, node.name)
             dot.render(path, view=view)
             return dot
         except Exception as e:
             logger.warning(f"Graph cannot be rendered, caught error: {e}")
             return None
 
-    def check(self, input_data: Optional[dict] = None) -> None:
+    def check(self) -> None:
         """
-        Check if the graph can be executed.
-
-        :param input_data: Input data for graph, where keys are names used in the graph definition.
-
-        :raises GraphError if the graph structure is not valid.
+        Check if the graph structure is valid.
+        :raises InvalidGraphError if the graph structure is not valid.
         """
+        input_data = {name: None for name in self.required_user_inputs}
         self._execute(input_data, False)
 
     def calculate(self, input_data: Optional[dict] = None) -> dict:
         """
         Execute every node in the graph.
         :param input_data: Input data for the graph, where keys are names used in the graph definition.
         :return: Output of every node, with node names as keys.
-
-        :raises GraphError if the graph structure is not valid.
+        :raises MissingInputError if the input_data doesn't contain all the required data.
+        :raises InvalidGraphError if the graph structure is not valid.
         """
+        self._check_input_data(input_data)
         return self._execute(input_data)
 
+    def _check_input_data(self, input_data):
+        if len(self.required_user_inputs) > 0:
+            for item in self.required_user_inputs:
+                if item not in input_data:
+                    raise MissingInputError(f"Input data is missing {item}")
+
     def _execute(self, input_data: Optional[dict] = None, run: Optional[bool] = True) -> dict:
         # Container where all the node inputs will be stored
         # This will be updated when the nodes are executed
         inputs = copy(input_data) if input_data is not None else {}
 
         nodes_to_execute = [i for i in range(len(self.nodes))]
         t_graph_start = time.time()
@@ -128,18 +137,17 @@
                     continue  # All the input data cannot be found for this node yet, so skip this node
                 output = self._run_node(node, node_input_data) if run else "output"
                 inputs[node.output_name] = output
                 nodes_executed.append(node_index)
                 logger.debug(f"Node {node} executed successfully")
 
             # Check that at least one of the nodes has been executed during this round
-            # If not, it means that the graph has invalid struct or that all the inputs are not provided
+            # If not, it means that the graph has invalid structure
             if len(nodes_executed) == 0:
-                raise GraphError(
-                    "Graph cannot be executed! One or multiple inputs are missing or the graph has invalid structure.")
+                raise InvalidGraphError("Graph cannot be executed! The graph has invalid structure.")
 
             for node_index in nodes_executed:
                 nodes_to_execute.remove(node_index)
 
         logger.debug("All nodes executed successfully")
         t_graph_end = time.time()
         logger.debug(f"Graph execution took {1000 * (t_graph_end - t_graph_start): 0.2f} ms")
@@ -174,23 +182,22 @@
             nodes = self.nodes + [nodes]
         return Graph(nodes, self.wrappers)
 
     def __repr__(self) -> str:
         return str([n.name for n in self.nodes])
 
     @staticmethod
-    def _check_nodes(nodes: List[Node]) -> None:
+    def _check_node_names_are_unique(nodes: List[Node]) -> None:
         node_names = [n.name for n in nodes]
         if len(set(node_names)) < len(node_names):
-            raise GraphError("All the nodes need to have unique name!")
+            raise InvalidGraphError("All the nodes need to have unique name!")
 
     @staticmethod
     def _get_node_input_data(node: Node, inputs: dict) -> list:
         input_data = []
         for i in node.inputs:
-            input_item = inputs.get(i, None)
-            if input_item is None:
+            if i in inputs:
+                input_data.append(inputs[i])
+            else:
                 logger.debug(f"Cannot find input {i} for node {node}.")
                 break  # We cannot execute node without full input, so no need to continue
-            else:
-                input_data.append(input_item)
         return input_data
```

### Comparing `tiny_dag-0.0.6/src/tinydag/node.py` & `tiny_dag-0.0.7/src/tinydag/node.py`

 * *Files identical despite different names*

