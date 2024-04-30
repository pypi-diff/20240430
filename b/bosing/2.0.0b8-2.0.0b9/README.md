# Comparing `tmp/bosing-2.0.0b8.tar.gz` & `tmp/bosing-2.0.0b9.tar.gz`

## Comparing `bosing-2.0.0b8.tar` & `bosing-2.0.0b9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 bosing-2.0.0b8/Cargo.toml
--rw-r--r--   0     1001      127      505 2024-04-29 09:00:49.000000 bosing-2.0.0b8/.github/dependabot.yml
--rw-r--r--   0     1001      127     6323 2024-04-29 09:00:49.000000 bosing-2.0.0b8/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      696 2024-04-29 09:00:49.000000 bosing-2.0.0b8/.gitignore
--rw-r--r--   0     1001      127      972 2024-04-29 09:00:49.000000 bosing-2.0.0b8/.readthedocs.yaml
--rw-r--r--   0     1001      127     1068 2024-04-29 09:00:49.000000 bosing-2.0.0b8/LICENSE.txt
--rw-r--r--   0     1001      127     1360 2024-04-29 09:00:49.000000 bosing-2.0.0b8/README.md
--rw-r--r--   0     1001      127    10422 2024-04-29 09:00:49.000000 bosing-2.0.0b8/bosing.pyi
--rw-r--r--   0     1001      127       78 2024-04-29 09:00:49.000000 bosing-2.0.0b8/clippy.toml
--rw-r--r--   0     1001      127      634 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/Makefile
--rw-r--r--   0     1001      127      175 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      127     1147 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/_templates/autosummary/module.rst
--rw-r--r--   0     1001      127       82 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/api.rst
--rw-r--r--   0     1001      127     1464 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/conf.py
--rw-r--r--   0     1001      127     1258 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/index.rst
--rw-r--r--   0     1001      127     1716 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/instruction.rst
--rw-r--r--   0     1001      127      765 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/make.bat
--rw-r--r--   0     1001      127      347 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/quickstart.rst
--rw-r--r--   0     1001      127       22 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/requirements.txt
--rw-r--r--   0     1001      127     5534 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/schedule.rst
--rw-r--r--   0     1001      127     1171 2024-04-29 09:00:49.000000 bosing-2.0.0b8/example/flexible.py
--rw-r--r--   0     1001      127      533 2024-04-29 09:00:49.000000 bosing-2.0.0b8/example/hann.py
--rw-r--r--   0     1001      127      788 2024-04-29 09:00:49.000000 bosing-2.0.0b8/example/interp.py
--rw-r--r--   0     1001      127      696 2024-04-29 09:00:49.000000 bosing-2.0.0b8/example/overlap.py
--rw-r--r--   0     1001      127     2074 2024-04-29 09:00:49.000000 bosing-2.0.0b8/example/schedule.py
--rw-r--r--   0     1001      127     1956 2024-04-29 09:00:49.000000 bosing-2.0.0b8/example/schedule_stress.py
--rw-r--r--   0     1001      127     6064 2024-04-29 09:00:49.000000 bosing-2.0.0b8/ruff_defaults.toml
--rw-r--r--   0     1001      127     7368 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/executor.rs
--rw-r--r--   0     1001      127    63728 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/lib.rs
--rw-r--r--   0     1001      127    12363 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/pulse.rs
--rw-r--r--   0     1001      127     1667 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/quant.rs
--rw-r--r--   0     1001      127     2481 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/schedule/absolute.rs
--rw-r--r--   0     1001      127     7389 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/schedule/grid.rs
--rw-r--r--   0     1001      127     3326 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/schedule/play.rs
--rw-r--r--   0     1001      127     2350 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/schedule/repeat.rs
--rw-r--r--   0     1001      127     3966 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/schedule/simple.rs
--rw-r--r--   0     1001      127     5760 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/schedule/stack.rs
--rw-r--r--   0     1001      127    11084 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/schedule.rs
--rw-r--r--   0     1001      127     6642 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/shape.rs
--rw-r--r--   0     1001      127       14 2024-04-29 09:00:49.000000 bosing-2.0.0b8/stubtest-allowlist.txt
--rw-r--r--   0     1001      127        0 2024-04-29 09:00:49.000000 bosing-2.0.0b8/tests/__init__.py
--rw-r--r--   0     1001      127     1291 2024-04-29 09:00:49.000000 bosing-2.0.0b8/tests/test_basic.py
--rw-r--r--   0     1001      127    18617 2024-04-29 09:01:00.000000 bosing-2.0.0b8/Cargo.lock
--rw-r--r--   0     1001      127     1867 2024-04-29 09:00:49.000000 bosing-2.0.0b8/pyproject.toml
--rw-r--r--   0        0        0     2230 1970-01-01 00:00:00.000000 bosing-2.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 bosing-2.0.0b9/Cargo.toml
+-rw-r--r--   0     1001      127      505 2024-04-29 16:20:07.000000 bosing-2.0.0b9/.github/dependabot.yml
+-rw-r--r--   0     1001      127     6323 2024-04-29 16:20:07.000000 bosing-2.0.0b9/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      696 2024-04-29 16:20:07.000000 bosing-2.0.0b9/.gitignore
+-rw-r--r--   0     1001      127      972 2024-04-29 16:20:07.000000 bosing-2.0.0b9/.readthedocs.yaml
+-rw-r--r--   0     1001      127     1068 2024-04-29 16:20:07.000000 bosing-2.0.0b9/LICENSE.txt
+-rw-r--r--   0     1001      127     1360 2024-04-29 16:20:07.000000 bosing-2.0.0b9/README.md
+-rw-r--r--   0     1001      127    10696 2024-04-29 16:20:07.000000 bosing-2.0.0b9/bosing.pyi
+-rw-r--r--   0     1001      127       78 2024-04-29 16:20:07.000000 bosing-2.0.0b9/clippy.toml
+-rw-r--r--   0     1001      127      634 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/Makefile
+-rw-r--r--   0     1001      127      175 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      127     1147 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/_templates/autosummary/module.rst
+-rw-r--r--   0     1001      127       82 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/api.rst
+-rw-r--r--   0     1001      127     1464 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/conf.py
+-rw-r--r--   0     1001      127     1258 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/index.rst
+-rw-r--r--   0     1001      127     1716 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/instruction.rst
+-rw-r--r--   0     1001      127      765 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/make.bat
+-rw-r--r--   0     1001      127      347 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/quickstart.rst
+-rw-r--r--   0     1001      127       22 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/requirements.txt
+-rw-r--r--   0     1001      127     5534 2024-04-29 16:20:07.000000 bosing-2.0.0b9/docs/schedule.rst
+-rw-r--r--   0     1001      127     1171 2024-04-29 16:20:07.000000 bosing-2.0.0b9/example/flexible.py
+-rw-r--r--   0     1001      127      533 2024-04-29 16:20:07.000000 bosing-2.0.0b9/example/hann.py
+-rw-r--r--   0     1001      127      788 2024-04-29 16:20:07.000000 bosing-2.0.0b9/example/interp.py
+-rw-r--r--   0     1001      127      696 2024-04-29 16:20:07.000000 bosing-2.0.0b9/example/overlap.py
+-rw-r--r--   0     1001      127     2074 2024-04-29 16:20:07.000000 bosing-2.0.0b9/example/schedule.py
+-rw-r--r--   0     1001      127     2329 2024-04-29 16:20:07.000000 bosing-2.0.0b9/example/schedule_stress.py
+-rw-r--r--   0     1001      127     6064 2024-04-29 16:20:07.000000 bosing-2.0.0b9/ruff_defaults.toml
+-rw-r--r--   0     1001      127     7368 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/executor.rs
+-rw-r--r--   0     1001      127    66930 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/lib.rs
+-rw-r--r--   0     1001      127    12363 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/pulse.rs
+-rw-r--r--   0     1001      127     1667 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/quant.rs
+-rw-r--r--   0     1001      127     2481 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/schedule/absolute.rs
+-rw-r--r--   0     1001      127     7389 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/schedule/grid.rs
+-rw-r--r--   0     1001      127     3326 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/schedule/play.rs
+-rw-r--r--   0     1001      127     2350 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/schedule/repeat.rs
+-rw-r--r--   0     1001      127     3966 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/schedule/simple.rs
+-rw-r--r--   0     1001      127     5760 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/schedule/stack.rs
+-rw-r--r--   0     1001      127    11084 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/schedule.rs
+-rw-r--r--   0     1001      127     6642 2024-04-29 16:20:07.000000 bosing-2.0.0b9/src/shape.rs
+-rw-r--r--   0     1001      127       14 2024-04-29 16:20:07.000000 bosing-2.0.0b9/stubtest-allowlist.txt
+-rw-r--r--   0     1001      127        0 2024-04-29 16:20:07.000000 bosing-2.0.0b9/tests/__init__.py
+-rw-r--r--   0     1001      127     1291 2024-04-29 16:20:07.000000 bosing-2.0.0b9/tests/test_basic.py
+-rw-r--r--   0     1001      127    18617 2024-04-29 16:20:12.000000 bosing-2.0.0b9/Cargo.lock
+-rw-r--r--   0     1001      127     1863 2024-04-29 16:20:07.000000 bosing-2.0.0b9/pyproject.toml
+-rw-r--r--   0        0        0     2251 1970-01-01 00:00:00.000000 bosing-2.0.0b9/PKG-INFO
```

### Comparing `bosing-2.0.0b8/Cargo.toml` & `bosing-2.0.0b9/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "bosing"
-version = "2.0.0-beta.8"
+version = "2.0.0-beta.9"
 edition = "2021"
 license = "MIT"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "bosing"
 crate-type = ["cdylib"]
