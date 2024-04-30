# Comparing `tmp/survival_data_handler-2024.4.7.tar.gz` & `tmp/survival_data_handler-2024.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survival_data_handler-2024.4.7.tar", last modified: Mon Apr 29 16:25:13 2024, max compression
+gzip compressed data, was "survival_data_handler-2024.4.9.tar", last modified: Tue Apr 30 08:54:27 2024, max compression
```

## Comparing `survival_data_handler-2024.4.7.tar` & `survival_data_handler-2024.4.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:25:13.116891 survival_data_handler-2024.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-29 16:25:13.116891 survival_data_handler-2024.4.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2108 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:25:13.116891 survival_data_handler-2024.4.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:25:13.116891 survival_data_handler-2024.4.7/survival_data_handler/
--rwxr-xr-x   0 runner    (1001) docker     (127)      762 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/survival_data_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/survival_data_handler/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15904 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/survival_data_handler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/survival_data_handler/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/survival_data_handler/plotting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6364 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/survival_data_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:25:13.116891 survival_data_handler-2024.4.7/survival_data_handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-29 16:25:13.000000 survival_data_handler-2024.4.7/survival_data_handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-29 16:25:13.000000 survival_data_handler-2024.4.7/survival_data_handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:25:13.000000 survival_data_handler-2024.4.7/survival_data_handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-29 16:25:13.000000 survival_data_handler-2024.4.7/survival_data_handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 16:25:13.000000 survival_data_handler-2024.4.7/survival_data_handler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:25:13.116891 survival_data_handler-2024.4.7/test/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6905 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:54:27.598006 survival_data_handler-2024.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-30 08:54:20.000000 survival_data_handler-2024.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-30 08:54:27.598006 survival_data_handler-2024.4.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2108 2024-04-30 08:54:20.000000 survival_data_handler-2024.4.9/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-30 08:54:20.000000 survival_data_handler-2024.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-30 08:54:20.000000 survival_data_handler-2024.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 08:54:27.598006 survival_data_handler-2024.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:54:27.594006 survival_data_handler-2024.4.9/survival_data_handler/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      762 2024-04-30 08:54:20.000000 survival_data_handler-2024.4.9/survival_data_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-30 08:54:20.000000 survival_data_handler-2024.4.9/survival_data_handler/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14365 2024-04-30 08:54:20.000000 survival_data_handler-2024.4.9/survival_data_handler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-30 08:54:20.000000 survival_data_handler-2024.4.9/survival_data_handler/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-30 08:54:20.000000 survival_data_handler-2024.4.9/survival_data_handler/plotting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6346 2024-04-30 08:54:20.000000 survival_data_handler-2024.4.9/survival_data_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:54:27.598006 survival_data_handler-2024.4.9/survival_data_handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-30 08:54:27.000000 survival_data_handler-2024.4.9/survival_data_handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-30 08:54:27.000000 survival_data_handler-2024.4.9/survival_data_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:54:27.000000 survival_data_handler-2024.4.9/survival_data_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 08:54:27.000000 survival_data_handler-2024.4.9/survival_data_handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 08:54:27.000000 survival_data_handler-2024.4.9/survival_data_handler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:54:27.598006 survival_data_handler-2024.4.9/test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7318 2024-04-30 08:54:20.000000 survival_data_handler-2024.4.9/test/test_main.py
```

### Comparing `survival_data_handler-2024.4.7/LICENSE` & `survival_data_handler-2024.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.4.7/PKG-INFO` & `survival_data_handler-2024.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: survival_data_handler
-Version: 2024.4.7
+Version: 2024.4.9
 Author-email: Vincent Laurent <vlaurent@eurobios.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3
 Requires-Dist: seaborn
 Requires-Dist: numba
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: pandas>2
 Requires-Dist: lifelines
 Requires-Dist: numpy
