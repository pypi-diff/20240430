# Comparing `tmp/automotifs-1.4.4.tar.gz` & `tmp/automotifs-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automotifs-1.4.4.tar", last modified: Mon Apr 29 11:11:19 2024, max compression
+gzip compressed data, was "automotifs-1.5.tar", last modified: Mon Apr 29 15:07:41 2024, max compression
```

## Comparing `automotifs-1.4.4.tar` & `automotifs-1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:11:19.243533 automotifs-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-29 11:10:55.000000 automotifs-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-29 11:11:19.243533 automotifs-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-29 11:10:55.000000 automotifs-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:11:19.243533 automotifs-1.4.4/automotif/
--rw-r--r--   0 runner    (1001) docker     (127)    18561 2024-04-29 11:10:55.000000 automotifs-1.4.4/automotif/GPU_Executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-29 11:10:55.000000 automotifs-1.4.4/automotif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17728 2024-04-29 11:10:55.000000 automotifs-1.4.4/automotif/automotif.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:11:19.243533 automotifs-1.4.4/automotifs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-29 11:11:19.000000 automotifs-1.4.4/automotifs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-29 11:11:19.000000 automotifs-1.4.4/automotifs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:11:19.000000 automotifs-1.4.4/automotifs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-29 11:11:19.000000 automotifs-1.4.4/automotifs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 11:11:19.000000 automotifs-1.4.4/automotifs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 11:11:19.243533 automotifs-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-29 11:10:55.000000 automotifs-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:11:19.243533 automotifs-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-29 11:10:55.000000 automotifs-1.4.4/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:41.159351 automotifs-1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-29 15:07:13.000000 automotifs-1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-29 15:07:41.159351 automotifs-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-29 15:07:13.000000 automotifs-1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:41.159351 automotifs-1.5/automotif/
+-rw-r--r--   0 runner    (1001) docker     (127)    18561 2024-04-29 15:07:13.000000 automotifs-1.5/automotif/GPU_Executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-29 15:07:13.000000 automotifs-1.5/automotif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18606 2024-04-29 15:07:13.000000 automotifs-1.5/automotif/automotif.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:41.159351 automotifs-1.5/automotifs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-29 15:07:41.000000 automotifs-1.5/automotifs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-29 15:07:41.000000 automotifs-1.5/automotifs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:07:41.000000 automotifs-1.5/automotifs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-29 15:07:41.000000 automotifs-1.5/automotifs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 15:07:41.000000 automotifs-1.5/automotifs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:07:41.159351 automotifs-1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-29 15:07:13.000000 automotifs-1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:07:41.159351 automotifs-1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-29 15:07:13.000000 automotifs-1.5/tests/test.py
```

### Comparing `automotifs-1.4.4/LICENSE` & `automotifs-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `automotifs-1.4.4/PKG-INFO` & `automotifs-1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automotifs
-Version: 1.4.4
+Version: 1.5
 Summary: A wrapper for automatic Motif Detection
 Home-page: https://github.com/GiorgioMB/auto_dotmotif/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `automotifs-1.4.4/README.md` & `automotifs-1.5/README.md`

 * *Files identical despite different names*

### Comparing `automotifs-1.4.4/automotif/GPU_Executor.py` & `automotifs-1.5/automotif/GPU_Executor.py`

 * *Files identical despite different names*

### Comparing `automotifs-1.4.4/automotif/automotif.py` & `automotifs-1.5/automotif/automotif.py`

 * *Files 9% similar despite different names*

```diff
@@ -102,39 +102,57 @@
         self.generate_required_motifs()
         self.motifs_found = None
         if find:
             return self.find_all_motifs()    
     
     def generate_graphs(self, n: int) -> list:
         """
-        Generate all possible directed graphs for n nodes, ignoring self-loops,
-        and ensure no isolated nodes are present. Each graph is represented by its adjacency matrix.
+        Generate all possible graphs for n nodes, ignoring self-loops.
+        If self.directed is False, generate directed graphs ensuring no isolated nodes.
+        If self.directed is True, generate undirected graphs with symmetric adjacency matrices.
+        Each graph is represented by its adjacency matrix.
         Inputs:
         - n (int): Number of nodes.
         """
-        if self.verbose == True:
-            print("Generating graphs for", n, "nodes")
+        if self.verbose:
+            print("Generating motifs for", n, "nodes")
         graphs = []
-        for edges in product([0, 1], repeat=n*(n-1)):
-            matrix = [[0 for _ in range(n)] for _ in range(n)]
-            edge_index = 0
-            for i in range(n):
-                for j in range(n):
-                    if i != j:  
-                        matrix[i][j] = edges[edge_index]
+        if not self.directed:
+            for edges in product([0, 1], repeat=int(n*(n-1)/2)):
+                matrix = [[0 for _ in range(n)] for _ in range(n)]
+                edge_index = 0
+                for i in range(n):
+                    for j in range(i+1, n):
+                        matrix[i][j] = matrix[j][i] = edges[edge_index]
                         edge_index += 1
-            has_isolated_node = False
-            for i in range(n):
-                if all(matrix[i][j] == 0 for j in range(n)) or all(matrix[j][i] == 0 for j in range(n)):
-                    has_isolated_node = True
-                    break
-            if not has_isolated_node:
-                graphs.append(matrix)
-        if self.verbose == True:
-            print("Generated", len(graphs), "graphs for", n, "nodes")
+                has_isolated_node = False
+                for i in range(n):
+                    if all(matrix[i][j] == 0 for j in range(n)):
+                        has_isolated_node = True
+                        break
+                if not has_isolated_node:
+                    graphs.append(matrix)
+        else:
+            for edges in product([0, 1], repeat=n*(n-1)):
+                matrix = [[0 for _ in range(n)] for _ in range(n)]
+                edge_index = 0
+                for i in range(n):
+                    for j in range(n):
+                        if i != j:
+                            matrix[i][j] = edges[edge_index]
+                            edge_index += 1
+                has_isolated_node = False
+                for i in range(n):
+                    if all(matrix[i][j] == 0 for j in range(n)) or all(matrix[j][i] == 0 for j in range(n)):
+                        has_isolated_node = True
+                        break
+                if not has_isolated_node:
+                    graphs.append(matrix)
+        if self.verbose:
+            print("Generated", len(graphs), "motifs for", n, "nodes")
         return graphs
     
     def matrix_to_motif(self, matrix: list, node_labels: list) -> Motif:
         """
         Convert an adjacency matrix to the specified motif format.
         Inputs:
         - matrix (list): Adjacency matrix.
```

### Comparing `automotifs-1.4.4/automotifs.egg-info/PKG-INFO` & `automotifs-1.5/automotifs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automotifs
-Version: 1.4.4
+Version: 1.5
 Summary: A wrapper for automatic Motif Detection
 Home-page: https://github.com/GiorgioMB/auto_dotmotif/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `automotifs-1.4.4/setup.py` & `automotifs-1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def run(self):
         install.run(self)
         # Running pip install for nx-cugraph with the specified extra index URL
         os.system("pip install nx-cugraph-cu11 --extra-index-url https://pypi.nvidia.com")
 
 setup(
     name='automotifs',
-    version='1.4.4', 
+    version='1.5', 
     packages=find_packages(),
     description='A wrapper for automatic Motif Detection',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Giorgio Micaletto',
     author_email='giorgio.micaletto@studbocconi.it',
     url='https://github.com/GiorgioMB/auto_dotmotif/',
```

### Comparing `automotifs-1.4.4/tests/test.py` & `automotifs-1.5/tests/test.py`

 * *Files identical despite different names*

