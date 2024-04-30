# Comparing `tmp/prophetverse-0.0.2.tar.gz` & `tmp/prophetverse-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophetverse-0.0.2.tar", max compression
+gzip compressed data, was "prophetverse-0.0.3a0.tar", max compression
```

## Comparing `prophetverse-0.0.2.tar` & `prophetverse-0.0.3a0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0    11357 2024-03-24 22:23:47.284971 prophetverse-0.0.2/LICENSE
--rw-r--r--   0        0        0     3328 2024-04-29 11:44:53.707810 prophetverse-0.0.2/README.md
--rw-r--r--   0        0        0      669 2024-04-29 16:40:37.232954 prophetverse-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       61 2024-04-28 22:01:32.488342 prophetverse-0.0.2/src/prophetverse/__init__.py
--rw-r--r--   0        0        0     1797 2024-04-28 22:01:32.488520 prophetverse-0.0.2/src/prophetverse/changepoint.py
--rw-r--r--   0        0        0    12748 2024-04-28 22:01:32.488733 prophetverse-0.0.2/src/prophetverse/effects.py
--rw-r--r--   0        0        0     6608 2024-04-28 22:01:32.488939 prophetverse-0.0.2/src/prophetverse/engine.py
--rw-r--r--   0        0        0       66 2024-04-28 22:01:32.489109 prophetverse-0.0.2/src/prophetverse/logger.py
--rw-r--r--   0        0        0      110 2024-04-28 22:01:32.489287 prophetverse-0.0.2/src/prophetverse/models/__init__.py
--rw-r--r--   0        0        0       25 2024-04-28 22:01:32.489463 prophetverse-0.0.2/src/prophetverse/models/multivariate_model/__init__.py
--rw-r--r--   0        0        0     2528 2024-04-28 22:01:32.489639 prophetverse-0.0.2/src/prophetverse/models/multivariate_model/_model.py
--rw-r--r--   0        0        0     1541 2024-04-28 22:01:32.489814 prophetverse-0.0.2/src/prophetverse/models/multivariate_model/changepoint.py
--rw-r--r--   0        0        0     5671 2024-04-28 22:01:32.489985 prophetverse-0.0.2/src/prophetverse/models/multivariate_model/multiindex.py
--rw-r--r--   0        0        0     1546 2024-04-28 22:01:32.490165 prophetverse-0.0.2/src/prophetverse/models/univariate_model.py
--rw-r--r--   0        0        0       77 2024-04-28 22:01:32.490361 prophetverse-0.0.2/src/prophetverse/sktime/__init__.py
--rw-r--r--   0        0        0     4364 2024-04-28 22:01:32.490543 prophetverse-0.0.2/src/prophetverse/sktime/_expand_column_per_level.py
--rw-r--r--   0        0        0    14564 2024-04-29 16:40:37.233591 prophetverse-0.0.2/src/prophetverse/sktime/base.py
--rw-r--r--   0        0        0    25882 2024-04-28 22:01:32.491238 prophetverse-0.0.2/src/prophetverse/sktime/multivariate.py
--rw-r--r--   0        0        0     2054 2024-04-29 00:54:41.355991 prophetverse-0.0.2/src/prophetverse/sktime/seasonality.py
--rw-r--r--   0        0        0    14192 2024-04-29 00:54:31.877365 prophetverse-0.0.2/src/prophetverse/sktime/univariate.py
--rw-r--r--   0        0        0     3813 2024-04-28 22:01:32.492061 prophetverse-0.0.2/src/prophetverse/utils/frame_to_array.py
--rw-r--r--   0        0        0     1206 2024-04-28 22:01:32.492245 prophetverse-0.0.2/src/prophetverse/utils/logistic.py
--rw-r--r--   0        0        0     1038 2024-04-28 22:01:32.492426 prophetverse-0.0.2/src/prophetverse/utils/multiindex.py
--rw-r--r--   0        0        0      396 2024-04-28 22:01:32.492609 prophetverse-0.0.2/src/prophetverse/utils/regex.py
--rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 prophetverse-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-30 12:07:43.248255 prophetverse-0.0.3a0/LICENSE
+-rw-r--r--   0        0        0     3328 2024-04-30 12:07:43.248255 prophetverse-0.0.3a0/README.md
+-rw-r--r--   0        0        0      671 2024-04-30 12:08:33.056820 prophetverse-0.0.3a0/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/__init__.py
+-rw-r--r--   0        0        0     1797 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/changepoint.py
+-rw-r--r--   0        0        0    14517 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/effects.py
+-rw-r--r--   0        0        0     6608 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/engine.py
+-rw-r--r--   0        0        0       66 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/logger.py
+-rw-r--r--   0        0        0      110 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/models/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/models/multivariate_model/__init__.py
+-rw-r--r--   0        0        0     2528 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/models/multivariate_model/_model.py
+-rw-r--r--   0        0        0     1541 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/models/multivariate_model/changepoint.py
+-rw-r--r--   0        0        0     4831 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/models/multivariate_model/multiindex.py
+-rw-r--r--   0        0        0     1546 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/models/univariate_model.py
+-rw-r--r--   0        0        0       77 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/sktime/__init__.py
+-rw-r--r--   0        0        0     4364 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/sktime/_expand_column_per_level.py
+-rw-r--r--   0        0        0    14328 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/sktime/base.py
+-rw-r--r--   0        0        0    25304 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/sktime/multivariate.py
+-rw-r--r--   0        0        0     2054 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/sktime/seasonality.py
+-rw-r--r--   0        0        0    13915 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/sktime/univariate.py
+-rw-r--r--   0        0        0     3813 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/utils/frame_to_array.py
+-rw-r--r--   0        0        0     1206 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/utils/logistic.py
+-rw-r--r--   0        0        0      756 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/utils/regex.py
+-rw-r--r--   0        0        0     3873 1970-01-01 00:00:00.000000 prophetverse-0.0.3a0/PKG-INFO
```

### Comparing `prophetverse-0.0.2/LICENSE` & `prophetverse-0.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.2/README.md` & `prophetverse-0.0.3a0/README.md`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.2/pyproject.toml` & `prophetverse-0.0.3a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prophetverse"
-version = "0.0.2"
+version = "0.0.3a0"
 description = ""
 authors = ["Felipe Angelim <felipeangelim@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "prophetverse", from="src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
```

