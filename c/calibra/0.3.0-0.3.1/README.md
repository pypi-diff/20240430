# Comparing `tmp/calibra-0.3.0.tar.gz` & `tmp/calibra-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calibra-0.3.0.tar", last modified: Tue Apr 23 16:53:15 2024, max compression
+gzip compressed data, was "calibra-0.3.1.tar", last modified: Tue Apr 30 17:09:31 2024, max compression
```

## Comparing `calibra-0.3.0.tar` & `calibra-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 16:53:14.993701 calibra-0.3.0/
--rw-rw-rw-   0        0        0      173 2024-01-24 19:10:57.000000 calibra-0.3.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3648 2024-01-24 19:10:57.000000 calibra-0.3.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2024-01-24 19:10:57.000000 calibra-0.3.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1092 2024-01-24 19:10:57.000000 calibra-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      273 2024-01-24 19:10:57.000000 calibra-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1759 2024-04-23 16:53:14.993701 calibra-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      919 2024-01-24 19:10:57.000000 calibra-0.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-23 16:53:14.912011 calibra-0.3.0/calibra/
--rw-rw-rw-   0        0        0      134 2024-01-24 19:10:57.000000 calibra-0.3.0/calibra/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-24 19:37:39.000000 calibra-0.3.0/calibra/calibrators.py
--rw-rw-rw-   0        0        0     4665 2024-04-23 16:43:18.000000 calibra-0.3.0/calibra/errors.py
--rw-rw-rw-   0        0        0    24536 2024-04-23 16:43:15.000000 calibra-0.3.0/calibra/plotting.py
--rw-rw-rw-   0        0        0    15779 2024-04-23 16:36:15.000000 calibra-0.3.0/calibra/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:53:14.951023 calibra-0.3.0/calibra.egg-info/
--rw-rw-rw-   0        0        0     1759 2024-04-23 16:53:14.000000 calibra-0.3.0/calibra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      666 2024-04-23 16:53:14.000000 calibra-0.3.0/calibra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 16:53:14.000000 calibra-0.3.0/calibra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-24 19:23:17.000000 calibra-0.3.0/calibra.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2024-04-23 16:53:14.000000 calibra-0.3.0/calibra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 16:53:14.000000 calibra-0.3.0/calibra.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-23 16:53:14.974921 calibra-0.3.0/docs/
--rw-rw-rw-   0        0        0      628 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/authors.rst
--rw-rw-rw-   0        0        0     4937 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/history.rst
--rw-rw-rw-   0        0        0      324 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/index.rst
--rw-rw-rw-   0        0        0     1181 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/installation.rst
--rwxrwxrwx   0        0        0      805 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/readme.rst
--rw-rw-rw-   0        0        0       76 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/usage.rst
--rw-rw-rw-   0        0        0      503 2024-04-23 16:53:15.001436 calibra-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1342 2024-04-23 16:52:11.000000 calibra-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:53:14.987696 calibra-0.3.0/tests/
--rw-rw-rw-   0        0        0       38 2024-01-24 19:10:57.000000 calibra-0.3.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:53:14.990698 calibra-0.3.0/tests/baseline/
--rw-rw-rw-   0        0        0    31261 2024-04-23 16:33:55.000000 calibra-0.3.0/tests/baseline/test_plot.png
--rw-rw-rw-   0        0        0    34731 2024-04-23 15:20:59.000000 calibra-0.3.0/tests/conftest.py
--rw-rw-rw-   0        0        0     5252 2024-03-22 19:03:42.000000 calibra-0.3.0/tests/test_errors.py
--rw-rw-rw-   0        0        0    24645 2024-04-23 16:33:44.000000 calibra-0.3.0/tests/test_plotting.py
--rw-rw-rw-   0        0        0    17088 2024-03-22 20:26:09.000000 calibra-0.3.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 17:09:31.754632 calibra-0.3.1/
+-rw-rw-rw-   0        0        0      173 2024-01-24 19:10:57.000000 calibra-0.3.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3648 2024-01-24 19:10:57.000000 calibra-0.3.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2024-01-24 19:10:57.000000 calibra-0.3.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1092 2024-01-24 19:10:57.000000 calibra-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      273 2024-01-24 19:10:57.000000 calibra-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1759 2024-04-30 17:09:31.754632 calibra-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      919 2024-01-24 19:10:57.000000 calibra-0.3.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-30 17:09:31.596124 calibra-0.3.1/calibra/
+-rw-rw-rw-   0        0        0      134 2024-04-30 17:07:57.000000 calibra-0.3.1/calibra/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-01-24 19:37:39.000000 calibra-0.3.1/calibra/calibrators.py
+-rw-rw-rw-   0        0        0     4428 2024-04-30 16:50:01.000000 calibra-0.3.1/calibra/errors.py
+-rw-rw-rw-   0        0        0    25056 2024-04-30 17:04:00.000000 calibra-0.3.1/calibra/plotting.py
+-rw-rw-rw-   0        0        0    17091 2024-04-29 22:02:38.000000 calibra-0.3.1/calibra/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 17:09:31.636976 calibra-0.3.1/calibra.egg-info/
+-rw-rw-rw-   0        0        0     1759 2024-04-30 17:09:31.000000 calibra-0.3.1/calibra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2024-04-30 17:09:31.000000 calibra-0.3.1/calibra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 17:09:31.000000 calibra-0.3.1/calibra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-01-24 19:23:17.000000 calibra-0.3.1/calibra.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2024-04-30 17:09:31.000000 calibra-0.3.1/calibra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-30 17:09:31.000000 calibra-0.3.1/calibra.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 17:09:31.734398 calibra-0.3.1/docs/
+-rw-rw-rw-   0        0        0      628 2024-01-24 19:10:57.000000 calibra-0.3.1/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2024-01-24 19:10:57.000000 calibra-0.3.1/docs/authors.rst
+-rw-rw-rw-   0        0        0     4937 2024-01-24 19:10:57.000000 calibra-0.3.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2024-01-24 19:10:57.000000 calibra-0.3.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-01-24 19:10:57.000000 calibra-0.3.1/docs/history.rst
+-rw-rw-rw-   0        0        0      324 2024-01-24 19:10:57.000000 calibra-0.3.1/docs/index.rst
+-rw-rw-rw-   0        0        0     1181 2024-01-24 19:10:57.000000 calibra-0.3.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      805 2024-01-24 19:10:57.000000 calibra-0.3.1/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2024-01-24 19:10:57.000000 calibra-0.3.1/docs/readme.rst
+-rw-rw-rw-   0        0        0       76 2024-01-24 19:10:57.000000 calibra-0.3.1/docs/usage.rst
+-rw-rw-rw-   0        0        0      503 2024-04-30 17:09:31.757632 calibra-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1342 2024-04-30 17:08:45.000000 calibra-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 17:09:31.747620 calibra-0.3.1/tests/
+-rw-rw-rw-   0        0        0       38 2024-01-24 19:10:57.000000 calibra-0.3.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 17:09:31.750619 calibra-0.3.1/tests/baseline/
+-rw-rw-rw-   0        0        0    31261 2024-04-23 16:33:55.000000 calibra-0.3.1/tests/baseline/test_plot.png
+-rw-rw-rw-   0        0        0    35240 2024-04-29 22:07:25.000000 calibra-0.3.1/tests/conftest.py
+-rw-rw-rw-   0        0        0     6099 2024-04-29 22:07:24.000000 calibra-0.3.1/tests/test_errors.py
+-rw-rw-rw-   0        0        0    25028 2024-04-29 22:07:25.000000 calibra-0.3.1/tests/test_plotting.py
+-rw-rw-rw-   0        0        0    18367 2024-04-29 22:07:24.000000 calibra-0.3.1/tests/test_utils.py
```

### Comparing `calibra-0.3.0/CONTRIBUTING.rst` & `calibra-0.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `calibra-0.3.0/LICENSE` & `calibra-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `calibra-0.3.0/PKG-INFO` & `calibra-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibra
-Version: 0.3.0
+Version: 0.3.1
 Summary: Toolkit for calibration of machine learning classifiers.
 Home-page: https://github.com/conorwalsh99/calibra
 Author: Conor Walsh
 Author-email: conorwalsh206@gmail.com
 License: MIT license
 Keywords: calibra
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `calibra-0.3.0/README.rst` & `calibra-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `calibra-0.3.0/calibra/errors.py` & `calibra-0.3.1/calibra/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,102 +1,105 @@
-import pandas as pd 
-import numpy as np 
-from typing import Union
+import numpy as np
+from typing import Union, Tuple
 
 from calibra.utils import bin_probabilities, _reshape_y_pred, _get_bin_weight
 
 
 def classwise_ece(
-        y_pred: np.ndarray, 
-        y_true: np.ndarray, 
-        num_bins: int = 20, 
-        method: str = 'width', 
-        return_classwise_errors: bool = False
-        ) -> Union[float, tuple]:
-    """ 
+    y_pred: np.ndarray,
+    y_true: np.ndarray,
+    num_bins: int = 20,
+    method: str = "width",
+    return_classwise_errors: bool = False,
+) -> Union[float, Tuple[float, np.ndarray]]:
+    """
     Calculate the class-wise Expected Calibration Error (ECE) of a set of predictions.
 
     Args:
-        y_pred (ndarray):
+        y_pred (np.ndarray):
             Array-like object of shape (num_samples, num_classes) where ij position is predicted probability of data point i belonging to class j.
             Alternatively may be of shape (num_samples,) for binary classification where i position is predicted probability of data point i belonging to class 1 (positive class).
-        y_true (ndarray):
-            This 1-D array of length num_samples contains the true label for each data point.        
+        y_true (np.ndarray):
+            This 1-D array of length num_samples contains the true label for each data point.
         num_bins (int):
             Number of bins the interval [0, 1] is divided into. Exact if method='width', approximate if method='frequency'.
         method (str):
             Method of splitting interval [0, 1] into bins. If set to 'width' divides the interval [0, 1] into num_bins bins of equal width.
-            If set to 'frequency' divides the interval [0, 1] into approximately num_bins bins, each containing approximately num_samples/num_bins data points. 
-            Defaults to 'width'.      
+            If set to 'frequency' divides the interval [0, 1] into approximately num_bins bins, each containing approximately num_samples/num_bins data points.
+            Defaults to 'width'.
         return_classwise_errors (bool):
-            If True returns a numpy array of shape (num_classes,) containing the contribution of each class to the class-wise expected calibration error. Defaults to False.
+            If True returns a numpy array of shape (num_classes,) containing the error for each class. Defaults to False.
 
-    Returns:    
+    Returns:
         float:
             Value of the class-wise expected calibration error. This is an element of [0,1].
-
         tuple:
             Tuple containing a float and a numpy array.
                 float:
                     Value of the class-wise expected calibration error. This is an element of [0,1].
                 np.ndarray:
-                    Numpy array of shape (num_classes) whose ith element represents the contribution of class i to the class-wise expected calibration error. 
+                    Numpy array of shape (num_classes) whose ith element represents the class i error.
     """
     y_pred = _reshape_y_pred(y_pred)
     num_samples, num_classes = y_pred.shape
 
-    bins = bin_probabilities(y_pred, y_true, num_bins, method)     
+    bins = bin_probabilities(y_pred, y_true, num_bins, method)
     classwise_errors = _get_classwise_errors(bins, num_bins, num_samples, num_classes)
     overall_error = classwise_errors.mean()
 
-    return (overall_error, classwise_errors) if return_classwise_errors else overall_error
+    return (
+        (overall_error, classwise_errors) if return_classwise_errors else overall_error
+    )
 
 
-def _get_classwise_errors(bins: dict, num_bins: int, num_samples: int, num_classes: int) -> np.ndarray:
+def _get_classwise_errors(
+    bins: dict, num_bins: int, num_samples: int, num_classes: int
+) -> np.ndarray:
     """
     Calculate the error for each class.
 
     Args:
         bins (dict):
-            Dictionary containing, for each class, each bin, itself containing the predicted probabilities and occurences of the given class.                    
+            Dictionary containing, for each class, each bin, itself containing the predicted probabilities and occurences of the given class.
         num_bins (int):
             Number of equal-width bins the interval [0, 1] is divided into.
         num_samples (int):
             Number of data points.
         num_classes (int):
             Number of classes.
 
     Returns:
         np.ndarray:
-            Numpy array of shape (num_classes) whose ith element represents the contribution of class i to the class-wise expected calibration error.                      
+            Numpy array of shape (num_classes) whose ith element represents the class i error.
     """
     errors = np.zeros(num_classes)
 
     for i in range(num_classes):
         for b in range(num_bins):
             bin_weight = _get_bin_weight(bins[i][b], num_samples)
-            if bin_weight > 0:      
+            if bin_weight > 0:
                 bin_deviation = _calculate_bin_deviation(bins[i][b])
                 weighted_bin_deviation = bin_weight * bin_deviation
-                errors[i] += weighted_bin_deviation 
-    
+                errors[i] += weighted_bin_deviation
+
     return errors
 
+
 def _calculate_bin_deviation(bin: dict) -> float:
     """
     Calculate the deviation between the expected rate of occurrence and the actual rate of occurrence, for a given bin.
 
     Args:
         bin (dict):
             Dictionary containing the predicted probabilities for a given class and the number of occurrences of that class, for a given bin.
 
     Returns:
-        float 
+        float
     """
-    probs, num_occurrences = bin['probs'], bin['num_occurrences']
+    probs, num_occurrences = bin["probs"], bin["num_occurrences"]
     num_trials = len(probs)
     expected_num_occurrences = sum(probs)
     actual_num_occurrences = num_occurrences
     expected_occurrence_rate = expected_num_occurrences / num_trials
     actual_occurrence_rate = actual_num_occurrences / num_trials
     deviation = abs(expected_occurrence_rate - actual_occurrence_rate)
     return deviation
```

### Comparing `calibra-0.3.0/calibra/plotting.py` & `calibra-0.3.1/calibra/plotting.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,48 +14,44 @@
     """
     Class to generate a calibration curve (AKA reliability curve) given a list of predictions and corresponding true labels.
 
     Uses matplotlib to generate plots. User can specify any matplotlib kwargs and interact directly with the matplotlib figure
     object to customise calibration curve graph to their desire.
 
     Args:
-        y_pred (ndarray):
+        y_pred (np.ndarray):
             Array-like object of shape (num_samples, num_classes) where ij position is predicted probability of data point i belonging to class j.
             Alternatively may be of shape (num_samples,) for binary classification where i position is predicted probability of data point i belonging to class 1 (positive class).
-        y_true (ndarray):
+        y_true (np.ndarray):
             This 1-D array of length num_samples contains the true label for each data point.
         num_bins (int):
             Number of bins the interval [0, 1] is divided into. Exact if method='width', approximate if method='frequency'.
         method (str):
             Method of splitting interval [0, 1] into bins. If set to 'width' divides the interval [0, 1] into num_bins bins of equal width.
             If set to 'frequency' divides the interval [0, 1] into approximately num_bins bins, each containing approximately (num_samples/num_bins) data points.
             Defaults to 'width'.
 
     Attributes:
-        y_pred (ndarray):
+        y_pred (np.ndarray):
             Array-like object of shape (num_samples, num_classes) where ij position is predicted probability of data point i belonging to class j.
             Alternatively may be of shape (num_samples,) for binary classification where i position is predicted probability of data point i belonging to class 1 (positive class).
-        y_true (ndarray):
+        y_true (np.ndarray):
             This 1-D array of length num_samples contains the true label for each data point.
         num_bins (int):
             Number of bins the interval [0, 1] is divided into. Exact if method='width', approximate if method='frequency'.
         method (str):
             Method of splitting interval [0, 1] into bins. If set to 'width' divides the interval [0, 1] into num_bins bins of equal width.
             If set to 'frequency' divides the interval [0, 1] into approximately num_bins bins, each containing approximately num_samples/num_bins data points.
             Defaults to 'width'.
-        num_samples (int):
-            Number of data points.
-        num_classes (int):
-            Number of classes.
         bins (Dict[int, Dict[int, Dict[str, Union[list, int]]]]):
             Dictionary containing, for each class, a dictionary for each bin, itself a dictionary containing the predicted probabilities and number of occurrences of the given class.
         classwise_bin_weights (np.ndarray):
             Numpy array of shape (num_classes, num_bins) whose ijth element represents the proportion of the overall dataset whose predictions for class i lie in bin j.
         bin_boundaries (list):
-            Ordered list of length num_bins + 1 containing start and end point of each bin on interval [0, 1].
+            Ordered list of length num_bins + 1 containing start and end point of each bin on interval [0, 1]. Only applies when method='width'.
         LIGHT_BLUE (np.ndarray):
             Normalised rgb value for light blue. Used as lightest shade of blue for density-based color mapping (i.e. for bins with extremely low density)
         DARK_BLUE (np.ndarray):
             Normalised rgb value for dark blue. Used as darkest shade of blue for density-based color mapping (i.e. for bins with extremely high density)
         COLORMAP (LinearSegmentedColormap):
             Color map which determines shade of blue the bin segments are plotted with (depending on weight of bin).
     """
@@ -73,21 +69,18 @@
         num_bins: int = 20,
         method: str = "width",
     ):
         self.y_pred = _reshape_y_pred(y_pred)
         self.y_true = y_true
         self.num_bins = num_bins
         self.method = method
-        self.num_samples, self.num_classes = self.y_pred.shape
         self.bins = bin_probabilities(
             self.y_pred, self.y_true, self.num_bins, self.method
         )
-        self.classwise_bin_weights = get_classwise_bin_weights(
-            self.bins, self.num_bins, self.num_samples, self.num_classes
-        )
+        self.classwise_bin_weights = get_classwise_bin_weights(self.bins)
         self.bin_boundaries = list(np.linspace(0, 1, self.num_bins + 1))
 
     @staticmethod
     def _segment_curve_data(
         x: List[float], y: List[float], weights: np.ndarray
     ) -> Tuple[List[List[float]], List[List[float]], List[List[float]]]:
         """Generate continuous segments of the non-empty bins to plot in the calibration curve.
