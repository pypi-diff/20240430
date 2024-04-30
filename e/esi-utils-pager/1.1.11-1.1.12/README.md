# Comparing `tmp/esi_utils_pager-1.1.11.tar.gz` & `tmp/esi_utils_pager-1.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esi_utils_pager-1.1.11.tar", last modified: Fri Apr 19 22:27:41 2024, max compression
+gzip compressed data, was "esi_utils_pager-1.1.12.tar", last modified: Tue Apr 30 15:41:35 2024, max compression
```

## Comparing `esi_utils_pager-1.1.11.tar` & `esi_utils_pager-1.1.12.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-19 22:27:41.103234 esi_utils_pager-1.1.11/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/LICENSE.md
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     7837 2024-04-19 22:27:41.103234 esi_utils_pager-1.1.11/PKG-INFO
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4697 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/README.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1254 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/pyproject.toml
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-04-19 22:27:41.103234 esi_utils_pager-1.1.11/setup.cfg
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-19 22:27:41.087235 esi_utils_pager-1.1.11/src/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-19 22:27:41.091235 esi_utils_pager-1.1.11/src/esi_utils_pager/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-19 22:26:33.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/__init__.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-19 22:27:41.091235 esi_utils_pager-1.1.11/src/esi_utils_pager/bin/
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     5872 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/bin/pagerlite.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8250 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/calc.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2629 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/config.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4444 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/country.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-19 22:27:41.099234 esi_utils_pager-1.1.11/src/esi_utils_pager/data/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   288256 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   366080 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   974848 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    44597 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/countries.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    54009 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/economic.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   324036 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/economy.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    33076 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/fatality.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   214515 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/fatality.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   176744 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_casualty.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   218436 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_casualty.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   260968 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_collapse_mmi.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   198134 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_collapse_mmi.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)  1006280 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_inventory.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   290497 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_inventory.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27120 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_workforce.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14527 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_workforce.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7424 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/econexposure.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    24334 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/emploss.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8367 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/exposure.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7078 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/growth.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      422 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/pandas_container.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2467 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/probs.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27500 2024-04-19 22:14:55.000000 esi_utils_pager-1.1.11/src/esi_utils_pager/semimodel.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-19 22:27:41.099234 esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     7837 2024-04-19 22:27:41.000000 esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/PKG-INFO
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1441 2024-04-19 22:27:41.000000 esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/SOURCES.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-04-19 22:27:41.000000 esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/dependency_links.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       65 2024-04-19 22:27:41.000000 esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/entry_points.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      281 2024-04-19 22:27:41.000000 esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/requires.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       16 2024-04-19 22:27:41.000000 esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/top_level.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-30 15:41:35.478279 esi_utils_pager-1.1.12/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/LICENSE.md
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     8128 2024-04-30 15:41:35.478279 esi_utils_pager-1.1.12/PKG-INFO
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4988 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/README.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1254 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/pyproject.toml
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-04-30 15:41:35.478279 esi_utils_pager-1.1.12/setup.cfg
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-30 15:41:35.466279 esi_utils_pager-1.1.12/src/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-30 15:41:35.466279 esi_utils_pager-1.1.12/src/esi_utils_pager/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/__init__.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-30 15:41:35.470279 esi_utils_pager-1.1.12/src/esi_utils_pager/bin/
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     9973 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/bin/pagerlite.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10037 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/calc.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2629 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/config.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4444 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/country.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-30 15:41:35.478279 esi_utils_pager-1.1.12/src/esi_utils_pager/data/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   288256 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   366080 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   974848 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    44597 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/countries.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    54009 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/economic.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   324036 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/economy.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    33076 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/fatality.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   214515 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/fatality.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   176744 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_casualty.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   218436 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_casualty.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   260968 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_collapse_mmi.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   198134 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_collapse_mmi.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)  1006280 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_inventory.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   290497 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_inventory.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27120 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_workforce.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14527 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_workforce.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7424 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/econexposure.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    24334 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/emploss.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8367 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/exposure.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7078 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/growth.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      422 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/pandas_container.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2467 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/probs.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27500 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/semimodel.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-30 15:41:35.478279 esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     8128 2024-04-30 15:41:35.000000 esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/PKG-INFO
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1441 2024-04-30 15:41:35.000000 esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/SOURCES.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-04-30 15:41:35.000000 esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/dependency_links.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       65 2024-04-30 15:41:35.000000 esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/entry_points.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      281 2024-04-30 15:41:35.000000 esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/requires.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       16 2024-04-30 15:41:35.000000 esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/top_level.txt
```

### Comparing `esi_utils_pager-1.1.11/LICENSE.md` & `esi_utils_pager-1.1.12/LICENSE.md`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/PKG-INFO` & `esi_utils_pager-1.1.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-utils-pager
-Version: 1.1.11
+Version: 1.1.12
 Summary: USGS PAGER loss modeling functionality
 Author-email: Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -184,14 +184,21 @@
 
 `pagerlite -e us7000lz23 -o output.xlsx`
 
 To run the PAGER empirical AND semi-empirical models, simply add the `-s` flag to any of the above commands:
 
 `pagerlite -e us7000lz23 -s -o output.xlsx`
 
+To run the PAGER empirical models on a folder but only for events between 2010 and 2017:
+
+`pagerlite -f /data/shakemap_output/ -t 2010-01-01 2017-12-31T23:59:59 -o output.xlsx`
+
+See the help for more options (spatial bounds and magnitude range) on restricting processing of ShakeMap
+grids.
+
 
 
 # Library Usage
 
 Usage of the relevant code modules is detailed in the Jupyter notebooks, most notably in the 
 [Earthquake Losses notebook](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/blob/main/notebooks/EarthquakeLosses.ipynb)
```

