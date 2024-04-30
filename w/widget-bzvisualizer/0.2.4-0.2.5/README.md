# Comparing `tmp/widget_bzvisualizer-0.2.4.tar.gz` & `tmp/widget_bzvisualizer-0.2.5.tar.gz`

## Comparing `widget_bzvisualizer-0.2.4.tar` & `widget_bzvisualizer-0.2.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/src/widget_bzvisualizer/__init__.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/src/widget_bzvisualizer/utils.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/src/widget_bzvisualizer/static/widget.css
--rw-r--r--   0        0        0   484471 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/src/widget_bzvisualizer/static/widget.js
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/.gitignore
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/README.md
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.5/src/widget_bzvisualizer/__init__.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.5/src/widget_bzvisualizer/utils.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.5/src/widget_bzvisualizer/static/widget.css
+-rw-r--r--   0        0        0   484471 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.5/src/widget_bzvisualizer/static/widget.js
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.5/README.md
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.5/PKG-INFO
```

### Comparing `widget_bzvisualizer-0.2.4/src/widget_bzvisualizer/__init__.py` & `widget_bzvisualizer-0.2.5/src/widget_bzvisualizer/__init__.py`

 * *Files identical despite different names*

### Comparing `widget_bzvisualizer-0.2.4/src/widget_bzvisualizer/utils.py` & `widget_bzvisualizer-0.2.5/src/widget_bzvisualizer/utils.py`

 * *Files identical despite different names*

### Comparing `widget_bzvisualizer-0.2.4/src/widget_bzvisualizer/static/widget.js` & `widget_bzvisualizer-0.2.5/src/widget_bzvisualizer/static/widget.js`

 * *Files identical despite different names*

### Comparing `widget_bzvisualizer-0.2.4/README.md` & `widget_bzvisualizer-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `widget_bzvisualizer-0.2.4/pyproject.toml` & `widget_bzvisualizer-0.2.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "widget-bzvisualizer"
-version = "0.2.4"
+version = "0.2.5"
 dependencies = [
-  "anywidget~=0.9.3",
+  "anywidget~=0.9.10",
   "numpy~=1.21",
   "scipy~=1.10",
   "seekpath~=2.1",
 ]
 readme = "README.md"
+keywords = [
+  'jupyter',
+  'jupyterlab',
+  'widget',
+  'anywidget',
+  'osscar',
+  'brillouin-zone',
+  'reciprocal-space',
+]
 
 [project.optional-dependencies]
-dev = [
-  "watchfiles",
-  "jupyterlab",
-  "ase",
-  "bumpver==2023.1129",
-]
+dev = ["watchfiles", "jupyterlab", "ase", "bumpver==2023.1129"]
 
 # automatically add the dev feature to the default env (e.g., hatch shell)
 [tool.hatch.envs.default]
 features = ["dev"]
 
 
 [tool.hatch.build]
@@ -37,19 +41,19 @@
 dependencies = ["hatch-jupyter-builder>=0.5.0"]
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
 npm = "npm"
 build_cmd = "build"
 
 [tool.bumpver]
-current_version = "v0.2.4"
+current_version = "v0.2.5"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
   'version = "{pep440_version}"',
   'current_version = "{version}"',
-]
+]
```

### Comparing `widget_bzvisualizer-0.2.4/PKG-INFO` & `widget_bzvisualizer-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.3
 Name: widget-bzvisualizer
-Version: 0.2.4
-Requires-Dist: anywidget~=0.9.3
+Version: 0.2.5
+Keywords: anywidget,brillouin-zone,jupyter,jupyterlab,osscar,reciprocal-space,widget
+Requires-Dist: anywidget~=0.9.10
 Requires-Dist: numpy~=1.21
 Requires-Dist: scipy~=1.10
 Requires-Dist: seekpath~=2.1
 Provides-Extra: dev
 Requires-Dist: ase; extra == 'dev'
 Requires-Dist: bumpver==2023.1129; extra == 'dev'
 Requires-Dist: jupyterlab; extra == 'dev'
```

