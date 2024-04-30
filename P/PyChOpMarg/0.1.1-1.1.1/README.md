# Comparing `tmp/PyChOpMarg-0.1.1.tar.gz` & `tmp/pychopmarg-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyChOpMarg-0.1.1.tar", last modified: Mon Mar 25 00:14:54 2024, max compression
+gzip compressed data, was "pychopmarg-1.1.1.tar", last modified: Tue Apr 30 11:31:51 2024, max compression
```

## Comparing `PyChOpMarg-0.1.1.tar` & `pychopmarg-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-03-25 00:14:54.908678 PyChOpMarg-0.1.1/
--rw-r--r--   0 dbanas     (501) staff       (20)     1498 2024-03-03 12:34:25.000000 PyChOpMarg-0.1.1/LICENSE
--rw-r--r--   0 dbanas     (501) staff       (20)     1433 2024-03-25 00:14:54.908487 PyChOpMarg-0.1.1/PKG-INFO
--rw-r--r--   0 dbanas     (501) staff       (20)       75 2024-03-03 12:34:25.000000 PyChOpMarg-0.1.1/README.md
--rw-r--r--   0 dbanas     (501) staff       (20)     2296 2024-03-25 00:10:39.000000 PyChOpMarg-0.1.1/pyproject.toml
--rw-r--r--   0 dbanas     (501) staff       (20)       38 2024-03-25 00:14:54.908712 PyChOpMarg-0.1.1/setup.cfg
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-03-25 00:14:54.905696 PyChOpMarg-0.1.1/src/
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-03-25 00:14:54.908308 PyChOpMarg-0.1.1/src/PyChOpMarg.egg-info/
--rw-r--r--   0 dbanas     (501) staff       (20)     1433 2024-03-25 00:14:54.000000 PyChOpMarg-0.1.1/src/PyChOpMarg.egg-info/PKG-INFO
--rw-r--r--   0 dbanas     (501) staff       (20)      362 2024-03-25 00:14:54.000000 PyChOpMarg-0.1.1/src/PyChOpMarg.egg-info/SOURCES.txt
--rw-r--r--   0 dbanas     (501) staff       (20)        1 2024-03-25 00:14:54.000000 PyChOpMarg-0.1.1/src/PyChOpMarg.egg-info/dependency_links.txt
--rw-r--r--   0 dbanas     (501) staff       (20)       50 2024-03-25 00:14:54.000000 PyChOpMarg-0.1.1/src/PyChOpMarg.egg-info/entry_points.txt
--rw-r--r--   0 dbanas     (501) staff       (20)       28 2024-03-25 00:14:54.000000 PyChOpMarg-0.1.1/src/PyChOpMarg.egg-info/requires.txt
--rw-r--r--   0 dbanas     (501) staff       (20)       11 2024-03-25 00:14:54.000000 PyChOpMarg-0.1.1/src/PyChOpMarg.egg-info/top_level.txt
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-03-25 00:14:54.908028 PyChOpMarg-0.1.1/src/pychopmarg/
--rw-r--r--   0 dbanas     (501) staff       (20)        0 2024-03-03 13:52:47.000000 PyChOpMarg-0.1.1/src/pychopmarg/__init__.py
--rw-r--r--   0 dbanas     (501) staff       (20)    35096 2024-03-24 23:58:06.000000 PyChOpMarg-0.1.1/src/pychopmarg/com.py
--rw-r--r--   0 dbanas     (501) staff       (20)      695 2024-03-24 23:59:53.000000 PyChOpMarg-0.1.1/src/pychopmarg/common.py
--rw-r--r--   0 dbanas     (501) staff       (20)     6895 2024-03-25 00:01:02.000000 PyChOpMarg-0.1.1/src/pychopmarg/utility.py
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-04-30 11:31:51.619740 pychopmarg-1.1.1/
+-rw-r--r--   0 dbanas     (501) staff       (20)     1498 2024-03-03 12:34:25.000000 pychopmarg-1.1.1/LICENSE
+-rw-r--r--   0 dbanas     (501) staff       (20)     1578 2024-04-30 11:31:51.619576 pychopmarg-1.1.1/PKG-INFO
+-rw-r--r--   0 dbanas     (501) staff       (20)       75 2024-03-03 12:34:25.000000 pychopmarg-1.1.1/README.md
+-rw-r--r--   0 dbanas     (501) staff       (20)     2381 2024-04-30 11:31:32.000000 pychopmarg-1.1.1/pyproject.toml
+-rw-r--r--   0 dbanas     (501) staff       (20)       38 2024-04-30 11:31:51.619770 pychopmarg-1.1.1/setup.cfg
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-04-30 11:31:51.617652 pychopmarg-1.1.1/src/
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-04-30 11:31:51.619415 pychopmarg-1.1.1/src/PyChOpMarg.egg-info/
+-rw-r--r--   0 dbanas     (501) staff       (20)     1578 2024-04-30 11:31:51.000000 pychopmarg-1.1.1/src/PyChOpMarg.egg-info/PKG-INFO
+-rw-r--r--   0 dbanas     (501) staff       (20)      407 2024-04-30 11:31:51.000000 pychopmarg-1.1.1/src/PyChOpMarg.egg-info/SOURCES.txt
+-rw-r--r--   0 dbanas     (501) staff       (20)        1 2024-04-30 11:31:51.000000 pychopmarg-1.1.1/src/PyChOpMarg.egg-info/dependency_links.txt
+-rw-r--r--   0 dbanas     (501) staff       (20)       50 2024-04-30 11:31:51.000000 pychopmarg-1.1.1/src/PyChOpMarg.egg-info/entry_points.txt
+-rw-r--r--   0 dbanas     (501) staff       (20)       55 2024-04-30 11:31:51.000000 pychopmarg-1.1.1/src/PyChOpMarg.egg-info/requires.txt
+-rw-r--r--   0 dbanas     (501) staff       (20)       11 2024-04-30 11:31:51.000000 pychopmarg-1.1.1/src/PyChOpMarg.egg-info/top_level.txt
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-04-30 11:31:51.619257 pychopmarg-1.1.1/src/pychopmarg/
+-rw-r--r--   0 dbanas     (501) staff       (20)      567 2024-04-14 15:14:28.000000 pychopmarg-1.1.1/src/pychopmarg/__init__.py
+-rw-r--r--   0 dbanas     (501) staff       (20)     1556 2024-04-14 15:03:46.000000 pychopmarg-1.1.1/src/pychopmarg/cli.py
+-rw-r--r--   0 dbanas     (501) staff       (20)    48717 2024-04-30 11:15:33.000000 pychopmarg-1.1.1/src/pychopmarg/com.py
+-rw-r--r--   0 dbanas     (501) staff       (20)      695 2024-03-26 09:15:39.000000 pychopmarg-1.1.1/src/pychopmarg/common.py
+-rw-r--r--   0 dbanas     (501) staff       (20)     6874 2024-03-28 22:20:34.000000 pychopmarg-1.1.1/src/pychopmarg/utility.py
+-rw-r--r--   0 dbanas     (501) staff       (20)    19144 2024-04-30 10:42:28.000000 pychopmarg-1.1.1/src/pychopmarg/view.py
```

### Comparing `PyChOpMarg-0.1.1/LICENSE` & `pychopmarg-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyChOpMarg-0.1.1/PKG-INFO` & `pychopmarg-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: PyChOpMarg
-Version: 0.1.1
+Version: 1.1.1
 Summary: Python implementation of COM, as per IEEE 802.3-22 Annex 93A.
 Author-email: David Banas <capn.freako@gmail.com>
 License: BSD3
+Project-URL: documentation, https://pychopmarg.readthedocs.io/en/latest/
 Keywords: com,channel,margin
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Intended Audience :: Science/Research
@@ -24,12 +25,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: System :: Emulators
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Utilities
 Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: chaco>=6.0.0
+Requires-Dist: click
+Requires-Dist: pyside6
 Requires-Dist: scikit-rf>=0.29
 Requires-Dist: traitsui>=8
 
 # PyChOpMarg
 Python implementation of COM, as per IEEE 802.3-22 Annex 93A.
```

### Comparing `PyChOpMarg-0.1.1/pyproject.toml` & `pychopmarg-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 [build-system]
-requires = ["setuptools>=45"]
+requires = [
+    "Cython<3",
+    "setuptools>=45",
+    "swig<4",
+]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyChOpMarg"
 description = "Python implementation of COM, as per IEEE 802.3-22 Annex 93A."
-version = "0.1.1"
+version = "1.1.1"
 authors = [{name = "David Banas", email = "capn.freako@gmail.com"}]
-# urls = { documentation = "https://github.com/capn-freako/PyBERT/wiki"}
+urls = { documentation = "https://pychopmarg.readthedocs.io/en/latest/"}
 readme = "README.md"
 requires-python = ">=3.9,<3.12"
 license = {text = "BSD3"}
 dependencies = [
+    "chaco>=6.0.0",
+    "click",
+    "pyside6",
     "scikit-rf>=0.29",
     "traitsui>=8",
 ]
 keywords=["com", "channel", "margin"]
 classifiers=[
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Console",
@@ -36,15 +43,15 @@
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: System :: Emulators",
     "Topic :: System :: Networking",
     "Topic :: Utilities"
 ]
 
 [project.scripts]
-pychopmarg = "pychopmarg.com:cli"
+pychopmarg = "pychopmarg.cli:cli"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.black]
 line-length = 119
```

### Comparing `PyChOpMarg-0.1.1/src/PyChOpMarg.egg-info/PKG-INFO` & `pychopmarg-1.1.1/src/PyChOpMarg.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: PyChOpMarg
-Version: 0.1.1
+Version: 1.1.1
 Summary: Python implementation of COM, as per IEEE 802.3-22 Annex 93A.
 Author-email: David Banas <capn.freako@gmail.com>
 License: BSD3
+Project-URL: documentation, https://pychopmarg.readthedocs.io/en/latest/
 Keywords: com,channel,margin
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Intended Audience :: Science/Research
@@ -24,12 +25,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: System :: Emulators
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Utilities
 Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: chaco>=6.0.0
+Requires-Dist: click
+Requires-Dist: pyside6
 Requires-Dist: scikit-rf>=0.29
 Requires-Dist: traitsui>=8
 
 # PyChOpMarg
 Python implementation of COM, as per IEEE 802.3-22 Annex 93A.
