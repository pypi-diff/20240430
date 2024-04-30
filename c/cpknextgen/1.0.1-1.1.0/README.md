# Comparing `tmp/cpknextgen-1.0.1.tar.gz` & `tmp/cpknextgen-1.1.0.tar.gz`

## Comparing `cpknextgen-1.0.1.tar` & `cpknextgen-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/requirements-test.txt
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/requirements.txt
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/tox.ini
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/src/cpknextgen/__init__.py
--rw-r--r--   0        0        0    18885 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/src/cpknextgen/__main__.py
--rw-r--r--   0        0        0     7302 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/src/cpknextgen/capability_index.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/src/cpknextgen/custom_exceptions.py
--rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/src/cpknextgen/graphics.py
--rw-r--r--   0        0        0    15119 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/src/cpknextgen/transformation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/src/cpknextgen/normal_mixture/__init__.py
--rw-r--r--   0        0        0     8355 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/src/cpknextgen/normal_mixture/inference.py
--rw-r--r--   0        0        0    14956 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/src/cpknextgen/normal_mixture/parameters_estimate.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/tests/capability_index_test.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/tests/utils.py
--rw-r--r--   0        0        0  1119638 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/tests/test_data/test_data.json
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/LICENSE
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/README.md
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 cpknextgen-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/requirements-test.txt
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/requirements.txt
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/tox.ini
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/src/cpknextgen/__init__.py
+-rw-r--r--   0        0        0    18957 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/src/cpknextgen/__main__.py
+-rw-r--r--   0        0        0     9039 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/src/cpknextgen/capability_index.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/src/cpknextgen/custom_exceptions.py
+-rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/src/cpknextgen/graphics.py
+-rw-r--r--   0        0        0    14130 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/src/cpknextgen/transformation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/src/cpknextgen/normal_mixture/__init__.py
+-rw-r--r--   0        0        0     8355 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/src/cpknextgen/normal_mixture/inference.py
+-rw-r--r--   0        0        0    14956 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/src/cpknextgen/normal_mixture/parameters_estimate.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/tests/capability_index_test.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/tests/utils.py
+-rw-r--r--   0        0        0  1119638 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/tests/test_data/test_data.json
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/README.md
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 cpknextgen-1.1.0/PKG-INFO
```

### Comparing `cpknextgen-1.0.1/CONTRIBUTING.md` & `cpknextgen-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cpknextgen-1.0.1/requirements-test.txt` & `cpknextgen-1.1.0/requirements-test.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,41 +4,41 @@
 #
 #    pip-compile --extra=test --output-file=requirements-test.txt pyproject.toml
 #
 colorama==0.4.6
     # via pytest
 iniconfig==2.0.0
     # via pytest
-joblib==1.3.1
+joblib==1.4.0
     # via scikit-learn
-llvmlite==0.40.1
+llvmlite==0.42.0
     # via numba
-numba==0.57.1
+numba==0.59.1
     # via cpknextgen (pyproject.toml)
-numpy==1.24.4
+numpy==1.26.4
     # via
     #   cpknextgen (pyproject.toml)
     #   numba
     #   scikit-learn
     #   scipy
-packaging==23.1
+packaging==24.0
     # via
     #   pytest
     #   pytest-sugar
-pluggy==1.2.0
+pluggy==1.5.0
     # via pytest
-pytest==7.4.0
+pytest==8.2.0
     # via
     #   cpknextgen (pyproject.toml)
     #   pytest-sugar
-pytest-sugar==0.9.7
+pytest-sugar==1.0.0
     # via cpknextgen (pyproject.toml)
-scikit-learn==1.3.0
+scikit-learn==1.4.2
     # via cpknextgen (pyproject.toml)
-scipy==1.11.1
+scipy==1.13.0
     # via
     #   cpknextgen (pyproject.toml)
     #   scikit-learn
-termcolor==2.3.0
+termcolor==2.4.0
     # via pytest-sugar
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
```

### Comparing `cpknextgen-1.0.1/requirements.txt` & `cpknextgen-1.1.0/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --output-file=requirements.txt pyproject.toml
 #
-joblib==1.3.1
+joblib==1.4.0
     # via scikit-learn
-llvmlite==0.40.1
+llvmlite==0.42.0
     # via numba
-numba==0.57.1
+numba==0.59.1
     # via cpknextgen (pyproject.toml)
-numpy==1.24.4
+numpy==1.26.4
     # via
     #   cpknextgen (pyproject.toml)
     #   numba
     #   scikit-learn
     #   scipy
