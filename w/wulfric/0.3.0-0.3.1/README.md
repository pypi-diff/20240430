# Comparing `tmp/wulfric-0.3.0.tar.gz` & `tmp/wulfric-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wulfric-0.3.0.tar", last modified: Mon Feb 26 18:22:42 2024, max compression
+gzip compressed data, was "wulfric-0.3.1.tar", last modified: Tue Apr 30 17:31:37 2024, max compression
```

## Comparing `wulfric-0.3.0.tar` & `wulfric-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2024-02-26 18:22:42.076869 wulfric-0.3.0/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    32473 2023-12-09 21:40:39.000000 wulfric-0.3.0/LICENSE
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3352 2024-02-26 18:22:42.076030 wulfric-0.3.0/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1953 2024-02-22 15:31:54.000000 wulfric-0.3.0/README.rst
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1461 2024-01-31 00:15:19.000000 wulfric-0.3.0/pyproject.toml
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2024-02-26 18:22:42.077003 wulfric-0.3.0/setup.cfg
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2024-02-26 18:22:42.049499 wulfric-0.3.0/src/
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2024-02-26 18:22:42.063572 wulfric-0.3.0/src/wulfric/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1906 2024-02-26 18:22:31.000000 wulfric-0.3.0/src/wulfric/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1931 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/__main__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1056 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/_osfix.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    39465 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/_pinfo.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    19419 2024-02-26 12:46:08.000000 wulfric-0.3.0/src/wulfric/atom.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2024-02-26 18:22:42.071406 wulfric-0.3.0/src/wulfric/bravais_lattice/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1084 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/bravais_lattice/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    14888 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/bravais_lattice/constructor.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4762 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/bravais_lattice/examples.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    20737 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/bravais_lattice/hs_points.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    20219 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/bravais_lattice/standardize.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     8839 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/bravais_lattice/variations.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     6431 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/cell.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     7190 2024-02-23 11:37:36.000000 wulfric-0.3.0/src/wulfric/constants.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18289 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/crystal.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2024-02-26 18:22:42.072837 wulfric-0.3.0/src/wulfric/decorate/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      832 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/decorate/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    12563 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/decorate/array.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    12216 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/geometry.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    28364 2024-02-26 12:16:49.000000 wulfric-0.3.0/src/wulfric/identify.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2024-02-26 18:22:42.074073 wulfric-0.3.0/src/wulfric/io/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      830 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/io/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     8184 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/io/vasp.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    14806 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/kpoints.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    35309 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    38211 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/lattice_plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3846 2024-02-22 15:54:26.000000 wulfric-0.3.0/src/wulfric/numerical.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2024-02-26 18:22:42.074969 wulfric-0.3.0/src/wulfric.egg-info/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3352 2024-02-26 18:22:42.000000 wulfric-0.3.0/src/wulfric.egg-info/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      937 2024-02-26 18:22:42.000000 wulfric-0.3.0/src/wulfric.egg-info/SOURCES.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2024-02-26 18:22:42.000000 wulfric-0.3.0/src/wulfric.egg-info/dependency_links.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       50 2024-02-26 18:22:42.000000 wulfric-0.3.0/src/wulfric.egg-info/entry_points.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       50 2024-02-26 18:22:42.000000 wulfric-0.3.0/src/wulfric.egg-info/requires.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        8 2024-02-26 18:22:42.000000 wulfric-0.3.0/src/wulfric.egg-info/top_level.txt
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2024-04-30 17:31:37.147948 wulfric-0.3.1/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    32473 2023-12-09 21:40:39.000000 wulfric-0.3.1/LICENSE
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3352 2024-04-30 17:31:37.147319 wulfric-0.3.1/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1953 2024-02-22 15:31:54.000000 wulfric-0.3.1/README.rst
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1461 2024-01-31 00:15:19.000000 wulfric-0.3.1/pyproject.toml
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2024-04-30 17:31:37.148080 wulfric-0.3.1/setup.cfg
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2024-04-30 17:31:37.119918 wulfric-0.3.1/src/
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2024-04-30 17:31:37.134262 wulfric-0.3.1/src/wulfric/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1903 2024-04-30 17:31:31.000000 wulfric-0.3.1/src/wulfric/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1931 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/__main__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1056 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/_osfix.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    39465 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/_pinfo.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    19419 2024-02-26 12:46:08.000000 wulfric-0.3.1/src/wulfric/atom.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2024-04-30 17:31:37.142448 wulfric-0.3.1/src/wulfric/bravais_lattice/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1084 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/bravais_lattice/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    14888 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/bravais_lattice/constructor.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5368 2024-04-30 17:28:35.000000 wulfric-0.3.1/src/wulfric/bravais_lattice/examples.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    20737 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/bravais_lattice/hs_points.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    20219 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/bravais_lattice/standardize.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     8839 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/bravais_lattice/variations.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     6431 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/cell.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     7190 2024-02-23 11:37:36.000000 wulfric-0.3.1/src/wulfric/constants.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18289 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/crystal.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2024-04-30 17:31:37.143768 wulfric-0.3.1/src/wulfric/decorate/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      832 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/decorate/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    12563 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/decorate/array.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    12216 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/geometry.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    28364 2024-02-26 12:16:49.000000 wulfric-0.3.1/src/wulfric/identify.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2024-04-30 17:31:37.145193 wulfric-0.3.1/src/wulfric/io/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      830 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/io/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     8184 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/io/vasp.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    16615 2024-04-30 17:28:35.000000 wulfric-0.3.1/src/wulfric/kpoints.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    35309 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    38211 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/lattice_plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3846 2024-02-22 15:54:26.000000 wulfric-0.3.1/src/wulfric/numerical.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2024-04-30 17:31:37.146166 wulfric-0.3.1/src/wulfric.egg-info/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3352 2024-04-30 17:31:37.000000 wulfric-0.3.1/src/wulfric.egg-info/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      937 2024-04-30 17:31:37.000000 wulfric-0.3.1/src/wulfric.egg-info/SOURCES.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2024-04-30 17:31:37.000000 wulfric-0.3.1/src/wulfric.egg-info/dependency_links.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       50 2024-04-30 17:31:37.000000 wulfric-0.3.1/src/wulfric.egg-info/entry_points.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       50 2024-04-30 17:31:37.000000 wulfric-0.3.1/src/wulfric.egg-info/requires.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        8 2024-04-30 17:31:37.000000 wulfric-0.3.1/src/wulfric.egg-info/top_level.txt
```

### Comparing `wulfric-0.3.0/LICENSE` & `wulfric-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/PKG-INFO` & `wulfric-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wulfric
-Version: 0.3.0
+Version: 0.3.1
 Summary: Crystal, Lattice, Atoms, K-path.
 Author-email: Andrey Rybakov <rybakov.ad@icloud.com>
 License: GPL-3.0 license
 Project-URL: Homepage, https://wulfric.org
 Project-URL: Documentation, https://wulfric.org
 Project-URL: Repository, https://github.com/adrybakov/wulfric.git
 Project-URL: Issues, https://github.com/adrybakov/wulfric/issues
