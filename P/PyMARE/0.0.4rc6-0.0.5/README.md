# Comparing `tmp/PyMARE-0.0.4rc6.tar.gz` & `tmp/PyMARE-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMARE-0.0.4rc6.tar", last modified: Wed Apr 17 19:03:33 2024, max compression
+gzip compressed data, was "PyMARE-0.0.5.tar", last modified: Tue Apr 30 16:10:48 2024, max compression
```

## Comparing `PyMARE-0.0.4rc6.tar` & `PyMARE-0.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.082545 PyMARE-0.0.4rc6/PyMARE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-17 19:03:33.000000 PyMARE-0.0.4rc6/PyMARE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-17 19:03:33.000000 PyMARE-0.0.4rc6/PyMARE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:03:33.000000 PyMARE-0.0.4rc6/PyMARE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:03:33.000000 PyMARE-0.0.4rc6/PyMARE.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 19:03:33.000000 PyMARE-0.0.4rc6/PyMARE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 19:03:33.000000 PyMARE-0.0.4rc6/PyMARE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/pymare/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/pymare/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.082545 PyMARE-0.0.4rc6/pymare/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/datasets/metadat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/pymare/effectsize/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/effectsize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21695 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/effectsize/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/effectsize/expressions.json
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/effectsize/expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/pymare/estimators/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/estimators/combination.py
--rw-r--r--   0 runner    (1001) docker     (127)    23611 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/estimators/estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.082545 PyMARE-0.0.4rc6/pymare/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/pymare/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/resources/datasets/michael2013.json
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/resources/datasets/michael2013.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    22187 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    79886 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:10:48.262538 PyMARE-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-30 16:10:39.000000 PyMARE-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 16:10:39.000000 PyMARE-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-30 16:10:48.262538 PyMARE-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:10:48.258538 PyMARE-0.0.5/PyMARE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-30 16:10:48.000000 PyMARE-0.0.5/PyMARE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-30 16:10:48.000000 PyMARE-0.0.5/PyMARE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:10:48.000000 PyMARE-0.0.5/PyMARE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:10:48.000000 PyMARE-0.0.5/PyMARE.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-30 16:10:48.000000 PyMARE-0.0.5/PyMARE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 16:10:48.000000 PyMARE-0.0.5/PyMARE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-30 16:10:39.000000 PyMARE-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:10:48.262538 PyMARE-0.0.5/pymare/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-30 16:10:48.262538 PyMARE-0.0.5/pymare/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:10:48.262538 PyMARE-0.0.5/pymare/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/datasets/metadat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:10:48.262538 PyMARE-0.0.5/pymare/effectsize/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/effectsize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21695 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/effectsize/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/effectsize/expressions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/effectsize/expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:10:48.262538 PyMARE-0.0.5/pymare/estimators/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/estimators/combination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23611 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/estimators/estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:10:48.258538 PyMARE-0.0.5/pymare/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:10:48.262538 PyMARE-0.0.5/pymare/resources/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/resources/datasets/michael2013.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/resources/datasets/michael2013.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    22187 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pymare/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-30 16:10:39.000000 PyMARE-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-30 16:10:48.262538 PyMARE-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-30 16:10:39.000000 PyMARE-0.0.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79886 2024-04-30 16:10:39.000000 PyMARE-0.0.5/versioneer.py
```

### Comparing `PyMARE-0.0.4rc6/LICENSE` & `PyMARE-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/PKG-INFO` & `PyMARE-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMARE
-Version: 0.0.4rc6
+Version: 0.0.5
 Summary: PyMARE: Python Meta-Analysis & Regression Engine
 Home-page: https://github.com/neurostuff/PyMARE
 Author: PyMARE developers
 Author-email: tsalo006@fiu.edu
 Maintainer: Taylor Salo
 Maintainer-email: tsalo006@fiu.edu
 License: MIT
```

### Comparing `PyMARE-0.0.4rc6/PyMARE.egg-info/PKG-INFO` & `PyMARE-0.0.5/PyMARE.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMARE
-Version: 0.0.4rc6
+Version: 0.0.5
 Summary: PyMARE: Python Meta-Analysis & Regression Engine
 Home-page: https://github.com/neurostuff/PyMARE
 Author: PyMARE developers
 Author-email: tsalo006@fiu.edu
 Maintainer: Taylor Salo
 Maintainer-email: tsalo006@fiu.edu
 License: MIT
