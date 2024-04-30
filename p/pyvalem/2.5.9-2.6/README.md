# Comparing `tmp/pyvalem-2.5.9.tar.gz` & `tmp/pyvalem-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvalem-2.5.9.tar", last modified: Mon Jul  4 15:58:02 2022, max compression
+gzip compressed data, was "pyvalem-2.6.tar", last modified: Tue Apr 30 13:26:26 2024, max compression
```

## Comparing `pyvalem-2.5.9.tar` & `pyvalem-2.6.tar`

### file list

```diff
@@ -1,37 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 15:58:02.472142 pyvalem-2.5.9/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-07-04 15:57:47.000000 pyvalem-2.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7680 2022-07-04 15:58:02.472142 pyvalem-2.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6564 2022-07-04 15:57:47.000000 pyvalem-2.5.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-07-04 15:57:47.000000 pyvalem-2.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-07-04 15:58:02.472142 pyvalem-2.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-07-04 15:57:47.000000 pyvalem-2.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 15:58:02.468142 pyvalem-2.5.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 15:58:02.472142 pyvalem-2.5.9/src/pyvalem/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5832 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/_data_atomic_weights.txt
--rw-r--r--   0 runner    (1001) docker     (121)   158055 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/_data_isotope_masses.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/_special_cases.py
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6432 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/atom_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    23560 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/formula.py
--rw-r--r--   0 runner    (1001) docker     (121)    15666 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/reaction.py
--rw-r--r--   0 runner    (1001) docker     (121)     5415 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/stateful_species.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 15:58:02.472142 pyvalem-2.5.9/src/pyvalem/states/
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/_base_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     1884 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/_state_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    10410 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/atomic_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     3247 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/atomic_term_symbol.py
--rw-r--r--   0 runner    (1001) docker     (121)     8354 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/diatomic_molecular_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/generic_excited_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/key_value_pair.py
--rw-r--r--   0 runner    (1001) docker     (121)     6843 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/molecular_term_symbol.py
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/racah_symbol.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/rotational_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     3156 2022-07-04 15:57:47.000000 pyvalem-2.5.9/src/pyvalem/states/vibrational_state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 15:58:02.472142 pyvalem-2.5.9/src/pyvalem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7680 2022-07-04 15:58:02.000000 pyvalem-2.5.9/src/pyvalem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      959 2022-07-04 15:58:02.000000 pyvalem-2.5.9/src/pyvalem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-04 15:58:02.000000 pyvalem-2.5.9/src/pyvalem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-07-04 15:58:02.000000 pyvalem-2.5.9/src/pyvalem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-04 15:58:02.000000 pyvalem-2.5.9/src/pyvalem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:26:26.362577 pyvalem-2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-30 13:26:15.000000 pyvalem-2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8128 2024-04-30 13:26:26.362577 pyvalem-2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-30 13:26:15.000000 pyvalem-2.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-30 13:26:15.000000 pyvalem-2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-30 13:26:26.362577 pyvalem-2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-30 13:26:15.000000 pyvalem-2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:26:26.354577 pyvalem-2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:26:26.354577 pyvalem-2.6/src/pyvalem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/_data_atomic_weights.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   158055 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/_data_isotope_masses.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/_special_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/atom_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23660 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15666 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/stateful_species.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:26:26.358577 pyvalem-2.6/src/pyvalem/states/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/_base_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/_state_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/atomic_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/atomic_term_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/compound_LS_coupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/diatomic_molecular_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/generic_excited_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/key_value_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/molecular_term_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/racah_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/rotational_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/vibrational_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:26:26.362577 pyvalem-2.6/src/pyvalem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8128 2024-04-30 13:26:26.000000 pyvalem-2.6/src/pyvalem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-30 13:26:26.000000 pyvalem-2.6/src/pyvalem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:26:26.000000 pyvalem-2.6/src/pyvalem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 13:26:26.000000 pyvalem-2.6/src/pyvalem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 13:26:26.000000 pyvalem-2.6/src/pyvalem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:26:26.362577 pyvalem-2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_atomic_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_atomic_term_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_atoms_isotopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_compound_LS_coupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_diatomic_molecular_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_generic_excited_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_key_value_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_molecular_term_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_racah_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_rotational_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_stateful_species.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_vibrational_state.py
```

### Comparing `pyvalem-2.5.9/LICENSE` & `pyvalem-2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.9/PKG-INFO` & `pyvalem-2.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvalem
-Version: 2.5.9
+Version: 2.6
 Summary: A package for managing simple chemical species and states
 Home-page: https://github.com/xnx/pyvalem
 Author: Christian Hill
 Author-email: ch.hill@iaea.org
 Project-URL: Bug Reports, https://github.com/xnx/pyvalem/issues
 Keywords: chemistry,formula,species,state,reaction
 Classifier: Development Status :: 4 - Beta
