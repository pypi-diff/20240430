# Comparing `tmp/timebasedcv-0.0.2.tar.gz` & `tmp/timebasedcv-0.1.0.tar.gz`

## Comparing `timebasedcv-0.0.2.tar` & `timebasedcv-0.1.0.tar`

### file list

```diff
@@ -1,39 +1,13 @@
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/Makefile
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/mkdocs.yml
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/setup.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/.github/dependabot.yaml
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/.github/workflows/check-typos.yaml
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/.github/workflows/deploy-docs.yaml
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/.github/workflows/pre-commit-update.yaml
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/.github/workflows/pull-request.yaml
--rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/docs/contribute.md
--rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/docs/getting-started.md
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/docs/index.md
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/docs/api/splitstate.md
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/docs/api/timebasedsplit.md
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/docs/api/types.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/docs/img/coverage.svg
--rw-r--r--   0        0        0   151367 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/docs/img/cross-validation.png
--rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/docs/img/interrogate-shield.svg
--rw-r--r--   0        0        0    45470 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/docs/img/timebasedcv-logo.png
--rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/docs/img/timebasedcv-logo.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/tests/splitstate_test.py
--rw-r--r--   0        0        0    10296 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/tests/timebasedsplit_test.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/tests/utils/backends_test.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/tests/utils/funcs_test.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/timebasedcv/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/timebasedcv/py.typed
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/timebasedcv/splitstate.py
--rw-r--r--   0        0        0    25081 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/timebasedcv/timebasedsplit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/timebasedcv/utils/__init__.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/timebasedcv/utils/_backends.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/timebasedcv/utils/_funcs.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/timebasedcv/utils/_types.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/LICENSE
--rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/README.md
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8215 2020-02-02 00:00:00.000000 timebasedcv-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 timebasedcv-0.1.0/timebasedcv/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timebasedcv-0.1.0/timebasedcv/py.typed
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 timebasedcv-0.1.0/timebasedcv/splitstate.py
+-rw-r--r--   0        0        0    25430 2020-02-02 00:00:00.000000 timebasedcv-0.1.0/timebasedcv/timebasedsplit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timebasedcv-0.1.0/timebasedcv/utils/__init__.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 timebasedcv-0.1.0/timebasedcv/utils/_backends.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 timebasedcv-0.1.0/timebasedcv/utils/_funcs.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 timebasedcv-0.1.0/timebasedcv/utils/_types.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 timebasedcv-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 timebasedcv-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 timebasedcv-0.1.0/README.md
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 timebasedcv-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 timebasedcv-0.1.0/PKG-INFO
```

### Comparing `timebasedcv-0.0.2/timebasedcv/splitstate.py` & `timebasedcv-0.1.0/timebasedcv/splitstate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import sys
 from dataclasses import dataclass
 from datetime import date, datetime, timedelta
 from operator import le as less_or_equal
 from typing import Generic
 
-import pandas as pd
-
 from timebasedcv.utils._funcs import pairwise, pairwise_comparison
 from timebasedcv.utils._types import DateTimeLike
 
 if sys.version_info >= (3, 11):
     from typing import Self  # pragma: no cover
 else:
     from typing_extensions import Self  # pragma: no cover
 
