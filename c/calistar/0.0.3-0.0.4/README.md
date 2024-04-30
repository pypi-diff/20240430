# Comparing `tmp/calistar-0.0.3.tar.gz` & `tmp/calistar-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calistar-0.0.3.tar", last modified: Sun Nov 12 20:23:07 2023, max compression
+gzip compressed data, was "calistar-0.0.4.tar", last modified: Tue Apr 30 08:43:02 2024, max compression
```

## Comparing `calistar-0.0.3.tar` & `calistar-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-11-12 20:23:07.402347 calistar-0.0.3/
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1070 2023-10-24 07:09:05.000000 calistar-0.0.3/LICENSE
--rw-r--r--   0 tomasstolker   (501) staff       (20)     2702 2023-11-12 20:23:07.402179 calistar-0.0.3/PKG-INFO
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1936 2023-10-28 16:30:41.000000 calistar-0.0.3/README.rst
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-11-12 20:23:07.401053 calistar-0.0.3/calistar/
--rw-r--r--   0 tomasstolker   (501) staff       (20)      212 2023-11-12 20:18:04.000000 calistar-0.0.3/calistar/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    37987 2023-11-12 19:46:24.000000 calistar-0.0.3/calistar/calistar.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-11-12 20:23:07.401950 calistar-0.0.3/calistar.egg-info/
--rw-r--r--   0 tomasstolker   (501) staff       (20)     2702 2023-11-12 20:23:07.000000 calistar-0.0.3/calistar.egg-info/PKG-INFO
--rw-r--r--   0 tomasstolker   (501) staff       (20)      259 2023-11-12 20:23:07.000000 calistar-0.0.3/calistar.egg-info/SOURCES.txt
--rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2023-11-12 20:23:07.000000 calistar-0.0.3/calistar.egg-info/dependency_links.txt
--rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2023-11-12 20:23:07.000000 calistar-0.0.3/calistar.egg-info/not-zip-safe
--rw-r--r--   0 tomasstolker   (501) staff       (20)       77 2023-11-12 20:23:07.000000 calistar-0.0.3/calistar.egg-info/requires.txt
--rw-r--r--   0 tomasstolker   (501) staff       (20)        9 2023-11-12 20:23:07.000000 calistar-0.0.3/calistar.egg-info/top_level.txt
--rw-r--r--   0 tomasstolker   (501) staff       (20)       38 2023-11-12 20:23:07.402407 calistar-0.0.3/setup.cfg
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1305 2023-11-12 20:18:08.000000 calistar-0.0.3/setup.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-30 08:43:02.964222 calistar-0.0.4/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1070 2023-10-24 07:09:05.000000 calistar-0.0.4/LICENSE
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2928 2024-04-30 08:43:02.964064 calistar-0.0.4/PKG-INFO
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2162 2024-04-03 18:15:26.000000 calistar-0.0.4/README.rst
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-30 08:43:02.962988 calistar-0.0.4/calistar/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      212 2024-04-30 08:35:27.000000 calistar-0.0.4/calistar/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    43695 2024-04-30 08:12:51.000000 calistar-0.0.4/calistar/calistar.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-30 08:43:02.963871 calistar-0.0.4/calistar.egg-info/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2928 2024-04-30 08:43:02.000000 calistar-0.0.4/calistar.egg-info/PKG-INFO
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      259 2024-04-30 08:43:02.000000 calistar-0.0.4/calistar.egg-info/SOURCES.txt
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2024-04-30 08:43:02.000000 calistar-0.0.4/calistar.egg-info/dependency_links.txt
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2024-04-30 08:43:02.000000 calistar-0.0.4/calistar.egg-info/not-zip-safe
+-rw-r--r--   0 tomasstolker   (501) staff       (20)       77 2024-04-30 08:43:02.000000 calistar-0.0.4/calistar.egg-info/requires.txt
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        9 2024-04-30 08:43:02.000000 calistar-0.0.4/calistar.egg-info/top_level.txt
+-rw-r--r--   0 tomasstolker   (501) staff       (20)       38 2024-04-30 08:43:02.964274 calistar-0.0.4/setup.cfg
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1305 2024-04-30 08:35:46.000000 calistar-0.0.4/setup.py
```

### Comparing `calistar-0.0.3/LICENSE` & `calistar-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `calistar-0.0.3/PKG-INFO` & `calistar-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calistar
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool to search for a single calibration star
 Home-page: https://github.com/tomasstolker/calistar
 Author: Tomas Stolker
 Author-email: stolker@strw.leidenuniv.nl
 License: MIT
 Project-URL: Documentation, https://calistar.readthedocs.io
 Keywords: calistar
@@ -18,34 +18,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 *calistar*
 ==========
 
-.. image:: https://img.shields.io/pypi/v/calistar
-   :target: https://pypi.python.org/pypi/calistar
-
-.. image:: https://img.shields.io/pypi/pyversions/calistar
-   :target: https://pypi.python.org/pypi/calistar
+.. container::
 
-.. image:: https://github.com/tomasstolker/calistar/workflows/CI/badge.svg?branch=main
-   :target: https://github.com/tomasstolker/calistar/actions
-
-.. image:: https://img.shields.io/readthedocs/calistar
-   :target: http://calistar.readthedocs.io
-
-.. image:: https://codecov.io/gh/tomasstolker/calistar/branch/main/graph/badge.svg?token=LSSCPMJ5JH
-   :target: https://codecov.io/gh/tomasstolker/calistar
-
-.. image:: https://img.shields.io/codefactor/grade/github/tomasstolker/calistar
-   :target: https://www.codefactor.io/repository/github/tomasstolker/calistar
-
-.. image:: https://img.shields.io/github/license/tomasstolker/calistar
-   :target: https://github.com/tomasstolker/calistar/blob/main/LICENSE
+    |PyPI Status| |Python Versions| |CI Status| |Docs Status| |Code Coverage| |Code Quality| |License|
 
 *calistar* is a tool to search for a single calibration star. For example to be used for reference-star differential imaging or aperture masking interferometry. The package has been released on `PyPI <https://pypi.org/project/calistar/>`_ and is actively developed and maintained on Github.
 
 Documentation
 -------------
 
 Documentation can be found at `http://calistar.readthedocs.io <http://calistar.readthedocs.io>`_.