```

### Comparing `bosing-2.0.0b8/.github/workflows/ci.yml` & `bosing-2.0.0b9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/.gitignore` & `bosing-2.0.0b9/.gitignore`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/.readthedocs.yaml` & `bosing-2.0.0b9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/LICENSE.txt` & `bosing-2.0.0b9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/README.md` & `bosing-2.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/bosing.pyi` & `bosing-2.0.0b9/bosing.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,39 @@
         base_freq: float,
         sample_rate: float,
         length: int,
         *,
         delay: float = ...,
         align_level: int = ...,
         iq_matrix: npt.ArrayLike | None = ...,
-        iq_offset: tuple[float, float] | None = ...,
+        iq_offset: tuple[float, float] = ...,
+        iir: npt.ArrayLike | None = ...,
+        fir: npt.ArrayLike | None = ...,
+        filter_offset: bool = ...,
     ) -> Self: ...
     @property
     def base_freq(self) -> float: ...
     @property
     def sample_rate(self) -> float: ...
     @property
     def length(self) -> int: ...
     @property
     def delay(self) -> float: ...
     @property
     def align_level(self) -> int: ...
     @property
     def iq_matrix(self) -> np.ndarray | None: ...
     @property
-    def iq_offset(self) -> tuple[float, float] | None: ...
+    def iq_offset(self) -> tuple[float, float]: ...
+    @property
+    def iir(self) -> np.ndarray | None: ...
+    @property
+    def fir(self) -> np.ndarray | None: ...
+    @property
+    def filter_offset(self) -> bool: ...
 
 @final
 class Alignment:
     End: ClassVar[Alignment]
     Start: ClassVar[Alignment]
     Center: ClassVar[Alignment]
     Stretch: ClassVar[Alignment]
```