+Requires-Dist: plotly
 
 # Survival data handler
 ![code coverage](https://raw.githubusercontent.com/eurobios-mews-labs/survival-data-handler/coverage-badge/coverage.svg?raw=true)
 [![PyPI version](https://badge.fury.io/py/palma.svg)](https://badge.fury.io/py/palma)
 
 ```python
 import pandas as pd
```

### Comparing `survival_data_handler-2024.4.7/README.md` & `survival_data_handler-2024.4.9/README.md`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.4.7/survival_data_handler/__init__.py` & `survival_data_handler-2024.4.9/survival_data_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.4.7/survival_data_handler/base.py` & `survival_data_handler-2024.4.9/survival_data_handler/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,55 +53,53 @@
 class TimeCurve:
 
     def __interpolator(self):
         pass
 
 
 class TimeCurveData(pd.DataFrame, TimeCurve):
-    def __init__(self, *args, unit='D', n_unit=1., ):
+    def __init__(self, *args):
         super().__init__(*args)
-        self.n_unit = n_unit
-        self.unit = unit
-        self.__unit = pd.to_timedelta(n_unit, unit=unit).total_seconds()
         self.__checks()
 
     def __checks(self):
         if not all(self.columns[i] <= self.columns[i + 1] for i in range(len(self.columns) - 1)):
             raise ValueError(
-                "Columns must be sorted")  # if not isinstance(self.columns[0], pd.Timedelta):  #     raise ValueError("Columns must symbolize time index")
+                "Columns must be sorted")
+        # if not isinstance(self.columns[0], pd.Timedelta):
+        #     raise ValueError("Columns must symbolize time index")
 
     def __interpolator(self):
         self.__interpolation = {
             c: interp1d(self.columns.astype(int), self.loc[c], fill_value="extrapolate")
             for c in self.index}
 
     def derivative(self):
-        return TimeCurveData(compute_derivative(self, self.__unit))
+        return TimeCurveData(compute_derivative(self))
 
     def log(self):
         return TimeCurveData(np.log(self))
 
     def exp(self):
         return TimeCurveData(np.exp(self))
 
     def __truediv__(self, other):
-        return TimeCurveData(pd.DataFrame(self.values / self.__other(other), columns=self.columns, index=self.index),
-                             unit=self.unit, n_unit=self.n_unit)
+        return TimeCurveData(
+            pd.DataFrame(self.values / self.__other(other), columns=self.columns, index=self.index), )
 
     def __add__(self, other):
         return TimeCurveData(pd.DataFrame(self.values + self.__other(other), columns=self.columns, index=self.index),
-                             unit=self.unit, n_unit=self.n_unit)
+                             )
 
     def __sub__(self, other):
         return TimeCurveData(pd.DataFrame(self.values - self.__other(other), columns=self.columns, index=self.index),
-                             unit=self.unit, n_unit=self.n_unit)
+                             )
 
     def __neg__(self):
-        return TimeCurveData(pd.DataFrame(-self.values, index=self.index, columns=self.columns), unit=self.unit,
-                             n_unit=self.n_unit)
+        return TimeCurveData(pd.DataFrame(-self.values, index=self.index, columns=self.columns))
 
     @property
     def interpolation(self) -> dict:
         if not hasattr(self, "__interpolation"):
             self.__interpolator()
         return self.__interpolation
 
@@ -136,15 +134,14 @@
         self.__window = window
 
     @property
     def interpolation(self) -> pd.Series:
         return pd.Series(self.__interpolation, name="interpolation")
 
     def __shift(self) -> TimeCurveData:
-
         data = pd.merge(
             self.__reduced_matching["index"].reset_index(),
             self.interpolation,
             right_index=True,
             left_on='index')
 
         data = data.set_index("origin_index").drop("index", axis=1)
```

### Comparing `survival_data_handler-2024.4.7/survival_data_handler/main.py` & `survival_data_handler-2024.4.9/survival_data_handler/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,58 +29,41 @@
 class Lifespan(SurvivalCurves):
     __index = "origin_index"
 
     def __init__(self, ageing_curves: pd.DataFrame, index: iter, age: iter, birth: iter, window: tuple,
                  default_precision="float"):
 
         self.__curves = TimeCurveData(ageing_curves.__deepcopy__())