### Comparing `esi_utils_pager-1.1.11/README.md` & `esi_utils_pager-1.1.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,21 @@
 
 `pagerlite -e us7000lz23 -o output.xlsx`
 
 To run the PAGER empirical AND semi-empirical models, simply add the `-s` flag to any of the above commands:
 
 `pagerlite -e us7000lz23 -s -o output.xlsx`
 
+To run the PAGER empirical models on a folder but only for events between 2010 and 2017:
+
+`pagerlite -f /data/shakemap_output/ -t 2010-01-01 2017-12-31T23:59:59 -o output.xlsx`
+
+See the help for more options (spatial bounds and magnitude range) on restricting processing of ShakeMap
+grids.
+
 
 
 # Library Usage
 
 Usage of the relevant code modules is detailed in the Jupyter notebooks, most notably in the 
 [Earthquake Losses notebook](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/blob/main/notebooks/EarthquakeLosses.ipynb)
```

### Comparing `esi_utils_pager-1.1.11/pyproject.toml` & `esi_utils_pager-1.1.12/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/calc.py` & `esi_utils_pager-1.1.12/src/esi_utils_pager/calc.py`

 * *Files 19% similar despite different names*

```diff
@@ -126,34 +126,75 @@
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         ltime = LocalTime(timezone_file, etime, lat, lon)
         localtime = ltime.getLocalTime()
     return localtime
 
 
