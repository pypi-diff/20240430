# Comparing `tmp/ragdaemon-0.3.1.tar.gz` & `tmp/ragdaemon-0.3.2.tar.gz`

## Comparing `ragdaemon-0.3.1.tar` & `ragdaemon-0.3.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0    13397 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/app.py
--rw-r--r--   0        0        0    10163 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/context.py
--rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/graph.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/llm.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/utils.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/prompts/chunker_llm.toml
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/test_comments.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/test_sample.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/annotators/test_chunker_llm.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    13397 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/app.py
+-rw-r--r--   0        0        0    10163 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/context.py
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/graph.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/llm.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/utils.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/prompts/chunker_llm.toml
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/conftest.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/test_comments.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/test_sample.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/annotators/test_chunker_llm.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.3.2/PKG-INFO
```

### Comparing `ragdaemon-0.3.1/scratch.ipynb` & `ragdaemon-0.3.2/scratch.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tutorial.ipynb` & `ragdaemon-0.3.2/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/.github/workflows/run-tests.yml` & `ragdaemon-0.3.2/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/app.py` & `ragdaemon-0.3.2/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/context.py` & `ragdaemon-0.3.2/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/daemon.py` & `ragdaemon-0.3.2/ragdaemon/daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/get_paths.py` & `ragdaemon-0.3.2/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/graph.py` & `ragdaemon-0.3.2/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/utils.py` & `ragdaemon-0.3.2/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/annotators/__init__.py` & `ragdaemon-0.3.2/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.3.2/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/annotators/chunker.py` & `ragdaemon-0.3.2/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.3.2/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.3.2/ragdaemon/annotators/chunker_llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     if not 1 <= start <= end <= last_valid_line:
         return False
     # TODO: Validate the ref, i.e. a parent chunk exists
 
     return True
 
 
-semaphore = asyncio.Semaphore(50)
+semaphore = asyncio.Semaphore(100)
 
 
 class ChunkerLLM(Chunker):
     name = "chunker_llm"
     chunk_field_id = "chunks_llm"
 
     async def get_llm_response(
```

### Comparing `ragdaemon-0.3.1/ragdaemon/annotators/diff.py` & `ragdaemon-0.3.2/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.3.2/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.3.2/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.3.2/ragdaemon/annotators/summarizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 It may be useful to name specific fucntions from the target repository (not built-in
 Python functions) which are integral to the functioning of the target code. Include a
 maximum of two (2) such named functions, but err on the side of brevity.
 """
 
 
-semaphore = asyncio.Semaphore(50)
+semaphore = asyncio.Semaphore(100)
 
 
 class Summarizer(Annotator):
     name = "summarizer"
 
     def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         return all(
```

### Comparing `ragdaemon-0.3.1/ragdaemon/database/__init__.py` & `ragdaemon-0.3.2/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/database/chroma_database.py` & `ragdaemon-0.3.2/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/database/database.py` & `ragdaemon-0.3.2/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/database/lite_database.py` & `ragdaemon-0.3.2/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/prompts/chunker_llm.toml` & `ragdaemon-0.3.2/ragdaemon/prompts/chunker_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/static/favicon.ico` & `ragdaemon-0.3.2/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.3.2/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/static/js/main.js` & `ragdaemon-0.3.2/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.3.2/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/static/js/three/node.js` & `ragdaemon-0.3.2/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.3.2/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/ragdaemon/templates/index.html` & `ragdaemon-0.3.2/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/conftest.py` & `ragdaemon-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/test_comments.py` & `ragdaemon-0.3.2/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/test_context.py` & `ragdaemon-0.3.2/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/test_daemon.py` & `ragdaemon-0.3.2/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/test_get_paths.py` & `ragdaemon-0.3.2/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/test_sample.py` & `ragdaemon-0.3.2/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/annotators/test_chunker.py` & `ragdaemon-0.3.2/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/annotators/test_chunker_llm.py` & `ragdaemon-0.3.2/tests/annotators/test_chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/annotators/test_diff.py` & `ragdaemon-0.3.2/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/annotators/test_hierarchy.py` & `ragdaemon-0.3.2/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.3.2/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/annotators/test_summarizer.py` & `ragdaemon-0.3.2/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/data/chunker_graph.json` & `ragdaemon-0.3.2/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/data/context_message.txt` & `ragdaemon-0.3.2/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/data/diff_graph.json` & `ragdaemon-0.3.2/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/data/hard_to_chunk.txt` & `ragdaemon-0.3.2/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/data/hierarchy_graph.json` & `ragdaemon-0.3.2/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.3.2/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/tests/sample/src/interface.py` & `ragdaemon-0.3.2/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/LICENSE` & `ragdaemon-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/README.md` & `ragdaemon-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.1/pyproject.toml` & `ragdaemon-0.3.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.3.1"
+version = "0.3.2"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.3.1/PKG-INFO` & `ragdaemon-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.3.1
+Version: 0.3.2
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

