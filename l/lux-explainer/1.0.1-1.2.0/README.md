# Comparing `tmp/lux-explainer-1.0.1.tar.gz` & `tmp/lux_explainer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lux-explainer-1.0.1.tar", last modified: Thu Feb 22 16:54:46 2024, max compression
+gzip compressed data, was "lux_explainer-1.2.0.tar", last modified: Tue Apr 30 10:43:44 2024, max compression
```

## Comparing `lux-explainer-1.0.1.tar` & `lux_explainer-1.2.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-02-22 16:54:46.418087 lux-explainer-1.0.1/
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     1063 2024-01-29 09:30:50.000000 lux-explainer-1.0.1/LICENSE
--rw-r--r--   0 sbk       (1000) sbk       (1000)     8477 2024-02-22 16:54:46.418087 lux-explainer-1.0.1/PKG-INFO
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     6331 2024-02-22 16:53:31.000000 lux-explainer-1.0.1/README.md
--rw-rw-r--   0 sbk       (1000) sbk       (1000)      953 2024-02-22 16:48:34.000000 lux-explainer-1.0.1/pyproject.toml
--rw-rw-r--   0 sbk       (1000) sbk       (1000)       38 2024-02-22 16:54:46.418087 lux-explainer-1.0.1/setup.cfg
-drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-02-22 16:54:46.418087 lux-explainer-1.0.1/src/
-drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-02-22 16:54:46.418087 lux-explainer-1.0.1/src/lux/
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     7247 2024-02-22 11:24:27.000000 lux-explainer-1.0.1/src/lux/UncertainSMOTE.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)       22 2024-02-22 11:28:53.000000 lux-explainer-1.0.1/src/lux/__init__.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)    36594 2024-02-22 12:54:33.000000 lux-explainer-1.0.1/src/lux/lux.py
-drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-02-22 16:54:46.418087 lux-explainer-1.0.1/src/lux/pyuid3/
--rw-rw-r--   0 sbk       (1000) sbk       (1000)       22 2024-02-22 11:28:53.000000 lux-explainer-1.0.1/src/lux/pyuid3/__init__.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     4344 2024-01-29 10:15:03.000000 lux-explainer-1.0.1/src/lux/pyuid3/att_stats.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     2085 2024-01-29 10:15:03.000000 lux-explainer-1.0.1/src/lux/pyuid3/attribute.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)    16634 2024-01-29 10:15:03.000000 lux-explainer-1.0.1/src/lux/pyuid3/data.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     4453 2024-01-29 10:15:03.000000 lux-explainer-1.0.1/src/lux/pyuid3/data_scrambler.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     2365 2024-01-29 10:15:03.000000 lux-explainer-1.0.1/src/lux/pyuid3/entropy_evaluator.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     1097 2024-01-29 10:15:03.000000 lux-explainer-1.0.1/src/lux/pyuid3/instance.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)      231 2024-01-29 10:15:03.000000 lux-explainer-1.0.1/src/lux/pyuid3/parse_exception.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     3290 2024-01-29 10:15:03.000000 lux-explainer-1.0.1/src/lux/pyuid3/reading.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)    24413 2024-02-22 16:45:22.000000 lux-explainer-1.0.1/src/lux/pyuid3/tree.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)      527 2024-01-29 10:15:03.000000 lux-explainer-1.0.1/src/lux/pyuid3/tree_edge.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     7595 2024-01-29 10:15:03.000000 lux-explainer-1.0.1/src/lux/pyuid3/tree_evaluator.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     1528 2024-01-29 10:15:03.000000 lux-explainer-1.0.1/src/lux/pyuid3/tree_node.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)    30277 2024-02-22 12:00:00.000000 lux-explainer-1.0.1/src/lux/pyuid3/uid3.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     1157 2024-01-29 10:15:03.000000 lux-explainer-1.0.1/src/lux/pyuid3/utils.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     1395 2024-01-29 10:15:03.000000 lux-explainer-1.0.1/src/lux/pyuid3/value.py
-drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-02-22 16:54:46.418087 lux-explainer-1.0.1/src/lux_explainer.egg-info/
--rw-r--r--   0 sbk       (1000) sbk       (1000)     8477 2024-02-22 16:54:46.000000 lux-explainer-1.0.1/src/lux_explainer.egg-info/PKG-INFO
--rw-rw-r--   0 sbk       (1000) sbk       (1000)      742 2024-02-22 16:54:46.000000 lux-explainer-1.0.1/src/lux_explainer.egg-info/SOURCES.txt
--rw-rw-r--   0 sbk       (1000) sbk       (1000)        1 2024-02-22 16:54:46.000000 lux-explainer-1.0.1/src/lux_explainer.egg-info/dependency_links.txt
--rw-rw-r--   0 sbk       (1000) sbk       (1000)      227 2024-02-22 16:54:46.000000 lux-explainer-1.0.1/src/lux_explainer.egg-info/requires.txt
--rw-rw-r--   0 sbk       (1000) sbk       (1000)        4 2024-02-22 16:54:46.000000 lux-explainer-1.0.1/src/lux_explainer.egg-info/top_level.txt
+drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-04-30 10:43:44.283125 lux_explainer-1.2.0/
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     1063 2024-01-29 09:30:50.000000 lux_explainer-1.2.0/LICENSE
+-rw-r--r--   0 sbk       (1000) sbk       (1000)     8662 2024-04-30 10:43:44.283125 lux_explainer-1.2.0/PKG-INFO
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     6383 2024-03-20 13:56:27.000000 lux_explainer-1.2.0/README.md
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     1066 2024-04-30 08:23:51.000000 lux_explainer-1.2.0/pyproject.toml
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)       38 2024-04-30 10:43:44.283125 lux_explainer-1.2.0/setup.cfg
+drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-04-30 10:43:44.275125 lux_explainer-1.2.0/src/
+drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-04-30 10:43:44.279125 lux_explainer-1.2.0/src/lux/
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     7114 2024-03-09 15:54:20.000000 lux_explainer-1.2.0/src/lux/UncertainSMOTE.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)       22 2024-03-08 10:52:00.000000 lux_explainer-1.2.0/src/lux/__init__.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)    46500 2024-04-30 07:41:18.000000 lux_explainer-1.2.0/src/lux/lux.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     8830 2024-04-29 12:39:41.000000 lux_explainer-1.2.0/src/lux/metrics.py
+drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-04-30 10:43:44.283125 lux_explainer-1.2.0/src/lux/pyuid3/
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)       22 2024-02-22 11:28:53.000000 lux_explainer-1.2.0/src/lux/pyuid3/__init__.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     4344 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/att_stats.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     2085 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/attribute.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)    16634 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/data.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     4453 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/data_scrambler.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     2365 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/entropy_evaluator.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     1097 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/instance.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)      231 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/parse_exception.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     3290 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/reading.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)    24853 2024-04-30 08:17:57.000000 lux_explainer-1.2.0/src/lux/pyuid3/tree.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)      527 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/tree_edge.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     7595 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/tree_evaluator.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     1528 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/tree_node.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)    30251 2024-04-30 07:45:14.000000 lux_explainer-1.2.0/src/lux/pyuid3/uid3.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     1157 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/utils.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     1395 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/value.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)    12662 2024-04-30 07:37:40.000000 lux_explainer-1.2.0/src/lux/samplers.py
+drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-04-30 10:43:44.283125 lux_explainer-1.2.0/src/lux_explainer.egg-info/
+-rw-r--r--   0 sbk       (1000) sbk       (1000)     8662 2024-04-30 10:43:44.000000 lux_explainer-1.2.0/src/lux_explainer.egg-info/PKG-INFO
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)      781 2024-04-30 10:43:44.000000 lux_explainer-1.2.0/src/lux_explainer.egg-info/SOURCES.txt
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)        1 2024-04-30 10:43:44.000000 lux_explainer-1.2.0/src/lux_explainer.egg-info/dependency_links.txt
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)      227 2024-04-30 10:43:44.000000 lux_explainer-1.2.0/src/lux_explainer.egg-info/requires.txt
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)        4 2024-04-30 10:43:44.000000 lux_explainer-1.2.0/src/lux_explainer.egg-info/top_level.txt
```

### Comparing `lux-explainer-1.0.1/LICENSE` & `lux_explainer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lux-explainer-1.0.1/PKG-INFO` & `lux_explainer-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lux-explainer
-Version: 1.0.1
+Version: 1.2.0
 Summary: Universal Local Rule-based Explainer