-def get_semi_losses(gridfile, popfile, popyear, isofile, urbanfile):
-    semimodel = SemiEmpiricalFatality.fromDefault()
+def get_semi_losses(gridfile, popfile, popyear, isofile, urbanfile, semi_folder):
+    if semi_folder is None:
+        semimodel = SemiEmpiricalFatality.fromDefault()
+    else:
+        semi_folder = pathlib.Path(semi_folder)
+        inventory_file = semi_folder / "semi_inventory.xlsx"
+        collapse_file = semi_folder / "semi_collapse_mmi.xlsx"
+        casualty_file = semi_folder / "semi_casualty.xlsx"
+        workforce_file = semi_folder / "semi_workforce.xlsx"
+        semimodel = SemiEmpiricalFatality.fromFiles(
+            inventory_file, collapse_file, casualty_file, workforce_file
+        )
     semimodel.setGlobalFiles(popfile, popyear, urbanfile, isofile)
     # Tuple of:
     #         1) Total number of fatalities
     #         2) Dictionary of residential fatalities per building type, per country.
     #         3) Dictionary of non-residential fatalities per building type, per country.
     semifat, resfat, nonresfat = semimodel.getLosses(gridfile)
     return (semifat, resfat, nonresfat)
 
 
-def calc_pager_event(gridfile, config, run_semi, fatality_file, economic_file):
+def calc_pager_event(
+    gridfile,
+    config,
+    run_semi,
+    fatality_file,
+    economic_file,
+    semi_folder,
+    starttime=None,
+    endtime=None,
+    bounds=None,
+    magrange=None,
+):
     # get all the basic event information and print it, if requested
     shake_tuple = getHeaderData(gridfile)
     local_time = get_local_time(
         shake_tuple[1]["event_timestamp"],
         config["model_data"]["timezones_file"],
         shake_tuple[1]["lat"],
         shake_tuple[1]["lon"],
     )
+    empty_dataframe = pd.DataFrame()
+    eventid = shake_tuple[1]["event_id"]
+    if (
+        shake_tuple[1]["event_timestamp"] < starttime
+        or shake_tuple[1]["event_timestamp"] > endtime
+    ):
+        print(f"Skipping event {eventid} (out of time range)")
+        return empty_dataframe
+    outside_lat = shake_tuple[1]["lat"] < bounds[2] or shake_tuple[1]["lat"] > bounds[3]
+    outside_lon = shake_tuple[1]["lon"] < bounds[0] or shake_tuple[1]["lon"] > bounds[1]
+    if outside_lat or outside_lon:
+        print(f"Skipping event {eventid} (out of spatial range)")
+        return empty_dataframe
+    if (
+        shake_tuple[1]["magnitude"] < magrange[0]
+        or shake_tuple[1]["magnitude"] > magrange[1]
+    ):
+        print(f"Skipping event {eventid} (out of magnitude range)")
+        return empty_dataframe
+    print(f"Processing event {eventid}...")
     master_row = {}
     master_row["EventID"] = shake_tuple[1]["event_id"]
     master_row["Time"] = shake_tuple[1]["event_timestamp"]
     master_row["LocalTime"] = local_time
     master_row["Latitude"] = shake_tuple[1]["lat"]
     master_row["Longitude"] = shake_tuple[1]["lon"]
     master_row["Depth"] = shake_tuple[1]["depth"]
@@ -173,15 +214,15 @@
     ecoframe = get_econ_losses(
         fatframe, popfile, pop_year, isofile, gridfile, economic_file
     )
 
     if run_semi:
         urbanfile = config["model_data"]["urban_rural_grid"]
         semifat, resfat, nonresfat = get_semi_losses(
-            gridfile, popfile, pop_year, isofile, urbanfile
+            gridfile, popfile, pop_year, isofile, urbanfile, semi_folder
         )
         resframe = pd.DataFrame(resfat).transpose()
         nonresframe = pd.DataFrame(nonresfat).transpose()
         final_frame = resframe.add(nonresframe)
         final_frame = final_frame.round()
         ny, nx = final_frame.shape
         if nx > 0 and ny > 0:
@@ -190,30 +231,50 @@
             btotal = final_frame.sum(axis="columns")
             final_frame["TotalSemiFatalities"] = btotal
             ecoframe = ecoframe.join(final_frame, on=["CountryCode"])
 
     return ecoframe
 
 