@@ -14,20 +14,29 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: pyparsing>=2.3
+Requires-Dist: importlib-resources>=1.0; python_version < "3.7.0"
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: ipython; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
 
 |Tests action| |GitHub license| |PyPI version| |PyPI pyversions| |Code style|
 
 .. |Tests action| image:: https://github.com/xnx/pyvalem/workflows/tests/badge.svg
    :target: https://github.com/xnx/pyvalem/actions
 .. |GitHub license| image:: https://img.shields.io/github/license/xnx/pyvalem.svg
    :target: https://github.com/xnx/pyvalem/blob/master/LICENSE
@@ -214,14 +223,20 @@
 After cloning or forking the project from its GitHub_ page, ``pyvalem`` might be
 installed into the virtual environment in editable mode with
 
 .. code-block:: bash
 
     pip install -e .[dev]
 
+or on zsh:
+
+.. code-block:: zsh
+
+   pip install -e .'[dev]'
+
 The ``[dev]`` extra installs (apart from the package dependencies) also several
 development-related packages, such as ``pytest``, ``black``, ``tox`` or ``ipython.``
 The tests can then be executed by running (from the project root directory)
 
 .. code-block:: bash
 
     # either
```

### Comparing `pyvalem-2.5.9/README.rst` & `pyvalem-2.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,20 @@
 After cloning or forking the project from its GitHub_ page, ``pyvalem`` might be
 installed into the virtual environment in editable mode with
 
 .. code-block:: bash
 
     pip install -e .[dev]
 
+or on zsh:
+
+.. code-block:: zsh
+
+   pip install -e .'[dev]'
+
 The ``[dev]`` extra installs (apart from the package dependencies) also several
 development-related packages, such as ``pytest``, ``black``, ``tox`` or ``ipython.``
 The tests can then be executed by running (from the project root directory)
 
 .. code-block:: bash
 
     # either
```

### Comparing `pyvalem-2.5.9/pyproject.toml` & `pyvalem-2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,11 +18,11 @@
     pp_h: pyparsing
     ir_l: importlib-resources==1.0
     ir_h: importlib-resources
 commands = pytest
 """
 
 [tool.coverage.run]
-omit = ["tests/*", "src/pyvalem/__init__.py", "doc/*"]
+omit = ["tests/*", "src/pyvalem/__init__.py", "docs/*"]
 
 [tool.coverage.html]
 directory = "htmlcov"
```

### Comparing `pyvalem-2.5.9/setup.py` & `pyvalem-2.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 root = Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (root / "README.rst").read_text(encoding="utf-8")
 
 setup(
     name="pyvalem",
-    version="2.5.9",
+    version="2.6",
     description="A package for managing simple chemical species and states",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/xnx/pyvalem",
     author="Christian Hill",
     author_email="ch.hill@iaea.org",
     classifiers=[
@@ -23,26 +23,28 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Operating System :: OS Independent",
     ],
     keywords="chemistry, formula, species, state, reaction",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     python_requires=">=3.6",
     install_requires=[
         "pyparsing>=2.3",
         'importlib-resources>=1.0; python_version < "3.7.0"',
     ],
-    extras_require={"dev": ["black", "pytest-cov", "tox", "ipython"]},
+    extras_require={"dev": ["black", "pytest-cov", "tox", "ipython", "sphinx"]},
     # package_data will include all the resolved globs into both the wheel and sdist
     package_data={"pyvalem": ["*.txt"]},
     # no need for MANIFEST.in, which should be reserved only for build-time files
     project_urls={
         "Bug Reports": "https://github.com/xnx/pyvalem/issues",
     },
 )
```

### Comparing `pyvalem-2.5.9/src/pyvalem/_data_atomic_weights.txt` & `pyvalem-2.6/src/pyvalem/_data_atomic_weights.txt`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.9/src/pyvalem/_data_isotope_masses.txt` & `pyvalem-2.6/src/pyvalem/_data_isotope_masses.txt`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.9/src/pyvalem/_special_cases.py` & `pyvalem-2.6/src/pyvalem/_special_cases.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.9/src/pyvalem/_utils.py` & `pyvalem-2.6/src/pyvalem/_utils.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.9/src/pyvalem/atom_data.py` & `pyvalem-2.6/src/pyvalem/atom_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,22 +34,25 @@
 
 >>> ar_isotope = isotopes["38Ar"]
 >>> ar_isotope.A, ar_isotope.N
 (38, 20)
 """
 
 import csv