### Comparing `prophetverse-0.0.2/src/prophetverse/changepoint.py` & `prophetverse-0.0.3a0/src/prophetverse/changepoint.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.2/src/prophetverse/effects.py` & `prophetverse-0.0.3a0/src/prophetverse/effects.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #  pylint: disable=g-import-not-at-top
-from typing import Protocol, TypedDict, Dict, Tuple, Callable
+from typing import Protocol, TypedDict, Dict, Tuple, Callable, List
 import jax.numpy as jnp
 import numpyro
 from numpyro import distributions as dist
 import re
 import logging
 import pandas as pd
 from abc import ABC, abstractmethod
@@ -17,16 +17,51 @@
     """Abstract class for effects.
     
     Effects should inherit from this class and implement the `compute_effect` method.
     The id is used to create unique names for the samples in the model.
     
     """
 
-    def __init__(self, id=""):
+    def __init__(self, id="", regex=None, **kwargs):
         self.id = id
+        self.regex = regex
+        
+        
+    def match_columns(self, columns : pd.Index) -> pd.Index:
+        """Match the columns of the DataFrame with the regex pattern.
+        
+        Args:
+            X (pd.DataFrame): The DataFrame to match.
+        
+        Returns:
+            pd.Index: The columns that match the regex pattern.
+        """
+        
+        if isinstance(columns, List):
+            columns = pd.Index(columns)
+            
+        if self.regex is None:
+            raise ValueError("To use this method, you must set the regex pattern")
+        return columns[columns.str.match(self.regex)]
+    
+    @staticmethod
+    def split_data_into_effects(X : pd.DataFrame, effects : List) -> Dict[str, pd.DataFrame]:
+        """Split the data into effects.
+        
+        Args:
+            X (pd.DataFrame): The DataFrame to split.
+            effects (List[AbstractEffect]): The effects to split the data into.
+        
+        Returns:
+            Dict[str, pd.DataFrame]: A dictionary mapping effect names to DataFrames.
+        """
+        data = {}
+        for effect in effects:
+            data[effect.id] = X[effect.match_columns(X)]
+        return data
 
     def sample(self, name : str, *args, **kwargs):
         """
         Sample a random variable with a unique name.
         """
         return numpyro.sample(f"{self.id}__{name}", *args, **kwargs)
 
