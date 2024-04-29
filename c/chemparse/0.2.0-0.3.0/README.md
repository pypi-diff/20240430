# Comparing `tmp/chemparse-0.2.0.tar.gz` & `tmp/chemparse-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemparse-0.2.0.tar", last modified: Tue Apr 16 21:43:21 2024, max compression
+gzip compressed data, was "chemparse-0.3.0.tar", last modified: Mon Apr 29 22:47:29 2024, max compression
```

## Comparing `chemparse-0.2.0.tar` & `chemparse-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2024-04-16 21:43:21.400973 chemparse-0.2.0/
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1077 2024-04-15 22:12:43.000000 chemparse-0.2.0/LICENSE.txt
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1534 2024-04-16 21:43:21.400973 chemparse-0.2.0/PKG-INFO
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1171 2024-04-15 22:18:03.000000 chemparse-0.2.0/README.md
-drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2024-04-16 21:43:21.400973 chemparse-0.2.0/chemparse/
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       30 2024-04-12 21:02:23.000000 chemparse-0.2.0/chemparse/__init__.py
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       48 2024-04-12 21:02:23.000000 chemparse-0.2.0/chemparse/__init__.pyi
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      679 2024-04-12 21:02:23.000000 chemparse-0.2.0/chemparse/exceptions.py
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      387 2024-04-12 21:02:23.000000 chemparse-0.2.0/chemparse/exceptions.pyi
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     5897 2024-04-12 21:02:23.000000 chemparse-0.2.0/chemparse/fun.py
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      584 2024-04-12 21:02:23.000000 chemparse-0.2.0/chemparse/fun.pyi
-drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2024-04-16 21:43:21.400973 chemparse-0.2.0/chemparse.egg-info/
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1534 2024-04-16 21:43:21.000000 chemparse-0.2.0/chemparse.egg-info/PKG-INFO
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      369 2024-04-16 21:43:21.000000 chemparse-0.2.0/chemparse.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        1 2024-04-16 21:43:21.000000 chemparse-0.2.0/chemparse.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        1 2024-04-16 21:43:21.000000 chemparse-0.2.0/chemparse.egg-info/not-zip-safe
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       10 2024-04-16 21:43:21.000000 chemparse-0.2.0/chemparse.egg-info/top_level.txt
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       38 2024-04-16 21:43:21.400973 chemparse-0.2.0/setup.cfg
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      705 2024-04-15 22:10:03.000000 chemparse-0.2.0/setup.py
-drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2024-04-16 21:43:21.400973 chemparse-0.2.0/test/
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1189 2024-04-12 21:02:23.000000 chemparse-0.2.0/test/test_chemparse.py
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1063 2024-04-12 21:02:23.000000 chemparse-0.2.0/test/test_exeptions.py
+drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2024-04-29 22:47:29.500927 chemparse-0.3.0/
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1077 2024-04-29 22:43:17.000000 chemparse-0.3.0/LICENSE.txt
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1675 2024-04-29 22:47:29.500927 chemparse-0.3.0/PKG-INFO
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1314 2024-04-29 22:45:56.000000 chemparse-0.3.0/README.md
+drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2024-04-29 22:47:29.500927 chemparse-0.3.0/chemparse/
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       30 2024-04-29 22:43:17.000000 chemparse-0.3.0/chemparse/__init__.py
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       48 2024-04-29 22:43:17.000000 chemparse-0.3.0/chemparse/__init__.pyi
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      679 2024-04-29 22:43:17.000000 chemparse-0.3.0/chemparse/exceptions.py
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      387 2024-04-29 22:43:17.000000 chemparse-0.3.0/chemparse/exceptions.pyi
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     5965 2024-04-29 22:43:17.000000 chemparse-0.3.0/chemparse/fun.py
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      584 2024-04-29 22:43:17.000000 chemparse-0.3.0/chemparse/fun.pyi
+drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2024-04-29 22:47:29.500927 chemparse-0.3.0/chemparse.egg-info/
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1675 2024-04-29 22:47:29.000000 chemparse-0.3.0/chemparse.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      369 2024-04-29 22:47:29.000000 chemparse-0.3.0/chemparse.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        1 2024-04-29 22:47:29.000000 chemparse-0.3.0/chemparse.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        1 2024-04-29 22:47:29.000000 chemparse-0.3.0/chemparse.egg-info/not-zip-safe
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       10 2024-04-29 22:47:29.000000 chemparse-0.3.0/chemparse.egg-info/top_level.txt
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       38 2024-04-29 22:47:29.500927 chemparse-0.3.0/setup.cfg
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      705 2024-04-29 22:43:39.000000 chemparse-0.3.0/setup.py
+drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2024-04-29 22:47:29.500927 chemparse-0.3.0/test/
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1319 2024-04-29 22:43:17.000000 chemparse-0.3.0/test/test_chemparse.py
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1063 2024-04-29 22:43:17.000000 chemparse-0.3.0/test/test_exeptions.py
```

### Comparing `chemparse-0.2.0/LICENSE.txt` & `chemparse-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chemparse-0.2.0/PKG-INFO` & `chemparse-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemparse
-Version: 0.2.0
+Version: 0.3.0
 Summary: Chemical formula parser
 Author: Grayson Boyer, Victor Ignatenko
 Author-email: gmboyer@asu.edu, vityaig@yandex.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -22,16 +22,18 @@
 * Convert a chemical formula string into a python dictionary.
     - example: `"CH4"` returns `{"C":1.0, "H":4.0}`
 * Handles fractional stoichiometry.
     - example: `"C1.5O3"` returns `{"C":1.5, "O":3.0}`
     - example: `"H2e-1O1e-1"` returns `{"H":0.2, "O":0.1}`
 * Handles groups with parentheses.
     - example: `"(CH3)2(CH2)4"` returns `{"C":6.0, "H":14.0}`
