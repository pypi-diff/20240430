# Comparing `tmp/dccquantities-1.4.2.tar.gz` & `tmp/dccquantities-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dccquantities-1.4.2.tar", last modified: Tue Apr 30 09:35:32 2024, max compression
+gzip compressed data, was "dccquantities-1.4.3.tar", last modified: Tue Apr 30 09:52:02 2024, max compression
```

## Comparing `dccquantities-1.4.2.tar` & `dccquantities-1.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-30 09:35:32.606084 dccquantities-1.4.2/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    26516 2024-04-29 13:28:01.000000 dccquantities-1.4.2/LICENSE
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)     1939 2024-04-30 09:35:32.606084 dccquantities-1.4.2/PKG-INFO
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)     1129 2024-04-30 07:44:37.000000 dccquantities-1.4.2/README.md
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)       80 2023-10-04 11:27:28.000000 dccquantities-1.4.2/pyproject.toml
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)      633 2024-04-30 09:35:32.606084 dccquantities-1.4.2/setup.cfg
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-30 09:35:32.605084 dccquantities-1.4.2/src/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)        0 2024-04-29 13:28:01.000000 dccquantities-1.4.2/src/__init__.py
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-30 09:35:32.605084 dccquantities-1.4.2/src/dccQuantities.egg-info/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)     1939 2024-04-30 09:35:32.000000 dccquantities-1.4.2/src/dccQuantities.egg-info/PKG-INFO
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)      398 2024-04-30 09:35:32.000000 dccquantities-1.4.2/src/dccQuantities.egg-info/SOURCES.txt
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)        1 2024-04-30 09:35:32.000000 dccquantities-1.4.2/src/dccQuantities.egg-info/dependency_links.txt
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)      162 2024-04-30 09:35:32.000000 dccquantities-1.4.2/src/dccQuantities.egg-info/requires.txt
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)       68 2024-04-30 09:35:32.000000 dccquantities-1.4.2/src/dccQuantities.egg-info/top_level.txt
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    68641 2024-04-30 09:34:03.000000 dccquantities-1.4.2/src/dccQuantities.py
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)     1931 2024-04-30 07:43:13.000000 dccquantities-1.4.2/src/dccQuantitiesConfiguration.py
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    12053 2024-04-30 08:34:28.000000 dccquantities-1.4.2/src/dccQuantitiesPlot.py
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-30 09:35:32.605084 dccquantities-1.4.2/tests/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    17747 2024-04-30 09:11:52.000000 dccquantities-1.4.2/tests/test_dccQuantsAndTabs.py
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)     2393 2024-04-30 07:43:13.000000 dccquantities-1.4.2/tests/test_tollerance.py
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-30 09:52:02.955029 dccquantities-1.4.3/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    26516 2024-04-29 13:28:01.000000 dccquantities-1.4.3/LICENSE
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)     1939 2024-04-30 09:52:02.955029 dccquantities-1.4.3/PKG-INFO
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)     1129 2024-04-30 07:44:37.000000 dccquantities-1.4.3/README.md
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)       80 2023-10-04 11:27:28.000000 dccquantities-1.4.3/pyproject.toml
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)      633 2024-04-30 09:52:02.955029 dccquantities-1.4.3/setup.cfg
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-30 09:52:02.954029 dccquantities-1.4.3/src/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)        0 2024-04-29 13:28:01.000000 dccquantities-1.4.3/src/__init__.py
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-30 09:52:02.954029 dccquantities-1.4.3/src/dccQuantities.egg-info/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)     1939 2024-04-30 09:52:02.000000 dccquantities-1.4.3/src/dccQuantities.egg-info/PKG-INFO
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)      398 2024-04-30 09:52:02.000000 dccquantities-1.4.3/src/dccQuantities.egg-info/SOURCES.txt
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)        1 2024-04-30 09:52:02.000000 dccquantities-1.4.3/src/dccQuantities.egg-info/dependency_links.txt
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)      162 2024-04-30 09:52:02.000000 dccquantities-1.4.3/src/dccQuantities.egg-info/requires.txt
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)       68 2024-04-30 09:52:02.000000 dccquantities-1.4.3/src/dccQuantities.egg-info/top_level.txt
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    68643 2024-04-30 09:51:28.000000 dccquantities-1.4.3/src/dccQuantities.py
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)     1931 2024-04-30 07:43:13.000000 dccquantities-1.4.3/src/dccQuantitiesConfiguration.py
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    12053 2024-04-30 09:51:28.000000 dccquantities-1.4.3/src/dccQuantitiesPlot.py
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-30 09:52:02.954029 dccquantities-1.4.3/tests/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    17747 2024-04-30 09:51:28.000000 dccquantities-1.4.3/tests/test_dccQuantsAndTabs.py
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)     2393 2024-04-30 07:43:13.000000 dccquantities-1.4.3/tests/test_tollerance.py
```

### Comparing `dccquantities-1.4.2/LICENSE` & `dccquantities-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dccquantities-1.4.2/PKG-INFO` & `dccquantities-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dccQuantities
-Version: 1.4.2
+Version: 1.4.3
 Summary: Python classes for working with DDC calibration data
 Home-page: https://gitlab1.ptb.de/digitaldynamicmeasurement/dccQuantities
 Author: Benedikt Seeger, Vanessa Stehr, Thomas Bruns
 Author-email: benedikt.seeger@ptb.de
 License: LGPL-2.1-or-later
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `dccquantities-1.4.2/README.md` & `dccquantities-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dccquantities-1.4.2/setup.cfg` & `dccquantities-1.4.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dccQuantities
-version = 1.4.2
+version = 1.4.3
 description = Python classes for working with DDC calibration data
 long_description = file: README.md
 license = LGPL-2.1-or-later
 author = Benedikt Seeger, Vanessa Stehr, Thomas Bruns
 author_email = benedikt.seeger@ptb.de
 url = https://gitlab1.ptb.de/digitaldynamicmeasurement/dccQuantities
```

