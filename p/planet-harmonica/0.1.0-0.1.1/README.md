# Comparing `tmp/planet-harmonica-0.1.0.tar.gz` & `tmp/planet_harmonica-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planet-harmonica-0.1.0.tar", last modified: Wed Dec 14 12:52:16 2022, max compression
+gzip compressed data, was "planet_harmonica-0.1.1.tar", last modified: Tue Apr 30 10:45:41 2024, max compression
```

## Comparing `planet-harmonica-0.1.0.tar` & `planet_harmonica-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 12:52:16.457332 planet-harmonica-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-14 12:51:55.000000 planet-harmonica-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2022-12-14 12:52:16.457332 planet-harmonica-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      973 2022-12-14 12:51:55.000000 planet-harmonica-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 12:52:16.457332 planet-harmonica-0.1.0/harmonica/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-14 12:51:55.000000 planet-harmonica-0.1.0/harmonica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2022-12-14 12:51:55.000000 planet-harmonica-0.1.0/harmonica/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2022-12-14 12:51:55.000000 planet-harmonica-0.1.0/harmonica/bindings.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 12:52:16.457332 planet-harmonica-0.1.0/harmonica/jax/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2022-12-14 12:51:55.000000 planet-harmonica-0.1.0/harmonica/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2022-12-14 12:51:55.000000 planet-harmonica-0.1.0/harmonica/jax/custom_primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 12:52:16.457332 planet-harmonica-0.1.0/harmonica/light_curve/
--rw-r--r--   0 runner    (1001) docker     (123)    31812 2022-12-14 12:51:55.000000 planet-harmonica-0.1.0/harmonica/light_curve/fluxes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    58266 2022-12-14 12:51:55.000000 planet-harmonica-0.1.0/harmonica/light_curve/gradients.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 12:52:16.457332 planet-harmonica-0.1.0/harmonica/orbit/
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2022-12-14 12:51:55.000000 planet-harmonica-0.1.0/harmonica/orbit/gradients.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2022-12-14 12:51:55.000000 planet-harmonica-0.1.0/harmonica/orbit/kepler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2022-12-14 12:51:55.000000 planet-harmonica-0.1.0/harmonica/orbit/trajectories.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 12:52:16.457332 planet-harmonica-0.1.0/planet_harmonica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2022-12-14 12:52:16.000000 planet-harmonica-0.1.0/planet_harmonica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-14 12:52:16.000000 planet-harmonica-0.1.0/planet_harmonica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 12:52:16.000000 planet-harmonica-0.1.0/planet_harmonica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-14 12:52:16.000000 planet-harmonica-0.1.0/planet_harmonica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-14 12:52:16.000000 planet-harmonica-0.1.0/planet_harmonica.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-14 12:51:55.000000 planet-harmonica-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-14 12:52:16.457332 planet-harmonica-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2022-12-14 12:51:55.000000 planet-harmonica-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:45:41.089426 planet_harmonica-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-30 10:45:41.089426 planet_harmonica-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:45:41.085425 planet_harmonica-0.1.1/harmonica/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/harmonica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/harmonica/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/harmonica/bindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:45:41.085425 planet_harmonica-0.1.1/harmonica/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/harmonica/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/harmonica/jax/custom_primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:45:41.089426 planet_harmonica-0.1.1/harmonica/light_curve/
+-rw-r--r--   0 runner    (1001) docker     (127)    31812 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/harmonica/light_curve/fluxes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    58266 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/harmonica/light_curve/gradients.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:45:41.089426 planet_harmonica-0.1.1/harmonica/orbit/
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/harmonica/orbit/gradients.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/harmonica/orbit/kepler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/harmonica/orbit/trajectories.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:45:41.089426 planet_harmonica-0.1.1/planet_harmonica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-30 10:45:41.000000 planet_harmonica-0.1.1/planet_harmonica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-30 10:45:41.000000 planet_harmonica-0.1.1/planet_harmonica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:45:41.000000 planet_harmonica-0.1.1/planet_harmonica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 10:45:41.000000 planet_harmonica-0.1.1/planet_harmonica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 10:45:41.000000 planet_harmonica-0.1.1/planet_harmonica.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 10:45:41.089426 planet_harmonica-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:45:41.089426 planet_harmonica-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/tests/test_flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15702 2024-04-30 10:45:30.000000 planet_harmonica-0.1.1/tests/test_flux_derivatives.py
```

### Comparing `planet-harmonica-0.1.0/LICENSE` & `planet_harmonica-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `planet-harmonica-0.1.0/PKG-INFO` & `planet_harmonica-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: planet-harmonica
-Version: 0.1.0
+Version: 0.1.1
 Summary: Light curves for exoplanet transmission mapping.
 Home-page: https://github.com/DavoGrant/harmonica
 Author: David Grant
 Author-email: david.grant@bristol.ac.uk
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: jax
+Requires-Dist: jaxlib
 
 Light curves for exoplanet transmission mapping.
```