-* **New in 2024** Chemparse now handles nested paretheses!
+* **New in 2024:** Chemparse now handles nested paretheses!
     - example: `"((CH3)2)3"` returns `{'C': 6, 'H': 18}`
+* **New in 2024:** Chemparse now handles square brackets
+    - example: `"K4[Fe(SCN)6]"` returns `{'S': 6.0, 'K': 4.0, 'N': 6.0, 'C': 6.0}`
 
 ## Installation
 
 Install `chemparse` with pip:
 
 ```
 $ pip install chemparse
```

### Comparing `chemparse-0.2.0/README.md` & `chemparse-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 * Convert a chemical formula string into a python dictionary.
     - example: `"CH4"` returns `{"C":1.0, "H":4.0}`
 * Handles fractional stoichiometry.
     - example: `"C1.5O3"` returns `{"C":1.5, "O":3.0}`
     - example: `"H2e-1O1e-1"` returns `{"H":0.2, "O":0.1}`
 * Handles groups with parentheses.
     - example: `"(CH3)2(CH2)4"` returns `{"C":6.0, "H":14.0}`
-* **New in 2024** Chemparse now handles nested paretheses!
+* **New in 2024:** Chemparse now handles nested paretheses!
     - example: `"((CH3)2)3"` returns `{'C': 6, 'H': 18}`
+* **New in 2024:** Chemparse now handles square brackets
+    - example: `"K4[Fe(SCN)6]"` returns `{'S': 6.0, 'K': 4.0, 'N': 6.0, 'C': 6.0}`
 
 ## Installation
 
 Install `chemparse` with pip:
 
 ```
 $ pip install chemparse
```

### Comparing `chemparse-0.2.0/chemparse/exceptions.py` & `chemparse-0.3.0/chemparse/exceptions.py`

 * *Files identical despite different names*

### Comparing `chemparse-0.2.0/chemparse/fun.py` & `chemparse-0.3.0/chemparse/fun.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,16 @@
         ch_number += 1
 
     return position
 
 def parse_formula(text:str) -> dict[str, float]:
     
     text = str(text)
