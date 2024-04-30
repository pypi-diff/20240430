# Comparing `tmp/neighpy-0.1.3.tar.gz` & `tmp/neighpy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neighpy-0.1.3.tar", max compression
+gzip compressed data, was "neighpy-0.1.4.tar", max compression
```

## Comparing `neighpy-0.1.3.tar` & `neighpy-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35420 2024-04-08 01:27:01.766051 neighpy-0.1.3/LICENSE.rst
--rw-r--r--   0        0        0     2445 2024-04-08 01:27:01.766051 neighpy-0.1.3/README.md
--rw-r--r--   0        0        0      100 2024-04-08 01:27:01.810050 neighpy-0.1.3/neighpy/__init__.py
--rw-r--r--   0        0        0     2465 2024-04-08 01:27:01.810050 neighpy-0.1.3/neighpy/_mcintegrals.py
--rw-r--r--   0        0        0      125 2024-04-08 01:27:16.037911 neighpy-0.1.3/neighpy/_version.py
--rw-r--r--   0        0        0    10604 2024-04-08 01:27:01.810050 neighpy-0.1.3/neighpy/appraise.py
--rw-r--r--   0        0        0     5472 2024-04-08 01:27:01.810050 neighpy-0.1.3/neighpy/search.py
--rw-r--r--   0        0        0     1624 2024-04-08 01:27:16.037911 neighpy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3400 1970-01-01 00:00:00.000000 neighpy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35420 2024-04-30 04:49:19.306407 neighpy-0.1.4/LICENSE.rst
+-rw-r--r--   0        0        0     2445 2024-04-30 04:49:19.306407 neighpy-0.1.4/README.md
+-rw-r--r--   0        0        0      100 2024-04-30 04:49:19.350407 neighpy-0.1.4/neighpy/__init__.py
+-rw-r--r--   0        0        0     2465 2024-04-30 04:49:19.350407 neighpy-0.1.4/neighpy/_mcintegrals.py
+-rw-r--r--   0        0        0      125 2024-04-30 04:49:35.158328 neighpy-0.1.4/neighpy/_version.py
+-rw-r--r--   0        0        0    10604 2024-04-30 04:49:19.350407 neighpy-0.1.4/neighpy/appraise.py
+-rw-r--r--   0        0        0     6529 2024-04-30 04:49:19.350407 neighpy-0.1.4/neighpy/search.py
+-rw-r--r--   0        0        0     1624 2024-04-30 04:49:35.154328 neighpy-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3400 1970-01-01 00:00:00.000000 neighpy-0.1.4/PKG-INFO
```

### Comparing `neighpy-0.1.3/LICENSE.rst` & `neighpy-0.1.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `neighpy-0.1.3/README.md` & `neighpy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `neighpy-0.1.3/neighpy/_mcintegrals.py` & `neighpy-0.1.4/neighpy/_mcintegrals.py`

 * *Files identical despite different names*

### Comparing `neighpy-0.1.3/neighpy/appraise.py` & `neighpy-0.1.4/neighpy/appraise.py`

 * *Files identical despite different names*

### Comparing `neighpy-0.1.3/neighpy/search.py` & `neighpy-0.1.4/neighpy/search.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,60 @@
 import numpy as np
 from numpy.typing import NDArray
-from typing import Callable, Tuple
+from typing import Any, Tuple, Protocol
 from joblib import Parallel, delayed
 from tqdm import tqdm
 
 
+class ObjectiveFunction(Protocol):
+    """
+    :meta private:
+    """
+
+    def __call__(self, x: NDArray, *args: Any) -> float:
+        # Any type hint because the objective function supplied by the user can have any signature
+        # as long as its first argument is of type NDArray and returns a float
+        # A type hint of Callable[[NDArray], float] would be too restrictive
+        # A type checker will probably complain about this, but it's the best we can do for now
+        # From python 3.10, we can use ParamSpec to define a generic type hint for the objective
+        # function, and remove this protocol
+        #
+        # Example:
+        # P = ParamSpec("P")
+        # class NASearcher:
+        #     def __init__(self, objective: Callable[Concatenate[NDArray, P], float]):
+        ...
+
+
 class NASearcher:
     """
     Args:
         objective (Callable[[NDArray], float]): The objective function to minimize.
             This function should take a single argument of type NDArray and return a float.
         ns (int): The number of samples generated at each iteration.
         nr (int): The number of cells to resample.
         ni (int): The number of samples from initial random search.
         n (int): The number of iterations.
         bounds (Tuple[Tuple[float, float], ...]): A tuple of tuples representing the bounds of the search space.
             Each inner tuple represents the lower and upper bounds for a specific dimension.
+        args (Tuple, optional): Additional arguments to pass to the objective function.
     """
 
     def __init__(
         self,
-        objective: Callable[[NDArray], float],
+        objective: ObjectiveFunction,
         ns: int,
         nr: int,
         ni: int,
         n: int,
         bounds: Tuple[Tuple[float, float], ...],
+        args: Tuple = (),
     ) -> None:
-        self.objective = objective
+        self._objective = objective
+        self.objective_args = args
 
         self.ns = ns  # number of samples generated at each iteration
         self.nr = nr  # number of cells to resample
         self.nspnr = ns // nr  # number of samples per cell to generate
         self.ni = ni  # number of samples from initial random search
         self.n = n  # number of iterations
         self.nt = ni + n * ns  # total number of samples
@@ -74,14 +97,17 @@
 
             new_samples = Parallel(n_jobs=self.nr if parallel else 1)(
                 delayed(self._random_walk_in_voronoi)(cell, k)
                 for k, cell in zip(inds, cells_to_resample)
             )
             self._update_ensemble(np.concatenate(new_samples))
 
+    def objective(self, x: NDArray) -> float:
+        return self._objective(x, *self.objective_args)
+
     def _initial_random_search(self) -> NDArray:
         return np.random.uniform(
             low=self.lower,
             high=self.upper,
             size=(self.ni, self.nd),
         )
```

### Comparing `neighpy-0.1.3/pyproject.toml` & `neighpy-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neighpy"
-version = "0.1.3"
+version = "0.1.4"
 description = "Neighbourhood Algorithm in Python"
 authors = ["auggiemarignier <augustin.marignier@anu.edu.au>"]
 homepage = "https://github.com/auggiemarignier/neighpy"
 repository = "https://github.com/auggiemarignier/neighpy"
 license = "GPL-3.0-or-later"
 documentation = "https://neighpy.readthedocs.io/en/latest/index.html"
 readme = "README.md"
```

### Comparing `neighpy-0.1.3/PKG-INFO` & `neighpy-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neighpy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Neighbourhood Algorithm in Python
 Home-page: https://github.com/auggiemarignier/neighpy
 License: GPL-3.0-or-later
 Author: auggiemarignier
 Author-email: augustin.marignier@anu.edu.au
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