@@ -54,10 +37,31 @@
 ------------
 
 Contributions are welcome so please consider `forking <https://help.github.com/en/articles/fork-a-repo>`_ the repository and creating a `pull request <https://github.com/tomasstolker/calistar/pulls>`_. Bug reports and feature requests can be provided by creating an `issue <https://github.com/tomasstolker/calistar/issues>`_ on the Github page.
 
 License
 -------
 
-Copyright 2023 Tomas Stolker
+Copyright 2023-2024 Tomas Stolker
 
 *calistar* is distributed under the MIT License. See `LICENSE <https://github.com/tomasstolker/pycrires/blob/main/LICENSE>`_ for the terms and conditions.
+
+.. |PyPI Status| image:: https://img.shields.io/pypi/v/calistar
+   :target: https://pypi.python.org/pypi/calistar
+
+.. |Python Versions| image:: https://img.shields.io/pypi/pyversions/calistar
+   :target: https://pypi.python.org/pypi/calistar
+
+.. |CI Status| image:: https://github.com/tomasstolker/calistar/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/tomasstolker/calistar/actions
+
+.. |Docs Status| image:: https://img.shields.io/readthedocs/calistar
+   :target: http://calistar.readthedocs.io
+
+.. |Code Coverage| image:: https://codecov.io/gh/tomasstolker/calistar/branch/main/graph/badge.svg?token=LSSCPMJ5JH
+   :target: https://codecov.io/gh/tomasstolker/calistar
+
+.. |Code Quality| image:: https://img.shields.io/codefactor/grade/github/tomasstolker/calistar
+   :target: https://www.codefactor.io/repository/github/tomasstolker/calistar
+
+.. |License| image:: https://img.shields.io/github/license/tomasstolker/calistar
+   :target: https://github.com/tomasstolker/calistar/blob/main/LICENSE
```

### Comparing `calistar-0.0.3/README.rst` & `calistar-0.0.4/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,13 @@
 *calistar*
 ==========
 
-.. image:: https://img.shields.io/pypi/v/calistar
-   :target: https://pypi.python.org/pypi/calistar
-
-.. image:: https://img.shields.io/pypi/pyversions/calistar
-   :target: https://pypi.python.org/pypi/calistar
+.. container::
 
-.. image:: https://github.com/tomasstolker/calistar/workflows/CI/badge.svg?branch=main
-   :target: https://github.com/tomasstolker/calistar/actions
-
-.. image:: https://img.shields.io/readthedocs/calistar
-   :target: http://calistar.readthedocs.io
-
-.. image:: https://codecov.io/gh/tomasstolker/calistar/branch/main/graph/badge.svg?token=LSSCPMJ5JH
-   :target: https://codecov.io/gh/tomasstolker/calistar
-
-.. image:: https://img.shields.io/codefactor/grade/github/tomasstolker/calistar
-   :target: https://www.codefactor.io/repository/github/tomasstolker/calistar
-
-.. image:: https://img.shields.io/github/license/tomasstolker/calistar
-   :target: https://github.com/tomasstolker/calistar/blob/main/LICENSE
+    |PyPI Status| |Python Versions| |CI Status| |Docs Status| |Code Coverage| |Code Quality| |License|
 
 *calistar* is a tool to search for a single calibration star. For example to be used for reference-star differential imaging or aperture masking interferometry. The package has been released on `PyPI <https://pypi.org/project/calistar/>`_ and is actively developed and maintained on Github.
 
 Documentation
 -------------
 
 Documentation can be found at `http://calistar.readthedocs.io <http://calistar.readthedocs.io>`_.
@@ -33,10 +16,31 @@
 ------------
 
 Contributions are welcome so please consider `forking <https://help.github.com/en/articles/fork-a-repo>`_ the repository and creating a `pull request <https://github.com/tomasstolker/calistar/pulls>`_. Bug reports and feature requests can be provided by creating an `issue <https://github.com/tomasstolker/calistar/issues>`_ on the Github page.
 
 License
 -------
 
-Copyright 2023 Tomas Stolker
+Copyright 2023-2024 Tomas Stolker
 
 *calistar* is distributed under the MIT License. See `LICENSE <https://github.com/tomasstolker/pycrires/blob/main/LICENSE>`_ for the terms and conditions.
+
+.. |PyPI Status| image:: https://img.shields.io/pypi/v/calistar
+   :target: https://pypi.python.org/pypi/calistar
+
+.. |Python Versions| image:: https://img.shields.io/pypi/pyversions/calistar
+   :target: https://pypi.python.org/pypi/calistar
+
+.. |CI Status| image:: https://github.com/tomasstolker/calistar/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/tomasstolker/calistar/actions
+
+.. |Docs Status| image:: https://img.shields.io/readthedocs/calistar
+   :target: http://calistar.readthedocs.io
+
+.. |Code Coverage| image:: https://codecov.io/gh/tomasstolker/calistar/branch/main/graph/badge.svg?token=LSSCPMJ5JH
+   :target: https://codecov.io/gh/tomasstolker/calistar
+
+.. |Code Quality| image:: https://img.shields.io/codefactor/grade/github/tomasstolker/calistar
+   :target: https://www.codefactor.io/repository/github/tomasstolker/calistar
+
+.. |License| image:: https://img.shields.io/github/license/tomasstolker/calistar
+   :target: https://github.com/tomasstolker/calistar/blob/main/LICENSE
```

### Comparing `calistar-0.0.3/calistar/calistar.py` & `calistar-0.0.4/calistar/calistar.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,17 +28,14 @@
 
 import calistar
 
 
 # No limit on the number of rows with a Gaia query
 Gaia.ROW_LIMIT = -1
 
