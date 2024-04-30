# Comparing `tmp/classification_lib-0.1.0.tar.gz` & `tmp/classification_lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classification_lib-0.1.0.tar", last modified: Tue Apr 16 14:32:51 2024, max compression
+gzip compressed data, was "classification_lib-0.2.0.tar", last modified: Tue Apr 30 14:38:24 2024, max compression
```

## Comparing `classification_lib-0.1.0.tar` & `classification_lib-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 14:32:51.598731 classification_lib-0.1.0/
--rw-rw-rw-   0        0        0     3070 2024-04-16 14:32:51.594741 classification_lib-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 14:32:51.554004 classification_lib-0.1.0/classification_lib/
--rw-rw-rw-   0        0        0       44 2024-04-16 14:01:48.000000 classification_lib-0.1.0/classification_lib/__init__.py
--rw-rw-rw-   0        0        0     2336 2024-04-11 14:44:44.000000 classification_lib-0.1.0/classification_lib/plots.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:32:51.592747 classification_lib-0.1.0/classification_lib.egg-info/
--rw-rw-rw-   0        0        0     3070 2024-04-16 14:32:51.000000 classification_lib-0.1.0/classification_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-04-16 14:32:51.000000 classification_lib-0.1.0/classification_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 14:32:51.000000 classification_lib-0.1.0/classification_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-16 14:32:51.000000 classification_lib-0.1.0/classification_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-16 14:32:51.000000 classification_lib-0.1.0/classification_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 14:32:51.598731 classification_lib-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1452 2024-04-16 14:01:48.000000 classification_lib-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:38:24.307646 classification_lib-0.2.0/
+-rw-rw-rw-   0        0        0     2993 2024-04-30 14:38:24.307646 classification_lib-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 14:38:24.292025 classification_lib-0.2.0/classification_lib/
+-rw-rw-rw-   0        0        0       44 2024-04-16 14:01:48.000000 classification_lib-0.2.0/classification_lib/__init__.py
+-rw-rw-rw-   0        0        0     2336 2024-04-11 14:44:44.000000 classification_lib-0.2.0/classification_lib/plots.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:38:24.307646 classification_lib-0.2.0/classification_lib.egg-info/
+-rw-rw-rw-   0        0        0     2993 2024-04-30 14:38:24.000000 classification_lib-0.2.0/classification_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-04-30 14:38:24.000000 classification_lib-0.2.0/classification_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 14:38:24.000000 classification_lib-0.2.0/classification_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-30 14:38:24.000000 classification_lib-0.2.0/classification_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-30 14:38:24.000000 classification_lib-0.2.0/classification_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 14:38:24.307646 classification_lib-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1438 2024-04-30 14:37:45.000000 classification_lib-0.2.0/setup.py
```

### Comparing `classification_lib-0.1.0/PKG-INFO` & `classification_lib-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: classification_lib
-Version: 0.1.0
-Summary: Module for libraries containing various utility functions for classification tasks
+Version: 0.2.0
+Summary: Module containing various utility functions for classification tasks
 Home-page: 
 Author: Felix Cobby Otoo
 Author-email: felixotoo75@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,76 +13,63 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: matplotlib
 
-# Classification_Lib
+# classification_lib
 A custom module that grants access to libraries with utility functions for performing classification tasks such as:
 
 * Creating precision-recall curves for multiple classifiers for easier comparisons.
 
 * Creating ROC curves for multiple classifiers for easier comparisons
 
 ### Installation
     pip install classification_lib
 
 ### Get Started
 How to plot different pr-curve(s) for classifier(s) using the __*plot_pr_curve*__ of this library:
 
 ```Python
-
 from classification_lib import Plots
 import numpy as np
 
-
-
 # Instantiating the precisions and recalls for two different classifiers
-
 classifier1_precisions = np.sort(0.791 + 0.168 * np.random.randn(794))
 classifier2_precisions = np.sort(0.5 + 0.142 * np.random.randn(794))
 classifier1_recalls = sorted(0.70 + 0.299 * np.random.randn(794), reverse=True)
 classifier2_recalls = sorted(0.3 + 0.5 * np.random.randn(794), reverse=True)
 classifier1_name = "Classifier 1"
 classifier2_name = "Classifier 2"
 classifiers = [(classifier1_name, classifier1_precisions, classifier1_recalls),
                (classifier2_name, classifier2_precisions, classifier2_recalls)]
 
 # Instantiate a Plot object
 plot = Plots(classifiers)
 
 # Call the pr_curve_plot method
 result = plot.plot_pr_curve()
-
 ```