+import platform
 
 try:
     import importlib.resources as pkg_resources
 except ImportError:
     # for python < 3.7, use the importlib-resources backport
     # noinspection PyUnresolvedReferences
     import importlib_resources as pkg_resources
 
+PYTHON3_VERSION = int(platform.python_version_tuple()[1])
+
 
 class Atom:
     """Class representing an atom instance.
 
     All the parameters are stored as instance attributes.
     The `Atom` instances are hashable.
 
@@ -168,42 +171,59 @@
     """
     try:
         return float(f)
     except ValueError:
         return None
 
 
-# list of all the element symbols recognised by pyvalem:
-element_symbols = []
-# pre-built mapping between element symbols and Atom instances:
-atoms = {}
-# Atom data is from Meija et al., "Atomic weights of the elements 2013
-# (IUPAC Technical Report)", Pure Appl. Chem. 88(3), 265-291, 2016.
-# See https://ciaaw.org/atomic-weights.htm
-with pkg_resources.open_text("pyvalem", "_data_atomic_weights.txt") as fi:
+def read_atom_data(fi, atoms):
+    """
+    Read atom data from open file handle fi into dictionary atoms, keyed by
+    element symbol.
+    """
+
     reader = csv.reader(fi, delimiter=",")
     header = ["Symbol", "Name", "Z", "atomic_weight", "atomic_weight_unc"]
     for row in reader:
         row = [val.strip() for val in row]
         if row == header:
             continue  # skip the header
         atom_dtypes = [str, str, int, float_or_none, float_or_none]
         atom_args = [dtype(val) for dtype, val in zip(atom_dtypes, row)]
         element_symbol = atom_args[0]
         element_symbols.append(element_symbol)
         atoms[element_symbol] = Atom(*atom_args)
+    return atoms
+
+
+# list of all the element symbols recognised by pyvalem:
+element_symbols = []
+# pre-built mapping between element symbols and Atom instances:
+atoms = {}
+# Atom data is from Meija et al., "Atomic weights of the elements 2013
+# (IUPAC Technical Report)", Pure Appl. Chem. 88(3), 265-291, 2016.
+# See https://ciaaw.org/atomic-weights.htm
+if PYTHON3_VERSION < 9:
+    # NB Python 3.8 and below use open_text:
+    with pkg_resources.open_text("pyvalem", "_data_atomic_weights.txt") as fi:
+        read_atom_data(fi, atoms)
+else:
+    # NB Python 3.9 and above use importlib.resources.files:
+    with pkg_resources.files("pyvalem").joinpath("_data_atomic_weights.txt").open(
+        "r", encoding="utf8"
+    ) as fi:
+        read_atom_data(fi, atoms)
+
+
+def read_isotope_data(fi, isotopes):
+    """
+    Read in isotope mass data from open file handle fi into dictionary isotopes,
+    keyed by isotope symbol (e.g. "46Ti").
+    """
 