@@ -179,15 +172,15 @@
         Therefore, we will create a new array of x values (x_new) containing values for the start, centre and end of each bin, and a new array  of the weights (w_new) containing
         two weight entries for each full bin.
 
         The only exceptions to this are the first bin, for which we only need to include its centre and endpoint in the x_new, (as the original calibration curve plot begins from this point)
         and the final bin, for which we only need to include the start and centre (as the original calibration curve plot finishes at its centre).
         Similarly, the weights of the first and final bins only need to be entered in w_new once.
 
-        The only other exception is for whose 'centre' (expected frequency) coincides with their start boundary. In this case we only include this point once
+        The only other exception is for bins whose 'centre' (expected frequency) coincides with their start boundary. In this case we only include this point once
         in x_new, and similarly, only include its weight once in the w_new (as we can simply plot the whole bin in one segment, start to finish).
 
         pseduo-code:
 
         -> if only one point, return as is
 
         -> else:
@@ -195,16 +188,16 @@
             -> add end boundary of first bin to x_new
             -> for remaining bins up to but excluding final bin:
                 -> check if centre already in x_new (if centre coincides with start boundary - end boundary of previous bin - this will be the case)
                     -> if not, add centre, weight to x_new, w_new
                 -> add end boundary, weight to x_new, w_new
             -> for final bin, check if centre already in x_new (this will be the case if the segment consists of two bins, and the centre of the second bin coincides with the start of the bin)
                 -> if not, add centre, weight of final bin to x_new, w_new
-                
-        Note: For equality checks, we may include tolerance EPSILON to account for floating point errors.
+
+        Note: For equality checks, we include tolerance EPSILON to account for floating point errors.
 
         Args:
             x (List[float]):
                 List of x values for given segment to be plotted as part of the calibration curve.
                 Each value represents the 'centre' of a bin (expected frequency) along the calibration curve.
             weights (List[float]):
                 List of weights corresponding to x values. Each value represents proportion of predictions residing in a given each bin.
@@ -213,32 +206,42 @@
             Tuple[List[float], List[float]]
         """
         if len(x) == 1:
             return x, weights
 
         x_new, w_new = [x[0]], [weights[0]]
         first_bin_end_boundary = list(
-            filter(lambda boundary: boundary - CalibrationCurve.EPSILON > x[0], self.bin_boundaries)
+            filter(
+                lambda boundary: boundary - CalibrationCurve.EPSILON > x[0],
+                self.bin_boundaries,
+            )
         )[0]
         x_new.append(first_bin_end_boundary)
 
         for bin_expected_freq, bin_weight in zip(x[1:-1], weights[1:-1]):
-            already_in_x_new = list(filter(lambda x: abs(x - bin_expected_freq) < CalibrationCurve.EPSILON, x_new))
+            already_in_x_new = list(
+                filter(
+                    lambda x: abs(x - bin_expected_freq) < CalibrationCurve.EPSILON,
+                    x_new,
+                )
+            )
             if not already_in_x_new:
                 x_new.append(bin_expected_freq)
                 w_new.append(bin_weight)
             bin_end_boundary = list(
                 filter(
-                    lambda boundary: boundary - CalibrationCurve.EPSILON > bin_expected_freq, self.bin_boundaries
+                    lambda boundary: boundary - CalibrationCurve.EPSILON
+                    > bin_expected_freq,
+                    self.bin_boundaries,
                 )
             )[0]
             x_new.append(bin_end_boundary)
             w_new.append(bin_weight)
 
-        if x[-1] not in x_new:     
+        if x[-1] not in x_new:
             x_new.append(x[-1])
             w_new.append(weights[-1])
 
         return x_new, w_new
 
     @staticmethod
     def _get_y_at_bin_centre(
@@ -326,23 +329,23 @@
     def _get_density_based_line_collection(
         self,
         x: List[float],
         y: List[float],
         weights: List[float],
         normalizer: Union[LogNorm, Normalize],
     ) -> LineCollection:
-        """Get collections of lines to plot calibration curve. Each line in the collection represents either half a bin, or a full bin
+        """Get collection of lines to plot the calibration curve. Each line in the collection represents either half a bin, or a full bin
         along the calibration curve. The color of each line is a function of the density (weight) of the given bin.
 
         Args:
             x (List[float]): List of expected frequencies of each bin ('centre' of bin) along given segment of the calibration curve.
             y (List[float]): List of actual frequencies of each bin along given segment of the calibration curve.
             weights (List[float]): List of weights corresponding to each bin along given segment of the calibration curve.
-            normalizer (Union[Normalize, LogNorm]): A function that scales bin weights from the specified range [vmin, vmax] in the plot() method to a normalized range [0, 1]. 
-                Values outside of [vmin, vmax] are clamped at 0 or 1. This normalized range is then used for density-based color mapping. The normalization can be either logarithmic or linear:
+            normalizer (Union[Normalize, LogNorm]): A function that scales bin weights from the specified range [vmin, vmax] in the plot() method to a normalized range [0, 1].
+                Values less than vmin are clamped at 0. This normalized range is then used for density-based color mapping. The normalization can be either logarithmic or linear:
                 - Linear normalization (Normalize) scales values directly proportionate to their distance between vmin and vmax.
                 - Logarithmic normalization (LogNorm) emphasizes differences in lower ranges by scaling the logarithm of values, making subtle variations in lower densities more visible.
                 Defaults to LogNorm.
 
         Returns:
             LineCollection:
                 Collection of lines where each line represents a segment of the calibration curve.
@@ -371,36 +374,37 @@
         normalization_type: str = "log",
         vmin: float = 0.01,
         vmax: float = 1,
     ) -> Tuple[bool, Union[LogNorm, Normalize]]:
         """
         Validate and configure inputs related to color mapping of calibration curve when show_density == True.
 
-        Ensure normalization_type, vmin and vmax values are valid. If binning method == 'frequency', show user warning message and set show_density to False. 
+        Ensure normalization_type, vmin and vmax values are valid. If binning method == 'frequency', show user warning message and set show_density to False.
 
         Args:
             show_density (bool):
                 If True, the color strength of the curve is a function of the bin density at each point.
                 Defaults to False.
             normalization_type (str):
-                Indicates method for scaling bin weights. These weights can be scaled either linearly or logarithmically from [vmin, vmax] to [0, 1] (with values 
-                outside of [vmin, vmax] being clamped to 0 or 1).
-            vmin (float): 
+                Indicates method for scaling bin weights. These weights can be scaled either linearly or logarithmically from [vmin, vmax] to [0, 1] (with values
+                less than vmin being clamped to 0).
+            vmin (float):
                 The minimum value used for normalization, setting the lower bound of the data range that maps to the lower end of the colormap.
             vmax (float):
                 The maximum value used for normalization, defining the upper bound of the data range that maps to the upper end of the colormap.
-        
+
         Returns:
             Tuple[bool, Union[LogNorm, Normalize]]
         """
         if self.method == "frequency":
             show_density = False
             warnings.warn(
                 """Density-based color mapping not available when method=='frequency', as bins do not have well-defined boundaries.  
