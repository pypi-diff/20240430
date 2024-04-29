# Comparing `tmp/ecopipeline-0.2.8.tar.gz` & `tmp/ecopipeline-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecopipeline-0.2.8.tar", last modified: Mon Apr 29 18:43:16 2024, max compression
+gzip compressed data, was "ecopipeline-0.2.9.tar", last modified: Mon Apr 29 22:10:05 2024, max compression
```

## Comparing `ecopipeline-0.2.8.tar` & `ecopipeline-0.2.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.049349 ecopipeline-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.049349 ecopipeline-0.2.8/src/ecopipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/src/ecopipeline/extract/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32173 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/extract/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/src/ecopipeline/load/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/load/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/src/ecopipeline/transform/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/transform/bayview.py
--rw-r--r--   0 runner    (1001) docker     (127)    33400 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/transform/lbnl.py
--rw-r--r--   0 runner    (1001) docker     (127)    30170 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/transform/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/src/ecopipeline/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/utils/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-29 18:42:45.000000 ecopipeline-0.2.8/src/ecopipeline/utils/unit_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:16.053349 ecopipeline-0.2.8/src/ecopipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-29 18:43:16.000000 ecopipeline-0.2.8/src/ecopipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-29 18:43:16.000000 ecopipeline-0.2.8/src/ecopipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:43:16.000000 ecopipeline-0.2.8/src/ecopipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-29 18:43:16.000000 ecopipeline-0.2.8/src/ecopipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 18:43:16.000000 ecopipeline-0.2.8/src/ecopipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.045734 ecopipeline-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-29 22:10:05.045734 ecopipeline-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-29 22:10:05.045734 ecopipeline-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.041734 ecopipeline-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.041734 ecopipeline-0.2.9/src/ecopipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.041734 ecopipeline-0.2.9/src/ecopipeline/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32173 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/extract/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.041734 ecopipeline-0.2.9/src/ecopipeline/load/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/load/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.045734 ecopipeline-0.2.9/src/ecopipeline/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17319 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/transform/bayview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33400 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/transform/lbnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30170 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/transform/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.045734 ecopipeline-0.2.9/src/ecopipeline/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/utils/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/utils/unit_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.045734 ecopipeline-0.2.9/src/ecopipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-29 22:10:05.000000 ecopipeline-0.2.9/src/ecopipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-29 22:10:05.000000 ecopipeline-0.2.9/src/ecopipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:10:05.000000 ecopipeline-0.2.9/src/ecopipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-29 22:10:05.000000 ecopipeline-0.2.9/src/ecopipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 22:10:05.000000 ecopipeline-0.2.9/src/ecopipeline.egg-info/top_level.txt
```

### Comparing `ecopipeline-0.2.8/PKG-INFO` & `ecopipeline-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.2.8
+Version: 0.2.9
 Summary: Contains functions for use in Ecotope Datapipelines
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ecopipeline-0.2.8/README.md` & `ecopipeline-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.8/setup.cfg` & `ecopipeline-0.2.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecopipeline
-version = 0.2.8
+version = 0.2.9
 authors = ["Carlos Bello, <bellocarlos@seattleu.edu>, Emil Fahrig <fahrigemil@seattleu.edu>, Casey Mang <cmang@seattleu.edu>, Julian Harris <harrisjulian@seattleu.edu>, Roger Tram <rtram@seattleu.edu>, Nolan Price <nolan@ecotope.com>"]
 description = Contains functions for use in Ecotope Datapipelines
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecopipeline-0.2.8/src/ecopipeline/extract/extract.py` & `ecopipeline-0.2.9/src/ecopipeline/extract/extract.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.8/src/ecopipeline/load/load.py` & `ecopipeline-0.2.9/src/ecopipeline/load/load.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.8/src/ecopipeline/transform/__init__.py` & `ecopipeline-0.2.9/src/ecopipeline/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.8/src/ecopipeline/transform/bayview.py` & `ecopipeline-0.2.9/src/ecopipeline/transform/bayview.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,14 +376,16 @@
     cop_inter = df [['Temp_RecircSupply_avg', 'HeatOut_PrimaryPlant', 'HeatOut_SecLoop', 'HeatOut_HW', 'HeatLoss_TempMaint_MXV1', 'HeatLoss_TempMaint_MXV2', 'EnergyIn_SecLoopPump', 'EnergyIn_HPWH']].resample('D').mean()
 
     cop_inter['HeatOut_HW_dyavg'] = energy_kwh_to_kbtu(avg_sd['Flow_CityWater'], cop_inter['Temp_RecircSupply_avg'] -
                                                        avg_sd_6['Temp_CityWater'])
     cop_inter['HeatOut_PrimaryPlant_dyavg'] = energy_kwh_to_kbtu(avg_sd['Flow_CityWater_atSkid'],
                                                                  avg_sd['Temp_PrimaryStorageOutTop'] -
                                                                  avg_sd_6['Temp_CityWater_atSkid'])
+    # in case of negative heat out, set to zero
+    cop_inter.loc['HeatOut_PrimaryPlant_dyavg'] = cop_inter.loc['HeatOut_PrimaryPlant_dyavg'].apply(lambda x: max(x, 0))
 
     return cop_inter
 
 
 def calculate_cop_values(df: pd.DataFrame, heatLoss_fixed: int, thermo_slice: str) -> pd.DataFrame:
     """
     Performs COP calculations using the daily aggregated data.
```

### Comparing `ecopipeline-0.2.8/src/ecopipeline/transform/lbnl.py` & `ecopipeline-0.2.9/src/ecopipeline/transform/lbnl.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.8/src/ecopipeline/transform/transform.py` & `ecopipeline-0.2.9/src/ecopipeline/transform/transform.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.8/src/ecopipeline/utils/ConfigManager.py` & `ecopipeline-0.2.9/src/ecopipeline/utils/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.8/src/ecopipeline/utils/unit_convert.py` & `ecopipeline-0.2.9/src/ecopipeline/utils/unit_convert.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.8/src/ecopipeline.egg-info/PKG-INFO` & `ecopipeline-0.2.9/src/ecopipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.2.8
+Version: 0.2.9
 Summary: Contains functions for use in Ecotope Datapipelines
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ecopipeline-0.2.8/src/ecopipeline.egg-info/SOURCES.txt` & `ecopipeline-0.2.9/src/ecopipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

