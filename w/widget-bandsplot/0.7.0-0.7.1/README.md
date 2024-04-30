# Comparing `tmp/widget_bandsplot-0.7.0.tar.gz` & `tmp/widget_bandsplot-0.7.1.tar.gz`

## Comparing `widget_bandsplot-0.7.0.tar` & `widget_bandsplot-0.7.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.0/src/widget_bandsplot/__init__.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.0/src/widget_bandsplot/static/widget.css
--rw-r--r--   0        0        0   539001 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.0/src/widget_bandsplot/static/widget.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.0/.gitignore
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.0/README.md
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.1/src/widget_bandsplot/__init__.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.1/src/widget_bandsplot/static/widget.css
+-rw-r--r--   0        0        0   539001 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.1/src/widget_bandsplot/static/widget.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.1/README.md
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.1/PKG-INFO
```

### Comparing `widget_bandsplot-0.7.0/src/widget_bandsplot/__init__.py` & `widget_bandsplot-0.7.1/src/widget_bandsplot/__init__.py`

 * *Files identical despite different names*

### Comparing `widget_bandsplot-0.7.0/src/widget_bandsplot/static/widget.css` & `widget_bandsplot-0.7.1/src/widget_bandsplot/static/widget.css`

 * *Files identical despite different names*

### Comparing `widget_bandsplot-0.7.0/src/widget_bandsplot/static/widget.js` & `widget_bandsplot-0.7.1/src/widget_bandsplot/static/widget.js`

 * *Files identical despite different names*

### Comparing `widget_bandsplot-0.7.0/README.md` & `widget_bandsplot-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `widget_bandsplot-0.7.0/pyproject.toml` & `widget_bandsplot-0.7.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "widget-bandsplot"
-version = "0.7.0"
-dependencies = [
-  "anywidget~=0.9.3"
-]
+version = "0.7.1"
+dependencies = ["anywidget~=0.9.10"]
 readme = "README.md"
+keywords = [
+  'jupyter',
+  'jupyterlab',
+  'widget',
+  'anywidget',
+  'osscar',
+  'electronic-structure',
+  'phonons',
+]
 
 [project.optional-dependencies]
-dev = [
-  "watchfiles",
-  "jupyterlab",
-  "bumpver==2023.1129",
-]
+dev = ["watchfiles", "jupyterlab", "bumpver==2023.1129"]
 
 # automatically add the dev feature to the default env (e.g., hatch shell)
 [tool.hatch.envs.default]
 features = ["dev"]
 
 
 [tool.hatch.build]
@@ -33,19 +36,19 @@
 dependencies = ["hatch-jupyter-builder>=0.5.0"]
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
 npm = "npm"
 build_cmd = "build"
 
 [tool.bumpver]
-current_version = "v0.7.0"
+current_version = "v0.7.1"
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

### Comparing `widget_bandsplot-0.7.0/PKG-INFO` & `widget_bandsplot-0.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.3
 Name: widget-bandsplot
-Version: 0.7.0
-Requires-Dist: anywidget~=0.9.3
+Version: 0.7.1
+Keywords: anywidget,electronic-structure,jupyter,jupyterlab,osscar,phonons,widget
+Requires-Dist: anywidget~=0.9.10
 Provides-Extra: dev
 Requires-Dist: bumpver==2023.1129; extra == 'dev'
 Requires-Dist: jupyterlab; extra == 'dev'
 Requires-Dist: watchfiles; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Jupyter widget: Band structure visualizer
```