-                        In any case, equal frequency bins have equal density, by definition. Setting show_density='False'.""", UserWarning
+                        In any case, equal frequency bins have equal density, by definition. Setting show_density=False.""",
+                UserWarning,
             )
 
         if normalization_type not in ["log", "linear"]:
             raise ValueError("normalization_type must be either 'log' or 'linear'")
 
         if vmin > vmax or vmin < 0 or vmax > 1:
             raise ValueError(
@@ -428,28 +432,35 @@
 
         Args:
             class_label (int):
                 Label of the class whose calibration curve is plotted. Defaults to 0 (the first class).
             show_density (bool):
                 If True, the color strength of the curve is a function of the bin density at each point.
                 Defaults to False.
+            normalization_type (str):
+                Indicates method for scaling bin weights. These weights can be scaled either linearly or logarithmically from [vmin, vmax] to [0, 1] (with values
+                less than vmin being clamped to 0).
+            vmin (float):
+                The minimum value used for normalization, setting the lower bound of the data range that maps to the lower end of the colormap.
+            vmax (float):
+                The maximum value used for normalization, defining the upper bound of the data range that maps to the upper end of the colormap.
             **kwargs (Dict[str, Any]):
                 matplotlib keyword arguments for customising the plot.
-        
+
         Returns:
             Tuple[Figure, Axes]
         """
         if show_density:
             show_density, normalizer = self._configure_show_density_settings(
                 show_density, normalization_type, vmin, vmax
             )
 
         fig, ax = plt.subplots()
         ax.plot(
-            [0, 1], [0, 1], color="black", linestyle="--", label="Perfectly Calibrated"
+            [0, 1], [0, 1], color="black", linestyle="--", label="Perfect Calibration"
         )
         x_segments, y_segments, weight_segments = self._generate_x_y(class_label)
 
         for x, y, weights in zip(x_segments, y_segments, weight_segments):
             if show_density and len(x) > 1:
                 lc = self._get_density_based_line_collection(x, y, weights, normalizer)
                 ax.add_collection(lc)
```

### Comparing `calibra-0.3.0/calibra/utils.py` & `calibra-0.3.1/calibra/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 import pandas as pd
 import numpy as np
-from typing import Callable, Any, List
+from typing import Callable, Any
 from functools import wraps
 
 
 def validate_input(func: Callable[..., Any]) -> Callable[..., Any]:
     """
     Validate the input parameters to ensure they are in the correct format. Convert to correct format where possible, otherwise, raise error.
 
@@ -22,15 +22,15 @@
     Raises:
       ValueError: If any of the inputs do not meet the validation criteria.
 
     Returns:
       The original function's return value, if all inputs are valid.
     """    
     @wraps(func)
-    def wrapper(y_pred, y_true, num_bins, method, *args, **kwargs):
+    def wrapper(y_pred, y_true, num_bins: int = 20, method: str = 'width', *args, **kwargs):
         
         y_pred = np.asarray(y_pred)
         if y_pred.ndim > 2 or np.any(y_pred < 0) or np.any(y_pred > 1):
             raise ValueError("y_pred must be a 1D or 2D array with values between 0 and 1.")
         
         if isinstance(y_true, list):
             if not all(label % 1 == 0 and label >= 0 for label in y_true):
@@ -54,23 +54,23 @@
             raise ValueError("Method must be either 'width' or 'frequency'")
 
         return func(y_pred, y_true, num_bins, method, *args, **kwargs)
     return wrapper
 
 
 @validate_input
-def bin_probabilities(y_pred: np.ndarray, y_true: np.ndarray, num_bins: int, method: str = 'width') -> dict:
+def bin_probabilities(y_pred: np.ndarray, y_true: np.ndarray, num_bins: int = 20, method: str = 'width') -> dict:
     """
     Group predictions into bins, along with corresponding true labels.
     
     Args:
-        y_pred (ndarray):
+        y_pred (np.ndarray):
             Array-like object of shape (num_samples, num_classes) where ij position is predicted probability of data point i belonging to class j.
             Alternatively may be of shape (num_samples,) for binary classification where i position is predicted probability of data point i belonging to class 1 (positive class).
-        y_true (ndarray):
+        y_true (np.ndarray):
             This 1-D array of length num_samples contains the true label for each data point.        
         num_bins (int):
             Number of bins the interval [0, 1] is divided into. Exact if method='width', approximate if method='frequency'.
         method (str):
             Method of splitting interval [0, 1] into bins. If set to 'width' divides the interval [0, 1] into num_bins bins of equal width.
             If set to 'frequency' divides the interval [0, 1] into approximately num_bins bins, each containing approximately num_samples/num_bins data points. 
             Defaults to 'width'.      
@@ -102,20 +102,20 @@
     return bins
 
 def _reshape_y_pred(y_pred: np.ndarray) -> np.ndarray:
     """
     If y_pred is a 1D array, reshape to (num_samples, num_classes)
 
     Args:
-        y_pred (ndarray):
+        y_pred (np.ndarray):
             Array-like object of shape (num_samples, num_classes) where ij position is predicted probability of data point i belonging to class j.
             Alternatively may be of shape (num_samples,) for binary classification where i position is predicted probability of data point i belonging to class 1 (positive class).
 
     Returns:
-        ndarray
+        np.ndarray
     """
     if np.asarray(y_pred).ndim == 1:
         y_pred = np.asarray(
             [
             [1 - prob, prob] for prob in y_pred
             ]
         )
@@ -142,17 +142,17 @@
 
 
 def _get_equal_width_bins(y_pred: np.ndarray, y_true: np.ndarray, num_classes: int, num_samples: int, num_bins: int, bins: dict) -> dict:
     """
     Group predictions into bins of equal width.
 
     Args:
-        y_pred (ndarray):
+        y_pred (np.ndarray):
             Array-like object of shape (num_samples, num_classes) where ij position is predicted probability of data point i belonging to class j.
-        y_true (ndarray):
+        y_true (np.ndarray):
             This 1-D array of length num_samples contains the true label for each data point.
         num_classes (int):
             Number of classes.        
         num_samples (int):
             Number of data points.                    
         num_bins (int):
             Number of equal-width bins the interval [0, 1] is divided into.
@@ -169,27 +169,27 @@
             map(
                 lambda x: (num_bins-1) if x==1 else math.floor(num_bins * x), 
                     y_pred_class_i
                 )
             ) 
         # returns num_bins-1 if p==1, else returns m for p in [m/num_bins, (m+1)/num_bins) 
         for j in range(num_samples): 
-            bins[i][bin_index[j]]['probs'].append(y_pred_class_i[j]) # group predicted probabilities into the bins
-            bins[i][bin_index[j]]['num_occurrences'] += y_true_class_i[j] # keep track of the number of occurrences of class i in each bin
+            bins[i][bin_index[j]]['probs'].append(y_pred_class_i[j]) 
+            bins[i][bin_index[j]]['num_occurrences'] += y_true_class_i[j] 
             
     return bins
 
 def _get_equal_frequency_bins(y_pred: np.ndarray, y_true: np.ndarray, num_classes: int, num_samples: int, num_bins: int, bins: dict) -> dict:
     """
     Group predictions into bins containing equal numbers of data points.
 
     Args:
-        y_pred (ndarray):
+        y_pred (np.ndarray):
             Array-like object of shape (num_samples, num_classes) where ij position is predicted probability of data point i belonging to class j.
-        y_true (ndarray):
+        y_true (np.ndarray):
             This 1-D array of length num_samples contains the true label for each data point.
         num_classes (int):
             Number of classes.        
         num_samples (int):
             Number of data points.                    
         num_bins (int):
             Approximate number of bins the interval [0, 1] is divided into, each containing approximately the same number of data points.
@@ -309,48 +309,78 @@
 
 
 def _sort_predictions(y_pred_class_i: list, y_true_class_i: list) -> tuple:
     """
     Sort the predicted probabilities in ascending order. Sort the true labels so they correspond to the sorted predictions.
 
     Args:
-        y_pred_class_i (ndarray):
+        y_pred_class_i (np.ndarray):
             Array-like object of shape (num_samples,) where i position is predicted probability of data point i belonging to given class.
-        y_true_class_i (ndarray):
+        y_true_class_i (np.ndarray):
             1-D array of length num_samples, where i position is 1 if data point i belongs to given class, 0 otherwise.
     
     Returns:
         tuple
     """
     zipped_list = list(zip(y_pred_class_i, y_true_class_i))
     sorted_zipped_list = sorted(zipped_list)
     y_pred_sorted, y_true_sorted = zip(*sorted_zipped_list)
 
     return list(y_pred_sorted), list(y_true_sorted)
 
 
-def get_classwise_bin_weights(bins: dict, num_bins: int, num_samples: int, num_classes: int) -> np.ndarray:
+def validate_bins(func: Callable[..., Any]) -> Callable[..., Any]:
     """
-    Calculate the 
+    Validate the input parameters to ensure they are in the correct format. Otherwise, raise error.
+
+    Args:
+        func: The method for which we validate the input.
+
+    Raises:
+      ValueError: If any of the inputs do not meet the validation criteria.
+
+    Returns:
+      The original function's return value, if all inputs are valid.
+    """    
+    @wraps(func)
+    def wrapper(bins: dict,  *args, **kwargs):
+        assert isinstance(bins, dict) and len(bins) > 0, "'bins' must be a non-empty dict"
+        assert all(isinstance(key, int) for key in bins.keys()), "'bins' keys must be integers"
+
+        for class_i_bins in bins.values():            
+            assert isinstance(class_i_bins, dict) and len(class_i_bins) > 0, "'bins' first-level values must themselves be non-empty dictionaries."
+            assert all(isinstance(key, int) for key in class_i_bins.keys()), "'bins' first-level values must themselves be non-empty dictionaries with integer keys."
+
+            for class_i_bin_j in class_i_bins.values():            
+                assert isinstance(class_i_bin_j, dict) and "probs" in class_i_bin_j, "'bins' second-level values must themselves be dictionaries with keys: {'probs', 'num_occurrences'}"            
+                                
+        return func(bins, *args, **kwargs)
+
+    return wrapper
+
+@validate_bins
+def get_classwise_bin_weights(bins: dict) -> np.ndarray:
+    """
+    Calculate the weight of each bin across all classes.
+
     Args:
         bins (dict):
             Dictionary containing, for each class, each bin, itself containing the predicted probabilities and occurences of the given class.                    
-        num_bins (int):
-            Number of equal-width bins the interval [0, 1] is divided into.
-        num_samples (int):
-            Number of data points.
-        num_classes (int):
-            Number of classes.
 
     Returns:
         np.ndarray:
             Numpy array of shape (num_classes, num_bins) whose ijth element represents the proportion of the overall dataset whose predictions for class i lie in bin j.    
-    """    
+    """
+    num_classes = len(bins)
+    num_bins = len(bins[0])
+    num_samples = sum(
+        [len(bins[0][i]['probs']) for i in range(num_bins)]
+    )
+
     weights = [
         [
             _get_bin_weight(bins[i][b], num_samples) for b in range(num_bins)
         ]
         for i in range(num_classes)
     ]
     
     return np.asarray(weights)
-
```

### Comparing `calibra-0.3.0/calibra.egg-info/PKG-INFO` & `calibra-0.3.1/calibra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibra
-Version: 0.3.0
+Version: 0.3.1
 Summary: Toolkit for calibration of machine learning classifiers.
 Home-page: https://github.com/conorwalsh99/calibra
 Author: Conor Walsh
 Author-email: conorwalsh206@gmail.com
 License: MIT license
 Keywords: calibra
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `calibra-0.3.0/calibra.egg-info/SOURCES.txt` & `calibra-0.3.1/calibra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calibra-0.3.0/docs/Makefile` & `calibra-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `calibra-0.3.0/docs/conf.py` & `calibra-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `calibra-0.3.0/docs/installation.rst` & `calibra-0.3.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `calibra-0.3.0/docs/make.bat` & `calibra-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `calibra-0.3.0/setup.py` & `calibra-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='calibra',
     name='calibra',
     packages=find_packages(include=['calibra', 'calibra.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/conorwalsh99/calibra',
-    version='0.3.0',
+    version='0.3.1',
     zip_safe=False,
 )
```

### Comparing `calibra-0.3.0/tests/baseline/test_plot.png` & `calibra-0.3.1/tests/baseline/test_plot.png`

 * *Files identical despite different names*

### Comparing `calibra-0.3.0/tests/conftest.py` & `calibra-0.3.1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -635,15 +635,14 @@
             3: {"probs": [], "num_occurrences": 0},
         },
     }
 
 
 @pytest.fixture
 def get_classwise_bin_weights_input():
-    num_bins, num_samples, num_classes = 5, 10, 2
     bins = {
         0: {
             0: {
                 "probs": [0.05, 0.15],
                 "num_occurrences": 0,
             },
             1: {
@@ -682,22 +681,27 @@
             },
             4: {
                 "probs": [0.85, 0.95],
                 "num_occurrences": 2,
             },
         },
     }
-    return bins, num_bins, num_samples, num_classes
+    return bins
 
 
 @pytest.fixture
 def get_classwise_bin_weights_expected():
     return np.asarray([[0.2, 0.2, 0.2, 0.2, 0.2], [0.2, 0.2, 0.2, 0.2, 0.2]])
 
 
+@pytest.fixture
+def get_classwise_bin_weights_bad_input():
+    return {}
+
+
 ###### test_errors.py ######
 
 
 @pytest.fixture
 def classwise_ece_perfectly_calibrated_input():
     """
     Input that should result in perfect calibration.
@@ -1157,21 +1161,81 @@
 def _generate_x_y_with_bin_boundaries_two_values_expected():
     """Interpolated by hand"""
     x_new = [0.15, 0.2]
     y_new = [0.1, 0.24]
     weights_new = [0.1]
     return x_new, y_new, weights_new
 
+
 @pytest.fixture
 def _get_density_based_line_collection_segment_start_boundaries():
     """Rather than generate an expected LineCollection object, it is easier to ensure the segments are as we expect them to be in terms of (half-) bin boundaries and associated weights"""
-    return [0.04, 0.1, 0.12, 0.2, 0.27, 0.3, 0.33, 0.4, 0.45, 0.5, 0.55, 0.6, 0.68, 0.7, 0.73, 0.8, 0.84, 0.9]
+    return [
+        0.04,
+        0.1,
+        0.12,
+        0.2,
+        0.27,
+        0.3,
+        0.33,
+        0.4,
+        0.45,
+        0.5,
+        0.55,
+        0.6,
+        0.68,
+        0.7,
+        0.73,
+        0.8,
+        0.84,
+        0.9,
+    ]
+
 
 @pytest.fixture
 def _get_density_based_line_collection_segment_end_boundaries():
     """Rather than generate an expected LineCollection object, it is easier to ensure the segments are as we expect them to be in terms of (half-) bin boundaries and associated weights"""
-    return [0.1, 0.12, 0.2, 0.27, 0.3, 0.33, 0.4, 0.45, 0.5, 0.55, 0.6, 0.68, 0.7, 0.73, 0.8, 0.84, 0.9, 0.96]
+    return [
+        0.1,
+        0.12,
+        0.2,
+        0.27,
+        0.3,
+        0.33,
+        0.4,
+        0.45,
+        0.5,
+        0.55,
+        0.6,
+        0.68,
+        0.7,
+        0.73,
+        0.8,
+        0.84,
+        0.9,
+        0.96,
+    ]
+
 
 @pytest.fixture
 def _get_density_based_line_collection_segment_weights():
     """Rather than generate an expected LineCollection object, it is easier to ensure the segments are as we expect them to be in terms of (half-) bin boundaries and associated weights"""
-    return [0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1]
+    return [
+        0.1,
+        0.1,
+        0.1,
+        0.1,
+        0.1,
+        0.1,
+        0.1,
+        0.1,
+        0.1,
+        0.1,
+        0.1,
+        0.1,
+        0.1,
+        0.1,
+        0.1,
+        0.1,
+        0.1,
+        0.1,
+    ]
```

### Comparing `calibra-0.3.0/tests/test_plotting.py` & `calibra-0.3.1/tests/test_plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,81 +377,129 @@
         assert np.allclose(
             y_result, y_expected
         ), f"_generate_x_y_with_bin_boundaries returned {y_result} instead of {y_expected}"
         assert np.allclose(
             weights_result, weights_expected
         ), f"_generate_x_y_with_bin_boundaries returned {weights_result} instead of {weights_expected}"
 
-    def test_get_density_based_line_collection(self, 
-                                            continuous_calibration_curve_input, 
-                                            continuous_calibration_curve_generate_x_y_expected, 
-                                            _get_density_based_line_collection_segment_start_boundaries, 
-                                            _get_density_based_line_collection_segment_end_boundaries, 
-                                            _get_density_based_line_collection_segment_weights):
+    def test_get_density_based_line_collection(
+        self,
+        continuous_calibration_curve_input,
+        continuous_calibration_curve_generate_x_y_expected,
+        _get_density_based_line_collection_segment_start_boundaries,
+        _get_density_based_line_collection_segment_end_boundaries,
+        _get_density_based_line_collection_segment_weights,
+    ):
         """
         Rather than generate an expected LineCollection object, it is easier to ensure the segments are as we expect them to be in terms of (half-) bin boundaries and associated weights
         """
         y_pred, y_true, num_bins, method = continuous_calibration_curve_input
         calibration_curve = CalibrationCurve(y_pred, y_true, num_bins, method)
         [x], [y], [weights] = continuous_calibration_curve_generate_x_y_expected
         normalizer = LogNorm(vmin=0.01, vmax=1)
-        result = calibration_curve._get_density_based_line_collection(x, y, weights, normalizer)
+        result = calibration_curve._get_density_based_line_collection(
+            x, y, weights, normalizer
+        )
 
         segments = result.get_segments()
         segment_start_boundaries_result = [segment[0][0] for segment in segments]
         segment_end_boundaries_result = [segment[1][0] for segment in segments]
         segment_weights_result = result.get_array()
 
-        segment_start_boundaries_expected = _get_density_based_line_collection_segment_start_boundaries
-        segment_end_boundaries_expected = _get_density_based_line_collection_segment_end_boundaries
+        segment_start_boundaries_expected = (
+            _get_density_based_line_collection_segment_start_boundaries
+        )
+        segment_end_boundaries_expected = (
+            _get_density_based_line_collection_segment_end_boundaries
+        )
         segment_weights_expected = _get_density_based_line_collection_segment_weights
-        
-        assert type(result) == LineCollection, f'_get_density_based_line_collection() failed to return LineCollection object.'
-        assert np.allclose(segment_start_boundaries_result, segment_start_boundaries_expected), f'Segment start boundaries different. Expected {segment_start_boundaries_expected}, got {segment_start_boundaries_result}'
-        assert np.allclose(segment_end_boundaries_result, segment_end_boundaries_expected), f'Segment end boundaries different. Expected {segment_end_boundaries_expected}, got {segment_end_boundaries_result}'
-        assert np.allclose(segment_weights_result, segment_weights_expected), f'Segment weights different. Expected {segment_weights_expected}, got {segment_weights_result}'                
 
-    def test_configure_show_density_settings_normal(self, continuous_calibration_curve_input):
+        assert (
+            type(result) == LineCollection
+        ), f"_get_density_based_line_collection() failed to return LineCollection object."
+        assert np.allclose(
+            segment_start_boundaries_result, segment_start_boundaries_expected
+        ), f"Segment start boundaries different. Expected {segment_start_boundaries_expected}, got {segment_start_boundaries_result}"
+        assert np.allclose(
+            segment_end_boundaries_result, segment_end_boundaries_expected
+        ), f"Segment end boundaries different. Expected {segment_end_boundaries_expected}, got {segment_end_boundaries_result}"
+        assert np.allclose(
+            segment_weights_result, segment_weights_expected
+        ), f"Segment weights different. Expected {segment_weights_expected}, got {segment_weights_result}"
+
+    def test_configure_show_density_settings_normal(
+        self, continuous_calibration_curve_input
+    ):
         y_pred, y_true, num_bins, method = continuous_calibration_curve_input
-        calibration_curve = CalibrationCurve(y_pred, y_true, num_bins, method)        
+        calibration_curve = CalibrationCurve(y_pred, y_true, num_bins, method)
         show_density = True
-        normalization_type = 'log'
+        normalization_type = "log"
         vmin, vmax = 0.01, 1
-        show_density_result, normalizer_result = calibration_curve._configure_show_density_settings(show_density, normalization_type, vmin, vmax)        
-        assert show_density_result == True, f'Failed to return correct show_density. Got {show_density_result} instead of {True}.'
-        assert type(normalizer_result) == LogNorm, f'Failed to return correct normalizer. Got {type(normalizer_result)} instead of {LogNorm}.'
-
-    def test_configure_show_density_settings_bad_normalizer(self, continuous_calibration_curve_input):
+        show_density_result, normalizer_result = (
+            calibration_curve._configure_show_density_settings(
+                show_density, normalization_type, vmin, vmax
+            )
+        )
+        assert (
+            show_density_result == True
+        ), f"Failed to return correct show_density. Got {show_density_result} instead of {True}."
+        assert (
+            type(normalizer_result) == LogNorm
+        ), f"Failed to return correct normalizer. Got {type(normalizer_result)} instead of {LogNorm}."
+
+    def test_configure_show_density_settings_bad_normalizer(
+        self, continuous_calibration_curve_input
+    ):
         y_pred, y_true, num_bins, method = continuous_calibration_curve_input
-        calibration_curve = CalibrationCurve(y_pred, y_true, num_bins, method)        
+        calibration_curve = CalibrationCurve(y_pred, y_true, num_bins, method)
         show_density = True
-        normalization_type = 'power'
+        normalization_type = "power"
         vmin, vmax = 0.01, 1
         with pytest.raises(ValueError):
-            show_density_result, normalizer_result = calibration_curve._configure_show_density_settings(show_density, normalization_type, vmin, vmax)
-    
-    def test_configure_show_density_settings_bad_vmin_vmax(self, continuous_calibration_curve_input):
+            show_density_result, normalizer_result = (
+                calibration_curve._configure_show_density_settings(
+                    show_density, normalization_type, vmin, vmax
+                )
+            )
+
+    def test_configure_show_density_settings_bad_vmin_vmax(
+        self, continuous_calibration_curve_input
+    ):
         y_pred, y_true, num_bins, method = continuous_calibration_curve_input
-        calibration_curve = CalibrationCurve(y_pred, y_true, num_bins, method)        
+        calibration_curve = CalibrationCurve(y_pred, y_true, num_bins, method)
         show_density = True
-        normalization_type = 'linear'
+        normalization_type = "linear"
         vmin, vmax = 2, -2
         with pytest.raises(ValueError):
-            show_density_result, normalizer_result = calibration_curve._configure_show_density_settings(show_density, normalization_type, vmin, vmax)
-
-    def test_configure_show_density_settings_method_is_frequency(self, continuous_calibration_curve_input):
-        y_pred, y_true, num_bins, method = continuous_calibration_curve_input
-        calibration_curve = CalibrationCurve(y_pred, y_true, num_bins, method='frequency')        
+            show_density_result, normalizer_result = (
+                calibration_curve._configure_show_density_settings(
+                    show_density, normalization_type, vmin, vmax
+                )
+            )
+
+    def test_configure_show_density_settings_method_is_frequency(
+        self, continuous_calibration_curve_input
+    ):
+        y_pred, y_true, num_bins, method = continuous_calibration_curve_input
+        calibration_curve = CalibrationCurve(
+            y_pred, y_true, num_bins, method="frequency"
+        )
         show_density = True
-        normalization_type = 'log'
+        normalization_type = "log"
         vmin, vmax = 0.1, 1
         with pytest.warns(UserWarning):
-            show_density_result, normalizer_result = calibration_curve._configure_show_density_settings(show_density, normalization_type, vmin, vmax)
-        assert show_density_result == False, f'Failed to set show_density=False.'
-        assert type(normalizer_result) == LogNorm, f'Failed to return correct normalizer. Got {normalizer_result} instead of {LogNorm}'
+            show_density_result, normalizer_result = (
+                calibration_curve._configure_show_density_settings(
+                    show_density, normalization_type, vmin, vmax
+                )
+            )
+        assert show_density_result == False, f"Failed to set show_density=False."
+        assert (
+            type(normalizer_result) == LogNorm
+        ), f"Failed to return correct normalizer. Got {normalizer_result} instead of {LogNorm}"
 
     @pytest.mark.mpl_image_compare
     def test_plot(self, continuous_calibration_curve_input):
         y_pred, y_true, num_bins, method = continuous_calibration_curve_input
         calibration_curve = CalibrationCurve(y_pred, y_true, num_bins, method)
         fig_result, ax_result = calibration_curve.plot()
-        return fig_result 
+        return fig_result
```

### Comparing `calibra-0.3.0/tests/test_utils.py` & `calibra-0.3.1/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,284 +1,398 @@
 import pytest
-import pandas as pd 
-import numpy as np 
+import pandas as pd
+import numpy as np
 
-from calibra.utils import (bin_probabilities, 
-                        _get_equal_width_bins, 
-                        _get_equal_frequency_bins, 
-                        _sort_predictions, 
-                        _reshape_y_pred,
-                        _get_bin_weight,
-                        _sum_occurrences,
-                        _back_fill_equal_frequency_bins,
-                        _forward_fill_equal_frequency_bins,
-                        get_classwise_bin_weights
-                    )
-    
-
-def test_sort_predictions_good_input(sort_predictions_good_input, expected_sort_predictions_good_input):
+from calibra.utils import (
+    bin_probabilities,
+    _get_equal_width_bins,
+    _get_equal_frequency_bins,
+    _sort_predictions,
+    _reshape_y_pred,
+    _get_bin_weight,
+    _sum_occurrences,
+    _back_fill_equal_frequency_bins,
+    _forward_fill_equal_frequency_bins,
+    get_classwise_bin_weights,
+)
+
+
+def test_sort_predictions_good_input(
+    sort_predictions_good_input, expected_sort_predictions_good_input
+):
     y_pred_class_i, y_true_class_i = sort_predictions_good_input
-    result_y_pred_class_i_sorted, result_y_true_class_i_sorted = _sort_predictions(y_pred_class_i, y_true_class_i)
-    expected_y_pred_class_i_sorted, expected_y_true_class_i_sorted = expected_sort_predictions_good_input
-    
+    result_y_pred_class_i_sorted, result_y_true_class_i_sorted = _sort_predictions(
+        y_pred_class_i, y_true_class_i
+    )
+    expected_y_pred_class_i_sorted, expected_y_true_class_i_sorted = (
+        expected_sort_predictions_good_input
+    )
+
     message = f"sort_predictions did not sort predictions correctly. Returned: {result_y_pred_class_i_sorted} instead of {expected_y_pred_class_i_sorted}"
     assert result_y_pred_class_i_sorted == expected_y_pred_class_i_sorted, message
 
     message = f"sort_predictions did not sort predictions correctly. Returned: {result_y_true_class_i_sorted} instead of {expected_y_true_class_i_sorted}"
     assert result_y_true_class_i_sorted == expected_y_true_class_i_sorted, message
 
 
-def test_sort_predictions_duplicate_predictions(sort_predictions_duplicate_predictions, expected_sort_predictions_duplicate_predictions):
+def test_sort_predictions_duplicate_predictions(
+    sort_predictions_duplicate_predictions,
+    expected_sort_predictions_duplicate_predictions,
+):
     y_pred_class_i, y_true_class_i = sort_predictions_duplicate_predictions
-    result_y_pred_class_i_sorted, result_y_true_class_i_sorted = _sort_predictions(y_pred_class_i, y_true_class_i)
-    expected_y_pred_class_i_sorted, expected_y_true_class_i_sorted = expected_sort_predictions_duplicate_predictions
+    result_y_pred_class_i_sorted, result_y_true_class_i_sorted = _sort_predictions(
+        y_pred_class_i, y_true_class_i
+    )
+    expected_y_pred_class_i_sorted, expected_y_true_class_i_sorted = (
+        expected_sort_predictions_duplicate_predictions
+    )
 
     message = f"sort_predictions did not sort predictions correctly. Returned: {result_y_pred_class_i_sorted} instead of {expected_y_pred_class_i_sorted}"
     assert result_y_pred_class_i_sorted == expected_y_pred_class_i_sorted, message
 
     message = f"sort_predictions did not sort predictions correctly. Returned: {result_y_true_class_i_sorted} instead of {expected_y_true_class_i_sorted}"
-    assert result_y_true_class_i_sorted == expected_y_true_class_i_sorted[0] or result_y_true_class_i_sorted == expected_y_true_class_i_sorted[1], message
+    assert (
+        result_y_true_class_i_sorted == expected_y_true_class_i_sorted[0]
+        or result_y_true_class_i_sorted == expected_y_true_class_i_sorted[1]
+    ), message
 
 
-def test_get_equal_width_bins(get_bins_good_input, expected_get_equal_width_bins_good_input):
+def test_get_equal_width_bins(
+    get_bins_good_input, expected_get_equal_width_bins_good_input
+):
     result = _get_equal_width_bins(*get_bins_good_input)
     expected = expected_get_equal_width_bins_good_input
     message = f"get_equal_width_bins returned {result}, instead of {expected}"
-    assert result == expected, message 
-    
-def test_get_equal_frequency_bins(get_bins_good_input, expected_get_equal_frequency_bins_good_input):
+    assert result == expected, message
+
+
+def test_get_equal_frequency_bins(
+    get_bins_good_input, expected_get_equal_frequency_bins_good_input
+):
     result = _get_equal_frequency_bins(*get_bins_good_input)
     expected = expected_get_equal_frequency_bins_good_input
     message = f"get_equal_frequency_bins returned {result}, instead of {expected}"
 
-def test_bin_probabilities_good_input_width_1d_ypred(bin_probabilities_good_input_width_1d_y_pred, expected_get_equal_width_bins_good_input):
+
+def test_bin_probabilities_good_input_width_1d_ypred(
+    bin_probabilities_good_input_width_1d_y_pred,
+    expected_get_equal_width_bins_good_input,
+):
     result = bin_probabilities(*bin_probabilities_good_input_width_1d_y_pred)
     expected = expected_get_equal_width_bins_good_input
     message = f"bin_probabilities returned {result}, instead of {expected}"
     dicts_equal = True
     try:
         for class_key in expected:
             expected_class_level_dict = expected[class_key]
             result_class_level_dict = result[class_key]
             for bin_key in expected_class_level_dict:
                 expected_bin_level_dict = expected_class_level_dict[bin_key]
                 result_bin_level_dict = result_class_level_dict[bin_key]
-                expected_probs = expected_bin_level_dict['probs']
-                result_probs = result_bin_level_dict['probs']
-                expected_num_occurrences = expected_bin_level_dict['num_occurrences']
-                result_num_occurrences = result_bin_level_dict['num_occurrences']
+                expected_probs = expected_bin_level_dict["probs"]
+                result_probs = result_bin_level_dict["probs"]
+                expected_num_occurrences = expected_bin_level_dict["num_occurrences"]
+                result_num_occurrences = result_bin_level_dict["num_occurrences"]
 
                 if expected_num_occurrences != result_num_occurrences:
                     dicts_equal = False
-                    print(f'Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}')
-                    raise AssertionError('Dictionaries not equal')
+                    print(
+                        f"Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}"
+                    )
+                    raise AssertionError("Dictionaries not equal")
                 elif len(expected_probs) != len(result_probs):
-                    print(f'Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}')
-                    raise AssertionError('Dictionaries not equal')
-                elif not all(abs(a - b) < 1e-8 for a, b in zip(expected_probs, result_probs)):
-                    print(f'Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}')
-                    raise AssertionError('Dictionaries not equal')
+                    print(
+                        f"Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}"
+                    )
+                    raise AssertionError("Dictionaries not equal")
+                elif not all(
+                    abs(a - b) < 1e-8 for a, b in zip(expected_probs, result_probs)
+                ):
+                    print(
+                        f"Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}"
+                    )
+                    raise AssertionError("Dictionaries not equal")
     except:
         dicts_equal = False
 
-    assert dicts_equal, message 
+    assert dicts_equal, message
 
 
-def test_bin_probabilities_good_input_width_2d_ypred(bin_probabilities_good_input_width_2d_y_pred, expected_get_equal_width_bins_good_input):
+def test_bin_probabilities_good_input_width_2d_ypred(
+    bin_probabilities_good_input_width_2d_y_pred,
+    expected_get_equal_width_bins_good_input,
+):
     result = bin_probabilities(*bin_probabilities_good_input_width_2d_y_pred)
     expected = expected_get_equal_width_bins_good_input
     message = f"bin_probabilities returned {result}, instead of {expected}"
     dicts_equal = True
     try:
         for class_key in expected:
             expected_class_level_dict = expected[class_key]
             result_class_level_dict = result[class_key]
             for bin_key in expected_class_level_dict:
                 expected_bin_level_dict = expected_class_level_dict[bin_key]
                 result_bin_level_dict = result_class_level_dict[bin_key]
-                expected_probs = expected_bin_level_dict['probs']
-                result_probs = result_bin_level_dict['probs']
-                expected_num_occurrences = expected_bin_level_dict['num_occurrences']
-                result_num_occurrences = result_bin_level_dict['num_occurrences']
+                expected_probs = expected_bin_level_dict["probs"]
+                result_probs = result_bin_level_dict["probs"]
+                expected_num_occurrences = expected_bin_level_dict["num_occurrences"]
+                result_num_occurrences = result_bin_level_dict["num_occurrences"]
 
                 if expected_num_occurrences != result_num_occurrences:
                     dicts_equal = False
-                    print(f'Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}')
-                    raise AssertionError('Dictionaries not equal')
+                    print(
+                        f"Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}"
+                    )
+                    raise AssertionError("Dictionaries not equal")
                 elif len(expected_probs) != len(result_probs):
-                    print(f'Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}')
-                    raise AssertionError('Dictionaries not equal')
-                elif not all(abs(a - b) < 1e-8 for a, b in zip(expected_probs, result_probs)):
-                    print(f'Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}')
-                    raise AssertionError('Dictionaries not equal')
+                    print(
+                        f"Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}"
+                    )
+                    raise AssertionError("Dictionaries not equal")
+                elif not all(
+                    abs(a - b) < 1e-8 for a, b in zip(expected_probs, result_probs)
+                ):
+                    print(
+                        f"Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}"
+                    )
+                    raise AssertionError("Dictionaries not equal")
     except:
         dicts_equal = False
 
-    assert dicts_equal, message 
+    assert dicts_equal, message
 
 
-def test_bin_probabilities_good_input_frequency_1d_ypred(bin_probabilities_good_input_frequency_1d_y_pred, expected_get_equal_frequency_bins_good_input):
+def test_bin_probabilities_good_input_frequency_1d_ypred(
+    bin_probabilities_good_input_frequency_1d_y_pred,
+    expected_get_equal_frequency_bins_good_input,
+):
     result = bin_probabilities(*bin_probabilities_good_input_frequency_1d_y_pred)
     expected = expected_get_equal_frequency_bins_good_input
     message = f"bin_probabilities returned {result}, instead of {expected}"
     dicts_equal = True
     try:
         for class_key in expected:
             expected_class_level_dict = expected[class_key]
             result_class_level_dict = result[class_key]
             for bin_key in expected_class_level_dict:
                 expected_bin_level_dict = expected_class_level_dict[bin_key]
                 result_bin_level_dict = result_class_level_dict[bin_key]
-                expected_probs = expected_bin_level_dict['probs']
-                result_probs = result_bin_level_dict['probs']
-                expected_num_occurrences = expected_bin_level_dict['num_occurrences']
-                result_num_occurrences = result_bin_level_dict['num_occurrences']
+                expected_probs = expected_bin_level_dict["probs"]
+                result_probs = result_bin_level_dict["probs"]
+                expected_num_occurrences = expected_bin_level_dict["num_occurrences"]
+                result_num_occurrences = result_bin_level_dict["num_occurrences"]
 
                 if expected_num_occurrences != result_num_occurrences:
                     dicts_equal = False
-                    print(f'Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}')
-                    raise AssertionError('Dictionaries not equal')
+                    print(
+                        f"Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}"
+                    )
+                    raise AssertionError("Dictionaries not equal")
                 elif len(expected_probs) != len(result_probs):
-                    print(f'Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}')
-                    raise AssertionError('Dictionaries not equal')
-                elif not all(abs(a - b) < 1e-8 for a, b in zip(expected_probs, result_probs)):
-                    print(f'Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}')
-                    raise AssertionError('Dictionaries not equal')
+                    print(
+                        f"Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}"
+                    )
+                    raise AssertionError("Dictionaries not equal")
+                elif not all(
+                    abs(a - b) < 1e-8 for a, b in zip(expected_probs, result_probs)
+                ):
+                    print(
+                        f"Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}"
+                    )
+                    raise AssertionError("Dictionaries not equal")
     except:
         dicts_equal = False
 
-    assert dicts_equal, message 
+    assert dicts_equal, message
 
 
-def test_bin_probabilities_good_input_frequency_2d_ypred(bin_probabilities_good_input_frequency_2d_y_pred, expected_get_equal_frequency_bins_good_input):
+def test_bin_probabilities_good_input_frequency_2d_ypred(
+    bin_probabilities_good_input_frequency_2d_y_pred,
+    expected_get_equal_frequency_bins_good_input,
+):
     result = bin_probabilities(*bin_probabilities_good_input_frequency_2d_y_pred)
     expected = expected_get_equal_frequency_bins_good_input
     message = f"bin_probabilities returned {result}, instead of {expected}"
     dicts_equal = True
     try:
         for class_key in expected:
             expected_class_level_dict = expected[class_key]
             result_class_level_dict = result[class_key]
             for bin_key in expected_class_level_dict:
                 expected_bin_level_dict = expected_class_level_dict[bin_key]
                 result_bin_level_dict = result_class_level_dict[bin_key]
-                expected_probs = expected_bin_level_dict['probs']
-                result_probs = result_bin_level_dict['probs']
-                expected_num_occurrences = expected_bin_level_dict['num_occurrences']
-                result_num_occurrences = result_bin_level_dict['num_occurrences']
+                expected_probs = expected_bin_level_dict["probs"]
+                result_probs = result_bin_level_dict["probs"]
+                expected_num_occurrences = expected_bin_level_dict["num_occurrences"]
+                result_num_occurrences = result_bin_level_dict["num_occurrences"]
 
                 if expected_num_occurrences != result_num_occurrences:
                     dicts_equal = False
-                    print(f'Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}')
-                    raise AssertionError('Dictionaries not equal')
+                    print(
+                        f"Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}"
+                    )
+                    raise AssertionError("Dictionaries not equal")
                 elif len(expected_probs) != len(result_probs):
-                    print(f'Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}')
-                    raise AssertionError('Dictionaries not equal')
-                elif not all(abs(a - b) < 1e-8 for a, b in zip(expected_probs, result_probs)):
-                    print(f'Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}')
-                    raise AssertionError('Dictionaries not equal')
+                    print(
+                        f"Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}"
+                    )
+                    raise AssertionError("Dictionaries not equal")
+                elif not all(
+                    abs(a - b) < 1e-8 for a, b in zip(expected_probs, result_probs)
+                ):
+                    print(
+                        f"Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}"
+                    )
+                    raise AssertionError("Dictionaries not equal")
     except:
         dicts_equal = False
 
     assert dicts_equal, message
 
-    
-def test_get_equal_frequency_bins_non_integer_freq(get_equal_frequency_bins_non_integer_freq, expected_get_equal_frequency_bins_non_integer_freq):
+
+def test_get_equal_frequency_bins_non_integer_freq(
+    get_equal_frequency_bins_non_integer_freq,
+    expected_get_equal_frequency_bins_non_integer_freq,
+):
     result = _get_equal_frequency_bins(*get_equal_frequency_bins_non_integer_freq)
     expected = expected_get_equal_frequency_bins_non_integer_freq
 
     message = f"Bins do not match. Returned {result} instead of {expected}."
 
     dicts_equal = True
     try:
         for class_key in expected:
             expected_class_level_dict = expected[class_key]
             result_class_level_dict = result[class_key]
             for bin_key in expected_class_level_dict:
                 expected_bin_level_dict = expected_class_level_dict[bin_key]
                 result_bin_level_dict = result_class_level_dict[bin_key]
-                expected_probs = expected_bin_level_dict['probs']
-                result_probs = result_bin_level_dict['probs']
-                expected_num_occurrences = expected_bin_level_dict['num_occurrences']
-                result_num_occurrences = result_bin_level_dict['num_occurrences']
+                expected_probs = expected_bin_level_dict["probs"]
+                result_probs = result_bin_level_dict["probs"]
+                expected_num_occurrences = expected_bin_level_dict["num_occurrences"]
+                result_num_occurrences = result_bin_level_dict["num_occurrences"]
 
                 if expected_num_occurrences != result_num_occurrences:
                     dicts_equal = False
-                    print(f'Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}')
-                    raise AssertionError('Dictionaries not equal')
+                    print(
+                        f"Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}"
+                    )
+                    raise AssertionError("Dictionaries not equal")
                 elif len(expected_probs) != len(result_probs):
-                    print(f'Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}')
-                    raise AssertionError('Dictionaries not equal')
-                elif not all(abs(a - b) < 1e-8 for a, b in zip(expected_probs, result_probs)):
-                    print(f'Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}')
-                    raise AssertionError('Dictionaries not equal')
+                    print(
+                        f"Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}"
+                    )
+                    raise AssertionError("Dictionaries not equal")
+                elif not all(
+                    abs(a - b) < 1e-8 for a, b in zip(expected_probs, result_probs)
+                ):
+                    print(
+                        f"Class: {class_key}, bin: {bin_key}, expected num_occurrences: {expected_num_occurrences}, result num_occurrences: {result_num_occurrences}"
+                    )
+                    raise AssertionError("Dictionaries not equal")
     except:
         dicts_equal = False
 
     assert dicts_equal, message
 
+
 def test_bin_probabilities_y_pred_greater_than_1(get_bins_y_pred_greater_than_1_input):
     """
     We expect an error to be raised as the input is bad.
     """
     with pytest.raises(ValueError):
         bin_probabilities(*get_bins_y_pred_greater_than_1_input)
-    
+
+
 def test_bin_probabilities_y_pred_less_than_0(get_bins_y_pred_less_than_0_input):
     """
     We expect an error to be raised as the input is bad.
     """
     with pytest.raises(ValueError):
         bin_probabilities(*get_bins_y_pred_less_than_0_input)
 
+
 def test_bin_probabilities_y_pred_3_dimensional(get_bins_y_pred_3_dimensional_input):
     """
     We expect an error to be raised as the input is bad.
     """
     with pytest.raises(ValueError):
-        bin_probabilities(*get_bins_y_pred_3_dimensional_input)    
+        bin_probabilities(*get_bins_y_pred_3_dimensional_input)
+
 
 def test_bin_probabilities_y_true_fractional(get_bins_y_true_fractional_input):
     """
     We expect an error to be raised as the input is bad.
     """
     with pytest.raises(ValueError):
         bin_probabilities(*get_bins_y_true_fractional_input)
 
+
 def test_bin_probabilities_negative_y_true(get_bins_negative_y_true_input):
     """
     We expect an error to be raised as the input is bad.
     """
     with pytest.raises(ValueError):
         bin_probabilities(*get_bins_negative_y_true_input)
 
 
 def test_reshape_y_pred(_reshape_y_pred_input, _reshape_y_pred_expected):
     expected = _reshape_y_pred_expected
     result = _reshape_y_pred(_reshape_y_pred_input)
-    assert np.allclose(result, expected), f'_reshape_y_pred returned {result} instead of {expected}.'
+    assert np.allclose(
+        result, expected
+    ), f"_reshape_y_pred returned {result} instead of {expected}."
+
 
 def test_get_bin_weight(_get_bin_weight_input, _get_bin_weight_expected):
     bin, num_samples = _get_bin_weight_input
     result = _get_bin_weight(bin, num_samples)
     expected = _get_bin_weight_expected
-    assert result == expected, f'_get_bin_weight returned {result} instead of {expected}.'
+    assert (
+        result == expected
+    ), f"_get_bin_weight returned {result} instead of {expected}."
+
 
 def test_sum_occurrences(_sum_occurrences_input, _sum_occurrences_expected):
     result = _sum_occurrences(*_sum_occurrences_input)
     expected = _sum_occurrences_expected
-    assert result == expected, f'_sum_occurrences returned {result} instead of {expected}.'
+    assert (
+        result == expected
+    ), f"_sum_occurrences returned {result} instead of {expected}."
+
 
-def test_forward_fill_equal_frequency_bins(_forward_fill_equal_frequency_bins_input, _forward_fill_equal_frequency_bins_expected):
-    result = _forward_fill_equal_frequency_bins(*_forward_fill_equal_frequency_bins_input)
+def test_forward_fill_equal_frequency_bins(
+    _forward_fill_equal_frequency_bins_input,
+    _forward_fill_equal_frequency_bins_expected,
+):
+    result = _forward_fill_equal_frequency_bins(
+        *_forward_fill_equal_frequency_bins_input
+    )
     expected = _forward_fill_equal_frequency_bins_expected
-    assert result == expected, f'_forward_fill_equal_frequency_bins returned {result} instead of {expected}.'
+    assert (
+        result == expected
+    ), f"_forward_fill_equal_frequency_bins returned {result} instead of {expected}."
 
-def test_back_fill_equal_frequency_bins(_back_fill_equal_frequency_bins_input, _back_fill_equal_frequency_bins_expected):
+
+def test_back_fill_equal_frequency_bins(
+    _back_fill_equal_frequency_bins_input, _back_fill_equal_frequency_bins_expected
+):
     result = _back_fill_equal_frequency_bins(*_back_fill_equal_frequency_bins_input)
     expected = _back_fill_equal_frequency_bins_expected
-    assert result == expected, f'_back_fill_equal_frequency_bins returned {result} instead of {expected}.'
+    assert (
+        result == expected
+    ), f"_back_fill_equal_frequency_bins returned {result} instead of {expected}."
+
 
-def test_get_classwise_bin_weights(get_classwise_bin_weights_input, get_classwise_bin_weights_expected):
-    result = get_classwise_bin_weights(*get_classwise_bin_weights_input)
+def test_get_classwise_bin_weights(
+    get_classwise_bin_weights_input, get_classwise_bin_weights_expected
+):
+    result = get_classwise_bin_weights(get_classwise_bin_weights_input)
     expected = get_classwise_bin_weights_expected
-    assert np.allclose(result, expected), f'get_classwise_bin_weights returned {result} instead of {expected}.'
+    assert np.allclose(
+        result, expected
+    ), f"get_classwise_bin_weights returned {result} instead of {expected}."
+
+
+def test_get_classwise_bin_weights_bad_input(get_classwise_bin_weights_bad_input):
+    with pytest.raises(AssertionError):
+        result = get_classwise_bin_weights(get_classwise_bin_weights_bad_input)
```

