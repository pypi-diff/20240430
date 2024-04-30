# Comparing `tmp/plastexdepgraph-0.0.3.tar.gz` & `tmp/plastexdepgraph-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pmassot/soft/plastexdepgraph/dist/.tmp-1x05smms/plastexdepgraph-0.0.3.tar", last modified: Tue Jan 30 23:18:38 2024, max compression
+gzip compressed data, was "/home/pmassot/soft/plastexdepgraph/dist/.tmp-3tjptd87/plastexdepgraph-0.0.4.tar", last modified: Tue Apr 30 03:00:30 2024, max compression
```

## Comparing `plastexdepgraph-0.0.3.tar` & `plastexdepgraph-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-01-30 23:18:38.075643 plastexdepgraph-0.0.3/
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      124 2024-01-30 22:47:00.000000 plastexdepgraph-0.0.3/MANIFEST.in
--rw-r--r--   0 pmassot   (1000) pmassot   (1000)      796 2024-01-30 23:18:38.075643 plastexdepgraph-0.0.3/PKG-INFO
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      344 2024-01-11 20:09:50.000000 plastexdepgraph-0.0.3/README.md
-drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-01-30 23:18:38.071643 plastexdepgraph-0.0.3/plastexdepgraph/
-drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-01-30 23:18:38.071643 plastexdepgraph-0.0.3/plastexdepgraph/Packages/
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)    14081 2024-01-11 20:09:12.000000 plastexdepgraph-0.0.3/plastexdepgraph/Packages/depgraph.py
-drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-01-30 23:18:38.071643 plastexdepgraph-0.0.3/plastexdepgraph/Packages/renderer_templates/
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       26 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.3/plastexdepgraph/Packages/renderer_templates/depgraph.jinja2s
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        0 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.3/plastexdepgraph/__init__.py
-drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-01-30 23:18:38.075643 plastexdepgraph-0.0.3/plastexdepgraph/static/
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)    80111 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.3/plastexdepgraph/static/d3-graphviz.js
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)   157612 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.3/plastexdepgraph/static/d3-graphviz.js.map
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)   247829 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.3/plastexdepgraph/static/d3.min.js
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)     2950 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.3/plastexdepgraph/static/dep_graph.css
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)   100896 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.3/plastexdepgraph/static/expatlib.wasm
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)  1099314 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.3/plastexdepgraph/static/graphvizlib.wasm
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)   117436 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.3/plastexdepgraph/static/hpcc.min.js
-drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-01-30 23:18:38.075643 plastexdepgraph-0.0.3/plastexdepgraph/templates/
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)     4612 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.3/plastexdepgraph/templates/dep_graph.html
-drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-01-30 23:18:38.075643 plastexdepgraph-0.0.3/plastexdepgraph.egg-info/
--rw-r--r--   0 pmassot   (1000) pmassot   (1000)      796 2024-01-30 23:18:38.000000 plastexdepgraph-0.0.3/plastexdepgraph.egg-info/PKG-INFO
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      716 2024-01-30 23:18:38.000000 plastexdepgraph-0.0.3/plastexdepgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        1 2024-01-30 23:18:38.000000 plastexdepgraph-0.0.3/plastexdepgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        1 2024-01-30 22:50:56.000000 plastexdepgraph-0.0.3/plastexdepgraph.egg-info/not-zip-safe
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       24 2024-01-30 23:18:38.000000 plastexdepgraph-0.0.3/plastexdepgraph.egg-info/requires.txt
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       16 2024-01-30 23:18:38.000000 plastexdepgraph-0.0.3/plastexdepgraph.egg-info/top_level.txt
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       82 2024-01-30 22:54:11.000000 plastexdepgraph-0.0.3/pyproject.toml
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      556 2024-01-30 23:18:38.075643 plastexdepgraph-0.0.3/setup.cfg
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       71 2024-01-30 22:45:00.000000 plastexdepgraph-0.0.3/setup.py
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 03:00:30.306811 plastexdepgraph-0.0.4/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)    11357 2024-02-15 15:15:10.000000 plastexdepgraph-0.0.4/LICENSE
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      124 2024-01-30 22:47:00.000000 plastexdepgraph-0.0.4/MANIFEST.in
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       36 2024-02-15 15:19:16.000000 plastexdepgraph-0.0.4/NOTICE
+-rw-r--r--   0 pmassot   (1000) pmassot   (1000)      839 2024-04-30 03:00:30.306811 plastexdepgraph-0.0.4/PKG-INFO
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      344 2024-01-11 20:09:50.000000 plastexdepgraph-0.0.4/README.md
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 03:00:30.302811 plastexdepgraph-0.0.4/plastexdepgraph/
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 03:00:30.302811 plastexdepgraph-0.0.4/plastexdepgraph/Packages/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)    14552 2024-04-29 20:11:39.000000 plastexdepgraph-0.0.4/plastexdepgraph/Packages/depgraph.py
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 03:00:30.302811 plastexdepgraph-0.0.4/plastexdepgraph/Packages/renderer_templates/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       26 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.4/plastexdepgraph/Packages/renderer_templates/depgraph.jinja2s
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        0 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.4/plastexdepgraph/__init__.py
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 03:00:30.306811 plastexdepgraph-0.0.4/plastexdepgraph/static/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)    80111 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.4/plastexdepgraph/static/d3-graphviz.js
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)   157612 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.4/plastexdepgraph/static/d3-graphviz.js.map
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)   247829 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.4/plastexdepgraph/static/d3.min.js
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)     2950 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.4/plastexdepgraph/static/dep_graph.css
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)   100896 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.4/plastexdepgraph/static/expatlib.wasm
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)  1099314 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.4/plastexdepgraph/static/graphvizlib.wasm
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)   117436 2024-01-05 14:28:25.000000 plastexdepgraph-0.0.4/plastexdepgraph/static/hpcc.min.js
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 03:00:30.306811 plastexdepgraph-0.0.4/plastexdepgraph/templates/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)     4635 2024-04-29 20:11:39.000000 plastexdepgraph-0.0.4/plastexdepgraph/templates/dep_graph.html
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 03:00:30.306811 plastexdepgraph-0.0.4/plastexdepgraph.egg-info/
+-rw-r--r--   0 pmassot   (1000) pmassot   (1000)      839 2024-04-30 03:00:30.000000 plastexdepgraph-0.0.4/plastexdepgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      731 2024-04-30 03:00:30.000000 plastexdepgraph-0.0.4/plastexdepgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        1 2024-04-30 03:00:30.000000 plastexdepgraph-0.0.4/plastexdepgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        1 2024-01-30 22:50:56.000000 plastexdepgraph-0.0.4/plastexdepgraph.egg-info/not-zip-safe
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       24 2024-04-30 03:00:30.000000 plastexdepgraph-0.0.4/plastexdepgraph.egg-info/requires.txt
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       16 2024-04-30 03:00:30.000000 plastexdepgraph-0.0.4/plastexdepgraph.egg-info/top_level.txt
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       82 2024-01-30 22:54:11.000000 plastexdepgraph-0.0.4/pyproject.toml
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      556 2024-04-30 03:00:30.306811 plastexdepgraph-0.0.4/setup.cfg
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       71 2024-01-30 22:45:00.000000 plastexdepgraph-0.0.4/setup.py
```

### Comparing `plastexdepgraph-0.0.3/PKG-INFO` & `plastexdepgraph-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: plastexdepgraph
-Version: 0.0.3
+Version: 0.0.4
 Summary: Dependency graph plugin for plasTeX.
 Home-page: https://github.com/PatrickMassot/plastexdepgraph
 Author: Patrick Massot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
 Requires-Dist: plasTeX>=3.1
 Requires-Dist: pygraphviz
 
 # plasTeX dependency graphs
 
 This is a [plasTeX](https://github.com/plastex/plastex/) plugin allowing
 to build dependency graphs.
```

### Comparing `plastexdepgraph-0.0.3/plastexdepgraph/Packages/depgraph.py` & `plastexdepgraph-0.0.4/plastexdepgraph/Packages/depgraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,18 +20,24 @@
 want to influence the dependency graph.
 
 * document.userdata['dep_graph']['shapes'] can be a dictionary whose keys are node
   kinds as strings and whose values are strings descripting graphviz shapes
   (see https://graphviz.org/doc/info/shapes.html).
   By default, everything uses an ellipse except definition which uses a box.
 
-* document.userdata['dep_graph']['colorizer'] and
-  document.userdata['dep_graph']['fillcolorizer'] can be functions taking as
-  input a plasTeX node and outputting CSS colors for the boundary and interior
-  of graph nodes respectively.
+* document.userdata['dep_graph']['colorizer'] can be a function taking as input
+  a plasTeX node and outputting a CSS color for the boundary of graph nodes.
+
+* document.userdata['dep_graph']['fillcolorizer'] can be a function taking as
+  input a plasTeX node and outputting a CSS color for the interior of graph
+  nodes.
+
+* document.userdata['dep_graph']['stylerizer'] can be a function taking as input
+  a plasTeX node and outputting a graphviz style
+  (see https://graphviz.org/docs/attr-types/style/).
 
 * document.userdata['dep_graph']['legend'] can be a list whose entries are pairs
   made of a visual description and an explanation.
   The default value is:
   [('Boxes', 'definitions'), ('Ellipses', 'theorems and lemmas')]
   Additional entries can also refer to colors.
 
@@ -112,25 +118,28 @@
         graph.node_attr['penwidth'] = 1.8
         graph.edge_attr.update(arrowhead='vee')
         for node in self.nodes:
             color = self.document.userdata['dep_graph'].get('colorizer', lambda x: '')(node)
             fillcolor = self.document.userdata['dep_graph'].get('fillcolorizer', lambda x: '')(node)
 
             if fillcolor:
+                style = self.document.userdata['dep_graph'].get('stylerizer', lambda x: 'filled')(node)
+
                 graph.add_node(node.id,
                                label=node.id.split(':')[-1],
                                shape=shapes.get(item_kind(node), 'ellipse'),
-                               style='filled',
+                               style=style,
                                color=color,
                                fillcolor=fillcolor)
             else:
+                style = self.document.userdata['dep_graph'].get('stylerizer', lambda x: '')(node)
                 graph.add_node(node.id,
                                label=node.id.split(':')[-1],
                                shape=shapes.get(item_kind(node), 'ellipse'),
-                               style='',
+                               style=style,
                                color=color)
         for s, t in self.edges:
             if s in self.nodes and t in self.nodes:
                 graph.add_edge(s.id, t.id, style='dashed')
         for s, t in self.proof_edges:
             if s in self.nodes and t in self.nodes:
                 graph.add_edge(s.id, t.id)
```

### Comparing `plastexdepgraph-0.0.3/plastexdepgraph/static/d3-graphviz.js` & `plastexdepgraph-0.0.4/plastexdepgraph/static/d3-graphviz.js`

 * *Files identical despite different names*

### Comparing `plastexdepgraph-0.0.3/plastexdepgraph/static/d3-graphviz.js.map` & `plastexdepgraph-0.0.4/plastexdepgraph/static/d3-graphviz.js.map`

 * *Files identical despite different names*

### Comparing `plastexdepgraph-0.0.3/plastexdepgraph/static/d3.min.js` & `plastexdepgraph-0.0.4/plastexdepgraph/static/d3.min.js`

 * *Files identical despite different names*

### Comparing `plastexdepgraph-0.0.3/plastexdepgraph/static/dep_graph.css` & `plastexdepgraph-0.0.4/plastexdepgraph/static/dep_graph.css`

 * *Files identical despite different names*

### Comparing `plastexdepgraph-0.0.3/plastexdepgraph/static/expatlib.wasm` & `plastexdepgraph-0.0.4/plastexdepgraph/static/expatlib.wasm`

 * *Files identical despite different names*

### Comparing `plastexdepgraph-0.0.3/plastexdepgraph/static/graphvizlib.wasm` & `plastexdepgraph-0.0.4/plastexdepgraph/static/graphvizlib.wasm`

 * *Files identical despite different names*

### Comparing `plastexdepgraph-0.0.3/plastexdepgraph/static/hpcc.min.js` & `plastexdepgraph-0.0.4/plastexdepgraph/static/hpcc.min.js`

 * *Files identical despite different names*

### Comparing `plastexdepgraph-0.0.3/plastexdepgraph/templates/dep_graph.html` & `plastexdepgraph-0.0.4/plastexdepgraph/templates/dep_graph.html`

 * *Files 9% similar despite different names*

```diff
@@ -107,34 +107,36 @@
 graphContainer.graphviz({useWorker: true})
     .width(width)
     .height(height)
     .fit(true)
     .renderDot(`{{ dot.replace('\n','') }}`)
     .on("end", interactive);
 
+latexLabelEscaper = function(label) {
+  return label.replace(/\./g, '\\.').replace(/:/g, '\\:')
+}
+
 clickNode = function() {
   $("#statements div").hide()
   var node_id = $('text', this).text();
-    console.log(node_id);
-  console.log('#'+node_id.replace(':', '\\:'));
   $('.thm').hide();
-  $('#'+node_id.replace(':', '\\:')).show().children().show();
+  $('#'+latexLabelEscaper(node_id)).show().children().show();
 }
 function interactive() {
     $("span#legend_title").on("click", function () {
            $(this).siblings('dl').toggle();
         })
 
     d3.selectAll('.node')
         .attr('pointer-events', 'fill')
         .on('click', function () {
            var title = d3.select(this).selectAll('title').text().trim();
            $('#statements > div').hide()
            $('.thm').hide();
-           $('#'+title.replace(':', '\\:')+'_modal').show().children().show().children().show();
+           $('#'+latexLabelEscaper(title)+'_modal').show().children().show().children().show();
            $('#statements').show()
         });
 
     d3.selectAll('.dep-closebtn').on('click', function() {
         var modal =
             d3.select(this).node().parentNode.parentNode.parentNode ;
         d3.select(modal).style('display', 'none');
```

### Comparing `plastexdepgraph-0.0.3/plastexdepgraph.egg-info/PKG-INFO` & `plastexdepgraph-0.0.4/plastexdepgraph.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: plastexdepgraph
-Version: 0.0.3
+Version: 0.0.4
 Summary: Dependency graph plugin for plasTeX.
 Home-page: https://github.com/PatrickMassot/plastexdepgraph
 Author: Patrick Massot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
 Requires-Dist: plasTeX>=3.1
 Requires-Dist: pygraphviz
 
 # plasTeX dependency graphs
 
 This is a [plasTeX](https://github.com/plastex/plastex/) plugin allowing
 to build dependency graphs.
```

### Comparing `plastexdepgraph-0.0.3/plastexdepgraph.egg-info/SOURCES.txt` & `plastexdepgraph-0.0.4/plastexdepgraph.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+LICENSE
 MANIFEST.in
+NOTICE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 plastexdepgraph/__init__.py
 plastexdepgraph.egg-info/PKG-INFO
 plastexdepgraph.egg-info/SOURCES.txt
```

### Comparing `plastexdepgraph-0.0.3/setup.cfg` & `plastexdepgraph-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = plastexdepgraph
 description = Dependency graph plugin for plasTeX.
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.0.3
+version = 0.0.4
 author = Patrick Massot
 url = https://github.com/PatrickMassot/plastexdepgraph
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