```

### Comparing `wulfric-0.3.0/README.rst` & `wulfric-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/pyproject.toml` & `wulfric-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/__init__.py` & `wulfric-0.3.1/src/wulfric/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __doclink__ = "wulfric.org"
-__git_hash__ = "5fb82627cf4e29e0bec963e761371a49e14d7ed7"
-__release_date__ = "26 February 2024"
+__git_hash__ = "3b45fdd8cd1a815934281c0e3d6758852dfeb4d5"
+__release_date__ = "30 April 2024"
 
 
 from . import bravais_lattice
 from . import cell as Cell
 from . import (
     constants,
     crystal,
```

### Comparing `wulfric-0.3.0/src/wulfric/__main__.py` & `wulfric-0.3.1/src/wulfric/__main__.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/_osfix.py` & `wulfric-0.3.1/src/wulfric/_osfix.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/_pinfo.py` & `wulfric-0.3.1/src/wulfric/_pinfo.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/atom.py` & `wulfric-0.3.1/src/wulfric/atom.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/bravais_lattice/__init__.py` & `wulfric-0.3.1/src/wulfric/bravais_lattice/__init__.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/bravais_lattice/constructor.py` & `wulfric-0.3.1/src/wulfric/bravais_lattice/constructor.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/bravais_lattice/examples.py` & `wulfric-0.3.1/src/wulfric/bravais_lattice/examples.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,24 +39,33 @@
 __all__ = [
     "lattice_example",
 ]
 
 
 def lattice_example(
     lattice_name: str = None,
+    convention: str = None,
 ):
     r"""
     Return an example of the lattice.
 
     Parameters
     ----------
     lattice_name : str, optional
         Name of the lattice to be returned.
         For available names see documentation of each Bravais lattice class.
         Lowercased before usage.
+    convention : str, optional
+        Name of the convention that is used for cell standardization.
+        Supported conventions are:
+        * "sc" - for Setyawan and Curtarolo standardization.
+
+        By default the lattice is not standardized.
+
+        .. versionadded:: 0.3.1
 
     Returns
     -------
     lattice : Lattice or list
         :py:class:`.Lattice` class is returned.
         If no math found a list with available examples is returned.
     """
@@ -77,75 +86,83 @@
         for name in BRAVAIS_LATTICE_VARIATIONS:
             message += f"  * {name}\n"
         raise ValueError(message)
 
     lattice_name = lattice_name.lower()
 
     if lattice_name == "cub":
-        return CUB(pi)
+        lattice = CUB(pi)
     elif lattice_name == "fcc":
-        return FCC(pi)
+        lattice = FCC(pi)
     elif lattice_name == "bcc":
-        return BCC(pi)
+        lattice = BCC(pi)
     elif lattice_name == "tet":
-        return TET(pi, 1.5 * pi)
+        lattice = TET(pi, 1.5 * pi)
     elif lattice_name in ["bct1", "bct"]:
-        return BCT(1.5 * pi, pi)
+        lattice = BCT(1.5 * pi, pi)
     elif lattice_name == "bct2":
-        return BCT(pi, 1.5 * pi)
+        lattice = BCT(pi, 1.5 * pi)
     elif lattice_name == "orc":
-        return ORC(pi, 1.5 * pi, 2 * pi)
+        lattice = ORC(pi, 1.5 * pi, 2 * pi)
     elif lattice_name in ["orcf1", "orcf"]:
-        return ORCF(0.7 * pi, 5 / 4 * pi, 5 / 3 * pi)
+        lattice = ORCF(0.7 * pi, 5 / 4 * pi, 5 / 3 * pi)
     elif lattice_name == "orcf2":
-        return ORCF(1.2 * pi, 5 / 4 * pi, 5 / 3 * pi)
+        lattice = ORCF(1.2 * pi, 5 / 4 * pi, 5 / 3 * pi)
     elif lattice_name == "orcf3":
-        return ORCF(pi, 5 / 4 * pi, 5 / 3 * pi)
+        lattice = ORCF(pi, 5 / 4 * pi, 5 / 3 * pi)
     elif lattice_name == "orci":
         return ORCI(pi, 1.3 * pi, 1.7 * pi)
     elif lattice_name == "orcc":
-        return ORCC(pi, 1.3 * pi, 1.7 * pi)
+        lattice = ORCC(pi, 1.3 * pi, 1.7 * pi)
     elif lattice_name == "hex":
-        return HEX(pi, 2 * pi)
+        lattice = HEX(pi, 2 * pi)
     elif lattice_name in ["rhl1", "rhl"]:
         # If alpha = 60 it is effectively FCC!
-        return RHL(pi, 70)
+        lattice = RHL(pi, 70)
     elif lattice_name == "rhl2":
-        return RHL(pi, 110)
+        lattice = RHL(pi, 110)
     elif lattice_name == "mcl":
-        return MCL(pi, 1.3 * pi, 1.6 * pi, alpha=75)
+        lattice = MCL(pi, 1.3 * pi, 1.6 * pi, alpha=75)
     elif lattice_name in ["mclc1", "mclc"]:
-        return MCLC(pi, 1.4 * pi, 1.7 * pi, 80)
+        lattice = MCLC(pi, 1.4 * pi, 1.7 * pi, 80)
     elif lattice_name == "mclc2":
-        return MCLC(1.4 * pi * sin(75 * TORADIANS), 1.4 * pi, 1.7 * pi, 75)
+        lattice = MCLC(1.4 * pi * sin(75 * TORADIANS), 1.4 * pi, 1.7 * pi, 75)
     elif lattice_name == "mclc3":
         b = pi
         x = 1.1
         alpha = 78
         ralpha = alpha * TORADIANS
         c = b * (x**2) / (x**2 - 1) * cos(ralpha) * 1.8
         a = x * b * sin(ralpha)
-        return MCLC(a, b, c, alpha)
+        lattice = MCLC(a, b, c, alpha)
     elif lattice_name == "mclc4":
         b = pi
         x = 1.2
         alpha = 65
         ralpha = alpha * TORADIANS
         c = b * (x**2) / (x**2 - 1) * cos(ralpha)
         a = x * b * sin(ralpha)
-        return MCLC(a, b, c, alpha)
+        lattice = MCLC(a, b, c, alpha)
     elif lattice_name == "mclc5":
         b = pi
         x = 1.4
         alpha = 53
         ralpha = alpha * TORADIANS
         c = b * (x**2) / (x**2 - 1) * cos(ralpha) * 0.9
         a = x * b * sin(ralpha)
-        return MCLC(a, b, c, alpha)
+        lattice = MCLC(a, b, c, alpha)
     elif lattice_name in ["tri1a", "tri1", "tri", "tria"]:
-        return TRI(1, 1.5, 2, 120, 110, 100, reciprocal=True)
+        lattice = TRI(1, 1.5, 2, 120, 110, 100, reciprocal=True)
     elif lattice_name in ["tri2a", "tri2"]:
-        return TRI(1, 1.5, 2, 120, 110, 90, reciprocal=True)
+        lattice = TRI(1, 1.5, 2, 120, 110, 90, reciprocal=True)
     elif lattice_name in ["tri1b", "trib"]:
-        return TRI(1, 1.5, 2, 60, 70, 80, reciprocal=True)
+        lattice = TRI(1, 1.5, 2, 60, 70, 80, reciprocal=True)
     elif lattice_name == "tri2b":
-        return TRI(1, 1.5, 2, 60, 70, 90, reciprocal=True)
+        lattice = TRI(1, 1.5, 2, 60, 70, 90, reciprocal=True)
+
+    if convention is not None:
+        if convention.lower() == "sc":
+            lattice.standardize()
+        else:
+            raise ValueError(f'Unknown standardization convention: "{convention}"')
+
+    return lattice
```

### Comparing `wulfric-0.3.0/src/wulfric/bravais_lattice/hs_points.py` & `wulfric-0.3.1/src/wulfric/bravais_lattice/hs_points.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/bravais_lattice/standardize.py` & `wulfric-0.3.1/src/wulfric/bravais_lattice/standardize.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/bravais_lattice/variations.py` & `wulfric-0.3.1/src/wulfric/bravais_lattice/variations.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/cell.py` & `wulfric-0.3.1/src/wulfric/cell.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/constants.py` & `wulfric-0.3.1/src/wulfric/constants.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/crystal.py` & `wulfric-0.3.1/src/wulfric/crystal.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/decorate/__init__.py` & `wulfric-0.3.1/src/wulfric/decorate/__init__.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/decorate/array.py` & `wulfric-0.3.1/src/wulfric/decorate/array.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/geometry.py` & `wulfric-0.3.1/src/wulfric/geometry.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/identify.py` & `wulfric-0.3.1/src/wulfric/identify.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/io/__init__.py` & `wulfric-0.3.1/src/wulfric/io/__init__.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/io/vasp.py` & `wulfric-0.3.1/src/wulfric/io/vasp.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/kpoints.py` & `wulfric-0.3.1/src/wulfric/kpoints.py`

 * *Files 10% similar despite different names*

```diff
@@ -445,7 +445,58 @@
         Returns
         -------
         kpoints : :py:class:`.Kpoints`
             Copy of the kpoints.
         """
 
         deepcopy(self)
+
+    ################################################################################
+    #                                Human readables                               #
+    ################################################################################
+
+    def hs_table(self, decimals=8):
+        r"""
+        High symmetry points table.
+
+        Parameters
+        ----------
+        decimals : int, optional
+            Number of decimal places to round the coordinates.
+
+        Returns
+        -------
+        table : str
+            String with N+1 lines, where N is the amount of high symmetry points.
+            Each line contains the name of the high symmetry point and its relative and
+            absolute coordinates in a reciprocal space, i.e.::
+
+                K1  0.0 0.0 0.0   0.0 0.0 0.0
+
+            First line is a header::
+
+                Name  rel_b1 rel_b2 rel_b3  k_x k_y k_z
+        """
+
+        d = decimals
+        table = [
+            (
+                f"{'Name':4}  "
+                + f"{'rel_b1':>{d+3}} "
+                + f"{'rel_b2':>{d+3}} "
+                + f"{'rel_b3':>{d+3}}  "
+                + f"{'k_x':>{d+3}} "
+                + f"{'k_y':>{d+3}} "
+                + f"{'k_z':>{d+3}}"
+            )
+        ]
+        for name in self.hs_names:
+            relative = self.hs_coordinates[name]
+            i = f"{relative[0]: {d+3}.{d}f}"
+            j = f"{relative[1]: {d+3}.{d}f}"
+            k = f"{relative[2]: {d+3}.{d}f}"
+            absolute = self.hs_coordinates[name] @ np.array([self.b1, self.b2, self.b3])
+            k_x = f"{absolute[0]: {d+3}.{d}f}"
+            k_y = f"{absolute[1]: {d+3}.{d}f}"
+            k_z = f"{absolute[2]: {d+3}.{d}f}"
+            table.append(f"{name:4}  {i} {j} {k}  {k_x} {k_y} {k_z}")
+        return "\n".join(table)
```

### Comparing `wulfric-0.3.0/src/wulfric/lattice.py` & `wulfric-0.3.1/src/wulfric/lattice.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/lattice_plotter.py` & `wulfric-0.3.1/src/wulfric/lattice_plotter.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric/numerical.py` & `wulfric-0.3.1/src/wulfric/numerical.py`

 * *Files identical despite different names*

### Comparing `wulfric-0.3.0/src/wulfric.egg-info/PKG-INFO` & `wulfric-0.3.1/src/wulfric.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wulfric
-Version: 0.3.0
+Version: 0.3.1
 Summary: Crystal, Lattice, Atoms, K-path.
 Author-email: Andrey Rybakov <rybakov.ad@icloud.com>
 License: GPL-3.0 license
 Project-URL: Homepage, https://wulfric.org
 Project-URL: Documentation, https://wulfric.org
 Project-URL: Repository, https://github.com/adrybakov/wulfric.git
 Project-URL: Issues, https://github.com/adrybakov/wulfric/issues
```

### Comparing `wulfric-0.3.0/src/wulfric.egg-info/SOURCES.txt` & `wulfric-0.3.1/src/wulfric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