-# Only return the nearest source with a Vizier query
-Vizier.ROW_LIMIT = 1
-
 
 class CaliStar:
     """
     Class for finding calibration stars based on their separation
     and magnitude difference with the selected ``gaia_source``.
     """
 
@@ -165,14 +162,16 @@
                 progressbar=True,
             )
 
     @typechecked
     def target_star(
         self,
         write_json: bool = True,
+        get_gaiaxp: bool = True,
+        allwise_catalog: bool = True,
     ) -> Dict[str, Union[str, float]]:
         """
         Function for retrieving the the astrometric and
         photometric properties of a target star of interest. The
         function returns a dictionary with the properties, but it
         also (optionally) stores the data in a JSON file in the
         working folder.
@@ -180,14 +179,23 @@
         Parameters
         ----------
         write_json : bool
             Write the target properties to a JSON file (default: True).
             The file will be stored in the working folder and starts
             with ``target_``. The filename contains also the Gaia
             release and the Gaia source ID of the target.
+        get_gaiaxp : bool
+            Retrieve the Gaia XP spectrum if available (default: True).
+            If set to ``True``, the spectrum will be written to a data
+            file and a plot will also be created. The spectrum is not
+            retrieved when the argument is set to ``False``.
+        allwise_catalog : bool
+            Select the WISE magnitudes from the ALLWISE catalog if set
+            to ``True`` or select the magnitudes from the earlier WISE
+            catalog if set to ``False``.
 
         Returns
         -------
         dict
             Dictionary with the properties of the target star.
         """
 
@@ -248,15 +256,22 @@
 
         mag_rp_error = (
             -2.5 / np.log(10.0) / gaia_result["phot_rp_mean_flux_over_error"][0]
         )
 
         mag_rp_error = np.sqrt(mag_rp_error**2 + gaia_rp_zp[1] ** 2)
 
-        target_dict["Gaia ID"] = int(gaia_result["source_id"][0])
+        if "SOURCE_ID" in gaia_result.columns:
+            gaia_source_id = int(gaia_result["SOURCE_ID"][0])
+        elif "source_id" in gaia_result.columns:
+            gaia_source_id = int(gaia_result["source_id"][0])
+        else:
+            raise ValueError(f"Gaia source ID not found in {gaia_result}")
+
+        target_dict["Gaia ID"] = gaia_source_id
 
         target_dict["Gaia release"] = self.gaia_release
 
         target_dict["Gaia epoch"] = gaia_result["ref_epoch"][0]
 
         target_dict["Gaia RA"] = (
             float(gaia_result["ra"][0]),  # (deg)
@@ -284,56 +299,55 @@
         )
 
         target_dict[f"GAIA/GAIA{self.gaia_idx}.G"] = (
             float(gaia_result["phot_g_mean_mag"][0]),
             mag_g_error,
         )
 
-        target_dict[f"GAIA/GAIA{self.gaia_idx}.Gbp"] = (
-            float(gaia_result["phot_bp_mean_mag"][0]),
-            mag_bp_error,
-        )
-
-        target_dict[f"GAIA/GAIA{self.gaia_idx}.Grp"] = (
-            float(gaia_result["phot_rp_mean_mag"][0]),
-            mag_rp_error,
-        )
-
-        target_dict[f"GAIA/GAIA{self.gaia_idx}.Grp"] = (
-            float(gaia_result["phot_rp_mean_mag"][0]),
-            mag_rp_error,
-        )
+        if "phot_bp_mean_mag" in gaia_result.columns:
+            if not np.ma.is_masked(gaia_result["phot_bp_mean_mag"][0]):
+                target_dict[f"GAIA/GAIA{self.gaia_idx}.Gbp"] = (
+                    float(gaia_result["phot_bp_mean_mag"][0]),
+                    mag_bp_error,
+                )
+
+        if "phot_rp_mean_mag" in gaia_result.columns:
+            if not np.ma.is_masked(gaia_result["phot_rp_mean_mag"][0]):
+                target_dict[f"GAIA/GAIA{self.gaia_idx}.Grp"] = (
+                    float(gaia_result["phot_rp_mean_mag"][0]),
+                    mag_rp_error,
+                )
 
         if "grvs_mag" in gaia_result.columns:
-            target_dict[f"GAIA/GAIA{self.gaia_idx}.Grvs"] = (
-                float(gaia_result["grvs_mag"][0]),
-                float(gaia_result["grvs_mag_error"][0]),
-            )
+            if not np.ma.is_masked(gaia_result["grvs_mag"][0]):
+                target_dict[f"GAIA/GAIA{self.gaia_idx}.Grvs"] = (
+                    float(gaia_result["grvs_mag"][0]),
+                    float(gaia_result["grvs_mag_error"][0]),
+                )
 
         # Create SkyCoord object from the RA and Dec of the selected Gaia source ID
 
         gaia_coord = SkyCoord(
             gaia_result["ra"][0],
             gaia_result["dec"][0],
             frame="icrs",
             unit=(u.deg, u.deg),
         )
 
         coord_str = gaia_coord.to_string(
             "hmsdms", alwayssign=True, precision=2, pad=True
         )
 
-        if self.gaia_source != gaia_result["source_id"][0]:
+        if self.gaia_source != gaia_source_id:
             raise ValueError(
-                f"The requested source ID ({self.gaia_source}) "
-                "is not equal to the retrieved source ID "
-                f"({gaia_result['source_id'][0]})."
+                f"The requested source ID ({self.gaia_source}) is not "
+                f"equal to the retrieved source ID ({gaia_source_id})."
             )
 
