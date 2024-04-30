# Comparing `tmp/kingdon-1.0.3.tar.gz` & `tmp/kingdon-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingdon-1.0.3.tar", last modified: Mon Apr 22 10:16:39 2024, max compression
+gzip compressed data, was "kingdon-1.0.4.tar", last modified: Tue Apr 30 15:45:31 2024, max compression
```

## Comparing `kingdon-1.0.3.tar` & `kingdon-1.0.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:16:39.278396 kingdon-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-22 10:16:35.000000 kingdon-1.0.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-22 10:16:35.000000 kingdon-1.0.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-22 10:16:35.000000 kingdon-1.0.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-22 10:16:35.000000 kingdon-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-22 10:16:35.000000 kingdon-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-22 10:16:39.278396 kingdon-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-04-22 10:16:35.000000 kingdon-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:16:39.274396 kingdon-1.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-22 10:16:35.000000 kingdon-1.0.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:16:39.274396 kingdon-1.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    94383 2024-04-22 10:16:35.000000 kingdon-1.0.3/docs/_static/graph_triangle.png
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 10:16:35.000000 kingdon-1.0.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-22 10:16:35.000000 kingdon-1.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 10:16:35.000000 kingdon-1.0.3/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:16:39.278396 kingdon-1.0.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-22 10:16:35.000000 kingdon-1.0.3/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 10:16:35.000000 kingdon-1.0.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-22 10:16:35.000000 kingdon-1.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-22 10:16:35.000000 kingdon-1.0.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-22 10:16:35.000000 kingdon-1.0.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-22 10:16:35.000000 kingdon-1.0.3/docs/module_docs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-22 10:16:35.000000 kingdon-1.0.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-22 10:16:35.000000 kingdon-1.0.3/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-22 10:16:35.000000 kingdon-1.0.3/docs/workings.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:16:39.278396 kingdon-1.0.3/kingdon/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-22 10:16:35.000000 kingdon-1.0.3/kingdon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21930 2024-04-22 10:16:35.000000 kingdon-1.0.3/kingdon/algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)    30710 2024-04-22 10:16:35.000000 kingdon-1.0.3/kingdon/codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-22 10:16:35.000000 kingdon-1.0.3/kingdon/graph.js
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-04-22 10:16:35.000000 kingdon-1.0.3/kingdon/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-22 10:16:35.000000 kingdon-1.0.3/kingdon/matrixreps.py
--rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-04-22 10:16:35.000000 kingdon-1.0.3/kingdon/multivector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-22 10:16:35.000000 kingdon-1.0.3/kingdon/operator_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-22 10:16:35.000000 kingdon-1.0.3/kingdon/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-22 10:16:35.000000 kingdon-1.0.3/kingdon/taperecorder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:16:39.278396 kingdon-1.0.3/kingdon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-22 10:16:39.000000 kingdon-1.0.3/kingdon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-22 10:16:39.000000 kingdon-1.0.3/kingdon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 10:16:39.000000 kingdon-1.0.3/kingdon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 10:16:39.000000 kingdon-1.0.3/kingdon.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 10:16:39.000000 kingdon-1.0.3/kingdon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 10:16:39.000000 kingdon-1.0.3/kingdon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-22 10:16:39.278396 kingdon-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-22 10:16:35.000000 kingdon-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:16:39.278396 kingdon-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 10:16:35.000000 kingdon-1.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-22 10:16:35.000000 kingdon-1.0.3/tests/performance_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-22 10:16:35.000000 kingdon-1.0.3/tests/test_expr_as_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-22 10:16:35.000000 kingdon-1.0.3/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    26180 2024-04-22 10:16:35.000000 kingdon-1.0.3/tests/test_kingdon.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-22 10:16:35.000000 kingdon-1.0.3/tests/test_operator_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-22 10:16:35.000000 kingdon-1.0.3/tests/test_polynomial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:31.628359 kingdon-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-30 15:45:26.000000 kingdon-1.0.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-30 15:45:26.000000 kingdon-1.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-30 15:45:26.000000 kingdon-1.0.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-30 15:45:26.000000 kingdon-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-30 15:45:26.000000 kingdon-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-30 15:45:31.628359 kingdon-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-04-30 15:45:26.000000 kingdon-1.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:31.628359 kingdon-1.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-30 15:45:26.000000 kingdon-1.0.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:31.628359 kingdon-1.0.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    94383 2024-04-30 15:45:26.000000 kingdon-1.0.4/docs/_static/graph_triangle.png
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 15:45:26.000000 kingdon-1.0.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-30 15:45:26.000000 kingdon-1.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 15:45:26.000000 kingdon-1.0.4/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:31.628359 kingdon-1.0.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-30 15:45:26.000000 kingdon-1.0.4/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 15:45:26.000000 kingdon-1.0.4/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-30 15:45:26.000000 kingdon-1.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-30 15:45:26.000000 kingdon-1.0.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-30 15:45:26.000000 kingdon-1.0.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-30 15:45:26.000000 kingdon-1.0.4/docs/module_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-30 15:45:26.000000 kingdon-1.0.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-30 15:45:26.000000 kingdon-1.0.4/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-30 15:45:26.000000 kingdon-1.0.4/docs/workings.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:31.628359 kingdon-1.0.4/kingdon/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-30 15:45:26.000000 kingdon-1.0.4/kingdon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21957 2024-04-30 15:45:26.000000 kingdon-1.0.4/kingdon/algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30710 2024-04-30 15:45:26.000000 kingdon-1.0.4/kingdon/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-30 15:45:26.000000 kingdon-1.0.4/kingdon/graph.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-30 15:45:26.000000 kingdon-1.0.4/kingdon/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-30 15:45:26.000000 kingdon-1.0.4/kingdon/matrixreps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19427 2024-04-30 15:45:26.000000 kingdon-1.0.4/kingdon/multivector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-30 15:45:26.000000 kingdon-1.0.4/kingdon/operator_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-30 15:45:26.000000 kingdon-1.0.4/kingdon/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-30 15:45:26.000000 kingdon-1.0.4/kingdon/taperecorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:31.628359 kingdon-1.0.4/kingdon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-30 15:45:31.000000 kingdon-1.0.4/kingdon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-30 15:45:31.000000 kingdon-1.0.4/kingdon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:45:31.000000 kingdon-1.0.4/kingdon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:45:31.000000 kingdon-1.0.4/kingdon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 15:45:31.000000 kingdon-1.0.4/kingdon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 15:45:31.000000 kingdon-1.0.4/kingdon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-30 15:45:31.632359 kingdon-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-30 15:45:26.000000 kingdon-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:31.628359 kingdon-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-30 15:45:26.000000 kingdon-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-30 15:45:26.000000 kingdon-1.0.4/tests/performance_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-30 15:45:26.000000 kingdon-1.0.4/tests/test_expr_as_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-30 15:45:26.000000 kingdon-1.0.4/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26274 2024-04-30 15:45:26.000000 kingdon-1.0.4/tests/test_kingdon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 15:45:26.000000 kingdon-1.0.4/tests/test_operator_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-30 15:45:26.000000 kingdon-1.0.4/tests/test_polynomial.py
```

### Comparing `kingdon-1.0.3/CONTRIBUTING.rst` & `kingdon-1.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/HISTORY.rst` & `kingdon-1.0.4/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/LICENSE` & `kingdon-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/PKG-INFO` & `kingdon-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingdon
-Version: 1.0.3
+Version: 1.0.4
 Summary: Pythonic Geometric Algebra Package
 Home-page: https://github.com/tbuli/kingdon
 Author: Martin Roelfs
 Author-email: martinroelfs@yahoo.com
 License: MIT license
 Keywords: kingdon
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kingdon-1.0.3/README.rst` & `kingdon-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/docs/Makefile` & `kingdon-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/docs/_static/graph_triangle.png` & `kingdon-1.0.4/docs/_static/graph_triangle.png`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/docs/conf.py` & `kingdon-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/docs/examples/index.rst` & `kingdon-1.0.4/docs/examples/index.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/docs/installation.rst` & `kingdon-1.0.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/docs/make.bat` & `kingdon-1.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/docs/module_docs.rst` & `kingdon-1.0.4/docs/module_docs.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/docs/readme.rst` & `kingdon-1.0.4/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/docs/usage.rst` & `kingdon-1.0.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/kingdon/algebra.py` & `kingdon-1.0.4/kingdon/algebra.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,15 +358,15 @@
 
     def pseudotrivector(self, *args, **kwargs) -> MultiVector:
         return self.purevector(*args, grade=self.d - 3, **kwargs)
 
     def pseudoquadvector(self, *args, **kwargs) -> MultiVector:
         return self.purevector(*args, grade=self.d - 4, **kwargs)
 
-    def graph(self, *subjects, **options):
+    def graph(self, *subjects, graph_widget=GraphWidget, **options):
         """
         The graph function outputs :code:`ganja.js` renders and is meant
         for use in jupyter notebooks. The syntax of the graph function will feel
         familiar to users of :code:`ganja.js`: all position arguments are considered
         as subjects to graph, while all keyword arguments are interpreted as options
         to :code:`ganja.js`'s :code:`Algebra.graph` method.
 
@@ -404,15 +404,15 @@
                 lineWidth=3, grid=1, labels=1
             )
 
         :param `*subjects`: Subjects to be graphed.
             Can be strings, hexadecimal colors, (lists of) MultiVector, (lists of) callables.
         :param `**options`: Options passed to :code:`ganja.js`'s :code:`Algebra.graph`.
         """
-        return GraphWidget(
+        return graph_widget(
             algebra=self,
             raw_subjects=subjects,
             options=options,
         )
 
 
 def _sort_product(prod):
```