```

### Comparing `PyChOpMarg-0.1.1/src/pychopmarg/com.py` & `pychopmarg-1.1.1/src/pychopmarg/com.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,57 +13,80 @@
 ToDo:
     1. Provide type hints for imports.
 """
 
 import numpy as np  # type: ignore
 import skrf as rf  # type: ignore
 
+from chaco.api import (
+    ArrayPlotData,
+    GridPlotContainer,
+    Plot,
+)  # type: ignore
+from chaco.tools.api import ZoomTool
 from scipy.interpolate import interp1d
-from traits.api import HasTraits, Property, Array, Float, cached_property  # type: ignore
-from typing import TypeVar, Any, Dict
+from traits.api import (
+    Array,
+    cached_property,
+    Enum,
+    File,
+    Float,
+    HasTraits,
+    Int,
+    List,
+    Property,
+    Str,
+)  # type: ignore
+from typing import Any, Optional, TypeVar
 
 from pychopmarg.common import Rvec, Cvec, COMParams, PI, TWOPI
 from pychopmarg.utility import import_s32p, sdd_21
 
-# Globals used by `calc_Hffe()`, to minimize the size of its cache.
+# Globals
+# These are used by `calc_Hffe()`, to minimize the size of its cache.
 # They are initialized by `COM.__init__()`.
 gFreqs: Rvec = None  # type: ignore
 gFb: float = None  # type: ignore
 gC0min: float = None  # type: ignore
 gNtaps: int = None  # type: ignore
+PLOT_SPACING = 20
 
 T = TypeVar('T', Any, Any)
 
 
+def from_dB(x: float) -> float:
+    """Convert from (dB) to real, assuming square law applies."""
+    return pow(10, x / 20)
+
+
 def all_combs(xss: list[list[T]]) -> list[list[T]]:
     """
     Generate all combinations of input.
 
     Args:
         xss([[T]]): The lists of candidates for each position in the final output.
 
     Returns:
-        [[T]]: All possible combinations of input lists.
+        All possible combinations of input lists.
     """
     if not xss:
         return [[]]
     head, *tail = xss
     yss = all_combs(tail)
     return [[x] + ys for x in head for ys in yss]
 
 
-# @cache
-# def calc_Hffe(tap_weights: Rvec) -> Cvec:
-def calc_Hffe(tap_weights: list[float]) -> Cvec:
+def calc_Hffe(tap_weights: list[float], n_post: int) -> Cvec:
     """
     Calculate the voltage transfer function, H(f), for the Tx FFE,
     according to (93A-21).
 
     Args:
         tap_weights: The vector of filter tap weights, excluding the cursor tap.
+        n_post: The number of post-cursor taps.
 
     Returns:
         The complex voltage transfer function, H(f), for the Tx FFE.
 
     Raises:
         RuntimeError: If the global variables above haven't been initialized.
         ValueError: If the length of the given tap weight vector is incorrect.
@@ -76,292 +99,398 @@
             of `HasTraits` subclasses are not actually memoized, like
             `@cache` decorated ordinary functions are.)
             (It is used in the innermost layer of the nested loop structure
             used to find the optimal EQ solution. And its input argument
             is repeated often.)
             (See the `opt_eq()` method of the `COM` class.)
         2. Currently, a single post-cursor tap is assumed.
