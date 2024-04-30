# Comparing `tmp/yedextended-1.0.0.tar.gz` & `tmp/yedextended-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yedextended-1.0.0.tar", last modified: Tue Apr 30 08:22:28 2024, max compression
+gzip compressed data, was "yedextended-1.0.1.tar", last modified: Tue Apr 30 09:21:54 2024, max compression
```

## Comparing `yedextended-1.0.0.tar` & `yedextended-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 08:22:28.407369 yedextended-1.0.0/
--rw-rw-rw-   0        0        0     1611 2024-04-17 13:10:11.000000 yedextended-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     5670 2024-04-30 08:22:28.404814 yedextended-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5010 2024-04-29 12:11:54.000000 yedextended-1.0.0/README.md
--rw-rw-rw-   0        0        0     2024 2024-04-30 08:21:46.000000 yedextended-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 08:22:28.407369 yedextended-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-30 08:22:28.368026 yedextended-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 08:22:28.383613 yedextended-1.0.0/src/yedextended/
--rw-rw-rw-   0        0        0    75125 2024-04-29 11:34:29.000000 yedextended-1.0.0/src/yedextended/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:22:28.404089 yedextended-1.0.0/src/yedextended.egg-info/
--rw-rw-rw-   0        0        0     5670 2024-04-30 08:22:28.000000 yedextended-1.0.0/src/yedextended.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-30 08:22:28.000000 yedextended-1.0.0/src/yedextended.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 08:22:28.000000 yedextended-1.0.0/src/yedextended.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-30 08:22:28.000000 yedextended-1.0.0/src/yedextended.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-30 08:22:28.000000 yedextended-1.0.0/src/yedextended.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-30 08:22:28.401073 yedextended-1.0.0/tests/
--rw-rw-rw-   0        0        0     7166 2024-04-19 09:40:10.000000 yedextended-1.0.0/tests/test_yedextended.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:21:54.756913 yedextended-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-30 09:21:46.000000 yedextended-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-30 09:21:54.756913 yedextended-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-04-30 09:21:46.000000 yedextended-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-30 09:21:46.000000 yedextended-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:21:54.756913 yedextended-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:21:54.756913 yedextended-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:21:54.756913 yedextended-1.0.1/src/yedextended/
+-rw-r--r--   0 runner    (1001) docker     (127)    73127 2024-04-30 09:21:46.000000 yedextended-1.0.1/src/yedextended/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:21:54.756913 yedextended-1.0.1/src/yedextended.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-30 09:21:54.000000 yedextended-1.0.1/src/yedextended.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-30 09:21:54.000000 yedextended-1.0.1/src/yedextended.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:21:54.000000 yedextended-1.0.1/src/yedextended.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 09:21:54.000000 yedextended-1.0.1/src/yedextended.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 09:21:54.000000 yedextended-1.0.1/src/yedextended.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:21:54.756913 yedextended-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-30 09:21:46.000000 yedextended-1.0.1/tests/test_yedextended.py
```

### Comparing `yedextended-1.0.0/LICENSE` & `yedextended-1.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-Copyright (c) 2024, Cole St John
-Copyright (c) 2020, James Scott-Brown & The Pyyed Contributors
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+Copyright (c) 2024, Cole St John
+Copyright (c) 2020, James Scott-Brown & The Pyyed Contributors
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `yedextended-1.0.0/PKG-INFO` & `yedextended-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,235 +1,235 @@
-Metadata-Version: 2.1
-Name: yedextended
-Version: 1.0.0
-Summary: Python library extending yEd functionality through programmatic interface to graphs.
-Author-email: Cole St John <info@colestjohn.com>
-Project-URL: Homepage, https://github.com/cole-st-john/yedextended
-Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: psutil
-Requires-Dist: pygetwindow
-Requires-Dist: openpyxl
-
-# Extended Python Support for yEd 
-
-This Python library extends [yEd](http://www.yworks.com/en/products_yed_about.html) functionality through programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following:
-
-- [x] creating graphs
-- [x] formatting graphs
-- [x] reading graphs
-- [x] bulk data addition or management (MS excel-based)
-- [x] management of the yEd application (starting, killing, maximizing)
-- [ ] enforcing rules on graphs
-- [ ] addition of standard sorting methods
-- [ ] graph comparison tools
-
-![image](images/graph.gif)
-
-
-# Basic Usage
-
-Below are some basic usages of yEdExtended in interfacing with yEd and GraphML files:
-
-
-## Installing yEdExtended
-
-From GITHUB
-```console
-$ python -m pip install git+https://github.com/cole-st-john/yEdExtended
-```
-or *Coming soon, to PyPI!*
-```console
-$ pip install yedextended  
-```
-
-
-## Importing yEdExtended for usage
-
-```python
-import yedextended as yed
-```
-
-
-## Programmatically creating GraphML files
-
-```python
-# Instantiate graph instance
-graph1 = yed.Graph()
-
-# Add arbitrary graph detail - nodes and edges
-graph1.add_node("a")
-graph1.add_node("b")
-graph1.add_edge("a", "b")
-
-# Add arbitrary graph detail - group and group objects
-group1 = graph1.add_group("group 1", shape="rectangle")
-group1.add_node("c")
-group1.add_node("d")
-group1.add_edge("c", "d")
-```
-
-```python
-# Adding graph objects based on csv input
-import csv
-with open("examples/test.csv", encoding="utf-8-sig") as csv_file: 
-	csv_reader = csv.reader(csv_file)
-	for row in csv_reader:
-	    graph1.add_node(row)
-```
-
-## Reading existing GraphML files
-
-```python
-# Read graph file into python graph objects
-graph1 = yed.Graph().from_existing_graph("examples/yed_created_edges.graphml")
-
-```
-
-
-## Using formatting
-
-```python
-# Add graph nodes and edges with some examples of non-default formatting
-graph1.add_node(
-    "foo",
-    font_family="Zapfino",
-)
-
-graph1.add_node(
-    "foo2",
-    shape="roundrectangle",
-    font_style="bolditalic",
-    underlined_text="true",
-)
-
-graph1.add_edge(
-    "foo1",
-    "foo2",
-)
-graph1.add_node(
-    "abc",
-    font_size="72",
-    height="100",
-)
-
-graph1.add_node(
-    "bar",
-    label="Multi\nline\ntext",
-)
-graph1.add_node(
-    "foobar",
-    label="""Multi
-Line
-Text!""",
-)
-
-graph1.add_edge(
-    "foo",
-    "foo1",
-    label="EDGE!",
-    width="3.0",
-    color="#0000FF",
-    arrowhead="white_diamond",
-    arrowfoot="standard",
-    line_type="dotted",
-)
-```
-
-
-## Manipulating data in MS Excel 
-
-```python
-# Manage data in excel (add/remove/modify objects)
-graph1.manage_graph_data_in_excel() # default is object and hierachy management
-
-# Manage data in excel (add/remove/modify relations)
-graph1.manage_graph_data_in_excel(type="relations")
-```
-
-### Adding Objects / Groups per Excel:
-
-![Excel Object Entry](images/excel_obj_entry.gif)
-
-### Result:
-
-![Graph result of excel data entry](images/graph_from_excel_obj.gif)
-
-### Adding Relationships per Excel:
-
-![Excel Relation Entry](images/excel_rel_entry.gif)
-
-### Result:
-
-![Graph result of excel relation entry](images/graph_from_excel_rel.gif)
-
-
-## Possible outputs of Graph
-
-```python
-# Demonstrate stringified GraphML version of structure
-print(graph1.stringify_graph())
-```
-
-```python
-# Several methods of writing graph to file ==============================
-
-with open("test_graph.graphml", "w") as fp:  # using standard python functionality
-    fp.write(graph1.stringify_graph())
-
-graph_file = graph1.persist_graph("test.graphml")   # using tool specific method
-
-graph_file = graph1.persist_graph("pretty_example.graphml", pretty_print=True)  #  tool specific with formatting
-
-```
-
-
-## Opening files in yEd Application *(assumes yEd installed and on PATH)*
-
-```python
-# From existing handle
-graph_file.open_with_yed(force=True)
-
-# From file path
-yed.open_yed_file("examples/test.graphml")
-```
-
-
-## Visualizing in yEd Application (Layout)
-
-Following programmatic creation or modification of a graph, consider using the following keystrokes in yEd to improve layout / positioning:
-
-- ``Tools -> Fit Node to Label``  (_Win: Alt + T + N_)
-- ``Layout -> Hierarchical``  (_Win: Alt + Shift + H_)
-
-
-# Options
-
-Provides comprehensive support for ``node_shapes``, ``line_types``, ``font_styles``, ``arrow_types``, custom parameters, UML, complex and deeply nested relationship structures and more.
-
-
-
-# Development
-
-
-Interested in contributing or co-managing further development?  Just reach out!
-
-Dev. Requirements:
-```console
-$ pip install pytest
-```
-
-To run the tests:
-```console
-$ PYTHONPATH=. pytest tests
-```
-
-References: 
-
-+ [pyyed](https://github.com/jamesscottbrown/pyyed)
-+ [GraphML Primer](http://graphml.graphdrawingraph1.org/primer/graphml-primer.html)
-+ [NetworkX](https://github.com/networkx/networkx)
+Metadata-Version: 2.1
+Name: yedextended
+Version: 1.0.1
+Summary: Python library extending yEd functionality through programmatic interface to graphs.
+Author-email: Cole St John <info@colestjohn.com>
+Project-URL: Homepage, https://github.com/cole-st-john/yedextended
+Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: psutil
+Requires-Dist: pygetwindow
+Requires-Dist: openpyxl
+
+# Extended Python Support for yEd 
+
+This Python library extends [yEd](http://www.yworks.com/en/products_yed_about.html) functionality through programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following:
+
+- [x] creating graphs
+- [x] formatting graphs
+- [x] reading graphs
+- [x] bulk data addition or management (MS excel-based)
+- [x] management of the yEd application (starting, killing, maximizing)
+- [ ] enforcing rules on graphs
+- [ ] addition of standard sorting methods
+- [ ] graph comparison tools
+
+![image](images/graph.gif)
+
+
+# Basic Usage
+
+Below are some basic usages of yEdExtended in interfacing with yEd and GraphML files:
+
+
+## Installing yEdExtended
+
+From GITHUB
+```console
+$ python -m pip install git+https://github.com/cole-st-john/yEdExtended
+```
+or *Coming soon, to PyPI!*
+```console
+$ pip install yedextended  
+```
+
+
+## Importing yEdExtended for usage
+
+```python
+import yedextended as yed
+```
+
+
+## Programmatically creating GraphML files
+
+```python
+# Instantiate graph instance
+graph1 = yed.Graph()
+
+# Add arbitrary graph detail - nodes and edges
+graph1.add_node("a")
+graph1.add_node("b")
+graph1.add_edge("a", "b")
+
+# Add arbitrary graph detail - group and group objects
+group1 = graph1.add_group("group 1", shape="rectangle")
+group1.add_node("c")
+group1.add_node("d")
+group1.add_edge("c", "d")
+```
+
+```python
+# Adding graph objects based on csv input
+import csv
+with open("examples/test.csv", encoding="utf-8-sig") as csv_file: 
+	csv_reader = csv.reader(csv_file)
+	for row in csv_reader:
+	    graph1.add_node(row)
+```
+
+## Reading existing GraphML files
+
+```python
+# Read graph file into python graph objects
+graph1 = yed.Graph().from_existing_graph("examples/yed_created_edges.graphml")
+
+```
+
+
+## Using formatting
+
+```python
+# Add graph nodes and edges with some examples of non-default formatting
+graph1.add_node(
+    "foo",
+    font_family="Zapfino",
+)
+
+graph1.add_node(
+    "foo2",
+    shape="roundrectangle",
+    font_style="bolditalic",
+    underlined_text="true",
+)
+
+graph1.add_edge(
+    "foo1",
+    "foo2",
+)
+graph1.add_node(
+    "abc",
+    font_size="72",
+    height="100",
+)
+
+graph1.add_node(
+    "bar",
+    label="Multi\nline\ntext",
+)
+graph1.add_node(
+    "foobar",
+    label="""Multi
+Line
+Text!""",
+)
+
+graph1.add_edge(
+    "foo",
+    "foo1",
+    label="EDGE!",
+    width="3.0",
+    color="#0000FF",
+    arrowhead="white_diamond",
+    arrowfoot="standard",
+    line_type="dotted",
+)
+```
+
+
+## Manipulating data in MS Excel 
+
+```python
+# Manage data in excel (add/remove/modify objects)
+graph1.manage_graph_data_in_excel() # default is object and hierachy management
+
+# Manage data in excel (add/remove/modify relations)
+graph1.manage_graph_data_in_excel(type="relations")
+```
+
+### Adding Objects / Groups per Excel:
+
+![Excel Object Entry](images/excel_obj_entry.gif)
+
+### Result:
+
+![Graph result of excel data entry](images/graph_from_excel_obj.gif)
+
+### Adding Relationships per Excel:
+
+![Excel Relation Entry](images/excel_rel_entry.gif)
+
+### Result:
+
+![Graph result of excel relation entry](images/graph_from_excel_rel.gif)
+
+
+## Possible outputs of Graph
+
+```python
+# Demonstrate stringified GraphML version of structure
+print(graph1.stringify_graph())
+```
+
+```python
+# Several methods of writing graph to file ==============================
+
+with open("test_graph.graphml", "w") as fp:  # using standard python functionality
+    fp.write(graph1.stringify_graph())
+
+graph_file = graph1.persist_graph("test.graphml")   # using tool specific method
+
+graph_file = graph1.persist_graph("pretty_example.graphml", pretty_print=True)  #  tool specific with formatting
+
+```
+
+
+## Opening files in yEd Application *(assumes yEd installed and on PATH)*
+
+```python
+# From existing handle
+graph_file.open_with_yed(force=True)
+
+# From file path
+yed.open_yed_file("examples/test.graphml")
+```
+
+
+## Visualizing in yEd Application (Layout)
+
+Following programmatic creation or modification of a graph, consider using the following keystrokes in yEd to improve layout / positioning:
+
+- ``Tools -> Fit Node to Label``  (_Win: Alt + T + N_)
+- ``Layout -> Hierarchical``  (_Win: Alt + Shift + H_)
+
+
+# Options
+
+Provides comprehensive support for ``node_shapes``, ``line_types``, ``font_styles``, ``arrow_types``, custom parameters, UML, complex and deeply nested relationship structures and more.
+
+
+
+# Development
+
+
+Interested in contributing or co-managing further development?  Just reach out!
+
+Dev. Requirements:
+```console
+$ pip install pytest
+```
+
+To run the tests:
+```console
+$ PYTHONPATH=. pytest tests
+```
+
+References: 
+
++ [pyyed](https://github.com/jamesscottbrown/pyyed)
++ [GraphML Primer](http://graphml.graphdrawingraph1.org/primer/graphml-primer.html)
++ [NetworkX](https://github.com/networkx/networkx)
```