-scikit-learn==1.3.0
+scikit-learn==1.4.2
     # via cpknextgen (pyproject.toml)
-scipy==1.11.1
+scipy==1.13.0
     # via
     #   cpknextgen (pyproject.toml)
     #   scikit-learn
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
```

### Comparing `cpknextgen-1.0.1/tox.ini` & `cpknextgen-1.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `cpknextgen-1.0.1/.github/workflows/release.yml` & `cpknextgen-1.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `cpknextgen-1.0.1/.github/workflows/test.yml` & `cpknextgen-1.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cpknextgen-1.0.1/src/cpknextgen/__main__.py` & `cpknextgen-1.1.0/src/cpknextgen/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,44 +288,44 @@
     point_mixture.estimate_quantiles()
 
     # if enough values are found at the extreme boundaries, use them instead of the quantile estimates
     if point_mixture.low_quantile_samples in boundary_data:
         point_process_low = point_mixture.low_quantile_samples
         sample_process_low = mixtures.low_quantile_samples
     else:
-        point_process_low = t.do_inverse_transform(point_mixture.low_quantile_samples)
-        sample_process_low = t.do_inverse_transform(mixtures.low_quantile_samples)
+        point_process_low = t.complete_transformation_inverse(point_mixture.low_quantile_samples)
+        sample_process_low = t.complete_transformation_inverse(mixtures.low_quantile_samples)
 
     if point_mixture.high_quantile_samples in boundary_data:
         point_process_high = point_mixture.high_quantile_samples
         sample_process_high = mixtures.high_quantile_samples
     else:
-        point_process_high = t.do_inverse_transform(point_mixture.high_quantile_samples)
-        sample_process_high = t.do_inverse_transform(mixtures.high_quantile_samples)
+        point_process_high = t.complete_transformation_inverse(point_mixture.high_quantile_samples)
+        sample_process_high = t.complete_transformation_inverse(mixtures.high_quantile_samples)
 
     if point_mixture.median_samples in boundary_data:
         point_process_center = point_mixture.median_samples
         sample_process_center = mixtures.median_samples
     else:
-        point_process_center = t.do_inverse_transform(point_mixture.median_samples)
-        sample_process_center = t.do_inverse_transform(mixtures.median_samples)
+        point_process_center = t.complete_transformation_inverse(point_mixture.median_samples)
+        sample_process_center = t.complete_transformation_inverse(mixtures.median_samples)
 
     ProcessStats.confidence = confidence
 
     sample_process_low, sample_process_center, sample_process_high, point_process_low, point_process_center, \
         point_process_high = small_infinity_handling(point_process_low, point_process_center, point_process_high,
                                                      sample_process_low, sample_process_center, sample_process_high,
                                                      data_boundaries)
 
     evaluation_result.capability_index = CapabilityIndex(
         process_low=ProcessStats(sample=sample_process_low, point=point_process_low),
         process_high=ProcessStats(sample=sample_process_high, point=point_process_high),
         process_center=ProcessStats(sample=sample_process_center, point=point_process_center),
-        specification_lower=t.lower_specification,
-        specification_upper=t.upper_specification,
+        specification_lower=_specification_limits[0],
+        specification_upper=_specification_limits[1],
         lower_boundary=data_boundaries[0],
         upper_boundary=data_boundaries[1])
 
     evaluation_result.graphics = get_results_graphics(data, t, mixtures, point_mixture, boundary_probabilities,
                                                       t.upper_boundary, t.lower_boundary, confidence=confidence)
     evaluation_result.boundary_occurrences = boundary_probabilities
```

### Comparing `cpknextgen-1.0.1/src/cpknextgen/capability_index.py` & `cpknextgen-1.1.0/src/cpknextgen/capability_index.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         EXTREMES = "Non-Standard Evaluation: Extremes as specification limits"
 
     class Cpk:
         STANDARD = "Standard evaluation"
         LOWER_MISSING = "Evaluation to Upper Specification only, c_pk = c_pk_upper"
         UPPER_MISSING = "Evaluation to Lower Specification only, c_pk = c_pk_lower"
         SPECIFICATIONS_MISSING = "Upper and Lower specifications missing"