@@ -56,45 +91,43 @@
 
     effect = scale * log(rate * data + 1)
 
     A gamma prior is used for the scale and rate parameters.
 
     Args:
         id (str): The identifier for the effect.
-        scale_prior (tuple): A tuple specifying the gamma prior for the scale parameter. 
-            The tuple should contain the gamma distribution class, followed by the parameters 
-            for the distribution (shape and rate).
-        rate_prior (tuple): A tuple specifying the gamma prior for the rate parameter. 
-            The tuple should contain the gamma distribution class, followed by the parameters 
-            for the distribution (shape and rate).
+        scale_prior (dist.Distribution): The prior distribution for the scale parameter.
+        rate_prior (dist.Distribution): The prior distribution for the rate parameter.
     """
 
-    def __init__(self,
-                 id="",
-                 scale_prior=(dist.Gamma, 1, 1),
-                 rate_prior=(dist.Gamma, 1, 1),
-                 effect_mode="multiplicative"):
+    def __init__(
+        self,
+        scale_prior=dist.Gamma(1, 1),
+        rate_prior=dist.Gamma(1, 1),
+        effect_mode="multiplicative",
+        **kwargs,
+    ):
         self.scale_prior = scale_prior
         self.rate_prior = rate_prior
         self.effect_mode = effect_mode
-        super().__init__(id)
+        super().__init__(**kwargs)
 
     def compute_effect(self, trend, data):
         """
         Computes the effect using the log transformation.
 
         Args:
             trend: The trend component.
             data: The input data.
 
         Returns:
             The computed effect.
         """
-        scale = self.sample("log_scale", self.scale_prior[0](*self.scale_prior[1:]))
-        rate = self.sample("log_rate", self.rate_prior[0](*self.rate_prior[1:]))
+        scale = self.sample("log_scale", self.scale_prior)
+        rate = self.sample("log_rate", self.rate_prior)
         effect = scale * jnp.log(rate * data + 1)
         if self.effect_mode == "additive":
             return effect
         return trend * effect
 
 
 class LinearEffect(AbstractEffect):
@@ -112,40 +145,44 @@
         effect_mode (str): The mode of the effect, either "multiplicative" or "additive".
 
     Methods:
         compute_effect(trend, data): Computes the effect based on the given trend and data.
 
     """
 
-    def __init__(self, id="", prior=(dist.Normal, 0, 1), effect_mode="multiplicative"):
+    def __init__(
+        self,
+        prior=(dist.Normal, 0, 1),
+        effect_mode="multiplicative",
+        **kwargs):
         self.prior = prior
         self.effect_mode = effect_mode
-        super().__init__(id)
+        super().__init__(**kwargs)
 
     def compute_effect(self, trend, data):
         """
         Computes the effect based on the given trend and data.
 
         Args:
             trend: The trend component of the hierarchical prophet model.
             data: The data used to compute the effect.
 
         Returns:
             The computed effect based on the given trend and data.
 
         """
         n_features = data.shape[-1]
-        
+
         dist = self.prior[0]
         dist_args = self.prior[1:]
         coefficients = self.sample(
             "coefs",
             dist(*[jnp.array([arg] * n_features) for arg in dist_args]),
         )
-        
+
         if coefficients.ndim == 1:
             coefficients = jnp.expand_dims(coefficients, axis=-1)
 
         if data.ndim == 3 and coefficients.ndim == 2:
             coefficients = jnp.expand_dims(coefficients, axis=0)
         if self.effect_mode == "multiplicative":
             return multiplicative_effect(trend, data, coefficients)
@@ -186,20 +223,20 @@
     """
 
     def __init__(self,
                  exogenous_priors: Dict[str, Tuple[dist.Distribution, ...]],
                  feature_names: pd.Index,
                  default_exogenous_prior=(dist.Normal, 0, 1),
                  effect_mode="multiplicative",
-                 id=""):
+                 **kwargs):
         self.exogenous_priors = exogenous_priors
         self.feature_names = pd.Index(feature_names)
         self.default_exogenous_prior = default_exogenous_prior
         self.effect_mode = effect_mode
-        super().__init__(id)
+        super().__init__(**kwargs)
 
         self.set_distributions_and_permutation_matrix()
 
     def compute_effect(self, trend, data):
         """
         Compute the effect on the trend using the sampled coefficients.
 