-        print(f"\nGAIA {self.gaia_release} source ID = {gaia_result['source_id'][0]}")
+        print(f"\nGAIA {self.gaia_release} source ID = {gaia_source_id}")
         print(f"Reference epoch = {gaia_result['ref_epoch'][0]}")
 
         print(
             f"Parallax = {gaia_result['parallax'][0]:.2f} "
             f"+/- {gaia_result['parallax_error'][0]:.2f} mas"
         )
 
@@ -351,45 +365,52 @@
         )
 
         print(
             f"Proper motion Dec = {gaia_result['pmdec'][0]:.2f} "
             f"+/- {gaia_result['pmdec_error'][0]:.2f} mas/yr"
         )
 
-        if "radial_velocity" in gaia_result.columns and not np.ma.is_masked(
-            gaia_result["radial_velocity"]
-        ):
-            print(
-                f"Radial velocity = {gaia_result['radial_velocity'][0]:.2f} "
-                f"+/- {gaia_result['radial_velocity_error'][0]:.2f} km/s"
-            )
+        if "radial_velocity" in gaia_result.columns:
+            if not np.ma.is_masked(gaia_result["radial_velocity"]):
+                print(
+                    f"Radial velocity = {gaia_result['radial_velocity'][0]:.2f} "
+                    f"+/- {gaia_result['radial_velocity_error'][0]:.2f} km/s"
+                )
 
         print(
             f"\nG mag = {gaia_result['phot_g_mean_mag'][0]:.6f} +/- {mag_g_error:.6f}"
         )
-        print(
-            f"BP mag = {gaia_result['phot_bp_mean_mag'][0]:.6f} +/- {mag_bp_error:.6f}"
-        )
-        print(
-            f"RP mag = {gaia_result['phot_rp_mean_mag'][0]:.6f} +/- {mag_rp_error:.6f}"
-        )
 
-        if "grvs_mag" in gaia_result.columns:
-            print(
-                f"GRVS mag = {gaia_result['grvs_mag'][0]:.6f} "
-                f"+/- {gaia_result['grvs_mag_error'][0]:.6f}"
-            )
+        if "phot_bp_mean_mag" in gaia_result.columns:
+            if not np.ma.is_masked(gaia_result["phot_bp_mean_mag"][0]):
+                print(
+                    f"BP mag = {gaia_result['phot_bp_mean_mag'][0]:.6f} +/- {mag_bp_error:.6f}"
+                )
+
+        if "phot_rp_mean_mag" in gaia_result.columns:
+            if not np.ma.is_masked(gaia_result["phot_rp_mean_mag"][0]):
+                print(
+                    f"RP mag = {gaia_result['phot_rp_mean_mag'][0]:.6f} +/- {mag_rp_error:.6f}"
+                )
 
-        if "teff_gspphot" in gaia_result.columns and not np.ma.is_masked(
-            gaia_result["teff_gspphot"]
-        ):
-            print(f"\nEffective temperature = {gaia_result['teff_gspphot'][0]:.0f} K")
-            print(f"Surface gravity = {gaia_result['logg_gspphot'][0]:.2f}")
-            print(f"Metallicity = {gaia_result['mh_gspphot'][0]:.2f}")
-            print(f"G-band extinction = {gaia_result['ag_gspphot'][0]:.2f}")
+        if "grvs_mag" in gaia_result.columns:
+            if not np.ma.is_masked(gaia_result["grvs_mag"][0]):
+                print(
+                    f"GRVS mag = {gaia_result['grvs_mag'][0]:.6f} "
+                    f"+/- {gaia_result['grvs_mag_error'][0]:.6f}"
+                )
+
+        if "teff_gspphot" in gaia_result.columns:
+            if not np.ma.is_masked(gaia_result["teff_gspphot"]):
+                print(
+                    f"\nEffective temperature = {gaia_result['teff_gspphot'][0]:.0f} K"
+                )
+                print(f"Surface gravity = {gaia_result['logg_gspphot'][0]:.2f}")
+                print(f"Metallicity = {gaia_result['mh_gspphot'][0]:.2f}")
+                print(f"G-band extinction = {gaia_result['ag_gspphot'][0]:.2f}")
 
         print(
             f"\nAstrometric excess noise = {gaia_result['astrometric_excess_noise'][0]:.2f}"
         )
 
         if "ruwe" in gaia_result.columns:
             print(f"RUWE = {gaia_result['ruwe'][0]:.2f}")
@@ -410,15 +431,15 @@
             print(f"XP sampled = {gaia_result['has_xp_sampled'][0]}")
 
         if "has_rvs" in gaia_result.columns:
             print(f"RVS spectrum = {gaia_result['has_rvs'][0]}")
 
         # Gaia XP spectrum
 