-def calc_pager_events(gridfolder, verbose, run_semi, fatality_file, economic_file):
+def calc_pager_events(
+    gridfolder,
+    verbose,
+    run_semi,
+    fatality_file,
+    economic_file,
+    semi_folder,
+    starttime=None,
+    endtime=None,
+    bounds=None,
+    magrange=None,
+):
     gridfolder = pathlib.Path(gridfolder)
     # read config file
     config = read_config()
     # Make sure grid.xml file exists
     if not gridfolder.is_dir():
         print(f"ShakeMap Grid folder {gridfolder} does not exist.")
         sys.exit(1)
 
     gridfiles = gridfolder.glob("**/*grid.xml")
     dataframes = []
     for gridfile in gridfiles:
         if verbose:
             logging.info(f"Parsing {gridfile}...")
         dataframe = calc_pager_event(
-            gridfile, config, run_semi, fatality_file, economic_file
+            gridfile,
+            config,
+            run_semi,
+            fatality_file,
+            economic_file,
+            semi_folder,
+            starttime=starttime,
+            endtime=endtime,
+            bounds=bounds,
+            magrange=magrange,
         )
         dataframes.append(dataframe)
 
     dataframe = pd.concat(dataframes)
     if run_semi:
         # make TotalSemiFatalities column the last one, if it exists
         fatcol = dataframe.pop("TotalSemiFatalities")
```

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/config.py` & `esi_utils_pager-1.1.12/src/esi_utils_pager/config.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/country.py` & `esi_utils_pager-1.1.12/src/esi_utils_pager/country.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/countries.xlsx` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/countries.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/economic.xlsx` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/economic.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/economy.xml` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/economy.xml`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/fatality.xlsx` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/fatality.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/fatality.xml` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/fatality.xml`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_casualty.hdf` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_casualty.hdf`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_casualty.xlsx` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_casualty.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_collapse_mmi.hdf` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_collapse_mmi.hdf`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_collapse_mmi.xlsx` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_collapse_mmi.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_inventory.hdf` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_inventory.hdf`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_inventory.xlsx` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_inventory.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_workforce.hdf` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_workforce.hdf`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/data/semi_workforce.xlsx` & `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_workforce.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/econexposure.py` & `esi_utils_pager-1.1.12/src/esi_utils_pager/econexposure.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/emploss.py` & `esi_utils_pager-1.1.12/src/esi_utils_pager/emploss.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/exposure.py` & `esi_utils_pager-1.1.12/src/esi_utils_pager/exposure.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/growth.py` & `esi_utils_pager-1.1.12/src/esi_utils_pager/growth.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/probs.py` & `esi_utils_pager-1.1.12/src/esi_utils_pager/probs.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager/semimodel.py` & `esi_utils_pager-1.1.12/src/esi_utils_pager/semimodel.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/PKG-INFO` & `esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-utils-pager
-Version: 1.1.11
+Version: 1.1.12
 Summary: USGS PAGER loss modeling functionality
 Author-email: Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -184,14 +184,21 @@
 
 `pagerlite -e us7000lz23 -o output.xlsx`
 
 To run the PAGER empirical AND semi-empirical models, simply add the `-s` flag to any of the above commands:
 
 `pagerlite -e us7000lz23 -s -o output.xlsx`
 
+To run the PAGER empirical models on a folder but only for events between 2010 and 2017:
+
+`pagerlite -f /data/shakemap_output/ -t 2010-01-01 2017-12-31T23:59:59 -o output.xlsx`
+
+See the help for more options (spatial bounds and magnitude range) on restricting processing of ShakeMap
+grids.
+
 
 
 # Library Usage
 
 Usage of the relevant code modules is detailed in the Jupyter notebooks, most notably in the 
 [Earthquake Losses notebook](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/blob/main/notebooks/EarthquakeLosses.ipynb)
```

### Comparing `esi_utils_pager-1.1.11/src/esi_utils_pager.egg-info/SOURCES.txt` & `esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