+        EXTREMES = "Non-Standard Evaluation: Extremes as specification limits"
 
 
 class ProcessStats:
     """
     Container for results of capability index calculations
 
     ## Instance attributes:
@@ -83,14 +84,17 @@
         self.process_high = process_high
         self.process_center = process_center
         self.specification_lower = specification_lower
         self.specification_upper = specification_upper
         self.upper_boundary = upper_boundary
         self.lower_boundary = lower_boundary
 
+        self.standard_evaluation_cp = None
+        self.standard_evaluation_cpk = None
+
         self.cp = ProcessStats()
         self.cp_type = ""
         self.cpk = ProcessStats()
         self.cpk_type = ""
 
         if process_high is not None and process_high.point is not None and \
                 process_low is not None and process_low.point is not None:
@@ -100,44 +104,66 @@
             return
 
         self._cpk_upper = None
         self._cpk_lower = None
 
         if None not in (specification_lower, specification_upper):
             self.cp, self.cp_type, self.cpk, self.cpk_type = self._standard()
+            self.standard_evaluation_cp = True
+            self.standard_evaluation_cpk = True
 
         elif specification_lower is None and specification_upper is not None:
             self.cp, self.cp_type, self.cpk, self.cpk_type = self._lower_specification_missing()
+            self.standard_evaluation_cp = False
+            self.standard_evaluation_cpk = True
 
         elif specification_lower is not None and specification_upper is None:
             self.cp, self.cp_type, self.cpk, self.cpk_type = self._upper_specification_missing()
+            self.standard_evaluation_cp = False
+            self.standard_evaluation_cpk = True
+
         else:
             self.cp, self.cp_type, self.cpk, self.cpk_type = self._specifications_missing()
+            self.standard_evaluation_cp = False
+            self.standard_evaluation_cpk = False
 
     @property
     def cpk_upper(self):
         if self._cpk_upper is None:
             if None not in [self.specification_upper, self.process_center, self.process_high]:
                 self._cpk_upper = ProcessStats(
                     sample=(self.specification_upper - self.process_center.sample) / (
                             self.process_high.sample - self.process_center.sample),
                     point=(self.specification_upper - self.process_center.point) / (
                             self.process_high.point - self.process_center.point))
+            elif None not in [self.upper_boundary, self.process_center, self.process_high]:
+                self._cpk_upper = ProcessStats(
+                    sample=(self.upper_boundary - self.process_center.sample) / (
+                            self.process_high.sample - self.process_center.sample),
+                    point=(self.upper_boundary - self.process_center.point) / (
+                            self.process_high.point - self.process_center.point))
         return self._cpk_upper
 
     @property
     def cpk_lower(self):
         if self._cpk_lower is None:
             if None not in [self.specification_lower, self.process_center, self.process_low]:
                 self._cpk_lower = ProcessStats(
                     sample=(self.process_center.sample - self.specification_lower) /
                            (self.process_center.sample - self.process_low.sample),
                     point=(self.process_center.point - self.specification_lower) /
                     (self.process_center.point - self.process_low.point)
                 )
+            elif None not in [self.lower_boundary, self.process_center, self.process_low]:
+                self._cpk_lower = ProcessStats(
+                    sample=(self.process_center.sample - self.lower_boundary) /
+                           (self.process_center.sample - self.process_low.sample),
+                    point=(self.process_center.point - self.lower_boundary) /
+                    (self.process_center.point - self.process_low.point)
+                )
         return self._cpk_lower
 
     def _get_cp(self, upper_limit=None, lower_limit=None) -> ProcessStats:
         result = ProcessStats(sample=(upper_limit - lower_limit) / self.process_width.sample,
                               point=(upper_limit - lower_limit) / self.process_width.point)
         return result
 
@@ -165,15 +191,19 @@
             cp = self._get_cp(upper_limit=self.upper_boundary, lower_limit=self.specification_lower)
             return cp, ResultTypes.Cp.UPPER_EXTREME, cpk, cpk_type
         else:
             cp = ProcessStats()
             return cp, ResultTypes.Cp.UPPER_MISSING, cpk, cpk_type
 
     def _specifications_missing(self):
-        cpk = ProcessStats()
-        cpk_type = ResultTypes.Cpk.SPECIFICATIONS_MISSING
         if None not in (self.lower_boundary, self.upper_boundary):
             cp = self._get_cp(lower_limit=self.lower_boundary, upper_limit=self.upper_boundary)
+            cpk = ProcessStats(sample=np.minimum(self.cpk_lower.sample, self.cpk_upper.sample),
+                               point=np.minimum(self.cpk_lower.point, self.cpk_upper.point))
+            cpk_type = ResultTypes.Cpk.EXTREMES
             return cp, ResultTypes.Cp.EXTREMES, cpk, cpk_type
         else:
             cp = ProcessStats()
+            cpk = ProcessStats()
+            cpk_type = ResultTypes.Cpk.SPECIFICATIONS_MISSING
+
             return cp, ResultTypes.Cp.SPECIFICATIONS_MISSING, cpk, cpk_type
```

### Comparing `cpknextgen-1.0.1/src/cpknextgen/graphics.py` & `cpknextgen-1.1.0/src/cpknextgen/graphics.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     point_cdf: dict = field(default_factory=dict)
     lower_sample_cdf: dict = field(default_factory=dict)
     upper_sample_cdf: dict = field(default_factory=dict)
     point_density: dict = field(default_factory=dict)
 
 
 def get_results_graphics(raw_measured_data,
-                         trans_instance: Transformation,
+                         transformation: Transformation,
                          mixtures: MixtureDistributions,
                          point_mixture: MixtureDistributions,
                          boundary_probabilities: np.ndarray,
                          upper_boundary: float,
                          lower_boundary: float,
                          confidence: float):
     """