@@ -302,14 +339,61 @@
                     "exogenous_coefficients_{}".format(regex), distribution
                 ).reshape((-1, 1))
             )
 
         return self.exogenous_permutation_matrix @ jnp.concatenate(parameters, axis=0)
 
 
+class HillEffect(AbstractEffect):
+    """
+    Represents a Hill effect in a time series model.
+
+    Attributes:
+        half_max_prior: Prior distribution for the half-maximum parameter.
+        slope_prior: Prior distribution for the slope parameter.
+        max_effect_prior: Prior distribution for the maximum effect parameter.
+        effect_mode: Mode of the effect (either "additive" or "multiplicative").
+    """
+
+    def __init__(
+        self,
+        half_max_prior=dist.Gamma(1, 1),
+        slope_prior=dist.HalfNormal(10),
+        max_effect_prior=dist.Gamma(1, 1),
+        effect_mode="multiplicative",
+        **kwargs,
+    ):
+        self.half_max_prior = half_max_prior
+        self.slope_prior = slope_prior
+        self.max_effect_prior = max_effect_prior
+        self.effect_mode = effect_mode
+        super().__init__(**kwargs)
+
+    def compute_effect(self, trend, data):
+        """
+        Computes the effect using the log transformation.
+
+        Args:
+            trend: The trend component.
+            data: The input data.
+
+        Returns:
+            The computed effect.
+        """
+
+        half_max = self.sample("half_max", self.half_max_prior)
+        slope = self.sample("slope", self.slope_prior)
+        max_effect = self.sample("max_effect", self.max_effect_prior)
+
+        effect = max_effect * (1 / (1 + (data / half_max) ** -slope))
+
+        if self.effect_mode == "additive":
+            return effect
+        return trend * effect
+
 
 def matrix_multiplication(data, coefficients):
     return data @ coefficients.reshape((-1, 1))
 
 
 def additive_effect(
     trend: jnp.ndarray, data: jnp.ndarray, coefficients: jnp.ndarray
@@ -317,29 +401,7 @@
     return matrix_multiplication(data, coefficients)
 
 
 def multiplicative_effect(
     trend: jnp.ndarray, data: jnp.ndarray, coefficients: jnp.ndarray
 ) -> jnp.ndarray:
     return trend * matrix_multiplication(data, coefficients)
-
-
-
-
-def _apply_exponent_safe(
-    data: jnp.ndarray,
-    exponent: jnp.ndarray,
-) -> jnp.ndarray:
-    """Applies an exponent to given data in a gradient safe way.
-
-    More info on the double jnp.where can be found:
-    https://github.com/tensorflow/probability/blob/main/discussion/where-nan.pdf
-
-    Args:
-      data: Input data to use.
-      exponent: Exponent required for the operations.
-
-    Returns:
-      The result of the exponent operation with the inputs provided.
-    """
-    exponent_safe = jnp.where(data == 0, 1, data) ** exponent
-    return jnp.where(data == 0, 0, exponent_safe)
```

### Comparing `prophetverse-0.0.2/src/prophetverse/engine.py` & `prophetverse-0.0.3a0/src/prophetverse/engine.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.2/src/prophetverse/models/multivariate_model/_model.py` & `prophetverse-0.0.3a0/src/prophetverse/models/multivariate_model/_model.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.2/src/prophetverse/models/multivariate_model/changepoint.py` & `prophetverse-0.0.3a0/src/prophetverse/models/multivariate_model/changepoint.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.2/src/prophetverse/models/univariate_model.py` & `prophetverse-0.0.3a0/src/prophetverse/models/univariate_model.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.2/src/prophetverse/sktime/_expand_column_per_level.py` & `prophetverse-0.0.3a0/src/prophetverse/sktime/_expand_column_per_level.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.2/src/prophetverse/sktime/base.py` & `prophetverse-0.0.3a0/src/prophetverse/sktime/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from numpyro.contrib.control_flow import scan
 from numpyro.infer import MCMC, NUTS, Predictive, init_to_mean
 from sktime.forecasting.base import BaseForecaster, ForecastingHorizon
 from collections import OrderedDict
 from prophetverse.engine import MAPInferenceEngine, MCMCInferenceEngine, InferenceEngine
 from prophetverse.effects import LinearEffect
 from prophetverse.utils.frame_to_array import series_to_tensor
-
+from prophetverse.effects import AbstractEffect
 import re
 import logging
 
 class BaseBayesianForecaster(BaseForecaster):
     """
     Base class for Bayesian forecasters in hierarchical-prophet.
 
@@ -376,72 +376,72 @@
 
     return params
 
 
 class ExogenousEffectMixin:
 
     def __init__(self,
-                 default_effect_mode,
-                 exogenous_effects: Dict[str, Tuple[str, Any]],
-                 default_exogenous_prior: Tuple[str, Any],
+                 
+                 exogenous_effects: List[AbstractEffect],
+                 default_effect = None,
                  **kwargs):
 
-        self.default_effect_mode = default_effect_mode
+        
         self.exogenous_effects = exogenous_effects
-        self.default_exogenous_prior = default_exogenous_prior
+        self.default_effect = default_effect
         super().__init__(**kwargs)
+        
+        if self.default_effect is None:
+            self.default_effect = LinearEffect(
+                id="default_exog",
+                prior=(dist.Normal, 0, 1),
+                effect_mode="additive",
+            )
 
     def _set_custom_effects(self, feature_names):
 
         effects_and_columns = {}
         columns_with_effects = set()
         exogenous_effects = self.exogenous_effects or {}
+        
 
-        for effect_name, (column_regex, effect) in exogenous_effects.items():
+        for effect in exogenous_effects:
 
-            columns = [
-                column for column in feature_names if re.match(column_regex, column)
-            ]
+            columns = effect.match_columns(feature_names)
 
             if columns_with_effects.intersection(columns):
                 raise ValueError(
                     "Columns {} are already set".format(
                         columns_with_effects.intersection(columns)
                     )
                 )
 
             if not len(columns):
-                logging.warning("No columns match the regex {}".format(column_regex))
+                logging.warning("No columns match the regex {}".format(effect.regex))
 
             columns_with_effects = columns_with_effects.union(columns)
 
             effects_and_columns.update(
                 {
-                    effect_name: (
+                    effect.id: (
                         columns,
                         effect,
                     )
                 }
             )
 
         features_without_effects: set = feature_names.difference(columns_with_effects)
 
         if len(features_without_effects):
 
-            default_dist = getattr(dist, self.default_exogenous_prior[0])
-            args = self.default_exogenous_prior[1:]
             effects_and_columns.update(
                 {
                     "default": (
                         features_without_effects,
-                        LinearEffect(
-                            id="exog",
-                            prior=(default_dist, *args),
-                            effect_mode=self.default_effect_mode,
-                        ),
+                        self.default_effect,
                     )
                 }
             )
 
         self._exogenous_effects_and_columns = effects_and_columns
 
     def _get_exogenous_data_array(self, X):
```

### Comparing `prophetverse-0.0.2/src/prophetverse/sktime/multivariate.py` & `prophetverse-0.0.3a0/src/prophetverse/sktime/multivariate.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from prophetverse.utils.frame_to_array import (
     convert_index_to_days_since_epoch,
     extract_timetensor_from_dataframe,
     loc_bottom_series,
     series_to_tensor,
 )
-from prophetverse.utils.multiindex import reindex_time_series
+from prophetverse.models.multivariate_model.multiindex import reindex_time_series
 from prophetverse.utils.logistic import suggest_logistic_rate_and_offset
 from prophetverse.sktime.base import (
     BaseBayesianForecaster,
     ExogenousEffectMixin,
     init_params,
 )
 
@@ -66,17 +66,16 @@
                                    If an int, the range will be that number of points. A negative int indicates number of points
                                    counting from the end of the history.
         changepoint_prior_scale (float): Parameter controlling the flexibility of the automatic changepoint selection.
         capacity_prior_scale (float): Scale parameter for the capacity prior. Defaults to 0.2.
         capacity_prior_loc (float): Location parameter for the capacity prior. Defaults to 1.1.
         trend (str): Type of trend. Either "linear" or "logistic". Defaults to "linear".
         feature_transformer (BaseTransformer or None): A transformer to preprocess the exogenous features. Defaults to None.
-        exogenous_effects (list or None): List of exogenous effects to include in the model. Defaults to None.
-        default_effect_mode (str): Default mode for exogenous effects. Either "multiplicative" or "additive". Defaults to "multiplicative".
-        default_exogenous_prior (tuple): Default prior distribution for exogenous effects. See numpyro.distributions for options. Defaults to ("Normal", 0, 1).
+        exogenous_effects (List[AbstractEffect]): A list defining the exogenous effects to be used in the model.
+        default_effect (AbstractEffect): The default effect to be used when no effect is specified for a variable.
         shared_features (list): List of shared features across series. Defaults to an empty list.
         mcmc_samples (int): Number of MCMC samples to draw. Defaults to 2000.
         mcmc_warmup (int): Number of warmup steps for MCMC. Defaults to 200.
         mcmc_chains (int): Number of MCMC chains. Defaults to 4.
         inference_method (str): Inference method to use. Either "map" or "mcmc". Defaults to "map".
         optimizer_name (str): Name of the optimizer to use. Defaults to "Adam".
         optimizer_kwargs (dict): Additional keyword arguments for the optimizer. Defaults to {"step_size": 1e-4}.
@@ -114,16 +113,15 @@
         changepoint_range=None,
         changepoint_prior_scale=0.1,
         capacity_prior_scale=0.2,
         capacity_prior_loc=1.1,
         trend="linear",
         feature_transformer: BaseTransformer = None,
         exogenous_effects=None,
-        default_effect_mode="multiplicative",
-        default_exogenous_prior=("Normal", 0, 1),
+        default_effect=None,
         shared_features=[],
         mcmc_samples=2000,
         mcmc_warmup=200,
         mcmc_chains=4,
         inference_method="map",
         optimizer_name="Adam",
         optimizer_kwargs={"step_size": 1e-4},
@@ -136,31 +134,29 @@
         self.changepoint_interval = changepoint_interval
         self.changepoint_range = changepoint_range
         self.changepoint_prior_scale = changepoint_prior_scale
         self.noise_scale = noise_scale
         self.capacity_prior_scale = capacity_prior_scale
         self.capacity_prior_loc = capacity_prior_loc
         self.trend = trend
-        self.default_exogenous_prior = default_exogenous_prior
         self.shared_features = shared_features
         self.feature_transformer = feature_transformer
         self.correlation_matrix_concentration = correlation_matrix_concentration
 
         super().__init__(
             rng_key=rng_key,
-            default_effect_mode=default_effect_mode,
             inference_method=inference_method,
             optimizer_name=optimizer_name,
             optimizer_kwargs=optimizer_kwargs,
             optimizer_steps=optimizer_steps,
             mcmc_samples=mcmc_samples,
             mcmc_warmup=mcmc_warmup,
             mcmc_chains=mcmc_chains,
+            default_effect=default_effect,
             exogenous_effects=exogenous_effects,
-            default_exogenous_prior=default_exogenous_prior,
         )
 
         self.model = model
         self._validate_hyperparams()
 
     def _validate_hyperparams(self):
         """
@@ -173,18 +169,15 @@
             raise ValueError("changepoint_prior_scale must be greater than 0.")
         if self.noise_scale <= 0:
             raise ValueError("noise_scale must be greater than 0.")
         if self.capacity_prior_scale <= 0:
             raise ValueError("capacity_prior_scale must be greater than 0.")
         if self.capacity_prior_loc <= 0:
             raise ValueError("capacity_prior_loc must be greater than 0.")
-        if self.default_effect_mode not in ["multiplicative", "additive"]:
-            raise ValueError(
-                'seasonality_mode must be either "multiplicative" or "additive".'
-            )
+
         if self.trend not in ["linear", "logistic"]:
             raise ValueError('trend must be either "linear" or "logistic".')
 
     def _get_fit_data(self, y, X, fh):
         """
         Prepare the data for the NumPyro model.
 
@@ -538,27 +531,25 @@
         Returns:
             np.ndarray: Predicted samples.
         """
         samples = super().predict_samples(X=X, fh=fh)
 
         return self.aggregator_.transform(samples)
 
-    
-
     def _get_predict_data(self, X: pd.DataFrame, fh: ForecastingHorizon) -> np.ndarray:
         """Generate samples for the given exogenous variables and forecasting horizon.
 
         Args:
             X (pd.DataFrame): Exogenous variables.
             fh (ForecastingHorizon): Forecasting horizon.
 
         Returns:
             np.ndarray: Predicted samples.
         """
-        
+
         fh_dates = fh.to_absolute(
             cutoff=self.full_y_indexes_.get_level_values(-1).max()
         )
         fh_as_index = pd.Index(list(fh_dates.to_numpy()))
 
         if not isinstance(fh, ForecastingHorizon):
             fh = self._check_fh(fh)
```

### Comparing `prophetverse-0.0.2/src/prophetverse/sktime/seasonality.py` & `prophetverse-0.0.3a0/src/prophetverse/sktime/seasonality.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.2/src/prophetverse/sktime/univariate.py` & `prophetverse-0.0.3a0/src/prophetverse/sktime/univariate.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,16 +68,16 @@
         mcmc_samples (int): Number of MCMC samples to draw.
         mcmc_warmup (int): Number of MCMC warmup steps.
         mcmc_chains (int): Number of MCMC chains to run in parallel.
         inference_method (str): Inference method to use. Can be "mcmc" or "map".
         optimizer_name (str): Name of the optimizer to use for variational inference.
         optimizer_kwargs (dict): Additional keyword arguments to pass to the optimizer.
         optimizer_steps (int): Number of optimization steps to perform for variational inference.
-        exogenous_effects (dict): Dictionary specifying the exogenous effects and their modes.
-        default_effect_mode (str): Default mode for exogenous effects.
+        exogenous_effects (List[AbstractEffect]): A list defining the exogenous effects to be used in the model.
+        default_effect (AbstractEffect): The default effect to be used when no effect is specified for a variable.
         default_exogenous_prior (tuple): Default prior distribution for exogenous effects.
         rng_key (jax.random.PRNGKey): Random number generator key.
 
 
     """
 
     _tags = {
@@ -99,16 +99,15 @@
         mcmc_warmup=200,
         mcmc_chains=4,
         inference_method="map",
         optimizer_name="Adam",
         optimizer_kwargs={"step_size" : 1e-4},
         optimizer_steps=100_000,
         exogenous_effects=None,
-        default_effect_mode="multiplicative",
-        default_exogenous_prior=("Normal", 0, 1),
+        default_effect=None,
         rng_key=random.PRNGKey(24),
     ):
         """
         Initializes the Prophet model.
         """
 
         self.changepoint_interval = changepoint_interval
@@ -119,16 +118,15 @@
         self.capacity_prior_scale = capacity_prior_scale
         self.capacity_prior_loc = capacity_prior_loc
         self.trend = trend
 
         super().__init__(
             rng_key=rng_key,
             # ExogenousEffectMixin
-            default_effect_mode=default_effect_mode,
-            default_exogenous_prior=default_exogenous_prior,
+            default_effect=default_effect,
             exogenous_effects=exogenous_effects,
             # BaseBayesianForecaster
             inference_method=inference_method,
             mcmc_samples=mcmc_samples,
             mcmc_warmup=mcmc_warmup,
             mcmc_chains=mcmc_chains,
             optimizer_name=optimizer_name,
@@ -150,18 +148,14 @@
             raise ValueError("changepoint_prior_scale must be greater than 0.")
         if self.noise_scale <= 0:
             raise ValueError("noise_scale must be greater than 0.")
         if self.capacity_prior_scale <= 0:
             raise ValueError("capacity_prior_scale must be greater than 0.")
         if self.capacity_prior_loc <= 0:
             raise ValueError("capacity_prior_loc must be greater than 0.")
-        if self.default_effect_mode not in ["multiplicative", "additive"]:
-            raise ValueError(
-                'seasonality_mode must be either "multiplicative" or "additive".'
-            )
         if self.trend not in ["linear", "logistic"]:
             raise ValueError('trend must be either "linear" or "logistic".')
 
     def _get_fit_data(self, y, X, fh):
         """
         Prepares the data for the Numpyro model.
```

### Comparing `prophetverse-0.0.2/src/prophetverse/utils/frame_to_array.py` & `prophetverse-0.0.3a0/src/prophetverse/utils/frame_to_array.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.2/src/prophetverse/utils/logistic.py` & `prophetverse-0.0.3a0/src/prophetverse/utils/logistic.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.2/PKG-INFO` & `prophetverse-0.0.3a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: prophetverse
-Version: 0.0.2
+Version: 0.0.3a0
 Summary: 
 Author: Felipe Angelim
 Author-email: felipeangelim@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpyro (>=0.13.2)
 Requires-Dist: optax (>=0.2)
 Requires-Dist: sktime (>=0.21)
 Description-Content-Type: text/markdown
 
 # Prophetverse
```