-
-    ToDo:
-        1. Remove the single post-cursor tap assumption.
     """
 
     assert len(gFreqs) and gFb and gC0min and gNtaps, RuntimeError(
-        "Called before global variables were initialized!")
+        f"Called before global variables were initialized!\n\tgFreqs: \
+        {gFreqs}, gFb: {gFb}, gC0min: {gC0min}, gNtaps: {gNtaps}")
     assert len(tap_weights) == gNtaps, ValueError(
-        "Length of given tap weight vector is incorrect!")
+        f"Length of given tap weight vector is incorrect!\n\tExpected: {gNtaps}; got: {len(tap_weights)}")
 
     c0 = 1 - sum(list(map(abs, tap_weights)))
     if c0 < gC0min:
         return np.ones(len(gFreqs))
     else:
         cs = tap_weights
-        cs.insert(-1, c0)  # Note the assumption of only one post-cursor tap!
+        cs.insert(-n_post, c0)
         return sum(list(map(lambda n_c: n_c[1] * np.exp(-1j * TWOPI * n_c[0] * gFreqs / gFb),
                             enumerate(cs))))
 
 
+def print_taps(ws: list[float]) -> str:
+    """Return formatted tap weight values."""
+    n_ws = len(ws)
+    if n_ws == 0:
+        return ""
+    res = f"{ws[0]:5.2f}"
+    if n_ws > 1:
+        if n_ws > 8:
+            for w in ws[1:8]:
+                res += f" {w:5.2f}"
+            res += f"\n{ws[8]:5.2f}"
+            for w in ws[9:]:
+                res += f" {w:5.2f}"
+        else:
+            for w in ws[1:]:
+                res += f" {w:5.2f}"
+    return res
+
+
 class COM(HasTraits):
     """
     Encoding of the IEEE 802.3-22 Annex 93A "Channel Operating Margin"
     (COM) specification, as a Python class making use of the Enthought
     Traits/UI machinery, for both calculation efficiency and easy GUI display.
     """
 
-    # Independent variable definitions
-    ui = Float(100e-12)  # Unit interval (s).
-    freqs = Array(value=np.arange(0, 40_010e6, 10e6))  # System frequencies (Hz).
-    gDC = Float(0)  # D.C. gain of Rx CTLE first stage (dB).
-    gDC2 = Float(0)  # D.C. gain of Rx CTLE first stage (dB).
+    status_str = Str("Ready")
+
+    # Independent variable definitions (Defaults from IEEE 802.3by.)
+    # Units are SI, except for: (dB), `zp`, and `eta0`.
+    # - System time/frequency vectors (decoupled!)
+    FB = 25e9 * 66. / 64.
+    fb = Float(0)  # Baud. rate.
+    nspui = Int(32)  # samples per UI.
+    tmax = Float(10e-9)  # system time vector maximum.
+    fstep = Float(10e6)  # system frequency vector step.
+    fmax = Float(40e9)  # system frequency vector maximum.
+    # - Tx Drive Settings
+    Av = Float(0.4)  # victim drive voltage (V).
+    Afe = Float(0.4)  # FEXT drive voltage (V).
+    Ane = Float(0.6)  # NEXT drive voltage (V).
+    L = Int(2)  # number of output levels.
+    RLM = Float(1.0)  # ratio level mismatch.
+    # - Linear EQ
+    nTxTaps = 6
+    tx_n_post = Int(3)
+    tx_taps_pos = Array(shape=(1, (1, nTxTaps)), dtype=int, value=[[-3, -2, -1, 1, 2, 3],])
+    tx_taps_min = Array(shape=(1, (1, nTxTaps)), dtype=float, value=[[0., 0., 0., 0., 0., 0.],])
+    tx_taps_max = Array(shape=(1, (1, nTxTaps)), dtype=float, value=[[0., 0., 0., 0., 0., 0.],])
+    tx_taps_step = Array(shape=(1, (1, nTxTaps)), dtype=float, value=[[0., 0., 0.02, 0.02, 0., 0.],])
+    tx_taps = Array(shape=(1, (1, nTxTaps)), dtype=float, value=[[0.] * nTxTaps,])  # Tx FFE tap weights.
+    c0_min = Float(0)  # minimum allowed Tx FFE main tap value.
+    fr = Float(0.75)  # AFE corner frequency (fb)
+    gDC_vals = List([-x for x in range(13)])  # D.C. gain of Rx CTLE first stage (dB).
+    gDC = Enum(0, values="gDC_vals")
+    gDC2_vals = List([0.,])  # D.C. gain of Rx CTLE second stage (dB).
+    gDC2 = Enum(0, values="gDC2_vals")
+    fz = Float(FB / 4.)  # CTLE zero frequency.
+    fp1 = Float(FB / 4.)  # CTLE first pole frequency.
+    fp2 = Float(FB)  # CTLE second pole frequency.
+    fLF = Float(1e6)  # CTLE low-f corner frequency.
+    # - DFE
+    N_DFE = 14  # number of DFE taps.
+    nDFE = Int(N_DFE)  # number of DFE taps.
+    bmax = List([1.0] * N_DFE)  # DFE maximum tap values.
+    bmin = List([-1.0] * N_DFE)  # DFE minimum tap values.
+    # - Package & Die Modeling
+    R0 = Float(50.0)  # system reference impedance.
+    Rd = Float(55.0)  # on-die termination impedance.
+    Cd = Float(0.25e-12)  # parasitic die capacitance.
+    Cb = Float(0.00e-12)  # parasitic bump capacitance.
+    Cp = Float(0.18e-12)  # parasitic ball capacitance.
+    zp_vals = List([12, 30])  # package transmission line lengths (mm).
+    zp = Enum(12, values="zp_vals")
+    zc = Float(78.2)  # package transmission line characteristic impedance.
+    # - Noise & DER
+    sigma_Rj = Float(0.01)  # random jitter standard deviation (ui).
+    Add = Float(0.05)  # deterministic jitter amplitude (ui).
+    eta0 = Float(5.2e-8)  # spectral noise density (V^2/GHz).
+    TxSNR = Float(27)  # Tx signal-to-noise ratio (dB).
+    DER0 = Float(1e-5)  # detector error rate threshold.
+    # - Channel file(s)
+    chnl_s32p = File("", entries=5, filter=["*.s32p"], exists=False)
+    chnl_s4p_thru = File("", entries=5, filter=["*.s4p"], exists=True)
+    chnl_s4p_fext1 = File("", entries=5, filter=["*.s4p"], exists=True)
+    chnl_s4p_fext2 = File("", entries=5, filter=["*.s4p"], exists=True)
+    chnl_s4p_fext3 = File("", entries=5, filter=["*.s4p"], exists=True)
+    chnl_s4p_next1 = File("", entries=5, filter=["*.s4p"], exists=True)
+    chnl_s4p_next2 = File("", entries=5, filter=["*.s4p"], exists=True)
+    chnl_s4p_next3 = File("", entries=5, filter=["*.s4p"], exists=True)
+    chnl_s4p_next4 = File("", entries=5, filter=["*.s4p"], exists=True)
+    vic_chnl_ix = Int(1)
+    # - Results
+    # -- COM
+    com = Float(0.0)
+    com_As = Float(0.0)
+    com_cursor_ix = Int(0)
+    com_sigma_Tx = Float(0.0)
+    com_sigma_G = Float(0.0)
+    com_sigma_N = Float(0.0)
+    com_dfe_taps = Str(print_taps([0.0] * N_DFE))
+    # -- FOM
+    fom = Float(0.0)
+    fom_As = Float(0.0)
+    Ani = Float(0.0)
+    fom_cursor_ix = Int(0)
+    sigma_ISI = Float(0.0)
+    sigma_J = Float(0.0)
+    sigma_XT = Float(0.0)
+    sigma_Tx = Float(0.0)
+    sigma_N = Float(0.0)
+    fom_tx_taps = Str(print_taps([0.0] * nTxTaps))
+    fom_dfe_taps = Str(print_taps([0.0] * N_DFE))
+
+    # Plots (plot containers, actually).
+    plotdata = ArrayPlotData()
+    plotdata.set_data("t_ns", np.linspace(0., 10., 100))
+    plotdata.set_data("pulse_raw", np.zeros(100))
+    plotdata.set_data("pulse_pkg", np.zeros(100))
+    plotdata.set_data("pulse_eq", np.zeros(100))
+    # - pulse responses.
+    plot1 = Plot(plotdata, padding_left=75)
+    plot1.plot(("t_ns", "pulse_raw"), name="Raw", type="line", color="red")
+    plot1.plot(("t_ns", "pulse_pkg"), name="w/ Pkg", type="line", color="green")
+    plot1.plot(("t_ns", "pulse_eq"), name="w/ EQ", type="line", color="blue")
+    plot1.title = "Pulse Responses"
+    plot1.index_axis.title = "Time (ns)"
+    plot1.value_axis.title = "p(t) (mV)"
+    plot1.legend.visible = True
+    plot1.legend.align = "ur"
+    zoom1 = ZoomTool(plot1, tool_mode="range", axis="index", always_on=False)
+    plot1.overlays.append(zoom1)
+    cont1 = GridPlotContainer(shape=(1, 1), spacing=(PLOT_SPACING, PLOT_SPACING))
+    cont1.add(plot1)
+
+    about_str = """
+      <H2><em>PyChOpMarg</em> - A Python implementation of COM, as per IEEE 802.3-22 Annex 93A.</H2>\n
+      <strong>By:</strong> David Banas <capn.freako@gmail.com><p>\n
+      <strong>On:</strong> April 30, 2024<p>\n
+      <strong>At:</strong> v1.1.0\n
+      <H3>Useful Links</H3>\n
+      (You'll probably need to: right click, select <em>Copy link address</em>, and paste into your browser.)
+        <UL>\n
+          <LI><a href="https://github.com/capn-freako/PyChOpMarg"><em>GitHub</em> Home</a>
+          <LI><a href="https://pypi.org/project/PyChOpMarg/"><em>PyPi</em> Home</a>
+          <LI><a href="https://readthedocs.org/projects/pychopmarg/"><em>Read the Docs</em> Home</a>
+        </UL>
+    """
+
+    def _fb_changed(self):
+        "Keep global version in sync."
+        global gFb
+        gFb = self.fb
+
+    def _c0_min_changed(self):
+        "Keep global version in sync."
+        global gC0min
+        gC0min = self.c0_min
+
+    def _tx_taps_min_changed(self):
+        "Keep global version in sync."
+        global gNtaps
+        gNtaps = len(self.tx_taps_min.flatten())
 
     # Dependent variable definitions
+    # - Unit interval (s).
+    ui = Property(Float, depends_on=["fb"])
+
+    @cached_property
+    def _get_ui(self):
+        """Unit interval (s)."""
+        return 1 / self.fb
+
+    # - system time vector; decoupled from system frequency vector!
+    times = Property(Array, depends_on=["fb", "nspui", "tmax"])
+
+    @cached_property
+    def _get_times(self):
+        """System times (s)."""
+        tstep = self.ui / self.nspui
+        rslt = np.arange(0, self.tmax + tstep, tstep)
+        self.plotdata.set_data("t_ns", rslt * 1e9)
+        return rslt
+
+    # - system frequency vector; decoupled from system time vector!
+    freqs = Property(Array, depends_on=["fstep", "fmax"])
+
+    @cached_property
+    def _get_freqs(self):
+        """System frequencies (Hz)."""
+        global gFreqs
+        freqs = np.arange(0, self.fmax + self.fstep, self.fstep)
+        gFreqs = freqs
+        return freqs
+
+    # - `irfft()` time vector; decoupled from system time vector!
+    t_irfft = Property(Array, depends_on=["freqs"])
+
+    @cached_property
+    def _get_t_irfft(self):
+        """`irfft()` result time index (s)."""
+        Ts = 0.5 / self.fmax  # Sample period satisfying Nyquist criteria.
+        return np.array([n * Ts for n in range(2 * (len(self.freqs) - 1))])
+
+    # - Rect(ui) in the frequency domain.
     Xsinc = Property(Array, depends_on=["ui", "freqs"])
 
     @cached_property
     def _get_Xsinc(self):
         """Frequency domain sinc(f) corresponding to Rect(ui)."""
         ui = self.ui
-        w = int(ui / self.Ts)
+        Ts = self.t_irfft[1]
+        w = int(ui / Ts)
         return w * np.sinc(ui * self.freqs)
 
+    # - Rx AFE voltage transfer function.
     Hr = Property(Array, depends_on=['freqs'])
 
     @cached_property
     def _get_Hr(self):
         """
         Return the voltage transfer function, H(f), of the Rx AFE,
         according to (93A-20).
         """
-        f = self.freqs / (self.params['fr'] * self.fb)
+        f = self.freqs / (self.fr * self.fb)
         return 1 / (1 - 3.414214 * f**2 + f**4 + 2.613126j * (f - f**3))
 
-    Hctf = Property(Array, depends_on=['freqs', 'gDC', 'gDC2'])
+    # - Rx CTLE voltage transfer function.
+    Hctf = Property(Array, depends_on=['freqs', 'gDC', 'gDC2', 'fz', 'fp1', 'fp2', 'fLF'])
 
     @cached_property
     def _get_Hctf(self):
+        return self.calc_Hctf(self.gDC, self.gDC2)
+
+    def calc_Hctf(self, gDC: Optional[float] = None, gDC2: Optional[float] = None) -> Cvec:
         """
         Return the voltage transfer function, H(f), of the Rx CTLE,
         according to (93A-22).
+
+        Keyword Args:
+            gDC: CTLE first stage d.c. gain (dB).
+                Default: None
+            gDC2: CTLE second stage d.c. gain (dB).
+                Default: None
+
+        Notes:
+            1. The instance's current value(s) for `gDC` and `gDC2` are used if not provided.
+                (Necessary, to accommodate sweeping when optimizing EQ.)
         """
+        if gDC is None:
+            gDC = self.gDC
+        if gDC2 is None:
+            gDC2 = self.gDC2
+        g1 = from_dB(gDC)
+        g2 = from_dB(gDC2)
         f = self.freqs
-        g1 = pow(10, self.gDC / 20)
-        g2 = pow(10, self.gDC2 / 20)
-        fz = self.params['fz'] * 1e9
-        fp1 = self.params['fp1'] * 1e9
-        fp2 = self.params['fp2'] * 1e9
-        fLF = self.params['fLF'] * 1e9
+        fz = self.fz
+        fp1 = self.fp1
+        fp2 = self.fp2
+        fLF = self.fLF
         num = (g1 + 1j * f / fz) * (g2 + 1j * f / fLF)
         den = (1 + 1j * f / fp1) * (1 + 1j * f / fp2) * (1 + 1j * f / fLF)
         return num / den
 
-    # Reserved functions
+    # - All possible Tx tap weight combinations.
+    tx_combs = Property(List, depends_on=['tx_taps_min', 'tx_taps_max', 'tx_taps_step'])
 
-    def __call__(self, do_opt_eq=True, tx_taps: Rvec = None):
+    @cached_property
+    def _get_tx_combs(self):
         """
-        Calculate the COM value.
-
-        KeywordArgs:
-            opt_eq: Perform optimization of linear equalization when True.
-                Default: True
-            tx_taps: Used when `do_opt_eq` = False.
-                Default: None
+        All possible Tx tap weight combinations.
         """
+        trips = list(zip(self.tx_taps_min.flatten(), self.tx_taps_max.flatten(), self.tx_taps_step.flatten()))
+        ranges = []
+        for trip in trips:
+            if trip[2]:  # non-zero step?
+                ranges.append(list(np.arange(trip[0], trip[1] + trip[2], trip[2])))
+            else:
+                ranges.append([0.0])
+        return all_combs(ranges)
 
-        assert self.opt_eq(do_opt_eq=do_opt_eq, tx_taps=tx_taps), RuntimeError(
-            "EQ optimization failed!")
-        self.gDC = self.rslts['gDC']
-        self.gDC2 = self.rslts['gDC2']
-        self.tx_taps = self.rslts['tx_taps']
+    # - Reflection coefficients
+    gamma1 = Property(Float, depends_on=['Rd', 'R0'])
+    gamma2 = Property(Float, depends_on=['gamma1'])
 
-        As, Ani, cursor_ix = self.calc_noise()
-        com = 20 * np.log10(As / Ani)
-        self.com = com
-        self.rslts['As'] = As * 1_000  # (mV)
-        self.rslts['Ani'] = Ani * 1_000  # (mV)
-        self.rslts['com'] = com
-        self.cursor_ix = cursor_ix
-        return com
-
-    def __init__(self, params: COMParams, chnl_files: list[str], vic_chnl_ix: int,
-                 zp_sel: int = 1, num_ui: int = 100, gui: bool = True):
+    @cached_property
+    def _get_gamma1(self):
         """
-        COM class initializer.
-
-        Args:
-            params: COM configuration parameters for desired standard.
-                Note: Assumed immutable. ToDo: Can we encode this assumption, using type annotations?
-            chnl_files: Touchstone file(s) representing channel, either:
-                1. 8 s4p files: [victim, ], or
-                2. 1 s32p file, according to VITA 68.2 convention.
-            vic_chnl_ix: Victim channel index (from 1).
-
-        KeywordArgs:
-            zp_sel: User selection of package T-line length option (from 1).
-                Default: 1
-            num_ui: Number of unit intervals to include in system time vector.
-                Default: 100
-            gui: Set to `False` for script/CLI based usage.
-                Default: True
+        Reflection coefficient looking out of the left end of the channel.
         """
+        Rd = self.Rd
+        R0 = self.R0
+        return (Rd - R0) / (Rd + R0)
 
-        # Super-class initialization is ABSOLUTELY NECESSARY, in order
-        # to get all the Traits/UI machinery setup correctly.
-        super().__init__()
-
-        # Set default parameter values, as necessary.
-        if 'zc' not in params:
-            params['zc'] = 78.2
-        if 'fLF' not in params:
-            params['fLF'] = 1
-
-        # Stash function parameters.
-        self.params = params
-        self.chnl_files = chnl_files
-        self.gui = gui
-
-        # Calculate intermediate variable values.
-        self.rslts = {}
-        self.fom_rslts: Dict[str, Any] = {}
-        self.dbg: Dict[str, Any] = {}
-        fb = params['fb'] * 1e9
-        ui = 1 / fb
-        M = self.params['M']
-        sample_per = ui / M
-        fstep = self.params['fstep']
-        trips = list(zip(self.params['tx_min'], self.params['tx_max'], self.params['tx_step']))
-        self.tx_combs = all_combs(list(map(
-            lambda trip: list(np.arange(trip[0], trip[1] + trip[2], trip[2])),
-            trips)))
-        self.gamma1 = (self.params['Rd'] - self.params['R0']) / (self.params['Rd'] + self.params['R0'])
-        self.gamma2 = self.gamma1
-
-        # Import channel Touchstone file(s).
-        if len(chnl_files) == 1:
-            _ntwks = import_s32p(chnl_files[0], vic_chnl_ix)
-            fmax = _ntwks[0][0].f[-1]
-        else:  # ToDo: Do I have the ordering correct here?
-            _ntwks = []
-            fmax = 1000e9
-            n_files = len(chnl_files)
-            for n, chnl_file in enumerate(chnl_files):
-                ntwk = sdd_21(rf.Network(chnl_file))
-                fmax = min(fmax, ntwk.f[-1])
-                if n >= n_files // 2:  # This one is a NEXT aggressor.
-                    _ntwks.append((ntwk, 'NEXT'))
-                elif n > 0:  # This one is a FEXT aggressor.
-                    _ntwks.append((ntwk, 'FEXT'))
-                else:  # This is the victim.
-                    _ntwks.append((ntwk, 'THRU'))
-
-        # Calculate system time/frequency vectors.
-        # - We use "decoupled" time/frequency vectors.
-        freqs = np.arange(0, fmax + fstep, fstep)  # [0,fN], i.e., one extra element
-        times = np.array([n * sample_per for n in range(num_ui * M)])  # independent of `freqs`
-        # - That requires a third vector for correctly timing `irfft()` results.
-        Ts = 0.5 / fmax  # Sample period satisfying Nyquist criteria.
-        t_irfft = np.array([n * Ts for n in range(2 * (len(freqs) - 1))])
-        self.freqs = freqs
-        self.times = times
-        self.Ts = Ts  # Not the same as `sample_per`!
-        self.t_irfft = t_irfft
-
-        # Augment w/ packages.
-        sTx_NEXT = self.sPkg(zp_opt=1, isTx=True)
-        sTx = self.sPkg(zp_opt=zp_sel, isTx=True)
-        sRx = self.sPkg(zp_opt=zp_sel, isTx=False)
-        ntwks = []
-        for ntwk, ntype in _ntwks:
-            if ntype == 'NEXT':
-                ntwks.append((sTx_NEXT ** ntwk ** sRx, ntype))
-            else:
-                ntwks.append((sTx ** ntwk ** sRx, ntype))
-
-        # Generate the pulse responses before/after adding the packages, for reference.
-        self.ntwks = _ntwks
-        self.pulse_resps_nopkg = self.gen_pulse_resps([], apply_eq=False)
-        self.ntwks = ntwks
-        self.pulse_resps_noeq = self.gen_pulse_resps([], apply_eq=False)
-        self.rslts['vic_pulse_pk'] = params['Av'] * max(self.pulse_resps_noeq[0]) * 1_000  # (mV)
-
-        # Store calculated results.
-        self.fb = fb
-        self.ui = ui
-        self.sample_per = sample_per
-        self.fmax = fmax
-        self.nDFE = len(self.params['dfe_max'])
+    @cached_property
+    def _get_gamma2(self):
+        """
+        Reflection coefficient looking out of the right end of the channel.
+        """
+        return self.gamma1
 
-        # Initialize global variables.
-        global gFreqs
-        global gFb
-        global gC0min
-        global gNtaps
-        gFreqs = freqs
-        gFb = fb
-        gC0min = params['c0min']
-        gNtaps = len(params['tx_min'])
+    # - Package response
+    sPkgRx   = Property(depends_on=['zc', 'R0', 'zp', 'freqs', 'Cd', 'Cp'])  # noqa E221
+    sPkgTx   = Property(depends_on=['zc', 'R0', 'zp', 'freqs', 'Cd', 'Cp'])  # noqa E221
+    sPkgNEXT = Property(depends_on=['zc', 'R0', 'zp', 'freqs', 'Cd', 'Cp'])  # noqa E221
+    sZp      = Property(depends_on=['zc', 'R0', 'zp', 'freqs'])  # noqa E221
+    sZpNEXT  = Property(depends_on=['zc', 'R0', 'zp', 'freqs'])  # noqa E221
 
-    # General functions
-    def sC(self, c: float) -> rf.Network:
+    @cached_property
+    def _get_sPkgRx(self) -> rf.Network:
         """
-        Return the 2-port network corresponding to a shunt capacitance,
-        according to (93A-8).
-
-        Args:
-            c: Value of shunt capacitance (F).
+        Rx package response.
+        """
+        return self.sC(self.Cp) ** self.sZp ** self.sC(self.Cd)
 
-        Returns:
-            ntwk: 2-port network equivalent to shunt capacitance, calculated at given frequencies.
+    @cached_property
+    def _get_sPkgTx(self) -> rf.Network:
+        """
+        Tx package response.
+        """
+        return self.sC(self.Cd) ** self.sZp ** self.sC(self.Cp)
 
-        Raises:
-            None
+    @cached_property
+    def _get_sPkgNEXT(self) -> rf.Network:
+        """
+        NEXT package response.
         """
+        return self.sC(self.Cd) ** self.sZpNEXT ** self.sC(self.Cp)
 
-        r0 = self.params['R0']
-        freqs = self.freqs
-        w = TWOPI * freqs
-        s = 1j * w
-        s2p = np.array(
-            [1 / (2 + _s * c * r0) * np.array(
-                [[-_s * c * r0, 2],
-                 [2, -_s * c * r0]])
-             for _s in s])
-        return rf.Network(s=s2p, f=freqs, z0=[2 * r0, 2 * r0])
+    @cached_property
+    def _get_sZp(self) -> rf.Network:
+        return self.calc_sZp()
+
+    @cached_property
+    def _get_sZpNEXT(self) -> rf.Network:
+        return self.calc_sZp(NEXT=True)
 
-    def sZp(self, zp_opt: int = 1) -> rf.Network:
+    def calc_sZp(self, NEXT: bool = False) -> rf.Network:
         """
         Return the 2-port network corresponding to a package transmission line,
         according to (93A-9:14).
 
-        KeywordArgs:
-            zp_opt: Package TL length option (from 1).
-                Default: 1
+        Keyword Args:
+            NEXT: Use first package T-line length option when True.
+                Default: False
 
         Returns:
-            ntwk: 2-port network equivalent to package transmission line.
-
-        Raises:
-            None
+            2-port network equivalent to package transmission line.
         """
 
-        n_zp_opts = len(self.params['zp'])
-        assert zp_opt <= n_zp_opts, ValueError(
-            f"Asked for zp option {zp_opt}, but there are only {n_zp_opts}!")
-        zc = self.params['zc']
-        r0 = self.params['R0']
-        zp = self.params['zp'][zp_opt - 1]
-
-        f_GHz  = self.freqs / 1e9
-        a1     = 1.734e-3  # sqrt(ns)/mm
-        a2     = 1.455e-4  # ns/mm
-        tau    = 6.141e-3  # ns/mm
-        rho    = (zc - 2 * r0) / (zc + 2 * r0)
+        zc = self.zc
+        r0 = self.R0
+        if NEXT:
+            zp = self.zp_vals[0]
+        else:
+            zp = self.zp
+
+        f_GHz  = self.freqs / 1e9               # noqa E221
+        a1     = 1.734e-3  # sqrt(ns)/mm        # noqa E221
+        a2     = 1.455e-4  # ns/mm              # noqa E221
+        tau    = 6.141e-3  # ns/mm              # noqa E221
+        rho    = (zc - 2 * r0) / (zc + 2 * r0)  # noqa E221
         gamma0 = 0         # 1/mm
         gamma1 = a1 * (1 + 1j)
 
-        def gamma2(f):
+        def gamma2(f: float) -> complex:
             "f in GHz!"
             return a2 * (1 - 1j * (2 / PI) * np.log(f)) + 1j * TWOPI * tau
 
         def gamma(f: float) -> complex:
             "Return complex propagation coefficient at frequency f (GHz)."
             if f == 0:
                 return gamma0
@@ -373,39 +502,252 @@
         s21 = s12 = (1 - rho**2) * np.exp(-g * zp) / (1 - rho**2 * np.exp(-g * 2 * zp))
         s2p = np.array(
             [[[_s11, _s12],
               [_s21, _s22]]
              for _s11, _s12, _s21, _s22 in zip(s11, s12, s21, s22)])
         return rf.Network(s=s2p, f=self.freqs, z0=[2 * r0, 2 * r0])
 
-    def sPkg(self, zp_opt: int = 1, isTx: bool = True) -> rf.Network:
+    # - Channels
+    def get_chnls(self) -> list[tuple[rf.Network, str]]:
+        """Import all channels from Touchstone file(s)."""
+        if self.chnl_s32p:
+            return self.get_chnls_s32p_wPkg()
+        else:
+            return self.get_chnls_s4p_wPkg()
+
+    def get_chnls_s32p_wPkg(self) -> list[tuple[rf.Network, str]]:
+        """Augment imported s32p channels, w/ package response."""
+        return self.add_pkgs(self.get_chnls_s32p_noPkg())
+
+    def get_chnls_s4p_wPkg(self) -> list[tuple[rf.Network, str]]:
+        """Augment imported s4p channels, w/ package response."""
+        return self.add_pkgs(self.get_chnls_s4p_noPkg())
+
+    def get_chnls_s32p_noPkg(self) -> list[tuple[rf.Network, str]]:
+        """Import s32p file, w/o package."""
+        if not self.chnl_s32p:
+            return []
+        ntwks = import_s32p(self.chnl_s32p, self.vic_chnl_ix)
+        self.fmax = ntwks[0][0].f[-1]
+
+        # Generate the pulse responses before adding the packages, for reference.
+        pulse_resps_nopkg = self.gen_pulse_resps(ntwks, [], apply_eq=False)
+        self.plotdata.set_data("pulse_raw", pulse_resps_nopkg[0])
+        self.pulse_resps_nopkg = pulse_resps_nopkg
+
+        return ntwks
+
+    # @cached_property
+    def get_chnls_s4p_noPkg(self) -> list[tuple[rf.Network, str]]:
+        """Import s4p files, w/o package."""
+        if not self.chnl_s4p_thru:
+            return []
+        ntwks = [(sdd_21(rf.Network(self.chnl_s4p_thru)), 'THRU')]
+        fmax = ntwks[0][0].f[-1]
+        for fname in [self.chnl_s4p_fext1, self.chnl_s4p_fext2, self.chnl_s4p_fext3]:
+            if fname:
+                ntwk = sdd_21(rf.Network(fname))
+                ntwks.append((ntwk, 'FEXT'))
+                if ntwk.f[-1] < fmax:
+                    fmax = ntwk.f[-1]
+        for fname in [self.chnl_s4p_next1, self.chnl_s4p_next2, self.chnl_s4p_next3, self.chnl_s4p_next4]:
+            if fname:
+                ntwk = sdd_21(rf.Network(fname))
+                ntwks.append((sdd_21(rf.Network(fname)), 'NEXT'))
+                if ntwk.f[-1] < fmax:
+                    fmax = ntwk.f[-1]
+        self.fmax = fmax
+
+        # Generate the pulse responses before adding the packages, for reference.
+        pulse_resps_nopkg = self.gen_pulse_resps(ntwks, [], apply_eq=False)
+        self.plotdata.set_data("pulse_raw", pulse_resps_nopkg[0])
+        self.pulse_resps_nopkg = pulse_resps_nopkg
+
+        return ntwks
+
+    def add_pkgs(self, ntwks: list[tuple[rf.Network, str]]) -> list[tuple[rf.Network, str]]:
+        """Add package response to raw channels and generate pulse responses."""
+        if not ntwks:
+            return []
+        _ntwks = list(map(self.add_pkg, ntwks))
+        pulse_resps_noeq = self.gen_pulse_resps(_ntwks, [], apply_eq=False)
+        self.rslts['vic_pulse_pk'] = max(pulse_resps_noeq[0]) * 1_000  # (mV)
+        self.pulse_resps_noeq = pulse_resps_noeq
+        self.plotdata.set_data("pulse_pkg", pulse_resps_noeq[0])
+        return _ntwks
+
+    def add_pkg(self, ntwk: tuple[rf.Network, str]) -> tuple[rf.Network, str]:
+        """Add package response to raw channel."""
+        ntype = ntwk[1]
+        if ntype == 'NEXT':
+            return (self.sPkgNEXT ** ntwk[0] ** self.sPkgRx, ntype)
+        else:
+            return (self.sPkgTx ** ntwk[0] ** self.sPkgRx, ntype)
+
+    # Reserved functions
+    def __init__(self):
+        """
+        Instance creation only! Must still initialize.
         """
-        Return the 2-port network corresponding to a complete package model,
-        according to (93A-15:16).
 
-        KeywordArgs:
-            zp_opt: Package TL length option (from 1).
-                Default: 1
-            isTx: Requesting Tx package when True.
+        # Super-class initialization is ABSOLUTELY NECESSARY, in order
+        # to get all the Traits/UI machinery setup correctly.
+        super().__init__()
+
+        self.rslts = {}
+        self.fom_rslts = {}
+        self.dbg = {}
+
+        self.fb = self.FB
+        self.c0_min = 0.62
+        self.tx_taps_min = [[0., 0., -0.18, -0.38, 0., 0.],]
+
+    @classmethod
+    def init(cls, params: dict, chnl_fnames: list[str], vic_id: int,
+             zp_sel: int = 1, num_ui: int = 500, gui: bool = False):
+        """
+        Legacy initializer supports my VITA notebook, which was created before
+        PyChOpMarg was altered to support a GUI.
+        """
+        obj = cls()
+        obj.set_params(params)
+        assert zp_sel > 0 and zp_sel <= len(obj.zp_vals), RuntimeError(
+            "`zp_sel` out of range!")
+        if len(chnl_fnames) == 1:
+            obj.chnl_s32p = chnl_fnames[0]
+        else:
+            obj.chnl_s4p_thru = chnl_fnames[0]
+            if len(chnl_fnames) > 1:
+                obj.chnl_s4p_fext1 = chnl_fnames[1]
+            if len(chnl_fnames) > 2:
+                obj.chnl_s4p_fext2 = chnl_fnames[2]
+            if len(chnl_fnames) > 3:
+                obj.chnl_s4p_next1 = chnl_fnames[3]
+            if len(chnl_fnames) > 4:
+                obj.chnl_s4p_next2 = chnl_fnames[4]
+            if len(chnl_fnames) > 5:
+                obj.chnl_s4p_next3 = chnl_fnames[5]
+        obj.vic_chnl_ix = vic_id
+        obj.zp = obj.zp_vals[zp_sel - 1]
+        obj.num_ui = num_ui
+        obj.gui = gui
+        return obj
+
+    def __call__(self, do_opt_eq=True, tx_taps: Rvec = None):
+        """
+        Calculate the COM value.
+
+        Keyword Args:
+            opt_eq: Perform optimization of linear equalization when True.
                 Default: True
+            tx_taps: Used when `do_opt_eq` = False.
+                Default: None
+        """
+
+        assert self.chnl_s32p or self.chnl_s4p_thru, RuntimeError(
+            "You must, at least, select a thru path channel file, either 32 or 4 port.")
+        self.chnls = self.get_chnls()
+        self.status_str = "Optimizing EQ..."
+        assert self.opt_eq(do_opt_eq=do_opt_eq, tx_taps=tx_taps), RuntimeError(
+            "EQ optimization failed!")
+
+        self.status_str = "Calculating noise..."
+        As, Ani, self.cursor_ix = self.calc_noise()
+        com = 20 * np.log10(As / Ani)
+        self.As = As
+        self.Ani = Ani
+        self.com = com
+        self.rslts['com'] = com
+        self.rslts['As'] = As * 1e3
+        self.rslts['Ani'] = Ani * 1e3
+        self.status_str = f"Ready; COM = {com: 5.1f} dB"
+        return com
+
+    # Initializers
+    def set_params(self, params: COMParams) -> None:
+        """
+        Set the COM instance parameters, according the the given dictionary.
+
+        Args:
+            params: Dictionary of COM parameter values.
+
+        Raises:
+            KeyError: If an expected key is not found in the provided dictionary.
+        """
+
+        # Set default parameter values, as necessary.
+        if 'z_c' not in params:
+            params['zc'] = 78.2
+        if 'C_b' not in params:
+            params['C_b'] = 0.0
+        if 'f_LF' not in params:
+            params['f_LF'] = 0.001
+        if 'g_DC2' not in params:
+            params['g_DC2'] = 0.0
+
+        # Capture parameters, adjusting units as necessary to keep all but (dB) and `eta0` SI.
+        self.fb = params['fb'] * 1e9
+        self.nspui = params['M']
+        self.L = params['L']
+        self.fstep = params['fstep']
+        self.tx_taps_min = params['tx_taps_min']
+        self.tx_taps_max = params['tx_taps_max']
+        self.tx_taps_step = params['tx_taps_step']
+        self.fr = params['f_r']
+        self.fz = params['f_z'] * 1e9
+        self.fp1 = params['f_p1'] * 1e9
+        self.fp2 = params['f_p2'] * 1e9
+        self.fLF = params['f_LF'] * 1e9
+        self.gDC_vals = params['g_DC']
+        self.gDC2_vals = params['g_DC2']
+        self.Rd = params['R_d']
+        self.R0 = params['R_0']
+        self.Cd = params['C_d'] / 1e12
+        self.Cb = params['C_b'] / 1e12
+        self.Cp = params['C_p'] / 1e12
+        self.Av = params['A_v']
+        self.Afe = params['A_fe']
+        self.Ane = params['A_ne']
+        self.DER0 = params['DER_0']
+        self.sigma_Rj = params['sigma_Rj']
+        self.Add = params['A_DD']
+        self.eta0 = params['eta_0']
+        self.TxSNR = params['SNR_TX']
+        self.zc = params['z_c']
+        self.zp_vals = params['z_p']
+
+        # Stash input parameters, for future reference.
+        self.params = params
+
+    # General functions
+    def sC(self, c: float) -> rf.Network:
+        """
+        Return the 2-port network corresponding to a shunt capacitance,
+        according to (93A-8).
+
+        Args:
+            c: Value of shunt capacitance (F).
 
         Returns:
-            ntwk: 2-port network equivalent to complete package model.
+            2-port network equivalent to shunt capacitance, calculated at given frequencies.
 
         Raises:
             None
         """
 
-        sd = self.sC(self.params['Cd'] / 1e12)
-        sp = self.sC(self.params['Cp'] / 1e12)
-        sl = self.sZp(zp_opt)
-        if isTx:
-            return sd ** sl ** sp
-        else:
-            return sp ** sl ** sd
+        r0 = self.R0
+        freqs = self.freqs
+        w = TWOPI * freqs
+        s = 1j * w
+        s2p = np.array(
+            [1 / (2 + _s * c * r0) * np.array(
+                [[-_s * c * r0, 2],
+                 [2, -_s * c * r0]])
+             for _s in s])
+        return rf.Network(s=s2p, f=freqs, z0=[2 * r0, 2 * r0])
 
     def H21(self, s2p: rf.Network) -> Cvec:
         """
         Return the voltage transfer function, H21(f), of a terminated two
         port network, according to (93A-18).
 
         Args:
@@ -414,164 +756,177 @@
         Returns:
             Complex voltage transfer function at given frequencies.
 
         Raises:
             ValueError: If given network is not two port.
 
         Notes:
-            1. It is at this point in the analysis that the "raw" Touchstone
-                data gets interpolated to our system frequency vector.
-            2. After this step, the package and R0/Rd mismatch have been
-                accounted for, but not the EQ.
+            1. It is at this point in the analysis that the "raw" Touchstone data
+                gets interpolated to our system frequency vector.
+            2. After this step, the package and R0/Rd mismatch have been accounted for,
+                but not the EQ.
         """
 
         assert s2p.s[0].shape == (2, 2), ValueError("I can only convert 2-port networks.")
         s2p.interpolate_self(self.freqs)
         g1 = self.gamma1
         g2 = self.gamma2
         s11 = s2p.s11.s.flatten()
         s12 = s2p.s12.s.flatten()
         s21 = s2p.s21.s.flatten()
         s22 = s2p.s22.s.flatten()
         dS = s11 * s22 - s12 * s21
         return (s21 * (1 - g1) * (1 + g2)) / (1 - s11 * g1 - s22 * g2 + g1 * g2 * dS)
 
-    def H(self, s2p: rf.Network, tap_weights: Rvec) -> Cvec:
+    def H(self, s2p: rf.Network, tap_weights: Rvec,
+          gDC: Optional[float] = None, gDC2: Optional[float] = None) -> Cvec:
         """
         Return the voltage transfer function, H(f), of a complete COM signal path,
         according to (93A-19).
 
         Args:
             s2p: Two port network of interest.
             tap_weights: Tx FFE tap weights.
 
+        Keyword Args:
+            gDC: CTLE first stage d.c. gain.
+            gDC2: CTLE second stage d.c. gain.
+
         Returns:
             Complex voltage transfer function of complete path.
 
         Raises:
             ValueError: If given network is not two port,
                 or length of `tap_weights` is incorrect.
 
         Notes:
             1. Assumes `self.gDC` and `self.gDC2` have been set correctly.
             2. It is in this processing step that linear EQ is first applied.
         """
 
         assert s2p.s[0, :, :].shape == (2, 2), ValueError(
             f"I can only convert 2-port networks. {s2p}")
-        self.H21_temp = self.H21(s2p)
-        return calc_Hffe(list(tap_weights)) * self.H21_temp * self.Hr * self.Hctf
+        H_tx = calc_Hffe(list(tap_weights.flatten()), self.tx_n_post)
+        H_rx = self.H21(s2p) * self.Hr * self.calc_Hctf(gDC, gDC2)
+        return (H_tx * H_rx)
 
     def pulse_resp(self, H: Cvec) -> Rvec:
         """
         Return the unit pulse response, p(t), corresponding to the given
         voltage transfer function, H(f), according to (93A-24).
 
         Args:
             H: The voltage transfer function, H(f).
                 Note: Possitive frequency components only, including fN.
 
         Returns:
-            p: The pulse response corresponding to the given voltage transfer function.
+            The pulse response corresponding to the given voltage transfer function.
 
         Raises:
             ValueError: If the length of the given voltage transfer
                 function differs from that of the system frequency vector.
 
         Notes:
             1. It is at this point in the signal processing chain that we change
                 time domains.
         """
 
         assert len(H) == len(self.freqs), ValueError(
             "Length of given H(f) does not match length of f!")
 
         Xsinc = self.Xsinc
+        Ts = self.t_irfft[1]
         p = np.fft.irfft(Xsinc * H)
         p_mag = np.abs(p)
-        p_beg = np.where(p_mag > 0.01 * max(p_mag))[0][0] - int(5 * self.ui / self.Ts)  # Give it some "front porch".
+        p_beg = np.where(p_mag > 0.01 * max(p_mag))[0][0] - int(5 * self.ui / Ts)  # Give it some "front porch".
         spln = interp1d(self.t_irfft, np.roll(p, -p_beg))  # `p` is not yet in our system time domain!
         return spln(self.times)                            # Now, it is.
 
-    def gen_pulse_resps(self, tx_taps: Rvec, apply_eq=True) -> list[Rvec]:
+    def gen_pulse_resps(self, ntwks: list[tuple[rf.Network, str]], tx_taps: Rvec,
+                        gDC: Optional[float] = None, gDC2: Optional[float] = None,
+                        apply_eq: bool = True) -> list[Rvec]:
         """
         Generate pulse responses for all networks.
 
         Args:
+            ntwks: The list of networks to generate pulse responses for.
             tx_taps: Desired Tx tap weights.
 
-        KeywordArgs:
+        Keyword Args:
             apply_eq: Include linear EQ when True; otherwise, exclude it.
                 Default: True
 
         Returns:
             List of pulse responses.
 
         Raises:
             None
 
         Notes:
-            1. Assumes `self.gDC` and `self.gDC2` have been set correctly.
+            1. Assumes `self.gDC` and `self.gDC2` have been set correctly, if not provided.
         """
 
         pulse_resps = []
-        for ntwk, ntype in self.ntwks:
+        for ntwk, ntype in ntwks:
             if apply_eq:
-                pr = self.pulse_resp(self.H(ntwk, tx_taps))
+                if ntype == 'NEXT':
+                    pr = self.pulse_resp(self.H(ntwk, np.zeros(tx_taps.shape), gDC, gDC2))
+                else:
+                    pr = self.pulse_resp(self.H(ntwk, tx_taps, gDC, gDC2))
             else:
                 pr = self.pulse_resp(self.H21(ntwk))
 
             if ntype == 'THRU':
-                pr *= self.params['Av']
+                pr *= self.Av
             elif ntype == 'NEXT':
-                pr *= self.params['Ane']
+                pr *= self.Ane
             else:
-                pr *= self.params['Afe']
+                pr *= self.Afe
 
             pulse_resps.append(pr)
 
         return pulse_resps
 
     def filt_pr_samps(self, pr_samps: Rvec, As: float, rel_thresh: float = 0.001) -> Rvec:
         """
         Filter a list of pulse response samples for minimum magnitude.
 
         Args:
             pr_samps: The pulse response samples to filter.
             As: Signal amplitude, as per 93A.1.6.c.
 
-        KeywordArgs:
+        Keyword Args:
             rel_thresh: Filtration threshold (As).
                 Default: 0.001 (i.e. - 0.1%, as per Note 2 of 93A.1.7.1)
 
         Returns:
-            filtered_samps: The subset of `pr_samps` passing filtration.
+            The subset of `pr_samps` passing filtration.
         """
 
         thresh = As * rel_thresh
         return np.array(list(filter(lambda x: abs(x) >= thresh, pr_samps)))
 
     def calc_hJ(self, pulse_resp: Rvec, As: float, cursor_ix: int, rel_thresh: float = 0.001) -> Rvec:
         """
         Calculate the set of slopes for valid pulse response samples.
 
         Args:
             pulse_resp: The pulse response of interest.
             As: Signal amplitude, as per 93A.1.6.c.
             cursor_ix: Cursor index.
 
-        KeywordArgs:
+        Keyword Args:
             rel_thresh: Filtration threshold (As).
                 Default: 0.001 (i.e. - 0.1%, as per Note 2 of 93A.1.7.1)
 
         Returns:
-            slopes: The calculated slopes around the valid samples.
+            The calculated slopes around the valid samples.
         """
 
-        M = self.params['M']
+        M = self.nspui
         thresh = As * rel_thresh
         valid_pr_samp_ixs = np.array(list(filter(lambda ix: abs(pulse_resp[ix]) >= thresh,
                                                  range(cursor_ix, len(pulse_resp) - 1, M))))
         m1s = pulse_resp[valid_pr_samp_ixs - 1]
         p1s = pulse_resp[valid_pr_samp_ixs + 1]
         return (p1s - m1s) / (2 / M)  # (93A-28)
 
@@ -579,28 +934,28 @@
         """
         Locate the cursor position for the given pulse response,
         according to (93A-25) and (93A-26).
 
         Args:
             pulse_resp: The pulse response of interest.
 
-        KeywordArgs:
+        Keyword Args:
             max_range: The search radius, from the peak.
 
         Returns:
             The index in the given pulse response vector of the cursor.
 
         Notes:
             1. As per v3.70 of the COM MATLAB code, we only minimize the
                 residual of (93A-25); we don't try to solve it exactly.
         """
 
-        M = self.params['M']
-        dfe_max = self.params['dfe_max']
-        dfe_min = self.params['dfe_min']
+        M = self.nspui
+        dfe_max = self.bmax
+        dfe_min = self.bmin
 
         # Find zero crossings.
         peak_loc = np.argmax(pulse_resp)
         peak_val = pulse_resp[peak_loc]
         search_start = max(0, peak_loc - 4 * M)
         zxi = np.where(np.diff(np.sign(pulse_resp[search_start:peak_loc] - .01 * peak_val)) >= 1)[0] + search_start
         assert zxi, RuntimeError("No zero crossings found!")
@@ -615,89 +970,98 @@
                           pulse_resp[ix + M] / pulse_resp[ix]))                          # (93A-26)
             res = abs(pulse_resp[ix - M] - (pulse_resp[ix + M] - b_1 * pulse_resp[ix]))  # (93A-25)
             if res < res_min:
                 ix_best = ix
                 res_min = res
         return ix_best
 
-    def calc_fom(self, tx_taps: Rvec) -> float:
+    def calc_fom(self, tx_taps: Rvec,
+                 gDC: Optional[float] = None, gDC2: Optional[float] = None) -> float:
         """
-        Calculate the _figure of merit_ (FOM), given the existing linear EQ settings.
+        Calculate the *figure of merit* (FOM), given the existing linear EQ settings.
 
         Args:
             tx_taps: The Tx FFE tap weights, excepting the cursor.
                 (The cursor takes whatever is left.)
 
+        Keyword Args:
+            gDC: CTLE first stage d.c. gain.
+            gDC2: CTLE second stage d.c. gain.
+
         Returns:
-            FOM: The resultant figure of merit.
+            The resultant figure of merit.
 
         Raises:
-            None.
+            None
 
         Notes:
-            1. Assumes that `self.gDC` and `self.gDC2` have been set correctly.
-            2. See: IEEE 802.3-2022 93A.1.6.
+            1. See: IEEE 802.3-2022 93A.1.6.
         """
 
-        L = self.params['L']
-        M = self.params['M']
+        L = self.L
+        M = self.nspui
         freqs = self.freqs
+        chnls = self.chnls
 
         # Step a - Pulse response construction.
-        pulse_resps = self.gen_pulse_resps(np.array(tx_taps))
+        pulse_resps = self.gen_pulse_resps(chnls, np.array(tx_taps), gDC=gDC, gDC2=gDC2)
 
         # Step b - Cursor identification.
-        vic_pulse_resp = np.array(pulse_resps[0])
+        try:
+            vic_pulse_resp = np.array(pulse_resps[0])
+        except Exception:
+            print(len(pulse_resps), len(chnls))
+            raise
         vic_peak_loc = np.argmax(vic_pulse_resp)
         cursor_ix = self.loc_curs(vic_pulse_resp)
 
         # Step c - As.
         vic_curs_val = vic_pulse_resp[cursor_ix]
-        As = self.params['RLM'] * vic_curs_val / (L - 1)
+        As = self.RLM * vic_curs_val / (L - 1)
 
         # Step d - Tx noise.
         varX = (L**2 - 1) / (3 * (L - 1)**2)  # (93A-29)
-        varTx = vic_curs_val**2 * pow(10, -self.params['TxSNR'] / 10)  # (93A-30)
+        varTx = vic_curs_val**2 * pow(10, -self.TxSNR / 10)  # (93A-30)
 
         # Step e - ISI.
-        nDFE = self.nDFE
+        nDFE = len(self.bmin)
         # This is not compliant to the standaard, but is consistent w/ v2.60 of MATLAB code.
         n_pre = cursor_ix // M
         first_pre_ix = cursor_ix - n_pre * M
         vic_pulse_resp_isi_samps = np.concatenate((vic_pulse_resp[first_pre_ix:cursor_ix:M],
                                                    vic_pulse_resp[cursor_ix + M::M]))
         vic_pulse_resp_post_samps = vic_pulse_resp_isi_samps[n_pre:]
         dfe_tap_weights = np.maximum(  # (93A-26)
-            self.params['dfe_min'],
+            self.bmin,
             np.minimum(
-                self.params['dfe_max'],
+                self.bmax,
                 (vic_pulse_resp_post_samps[:nDFE] / vic_curs_val)))
         hISI = vic_pulse_resp_isi_samps \
-             - vic_curs_val * np.pad(dfe_tap_weights,
+             - vic_curs_val * np.pad(dfe_tap_weights,  # noqa E127
                                      (n_pre, len(vic_pulse_resp_post_samps) - nDFE),
                                      mode='constant',
                                      constant_values=0)  # (93A-27)
         varISI = varX * sum(hISI**2)  # (93A-31)
         self.dbg['vic_pulse_resp_isi_samps'] = vic_pulse_resp_isi_samps
         self.dbg['vic_pulse_resp_post_samps'] = vic_pulse_resp_post_samps
         self.dbg['hISI'] = hISI
 
         # Step f - Jitter noise.
         hJ = self.calc_hJ(vic_pulse_resp, As, cursor_ix)
-        varJ = (self.params['Add']**2 + self.params['sigma_Rj']**2) * varX * sum(hJ**2)  # (93A-32)
+        varJ = (self.Add**2 + self.sigma_Rj**2) * varX * sum(hJ**2)  # (93A-32)
 
         # Step g - Crosstalk.
         varXT = 0
         for pulse_resp in pulse_resps[1:]:  # (93A-34)
             varXT += max([sum(np.array(self.filt_pr_samps(pulse_resp[m::M], As))**2) for m in range(M)])  # (93A-33)
         varXT *= varX
 
         # Step h - Spectral noise.
         df = freqs[1]
-        varN = self.params['eta0'] * sum(abs(self.Hr * self.Hctf)**2) * (df / 1e9)  # (93A-35)
+        varN = self.eta0 * sum(abs(self.Hr * self.calc_Hctf(gDC=gDC, gDC2=gDC2))**2) * (df / 1e9)  # (93A-35)
 
         # Step i - FOM calculation.
         fom = 10 * np.log10(As**2 / (varTx + varISI + varJ + varXT + varN))  # (93A-36)
 
         # Stash our calculation results.
         self.fom_rslts['pulse_resps'] = pulse_resps
         self.fom_rslts['vic_pulse_resp'] = vic_pulse_resp
@@ -714,43 +1078,41 @@
         return fom
 
     def opt_eq(self, do_opt_eq: bool = True, tx_taps: Rvec = None) -> bool:
         """
         Find the optimum values for the linear equalization parameters:
         c(-2), c(-1), c(1), gDC, and gDC2, as per IEEE 802.3-22 93A.1.6.
 
-        KeywordArgs:
+        Keyword Args:
             do_opt_eq: Perform optimization of linear EQ when True.
                 Default: True
             tx_taps: Used when `do_opt_eq` = False.
                 Default: None
 
         Returns:
-            success: True if no errors encountered; False otherwise.
+            True if no errors encountered; False otherwise.
         """
 
         if do_opt_eq:
             # Run the nested optimization loops.
             def check_taps(tx_taps: Rvec) -> bool:
-                if (1 - sum(abs(np.array(tx_taps)))) < self.params['c0min']:
+                if (1 - sum(abs(np.array(tx_taps)))) < self.c0_min:
                     return False
                 else:
                     return True
 
             fom_max = -100.0
             fom_max_changed = False
             foms = []
-            for gDC2 in self.params['gDC2']:
-                self.gDC2 = gDC2
-                for gDC in self.params['gDC']:
-                    self.gDC = gDC
+            for gDC2 in self.gDC2_vals:
+                for gDC in self.gDC_vals:
                     for n, tx_taps in enumerate(self.tx_combs):
                         if not check_taps(np.array(tx_taps)):
                             continue
-                        fom = self.calc_fom(tx_taps)
+                        fom = self.calc_fom(tx_taps, gDC=gDC, gDC2=gDC2)
                         foms.append(fom)
                         if fom > fom_max:
                             fom_max_changed = True
                             fom_max = fom
                             gDC2_best = gDC2
                             gDC_best = gDC
                             tx_taps_best = tx_taps
@@ -758,14 +1120,15 @@
                             cursor_ix_best = self.fom_rslts['cursor_ix']
                             As_best = self.fom_rslts['As']
                             varTx_best = self.fom_rslts['varTx']
                             varISI_best = self.fom_rslts['varISI']
                             varJ_best = self.fom_rslts['varJ']
                             varXT_best = self.fom_rslts['varXT']
                             varN_best = self.fom_rslts['varN']
+                            vic_pulse_resp = self.fom_rslts['vic_pulse_resp']
         else:
             assert tx_taps, RuntimeError("You must define `tx_taps` when setting `do_opt_eq` False!")
             fom = self.calc_fom(tx_taps)
             foms = [fom]
             fom_max = fom
             fom_max_changed = True
             gDC2_best = self.gDC2
@@ -775,86 +1138,87 @@
             cursor_ix_best = self.fom_rslts['cursor_ix']
             As_best = self.fom_rslts['As']
             varTx_best = self.fom_rslts['varTx']
             varISI_best = self.fom_rslts['varISI']
             varJ_best = self.fom_rslts['varJ']
             varXT_best = self.fom_rslts['varXT']
             varN_best = self.fom_rslts['varN']
+            vic_pulse_resp = self.fom_rslts['vic_pulse_resp']
 
         # Check for error and save the best results.
         if not fom_max_changed:
             return False
+        self.fom = fom_max
+        self.gDC2 = gDC2_best
+        self.gDC = gDC_best
+        self.tx_taps = [tx_taps_best,]
+        self.fom_tx_taps = print_taps(tx_taps_best)
+        self.fom_dfe_taps = print_taps(dfe_tap_weights_best)
+        self.fom_cursor_ix = cursor_ix_best
+        self.fom_As = As_best
+        self.sigma_ISI = np.sqrt(varISI_best)
+        self.sigma_J = np.sqrt(varJ_best)
+        self.sigma_XT = np.sqrt(varXT_best)
+        # These two are also calculated by `calc_noise()`.
+        self.sigma_Tx = np.sqrt(varTx_best)
+        self.sigma_N = np.sqrt(varN_best)
+        self.foms = foms
+        self.plotdata.set_data("pulse_eq", vic_pulse_resp)
         self.rslts['fom'] = fom_max
-        self.rslts['gDC2'] = gDC2_best
         self.rslts['gDC'] = gDC_best
-        self.rslts['tx_taps'] = tx_taps_best
-        self.rslts['dfe_tap_weights'] = dfe_tap_weights_best
-        self.rslts['cursor_ix'] = cursor_ix_best
-        self.rslts['As'] = As_best * 1_000  # (mV)
-        self.rslts['sigma_ISI'] = np.sqrt(varISI_best) * 1_000  # (mV)
-        self.rslts['sigma_J'] = np.sqrt(varJ_best) * 1_000  # (mV)
-        self.rslts['sigma_XT'] = np.sqrt(varXT_best) * 1_000  # (mV)
-        # These two are also calculated by `calc_noise()`; so, add "_best".
-        self.rslts['sigma_Tx_best'] = np.sqrt(varTx_best) * 1_000  # (mV)
-        self.rslts['sigma_N_best'] = np.sqrt(varN_best) * 1_000  # (mV)
-        self.rslts['foms'] = foms
+        self.rslts['gDC2'] = gDC2_best
+        self.rslts['tx_taps'] = tx_taps_best[2:4]
+        self.rslts['dfe_taps'] = dfe_tap_weights_best
+        self.rslts['sigma_ISI'] = self.sigma_ISI * 1e3
+        self.rslts['sigma_XT'] = self.sigma_XT * 1e3
+        self.rslts['sigma_J'] = self.sigma_J * 1e3
         return True
 
     def calc_noise(self) -> tuple[float, float, int]:
         """
         Calculate the interference and noise for COM.
 
-        KeywordArgs:
-            npts: Number of vector points.
-                Default: 2001
-
         Returns:
-            (As, Ani, cursor_ix): Triple containing:
-                - signal amplitude,
-                - noise + interference amplitude (V), and
-                - cursor location within victim pulse response vector.
-
-        Raises:
-            None
-
-        Warns:
-            1. If `2*As/npts` rises above 10 uV, against standard's recommendation.
+            - signal amplitude
+            - noise + interference amplitude (V)
+            - cursor location within victim pulse response vector
 
         Notes:
             1. Assumes the following instance variables have been set:
                 - gDC
                 - gDC2
                 - tx_taps
+            2. Warns if `2*As/npts` rises above 10 uV, against standard's recommendation.
         """
 
-        L = self.params['L']
-        M = self.params['M']
+        L = self.L
+        M = self.nspui
         freqs = self.freqs
-        nDFE = self.nDFE
+        nDFE = len(self.bmin)
 
-        pulse_resps = self.gen_pulse_resps(np.array(self.tx_taps))
+        pulse_resps = self.gen_pulse_resps(self.chnls, np.array(self.tx_taps))
         vic_pulse_resp = pulse_resps[0]
         cursor_ix = self.loc_curs(vic_pulse_resp)
         vic_curs_val = vic_pulse_resp[cursor_ix]
-        As = self.params['RLM'] * vic_curs_val / (L - 1)
+        As = self.RLM * vic_curs_val / (L - 1)
         npts = 2 * max(int(As / 0.001), 1_000) + 1  # Note 1 of 93A.1.7.1; MUST BE ODD!
         y = np.linspace(-As, As, npts)
         ystep = 2 * As / (npts - 1)
 
         delta = np.zeros(npts)
         delta[npts // 2] = 1
         varX = (L**2 - 1) / (3 * (L - 1)**2)  # (93A-29)
         df = freqs[1]
 
         def pn(hn: float) -> Rvec:
             """
             (93A-39)
             """
-            return 1 / L * sum([np.roll(delta, int((2 * l / (L - 1) - 1) * hn / ystep))
-                                for l in range(L)])
+            return 1 / L * sum([np.roll(delta, int((2 * el / (L - 1) - 1) * hn / ystep))
+                                for el in range(L)])
 
         def p(h_samps: Rvec) -> Rvec:
             """
             Calculate the "delta-pmf" for a set of pulse response samples,
             as per (93A-40).
 
             Args:
@@ -883,38 +1247,38 @@
                 rslts.append(rslt)
             rslt /= sum(rslt)  # Enforce a PMF. Commenting out didn't make a difference.
             self.dbg['pns'] = pns
             self.dbg['rslts'] = rslts
             return rslt
 
         # Sec. 93A.1.7.2
-        varN = self.params['eta0'] * sum(abs(self.Hr * self.Hctf)**2) * (df / 1e9)  # (93A-35)
-        varTx = vic_curs_val**2 * pow(10, -self.params['TxSNR'] / 10)               # (93A-30)
+        varN = self.eta0 * sum(abs(self.Hr * self.Hctf)**2) * (df / 1e9)  # (93A-35)
+        varTx = vic_curs_val**2 * pow(10, -self.TxSNR / 10)               # (93A-30)
         hJ = self.calc_hJ(vic_pulse_resp, As, cursor_ix)
-        pJ = p(self.params['Add'] * hJ)
+        pJ = p(self.Add * hJ)
         self.dbg['pJ'] = pJ
         self.dbg['hJ'] = hJ
-        varG = varTx + self.params['sigma_Rj']**2 * varX * sum(hJ**2) + varN  # (93A-41)
+        varG = varTx + self.sigma_Rj**2 * varX * sum(hJ**2) + varN  # (93A-41)
         pG = np.exp(-y**2 / (2 * varG)) / np.sqrt(TWOPI * varG)               # (93A-42)
         pN = np.convolve(pG, pJ, mode='same')                                 # (93A-43)
 
         # Sec. 93A.1.7.3
         # - ISI (Inconsistent w/ IEEE 802.3-22, but consistent w/ v2.60 of MATLAB code.)
         n_pre = cursor_ix // M
         first_pre_ix = cursor_ix - n_pre * M
         vic_pulse_resp_isi_samps = np.concatenate((vic_pulse_resp[first_pre_ix:cursor_ix:M],
                                                    vic_pulse_resp[cursor_ix + M::M]))
         vic_pulse_resp_post_samps = vic_pulse_resp_isi_samps[n_pre:]
         dfe_tap_weights = np.maximum(  # (93A-26)
-            self.params['dfe_min'],
+            self.bmin,
             np.minimum(
-                self.params['dfe_max'],
+                self.bmax,
                 (vic_pulse_resp_post_samps[:nDFE] / vic_curs_val)))
         hISI = vic_pulse_resp_isi_samps \
-             - vic_curs_val * np.pad(dfe_tap_weights,
+             - vic_curs_val * np.pad(dfe_tap_weights,  # noqa E127
                                      (n_pre, len(vic_pulse_resp_post_samps) - nDFE),
                                      mode='constant',
                                      constant_values=0)  # (93A-27)
         hISI = self.filt_pr_samps(hISI, As)
         py = p(hISI)  # `hISI` from (93A-27); `p(y)` as per (93A-40)
 
         # - Crosstalk
@@ -935,21 +1299,25 @@
 
         # Final calculation
         Py = np.cumsum(py)
         Py /= Py[-1]  # Enforce cumulative probability distribution.
 
         # Store some results.
         self.pulse_resps = pulse_resps
-        self.cursor_ix = cursor_ix
-        self.rslts['sigma_Tx'] = np.sqrt(varTx) * 1_000  # (mV)
-        self.rslts['sigma_G'] = np.sqrt(varG) * 1_000  # (mV)
-        self.rslts['sigma_N'] = np.sqrt(varN) * 1_000  # (mV)
+        self.com_cursor_ix = cursor_ix
+        self.com_sigma_Tx = np.sqrt(varTx)
+        self.com_sigma_G = np.sqrt(varG)
+        self.com_sigma_N = np.sqrt(varN)
         self.rslts['pG'] = pG
         self.rslts['pN'] = pN
         self.rslts['py'] = py
         self.rslts['Py'] = Py
         self.rslts['y'] = y
-        self.rslts['dfe_taps'] = dfe_tap_weights
+        self.com_dfe_taps = print_taps(dfe_tap_weights)
+        self.com_As = As
+        self.rslts['sigma_G'] = self.com_sigma_G * 1e3
+        self.rslts['sigma_Tx'] = self.com_sigma_Tx * 1e3
+        self.rslts['sigma_N'] = self.com_sigma_N * 1e3
 
         return (As,
-                abs(np.where(Py >= self.params['DER'])[0][0] - npts // 2) * ystep,
+                abs(np.where(Py >= self.DER0)[0][0] - npts // 2) * ystep,
                 cursor_ix)
```

### Comparing `PyChOpMarg-0.1.1/src/pychopmarg/common.py` & `pychopmarg-1.1.1/src/pychopmarg/common.py`

 * *Files identical despite different names*

### Comparing `PyChOpMarg-0.1.1/src/pychopmarg/utility.py` & `pychopmarg-1.1.1/src/pychopmarg/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
     """
     Given a 4-port single-ended network, return its differential throughput
     as a 2-port network.
 
     Args:
         ntwk: 4-port single ended network.
 
-    KeywordArgs:
+    Keyword Args:
         norm: Normalization factor. (Default = 0.5)
         renumber: Automatically detect correct through path when True.
-            Default: False
+                  Default: False
 
     Returns:
         Sdd (2-port).
 
     Notes:
         1. A "1->2/3->4" port ordering convention is assumed when `renumber` is False.
         2. Automatic renumbering should not be used unless a solid d.c. thru path exists.
@@ -39,21 +39,21 @@
 def se2mm(ntwk: rf.Network, norm: float = 0.5, renumber: bool = False) -> rf.Network:
     """
     Given a 4-port single-ended network, return its mixed mode equivalent.
 
     Args:
         ntwk: 4-port single ended network.
 
-    KeywordArgs:
+    Keyword Args:
         norm: Normalization factor. (Default = 0.5)
         renumber: Automatically detect correct through path when True.
-            Default: False
+                  Default: False
 
     Returns:
-        skrf.Network: Mixed mode equivalent network, in the following format:
+        Mixed mode equivalent network, in the following format:
             Sdd11  Sdd12  Sdc11  Sdc12
             Sdd21  Sdd22  Sdc21  Sdc22
             Scd11  Scd12  Scc11  Scc12
             Scd21  Scd22  Scc21  Scc22
 
     Notes:
         1. A "1->2/3->4" port ordering convention is assumed when `renumber` is False.
@@ -104,32 +104,32 @@
     """Read in a 32-port Touchstone file, and return an equivalent list
     of 8 2-port differential networks: a single victim through channel and
     7 crosstalk aggressors, according to the VITA 68.2 convention.
 
     Args:
         filename: Name of Touchstone file to read in.
 
-    KeywordArgs:
+    Keyword Args:
         vic_chnl: Victim channel number (from 1).
             Default = 1
 
     Returns:
-        [(skrf.Network, str)]: List of 8 pairs, each consisting of:
+        List of 8 pairs, each consisting of:
             - a 2-port network representing a *differential* channel, and
             - the type of that channel, one of: 'THRU', 'NEXT', or 'FEXT.
-            (First element is the victim and the only one of type 'THRU'.)
+                (First element is the victim and the only one of type 'THRU'.)
 
     Raises:
         ValueError: If Touchstone file is not 32-port.
 
     Notes:
         1. Input Touchstone file is assumed single-ended.
         2. The differential through and xtalk channels are returned.
-        3. Port 2 of all returned channels correspond to the same
-        physical circuit node, typically, the Rx input node.
+        3. Port 2 of all returned channels correspond to the same physical circuit node,
+            typically, the Rx input node.
     """
 
     # Import and sanity check the Touchstone file.
     ntwk = rf.Network(filename)
     (fs, rs, cs) = ntwk.s.shape
     assert rs == cs, "Non-square Touchstone file S-matrix!"
     assert rs == 32, f"Touchstone file must have 32 ports!\n\t{ntwk}"
@@ -141,15 +141,15 @@
         left and right channel ID (from 1), assuming "1=>2/3=>4" convention.
 
         Args:
             left(int): Left side channel number (from 1).
             right(int): Right side channel number (from 1).
 
         Returns:
-            [int]: List of ports (from 0) for desired channel.
+            List of ports (from 0) for desired channel.
         """
         left0 = left - 1     # 0-based
         right0 = right - 1
         return [left0 * 4, right0 * 4 + 1, left0 * 4 + 2, right0 * 4 + 3]
 
     vic_ports = ports_from_chnls(vic_chnl, vic_chnl)
     vic = sdd_21(rf.subnetwork(ntwk, vic_ports))
```