### Comparing `dccquantities-1.4.2/src/dccQuantities.egg-info/PKG-INFO` & `dccquantities-1.4.3/src/dccQuantities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dccQuantities
-Version: 1.4.2
+Version: 1.4.3
 Summary: Python classes for working with DDC calibration data
 Home-page: https://gitlab1.ptb.de/digitaldynamicmeasurement/dccQuantities
 Author: Benedikt Seeger, Vanessa Stehr, Thomas Bruns
 Author-email: benedikt.seeger@ptb.de
 License: LGPL-2.1-or-later
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `dccquantities-1.4.2/src/dccQuantities.py` & `dccquantities-1.4.3/src/dccQuantities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1478,20 +1478,20 @@
     
     def __getitem__(self, item):
         """See pyDCCToolsExamplesNoteBook.ipynb for detailed indexing Examples"""
         if type(item) == str:
             if item != "index":
                 try:
                     return self.valueQuantites[self.valueQuantityNames.index(item)]
-                except KeyError as ke:
+                except ValueError as ve:
                     # TODO fix this for multi indexing
                     if item in self.indexQuantityNames:
                         return self.index[self.indexQuantityNames.index(item)]
                     else:
-                        raise ke
+                        raise ve
             else:
                 return self.index
 
         elif type(item) == tuple:
             if type(item[0]) == str:
                 try:
                     return self.interpolators[item[0]](item[1])
```

### Comparing `dccquantities-1.4.2/src/dccQuantitiesConfiguration.py` & `dccquantities-1.4.3/src/dccQuantitiesConfiguration.py`

 * *Files identical despite different names*

### Comparing `dccquantities-1.4.2/src/dccQuantitiesPlot.py` & `dccquantities-1.4.3/src/dccQuantitiesPlot.py`

 * *Files identical despite different names*

### Comparing `dccquantities-1.4.2/tests/test_dccQuantsAndTabs.py` & `dccquantities-1.4.3/tests/test_dccQuantsAndTabs.py`

 * *Files identical despite different names*

### Comparing `dccquantities-1.4.2/tests/test_tollerance.py` & `dccquantities-1.4.3/tests/test_tollerance.py`

 * *Files identical despite different names*