-        self.df_idx = pd.DataFrame(dict(age=age, birth=birth, index=index))
-
-        self.df_idx.index.name = self.__index
-        self.index = index
-        self.age = age
-        self.window = window
-        self.__p = default_precision
-        self.__survival_estimation = SurvivalEstimation(self.curves, unit='D', n_unit=365.25)
+        self.estimations = SurvivalEstimation(self.curves)
 
         self.__tci = TimeCurveInterpolation(
-            self.__survival_estimation.survival_function.interpolation,
+            self.estimations.survival_function.interpolation,
             birth,
             index,
             window,
             pd.to_timedelta(30, "D")
         )
 
         self.__check_args()
-
-        # self._df_idx_unique = self.df_idx.drop_duplicates(subset=["index", "birth"])
-        # self.starting_dates = self._df_idx_unique["birth"]
-        # c = ["birth", "index"]
-
-        # self._corresp = pd.merge(self._df_idx_unique[c].reset_index(), self.df_idx[c].reset_index(),
-        #                          on=["birth", "index"], suffixes=("_u", ""))
-        #
-        # self._corresp = self._corresp.drop(columns=c)
         self.confusion_matrix_threshold = np.nan
         self.__computed = []
         self.__supervised = False
         self.__interpolator = {}
         super().__init__(self.__tci.curve)
 
     def __check_args(self):
-
         if hasattr(self.curves.columns, "dt"):
             ValueError("curves index must have dt property")
 
     @property
     def computed_historical_data(self):
         return self.__computed
 
     @property
-    def supervised(self):
+    def supervised(self) -> bool:
         return self.__supervised
 
     def add_supervision(self, event, durations, entry=None):
         self.event = event
         self.durations = durations
         self.entry = entry
         self.__supervised = True
@@ -90,29 +73,14 @@
         if not get_supervision:
             return ret, None, None, None
         else:
             index = [i for i in ret.index if i in self.event.index]
             entry = self.entry if self.entry is None else self.entry.loc[index]
             return ret.loc[index], self.event.loc[index], self.durations.loc[index], entry
 
-    # def _decompose_unique(self, data, get_supervision=False):
-    #     ret = pd.merge(self._corresp, data, right_index=True, left_on='origin_index_u').drop(
-    #         columns=["origin_index_u"]).set_index("origin_index")
-    #
-    #     if not get_supervision:
-    #         return ret, None, None, None
-    #     else:
-    #         index = [i for i in ret.index if i in self.event.index]
-    #         entry = self.entry if self.entry is None else self.entry.loc[index]
-    #         return ret.loc[index], self.event.loc[index], self.durations.loc[index], entry
-
-    @property
-    def residual_expected_life(self) -> pd.DataFrame:
-        return self.residual_life
-
     # ==============================================
     #           ENRICH REPRESENTATION
     # ==============================================
 
     def residual_survival(self, t0) -> pd.DataFrame:
 
         t0 = max(t0, self.survival_function.columns[0])
@@ -122,15 +90,16 @@
         return df
 
     def compute_times(self, p=0.95, on="survival_function"):
         cond_low = (self.__getattribute__(on) > p).sum(axis=1)
         dates = self.__getattribute__(on).columns.to_numpy()
         return pd.Series(dates[cond_low])
 
-    def remove_the_dead(self, data: pd.DataFrame, error="coerce"):
+    def remove_the_dead(self, on, error="coerce"):
+        data = self.__getattribute__(on)
         try:
             data = data.loc[self.event.index[~self.event.astype(bool)]]
         except KeyError as e:
             print(e)
 
             if error == "raise":
                 raise KeyError(e)
@@ -189,15 +158,15 @@
 
         return df_matrix
 
     # ==============================================
     #           PLOTS CURVES
     # ==============================================
     def plot_curves_residual_life(self, **kwargs):
-        self.__survival_estimation.plot_residual_life(**kwargs)
+        self.estimations.plot_residual_life(**kwargs)
         plt.ylabel("Expected residual lifespan")
         plt.xlabel("Time [Y]")
 
     def plot_average_tagged(self, on: str, event_type=None, plot_test_window=False, plot_type="dist"):
         corresp, event, duration, entry = self.__get_align_data(on, get_supervision=True)
         if event_type == "censored":
             sample = corresp[~event.astype(bool)].astype("float32")
