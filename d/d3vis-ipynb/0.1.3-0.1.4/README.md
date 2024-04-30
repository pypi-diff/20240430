# Comparing `tmp/d3vis_ipynb-0.1.3.tar.gz` & `tmp/d3vis_ipynb-0.1.4.tar.gz`

## Comparing `d3vis_ipynb-0.1.3.tar` & `d3vis_ipynb-0.1.4.tar`

### file list

```diff
@@ -1,45 +1,42 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/D3vis_ipynb.json
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/MANIFEST.in
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/RELEASE.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/install.json
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/setup.cfg
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/setup.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/_version.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/embedding.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/web.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/widgets.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/package.json
--rw-r--r--   0        0        0    27776 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/363.e98e5e3babbb9b69956a.js
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/493.053b071a46f0bcccaab9.js
--rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/remoteEntry.8f26db161f1984f5ad68.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/style.js
--rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    93598 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/nbextension/index.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/amd-public-path.js
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/package.json
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/webpack.config.js
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/webpack.exports.config.js
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/css/widget.css
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/extension.js
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/index.js
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/labplugin.js
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/web-dev.js
--rw-r--r--   0        0        0    12733 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/widgets.js
--rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/graphs/barplot.js
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/graphs/histogramplot.js
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/graphs/linearhistplot.js
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/graphs/rangeslider.js
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/graphs/scatterplot.js
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/tools/lasso.js
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/wrappers/embedding.wrapper.js
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/testes/index.html
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/testes/index.js
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/testes/style.css
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/.gitignore
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/README.md
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/D3vis_ipynb.json
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/MANIFEST.in
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/RELEASE.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/install.json
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/setup.cfg
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/setup.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/_version.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/embedding.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/web.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/widgets.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/package.json
+-rw-r--r--   0        0        0    27995 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/363.eafafc6b255bbd58c086.js
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/493.053b071a46f0bcccaab9.js
+-rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/remoteEntry.d538e52840abf118c637.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/style.js
+-rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    93817 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/nbextension/index.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/amd-public-path.js
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/package.json
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/webpack.config.js
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/webpack.exports.config.js
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/css/widget.css
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/extension.js
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/index.js
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/labplugin.js
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/web-dev.js
+-rw-r--r--   0        0        0    12873 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/widgets.js
+-rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/graphs/barplot.js
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/graphs/histogramplot.js
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/graphs/linearhistplot.js
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/graphs/rangeslider.js
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/graphs/scatterplot.js
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/tools/lasso.js
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/wrappers/embedding.wrapper.js
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/README.md
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/PKG-INFO
```

### Comparing `d3vis_ipynb-0.1.3/RELEASE.md` & `d3vis_ipynb-0.1.4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/setup.cfg` & `d3vis_ipynb-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/d3vis_ipynb/__init__.py` & `d3vis_ipynb-0.1.4/d3vis_ipynb/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+import sys
+
 from ._version import __version__
 from .embedding import Embedding
 from .web import WebWidget
 from .widgets import *
 
