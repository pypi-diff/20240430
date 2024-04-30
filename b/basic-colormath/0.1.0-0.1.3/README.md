# Comparing `tmp/basic_colormath-0.1.0.tar.gz` & `tmp/basic_colormath-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic_colormath-0.1.0.tar", max compression
+gzip compressed data, was "basic_colormath-0.1.3.tar", last modified: Tue Apr 30 17:10:28 2024, max compression
```

## Comparing `basic_colormath-0.1.0.tar` & `basic_colormath-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,36 @@
--rw-r--r--   0        0        0     1302 2023-05-01 17:10:26.221969 basic_colormath-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5733 2023-05-01 17:10:26.221969 basic_colormath-0.1.0/README.md
--rw-r--r--   0        0        0     1050 2023-05-01 17:10:26.221969 basic_colormath-0.1.0/src/basic_colormath/__init__.py
--rw-r--r--   0        0        0     6017 2023-05-01 17:10:26.221969 basic_colormath-0.1.0/src/basic_colormath/conversion.py
--rw-r--r--   0        0        0     7695 2023-05-01 17:10:26.221969 basic_colormath-0.1.0/src/basic_colormath/distance.py
--rw-r--r--   0        0        0     3942 2023-05-01 17:10:26.221969 basic_colormath-0.1.0/src/basic_colormath/mix.py
--rw-r--r--   0        0        0        0 2023-05-01 17:10:26.221969 basic_colormath-0.1.0/src/basic_colormath/py.typed
--rw-r--r--   0        0        0      735 2023-05-01 17:10:26.221969 basic_colormath-0.1.0/src/basic_colormath/type_hints.py
--rw-r--r--   0        0        0     6063 1970-01-01 00:00:00.000000 basic_colormath-0.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:10:28.798097 basic_colormath-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:10:28.794097 basic_colormath-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:10:28.794097 basic_colormath-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/.github/workflows/pypi-project.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/.vimrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/.vimspector.json
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-30 17:10:28.798097 basic_colormath-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/delta_e.vim
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 17:10:28.798097 basic_colormath-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:10:28.794097 basic_colormath-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:10:28.798097 basic_colormath-0.1.3/src/basic_colormath/
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/src/basic_colormath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/src/basic_colormath/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/src/basic_colormath/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/src/basic_colormath/mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/src/basic_colormath/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/src/basic_colormath/type_hints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:10:28.798097 basic_colormath-0.1.3/src/basic_colormath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-30 17:10:28.000000 basic_colormath-0.1.3/src/basic_colormath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-30 17:10:28.000000 basic_colormath-0.1.3/src/basic_colormath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 17:10:28.000000 basic_colormath-0.1.3/src/basic_colormath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 17:10:28.000000 basic_colormath-0.1.3/src/basic_colormath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 17:10:28.000000 basic_colormath-0.1.3/src/basic_colormath.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:10:28.798097 basic_colormath-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/tests/test_delta_e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-30 17:10:23.000000 basic_colormath-0.1.3/tests/test_mix.py
```

### Comparing `basic_colormath-0.1.0/README.md` & `basic_colormath-0.1.3/README.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-# basic_colormath
-
-Everything I wanted to salvage from the [python-colormath](https://github.com/gtaylor/python-colormath/tree/master) library ... with no numpy deps and 14x speed.
-
-* Perceptual (DeltaE CIE 2000) and Euclidean distance between colors
-* Conversion between RGB, HSV, HSL, and 8-bit hex colors
-* Simple, one-way conversion to Lab
-* Some convenience functions for RGB tuples and 8-bit hex color strings
-
-Lab and LCh color formats are exciting because they can cover a larger colorspace than RGB. But don't get *too* excited yet. If you convert an RGB tuple to Lab or LCh *with no additional information*, then the result will---of course---*not* contain more information than the RGB tuple you converted from. Other parameters are necessary to get anything out of these elaborate formats. I don't know how to do that, and most likely neither do you, so why not drop all of that complexity?
-
-I've installed [python-colormath](https://github.com/gtaylor/python-colormath/tree/master) on a lot of projects. The library does many interesting things, but most of what I wanted was perceptual color distance. This requires Lab colors, which have more parameters than an RGB tuple provides. Colormath didn't use those parameters, so the result didn't require the elaborate classes and methods provided by Colormath.
-
-The color distance I provide here is DeltaE CIE 2000. Aside from (presumably) some specialized applications, this is the best of the multiple color distances provided by [python-colormath](https://github.com/gtaylor/python-colormath/tree/master). Tuples in, float out, and with a lot more speed. It doesn't use all of those expert parameters, but neither did Colormath. This is the same result you'll get from any of the online DeltaE calculators you're likely to find.
-
-This library is more or less specialized for working with "upscaled" RGB tuples `([0, 255], [0, 255], [0, 255])`. Functions will take floats or ints in that range and return floats. If you want ints, use `float_tuple_to_8bit_int_tuple`. This is dramatically better int conversion than `int(float)` or `int(round(float))`, so use it insead of those.
-
-## distance functions
-
-    RGB = Annotated[tuple[float, float, float], ([0, 255], [0, 255], [0, 255])]
-    HSV = Annotated[tuple[float, float, float], ([0, 365), [0, 100], [0, 100])]
-    HSL = Annotated[tuple[float, float, float], ([0, 365), [0, 100], [0, 100])]
-    Lab = Annotated[tuple[float, float, float], ([0, 100], [-128, 127], [-128, 127])]
-    Hex = Annotated[str, "#000fff"]
-
-    rgb_to_lab(rgb: RGB) -> Lab:
-        # Converts RGB to Lab. To optionally cache for get_delta_e_lab
-
-    hex_to_lab(hex: Hex) -> Lab:
-        # Converts hex to Lab. To optionally cache for get_delta_e_lab
-
-    get_delta_e(rgb_a: RGB, rgb_b: RGB) -> float:
-        # Calculate the Delta E (CIE 2000) between two RGB colors.
-        # This is the one you'll usually want.
-
-    get_delta_e_hex(hex_a: Hex, hex_b: Hex) -> float:
-        # Calculate the Delta E (CIE 2000) between two hex colors.
-        # Takes and returns hex colorstrings.
-
-    get_delta_e_lab(lab_a: Lab, lab_b: Lab) -> float:
-        # Calculate the Delta E (CIE2000) of two Lab colors.
-        # To call with cached Lab values.
-
-    get_sqeuclidean(rgb_a: RGB, rgb_b: RGB) -> float:
-        # Calculate the squared Euclidean distance between two RGB colors.
-
-    get_sqeuclidean_hex(hex_a: Hex, hex_b: Hex) -> float:
-        # Calculate the squared Euclidean distance between two HEX colors.
-
-    get_euclidean(rgb_a: RGB, rgb_b: RGB) -> float:
-        # Calculate the Euclidean distance between two RGB colors.
-
-    get_euclidean_hex(hex_a: Hex, hex_b: Hex) -> float:
-        # Calculate the Euclidean distance between two HEX colors.
-
-## other conversions
-
-Converts to other simple formats.
-
-    rgb_to_hsv(rgb: RGB) -> HSV
-
-    hsv_to_rgb(hsv: HSV) -> RGB
-
-    rgb_to_hsl(rgb: RGB) -> HSL
-
-    hsl_to_rgb(hsl: HSL) -> RGB
-
-    rgb_to_hex(rgb: RGB) -> Hex
-
-    hex_to_rgb(hex_: Hex) -> RGB
-
-## convenience functions
-
-    _Ratio = float | tuple[float, ...] | None
-
-    scale_rgb(rgb: RGB, scalar: float) -> RGB:
-        # Scale an rgb tuple by a scalar.
-
-    mix_rgb(*rgb_args: RGB, ratio: _Ratio=None) -> RGB:
-        # Mix any number of rgb tuples.
-
-        :param rgb_args: rgb tuples ([0, 255], [0, 255], [0, 255])
-        :param ratio: 0.0 to 1.0 for the weight of the first rgb_arg or a tuple of floats
-            to distribute across rgb_args or None for equal ratios. Ratios will be
-            normalized and (if fewer ratios than colors are provided) the remaining
-            ratios will be equal.
-        :return: rgb tuple ([0, 255], [0, 255], [0, 255])
-
-    scale_hex(hex_: Hex, scalar: float)-> Hex
-
-    mix_hex(*hex_args: Hex, ratio: _Ratio=None) -> Hex
-
-## better float to int conversion
-
-    float_to_8bit_int(float_: float | int) -> int:
-
-    float_tuple_to_8bit_int_tuple(rgb: RGB) -> tuple[int, int, int]:
-
-
-## If you need more
-
-Sadly, [python-colormath](https://github.com/gtaylor/python-colormath/tree/master) has been abandoned, long enough now that a numpy function on which it relies has been not only deprecated but removed. If you still need to use [python-colormath](https://github.com/gtaylor/python-colormath/tree/master), patch `np.asscalar`:
-
-    import numpy as np
-    import numpy.typing as npt
-
-    def _patch_asscalar(a: npt.NDArray[np.float_]) -> float:
-        """Alias for np.item(). Patch np.asscalar for colormath.
-
-        :param a: numpy array
-        :return: input array as scalar
-        """
-        return a.item()
-
-    np.asscalar = _patch_asscalar  # type: ignore
+# basic_colormath
+
+Everything I wanted to salvage from the [python-colormath](https://github.com/gtaylor/python-colormath/tree/master) library ... with no numpy deps and 14x speed.
+
+* Perceptual (DeltaE CIE 2000) and Euclidean distance between colors
+* Conversion between RGB, HSV, HSL, and 8-bit hex colors
+* Simple, one-way conversion to Lab
+* Some convenience functions for RGB tuples and 8-bit hex color strings
+
+Lab and LCh color formats are exciting because they can cover a larger colorspace than RGB. But don't get *too* excited yet. If you convert an RGB tuple to Lab or LCh *with no additional information*, then the result will---of course---*not* contain more information than the RGB tuple you converted from. Other parameters are necessary to get anything out of these elaborate formats. I don't know how to do that, and most likely neither do you, so why not drop all of that complexity?
+
+I've installed [python-colormath](https://github.com/gtaylor/python-colormath/tree/master) on a lot of projects. The library does many interesting things, but most of what I wanted was perceptual color distance. This requires Lab colors, which have more parameters than an RGB tuple provides. Colormath didn't use those parameters, so the result didn't require the elaborate classes and methods provided by Colormath.
+
+The color distance I provide here is DeltaE CIE 2000. Aside from (presumably) some specialized applications, this is the best of the multiple color distances provided by [python-colormath](https://github.com/gtaylor/python-colormath/tree/master). Tuples in, float out, and with a lot more speed. It doesn't use all of those expert parameters, but neither did Colormath. This is the same result you'll get from any of the online DeltaE calculators you're likely to find.
+
+This library is more or less specialized for working with "upscaled" RGB tuples `([0, 255], [0, 255], [0, 255])`. Functions will take floats or ints in that range and return floats. If you want ints, use `float_tuple_to_8bit_int_tuple`. This is dramatically better int conversion than `int(float)` or `int(round(float))`, so use it insead of those.
+
+## distance functions
+
+    RGB = Annotated[tuple[float, float, float], ([0, 255], [0, 255], [0, 255])]
+    HSV = Annotated[tuple[float, float, float], ([0, 365), [0, 100], [0, 100])]
+    HSL = Annotated[tuple[float, float, float], ([0, 365), [0, 100], [0, 100])]
+    Lab = Annotated[tuple[float, float, float], ([0, 100], [-128, 127], [-128, 127])]
+    Hex = Annotated[str, "#000fff"]
+
+    rgb_to_lab(rgb: RGB) -> Lab:
+        # Converts RGB to Lab. To optionally cache for get_delta_e_lab
+
+    hex_to_lab(hex: Hex) -> Lab:
+        # Converts hex to Lab. To optionally cache for get_delta_e_lab
+
+    get_delta_e(rgb_a: RGB, rgb_b: RGB) -> float:
+        # Calculate the Delta E (CIE 2000) between two RGB colors.
+        # This is the one you'll usually want.
+
+    get_delta_e_hex(hex_a: Hex, hex_b: Hex) -> float:
+        # Calculate the Delta E (CIE 2000) between two hex colors.
+        # Takes and returns hex colorstrings.
+
+    get_delta_e_lab(lab_a: Lab, lab_b: Lab) -> float:
+        # Calculate the Delta E (CIE2000) of two Lab colors.
+        # To call with cached Lab values.
+
+    get_sqeuclidean(rgb_a: RGB, rgb_b: RGB) -> float:
+        # Calculate the squared Euclidean distance between two RGB colors.
+
+    get_sqeuclidean_hex(hex_a: Hex, hex_b: Hex) -> float:
+        # Calculate the squared Euclidean distance between two HEX colors.
+
+    get_euclidean(rgb_a: RGB, rgb_b: RGB) -> float:
+        # Calculate the Euclidean distance between two RGB colors.
+
+    get_euclidean_hex(hex_a: Hex, hex_b: Hex) -> float:
+        # Calculate the Euclidean distance between two HEX colors.
+
+## other conversions
+
+Converts to other simple formats.
+
+    rgb_to_hsv(rgb: RGB) -> HSV
+
+    hsv_to_rgb(hsv: HSV) -> RGB
+
+    rgb_to_hsl(rgb: RGB) -> HSL
+
+    hsl_to_rgb(hsl: HSL) -> RGB
+
+    rgb_to_hex(rgb: RGB) -> Hex
+
+    hex_to_rgb(hex_: Hex) -> RGB
+
+## convenience functions
+
+    _Ratio = float | tuple[float, ...] | None
+
+    scale_rgb(rgb: RGB, scalar: float) -> RGB:
+        # Scale an rgb tuple by a scalar.
+
+    mix_rgb(*rgb_args: RGB, ratio: _Ratio=None) -> RGB:
+        # Mix any number of rgb tuples.
+
+        :param rgb_args: rgb tuples ([0, 255], [0, 255], [0, 255])
+        :param ratio: 0.0 to 1.0 for the weight of the first rgb_arg or a tuple of floats
+            to distribute across rgb_args or None for equal ratios. Ratios will be
+            normalized and (if fewer ratios than colors are provided) the remaining
+            ratios will be equal.
+        :return: rgb tuple ([0, 255], [0, 255], [0, 255])
+
+    scale_hex(hex_: Hex, scalar: float)-> Hex
+
+    mix_hex(*hex_args: Hex, ratio: _Ratio=None) -> Hex
+
+## better float to int conversion
+
+    float_to_8bit_int(float_: float | int) -> int:
+
+    float_tuple_to_8bit_int_tuple(rgb: RGB) -> tuple[int, int, int]:
+
+
+## If you need more
+
+Sadly, [python-colormath](https://github.com/gtaylor/python-colormath/tree/master) has been abandoned, long enough now that a numpy function on which it relies has been not only deprecated but removed. If you still need to use [python-colormath](https://github.com/gtaylor/python-colormath/tree/master), patch `np.asscalar`:
+
+    import numpy as np
+    import numpy.typing as npt
+
+    def _patch_asscalar(a: npt.NDArray[np.float_]) -> float:
+        """Alias for np.item(). Patch np.asscalar for colormath.
+
+        :param a: numpy array
+        :return: input array as scalar
+        """
+        return a.item()
+
+    np.asscalar = _patch_asscalar  # type: ignore
```

### Comparing `basic_colormath-0.1.0/src/basic_colormath/__init__.py` & `basic_colormath-0.1.3/src/basic_colormath/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-"""Raise public functions into the package namespace.
-
-:author: Shay Hill
-:created: 2023-04-30
-"""
-
-from basic_colormath.conversion import (
-    float_to_8bit_int,
-    float_tuple_to_8bit_int_tuple,
-    hex_to_rgb,
-    hsl_to_rgb,
-    hsv_to_rgb,
-    rgb_to_hex,
-    rgb_to_hsl,
-    rgb_to_hsv,
-)
-from basic_colormath.distance import (
-    get_delta_e,
-    get_delta_e_hex,
-    get_delta_e_lab,
-    get_euclidean,
-    get_euclidean_hex,
-    get_sqeuclidean,
-    get_sqeuclidean_hex,
-    rgb_to_lab,
-)
-from basic_colormath.mix import mix_hex, mix_rgb, scale_hex, scale_rgb
-
-__all__ = [
-    "float_to_8bit_int",
-    "float_tuple_to_8bit_int_tuple",
-    "get_delta_e",
-    "get_delta_e_hex",
-    "get_delta_e_lab",
-    "get_euclidean",
-    "get_euclidean_hex",
-    "get_sqeuclidean",
-    "get_sqeuclidean_hex",
-    "hex_to_rgb",
-    "hsl_to_rgb",
-    "hsv_to_rgb",
-    "mix_hex",
-    "mix_rgb",
-    "rgb_to_hex",
-    "rgb_to_hsl",
-    "rgb_to_hsv",
-    "rgb_to_lab",
-    "scale_hex",
-    "scale_rgb",
-]
+"""Raise public functions into the package namespace.
+
+:author: Shay Hill
+:created: 2023-04-30
+"""
+
+from basic_colormath.conversion import (
+    float_to_8bit_int,
+    float_tuple_to_8bit_int_tuple,
+    hex_to_rgb,
+    hsl_to_rgb,
+    hsv_to_rgb,
+    rgb_to_hex,
+    rgb_to_hsl,
+    rgb_to_hsv,
+)
+from basic_colormath.distance import (
+    get_delta_e,
+    get_delta_e_hex,
+    get_delta_e_lab,
+    get_euclidean,
+    get_euclidean_hex,
+    get_sqeuclidean,
+    get_sqeuclidean_hex,
+    rgb_to_lab,
+)
+from basic_colormath.mix import mix_hex, mix_rgb, scale_hex, scale_rgb
+
+__all__ = [
+    "float_to_8bit_int",
+    "float_tuple_to_8bit_int_tuple",
+    "get_delta_e",
+    "get_delta_e_hex",
+    "get_delta_e_lab",
+    "get_euclidean",
+    "get_euclidean_hex",
+    "get_sqeuclidean",
+    "get_sqeuclidean_hex",
+    "hex_to_rgb",
+    "hsl_to_rgb",
+    "hsv_to_rgb",
+    "mix_hex",
+    "mix_rgb",
+    "rgb_to_hex",
+    "rgb_to_hsl",
+    "rgb_to_hsv",
+    "rgb_to_lab",
+    "scale_hex",
+    "scale_rgb",
+]
```

### Comparing `basic_colormath-0.1.0/src/basic_colormath/conversion.py` & `basic_colormath-0.1.3/src/basic_colormath/conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,177 +1,179 @@
-"""Convert between (upscaled) RGB, HSL, HSV, and HEX.
-
-These are the straightforward conversions. This library also converts to Lab
-(niavely, there are parameters that are not taken into account), but only for finding
-CIEDE2000 color differences.
-
-That conversion is in the distance.py module.
-
-:author: Shay Hill
-:created: 2023-04-30
-"""
-
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from basic_colormath.type_hints import HSL, HSV, RGB, Hex
-
-
-def _get_hue_from_rgb(rgb: RGB, min_: float, max_: float) -> float:
-    """Get the hue value in degrees from an rgb tuple.
-
-    :param rgb: A tuple of red, green, and blue values, ([0, 255], [0, 255], [0, 255]).
-    :param min_: The minimum value in the rgb tuple.
-    :param max_: The maximum value in the rgb tuple.
-    :return: The hue value in degrees, [0, 360).
-    """
-    red, grn, blu = rgb
-    if max_ == min_:
-        return 0
-    if max_ == red:
-        return (60 * ((grn - blu) / (max_ - min_)) + 360) % 360
-    if max_ == grn:
-        return 60 * ((blu - red) / (max_ - min_)) + 120
-    return 60 * ((red - grn) / (max_ - min_)) + 240
-
-
-def _sort_channels_given_hue(hue: float, min_mid_max: RGB) -> RGB:
-    """Sort the channels of an rgb tuple given a hue value.
-
-    :param hue: The hue value in degrees, [0, 360).
-    :param min_mid_max: A tuple of the minimum, middle, and maximum values in the rgb
-    :return: an arrangement of min_mid_max that corresponds to the hue.
-
-    Regardless of saturation, lightness, value, etc., the order of minimum, middle,
-    and maximum values in an rgb tuple will be consistent. For instance, given a hue
-    of 0, the red channel will always be the highest value.
-    """
-    hue %= 360
-    sextant2order = {
-        0: (2, 1, 0),
-        1: (1, 2, 0),
-        2: (0, 2, 1),
-        3: (0, 1, 2),
-        4: (1, 0, 2),
-        5: (2, 0, 1),
-    }
-    red, grn, blu = (min_mid_max[i] for i in sextant2order[int(hue // 60)])
-    return red, grn, blu
-
-
-def rgb_to_hsv(rgb: RGB) -> HSV:
-    """Convert from rgb to hsv.
-
-    :param rgb: a tuple of red, green, and blue values ([0, 255], [0, 255], [0, 255]).
-    :return: a tuple of hue, saturation, and value ([0, 360), [0, 100], [0, 100]).
-    """
-    min_ = min(rgb)
-    max_ = max(rgb)
-    hue = _get_hue_from_rgb(rgb, min_, max_)
-    sat = 0 if max_ == 0 else (1 - (min_ / max_)) * 100
-    val = max_ / 2.55
-    return hue, sat, val
-
-
-def hsv_to_rgb(hsv: HSV) -> RGB:
-    """Convert from hsv to rgb.
-
-    :param hsv: a tuple of hue, saturation, and value ([0, 360], [0, 100], [0, 100]).
-    :return: a tuple of red, green, and blue values ([0, 255], [0, 255], [0, 255]).
-    """
-    hue, sat, val = hsv
-    scaled_val = val * 2.55
-    if sat == 0 or val == 0:
-        return scaled_val, scaled_val, scaled_val
-    max_ = scaled_val
-    min_ = max_ - (sat / 100 * max_)
-    hue_mid_ratio = 1 - abs((hue / 60) % 2 - 1)
-    mid = hue_mid_ratio * (max_ - min_) + min_
-    return _sort_channels_given_hue(hue, (min_, mid, max_))
-
-
-def rgb_to_hsl(rgb: RGB) -> HSL:
-    """Convert rgb to hsl.
-
-    :param rgb: a tuple of red, green, and blue values ([0, 255], [0, 255], [0, 255]).
-    :return: a tuple of hue, saturation, and lightness ([0, 360), [0, 100], [0, 100]).
-    """
-    var_min = min(rgb)
-    var_max = max(rgb)
-    hue = _get_hue_from_rgb(rgb, var_min, var_max)
-    lig = var_max + var_min
-
-    if var_max == var_min:
-        sat = 0.0
-    elif lig <= 255:
-        sat = (var_max - var_min) / (0.01 * lig)
-    else:
-        sat = (var_max - var_min) / (5.1 - (0.01 * lig))
-    return hue, sat, lig / 5.1
-
-
-def hsl_to_rgb(hsl: HSL) -> RGB:
-    """Convert hsl to rgb.
-
-    :param hsl: a tuple of hue, sat, and lightness ([0, 360], [0, 100], [0, 100]).
-    :return: a tuple of red, green, and blue values ([0, 255], [0, 255], [0, 255]).
-    """
-    hue, sat, lig = hsl
-    max_p = (100 - abs(2 * lig - 100)) * sat * 0.0255
-    mid_p = max_p * (1 - abs((hue / 60) % 2 - 1))
-    min_ = (lig - max_p / 5.1) * 2.55
-    return _sort_channels_given_hue(hue, (min_, mid_p + min_, max_p + min_))
-
-
-_BIG_INT = 2**32 - 1
-
-
-def float_to_8bit_int(float_: float | int) -> int:
-    """Convert a float between 0 and 255 to an int between 0 and 255.
-
-    :param float_: a float in the closed interval [0 .. 255]
-    :return: an interval in the closed interval [0 .. 255]
-    :raise ValueError: if float_ is not in the closed interval [0 .. 255]
-
-    Convert color floats [0 .. 255] to ints [0 .. 255] without rounding, which "short
-    changes" 0 and 255.
-    """
-    if not 0 <= float_ <= 255:
-        msg = f"float argument must be in [0 .. 255], not `{float_}`"
-        raise ValueError(msg)
-    if isinstance(float_, int):
-        return float_
-    high_int = int(float_ / 255 * _BIG_INT)
-    return high_int >> 24
-
-
-def float_tuple_to_8bit_int_tuple(rgb: RGB) -> tuple[int, int, int]:
-    """Convert an rgb float tuple to an rgb int tuple.
-
-    :param rgb: a tuple of floats in the closed interval [0 .. 255]
-    :return: a tuple of ints in the closed interval [0 .. 255]
-    """
-    red, grn, blu = (float_to_8bit_int(c) for c in rgb)
-    return red, grn, blu
-
-
-def rgb_to_hex(rgb: RGB) -> Hex:
-    """Convert rgb to hex.
-
-    :param rgb: a tuple of red, green, and blue values ([0, 255], [0, 255], [0, 255]).
-    :return: a hex string representation of the rgb value.
-    """
-    red, grn, blu = (float_to_8bit_int(c) for c in rgb)
-    return f"#{red:02x}{grn:02x}{blu:02x}"
-
-
-def hex_to_rgb(hex_: Hex) -> tuple[int, int, int]:
-    """Convert hex to rgb.
-
-    :param hex_: a hex string representation of an rgb value. With or w/o leading #.
-    :return: a tuple of red, green, and blue ints ([0, 255], [0, 255], [0, 255]).
-    """
-    hex_ = hex_.lstrip("#")
-    red, grn, blu = (int(hex_[i : i + 2], 16) for i in (0, 2, 4))
-    return (red, grn, blu)
+"""Convert between (upscaled) RGB, HSL, HSV, and HEX.
+
+These are the straightforward conversions. This library also converts to Lab
+(niavely, there are parameters that are not taken into account), but only for finding
+CIEDE2000 color differences.
+
+That conversion is in the distance.py module.
+
+:author: Shay Hill
+:created: 2023-04-30
+"""
+
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+_MAX_8BIT = 255
+
+if TYPE_CHECKING:
+    from basic_colormath.type_hints import HSL, HSV, RGB, Hex
+
+
+def _get_hue_from_rgb(rgb: RGB, min_: float, max_: float) -> float:
+    """Get the hue value in degrees from an rgb tuple.
+
+    :param rgb: A tuple of red, green, and blue values, ([0, 255], [0, 255], [0, 255]).
+    :param min_: The minimum value in the rgb tuple.
+    :param max_: The maximum value in the rgb tuple.
+    :return: The hue value in degrees, [0, 360).
+    """
+    red, grn, blu = rgb
+    if max_ == min_:
+        return 0
+    if max_ == red:
+        return (60 * ((grn - blu) / (max_ - min_)) + 360) % 360
+    if max_ == grn:
+        return 60 * ((blu - red) / (max_ - min_)) + 120
+    return 60 * ((red - grn) / (max_ - min_)) + 240
+
+
+def _sort_channels_given_hue(hue: float, min_mid_max: RGB) -> RGB:
+    """Sort the channels of an rgb tuple given a hue value.
+
+    :param hue: The hue value in degrees, [0, 360).
+    :param min_mid_max: A tuple of the minimum, middle, and maximum values in the rgb
+    :return: an arrangement of min_mid_max that corresponds to the hue.
+
+    Regardless of saturation, lightness, value, etc., the order of minimum, middle,
+    and maximum values in an rgb tuple will be consistent. For instance, given a hue
+    of 0, the red channel will always be the highest value.
+    """
+    hue %= 360
+    sextant2order = {
+        0: (2, 1, 0),
+        1: (1, 2, 0),
+        2: (0, 2, 1),
+        3: (0, 1, 2),
+        4: (1, 0, 2),
+        5: (2, 0, 1),
+    }
+    red, grn, blu = (min_mid_max[i] for i in sextant2order[int(hue // 60)])
+    return red, grn, blu
+
+
+def rgb_to_hsv(rgb: RGB) -> HSV:
+    """Convert from rgb to hsv.
+
+    :param rgb: a tuple of red, green, and blue values ([0, 255], [0, 255], [0, 255]).
+    :return: a tuple of hue, saturation, and value ([0, 360), [0, 100], [0, 100]).
+    """
+    min_ = min(rgb)
+    max_ = max(rgb)
+    hue = _get_hue_from_rgb(rgb, min_, max_)
+    sat = 0 if max_ == 0 else (1 - (min_ / max_)) * 100
+    val = max_ / 2.55
+    return hue, sat, val
+
+
+def hsv_to_rgb(hsv: HSV) -> RGB:
+    """Convert from hsv to rgb.
+
+    :param hsv: a tuple of hue, saturation, and value ([0, 360], [0, 100], [0, 100]).
+    :return: a tuple of red, green, and blue values ([0, 255], [0, 255], [0, 255]).
+    """
+    hue, sat, val = hsv
+    scaled_val = val * 2.55
+    if sat == 0 or val == 0:
+        return scaled_val, scaled_val, scaled_val
+    max_ = scaled_val
+    min_ = max_ - (sat / 100 * max_)
+    hue_mid_ratio = 1 - abs((hue / 60) % 2 - 1)
+    mid = hue_mid_ratio * (max_ - min_) + min_
+    return _sort_channels_given_hue(hue, (min_, mid, max_))
+
+
+def rgb_to_hsl(rgb: RGB) -> HSL:
+    """Convert rgb to hsl.
+
+    :param rgb: a tuple of red, green, and blue values ([0, 255], [0, 255], [0, 255]).
+    :return: a tuple of hue, saturation, and lightness ([0, 360), [0, 100], [0, 100]).
+    """
+    var_min = min(rgb)
+    var_max = max(rgb)
+    hue = _get_hue_from_rgb(rgb, var_min, var_max)
+    lig = var_max + var_min
+
+    if var_max == var_min:
+        sat = 0.0
+    elif lig <= _MAX_8BIT:
+        sat = (var_max - var_min) / (0.01 * lig)
+    else:
+        sat = (var_max - var_min) / (5.1 - (0.01 * lig))
+    return hue, sat, lig / 5.1
+
+
+def hsl_to_rgb(hsl: HSL) -> RGB:
+    """Convert hsl to rgb.
+
+    :param hsl: a tuple of hue, sat, and lightness ([0, 360], [0, 100], [0, 100]).
+    :return: a tuple of red, green, and blue values ([0, 255], [0, 255], [0, 255]).
+    """
+    hue, sat, lig = hsl
+    max_p = (100 - abs(2 * lig - 100)) * sat * 0.0255
+    mid_p = max_p * (1 - abs((hue / 60) % 2 - 1))
+    min_ = (lig - max_p / 5.1) * 2.55
+    return _sort_channels_given_hue(hue, (min_, mid_p + min_, max_p + min_))
+
+
+_BIG_INT = 2**32 - 1
+
+
+def float_to_8bit_int(float_: float) -> int:
+    """Convert a float between 0 and 255 to an int between 0 and 255.
+
+    :param float_: a float in the closed interval [0 .. 255]
+    :return: an interval in the closed interval [0 .. 255]
+    :raise ValueError: if float_ is not in the closed interval [0 .. 255]
+
+    Convert color floats [0 .. 255] to ints [0 .. 255] without rounding, which "short
+    changes" 0 and 255.
+    """
+    if not 0 <= float_ <= _MAX_8BIT:
+        msg = f"float argument must be in [0 .. 255], not `{float_}`"
+        raise ValueError(msg)
+    if isinstance(float_, int):
+        return float_
+    high_int = int(float_ / _MAX_8BIT * _BIG_INT)
+    return high_int >> 24
+
+
+def float_tuple_to_8bit_int_tuple(rgb: RGB) -> tuple[int, int, int]:
+    """Convert an rgb float tuple to an rgb int tuple.
+
+    :param rgb: a tuple of floats in the closed interval [0 .. 255]
+    :return: a tuple of ints in the closed interval [0 .. 255]
+    """
+    red, grn, blu = (float_to_8bit_int(c) for c in rgb)
+    return red, grn, blu
+
+
+def rgb_to_hex(rgb: RGB) -> Hex:
+    """Convert rgb to hex.
+
+    :param rgb: a tuple of red, green, and blue values ([0, 255], [0, 255], [0, 255]).
+    :return: a hex string representation of the rgb value.
+    """
+    red, grn, blu = (float_to_8bit_int(c) for c in rgb)
+    return f"#{red:02x}{grn:02x}{blu:02x}"
+
+
+def hex_to_rgb(hex_: Hex) -> tuple[int, int, int]:
+    """Convert hex to rgb.
+
+    :param hex_: a hex string representation of an rgb value. With or w/o leading #.
+    :return: a tuple of red, green, and blue ints ([0, 255], [0, 255], [0, 255]).
+    """
+    hex_ = hex_.lstrip("#")
+    red, grn, blu = (int(hex_[i : i + 2], 16) for i in (0, 2, 4))
+    return (red, grn, blu)
```

### Comparing `basic_colormath-0.1.0/src/basic_colormath/distance.py` & `basic_colormath-0.1.3/src/basic_colormath/distance.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,255 +1,275 @@
-"""Get the delta_e cielab 2000 distance between two color tuples.
-
-Three DeltaE CIE 2000 distance functions are provided:
-
-get_delta_e  ->  get DeltaE CIE 2000 distance between two rgb tuples [0-255]
-get_delta_e_hex  ->  get DeltaE CIE 2000 distance between two hex strings
-get_delta_e_lab  ->  get DeltaE CIE 2000 distance between cached `_to_lab` calls
-
-I've also provided squared Euclidean and Euclidean distance between rgb tuples or hex
-strings.
-
-get_sqeuclidean
-get_sqeuclidean_hex
-get_euclidean
-get_euclidean_hex
-
-
-`get_delta_e` is the function you'll usually want, but `get_delta_e_lab` will be a
-bit faster if you want to cache the results of `rgb_to_lab` or `hex_to_lab` yourself.
-
-Most of the math can be found here:
-http://www.brucelindbloom.com/index.html?Eqn_DeltaE_CIE2000.html
-
-I've tried to preserve Bruce Lindbloom's naming conventions so you can follow along.
-
-:author: Shay Hill
-:created: 2023-04-29
-"""
-from __future__ import annotations
-
-import math
-from typing import TYPE_CHECKING, Tuple
-
-from basic_colormath.conversion import hex_to_rgb
-
-if TYPE_CHECKING:
-    from basic_colormath.type_hints import RGB, Hex, Lab
-
-_Triple = Tuple[float, float, float]
-
-_RGB_TO_XYZ = [
-    [0.412424, 0.357579, 0.180464],
-    [0.212656, 0.715158, 0.0721856],
-    [0.0193324, 0.119193, 0.950444],
-]
-
-
-def _rgb_to_xyz(rgb: RGB) -> _Triple:
-    """RGB to XYZ conversion. Expects RGB values between 0 and 255.
-
-    :param rgb: RGB values between 0 and 255 inclusive.
-    :return: XYZ values between 0 and 1 inclusive.
-
-    The standard rgb to xyz conversion scaled for [0, 255] color values.
-    """
-    lin: list[float] = []
-    for channel in rgb:
-        if channel <= 10.31475:
-            lin.append(channel / 3294.6)
-        else:
-            lin.append(((channel + 14.025) / 269.025) ** 2.4)
-
-    result_matrix = [sum(x * y for x, y in zip(row, lin)) for row in _RGB_TO_XYZ]
-    rgb_r, rgb_g, rgb_b = (max(c, 0) for c in result_matrix)
-    return rgb_r, rgb_g, rgb_b
-
-
-_CIE_E = 216 / 24389
-_1_3RD = 1 / 3
-_16_116THS = 16 / 116
-
-# this will always be the illuminant when rgb is converted to xyz from an without
-# an illuminant argument
-_XYZ_ILLUM = (0.95047, 1.0, 1.08883)
-
-
-def _xyz_to_lab(xyz: _Triple) -> Lab:
-    """Convert XYZ to Lab.
-
-    :param xyz: XYZ color tuple
-    :return: Lab color tuple
-    """
-    # this will always be the illuminant when rgb is converted to xyz from an without
-    # an illuminant argument
-    scaled_xyz = [c / y for c, y in zip(xyz, _XYZ_ILLUM)]
-    for i, channel in enumerate(scaled_xyz):
-        if channel > _CIE_E:
-            scaled_xyz[i] = channel**_1_3RD
-        else:
-            scaled_xyz[i] = (7.787 * channel) + _16_116THS
-
-    x, y, z = scaled_xyz
-    lab_l = (116 * y) - 16.0
-    lab_a = 500 * (x - y)
-    lab_b = 200 * (y - z)
-    return lab_l, lab_a, lab_b
-
-
-_RAD_6 = math.radians(6)
-_RAD_25 = math.radians(25)
-_RAD_30 = math.radians(30)
-_RAD_63 = math.radians(63)
-_RAD_180 = math.radians(180)
-_RAD_275 = math.radians(275)
-_RAD_360 = math.radians(360)
-_RAD_720 = math.radians(720)
-_V25_E7 = 25**7
-
-
-def rgb_to_lab(rgb: RGB) -> Lab:
-    """Convert RGB to Lab.
-
-    :param rgb: The RGB color to convert.
-    :return: The Lab color.
-    """
-    xyz = _rgb_to_xyz(rgb)
-    return _xyz_to_lab(xyz)
-
-
-def hex_to_lab(hex_: Hex) -> Lab:
-    """Convert hex color to Lab.
-
-    :param hex_: The hex color to convert.
-    :return: The Lab color.
-    """
-    rgb = hex_to_rgb(hex_)
-    return rgb_to_lab(rgb)
-
-
-def get_delta_e_lab(lab_a: Lab, lab_b: Lab) -> float:
-    """Calculate the Delta E (CIE2000) of two Lab colors.
-
-    :param lab_a: The first Lab color.
-    :param lab_b: The second Lab color.
-    :return: The Delta E (CIE2000) of the two colors.
-    """
-    lab_a_bsq = lab_a[2] ** 2
-    lab_b_bsq = lab_b[2] ** 2
-
-    Lp = (lab_a[0] + lab_b[0]) / 2.0
-
-    C1 = (lab_a[1] ** 2 + lab_a_bsq) ** 0.5
-    C2 = (lab_b[1] ** 2 + lab_b_bsq) ** 0.5
-    avg_c_e7 = ((C1 + C2) / 2.0) ** 7
-    G = 0.5 * (1 - (avg_c_e7 / (avg_c_e7 + _V25_E7)) ** 0.5) + 1
-
-    a1p, a2p = (lab[1] * G for lab in (lab_a, lab_b))
-
-    C1p = (a1p**2 + lab_a_bsq) ** 0.5
-    C2p = (a2p**2 + lab_b_bsq) ** 0.5
-    Cp = (C1p + C2p) / 2.0
-
-    h1p = math.atan2(lab_a[2], a1p)
-    h1p = h1p if h1p >= 0 else h1p + _RAD_360
-    h2p = math.atan2(lab_b[2], a2p)
-    h2p = h2p if h2p >= 0 else h2p + _RAD_360
-    Hp = (h1p + h2p) / 2
-    Hp = Hp if abs(h1p - h2p) <= _RAD_180 else Hp + _RAD_180
-
-    T = (
-        1
-        - 0.17 * math.cos(Hp - _RAD_30)
-        + 0.24 * math.cos(2 * Hp)
-        + 0.32 * math.cos(3 * Hp + _RAD_6)
-        - 0.2 * math.cos(4 * Hp - _RAD_63)
-    )
-
-    delta_hp = h2p - h1p
-    if abs(delta_hp) > _RAD_180:
-        if h2p > h1p:
-            delta_hp -= _RAD_360
-        else:
-            delta_hp += _RAD_360
-
-    delta_Lp = lab_b[0] - lab_a[0]
-    delta_Cp = C2p - C1p
-    delta_Hp = 2 * (C2p * C1p) ** 0.5 * math.sin(delta_hp / 2)
-
-    lp_minus_50_sq = (Lp - 50) ** 2
-    S_L = 1 + (0.015 * lp_minus_50_sq) / (20 + lp_minus_50_sq) ** 0.5
-    S_C = 1 + 0.045 * Cp
-    S_H = 1 + 0.015 * Cp * T
-
-    delta_ro = _RAD_30 * math.exp(-(((Hp - _RAD_275) / _RAD_25) ** 2))
-
-    avg_cp_e7 = Cp**7
-    R_C = (avg_cp_e7 / (avg_cp_e7 + _V25_E7)) ** 0.5
-    R_T = -2 * R_C * math.sin(2 * delta_ro)
-
-    return (
-        (delta_Lp / S_L) ** 2
-        + (delta_Cp / S_C) ** 2
-        + (delta_Hp / S_H) ** 2
-        + R_T * delta_Cp / S_C * delta_Hp / S_H
-    ) ** 0.5
-
-
-def get_sqeuclidean(rgb_a: RGB, rgb_b: RGB) -> float:
-    """Calculate the squared Euclidean distance between two RGB colors.
-
-    :param rgb_a: The first RGB color.
-    :param rgb_b: The second RGB color.
-    :return: The squared Euclidean distance between the two RGB colors.
-    """
-    return sum((a - b) ** 2 for a, b in zip(rgb_a, rgb_b))
-
-
-def get_sqeuclidean_hex(hex_a: Hex, hex_b: Hex) -> float:
-    """Calculate the squared Euclidean distance between two HEX colors.
-
-    :param hex_a: The first HEX color.
-    :param hex_b: The second HEX color.
-    :return: The squared Euclidean distance between the two HEX colors.
-    """
-    return get_sqeuclidean(hex_to_rgb(hex_a), hex_to_rgb(hex_b))
-
-
-def get_euclidean(rgb_a: RGB, rgb_b: RGB) -> float:
-    """Calculate the Euclidean distance between two RGB colors.
-
-    :param rgb_a: The first RGB color.
-    :param rgb_b: The second RGB color.
-    :return: The Euclidean distance between the two RGB colors.
-    """
-    return get_sqeuclidean(rgb_a, rgb_b) ** 0.5
-
-
-def get_euclidean_hex(hex_a: Hex, hex_b: Hex) -> float:
-    """Calculate the Euclidean distance between two HEX colors.
-
-    :param hex_a: The first HEX color.
-    :param hex_b: The second HEX color.
-    :return: The Euclidean distance between the two HEX colors.
-    """
-    return get_euclidean(hex_to_rgb(hex_a), hex_to_rgb(hex_b))
-
-
-def get_delta_e(rgb_a: RGB, rgb_b: RGB) -> float:
-    """Calculate the Delta E (CIE 2000) between two RGB colors.
-
-    :param rgb_a: The first RGB color.
-    :param rgb_b: The second RGB color.
-    :return: The Delta E (CIE 2000) between the two RGB colors.
-    """
-    return get_delta_e_lab(rgb_to_lab(rgb_a), rgb_to_lab(rgb_b))
-
-
-def get_delta_e_hex(hex_a: Hex, hex_b: Hex) -> float:
-    """Calculate the Delta E (CIE 2000) between two hex colors.
-
-    :param hex_a: The first hex color.
-    :param hex_b: The second hex color.
-    :return: The Delta E (CIE 2000) between the two hex colors.
-    """
-    return get_delta_e_lab(hex_to_lab(hex_a), hex_to_lab(hex_b))
+"""Get the delta_e cielab 2000 distance between two color tuples.
+
+Three DeltaE CIE 2000 distance functions are provided:
+
+get_delta_e  ->  get DeltaE CIE 2000 distance between two rgb tuples [0-255]
+get_delta_e_hex  ->  get DeltaE CIE 2000 distance between two hex strings
+get_delta_e_lab  ->  get DeltaE CIE 2000 distance between cached `_to_lab` calls
+
+I've also provided squared Euclidean and Euclidean distance between rgb tuples or hex
+strings.
+
+get_sqeuclidean
+get_sqeuclidean_hex
+get_euclidean
+get_euclidean_hex
+
+
+`get_delta_e` is the function you'll usually want, but `get_delta_e_lab` will be a
+bit faster if you want to cache the results of `rgb_to_lab` or `hex_to_lab` yourself.
+
+Most of the math can be found here:
+http://www.brucelindbloom.com/index.html?Eqn_DeltaE_CIE2000.html
+
+I've tried to preserve Bruce Lindbloom's naming conventions so you can follow along.
+
+Intermediate color formats are 3-tuples with the following ranges:
+
+    * RGB [0..255], [0..255], [0.255]
+    * XYZ [0.0, 1.0286], [0.0, 1.0822], [0.0, 1.178]
+    * Lab [0.0, 100], [-86.183, 98.235], [-107.865, 94.477]
+
+:author: Shay Hill
+:created: 2023-04-29
+"""
+
+from __future__ import annotations
+
+import math
+from typing import TYPE_CHECKING, Tuple
+
+from basic_colormath.conversion import hex_to_rgb
+
+if TYPE_CHECKING:
+    from basic_colormath.type_hints import RGB, Hex, Lab
+
+_Triple = Tuple[float, float, float]
+
+_RGB_TO_XYZ = [
+    [0.412424, 0.357579, 0.180464],
+    [0.212656, 0.715158, 0.0721856],
+    [0.0193324, 0.119193, 0.950444],
+]
+
+
+# constants to "linearize" rgb values
+_XYZ_NORMALIZATION_THRESHOLD = 10.31475
+_XYZ_SML_VAL_DENOMINATOR = 3294.6
+_XYZ_LRG_VAL_OFFSET = 14.025
+_XYZ_LRG_VAL_DENOMINATOR = 269.025
+_XYZ_LRG_VAL_EXPONENT = 2.4
+
+
+def _rgb_to_xyz(rgb: RGB) -> _Triple:
+    """RGB to XYZ conversion. Expects RGB values between 0 and 255.
+
+    :param rgb: RGB values between 0 and 255 inclusive.
+    :return: XYZ values between 0 and 1 inclusive.
+
+    The standard rgb to xyz conversion scaled for [0, 255] color values.
+    """
+    linear_channels: list[float] = []
+    for channel in rgb:
+        if channel <= _XYZ_NORMALIZATION_THRESHOLD:
+            linear_channel = channel / _XYZ_SML_VAL_DENOMINATOR
+        else:
+            linear_channel = channel + _XYZ_LRG_VAL_OFFSET
+            linear_channel /= _XYZ_LRG_VAL_DENOMINATOR
+            linear_channel = pow(linear_channel, _XYZ_LRG_VAL_EXPONENT)
+        linear_channels.append(linear_channel)
+
+    result_matrix = [
+        sum(x * y for x, y in zip(row, linear_channels)) for row in _RGB_TO_XYZ
+    ]
+    rgb_r, rgb_g, rgb_b = (max(c, 0) for c in result_matrix)
+    return rgb_r, rgb_g, rgb_b
+
+
+_CIE_E = 216 / 24389
+_1_3RD = 1 / 3
+_16_116THS = 16 / 116
+
+# this will always be the illuminant when rgb is converted to xyz from an without
+# an illuminant argument
+_XYZ_ILLUM = (0.95047, 1.0, 1.08883)
+
+
+def _xyz_to_lab(xyz: _Triple) -> Lab:
+    """Convert XYZ to Lab.
+
+    :param xyz: XYZ color tuple
+    :return: Lab color tuple
+    """
+    # this will always be the illuminant when rgb is converted to xyz from an without
+    # an illuminant argument
+    scaled_xyz = [c / y for c, y in zip(xyz, _XYZ_ILLUM)]
+    for i, channel in enumerate(scaled_xyz):
+        if channel > _CIE_E:
+            scaled_xyz[i] = channel**_1_3RD
+        else:
+            scaled_xyz[i] = (7.787 * channel) + _16_116THS
+
+    x, y, z = scaled_xyz
+    lab_l = (116 * y) - 16.0
+    lab_a = 500 * (x - y)
+    lab_b = 200 * (y - z)
+    return lab_l, lab_a, lab_b
+
+
+_RAD_6 = math.radians(6)
+_RAD_25 = math.radians(25)
+_RAD_30 = math.radians(30)
+_RAD_63 = math.radians(63)
+_RAD_180 = math.radians(180)
+_RAD_275 = math.radians(275)
+_RAD_360 = math.radians(360)
+_RAD_720 = math.radians(720)
+_V25_E7 = 25**7
+
+
+def rgb_to_lab(rgb: RGB) -> Lab:
+    """Convert RGB to Lab.
+
+    :param rgb: The RGB color to convert.
+    :return: The Lab color.
+    """
+    xyz = _rgb_to_xyz(rgb)
+    return _xyz_to_lab(xyz)
+
+
+def hex_to_lab(hex_: Hex) -> Lab:
+    """Convert hex color to Lab.
+
+    :param hex_: The hex color to convert.
+    :return: The Lab color.
+    """
+    rgb = hex_to_rgb(hex_)
+    return rgb_to_lab(rgb)
+
+
+def get_delta_e_lab(lab_a: Lab, lab_b: Lab) -> float:
+    """Calculate the Delta E (CIE2000) of two Lab colors.
+
+    :param lab_a: The first Lab color.
+    :param lab_b: The second Lab color.
+    :return: The Delta E (CIE2000) of the two colors.
+    """
+    lab_a_bsq = lab_a[2] ** 2
+    lab_b_bsq = lab_b[2] ** 2
+
+    Lp = (lab_a[0] + lab_b[0]) / 2.0
+
+    C1 = (lab_a[1] ** 2 + lab_a_bsq) ** 0.5
+    C2 = (lab_b[1] ** 2 + lab_b_bsq) ** 0.5
+    avg_c_e7 = ((C1 + C2) / 2.0) ** 7
+    G = 0.5 * (1 - (avg_c_e7 / (avg_c_e7 + _V25_E7)) ** 0.5) + 1
+
+    a1p, a2p = (lab[1] * G for lab in (lab_a, lab_b))
+
+    C1p = (a1p**2 + lab_a_bsq) ** 0.5
+    C2p = (a2p**2 + lab_b_bsq) ** 0.5
+    Cp = (C1p + C2p) / 2.0
+
+    h1p = math.atan2(lab_a[2], a1p)
+    h1p = h1p if h1p >= 0 else h1p + _RAD_360
+    h2p = math.atan2(lab_b[2], a2p)
+    h2p = h2p if h2p >= 0 else h2p + _RAD_360
+    Hp = (h1p + h2p) / 2
+    Hp = Hp if abs(h1p - h2p) <= _RAD_180 else Hp + _RAD_180
+
+    T = (
+        1
+        - 0.17 * math.cos(Hp - _RAD_30)
+        + 0.24 * math.cos(2 * Hp)
+        + 0.32 * math.cos(3 * Hp + _RAD_6)
+        - 0.2 * math.cos(4 * Hp - _RAD_63)
+    )
+
+    delta_hp = h2p - h1p
+    if abs(delta_hp) > _RAD_180:
+        if h2p > h1p:
+            delta_hp -= _RAD_360
+        else:
+            delta_hp += _RAD_360
+
+    delta_Lp = lab_b[0] - lab_a[0]
+    delta_Cp = C2p - C1p
+    delta_Hp = 2 * (C2p * C1p) ** 0.5 * math.sin(delta_hp / 2)
+
+    lp_minus_50_sq = (Lp - 50) ** 2
+    S_L = 1 + (0.015 * lp_minus_50_sq) / (20 + lp_minus_50_sq) ** 0.5
+    S_C = 1 + 0.045 * Cp
+    S_H = 1 + 0.015 * Cp * T
+
+    delta_ro = _RAD_30 * math.exp(-(((Hp - _RAD_275) / _RAD_25) ** 2))
+
+    avg_cp_e7 = Cp**7
+    R_C = (avg_cp_e7 / (avg_cp_e7 + _V25_E7)) ** 0.5
+    R_T = -2 * R_C * math.sin(2 * delta_ro)
+
+    return (
+        (delta_Lp / S_L) ** 2
+        + (delta_Cp / S_C) ** 2
+        + (delta_Hp / S_H) ** 2
+        + R_T * delta_Cp / S_C * delta_Hp / S_H
+    ) ** 0.5
+
+
+def get_sqeuclidean(rgb_a: RGB, rgb_b: RGB) -> float:
+    """Calculate the squared Euclidean distance between two RGB colors.
+
+    :param rgb_a: The first RGB color.
+    :param rgb_b: The second RGB color.
+    :return: The squared Euclidean distance between the two RGB colors.
+    """
+    return sum((a - b) ** 2 for a, b in zip(rgb_a, rgb_b))
+
+
+def get_sqeuclidean_hex(hex_a: Hex, hex_b: Hex) -> float:
+    """Calculate the squared Euclidean distance between two HEX colors.
+
+    :param hex_a: The first HEX color.
+    :param hex_b: The second HEX color.
+    :return: The squared Euclidean distance between the two HEX colors.
+    """
+    return get_sqeuclidean(hex_to_rgb(hex_a), hex_to_rgb(hex_b))
+
+
+def get_euclidean(rgb_a: RGB, rgb_b: RGB) -> float:
+    """Calculate the Euclidean distance between two RGB colors.
+
+    :param rgb_a: The first RGB color.
+    :param rgb_b: The second RGB color.
+    :return: The Euclidean distance between the two RGB colors.
+    """
+    return get_sqeuclidean(rgb_a, rgb_b) ** 0.5
+
+
+def get_euclidean_hex(hex_a: Hex, hex_b: Hex) -> float:
+    """Calculate the Euclidean distance between two HEX colors.
+
+    :param hex_a: The first HEX color.
+    :param hex_b: The second HEX color.
+    :return: The Euclidean distance between the two HEX colors.
+    """
+    return get_euclidean(hex_to_rgb(hex_a), hex_to_rgb(hex_b))
+
+
+def get_delta_e(rgb_a: RGB, rgb_b: RGB) -> float:
+    """Calculate the Delta E (CIE 2000) between two RGB colors.
+
+    :param rgb_a: The first RGB color.
+    :param rgb_b: The second RGB color.
+    :return: The Delta E (CIE 2000) between the two RGB colors.
+    """
+    return get_delta_e_lab(rgb_to_lab(rgb_a), rgb_to_lab(rgb_b))
+
+
+def get_delta_e_hex(hex_a: Hex, hex_b: Hex) -> float:
+    """Calculate the Delta E (CIE 2000) between two hex colors.
+
+    :param hex_a: The first hex color.
+    :param hex_b: The second hex color.
+    :return: The Delta E (CIE 2000) between the two hex colors.
+    """
+    return get_delta_e_lab(hex_to_lab(hex_a), hex_to_lab(hex_b))
```

### Comparing `basic_colormath-0.1.0/src/basic_colormath/mix.py` & `basic_colormath-0.1.3/src/basic_colormath/mix.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-"""Mix rgb or hex color values.
-
-:author: Shay Hill
-:created: 2023-04-30
-"""
-
-from __future__ import annotations
-
-from typing import TYPE_CHECKING, Union
-
-from basic_colormath.conversion import hex_to_rgb, rgb_to_hex
-
-if TYPE_CHECKING:
-    from basic_colormath.type_hints import RGB, Hex
-
-_Ratio = Union[float, "tuple[float, ...]", None]
-
-
-def _split_float(f: float, num: int) -> tuple[float, ...]:
-    """Divide a float into num parts.
-
-    :param f: float to divide
-    :param num: number of parts
-    :return: tuple of floats
-    """
-    return (f / num,) * num
-
-
-def _infer_ps(ratio: float | tuple[float, ...] | None, num: int) -> tuple[float, ...]:
-    """Infer p values from a single float or tuple of floats.
-
-    :param ratios: float or tuple of floats
-    :param num: number of ratios to return (len of rgb_args)
-    :return: tuple of floats summing to 1
-    :raise ValueError: if ratios cannot be distributed across values and sum to 1
-
-    Three cases:
-    1. ratio is None: return (1/num, ...)
-    2. ratio is a float: return (ratios, ((1-ratios) / (num-1), ...)
-    3. ratio is a tuple: fill in missing ratios with (1-sum(ratios)) / missing
-    """
-    # preserve ratio arg for error messages
-    ratio_arg = ratio
-    if ratio is None:
-        return _split_float(1, num)
-    if isinstance(ratio, (float, int)):
-        ratio = (ratio,)
-
-    if any(r < 0 for r in ratio):
-        msg = f"ratios must be >= 0, not {ratio_arg}"
-        raise ValueError(msg)
-    if len(ratio) > num:
-        msg = f"ratios has {len(ratio)} elements, but only <= {num} are allowed"
-        raise ValueError(msg)
-    sum_ratios = sum(ratio)
-    missing = num - len(ratio)
-    if sum_ratios == 0 and missing == 0:
-        msg = f"ratios must sum to > 0, not {sum_ratios}"
-        raise ValueError(msg)
-    if sum_ratios >= 1:
-        return tuple(r / sum_ratios for r in ratio) + _split_float(0, missing)
-    return ratio + _split_float(1 - sum_ratios, missing)
-
-
-def scale_rgb(rgb: RGB, scalar: float) -> RGB:
-    """Scale an rgb tuple by a scalar.
-
-    :param rgb: rgb tuple to scale ([0, 255], [0, 255], [0, 255])
-    :param scalar: scalar to multiply each element by
-    :return: scaled rgb tuple
-    """
-    red, grn, blu = (scalar * i for i in rgb)
-    return red, grn, blu
-
-
-def mix_rgb(*rgb_args: RGB, ratio: _Ratio = None) -> RGB:
-    """Mix any number of rgb tuples.
-
-    :param rgb_args: rgb tuples ([0, 255], [0, 255], [0, 255])
-    :param ratio: 0.0 to 1.0 for the weight of the first rgb_arg or a tuple of floats
-        to distribute across rgb_args or None for equal ratios. Ratios will be
-        normalized and (if fewer ratios than colors are provided) the remaining
-        ratios will be equal.
-    :return: rgb tuple ([0, 255], [0, 255], [0, 255])
-    """
-    ps = _infer_ps(ratio, len(rgb_args))
-    scaled_rgbs = [scale_rgb(rgb, p) for rgb, p in zip(rgb_args, ps)]
-    red, grn, blu = (sum(i) for i in zip(*scaled_rgbs))
-    return (red, grn, blu)
-
-
-def scale_hex(hex_: Hex, scalar: float) -> Hex:
-    """Scale a hex color by a scalar.
-
-    :param hex_: hex color with or without leading #
-    :param scalar: scalar to multiply each element by
-    :return: scaled hex color with leading #
-    """
-    return rgb_to_hex(scale_rgb(hex_to_rgb(hex_), scalar))
-
-
-def mix_hex(*hex_args: Hex, ratio: _Ratio = None) -> Hex:
-    """Mix any number of hex colors.
-
-    :param hex_args: hex colors with or without leading #
-    :param ratio: 0.0 to 1.0 for the weight of the first rgb_arg or a tuple of floats
-        to distribute across rgb_args or None for equal ratios. Ratios will be
-        normalized and (if fewer ratios than colors are provided) the remaining
-        ratios will be equal.
-    :return: hex string with leading #
-    """
-    return rgb_to_hex(mix_rgb(*(hex_to_rgb(i) for i in hex_args), ratio=ratio))
+"""Mix rgb or hex color values.
+
+:author: Shay Hill
+:created: 2023-04-30
+"""
+
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Union
+
+from basic_colormath.conversion import hex_to_rgb, rgb_to_hex
+
+if TYPE_CHECKING:
+    from basic_colormath.type_hints import RGB, Hex
+
+_Ratio = Union[float, "tuple[float, ...]", None]
+
+
+def _split_float(f: float, num: int) -> tuple[float, ...]:
+    """Divide a float into num parts.
+
+    :param f: float to divide
+    :param num: number of parts
+    :return: tuple of floats
+    """
+    return (f / num,) * num
+
+
+def _infer_ps(ratio: float | tuple[float, ...] | None, num: int) -> tuple[float, ...]:
+    """Infer p values from a single float or tuple of floats.
+
+    :param ratios: float or tuple of floats
+    :param num: number of ratios to return (len of rgb_args)
+    :return: tuple of floats summing to 1
+    :raise ValueError: if ratios cannot be distributed across values and sum to 1
+
+    Three cases:
+    1. ratio is None: return (1/num, ...)
+    2. ratio is a float: return (ratios, ((1-ratios) / (num-1), ...)
+    3. ratio is a tuple: fill in missing ratios with (1-sum(ratios)) / missing
+    """
+    # preserve ratio arg for error messages
+    ratio_arg = ratio
+    if ratio is None:
+        return _split_float(1, num)
+    if isinstance(ratio, (float, int)):
+        ratio = (ratio,)
+
+    if any(r < 0 for r in ratio):
+        msg = f"ratios must be >= 0, not {ratio_arg}"
+        raise ValueError(msg)
+    if len(ratio) > num:
+        msg = f"ratios has {len(ratio)} elements, but only <= {num} are allowed"
+        raise ValueError(msg)
+    sum_ratios = sum(ratio)
+    missing = num - len(ratio)
+    if sum_ratios == 0 and missing == 0:
+        msg = f"ratios must sum to > 0, not {sum_ratios}"
+        raise ValueError(msg)
+    if sum_ratios >= 1:
+        return tuple(r / sum_ratios for r in ratio) + _split_float(0, missing)
+    return ratio + _split_float(1 - sum_ratios, missing)
+
+
+def scale_rgb(rgb: RGB, scalar: float) -> RGB:
+    """Scale an rgb tuple by a scalar.
+
+    :param rgb: rgb tuple to scale ([0, 255], [0, 255], [0, 255])
+    :param scalar: scalar to multiply each element by
+    :return: scaled rgb tuple
+    """
+    red, grn, blu = (scalar * i for i in rgb)
+    return red, grn, blu
+
+
+def mix_rgb(*rgb_args: RGB, ratio: _Ratio = None) -> RGB:
+    """Mix any number of rgb tuples.
+
+    :param rgb_args: rgb tuples ([0, 255], [0, 255], [0, 255])
+    :param ratio: 0.0 to 1.0 for the weight of the first rgb_arg or a tuple of floats
+        to distribute across rgb_args or None for equal ratios. Ratios will be
+        normalized and (if fewer ratios than colors are provided) the remaining
+        ratios will be equal.
+    :return: rgb tuple ([0, 255], [0, 255], [0, 255])
+    """
+    ps = _infer_ps(ratio, len(rgb_args))
+    scaled_rgbs = [scale_rgb(rgb, p) for rgb, p in zip(rgb_args, ps)]
+    red, grn, blu = (sum(i) for i in zip(*scaled_rgbs))
+    return (red, grn, blu)
+
+
+def scale_hex(hex_: Hex, scalar: float) -> Hex:
+    """Scale a hex color by a scalar.
+
+    :param hex_: hex color with or without leading #
+    :param scalar: scalar to multiply each element by
+    :return: scaled hex color with leading #
+    """
+    return rgb_to_hex(scale_rgb(hex_to_rgb(hex_), scalar))
+
+
+def mix_hex(*hex_args: Hex, ratio: _Ratio = None) -> Hex:
+    """Mix any number of hex colors.
+
+    :param hex_args: hex colors with or without leading #
+    :param ratio: 0.0 to 1.0 for the weight of the first rgb_arg or a tuple of floats
+        to distribute across rgb_args or None for equal ratios. Ratios will be
+        normalized and (if fewer ratios than colors are provided) the remaining
+        ratios will be equal.
+    :return: hex string with leading #
+    """
+    return rgb_to_hex(mix_rgb(*(hex_to_rgb(i) for i in hex_args), ratio=ratio))
```

### Comparing `basic_colormath-0.1.0/src/basic_colormath/type_hints.py` & `basic_colormath-0.1.3/src/basic_colormath/type_hints.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-"""Type hints for color tuples.
-
-:author: Shay Hill
-:created: 2023-04-30
-"""
-from typing import Tuple
-
-# Type annotations lose Python 3.8 compatibility. Not enough justification IMO, but
-# the information is useful.
-
-"""
-RGB = Annotated[tuple[float, float, float], ([0, 255], [0, 255], [0, 255])]
-HSV = Annotated[tuple[float, float, float], ([0, 365), [0, 100], [0, 100])]
-HSL = Annotated[tuple[float, float, float], ([0, 365), [0, 100], [0, 100])]
-Lab = Annotated[tuple[float, float, float], ([0, 100], [-128, 127], [-128, 127])]
-Hex = Annotated[str, "#000fff"]
-"""
-
-
-RGB = Tuple[float, float, float]
-HSV = Tuple[float, float, float]
-HSL = Tuple[float, float, float]
-Lab = Tuple[float, float, float]
-Hex = str
+"""Type hints for color tuples.
+
+:author: Shay Hill
+:created: 2023-04-30
+
+Type annotations lose Python 3.8 compatibility. Not enough justification IMO, but the
+information is useful.
+
+RGB = Annotated[tuple[float, float, float], ([0, 255], [0, 255], [0, 255])]
+HSV = Annotated[tuple[float, float, float], ([0, 365), [0, 100], [0, 100])]
+HSL = Annotated[tuple[float, float, float], ([0, 365), [0, 100], [0, 100])]
+Lab = Annotated[tuple[float, float, float], ([0, 100], [-128, 127], [-128, 127])]
+Hex = Annotated[str, "#000fff"]
+"""
+
+from typing import Tuple
+
+RGB = Tuple[float, float, float]
+HSV = Tuple[float, float, float]
+HSL = Tuple[float, float, float]
+Lab = Tuple[float, float, float]
+Hex = str
```

### Comparing `basic_colormath-0.1.0/PKG-INFO` & `basic_colormath-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
-Name: basic-colormath
-Version: 0.1.0
-Summary: 
-Author: Shay Hill
-Author-email: shay_public@hotmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Name: basic_colormath
+Version: 0.1.3
+Summary: Simple color conversion and perceptual (DeltaE CIE 2000) difference
+Author-email: Shay Hill <shay_public@hotmail.com>
+License: MIT
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Requires-Dist: commitizen; extra == "dev"
+Requires-Dist: colormath; extra == "dev"
+Requires-Dist: numpy; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 
 # basic_colormath
 
 Everything I wanted to salvage from the [python-colormath](https://github.com/gtaylor/python-colormath/tree/master) library ... with no numpy deps and 14x speed.
 
 * Perceptual (DeltaE CIE 2000) and Euclidean distance between colors
 * Conversion between RGB, HSV, HSL, and 8-bit hex colors
@@ -123,8 +125,7 @@
 
         :param a: numpy array
         :return: input array as scalar
         """
         return a.item()
 
     np.asscalar = _patch_asscalar  # type: ignore
-
```