-# pre-built mapping between element isotopic symbols and Isotope instances:
-isotopes = {}
-# Isotope data is from the AME2016 Atomic Mass Evaluation reports,
-# Huang et al., "The Ame2016 atomic mass evaluation (I)", Chinese Physics C41,
-# 030002 (2017); Wang et al., "The Ame2016 atomic mass evaluation (II)",
-# Chinese Physics C41, 030003 (2017).
-# See http://amdc.impcas.ac.cn/masstables/Ame2016/mass16.txt
-with pkg_resources.open_text("pyvalem", "_data_isotope_masses.txt") as fi:
     reader = csv.reader(fi, delimiter=",")
     header = ["Z", "A", "Symbol", "mass", "mass_unc", "estimated_flag"]
     iso_attribs = [
         "atomic_number",
         "mass_number",
         "symbol",
         "mass",
@@ -221,7 +241,26 @@
         iso_name = "{}-{}".format(
             atoms[iso_kwargs["symbol"]].name, iso_kwargs["mass_number"]
         )
         iso_kwargs["name"] = iso_name
         iso_symbol = "{:d}{:s}".format(iso_kwargs["mass_number"], iso_kwargs["symbol"])
         iso_kwargs["symbol"] = iso_symbol
         isotopes[iso_symbol] = Isotope(**iso_kwargs)
+
+
+# pre-built mapping between element isotopic symbols and Isotope instances:
+isotopes = {}
+# Isotope data is from the AME2016 Atomic Mass Evaluation reports,
+# Huang et al., "The Ame2016 atomic mass evaluation (I)", Chinese Physics C41,
+# 030002 (2017); Wang et al., "The Ame2016 atomic mass evaluation (II)",
+# Chinese Physics C41, 030003 (2017).
+# See http://amdc.impcas.ac.cn/masstables/Ame2016/mass16.txt
+if PYTHON3_VERSION < 9:
+    # NB Python 3.8 and below use open_text:
+    with pkg_resources.open_text("pyvalem", "_data_isotope_masses.txt") as fi:
+        read_isotope_data(fi, isotopes)
+else:
+    # NB Python 3.9 and above use importlib.resources.files:
+    with pkg_resources.files("pyvalem").joinpath("_data_isotope_masses.txt").open(
+        "r", encoding="utf8"
+    ) as fi:
+        read_isotope_data(fi, isotopes)
```

### Comparing `pyvalem-2.5.9/src/pyvalem/formula.py` & `pyvalem-2.6/src/pyvalem/formula.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,17 +196,18 @@
     Raises
     ------
     FormulaParseError
         When an incompatible `formula` string is passed into the constructor
 
     Notes
     -----
-    The ``__repr__`` method is overloaded to provide a *canonicalised* representation
-    of the formula. The idea is that two formulas representing the same physical entity
-    will have the same ``repr(formula)`` representation.
+    The ``__repr__`` method is intended to be a *canonicalised* representation
+    of the formula, but no check is made to ensure that a single formula is used
+    to describe a unique species (e.g. "HD" and "DH" and "H(2H)" all have
+    different __repr__ representations.
 
     Examples
     --------
     >>> Formula("H2+")  # a simple chemical formula instantiation
     H2+
 
     >>> Formula("(1H)2(16O)")  # isotopologue instantiation
@@ -317,14 +318,18 @@
         # We make a particular exception for various special cases, including
         # photons, electrons, positrons and "M", denoting an unspecified
         # "third-body" in many reactions. Note that M does not have a defined
         # charge or mass.
         if formula == "e":
             # Quietly convert e to e-.
             self.formula = formula = "e-"
+
+        if self.formula == "hv":
+            self.formula = "hν"
+
         if formula in special_cases:
             for attr, val in special_cases[formula].items():
                 setattr(self, attr, val)
             return
 
         try:
             moieties = complexChemicalFormula.parseString(formula)
@@ -502,20 +507,21 @@
             moiety_charge_slug = "_{:s}{:s}".format(
                 slug_charge_sign[s_charge_sign], s_charge
             )
             return moiety_charge_html, moiety_charge_latex, moiety_charge_slug
         return "", "", ""
 
     def __repr__(self):
-        if self.formula == "hv":
-            return "hν"
         return self.formula
 
+    def __hash__(self):
+        return hash(self.formula)
+
     def __eq__(self, other):
-        return repr(self.formula) == repr(other.formula)
+        return self.formula == other.formula
 
     def _stoichiometric_formula_atomic_number(self):
         """Return a list of atoms/isotopes and their stoichiometries.
 
         The returned list is sorted in order of increasing atomic number.
         """
```

### Comparing `pyvalem-2.5.9/src/pyvalem/reaction.py` & `pyvalem-2.6/src/pyvalem/reaction.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.9/src/pyvalem/stateful_species.py` & `pyvalem-2.6/src/pyvalem/stateful_species.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.9/src/pyvalem/states/__init__.py` & `pyvalem-2.6/src/pyvalem/states/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.9/src/pyvalem/states/_base_state.py` & `pyvalem-2.6/src/pyvalem/states/_base_state.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.9/src/pyvalem/states/_state_parser.py` & `pyvalem-2.6/src/pyvalem/states/_state_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 from .diatomic_molecular_configuration import DiatomicMolecularConfiguration
 from .generic_excited_state import GenericExcitedState
 from .key_value_pair import KeyValuePair
 from .molecular_term_symbol import MolecularTermSymbol
 from .racah_symbol import RacahSymbol
 from .rotational_state import RotationalState
 from .vibrational_state import VibrationalState
+from .compound_LS_coupling import CompoundLSCoupling
 
 # the following has two purposes: keys determine the order in which the
 # states are parsed, and the values determine the sorting order of states
 # for StatefulSpecies.__repr__.
 STATES = OrderedDict(
     [
         (GenericExcitedState, 0),
         (AtomicConfiguration, 1),
+        (CompoundLSCoupling, 1),
         (AtomicTermSymbol, 2),
         (DiatomicMolecularConfiguration, 1),
         (MolecularTermSymbol, 2),
         (VibrationalState, 3),
         (RotationalState, 4),
         (RacahSymbol, 5),
         (KeyValuePair, 6),
```

### Comparing `pyvalem-2.5.9/src/pyvalem/states/atomic_configuration.py` & `pyvalem-2.6/src/pyvalem/states/atomic_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,30 @@
 integer = pp.Word(pp.nums).setParseAction(lambda t: int(t[0]))
 nocc_integer = pp.Optional(pp.Word(pp.nums), default="1").setParseAction(
     lambda t: int(t[0])
 )
 
 # NB no "j" orbital.
 atomic_orbital_symbols = tuple("spdfghiklmnoqrtuvwxyz")
+
 noble_gases = ["He", "Ne", "Ar", "Kr", "Xe", "Rn"]
 noble_gas_configs = {
     "He": "1s2",
     "Ne": "[He].2s2.2p6",
     "Ar": "[Ne].3s2.3p6",
     "Kr": "[Ar].3d10.4s2.4p6",
     "Xe": "[Kr].4d10.5s2.5p6",
     "Rn": "[Xe].4f14.5d10.6s2.6p6",
 }
+# Expand out the noble gas configurations to explicitly list all orbitals.
+for i, elm in enumerate(noble_gases[1:], start=1):
+    s = noble_gases[i - 1]
+    c = noble_gas_configs[s]
+    noble_gas_configs[elm] = noble_gas_configs[elm].replace(f"[{s}]", c)
+
 noble_gas_nelectrons = {"He": 2, "Ne": 10, "Ar": 18, "Kr": 36, "Xe": 54, "Rn": 86}
 
 noble_gas = pp.oneOf(["[{}]".format(symbol) for symbol in noble_gases])
 
 atom_orbital = pp.Group(
     integer.setResultsName("n")
     + pp.oneOf(atomic_orbital_symbols).setResultsName("lletter")
@@ -219,19 +226,19 @@
 
     >>> ac2 = AtomicConfiguration("[Ne].3p")
     >>> repr(ac2)
     '1s2.2s2.2p6.3p'
     """
 
     def __init__(self, state_str):
-        self.state_str = state_str
+        self.state_str = self._contract_to_noble_gas_config(state_str)
         self.orbitals = []
         self.noble_gas_config = None
         self.nelectrons = 0
-        self._parse_state(state_str)
+        self._parse_state(self.state_str)
 
     def _parse_state(self, state_str):
         """Parses the `AtomicConfiguration` instance from the supplied `state_str`.
 
         Parameters
         ----------
         state_str : str
@@ -294,15 +301,15 @@
         if self.noble_gas_config:
             latex_chunks.append(r"\mathrm{{{}}}".format(self.noble_gas_config))
         for orbital in self.orbitals:
             latex_chunks.append(orbital.latex)
         return "".join(latex_chunks)
 
     def _expand_noble_gas_config(self, config):
-        """Recursively expand out the noble gas notation to orbitals.
+        """Expand out the noble gas notation to orbitals.
 
         For example:
         '[He].2s1' -> '1s2.2s2',
         '[Xe].4f7' -> '1s2.2s2.2p6.3s2.3p6.3d10.4s2.4p6.4d10.5s2.5p6.4f7'
 
         Parameters
         ----------
@@ -312,20 +319,26 @@
         Returns
         -------
         str
         """
 
         if config[0] != "[":
             return config
-        return (
-            self._expand_noble_gas_config(noble_gas_configs[config[1:3]]) + config[4:]
-        )
+        return noble_gas_configs[config[1:3]] + config[4:]
+
+    def _contract_to_noble_gas_config(self, state_str):
+        """Replace explicit atomic orbital sequence with noble gas notation."""
+        for noble_gas in noble_gases[:1:-1]:
+            config = noble_gas_configs[noble_gas]
+            if config in state_str:
+                state_str = state_str.replace(config, f"[{noble_gas}]")
+        return state_str
 
     def __repr__(self):
         """See the `State` base class."""
         if self.noble_gas_config:
-            state_repr = self._expand_noble_gas_config(self.noble_gas_config)
+            state_repr = noble_gas_configs[self.noble_gas_config[1:3]]
             if self.orbitals:
                 state_repr += "." + ".".join(repr(orbital) for orbital in self.orbitals)
             return state_repr
         else:
             return ".".join(repr(orbital) for orbital in self.orbitals)
```

### Comparing `pyvalem-2.5.9/src/pyvalem/states/atomic_term_symbol.py` & `pyvalem-2.6/src/pyvalem/states/rotational_state.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,76 @@
 """
-The AtomicTermSymbol class, representing an atomic term symbol, with
-methods for parsing a string into quantum numbers and labels, creating
-an HTML representation of the term symbol, etc.
+The RotationalState class, representing a rotational quantum number, with
+methods for parsing a string into a value and an HTML representation, etc.
 """
 
 import pyparsing as pp
 
 from pyvalem.states._base_state import State, StateParseError
-from pyvalem._utils import parse_fraction, float_to_fraction
-
-atom_L_symbols = "S P D F G H I K L M N O Q R T U V W X Y Z".split()
 
 integer = pp.Word(pp.nums)
+integer_string = (integer + pp.StringEnd()).setResultsName("integer")
+frac_string = (
+    integer + pp.Suppress("/") + pp.Suppress(pp.Literal("2")) + pp.StringEnd()
+).setResultsName("fraction_half")
+decimal_string = (
+    integer + pp.Suppress(".") + pp.Suppress(pp.Literal("5")) + pp.StringEnd()
+).setResultsName("decimal_half")
 
-atom_Smult = integer.setResultsName("Smult")
-atom_Lletter = pp.oneOf(atom_L_symbols).setResultsName("Lletter")
-atom_Jstr = (
-    integer + pp.Optional(pp.Suppress("/") + "2") + pp.StringEnd()
-).setResultsName("Jstr")
-atom_parity = pp.Literal("o").setResultsName("parity")
-atom_term = (
-    atom_Smult
-    + atom_Lletter
-    + pp.Optional(atom_parity)
-    + pp.Optional(pp.Suppress("_") + atom_Jstr)
-    + pp.StringEnd()
-)
+Jstr = integer_string | frac_string | decimal_string
 
 
-class AtomicTermSymbolError(StateParseError):
+class RotationalStateError(StateParseError):
     pass
 
 
-class AtomicTermSymbol(State):
+class RotationalState(State):
     def __init__(self, state_str):
-        self.state_str = state_str
-        self.Smult = None
-        self.S = None
-        self.Lletter = None
-        self.L = None
-        self.parity = None
+        self.state_str = None
         self.J = None
         self._parse_state(state_str)
 
     def _parse_state(self, state_str):
         try:
-            components = atom_term.parseString(state_str)
-        except pp.ParseException:
-            raise AtomicTermSymbolError(
-                "Invalid atomic term symbol syntax:" " {0}".format(state_str)
-            )
-        self.Smult = int(components.Smult)
-        self.S = (self.Smult - 1) / 2.0
-        self.Lletter = components.Lletter
-        self.L = atom_L_symbols.index(components.Lletter)
-        self.parity = components.get("parity")
-        try:
-            self.J = parse_fraction(components.Jstr)
-        except ValueError as err:
-            raise AtomicTermSymbolError(err)
-        if self.J is not None:
-            self._validate_j()
+            k, v = state_str.split("=")
+            if k.strip() != "J":
+                raise ValueError
+        except ValueError:
+            raise RotationalStateError("Rotational states must start with" ' "J="')
+
+        state_str = v.strip()
+
+        self.J = None
+        if state_str not in ("*", "**", "***"):
+            try:
+                components = Jstr.parseString(state_str)
+            except pp.ParseException:
+                raise RotationalStateError(
+                    "Invalid rotational state value" " syntax: {0}".format(state_str)
+                )
+
+            if "integer" in components:
+                self.J = int(components["integer"][0])
+            elif "fraction_half" in components:
+                self.J = int(components["fraction_half"][0]) / 2
+            elif "decimal_half" in components:
+                self.J = float(components["decimal_half"][0]) + 0.5
+                state_str = "{}/2".format(int(2 * self.J))
+            else:
+                raise RotationalStateError(
+                    "Invalid rotational state value" " syntax: {0}".format(state_str)
+                )
+
+            if self.J is not None:
+                self._validate_j()
+
+        self.state_str = "J={}".format(state_str)
 
     def _validate_j(self):
-        s_is_half_integer = int(2 * self.S) % 2
-        j_is_half_integer = int(2 * self.J) % 2
-        if s_is_half_integer != j_is_half_integer:
-            raise AtomicTermSymbolError(
-                "J={} is invalid for S={}.".format(self.J, self.S)
+        if self.J % 0.5 != 0:
+            raise RotationalStateError(
+                "Invalid rotational state value: {}."
+                "Must be a multiple of 1/2.".format(self.state_str)
             )
-        if not abs(self.L - self.S) <= self.J <= self.L + self.S:
-            raise AtomicTermSymbolError(
-                "Invalid atomic term symbol: {0:s}"
-                " |L-S| <= J <= L+S must be satisfied.".format(self.state_str)
-            )
-
-    @property
-    def html(self):
-        html_chunks = ["<sup>{0:d}</sup>{1:s}".format(self.Smult, self.Lletter)]
-        if self.parity:
-            html_chunks.append("<sup>o</sup>")
-        if self.J is not None:
-            j_str = float_to_fraction(self.J)
-            html_chunks.append("<sub>{0:s}</sub>".format(j_str))
-        return "".join(html_chunks)
-
-    @property
-    def latex(self):
-        latex_chunks = ["{{}}^{{{}}}\mathrm{{{}}}".format(self.Smult, self.Lletter)]
-        if self.parity:
-            latex_chunks.append("^o")
-        if self.J is not None:
-            j_str = float_to_fraction(self.J)
-            latex_chunks.append("_{{{}}}".format(j_str))
-        return "".join(latex_chunks)
 
     def __repr__(self):
         return self.state_str
```

### Comparing `pyvalem-2.5.9/src/pyvalem/states/diatomic_molecular_configuration.py` & `pyvalem-2.6/src/pyvalem/states/diatomic_molecular_configuration.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.9/src/pyvalem/states/generic_excited_state.py` & `pyvalem-2.6/src/pyvalem/states/generic_excited_state.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.9/src/pyvalem/states/key_value_pair.py` & `pyvalem-2.6/src/pyvalem/states/key_value_pair.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.9/src/pyvalem/states/molecular_term_symbol.py` & `pyvalem-2.6/src/pyvalem/states/molecular_term_symbol.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,14 @@
         self.S = None
         self.irrep = None
         self.term_label = None
         self.Omega = None
         self._parse_state(state_str)
 
     def _parse_state(self, state_str):
-
         try:
             components = molecule_term_with_label.parseString(state_str)
         except pp.ParseException:
             raise MolecularTermSymbolError(
                 "Invalid molecular term symbol syntax: {0}".format(state_str)
             )
         self.Smult = int(components.Smult)
```

### Comparing `pyvalem-2.5.9/src/pyvalem/states/racah_symbol.py` & `pyvalem-2.6/src/pyvalem/states/racah_symbol.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,48 +9,52 @@
 from pyvalem.states._base_state import State, StateParseError
 
 integer = pp.Word(pp.nums)
 atom_principal = integer.setResultsName("principal")
 
 orbital_labels = ("s", "s'", "p", "p'", "d", "d'", "f", "f'")
 atom_orbital = pp.oneOf(orbital_labels).setResultsName("orbital")
+parity_label = pp.Literal("o").setResultsName("parity")
 
 atom_k_term = (
     integer.setResultsName("k_num") + pp.Suppress("/") + integer.setResultsName("k_den")
 )
 
 atom_j_term = integer.setResultsName("jterm")
 
 racah_symbol_template = (
     atom_principal
     + atom_orbital
     + pp.Suppress("[")
     + atom_k_term
-    + pp.Suppress("]_")
-    + atom_j_term
+    + pp.Suppress("]")
+    + pp.Optional(parity_label)
+    + pp.Optional("_" + atom_j_term)
 )
 
 
 class RacahSymbol(State):
     """
     The RacahSymbol class representing an atomic state in Racah notation.
 
     This class is currently little more than a stub. The term symbol of the
     parent configuration must be specified as a separate State; this class
-    defines nl[K]_J, without the parity label ("superscript-o").
+    defines nl[K]_J, where _J is optional to allow for the case where a
+    state is an average over J levels.
     """
 
     def __init__(self, state_str):
         self.state_str = state_str
         self.principal = None
         self.orbital = None
         self.parent_rot = None
         self.k_num = None
         self.k_den = None
         self.j_term = None
+        self.parity = None
         self._parse_state(state_str)
 
     def _parse_state(self, state_str):
         try:
             components = racah_symbol_template.parseString(state_str)
         except pp.ParseException:
             raise StateParseError("Invalid Racah notation syntax: {}".format(state_str))
@@ -58,19 +62,24 @@
         self.orbital = components.orbital
         if "'" in self.orbital:
             self.parent_rot = 0.5
         else:
             self.parent_rot = 1.5
         self.k_num = int(components.k_num)
         self.k_den = int(components.k_den)
-        self.j_term = int(components.jterm)
+        self.parity = "o" if components.parity else ""
+        if components.jterm != "":
+            self.j_term = int(components.jterm)
 
     def __repr__(self):
-        parent = "{}{}".format(self.principal, self.orbital)
-        k = "{}/{}".format(self.k_num, self.k_den)
-        return "{}[{}]_{}".format(parent, k, self.j_term)
+        parent = f"{self.principal}{self.orbital}"
+        k = f"{self.k_num}/{self.k_den}"
+        s_jterm = f"_{self.j_term}" if self.j_term is not None else ""
+        return f"{parent}[{k}]{self.parity}{s_jterm}"
 
     @property
     def html(self):
-        parent = "{}{}".format(self.principal, self.orbital)
-        k = "{}/{}".format(self.k_num, self.k_den)
-        return "{}[{}]<sub>{}</sub>".format(parent, k, self.j_term)
+        parent = f"{self.principal}{self.orbital}"
+        k = f"{self.k_num}/{self.k_den}"
+        s_parity = "<sup>o</sup>" if self.parity else ""
+        s_jterm = f"<sub>{self.j_term}</sub>" if self.j_term is not None else ""
+        return f"{parent}[{k}]{s_parity}{s_jterm}"
```

### Comparing `pyvalem-2.5.9/src/pyvalem/states/vibrational_state.py` & `pyvalem-2.6/src/pyvalem/states/vibrational_state.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.5.9/src/pyvalem.egg-info/PKG-INFO` & `pyvalem-2.6/src/pyvalem.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvalem
-Version: 2.5.9
+Version: 2.6
 Summary: A package for managing simple chemical species and states
 Home-page: https://github.com/xnx/pyvalem
 Author: Christian Hill
 Author-email: ch.hill@iaea.org
 Project-URL: Bug Reports, https://github.com/xnx/pyvalem/issues
 Keywords: chemistry,formula,species,state,reaction
 Classifier: Development Status :: 4 - Beta
@@ -14,20 +14,29 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: pyparsing>=2.3
+Requires-Dist: importlib-resources>=1.0; python_version < "3.7.0"
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: ipython; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
 
 |Tests action| |GitHub license| |PyPI version| |PyPI pyversions| |Code style|
 
 .. |Tests action| image:: https://github.com/xnx/pyvalem/workflows/tests/badge.svg
    :target: https://github.com/xnx/pyvalem/actions
 .. |GitHub license| image:: https://img.shields.io/github/license/xnx/pyvalem.svg
    :target: https://github.com/xnx/pyvalem/blob/master/LICENSE
@@ -214,14 +223,20 @@
 After cloning or forking the project from its GitHub_ page, ``pyvalem`` might be
 installed into the virtual environment in editable mode with
 
 .. code-block:: bash
 
     pip install -e .[dev]
 
+or on zsh:
+
+.. code-block:: zsh
+
+   pip install -e .'[dev]'
+
 The ``[dev]`` extra installs (apart from the package dependencies) also several
 development-related packages, such as ``pytest``, ``black``, ``tox`` or ``ipython.``
 The tests can then be executed by running (from the project root directory)
 
 .. code-block:: bash
 
     # either
```

