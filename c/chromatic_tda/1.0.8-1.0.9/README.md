# Comparing `tmp/chromatic_tda-1.0.8.tar.gz` & `tmp/chromatic_tda-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromatic_tda-1.0.8.tar", max compression
+gzip compressed data, was "chromatic_tda-1.0.9.tar", max compression
```

## Comparing `chromatic_tda-1.0.8.tar` & `chromatic_tda-1.0.9.tar`

### file list

```diff
@@ -1,40 +1,58 @@
--rw-r--r--   0        0        0    31702 2023-08-11 17:00:30.665859 chromatic_tda-1.0.8/LICENSE.txt
--rw-r--r--   0        0        0     3608 2024-02-08 14:33:39.527104 chromatic_tda-1.0.8/README.md
--rw-r--r--   0        0        0      290 2023-08-19 16:35:10.327478 chromatic_tda-1.0.8/chromatic_tda/__init__.py
--rw-r--r--   0        0        0        0 2023-08-11 15:07:25.970000 chromatic_tda-1.0.8/chromatic_tda/algorithms/__init__.py
--rw-r--r--   0        0        0     5566 2024-02-15 20:40:06.342536 chromatic_tda-1.0.8/chromatic_tda/algorithms/chromatic_subcomplex_utils.py
--rw-r--r--   0        0        0     9579 2024-02-14 18:51:10.858186 chromatic_tda-1.0.8/chromatic_tda/algorithms/persistence_algorithm.py
--rw-r--r--   0        0        0    11481 2024-02-14 19:14:31.632775 chromatic_tda-1.0.8/chromatic_tda/algorithms/radius_function_utils.py
--rw-r--r--   0        0        0     1258 2024-02-14 18:51:10.843251 chromatic_tda-1.0.8/chromatic_tda/algorithms/reduce_matrix.py
--rw-r--r--   0        0        0        0 2023-08-11 15:07:25.999000 chromatic_tda-1.0.8/chromatic_tda/algorithms/test/__init__.py
--rw-r--r--   0        0        0     5560 2024-02-15 20:14:50.105812 chromatic_tda-1.0.8/chromatic_tda/algorithms/test/test_chromatic_subcomplex.py
--rw-r--r--   0        0        0        0 2023-08-11 15:07:25.954000 chromatic_tda-1.0.8/chromatic_tda/core/__init__.py
--rw-r--r--   0        0        0     5850 2024-02-20 17:36:52.150534 chromatic_tda-1.0.8/chromatic_tda/core/chromatic_alpha_complex_factory.py
--rw-r--r--   0        0        0     3701 2024-02-20 17:21:09.036460 chromatic_tda-1.0.8/chromatic_tda/core/core_chromatic_alpha_complex.py
--rw-r--r--   0        0        0     6559 2024-02-14 19:14:31.637038 chromatic_tda-1.0.8/chromatic_tda/core/core_simplicial_complex.py
--rw-r--r--   0        0        0     4062 2024-02-15 17:05:29.989362 chromatic_tda-1.0.8/chromatic_tda/core/simplicial_complex_factory.py
--rw-r--r--   0        0        0        0 2024-02-20 15:34:57.785386 chromatic_tda-1.0.8/chromatic_tda/core/test/__init__.py
--rw-r--r--   0        0        0     2504 2024-02-20 16:52:32.468084 chromatic_tda-1.0.8/chromatic_tda/core/test/chromatic_alpha_complex_construction_test.py
--rw-r--r--   0        0        0    14035 2024-02-20 16:13:32.555508 chromatic_tda-1.0.8/chromatic_tda/core/test/test_data/chralph_random_10_10.json
--rw-r--r--   0        0        0    41541 2024-02-20 16:46:03.165063 chromatic_tda-1.0.8/chromatic_tda/core/test/test_data/chralph_random_10_10_5.json
--rw-r--r--   0        0        0    23366 2024-02-20 16:51:32.589112 chromatic_tda-1.0.8/chromatic_tda/core/test/test_data/chralph_random_15_15.json
--rw-r--r--   0        0        0    54399 2024-02-20 16:51:50.980261 chromatic_tda-1.0.8/chromatic_tda/core/test/test_data/chralph_random_15_8_7.json
--rw-r--r--   0        0        0     5470 2024-02-20 16:48:27.796544 chromatic_tda-1.0.8/chromatic_tda/core/test/test_data/chralph_random_5_2_1.json
--rw-r--r--   0        0        0        0 2023-08-11 15:07:26.002000 chromatic_tda-1.0.8/chromatic_tda/entities/__init__.py
--rw-r--r--   0        0        0     5830 2024-02-20 15:36:46.366866 chromatic_tda-1.0.8/chromatic_tda/entities/chromatic_alpha_complex.py
--rw-r--r--   0        0        0      493 2023-08-11 15:45:50.792041 chromatic_tda-1.0.8/chromatic_tda/entities/external_delaunay.py
--rw-r--r--   0        0        0     7697 2024-02-15 20:34:55.400587 chromatic_tda-1.0.8/chromatic_tda/entities/simplicial_complex.py
--rw-r--r--   0        0        0        0 2023-08-11 15:07:25.999000 chromatic_tda-1.0.8/chromatic_tda/entities/test/__init__.py
--rw-r--r--   0        0        0     2437 2024-02-20 15:36:46.390476 chromatic_tda-1.0.8/chromatic_tda/entities/test/simplicial_complex_construction_test.py
--rw-r--r--   0        0        0        0 2023-08-11 15:07:26.011000 chromatic_tda-1.0.8/chromatic_tda/plots/__init__.py
--rw-r--r--   0        0        0    11124 2024-02-08 20:17:37.993929 chromatic_tda-1.0.8/chromatic_tda/plots/plotting_functions.py
--rw-r--r--   0        0        0        0 2023-08-11 15:07:25.980000 chromatic_tda-1.0.8/chromatic_tda/utils/__init__.py
--rw-r--r--   0        0        0      613 2024-02-14 19:07:07.273887 chromatic_tda-1.0.8/chromatic_tda/utils/boundary_matrix_utils.py
--rw-r--r--   0        0        0      832 2024-02-14 19:16:39.052368 chromatic_tda-1.0.8/chromatic_tda/utils/filter_functions.py
--rw-r--r--   0        0        0     1003 2024-02-14 19:14:31.627399 chromatic_tda-1.0.8/chromatic_tda/utils/floating_point_utils.py
--rw-r--r--   0        0        0     2060 2024-02-14 19:14:31.642601 chromatic_tda-1.0.8/chromatic_tda/utils/geometrical_utils.py
--rw-r--r--   0        0        0       64 2024-02-14 19:07:07.287441 chromatic_tda-1.0.8/chromatic_tda/utils/simplex_utils.py
--rw-r--r--   0        0        0      225 2023-08-11 15:07:25.995220 chromatic_tda-1.0.8/chromatic_tda/utils/singleton.py
--rw-r--r--   0        0        0     1184 2023-08-11 15:45:50.759825 chromatic_tda-1.0.8/chromatic_tda/utils/timing.py
--rw-r--r--   0        0        0      901 2024-02-20 17:39:33.097941 chromatic_tda-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     4708 1970-01-01 00:00:00.000000 chromatic_tda-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    31702 2023-08-11 17:00:30.665859 chromatic_tda-1.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     3777 2024-04-30 04:40:18.848738 chromatic_tda-1.0.9/README.md
+-rw-r--r--   0        0        0      290 2024-02-28 11:19:34.002767 chromatic_tda-1.0.9/chromatic_tda/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-11 15:07:25.970000 chromatic_tda-1.0.9/chromatic_tda/algorithms/__init__.py
+-rw-r--r--   0        0        0     7393 2024-04-29 15:03:28.218890 chromatic_tda-1.0.9/chromatic_tda/algorithms/chromatic_subcomplex_utils.py
+-rw-r--r--   0        0        0       64 2024-03-01 20:05:56.726799 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/.git
+-rw-r--r--   0        0        0     1319 2024-03-01 20:05:56.744420 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       82 2024-03-01 20:05:56.744586 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/.gitignore
+-rw-r--r--   0        0        0     1078 2024-03-01 20:05:56.744761 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/LICENSE
+-rw-r--r--   0        0        0       41 2024-03-01 20:05:56.744904 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/MANIFEST.in
+-rw-r--r--   0        0        0     3969 2024-03-01 20:05:56.745084 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/README.rst
+-rw-r--r--   0        0        0        0 2024-03-01 20:05:56.745000 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/__init__.py
+-rw-r--r--   0        0        0      236 2024-03-01 20:08:31.359436 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      252 2024-04-09 06:09:45.245297 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3612 2024-03-01 20:11:10.924544 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/__pycache__/miniball.cpython-310.pyc
+-rw-r--r--   0        0        0     6354 2024-04-09 06:09:45.247106 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/__pycache__/miniball.cpython-311.pyc
+-rw-r--r--   0        0        0    12639 2024-04-09 06:10:51.761866 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/__pycache__/test_miniball.cpython-311-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0    12639 2024-04-30 04:36:28.384375 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/__pycache__/test_miniball.cpython-311-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     4498 2024-03-01 20:10:06.995661 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/miniball.py
+-rw-r--r--   0        0        0        6 2024-03-01 20:05:56.747830 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/requirements.txt
+-rw-r--r--   0        0        0       34 2024-03-01 20:05:56.747966 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/setup.cfg
+-rw-r--r--   0        0        0     2528 2024-03-01 20:05:56.748134 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/setup.py
+-rw-r--r--   0        0        0     3625 2024-04-09 06:10:48.947495 chromatic_tda-1.0.9/chromatic_tda/algorithms/miniball/test_miniball.py
+-rw-r--r--   0        0        0     9579 2024-04-29 14:42:32.075664 chromatic_tda-1.0.9/chromatic_tda/algorithms/persistence_algorithm.py
+-rw-r--r--   0        0        0    11481 2024-04-29 14:42:32.076505 chromatic_tda-1.0.9/chromatic_tda/algorithms/radius_function_utils.py
+-rw-r--r--   0        0        0     1258 2024-04-29 14:42:32.078078 chromatic_tda-1.0.9/chromatic_tda/algorithms/reduce_matrix.py
+-rw-r--r--   0        0        0        0 2023-08-11 15:07:25.999000 chromatic_tda-1.0.9/chromatic_tda/algorithms/test/__init__.py
+-rw-r--r--   0        0        0     9956 2024-04-29 15:03:28.219865 chromatic_tda-1.0.9/chromatic_tda/algorithms/test/test_chromatic_subcomplex.py
+-rw-r--r--   0        0        0        0 2023-08-11 15:07:25.954000 chromatic_tda-1.0.9/chromatic_tda/core/__init__.py
+-rw-r--r--   0        0        0     5840 2024-04-29 15:34:15.186734 chromatic_tda-1.0.9/chromatic_tda/core/chromatic_alpha_complex_factory.py
+-rw-r--r--   0        0        0     3796 2024-04-29 15:34:40.894986 chromatic_tda-1.0.9/chromatic_tda/core/core_chromatic_alpha_complex.py
+-rw-r--r--   0        0        0     6716 2024-04-29 14:42:32.083934 chromatic_tda-1.0.9/chromatic_tda/core/core_simplicial_complex.py
+-rw-r--r--   0        0        0     4396 2024-04-29 15:03:24.042872 chromatic_tda-1.0.9/chromatic_tda/core/simplicial_complex_factory.py
+-rw-r--r--   0        0        0        0 2024-02-20 15:34:57.785000 chromatic_tda-1.0.9/chromatic_tda/core/test/__init__.py
+-rw-r--r--   0        0        0     2504 2024-04-29 15:37:47.783272 chromatic_tda-1.0.9/chromatic_tda/core/test/chromatic_alpha_complex_construction_test.py
+-rw-r--r--   0        0        0    14035 2024-02-20 16:13:32.555508 chromatic_tda-1.0.9/chromatic_tda/core/test/test_data/chralph_random_10_10.json
+-rw-r--r--   0        0        0    41541 2024-02-20 16:46:03.165063 chromatic_tda-1.0.9/chromatic_tda/core/test/test_data/chralph_random_10_10_5.json
+-rw-r--r--   0        0        0    23366 2024-02-20 16:51:32.589112 chromatic_tda-1.0.9/chromatic_tda/core/test/test_data/chralph_random_15_15.json
+-rw-r--r--   0        0        0    54399 2024-02-20 16:51:50.980261 chromatic_tda-1.0.9/chromatic_tda/core/test/test_data/chralph_random_15_8_7.json
+-rw-r--r--   0        0        0     5470 2024-02-20 16:48:27.796544 chromatic_tda-1.0.9/chromatic_tda/core/test/test_data/chralph_random_5_2_1.json
+-rw-r--r--   0        0        0        0 2023-08-11 15:07:26.002000 chromatic_tda-1.0.9/chromatic_tda/entities/__init__.py
+-rw-r--r--   0        0        0     5922 2024-04-29 15:27:55.905609 chromatic_tda-1.0.9/chromatic_tda/entities/chromatic_alpha_complex.py
+-rw-r--r--   0        0        0      493 2024-04-29 14:42:32.089047 chromatic_tda-1.0.9/chromatic_tda/entities/external_delaunay.py
+-rw-r--r--   0        0        0     7714 2024-04-29 15:23:53.967550 chromatic_tda-1.0.9/chromatic_tda/entities/simplicial_complex.py
+-rw-r--r--   0        0        0        0 2023-08-11 15:07:25.999000 chromatic_tda-1.0.9/chromatic_tda/entities/test/__init__.py
+-rw-r--r--   0        0        0     2437 2024-02-20 15:36:46.390476 chromatic_tda-1.0.9/chromatic_tda/entities/test/simplicial_complex_construction_test.py
+-rw-r--r--   0        0        0        0 2023-08-11 15:07:26.011000 chromatic_tda-1.0.9/chromatic_tda/plots/__init__.py
+-rw-r--r--   0        0        0    11124 2024-02-08 20:17:37.993929 chromatic_tda-1.0.9/chromatic_tda/plots/plotting_functions.py
+-rw-r--r--   0        0        0        0 2023-08-11 15:07:25.980000 chromatic_tda-1.0.9/chromatic_tda/utils/__init__.py
+-rw-r--r--   0        0        0      613 2024-04-29 14:42:32.090880 chromatic_tda-1.0.9/chromatic_tda/utils/boundary_matrix_utils.py
+-rw-r--r--   0        0        0      832 2024-02-14 19:16:39.052368 chromatic_tda-1.0.9/chromatic_tda/utils/filter_functions.py
+-rw-r--r--   0        0        0     1003 2024-04-29 14:42:32.092060 chromatic_tda-1.0.9/chromatic_tda/utils/floating_point_utils.py
+-rw-r--r--   0        0        0     2060 2024-04-29 14:42:32.092607 chromatic_tda-1.0.9/chromatic_tda/utils/geometrical_utils.py
+-rw-r--r--   0        0        0       64 2024-04-29 14:42:32.093731 chromatic_tda-1.0.9/chromatic_tda/utils/simplex_utils.py
+-rw-r--r--   0        0        0      225 2023-08-11 15:07:25.995220 chromatic_tda-1.0.9/chromatic_tda/utils/singleton.py
+-rw-r--r--   0        0        0     1184 2024-04-29 14:42:32.095411 chromatic_tda-1.0.9/chromatic_tda/utils/timing.py
+-rw-r--r--   0        0        0      901 2024-04-30 04:45:44.910456 chromatic_tda-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4877 1970-01-01 00:00:00.000000 chromatic_tda-1.0.9/PKG-INFO
```

### Comparing `chromatic_tda-1.0.8/LICENSE.txt` & `chromatic_tda-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/README.md` & `chromatic_tda-1.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # chromatic_tda
 
