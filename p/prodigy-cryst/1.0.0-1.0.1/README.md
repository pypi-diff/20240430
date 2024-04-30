# Comparing `tmp/prodigy_cryst-1.0.0.tar.gz` & `tmp/prodigy_cryst-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodigy_cryst-1.0.0.tar", max compression
+gzip compressed data, was "prodigy_cryst-1.0.1.tar", max compression
```

## Comparing `prodigy_cryst-1.0.0.tar` & `prodigy_cryst-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11375 2024-03-20 10:59:53.488442 prodigy_cryst-1.0.0/LICENSE
--rw-r--r--   0        0        0     3534 2024-04-30 15:48:33.308941 prodigy_cryst-1.0.0/README.md
--rw-r--r--   0        0        0     1065 2024-04-30 15:58:56.697929 prodigy_cryst-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 10:59:53.488442 prodigy_cryst-1.0.0/src/prodigy_cryst/__init__.py
--rwxr-xr-x   0        0        0      788 2024-03-20 10:59:53.498442 prodigy_cryst-1.0.0/src/prodigy_cryst/classify.py
--rw-r--r--   0        0        0   827201 2024-03-20 10:59:53.498442 prodigy_cryst-1.0.0/src/prodigy_cryst/data/List_of_features-MANY.csv
--rw-r--r--   0        0        0 15475492 2024-03-20 10:59:53.528443 prodigy_cryst-1.0.0/src/prodigy_cryst/data/classifier.sav
--rwxr-xr-x   0        0        0    10844 2024-04-30 15:59:58.468304 prodigy_cryst-1.0.0/src/prodigy_cryst/interface_classifier.py
--rw-r--r--   0        0        0      280 2024-03-20 10:59:53.528443 prodigy_cryst-1.0.0/src/prodigy_cryst/modules/__init__.py
--rw-r--r--   0        0        0     2857 2024-03-20 10:59:53.528443 prodigy_cryst-1.0.0/src/prodigy_cryst/modules/aa_properties.py
--rw-r--r--   0        0        0     3596 2024-03-20 10:59:53.528443 prodigy_cryst-1.0.0/src/prodigy_cryst/modules/parsers.py
--rw-r--r--   0        0        0      543 2024-03-20 10:59:53.528443 prodigy_cryst-1.0.0/src/prodigy_cryst/modules/utils.py
--rw-r--r--   0        0        0     4320 1970-01-01 00:00:00.000000 prodigy_cryst-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11375 2024-03-20 10:59:53.488442 prodigy_cryst-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1302 2024-04-30 15:21:02.710899 prodigy_cryst-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 10:59:53.488442 prodigy_cryst-1.0.1/prodigy_cryst/__init__.py
+-rwxr-xr-x   0        0        0      788 2024-03-20 10:59:53.498442 prodigy_cryst-1.0.1/prodigy_cryst/classify.py
+-rw-r--r--   0        0        0   827201 2024-03-20 10:59:53.498442 prodigy_cryst-1.0.1/prodigy_cryst/data/List_of_features-MANY.csv
+-rw-r--r--   0        0        0 15475492 2024-03-20 10:59:53.528443 prodigy_cryst-1.0.1/prodigy_cryst/data/classifier.sav
+-rwxr-xr-x   0        0        0    10834 2024-04-30 15:16:45.676602 prodigy_cryst-1.0.1/prodigy_cryst/interface_classifier.py
+-rw-r--r--   0        0        0      280 2024-03-20 10:59:53.528443 prodigy_cryst-1.0.1/prodigy_cryst/lib/__init__.py
+-rw-r--r--   0        0        0     2857 2024-03-20 10:59:53.528443 prodigy_cryst-1.0.1/prodigy_cryst/lib/aa_properties.py
+-rw-r--r--   0        0        0     3596 2024-03-20 10:59:53.528443 prodigy_cryst-1.0.1/prodigy_cryst/lib/parsers.py
+-rw-r--r--   0        0        0      543 2024-03-20 10:59:53.528443 prodigy_cryst-1.0.1/prodigy_cryst/lib/utils.py
+-rw-r--r--   0        0        0      946 2024-04-30 15:31:29.861743 prodigy_cryst-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2291 1970-01-01 00:00:00.000000 prodigy_cryst-1.0.1/PKG-INFO
```

### Comparing `prodigy_cryst-1.0.0/LICENSE` & `prodigy_cryst-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prodigy_cryst-1.0.0/pyproject.toml` & `prodigy_cryst-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 [tool.poetry]
 name = "prodigy-cryst"