### Comparing `bosing-2.0.0b8/docs/Makefile` & `bosing-2.0.0b9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/docs/_templates/autosummary/module.rst` & `bosing-2.0.0b9/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/docs/conf.py` & `bosing-2.0.0b9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/docs/index.rst` & `bosing-2.0.0b9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/docs/instruction.rst` & `bosing-2.0.0b9/docs/instruction.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/docs/make.bat` & `bosing-2.0.0b9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/docs/schedule.rst` & `bosing-2.0.0b9/docs/schedule.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/example/flexible.py` & `bosing-2.0.0b9/example/flexible.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/example/hann.py` & `bosing-2.0.0b9/example/hann.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/example/interp.py` & `bosing-2.0.0b9/example/interp.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/example/overlap.py` & `bosing-2.0.0b9/example/overlap.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/example/schedule.py` & `bosing-2.0.0b9/example/schedule.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/example/schedule_stress.py` & `bosing-2.0.0b9/example/schedule_stress.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 """An example of using bosing to generate a pulse sequence."""
 
 import time
 from itertools import cycle
 
 import numpy as np
+from scipy import signal
 from scipy.interpolate import make_interp_spline
 
 from bosing import Absolute, Barrier, Channel, Hann, Interp, Play, Stack, generate_waveforms
 
 
+def get_biquad(amp, tau, fs):
+    z = [-1 / (t * (1 + a)) for (a, t) in zip(amp, tau)]
+    p = [-1 / t for t in tau]
+    k = np.prod([1 + a for a in amp])
+    z, p, k = signal.bilinear_zpk(z, p, k, fs)
+    return signal.zpk2sos(p, z, 1 / k)
+
+
 def gen_n(n: int):
     t0 = time.perf_counter()
     nxy = 64
     nu = 2 * nxy
     nm = nxy // 8