-Author-email: LUX <szymon.bobek@gmail.com>
+Author-email: Szymon Bobek <szymon.bobek@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 sbobek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -22,14 +22,16 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/sbobek/lux
+Project-URL: Documentation, https://lux-explainer.readthedocs.org
+Project-URL: Issues, https://github.com/sbobek/lux/issues
 Keywords: xai,explainability,model-agnostic,rule-based
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -45,15 +47,15 @@
 Requires-Dist: anchor-exp>=0.0.2.0
 Requires-Dist: imbalanced-learn>=0.9.1
 Requires-Dist: gower>=0.1.2
 Requires-Dist: numdifftools>=0.9.41
 
 # LUX (Local Universal Rule-based Explainer)
 ## Main features
-  <img align="right"  src="./pix/lux-logo.png" width="200">
+  <img align="right"  src="https://raw.githubusercontent.com/sbobek/lux/main/pix/lux-logo.png" width="200">
   
   * Model-agnostic, rule-based and visual local explanations of black-box ML models
   * Integrated counterfactual explanations
   * Rule-based explanations (that are executable at the same time)
   * Oblique trees backbone, which allows to explain more reliable linear decision boundaries
   * Integration with [Shapley values](https://shap.readthedocs.io/en/latest/) or [Lime](https://github.com/marcotcr/lime) importances (or any other explainer that produces importances) that help in generating high quality rules
   
@@ -78,26 +80,26 @@
 
 ```
 pip install lux-explainer
 ```
 If you want to use LUX with [JupyterLab](https://jupyter.org/) install it and run:
 
 ```
-pip isntall jupyterlab
+pip installta jupyterlab
 jupyter lab
 ```
 
 **Caution**: If you want to use LUX with categorical data, it is advised to use [multiprocessing gower distance](https://github.com/sbobek/gower/tree/add-multiprocessing) package (due to high computational complexity of the problem). 
 
 ## Usage
 
   * For complete usage see [lux_usage_example.ipynb](https://raw.githubusercontent.com/sbobek/lux/main/examples/lux_usage_example.ipynb)
   * Fos usage example with Shap integration see [lux_usage_example_shap.ipynb](https://raw.githubusercontent.com/sbobek/lux/main/examples/lux_usage_example_shap.ipynb)
 
-### Simple exmaple on Iris dataset
+### Simple example on Iris dataset
 
 ``` python
 from lux.lux import LUX
 from sklearn import datasets
 from sklearn.model_selection import train_test_split
 from sklearn import svm
 import numpy as np
@@ -131,15 +133,15 @@
 ```
 
 The above code should give you the answer as follows:
 ```
 ['IF petal_length >= 5.15 THEN class = 2 # 0.9833409059468439\n']
 ```
 
-Alternatively one can get counterfactual explanation for agiven instance by calling:
+Alternatively one can get counterfactual explanation for a given instance by calling:
 
 ``` python
 cf = lux.counterfactual(np.array(iris_instance), train[features], counterfactual_representative='nearest', topn=1)[0]
 print(f"Counterfactual for {iris_instance} to change from class {lux.predict(np.array(iris_instance))[0]} to class {cf['prediction']}: \n{cf['counterfactual']}")
 ```
 The result from the above query should look as follows:
 
@@ -148,15 +150,15 @@
 sepal_length    6.9
 sepal_width     3.1
 petal_length    5.1
 petal_width     2.3
 ```
 
 ### Rule-based model for local uncertain explanations
-You can obtain a whole rule-based model for the local uncertian explanation that was generated by LUX for given instance by running following code
+You can obtain a whole rule-based model for the local uncertain explanation that was generated by LUX for given instance by running following code
 
 ``` python
 #have a look at the entire rule-based model that can be executed with https:://heartdroid.re
 print(lux.to_HMR())
 ```
 
 This will generate model which can later be executed by [HeaRTDroid](https://heartdroid.re)
@@ -201,15 +203,15 @@
 from IPython.display import SVG, Image
 lux.uid3.tree.save_dot('tree.dot',fmt='.2f',visual=True, background_data=train)
 gvz=graphviz.Source.from_file('tree.dot')
 !dot -Tpng tree.dot > tree.png
 Image('tree.png')
 ```
 
-The code should yeld something like that (depending on the instance that was selected):
+The code should yield something like that (depending on the instance that was selected):
 
 ![](https://raw.githubusercontent.com/sbobek/lux/main/pix/utree.png)
 
 # Cite this work
 
 ```
 @misc{bobek2023local,
```

### Comparing `lux-explainer-1.0.1/README.md` & `lux_explainer-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # LUX (Local Universal Rule-based Explainer)
 ## Main features
-  <img align="right"  src="./pix/lux-logo.png" width="200">
+  <img align="right"  src="https://raw.githubusercontent.com/sbobek/lux/main/pix/lux-logo.png" width="200">
   
   * Model-agnostic, rule-based and visual local explanations of black-box ML models
   * Integrated counterfactual explanations
   * Rule-based explanations (that are executable at the same time)
   * Oblique trees backbone, which allows to explain more reliable linear decision boundaries
   * Integration with [Shapley values](https://shap.readthedocs.io/en/latest/) or [Lime](https://github.com/marcotcr/lime) importances (or any other explainer that produces importances) that help in generating high quality rules
   
@@ -29,26 +29,26 @@
 
 ```
 pip install lux-explainer
 ```
 If you want to use LUX with [JupyterLab](https://jupyter.org/) install it and run:
 
 ```
-pip isntall jupyterlab
+pip installta jupyterlab
 jupyter lab
 ```
 
 **Caution**: If you want to use LUX with categorical data, it is advised to use [multiprocessing gower distance](https://github.com/sbobek/gower/tree/add-multiprocessing) package (due to high computational complexity of the problem). 
 
 ## Usage
 
   * For complete usage see [lux_usage_example.ipynb](https://raw.githubusercontent.com/sbobek/lux/main/examples/lux_usage_example.ipynb)
   * Fos usage example with Shap integration see [lux_usage_example_shap.ipynb](https://raw.githubusercontent.com/sbobek/lux/main/examples/lux_usage_example_shap.ipynb)
 
-### Simple exmaple on Iris dataset
+### Simple example on Iris dataset
 
 ``` python
 from lux.lux import LUX
 from sklearn import datasets
 from sklearn.model_selection import train_test_split
 from sklearn import svm
 import numpy as np
@@ -82,15 +82,15 @@
 ```
 
 The above code should give you the answer as follows:
 ```
 ['IF petal_length >= 5.15 THEN class = 2 # 0.9833409059468439\n']
 ```
 
-Alternatively one can get counterfactual explanation for agiven instance by calling:
+Alternatively one can get counterfactual explanation for a given instance by calling:
 
 ``` python
 cf = lux.counterfactual(np.array(iris_instance), train[features], counterfactual_representative='nearest', topn=1)[0]
 print(f"Counterfactual for {iris_instance} to change from class {lux.predict(np.array(iris_instance))[0]} to class {cf['prediction']}: \n{cf['counterfactual']}")
 ```
 The result from the above query should look as follows:
 
@@ -99,15 +99,15 @@
 sepal_length    6.9
 sepal_width     3.1
 petal_length    5.1
 petal_width     2.3
 ```
 
 ### Rule-based model for local uncertain explanations
-You can obtain a whole rule-based model for the local uncertian explanation that was generated by LUX for given instance by running following code
+You can obtain a whole rule-based model for the local uncertain explanation that was generated by LUX for given instance by running following code
 
 ``` python
 #have a look at the entire rule-based model that can be executed with https:://heartdroid.re
 print(lux.to_HMR())
 ```
 
 This will generate model which can later be executed by [HeaRTDroid](https://heartdroid.re)
@@ -152,15 +152,15 @@
 from IPython.display import SVG, Image
 lux.uid3.tree.save_dot('tree.dot',fmt='.2f',visual=True, background_data=train)
 gvz=graphviz.Source.from_file('tree.dot')
 !dot -Tpng tree.dot > tree.png
 Image('tree.png')
 ```
 
-The code should yeld something like that (depending on the instance that was selected):
+The code should yield something like that (depending on the instance that was selected):
 
 ![](https://raw.githubusercontent.com/sbobek/lux/main/pix/utree.png)
 
 # Cite this work
 
 ```
 @misc{bobek2023local,
```

### Comparing `lux-explainer-1.0.1/pyproject.toml` & `lux_explainer-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lux-explainer"
-version = "1.0.1"
+version = "1.2.0"
 description = "Universal Local Rule-based Explainer"
 readme = "README.md"
-authors = [{ name = "LUX", email = "szymon.bobek@gmail.com" }]
+authors = [{ name = "Szymon Bobek", email = "szymon.bobek@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["xai", "explainability", "model-agnostic", "rule-based"]
@@ -29,8 +29,10 @@
     "gower>=0.1.2",
     "numdifftools>=0.9.41"
 ]
 requires-python = ">=3.8"
 
 
 [project.urls]
-Homepage = "https://github.com/sbobek/lux"
+Homepage = "https://github.com/sbobek/lux"
+Documentation = "https://lux-explainer.readthedocs.org"
+Issues = "https://github.com/sbobek/lux/issues"
```

### Comparing `lux-explainer-1.0.1/src/lux/UncertainSMOTE.py` & `lux_explainer-1.2.0/src/lux/UncertainSMOTE.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,16 @@
 __all__ = ['UncertainSMOTE']
 
 from imblearn.over_sampling._smote.base import BaseSMOTE
-import numpy as np 
-
-import math
-import numbers
+import numpy as np
 import warnings
-from collections import Counter
-
 from scipy import sparse
-from sklearn.preprocessing import OneHotEncoder, OrdinalEncoder
 from sklearn.utils import _safe_indexing, check_array, check_random_state
 from sklearn.metrics import pairwise_distances
 
-from imblearn.utils import Substitution, check_target_type
-from imblearn.utils._docstring import _n_jobs_docstring, _random_state_docstring
-
 
 class UncertainSMOTE(BaseSMOTE):
         
     def __init__(
         self,
         *,
         predict_proba,
@@ -29,14 +20,27 @@
         n_jobs=None,
         sigma=1,
         m_neighbors=10,
         min_samples=0.1,
         instance_to_explain=None, 
         kind="borderline-1",
     ):
+        """
+
+        :param predict_proba:
+        :param sampling_strategy:
+        :param random_state:
+        :param k_neighbors:
+        :param n_jobs:
+        :param sigma:
+        :param m_neighbors:
+        :param min_samples:
+        :param instance_to_explain:
+        :param kind:
+        """
         super().__init__(
             sampling_strategy=sampling_strategy,
             random_state=random_state,
             k_neighbors=k_neighbors,
             n_jobs=n_jobs,
         )
         self.m_neighbors = m_neighbors
@@ -44,14 +48,20 @@
         self.predict_proba=predict_proba
         self.sigma=sigma
         self.min_samples=min_samples
         self.instance_to_explain = instance_to_explain
 
 
     def _fit_resample(self, X, y):
+        """
+
+        :param X:
+        :param y:
+        :return:
+        """
         # FIXME: to be removed in 0.12
         if self.n_jobs is not None:
             warnings.warn(
                 "The parameter `n_jobs` has been deprecated in 0.10 and will be "
                 "removed in 0.12. You can pass an nearest neighbors estimator where "
                 "`n_jobs` is already set instead.",
                 FutureWarning,
@@ -140,38 +150,30 @@
                 y_resampled = np.hstack((y_resampled, y_new_1, y_new_2))
 
         return X_resampled, y_resampled
     
     
     
     def _in_danger_noise(self, predict_proba, samples, target_class, y, kind="danger"):
-        """Estimate if a set of sample are in danger or noise.
-        Used by BorderlineSMOTE and SVMSMOTE.
-        Parameters
-        ----------
-        nn_estimator : estimator object
-            An estimator that inherits from
-            :class:`~sklearn.neighbors.base.KNeighborsMixin` use to determine
-            if a sample is in danger/noise.
-            NOT USED
-        samples : {array-like, sparse matrix} of shape (n_samples, n_features)
-            The samples to check if either they are in danger or not.
-        target_class : int or str
-            The target corresponding class being over-sampled.
-        y : array-like of shape (n_samples,)
-            The true label in order to check the neighbour labels.
-            NOT USED
-        kind : {'danger', 'noise'}, default='danger'
+        """
+        Estimate if a set of sample are in danger or noise.
+        :param predict_proba:
+           function returning probability estimates for samples
+        :param samples: {array-like, sparse matrix} of shape (n_samples, n_features).
+           The samples to check if either they are in danger or not.
+        :param target_class: nt or str.
+           The target corresponding class being over-sampled.
+        :param y: array-like of shape (n_samples,).
+           The true label in order to check the neighbour labels.
+        :param kind: {'danger', 'noise'}, default='danger'
             The type of classification to use. Can be either:
             - If 'danger', check if samples are in danger,
             - If 'noise', check if samples are noise.
-        Returns
-        -------
-        output : ndarray of shape (n_samples,)
-            A boolean array where True refer to samples in danger or noise.
+
+        :return: ndarray of shape (n_samples,). A boolean array where True refer to samples in danger or noise.
         """
         
         c_labels  = samples[np.argmax(self.predict_proba(samples),axis=1) ==target_class]
         prediction_certainty = np.max(self.predict_proba(c_labels),axis=1)
         
         #shuld this be thresholded like that, or keep n-lowest?
         confidence_threshold = np.mean(prediction_certainty)-self.sigma*np.std(prediction_certainty) #changed to + (plus)
```

### Comparing `lux-explainer-1.0.1/src/lux/lux.py` & `lux_explainer-1.2.0/src/lux/lux.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,32 +10,84 @@
 from sklearn.cluster import OPTICS
 import shap
 import sklearn
 import gower
 import numpy as np
 import warnings
 
-from sklearn.linear_model import LinearRegression
-import numdifftools as nd
+from lux.samplers import ImportanceSampler
 
 
 class LUX(BaseEstimator):
+    """
+    This class contains functions that implement generation of local rule-based model-agnostic explanations.
+    (np.array(iris_instance))
+    """
+
     REPRESENTATIVE_CENTROID = "centroid"
+    "REPRESENTATIVE_CENTROID (:obj:`str`): A constant representing centroid as the representative strategy."
+
     REPRESENTATIVE_NEAREST = "nearest"
+    "REPRESENTATIVE_NEAREST (:obj:`str`): A constant representing nearest as the representative strategy."
 
     CF_REPRESENTATIVE_MEDOID = "medoid"
+    "CF_REPRESENTATIVE_MEDOID (:obj:`str`): A constant representing medoid as the counterfactual representative strategy."
+
     CF_REPRESENTATIVE_NEAREST = "nearest"
+    "CF_REPRESENTATIVE_NEAREST (:obj:`str`): A constant representing nearest as the counterfactual representative strategy."
 
     OS_STRATEGY_SMOTE = 'smote'
+    "OS_STRATEGY_SMOTE (:obj:`str`): A constant representing SMOTE as the oversampling strategy."
+
     OS_STRATEGY_IMPORTANCE = 'importance'
+    "OS_STRATEGY_IMPORTANCE (:obj:`str`): A constant representing importance sampling as the oversampling strategy."
+
     OS_STRATEGY_BOTH = 'both'
+    "OS_STRATEGY_BOTH (:obj:`str`): A constant representing both SMOTE and importance sampling as the oversampling strategy."
 
-    def __init__(self, predict_proba, classifier=None, neighborhood_size=0.1, max_depth=2, node_size_limit=1,
+    def __init__(self, predict_proba, classifier=None, neighborhood_size=0.1, max_depth=None, node_size_limit=1,
                  grow_confidence_threshold=0, min_impurity_decrease=0, min_samples=5, min_generate_samples=0.02,
-                 uncertainty_sigma=2, oversampling_strategy='smote'):
+                 uncertainty_sigma=2, oversampling_strategy='both'):
+        """ Initialize the LUX explainer model.
+
+        :param predict_proba: callable
+            The predict_proba function of the balckbox classifier.
+        :type predict_proba: callable
+        :param classifier: object, optional
+            The underlying classifier. If it is provided the SHAP-based sampling can be used.
+        :param neighborhood_size: float, optional
+            The neighborhood size for generating explanations. Default is 0.1.
+        :type neighborhood_size: float
+        :param max_depth: int, optional
+            The maximum depth of the decision tree. Default is None meaning no limit.
+        :type max_depth: int
+        :param node_size_limit: int, optional
+            The minimum number of samples required to split an internal node. Default is 1.
+        :type node_size_limit: int
+        :param grow_confidence_threshold: float, optional
+            The threshold for growing decision tree nodes. Default is 0.
+        :type grow_confidence_threshold: float
+        :param min_impurity_decrease: float, optional
+            A node will be split if this split induces a decrease of the impurity greater than or equal to this value.
+            Default is 0.
+        :type min_impurity_decrease: float
+        :param min_samples: int, optional
+            The minimum number of samples required to be at a leaf node. Default is 5.
+        :type min_samples: int
+        :param min_generate_samples: float, optional
+            The minimum proportion of the dataset size to generate perturbed instances. This is used by the UncertainSMOTE algotrothm. Default is 0.02.
+        :type min_generate_samples: float
+        :param uncertainty_sigma: float, optional
+            The uncertainty parameter sigma used in the filtering uncertain samples. Every sample that is 2*uncertainty_sigma away from the mean will be removed. Default is 2.
+        :type uncertainty_sigma: float
+        :param oversampling_strategy: str, optional
+            The strategy for oversampling. It can be 'smote', 'importance', or 'both'. Default is 'smote'.
+        :type oversampling_strategy: str
+        """
+
         self.neighborhood_size = neighborhood_size
         self.max_depth = max_depth
         self.node_size_limit = node_size_limit
         self.grow_confidence_threshold = grow_confidence_threshold
         self.predict_proba = predict_proba
         self.attributes_names = None
         self.min_impurity_decrease = min_impurity_decrease
@@ -46,18 +98,88 @@
         self.oversampling_strategy = oversampling_strategy
         self.uncertainty_sigma = uncertainty_sigma
 
         if classifier is None:
             self.oversampling_strategy = self.OS_STRATEGY_SMOTE
 
     def fit(self, X, y, instance_to_explain, X_importances=None, exclude_neighbourhood=False, use_parity=True,
-            parity_strategy='global', inverse_sampling=False, class_names=None, discount_importance=False,
+            parity_strategy='global', inverse_sampling=True, class_names=None, discount_importance=False,
             uncertain_entropy_evaluator=UncertainEntropyEvaluator(), beta=1, representative='centroid',
-            density_sampling=False, radius_sampling=False, oversampling=False, categorical=None, prune=False,
+            density_sampling=False, radius_sampling=False, oversampling=False, categorical=None, prune=True,
             oblique=False, n_jobs=None):
+        """ Fit the LUX explainer model.
+
+        :param X:
+            The input data used to train the model.
+        :type X: pandas.DataFrame
+        :param y:
+            The target values corresponding to the input data.
+        :type y: array-like
+        :param instance_to_explain:
+            The instance(s) to explain. Can be a single instance or a list/array of instances. The instances are not explained one after another, but the neighbourhood is created
+            for the whole set of instances. Hence, they form so called bounding box for the explanation.
+        :type instance_to_explain: array-like or list
+        :param X_importances: optional
+            The importances of features in the input data. If provided as a DataFrame, column names should match feature names.
+        :type X_importances: array-like or pandas.DataFrame or None
+        :param exclude_neighbourhood: optional
+            Whether to exclude the neighborhood of the instance(s) being explained. Default is False.
+        :type exclude_neighbourhood: bool
+        :param use_parity: optional
+            Whether to use parity constraints in explanation generation. Default is True.
+        :type use_parity: bool
+        :param parity_strategy: optional
+            The strategy for applying parity constraints. It can be 'global' or 'local'. Default is 'global'.
+        :type parity_strategy: str
+        :param inverse_sampling: optional
+            Whether to use inverse sampling for feature selection. Default is True.
+        :type inverse_sampling: bool
+        :param class_names: optional
+            The names of the classes. If not provided, inferred from the target values.
+        :type class_names: array-like or None
+        :param discount_importance: optional
+            Whether to discount feature importance. Default is False.
+        :type discount_importance: bool
+        :param uncertain_entropy_evaluator: optional
+            The evaluator for uncertain entropy. Default is UncertainEntropyEvaluator().
+        :type uncertain_entropy_evaluator: object
+        :param beta: optional
+            The beta parameter for F-beta score used in uncertain entropy computation. Default is 1.
+        :type beta: float
+        :param representative: optional
+            The representative method for selecting representative instances. It can be 'centroid' or 'prototype'.
+            Default is 'centroid'.
+        :type representative: str
+        :param density_sampling: optional
+            Whether to use density-based sampling for instance selection. Default is False.
+        :type density_sampling: bool
+        :param radius_sampling: optional
+            Whether to use radius-based sampling for instance selection. Default is False.
+        :type radius_sampling: bool
+        :param oversampling: optional
+            Whether to perform oversampling of instances. Default is False.
+        :type oversampling: bool
+        :param categorical: optional
+            A list indicating whether each feature is categorical or not.
+        :type categorical: array-like or None
+        :param prune: optional
+            Whether to prune branches in decision tree that produces splits which do not change classification result. Default is True.
+        :type prune: bool
+        :param oblique: optional
+            Whether to use oblique decision rules. Default is False.
+        :type oblique: bool
+        :param n_jobs: optional
+            The number of parallel jobs to run. Default is None.
+        :type n_jobs: int or None
+
+        :return:
+            The trained LUX explainer model.
+        :rtype: lux.lux.LUX
+        """
+
         if class_names is None:
             class_names = np.unique(y)
         if class_names is not None and len(class_names) != len(np.unique(y)):
             raise ValueError('Length of class_names not aligned with number of classess in y')
 
         self.attributes_names = X.columns
         self.categorical = categorical
@@ -82,18 +204,69 @@
                 raise ValueError('Dimensions of point to explain not aligned with dataset')
 
     def fit_bounding_boxes(self, X, y, boundiong_box_points, X_importances=None, exclude_neighbourhood=False,
                            use_parity=True, parity_strategy='global', inverse_sampling=False, class_names=None,
                            discount_importance=False, uncertain_entropy_evaluator=UncertainEntropyEvaluator(), beta=1,
                            representative='centroid', density_sampling=False, radius_sampling=False, oversampling=False,
                            categorical=None, prune=False, oblique=False, n_jobs=None):
+        """ Fit LUX explainer model for the neighbourhood data defined by the bounding box constructed of several points.
+        Usually only one point is provided.
+
+        :param X:
+            Input features.
+        :type X: array-like or sparse matrix of shape (n_samples, n_features)
+        :param y:
+            Target values.
+        :param bounding_box_points:
+            Points defining the bounding box.
+        :type bounding_box_points: array-like of shape (n_points, n_dimensions)
+        :param X_importances:
+            Importance matrix for features. Default is None.
+        :param exclude_neighbourhood:
+            Whether to exclude neighborhood points. Default is False.
+        :param use_parity:
+            Whether to use parity. Default is True.
+        :param parity_strategy:
+            Strategy for parity. Default is 'global'.
+        :param inverse_sampling:
+            Whether to use inverse sampling. Default is False.
+        :param class_names:
+            Names of classes. Default is None.
+        :param discount_importance:
+            Whether to discount importance. Default is False.
+        :param uncertain_entropy_evaluator:
+            Evaluator for uncertain entropy. Default is UncertainEntropyEvaluator().
+        :param beta:
+            Beta value for fitting. Default is 1.
+        :param representative:
+            Representative strategy. Default is 'centroid'.
+        :param density_sampling:
+            Whether to use density sampling. Default is False.
+        :param radius_sampling:
+            Whether to use radius sampling. Default is False.
+        :param oversampling:
+            Whether to use oversampling. Default is False.
+        :param categorical:
+            Categorical information. Default is None.
+        :param prune:
+            Whether to prune. Default is False.
+        :param oblique:
+            Whether to use oblique splits. Default is False.
+        :param n_jobs:
+            Number of jobs to run in parallel. Default is None.
+
+        Raises:
+        :raises ValueError:
+            If the length of class_names does not match the number of classes in y,
+                           or if bounding_box_points is not 2D.
+        """
         if class_names is None:
             class_names = np.unique(y)
         if class_names is not None and len(class_names) != len(np.unique(y)):
-            raise ValueError('Length of class_names not aligned with number of classess in y')
+            raise ValueError('Length of class_names not aligned with number of classes in y')
 
         if isinstance(boundiong_box_points, (list)):
             boundiong_box_points = np.array(boundiong_box_points)
         if len(boundiong_box_points.shape) != 2:
             raise ValueError('Bounding box should be 2D.')
 
         if X_importances is not None:
@@ -149,38 +322,85 @@
                                       discount_importance=discount_importance, beta=beta, prune=prune, oblique=oblique,
                                       n_jobs=n_jobs)
 
     def create_sample_bb(self, X, y, boundiong_box_points, X_importances=None, exclude_neighbourhood=False,
                          use_parity=True, parity_strategy='global', inverse_sampling=False, class_names=None,
                          representative='centroid', density_sampling=False, radius_sampling=False, radius=None,
                          oversampling=False, categorical=None, n_jobs=None):
+        """ Create a sample for the LUX explainer to be fitted to, based on the provided data.
+
+
+        :param X:
+           Input features.
+        :type X: array-like or sparse matrix of shape (n_samples, n_features)
+        :param y:
+           Target values.
+        :param bounding_box_points:
+           Points defining the bounding box.
+        :type bounding_box_points: array-like of shape (n_points, n_dimensions)
+        :param X_importances:
+           Importance matrix for features. Default is None.
+        :param exclude_neighbourhood:
+           Whether to exclude neighborhood points. Default is False.
+        :param use_parity:
+           Whether to use parity. Default is True.
+        :param parity_strategy:
+           Strategy for parity. Default is 'global'.
+        :param inverse_sampling:
+           Whether to use inverse sampling. Default is False.
+        :param class_names:
+           Names of classes. Default is None.
+        :param representative:
+           Representative strategy. Default is 'centroid'.
+        :param density_sampling:
+           Whether to use density sampling. Default is False.
+        :param radius_sampling:
+           Whether to use radius sampling. Default is False.
+        :param radius:
+           Radius for radius sampling. Default is None.
+        :param oversampling:
+           Whether to use oversampling. Default is False.
+        :param categorical:
+           Categorical information. Default is None.
+        :param n_jobs:
+           Number of jobs to run in parallel. Default is None.
+
+        Returns:
+        :return: X_train_sample:
+           Sampled input features.
+        :rtype: array-like or sparse matrix of shape (n_samples, n_features)
+        :return: X_train_sample_importances:
+           Sampled importance matrix for features.
+        :rtype: pd.DataFrame or None
+        """
         neighbourhoods = []
         importances = []
 
         if X_importances is not None:
             if not isinstance(X_importances, pd.DataFrame):
                 raise ValueError('Feature importance matrix has to be DataFrame.')
 
         if categorical is None or sum(categorical) == 0:
             metric = 'minkowski'
         else:
             metric = 'precomputed'
 
+        # TODO: if classifier is present, then use it to obtain SHAP, thenm
+
         if use_parity:
             for instance_to_explain in boundiong_box_points:
                 nn_instance_to_explain = np.array(instance_to_explain).reshape(1, -1)
                 instance_class = np.argmax(self.predict_proba(np.array(instance_to_explain).reshape(1, -1)))
                 class_names_instance_last = [c for c in class_names if c not in [instance_class]] + [instance_class]
                 neighbourhoods_bbox = []
                 importances_bbox = []
                 for c in class_names_instance_last:
                     X_c_only = X[y == c]
                     if self.neighborhood_size <= 1.0:
                         n_neighbors = min(len(X_c_only) - 1, max(1, int(self.neighborhood_size * len(X_c_only))))
-                        # TODO ADD WARNING
                         nn = NearestNeighbors(n_neighbors=max(1, int(n_neighbors / len(boundiong_box_points))),
                                               n_jobs=n_jobs)
                     else:
                         min_occurances_lables = list(np.array(y)).count(c)
                         if self.neighborhood_size > min_occurances_lables:
                             n_neighbors = min_occurances_lables
                             warnings.warn(
@@ -201,16 +421,17 @@
                                                                                                 nn=nn, n_jobs=n_jobs)
                         neighbourhoods_bbox += neighbourhoods_bbox_inv
                         if X_importances is not None:
                             importances_bbox += importances_bbox_inv
 
                     if metric == 'precomputed':
                         ids_c = \
-                        gower.gower_topn(nn_instance_to_explain, X_c_only, cat_features=categorical, n=nn.n_neighbors,
-                                         n_jobs=n_jobs)['index']
+                            gower.gower_topn(nn_instance_to_explain, X_c_only, cat_features=categorical,
+                                             n=nn.n_neighbors,
+                                             n_jobs=n_jobs)['index']
                     else:
                         nn.fit(X_c_only.values)
                         _, ids_c = nn.kneighbors(nn_instance_to_explain)
                     neighbourhoods_bbox.append(X_c_only.iloc[ids_c.ravel()])
                     if X_importances is not None:
                         X_c_only_importances = X_importances.loc[(y == c)]
                         neighbourhood_importances = X_c_only_importances.iloc[ids_c.ravel()]
@@ -224,15 +445,14 @@
             X_train_sample = X_train_sample[~X_train_sample.index.duplicated(keep='first')]
 
             if X_importances is not None:
                 X_train_sample_importances = pd.concat(importances)
                 X_train_sample_importances = X_train_sample_importances[
                     ~X_train_sample_importances.index.duplicated(keep='first')]
 
-            # TODO: filter out samples which are further away than the max distance to the point in nearest class
             #########################################
             if parity_strategy == 'local':
                 X_train_sample_c = X_train_sample.copy()
                 attributes = [a for a in X_train_sample]
                 X_train_sample_c['target'] = np.argmax(self.predict_proba(X_train_sample_c), axis=1)
                 representations = X_train_sample_c.groupby('target').agg(np.median)
                 representations['target'] = np.argmax(self.predict_proba(representations[attributes]))
@@ -265,16 +485,16 @@
 
             if metric != 'precomputed':
                 nn.fit(X_c_only.values)
             for instance_to_explain in boundiong_box_points:
                 nn_instance_to_explain = np.array(instance_to_explain).reshape(1, -1)
                 if metric == 'precomputed':
                     ids_c = \
-                    gower.gower_topn(nn_instance_to_explain, X_c_only, cat_features=categorical, n=nn.n_neighbors,
-                                     n_jobs=n_jobs)['index']
+                        gower.gower_topn(nn_instance_to_explain, X_c_only, cat_features=categorical, n=nn.n_neighbors,
+                                         n_jobs=n_jobs)['index']
                 else:
                     _, ids_c = nn.kneighbors(nn_instance_to_explain)
                 neighbourhoods.append(X_c_only.iloc[ids_c.ravel()])
                 if X_importances is not None:
                     neighbourhood_importances = X_importances.iloc[ids_c.ravel()]
 
             X_train_sample = X_c_only[X_c_only.index.isin(pd.concat(neighbourhoods).index)]
@@ -333,38 +553,59 @@
                 X_train_sample_importances = X_importances.iloc[idxs]
 
         if exclude_neighbourhood:
             X_train_sample = X.loc[~X_train_sample.index]
             if X_importances is not None:
                 X_train_sample_importances = X_importances.loc[~X_train_sample_importances.index]
 
+        # in case of dim reduciton, here is where we need to go back to original feature-space
+        # the return should be made based on the indices from the X_train_sample
         if oversampling:
             if X_importances is not None:
                 warnings.warn("WARNING: X_importances have no effect when oversampling is True.")
                 X_importances = None
             if self.oversampling_strategy == self.OS_STRATEGY_SMOTE:
                 instance_to_explain = boundiong_box_points[
                     0]  # Todo in case of BBozes, rasius should be calculated for all of them
                 X_train_sample = self.__oversample_smote(X_train_sample, categorical=categorical,
                                                          instance_to_explain=instance_to_explain)
             elif self.oversampling_strategy == self.OS_STRATEGY_IMPORTANCE:
                 instance_to_explain = boundiong_box_points[0]
-                X_train_sample = self.__importance_sampler(X_train_sample, instance_to_explain)
+                isam = ImportanceSampler(classifier=self.classifier, predict_proba=self.predict_proba,
+                                         indstance2explain=instance_to_explain,
+                                         min_generate_samples=self.min_generate_samples)
+                X_train_sample = isam.fit_transform(X_train_sample)
             elif self.oversampling_strategy == self.OS_STRATEGY_BOTH:
                 instance_to_explain = boundiong_box_points[0]
-                X_train_sample = self.__importance_sampler(X_train_sample, instance_to_explain)
                 X_train_sample = self.__oversample_smote(X_train_sample, categorical=categorical,
                                                          instance_to_explain=instance_to_explain)
+                isam = ImportanceSampler(classifier=self.classifier, predict_proba=self.predict_proba,
+                                         indstance2explain=instance_to_explain,
+                                         min_generate_samples=self.min_generate_samples)
+                X_train_sample = isam.fit_transform(X_train_sample)
+
+            cols = X_train_sample.columns
+            X_train_sample_arr = np.concatenate((X_train_sample, np.ones((int(0.3 * X_train_sample.shape[0]), X_train_sample.shape[1])) * instance_to_explain))
+            X_train_sample = pd.DataFrame(X_train_sample_arr, columns=cols)
 
         if X_importances is not None:
             return X_train_sample, X_train_sample_importances
         else:
             return X_train_sample, None
 
     def __oversample_smote(self, X_train_sample, sigma=1, iterations=1, instance_to_explain=None, categorical=None):
+        """ Generate samples based on their uncertainty.
+
+        :param X_train_sample:
+        :param sigma:
+        :param iterations:
+        :param instance_to_explain:
+        :param categorical:
+        :return:
+        """
         for iteration in np.arange(0, iterations):
             try:
                 sm = UncertainSMOTE(predict_proba=self.predict_proba, sigma=sigma, sampling_strategy='all',
                                     min_samples=self.min_generate_samples,
                                     instance_to_explain=instance_to_explain)
                 X_train_sample, _ = sm.fit_resample(X_train_sample,
                                                     np.argmax(self.predict_proba(X_train_sample), axis=1))
@@ -372,14 +613,29 @@
                 warnings.warn("WARNING: Selected class has low number of borderline points.")
 
         return X_train_sample
 
     def __inverse_sampling(self, X, y, instance_to_explain, nn, sampling_class_label, opposite_neighbourhood,
                            X_importances=None, representative='centroid', categorical=None, metric='minkowski',
                            n_jobs=None):
+        """ Samples instances from opposite classes making sure every class is well represented in the representative dataset.
+
+        :param X:
+        :param y:
+        :param instance_to_explain:
+        :param nn:
+        :param sampling_class_label:
+        :param opposite_neighbourhood:
+        :param X_importances:
+        :param representative:
+        :param categorical:
+        :param metric:
+        :param n_jobs:
+        :return:
+        """
         # representative as centropid (mean value), but cna be prototype, nearest, etc.
         X_sample = X[y == sampling_class_label]
         if X_importances is not None:
             X_importances_sample = X_importances[(y == sampling_class_label).values]
 
         nn_instance_to_explain = np.array(instance_to_explain).reshape(1, -1)
 
@@ -416,14 +672,20 @@
 
         if X_importances is not None:
             return inverse_neighbourhood, inverse_neighbourhood_importances
         else:
             return inverse_neighbourhood, None
 
     def predict(self, X, y=None):
+        """ Predicts the outcome with an explainable model previously fitted
+
+        :param X:
+        :param y:
+        :return:
+        """
         if isinstance(X, pd.DataFrame):
             pass
         elif isinstance(X, np.ndarray):
             X = pd.DataFrame(X, columns=self.attributes_names)
         else:
             raise ValueError("Only 2D arrrays are allowed as an input")
 
@@ -432,15 +694,20 @@
                           index=X.index)  # This is not used, but Data resered last
 
         X = pd.concat((X, y), axis=1)
         XData = Data.parse_dataframe(X, 'lux')
         return [int(f.get_name()) for f in self.uid3.predict(XData.get_instances())]
 
     def justify(self, X, to_dict=False, reduce=True):
-        """Traverse down the path for given x."""
+        """Traverse down the path for given x.
+        :param X:
+        :param to_dict:
+        :param reduce:
+        :return:
+        """
         if isinstance(X, pd.DataFrame):
             pass
         elif isinstance(X, np.ndarray):
             X = pd.DataFrame(X, columns=self.attributes_names)
         else:
             raise ValueError("Only 2D arrrays are allowed as an input")
 
@@ -451,28 +718,46 @@
 
         if to_dict:
             return [self.uid3.tree.justification_tree(i).to_dict(reduce=reduce) for i in XData.get_instances()]
         else:
             return [self.uid3.tree.justification_tree(i).to_pseudocode(reduce=reduce) for i in XData.get_instances()]
 
     def __get_covered(self, rule, dataset, features, categorical=None):
+        """ Returns covered instances from a given dataset and a rule
+
+        :param rule:
+        :param dataset:
+        :param features:
+        :param categorical:
+        :return:
+        """
         if categorical is None:
             categorical = [False] * len(features)
         query = []
         if rule == {}:
             return 0, 0
         for i, v in rule.items():
             op = '' if dict(zip(features, categorical))[i] == False else '=='
             query.append(f'{i}{op}' + f'and {i}{op}'.join(v))
 
         covered = dataset.query(' and '.join(query))
         return covered
 
     def counterfactual(self, instance_to_explain, background, counterfactual_representative='medoid', reduce=True,
                        topn=None, n_jobs=None):
+        """ Generates a counterfactual for a given instance and background data
+
+        :param instance_to_explain:
+        :param background:
+        :param counterfactual_representative:
+        :param reduce:
+        :param topn:
+        :param n_jobs:
+        :return:
+        """
         not_class = np.argmax(self.predict_proba(instance_to_explain))
         rules = self.uid3.tree.to_dict(reduce=reduce)
         bbox_predictions = np.argmax(self.predict_proba(background), axis=1)
         lux_predictions = self.predict(background)
         background = background[(bbox_predictions == lux_predictions)]
         # filter out rules with class same as not_class
         counterfactual_rules = []
@@ -518,123 +803,46 @@
         # find closest representative to the instance_to_explain and return as counterfactual, along with rules
         counterfactual_rules = sorted(counterfactual_rules, key=lambda d: d['distance'])
         if topn is None:
             return counterfactual_rules
         else:
             return counterfactual_rules[:topn]
 
-    def __getshap(self, X_train_sample):
-        # calculate shap values
-        try:
-            explainer = shap.Explainer(self.classifier, X_train_sample)
-            if hasattr(explainer, "shap_values"):
-                shap_values = explainer.shap_values(X_train_sample, check_additivity=False)
-            else:
-                shap_values = explainer(X_train_sample).values
-                shap_values = [sv for sv in np.moveaxis(shap_values, 2, 0)]
-            if hasattr(explainer, "expected_value"):
-                expected_values = explainer.expected_value
-            else:
-                expected_values = [np.mean(v) for v in shap_values]
-        except TypeError:
-            explainer = shap.Explainer(self.predict_proba, X_train_sample)
-            shap_values = explainer(X_train_sample).values
-            shap_values = [sv for sv in np.moveaxis(shap_values, 2, 0)]
-            expected_values = [np.mean(v) for v in shap_values]
-
-        if type(shap_values) is not list:
-            shap_values = [-shap_values, shap_values]
-            expected_values = [np.mean(v) for v in shap_values]
-
-        return shap_values, expected_values
-
-    def __importance_sampler(self, X_train_sample, instance_to_explain, num=10):
-        shap_values, _ = self.__getshap(X_train_sample)
-        abs_shap = np.array([abs(sv).mean(1) for sv in shap_values])
-        indexer = self.classifier.predict(X_train_sample)
-        shapclass = []
-
-        for i in range(0, len(X_train_sample)):
-            # we move sample towards the expected value, which should be decision boundary in balanced, binary case
-            best_index = indexer[i]
-            shapclass.append([shap_values[best_index][i, :]])
-        shapclass = np.concatenate(shapclass)
-        shapcols = [c + '_shap' for c in X_train_sample.columns]
-        cols = [c for c in X_train_sample.columns]
-
-        shapdf = pd.DataFrame(shapclass, columns=shapcols)
-
-        fulldf = pd.concat([X_train_sample.reset_index(drop=True), shapdf.reset_index(drop=True)], axis=1)
-        fulldf.index = X_train_sample.index
-        class_of_i2e = self.classifier.predict(instance_to_explain.reshape(1, -1))
-        predictions = self.classifier.predict(fulldf[cols])
-        # fulldf=fulldf[predictions==class_of_i2e]
-
-        gradsf = {}
-        gradst = []
-
-        for cl in np.unique(indexer):
-            gradcl = []
-            gradstcl = []
-            for dim in range(0, X_train_sample.shape[1]):
-                mask = indexer == cl
-                xs = X_train_sample.iloc[mask, dim]
-                ys = shapclass[mask, dim]
-                # plt.plot(xs,ys)
-                # plt.show()
-                grads = np.gradient(ys, xs)
-                gradstcl.append(grads)
-                svrr = LinearRegression()  # SVR()
-                svrr.fit(xs.values.reshape(-1, 1), ys)
-
-                F = lambda x, svr=svrr: svr.predict(x.reshape(1, -1))
-                gradient = nd.Gradient(F)
-
-                gradcl.append(gradient)
-            gradsf[cl] = gradcl
-            gradst.append(gradstcl)
-
-        alpha = np.ones(len(cols)) * (shapclass.max() - shapclass.min())
-
-        def perturb(x, num, alpha, gradients, cols, shapcols):
-            newx = []
-            last = x[cols].values
-            newx.append(last)
-            cl = self.classifier.predict(last.reshape(1, -1))[0]
-
-            grad = np.array([g(last[i]) for i, g in enumerate(gradients[cl])])
-            for _ in range(0, num):
-                last = last - alpha * grad
-                if cl != self.classifier.predict(last.reshape(1, -1))[0]:
-                    break
-                newx.append(last)
-            return np.array(newx)
-
-        if fulldf.shape[0] > 0:
-            upsamples = np.concatenate(
-                fulldf.sample(int(self.min_generate_samples*len(fulldf))).apply(perturb, args=(num, alpha, gradsf, cols, shapcols),
-                                                            axis=1).values)
-            upsamples = upsamples[np.random.choice(upsamples.shape[0], max(len(fulldf),upsamples.shape[0]), replace=False), :]
-        else:
-            upsamples = fulldf
-
-        return pd.concat((pd.DataFrame(upsamples, columns=X_train_sample.columns), X_train_sample))
+    def visualize(self, data, target_column_name='class',instance2explain=None, counterfactual=None, filename='tree.dot'):
+        cfdf = pd.DataFrame(counterfactual['counterfactual']).T
+        cfdf[target_column_name] = np.argmax(self.predict_proba(cfdf.values.reshape(1, -1))[0])
+        i2edf = pd.DataFrame(instance2explain, columns=self.attributes_names)
+        i2edf[target_column_name] = np.argmax(self.predict_proba(i2edf.values.reshape(1, -1))[0])
+        self.uid3.tree.save_dot(filename, fmt='.2f', visual=True, background_data=data, instance2explain=i2edf,
+                                counterfactual=cfdf)
 
     def to_HMR(self):
+        """ Exports to HMR format that can be executed by the HeaRTDroid rule-engine
+
+        :return:
+        """
         return self.tree.to_HMR()
 
     @staticmethod
     def generate_uarff(X, y, class_names, X_importances=None, categorical=None):
         """ Generates uncertain ARFF file
-        Arguments:
-            X : DataFrame containing dataset for training
-            y : target values returned by predict_proba function
-            class_names : names for the classess to be used in uID3
-            X_confidence : confidence for each reading obtained. This matrix should be normalized to the range [0;1].
-        
+
+            :param X:
+                DataFrame containing dataset for training
+            :param y:
+                target values returned by predict_proba function
+            :param class_names:
+                names for the classes to be used in uID3
+            :param X_importances:
+                confidence for each reading obtained. This matrix should be normalized to the range [0;1].
+            :param categorical:
+                array indicating which parameters should be treated as categorical
+            :return:
+                String representing the ARFF file
+
         """
         if X_importances is not None:
             if not isinstance(X_importances, pd.DataFrame):
                 raise ValueError('Reading confidence matrix has to be DataFrame.')
             if X.shape != X_importances.shape:
                 raise ValueError("Confidence for readings have to be exaclty the size of X.")
         if categorical is None:
```

### Comparing `lux-explainer-1.0.1/src/lux/pyuid3/att_stats.py` & `lux_explainer-1.2.0/src/lux/pyuid3/att_stats.py`

 * *Files identical despite different names*

### Comparing `lux-explainer-1.0.1/src/lux/pyuid3/attribute.py` & `lux_explainer-1.2.0/src/lux/pyuid3/attribute.py`

 * *Files identical despite different names*

### Comparing `lux-explainer-1.0.1/src/lux/pyuid3/data.py` & `lux_explainer-1.2.0/src/lux/pyuid3/data.py`

 * *Files identical despite different names*

### Comparing `lux-explainer-1.0.1/src/lux/pyuid3/data_scrambler.py` & `lux_explainer-1.2.0/src/lux/pyuid3/data_scrambler.py`

 * *Files identical despite different names*

### Comparing `lux-explainer-1.0.1/src/lux/pyuid3/entropy_evaluator.py` & `lux_explainer-1.2.0/src/lux/pyuid3/entropy_evaluator.py`

 * *Files identical despite different names*

### Comparing `lux-explainer-1.0.1/src/lux/pyuid3/instance.py` & `lux_explainer-1.2.0/src/lux/pyuid3/instance.py`

 * *Files identical despite different names*

### Comparing `lux-explainer-1.0.1/src/lux/pyuid3/reading.py` & `lux_explainer-1.2.0/src/lux/pyuid3/reading.py`

 * *Files identical despite different names*

### Comparing `lux-explainer-1.0.1/src/lux/pyuid3/tree.py` & `lux_explainer-1.2.0/src/lux/pyuid3/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,19 +155,24 @@
             #conditions
             for att in atts:
                 if att.get_name() == self.get_class_attribute().get_name():
                     continue
 
                 value = Value("any", 1.0)
 
+                found = False
                 for c in rule:
                     if c.att_name == att.get_name():
+                        found=True
                         value = c.value
                         result +=  f"{att.get_name()} {value.get_name().replace('>=',' gte ').replace('<',' lt ')}, "
 
+                if not found:
+                    result += f"{att.get_name()} eq any, "
+
             result = f"{result.strip()[:-1]}] ==> ["
 
             #decision
 
             confidence = 1
             for c in rule:
                 confidence *= c.value.get_confidence()
@@ -439,18 +444,22 @@
             os.makedirs(path+'/imgs/')
         if parent:
             result = ""
             col = "red" if parent.is_leaf() else "black"
             if parent.is_leaf():
                 fig,ax=plt.subplots(figsize=(3,3))
                 if instance2explain is not None:
+                    instance2explain[target_column] = instance2explain[target_column].astype(str)
                     background_data = pd.concat((instance2explain,background_data))
                 if counterfactual is not None:
+                    counterfactual[target_column] = counterfactual[target_column].astype(str)
                     background_data = pd.concat((counterfactual,background_data))
+                background_data[target_column] = background_data[target_column].astype(str)
                 stats = background_data[[target_column]].value_counts().to_frame('samples').sort_index().reset_index()
+
                 sns.barplot(data = stats,
                             x=target_column,y='samples', alpha=0.7,palette=palette,ax=ax)
 
                 if instance2explain is not None:
                     pos = stats[stats[target_column]==instance2explain[target_column].values[0]].index[0]
                     ax.plot(pos,1, 'or', markersize=8)
                 if counterfactual is not None:
```

### Comparing `lux-explainer-1.0.1/src/lux/pyuid3/tree_edge.py` & `lux_explainer-1.2.0/src/lux/pyuid3/tree_edge.py`

 * *Files identical despite different names*

### Comparing `lux-explainer-1.0.1/src/lux/pyuid3/tree_evaluator.py` & `lux_explainer-1.2.0/src/lux/pyuid3/tree_evaluator.py`

 * *Files identical despite different names*

### Comparing `lux-explainer-1.0.1/src/lux/pyuid3/tree_node.py` & `lux_explainer-1.2.0/src/lux/pyuid3/tree_node.py`

 * *Files identical despite different names*

### Comparing `lux-explainer-1.0.1/src/lux/pyuid3/uid3.py` & `lux_explainer-1.2.0/src/lux/pyuid3/uid3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: src/uId3.ipynb (unless otherwise specified).
 
 __all__ = ['UId3']
 
 # Cell
-from graphviz import Source
 from sklearn.base import BaseEstimator
 import numpy as np
 import pandas as pd
 from sklearn.tree import DecisionTreeClassifier
 
 from .attribute import Attribute
 from .data import Data
 from .entropy_evaluator import EntropyEvaluator, UncertainEntropyEvaluator
 from .tree import Tree
 from .tree_node import TreeNode
 from .tree_edge import TreeEdge
 from .tree_evaluator import TreeEvaluator
 from .value import Value
-from .reading import Reading
-from .instance import Instance
 from .utils import StandardRescaler
 from multiprocessing import cpu_count,Pool
-import math
 import shap
 from sklearn.svm import LinearSVC
 from sklearn.preprocessing import StandardScaler
 
 # Cell
 class UId3(BaseEstimator):
     
     PARALLEL_ENTRY_FACTOR = 1000
 
-    def __init__(self, max_depth=2, node_size_limit = 1, grow_confidence_threshold = 0, min_impurity_decrease=0):
+    def __init__(self, max_depth=None, node_size_limit = 1, grow_confidence_threshold = 0, min_impurity_decrease=0):
         self.TREE_DEPTH_LIMIT= max_depth
         self.NODE_SIZE_LIMIT = node_size_limit
         self.GROW_CONFIDENCE_THRESHOLD = grow_confidence_threshold
         self.tree = None
         self.node_size_limit = node_size_limit
         self.min_impurity_decrease=min_impurity_decrease
         
@@ -97,28 +93,28 @@
             
             if type(shap_values) is not list:
                 shap_values = [-shap_values, shap_values]
                 expected_values=[np.mean(v) for v in shap_values]
 
 
             #find max and rescale:
-            #maxshap = max([np.max(np.abs(sv)) for sv in shap_values]) #ADD
-            #shap_values = [sv/maxshap for sv in shap_values] #ADD
+            maxshap = max([np.max(np.abs(sv)) for sv in shap_values]) #ADD
+            shap_values = [sv/maxshap for sv in shap_values] #ADD
             
             shap_dict={}
             expected_dict={}
             for i,v in enumerate(shap_values):
                 shap_dict[str(i)] = pd.DataFrame(v, columns = datadf.columns[:-1])
                 expected_dict[str(i)] = expected_values[i] #/maxshap #ADD
                 
             data = data.set_importances(pd.concat(shap_dict,axis=1), expected_values = expected_dict)
         
         if len(data.get_instances()) < self.NODE_SIZE_LIMIT:
             return None
-        if depth > self.TREE_DEPTH_LIMIT:
+        if self.TREE_DEPTH_LIMIT is not None and depth > self.TREE_DEPTH_LIMIT:
             return None
         entropy = entropyEvaluator.calculate_entropy(data)
 
         data.update_attribute_domains()
 
         # of the set is heterogeneous or no attributes to split, just class -- return
         # leaf
@@ -435,21 +431,21 @@
     @staticmethod
     def calculate_gains_numeric(stat_for_lt_value, stat_for_gte_value, conf_for_value, avg_abs_importance,  subdata_less_than,subdata_greater_equal, attribute, entropyEvaluator, globalEntropy, beta,shap):
         if shap:
             pure_single_temp_gain = (globalEntropy - (stat_for_lt_value*entropyEvaluator.calculate_entropy(subdata_less_than)+
                                                                            (stat_for_gte_value)*entropyEvaluator.calculate_entropy(subdata_greater_equal) ))
 
 
-            pure_single_temp_gain_shap = avg_abs_importance
+            pure_single_temp_gain_shap = avg_abs_importance*globalEntropy #ADD
 
             if pure_single_temp_gain*pure_single_temp_gain_shap == 0:
                 #to prevent from 0-division
                 single_temp_gain=0
             else:
-                single_temp_gain =pure_single_temp_gain_shap*pure_single_temp_gain#((1+beta**2)*pure_single_temp_gain_shap*pure_single_temp_gain)/((beta**2*pure_single_temp_gain_shap)+pure_single_temp_gain)*conf_for_value
+                single_temp_gain =(beta*pure_single_temp_gain_shap*pure_single_temp_gain)/(1+beta)#((1+beta**2)*pure_single_temp_gain_shap*pure_single_temp_gain)/((beta**2*pure_single_temp_gain_shap)+pure_single_temp_gain)*conf_for_value
         else:
             pure_single_temp_gain = (globalEntropy - (stat_for_lt_value*entropyEvaluator.calculate_entropy(subdata_less_than)+
                                                                                    (stat_for_gte_value)*entropyEvaluator.calculate_entropy(subdata_greater_equal) ))
             single_temp_gain = pure_single_temp_gain*conf_for_value
     
         return single_temp_gain, pure_single_temp_gain
```

### Comparing `lux-explainer-1.0.1/src/lux/pyuid3/utils.py` & `lux_explainer-1.2.0/src/lux/pyuid3/utils.py`

 * *Files identical despite different names*

### Comparing `lux-explainer-1.0.1/src/lux/pyuid3/value.py` & `lux_explainer-1.2.0/src/lux/pyuid3/value.py`

 * *Files identical despite different names*

### Comparing `lux-explainer-1.0.1/src/lux_explainer.egg-info/PKG-INFO` & `lux_explainer-1.2.0/src/lux_explainer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lux-explainer
-Version: 1.0.1
+Version: 1.2.0
 Summary: Universal Local Rule-based Explainer
-Author-email: LUX <szymon.bobek@gmail.com>
+Author-email: Szymon Bobek <szymon.bobek@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 sbobek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -22,14 +22,16 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/sbobek/lux
+Project-URL: Documentation, https://lux-explainer.readthedocs.org
+Project-URL: Issues, https://github.com/sbobek/lux/issues
 Keywords: xai,explainability,model-agnostic,rule-based
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -45,15 +47,15 @@
 Requires-Dist: anchor-exp>=0.0.2.0
 Requires-Dist: imbalanced-learn>=0.9.1
 Requires-Dist: gower>=0.1.2
 Requires-Dist: numdifftools>=0.9.41
 
 # LUX (Local Universal Rule-based Explainer)
 ## Main features
-  <img align="right"  src="./pix/lux-logo.png" width="200">
+  <img align="right"  src="https://raw.githubusercontent.com/sbobek/lux/main/pix/lux-logo.png" width="200">
   
   * Model-agnostic, rule-based and visual local explanations of black-box ML models
   * Integrated counterfactual explanations
   * Rule-based explanations (that are executable at the same time)
   * Oblique trees backbone, which allows to explain more reliable linear decision boundaries
   * Integration with [Shapley values](https://shap.readthedocs.io/en/latest/) or [Lime](https://github.com/marcotcr/lime) importances (or any other explainer that produces importances) that help in generating high quality rules
   
@@ -78,26 +80,26 @@
 
 ```
 pip install lux-explainer
 ```
 If you want to use LUX with [JupyterLab](https://jupyter.org/) install it and run:
 
 ```
-pip isntall jupyterlab
+pip installta jupyterlab
 jupyter lab
 ```
 
 **Caution**: If you want to use LUX with categorical data, it is advised to use [multiprocessing gower distance](https://github.com/sbobek/gower/tree/add-multiprocessing) package (due to high computational complexity of the problem). 
 
 ## Usage
 
   * For complete usage see [lux_usage_example.ipynb](https://raw.githubusercontent.com/sbobek/lux/main/examples/lux_usage_example.ipynb)
   * Fos usage example with Shap integration see [lux_usage_example_shap.ipynb](https://raw.githubusercontent.com/sbobek/lux/main/examples/lux_usage_example_shap.ipynb)
 
-### Simple exmaple on Iris dataset
+### Simple example on Iris dataset
 
 ``` python
 from lux.lux import LUX
 from sklearn import datasets
 from sklearn.model_selection import train_test_split
 from sklearn import svm
 import numpy as np
@@ -131,15 +133,15 @@
 ```
 
 The above code should give you the answer as follows:
 ```
 ['IF petal_length >= 5.15 THEN class = 2 # 0.9833409059468439\n']
 ```
 
-Alternatively one can get counterfactual explanation for agiven instance by calling:
+Alternatively one can get counterfactual explanation for a given instance by calling:
 
 ``` python
 cf = lux.counterfactual(np.array(iris_instance), train[features], counterfactual_representative='nearest', topn=1)[0]
 print(f"Counterfactual for {iris_instance} to change from class {lux.predict(np.array(iris_instance))[0]} to class {cf['prediction']}: \n{cf['counterfactual']}")
 ```
 The result from the above query should look as follows:
 
@@ -148,15 +150,15 @@
 sepal_length    6.9
 sepal_width     3.1
 petal_length    5.1
 petal_width     2.3
 ```
 
 ### Rule-based model for local uncertain explanations
-You can obtain a whole rule-based model for the local uncertian explanation that was generated by LUX for given instance by running following code
+You can obtain a whole rule-based model for the local uncertain explanation that was generated by LUX for given instance by running following code
 
 ``` python
 #have a look at the entire rule-based model that can be executed with https:://heartdroid.re
 print(lux.to_HMR())
 ```
 
 This will generate model which can later be executed by [HeaRTDroid](https://heartdroid.re)
@@ -201,15 +203,15 @@
 from IPython.display import SVG, Image
 lux.uid3.tree.save_dot('tree.dot',fmt='.2f',visual=True, background_data=train)
 gvz=graphviz.Source.from_file('tree.dot')
 !dot -Tpng tree.dot > tree.png
 Image('tree.png')
 ```
 
-The code should yeld something like that (depending on the instance that was selected):
+The code should yield something like that (depending on the instance that was selected):
 
 ![](https://raw.githubusercontent.com/sbobek/lux/main/pix/utree.png)
 
 # Cite this work
 
 ```
 @misc{bobek2023local,
```

### Comparing `lux-explainer-1.0.1/src/lux_explainer.egg-info/SOURCES.txt` & `lux_explainer-1.2.0/src/lux_explainer.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 src/lux/UncertainSMOTE.py
 src/lux/__init__.py
 src/lux/lux.py
+src/lux/metrics.py
+src/lux/samplers.py
 src/lux/pyuid3/__init__.py
 src/lux/pyuid3/att_stats.py
 src/lux/pyuid3/attribute.py
 src/lux/pyuid3/data.py
 src/lux/pyuid3/data_scrambler.py
 src/lux/pyuid3/entropy_evaluator.py
 src/lux/pyuid3/instance.py
```