@@ -65,18 +65,18 @@
     # np.nanquantile ignores NaN
     mixture_model_cdf_samples_x_low = np.nanquantile(mixtures.percentile_samples, (1 - confidence) / 2, axis=0)
     mixture_model_cdf_samples_x_median = np.nanquantile(mixtures.percentile_samples, 0.5, axis=0)
     mixture_model_cdf_samples_x_high = np.nanquantile(mixtures.percentile_samples, confidence + (1 - confidence) / 2,
                                                       axis=0)
 
     with np.errstate(invalid="ignore"):  # ignore "invalid value" warnings; result array can contain NaN
-        ecdf_lower_error = trans_instance.do_inverse_transform(mixture_model_cdf_samples_x_low)
-        median_sample_cdf = trans_instance.do_inverse_transform(mixture_model_cdf_samples_x_median)
-        ecdf_upper_error = trans_instance.do_inverse_transform(mixture_model_cdf_samples_x_high)
-        ecdf_point_error = trans_instance.do_inverse_transform(point_mixture.percentile_samples)
+        ecdf_lower_error = transformation.complete_transformation_inverse(mixture_model_cdf_samples_x_low)
+        median_sample_cdf = transformation.complete_transformation_inverse(mixture_model_cdf_samples_x_median)
+        ecdf_upper_error = transformation.complete_transformation_inverse(mixture_model_cdf_samples_x_high)
+        ecdf_point_error = transformation.complete_transformation_inverse(point_mixture.percentile_samples)
 
     grid_to_plot = mixtures.z_grid.copy()
     median_sample_cdf_to_plot = median_sample_cdf.copy()
     ecdf_lower_error_to_plot = ecdf_lower_error.copy()
     ecdf_upper_error_to_plot = ecdf_upper_error.copy()
     ecdf_point_error_to_plot = ecdf_point_error.copy().reshape(-1)
 
@@ -104,43 +104,43 @@
     graphics_result.point_cdf = dict(x=ecdf_point_error_to_plot, y=grid_to_plot)
 
     # density calculation
     lower_bound_estimated = np.min(median_sample_cdf_to_plot)
     upper_bound_estimated = np.max(median_sample_cdf_to_plot)
 
     how_many_points = 202