+    iir = get_biquad([0.1, -0.1], [100e-9, 1e-6], 2e9)
+    fir = [1, 0.1, 0.01, 0.001]
     channels = (
         {f"xy{i}": Channel(3e6 * i, 2e9, 100000, iq_matrix=[[1, 0.1], [0.1, 1]]) for i in range(nxy)}
-        | {f"u{i}": Channel(0, 2e9, 100000) for i in range(nu)}
+        | {f"u{i}": Channel(0, 2e9, 100000, iir=iir, fir=fir) for i in range(nu)}
         | {f"m{i}": Channel(0, 2e9, 100000) for i in range(nm)}
     )
     halfcos = np.sin(np.linspace(0, np.pi, 10))
     spline = make_interp_spline(np.linspace(-0.5, 0.5, 10), halfcos)
     shapes = {
         "hann": Hann(),
         "halfcos": Interp(spline.t, spline.c, spline.k),
```

### Comparing `bosing-2.0.0b8/ruff_defaults.toml` & `bosing-2.0.0b9/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/src/executor.rs` & `bosing-2.0.0b9/src/executor.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/src/lib.rs` & `bosing-2.0.0b9/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 //! Although Element struct may contains [`Py<Element>`] as children, it is not
 //! possible to create cyclic references because we don't allow mutate the
 //! children after creation.
 use std::sync::Arc;
 
 use hashbrown::HashMap;
 use indoc::indoc;
-use numpy::{dot_bound, prelude::*, pyarray_bound, AllowTypeChange, PyArray2, PyArrayLike2};
+use numpy::{
+    dot_bound, prelude::*, pyarray_bound, AllowTypeChange, PyArray1, PyArray2, PyArrayLike1,
+    PyArrayLike2,
+};
 use pyo3::{
     exceptions::{PyRuntimeError, PyTypeError, PyValueError},
     prelude::*,
     types::PyDict,
 };
 
 use crate::{
@@ -37,59 +40,105 @@
 ///     length (int): Length of the waveform.
 ///     delay (float): Delay of the channel. Defaults to 0.0.
 ///     align_level (int): Time axis alignment granularity. Defaults to -10.
 ///     iq_matrix (array_like[2, 2] | None): IQ matrix of the channel. Defaults
 ///         to None.
 ///     iq_offset (tuple[float, float]): IQ offset of the channel. Defaults to
 ///         (0.0, 0.0).
+///     iir (array_like[N, 6] | None): IIR filter of the channel. The format of
+///         the array is ``[[b0, b1, b2, a0, a1, a2], ...]``, which is the same
+///         as `sos` parameter of :func:`scipy.signal.sosfilt`. Defaults to None.
+///     fir (array_like[M] | None): FIR filter of the channel. Defaults to None.
+///     filter_offset (bool): Whether to apply filter to the offset. Defaults to
+///         False.
 #[pyclass(get_all, frozen)]
 #[derive(Debug, Clone)]
 struct Channel {
     base_freq: f64,
     sample_rate: f64,
     length: usize,
     delay: f64,
     align_level: i32,
     iq_matrix: Option<Py<PyArray2<f64>>>,
     iq_offset: (f64, f64),
+    iir: Option<Py<PyArray2<f64>>>,
+    fir: Option<Py<PyArray1<f64>>>,
+    filter_offset: bool,
 }
 
 #[pymethods]
 impl Channel {
     #[new]
-    #[pyo3(signature = (base_freq, sample_rate, length, *, delay=0.0, align_level=-10, iq_matrix=None, iq_offset=(0.0, 0.0)))]
+    #[pyo3(signature = (
+        base_freq,
+        sample_rate,
+        length,
+        *,
+        delay=0.0,
+        align_level=-10,
+        iq_matrix=None,
+        iq_offset=(0.0, 0.0),
+        iir=None,
+        fir=None,
+        filter_offset=false,
+    ))]
     fn new(
         py: Python<'_>,
         base_freq: f64,
         sample_rate: f64,
         length: usize,
         delay: f64,
         align_level: i32,
         iq_matrix: Option<PyArrayLike2<f64, AllowTypeChange>>,
         iq_offset: (f64, f64),
+        iir: Option<PyArrayLike2<f64, AllowTypeChange>>,
+        fir: Option<PyArrayLike1<f64, AllowTypeChange>>,
+        filter_offset: bool,
     ) -> PyResult<Self> {
         let iq_matrix = if let Some(iq_matrix) = iq_matrix {
             if iq_matrix.shape() != [2, 2] {
                 return Err(PyValueError::new_err("iq_matrix should be a 2x2 matrix"));
             }
             let kwargs = PyDict::new_bound(py);
             kwargs.set_item("write", false)?;
             iq_matrix.getattr("setflags")?.call((), Some(&kwargs))?;
             Some(Bound::clone(&iq_matrix).unbind())
         } else {
             None
         };
+        let iir = if let Some(iir) = iir {
+            if !matches!(iir.shape(), [_, 6]) {
+                return Err(PyValueError::new_err("iir should be a Nx6 matrix"));
+            }
+            let kwargs = PyDict::new_bound(py);
+            kwargs.set_item("write", false)?;
+            iir.getattr("setflags")?.call((), Some(&kwargs))?;
+            Some(Bound::clone(&iir).unbind())
+        } else {
+            None
+        };
+        let fir = if let Some(fir) = fir {
+            let kwargs = PyDict::new_bound(py);
+            kwargs.set_item("write", false)?;
+            fir.getattr("setflags")?.call((), Some(&kwargs))?;
+            Some(Bound::clone(&fir).unbind())
+        } else {
+            None
+        };
         Ok(Channel {
             base_freq,
             sample_rate,
             length,
             delay,
             align_level,
             iq_matrix,
             iq_offset,
+            iir,
+            fir,
+            filter_offset,
         })
     }
 }
 
 /// Alignment of a schedule element.
 ///
 /// The alignment of a schedule element is used to align the element within its