+if "google.colab.output" in sys.modules:
+    sys.modules["google.colab.output"].enable_custom_widget_manager()
+
 
 def _jupyter_labextension_paths():
     """Called by Jupyter Lab Server to detect if it is a valid labextension and
     to install the widget
 
     Returns
     =======
```

### Comparing `d3vis_ipynb-0.1.3/d3vis_ipynb/embedding.py` & `d3vis_ipynb-0.1.4/d3vis_ipynb/embedding.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/d3vis_ipynb/web.py` & `d3vis_ipynb-0.1.4/d3vis_ipynb/web.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/d3vis_ipynb/widgets.py` & `d3vis_ipynb-0.1.4/d3vis_ipynb/widgets.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/package.json` & `d3vis_ipynb-0.1.4/js/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9519230769230769%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.1.4'"}*

```diff
@@ -14,18 +14,14 @@
     },
     "files": [
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.8f26db161f1984f5ad68.js"
-        },
         "extension": "lib/labplugin",
         "outputDir": "../d3vis_ipynb/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
@@ -54,9 +50,9 @@
         "export": "webpack --env export --config webpack.exports.config.js",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
         "start:export": "webpack serve --open --config webpack.exports.config.js --env export",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.1.3"
+    "version": "0.1.4"
 }
```

### Comparing `d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/363.e98e5e3babbb9b69956a.js` & `d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/363.eafafc6b255bbd58c086.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -309,21 +309,22 @@
                 }
                 plot() {
                     const e = this.model.get("data"),
                         t = this.model.get("x"),
                         n = this.model.get("y"),
                         a = this.model.get("hue"),
                         i = this.model.get("elementId");
+                    console.log("barplot"), console.log("elementId:"), console.log(i);
                     let o = y,
                         s = this.el;
                     i && (s = document.getElementById(i), o = s.clientHeight),
                         function(e, t, n, a, i, o, s, r) {
                             const l = o - r.left - r.right,
                                 d = s - r.top - r.bottom;
-                            _.select(i).selectAll("*").remove();
+                            console.log("element:"), console.log(i), console.log("width:"), console.log(o), console.log("height:"), console.log(s), _.select(i).selectAll("*").remove();
                             const c = _.select(i).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + r.left + "," + r.top + ")");
                             a || (a = t);
                             const m = e.reduce(((e, t) => (e && -1 === e.indexOf(t[a]) && e.push(t[a]), e)), []),
                                 u = {},
                                 p = _.scaleOrdinal(_.schemeCategory10);
                             a == t ? function() {
                                 let a = e.reduce(((e, a) => {
@@ -562,15 +563,15 @@
                         n = this.model.get("grid_template_areas");
                     let a = this.model.get("style");
                     a || (a = "basic");
                     const i = document.createElement("div");
                     i.classList.add(a), i.style.display = "grid", i.style.gridTemplateAreas = n, i.style.gridTemplateRows = "repeat(" + e.length + ", 20vh)", i.style.gridTemplateColumns = "repeat(" + e[0].length + ", 1fr)", i.style.width = "100%", t.forEach((e => {
                         const t = document.createElement("div");
                         t.setAttribute("id", e), t.style.gridArea = e, t.classList.add("dashboard-div"), i.appendChild(t)
-                    })), this.el.appendChild(i)
+                    })), this.el.appendChild(i), console.log("Embedding:"), console.log(i)
                 }
             }
             class I extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
                         _model_name: I.model_name,
@@ -828,11 +829,11 @@
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
         330: e => {
-            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.3","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.4","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/493.053b071a46f0bcccaab9.js` & `d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/493.053b071a46f0bcccaab9.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js` & `d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/remoteEntry.8f26db161f1984f5ad68.js` & `d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/remoteEntry.d538e52840abf118c637.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, d, u, s, l, f, c, p, h, v, b, g, m, y, w = {
+    var e, r, t, n, o, i, a, u, s, d, l, f, p, c, h, v, g, b, m, y, w = {
             772: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(363).then((() => () => t(363))),
                         "./extension": () => Promise.all([t.e(363), t.e(493)]).then((() => () => t(493)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -42,51 +42,51 @@
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        363: "e98e5e3babbb9b69956a",
+        363: "eafafc6b255bbd58c086",
         493: "053b071a46f0bcccaab9",
         693: "c8409ce8329f6703470f"
     } [e] + ".js?v=" + {
-        363: "e98e5e3babbb9b69956a",
+        363: "eafafc6b255bbd58c086",
         493: "053b071a46f0bcccaab9",
         693: "c8409ce8329f6703470f"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "d3vis_ipynb:", E.l = (t, n, o, i) => {
         if (e[t]) e[t].push(n);
         else {
-            var a, d;
+            var a, u;
             if (void 0 !== o)
-                for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
-                    var l = u[s];
+                for (var s = document.getElementsByTagName("script"), d = 0; d < s.length; d++) {
+                    var l = s[d];
                     if (l.getAttribute("src") == t || l.getAttribute("data-webpack") == r + o) {
                         a = l;
                         break
                     }
                 }
-            a || (d = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, E.nc && a.setAttribute("nonce", E.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
+            a || (u = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, E.nc && a.setAttribute("nonce", E.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
             var f = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(c);
+                    a.onerror = a.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
-            a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), d && document.head.appendChild(a)
+            a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), u && document.head.appendChild(a)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -98,25 +98,25 @@
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
                 E.o(E.S, t) || (E.S[t] = {});
                 var i = E.S[t],
                     a = "d3vis_ipynb",
-                    d = (e, r, t, n) => {
+                    u = (e, r, t, n) => {
                         var o = i[e] = i[e] || {},
-                            d = o[r];
-                        (!d || !d.loaded && (!n != !d.eager ? n : a > d.from)) && (o[r] = {
+                            u = o[r];
+                        (!u || !u.loaded && (!n != !u.eager ? n : a > u.from)) && (o[r] = {
                             get: t,
                             from: a,
                             eager: !!n
                         })
                     },
-                    u = [];
-                return "default" === t && (d("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), d("d3vis_ipynb", "0.1.3", (() => E.e(363).then((() => () => E(363)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                    s = [];
+                return "default" === t && (u("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), u("d3vis_ipynb", "0.1.4", (() => E.e(363).then((() => () => E(363)))))), e[t] = s.length ? Promise.all(s).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -135,122 +135,122 @@
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var o = e[n],
                 i = (typeof o)[0];
             if (n >= r.length) return "u" == i;
             var a = r[n],
-                d = (typeof a)[0];
-            if (i != d) return "o" == i && "n" == d || "s" == d || "u" == i;
+                u = (typeof a)[0];
+            if (i != u) return "o" == i && "n" == u || "s" == u || "u" == i;
             if ("o" != i && "u" != i && o != a) return o < a;
             n++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(d = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, d);
+            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(u = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var a = [];
         for (i = 1; i < e.length; i++) {
-            var d = e[i];
-            a.push(0 === d ? "not(" + u() + ")" : 1 === d ? "(" + u() + " || " + u() + ")" : 2 === d ? a.pop() + " " + a.pop() : o(d))
+            var u = e[i];
+            a.push(0 === u ? "not(" + s() + ")" : 1 === u ? "(" + s() + " || " + s() + ")" : 2 === u ? a.pop() + " " + a.pop() : o(u))
         }
-        return u();
+        return s();
 
-        function u() {
+        function s() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var a = 0, d = 1, u = !0;; d++, a++) {
-                var s, l, f = d < e.length ? (typeof e[d])[0] : "";
-                if (a >= r.length || "o" == (l = (typeof(s = r[a]))[0])) return !u || ("u" == f ? d > n && !o : "" == f != o);
+            for (var a = 0, u = 1, s = !0;; u++, a++) {
+                var d, l, f = u < e.length ? (typeof e[u])[0] : "";
+                if (a >= r.length || "o" == (l = (typeof(d = r[a]))[0])) return !s || ("u" == f ? u > n && !o : "" == f != o);
                 if ("u" == l) {
-                    if (!u || "u" != f) return !1
-                } else if (u)
+                    if (!s || "u" != f) return !1
+                } else if (s)
                     if (f == l)
-                        if (d <= n) {
-                            if (s != e[d]) return !1
+                        if (u <= n) {
+                            if (d != e[u]) return !1
                         } else {
-                            if (o ? s > e[d] : s < e[d]) return !1;
-                            s != e[d] && (u = !1)
+                            if (o ? d > e[u] : d < e[u]) return !1;
+                            d != e[u] && (s = !1)
                         }
                 else if ("s" != f && "n" != f) {
-                    if (o || d <= n) return !1;
-                    u = !1, d--
+                    if (o || u <= n) return !1;
+                    s = !1, u--
                 } else {
-                    if (d <= n || l < f != o) return !1;
-                    u = !1
-                } else "s" != f && "n" != f && (u = !1, d--)
+                    if (u <= n || l < f != o) return !1;
+                    s = !1
+                } else "s" != f && "n" != f && (s = !1, u--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, a = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, d = (e, r) => {
+    }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
-        var o = d(e, t);
-        return i(n, o) || f(u(e, t, o, n)), c(e[t][o])
+    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", d = (e, r, t, n) => {
+        var o = u(e, t);
+        return i(n, o) || f(s(e, t, o, n)), p(e[t][o])
     }, l = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !i(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
+    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, o) {
         var i = E.I(r);
         return i && i.then ? i.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (a(e, t), d(r, 0, t, n)))), v = c(((e, r, t, n, o) => {
         var i = r && E.o(r, t) && l(r, t, n);
-        return i ? c(i) : o()
-    })), b = {}, g = {
+        return i ? p(i) : o()
+    })), g = {}, b = {
         801: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1], 1, 1, 1, 1
         ]),
         840: () => v("default", "d3", [1, 7, 9, 0], (() => E.e(693).then((() => () => E(693)))))
     }, m = {
         363: [801, 840]
     }, y = {}, E.f.consumes = (e, r) => {
         E.o(m, e) && m[e].forEach((e => {
-            if (E.o(b, e)) return r.push(b[e]);
+            if (E.o(g, e)) return r.push(g[e]);
             if (!y[e]) {
                 var t = r => {
-                    b[e] = 0, E.m[e] = t => {
+                    g[e] = 0, E.m[e] = t => {
                         delete E.c[e], t.exports = r()
                     }
                 };
                 y[e] = !0;
                 var n = r => {
-                    delete b[e], E.m[e] = t => {
+                    delete g[e], E.m[e] = t => {
                         throw delete E.c[e], r
                     }
                 };
                 try {
-                    var o = g[e]();
-                    o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
+                    var o = b[e]();
+                    o.then ? r.push(g[e] = o.then(t).catch(n)) : t(o)
                 } catch (e) {
                     n(e)
                 }
             }
         }))
     }, (() => {
         var e = {
@@ -271,21 +271,21 @@
                                 i = t && t.target && t.target.src;
                             a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, o, [i, a, d] = t,
-                    u = 0;
+                var n, o, [i, a, u] = t,
+                    s = 0;
                 if (i.some((r => 0 !== e[r]))) {
                     for (n in a) E.o(a, n) && (E.m[n] = a[n]);
-                    d && d(E)
+                    u && u(E)
                 }
-                for (r && r(t); u < i.length; u++) o = i[u], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); s < i.length; s++) o = i[s], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkd3vis_ipynb = self.webpackChunkd3vis_ipynb || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), E.nc = void 0;
     var P = E(772);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).d3vis_ipynb = P
 })();
```

### Comparing `d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/third-party-licenses.json` & `d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/d3vis_ipynb/nbextension/index.js` & `d3vis_ipynb-0.1.4/d3vis_ipynb/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -179,15 +179,15 @@
             55: t => {
                 t.exports = e
             },
             308: e => {
                 e.exports = t
             },
             330: t => {
-                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.3","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.4","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         r = {};
 
     function i(t) {
         var e = r[t];
         if (void 0 !== e) return e.exports;
@@ -3698,21 +3698,22 @@
             }
             plot() {
                 const t = this.model.get("data"),
                     e = this.model.get("x"),
                     n = this.model.get("y"),
                     r = this.model.get("hue"),
                     i = this.model.get("elementId");
+                console.log("barplot"), console.log("elementId:"), console.log(i);
                 let o = Si,
                     a = this.el;
                 i && (a = document.getElementById(i), o = a.clientHeight),
                     function(t, e, n, r, i, o, a, s) {
                         const l = o - s.left - s.right,
                             u = a - s.top - s.bottom;
-                        mr(i).selectAll("*").remove();
+                        console.log("element:"), console.log(i), console.log("width:"), console.log(o), console.log("height:"), console.log(a), mr(i).selectAll("*").remove();
                         const c = mr(i).append("svg").attr("width", o).attr("height", a).append("g").attr("transform", "translate(" + s.left + "," + s.top + ")");
                         r || (r = e);
                         const h = t.reduce(((t, e) => (t && -1 === t.indexOf(e[r]) && t.push(e[r]), t)), []),
                             f = {},
                             d = jr(si);
                         r == e ? function() {
                             let r = t.reduce(((t, r) => {
@@ -3951,15 +3952,15 @@
                     n = this.model.get("grid_template_areas");
                 let r = this.model.get("style");
                 r || (r = "basic");
                 const i = document.createElement("div");
                 i.classList.add(r), i.style.display = "grid", i.style.gridTemplateAreas = n, i.style.gridTemplateRows = "repeat(" + t.length + ", 20vh)", i.style.gridTemplateColumns = "repeat(" + t[0].length + ", 1fr)", i.style.width = "100%", e.forEach((t => {
                     const e = document.createElement("div");
                     e.setAttribute("id", t), e.style.gridArea = t, e.classList.add("dashboard-div"), i.appendChild(e)
-                })), this.el.appendChild(i)
+                })), this.el.appendChild(i), console.log("Embedding:"), console.log(i)
             }
         }
         class zi extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
                     _model_name: zi.model_name,
```

### Comparing `d3vis_ipynb-0.1.3/js/amd-public-path.js` & `d3vis_ipynb-0.1.4/js/amd-public-path.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/js/package.json` & `d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/package.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9519230769230769%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.d538e52840abf118c637.js'), "*

 * *                 "('extension', './extension')])}",*

 * * "'version'": "'0.1.4'"}*

```diff
@@ -14,14 +14,18 @@
     },
     "files": [
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.d538e52840abf118c637.js"
+        },
         "extension": "lib/labplugin",
         "outputDir": "../d3vis_ipynb/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
@@ -50,9 +54,9 @@
         "export": "webpack --env export --config webpack.exports.config.js",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
         "start:export": "webpack serve --open --config webpack.exports.config.js --env export",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.1.3"
+    "version": "0.1.4"
 }
```

### Comparing `d3vis_ipynb-0.1.3/js/webpack.config.js` & `d3vis_ipynb-0.1.4/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/js/webpack.exports.config.js` & `d3vis_ipynb-0.1.4/js/webpack.exports.config.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/js/css/widget.css` & `d3vis_ipynb-0.1.4/js/css/widget.css`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/js/lib/labplugin.js` & `d3vis_ipynb-0.1.4/js/lib/labplugin.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/js/lib/web-dev.js` & `d3vis_ipynb-0.1.4/js/lib/web-dev.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/js/lib/widgets.js` & `d3vis_ipynb-0.1.4/js/lib/widgets.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -242,14 +242,18 @@
     plot() {
         const data = this.model.get("data");
         const x = this.model.get("x");
         const y = this.model.get("y");
         const hue = this.model.get("hue");
         const elementId = this.model.get("elementId");
 
+        console.log("barplot");
+        console.log("elementId:");
+        console.log(elementId);
+
         let height = WIDGET_HEIGHT;
         let element = this.el;
         if (elementId) {
             element = document.getElementById(elementId);
             height = element.clientHeight;
         }
         let width = element.clientWidth;
@@ -374,14 +378,16 @@
             grid_area.setAttribute("id", area);
             grid_area.style.gridArea = area;
             grid_area.classList.add("dashboard-div");
             node.appendChild(grid_area);
         });
 
         this.el.appendChild(node);
+        console.log("Embedding:")
+        console.log(node)
     }
 }
 
 export class RangeSliderModel extends DOMWidgetModel {
     defaults() {
         return {
             ...super.defaults(),
```

### Comparing `d3vis_ipynb-0.1.3/js/lib/graphs/barplot.js` & `d3vis_ipynb-0.1.4/js/lib/graphs/barplot.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,28 @@
 import * as d3 from "d3";
 
-export function barplot(data, x_axis, y_axis, hue_axis, element, width, height, margin) {
-    const innerWidth = width - margin.left - margin.right
-    const innerHeight = height - margin.top - margin.bottom
+export function barplot(
+    data,
+    x_axis,
+    y_axis,
+    hue_axis,
+    element,
+    width,
+    height,
+    margin
+) {
+    const innerWidth = width - margin.left - margin.right;
+    const innerHeight = height - margin.top - margin.bottom;
+
+    console.log("element:");
+    console.log(element);
+    console.log("width:");
+    console.log(width);
+    console.log("height:");
+    console.log(height);
 
     d3.select(element).selectAll("*").remove();
 
     const svg = d3
         .select(element)
         .append("svg")
         .attr("width", width)
@@ -79,15 +95,19 @@
         if (y_domain[0] > 0 && y_domain[1] > 0) y_domain[0] = 0;
         else if (y_domain[0] < 0 && y_domain[1] < 0) y_domain[1] = 0;
 
         const y = d3.scaleLinear().domain(y_domain).range([innerHeight, 0]);
 
         svg.append("g").call(d3.axisLeft(y));
 
-        const x = d3.scaleBand().domain(groups).range([0, innerWidth]).padding([0.2]);
+        const x = d3
+            .scaleBand()
+            .domain(groups)
+            .range([0, innerWidth])
+            .padding([0.2]);
 
         svg
             .append("g")
             .selectAll("g")
             .data(result)
             .enter()
             .append("rect")
@@ -215,15 +235,19 @@
         if (y_domain[0] > 0 && y_domain[1] > 0) y_domain[0] = 0;
         else if (y_domain[0] < 0 && y_domain[1] < 0) y_domain[1] = 0;
 
         const y = d3.scaleLinear().domain(y_domain).range([innerHeight, 0]);
 
         svg.append("g").call(d3.axisLeft(y));
 
-        const x = d3.scaleBand().domain(groups).range([0, innerWidth]).padding([0.2]);
+        const x = d3
+            .scaleBand()
+            .domain(groups)
+            .range([0, innerWidth])
+            .padding([0.2]);
 
         const xSubgroup = d3
             .scaleBand()
             .domain(subgroups)
             .range([0, x.bandwidth()])
             .padding([0.05]);
```

### Comparing `d3vis_ipynb-0.1.3/js/lib/graphs/histogramplot.js` & `d3vis_ipynb-0.1.4/js/lib/graphs/histogramplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/js/lib/graphs/linearhistplot.js` & `d3vis_ipynb-0.1.4/js/lib/graphs/linearhistplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/js/lib/graphs/rangeslider.js` & `d3vis_ipynb-0.1.4/js/lib/graphs/rangeslider.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/js/lib/graphs/scatterplot.js` & `d3vis_ipynb-0.1.4/js/lib/graphs/scatterplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/js/lib/tools/lasso.js` & `d3vis_ipynb-0.1.4/js/lib/tools/lasso.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/js/lib/wrappers/embedding.wrapper.js` & `d3vis_ipynb-0.1.4/js/lib/wrappers/embedding.wrapper.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/LICENSE.txt` & `d3vis_ipynb-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/README.md` & `d3vis_ipynb-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.3/pyproject.toml` & `d3vis_ipynb-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "ipywidgets>=7.7.1",
     "simplejson >=3.19.0",
     "anywidget >= 0.9.6"
 ]
-version = "0.1.3"
+version = "0.1.4"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
```

### Comparing `d3vis_ipynb-0.1.3/PKG-INFO` & `d3vis_ipynb-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: d3vis_ipynb
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Custom Jupyter Widget Library with visualizations created with D3.js.
 Project-URL: Homepage, https://github.com/H-IAAC/d3vis_ipynb
 Author-email: Daniel Adam Miranda <daniel.miranda@eldorado.org.br>
 License: Copyright (c) 2024 Daniel Adam Miranda
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