+from narwhals.dependencies import get_pandas
+
 
 @dataclass(frozen=True)
 class SplitState(Generic[DateTimeLike]):
     """The `SplitState` class represents the state of a split, which is a set of split points where to partition a time
     series into training set and forecast set.
 
     The class ensures that the split is valid by checking that the attributes are of the correct type and are ordered
@@ -53,18 +53,20 @@
         """Post init used to validate the `SplitState` instance attributes."""
 
         # Validate types
         _slots = self.__slots__
         _values = tuple(getattr(self, _attr) for _attr in _slots)
         _types = tuple(type(_value) for _value in _values)
 
+        pd = get_pandas()
+
         if not (
             all(_type is datetime for _type in _types)
             or all(_type is date for _type in _types)
-            or all(_type is pd.Timestamp for _type in _types)
+            or (pd is not None and all(_type is pd.Timestamp for _type in _types))
         ):
             # cfr: https://stackoverflow.com/questions/16991948/detect-if-a-variable-is-a-datetime-object
             raise TypeError("All attributes must be of type `datetime`, `date` or `pd.Timestamp`.")
 
         # Validate order
         _ordered = tuple(pairwise_comparison(_values, less_or_equal))
```

### Comparing `timebasedcv-0.0.2/timebasedcv/timebasedsplit.py` & `timebasedcv-0.1.0/timebasedcv/timebasedsplit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 from datetime import timedelta
 from itertools import chain
 from typing import Generator, Tuple, Union, get_args
 
+import narwhals as nw
 import numpy as np
 
 from timebasedcv.splitstate import SplitState
 from timebasedcv.utils._backends import (
     BACKEND_TO_INDEXING_METHOD,
     default_indexing_method,
 )
@@ -367,14 +368,16 @@
         if n_arrays == 0:
             raise ValueError("At least one array required as input")
 
         ts_shape = time_series.shape
         if len(ts_shape) != 1:
             raise ValueError(f"Time series must be 1-dimensional. Got {len(ts_shape)} dimensions.")
 
+        arrays = tuple([nw.from_native(array, eager_only=True, allow_series=True, strict=False) for array in arrays])
+        time_series = nw.from_native(time_series, series_only=True, strict=False)
         a0 = arrays[0]
         arr_len = a0.shape[0]
 
         if n_arrays > 1 and not all(a.shape[0] == arr_len for a in arrays[1:]):
             raise ValueError(f"All arrays must have the same length. Got {[a.shape[0] for a in arrays]}")
 
         if arr_len != ts_shape[0]:
@@ -389,15 +392,18 @@
         _index_methods = tuple(BACKEND_TO_INDEXING_METHOD.get(_type, default_indexing_method) for _type in _arr_types)
         for split in self._splits_from_period(time_start, time_end):
             train_mask = (time_series >= split.train_start) & (time_series < split.train_end)
             forecast_mask = (time_series >= split.forecast_start) & (time_series < split.forecast_end)
 
             train_forecast_arrays = tuple(
                 chain.from_iterable(
-                    (_idx_method(_arr, train_mask), _idx_method(_arr, forecast_mask))
+                    (
+                        nw.to_native(_idx_method(_arr, train_mask), strict=False),
+                        nw.to_native(_idx_method(_arr, forecast_mask), strict=False),
+                    )
                     for _arr, _idx_method in zip(arrays, _index_methods)
                 )
             )
 
             if return_splitstate:
                 yield train_forecast_arrays, split
             else:
```

### Comparing `timebasedcv-0.0.2/timebasedcv/utils/_funcs.py` & `timebasedcv-0.1.0/timebasedcv/utils/_funcs.py`

 * *Files identical despite different names*

### Comparing `timebasedcv-0.0.2/timebasedcv/utils/_types.py` & `timebasedcv-0.1.0/timebasedcv/utils/_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 import sys
 from datetime import date, datetime
-from typing import Literal, Protocol, Tuple, TypeVar, Union
-
-import pandas as pd
+from typing import TYPE_CHECKING, Literal, Protocol, Tuple, TypeVar, Union
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias  # pragma: no cover
 else:
     from typing_extensions import TypeAlias  # pragma: no cover
 
 if sys.version_info >= (3, 11):
     from typing import Self  # pragma: no cover
 else:
     from typing_extensions import Self  # pragma: no cover
 
-DateTimeLike = TypeVar("DateTimeLike", datetime, date, pd.Timestamp)
+if TYPE_CHECKING:
+    import pandas as pd
+
+
+DateTimeLike = TypeVar("DateTimeLike", datetime, date, "pd.Timestamp")
 FrequencyUnit: TypeAlias = Literal["days", "seconds", "microseconds", "milliseconds", "minutes", "hours", "weeks"]
 WindowType: TypeAlias = Literal["rolling", "expanding"]
 
 T = TypeVar("T")
 
 
 class SeriesLike(Protocol[T]):
@@ -39,40 +41,33 @@
         ...
 
     def max(self: Self) -> T:
         """Support for `.max()` method."""
         ...
 
     @property
-    def shape(self: Self) -> Tuple[int]:
-        ...
+    def shape(self: Self) -> Tuple[int]: ...
 
-    def __lt__(self: Self, other: Union[T, SeriesLike[T]]) -> SeriesLike[bool]:
-        ...
+    def __lt__(self: Self, other: Union[T, SeriesLike[T]]) -> SeriesLike[bool]: ...
 
-    def __gt__(self: Self, other: Union[T, SeriesLike[T]]) -> SeriesLike[bool]:
-        ...
+    def __gt__(self: Self, other: Union[T, SeriesLike[T]]) -> SeriesLike[bool]: ...
 
-    def __le__(self: Self, other: Union[T, SeriesLike[T]]) -> SeriesLike[bool]:
-        ...
+    def __le__(self: Self, other: Union[T, SeriesLike[T]]) -> SeriesLike[bool]: ...
 
-    def __ge__(self: Self, other: Union[T, SeriesLike[T]]) -> SeriesLike[bool]:
-        ...
+    def __ge__(self: Self, other: Union[T, SeriesLike[T]]) -> SeriesLike[bool]: ...
 
-    def __and__(self: SeriesLike[bool], other: SeriesLike[bool]) -> SeriesLike[bool]:
-        ...
+    def __and__(self: SeriesLike[bool], other: SeriesLike[bool]) -> SeriesLike[bool]: ...
 
 
 T_co = TypeVar("T_co", covariant=True)
 
 
 class TensorLike(Protocol[T_co]):
     """TensorLike protocol for type hinting purposes.
 
     This protocol is used to indicate that the class should supports:
 
     - `.shape` attribute
     """
 
     @property
-    def shape(self: Self) -> Tuple[int, ...]:
-        ...
+    def shape(self: Self) -> Tuple[int, ...]: ...
```

### Comparing `timebasedcv-0.0.2/.gitignore` & `timebasedcv-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `timebasedcv-0.0.2/LICENSE` & `timebasedcv-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timebasedcv-0.0.2/README.md` & `timebasedcv-0.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,87 @@
 <img src="docs/img/timebasedcv-logo.svg" width=185 height=185 align="right">
 
-![](https://img.shields.io/github/license/FBruzzesi/timebasedcv)
-<img src ="docs/img/interrogate-shield.svg">
+![license-shield](https://img.shields.io/github/license/FBruzzesi/timebasedcv)
+![interrogate-badge](docs/img/interrogate-shield.svg)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-<img src="docs/img/coverage.svg">
-<img src="https://img.shields.io/pypi/pyversions/timebasedcv">
+![coverage-badge](docs/img/coverage.svg)
+![versions-shield](https://img.shields.io/pypi/pyversions/timebasedcv)
 
 # Time based cross validation
 
 **timebasedcv** is a Python codebase that provides a cross validation strategy based on time.
 
 ---
 
-**Documentation**: https://fbruzzesi.github.io/timebasedcv
-
-**Source Code**: https://github.com/fbruzzesi/timebasedcv
+[Documentation](https://fbruzzesi.github.io/timebasedcv) | [Repository](https://github.com/fbruzzesi/timebasedcv) | [Issue Tracker](https://github.com/fbruzzesi/timebasedcv/issues)
 
 ---
 
 ## Alpha Notice
 
 This codebase is experimental and is working for my use cases. It is very probable that there are cases not covered and for which it breaks (badly). If you find them, please feel free to open an issue in the [issue page](https://github.com/FBruzzesi/timebasedcv/issues) of the repo.
 
 ## Description
 
 The current implementation of [scikit-learn TimeSeriesSplit](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.TimeSeriesSplit.html) lacks the flexibility of having multiple samples within the same time period/unit.
 
-This codebase addresses such problem by providing a cross validation strategy based on a time period rather than the number of samples. This is useful when the data is time dependent, and the model should be trained on past data and tested on future data, independently from the number of observations present within a given time period.
+This codebase addresses such problem by providing a cross validation strategy based on a **time period** rather than the number of samples. This is useful when the data is time dependent, and the model should be trained on past data and tested on future data, independently from the number of observations present within a given time period.
+
+Temporal data leakage is an issue and we want to prevent that from happening!
 
 We introduce two main classes:
 
-- [`TimeBasedSplit`](https://fbruzzesi.github.io/timebasedcv/api/timebasedsplit/#timebasedcv.timebasedsplit.TimeBasedSplit): a class that allows to define a time based split with a given frequency, train size, test size, gap, stride and window type. It's core method `split` requires to pass a time series as input to create the boolean masks for train and test from the instance information defined above. Therefore it is not compatible with [scikit-learn CV Splitters](https://scikit-learn.org/stable/common_pitfalls.html#id3).
-- [`TimeBasedCVSplitter`](https://fbruzzesi.github.io/timebasedcv/api/timebasedsplit/#timebasedcv.timebasedsplit.TimeBasedCVSplitter): a class that conforms with scikit-learn CV Splitters but requires to pass the time series as input to the instance. That is because a CV Splitter needs to know a priori the number of splits and the `split` method shouldn't take any extra arguments as input other than the arrays to split.
+- [`TimeBasedSplit`](https://fbruzzesi.github.io/timebasedcv/api/timebasedsplit/#timebasedcv.timebasedsplit.TimeBasedSplit) allows to define a time based split with a given frequency, train size, test size, gap, stride and window type. Its core method `split` requires to pass a time series as input to create the boolean masks for train and test from the instance information defined above. Therefore it is not compatible with [scikit-learn CV Splitters](https://scikit-learn.org/stable/common_pitfalls.html#id3).
+- [`TimeBasedCVSplitter`](https://fbruzzesi.github.io/timebasedcv/api/timebasedsplit/#timebasedcv.timebasedsplit.TimeBasedCVSplitter) conforms with scikit-learn CV Splitters but requires to pass the time series as input to the instance. That is because a CV Splitter needs to know a priori the number of splits, and the `split` method shouldn't take any extra arguments as input other than the arrays to split.
 
 ## Installation
 
 **timebasedcv** is a published Python package on [pypi](https://pypi.org/), therefore it can be installed directly via pip, as well as from source using pip and git, or with a local clone:
 
-- **pip**: `python -m pip install timebasedcv` (suggested)
-- **pip + source/git**: `python -m pip install git+https://github.com/FBruzzesi/timebasedcv.git`
-- **local clone**:
-
-    ```bash
-    git clone https://github.com/FBruzzesi/timebasedcv.git
-    cd timebasedcv
-    python -m pip install .
-    ```
+<details open>
+
+<summary> <b>pip</b> (suggested)</summary>
+
+```bash
+python -m pip install timebasedcv
+```
+
+</details>
+
+<details closed>
+
+<summary> <b>pip + source/git</b></summary>
+
+```bash
+python -m pip install git+https://github.com/FBruzzesi/timebasedcv.git
+```
+
+</details>
+
+<details closed>
+
+<summary> <b>local clone</b></summary>
+
+```bash
+git clone https://github.com/FBruzzesi/timebasedcv.git
+cd timebasedcv
+python -m pip install .
+```
+
+</details>
+
+## Dependencies
+
+As of **timebasecv v0.1.0**, the only two dependencies are [`numpy`](https://numpy.org/doc/stable/index.html) and [`narwhals>=0.7.15`](https://marcogorelli.github.io/narwhals/).
+
+The latter allows to have a compatibility layer between polars, pandas and other dataframe libraries. Therefore, as long as narwhals supports such dataframe object, we will as well.
 
 ## Quickstart
 
-As a **quickstart**, you can use the following code snippet to get started.
-Consider checkout out the [Getting Started](https://fbruzzesi.github.io/timebasedcv/getting-started/) section of for a detailed guide on how to use the library.
+The following code snippet is all you need to get started, yet consider checking out the [Getting Started](https://fbruzzesi.github.io/timebasedcv/getting-started/) section of the documentation for a detailed guide on how to use the library.
 
 First let's generate some data with different number of points per day:
 
 ```python
 import pandas as pd
 import numpy as np
 np.random.seed(42)
@@ -68,21 +95,23 @@
         "value": np.random.randn(_size-1)/25,
     })
     for start, end, _size in zip(dates[:size], dates[1:], np.random.randint(2, 24, size-1))
 ]).reset_index(drop=True)
 
 time_series, X = df["time"], df["value"]
 df.set_index("time").resample("D").count().head(5)
+```
 
-# time	        value
-# 2023-01-01	14
-# 2023-01-02	2
-# 2023-01-03	22
-# 2023-01-04	11
-# 2023-01-05	1
+```terminal
+time	        value
+2023-01-01	14
+2023-01-02	2
+2023-01-03	22
+2023-01-04	11
+2023-01-05	1
 ```
 
 Now let's run the split with a given frequency, train size, test size, gap, stride and window type:
 
 ```python
 from timebasedcv import TimeBasedSplit
 
@@ -94,30 +123,28 @@
         "gap": 2,
         "stride": 5,
         "window": "expanding"
     },
     ...
 ]
 
-tbs = TimeBasedSplit(
-        **config,
-    )
+tbs = TimeBasedSplit(**config)
 
 
 fmt = "%Y-%m-%d"
 for train_set, forecast_set in tbs.split(X, time_series=time_series):
 
     # Do some magic here
 ```
 
 Let's see how `train_set` and `forecasting_set` splits would look likes for different split strategies (or configurations).
 
-The green dots represent the train points, while the red dots represent the forecastng points.
+The blue dots represent the train points, while the red dots represent the forecastng points.
 
-<img src="docs/img/cross-validation.png" align="center">
+![cross-validation](docs/img/cross-validation.png)
 
 ## Contributing
 
 Please read the [Contributing guidelines](https://fbruzzesi.github.io/timebasedcv/contribute/) in the documentation site.
 
 ## License
```

### Comparing `timebasedcv-0.0.2/pyproject.toml` & `timebasedcv-0.1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "timebasedcv"
-version = "0.0.2"
+version = "0.1.0"
 description = "Time based cross validation"
 
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{name = "Francesco Bruzzesi"}]
 
 dependencies = [
     "numpy",
-    "pandas",
+    "narwhals>=0.7.15",
     "typing-extensions>=4.4.0; python_version < '3.11'",
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -32,23 +32,24 @@
 
 [project.urls]
 documentation = "https://fbruzzesi.github.io/timebasedcv/"
 repository = "https://github.com/fbruzzesi/timebasedcv"
 issue-tracker = "https://github.com/fbruzzesi/timebasedcv/issues"
 
 [project.optional-dependencies]
-polars = ["polars"]
+polars = ["polars>=0.20.3"]
+pandas = ["pandas>=1.2.0"]
 
 dev = [
     "pre-commit==2.21.0",
     "hatch"
 ]
 
 lint = [
-    "ruff>=0.1.0"
+    "ruff>=0.4.0"
 ]
 
 docs = [
     "mkdocs>=1.4.2",
     "mkdocs-material>=9.2.0",
     "mkdocstrings[python]>=0.20.0",
     "mkdocs-autorefs",
@@ -58,27 +59,36 @@
     "interrogate>=1.5.0",
     "pytest==7.2.0",
     "pytest-xdist==3.2.1",
     "coverage==7.2.1",
     "scikit-learn>=0.19",
 ]
 
-all = ["timebasedcv[polars]"]
-all-dev = ["timebasedcv[dev,docs,lint,polars,test]"]
+all = ["timebasedcv[pandas,polars]"]
+all-dev = ["timebasedcv[dev,docs,lint,pandas,polars,test]"]
 
-[tool.setuptools.packages.find]
-include = ["timebasedcv*"]
-exclude = ["docs", "tests", "data", "docker", "results", "notebooks", "kubernetes"]
+[tool.hatch.build.targets.sdist]
+only-include = ["timebasedcv"]
 
-[tool.setuptools.package-data]
-timebasedcv = ["py.typed"]
+[tool.hatch.build.targets.wheel]
+packages = ["timebasedcv"]
 
 [tool.ruff]
 line-length = 120
-extend-select = ["I"]
+
+[tool.ruff.lint]
+extend-select = [
+    "E",
+    "F",
+    "I",
+    # "N",  # pep8-naming
+    "W",
+    "PERF",
+    "RUF",
+]
 ignore = [
     "E731",  # do not assign a `lambda` expression, use a `def`
     ]
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
```

### Comparing `timebasedcv-0.0.2/PKG-INFO` & `timebasedcv-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: timebasedcv
-Version: 0.0.2
+Version: 0.1.0
 Summary: Time based cross validation
 Project-URL: documentation, https://fbruzzesi.github.io/timebasedcv/
 Project-URL: repository, https://github.com/fbruzzesi/timebasedcv
 Project-URL: issue-tracker, https://github.com/fbruzzesi/timebasedcv/issues
 Author: Francesco Bruzzesi
 License: MIT License
         
@@ -34,94 +34,137 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
+Requires-Dist: narwhals>=0.7.15
 Requires-Dist: numpy
-Requires-Dist: pandas
 Requires-Dist: typing-extensions>=4.4.0; python_version < '3.11'
 Provides-Extra: all
-Requires-Dist: timebasedcv[polars]; extra == 'all'
+Requires-Dist: pandas>=1.2.0; extra == 'all'
+Requires-Dist: polars>=0.20.3; extra == 'all'
 Provides-Extra: all-dev
-Requires-Dist: timebasedcv[dev,docs,lint,polars,test]; extra == 'all-dev'
+Requires-Dist: coverage==7.2.1; extra == 'all-dev'
+Requires-Dist: hatch; extra == 'all-dev'
+Requires-Dist: interrogate>=1.5.0; extra == 'all-dev'
+Requires-Dist: mkdocs-autorefs; extra == 'all-dev'
+Requires-Dist: mkdocs-material>=9.2.0; extra == 'all-dev'
+Requires-Dist: mkdocs>=1.4.2; extra == 'all-dev'
+Requires-Dist: mkdocstrings[python]>=0.20.0; extra == 'all-dev'
+Requires-Dist: pandas>=1.2.0; extra == 'all-dev'
+Requires-Dist: polars>=0.20.3; extra == 'all-dev'
+Requires-Dist: pre-commit==2.21.0; extra == 'all-dev'
+Requires-Dist: pytest-xdist==3.2.1; extra == 'all-dev'
+Requires-Dist: pytest==7.2.0; extra == 'all-dev'
+Requires-Dist: ruff>=0.4.0; extra == 'all-dev'
+Requires-Dist: scikit-learn>=0.19; extra == 'all-dev'
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: pre-commit==2.21.0; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs-autorefs; extra == 'docs'
 Requires-Dist: mkdocs-material>=9.2.0; extra == 'docs'
 Requires-Dist: mkdocs>=1.4.2; extra == 'docs'
 Requires-Dist: mkdocstrings[python]>=0.20.0; extra == 'docs'
 Provides-Extra: lint
-Requires-Dist: ruff>=0.1.0; extra == 'lint'
+Requires-Dist: ruff>=0.4.0; extra == 'lint'
+Provides-Extra: pandas
+Requires-Dist: pandas>=1.2.0; extra == 'pandas'
 Provides-Extra: polars
-Requires-Dist: polars; extra == 'polars'
+Requires-Dist: polars>=0.20.3; extra == 'polars'
 Provides-Extra: test
 Requires-Dist: coverage==7.2.1; extra == 'test'
 Requires-Dist: interrogate>=1.5.0; extra == 'test'
 Requires-Dist: pytest-xdist==3.2.1; extra == 'test'
 Requires-Dist: pytest==7.2.0; extra == 'test'
 Requires-Dist: scikit-learn>=0.19; extra == 'test'
 Description-Content-Type: text/markdown
 
 <img src="docs/img/timebasedcv-logo.svg" width=185 height=185 align="right">
 
-![](https://img.shields.io/github/license/FBruzzesi/timebasedcv)
-<img src ="docs/img/interrogate-shield.svg">
+![license-shield](https://img.shields.io/github/license/FBruzzesi/timebasedcv)
+![interrogate-badge](docs/img/interrogate-shield.svg)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-<img src="docs/img/coverage.svg">
-<img src="https://img.shields.io/pypi/pyversions/timebasedcv">
+![coverage-badge](docs/img/coverage.svg)
+![versions-shield](https://img.shields.io/pypi/pyversions/timebasedcv)
 
 # Time based cross validation
 
 **timebasedcv** is a Python codebase that provides a cross validation strategy based on time.
 
 ---
 
-**Documentation**: https://fbruzzesi.github.io/timebasedcv
-
-**Source Code**: https://github.com/fbruzzesi/timebasedcv
+[Documentation](https://fbruzzesi.github.io/timebasedcv) | [Repository](https://github.com/fbruzzesi/timebasedcv) | [Issue Tracker](https://github.com/fbruzzesi/timebasedcv/issues)
 
 ---
 
 ## Alpha Notice
 
 This codebase is experimental and is working for my use cases. It is very probable that there are cases not covered and for which it breaks (badly). If you find them, please feel free to open an issue in the [issue page](https://github.com/FBruzzesi/timebasedcv/issues) of the repo.
 
 ## Description
 
 The current implementation of [scikit-learn TimeSeriesSplit](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.TimeSeriesSplit.html) lacks the flexibility of having multiple samples within the same time period/unit.
 
-This codebase addresses such problem by providing a cross validation strategy based on a time period rather than the number of samples. This is useful when the data is time dependent, and the model should be trained on past data and tested on future data, independently from the number of observations present within a given time period.
+This codebase addresses such problem by providing a cross validation strategy based on a **time period** rather than the number of samples. This is useful when the data is time dependent, and the model should be trained on past data and tested on future data, independently from the number of observations present within a given time period.
+
+Temporal data leakage is an issue and we want to prevent that from happening!
 
 We introduce two main classes:
 
-- [`TimeBasedSplit`](https://fbruzzesi.github.io/timebasedcv/api/timebasedsplit/#timebasedcv.timebasedsplit.TimeBasedSplit): a class that allows to define a time based split with a given frequency, train size, test size, gap, stride and window type. It's core method `split` requires to pass a time series as input to create the boolean masks for train and test from the instance information defined above. Therefore it is not compatible with [scikit-learn CV Splitters](https://scikit-learn.org/stable/common_pitfalls.html#id3).
-- [`TimeBasedCVSplitter`](https://fbruzzesi.github.io/timebasedcv/api/timebasedsplit/#timebasedcv.timebasedsplit.TimeBasedCVSplitter): a class that conforms with scikit-learn CV Splitters but requires to pass the time series as input to the instance. That is because a CV Splitter needs to know a priori the number of splits and the `split` method shouldn't take any extra arguments as input other than the arrays to split.
+- [`TimeBasedSplit`](https://fbruzzesi.github.io/timebasedcv/api/timebasedsplit/#timebasedcv.timebasedsplit.TimeBasedSplit) allows to define a time based split with a given frequency, train size, test size, gap, stride and window type. Its core method `split` requires to pass a time series as input to create the boolean masks for train and test from the instance information defined above. Therefore it is not compatible with [scikit-learn CV Splitters](https://scikit-learn.org/stable/common_pitfalls.html#id3).
+- [`TimeBasedCVSplitter`](https://fbruzzesi.github.io/timebasedcv/api/timebasedsplit/#timebasedcv.timebasedsplit.TimeBasedCVSplitter) conforms with scikit-learn CV Splitters but requires to pass the time series as input to the instance. That is because a CV Splitter needs to know a priori the number of splits, and the `split` method shouldn't take any extra arguments as input other than the arrays to split.
 
 ## Installation
 
 **timebasedcv** is a published Python package on [pypi](https://pypi.org/), therefore it can be installed directly via pip, as well as from source using pip and git, or with a local clone:
 
-- **pip**: `python -m pip install timebasedcv` (suggested)
-- **pip + source/git**: `python -m pip install git+https://github.com/FBruzzesi/timebasedcv.git`
-- **local clone**:
-
-    ```bash
-    git clone https://github.com/FBruzzesi/timebasedcv.git
-    cd timebasedcv
-    python -m pip install .
-    ```
+<details open>
+
+<summary> <b>pip</b> (suggested)</summary>
+
+```bash
+python -m pip install timebasedcv
+```
+
+</details>
+
+<details closed>
+
+<summary> <b>pip + source/git</b></summary>
+
+```bash
+python -m pip install git+https://github.com/FBruzzesi/timebasedcv.git
+```
+
+</details>
+
+<details closed>
+
+<summary> <b>local clone</b></summary>
+
+```bash
+git clone https://github.com/FBruzzesi/timebasedcv.git
+cd timebasedcv
+python -m pip install .
+```
+
+</details>
+
+## Dependencies
+
+As of **timebasecv v0.1.0**, the only two dependencies are [`numpy`](https://numpy.org/doc/stable/index.html) and [`narwhals>=0.7.15`](https://marcogorelli.github.io/narwhals/).
+
+The latter allows to have a compatibility layer between polars, pandas and other dataframe libraries. Therefore, as long as narwhals supports such dataframe object, we will as well.
 
 ## Quickstart
 
-As a **quickstart**, you can use the following code snippet to get started.
-Consider checkout out the [Getting Started](https://fbruzzesi.github.io/timebasedcv/getting-started/) section of for a detailed guide on how to use the library.
+The following code snippet is all you need to get started, yet consider checking out the [Getting Started](https://fbruzzesi.github.io/timebasedcv/getting-started/) section of the documentation for a detailed guide on how to use the library.
 
 First let's generate some data with different number of points per day:
 
 ```python
 import pandas as pd
 import numpy as np
 np.random.seed(42)
@@ -135,21 +178,23 @@
         "value": np.random.randn(_size-1)/25,
     })
     for start, end, _size in zip(dates[:size], dates[1:], np.random.randint(2, 24, size-1))
 ]).reset_index(drop=True)
 
 time_series, X = df["time"], df["value"]
 df.set_index("time").resample("D").count().head(5)
+```
 
-# time	        value
-# 2023-01-01	14
-# 2023-01-02	2
-# 2023-01-03	22
-# 2023-01-04	11
-# 2023-01-05	1
+```terminal
+time	        value
+2023-01-01	14
+2023-01-02	2
+2023-01-03	22
+2023-01-04	11
+2023-01-05	1
 ```
 
 Now let's run the split with a given frequency, train size, test size, gap, stride and window type:
 
 ```python
 from timebasedcv import TimeBasedSplit
 
@@ -161,30 +206,28 @@
         "gap": 2,
         "stride": 5,
         "window": "expanding"
     },
     ...
 ]
 
-tbs = TimeBasedSplit(
-        **config,
-    )
+tbs = TimeBasedSplit(**config)
 
 
 fmt = "%Y-%m-%d"
 for train_set, forecast_set in tbs.split(X, time_series=time_series):
 
     # Do some magic here
 ```
 
 Let's see how `train_set` and `forecasting_set` splits would look likes for different split strategies (or configurations).
 
-The green dots represent the train points, while the red dots represent the forecastng points.
+The blue dots represent the train points, while the red dots represent the forecastng points.
 
-<img src="docs/img/cross-validation.png" align="center">
+![cross-validation](docs/img/cross-validation.png)
 
 ## Contributing
 
 Please read the [Contributing guidelines](https://fbruzzesi.github.io/timebasedcv/contribute/) in the documentation site.
 
 ## License
```