@@ -277,29 +246,33 @@
     def plotly_auc_vs_score(self, on: str, temporal_metric: pd.Series, **kwargs):
         corresp, event, duration, entry = self.__get_align_data(on, get_supervision=True)
         time_start, time_stop = duration.min(), duration.max()
         corresp = corresp[[c for c in corresp.columns if time_start <= c <= time_stop]]
         return plotting.auc_vs_score_plotly(temporal_scores=corresp, event_observed=event, censoring_time=duration,
                                             entry_time=entry, temporal_metric=temporal_metric, **kwargs)
 
-    @staticmethod
-    def plotly_roc_curve(roc: dict, colormap="magma_r", template="plotly_white", **kwargs):
+    def plotly_roc_curve(self, on, method="roc-cd", colormap="magma_r", template="plotly_white", **kwargs):
+        roc = self.assess_metric(on, method, metric=metrics.roc_curve)
         return plotting.plot_roc_curve_plotly(roc, colormap=colormap, template=template, **kwargs)
 
     # ==============================================
     #           METRIC ASSESSMENT
     # ==============================================
-    def assess_metric(self, data, method="roc-cd", metric=metrics.roc_auc_score):
-
-        corresp, event, duration, _ = self._decompose_unique(data, get_supervision=True)
+    def assess_metric(self, on, method="roc-cd", metric=metrics.roc_auc_score):
+        from survival_data_handler.metric import time_dependent_helper
+        data, event, duration, entry = self.__get_align_data(on, get_supervision=True)
 
         time_start, time_stop = duration.min(), duration.max()
-        corresp = corresp[[c for c in corresp.columns if time_start <= c <= time_stop]]
-        return metric.time_dependent_helper(corresp, event_observed=event, censoring_time=duration, method=method,
-                                            function=metric)
+        data = data[[c for c in data.columns if time_start <= c <= time_stop]]
+        return time_dependent_helper(
+            data,
+            event_observed=event,
+            censoring_time=duration,
+            method=method,
+            function=metric)
 
     # ==============================================
     #           Properties
     # ==============================================
     @property
     def curves(self) -> TimeCurveData:
         return self.__curves
@@ -311,45 +284,40 @@
 
 
 class SurvivalEstimation(SurvivalCurves):
     """
     Instantiate class with data as survival curves. Columns must be timedelta objects
     """
 
-    def __init__(self, survival_curves: pd.DataFrame, unit='D', n_unit=1., process_input_data=True):
+    def __init__(self, survival_curves: pd.DataFrame, process_input_data=True):
 
         super().__init__(survival_curves)
         survival_curves = survival_curves.__deepcopy__()
         if process_input_data:
             survival_curves = process_survival_function(survival_curves)
 
-        self.__survival = TimeCurveData(survival_curves, unit='D', n_unit=1.)
-        self.unit = pd.to_timedelta(n_unit, unit=unit).total_seconds()
+        self.__survival = TimeCurveData(survival_curves)
         self.__check_args()
 
-        self.__survival_d = self.survival_function.__deepcopy__()
-        self.__survival_d.columns = pd.to_timedelta(self.__survival_d.columns).total_seconds() / self.unit
-        self.residual_survival = None
-
     def plot_residual_life(self, sample=None, mean_behaviour=True, unit=pd.to_timedelta(1, "D")):
         if not mean_behaviour:
             if sample is not None:
                 residual_life_ = self.residual_life.sample(sample)
             else:
                 residual_life_ = self.residual_life
-            residual_life_.columns = pd.to_timedelta(self.survival_function.columns).total_seconds() / self.unit
+            residual_life_.columns = pd.to_timedelta(self.survival_function.columns).total_seconds() / unit.total_seconds()
             color = plt.get_cmap("magma_r")(residual_life_.iloc[:, 0] / residual_life_.iloc[:, 0].max())
 
             residual_life_.T.plot(legend=False, ax=plt.gca(), color=color, lw=0.15, alpha=1)
             plt.grid()
             bounds = residual_life_.columns.min(), residual_life_.columns.max()
             plt.plot(bounds, bounds[::-1], c="k", alpha=0.5, lw=2, ls="--")
         else:
             des = (self.residual_life / unit).describe([0.05, .25, .5, .75, 0.95])