-version = "1.0.0"
+version = "1.0.1"
 description = "Predicts if a protein complex interface is biological or crystallographic."
 authors = ["BonvinLab <bonvinlab.support@uu.nl>"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3.8",
   "Topic :: Scientific/Engineering :: Chemistry",
   "Topic :: Scientific/Engineering :: Bio-Informatics",
   "Intended Audience :: Science/Research",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.9"
+python = "^3.8"
 scikit-learn = "0.22"
 biopython = "^1.79"
 numpy = "~1.20"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 coverage = "^7.5.0"
 pytest-cov = "^5.0.0"
 hypothesis = "^6.100.2"
 
 [tool.poetry.scripts]
 prodigy_cryst = "prodigy_cryst.interface_classifier:main"
 
-[tool.setuptools]
-include-package-data = true
-packages = ["src"]
-
-[tool.pytest.ini_options]
-pythonpath = ["src"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `prodigy_cryst-1.0.0/src/prodigy_cryst/classify.py` & `prodigy_cryst-1.0.1/prodigy_cryst/classify.py`

 * *Files identical despite different names*

### Comparing `prodigy_cryst-1.0.0/src/prodigy_cryst/data/List_of_features-MANY.csv` & `prodigy_cryst-1.0.1/prodigy_cryst/data/List_of_features-MANY.csv`

 * *Files identical despite different names*

### Comparing `prodigy_cryst-1.0.0/src/prodigy_cryst/data/classifier.sav` & `prodigy_cryst-1.0.1/prodigy_cryst/data/classifier.sav`

 * *Files identical despite different names*

### Comparing `prodigy_cryst-1.0.0/src/prodigy_cryst/interface_classifier.py` & `prodigy_cryst-1.0.1/prodigy_cryst/interface_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 
 try:
     from Bio.PDB import NeighborSearch
 except ImportError as e:
     logging.error("[!] The interface classifier tool requires Biopython")
     raise ImportError(e)
 
-from prodigy_cryst.modules import aa_properties
-from prodigy_cryst.modules.parsers import parse_structure
+from prodigy_cryst.lib import aa_properties
+from prodigy_cryst.lib.parsers import parse_structure
 
 # from prodigy_cryst.lib.freesasa import execute_freesasa
-from prodigy_cryst.modules.utils import _check_path
+from prodigy_cryst.lib.utils import _check_path
 
 
 def calculate_ic(structure, d_cutoff=5.0, selection=None):
     """
     Calculates intermolecular contacts in a parsed structure object.
     """
     atom_list = list(structure.get_atoms())
@@ -95,15 +95,15 @@
         "THR": 0,
         "TRP": 0,
         "VAL": 0,
         "TYR": 0,
     }
 
     _data = aa_properties.aa_character_ic
-    for res_i, res_j in contact_list:
+    for (res_i, res_j) in contact_list:
         contact_type = (_data.get(res_i.resname), _data.get(res_j.resname))
         contact_type = "".join(sorted(contact_type))
         bins[contact_type] += 1
         bins[res_i.resname] += 1
         bins[res_j.resname] += 1
 
     return bins
```

### Comparing `prodigy_cryst-1.0.0/src/prodigy_cryst/modules/aa_properties.py` & `prodigy_cryst-1.0.1/prodigy_cryst/lib/aa_properties.py`

 * *Files identical despite different names*

### Comparing `prodigy_cryst-1.0.0/src/prodigy_cryst/modules/parsers.py` & `prodigy_cryst-1.0.1/prodigy_cryst/lib/parsers.py`

 * *Files identical despite different names*

### Comparing `prodigy_cryst-1.0.0/src/prodigy_cryst/modules/utils.py` & `prodigy_cryst-1.0.1/prodigy_cryst/lib/utils.py`

 * *Files identical despite different names*