@@ -2051,56 +2100,119 @@
     }
     executor.execute(&arranged);
     let results = executor.into_result();
     let waveforms: HashMap<String, Bound<PyArray2<f64>>> = channels
         .iter()
         .map(|(n, c)| (n.clone(), PyArray2::zeros_bound(py, (2, c.length), false)))
         .collect();
-    let mut sampler = Sampler::new(results);
-    for (n, c) in &channels {
-        // SAFETY: These arrays are just created.
-        let array = unsafe { waveforms[n].as_array_mut() };
-        sampler.add_channel(
-            n.clone(),
-            array,
-            Frequency::new(c.sample_rate).unwrap(),
-            Time::new(c.delay).unwrap(),
-            c.align_level,
-        );
-    }
-    if let Some((crosstalk, names)) = &crosstalk {
-        sampler.set_crosstalk(crosstalk.as_array(), names.clone());
+    {
+        let mut sampler = Sampler::new(results);
+        for (n, c) in &channels {
+            // SAFETY: These arrays are just created.
+            let array = unsafe { waveforms[n].as_array_mut() };
+            sampler.add_channel(
+                n.clone(),
+                array,
+                Frequency::new(c.sample_rate).unwrap(),
+                Time::new(c.delay).unwrap(),
+                c.align_level,
+            );
+        }
+        if let Some((crosstalk, names)) = &crosstalk {
+            sampler.set_crosstalk(crosstalk.as_array(), names.clone());
+        }
+        sampler.sample(time_tolerance);
     }
-    sampler.sample(time_tolerance);
     let waveforms = waveforms
         .into_iter()
         .map(|(n, mut w)| {
             let c = &channels[&n];
             if let Some(iq_matrix) = &c.iq_matrix {
                 w = dot_bound(iq_matrix.bind(py), &w)?;
             }
-            if c.iq_offset.0 != 0.0 || c.iq_offset.1 != 0.0 {
-                let locals = PyDict::new_bound(py);
-                locals.set_item("w", w.clone())?;
-                locals.set_item("offset", pyarray_bound![py, c.iq_offset.0, c.iq_offset.1])?;
-                py.run_bound(
-                    indoc! {"
-                        import numpy as np
-                        w += offset[:, np.newaxis]
-                    "},
-                    None,
-                    Some(&locals),
-                )?;
+            if c.filter_offset {
+                apply_offset(py, &w, c.iq_offset)?;
+                if let Some(iir) = &c.iir {
+                    apply_iir(py, &w, iir.bind(py))?;
+                }
+                if let Some(fir) = &c.fir {
+                    apply_fir(py, &w, fir.bind(py))?;
+                }
+            } else {
+                if let Some(iir) = &c.iir {
+                    apply_iir(py, &w, iir.bind(py))?;
+                }
+                if let Some(fir) = &c.fir {
+                    apply_fir(py, &w, fir.bind(py))?;
+                }
+                apply_offset(py, &w, c.iq_offset)?;
             }
             Ok((n, w.unbind()))
         })
         .collect::<PyResult<_>>()?;
     Ok(waveforms)
 }
 
+fn apply_offset(py: Python<'_>, w: &Bound<'_, PyArray2<f64>>, offset: (f64, f64)) -> PyResult<()> {
+    if offset.0 == 0.0 && offset.1 == 0.0 {
+        return Ok(());
+    }
+    let locals = PyDict::new_bound(py);
+    locals.set_item("w", w)?;
+    locals.set_item("offset", pyarray_bound![py, offset.0, offset.1])?;
+    py.run_bound(
+        indoc! {"
+            import numpy as np
+            w += offset[:, np.newaxis]
+        "},
+        None,
+        Some(&locals),
+    )?;
+    Ok(())
+}
+
+fn apply_iir<'py>(
+    py: Python<'py>,
+    w: &Bound<'py, PyArray2<f64>>,
+    iir: &Bound<'py, PyArray2<f64>>,
+) -> PyResult<()> {
+    let locals = PyDict::new_bound(py);
+    locals.set_item("w", w)?;
+    locals.set_item("iir", iir)?;
+    py.run_bound(
+        indoc! {"
+            from scipy import signal
+            w[:] = signal.sosfilt(np.array(iir), w)
+        "},
+        None,
+        Some(&locals),
+    )?;
+    Ok(())
+}
+
+fn apply_fir<'py>(
+    py: Python<'py>,
+    w: &Bound<'py, PyArray2<f64>>,
+    fir: &Bound<'py, PyArray1<f64>>,
+) -> PyResult<()> {
+    let locals = PyDict::new_bound(py);
+    locals.set_item("w", w)?;
+    locals.set_item("fir", fir)?;
+    py.run_bound(
+        indoc! {"
+            from scipy import signal
+            for wi in w:
+                wi[:] = signal.convolve(wi, fir, mode='full')[:len(wi)]
+        "},
+        None,
+        Some(&locals),
+    )?;
+    Ok(())
+}
+
 /// Generates microwave pulses for superconducting quantum computing
 /// experiments.
 ///
 /// .. caution::
 ///
 ///     The unit of phase is number of cycles, not radians. For example, a phase
 ///     of :math:`0.5` means a phase shift of :math:`\pi` radians.
```

### Comparing `bosing-2.0.0b8/src/pulse.rs` & `bosing-2.0.0b9/src/pulse.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/src/quant.rs` & `bosing-2.0.0b9/src/quant.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/src/schedule/absolute.rs` & `bosing-2.0.0b9/src/schedule/absolute.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/src/schedule/grid.rs` & `bosing-2.0.0b9/src/schedule/grid.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/src/schedule/play.rs` & `bosing-2.0.0b9/src/schedule/play.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/src/schedule/repeat.rs` & `bosing-2.0.0b9/src/schedule/repeat.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/src/schedule/simple.rs` & `bosing-2.0.0b9/src/schedule/simple.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/src/schedule/stack.rs` & `bosing-2.0.0b9/src/schedule/stack.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/src/schedule.rs` & `bosing-2.0.0b9/src/schedule.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/src/shape.rs` & `bosing-2.0.0b9/src/shape.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/tests/test_basic.py` & `bosing-2.0.0b9/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b8/Cargo.lock` & `bosing-2.0.0b9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bosing"
-version = "2.0.0-beta.8"
+version = "2.0.0-beta.9"
 dependencies = [
  "anyhow",
  "bspline",
  "cached",
  "enum_dispatch",
  "float-cmp",
  "hashbrown",
```

### Comparing `bosing-2.0.0b8/pyproject.toml` & `bosing-2.0.0b9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,27 @@
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "License :: OSI Approved :: MIT License",
 ]
-dependencies = ["numpy"]
+dependencies = ["numpy", "scipy"]
 
 [project.urls]
 Documentation = "https://bosing.readthedocs.io"
 Issues = "https://github.com/kahojyun/Bosing/issues"
 Source = "https://github.com/kahojyun/Bosing"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 
 [tool.hatch.envs.default]
 dependencies = [
     "maturin>=1.5,<2.0",
-    "scipy",
     "matplotlib",
     "ipython",
     "sphinx",
     "furo",
     "mypy",
 ]
```

### Comparing `bosing-2.0.0b8/PKG-INFO` & `bosing-2.0.0b9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.3
 Name: bosing
-Version: 2.0.0b8
+Version: 2.0.0b9
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy
+Requires-Dist: scipy
 License-File: LICENSE.txt
 Summary: Waveform generator for pulse sequences in quantum computing
 Keywords: 
 Author-email: kaho <kaho0769@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