+    text = text.replace("[", "(")
+    text = text.replace("]", ")")
     
     # get indices of starting parentheses "(" and ending ")"
     open_parenth_idx_list = find_occurrences(text, "(")
     closed_parenth_idx_list = find_occurrences(text, ")")
     
     if len(open_parenth_idx_list) != len(closed_parenth_idx_list):
         raise ParenthesesMismatchError(text)
```

### Comparing `chemparse-0.2.0/chemparse/fun.pyi` & `chemparse-0.3.0/chemparse/fun.pyi`

 * *Files identical despite different names*

### Comparing `chemparse-0.2.0/chemparse.egg-info/PKG-INFO` & `chemparse-0.3.0/chemparse.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemparse
-Version: 0.2.0
+Version: 0.3.0
 Summary: Chemical formula parser
 Author: Grayson Boyer, Victor Ignatenko
 Author-email: gmboyer@asu.edu, vityaig@yandex.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -22,16 +22,18 @@
 * Convert a chemical formula string into a python dictionary.
     - example: `"CH4"` returns `{"C":1.0, "H":4.0}`
 * Handles fractional stoichiometry.
     - example: `"C1.5O3"` returns `{"C":1.5, "O":3.0}`
     - example: `"H2e-1O1e-1"` returns `{"H":0.2, "O":0.1}`
 * Handles groups with parentheses.
     - example: `"(CH3)2(CH2)4"` returns `{"C":6.0, "H":14.0}`
-* **New in 2024** Chemparse now handles nested paretheses!
+* **New in 2024:** Chemparse now handles nested paretheses!
     - example: `"((CH3)2)3"` returns `{'C': 6, 'H': 18}`
+* **New in 2024:** Chemparse now handles square brackets
+    - example: `"K4[Fe(SCN)6]"` returns `{'S': 6.0, 'K': 4.0, 'N': 6.0, 'C': 6.0}`
 
 ## Installation
 
 Install `chemparse` with pip:
 
 ```
 $ pip install chemparse
```

### Comparing `chemparse-0.2.0/setup.py` & `chemparse-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="chemparse",
-    version="0.2.0",
+    version="0.3.0",
     author="Grayson Boyer, Victor Ignatenko",
     author_email="gmboyer@asu.edu, vityaig@yandex.ru",
     description="Chemical formula parser",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={},
     packages=['chemparse'],
```

### Comparing `chemparse-0.2.0/test/test_chemparse.py` & `chemparse-0.3.0/test/test_chemparse.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
     ("((CH3)2)3",{'C': 6, 'H': 18}),
     ("(((CH3)2)3)4",{'C': 24, 'H': 72}),
     ("(Al(Ga2O)5)3",{'Al': 3, 'O': 15, 'Ga': 30}),
     ("((CH3)2)3NH3",{'C': 6, 'N': 1, 'H': 21}),
     ("(Al(Ga2O3)5)3((CH3)2)3NH3",{'O': 45, 'Al': 3, 'H': 21, 'N': 1, 'C': 6, 'Ga': 30}),
     ("(Al(Ga2O3)5)3NH3((CH3)2)3",{'O': 45, 'Al': 3, 'H': 21, 'N': 1, 'C': 6, 'Ga': 30}),
+    ("K4[Fe(SCN)6]",{'S': 6, 'K': 4, 'N': 6, 'C': 6, "Fe":1}),
+    ("K4[Fe(SCN)6]2",{'S': 12, 'K': 4, 'N': 12, 'C': 12, "Fe":2}),
 ]
 
 def test_chemparse(formula:str, expected:dict[str,int]):
     assert chemparse.parse_formula(formula) == expected
 
 def pytest_generate_tests (metafunc:pytest.Metafunc):
     metafunc.parametrize("formula,expected", species)
```

### Comparing `chemparse-0.2.0/test/test_exeptions.py` & `chemparse-0.3.0/test/test_exeptions.py`

 * *Files identical despite different names*