-
 How to plot different pr-curve(s) for classifier(s) using the __*plot_roc_curve*__ of this library:
-
 ```Python
-
 import numpy as np
 from classification_lib import Plots
 
 classifier1_false_positive_rate = sorted(0.29 + 0.248 * np.random.randn(219))
 classifier2_false_positive_rate = sorted(0.7 + 0.4 * np.random.randn(219))
 classifier1_true_positive_rate= sorted(0.788 + 0.2 * np.random.randn(219))
 classifier2_true_positive_rate = sorted(0.6 + 0.3 * np.random.randn(219))
-
 classifier1_name = "Classifier 1"
 classifier2_name = "Classifier 2"
-
 classifiers = [(classifier1_name, classifier1_false_positive_rate, classifier1_true_positive_rate),
                (classifier2_name, classifier2_false_positive_rate, classifier2_true_positive_rate)]
 
-
 # Instantiate a Plot object
 plot = Plots(classifiers)
 
 # Call the pr_curve_plot method
 result = plot.plot_roc_curve()
-
 ```
```

### Comparing `classification_lib-0.1.0/classification_lib/plots.py` & `classification_lib-0.2.0/classification_lib/plots.py`

 * *Files identical despite different names*

### Comparing `classification_lib-0.1.0/classification_lib.egg-info/PKG-INFO` & `classification_lib-0.2.0/classification_lib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: classification_lib
-Version: 0.1.0
-Summary: Module for libraries containing various utility functions for classification tasks
+Name: classification-lib
+Version: 0.2.0
+Summary: Module containing various utility functions for classification tasks
 Home-page: 
 Author: Felix Cobby Otoo
 Author-email: felixotoo75@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,76 +13,63 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: matplotlib
 
-# Classification_Lib
+# classification_lib
 A custom module that grants access to libraries with utility functions for performing classification tasks such as:
 
 * Creating precision-recall curves for multiple classifiers for easier comparisons.
 
 * Creating ROC curves for multiple classifiers for easier comparisons
 
 ### Installation
     pip install classification_lib
 
 ### Get Started
 How to plot different pr-curve(s) for classifier(s) using the __*plot_pr_curve*__ of this library:
 
 ```Python
-
 from classification_lib import Plots
 import numpy as np
 
-
-
 # Instantiating the precisions and recalls for two different classifiers
-
 classifier1_precisions = np.sort(0.791 + 0.168 * np.random.randn(794))
 classifier2_precisions = np.sort(0.5 + 0.142 * np.random.randn(794))
 classifier1_recalls = sorted(0.70 + 0.299 * np.random.randn(794), reverse=True)
 classifier2_recalls = sorted(0.3 + 0.5 * np.random.randn(794), reverse=True)
 classifier1_name = "Classifier 1"
 classifier2_name = "Classifier 2"
 classifiers = [(classifier1_name, classifier1_precisions, classifier1_recalls),
                (classifier2_name, classifier2_precisions, classifier2_recalls)]
 
 # Instantiate a Plot object
 plot = Plots(classifiers)
 
 # Call the pr_curve_plot method
 result = plot.plot_pr_curve()
-
 ```
-
 How to plot different pr-curve(s) for classifier(s) using the __*plot_roc_curve*__ of this library:
-
 ```Python
-
 import numpy as np
 from classification_lib import Plots
 
 classifier1_false_positive_rate = sorted(0.29 + 0.248 * np.random.randn(219))
 classifier2_false_positive_rate = sorted(0.7 + 0.4 * np.random.randn(219))
 classifier1_true_positive_rate= sorted(0.788 + 0.2 * np.random.randn(219))
 classifier2_true_positive_rate = sorted(0.6 + 0.3 * np.random.randn(219))
-
 classifier1_name = "Classifier 1"
 classifier2_name = "Classifier 2"
-
 classifiers = [(classifier1_name, classifier1_false_positive_rate, classifier1_true_positive_rate),
                (classifier2_name, classifier2_false_positive_rate, classifier2_true_positive_rate)]
 
-
 # Instantiate a Plot object
 plot = Plots(classifiers)
 
 # Call the pr_curve_plot method
 result = plot.plot_roc_curve()
-
 ```
```

### Comparing `classification_lib-0.1.0/setup.py` & `classification_lib-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # Get the long description from the README file
 with open(path.join(HERE, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="classification_lib",
-    version="0.1.0",
-    description="Module for libraries containing various utility functions for classification tasks",
+    version="0.2.0",
+    description="Module containing various utility functions for classification tasks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=URL,
     author="Felix Cobby Otoo",
     author_email="felixotoo75@gmail.com",
     license="MIT",
     classifiers=[
```