### Comparing `planet-harmonica-0.1.0/README.md` & `planet_harmonica-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 <h1 align="center">Harmonica</h1>
 <p align="center">
   Light curves for exoplanet transmission mapping in python.
 </p>
 
 <p align="center">
-  <a href="https://github.com/DavoGrant/ExoTiC-MIRI/actions/workflows/python-app.yml">
-    <img alt="GitHub Workflow Status" src="https://github.com/DavoGrant/ExoTiC-MIRI/workflows/unittests/badge.svg">
+  <a href="https://github.com/DavoGrant/harmonica/actions/workflows/unittests.yml">
+    <img alt="GitHub Workflow Status" src="https://github.com/DavoGrant/harmonica/actions/workflows/unittests.yml/badge.svg">
   </a>
-  <a href="https://exotic-miri.readthedocs.io/en/latest/?badge=latest">
-    <img alt="Read the Docs" src="https://readthedocs.org/projects/exotic-miri/badge/?version=latest">
+  <a href="https://harmonica.readthedocs.io/en/latest/?badge=latest">
+    <img alt="Read the Docs" src="https://readthedocs.org/projects/harmonica/badge/?version=latest">
   </a>
 </p>
 
 ```
 pip install planet-harmonica
 ```
 
 Read the full documentation at: [harmonica.readthedocs.io](https://harmonica.readthedocs.io).<br>
-Read the full methods paper at: [mnras](https://doi.org/10.1093/mnras/stac3632) or on the [arxiv](https://link/to/arxiv/paper).<br>
+Read the full methods paper at: [mnras](https://doi.org/10.1093/mnras/stac3632) or on the [arxiv](http://arxiv.org/abs/2212.07294).<br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
                                   [Harmonica]
                             ************ HHaarrmmoonniiccaa ************
           Light curves for exoplanet transmission mapping in python.
                     _[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_]_[_R_e_a_d_ _t_h_e_ _D_o_c_s_]
 ``` pip install planet-harmonica ``` Read the full documentation at:
 [harmonica.readthedocs.io](https://harmonica.readthedocs.io).
 Read the full methods paper at: [mnras](https://doi.org/10.1093/mnras/stac3632)
-or on the [arxiv](https://link/to/arxiv/paper).
+or on the [arxiv](http://arxiv.org/abs/2212.07294).
```

### Comparing `planet-harmonica-0.1.0/harmonica/api.py` & `planet_harmonica-0.1.1/harmonica/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         planet lies entirely inside the stellar disc, and pnl_e
         corresponds to when the planet intersects the stellar limb.
         Allowed values = {10, 20, 100, 200, 500}. Use
         get_precision_estimate() to check model precision.
 
     Notes
     -----
-    The algorithm is detailed in Grant and Wakeford 2022.
+    The algorithm is detailed in Grant and Wakeford 2023.
 
     """
 
     def __init__(self, times=None, pnl_c=20, pnl_e=50):
         # Orbital parameters.
         self._t0 = None
         self._period = None
```

### Comparing `planet-harmonica-0.1.0/harmonica/bindings.cpp` & `planet_harmonica-0.1.1/harmonica/bindings.cpp`

 * *Files identical despite different names*

### Comparing `planet-harmonica-0.1.0/harmonica/jax/custom_primitives.py` & `planet_harmonica-0.1.1/harmonica/jax/custom_primitives.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
+import jax
 import numpy as np
 import jax.numpy as jnp
-from jax.config import config
 from jaxlib import xla_client
 from functools import partial
-from jax.interpreters import ad
-from jax import abstract_arrays, core, xla
+from jax.interpreters import ad, xla
 
 from harmonica import bindings
 
 # Enable double floating precision.
-config.update("jax_enable_x64", True)
+jax.config.update("jax_enable_x64", True)
 
 
 def harmonica_transit_quad_ld(times, t0, period, a, inc, ecc=0., omega=0.,
                               u1=0., u2=0., r=jnp.array([0.1])):
     """ Harmonica transits with jax -- quadratic limb darkening.
 
     Parameters
@@ -68,20 +67,20 @@
     """ Define new JAX primitive. """
     return jax_light_curve_quad_ld_p.bind(times, *params)
 
 
 def jax_light_curve_quad_ld_abstract_eval(abstract_times, *abstract_params):
     """ Define the abstract evaluation. """
     # Define first model output.
-    abstract_model_eval = abstract_arrays.ShapedArray(
+    abstract_model_eval = jax.core.ShapedArray(
         abstract_times.shape, abstract_times.dtype)
 
     # Define second model output.
     n_params = len(abstract_params)
-    abstract_model_derivatives = abstract_arrays.ShapedArray(
+    abstract_model_derivatives = jax.core.ShapedArray(
         tuple(abstract_times.shape) + (n_params,), abstract_times.dtype)
 
     return abstract_model_eval, abstract_model_derivatives
 
 
 def jax_light_curve_quad_ld_xla_translation(c, timesc, *paramssc):
     """ XLA compilation rules. """
@@ -204,20 +203,20 @@
     """ Define new JAX primitive. """
     return jax_light_curve_nonlinear_ld_p.bind(times, *params)
 
 
 def jax_light_curve_nonlinear_ld_abstract_eval(abstract_times, *abstract_params):
     """ Define the abstract evaluation. """
     # Define first model output.
-    abstract_model_eval = abstract_arrays.ShapedArray(
+    abstract_model_eval = jax.core.ShapedArray(
         abstract_times.shape, abstract_times.dtype)
 
     # Define second model output.
     n_params = len(abstract_params)
-    abstract_model_derivatives = abstract_arrays.ShapedArray(
+    abstract_model_derivatives = jax.core.ShapedArray(
         tuple(abstract_times.shape) + (n_params,), abstract_times.dtype)
 
     return abstract_model_eval, abstract_model_derivatives
 
 
 def jax_light_curve_nonlinear_xla_translation(c, timesc, *paramssc):
     """ XLA compilation rules. """
@@ -286,23 +285,23 @@
 # Register the C++ models, bytes string required.
 xla_client.register_custom_call_target(
     b'jax_light_curve_quad_ld', bindings.jax_registrations()['jax_light_curve_quad_ld'])
 xla_client.register_custom_call_target(
     b'jax_light_curve_nonlinear_ld', bindings.jax_registrations()['jax_light_curve_nonlinear_ld'])
 
 # Create a primitive for quad ld.
-jax_light_curve_quad_ld_p = core.Primitive('jax_light_curve_quad_ld')
+jax_light_curve_quad_ld_p = jax.core.Primitive('jax_light_curve_quad_ld')
 jax_light_curve_quad_ld_p.multiple_results = True
 jax_light_curve_quad_ld_p.def_impl(partial(xla.apply_primitive, jax_light_curve_quad_ld_p))
 jax_light_curve_quad_ld_p.def_abstract_eval(jax_light_curve_quad_ld_abstract_eval)
 xla.backend_specific_translations['cpu'][jax_light_curve_quad_ld_p] = \
     jax_light_curve_quad_ld_xla_translation
 ad.primitive_jvps[jax_light_curve_quad_ld_p] = jax_light_curve_quad_ld_value_and_jvp
 
 # Create a primitive for non-linear ld.
-jax_light_curve_nonlinear_ld_p = core.Primitive('jax_light_curve_nonlinear_ld')
+jax_light_curve_nonlinear_ld_p = jax.core.Primitive('jax_light_curve_nonlinear_ld')
 jax_light_curve_nonlinear_ld_p.multiple_results = True
 jax_light_curve_nonlinear_ld_p.def_impl(partial(xla.apply_primitive, jax_light_curve_nonlinear_ld_p))
 jax_light_curve_nonlinear_ld_p.def_abstract_eval(jax_light_curve_nonlinear_ld_abstract_eval)
 xla.backend_specific_translations['cpu'][jax_light_curve_nonlinear_ld_p] = \
     jax_light_curve_nonlinear_xla_translation
 ad.primitive_jvps[jax_light_curve_nonlinear_ld_p] = jax_light_curve_nonlinear_ld_value_and_jvp
```

### Comparing `planet-harmonica-0.1.0/harmonica/light_curve/fluxes.cpp` & `planet_harmonica-0.1.1/harmonica/light_curve/fluxes.cpp`

 * *Files identical despite different names*

### Comparing `planet-harmonica-0.1.0/harmonica/light_curve/gradients.cpp` & `planet_harmonica-0.1.1/harmonica/light_curve/gradients.cpp`

 * *Files identical despite different names*

### Comparing `planet-harmonica-0.1.0/harmonica/orbit/gradients.cpp` & `planet_harmonica-0.1.1/harmonica/orbit/gradients.cpp`

 * *Files identical despite different names*

### Comparing `planet-harmonica-0.1.0/harmonica/orbit/kepler.cpp` & `planet_harmonica-0.1.1/harmonica/orbit/kepler.cpp`

 * *Files identical despite different names*

### Comparing `planet-harmonica-0.1.0/harmonica/orbit/trajectories.cpp` & `planet_harmonica-0.1.1/harmonica/orbit/trajectories.cpp`

 * *Files identical despite different names*

### Comparing `planet-harmonica-0.1.0/planet_harmonica.egg-info/PKG-INFO` & `planet_harmonica-0.1.1/planet_harmonica.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: planet-harmonica
-Version: 0.1.0
+Version: 0.1.1
 Summary: Light curves for exoplanet transmission mapping.
 Home-page: https://github.com/DavoGrant/harmonica
 Author: David Grant
 Author-email: david.grant@bristol.ac.uk
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: jax
+Requires-Dist: jaxlib
 
 Light curves for exoplanet transmission mapping.
```

### Comparing `planet-harmonica-0.1.0/planet_harmonica.egg-info/SOURCES.txt` & `planet_harmonica-0.1.1/planet_harmonica.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,8 +12,10 @@
 harmonica/orbit/gradients.cpp
 harmonica/orbit/kepler.cpp
 harmonica/orbit/trajectories.cpp
 planet_harmonica.egg-info/PKG-INFO
 planet_harmonica.egg-info/SOURCES.txt
 planet_harmonica.egg-info/dependency_links.txt
 planet_harmonica.egg-info/requires.txt
-planet_harmonica.egg-info/top_level.txt
+planet_harmonica.egg-info/top_level.txt
+tests/test_flux.py
+tests/test_flux_derivatives.py
```

### Comparing `planet-harmonica-0.1.0/setup.py` & `planet_harmonica-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         language="c++",
         extra_compile_args=["-O2", "-ffast-math"]
     ),
 ]
 
 setup(
     name="planet-harmonica",
-    version="0.1.0",
+    version="0.1.1",
     author="David Grant",
     author_email="david.grant@bristol.ac.uk",
     url="https://github.com/DavoGrant/harmonica",
     license="MIT",
     packages=["harmonica", "harmonica.jax"],
     description="Light curves for exoplanet transmission mapping.",
     long_description="Light curves for exoplanet transmission mapping.",
```