-    if trans_instance.upper_boundary is not None and trans_instance.lower_boundary is not None:
-        y = trans_instance.do_transform(
-            np.linspace(trans_instance.lower_boundary, trans_instance.upper_boundary,
+    if transformation.upper_boundary is not None and transformation.lower_boundary is not None:
+        y = transformation.complete_transformation(
+            np.linspace(transformation.lower_boundary, transformation.upper_boundary,
                         how_many_points)[1:-1])
-    elif trans_instance.upper_boundary is not None:
-        y = trans_instance.do_transform(np.linspace(lower_bound_estimated,
-                                                    trans_instance.upper_boundary, how_many_points)[1:-1])
-    elif trans_instance.lower_boundary is not None:
-        y = trans_instance.do_transform(
-            np.linspace(trans_instance.lower_boundary, upper_bound_estimated,
+    elif transformation.upper_boundary is not None:
+        y = transformation.complete_transformation(np.linspace(lower_bound_estimated,
+                                                               transformation.upper_boundary, how_many_points)[1:-1])
+    elif transformation.lower_boundary is not None:
+        y = transformation.complete_transformation(
+            np.linspace(transformation.lower_boundary, upper_bound_estimated,
                         how_many_points)[1:-1])
     else:
-        y = trans_instance.do_transform(
+        y = transformation.complete_transformation(
             np.linspace(lower_bound_estimated, upper_bound_estimated, how_many_points)[1:-1])
 
     result1 = mixture_of_normals_density(point_mixture.weights_samples, point_mixture.means_samples,
                                          point_mixture.scales_samples, y)
 
-    y2 = trans_instance.do_inverse_transform(y, order=1)
-    result2 = trans_instance.relative_to_specification_derivative(y2)
+    y2 = transformation.complete_transformation_inverse(y, order=1)
+    result2 = transformation.normalisation_transformation_derivative(y2)
 
-    y3 = trans_instance.do_inverse_transform(y, order=2)
-    result3 = trans_instance.yeojohnson.derivative_transform(y3)
+    y3 = transformation.complete_transformation_inverse(y, order=2)
+    result3 = transformation.yeojohnson.derivative_transform(y3)
 
-    y4 = trans_instance.do_inverse_transform(y, order=3)
-    result4 = trans_instance.relative_to_specification_derivative(y4, order=1)
+    y4 = transformation.complete_transformation_inverse(y, order=3)
+    result4 = transformation.normalisation_transformation_derivative(y4, order=1)
 
-    original_axis_x = trans_instance.do_inverse_transform(y, order=4)
-    result5 = trans_instance.relative_to_boundaries_derivative(original_axis_x)
+    original_axis_x = transformation.complete_transformation_inverse(y, order=4)
+    result5 = transformation.boundaries_transformation_derivative(original_axis_x)
 
     density_y = result1 * (result2 * result3 * result4 * result5)
 
     # When some datapoints are on extreme boundaries, the density needs to be rescaled
     if boundary_probabilities[0] is not None and boundary_probabilities[1] is not None:
         normalising_coefficient = 1 - boundary_probabilities[0] - boundary_probabilities[1]
     elif boundary_probabilities[0] is not None:
```

### Comparing `cpknextgen-1.0.1/src/cpknextgen/transformation.py` & `cpknextgen-1.1.0/src/cpknextgen/transformation.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,23 +66,23 @@
         """
         x_tiny = np.finfo(np.float64).tiny
 
         def _neg_log_likelihood(lmbda):
             """Return the negative log likelihood of the observed data x as a
             function of lambda."""
 
-            x_trans = self.transform(x, lmbda)
+            x_transformed = self.transform(x, lmbda)
             n_samples = x.shape[0]
-            x_trans_var = x_trans.var()
+            x_transfsormed_var = x_transformed.var()
 
             # Reject transformed data that would raise a RuntimeWarning in np.log
-            if x_trans_var < x_tiny:
+            if x_transfsormed_var < x_tiny:
                 return np.inf
 
-            log_var = np.log(x_trans_var)
+            log_var = np.log(x_transfsormed_var)
             loglike = -n_samples / 2 * log_var
             loglike += (lmbda - 1) * (np.sign(x) * np.log1p(np.abs(x))).sum()
 
             return -loglike
 
         # the computation of lambda is influenced by NaNs so we need to
         # get rid of them
@@ -170,182 +170,164 @@
 
         self.data = jitter_data(data, lower_boundary, upper_boundary, kernel=jitter_kernel, resolution=resolution)
 
         self.standard_computation = True
         self.lower_boundary = lower_boundary
         self.upper_boundary = upper_boundary
 
-        self.lower_specification = lower_specification_limit
-        self.upper_specification = upper_specification_limit
-
-        self.lower_boundary_data = None
-        self.upper_boundary_data = None
         self.len_of_data = len(self.data)
 
         self.upper_boundary_data = np.sum(self.data == self.upper_boundary)
         self.lower_boundary_data = np.sum(self.data == self.lower_boundary)
 
         self.boundaryless_data = self.data[self.data != self.upper_boundary]
         self.boundaryless_data = self.boundaryless_data[self.boundaryless_data != self.lower_boundary]
 
         if len(np.unique(self.boundaryless_data)) < 3 and jitter_kernel == 'no_jitter':
             raise InvalidDataError("More unique values are required to calculate capability indexes.")
 
-        self.lower_normalization_limit, self.upper_normalization_limit, self.standard_computation = self._check_limits(
+        self.normalization_limits, self.standard_computation = self._check_limits(
             self.boundaryless_data,
             lower_specification_limit,
             upper_specification_limit,
             limit_quantiles,
             lower_boundary,
             upper_boundary)
 
-        self.lower_normalization_limit_transformed = None
-        self.upper_normalization_limit_transformed = None
-
-        self.lower_boundary_transformed = None
-        self.upper_boundary_transformed = None
+        self.limits_to_boundaries = self.boundaries_transformation(self.normalization_limits)
+        data_to_boundaries = self.boundaries_transformation(self.boundaryless_data)
 
-        self.specification_to_boundaries = self.relative_to_boundaries(
-            np.array([self.lower_normalization_limit, self.upper_normalization_limit]))
+        limits_to_normalisation_1 = np.array([-1, 1])
+        data_normalisation_1 = self.normalisation_transformation(data_to_boundaries, order=1)
 
-        data_relative_to_boundaries = self.relative_to_boundaries(self.boundaryless_data)
-        data_to_specification_1 = self.relative_to_specification(data_relative_to_boundaries, order=1)
-        self.yeojohnson = YeoJohnson(data_to_specification_1)
+        self.yeojohnson = YeoJohnson(data_normalisation_1)
 
-        specifications_to_specification_1 = np.array([-1, 1])
-        self.lower_normalization_limit_transformed, self.upper_normalization_limit_transformed = self.yeojohnson.transform(
-            specifications_to_specification_1)
+        self.limits_to_yeo = self.yeojohnson.transform(limits_to_normalisation_1)
 
-        self.data_transformed = self.do_transform(self.boundaryless_data)
+        self.data_transformed = self.complete_transformation(self.boundaryless_data)
 
     @staticmethod
     def _check_limits(data, lower_specification_limit: float = None,
                       upper_specification_limit: float = None,
                       limit_quantiles: tuple = (),
                       lower_boundary: float = None,
                       upper_boundary: float = None) -> tuple:
         standard_computation = True
-        max_data = np.max(data)
-        min_data = np.min(data)
-        if upper_boundary is not None and upper_boundary < max_data:
+        if upper_boundary is not None and upper_boundary < np.max(data):
             raise InvalidDataError("User supplied upper boundary is less than maximum of data!")
-        if lower_boundary is not None and lower_boundary > min_data:
+        if lower_boundary is not None and lower_boundary > np.min(data):
             raise InvalidDataError("User supplied lower boundary is greater than minimum of data!")
         if len(limit_quantiles) != 2:
             limit_quantiles = (0.01, 0.99)
 
         lower_normalization_limit = np.quantile(data, limit_quantiles[
             0], method="inverted_cdf") if lower_specification_limit is None else lower_specification_limit
         upper_normalization_limit = np.quantile(data, limit_quantiles[
             1], method="inverted_cdf") if upper_specification_limit is None else upper_specification_limit
 
         if lower_normalization_limit >= upper_normalization_limit:
             standard_computation = False
             if len(np.unique(data)) > 1:
                 if lower_specification_limit is None:
                     if lower_boundary is None:
-                        lower_normalization_limit = np.min([lower_normalization_limit, upper_normalization_limit]) - np.min(
-                            np.diff(np.sort(np.unique(data))))
+                        lower_normalization_limit = (np.min([lower_normalization_limit, upper_normalization_limit]) -
+                                                     np.min(np.diff(np.sort(np.unique(data)))))
                     else:
-                        lower_normalization_limit = np.max([np.min([lower_normalization_limit, upper_normalization_limit]) - np.min(
-                            np.diff(np.sort(np.unique(data)))), lower_boundary])
+                        lower_normalization_limit = np.max([np.min([lower_normalization_limit, upper_normalization_limit]) -
+                                                            np.min(np.diff(np.sort(np.unique(data)))), lower_boundary])
                 if upper_specification_limit is None:
                     if upper_boundary is None:
-                        upper_normalization_limit = np.max([lower_normalization_limit, upper_normalization_limit]) + np.min(
-                            np.diff(np.sort(np.unique(data))))
+                        upper_normalization_limit = (np.max([lower_normalization_limit, upper_normalization_limit]) +
+                                                     np.min(np.diff(np.sort(np.unique(data)))))
                     else:
-                        upper_normalization_limit = np.min([np.max([lower_normalization_limit, upper_normalization_limit]) + np.min(
-                            np.diff(np.sort(np.unique(data)))), upper_boundary])
+                        upper_normalization_limit = np.min([np.max([lower_normalization_limit, upper_normalization_limit]) +
+                                                            np.min(np.diff(np.sort(np.unique(data)))), upper_boundary])
 
-        return lower_normalization_limit, upper_normalization_limit, standard_computation
+        return np.array([lower_normalization_limit, upper_normalization_limit]), standard_computation
 
-    def relative_to_boundaries(self, data, inverse=False):
-        max_bound = 30
+    def boundaries_transformation(self, data, inverse=False):
+        # maximum value to avoid overflow
+        absolute_bound = 30
         if self.lower_boundary is None and self.upper_boundary is None:
             return data
 
         elif self.lower_boundary is None:
             if not inverse:
                 return -np.log(- (data - self.upper_boundary))
             else:
-                data = np.maximum(data, -max_bound)
+                data = np.maximum(data, -absolute_bound)
                 return -np.exp(-data) + self.upper_boundary
 
         elif self.upper_boundary is None:
             if not inverse:
                 return np.log(data - self.lower_boundary)
             else:
-                data = np.minimum(data, max_bound)
+                data = np.minimum(data, absolute_bound)
                 return np.exp(data) + self.lower_boundary
         else:
             if not inverse:
                 scaled_data = (data - self.lower_boundary) / (self.upper_boundary - self.lower_boundary)
                 return np.log(scaled_data / (1 - scaled_data))
             else:
-                data = np.minimum(data, max_bound)
+                data = np.minimum(data, absolute_bound)
                 k = self.upper_boundary - self.lower_boundary
                 return self.lower_boundary + (np.exp(data) / (1 + np.exp(data)) * k)
 
-    def relative_to_boundaries_derivative(self, data):
+    def boundaries_transformation_derivative(self, data):
         if self.lower_boundary is None and self.upper_boundary is None:
             return np.ones_like(data)
 
         elif self.lower_boundary is None:
             return -1 / (data - self.upper_boundary)
 
         elif self.upper_boundary is None:
             return 1 / (data - self.lower_boundary)
         else:
             k = self.upper_boundary - self.lower_boundary
             return k / (data - self.lower_boundary) / (self.upper_boundary - data)
 
-    def relative_to_specification(self, data, inverse=False, order=2):
-        lower_normalization_limit_transformed = self.lower_normalization_limit_transformed
-        upper_normalization_limit_transformed = self.upper_normalization_limit_transformed
-
+    def normalisation_transformation(self, data, inverse=False, order=2):
         if order == 1:
-            lower_normalization_limit_transformed = self.specification_to_boundaries[0]
-            upper_normalization_limit_transformed = self.specification_to_boundaries[1]
+            normalization_limits = self.limits_to_boundaries
+        else:
+            normalization_limits = self.limits_to_yeo
 
-        if lower_normalization_limit_transformed is None or upper_normalization_limit_transformed is None:
+        if normalization_limits[0] is None or normalization_limits[1] is None:
             return data
 
-        _diff = upper_normalization_limit_transformed - lower_normalization_limit_transformed
+        _diff = normalization_limits[1] - normalization_limits[0]
         if not inverse:
-            return (2 * (data - lower_normalization_limit_transformed) / _diff) - 1
+            return (2 * (data - normalization_limits[0]) / _diff) - 1
         else:
-            return (data + 1) / 2 * _diff + lower_normalization_limit_transformed
-
-    def relative_to_specification_derivative(self, data, order=2):
-
-        lower_normalization_limit_transformed = self.lower_normalization_limit_transformed
-        upper_normalization_limit_transformed = self.upper_normalization_limit_transformed
+            return (data + 1) / 2 * _diff + normalization_limits[0]
 
+    def normalisation_transformation_derivative(self, data, order=2):
         if order == 1:
-            lower_normalization_limit_transformed = self.specification_to_boundaries[0]
-            upper_normalization_limit_transformed = self.specification_to_boundaries[1]
+            normalization_limits = self.limits_to_boundaries
+        else:
+            normalization_limits = self.limits_to_yeo
 
-        if lower_normalization_limit_transformed is None or upper_normalization_limit_transformed is None:
+        if normalization_limits[0] is None or normalization_limits[1] is None:
             return np.ones_like(data)
-        _diff = upper_normalization_limit_transformed - lower_normalization_limit_transformed
+        _diff = normalization_limits[1] - normalization_limits[0]
         return np.ones_like(data) * 2 / _diff
 
-    def do_transform(self, data):
-        data_extreme_bounds = self.relative_to_boundaries(data)
-        data_to_specification_1 = self.relative_to_specification(data_extreme_bounds, order=1)
-
-        yeo_johnson_data = self.yeojohnson.transform(data_to_specification_1)
-        data_to_specification_2 = self.relative_to_specification(yeo_johnson_data)
-        return data_to_specification_2
+    def complete_transformation(self, data):
+        data_to_boundaries = self.boundaries_transformation(data)
+        data_normalisation_1 = self.normalisation_transformation(data_to_boundaries, order=1)
+
+        data_to_yeo = self.yeojohnson.transform(data_normalisation_1)
+        data_normalisation_2 = self.normalisation_transformation(data_to_yeo)
+        return data_normalisation_2
 
-    def do_inverse_transform(self, data, order=4):
-        data_back_specification_2 = self.relative_to_specification(data, inverse=True)
+    def complete_transformation_inverse(self, data, order=4):
+        data_normalisation_2_inverse = self.normalisation_transformation(data, inverse=True)
         if order == 1:
-            return data_back_specification_2
-        data_back_yeo = self.yeojohnson.inverse(data_back_specification_2)
+            return data_normalisation_2_inverse
+        data_to_yeo_inverse = self.yeojohnson.inverse(data_normalisation_2_inverse)
         if order == 2:
-            return data_back_yeo
-        data_back_specification_1 = self.relative_to_specification(data_back_yeo, inverse=True, order=1)
+            return data_to_yeo_inverse
+        data_normalisation_1_inverse = self.normalisation_transformation(data_to_yeo_inverse, inverse=True, order=1)
         if order == 3:
-            return data_back_specification_1
-        data_back_extreme_bounds = self.relative_to_boundaries(data_back_specification_1, inverse=True)
-        return data_back_extreme_bounds
+            return data_normalisation_1_inverse
+        data_to_boundaries_inverse = self.boundaries_transformation(data_normalisation_1_inverse, inverse=True)
+        return data_to_boundaries_inverse
```

### Comparing `cpknextgen-1.0.1/src/cpknextgen/normal_mixture/inference.py` & `cpknextgen-1.1.0/src/cpknextgen/normal_mixture/inference.py`

 * *Files identical despite different names*

### Comparing `cpknextgen-1.0.1/src/cpknextgen/normal_mixture/parameters_estimate.py` & `cpknextgen-1.1.0/src/cpknextgen/normal_mixture/parameters_estimate.py`

 * *Files identical despite different names*

### Comparing `cpknextgen-1.0.1/tests/capability_index_test.py` & `cpknextgen-1.1.0/tests/capability_index_test.py`

 * *Files identical despite different names*

### Comparing `cpknextgen-1.0.1/tests/utils.py` & `cpknextgen-1.1.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cpknextgen-1.0.1/tests/test_data/test_data.json` & `cpknextgen-1.1.0/tests/test_data/test_data.json`

 * *Files identical despite different names*

### Comparing `cpknextgen-1.0.1/LICENSE` & `cpknextgen-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpknextgen-1.0.1/README.md` & `cpknextgen-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cpknextgen-1.0.1/pyproject.toml` & `cpknextgen-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpknextgen"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
 	{ name = "Stanislav Král", email = "stanislav.kral@diribet.cz" },
 	{ name = "Jaroslav Staněk", email = "jaroslav.stanek@diribet.cz" },
 	{ name = "Helena Paulasová", email = "helena.paulasova@diribet.cz" },
 	{ name = "Vlastimil Dolejš", email = "vlastimil.dolejs@diribet.cz" },
 ]
 description = "Cpk NextGen"
```

### Comparing `cpknextgen-1.0.1/PKG-INFO` & `cpknextgen-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cpknextgen
-Version: 1.0.1
+Version: 1.1.0
 Summary: Cpk NextGen
 Project-URL: Homepage, https://github.com/diribet/cpknextgen
 Project-URL: Issues, https://github.com/diribet/cpknextgen/issues
 Author-email: Stanislav Král <stanislav.kral@diribet.cz>, Jaroslav Staněk <jaroslav.stanek@diribet.cz>, Helena Paulasová <helena.paulasova@diribet.cz>, Vlastimil Dolejš <vlastimil.dolejs@diribet.cz>
 License: MIT License
 License-File: LICENSE
 Keywords: Cp,Cpk,Process capability
```