### Comparing `kingdon-1.0.3/kingdon/codegen.py` & `kingdon-1.0.4/kingdon/codegen.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/kingdon/graph.js` & `kingdon-1.0.4/kingdon/graph.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -7,16 +7,15 @@
     });
 
 function render({
     model,
     el
 }) {
     var canvas = Algebra({
-        metric: model.get('signature'),
-        Cayley: model.get('cayley')
+        metric: model.get('signature')
     }).inline((model) => {
         // Define constants
         var key2idx = model.get('key2idx');
         var draggable_points_idxs = model.get('draggable_points_idxs');
         var options = model.get('options');
 
         // Define helper functions.
```

### Comparing `kingdon-1.0.3/kingdon/graph.py` & `kingdon-1.0.4/kingdon/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     @traitlets.default('key2idx')
     def get_key2idx(self):
         return {k: i for i, k in enumerate(self.algebra.canon2bin.values())}
 
     @traitlets.default('signature')
     def get_signature(self):
-        return list(self.algebra.signature)
+        return [int(s) for s in self.algebra.signature]
 
     @traitlets.default('cayley')
     def get_cayley(self):
         cayley_table = [[s if (s := self.algebra.cayley[eJ, eI])[-1] != 'e' else f"{s[:-1]}1"
                          for eI in self.algebra.canon2bin]
                          for eJ in self.algebra.canon2bin]
         return cayley_table
```

### Comparing `kingdon-1.0.3/kingdon/matrixreps.py` & `kingdon-1.0.4/kingdon/matrixreps.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/kingdon/multivector.py` & `kingdon-1.0.4/kingdon/multivector.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,21 +226,24 @@
 
     def sub(self, other):
         return self.algebra.sub(self, other)
 
     __sub__ = sub
 
     def __rsub__(self, other):
-        return other + (-self)
+        return self.algebra.sub(other, self)
 
     def div(self, other):
         return self.algebra.div(self, other)
 
     __truediv__ = div
 
+    def __rtruediv__(self, other):
+        return self.algebra.div(other, self)
+
     def __str__(self):
         if not len(self.values()):
             return '0'
 
         def print_value(val):
             if isinstance(val, Expr):
                 if val.is_Symbol:
```

### Comparing `kingdon-1.0.3/kingdon/operator_dict.py` & `kingdon-1.0.4/kingdon/operator_dict.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/kingdon/polynomial.py` & `kingdon-1.0.4/kingdon/polynomial.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/kingdon/taperecorder.py` & `kingdon-1.0.4/kingdon/taperecorder.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/kingdon.egg-info/PKG-INFO` & `kingdon-1.0.4/kingdon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingdon
-Version: 1.0.3
+Version: 1.0.4
 Summary: Pythonic Geometric Algebra Package
 Home-page: https://github.com/tbuli/kingdon
 Author: Martin Roelfs
 Author-email: martinroelfs@yahoo.com
 License: MIT license
 Keywords: kingdon
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kingdon-1.0.3/kingdon.egg-info/SOURCES.txt` & `kingdon-1.0.4/kingdon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/setup.py` & `kingdon-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,10 +37,10 @@
     include_package_data=True,
     keywords='kingdon',
     name='kingdon',
     packages=find_packages(include=['kingdon', 'kingdon.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/tbuli/kingdon',
-    version='1.0.3',
+    version='1.0.4',
     zip_safe=False,
 )
```

### Comparing `kingdon-1.0.3/tests/performance_check.py` & `kingdon-1.0.4/tests/performance_check.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/tests/test_expr_as_matrix.py` & `kingdon-1.0.4/tests/test_expr_as_matrix.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/tests/test_kingdon.py` & `kingdon-1.0.4/tests/test_kingdon.py`

 * *Files 1% similar despite different names*

```diff
@@ -812,7 +812,12 @@
     assert y & x == yfunc & x
     assert x | y == x | yfunc
     assert y | x == yfunc | x
     assert x @ y == x @ yfunc
     assert y @ x == yfunc @ x
     assert x >> y == x >> yfunc
     assert y >> x == yfunc >> x
+
+def test_43():
+    alg = Algebra(2)
+    x = alg.vector(name='x')
+    assert x.inv() == 1 / x
```

### Comparing `kingdon-1.0.3/tests/test_operator_dict.py` & `kingdon-1.0.4/tests/test_operator_dict.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.3/tests/test_polynomial.py` & `kingdon-1.0.4/tests/test_polynomial.py`

 * *Files identical despite different names*