-        if (
+        if get_gaiaxp and (
             "has_xp_continuous" in gaia_result.columns
             and gaia_result["has_xp_continuous"][0]
         ):
             # Sampling adopted from the Gaia XP documentation
             df_cal, sampling = calibrate(
                 input_object=[f"{self.gaia_source}"],
                 sampling=np.geomspace(330, 1049.9999999999, 361),
@@ -428,15 +449,15 @@
                 # output_file=f"{self.gaia_source}_gaiaxp",
                 output_format=None,
                 save_file=False,
                 username=None,
                 password=None,
             )
 
-            xp_plot = f"{self.gaia_source}_gaiaxp"
+            xp_plot = f"gaiaxp_{self.gaia_source}"
             print(f"\nStoring Gaia XP plot: {xp_plot}_0.jpg")
 
             plot_spectra(
                 spectra=df_cal,
                 sampling=sampling,
                 multi=False,
                 show_plot=False,
@@ -447,192 +468,288 @@
             )
 
             xp_wavel = sampling * 1e-3  # (nm) -> (um)
             xp_flux = 1e3 * df_cal["flux"].to_numpy()[0]  # (W m-2 nm-1) -> (W m-2 um-1)
             xp_error = 1e3 * df_cal["flux_error"].to_numpy()[0]
 
             header = "Wavelength (um) - Flux (W m-2 um-1) - Uncertainty (W m-2 um-1)"
-            xp_file = f"{self.gaia_source}_gaiaxp_spec.dat"
+            xp_file = f"gaiaxp_{self.gaia_source}.dat"
             xp_spec = np.column_stack([xp_wavel, xp_flux, xp_error])
             np.savetxt(xp_file, xp_spec, header=header)
-            print(f"Storing Gaia XP spectrum: {xp_file}")
+            print(f"Storing Gaia XP data: {xp_file}")
 
         # Add spectral type to the Simbad output
 
         # print(Simbad.list_votable_fields())
 
         Simbad.add_votable_fields(
             "sptype",
+            "ids",
             # "flux(J)",
             # "flux(H)",
             # "flux(K)",
             # "flux_error(J)",
             # "flux_error(H)",
             # "flux_error(K)",
         )
 
         # Simbad query for selected Gaia source ID
 
         print("\n-> Querying Simbad...\n")
+
         simbad_result = Simbad.query_object(
             f"GAIA {self.gaia_release} {self.gaia_source}"
         )
-        simbad_result = simbad_result[0]
 
-        # print(simbad_result.columns)
+        if simbad_result is not None:
+            simbad_result = simbad_result[0]
+
+            print(f"Simbad ID = {simbad_result['MAIN_ID']}")
 
-        print(f"Simbad ID = {simbad_result['MAIN_ID']}")
+            print(f"Spectral type = {simbad_result['SP_TYPE']}")
 
-        print(f"Spectral type = {simbad_result['SP_TYPE']}")
+            target_dict["Simbad ID"] = simbad_result["MAIN_ID"]
 
-        # print(
-        #     f"\n2MASS J mag = {simbad_result['FLUX_J']:.3f} "
-        #     f"+/- {simbad_result['FLUX_ERROR_J']:.3f}"
-        # )
-        #
-        # print(
-        #     f"2MASS H mag = {simbad_result['FLUX_H']:.3f} "
-        #     f"+/- {simbad_result['FLUX_ERROR_H']:.3f}"
-        # )
-        #
-        # print(
-        #     f"2MASS Ks mag = {simbad_result['FLUX_K']:.3f} "
-        #     f"+/- {simbad_result['FLUX_ERROR_K']:.3f}"
-        # )
-
-        target_dict["Simbad ID"] = simbad_result["MAIN_ID"]
-
-        target_dict["SpT"] = simbad_result["SP_TYPE"]
-
-        # target_dict["2MASS/2MASS.J"] = (
-        #     float(simbad_result["FLUX_J"]),
-        #     float(simbad_result["FLUX_ERROR_J"]),
-        # )
-        #
-        # target_dict["2MASS/2MASS.H"] = (
-        #     float(simbad_result["FLUX_H"]),
-        #     float(simbad_result["FLUX_ERROR_H"]),
-        # )
-        #
-        # target_dict["2MASS/2MASS.Ks"] = (
-        #     float(simbad_result["FLUX_K"]),
-        #     float(simbad_result["FLUX_ERROR_K"]),
-        # )
+            target_dict["SpT"] = simbad_result["SP_TYPE"]
+
+            # print(
+            #     f"\n2MASS J mag = {simbad_result['FLUX_J']:.3f} "
+            #     f"+/- {simbad_result['FLUX_ERROR_J']:.3f}"
+            # )
+            #
+            # print(
+            #     f"2MASS H mag = {simbad_result['FLUX_H']:.3f} "
+            #     f"+/- {simbad_result['FLUX_ERROR_H']:.3f}"
+            # )
+            #
+            # print(
+            #     f"2MASS Ks mag = {simbad_result['FLUX_K']:.3f} "
+            #     f"+/- {simbad_result['FLUX_ERROR_K']:.3f}"
+            # )
+
+            # target_dict["2MASS/2MASS.J"] = (
+            #     float(simbad_result["FLUX_J"]),
+            #     float(simbad_result["FLUX_ERROR_J"]),
+            # )
+            #
+            # target_dict["2MASS/2MASS.H"] = (
+            #     float(simbad_result["FLUX_H"]),
+            #     float(simbad_result["FLUX_ERROR_H"]),
+            # )
+            #
+            # target_dict["2MASS/2MASS.Ks"] = (
+            #     float(simbad_result["FLUX_K"]),
+            #     float(simbad_result["FLUX_ERROR_K"]),
+            # )
+
+        else:
+            print("\nTarget not found on Simbad")
 
         # VizieR query for the selected Gaia source ID
         # Sort the result by distance from the queried object
 
         print("\n-> Querying VizieR...\n")
 
         vizier_obj = Vizier(
-            columns=["*", "+_r"], catalog=["II/246/out", "II/328/allwise"]
+            columns=["*", "+_r"],
+            catalog=["II/246/out", "II/328/allwise", "II/311/wise"],
+            timeout=10.0,
+            row_limit=1,
         )
 
         radius = u.Quantity(1.0 * u.arcmin)
 
         vizier_result = vizier_obj.query_object(
             f"GAIA {self.gaia_release} {self.gaia_source}", radius=radius
         )
 
         # 2MASS data from VizieR
 
         vizier_2mass = vizier_result["II/246/out"]
-        vizier_2mass = vizier_2mass[0]
 
-        print(f"2MASS source ID = {vizier_2mass['_2MASS']}")
+        if vizier_2mass is not None:
+            vizier_2mass = vizier_2mass[0]
 
-        print(
-            f"Separation between Gaia and 2MASS source = "
-            f"{1e3*vizier_2mass['_r']:.1f} mas"
-        )
+            print(f"2MASS source ID = {vizier_2mass['_2MASS']}")
 
-        print(
-            f"\n2MASS J mag = {vizier_2mass['Jmag']:.3f} "
-            f"+/- {vizier_2mass['e_Jmag']:.3f}"
-        )
+            print(
+                f"Separation between Gaia and 2MASS source = "
+                f"{1e3*vizier_2mass['_r']:.1f} mas"
+            )
 
-        print(
-            f"2MASS H mag = {vizier_2mass['Hmag']:.3f} "
-            f"+/- {vizier_2mass['e_Hmag']:.3f}"
-        )
+            if np.ma.is_masked(vizier_2mass["e_Jmag"]):
+                print(f"\n2MASS J mag = >{vizier_2mass['Jmag']:.3f}")
 
-        print(
-            f"2MASS Ks mag = {vizier_2mass['Kmag']:.3f} "
-            f"+/- {vizier_2mass['e_Kmag']:.3f}"
-        )
+            else:
+                print(
+                    f"\n2MASS J mag = {vizier_2mass['Jmag']:.3f} "
+                    f"+/- {vizier_2mass['e_Jmag']:.3f}"
+                )
+
+                target_dict["2MASS/2MASS.J"] = (
+                    float(vizier_2mass["Jmag"]),
+                    float(vizier_2mass["e_Jmag"]),
+                )
+
+            if np.ma.is_masked(vizier_2mass["e_Hmag"]):
+                print(f"2MASS H mag = >{vizier_2mass['Hmag']:.3f}")
+
+            else:
+                print(
+                    f"2MASS H mag = {vizier_2mass['Hmag']:.3f} "
+                    f"+/- {vizier_2mass['e_Hmag']:.3f}"
+                )
+
+                target_dict["2MASS/2MASS.H"] = (
+                    float(vizier_2mass["Hmag"]),
+                    float(vizier_2mass["e_Hmag"]),
+                )
+
+            if np.ma.is_masked(vizier_2mass["e_Kmag"]):
+                print(f"2MASS Ks mag = >{vizier_2mass['Kmag']:.3f}")
+
+            else:
+                print(
+                    f"2MASS Ks mag = {vizier_2mass['Kmag']:.3f} "
+                    f"+/- {vizier_2mass['e_Kmag']:.3f}"
+                )
+
+                target_dict["2MASS/2MASS.Ks"] = (
+                    float(vizier_2mass["Kmag"]),
+                    float(vizier_2mass["e_Kmag"]),
+                )
 
-        target_dict["2MASS/2MASS.J"] = (
-            float(vizier_2mass["Jmag"]),
-            float(vizier_2mass["e_Jmag"]),
-        )
-        target_dict["2MASS/2MASS.H"] = (
-            float(vizier_2mass["Hmag"]),
-            float(vizier_2mass["e_Hmag"]),
-        )
-        target_dict["2MASS/2MASS.Ks"] = (
-            float(vizier_2mass["Kmag"]),
-            float(vizier_2mass["e_Kmag"]),
-        )
+        else:
+            print("Target not found in 2MASS catalog")
 
         # WISE data from VizieR
 
-        vizier_wise = vizier_result["II/328/allwise"]
-        vizier_wise = vizier_wise[0]
+        if allwise_catalog:
+            vizier_wise = vizier_result["II/328/allwise"]
+        else:
+            vizier_wise = vizier_result["II/311/wise"]
+
+        if vizier_wise is not None:
+            vizier_wise = vizier_wise[0]
+
+            if allwise_catalog:
+                print(f"\nALLWISE source ID = {vizier_wise['AllWISE']}")
+            else:
+                print(f"\nWISE source ID = {vizier_wise['WISE']}")
 
-        print(f"\nALLWISE source ID = {vizier_wise['AllWISE']}")
+            print(
+                f"Separation between Gaia and WISE source = "
+                f"{1e3*vizier_wise['_r']:.1f} mas"
+            )
 
-        print(
-            f"Separation between Gaia and ALLWISE source = "
-            f"{1e3*vizier_wise['_r']:.1f} mas"
-        )
+            if np.ma.is_masked(vizier_wise["e_W1mag"]):
+                print(f"\nWISE W1 mag = >{vizier_wise['W1mag']:.3f}")
 
-        print(
-            f"\nWISE W1 mag = {vizier_wise['W1mag']:.3f} "
-            f"+/- {vizier_wise['e_W1mag']:.3f}"
-        )
+            else:
+                print(
+                    f"\nWISE W1 mag = {vizier_wise['W1mag']:.3f} "
+                    f"+/- {vizier_wise['e_W1mag']:.3f}"
+                )
 
-        print(
-            f"WISE W2 mag = {vizier_wise['W2mag']:.3f} "
-            f"+/- {vizier_wise['e_W2mag']:.3f}"
-        )
+                target_dict["WISE/WISE.W1"] = (
+                    float(vizier_wise["W1mag"]),
+                    float(vizier_wise["e_W1mag"]),
+                )
 
-        print(
-            f"WISE W3 mag = {vizier_wise['W3mag']:.3f} "
-            f"+/- {vizier_wise['e_W3mag']:.3f}"
-        )
+            if np.ma.is_masked(vizier_wise["e_W2mag"]):
+                print(f"WISE W2 mag = >{vizier_wise['W2mag']:.3f}")
 
-        print(
-            f"WISE W4 mag = {vizier_wise['W4mag']:.3f} "
-            f"+/- {vizier_wise['e_W4mag']:.3f}"
-        )
+            else:
+                print(
+                    f"WISE W2 mag = {vizier_wise['W2mag']:.3f} "
+                    f"+/- {vizier_wise['e_W2mag']:.3f}"
+                )
 
-        target_dict["WISE/WISE.W1"] = (
-            float(vizier_wise["W1mag"]),
-            float(vizier_wise["e_W4mag"]),
-        )
+                target_dict["WISE/WISE.W2"] = (
+                    float(vizier_wise["W2mag"]),
+                    float(vizier_wise["e_W2mag"]),
+                )
 
-        target_dict["WISE/WISE.W2"] = (
-            float(vizier_wise["W2mag"]),
-            float(vizier_wise["e_W4mag"]),
-        )
+            if np.ma.is_masked(vizier_wise["e_W3mag"]):
+                print(f"WISE W3 mag = >{vizier_wise['W3mag']:.3f}")
 
-        target_dict["WISE/WISE.W3"] = (
-            float(vizier_wise["W3mag"]),
-            float(vizier_wise["e_W4mag"]),
-        )
+            else:
+                print(
+                    f"WISE W3 mag = {vizier_wise['W3mag']:.3f} "
+                    f"+/- {vizier_wise['e_W3mag']:.3f}"
+                )
 
-        target_dict["WISE/WISE.W4"] = (
-            float(vizier_wise["W4mag"]),
-            float(vizier_wise["e_W4mag"]),
-        )
+                target_dict["WISE/WISE.W3"] = (
+                    float(vizier_wise["W3mag"]),
+                    float(vizier_wise["e_W3mag"]),
+                )
+
+            if np.ma.is_masked(vizier_wise["e_W4mag"]):
+                print(f"WISE W4 mag = >{vizier_wise['W4mag']:.3f}")
+
+            else:
+                print(
+                    f"WISE W4 mag = {vizier_wise['W4mag']:.3f} "
+                    f"+/- {vizier_wise['e_W4mag']:.3f}"
+                )
+
+                target_dict["WISE/WISE.W4"] = (
+                    float(vizier_wise["W4mag"]),
+                    float(vizier_wise["e_W4mag"]),
+                )
+
+        else:
+            print("Target not found in WISE catalog")
+
+        # write_json = False
+
+        print("\n-> Querying Washington Double Star catalog...\n")
+
+        if simbad_result is not None:
+            simbad_ids = simbad_result["IDS"].split("|")
+            wds_id = list(filter(lambda x: x.startswith("WDS"), simbad_ids))
+
+            if len(wds_id) == 1:
+                wds_table = Table.read(self.wds_file, path="wds_catalog")
+                # print(wds_table.columns)
+
+                id_crop = wds_id[0].split(" ")[-1][1:11]
+                id_idx = np.where(id_crop == wds_table["WDS"])[0]
+
+                target_dict["WDS ID"] = wds_id[0]
+
+                for wds_idx in range(len(id_idx)):
+                    if wds_idx > 0:
+                        print()
+
+                    wds_select = wds_table[id_idx[wds_idx]]
+                    print(f"WDS ID = {wds_select['WDS']}")
+
+                    if len(wds_select["Comp"]) > 0:
+                        print(f"Companion = {wds_select['Comp']}")
+
+                    print(f"Observation 1 = {wds_select['Obs1']}")
+                    print(f"Observation 2 = {wds_select['Obs2']}")
+                    print(f"Separation 1 (arcsec) = {wds_select['sep1']:.2f}")
+                    print(f"Separation 2 (arcsec) = {wds_select['sep2']:.2f}")
+                    print(f"Position angle 1 (deg) = {wds_select['pa1']:.2f}")
+                    print(f"Position angle 2 (deg) = {wds_select['pa2']:.2f}")
+                    print(f"Magnitude 1 = {wds_select['mag1']:.2f}")
+                    print(f"Magnitude 2 = {wds_select['mag2']:.2f}")
+
+                # write_json = True
+
+            if len(wds_id) == 0 or len(id_idx) == 0:
+                print("Target not found in WDS catalog")
+
+        else:
+            print("Target not found in WDS catalog")
 
         if write_json:
-            json_file = (
-                f"target_{self.gaia_release.lower()}" f"_{self.gaia_source}.json"
-            )
+            json_file = f"target_{self.gaia_release.lower()}_{self.gaia_source}.json"
 
             print(f"\nStoring JSON output: {json_file}")
 
             with open(json_file, "w", encoding="utf-8") as open_file:
                 json.dump(target_dict, open_file, indent=4)
 
         return target_dict
@@ -767,18 +884,25 @@
         # Initiate all values in the dataframe to NaN
         cal_df = pd.DataFrame(index=range(len(gaia_results)), columns=columns)
 
         drop_indices = []
 
         warnings.filterwarnings("ignore", category=UserWarning)
 
-        vizier_obj = Vizier(columns=["*", "+_r"])
+        vizier_obj = Vizier(columns=["*", "+_r"], timeout=10.0, row_limit=1)
 
         for gaia_item in track(gaia_results, description="Processing..."):
-            cal_df.loc[gaia_item.index, "Gaia ID"] = gaia_item["source_id"]
+            if "SOURCE_ID" in gaia_item.columns:
+                gaia_source_id = int(gaia_item["SOURCE_ID"])
+            elif "source_id" in gaia_item.columns:
+                gaia_source_id = int(gaia_item["source_id"])
+            else:
+                raise ValueError(f"Gaia source ID not found in {gaia_item}")
+
+            cal_df.loc[gaia_item.index, "Gaia ID"] = gaia_source_id
 
             coord_target = SkyCoord(
                 target_dict["Gaia RA"][0],
                 target_dict["Gaia Dec"][0],
                 frame="icrs",
                 unit=(u.deg, u.deg),
             )
@@ -795,15 +919,15 @@
             cal_df.loc[gaia_item.index, "Separation"] = separation.deg
 
             cal_df.loc[gaia_item.index, f"GAIA/GAIA{self.gaia_idx}.G"] = gaia_item[
                 "phot_g_mean_mag"
             ]
 
             simbad_result = Simbad.query_object(
-                f"GAIA {self.gaia_release} {gaia_item['source_id']}"
+                f"GAIA {self.gaia_release} {gaia_source_id}"
             )
 
             if simbad_result is not None:
                 simbad_result = simbad_result[0]
 
                 if np.ma.is_masked(simbad_result["MAIN_ID"]):
                     cal_df.loc[gaia_item.index, "Simbad ID"] = np.nan
@@ -835,15 +959,15 @@
                 #     cal_df.loc[gaia_item.index, "2MASS/2MASS.Ks"] = simbad_result[
                 #         "FLUX_K"
                 #     ]
 
             radius = u.Quantity(1.0 * u.arcmin)
 
             vizier_result = vizier_obj.query_object(
-                f"GAIA {self.gaia_release} {gaia_item['source_id']}",
+                f"GAIA {self.gaia_release} {gaia_source_id}",
                 radius=radius,
                 catalog=["II/246/out", "II/328/allwise"],
             )
 
             if len(vizier_result) == 2:
                 # 2MASS
                 vizier_2mass = vizier_result["II/246/out"][0]
```

### Comparing `calistar-0.0.3/calistar.egg-info/PKG-INFO` & `calistar-0.0.4/calistar.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calistar
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool to search for a single calibration star
 Home-page: https://github.com/tomasstolker/calistar
 Author: Tomas Stolker
 Author-email: stolker@strw.leidenuniv.nl
 License: MIT
 Project-URL: Documentation, https://calistar.readthedocs.io
 Keywords: calistar
@@ -18,34 +18,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 *calistar*
 ==========
 
-.. image:: https://img.shields.io/pypi/v/calistar
-   :target: https://pypi.python.org/pypi/calistar
-
-.. image:: https://img.shields.io/pypi/pyversions/calistar
-   :target: https://pypi.python.org/pypi/calistar
+.. container::
 
-.. image:: https://github.com/tomasstolker/calistar/workflows/CI/badge.svg?branch=main
-   :target: https://github.com/tomasstolker/calistar/actions
-
-.. image:: https://img.shields.io/readthedocs/calistar
-   :target: http://calistar.readthedocs.io
-
-.. image:: https://codecov.io/gh/tomasstolker/calistar/branch/main/graph/badge.svg?token=LSSCPMJ5JH
-   :target: https://codecov.io/gh/tomasstolker/calistar
-
-.. image:: https://img.shields.io/codefactor/grade/github/tomasstolker/calistar
-   :target: https://www.codefactor.io/repository/github/tomasstolker/calistar
-
-.. image:: https://img.shields.io/github/license/tomasstolker/calistar
-   :target: https://github.com/tomasstolker/calistar/blob/main/LICENSE
+    |PyPI Status| |Python Versions| |CI Status| |Docs Status| |Code Coverage| |Code Quality| |License|
 
 *calistar* is a tool to search for a single calibration star. For example to be used for reference-star differential imaging or aperture masking interferometry. The package has been released on `PyPI <https://pypi.org/project/calistar/>`_ and is actively developed and maintained on Github.
 
 Documentation
 -------------
 
 Documentation can be found at `http://calistar.readthedocs.io <http://calistar.readthedocs.io>`_.
@@ -54,10 +37,31 @@
 ------------
 
 Contributions are welcome so please consider `forking <https://help.github.com/en/articles/fork-a-repo>`_ the repository and creating a `pull request <https://github.com/tomasstolker/calistar/pulls>`_. Bug reports and feature requests can be provided by creating an `issue <https://github.com/tomasstolker/calistar/issues>`_ on the Github page.
 
 License
 -------
 
-Copyright 2023 Tomas Stolker
+Copyright 2023-2024 Tomas Stolker
 
 *calistar* is distributed under the MIT License. See `LICENSE <https://github.com/tomasstolker/pycrires/blob/main/LICENSE>`_ for the terms and conditions.
+
+.. |PyPI Status| image:: https://img.shields.io/pypi/v/calistar
+   :target: https://pypi.python.org/pypi/calistar
+
+.. |Python Versions| image:: https://img.shields.io/pypi/pyversions/calistar
+   :target: https://pypi.python.org/pypi/calistar
+
+.. |CI Status| image:: https://github.com/tomasstolker/calistar/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/tomasstolker/calistar/actions
+
+.. |Docs Status| image:: https://img.shields.io/readthedocs/calistar
+   :target: http://calistar.readthedocs.io
+
+.. |Code Coverage| image:: https://codecov.io/gh/tomasstolker/calistar/branch/main/graph/badge.svg?token=LSSCPMJ5JH
+   :target: https://codecov.io/gh/tomasstolker/calistar
+
+.. |Code Quality| image:: https://img.shields.io/codefactor/grade/github/tomasstolker/calistar
+   :target: https://www.codefactor.io/repository/github/tomasstolker/calistar
+
+.. |License| image:: https://img.shields.io/github/license/tomasstolker/calistar
+   :target: https://github.com/tomasstolker/calistar/blob/main/LICENSE
```

### Comparing `calistar-0.0.3/setup.py` & `calistar-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open('requirements.txt') as req_txt:
     parse_req = pkg_resources.parse_requirements(req_txt)
     install_requires = [str(req) for req in parse_req]
 
 setuptools.setup(
     name='calistar',
-    version='0.0.3',
+    version='0.0.4',
     description='Tool to search for a single calibration star',
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     author='Tomas Stolker',
     author_email='stolker@strw.leidenuniv.nl',
     url='https://github.com/tomasstolker/calistar',
     project_urls={'Documentation': 'https://calistar.readthedocs.io'},
```