-`chromatic_tda` is a package for computing six-packs of persistent diagrams of colored point clouds. Currently point clouds in R^2 with 2 or 3 colors are supported (see Future).
+`chromatic_tda` is a package for computing six-packs of persistent diagrams of colored point clouds.
+Currently, point clouds in R^2 with 2 or 3 colors are supported (see Future; an alpha version with support for higher dimension is already available!).
 
 # Installation
 
 ## Install with `pip`
 
 The package is uploaded to [PyPI](https://pypi.org/project/chromatic-tda/), so it can be installed with `pip`.
 
@@ -25,27 +26,27 @@
 
 The basic use of the package is as follows:
 ```
 import chromatic_tda as chro
 points, labels = ... # load points, labels
 chro_alpha = chro.ChromaticAlphaComplex(points, labels) simplicial_complex = chro_alpha.get_simplicial_complex(
              sub_complex=‘bi-chromatic’
-             complex=‘all’
+             full_complex=‘all’
              relative=‘mono-chromatic’
 )  # these options make sense for three colors; for two use, e.g., just sub_complex='mono-chromatic'
-six_pack = simplicial_complex.bars_six_pack() chro.plot_six_pack(six_pack)
+six_pack = simplicial_complex.bars_six_pack()
+chro.plot_six_pack(six_pack)
 ```
 
 For more details check the docstrings of the methods and the jupyter notebook file `manual` (in [github repo](https://github.com/OnDraganov/chromatic-tda)). For more background on the theory, check the resources listed below.
 
 # Future
 
-The code is under active developement. The future plans include:
-- Adding support for points in R^3
-- Making persistence computation faster with clearing.
+The code is under active development. The future plans include:
+- Adding support for points in R^3 --> alpha version with a 3D support available in a separate branch: see https://github.com/OnDraganov/chromatic-tda/tree/general-radius-function
 
 # Resources
 
 The code is based on research done at Institute of Science and Technology by Ranita Biswas, Sebastiano Cultrera di Montesano, Ondřej Draganov, Herbert Edelsbrunner and Morteza Saghafian. A draft write up can be found on [arxiv](https://arxiv.org/abs/2212.03128).
 
 A presentation about the main concepts used in this package can be viewed on YouTube: [AATRN Online Seminar: TDA for Chromatic Point Clouds](https://youtu.be/HIqiF00yKaw). A recording of a complementary talk focusing more on the motivations of the work and the combinatorial structures underlying it is accessible through [google drive](https://drive.google.com/file/d/1RBiGlgY4mlRL59eAVmMLrgBCZYN97QnZ/view).
```

### Comparing `chromatic_tda-1.0.8/chromatic_tda/algorithms/chromatic_subcomplex_utils.py` & `chromatic_tda-1.0.9/chromatic_tda/algorithms/chromatic_subcomplex_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,107 +1,133 @@
 import itertools
 
 from chromatic_tda.core.core_simplicial_complex import CoreSimplicialComplex
 from chromatic_tda.core.simplicial_complex_factory import CoreSimplicialComplexFactory
 
 
-def get_chromatic_subcomplex(sub_complex, full_complex, relative,
-                             simplicial_complex: CoreSimplicialComplex, internal_labeling,
-                             labels_user_to_internal=None, allow_unused_labels=False) -> CoreSimplicialComplex:
-    list_of_input_labels = construct_list_of_labels(internal_labeling=internal_labeling,
-                                                    labels_user_to_internal=labels_user_to_internal)
-    if full_complex is None or full_complex == '' or full_complex.lower().strip() == 'all':
-        complex_simplices = set(simplicial_complex.boundary)
-    else:
-        pattern = read_pattern_input(full_complex, list_of_input_labels, check_labels=not allow_unused_labels)
-        if labels_user_to_internal is not None:
-            pattern = pattern_translate(pattern=pattern, translation_function=labels_user_to_internal)
-        complex_simplices = select_simplices_with_chromatic_pattern(
-            simplices=simplicial_complex.boundary.keys(), labeling_function=internal_labeling, pattern=pattern)
-
-    if relative is None or relative == '':
-        relative_simplices = set()
-    else:
-        pattern = read_pattern_input(relative, list_of_input_labels, check_labels=not allow_unused_labels)
-        if labels_user_to_internal is not None:
-            pattern = pattern_translate(pattern=pattern, translation_function=labels_user_to_internal)
-        relative_simplices = select_simplices_with_chromatic_pattern(
-            simplices=simplicial_complex.boundary.keys(), labeling_function=internal_labeling, pattern=pattern)
-
-    if sub_complex is None or sub_complex == '':
-        sub_complex_simplices = set()
-    else:
-        pattern = read_pattern_input(sub_complex, list_of_input_labels, check_labels=not allow_unused_labels)
+class ChromaticComplexUtils:
+    @staticmethod
+    def get_chromatic_subcomplex(sub_complex, full_complex, relative,
+                                 simplicial_complex: CoreSimplicialComplex, internal_labeling,
+                                 labels_user_to_internal=None, allow_unused_labels=False) -> CoreSimplicialComplex:
+        list_of_input_labels = ChromaticComplexUtils.construct_list_of_labels(
+            internal_labeling=internal_labeling, labels_user_to_internal=labels_user_to_internal)
+        if (full_complex is None or full_complex == '' or
+                (isinstance(full_complex, str) and full_complex.lower().strip() == 'all')):
+            complex_simplices = set(simplicial_complex.boundary)
+        else:
+            pattern = ChromaticComplexUtils.read_pattern_input(full_complex, list_of_input_labels,
+                                                               check_labels=not allow_unused_labels)
+            if labels_user_to_internal is not None:
+                pattern = ChromaticComplexUtils.pattern_translate(pattern=pattern,
+                                                                  translation_function=labels_user_to_internal)
+            complex_simplices = ChromaticComplexUtils.select_simplices_with_chromatic_pattern(
+                simplices=simplicial_complex.boundary.keys(), labeling_function=internal_labeling, pattern=pattern)
+
+        if relative is None or relative == '':
+            relative_simplices = set()
+        elif isinstance(relative, str) and relative.lower().strip() == 'all':
+            relative_simplices = set(simplicial_complex.boundary)
+        else:
+            pattern = ChromaticComplexUtils.read_pattern_input(relative, list_of_input_labels,
+                                                               check_labels=not allow_unused_labels)
+            if labels_user_to_internal is not None:
+                pattern = ChromaticComplexUtils.pattern_translate(pattern=pattern,
+                                                                  translation_function=labels_user_to_internal)
+            relative_simplices = ChromaticComplexUtils.select_simplices_with_chromatic_pattern(
+                simplices=simplicial_complex.boundary.keys(), labeling_function=internal_labeling, pattern=pattern)
+
+        if sub_complex is None or sub_complex == '':
+            sub_complex_simplices = set()
+        elif isinstance(sub_complex, str) and sub_complex.lower().strip() == 'all':
+            sub_complex_simplices = set(simplicial_complex.boundary)
+        else:
+            pattern = ChromaticComplexUtils.read_pattern_input(sub_complex, list_of_input_labels,
+                                                               check_labels=not allow_unused_labels)
+            if labels_user_to_internal is not None:
+                pattern = ChromaticComplexUtils.pattern_translate(pattern=pattern,
+                                                                  translation_function=labels_user_to_internal)
+            sub_complex_simplices = ChromaticComplexUtils.select_simplices_with_chromatic_pattern(
+                simplices=simplicial_complex.boundary.keys(), labeling_function=internal_labeling, pattern=pattern)
+
+        restricted_complex: CoreSimplicialComplex = CoreSimplicialComplexFactory().create_restricted_instance(
+            simplicial_complex, complex_simplices - relative_simplices)
+        restricted_complex.set_sub_complex(sub_complex_simplices - relative_simplices)
+
+        return restricted_complex
+
+    @staticmethod
+    def construct_list_of_labels(internal_labeling, labels_user_to_internal):
         if labels_user_to_internal is not None:
-            pattern = pattern_translate(pattern=pattern, translation_function=labels_user_to_internal)
-        sub_complex_simplices = select_simplices_with_chromatic_pattern(
-            simplices=simplicial_complex.boundary.keys(), labeling_function=internal_labeling, pattern=pattern)
-
-    restricted_complex : CoreSimplicialComplex = CoreSimplicialComplexFactory().create_restricted_instance(
-        simplicial_complex, complex_simplices - relative_simplices)
-    restricted_complex.set_sub_complex(sub_complex_simplices - relative_simplices)
-
-    return restricted_complex
-
-
-def construct_list_of_labels(internal_labeling, labels_user_to_internal):
-    if labels_user_to_internal is not None:
-        return set(labels_user_to_internal.keys())
-    if isinstance(internal_labeling, dict):
-        return set(internal_labeling.values())
-    return set(internal_labeling)
-
-
-def read_pattern_input(parameter, labels=None, check_labels=True):
-    if isinstance(parameter, str):
-        pattern_list_of_sets = read_pattern_input_string(parameter, labels=labels)
-    else:
-        pattern_list_of_sets = [set(color_set) for color_set in parameter]
-
-    if labels is not None and check_labels:  # check that the pattern only uses the given labels
-        for lab in set().union(*pattern_list_of_sets):
-            if lab not in labels:
-                raise ValueError(f"There is no point labeled by `{lab}`. "
-                                 f"To suppress this error, pass allow_unused_labels=True to get_complex function")
-
-    return pattern_list_of_sets
-
-
-def read_pattern_input_string(parameter: str, labels=None):
-    parameter = parameter.lower().strip()
-    if parameter.endswith('chromatic'):
-        chromaticity = parameter.replace('chromatic', '').replace('-', '')
-        words_to_numbers = {'mono': 1, 'one': 1, 'bi': 2, 'two': 2, 'tri': 3, 'three': 3, 'tetra': 4, 'four': 4}
-        if chromaticity in words_to_numbers:
-            chromaticity = words_to_numbers[chromaticity]
-        elif chromaticity.isnumeric() and chromaticity != '0':
-            chromaticity = int(chromaticity)
+            return set(labels_user_to_internal.keys())
+        if isinstance(internal_labeling, dict):
+            return set(internal_labeling.values())
+        return set(internal_labeling)
+
+    @staticmethod
+    def read_pattern_input(parameter, labels=None, check_labels=True):
+        if isinstance(parameter, str):
+            pattern_list_of_sets = ChromaticComplexUtils.read_pattern_input_string(parameter, labels=labels)
         else:
-            raise ValueError(f"The color pattern `{parameter}` is invalid")
-        if labels is None:
-            raise ValueError(f"'k-chromatic' option given with labels=None. List of labels is needed for this option.")
-        if labels and chromaticity > len(labels):
-            chromaticity = len(labels)  # 4-chromatic subcomplex of 3-colored should still be the full complex
-        pattern_list_of_sets = [set(x) for x in itertools.combinations(labels, chromaticity)]
-    else:
-        pattern_list_of_sets = [{int(ch) if ch.isnumeric() else ch for ch in w} for w in parameter.split(',')]
-
-    return pattern_list_of_sets
-
-
-def simplex_satisfies_pattern(simplex, labeling_function, pattern):
-    """
-    Return true iff the colors of the simplex are subset of one of the patterns.
-    simplex ... sorted tuple of vertices
-    labeling ... list or dictionary giving a label to each possible vertex
-    pattern ... collection of sets of labels
-    """
-    simplex_labels = {labeling_function[v] for v in simplex}
-    return any(simplex_labels.issubset(s) for s in pattern)
+            pattern_list_of_sets = [set(color_set) for color_set in parameter]
 
+        if labels is not None and check_labels:  # check that the pattern only uses the given labels
+            for lab in set().union(*pattern_list_of_sets):
+                if lab not in labels:
+                    raise ValueError(f"There is no point labeled by `{lab}`. "
+                                     f"To suppress this error, pass allow_unused_labels=True to get_complex function")
+
+        return pattern_list_of_sets
+
+    @staticmethod
+    def read_pattern_input_string(parameter: str, labels=None):
+        parameter = parameter.lower().strip()
+        if parameter.endswith('chromatic'):
+            chromaticity = parameter.replace('chromatic', '').replace('-', '')
+            words_to_numbers = {'mono': 1, 'one': 1, 'bi': 2, 'two': 2, 'tri': 3, 'three': 3, 'tetra': 4, 'four': 4}
+            if chromaticity in words_to_numbers:
+                chromaticity = words_to_numbers[chromaticity]
+            elif chromaticity.isnumeric() and chromaticity != '0':
+                chromaticity = int(chromaticity)
+            else:
+                raise ValueError(f"The color pattern `{parameter}` is invalid")
+            if labels is None:
+                raise ValueError(
+                    f"'k-chromatic' option given with labels=None. List of labels is needed for this option.")
+            if labels and chromaticity > len(labels):
+                chromaticity = len(labels)  # 4-chromatic subcomplex of 3-colored should still be the full complex
+            pattern_list_of_sets = [set(x) for x in itertools.combinations(labels, chromaticity)]
+        else:
+            pattern_list_of_sets = [{int(ch) if ch.isnumeric() else ch for ch in w} for w in parameter.split(',')]
 
-def select_simplices_with_chromatic_pattern(simplices, labeling_function, pattern):
-    return set(simplex for simplex in simplices if simplex_satisfies_pattern(simplex, labeling_function, pattern))
+        return pattern_list_of_sets
 
+    @staticmethod
+    def simplex_satisfies_pattern(simplex, labeling_function, pattern):
+        """
+        Return true iff the colors of the simplex are subset of one of the patterns.
+        simplex ... sorted tuple of vertices
+        labeling ... list or dictionary giving a label to each possible vertex
+        pattern ... collection of sets of labels
+        """
+        simplex_labels = {labeling_function[v] for v in simplex}
+        return any(simplex_labels.issubset(s) for s in pattern)
+
+    @staticmethod
+    def select_simplices_with_chromatic_pattern(simplices, labeling_function, pattern):
+        return set(simplex for simplex in simplices
+                   if ChromaticComplexUtils.simplex_satisfies_pattern(simplex, labeling_function, pattern))
+
+    @staticmethod
+    def pattern_translate(pattern, translation_function):
+        return [set(translation_function[lab] for lab in face if lab in translation_function) for face in pattern]
+
+    @staticmethod
+    def split_simplex_by_labels(simplex: tuple, labeling) -> dict:
+        simplex_split = {}
+        for v in simplex:
+            lab = labeling[v]
+            if lab not in simplex_split:
+                simplex_split[lab] = []
+            simplex_split[lab].append(v)
 
-def pattern_translate(pattern, translation_function):
-    return [set(translation_function[lab] for lab in face) for face in pattern]
+        return simplex_split
```

### Comparing `chromatic_tda-1.0.8/chromatic_tda/algorithms/persistence_algorithm.py` & `chromatic_tda-1.0.9/chromatic_tda/algorithms/persistence_algorithm.py`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/chromatic_tda/algorithms/radius_function_utils.py` & `chromatic_tda-1.0.9/chromatic_tda/algorithms/radius_function_utils.py`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/chromatic_tda/algorithms/reduce_matrix.py` & `chromatic_tda-1.0.9/chromatic_tda/algorithms/reduce_matrix.py`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/chromatic_tda/core/chromatic_alpha_complex_factory.py` & `chromatic_tda-1.0.9/chromatic_tda/core/chromatic_alpha_complex_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     @staticmethod
     def init_labels(alpha_complex: CoreChromaticAlphaComplex, labels) -> None:
         alpha_complex.input_labels_to_internal_labels_dict = {lab: i for i, lab in enumerate(sorted(set(labels)))}
         alpha_complex.internal_labels_to_input_labels_dict = {
             i: lab for lab, i in alpha_complex.input_labels_to_internal_labels_dict.items()
         }
         alpha_complex.labels_number = len(alpha_complex.input_labels_to_internal_labels_dict)
-        alpha_complex.internal_labels = [alpha_complex.input_labels_to_internal_labels_dict[lab] for lab in labels]
+        alpha_complex.internal_labeling = [alpha_complex.input_labels_to_internal_labels_dict[lab] for lab in labels]
 
     @staticmethod
     def perturb_points(points, point_perturbation):
         return [[p + point_perturbation * (random.random() - .5) for p in pt] for pt in points]
 
     def build_alpha_complex_structure(self, alpha_complex: CoreChromaticAlphaComplex, lift_perturbation) -> None:
         """
@@ -60,21 +60,21 @@
         TimingUtils().start("Build Alpha Complex Structure")
 
         if alpha_complex.points.shape[1] != 2:
             raise ValueError("Points has to be an iterable of two-dimensional points.")
 
         if alpha_complex.labels_number > 3:
             raise ValueError(f"There can be at most 3 different labels, {alpha_complex.labels_number} given.")
-        if len(alpha_complex.points) != len(alpha_complex.internal_labels):
+        if len(alpha_complex.points) != len(alpha_complex.internal_labeling):
             raise ValueError("The list of labels must have the same length as the list of points.")
 
         colorful_maximal_simplices = self.compute_chromatic_delaunay(alpha_complex, lift_perturbation)
-        TimingUtils().start("Build Chromatic Delaunay from Max Simplices")
+        TimingUtils().start("Build Chro Del from Max Simplices")
         alpha_complex.simplicial_complex = CoreSimplicialComplexFactory().create_instance(colorful_maximal_simplices)
-        TimingUtils().stop("Build Chromatic Delaunay from Max Simplices")
+        TimingUtils().stop("Build Chro Del from Max Simplices")
 
         alpha_complex.simplicial_complex.co_boundary = boundary_matrix_utils.make_co_boundary(
             alpha_complex.simplicial_complex.boundary)
 
         RadiusFunctionUtils().compute_radius_function(alpha_complex)
 
         TimingUtils().stop("Build Alpha Complex Structure")
@@ -89,30 +89,30 @@
         Returns
         -------
         List of maximal simplices of the chromatic Delaunay complex.
         """
         TimingUtils().start("Compute Chromatic Delaunay")
 
         del_complex = Delaunay(self.chromatic_lift(alpha_complex, lift_perturbation))
-        all_labels = set(alpha_complex.internal_labels)
+        all_labels = set(alpha_complex.internal_labeling)
         colorful_maximal_simplices = [simplex for simplex in del_complex.simplices
-                                      if set(alpha_complex.internal_labels[i] for i in simplex) == all_labels]
+                                      if set(alpha_complex.internal_labeling[i] for i in simplex) == all_labels]
 
         TimingUtils().stop("Compute Chromatic Delaunay")
 
         return colorful_maximal_simplices
 
     @staticmethod
     def chromatic_lift(alpha_complex: CoreChromaticAlphaComplex, lift_perturbation):
         """
         Add extra coordinates to lift points to the chromatic simplex. Here we choose one-hot embedding without
         the first coordinate. That is, 0 --> (0,0,0,...), 1 --> (1,0,0,...), 2 --> (0,1,0,...), etc.
         """
         pts_lift = np.array([
             np.concatenate((point, [1 if i == label else 0 for i in range(1, alpha_complex.labels_number)]))
-            for point, label in zip(alpha_complex.points, alpha_complex.internal_labels)])
+            for point, label in zip(alpha_complex.points, alpha_complex.internal_labeling)])
         if lift_perturbation:
             prefix = [0] * alpha_complex.points_dimension
             for pt in pts_lift:
                 pt += prefix + [lift_perturbation * random.random() for _ in range(1, alpha_complex.labels_number)]
 
         return pts_lift
```

### Comparing `chromatic_tda-1.0.8/chromatic_tda/core/core_chromatic_alpha_complex.py` & `chromatic_tda-1.0.9/chromatic_tda/core/core_chromatic_alpha_complex.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import numpy as np
 
+from chromatic_tda.algorithms.chromatic_subcomplex_utils import ChromaticComplexUtils
 from chromatic_tda.core.core_simplicial_complex import CoreSimplicialComplex
 from chromatic_tda.utils.geometrical_utils import sq_dist
 from chromatic_tda.algorithms import chromatic_subcomplex_utils
 
 
 class CoreChromaticAlphaComplex:
     points: np.ndarray
     points_dimension: int
     input_labels_to_internal_labels_dict: dict
     internal_labels_to_input_labels_dict: dict
     labels_number: int
-    internal_labels: list
+    internal_labeling: list
     simplicial_complex: CoreSimplicialComplex
     sq_rad: dict
 
     def __init__(self) -> None:
         self.input_labels_to_internal_labels_dict = {}
         self.labels_number = 0
-        self.internal_labels = []
+        self.internal_labeling = []
         self.sq_rad = {}
 
     def __iter__(self):
         yield from self.simplicial_complex
 
     def __len__(self) -> int:
         return len(self.simplicial_complex)
@@ -31,24 +32,24 @@
         return element in self.simplicial_complex
 
     def copy_points(self):
         """Return a copy of the points"""
         return np.array(self.points)
 
     def simplex_labels_internal(self, simplex):
-        return {self.internal_labels[v] for v in simplex}
+        return {self.internal_labeling[v] for v in simplex}
 
     def simplex_labels_input(self, simplex):
         """Return set of labels of the vertices of the given simplex"""
         return {self.internal_labels_to_input_labels_dict[lab] for lab in self.simplex_labels_internal(simplex)}
 
-    def get_complex(self, sub_complex, full_complex, relative, allow_unused_labels=False) -> CoreSimplicialComplex:
-        return chromatic_subcomplex_utils.get_chromatic_subcomplex(
+    def get_complex(self, sub_complex, full_complex, relative, allow_unused_labels) -> CoreSimplicialComplex:
+        return ChromaticComplexUtils.get_chromatic_subcomplex(
             sub_complex=sub_complex, full_complex=full_complex, relative=relative,
-            simplicial_complex=self.simplicial_complex, internal_labeling=self.internal_labels,
+            simplicial_complex=self.simplicial_complex, internal_labeling=self.internal_labeling,
             labels_user_to_internal=self.input_labels_to_internal_labels_dict,
             allow_unused_labels=allow_unused_labels
         )
 
     def star_vertices(self, simplex) -> set:
         return set().union(*self.simplicial_complex.co_boundary[simplex]) - set(simplex)
 
@@ -61,28 +62,28 @@
         the corresponding colors. Colors not present in simplex
         are treated as automatically satisfied.
         """
         vertices_to_check = self.star_vertices(simplex)
         for mono_chrom_face in self.split_simplex(simplex):  # for every color
             if len(mono_chrom_face) > 0:  # if the color is present in simplex
                 radius = sq_dist(center, self.points[mono_chrom_face[0]])
-                if any((self.internal_labels[mono_chrom_face[0]] == self.internal_labels[v] and
+                if any((self.internal_labeling[mono_chrom_face[0]] == self.internal_labeling[v] and
                         sq_dist(center, self.points[v]) < radius)
                        for v in vertices_to_check):
                     return False
         return True
 
     def split_simplex(self, simplex) -> list:
-        return [tuple(i for i in simplex if self.internal_labels[i] == 0),
-                tuple(i for i in simplex if self.internal_labels[i] == 1),
-                tuple(i for i in simplex if self.internal_labels[i] == 2)]
+        return [tuple(i for i in simplex if self.internal_labeling[i] == 0),
+                tuple(i for i in simplex if self.internal_labeling[i] == 1),
+                tuple(i for i in simplex if self.internal_labeling[i] == 2)]
 
     def split_simplex_sort_by_size(self, simplex) -> list:
         return sorted(self.split_simplex(simplex), key=len, reverse=True)
 
     def write(self) -> None:
         print()
         print(f"**** Delaunay Complex (dimension = {self.simplicial_complex.get_dimension()}) ****")
-        for (p, l) in zip(self.points, self.internal_labels):
+        for (p, l) in zip(self.points, self.internal_labeling):
             print(f"{p} -> {l}")
         print(42 * "*")
         print()
```

### Comparing `chromatic_tda-1.0.8/chromatic_tda/core/core_simplicial_complex.py` & `chromatic_tda-1.0.9/chromatic_tda/core/core_simplicial_complex.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         return len(self.boundary)
 
     def __contains__(self, item) -> bool:
         return item in self.boundary
 
     def clear(self) -> None:
         self.dim_simplex_dict = {}
-        self.simplex_weights = {}
+        self.simplex_weights = {}  # radius values of simplices
 
         self.boundary = {}  # example: {(1,2,3) : {(1,2), (1,3), (2,3)}, (1,2) : {(1), (2)}, ...}
         self.co_boundary = {}  # example:  {(1,2) : {(1,2,3), (1,2,4)}, (1,3) : {(1,2,3), (1,3,4)}, ...}
 
         self.sub_complex = set()
         self.persistence_data = {}
         self.birth_death = {}
@@ -99,17 +99,19 @@
 
         Note: Monotonicity is NOT checked.
         """
         self.simplex_weights = {simplex: default_value for simplex in self.boundary}
         for simplex, weight in weight_function.items():
             simplex_tuple = tuple(sorted(simplex))
             if simplex_tuple not in self.boundary:
-                raise ValueError(f"Simplex {simplex} is not in the simplicial complex, cannot add its weight.")
+                raise ValueError(f"Simplex {simplex_tuple} is not in the simplicial complex, cannot add its weight.")
+            if weight < default_value:
+                raise Warning(f"Simplex {simplex_tuple} given weight lower than default.")
             self.simplex_weights[simplex_tuple] = weight
-        co_boundary = (self.co_boundary if len(self.co_boundary) > 0
+        co_boundary = (self.co_boundary if self.co_boundary
                        else boundary_matrix_utils.make_co_boundary(self.boundary))
         floating_point_utils.ensure_weights_monotonicity_and_equal_values(self.simplex_weights, co_boundary)
 
     def get_weight_function_copy(self) -> dict:
         """Return copy of {simplex : weight} dictionary."""
         return {simplex: weight for simplex, weight in self.simplex_weights.items()}
```

### Comparing `chromatic_tda-1.0.8/chromatic_tda/core/simplicial_complex_factory.py` & `chromatic_tda-1.0.9/chromatic_tda/core/simplicial_complex_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from itertools import combinations
 from chromatic_tda.core.core_simplicial_complex import CoreSimplicialComplex
 from chromatic_tda.utils import boundary_matrix_utils, simplex_utils
 
 
 @singleton
 class CoreSimplicialComplexFactory:
+    EMPTY_COMPLEX_DIMENSION = -1
 
     def create_instance(self, simplices) -> CoreSimplicialComplex:
         simplicial_complex = CoreSimplicialComplex()
         self.build_complex(simplicial_complex, simplices)
 
         return simplicial_complex
 
@@ -34,15 +35,16 @@
         simplicial_complex.dim_simplex_dict = self.build_dimension_dictionary(
             simplex_list, max_dimension=simplicial_complex.dimension)
         self.add_boundary_and_missing_simplices(simplicial_complex)
         simplicial_complex.set_simplex_weights({})
 
     @staticmethod
     def find_maximal_dimension(simplex_list):
-        return max(simplex_utils.dimension(simplex) for simplex in simplex_list)
+        return max((simplex_utils.dimension(simplex) for simplex in simplex_list),
+                   default = CoreSimplicialComplexFactory().EMPTY_COMPLEX_DIMENSION)
 
     @staticmethod
     def build_dimension_dictionary(simplex_list, max_dimension):
         dim_simplex_dict = {dim : set() for dim in range(max_dimension, -1, -1)}
         for simplex in simplex_list:
             simplex_dim = simplex_utils.dimension(simplex)
             dim_simplex_dict[simplex_dim].add(tuple(sorted(simplex)))
@@ -55,24 +57,26 @@
                 simplicial_complex.boundary[simplex] = set(combinations(simplex, dim))
             simplicial_complex.dim_simplex_dict[dim - 1] = simplicial_complex.dim_simplex_dict[dim - 1].union(
                 *[simplicial_complex.boundary[simplex] for simplex in simplicial_complex.dim_simplex_dict[dim]])
         for vertex in simplicial_complex.dim_simplex_dict[0]:
             simplicial_complex.boundary[vertex] = set()
 
     @staticmethod
-    def create_restricted_instance(complex: CoreSimplicialComplex, restricted_simplices) -> CoreSimplicialComplex:
+    def create_restricted_instance(simplicial_complex: CoreSimplicialComplex,
+                                   restricted_simplices) -> CoreSimplicialComplex:
         """Return a new SimplicialComplex restricted to given simplices."""
         new_complex : CoreSimplicialComplex = CoreSimplicialComplex()
         restricted_simplices_set : set = set(restricted_simplices)
 
-        new_complex.dim_simplex_dict = {d : complex.dim_simplex_dict[d] & restricted_simplices_set
-                                        for d in complex.dim_simplex_dict}
+        new_complex.dim_simplex_dict = {d : simplicial_complex.dim_simplex_dict[d] & restricted_simplices_set
+                                        for d in simplicial_complex.dim_simplex_dict}
         new_complex.clear_empty_dimensions()
-        new_complex.dimension = max(new_complex.dim_simplex_dict)
+        new_complex.dimension = max(new_complex.dim_simplex_dict,
+                                    default = CoreSimplicialComplexFactory().EMPTY_COMPLEX_DIMENSION)
 
-        new_complex.boundary = {simplex: complex.boundary[simplex] & restricted_simplices_set
-                                for simplex in set(complex.boundary) & restricted_simplices_set}
+        new_complex.boundary = {simplex: simplicial_complex.boundary[simplex] & restricted_simplices_set
+                                for simplex in set(simplicial_complex.boundary) & restricted_simplices_set}
         new_complex.co_boundary = boundary_matrix_utils.make_co_boundary(new_complex.boundary)
-        new_complex.simplex_weights = {simplex : complex.simplex_weights[simplex] for simplex in new_complex.boundary}
-        new_complex.sub_complex = complex.sub_complex & restricted_simplices_set
+        new_complex.simplex_weights = {simplex : simplicial_complex.simplex_weights[simplex] for simplex in new_complex.boundary}
+        new_complex.sub_complex = simplicial_complex.sub_complex & restricted_simplices_set
 
         return new_complex
```

### Comparing `chromatic_tda-1.0.8/chromatic_tda/core/test/chromatic_alpha_complex_construction_test.py` & `chromatic_tda-1.0.9/chromatic_tda/core/test/chromatic_alpha_complex_construction_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     def test_chromatic_alpha_random_15_8_7(self):
         result = self.single_test(data_name='chralph_random_15_8_7')
         assert result
 
     def single_test(self, data_name, data_folder=None):
         data = self.load_data(data_name, data_folder)
         factory = CoreChromaticAlphaComplexFactory()
-        alpha = factory.create_instance(points=data['points'], labels=data['labels'], lift_perturbation=1e-9,
-                                        point_perturbation=None)
+        alpha = factory.create_instance(points=data['points'], labels=data['labels'],
+                                        lift_perturbation=1e-9, point_perturbation=None)
         return self.compare_complex(alpha, data['weight_function'])
 
     def load_data(self, data_name, data_folder):
         if data_folder is None:
             data_folder = self.data_folder
         with open(data_folder / (data_name + '.json'), 'r') as file:
             data = json.load(file)
```

### Comparing `chromatic_tda-1.0.8/chromatic_tda/core/test/test_data/chralph_random_10_10.json` & `chromatic_tda-1.0.9/chromatic_tda/core/test/test_data/chralph_random_10_10.json`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/chromatic_tda/core/test/test_data/chralph_random_10_10_5.json` & `chromatic_tda-1.0.9/chromatic_tda/core/test/test_data/chralph_random_10_10_5.json`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/chromatic_tda/core/test/test_data/chralph_random_15_15.json` & `chromatic_tda-1.0.9/chromatic_tda/core/test/test_data/chralph_random_15_15.json`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/chromatic_tda/core/test/test_data/chralph_random_15_8_7.json` & `chromatic_tda-1.0.9/chromatic_tda/core/test/test_data/chralph_random_15_8_7.json`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/chromatic_tda/core/test/test_data/chralph_random_5_2_1.json` & `chromatic_tda-1.0.9/chromatic_tda/core/test/test_data/chralph_random_5_2_1.json`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/chromatic_tda/entities/chromatic_alpha_complex.py` & `chromatic_tda-1.0.9/chromatic_tda/entities/chromatic_alpha_complex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from chromatic_tda.core.core_chromatic_alpha_complex import CoreChromaticAlphaComplex
 from chromatic_tda.core.chromatic_alpha_complex_factory import CoreChromaticAlphaComplexFactory
 from chromatic_tda.entities.simplicial_complex import SimplicialComplex
 
 
 class ChromaticAlphaComplex:
 
-    def __init__(self, points, labels, lift_perturbation=1e-9, point_perturbation=None, **kwargs) -> None:
+    def __init__(self, points, labels, lift_perturbation=1e-9, point_perturbation=None) -> None:
         """Create an instance of ChromaticAlphaComplex. The object contains the full chromatic Delaunay complex together
         with its alpha radius function.
 
         Arguments:
             points ... List of point coordinates
             labels ... List of labels. The length has to be the same as the number of points.
                        The first label goes with the first point, etc... The labels can be any hashable object.
@@ -18,26 +18,27 @@
             point_perturbation ... Perturb the points given on the input by +-point_perturbation/2 in each coordinate.
                                    (default: None)
             lift_perturbation ... Compute the Delaunay complex with perturbed lifting to break the non-general position.
                                   Generally leads to faster computation, as QHull does not need to deal with the
                                   non-generality itself. (default: 1e-9)
         """
         self.core_alpha_complex : CoreChromaticAlphaComplex = CoreChromaticAlphaComplexFactory().create_instance(
-            points, labels, lift_perturbation=lift_perturbation, point_perturbation=point_perturbation, **kwargs)
+            points, labels, lift_perturbation=lift_perturbation, point_perturbation=point_perturbation)
 
     def __iter__(self):
         yield from self.core_alpha_complex
 
     def __len__(self) -> int:
         return len(self.core_alpha_complex)
 
     def __contains__(self, element) -> bool:
         return element in self.core_alpha_complex
 
-    def get_simplicial_complex(self, sub_complex=None, complex=None, relative=None, allow_unused_labels=False) -> SimplicialComplex:
+    def get_simplicial_complex(self, sub_complex=None, full_complex=None, relative=None,
+                               allow_unused_labels=False) -> SimplicialComplex:
         """Generate a simplicial complex and sub-complex pair based on the parameters given.
         The parameter complex restricts the complex, the parameter sub_complex defines the sub-complex,
         and the parameter relative erases simplices from the complex to represent a relative simplicial complex.
 
         Each parameter can be given as a list of lists of labels. Each simplex is kept (for sub_complex and complex)
         or erased (for relative) iff the set of labels of its vertices is contained in one of the lists of labels.
         For example sub_complex=[['blue', 'red'], ['blue', 'green']] chooses those simplices whose vertices are labeled
@@ -56,15 +57,16 @@
             Can also be written as 'one-chromatic' or '1-chromatic' etc... The dash is optional.
 
         Keyword arguments:
         allow_unused_labels ... By default (False), an error is raised if the sub_complex/complex/relative parameters
                                 contain a label that is not used. To suppress this behavior, set this parameter to True.
                                 In that case the unused labels make no difference on the result.
         """
-        return SimplicialComplex(self.core_alpha_complex.get_complex(sub_complex, complex, relative, allow_unused_labels))
+        return SimplicialComplex(self.core_alpha_complex.get_complex(sub_complex, full_complex, relative,
+                                                                     allow_unused_labels))
 
     def weight_function(self, simplex=None):
         """If simplex is given, return the weight/radius of the simplex.
         If no simplex is given, return the weight/radius function as a dictionary {simplex : weight}."""
         if simplex is None:
             return self.core_alpha_complex.simplicial_complex.get_weight_function_copy()
         return self.core_alpha_complex.simplicial_complex.get_simplex_weight(simplex)
@@ -90,8 +92,8 @@
     def points(self):
         """Return the point cloud defining the complex."""
         return self.core_alpha_complex.copy_points()
 
     def labels(self):
         """Return the labels for the points defining the complex."""
         return [self.core_alpha_complex.internal_labels_to_input_labels_dict[lab]
-                for lab in self.core_alpha_complex.internal_labels]
+                for lab in self.core_alpha_complex.internal_labeling]
```

### Comparing `chromatic_tda-1.0.8/chromatic_tda/entities/simplicial_complex.py` & `chromatic_tda-1.0.9/chromatic_tda/entities/simplicial_complex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
+from chromatic_tda.algorithms.chromatic_subcomplex_utils import ChromaticComplexUtils
 from chromatic_tda.algorithms.persistence_algorithm import PersistenceAlgorithm
 from chromatic_tda.core.core_simplicial_complex import CoreSimplicialComplex
 from chromatic_tda.core.simplicial_complex_factory import CoreSimplicialComplexFactory
-from chromatic_tda.algorithms import chromatic_subcomplex_utils
 
 
 class SimplicialComplex:
 
     GROUPS = ['kernel', 'sub_complex', 'image', 'complex', 'cokernel', 'relative']
     core_complex: CoreSimplicialComplex
 
@@ -135,11 +135,11 @@
 
     def get_chromatic_subcomplex(self, labeling, sub_complex=None, full_complex=None, relative=None,
                                  allow_unused_labels=False):
         """Ignoring the current subcomplex, return a new SimplicialComplex as a chromatic subcomplex given by
         the parameters (see docstring of ChromaticAlphaComplex.get_simplicial_complex).
         Argument labeling is a dictionary or a list such that labeling[vertex] = label;
         A previously defined sub_complex of the complex is NOT preserved."""
-        return SimplicialComplex(chromatic_subcomplex_utils.get_chromatic_subcomplex(
+        return SimplicialComplex(ChromaticComplexUtils.get_chromatic_subcomplex(
             internal_labeling=labeling, sub_complex=sub_complex, full_complex=full_complex, relative=relative,
             simplicial_complex=self.core_complex, allow_unused_labels=allow_unused_labels)
         )
```

### Comparing `chromatic_tda-1.0.8/chromatic_tda/entities/test/simplicial_complex_construction_test.py` & `chromatic_tda-1.0.9/chromatic_tda/entities/test/simplicial_complex_construction_test.py`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/chromatic_tda/plots/plotting_functions.py` & `chromatic_tda-1.0.9/chromatic_tda/plots/plotting_functions.py`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/chromatic_tda/utils/boundary_matrix_utils.py` & `chromatic_tda-1.0.9/chromatic_tda/utils/boundary_matrix_utils.py`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/chromatic_tda/utils/filter_functions.py` & `chromatic_tda-1.0.9/chromatic_tda/utils/filter_functions.py`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/chromatic_tda/utils/floating_point_utils.py` & `chromatic_tda-1.0.9/chromatic_tda/utils/floating_point_utils.py`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/chromatic_tda/utils/geometrical_utils.py` & `chromatic_tda-1.0.9/chromatic_tda/utils/geometrical_utils.py`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/chromatic_tda/utils/timing.py` & `chromatic_tda-1.0.9/chromatic_tda/utils/timing.py`

 * *Files identical despite different names*

### Comparing `chromatic_tda-1.0.8/pyproject.toml` & `chromatic_tda-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chromatic_tda"
-version = "1.0.8"
+version = "1.0.9"
 description = "Tool to compute six-packs of persistence diagrams for chromatic point clouds"
 authors = [
     "Ondrej Draganov <ondrej.draganov@ist.ac.at>",
     "Mohammad Mahini <m.mahini@gmail.com>"
     ]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
@@ -16,17 +16,17 @@
 ]
 keywords = [
     "tda", "topological data analysis", "chromatic", "chromatic alpha", "delaunay", "persistence", "persistent homology"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
-numpy = "^1.24.2"
+numpy = "^1.26.4"
 matplotlib = "^3.7.0"
 scipy = "^1.10.1"
 mypy = "^1.3.0"
-pytest = "^8.0.0"
+pytest = "^8.1.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `chromatic_tda-1.0.8/PKG-INFO` & `chromatic_tda-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: chromatic_tda
-Version: 1.0.8
+Version: 1.0.9
 Summary: Tool to compute six-packs of persistence diagrams for chromatic point clouds
 Home-page: https://github.com/OnDraganov/chromatic-tda
 License: AGPL-3.0-or-later
 Keywords: tda,topological data analysis,chromatic,chromatic alpha,delaunay,persistence,persistent homology
 Author: Ondrej Draganov
 Author-email: ondrej.draganov@ist.ac.at
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
 Requires-Dist: mypy (>=1.3.0,<2.0.0)
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: pytest (>=8.0.0,<9.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Project-URL: Documentation, https://github.com/OnDraganov/chromatic-tda
 Project-URL: Repository, https://github.com/OnDraganov/chromatic-tda
 Description-Content-Type: text/markdown
 
 # chromatic_tda
 
-`chromatic_tda` is a package for computing six-packs of persistent diagrams of colored point clouds. Currently point clouds in R^2 with 2 or 3 colors are supported (see Future).
+`chromatic_tda` is a package for computing six-packs of persistent diagrams of colored point clouds.
+Currently, point clouds in R^2 with 2 or 3 colors are supported (see Future; an alpha version with support for higher dimension is already available!).
 
 # Installation
 
 ## Install with `pip`
 
 The package is uploaded to [PyPI](https://pypi.org/project/chromatic-tda/), so it can be installed with `pip`.
 
@@ -49,27 +50,27 @@
 
 The basic use of the package is as follows:
 ```
 import chromatic_tda as chro
 points, labels = ... # load points, labels
 chro_alpha = chro.ChromaticAlphaComplex(points, labels) simplicial_complex = chro_alpha.get_simplicial_complex(
              sub_complex=‘bi-chromatic’
-             complex=‘all’
+             full_complex=‘all’
              relative=‘mono-chromatic’
 )  # these options make sense for three colors; for two use, e.g., just sub_complex='mono-chromatic'
-six_pack = simplicial_complex.bars_six_pack() chro.plot_six_pack(six_pack)
+six_pack = simplicial_complex.bars_six_pack()
+chro.plot_six_pack(six_pack)
 ```
 
 For more details check the docstrings of the methods and the jupyter notebook file `manual` (in [github repo](https://github.com/OnDraganov/chromatic-tda)). For more background on the theory, check the resources listed below.
 
 # Future
 
-The code is under active developement. The future plans include:
-- Adding support for points in R^3
-- Making persistence computation faster with clearing.
+The code is under active development. The future plans include:
+- Adding support for points in R^3 --> alpha version with a 3D support available in a separate branch: see https://github.com/OnDraganov/chromatic-tda/tree/general-radius-function
 
 # Resources
 
 The code is based on research done at Institute of Science and Technology by Ranita Biswas, Sebastiano Cultrera di Montesano, Ondřej Draganov, Herbert Edelsbrunner and Morteza Saghafian. A draft write up can be found on [arxiv](https://arxiv.org/abs/2212.03128).
 
 A presentation about the main concepts used in this package can be viewed on YouTube: [AATRN Online Seminar: TDA for Chromatic Point Clouds](https://youtu.be/HIqiF00yKaw). A recording of a complementary talk focusing more on the motivations of the work and the combinatorial structures underlying it is accessible through [google drive](https://drive.google.com/file/d/1RBiGlgY4mlRL59eAVmMLrgBCZYN97QnZ/view).
```