```

### Comparing `PyMARE-0.0.4rc6/PyMARE.egg-info/SOURCES.txt` & `PyMARE-0.0.5/PyMARE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/PyMARE.egg-info/requires.txt` & `PyMARE-0.0.5/PyMARE.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/README.md` & `PyMARE-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/pymare/__init__.py` & `PyMARE-0.0.5/pymare/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/pymare/core.py` & `PyMARE-0.0.5/pymare/core.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/pymare/datasets/metadat.py` & `PyMARE-0.0.5/pymare/datasets/metadat.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/pymare/effectsize/base.py` & `PyMARE-0.0.5/pymare/effectsize/base.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/pymare/effectsize/expressions.json` & `PyMARE-0.0.5/pymare/effectsize/expressions.json`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/pymare/effectsize/expressions.py` & `PyMARE-0.0.5/pymare/effectsize/expressions.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/pymare/estimators/__init__.py` & `PyMARE-0.0.5/pymare/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/pymare/estimators/combination.py` & `PyMARE-0.0.5/pymare/estimators/combination.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,28 +109,30 @@
     ----------
     .. footbibliography::
     """
 
     # Maps Dataset attributes onto fit() args; see BaseEstimator for details.
     _dataset_attr_map = {"z": "y", "w": "n", "g": "v"}
 
-    def _inflation_term(self, z, w, g):
+    def _inflation_term(self, z, w, g, corr=None):
         """Calculate the variance inflation term for each group.
 
         This term is used to adjust the variance of the combined z-score when
         multiple sample come from the same study.
 
         Parameters
         ----------
         z : :obj:`numpy.ndarray` of shape (n, d)
             Array of z-values.
         w : :obj:`numpy.ndarray` of shape (n, d)
             Array of weights.
         g : :obj:`numpy.ndarray` of shape (n, d)
             Array of group labels.
+        corr : :obj:`numpy.ndarray` of shape (n, n), optional
+            The correlation matrix of the z-values. If None, it will be calculated.
 
         Returns
         -------
         sigma : float
             The variance inflation term.
         """
         # Only center if the samples are not all the same, to prevent division by zero
@@ -153,34 +155,46 @@
 
             # For groups with only one sample the contribution to the summand is 0
             n_samples = len(group_indices)
             if n_samples < 2:
                 continue
 
             # Calculate the within group correlation matrix and sum the non-diagonal elements
-            corr = np.corrcoef(group_z, rowvar=True)
+            if corr is None:
+                if z.shape[1] < 2:
+                    raise ValueError("The number of features must be greater than 1.")
+                group_corr = np.corrcoef(group_z, rowvar=True)
+            else:
+                group_corr = corr[group_indices][:, group_indices]
+
             upper_indices = np.triu_indices(n_samples, k=1)
-            non_diag_corr = corr[upper_indices]
+            non_diag_corr = group_corr[upper_indices]
             w_i, w_j = weights[upper_indices[0]], weights[upper_indices[1]]
 
             sigma += (2 * w_i * w_j * non_diag_corr).sum()
 
         return sigma
 
-    def fit(self, z, w=None, g=None):
+    def fit(self, z, w=None, g=None, corr=None):
         """Fit the estimator to z-values, optionally with weights and groups."""
-        return super().fit(z, w=w, g=g)
+        return super().fit(z, w=w, g=g, corr=corr)
 
-    def p_value(self, z, w=None, g=None):
+    def p_value(self, z, w=None, g=None, corr=None):
         """Calculate p-values."""
         if w is None:
             w = np.ones_like(z)
 
+        if g is None and corr is not None:
+            warnings.warn("Correlation matrix provided without groups. Ignoring.")
+
+        if g is not None and corr is not None and g.shape[0] != corr.shape[0]:
+            raise ValueError("Group labels must have the same length as the correlation matrix.")
+
         # Calculate the variance inflation term, sum of non-diagonal elements of sigma.
-        sigma = self._inflation_term(z, w, g) if g is not None else 0
+        sigma = self._inflation_term(z, w, g, corr=corr) if g is not None else 0
 
         # The sum of diagonal elements of sigma is given by (w**2).sum(0).
         variance = (w**2).sum(0) + sigma
 
         cz = (z * w).sum(0) / np.sqrt(variance)
         return ss.norm.sf(cz)
```

### Comparing `PyMARE-0.0.4rc6/pymare/estimators/estimators.py` & `PyMARE-0.0.5/pymare/estimators/estimators.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/pymare/resources/datasets/michael2013.json` & `PyMARE-0.0.5/pymare/resources/datasets/michael2013.json`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/pymare/resources/datasets/michael2013.tsv` & `PyMARE-0.0.5/pymare/resources/datasets/michael2013.tsv`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/pymare/results.py` & `PyMARE-0.0.5/pymare/results.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/pymare/stats.py` & `PyMARE-0.0.5/pymare/stats.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/pymare/utils.py` & `PyMARE-0.0.5/pymare/utils.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/setup.cfg` & `PyMARE-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc6/versioneer.py` & `PyMARE-0.0.5/versioneer.py`

 * *Files identical despite different names*