### Comparing `yedextended-1.0.0/README.md` & `yedextended-1.0.1/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,218 +1,218 @@
-# Extended Python Support for yEd 
-
-This Python library extends [yEd](http://www.yworks.com/en/products_yed_about.html) functionality through programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following:
-
-- [x] creating graphs
-- [x] formatting graphs
-- [x] reading graphs
-- [x] bulk data addition or management (MS excel-based)
-- [x] management of the yEd application (starting, killing, maximizing)
-- [ ] enforcing rules on graphs
-- [ ] addition of standard sorting methods
-- [ ] graph comparison tools
-
-![image](images/graph.gif)
-
-
-# Basic Usage
-
-Below are some basic usages of yEdExtended in interfacing with yEd and GraphML files:
-
-
-## Installing yEdExtended
-
-From GITHUB
-```console
-$ python -m pip install git+https://github.com/cole-st-john/yEdExtended
-```
-or *Coming soon, to PyPI!*
-```console
-$ pip install yedextended  
-```
-
-
-## Importing yEdExtended for usage
-
-```python
-import yedextended as yed
-```
-
-
-## Programmatically creating GraphML files
-
-```python
-# Instantiate graph instance
-graph1 = yed.Graph()
-
-# Add arbitrary graph detail - nodes and edges
-graph1.add_node("a")
-graph1.add_node("b")
-graph1.add_edge("a", "b")
-
-# Add arbitrary graph detail - group and group objects
-group1 = graph1.add_group("group 1", shape="rectangle")
-group1.add_node("c")
-group1.add_node("d")
-group1.add_edge("c", "d")
-```
-
-```python
-# Adding graph objects based on csv input
-import csv
-with open("examples/test.csv", encoding="utf-8-sig") as csv_file: 
-	csv_reader = csv.reader(csv_file)
-	for row in csv_reader:
-	    graph1.add_node(row)
-```
-
-## Reading existing GraphML files
-
-```python
-# Read graph file into python graph objects
-graph1 = yed.Graph().from_existing_graph("examples/yed_created_edges.graphml")
-
-```
-
-
-## Using formatting
-
-```python
-# Add graph nodes and edges with some examples of non-default formatting
-graph1.add_node(
-    "foo",
-    font_family="Zapfino",
-)
-
-graph1.add_node(
-    "foo2",
-    shape="roundrectangle",
-    font_style="bolditalic",
-    underlined_text="true",
-)
-
-graph1.add_edge(
-    "foo1",
-    "foo2",
-)
-graph1.add_node(
-    "abc",
-    font_size="72",
-    height="100",
-)
-
-graph1.add_node(
-    "bar",
-    label="Multi\nline\ntext",
-)
-graph1.add_node(
-    "foobar",
-    label="""Multi
-Line
-Text!""",
-)
-
-graph1.add_edge(
-    "foo",
-    "foo1",
-    label="EDGE!",
-    width="3.0",
-    color="#0000FF",
-    arrowhead="white_diamond",
-    arrowfoot="standard",
-    line_type="dotted",
-)
-```
-
-
-## Manipulating data in MS Excel 
-
-```python
-# Manage data in excel (add/remove/modify objects)
-graph1.manage_graph_data_in_excel() # default is object and hierachy management
-
-# Manage data in excel (add/remove/modify relations)
-graph1.manage_graph_data_in_excel(type="relations")
-```
-
-### Adding Objects / Groups per Excel:
-
-![Excel Object Entry](images/excel_obj_entry.gif)
-
-### Result:
-
-![Graph result of excel data entry](images/graph_from_excel_obj.gif)
-
-### Adding Relationships per Excel:
-
-![Excel Relation Entry](images/excel_rel_entry.gif)
-
-### Result:
-
-![Graph result of excel relation entry](images/graph_from_excel_rel.gif)
-
-
-## Possible outputs of Graph
-
-```python
-# Demonstrate stringified GraphML version of structure
-print(graph1.stringify_graph())
-```
-
-```python
-# Several methods of writing graph to file ==============================
-
-with open("test_graph.graphml", "w") as fp:  # using standard python functionality
-    fp.write(graph1.stringify_graph())
-
-graph_file = graph1.persist_graph("test.graphml")   # using tool specific method
-
-graph_file = graph1.persist_graph("pretty_example.graphml", pretty_print=True)  #  tool specific with formatting
-
-```
-
-
-## Opening files in yEd Application *(assumes yEd installed and on PATH)*
-
-```python
-# From existing handle
-graph_file.open_with_yed(force=True)
-
-# From file path
-yed.open_yed_file("examples/test.graphml")
-```
-
-
-## Visualizing in yEd Application (Layout)
-
-Following programmatic creation or modification of a graph, consider using the following keystrokes in yEd to improve layout / positioning:
-
-- ``Tools -> Fit Node to Label``  (_Win: Alt + T + N_)
-- ``Layout -> Hierarchical``  (_Win: Alt + Shift + H_)
-
-
-# Options
-
-Provides comprehensive support for ``node_shapes``, ``line_types``, ``font_styles``, ``arrow_types``, custom parameters, UML, complex and deeply nested relationship structures and more.
-
-
-
-# Development
-
-
-Interested in contributing or co-managing further development?  Just reach out!
-
-Dev. Requirements:
-```console
-$ pip install pytest
-```
-
-To run the tests:
-```console
-$ PYTHONPATH=. pytest tests
-```
-
-References: 
-
-+ [pyyed](https://github.com/jamesscottbrown/pyyed)
-+ [GraphML Primer](http://graphml.graphdrawingraph1.org/primer/graphml-primer.html)
-+ [NetworkX](https://github.com/networkx/networkx)
+# Extended Python Support for yEd 
+
+This Python library extends [yEd](http://www.yworks.com/en/products_yed_about.html) functionality through programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following:
+
+- [x] creating graphs
+- [x] formatting graphs
+- [x] reading graphs
+- [x] bulk data addition or management (MS excel-based)
+- [x] management of the yEd application (starting, killing, maximizing)
+- [ ] enforcing rules on graphs
+- [ ] addition of standard sorting methods
+- [ ] graph comparison tools
+
+![image](images/graph.gif)
+
+
+# Basic Usage
+
+Below are some basic usages of yEdExtended in interfacing with yEd and GraphML files:
+
+
+## Installing yEdExtended
+
+From GITHUB
+```console
+$ python -m pip install git+https://github.com/cole-st-john/yEdExtended
+```
+or *Coming soon, to PyPI!*
+```console
+$ pip install yedextended  
+```
+
+
+## Importing yEdExtended for usage
+
+```python
+import yedextended as yed
+```
+
+
+## Programmatically creating GraphML files
+
+```python
+# Instantiate graph instance
+graph1 = yed.Graph()
+
+# Add arbitrary graph detail - nodes and edges
+graph1.add_node("a")
+graph1.add_node("b")
+graph1.add_edge("a", "b")
+
+# Add arbitrary graph detail - group and group objects
+group1 = graph1.add_group("group 1", shape="rectangle")
+group1.add_node("c")
+group1.add_node("d")
+group1.add_edge("c", "d")
+```
+
+```python
+# Adding graph objects based on csv input
+import csv
+with open("examples/test.csv", encoding="utf-8-sig") as csv_file: 
+	csv_reader = csv.reader(csv_file)
+	for row in csv_reader:
+	    graph1.add_node(row)
+```
+
+## Reading existing GraphML files
+
+```python
+# Read graph file into python graph objects
+graph1 = yed.Graph().from_existing_graph("examples/yed_created_edges.graphml")
+
+```
+
+
+## Using formatting
+
+```python
+# Add graph nodes and edges with some examples of non-default formatting
+graph1.add_node(
+    "foo",
+    font_family="Zapfino",
+)
+
+graph1.add_node(
+    "foo2",
+    shape="roundrectangle",
+    font_style="bolditalic",
+    underlined_text="true",
+)
+
+graph1.add_edge(
+    "foo1",
+    "foo2",
+)
+graph1.add_node(
+    "abc",
+    font_size="72",
+    height="100",
+)
+
+graph1.add_node(
+    "bar",
+    label="Multi\nline\ntext",
+)
+graph1.add_node(
+    "foobar",
+    label="""Multi
+Line
+Text!""",
+)
+
+graph1.add_edge(
+    "foo",
+    "foo1",
+    label="EDGE!",
+    width="3.0",
+    color="#0000FF",
+    arrowhead="white_diamond",
+    arrowfoot="standard",
+    line_type="dotted",
+)
+```
+
+
+## Manipulating data in MS Excel 
+
+```python
+# Manage data in excel (add/remove/modify objects)
+graph1.manage_graph_data_in_excel() # default is object and hierachy management
+
+# Manage data in excel (add/remove/modify relations)
+graph1.manage_graph_data_in_excel(type="relations")
+```
+
+### Adding Objects / Groups per Excel:
+
+![Excel Object Entry](images/excel_obj_entry.gif)
+
+### Result:
+
+![Graph result of excel data entry](images/graph_from_excel_obj.gif)
+
+### Adding Relationships per Excel:
+
+![Excel Relation Entry](images/excel_rel_entry.gif)
+
+### Result:
+
+![Graph result of excel relation entry](images/graph_from_excel_rel.gif)
+
+
+## Possible outputs of Graph
+
+```python
+# Demonstrate stringified GraphML version of structure
+print(graph1.stringify_graph())
+```
+
+```python
+# Several methods of writing graph to file ==============================
+
+with open("test_graph.graphml", "w") as fp:  # using standard python functionality
+    fp.write(graph1.stringify_graph())
+
+graph_file = graph1.persist_graph("test.graphml")   # using tool specific method
+
+graph_file = graph1.persist_graph("pretty_example.graphml", pretty_print=True)  #  tool specific with formatting
+
+```
+
+
+## Opening files in yEd Application *(assumes yEd installed and on PATH)*
+
+```python
+# From existing handle
+graph_file.open_with_yed(force=True)
+
+# From file path
+yed.open_yed_file("examples/test.graphml")
+```
+
+
+## Visualizing in yEd Application (Layout)
+
+Following programmatic creation or modification of a graph, consider using the following keystrokes in yEd to improve layout / positioning:
+
+- ``Tools -> Fit Node to Label``  (_Win: Alt + T + N_)
+- ``Layout -> Hierarchical``  (_Win: Alt + Shift + H_)
+
+
+# Options
+
+Provides comprehensive support for ``node_shapes``, ``line_types``, ``font_styles``, ``arrow_types``, custom parameters, UML, complex and deeply nested relationship structures and more.
+
+
+
+# Development
+
+
+Interested in contributing or co-managing further development?  Just reach out!
+
+Dev. Requirements:
+```console
+$ pip install pytest
+```
+
+To run the tests:
+```console
+$ PYTHONPATH=. pytest tests
+```
+
+References: 
+
++ [pyyed](https://github.com/jamesscottbrown/pyyed)
++ [GraphML Primer](http://graphml.graphdrawingraph1.org/primer/graphml-primer.html)
++ [NetworkX](https://github.com/networkx/networkx)
```

### Comparing `yedextended-1.0.0/src/yedextended.egg-info/PKG-INFO` & `yedextended-1.0.1/src/yedextended.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,235 +1,235 @@
-Metadata-Version: 2.1
-Name: yedextended
-Version: 1.0.0
-Summary: Python library extending yEd functionality through programmatic interface to graphs.
-Author-email: Cole St John <info@colestjohn.com>
-Project-URL: Homepage, https://github.com/cole-st-john/yedextended
-Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: psutil
-Requires-Dist: pygetwindow
-Requires-Dist: openpyxl
-
-# Extended Python Support for yEd 
-
-This Python library extends [yEd](http://www.yworks.com/en/products_yed_about.html) functionality through programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following:
-
-- [x] creating graphs
-- [x] formatting graphs
-- [x] reading graphs
-- [x] bulk data addition or management (MS excel-based)
-- [x] management of the yEd application (starting, killing, maximizing)
-- [ ] enforcing rules on graphs
-- [ ] addition of standard sorting methods
-- [ ] graph comparison tools
-
-![image](images/graph.gif)
-
-
-# Basic Usage
-
-Below are some basic usages of yEdExtended in interfacing with yEd and GraphML files:
-
-
-## Installing yEdExtended
-
-From GITHUB
-```console
-$ python -m pip install git+https://github.com/cole-st-john/yEdExtended
-```
-or *Coming soon, to PyPI!*
-```console
-$ pip install yedextended  
-```
-
-
-## Importing yEdExtended for usage
-
-```python
-import yedextended as yed
-```
-
-
-## Programmatically creating GraphML files
-
-```python
-# Instantiate graph instance
-graph1 = yed.Graph()
-
-# Add arbitrary graph detail - nodes and edges
-graph1.add_node("a")
-graph1.add_node("b")
-graph1.add_edge("a", "b")
-
-# Add arbitrary graph detail - group and group objects
-group1 = graph1.add_group("group 1", shape="rectangle")
-group1.add_node("c")
-group1.add_node("d")
-group1.add_edge("c", "d")
-```
-
-```python
-# Adding graph objects based on csv input
-import csv
-with open("examples/test.csv", encoding="utf-8-sig") as csv_file: 
-	csv_reader = csv.reader(csv_file)
-	for row in csv_reader:
-	    graph1.add_node(row)
-```
-
-## Reading existing GraphML files
-
-```python
-# Read graph file into python graph objects
-graph1 = yed.Graph().from_existing_graph("examples/yed_created_edges.graphml")
-
-```
-
-
-## Using formatting
-
-```python
-# Add graph nodes and edges with some examples of non-default formatting
-graph1.add_node(
-    "foo",
-    font_family="Zapfino",
-)
-
-graph1.add_node(
-    "foo2",
-    shape="roundrectangle",
-    font_style="bolditalic",
-    underlined_text="true",
-)
-
-graph1.add_edge(
-    "foo1",
-    "foo2",
-)
-graph1.add_node(
-    "abc",
-    font_size="72",
-    height="100",
-)
-
-graph1.add_node(
-    "bar",
-    label="Multi\nline\ntext",
-)
-graph1.add_node(
-    "foobar",
-    label="""Multi
-Line
-Text!""",
-)
-
-graph1.add_edge(
-    "foo",
-    "foo1",
-    label="EDGE!",
-    width="3.0",
-    color="#0000FF",
-    arrowhead="white_diamond",
-    arrowfoot="standard",
-    line_type="dotted",
-)
-```
-
-
-## Manipulating data in MS Excel 
-
-```python
-# Manage data in excel (add/remove/modify objects)
-graph1.manage_graph_data_in_excel() # default is object and hierachy management
-
-# Manage data in excel (add/remove/modify relations)
-graph1.manage_graph_data_in_excel(type="relations")
-```
-
-### Adding Objects / Groups per Excel:
-
-![Excel Object Entry](images/excel_obj_entry.gif)
-
-### Result:
-
-![Graph result of excel data entry](images/graph_from_excel_obj.gif)
-
-### Adding Relationships per Excel:
-
-![Excel Relation Entry](images/excel_rel_entry.gif)
-
-### Result:
-
-![Graph result of excel relation entry](images/graph_from_excel_rel.gif)
-
-
-## Possible outputs of Graph
-
-```python
-# Demonstrate stringified GraphML version of structure
-print(graph1.stringify_graph())
-```
-
-```python
-# Several methods of writing graph to file ==============================
-
-with open("test_graph.graphml", "w") as fp:  # using standard python functionality
-    fp.write(graph1.stringify_graph())
-
-graph_file = graph1.persist_graph("test.graphml")   # using tool specific method
-
-graph_file = graph1.persist_graph("pretty_example.graphml", pretty_print=True)  #  tool specific with formatting
-
-```
-
-
-## Opening files in yEd Application *(assumes yEd installed and on PATH)*
-
-```python
-# From existing handle
-graph_file.open_with_yed(force=True)
-
-# From file path
-yed.open_yed_file("examples/test.graphml")
-```
-
-
-## Visualizing in yEd Application (Layout)
-
-Following programmatic creation or modification of a graph, consider using the following keystrokes in yEd to improve layout / positioning:
-
-- ``Tools -> Fit Node to Label``  (_Win: Alt + T + N_)
-- ``Layout -> Hierarchical``  (_Win: Alt + Shift + H_)
-
-
-# Options
-
-Provides comprehensive support for ``node_shapes``, ``line_types``, ``font_styles``, ``arrow_types``, custom parameters, UML, complex and deeply nested relationship structures and more.
-
-
-
-# Development
-
-
-Interested in contributing or co-managing further development?  Just reach out!
-
-Dev. Requirements:
-```console
-$ pip install pytest
-```
-
-To run the tests:
-```console
-$ PYTHONPATH=. pytest tests
-```
-
-References: 
-
-+ [pyyed](https://github.com/jamesscottbrown/pyyed)
-+ [GraphML Primer](http://graphml.graphdrawingraph1.org/primer/graphml-primer.html)
-+ [NetworkX](https://github.com/networkx/networkx)
+Metadata-Version: 2.1
+Name: yedextended
+Version: 1.0.1
+Summary: Python library extending yEd functionality through programmatic interface to graphs.
+Author-email: Cole St John <info@colestjohn.com>
+Project-URL: Homepage, https://github.com/cole-st-john/yedextended
+Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: psutil
+Requires-Dist: pygetwindow
+Requires-Dist: openpyxl
+
+# Extended Python Support for yEd 
+
+This Python library extends [yEd](http://www.yworks.com/en/products_yed_about.html) functionality through programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following:
+
+- [x] creating graphs
+- [x] formatting graphs
+- [x] reading graphs
+- [x] bulk data addition or management (MS excel-based)
+- [x] management of the yEd application (starting, killing, maximizing)
+- [ ] enforcing rules on graphs
+- [ ] addition of standard sorting methods
+- [ ] graph comparison tools
+
+![image](images/graph.gif)
+
+
+# Basic Usage
+
+Below are some basic usages of yEdExtended in interfacing with yEd and GraphML files:
+
+
+## Installing yEdExtended
+
+From GITHUB
+```console
+$ python -m pip install git+https://github.com/cole-st-john/yEdExtended
+```
+or *Coming soon, to PyPI!*
+```console
+$ pip install yedextended  
+```
+
+
+## Importing yEdExtended for usage
+
+```python
+import yedextended as yed
+```
+
+
+## Programmatically creating GraphML files
+
+```python
+# Instantiate graph instance
+graph1 = yed.Graph()
+
+# Add arbitrary graph detail - nodes and edges
+graph1.add_node("a")
+graph1.add_node("b")
+graph1.add_edge("a", "b")
+
+# Add arbitrary graph detail - group and group objects
+group1 = graph1.add_group("group 1", shape="rectangle")
+group1.add_node("c")
+group1.add_node("d")
+group1.add_edge("c", "d")
+```
+
+```python
+# Adding graph objects based on csv input
+import csv
+with open("examples/test.csv", encoding="utf-8-sig") as csv_file: 
+	csv_reader = csv.reader(csv_file)
+	for row in csv_reader:
+	    graph1.add_node(row)
+```
+
+## Reading existing GraphML files
+
+```python
+# Read graph file into python graph objects
+graph1 = yed.Graph().from_existing_graph("examples/yed_created_edges.graphml")
+
+```
+
+
+## Using formatting
+
+```python
+# Add graph nodes and edges with some examples of non-default formatting
+graph1.add_node(
+    "foo",
+    font_family="Zapfino",
+)
+
+graph1.add_node(
+    "foo2",
+    shape="roundrectangle",
+    font_style="bolditalic",
+    underlined_text="true",
+)
+
+graph1.add_edge(
+    "foo1",
+    "foo2",
+)
+graph1.add_node(
+    "abc",
+    font_size="72",
+    height="100",
+)
+
+graph1.add_node(
+    "bar",
+    label="Multi\nline\ntext",
+)
+graph1.add_node(
+    "foobar",
+    label="""Multi
+Line
+Text!""",
+)
+
+graph1.add_edge(
+    "foo",
+    "foo1",
+    label="EDGE!",
+    width="3.0",
+    color="#0000FF",
+    arrowhead="white_diamond",
+    arrowfoot="standard",
+    line_type="dotted",
+)
+```
+
+
+## Manipulating data in MS Excel 
+
+```python
+# Manage data in excel (add/remove/modify objects)
+graph1.manage_graph_data_in_excel() # default is object and hierachy management
+
+# Manage data in excel (add/remove/modify relations)
+graph1.manage_graph_data_in_excel(type="relations")
+```
+
+### Adding Objects / Groups per Excel:
+
+![Excel Object Entry](images/excel_obj_entry.gif)
+
+### Result:
+
+![Graph result of excel data entry](images/graph_from_excel_obj.gif)
+
+### Adding Relationships per Excel:
+
+![Excel Relation Entry](images/excel_rel_entry.gif)
+
+### Result:
+
+![Graph result of excel relation entry](images/graph_from_excel_rel.gif)
+
+
+## Possible outputs of Graph
+
+```python
+# Demonstrate stringified GraphML version of structure
+print(graph1.stringify_graph())
+```
+
+```python
+# Several methods of writing graph to file ==============================
+
+with open("test_graph.graphml", "w") as fp:  # using standard python functionality
+    fp.write(graph1.stringify_graph())
+
+graph_file = graph1.persist_graph("test.graphml")   # using tool specific method
+
+graph_file = graph1.persist_graph("pretty_example.graphml", pretty_print=True)  #  tool specific with formatting
+
+```
+
+
+## Opening files in yEd Application *(assumes yEd installed and on PATH)*
+
+```python
+# From existing handle
+graph_file.open_with_yed(force=True)
+
+# From file path
+yed.open_yed_file("examples/test.graphml")
+```
+
+
+## Visualizing in yEd Application (Layout)
+
+Following programmatic creation or modification of a graph, consider using the following keystrokes in yEd to improve layout / positioning:
+
+- ``Tools -> Fit Node to Label``  (_Win: Alt + T + N_)
+- ``Layout -> Hierarchical``  (_Win: Alt + Shift + H_)
+
+
+# Options
+
+Provides comprehensive support for ``node_shapes``, ``line_types``, ``font_styles``, ``arrow_types``, custom parameters, UML, complex and deeply nested relationship structures and more.
+
+
+
+# Development
+
+
+Interested in contributing or co-managing further development?  Just reach out!
+
+Dev. Requirements:
+```console
+$ pip install pytest
+```
+
+To run the tests:
+```console
+$ PYTHONPATH=. pytest tests
+```
+
+References: 
+
++ [pyyed](https://github.com/jamesscottbrown/pyyed)
++ [GraphML Primer](http://graphml.graphdrawingraph1.org/primer/graphml-primer.html)
++ [NetworkX](https://github.com/networkx/networkx)
```