-            des.columns = pd.to_timedelta(self.survival_function.columns).total_seconds() / self.unit
+            des.columns = pd.to_timedelta(self.survival_function.columns).total_seconds() / unit.total_seconds()
             des = des.T.dropna().T
             des = des.drop(["count", "mean", "std"])
             for i, d in enumerate(des.index):
                 c = plt.get_cmap("crest")(i / (len(des) - 1))
                 des.loc[d].plot(color=c, ax=plt.gca())
                 if i > 0:
                     plt.fill_between(
```

### Comparing `survival_data_handler-2024.4.7/survival_data_handler/metric.py` & `survival_data_handler-2024.4.9/survival_data_handler/metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,51 +82,33 @@
             return (censoring_time <= t_) & event_observed
 
         def marker(t_):
             return temporal_score[t_]
 
     elif method == "roc-id":
         def outcome(t_):
-            out = np.where(censoring_time < t_, np.nan, censoring_time)
-            return (t_ == out) & event_observed
+            out = censoring_time
+            out = (t_ == out) & event_observed
+            out[censoring_time < t_] = np.nan
+            return out
 
         def marker(t_):
             return temporal_score[t_]
     else:
         raise ValueError(f"method : {method} is not known")
 
     for t in temporal_score.columns:
         try:
             y_true = np.array(outcome(t))
             y_score = np.array(marker(t))
 
-            nan_ = np.isnan(y_true)
+            nan_ = np.isnan(y_true.astype(bool))
             nan_ |= np.isnan(y_score)
 
             result[t] = function(
                 y_true=y_true[~nan_],
                 y_score=y_score[~nan_]
             )
         except ValueError:
             pass
     return result
 
-
-@__validate_decorator
-def time_dependent_auc(
-        temporal_score: pd.DataFrame,
-        event_observed: iter,
-        censoring_time: iter,
-        method="harrell"
-) -> pd.Series:
-    """
-    method
-        - roc-cd : Cumulative sensitivity and dynamic specificity (C/D)
-        - roc-id : Incident sensitivity and dynamic specificity (I/D)
-    """
-    result = time_dependent_helper(
-        temporal_score,
-        event_observed,
-        censoring_time,
-        sk_metrics.roc_auc_score,
-        method)
-    return pd.Series(result, name=method)
```

### Comparing `survival_data_handler-2024.4.7/survival_data_handler/plotting.py` & `survival_data_handler-2024.4.9/survival_data_handler/plotting.py`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.4.7/survival_data_handler/utils.py` & `survival_data_handler-2024.4.9/survival_data_handler/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,22 +46,22 @@
     # apply correction
     data_correct = _cut(data_correct.astype("float32").values).astype(
         "float16")
     data.loc[crit_lines] = data_correct
     return data
 
 
-def compute_derivative(data: pd.DataFrame,
-                       unit) -> pd.DataFrame:
-    times = data.columns.to_numpy()
-    diff = data.T.diff()
-    return diff.divide(
-        pd.Series(times, index=times).diff().dt.total_seconds() / unit,
-        axis=0
-    ).T
+def compute_derivative(data: pd.DataFrame) -> pd.DataFrame:
+    timestamp = data.columns.to_series().diff()
+    if hasattr(timestamp, "dt"):
+        dt = timestamp.dt.total_seconds()
+    else:
+        dt = timestamp
+
+    return data.diff(axis=1) / dt
 
 
 def _cut(x):
     y = x.copy()
     for i in range(0, y.shape[1] - 1):
         y[:, i] = np.nanmin(y[:, :i + 1], axis=1)
     return y
```

### Comparing `survival_data_handler-2024.4.7/survival_data_handler.egg-info/PKG-INFO` & `survival_data_handler-2024.4.9/survival_data_handler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: survival_data_handler
-Version: 2024.4.7
+Version: 2024.4.9
 Author-email: Vincent Laurent <vlaurent@eurobios.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3
 Requires-Dist: seaborn
 Requires-Dist: numba
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: pandas>2
 Requires-Dist: lifelines
 Requires-Dist: numpy
+Requires-Dist: plotly
 
 # Survival data handler
 ![code coverage](https://raw.githubusercontent.com/eurobios-mews-labs/survival-data-handler/coverage-badge/coverage.svg?raw=true)
 [![PyPI version](https://badge.fury.io/py/palma.svg)](https://badge.fury.io/py/palma)
 
 ```python
 import pandas as pd
```

### Comparing `survival_data_handler-2024.4.7/test/test_main.py` & `survival_data_handler-2024.4.9/test/test_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,27 +45,25 @@
     curves.iloc[:, 1] = 1
     ret = process_survival_function(curves)
     assert any(pd.DataFrame(ret == curves))
 
 
 def test_utils_compute_derivative(data):
     _, curves = data
-    unit = pd.to_timedelta(7, unit="D").total_seconds()
-    ret = compute_derivative(curves, unit)
+    ret = compute_derivative(curves)
     assert all(pd.DataFrame(ret < 0))
 
 
 def test_survival_estimation(data):
     _, curves = data
     se = SurvivalEstimation(
-        curves.drop_duplicates(),
-        unit='D',
-        n_unit=365.25)
+        curves.drop_duplicates())
     se.plot_residual_life()
     se.plot_residual_life(mean_behaviour=False)
+    se.plot_residual_life(sample=10)
 
 
 def test_survival_estimation_attributes(data):
     rossi, curves = data
 
     rossi["index"] = rossi.index
     se = SurvivalEstimation(survival_curves=curves)
@@ -96,15 +94,14 @@
     lifespan.plot_curves_residual_life()
     lifespan.add_supervision(event=rossi["arrest"],
                              durations=pd.to_timedelta(rossi["week"] * 7, unit="D"))
 
     assert isinstance(lifespan.survival_function, pd.DataFrame)
     assert isinstance(lifespan.residual_survival(pd.to_datetime("2022")), pd.DataFrame)
     assert isinstance(lifespan.percentile_life(0.1), pd.DataFrame)
-    assert isinstance(lifespan.residual_expected_life, pd.DataFrame)
     assert isinstance(lifespan.density_function, pd.DataFrame)
     assert isinstance(lifespan.cumulative_hazard_function, pd.DataFrame)
     assert isinstance(lifespan.hazard_function, pd.DataFrame)
     assert isinstance(lifespan.lifetime_distribution_function, pd.DataFrame)
     assert isinstance(lifespan.residual_life, pd.DataFrame)
 
     t = lifespan.compute_times(p=0.5)
@@ -129,16 +126,24 @@
 
     lifespan.compute_confusion_matrix(on="survival_function", threshold=0.2)
     lifespan.plot_average_tagged(on="survival_function")
     lifespan.plot_average_tagged(on="survival_function", plot_test_window=True, plot_type=None)
     lifespan.plot_dist_facet_grid(on="survival_function")
     lifespan.plot_tagged_sample(on="survival_function", n_sample=10)
     lifespan.plot_tagged_sample(on="survival_function", n_sample_pos=10)
-    lifespan.plot_tagged_sample(on="survival_function")
+    lifespan.plot_average_tagged(on="survival_function", event_type="censored")
+    lifespan.plot_average_tagged(on="survival_function", event_type="observed")
+    lifespan.plot_tagged_sample(on="hazard_function")
     test_is_survival_curves(lifespan.survival_function.round(3))
+    lifespan.assess_metric(on="survival_function", method="roc-id")
+    lifespan.assess_metric(on="survival_function", method="roc-cd")
+    lifespan.assess_metric(on="survival_function", method="harrell")
+    lifespan.plotly_roc_curve(on="survival_function")
+    assert lifespan.supervised
+    assert len(lifespan.remove_the_dead(on="survival_function")) <= len(lifespan.survival_function)
 
 
 def test_curve_object(data):
     rossi, curves = data
     tc = TimeCurveData(curves)
     tc_prime = tc.derivative()
     assert isinstance(tc_prime, TimeCurveData)
```

