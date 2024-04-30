# Comparing `tmp/cropharvest-0.6.0.tar.gz` & `tmp/cropharvest-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cropharvest-0.6.0.tar", last modified: Mon Oct 31 19:00:06 2022, max compression
+gzip compressed data, was "cropharvest-0.7.0.tar", last modified: Tue Apr 30 14:37:39 2024, max compression
```

## Comparing `cropharvest-0.6.0.tar` & `cropharvest-0.7.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-31 19:00:06.354711 cropharvest-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (116)    20131 2022-10-31 18:59:52.000000 cropharvest-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)       40 2022-10-31 18:59:52.000000 cropharvest-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     8764 2022-10-31 19:00:06.354711 cropharvest-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8453 2022-10-31 18:59:52.000000 cropharvest-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-31 19:00:06.350711 cropharvest-0.6.0/cropharvest/
--rw-r--r--   0 runner    (1001) docker     (116)      237 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1823 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/bands.py
--rw-r--r--   0 runner    (1001) docker     (116)     2545 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/bbox.py
--rw-r--r--   0 runner    (1001) docker     (116)     1137 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/columns.py
--rw-r--r--   0 runner    (1001) docker     (116)     1538 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     1821 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/countries.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-31 19:00:06.350711 cropharvest-0.6.0/cropharvest/country_shapefile/
--rw-r--r--   0 runner    (1001) docker     (116)   546979 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/country_shapefile/ne_50m_admin_0_countries.dbf
--rw-r--r--   0 runner    (1001) docker     (116)  1612740 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/country_shapefile/ne_50m_admin_0_countries.shp
--rw-r--r--   0 runner    (1001) docker     (116)     2028 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/country_shapefile/ne_50m_admin_0_countries.shx
--rw-r--r--   0 runner    (1001) docker     (116)     1285 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/crops.py
--rw-r--r--   0 runner    (1001) docker     (116)    18175 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/datasets.py
--rw-r--r--   0 runner    (1001) docker     (116)    23601 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/engineer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-31 19:00:06.354711 cropharvest-0.6.0/cropharvest/eo/
--rw-r--r--   0 runner    (1001) docker     (116)       72 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/eo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4931 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/eo/ee_boundingbox.py
--rw-r--r--   0 runner    (1001) docker     (116)    17940 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/eo/eo.py
--rw-r--r--   0 runner    (1001) docker     (116)     1803 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/eo/era5.py
--rw-r--r--   0 runner    (1001) docker     (116)     2681 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/eo/sentinel1.py
--rw-r--r--   0 runner    (1001) docker     (116)     6133 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/eo/sentinel2.py
--rw-r--r--   0 runner    (1001) docker     (116)      388 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/eo/srtm.py
--rw-r--r--   0 runner    (1001) docker     (116)      917 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/eo/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     3693 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/inference.py
--rw-r--r--   0 runner    (1001) docker     (116)     4200 2022-10-31 18:59:52.000000 cropharvest-0.6.0/cropharvest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-31 19:00:06.350711 cropharvest-0.6.0/cropharvest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8764 2022-10-31 19:00:06.000000 cropharvest-0.6.0/cropharvest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      865 2022-10-31 19:00:06.000000 cropharvest-0.6.0/cropharvest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-31 19:00:06.000000 cropharvest-0.6.0/cropharvest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      118 2022-10-31 19:00:06.000000 cropharvest-0.6.0/cropharvest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2022-10-31 19:00:06.000000 cropharvest-0.6.0/cropharvest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      161 2022-10-31 18:59:53.000000 cropharvest-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-10-31 19:00:06.354711 cropharvest-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1223 2022-10-31 18:59:53.000000 cropharvest-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:37:39.062629 cropharvest-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    20131 2024-04-30 14:37:33.000000 cropharvest-0.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-30 14:37:33.000000 cropharvest-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-04-30 14:37:39.062629 cropharvest-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-04-30 14:37:33.000000 cropharvest-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:37:39.054629 cropharvest-0.7.0/cropharvest/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/countries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:37:39.058629 cropharvest-0.7.0/cropharvest/country_shapefile/
+-rw-r--r--   0 runner    (1001) docker     (127)   546979 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/country_shapefile/ne_50m_admin_0_countries.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)  1612740 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/country_shapefile/ne_50m_admin_0_countries.shp
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/country_shapefile/ne_50m_admin_0_countries.shx
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/crops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18673 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23596 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/engineer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:37:39.062629 cropharvest-0.7.0/cropharvest/eo/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/eo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/eo/ee_boundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17932 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/eo/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/eo/era5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/eo/sentinel1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/eo/sentinel2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/eo/srtm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/eo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-30 14:37:33.000000 cropharvest-0.7.0/cropharvest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:37:39.062629 cropharvest-0.7.0/cropharvest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-04-30 14:37:39.000000 cropharvest-0.7.0/cropharvest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-30 14:37:39.000000 cropharvest-0.7.0/cropharvest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:37:39.000000 cropharvest-0.7.0/cropharvest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-30 14:37:39.000000 cropharvest-0.7.0/cropharvest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 14:37:39.000000 cropharvest-0.7.0/cropharvest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 14:37:34.000000 cropharvest-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:37:39.062629 cropharvest-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-30 14:37:34.000000 cropharvest-0.7.0/setup.py
```

### Comparing `cropharvest-0.6.0/LICENSE.txt` & `cropharvest-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cropharvest-0.6.0/PKG-INFO` & `cropharvest-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6372 6f70  : 2.1.Name: crop
 00000020: 6861 7276 6573 740a 5665 7273 696f 6e3a  harvest.Version:
-00000030: 2030 2e36 2e30 0a53 756d 6d61 7279 3a20   0.6.0.Summary: 
+00000030: 2030 2e37 2e30 0a53 756d 6d61 7279 3a20   0.7.0.Summary: 
 00000040: 4f70 656e 2073 6f75 7263 6520 7265 6d6f  Open source remo
 00000050: 7465 2073 656e 7369 6e67 2064 6174 6173  te sensing datas
 00000060: 6574 2077 6974 6820 6265 6e63 686d 6172  et with benchmar
 00000070: 6b73 0a48 6f6d 652d 7061 6765 3a20 6874  ks.Home-page: ht
 00000080: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000090: 2f6e 6173 6168 6172 7665 7374 2f63 726f  /nasaharvest/cro
 000000a0: 7068 6172 7665 7374 0a41 7574 686f 723a  pharvest.Author:
@@ -22,527 +22,555 @@
 00000150: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
 00000160: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
 00000170: 6e64 656e 740a 5265 7175 6972 6573 2d50  ndent.Requires-P
 00000180: 7974 686f 6e3a 203e 3d33 2e36 0a44 6573  ython: >=3.6.Des
 00000190: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
 000001a0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
 000001b0: 646f 776e 0a4c 6963 656e 7365 2d46 696c  down.License-Fil
-000001c0: 653a 204c 4943 454e 5345 2e74 7874 0a0a  e: LICENSE.txt..
-000001d0: 2320 4372 6f70 4861 7276 6573 740a 0a43  # CropHarvest..C
-000001e0: 726f 7048 6172 7665 7374 2069 7320 616e  ropHarvest is an
-000001f0: 206f 7065 6e20 736f 7572 6365 2072 656d   open source rem
-00000200: 6f74 6520 7365 6e73 696e 6720 6461 7461  ote sensing data
-00000210: 7365 7420 666f 7220 6167 7269 6375 6c74  set for agricult
-00000220: 7572 6520 7769 7468 2062 656e 6368 6d61  ure with benchma
-00000230: 726b 732e 2049 7420 636f 6c6c 6563 7473  rks. It collects
-00000240: 2064 6174 6120 6672 6f6d 2061 2076 6172   data from a var
-00000250: 6965 7479 206f 6620 6167 7269 6375 6c74  iety of agricult
-00000260: 7572 616c 206c 616e 6420 7573 6520 6461  ural land use da
-00000270: 7461 7365 7473 2061 6e64 2072 656d 6f74  tasets and remot
-00000280: 6520 7365 6e73 696e 6720 7072 6f64 7563  e sensing produc
-00000290: 7473 2e0a 0a0a 5468 6520 6461 7461 7365  ts....The datase
-000002a0: 7420 636f 6e73 6973 7473 206f 6620 2a2a  t consists of **
-000002b0: 3935 2c31 3836 2a2a 2064 6174 6170 6f69  95,186** datapoi
-000002c0: 6e74 732c 206f 6620 7768 6963 6820 2a2a  nts, of which **
-000002d0: 3333 2c32 3035 2a2a 2028 3335 2529 2068  33,205** (35%) h
-000002e0: 6176 6520 6d75 6c74 6963 6c61 7373 206c  ave multiclass l
-000002f0: 6162 656c 732e 2041 6c6c 206f 7468 6572  abels. All other
-00000300: 2064 6174 6170 6f69 6e74 7320 6f6e 6c79   datapoints only
-00000310: 2068 6176 6520 6269 6e61 7279 2063 726f   have binary cro
-00000320: 7020 2f20 6e6f 6e2d 6372 6f70 206c 6162  p / non-crop lab
-00000330: 656c 732e 0a0a 2a2a 3730 2c32 3133 2a2a  els...**70,213**
-00000340: 2028 3734 2529 206f 6620 7468 6573 6520   (74%) of these 
-00000350: 6c61 6265 6c73 2061 7265 2070 6169 7265  labels are paire
-00000360: 6420 7769 7468 2072 656d 6f74 6520 7365  d with remote se
-00000370: 6e73 696e 6720 616e 6420 636c 696d 6174  nsing and climat
-00000380: 6f6c 6f67 7920 6461 7461 2c20 7370 6563  ology data, spec
-00000390: 6966 6963 616c 6c79 205b 5365 6e74 696e  ifically [Sentin
-000003a0: 656c 2d32 5d28 6874 7470 733a 2f2f 7365  el-2](https://se
-000003b0: 6e74 696e 656c 2e65 7361 2e69 6e74 2f77  ntinel.esa.int/w
-000003c0: 6562 2f73 656e 7469 6e65 6c2f 6d69 7373  eb/sentinel/miss
-000003d0: 696f 6e73 2f73 656e 7469 6e65 6c2d 3229  ions/sentinel-2)
-000003e0: 2c20 5b53 656e 7469 6e65 6c2d 315d 2868  , [Sentinel-1](h
-000003f0: 7474 7073 3a2f 2f73 656e 7469 6e65 6c2e  ttps://sentinel.
-00000400: 6573 612e 696e 742f 7765 622f 7365 6e74  esa.int/web/sent
-00000410: 696e 656c 2f6d 6973 7369 6f6e 732f 7365  inel/missions/se
-00000420: 6e74 696e 656c 2d31 2f29 2c20 7468 6520  ntinel-1/), the 
-00000430: 5b53 5254 4d20 4469 6769 7461 6c20 456c  [SRTM Digital El
-00000440: 6576 6174 696f 6e20 4d6f 6465 6c5d 2868  evation Model](h
-00000450: 7474 7073 3a2f 2f63 6769 6172 6373 692e  ttps://cgiarcsi.
-00000460: 636f 6d6d 756e 6974 792f 6461 7461 2f73  community/data/s
-00000470: 7274 6d2d 3930 6d2d 6469 6769 7461 6c2d  rtm-90m-digital-
-00000480: 656c 6576 6174 696f 6e2d 6461 7461 6261  elevation-databa
-00000490: 7365 2d76 342d 312f 2920 616e 6420 5b45  se-v4-1/) and [E
-000004a0: 5241 2035 2063 6c69 6d61 746f 6c6f 6779  RA 5 climatology
-000004b0: 2064 6174 615d 2868 7474 7073 3a2f 2f77   data](https://w
-000004c0: 7777 2e65 636d 7766 2e69 6e74 2f65 6e2f  ww.ecmwf.int/en/
-000004d0: 666f 7265 6361 7374 732f 6461 7461 7365  forecasts/datase
-000004e0: 7473 2f72 6561 6e61 6c79 7369 732d 6461  ts/reanalysis-da
-000004f0: 7461 7365 7473 2f65 7261 3529 2e0a 0a32  tasets/era5)...2
-00000500: 3120 6461 7461 7365 7473 2061 7265 2061  1 datasets are a
-00000510: 6767 7265 6761 7465 6420 696e 746f 2043  ggregated into C
-00000520: 726f 7048 6172 7665 7374 202d 2074 6865  ropHarvest - the
-00000530: 7365 2061 7265 2064 6f63 756d 656e 7465  se are documente
-00000540: 6420 5b68 6572 655d 2868 7474 7073 3a2f  d [here](https:/
-00000550: 2f67 6974 6875 622e 636f 6d2f 6e61 7361  /github.com/nasa
-00000560: 6861 7276 6573 742f 6372 6f70 6861 7276  harvest/cropharv
-00000570: 6573 742f 626c 6f62 2f6d 6169 6e2f 6461  est/blob/main/da
-00000580: 7461 7365 7473 2e6d 6429 2e0a 0a4d 6f72  tasets.md)...Mor
-00000590: 6520 6465 7461 696c 7320 6162 6f75 7420  e details about 
-000005a0: 4372 6f70 4861 7276 6573 7420 616e 6420  CropHarvest and 
-000005b0: 7468 6520 6265 6e63 686d 6172 6b73 2061  the benchmarks a
-000005c0: 7265 2061 7661 696c 6162 6c65 2069 6e20  re available in 
-000005d0: 5b74 6869 7320 7061 7065 725d 2868 7474  [this paper](htt
-000005e0: 7073 3a2f 2f6f 7065 6e72 6576 6965 772e  ps://openreview.
-000005f0: 6e65 742f 666f 7275 6d3f 6964 3d4a 746a  net/forum?id=Jtj
-00000600: 7a55 5850 4561 4375 292e 0a0a 2323 2320  zUXPEaCu)...### 
-00000610: 5069 7065 6c69 6e65 0a54 6865 2063 6f64  Pipeline.The cod
-00000620: 6520 696e 2074 6869 7320 7265 706f 7369  e in this reposi
-00000630: 746f 7279 0a0a 3129 2063 6f6d 6269 6e65  tory..1) combine
-00000640: 7320 7468 6520 636f 6e73 7469 7475 656e  s the constituen
-00000650: 7420 6461 7461 7365 7473 2069 6e74 6f20  t datasets into 
-00000660: 6120 7369 6e67 6c65 2067 656f 4a53 4f4e  a single geoJSON
-00000670: 2066 696c 652c 0a32 2920 6578 706f 7274   file,.2) export
-00000680: 7320 7468 6520 6173 736f 6369 6174 6564  s the associated
-00000690: 2073 6174 656c 6c69 7465 2064 6174 6120   satellite data 
-000006a0: 6672 6f6d 2045 6172 7468 2045 6e67 696e  from Earth Engin
-000006b0: 652c 0a33 2920 636f 6d62 696e 6573 2062  e,.3) combines b
-000006c0: 6f74 6820 6461 7461 7365 7473 2074 6f20  oth datasets to 
-000006d0: 6372 6561 7465 2060 2858 2c79 2960 2074  create `(X,y)` t
-000006e0: 7261 696e 696e 6720 7475 706c 6573 2061  raining tuples a
-000006f0: 6e64 0a34 2920 6578 706f 7365 7320 7468  nd.4) exposes th
-00000700: 6f73 6520 7475 706c 6573 2076 6961 2061  ose tuples via a
-00000710: 2060 4461 7461 7365 7460 206f 626a 6563   `Dataset` objec
-00000720: 742e 0a0a 5468 6520 7069 7065 6c69 6e65  t...The pipeline
-00000730: 2074 6872 6f75 6768 2077 6869 6368 2074   through which t
-00000740: 6869 7320 6861 7070 656e 7320 6973 2073  his happens is s
-00000750: 686f 776e 2062 656c 6f77 3a0a 0a0a 416c  hown below:...Al
-00000760: 6c20 626c 7565 2062 6f78 6573 2061 7265  l blue boxes are
-00000770: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-00000780: 2063 6f64 6520 696e 2074 6869 7320 7265   code in this re
-00000790: 706f 7369 746f 7279 2e20 416e 7974 6869  pository. Anythi
-000007a0: 6e67 2067 7265 656e 2069 7320 6461 7461  ng green is data
-000007b0: 2061 6363 6573 7369 626c 6520 7669 6120   accessible via 
-000007c0: 5b5a 656e 6f64 6f5d 2868 7474 7073 3a2f  [Zenodo](https:/
-000007d0: 2f7a 656e 6f64 6f2e 6f72 672f 7265 636f  /zenodo.org/reco
-000007e0: 7264 2f35 3832 3838 3933 292e 2042 7920  rd/5828893). By 
-000007f0: 6465 6661 756c 742c 2074 6865 205a 656e  default, the Zen
-00000800: 6f64 6f20 6461 7461 2077 696c 6c20 6765  odo data will ge
-00000810: 7420 646f 776e 6c6f 6164 6564 2074 6f20  t downloaded to 
-00000820: 7468 6520 5b64 6174 6120 666f 6c64 6572  the [data folder
-00000830: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000840: 2e63 6f6d 2f6e 6173 6168 6172 7665 7374  .com/nasaharvest
-00000850: 2f63 726f 7068 6172 7665 7374 2f74 7265  /cropharvest/tre
-00000860: 652f 6d61 696e 2f64 6174 6129 202d 2074  e/main/data) - t
-00000870: 6865 2064 6174 6120 666f 6c64 6572 2773  he data folder's
-00000880: 205b 5265 6164 6d65 5d28 6874 7470 733a   [Readme](https:
-00000890: 2f2f 6769 7468 7562 2e63 6f6d 2f6e 6173  //github.com/nas
-000008a0: 6168 6172 7665 7374 2f63 726f 7068 6172  aharvest/crophar
-000008b0: 7665 7374 2f62 6c6f 622f 6d61 696e 2f64  vest/blob/main/d
-000008c0: 6174 612f 5245 4144 4d45 2e6d 6429 2068  ata/README.md) h
-000008d0: 6173 206d 6f72 6520 696e 666f 726d 6174  as more informat
-000008e0: 696f 6e20 6162 6f75 7420 7468 6520 6578  ion about the ex
-000008f0: 6163 7420 7374 7275 6374 7572 6520 6f66  act structure of
-00000900: 2074 6865 2064 6174 612e 0a0a 5468 6572   the data...Ther
-00000910: 6520 6172 6520 756e 6971 7565 2063 6173  e are unique cas
-00000920: 6573 2077 6865 7265 2079 6f75 206d 6179  es where you may
-00000930: 206e 6565 6420 746f 2075 7365 2074 6865   need to use the
-00000940: 2060 4561 7274 6845 6e67 696e 6545 7870   `EarthEngineExp
-00000950: 6f72 7465 7260 2064 6972 6563 746c 792c  orter` directly,
-00000960: 2074 6865 7365 2075 7365 2063 6173 6573   these use cases
-00000970: 2061 7265 2064 656d 6f6e 7374 7261 7465   are demonstrate
-00000980: 6420 696e 2074 6865 205b 6064 656d 6f5f  d in the [`demo_
-00000990: 6578 706f 7274 696e 675f 6461 7461 2e69  exporting_data.i
-000009a0: 7079 6e62 605d 2868 7474 7073 3a2f 2f67  pynb`](https://g
-000009b0: 6974 6875 622e 636f 6d2f 6e61 7361 6861  ithub.com/nasaha
-000009c0: 7276 6573 742f 6372 6f70 6861 7276 6573  rvest/cropharves
-000009d0: 742f 626c 6f62 2f6d 6169 6e2f 6465 6d6f  t/blob/main/demo
-000009e0: 5f65 7870 6f72 7469 6e67 5f64 6174 612e  _exporting_data.
-000009f0: 6970 796e 6229 206e 6f74 6562 6f6f 6b2e  ipynb) notebook.
-00000a00: 0a0a 2323 2320 496e 7374 616c 6c61 7469  ..### Installati
-00000a10: 6f6e 0a4c 696e 7578 2061 6e64 204d 6163  on.Linux and Mac
-00000a20: 4f53 2075 7365 7273 2063 616e 2069 6e73  OS users can ins
-00000a30: 7461 6c6c 2074 6865 206c 6174 6573 7420  tall the latest 
-00000a40: 7665 7273 696f 6e20 6f66 2043 726f 7048  version of CropH
-00000a50: 6172 7665 7374 2077 6974 6820 7468 6520  arvest with the 
-00000a60: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
-00000a70: 643a 0a60 6060 6261 7368 0a70 6970 2069  d:.```bash.pip i
-00000a80: 6e73 7461 6c6c 2063 726f 7068 6172 7665  nstall cropharve
-00000a90: 7374 0a60 6060 0a57 696e 646f 7773 2075  st.```.Windows u
-00000aa0: 7365 7273 206d 7573 7420 696e 7374 616c  sers must instal
-00000ab0: 6c20 7468 6520 4372 6f70 4861 7276 6573  l the CropHarves
-00000ac0: 7420 7769 7468 696e 2061 205b 636f 6e64  t within a [cond
-00000ad0: 615d 2868 7474 7073 3a2f 2f64 6f63 732e  a](https://docs.
-00000ae0: 636f 6e64 612e 696f 2f65 6e2f 6c61 7465  conda.io/en/late
-00000af0: 7374 2f6d 696e 6963 6f6e 6461 2e68 746d  st/miniconda.htm
-00000b00: 6c29 2065 6e76 6972 6f6e 6d65 6e74 2074  l) environment t
-00000b10: 6f20 656e 7375 7265 2061 6c6c 2064 6570  o ensure all dep
-00000b20: 656e 6465 6e63 6965 7320 6172 6520 696e  endencies are in
-00000b30: 7374 616c 6c65 6420 636f 7272 6563 746c  stalled correctl
-00000b40: 793a 0a60 6060 6261 7368 0a63 6f6e 6461  y:.```bash.conda
-00000b50: 2069 6e73 7461 6c6c 2027 6669 6f6e 613e   install 'fiona>
-00000b60: 3d31 2e35 2720 2772 6173 7465 7269 6f3e  =1.5' 'rasterio>
-00000b70: 3d31 2e32 2e36 270a 7069 7020 696e 7374  =1.2.6'.pip inst
-00000b80: 616c 6c20 6372 6f70 6861 7276 6573 740a  all cropharvest.
-00000b90: 6060 600a 0a23 2323 2047 6574 7469 6e67  ```..### Getting
-00000ba0: 2073 7461 7274 6564 205b 215b 4f70 656e   started [![Open
-00000bb0: 2049 6e20 436f 6c61 625d 2868 7474 7073   In Colab](https
-00000bc0: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
-00000bd0: 682e 676f 6f67 6c65 2e63 6f6d 2f61 7373  h.google.com/ass
-00000be0: 6574 732f 636f 6c61 622d 6261 6467 652e  ets/colab-badge.
-00000bf0: 7376 6729 5d28 6874 7470 733a 2f2f 636f  svg)](https://co
-00000c00: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00000c10: 676c 652e 636f 6d2f 6769 7468 7562 2f6e  gle.com/github/n
-00000c20: 6173 6168 6172 7665 7374 2f63 726f 7068  asaharvest/croph
-00000c30: 6172 7665 7374 2f62 6c6f 622f 6d61 696e  arvest/blob/main
-00000c40: 2f64 656d 6f2e 6970 796e 6229 0a53 6565  /demo.ipynb).See
-00000c50: 2074 6865 205b 6064 656d 6f2e 6970 796e   the [`demo.ipyn
-00000c60: 6260 5d28 6874 7470 733a 2f2f 6769 7468  b`](https://gith
-00000c70: 7562 2e63 6f6d 2f6e 6173 6168 6172 7665  ub.com/nasaharve
-00000c80: 7374 2f63 726f 7068 6172 7665 7374 2f62  st/cropharvest/b
-00000c90: 6c6f 622f 6d61 696e 2f64 656d 6f2e 6970  lob/main/demo.ip
-00000ca0: 796e 6229 206e 6f74 6562 6f6f 6b20 666f  ynb) notebook fo
-00000cb0: 7220 616e 2065 7861 6d70 6c65 206f 6e20  r an example on 
-00000cc0: 686f 7720 746f 2064 6f77 6e6c 6f61 6420  how to download 
-00000cd0: 7468 6520 6461 7461 2066 726f 6d20 5b5a  the data from [Z
-00000ce0: 656e 6f64 6f5d 2868 7474 7073 3a2f 2f7a  enodo](https://z
-00000cf0: 656e 6f64 6f2e 6f72 672f 7265 636f 7264  enodo.org/record
-00000d00: 2f37 3235 3736 3838 2920 616e 6420 7472  /7257688) and tr
-00000d10: 6169 6e20 6120 7261 6e64 6f6d 2066 6f72  ain a random for
-00000d20: 6573 7420 6167 6169 6e73 7420 7468 6973  est against this
-00000d30: 2064 6174 612e 0a0a 466f 7220 6d6f 7265   data...For more
-00000d40: 2065 7861 6d70 6c65 7320 6f66 206d 6f64   examples of mod
-00000d50: 656c 7320 7472 6169 6e65 6420 6167 6169  els trained agai
-00000d60: 6e73 7420 7468 6973 2064 6174 6173 6574  nst this dataset
-00000d70: 2c20 7365 6520 7468 6520 5b62 656e 6368  , see the [bench
-00000d80: 6d61 726b 735d 2868 7474 7073 3a2f 2f67  marks](https://g
-00000d90: 6974 6875 622e 636f 6d2f 6e61 7361 6861  ithub.com/nasaha
-00000da0: 7276 6573 742f 6372 6f70 6861 7276 6573  rvest/cropharves
-00000db0: 742f 626c 6f62 2f6d 6169 6e2f 6265 6e63  t/blob/main/benc
-00000dc0: 686d 6172 6b73 292e 0a0a 2323 2320 436f  hmarks)...### Co
-00000dd0: 6e74 7269 6275 7469 6e67 0a49 6620 796f  ntributing.If yo
-00000de0: 7520 776f 756c 6420 6c69 6b65 2074 6f20  u would like to 
-00000df0: 636f 6e74 7269 6275 7465 2061 2064 6174  contribute a dat
-00000e00: 6173 6574 2c20 706c 6561 7365 2073 6565  aset, please see
-00000e10: 2074 6865 205b 636f 6e74 7269 6275 7469   the [contributi
-00000e20: 6e67 2072 6561 646d 655d 2868 7474 7073  ng readme](https
-00000e30: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e61  ://github.com/na
-00000e40: 7361 6861 7276 6573 742f 6372 6f70 6861  saharvest/cropha
-00000e50: 7276 6573 742f 626c 6f62 2f6d 6169 6e2f  rvest/blob/main/
-00000e60: 636f 6e74 7269 6275 7469 6e67 2e6d 6429  contributing.md)
-00000e70: 2e0a 0a23 2323 207e 7e46 4151 7e7e 2051  ...### ~~FAQ~~ Q
-00000e80: 7565 7374 696f 6e73 2061 736b 6564 2061  uestions asked a
-00000e90: 7420 6c65 6173 7420 6f6e 6365 0a0a 3c64  t least once..<d
-00000ea0: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
-00000eb0: 3e3c 6120 6872 6566 3d68 7474 7073 3a2f  ><a href=https:/
-00000ec0: 2f67 6974 6875 622e 636f 6d2f 6e61 7361  /github.com/nasa
-00000ed0: 6861 7276 6573 742f 6372 6f70 6861 7276  harvest/cropharv
-00000ee0: 6573 742f 6973 7375 6573 2f39 353e 486f  est/issues/95>Ho
-00000ef0: 7720 646f 2049 2075 7365 2043 726f 7048  w do I use CropH
-00000f00: 6172 7665 7374 2066 6f72 2061 2073 7065  arvest for a spe
-00000f10: 6369 6669 6320 6765 6f67 7261 7068 793f  cific geography?
-00000f20: 3c2f 613e 3c2f 7375 6d6d 6172 793e 0a0a  </a></summary>..
-00000f30: 416c 6c20 7468 6520 6461 7461 2069 7320  All the data is 
-00000f40: 6163 6365 7373 6962 6c65 2074 6872 6f75  accessible throu
-00000f50: 6768 2074 6865 2060 6372 6f70 6861 7276  gh the `cropharv
-00000f60: 6573 742e 6461 7461 7365 7473 2e43 726f  est.datasets.Cro
-00000f70: 7048 6172 7665 7374 6020 6f62 6a65 6374  pHarvest` object
-00000f80: 2e20 5468 6520 6d61 696e 2070 6172 616d  . The main param
-00000f90: 6574 6572 7320 7768 6963 6820 796f 7520  eters which you 
-00000fa0: 6d69 6768 7420 6265 2069 6e74 6572 6573  might be interes
-00000fb0: 7465 6420 696e 206d 616e 6970 756c 6174  ted in manipulat
-00000fc0: 696e 6720 6172 6520 636f 6e74 726f 6c6c  ing are controll
-00000fd0: 6162 6c65 2074 6872 6f75 6768 2061 2060  able through a `
-00000fe0: 6372 6f70 6861 7276 6573 742e 6461 7461  cropharvest.data
-00000ff0: 7365 7473 2e54 6173 6b60 2c20 7768 6963  sets.Task`, whic
-00001000: 6820 7461 6b65 7320 6173 2069 6e70 7574  h takes as input
-00001010: 2074 6865 2066 6f6c 6c6f 7769 6e67 2070   the following p
-00001020: 6172 616d 6574 6572 733a 0a2d 2041 2062  arameters:.- A b
-00001030: 6f75 6e64 696e 6720 626f 782c 2077 6869  ounding box, whi
-00001040: 6368 2064 6566 696e 6573 2074 6865 2073  ch defines the s
-00001050: 7061 7469 616c 2062 6f75 6e64 6172 6965  patial boundarie
-00001060: 7320 6f66 2074 6865 206c 6162 656c 7320  s of the labels 
-00001070: 7265 7472 6965 7665 730a 2d20 4120 7461  retrieves.- A ta
-00001080: 7267 6574 206c 6162 656c 2c20 7768 6963  rget label, whic
-00001090: 6820 6465 6669 6e65 7320 7468 6520 636c  h defines the cl
-000010a0: 6173 7320 6f66 2074 6865 2070 6f73 6974  ass of the posit
-000010b0: 6976 6520 6c61 6265 6c73 2028 6966 2074  ive labels (if t
-000010c0: 6869 7320 6973 206c 6566 7420 746f 2060  his is left to `
-000010d0: 4e6f 6e65 602c 2074 6865 6e20 7468 6520  None`, then the 
-000010e0: 706f 7369 7469 7665 2063 6c61 7373 2077  positive class w
-000010f0: 696c 6c20 6265 2063 726f 7073 2061 6e64  ill be crops and
-00001100: 2074 6865 206e 6567 6174 6976 6520 636c   the negative cl
-00001110: 6173 7320 7769 6c6c 2062 6520 6e6f 6e2d  ass will be non-
-00001120: 6372 6f70 7329 0a2d 2041 2062 6f6f 6c65  crops).- A boole
-00001130: 616e 2064 6566 696e 696e 6720 7768 6574  an defining whet
-00001140: 6865 7220 6f72 206e 6f74 2074 6f20 6261  her or not to ba
-00001150: 6c61 6e63 6520 7468 6520 6372 6f70 7320  lance the crops 
-00001160: 616e 6420 6e6f 6e2d 6372 6f70 7320 696e  and non-crops in
-00001170: 2074 6865 206e 6567 6174 6976 6520 636c   the negative cl
-00001180: 6173 730a 2d20 4120 7465 7374 5f69 6465  ass.- A test_ide
-00001190: 6e74 6966 6965 7220 7374 7269 6e67 2c20  ntifier string, 
-000011a0: 7768 6963 6820 7465 6c6c 7320 7468 6520  which tells the 
-000011b0: 6461 7461 7365 7420 7768 6574 6865 7220  dataset whether 
-000011c0: 6f72 206e 6f74 2074 6f20 7265 7472 6965  or not to retrie
-000011d0: 7665 2061 2066 696c 6520 6672 6f6d 2074  ve a file from t
-000011e0: 6865 2060 7465 7374 5f66 6561 7475 7265  he `test_feature
-000011f0: 7360 2066 6f6c 6465 7220 616e 6420 7265  s` folder and re
-00001200: 7475 726e 2069 7420 6173 2074 6865 2074  turn it as the t
-00001210: 6573 7420 6461 7461 2e0a 0a53 6f20 6966  est data...So if
-00001220: 2049 2077 616e 7465 6420 746f 2075 7365   I wanted to use
-00001230: 2074 6869 7320 746f 2074 7261 696e 2061   this to train a
-00001240: 206d 6f64 656c 2074 6f20 6964 656e 7469   model to identi
-00001250: 6679 2063 726f 7020 7673 2e20 6e6f 6e20  fy crop vs. non 
-00001260: 6372 6f70 2069 6e20 4672 616e 6365 2c20  crop in France, 
-00001270: 4920 6d69 6768 7420 646f 2069 7420 6c69  I might do it li
-00001280: 6b65 2074 6869 733a 0a0a 6060 6070 7974  ke this:..```pyt
-00001290: 686f 6e0a 6672 6f6d 2073 6b6c 6561 726e  hon.from sklearn
-000012a0: 2e65 6e73 656d 626c 6520 696d 706f 7274  .ensemble import
-000012b0: 2052 616e 646f 6d46 6f72 6573 7443 6c61   RandomForestCla
-000012c0: 7373 6966 6965 720a 0a66 726f 6d20 6372  ssifier..from cr
-000012d0: 6f70 6861 7276 6573 742e 6461 7461 7365  opharvest.datase
-000012e0: 7473 2069 6d70 6f72 7420 5461 736b 2c20  ts import Task, 
-000012f0: 4372 6f70 4861 7276 6573 740a 6672 6f6d  CropHarvest.from
-00001300: 2063 726f 7068 6172 7665 7374 2e63 6f75   cropharvest.cou
-00001310: 6e74 7269 6573 2069 6d70 6f72 7420 6765  ntries import ge
-00001320: 745f 636f 756e 7472 795f 6262 6f78 0a0a  t_country_bbox..
-00001330: 2320 666f 6c64 6572 2069 6e74 6f20 7768  # folder into wh
-00001340: 6963 6820 7468 6520 6461 7461 2077 696c  ich the data wil
-00001350: 6c20 6265 2064 6f77 6e6c 6f61 6465 6420  l be downloaded 
-00001360: 2f20 616c 7265 6164 7920 6578 6973 7473  / already exists
-00001370: 0a64 6174 615f 6469 7220 3d20 2264 6174  .data_dir = "dat
-00001380: 6122 0a0a 2320 6765 745f 636f 756e 7472  a"..# get_countr
-00001390: 795f 6262 6f78 2072 6574 7572 6e73 2061  y_bbox returns a
-000013a0: 206c 6973 7420 6f66 2062 6f75 6e64 696e   list of boundin
-000013b0: 6720 626f 7865 732e 0a23 2074 6865 206f  g boxes..# the o
-000013c0: 6e65 2072 6570 7265 7365 6e74 696e 6720  ne representing 
-000013d0: 4d65 7472 6f70 6f6c 6974 616e 2046 7261  Metropolitan Fra
-000013e0: 6e63 6520 6973 2074 6865 2032 6e64 2062  nce is the 2nd b
-000013f0: 6f78 0a6d 6574 726f 706f 6c69 7461 6e5f  ox.metropolitan_
-00001400: 6672 616e 6365 5f62 626f 7820 3d20 6765  france_bbox = ge
-00001410: 745f 636f 756e 7472 795f 6262 6f78 2822  t_country_bbox("
-00001420: 4672 616e 6365 2229 5b31 5d0a 0a74 6173  France")[1]..tas
-00001430: 6b20 3d20 5461 736b 2862 6f75 6e64 696e  k = Task(boundin
-00001440: 675f 626f 783d 6d65 7472 6f70 6f6c 6974  g_box=metropolit
-00001450: 616e 5f66 7261 6e63 655f 6262 6f78 2c20  an_france_bbox, 
-00001460: 6e6f 726d 616c 697a 653d 5472 7565 290a  normalize=True).
-00001470: 0a6d 795f 6461 7461 7365 7420 3d20 4372  .my_dataset = Cr
-00001480: 6f70 4861 7276 6573 7428 6461 7461 5f64  opHarvest(data_d
-00001490: 6972 2c20 7461 736b 290a 0a58 2c20 7920  ir, task)..X, y 
-000014a0: 3d20 6d79 5f64 6174 6173 6574 2e61 735f  = my_dataset.as_
-000014b0: 6172 7261 7928 666c 6174 7465 6e5f 783d  array(flatten_x=
-000014c0: 5472 7565 290a 6d6f 6465 6c20 3d20 5261  True).model = Ra
-000014d0: 6e64 6f6d 466f 7265 7374 436c 6173 7369  ndomForestClassi
-000014e0: 6669 6572 2872 616e 646f 6d5f 7374 6174  fier(random_stat
-000014f0: 653d 3029 0a6d 6f64 656c 2e66 6974 2858  e=0).model.fit(X
-00001500: 2c20 7929 0a60 6060 0a3c 2f64 6574 6169  , y).```.</detai
-00001510: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a3c  ls>..<details>.<
-00001520: 7375 6d6d 6172 793e 3c61 2068 7265 663d  summary><a href=
-00001530: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001540: 6f6d 2f6e 6173 6168 6172 7665 7374 2f63  om/nasaharvest/c
-00001550: 726f 7068 6172 7665 7374 2f69 7373 7565  ropharvest/issue
-00001560: 732f 3130 363e 486f 7720 646f 2049 206c  s/106>How do I l
-00001570: 6f61 6420 6120 7370 6563 6966 6963 2070  oad a specific p
-00001580: 6978 656c 2074 696d 6573 6572 6965 733f  ixel timeseries?
-00001590: 3c2f 613e 3c2f 7375 6d6d 6172 793e 0a0a  </a></summary>..
-000015a0: 5468 6520 3c61 2068 7265 663d 6874 7470  The <a href=http
-000015b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
-000015c0: 6173 6168 6172 7665 7374 2f63 726f 7068  asaharvest/croph
-000015d0: 6172 7665 7374 2f69 7373 7565 732f 3130  arvest/issues/10
-000015e0: 363e 7370 6563 6966 6963 2075 7365 2063  6>specific use c
-000015f0: 6173 653c 2f61 3e20 6865 7265 2069 7320  ase</a> here is 
-00001600: 746f 2072 6574 7269 6576 6520 4e44 5649  to retrieve NDVI
-00001610: 2076 616c 7565 7320 666f 7220 6120 7370   values for a sp
-00001620: 6563 6966 6963 2072 6f77 2069 6e20 7468  ecific row in th
-00001630: 6520 606c 6162 656c 732e 6765 6f6a 736f  e `labels.geojso
-00001640: 6e60 2e20 4865 7265 2069 7320 686f 7720  n`. Here is how 
-00001650: 796f 7520 6d69 6768 7420 676f 2061 626f  you might go abo
-00001660: 7574 2064 6f69 6e67 2074 6861 743a 0a0a  ut doing that:..
-00001670: 4669 7273 746c 792c 2049 2077 696c 6c20  Firstly, I will 
-00001680: 6c6f 6164 2074 6865 2067 656f 736a 6f6e  load the geosjon
-00001690: 2e20 4927 6c6c 2064 6f20 6974 2074 6872  . I'll do it thr
-000016a0: 6f75 6768 2061 2060 4372 6f70 4861 7276  ough a `CropHarv
-000016b0: 6573 744c 6162 656c 7360 206f 626a 6563  estLabels` objec
-000016c0: 742c 2077 6869 6368 2069 7320 6a75 7374  t, which is just
-000016d0: 2061 2077 7261 7070 6572 2061 726f 756e   a wrapper aroun
-000016e0: 6420 7468 6520 6765 6f6a 736f 6e20 6275  d the geojson bu
-000016f0: 7420 7072 6f76 6964 6573 2073 6f6d 6520  t provides some 
-00001700: 6e69 6365 2075 7469 6c69 7479 2066 756e  nice utility fun
-00001710: 6374 696f 6e73 2e0a 6060 6070 7974 686f  ctions..```pytho
-00001720: 6e0a 3e3e 3e20 6672 6f6d 2063 726f 7068  n.>>> from croph
-00001730: 6172 7665 7374 2e64 6174 6173 6574 7320  arvest.datasets 
-00001740: 696d 706f 7274 2043 726f 7048 6172 7665  import CropHarve
-00001750: 7374 4c61 6265 6c73 0a3e 3e3e 0a3e 3e3e  stLabels.>>>.>>>
-00001760: 206c 6162 656c 7320 3d20 4372 6f70 4861   labels = CropHa
-00001770: 7276 6573 744c 6162 656c 7328 2263 726f  rvestLabels("cro
-00001780: 7068 6172 7665 7374 2f64 6174 6122 290a  pharvest/data").
-00001790: 3e3e 3e20 6c61 6265 6c73 5f67 656f 6a73  >>> labels_geojs
-000017a0: 6f6e 203d 206c 6162 656c 732e 6173 5f67  on = labels.as_g
-000017b0: 656f 6a73 6f6e 2829 0a3e 3e3e 206c 6162  eojson().>>> lab
-000017c0: 656c 735f 6765 6f6a 736f 6e2e 6865 6164  els_geojson.head
-000017d0: 2829 0a20 2068 6172 7665 7374 5f64 6174  ().  harvest_dat
-000017e0: 6520 706c 616e 7469 6e67 5f64 6174 6520  e planting_date 
-000017f0: 202e 2e2e 2069 735f 7465 7374 2020 2020   ... is_test    
-00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001820: 2020 2020 2020 2067 656f 6d65 7472 790a         geometry.
-00001830: 3020 2020 2020 2020 2020 4e6f 6e65 2020  0         None  
-00001840: 2020 2020 2020 2020 4e6f 6e65 2020 2e2e          None  ..
-00001850: 2e20 2020 4661 6c73 6520 2050 4f4c 5947  .   False  POLYG
-00001860: 4f4e 2028 2833 372e 3038 3235 3220 3130  ON ((37.08252 10
-00001870: 2e37 3132 3734 2c20 3337 2e30 3833 3438  .71274, 37.08348
-00001880: 2031 302e 3731 3239 312e 2e2e 0a31 2020   10.71291....1  
-00001890: 2020 2020 2020 204e 6f6e 6520 2020 2020         None     
-000018a0: 2020 2020 204e 6f6e 6520 202e 2e2e 2020       None  ...  
-000018b0: 2046 616c 7365 2020 504f 4c59 474f 4e20   False  POLYGON 
-000018c0: 2828 3337 2e30 3837 3231 2031 302e 3732  ((37.08721 10.72
-000018d0: 3339 382c 2033 372e 3038 3731 3420 3130  398, 37.08714 10
-000018e0: 2e37 3234 3239 2e2e 2e0a 3220 2020 2020  .72429....2     
-000018f0: 2020 2020 4e6f 6e65 2020 2020 2020 2020      None        
-00001900: 2020 4e6f 6e65 2020 2e2e 2e20 2020 4661    None  ...   Fa
-00001910: 6c73 6520 2050 4f4c 5947 4f4e 2028 2833  lse  POLYGON ((3
-00001920: 372e 3038 3439 3820 3130 2e37 3133 3731  7.08498 10.71371
-00001930: 2c20 3337 2e30 3834 3831 2031 302e 3731  , 37.08481 10.71
-00001940: 3339 332e 2e2e 0a33 2020 2020 2020 2020  393....3        
-00001950: 204e 6f6e 6520 2020 2020 2020 2020 204e   None          N
-00001960: 6f6e 6520 202e 2e2e 2020 2046 616c 7365  one  ...   False
-00001970: 2020 504f 4c59 474f 4e20 2828 3337 2e30    POLYGON ((37.0
-00001980: 3930 3231 2031 302e 3731 3332 302c 2033  9021 10.71320, 3
-00001990: 372e 3039 3031 3420 3130 2e37 3133 3431  7.09014 10.71341
-000019a0: 2e2e 2e0a 3420 2020 2020 2020 2020 4e6f  ....4         No
-000019b0: 6e65 2020 2020 2020 2020 2020 4e6f 6e65  ne          None
-000019c0: 2020 2e2e 2e20 2020 4661 6c73 6520 2050    ...   False  P
-000019d0: 4f4c 5947 4f4e 2028 2833 372e 3038 3330  OLYGON ((37.0830
-000019e0: 3720 3130 2e37 3231 3630 2c20 3337 2e30  7 10.72160, 37.0
-000019f0: 3832 3831 2031 302e 3732 3139 372e 2e2e  8281 10.72197...
-00001a00: 0a0a 5b35 2072 6f77 7320 7820 3133 2063  ..[5 rows x 13 c
-00001a10: 6f6c 756d 6e73 5d0a 6060 600a 0a4e 6f77  olumns].```..Now
-00001a20: 2c20 4920 6361 6e20 7573 6520 7468 6520  , I can use the 
-00001a30: 606c 6162 656c 7360 206f 626a 6563 7420  `labels` object 
-00001a40: 746f 2072 6574 7269 6576 6520 7468 6520  to retrieve the 
-00001a50: 6669 6c65 7061 7468 206f 6620 7468 6520  filepath of the 
-00001a60: 7072 6f63 6573 7365 6420 7361 7465 6c6c  processed satell
-00001a70: 6974 6520 6461 7461 2066 6f72 2065 6163  ite data for eac
-00001a80: 6820 726f 7720 696e 2074 6865 206c 6162  h row in the lab
-00001a90: 656c 7320 6765 6f6a 736f 6e3a 0a60 6060  els geojson:.```
-00001aa0: 7079 7468 6f6e 0a3e 3e3e 2070 6174 685f  python.>>> path_
-00001ab0: 746f 5f66 696c 6520 3d20 6c61 6265 6c73  to_file = labels
-00001ac0: 2e5f 7061 7468 5f66 726f 6d5f 726f 7728  ._path_from_row(
-00001ad0: 6c61 6265 6c73 5f67 656f 6a73 6f6e 2e69  labels_geojson.i
-00001ae0: 6c6f 635b 305d 290a 6060 600a 5468 6973  loc[0]).```.This
-00001af0: 2070 726f 6365 7373 6564 2073 6174 656c   processed satel
-00001b00: 6c69 7465 2064 6174 6120 6973 2073 746f  lite data is sto
-00001b10: 7265 6420 6173 2060 6835 7079 6020 6669  red as `h5py` fi
-00001b20: 6c65 732c 2073 6f20 4920 6361 6e20 6c6f  les, so I can lo
-00001b30: 6164 2069 7420 7570 2061 7320 666f 6c6c  ad it up as foll
-00001b40: 6f77 733a 0a60 6060 7079 7468 6f6e 0a3e  ows:.```python.>
-00001b50: 3e3e 2069 6d70 6f72 7420 6835 7079 0a3e  >> import h5py.>
-00001b60: 3e3e 2068 3570 795f 6669 6c65 203d 2068  >> h5py_file = h
-00001b70: 3570 792e 4669 6c65 2870 6174 685f 746f  5py.File(path_to
-00001b80: 5f66 696c 652c 2022 7222 290a 3e3e 3e20  _file, "r").>>> 
-00001b90: 7820 3d20 6835 7079 5f66 696c 652e 6765  x = h5py_file.ge
-00001ba0: 7428 2261 7272 6179 2229 5b3a 5d0a 3e3e  t("array")[:].>>
-00001bb0: 3e20 782e 7368 6170 650a 2831 322c 2031  > x.shape.(12, 1
-00001bc0: 3829 0a60 6060 0a54 6865 2073 6861 7065  8).```.The shape
-00001bd0: 206f 6620 6078 6020 7265 7072 6573 656e   of `x` represen
-00001be0: 7473 2031 3220 7469 6d65 7374 6570 7320  ts 12 timesteps 
-00001bf0: 616e 6420 3138 2062 616e 6473 2e20 546f  and 18 bands. To
-00001c00: 2072 6574 7269 6576 6520 7468 6520 6261   retrieve the ba
-00001c10: 6e64 2049 2061 6d20 696e 7465 7265 7374  nd I am interest
-00001c20: 6564 2069 6e3a 0a60 6060 7079 7468 6f6e  ed in:.```python
-00001c30: 0a3e 3e3e 2066 726f 6d20 6372 6f70 6861  .>>> from cropha
-00001c40: 7276 6573 742e 6261 6e64 7320 696d 706f  rvest.bands impo
-00001c50: 7274 2042 414e 4453 0a3e 3e3e 2078 5b3a  rt BANDS.>>> x[:
-00001c60: 2c20 4241 4e44 532e 696e 6465 7828 224e  , BANDS.index("N
-00001c70: 4456 4922 295d 0a61 7272 6179 285b 302e  DVI")].array([0.
-00001c80: 3238 3939 3230 3732 2c20 302e 3238 3833  28992072, 0.2883
-00001c90: 3833 3433 2c20 302e 3236 3833 3335 3739  8343, 0.26833579
-00001ca0: 2c20 302e 3232 3537 3736 3333 2c20 302e  , 0.22577633, 0.
-00001cb0: 3237 3133 3839 3836 2c0a 2020 2020 2020  27138986,.      
-00001cc0: 2030 2e30 3635 3834 3131 342c 2030 2e34   0.06584114, 0.4
-00001cd0: 3938 3939 3820 202c 2030 2e35 3031 3437  98998  , 0.50147
-00001ce0: 3230 332c 2030 2e35 3034 3337 3734 332c  203, 0.50437743,
-00001cf0: 2030 2e34 3433 3236 3334 332c 0a20 2020   0.44326343,.   
-00001d00: 2020 2020 302e 3333 3733 3538 3439 2c20      0.33735849, 
-00001d10: 302e 3238 3337 3539 3637 5d29 0a60 6060  0.28375967]).```
-00001d20: 0a54 6865 7365 2061 7265 2031 3220 4e44  .These are 12 ND
-00001d30: 5649 2076 616c 7565 732c 2063 6f72 7265  VI values, corre
-00001d40: 7370 6f6e 6469 6e67 2074 6f20 7468 6520  sponding to the 
-00001d50: 3132 206d 6f6e 7468 7320 6361 7074 7572  12 months captur
-00001d60: 6564 2069 6e20 7468 6973 2074 696d 6573  ed in this times
-00001d70: 6572 6965 732e 2054 6f20 6669 6e64 206f  eries. To find o
-00001d80: 7574 2065 7861 6374 6c79 2077 6869 6368  ut exactly which
-00001d90: 206d 6f6e 7468 2065 6163 6820 7469 6d65   month each time
-00001da0: 7374 6570 2072 6570 7265 7365 6e74 732c  step represents,
-00001db0: 2049 2063 616e 2064 6f0a 6060 6070 7974   I can do.```pyt
-00001dc0: 686f 6e0a 3e3e 3e20 6c61 6265 6c73 5f67  hon.>>> labels_g
-00001dd0: 656f 6a73 6f6e 2e69 6c6f 635b 305d 2e65  eojson.iloc[0].e
-00001de0: 7870 6f72 745f 656e 645f 6461 7465 0a27  xport_end_date.'
-00001df0: 3230 3231 2d30 322d 3031 5430 303a 3030  2021-02-01T00:00
-00001e00: 3a30 3027 0a60 6060 0a57 6963 6820 7465  :00'.```.Wich te
-00001e10: 6c6c 7320 6d65 2074 6861 7420 7468 6520  lls me that the 
-00001e20: 6c61 7374 2074 696d 6573 7465 7020 7265  last timestep re
-00001e30: 7072 6573 656e 7473 204a 616e 7561 7279  presents January
-00001e40: 2032 3032 312e 2049 2063 616e 2077 6f72   2021. I can wor
-00001e50: 6b20 6261 636b 7761 7264 7320 6672 6f6d  k backwards from
-00001e60: 2074 6865 7265 2e0a 0a3c 2f64 6574 6169   there...</detai
-00001e70: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a3c  ls>..<details>.<
-00001e80: 7375 6d6d 6172 793e 3c61 2068 7265 663d  summary><a href=
-00001e90: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00001ea0: 636f 6d2f 6e61 7361 6861 7276 6573 742f  com/nasaharvest/
-00001eb0: 6372 6f70 6861 7276 6573 742f 6973 7375  cropharvest/issu
-00001ec0: 6573 2f38 3822 3e57 6861 7420 6973 2074  es/88">What is t
-00001ed0: 6865 2064 6174 6120 666f 726d 6174 3f3c  he data format?<
-00001ee0: 2f61 3e3c 2f73 756d 6d61 7279 3e0a 5468  /a></summary>.Th
-00001ef0: 6520 7374 7275 6374 7572 6520 6f66 2074  e structure of t
-00001f00: 6865 2064 6966 6665 7265 6e74 2064 6174  he different dat
-00001f10: 6120 6669 6c65 7320 6973 206e 6f77 2064  a files is now d
-00001f20: 6573 6372 6962 6564 2069 6e20 6465 7074  escribed in dept
-00001f30: 6820 696e 2074 6865 2064 6174 6120 666f  h in the data fo
-00001f40: 6c64 6572 2773 205b 5265 6164 6d65 5d28  lder's [Readme](
-00001f50: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001f60: 6f6d 2f6e 6173 6168 6172 7665 7374 2f63  om/nasaharvest/c
-00001f70: 726f 7068 6172 7665 7374 2f62 6c6f 622f  ropharvest/blob/
-00001f80: 6d61 696e 2f64 6174 612f 5245 4144 4d45  main/data/README
-00001f90: 2e6d 6429 0a3c 2f64 6574 6169 6c73 3e0a  .md).</details>.
-00001fa0: 0a23 2323 204c 6963 656e 7365 0a43 726f  .### License.Cro
-00001fb0: 7048 6172 7665 7374 2068 6173 2061 205b  pHarvest has a [
-00001fc0: 4372 6561 7469 7665 2043 6f6d 6d6f 6e73  Creative Commons
-00001fd0: 2041 7474 7269 6275 7469 6f6e 2d53 6861   Attribution-Sha
-00001fe0: 7265 416c 696b 6520 342e 3020 496e 7465  reAlike 4.0 Inte
-00001ff0: 726e 6174 696f 6e61 6c5d 2868 7474 7073  rnational](https
-00002000: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e61  ://github.com/na
-00002010: 7361 6861 7276 6573 742f 6372 6f70 6861  saharvest/cropha
-00002020: 7276 6573 742f 626c 6f62 2f6d 6169 6e2f  rvest/blob/main/
-00002030: 4c49 4345 4e53 452e 7478 7429 206c 6963  LICENSE.txt) lic
-00002040: 656e 7365 2e0a 0a23 2323 2043 6974 6174  ense...### Citat
-00002050: 696f 6e0a 0a49 6620 796f 7520 7573 6520  ion..If you use 
-00002060: 4372 6f70 4861 7276 6573 7420 696e 2079  CropHarvest in y
-00002070: 6f75 7220 7265 7365 6172 6368 2c20 706c  our research, pl
-00002080: 6561 7365 2075 7365 2074 6865 2066 6f6c  ease use the fol
-00002090: 6c6f 7769 6e67 2063 6974 6174 696f 6e3a  lowing citation:
-000020a0: 0a60 6060 0a40 696e 7072 6f63 6565 6469  .```.@inproceedi
-000020b0: 6e67 737b 0a20 2020 2074 7365 6e67 3230  ngs{.    tseng20
-000020c0: 3231 6372 6f70 6861 7276 6573 742c 0a20  21cropharvest,. 
-000020d0: 2020 2074 6974 6c65 3d7b 4372 6f70 4861     title={CropHa
-000020e0: 7276 6573 743a 2041 2067 6c6f 6261 6c20  rvest: A global 
-000020f0: 6461 7461 7365 7420 666f 7220 6372 6f70  dataset for crop
-00002100: 2d74 7970 6520 636c 6173 7369 6669 6361  -type classifica
-00002110: 7469 6f6e 7d2c 0a20 2020 2061 7574 686f  tion},.    autho
-00002120: 723d 7b47 6162 7269 656c 2054 7365 6e67  r={Gabriel Tseng
-00002130: 2061 6e64 2049 7661 6e20 5a76 6f6e 6b6f   and Ivan Zvonko
-00002140: 7620 616e 6420 4361 7468 6572 696e 6520  v and Catherine 
-00002150: 4c69 6c69 616e 204e 616b 616c 656d 6265  Lilian Nakalembe
-00002160: 2061 6e64 2048 616e 6e61 6820 4b65 726e   and Hannah Kern
-00002170: 6572 7d2c 0a20 2020 2062 6f6f 6b74 6974  er},.    booktit
-00002180: 6c65 3d7b 5468 6972 7479 2d66 6966 7468  le={Thirty-fifth
-00002190: 2043 6f6e 6665 7265 6e63 6520 6f6e 204e   Conference on N
-000021a0: 6575 7261 6c20 496e 666f 726d 6174 696f  eural Informatio
-000021b0: 6e20 5072 6f63 6573 7369 6e67 2053 7973  n Processing Sys
-000021c0: 7465 6d73 2044 6174 6173 6574 7320 616e  tems Datasets an
-000021d0: 6420 4265 6e63 686d 6172 6b73 2054 7261  d Benchmarks Tra
-000021e0: 636b 2028 526f 756e 6420 3229 7d2c 0a20  ck (Round 2)},. 
-000021f0: 2020 2079 6561 723d 7b32 3032 317d 2c0a     year={2021},.
-00002200: 2020 2020 7572 6c3d 7b68 7474 7073 3a2f      url={https:/
-00002210: 2f6f 7065 6e72 6576 6965 772e 6e65 742f  /openreview.net/
-00002220: 666f 7275 6d3f 6964 3d4a 746a 7a55 5850  forum?id=JtjzUXP
-00002230: 4561 4375 7d0a 7d0a 6060 600a            EaCu}.}.```.
+000001c0: 653a 204c 4943 454e 5345 2e74 7874 0a52  e: LICENSE.txt.R
+000001d0: 6571 7569 7265 732d 4469 7374 3a20 7061  equires-Dist: pa
+000001e0: 6e64 6173 3c32 2e30 2e30 0a52 6571 7569  ndas<2.0.0.Requi
+000001f0: 7265 732d 4469 7374 3a20 6765 6f70 616e  res-Dist: geopan
+00000200: 6461 733d 3d30 2e39 2e30 0a52 6571 7569  das==0.9.0.Requi
+00000210: 7265 732d 4469 7374 3a20 7861 7272 6179  res-Dist: xarray
+00000220: 3c30 2e32 302e 302c 3e3d 302e 3136 2e32  <0.20.0,>=0.16.2
+00000230: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000240: 7471 646d 3e3d 342e 3631 2e31 0a52 6571  tqdm>=4.61.1.Req
+00000250: 7569 7265 732d 4469 7374 3a20 6835 7079  uires-Dist: h5py
+00000260: 213d 332e 372e 302c 3e3d 332e 312e 300a  !=3.7.0,>=3.1.0.
+00000270: 5265 7175 6972 6573 2d44 6973 743a 2072  Requires-Dist: r
+00000280: 6173 7465 7269 6f3e 3d31 2e32 2e36 0a52  asterio>=1.2.6.R
+00000290: 6571 7569 7265 732d 4469 7374 3a20 6f70  equires-Dist: op
+000002a0: 656e 7079 786c 3e3d 322e 352e 390a 5265  enpyxl>=2.5.9.Re
+000002b0: 7175 6972 6573 2d44 6973 743a 2073 6369  quires-Dist: sci
+000002c0: 6b69 742d 6c65 6172 6e3e 3d30 2e32 322e  kit-learn>=0.22.
+000002d0: 320a 0a23 2043 726f 7048 6172 7665 7374  2..# CropHarvest
+000002e0: 0a0a 4372 6f70 4861 7276 6573 7420 6973  ..CropHarvest is
+000002f0: 2061 6e20 6f70 656e 2073 6f75 7263 6520   an open source 
+00000300: 7265 6d6f 7465 2073 656e 7369 6e67 2064  remote sensing d
+00000310: 6174 6173 6574 2066 6f72 2061 6772 6963  ataset for agric
+00000320: 756c 7475 7265 2077 6974 6820 6265 6e63  ulture with benc
+00000330: 686d 6172 6b73 2e20 4974 2063 6f6c 6c65  hmarks. It colle
+00000340: 6374 7320 6461 7461 2066 726f 6d20 6120  cts data from a 
+00000350: 7661 7269 6574 7920 6f66 2061 6772 6963  variety of agric
+00000360: 756c 7475 7261 6c20 6c61 6e64 2075 7365  ultural land use
+00000370: 2064 6174 6173 6574 7320 616e 6420 7265   datasets and re
+00000380: 6d6f 7465 2073 656e 7369 6e67 2070 726f  mote sensing pro
+00000390: 6475 6374 732e 0a0a 0a54 6865 2064 6174  ducts....The dat
+000003a0: 6173 6574 2063 6f6e 7369 7374 7320 6f66  aset consists of
+000003b0: 202a 2a39 352c 3138 362a 2a20 6461 7461   **95,186** data
+000003c0: 706f 696e 7473 2c20 6f66 2077 6869 6368  points, of which
+000003d0: 202a 2a33 332c 3230 352a 2a20 2833 3525   **33,205** (35%
+000003e0: 2920 6861 7665 206d 756c 7469 636c 6173  ) have multiclas
+000003f0: 7320 6c61 6265 6c73 2e20 416c 6c20 6f74  s labels. All ot
+00000400: 6865 7220 6461 7461 706f 696e 7473 206f  her datapoints o
+00000410: 6e6c 7920 6861 7665 2062 696e 6172 7920  nly have binary 
+00000420: 6372 6f70 202f 206e 6f6e 2d63 726f 7020  crop / non-crop 
+00000430: 6c61 6265 6c73 2e0a 0a2a 2a37 302c 3231  labels...**70,21
+00000440: 332a 2a20 2837 3425 2920 6f66 2074 6865  3** (74%) of the
+00000450: 7365 206c 6162 656c 7320 6172 6520 7061  se labels are pa
+00000460: 6972 6564 2077 6974 6820 7265 6d6f 7465  ired with remote
+00000470: 2073 656e 7369 6e67 2061 6e64 2063 6c69   sensing and cli
+00000480: 6d61 746f 6c6f 6779 2064 6174 612c 2073  matology data, s
+00000490: 7065 6369 6669 6361 6c6c 7920 5b53 656e  pecifically [Sen
+000004a0: 7469 6e65 6c2d 325d 2868 7474 7073 3a2f  tinel-2](https:/
+000004b0: 2f73 656e 7469 6e65 6c2e 6573 612e 696e  /sentinel.esa.in
+000004c0: 742f 7765 622f 7365 6e74 696e 656c 2f6d  t/web/sentinel/m
+000004d0: 6973 7369 6f6e 732f 7365 6e74 696e 656c  issions/sentinel
+000004e0: 2d32 292c 205b 5365 6e74 696e 656c 2d31  -2), [Sentinel-1
+000004f0: 5d28 6874 7470 733a 2f2f 7365 6e74 696e  ](https://sentin
+00000500: 656c 2e65 7361 2e69 6e74 2f77 6562 2f73  el.esa.int/web/s
+00000510: 656e 7469 6e65 6c2f 6d69 7373 696f 6e73  entinel/missions
+00000520: 2f73 656e 7469 6e65 6c2d 312f 292c 2074  /sentinel-1/), t
+00000530: 6865 205b 5352 544d 2044 6967 6974 616c  he [SRTM Digital
+00000540: 2045 6c65 7661 7469 6f6e 204d 6f64 656c   Elevation Model
+00000550: 5d28 6874 7470 733a 2f2f 6367 6961 7263  ](https://cgiarc
+00000560: 7369 2e63 6f6d 6d75 6e69 7479 2f64 6174  si.community/dat
+00000570: 612f 7372 746d 2d39 306d 2d64 6967 6974  a/srtm-90m-digit
+00000580: 616c 2d65 6c65 7661 7469 6f6e 2d64 6174  al-elevation-dat
+00000590: 6162 6173 652d 7634 2d31 2f29 2061 6e64  abase-v4-1/) and
+000005a0: 205b 4552 4120 3520 636c 696d 6174 6f6c   [ERA 5 climatol
+000005b0: 6f67 7920 6461 7461 5d28 6874 7470 733a  ogy data](https:
+000005c0: 2f2f 7777 772e 6563 6d77 662e 696e 742f  //www.ecmwf.int/
+000005d0: 656e 2f66 6f72 6563 6173 7473 2f64 6174  en/forecasts/dat
+000005e0: 6173 6574 732f 7265 616e 616c 7973 6973  asets/reanalysis
+000005f0: 2d64 6174 6173 6574 732f 6572 6135 292e  -datasets/era5).
+00000600: 0a0a 3231 2064 6174 6173 6574 7320 6172  ..21 datasets ar
+00000610: 6520 6167 6772 6567 6174 6564 2069 6e74  e aggregated int
+00000620: 6f20 4372 6f70 4861 7276 6573 7420 2d20  o CropHarvest - 
+00000630: 7468 6573 6520 6172 6520 646f 6375 6d65  these are docume
+00000640: 6e74 6564 205b 6865 7265 5d28 6874 7470  nted [here](http
+00000650: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
+00000660: 6173 6168 6172 7665 7374 2f63 726f 7068  asaharvest/croph
+00000670: 6172 7665 7374 2f62 6c6f 622f 6d61 696e  arvest/blob/main
+00000680: 2f64 6174 6173 6574 732e 6d64 292e 0a0a  /datasets.md)...
+00000690: 4d6f 7265 2064 6574 6169 6c73 2061 626f  More details abo
+000006a0: 7574 2043 726f 7048 6172 7665 7374 2061  ut CropHarvest a
+000006b0: 6e64 2074 6865 2062 656e 6368 6d61 726b  nd the benchmark
+000006c0: 7320 6172 6520 6176 6169 6c61 626c 6520  s are available 
+000006d0: 696e 205b 7468 6973 2070 6170 6572 5d28  in [this paper](
+000006e0: 6874 7470 733a 2f2f 6f70 656e 7265 7669  https://openrevi
+000006f0: 6577 2e6e 6574 2f66 6f72 756d 3f69 643d  ew.net/forum?id=
+00000700: 4a74 6a7a 5558 5045 6143 7529 2e0a 0a23  JtjzUXPEaCu)...#
+00000710: 2323 2050 6970 656c 696e 650a 5468 6520  ## Pipeline.The 
+00000720: 636f 6465 2069 6e20 7468 6973 2072 6570  code in this rep
+00000730: 6f73 6974 6f72 790a 0a31 2920 636f 6d62  ository..1) comb
+00000740: 696e 6573 2074 6865 2063 6f6e 7374 6974  ines the constit
+00000750: 7565 6e74 2064 6174 6173 6574 7320 696e  uent datasets in
+00000760: 746f 2061 2073 696e 676c 6520 6765 6f4a  to a single geoJ
+00000770: 534f 4e20 6669 6c65 2c0a 3229 2065 7870  SON file,.2) exp
+00000780: 6f72 7473 2074 6865 2061 7373 6f63 6961  orts the associa
+00000790: 7465 6420 7361 7465 6c6c 6974 6520 6461  ted satellite da
+000007a0: 7461 2066 726f 6d20 4561 7274 6820 456e  ta from Earth En
+000007b0: 6769 6e65 2c0a 3329 2063 6f6d 6269 6e65  gine,.3) combine
+000007c0: 7320 626f 7468 2064 6174 6173 6574 7320  s both datasets 
+000007d0: 746f 2063 7265 6174 6520 6028 582c 7929  to create `(X,y)
+000007e0: 6020 7472 6169 6e69 6e67 2074 7570 6c65  ` training tuple
+000007f0: 7320 616e 640a 3429 2065 7870 6f73 6573  s and.4) exposes
+00000800: 2074 686f 7365 2074 7570 6c65 7320 7669   those tuples vi
+00000810: 6120 6120 6044 6174 6173 6574 6020 6f62  a a `Dataset` ob
+00000820: 6a65 6374 2e0a 0a54 6865 2070 6970 656c  ject...The pipel
+00000830: 696e 6520 7468 726f 7567 6820 7768 6963  ine through whic
+00000840: 6820 7468 6973 2068 6170 7065 6e73 2069  h this happens i
+00000850: 7320 7368 6f77 6e20 6265 6c6f 773a 0a0a  s shown below:..
+00000860: 0a41 6c6c 2062 6c75 6520 626f 7865 7320  .All blue boxes 
+00000870: 6172 6520 6173 736f 6369 6174 6564 2077  are associated w
+00000880: 6974 6820 636f 6465 2069 6e20 7468 6973  ith code in this
+00000890: 2072 6570 6f73 6974 6f72 792e 2041 6e79   repository. Any
+000008a0: 7468 696e 6720 6772 6565 6e20 6973 2064  thing green is d
+000008b0: 6174 6120 6163 6365 7373 6962 6c65 2076  ata accessible v
+000008c0: 6961 205b 5a65 6e6f 646f 5d28 6874 7470  ia [Zenodo](http
+000008d0: 733a 2f2f 7a65 6e6f 646f 2e6f 7267 2f72  s://zenodo.org/r
+000008e0: 6563 6f72 642f 3538 3238 3839 3329 2e20  ecord/5828893). 
+000008f0: 4279 2064 6566 6175 6c74 2c20 7468 6520  By default, the 
+00000900: 5a65 6e6f 646f 2064 6174 6120 7769 6c6c  Zenodo data will
+00000910: 2067 6574 2064 6f77 6e6c 6f61 6465 6420   get downloaded 
+00000920: 746f 2074 6865 205b 6461 7461 2066 6f6c  to the [data fol
+00000930: 6465 725d 2868 7474 7073 3a2f 2f67 6974  der](https://git
+00000940: 6875 622e 636f 6d2f 6e61 7361 6861 7276  hub.com/nasaharv
+00000950: 6573 742f 6372 6f70 6861 7276 6573 742f  est/cropharvest/
+00000960: 7472 6565 2f6d 6169 6e2f 6461 7461 2920  tree/main/data) 
+00000970: 2d20 7468 6520 6461 7461 2066 6f6c 6465  - the data folde
+00000980: 7227 7320 5b52 6561 646d 655d 2868 7474  r's [Readme](htt
+00000990: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000009a0: 6e61 7361 6861 7276 6573 742f 6372 6f70  nasaharvest/crop
+000009b0: 6861 7276 6573 742f 626c 6f62 2f6d 6169  harvest/blob/mai
+000009c0: 6e2f 6461 7461 2f52 4541 444d 452e 6d64  n/data/README.md
+000009d0: 2920 6861 7320 6d6f 7265 2069 6e66 6f72  ) has more infor
+000009e0: 6d61 7469 6f6e 2061 626f 7574 2074 6865  mation about the
+000009f0: 2065 7861 6374 2073 7472 7563 7475 7265   exact structure
+00000a00: 206f 6620 7468 6520 6461 7461 2e0a 0a54   of the data...T
+00000a10: 6865 7265 2061 7265 2075 6e69 7175 6520  here are unique 
+00000a20: 6361 7365 7320 7768 6572 6520 796f 7520  cases where you 
+00000a30: 6d61 7920 6e65 6564 2074 6f20 7573 6520  may need to use 
+00000a40: 7468 6520 6045 6172 7468 456e 6769 6e65  the `EarthEngine
+00000a50: 4578 706f 7274 6572 6020 6469 7265 6374  Exporter` direct
+00000a60: 6c79 2c20 7468 6573 6520 7573 6520 6361  ly, these use ca
+00000a70: 7365 7320 6172 6520 6465 6d6f 6e73 7472  ses are demonstr
+00000a80: 6174 6564 2069 6e20 7468 6520 5b60 6465  ated in the [`de
+00000a90: 6d6f 5f65 7870 6f72 7469 6e67 5f64 6174  mo_exporting_dat
+00000aa0: 612e 6970 796e 6260 5d28 6874 7470 733a  a.ipynb`](https:
+00000ab0: 2f2f 6769 7468 7562 2e63 6f6d 2f6e 6173  //github.com/nas
+00000ac0: 6168 6172 7665 7374 2f63 726f 7068 6172  aharvest/crophar
+00000ad0: 7665 7374 2f62 6c6f 622f 6d61 696e 2f64  vest/blob/main/d
+00000ae0: 656d 6f5f 6578 706f 7274 696e 675f 6461  emo_exporting_da
+00000af0: 7461 2e69 7079 6e62 2920 6e6f 7465 626f  ta.ipynb) notebo
+00000b00: 6f6b 2e0a 0a23 2323 2049 6e73 7461 6c6c  ok...### Install
+00000b10: 6174 696f 6e0a 4c69 6e75 7820 616e 6420  ation.Linux and 
+00000b20: 4d61 634f 5320 7573 6572 7320 6361 6e20  MacOS users can 
+00000b30: 696e 7374 616c 6c20 7468 6520 6c61 7465  install the late
+00000b40: 7374 2076 6572 7369 6f6e 206f 6620 4372  st version of Cr
+00000b50: 6f70 4861 7276 6573 7420 7769 7468 2074  opHarvest with t
+00000b60: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00000b70: 6d61 6e64 3a0a 6060 6062 6173 680a 7069  mand:.```bash.pi
+00000b80: 7020 696e 7374 616c 6c20 6372 6f70 6861  p install cropha
+00000b90: 7276 6573 740a 6060 600a 5769 6e64 6f77  rvest.```.Window
+00000ba0: 7320 7573 6572 7320 6d75 7374 2069 6e73  s users must ins
+00000bb0: 7461 6c6c 2074 6865 2043 726f 7048 6172  tall the CropHar
+00000bc0: 7665 7374 2077 6974 6869 6e20 6120 5b63  vest within a [c
+00000bd0: 6f6e 6461 5d28 6874 7470 733a 2f2f 646f  onda](https://do
+00000be0: 6373 2e63 6f6e 6461 2e69 6f2f 656e 2f6c  cs.conda.io/en/l
+00000bf0: 6174 6573 742f 6d69 6e69 636f 6e64 612e  atest/miniconda.
+00000c00: 6874 6d6c 2920 656e 7669 726f 6e6d 656e  html) environmen
+00000c10: 7420 746f 2065 6e73 7572 6520 616c 6c20  t to ensure all 
+00000c20: 6465 7065 6e64 656e 6369 6573 2061 7265  dependencies are
+00000c30: 2069 6e73 7461 6c6c 6564 2063 6f72 7265   installed corre
+00000c40: 6374 6c79 3a0a 6060 6062 6173 680a 636f  ctly:.```bash.co
+00000c50: 6e64 6120 696e 7374 616c 6c20 2766 696f  nda install 'fio
+00000c60: 6e61 3e3d 312e 3527 2027 7261 7374 6572  na>=1.5' 'raster
+00000c70: 696f 3e3d 312e 322e 3627 0a70 6970 2069  io>=1.2.6'.pip i
+00000c80: 6e73 7461 6c6c 2063 726f 7068 6172 7665  nstall cropharve
+00000c90: 7374 0a60 6060 0a49 6e20 6164 6469 7469  st.```.In additi
+00000ca0: 6f6e 2c20 6974 205b 6d61 7920 6265 206e  on, it [may be n
+00000cb0: 6563 6573 7361 7279 5d28 6874 7470 733a  ecessary](https:
+00000cc0: 2f2f 6769 7468 7562 2e63 6f6d 2f68 3570  //github.com/h5p
+00000cd0: 792f 6835 7079 2f69 7373 7565 732f 3137  y/h5py/issues/17
+00000ce0: 3734 2920 746f 2069 6e73 7461 6c6c 2060  74) to install `
+00000cf0: 6835 7079 6020 7573 696e 6720 636f 6e64  h5py` using cond
+00000d00: 6120 6173 2077 656c 6c20 2860 636f 6e64  a as well (`cond
+00000d10: 6120 696e 7374 616c 6c20 2768 3570 793e  a install 'h5py>
+00000d20: 332e 372e 3027 6029 2070 7269 6f72 2074  3.7.0'`) prior t
+00000d30: 6f20 7069 702d 696e 7374 616c 6c69 6e67  o pip-installing
+00000d40: 2063 726f 7068 6172 7665 7374 2e0a 0a23   cropharvest...#
+00000d50: 2323 2047 6574 7469 6e67 2073 7461 7274  ## Getting start
+00000d60: 6564 205b 215b 4f70 656e 2049 6e20 436f  ed [![Open In Co
+00000d70: 6c61 625d 2868 7474 7073 3a2f 2f63 6f6c  lab](https://col
+00000d80: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
+00000d90: 6c65 2e63 6f6d 2f61 7373 6574 732f 636f  le.com/assets/co
+00000da0: 6c61 622d 6261 6467 652e 7376 6729 5d28  lab-badge.svg)](
+00000db0: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
+00000dc0: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
+00000dd0: 6d2f 6769 7468 7562 2f6e 6173 6168 6172  m/github/nasahar
+00000de0: 7665 7374 2f63 726f 7068 6172 7665 7374  vest/cropharvest
+00000df0: 2f62 6c6f 622f 6d61 696e 2f64 656d 6f2e  /blob/main/demo.
+00000e00: 6970 796e 6229 0a53 6565 2074 6865 205b  ipynb).See the [
+00000e10: 6064 656d 6f2e 6970 796e 6260 5d28 6874  `demo.ipynb`](ht
+00000e20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000e30: 2f6e 6173 6168 6172 7665 7374 2f63 726f  /nasaharvest/cro
+00000e40: 7068 6172 7665 7374 2f62 6c6f 622f 6d61  pharvest/blob/ma
+00000e50: 696e 2f64 656d 6f2e 6970 796e 6229 206e  in/demo.ipynb) n
+00000e60: 6f74 6562 6f6f 6b20 666f 7220 616e 2065  otebook for an e
+00000e70: 7861 6d70 6c65 206f 6e20 686f 7720 746f  xample on how to
+00000e80: 2064 6f77 6e6c 6f61 6420 7468 6520 6461   download the da
+00000e90: 7461 2066 726f 6d20 5b5a 656e 6f64 6f5d  ta from [Zenodo]
+00000ea0: 2868 7474 7073 3a2f 2f7a 656e 6f64 6f2e  (https://zenodo.
+00000eb0: 6f72 672f 7265 636f 7264 2f37 3235 3736  org/record/72576
+00000ec0: 3838 2920 616e 6420 7472 6169 6e20 6120  88) and train a 
+00000ed0: 7261 6e64 6f6d 2066 6f72 6573 7420 6167  random forest ag
+00000ee0: 6169 6e73 7420 7468 6973 2064 6174 612e  ainst this data.
+00000ef0: 0a0a 466f 7220 6d6f 7265 2065 7861 6d70  ..For more examp
+00000f00: 6c65 7320 6f66 206d 6f64 656c 7320 7472  les of models tr
+00000f10: 6169 6e65 6420 6167 6169 6e73 7420 7468  ained against th
+00000f20: 6973 2064 6174 6173 6574 2c20 7365 6520  is dataset, see 
+00000f30: 7468 6520 5b62 656e 6368 6d61 726b 735d  the [benchmarks]
+00000f40: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000f50: 636f 6d2f 6e61 7361 6861 7276 6573 742f  com/nasaharvest/
+00000f60: 6372 6f70 6861 7276 6573 742f 626c 6f62  cropharvest/blob
+00000f70: 2f6d 6169 6e2f 6265 6e63 686d 6172 6b73  /main/benchmarks
+00000f80: 292e 0a0a 2323 2320 436f 6e74 7269 6275  )...### Contribu
+00000f90: 7469 6e67 0a49 6620 796f 7520 776f 756c  ting.If you woul
+00000fa0: 6420 6c69 6b65 2074 6f20 636f 6e74 7269  d like to contri
+00000fb0: 6275 7465 2061 2064 6174 6173 6574 2c20  bute a dataset, 
+00000fc0: 706c 6561 7365 2073 6565 2074 6865 205b  please see the [
+00000fd0: 636f 6e74 7269 6275 7469 6e67 2072 6561  contributing rea
+00000fe0: 646d 655d 2868 7474 7073 3a2f 2f67 6974  dme](https://git
+00000ff0: 6875 622e 636f 6d2f 6e61 7361 6861 7276  hub.com/nasaharv
+00001000: 6573 742f 6372 6f70 6861 7276 6573 742f  est/cropharvest/
+00001010: 626c 6f62 2f6d 6169 6e2f 636f 6e74 7269  blob/main/contri
+00001020: 6275 7469 6e67 2e6d 6429 2e0a 0a23 2323  buting.md)...###
+00001030: 207e 7e46 4151 7e7e 2051 7565 7374 696f   ~~FAQ~~ Questio
+00001040: 6e73 2061 736b 6564 2061 7420 6c65 6173  ns asked at leas
+00001050: 7420 6f6e 6365 0a0a 3c64 6574 6169 6c73  t once..<details
+00001060: 3e0a 3c73 756d 6d61 7279 3e3c 6120 6872  >.<summary><a hr
+00001070: 6566 3d68 7474 7073 3a2f 2f67 6974 6875  ef=https://githu
+00001080: 622e 636f 6d2f 6e61 7361 6861 7276 6573  b.com/nasaharves
+00001090: 742f 6372 6f70 6861 7276 6573 742f 6973  t/cropharvest/is
+000010a0: 7375 6573 2f39 353e 486f 7720 646f 2049  sues/95>How do I
+000010b0: 2075 7365 2043 726f 7048 6172 7665 7374   use CropHarvest
+000010c0: 2066 6f72 2061 2073 7065 6369 6669 6320   for a specific 
+000010d0: 6765 6f67 7261 7068 793f 3c2f 613e 3c2f  geography?</a></
+000010e0: 7375 6d6d 6172 793e 0a0a 416c 6c20 7468  summary>..All th
+000010f0: 6520 6461 7461 2069 7320 6163 6365 7373  e data is access
+00001100: 6962 6c65 2074 6872 6f75 6768 2074 6865  ible through the
+00001110: 2060 6372 6f70 6861 7276 6573 742e 6461   `cropharvest.da
+00001120: 7461 7365 7473 2e43 726f 7048 6172 7665  tasets.CropHarve
+00001130: 7374 6020 6f62 6a65 6374 2e20 5468 6520  st` object. The 
+00001140: 6d61 696e 2070 6172 616d 6574 6572 7320  main parameters 
+00001150: 7768 6963 6820 796f 7520 6d69 6768 7420  which you might 
+00001160: 6265 2069 6e74 6572 6573 7465 6420 696e  be interested in
+00001170: 206d 616e 6970 756c 6174 696e 6720 6172   manipulating ar
+00001180: 6520 636f 6e74 726f 6c6c 6162 6c65 2074  e controllable t
+00001190: 6872 6f75 6768 2061 2060 6372 6f70 6861  hrough a `cropha
+000011a0: 7276 6573 742e 6461 7461 7365 7473 2e54  rvest.datasets.T
+000011b0: 6173 6b60 2c20 7768 6963 6820 7461 6b65  ask`, which take
+000011c0: 7320 6173 2069 6e70 7574 2074 6865 2066  s as input the f
+000011d0: 6f6c 6c6f 7769 6e67 2070 6172 616d 6574  ollowing paramet
+000011e0: 6572 733a 0a2d 2041 2062 6f75 6e64 696e  ers:.- A boundin
+000011f0: 6720 626f 782c 2077 6869 6368 2064 6566  g box, which def
+00001200: 696e 6573 2074 6865 2073 7061 7469 616c  ines the spatial
+00001210: 2062 6f75 6e64 6172 6965 7320 6f66 2074   boundaries of t
+00001220: 6865 206c 6162 656c 7320 7265 7472 6965  he labels retrie
+00001230: 7665 730a 2d20 4120 7461 7267 6574 206c  ves.- A target l
+00001240: 6162 656c 2c20 7768 6963 6820 6465 6669  abel, which defi
+00001250: 6e65 7320 7468 6520 636c 6173 7320 6f66  nes the class of
+00001260: 2074 6865 2070 6f73 6974 6976 6520 6c61   the positive la
+00001270: 6265 6c73 2028 6966 2074 6869 7320 6973  bels (if this is
+00001280: 206c 6566 7420 746f 2060 4e6f 6e65 602c   left to `None`,
+00001290: 2074 6865 6e20 7468 6520 706f 7369 7469   then the positi
+000012a0: 7665 2063 6c61 7373 2077 696c 6c20 6265  ve class will be
+000012b0: 2063 726f 7073 2061 6e64 2074 6865 206e   crops and the n
+000012c0: 6567 6174 6976 6520 636c 6173 7320 7769  egative class wi
+000012d0: 6c6c 2062 6520 6e6f 6e2d 6372 6f70 7329  ll be non-crops)
+000012e0: 0a2d 2041 2062 6f6f 6c65 616e 2064 6566  .- A boolean def
+000012f0: 696e 696e 6720 7768 6574 6865 7220 6f72  ining whether or
+00001300: 206e 6f74 2074 6f20 6261 6c61 6e63 6520   not to balance 
+00001310: 7468 6520 6372 6f70 7320 616e 6420 6e6f  the crops and no
+00001320: 6e2d 6372 6f70 7320 696e 2074 6865 206e  n-crops in the n
+00001330: 6567 6174 6976 6520 636c 6173 730a 2d20  egative class.- 
+00001340: 4120 7465 7374 5f69 6465 6e74 6966 6965  A test_identifie
+00001350: 7220 7374 7269 6e67 2c20 7768 6963 6820  r string, which 
+00001360: 7465 6c6c 7320 7468 6520 6461 7461 7365  tells the datase
+00001370: 7420 7768 6574 6865 7220 6f72 206e 6f74  t whether or not
+00001380: 2074 6f20 7265 7472 6965 7665 2061 2066   to retrieve a f
+00001390: 696c 6520 6672 6f6d 2074 6865 2060 7465  ile from the `te
+000013a0: 7374 5f66 6561 7475 7265 7360 2066 6f6c  st_features` fol
+000013b0: 6465 7220 616e 6420 7265 7475 726e 2069  der and return i
+000013c0: 7420 6173 2074 6865 2074 6573 7420 6461  t as the test da
+000013d0: 7461 2e0a 0a53 6f20 6966 2049 2077 616e  ta...So if I wan
+000013e0: 7465 6420 746f 2075 7365 2074 6869 7320  ted to use this 
+000013f0: 746f 2074 7261 696e 2061 206d 6f64 656c  to train a model
+00001400: 2074 6f20 6964 656e 7469 6679 2063 726f   to identify cro
+00001410: 7020 7673 2e20 6e6f 6e20 6372 6f70 2069  p vs. non crop i
+00001420: 6e20 4672 616e 6365 2c20 4920 6d69 6768  n France, I migh
+00001430: 7420 646f 2069 7420 6c69 6b65 2074 6869  t do it like thi
+00001440: 733a 0a0a 6060 6070 7974 686f 6e0a 6672  s:..```python.fr
+00001450: 6f6d 2073 6b6c 6561 726e 2e65 6e73 656d  om sklearn.ensem
+00001460: 626c 6520 696d 706f 7274 2052 616e 646f  ble import Rando
+00001470: 6d46 6f72 6573 7443 6c61 7373 6966 6965  mForestClassifie
+00001480: 720a 0a66 726f 6d20 6372 6f70 6861 7276  r..from cropharv
+00001490: 6573 742e 6461 7461 7365 7473 2069 6d70  est.datasets imp
+000014a0: 6f72 7420 5461 736b 2c20 4372 6f70 4861  ort Task, CropHa
+000014b0: 7276 6573 740a 6672 6f6d 2063 726f 7068  rvest.from croph
+000014c0: 6172 7665 7374 2e63 6f75 6e74 7269 6573  arvest.countries
+000014d0: 2069 6d70 6f72 7420 6765 745f 636f 756e   import get_coun
+000014e0: 7472 795f 6262 6f78 0a0a 2320 666f 6c64  try_bbox..# fold
+000014f0: 6572 2069 6e74 6f20 7768 6963 6820 7468  er into which th
+00001500: 6520 6461 7461 2077 696c 6c20 6265 2064  e data will be d
+00001510: 6f77 6e6c 6f61 6465 6420 2f20 616c 7265  ownloaded / alre
+00001520: 6164 7920 6578 6973 7473 0a64 6174 615f  ady exists.data_
+00001530: 6469 7220 3d20 2264 6174 6122 0a0a 2320  dir = "data"..# 
+00001540: 6765 745f 636f 756e 7472 795f 6262 6f78  get_country_bbox
+00001550: 2072 6574 7572 6e73 2061 206c 6973 7420   returns a list 
+00001560: 6f66 2062 6f75 6e64 696e 6720 626f 7865  of bounding boxe
+00001570: 732e 0a23 2074 6865 206f 6e65 2072 6570  s..# the one rep
+00001580: 7265 7365 6e74 696e 6720 4d65 7472 6f70  resenting Metrop
+00001590: 6f6c 6974 616e 2046 7261 6e63 6520 6973  olitan France is
+000015a0: 2074 6865 2032 6e64 2062 6f78 0a6d 6574   the 2nd box.met
+000015b0: 726f 706f 6c69 7461 6e5f 6672 616e 6365  ropolitan_france
+000015c0: 5f62 626f 7820 3d20 6765 745f 636f 756e  _bbox = get_coun
+000015d0: 7472 795f 6262 6f78 2822 4672 616e 6365  try_bbox("France
+000015e0: 2229 5b31 5d0a 0a74 6173 6b20 3d20 5461  ")[1]..task = Ta
+000015f0: 736b 2862 6f75 6e64 696e 675f 626f 783d  sk(bounding_box=
+00001600: 6d65 7472 6f70 6f6c 6974 616e 5f66 7261  metropolitan_fra
+00001610: 6e63 655f 6262 6f78 2c20 6e6f 726d 616c  nce_bbox, normal
+00001620: 697a 653d 5472 7565 290a 0a6d 795f 6461  ize=True)..my_da
+00001630: 7461 7365 7420 3d20 4372 6f70 4861 7276  taset = CropHarv
+00001640: 6573 7428 6461 7461 5f64 6972 2c20 7461  est(data_dir, ta
+00001650: 736b 290a 0a58 2c20 7920 3d20 6d79 5f64  sk)..X, y = my_d
+00001660: 6174 6173 6574 2e61 735f 6172 7261 7928  ataset.as_array(
+00001670: 666c 6174 7465 6e5f 783d 5472 7565 290a  flatten_x=True).
+00001680: 6d6f 6465 6c20 3d20 5261 6e64 6f6d 466f  model = RandomFo
+00001690: 7265 7374 436c 6173 7369 6669 6572 2872  restClassifier(r
+000016a0: 616e 646f 6d5f 7374 6174 653d 3029 0a6d  andom_state=0).m
+000016b0: 6f64 656c 2e66 6974 2858 2c20 7929 0a60  odel.fit(X, y).`
+000016c0: 6060 0a3c 2f64 6574 6169 6c73 3e0a 0a3c  ``.</details>..<
+000016d0: 6465 7461 696c 733e 0a3c 7375 6d6d 6172  details>.<summar
+000016e0: 793e 3c61 2068 7265 663d 6874 7470 733a  y><a href=https:
+000016f0: 2f2f 6769 7468 7562 2e63 6f6d 2f6e 6173  //github.com/nas
+00001700: 6168 6172 7665 7374 2f63 726f 7068 6172  aharvest/crophar
+00001710: 7665 7374 2f69 7373 7565 732f 3130 363e  vest/issues/106>
+00001720: 486f 7720 646f 2049 206c 6f61 6420 6120  How do I load a 
+00001730: 7370 6563 6966 6963 2070 6978 656c 2074  specific pixel t
+00001740: 696d 6573 6572 6965 733f 3c2f 613e 3c2f  imeseries?</a></
+00001750: 7375 6d6d 6172 793e 0a0a 5468 6520 3c61  summary>..The <a
+00001760: 2068 7265 663d 6874 7470 733a 2f2f 6769   href=https://gi
+00001770: 7468 7562 2e63 6f6d 2f6e 6173 6168 6172  thub.com/nasahar
+00001780: 7665 7374 2f63 726f 7068 6172 7665 7374  vest/cropharvest
+00001790: 2f69 7373 7565 732f 3130 363e 7370 6563  /issues/106>spec
+000017a0: 6966 6963 2075 7365 2063 6173 653c 2f61  ific use case</a
+000017b0: 3e20 6865 7265 2069 7320 746f 2072 6574  > here is to ret
+000017c0: 7269 6576 6520 4e44 5649 2076 616c 7565  rieve NDVI value
+000017d0: 7320 666f 7220 6120 7370 6563 6966 6963  s for a specific
+000017e0: 2072 6f77 2069 6e20 7468 6520 606c 6162   row in the `lab
+000017f0: 656c 732e 6765 6f6a 736f 6e60 2e20 4865  els.geojson`. He
+00001800: 7265 2069 7320 686f 7720 796f 7520 6d69  re is how you mi
+00001810: 6768 7420 676f 2061 626f 7574 2064 6f69  ght go about doi
+00001820: 6e67 2074 6861 743a 0a0a 4669 7273 746c  ng that:..Firstl
+00001830: 792c 2049 2077 696c 6c20 6c6f 6164 2074  y, I will load t
+00001840: 6865 2067 656f 736a 6f6e 2e20 4927 6c6c  he geosjon. I'll
+00001850: 2064 6f20 6974 2074 6872 6f75 6768 2061   do it through a
+00001860: 2060 4372 6f70 4861 7276 6573 744c 6162   `CropHarvestLab
+00001870: 656c 7360 206f 626a 6563 742c 2077 6869  els` object, whi
+00001880: 6368 2069 7320 6a75 7374 2061 2077 7261  ch is just a wra
+00001890: 7070 6572 2061 726f 756e 6420 7468 6520  pper around the 
+000018a0: 6765 6f6a 736f 6e20 6275 7420 7072 6f76  geojson but prov
+000018b0: 6964 6573 2073 6f6d 6520 6e69 6365 2075  ides some nice u
+000018c0: 7469 6c69 7479 2066 756e 6374 696f 6e73  tility functions
+000018d0: 2e0a 6060 6070 7974 686f 6e0a 3e3e 3e20  ..```python.>>> 
+000018e0: 6672 6f6d 2063 726f 7068 6172 7665 7374  from cropharvest
+000018f0: 2e64 6174 6173 6574 7320 696d 706f 7274  .datasets import
+00001900: 2043 726f 7048 6172 7665 7374 4c61 6265   CropHarvestLabe
+00001910: 6c73 0a3e 3e3e 0a3e 3e3e 206c 6162 656c  ls.>>>.>>> label
+00001920: 7320 3d20 4372 6f70 4861 7276 6573 744c  s = CropHarvestL
+00001930: 6162 656c 7328 2263 726f 7068 6172 7665  abels("cropharve
+00001940: 7374 2f64 6174 6122 290a 3e3e 3e20 6c61  st/data").>>> la
+00001950: 6265 6c73 5f67 656f 6a73 6f6e 203d 206c  bels_geojson = l
+00001960: 6162 656c 732e 6173 5f67 656f 6a73 6f6e  abels.as_geojson
+00001970: 2829 0a3e 3e3e 206c 6162 656c 735f 6765  ().>>> labels_ge
+00001980: 6f6a 736f 6e2e 6865 6164 2829 0a20 2068  ojson.head().  h
+00001990: 6172 7665 7374 5f64 6174 6520 706c 616e  arvest_date plan
+000019a0: 7469 6e67 5f64 6174 6520 202e 2e2e 2069  ting_date  ... i
+000019b0: 735f 7465 7374 2020 2020 2020 2020 2020  s_test          
+000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019e0: 2067 656f 6d65 7472 790a 3020 2020 2020   geometry.0     
+000019f0: 2020 2020 4e6f 6e65 2020 2020 2020 2020      None        
+00001a00: 2020 4e6f 6e65 2020 2e2e 2e20 2020 4661    None  ...   Fa
+00001a10: 6c73 6520 2050 4f4c 5947 4f4e 2028 2833  lse  POLYGON ((3
+00001a20: 372e 3038 3235 3220 3130 2e37 3132 3734  7.08252 10.71274
+00001a30: 2c20 3337 2e30 3833 3438 2031 302e 3731  , 37.08348 10.71
+00001a40: 3239 312e 2e2e 0a31 2020 2020 2020 2020  291....1        
+00001a50: 204e 6f6e 6520 2020 2020 2020 2020 204e   None          N
+00001a60: 6f6e 6520 202e 2e2e 2020 2046 616c 7365  one  ...   False
+00001a70: 2020 504f 4c59 474f 4e20 2828 3337 2e30    POLYGON ((37.0
+00001a80: 3837 3231 2031 302e 3732 3339 382c 2033  8721 10.72398, 3
+00001a90: 372e 3038 3731 3420 3130 2e37 3234 3239  7.08714 10.72429
+00001aa0: 2e2e 2e0a 3220 2020 2020 2020 2020 4e6f  ....2         No
+00001ab0: 6e65 2020 2020 2020 2020 2020 4e6f 6e65  ne          None
+00001ac0: 2020 2e2e 2e20 2020 4661 6c73 6520 2050    ...   False  P
+00001ad0: 4f4c 5947 4f4e 2028 2833 372e 3038 3439  OLYGON ((37.0849
+00001ae0: 3820 3130 2e37 3133 3731 2c20 3337 2e30  8 10.71371, 37.0
+00001af0: 3834 3831 2031 302e 3731 3339 332e 2e2e  8481 10.71393...
+00001b00: 0a33 2020 2020 2020 2020 204e 6f6e 6520  .3         None 
+00001b10: 2020 2020 2020 2020 204e 6f6e 6520 202e           None  .
+00001b20: 2e2e 2020 2046 616c 7365 2020 504f 4c59  ..   False  POLY
+00001b30: 474f 4e20 2828 3337 2e30 3930 3231 2031  GON ((37.09021 1
+00001b40: 302e 3731 3332 302c 2033 372e 3039 3031  0.71320, 37.0901
+00001b50: 3420 3130 2e37 3133 3431 2e2e 2e0a 3420  4 10.71341....4 
+00001b60: 2020 2020 2020 2020 4e6f 6e65 2020 2020          None    
+00001b70: 2020 2020 2020 4e6f 6e65 2020 2e2e 2e20        None  ... 
+00001b80: 2020 4661 6c73 6520 2050 4f4c 5947 4f4e    False  POLYGON
+00001b90: 2028 2833 372e 3038 3330 3720 3130 2e37   ((37.08307 10.7
+00001ba0: 3231 3630 2c20 3337 2e30 3832 3831 2031  2160, 37.08281 1
+00001bb0: 302e 3732 3139 372e 2e2e 0a0a 5b35 2072  0.72197.....[5 r
+00001bc0: 6f77 7320 7820 3133 2063 6f6c 756d 6e73  ows x 13 columns
+00001bd0: 5d0a 6060 600a 0a4e 6f77 2c20 4920 6361  ].```..Now, I ca
+00001be0: 6e20 7573 6520 7468 6520 606c 6162 656c  n use the `label
+00001bf0: 7360 206f 626a 6563 7420 746f 2072 6574  s` object to ret
+00001c00: 7269 6576 6520 7468 6520 6669 6c65 7061  rieve the filepa
+00001c10: 7468 206f 6620 7468 6520 7072 6f63 6573  th of the proces
+00001c20: 7365 6420 7361 7465 6c6c 6974 6520 6461  sed satellite da
+00001c30: 7461 2066 6f72 2065 6163 6820 726f 7720  ta for each row 
+00001c40: 696e 2074 6865 206c 6162 656c 7320 6765  in the labels ge
+00001c50: 6f6a 736f 6e3a 0a60 6060 7079 7468 6f6e  ojson:.```python
+00001c60: 0a3e 3e3e 2070 6174 685f 746f 5f66 696c  .>>> path_to_fil
+00001c70: 6520 3d20 6c61 6265 6c73 2e5f 7061 7468  e = labels._path
+00001c80: 5f66 726f 6d5f 726f 7728 6c61 6265 6c73  _from_row(labels
+00001c90: 5f67 656f 6a73 6f6e 2e69 6c6f 635b 305d  _geojson.iloc[0]
+00001ca0: 290a 6060 600a 5468 6973 2070 726f 6365  ).```.This proce
+00001cb0: 7373 6564 2073 6174 656c 6c69 7465 2064  ssed satellite d
+00001cc0: 6174 6120 6973 2073 746f 7265 6420 6173  ata is stored as
+00001cd0: 2060 6835 7079 6020 6669 6c65 732c 2073   `h5py` files, s
+00001ce0: 6f20 4920 6361 6e20 6c6f 6164 2069 7420  o I can load it 
+00001cf0: 7570 2061 7320 666f 6c6c 6f77 733a 0a60  up as follows:.`
+00001d00: 6060 7079 7468 6f6e 0a3e 3e3e 2069 6d70  ``python.>>> imp
+00001d10: 6f72 7420 6835 7079 0a3e 3e3e 2068 3570  ort h5py.>>> h5p
+00001d20: 795f 6669 6c65 203d 2068 3570 792e 4669  y_file = h5py.Fi
+00001d30: 6c65 2870 6174 685f 746f 5f66 696c 652c  le(path_to_file,
+00001d40: 2022 7222 290a 3e3e 3e20 7820 3d20 6835   "r").>>> x = h5
+00001d50: 7079 5f66 696c 652e 6765 7428 2261 7272  py_file.get("arr
+00001d60: 6179 2229 5b3a 5d0a 3e3e 3e20 782e 7368  ay")[:].>>> x.sh
+00001d70: 6170 650a 2831 322c 2031 3829 0a60 6060  ape.(12, 18).```
+00001d80: 0a54 6865 2073 6861 7065 206f 6620 6078  .The shape of `x
+00001d90: 6020 7265 7072 6573 656e 7473 2031 3220  ` represents 12 
+00001da0: 7469 6d65 7374 6570 7320 616e 6420 3138  timesteps and 18
+00001db0: 2062 616e 6473 2e20 546f 2072 6574 7269   bands. To retri
+00001dc0: 6576 6520 7468 6520 6261 6e64 2049 2061  eve the band I a
+00001dd0: 6d20 696e 7465 7265 7374 6564 2069 6e3a  m interested in:
+00001de0: 0a60 6060 7079 7468 6f6e 0a3e 3e3e 2066  .```python.>>> f
+00001df0: 726f 6d20 6372 6f70 6861 7276 6573 742e  rom cropharvest.
+00001e00: 6261 6e64 7320 696d 706f 7274 2042 414e  bands import BAN
+00001e10: 4453 0a3e 3e3e 2078 5b3a 2c20 4241 4e44  DS.>>> x[:, BAND
+00001e20: 532e 696e 6465 7828 224e 4456 4922 295d  S.index("NDVI")]
+00001e30: 0a61 7272 6179 285b 302e 3238 3939 3230  .array([0.289920
+00001e40: 3732 2c20 302e 3238 3833 3833 3433 2c20  72, 0.28838343, 
+00001e50: 302e 3236 3833 3335 3739 2c20 302e 3232  0.26833579, 0.22
+00001e60: 3537 3736 3333 2c20 302e 3237 3133 3839  577633, 0.271389
+00001e70: 3836 2c0a 2020 2020 2020 2030 2e30 3635  86,.       0.065
+00001e80: 3834 3131 342c 2030 2e34 3938 3939 3820  84114, 0.498998 
+00001e90: 202c 2030 2e35 3031 3437 3230 332c 2030   , 0.50147203, 0
+00001ea0: 2e35 3034 3337 3734 332c 2030 2e34 3433  .50437743, 0.443
+00001eb0: 3236 3334 332c 0a20 2020 2020 2020 302e  26343,.       0.
+00001ec0: 3333 3733 3538 3439 2c20 302e 3238 3337  33735849, 0.2837
+00001ed0: 3539 3637 5d29 0a60 6060 0a54 6865 7365  5967]).```.These
+00001ee0: 2061 7265 2031 3220 4e44 5649 2076 616c   are 12 NDVI val
+00001ef0: 7565 732c 2063 6f72 7265 7370 6f6e 6469  ues, correspondi
+00001f00: 6e67 2074 6f20 7468 6520 3132 206d 6f6e  ng to the 12 mon
+00001f10: 7468 7320 6361 7074 7572 6564 2069 6e20  ths captured in 
+00001f20: 7468 6973 2074 696d 6573 6572 6965 732e  this timeseries.
+00001f30: 2054 6f20 6669 6e64 206f 7574 2065 7861   To find out exa
+00001f40: 6374 6c79 2077 6869 6368 206d 6f6e 7468  ctly which month
+00001f50: 2065 6163 6820 7469 6d65 7374 6570 2072   each timestep r
+00001f60: 6570 7265 7365 6e74 732c 2049 2063 616e  epresents, I can
+00001f70: 2064 6f0a 6060 6070 7974 686f 6e0a 3e3e   do.```python.>>
+00001f80: 3e20 6c61 6265 6c73 5f67 656f 6a73 6f6e  > labels_geojson
+00001f90: 2e69 6c6f 635b 305d 2e65 7870 6f72 745f  .iloc[0].export_
+00001fa0: 656e 645f 6461 7465 0a27 3230 3231 2d30  end_date.'2021-0
+00001fb0: 322d 3031 5430 303a 3030 3a30 3027 0a60  2-01T00:00:00'.`
+00001fc0: 6060 0a57 6963 6820 7465 6c6c 7320 6d65  ``.Wich tells me
+00001fd0: 2074 6861 7420 7468 6520 6c61 7374 2074   that the last t
+00001fe0: 696d 6573 7465 7020 7265 7072 6573 656e  imestep represen
+00001ff0: 7473 204a 616e 7561 7279 2032 3032 312e  ts January 2021.
+00002000: 2049 2063 616e 2077 6f72 6b20 6261 636b   I can work back
+00002010: 7761 7264 7320 6672 6f6d 2074 6865 7265  wards from there
+00002020: 2e0a 0a3c 2f64 6574 6169 6c73 3e0a 0a3c  ...</details>..<
+00002030: 6465 7461 696c 733e 0a3c 7375 6d6d 6172  details>.<summar
+00002040: 793e 3c61 2068 7265 663d 2268 7474 7073  y><a href="https
+00002050: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e61  ://github.com/na
+00002060: 7361 6861 7276 6573 742f 6372 6f70 6861  saharvest/cropha
+00002070: 7276 6573 742f 6973 7375 6573 2f38 3822  rvest/issues/88"
+00002080: 3e57 6861 7420 6973 2074 6865 2064 6174  >What is the dat
+00002090: 6120 666f 726d 6174 3f3c 2f61 3e3c 2f73  a format?</a></s
+000020a0: 756d 6d61 7279 3e0a 5468 6520 7374 7275  ummary>.The stru
+000020b0: 6374 7572 6520 6f66 2074 6865 2064 6966  cture of the dif
+000020c0: 6665 7265 6e74 2064 6174 6120 6669 6c65  ferent data file
+000020d0: 7320 6973 206e 6f77 2064 6573 6372 6962  s is now describ
+000020e0: 6564 2069 6e20 6465 7074 6820 696e 2074  ed in depth in t
+000020f0: 6865 2064 6174 6120 666f 6c64 6572 2773  he data folder's
+00002100: 205b 5265 6164 6d65 5d28 6874 7470 733a   [Readme](https:
+00002110: 2f2f 6769 7468 7562 2e63 6f6d 2f6e 6173  //github.com/nas
+00002120: 6168 6172 7665 7374 2f63 726f 7068 6172  aharvest/crophar
+00002130: 7665 7374 2f62 6c6f 622f 6d61 696e 2f64  vest/blob/main/d
+00002140: 6174 612f 5245 4144 4d45 2e6d 6429 0a3c  ata/README.md).<
+00002150: 2f64 6574 6169 6c73 3e0a 0a23 2323 204c  /details>..### L
+00002160: 6963 656e 7365 0a43 726f 7048 6172 7665  icense.CropHarve
+00002170: 7374 2068 6173 2061 205b 4372 6561 7469  st has a [Creati
+00002180: 7665 2043 6f6d 6d6f 6e73 2041 7474 7269  ve Commons Attri
+00002190: 6275 7469 6f6e 2d53 6861 7265 416c 696b  bution-ShareAlik
+000021a0: 6520 342e 3020 496e 7465 726e 6174 696f  e 4.0 Internatio
+000021b0: 6e61 6c5d 2868 7474 7073 3a2f 2f67 6974  nal](https://git
+000021c0: 6875 622e 636f 6d2f 6e61 7361 6861 7276  hub.com/nasaharv
+000021d0: 6573 742f 6372 6f70 6861 7276 6573 742f  est/cropharvest/
+000021e0: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
+000021f0: 452e 7478 7429 206c 6963 656e 7365 2e0a  E.txt) license..
+00002200: 0a23 2323 2043 6974 6174 696f 6e0a 0a49  .### Citation..I
+00002210: 6620 796f 7520 7573 6520 4372 6f70 4861  f you use CropHa
+00002220: 7276 6573 7420 696e 2079 6f75 7220 7265  rvest in your re
+00002230: 7365 6172 6368 2c20 706c 6561 7365 2075  search, please u
+00002240: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
+00002250: 2063 6974 6174 696f 6e3a 0a60 6060 0a40   citation:.```.@
+00002260: 696e 7072 6f63 6565 6469 6e67 737b 0a20  inproceedings{. 
+00002270: 2020 2074 7365 6e67 3230 3231 6372 6f70     tseng2021crop
+00002280: 6861 7276 6573 742c 0a20 2020 2074 6974  harvest,.    tit
+00002290: 6c65 3d7b 4372 6f70 4861 7276 6573 743a  le={CropHarvest:
+000022a0: 2041 2067 6c6f 6261 6c20 6461 7461 7365   A global datase
+000022b0: 7420 666f 7220 6372 6f70 2d74 7970 6520  t for crop-type 
+000022c0: 636c 6173 7369 6669 6361 7469 6f6e 7d2c  classification},
+000022d0: 0a20 2020 2061 7574 686f 723d 7b47 6162  .    author={Gab
+000022e0: 7269 656c 2054 7365 6e67 2061 6e64 2049  riel Tseng and I
+000022f0: 7661 6e20 5a76 6f6e 6b6f 7620 616e 6420  van Zvonkov and 
+00002300: 4361 7468 6572 696e 6520 4c69 6c69 616e  Catherine Lilian
+00002310: 204e 616b 616c 656d 6265 2061 6e64 2048   Nakalembe and H
+00002320: 616e 6e61 6820 4b65 726e 6572 7d2c 0a20  annah Kerner},. 
+00002330: 2020 2062 6f6f 6b74 6974 6c65 3d7b 5468     booktitle={Th
+00002340: 6972 7479 2d66 6966 7468 2043 6f6e 6665  irty-fifth Confe
+00002350: 7265 6e63 6520 6f6e 204e 6575 7261 6c20  rence on Neural 
+00002360: 496e 666f 726d 6174 696f 6e20 5072 6f63  Information Proc
+00002370: 6573 7369 6e67 2053 7973 7465 6d73 2044  essing Systems D
+00002380: 6174 6173 6574 7320 616e 6420 4265 6e63  atasets and Benc
+00002390: 686d 6172 6b73 2054 7261 636b 2028 526f  hmarks Track (Ro
+000023a0: 756e 6420 3229 7d2c 0a20 2020 2079 6561  und 2)},.    yea
+000023b0: 723d 7b32 3032 317d 2c0a 2020 2020 7572  r={2021},.    ur
+000023c0: 6c3d 7b68 7474 7073 3a2f 2f6f 7065 6e72  l={https://openr
+000023d0: 6576 6965 772e 6e65 742f 666f 7275 6d3f  eview.net/forum?
+000023e0: 6964 3d4a 746a 7a55 5850 4561 4375 7d0a  id=JtjzUXPEaCu}.
+000023f0: 7d0a 6060 600a                           }.```.
```

### Comparing `cropharvest-0.6.0/README.md` & `cropharvest-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 pip install cropharvest
 ```
 Windows users must install the CropHarvest within a [conda](https://docs.conda.io/en/latest/miniconda.html) environment to ensure all dependencies are installed correctly:
 ```bash
 conda install 'fiona>=1.5' 'rasterio>=1.2.6'
 pip install cropharvest
 ```
+In addition, it [may be necessary](https://github.com/h5py/h5py/issues/1774) to install `h5py` using conda as well (`conda install 'h5py>3.7.0'`) prior to pip-installing cropharvest.
 
 ### Getting started [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nasaharvest/cropharvest/blob/main/demo.ipynb)
 See the [`demo.ipynb`](https://github.com/nasaharvest/cropharvest/blob/main/demo.ipynb) notebook for an example on how to download the data from [Zenodo](https://zenodo.org/record/7257688) and train a random forest against this data.
 
 For more examples of models trained against this dataset, see the [benchmarks](https://github.com/nasaharvest/cropharvest/blob/main/benchmarks).
 
 ### Contributing
```

#### html2text {}

```diff
@@ -27,21 +27,23 @@
 these use cases are demonstrated in the [`demo_exporting_data.ipynb`](https://
 github.com/nasaharvest/cropharvest/blob/main/demo_exporting_data.ipynb)
 notebook. ### Installation Linux and MacOS users can install the latest version
 of CropHarvest with the following command: ```bash pip install cropharvest ```
 Windows users must install the CropHarvest within a [conda](https://
 docs.conda.io/en/latest/miniconda.html) environment to ensure all dependencies
 are installed correctly: ```bash conda install 'fiona>=1.5' 'rasterio>=1.2.6'
-pip install cropharvest ``` ### Getting started [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/nasaharvest/cropharvest/blob/main/demo.ipynb)
-See the [`demo.ipynb`](https://github.com/nasaharvest/cropharvest/blob/main/
-demo.ipynb) notebook for an example on how to download the data from [Zenodo]
-(https://zenodo.org/record/7257688) and train a random forest against this
-data. For more examples of models trained against this dataset, see the
+pip install cropharvest ``` In addition, it [may be necessary](https://
+github.com/h5py/h5py/issues/1774) to install `h5py` using conda as well (`conda
+install 'h5py>3.7.0'`) prior to pip-installing cropharvest. ### Getting started
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/github/nasaharvest/cropharvest/blob/main/
+demo.ipynb) See the [`demo.ipynb`](https://github.com/nasaharvest/cropharvest/
+blob/main/demo.ipynb) notebook for an example on how to download the data from
+[Zenodo](https://zenodo.org/record/7257688) and train a random forest against
+this data. For more examples of models trained against this dataset, see the
 [benchmarks](https://github.com/nasaharvest/cropharvest/blob/main/benchmarks).
 ### Contributing If you would like to contribute a dataset, please see the
 [contributing readme](https://github.com/nasaharvest/cropharvest/blob/main/
 contributing.md). ### ~~FAQ~~ Questions asked at least once _H_o_w_ _d_o_ _I_ _u_s_e
 _C_r_o_p_H_a_r_v_e_s_t_ _f_o_r_ _a_ _s_p_e_c_i_f_i_c_ _g_e_o_g_r_a_p_h_y_? All the data is accessible through the
 `cropharvest.datasets.CropHarvest` object. The main parameters which you might
 be interested in manipulating are controllable through a
```

### Comparing `cropharvest-0.6.0/cropharvest/bands.py` & `cropharvest-0.7.0/cropharvest/bands.py`

 * *Files identical despite different names*

### Comparing `cropharvest-0.6.0/cropharvest/bbox.py` & `cropharvest-0.7.0/cropharvest/bbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import List, Tuple
 
 from typing import Optional
 
 
 @dataclass
 class BBox:
-
     min_lat: float
     max_lat: float
     min_lon: float
     max_lon: float
 
     name: Optional[str] = None
 
@@ -49,15 +48,14 @@
         an ML model, we want it to know the extremes are close together.
         Mapping them to 3d space allows us to do that
         """
         lat, lon = self.get_centre(in_radians=True)
         return [cos(lat) * cos(lon), cos(lat) * sin(lon), sin(lat)]
 
     def get_centre(self, in_radians: bool = True) -> Tuple[float, float]:
-
         # roughly calculate the centres
         lat = self.min_lat + ((self.max_lat - self.min_lat) / 2)
         lon = self.min_lon + ((self.max_lon - self.min_lon) / 2)
         if in_radians:
             return radians(lat), radians(lon)
         else:
             return lat, lon
```

### Comparing `cropharvest-0.6.0/cropharvest/columns.py` & `cropharvest-0.7.0/cropharvest/columns.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
     @classmethod
     def date_columns(cls) -> List[str]:
         raise NotImplementedError
 
 
 class RequiredColumns(Columns):
-
     INDEX = "index"
     IS_CROP = "is_crop"
     LAT = "lat"
     LON = "lon"
     DATASET = "dataset"
     COLLECTION_DATE = "collection_date"
     EXPORT_END_DATE = "export_end_date"
```

### Comparing `cropharvest-0.6.0/cropharvest/config.py` & `cropharvest-0.7.0/cropharvest/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WARNING: some logic in the loading functions (e.g.
 # for the central asia loader) assumes a February export
 # date, so its recommended the loading functions are reviewed
 # if this is changed
 EXPORT_END_MONTH = 2
 EXPORT_END_DAY = 1
 
-DATASET_VERSION_ID = 7257688
+DATASET_VERSION_ID = 10251170
 DATASET_URL = f"https://zenodo.org/record/{DATASET_VERSION_ID}"
 LABELS_FILENAME = "labels.geojson"
 FEATURES_DIR = "features"
 TEST_FEATURES_DIR = "test_features"
 
 # the default seed is useful because it also seeds the deterministic
 # shuffling algorithm we use (in cropharvest.utils.deterministic_shuffle)
@@ -42,8 +42,8 @@
         min_lat=-12.1995, max_lat=-12.1226, min_lon=-45.8238, max_lon=-45.7579
     ),
     "Brazil_coffee_2021_0": BBox(
         min_lat=-12.1995, max_lat=-12.1226, min_lon=-45.8238, max_lon=-45.7579
     ),
 }
 
-TEST_DATASETS = {"Togo": "togo-eval"}
+TEST_DATASETS = {"Togo": "togo-eval", "People's Republic of China": "china-crop"}
```

### Comparing `cropharvest-0.6.0/cropharvest/countries.py` & `cropharvest-0.7.0/cropharvest/countries.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 @memoized
 def load_country_shapefile():
     return geopandas.read_file(str(Path(__file__).parent / "country_shapefile"))
 
 
 def get_country_bbox(country_name: str, largest_only: bool = False) -> List[BBox]:
-
     country_shapefile = load_country_shapefile()
     country = country_shapefile[country_shapefile.NAME_EN == country_name]
     if len(country) != 1:
         raise RuntimeError(f"Unrecognized country {country_name}")
     polygon = country.geometry.iloc[0]
     if isinstance(polygon, Polygon):
         return [BBox.polygon_to_bbox(polygon, country_name)]
```

### Comparing `cropharvest-0.6.0/cropharvest/country_shapefile/ne_50m_admin_0_countries.dbf` & `cropharvest-0.7.0/cropharvest/country_shapefile/ne_50m_admin_0_countries.dbf`

 * *Files identical despite different names*

### Comparing `cropharvest-0.6.0/cropharvest/country_shapefile/ne_50m_admin_0_countries.shp` & `cropharvest-0.7.0/cropharvest/country_shapefile/ne_50m_admin_0_countries.shp`

 * *Files identical despite different names*

### Comparing `cropharvest-0.6.0/cropharvest/country_shapefile/ne_50m_admin_0_countries.shx` & `cropharvest-0.7.0/cropharvest/country_shapefile/ne_50m_admin_0_countries.shx`

 * *Files identical despite different names*

### Comparing `cropharvest-0.6.0/cropharvest/crops.py` & `cropharvest-0.7.0/cropharvest/crops.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     beverage_spice = 6
     leguminous = 7
     sugar = 8
     other = 9
 
 
 def to_one_hot(crop_name: str) -> List[float]:
-
     if crop_name in [x.name for x in CropClassifications]:
         encoding = np.zeros(len(CropClassifications))
         encoding[CropClassifications.__getitem__(crop_name).value] = 1
     elif crop_name == "crop":
         encoding = np.ones(len(CropClassifications))
         encoding[CropClassifications.__getitem__("non_crop").value] = 0
         # normalize the one hot encoding
```

### Comparing `cropharvest-0.6.0/cropharvest/datasets.py` & `cropharvest-0.7.0/cropharvest/datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -199,14 +199,23 @@
     def from_labels(cls):
         pass
 
 
 class CropHarvest(BaseDataset):
     """Dataset consisting of satellite data and associated labels"""
 
+    filepaths: List[Path]
+    y_vals: List[int]
+    positive_indices: List[int]
+    negative_indices: List[int]
+    # used in the sample() function, to ensure filepaths are sampled without
+    # duplication as much as possible
+    sampled_positive_indices: List[int]
+    sampled_negative_indices: List[int]
+
     def __init__(
         self,
         root,
         task: Optional[Task] = None,
         download=False,
         val_ratio: float = 0.0,
         is_val: bool = False,
@@ -214,45 +223,48 @@
         super().__init__(root, download, filenames=(FEATURES_DIR, TEST_FEATURES_DIR))
 
         labels = CropHarvestLabels(root, download=download)
         if task is None:
             print("Using the default task; crop vs. non crop globally")
             task = Task()
         self.task = task
+        self.is_val = is_val
+        self.val_ratio = val_ratio
 
         self.normalizing_dict = load_normalizing_dict(
             Path(root) / f"{FEATURES_DIR}/normalizing_dict.h5"
         )
+        self.update_labels(labels)
 
+    def paths_from_labels(self, labels: CropHarvestLabels) -> Tuple[List[Path], List[Path]]:
         positive_paths, negative_paths = labels.construct_positive_and_negative_labels(
-            task, filter_test=True
+            self.task, filter_test=True
         )
-        if val_ratio > 0.0:
+        if self.val_ratio > 0.0:
             # the fixed seed is to ensure the validation set is always
             # different from the training set
             positive_paths = deterministic_shuffle(positive_paths, seed=42)
             negative_paths = deterministic_shuffle(negative_paths, seed=42)
-            if is_val:
-                positive_paths = positive_paths[: int(len(positive_paths) * val_ratio)]
-                negative_paths = negative_paths[: int(len(negative_paths) * val_ratio)]
+            if self.is_val:
+                positive_paths = positive_paths[: int(len(positive_paths) * self.val_ratio)]
+                negative_paths = negative_paths[: int(len(negative_paths) * self.val_ratio)]
             else:
-                positive_paths = positive_paths[int(len(positive_paths) * val_ratio) :]
-                negative_paths = negative_paths[int(len(negative_paths) * val_ratio) :]
-
-        self.filepaths: List[Path] = positive_paths + negative_paths
-        self.y_vals: List[int] = [1] * len(positive_paths) + [0] * len(negative_paths)
+                positive_paths = positive_paths[int(len(positive_paths) * self.val_ratio) :]
+                negative_paths = negative_paths[int(len(negative_paths) * self.val_ratio) :]
+        return positive_paths, negative_paths
+
+    def update_labels(self, labels: CropHarvestLabels) -> None:
+        positive_paths, negative_paths = self.paths_from_labels(labels)
+        self.filepaths = positive_paths + negative_paths
+        self.y_vals = [1] * len(positive_paths) + [0] * len(negative_paths)
         self.positive_indices = list(range(len(positive_paths)))
         self.negative_indices = list(
             range(len(positive_paths), len(positive_paths) + len(negative_paths))
         )
-
-        # used in the sample() function, to ensure filepaths are sampled without
-        # duplication as much as possible
-        self.sampled_positive_indices: List[int] = []
-        self.sampled_negative_indices: List[int] = []
+        self.reset_sampled_indices()
 
     def reset_sampled_indices(self) -> None:
         self.sampled_positive_indices = []
         self.sampled_negative_indices = []
 
     def shuffle(self, seed: int) -> None:
         self.reset_sampled_indices()
@@ -440,15 +452,14 @@
         return f"{class_name}({self.id}, {self.task.test_identifier})"
 
     @property
     def id(self) -> str:
         return self.task.id
 
     def _get_positive_and_negative_indices(self) -> Tuple[List[int], List[int]]:
-
         positive_indices: List[int] = []
         negative_indices: List[int] = []
 
         for i, y_val in enumerate(self.y_vals):
             if y_val == 1:
                 positive_indices.append(i)
             else:
```

### Comparing `cropharvest-0.6.0/cropharvest/engineer.py` & `cropharvest-0.7.0/cropharvest/engineer.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from .utils import DATAFOLDER_PATH, load_normalizing_dict
 
 from typing import cast, Optional, Dict, Union, Tuple, List, Sequence
 
 
 @dataclass
 class DataInstance:
-
     dataset: str
     label_lat: float
     label_lon: float
     instance_lat: float
     instance_lon: float
     array: np.ndarray
     is_crop: int
@@ -72,15 +71,14 @@
     @classmethod
     def load_from_h5(cls, h5: h5py.File):
         x = h5.get("x")[:]
         return cls(x=x, y=h5.get("y")[:], lats=h5.get("lats")[:], lons=h5.get("lons")[:])
 
     @classmethod
     def load_from_nc(cls, filepaths: Union[Path, List[Path]]) -> Tuple:
-
         y: List[np.ndarray] = []
         preds: List[np.ndarray] = []
         lats: List[np.ndarray] = []
         lons: List[np.ndarray] = []
 
         if isinstance(filepaths, Path):
             filepaths = [filepaths]
@@ -264,28 +262,26 @@
             x = array[time_idx, :]
 
             delta = x - self.norm_interim["mean"]
             self.norm_interim["mean"] += delta / self.norm_interim["n"]
             self.norm_interim["M2"] += delta * (x - self.norm_interim["mean"])
 
     def calculate_normalizing_dict(self) -> Optional[Dict[str, np.ndarray]]:
-
         if "mean" not in self.norm_interim:
             print("No normalizing dict calculated! Make sure to call update_normalizing_values")
             return None
 
         variance = self.norm_interim["M2"] / (self.norm_interim["n"] - 1)
         std = np.sqrt(variance)
         return {"mean": cast(np.ndarray, self.norm_interim["mean"]), "std": cast(np.ndarray, std)}
 
     @staticmethod
     def adjust_normalizing_dict(
         dicts: Sequence[Tuple[int, Optional[Dict[str, np.ndarray]]]]
     ) -> Optional[Dict[str, np.ndarray]]:
-
         for _, single_dict in dicts:
             if single_dict is None:
                 return None
 
         dicts = cast(Sequence[Tuple[int, Dict[str, np.ndarray]]], dicts)
 
         new_total = sum([x[0] for x in dicts])
@@ -585,15 +581,14 @@
                     (self.labels[RequiredColumns.DATASET] == dataset)
                     & (self.labels[RequiredColumns.INDEX] == file_index)
                 )
             ].iloc[0]
 
             instance = self.process_single_file(file_path, row=file_row)
             if instance is not None:
-
                 hf = h5py.File(arrays_dir / file_name, "w")
                 hf.create_dataset("array", data=instance.array)
 
                 for key, val in instance.attrs.items():
                     hf.attrs[key] = val
                 hf.close()
```

### Comparing `cropharvest-0.6.0/cropharvest/eo/ee_boundingbox.py` & `cropharvest-0.7.0/cropharvest/eo/ee_boundingbox.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 @dataclass
 class EEBoundingBox(BBox):
     r"""
     A bounding box with additional earth-engine specific
     functionality
     """
 
-    def to_ee_polygon(self) -> ee.Geometry.Polygon:
-        return ee.Geometry.Polygon(
+    def to_ee_polygon(self) -> ee.Geometry:
+        return ee.Geometry(
             [
                 [
                     [self.min_lon, self.min_lat],
                     [self.min_lon, self.max_lat],
                     [self.max_lon, self.max_lat],
                     [self.max_lon, self.min_lat],
                 ]
@@ -34,16 +34,15 @@
         m_per_deg_lat, m_per_deg_lon = self.metre_per_degree(mid_lat)
 
         delta_lat = self.max_lat - self.min_lat
         delta_lon = self.max_lon - self.min_lon
 
         return delta_lat * m_per_deg_lat, delta_lon * m_per_deg_lon
 
-    def to_polygons(self, metres_per_patch: int = 3300) -> List[ee.Geometry.Polygon]:
-
+    def to_polygons(self, metres_per_patch: int = 3300) -> List[ee.Geometry]:
         lat_metres, lon_metres = self.to_metres()
 
         num_cols = int(lon_metres / metres_per_patch)
         num_rows = int(lat_metres / metres_per_patch)
 
         if num_cols == 0 or num_rows == 0:
             print(
@@ -56,15 +55,15 @@
             num_rows = 1
 
         print(f"Splitting into {num_cols} columns and {num_rows} rows")
 
         lon_size = (self.max_lon - self.min_lon) / num_cols
         lat_size = (self.max_lat - self.min_lat) / num_rows
 
-        output_polygons: List[ee.Geometry.Polygon] = []
+        output_polygons: List[ee.Geometry] = []
 
         cur_lon = self.min_lon
         while cur_lon < self.max_lon:
             cur_lat = self.min_lat
             while cur_lat < self.max_lat:
                 output_polygons.append(
                     ee.Geometry.Polygon(
@@ -102,15 +101,14 @@
 
         return m_per_degree_lat, m_per_degree_lon
 
     @staticmethod
     def from_centre(
         mid_lat: float, mid_lon: float, surrounding_metres: Union[int, Tuple[int, int]]
     ) -> "EEBoundingBox":
-
         m_per_deg_lat, m_per_deg_lon = EEBoundingBox.metre_per_degree(mid_lat)
 
         if isinstance(surrounding_metres, int):
             surrounding_metres = (surrounding_metres, surrounding_metres)
 
         surrounding_lat, surrounding_lon = surrounding_metres
 
@@ -119,15 +117,15 @@
 
         max_lat, min_lat = mid_lat + deg_lat, mid_lat - deg_lat
         max_lon, min_lon = mid_lon + deg_lon, mid_lon - deg_lon
 
         return EEBoundingBox(max_lon=max_lon, min_lon=min_lon, max_lat=max_lat, min_lat=min_lat)
 
     @staticmethod
-    def from_bounding_box(bounding_box: BBox, padding_metres: int) -> ee.Geometry.Polygon:
+    def from_bounding_box(bounding_box: BBox, padding_metres: int) -> "EEBoundingBox":
         # get the mid lat, in degrees (the bounding box function returns it in radians)
         mid_lat, _ = bounding_box.get_centre(in_radians=False)
         m_per_deg_lat, m_per_deg_lon = EEBoundingBox.metre_per_degree(mid_lat)
 
         extra_degrees_lon = padding_metres / m_per_deg_lon
         extra_degrees_lat = padding_metres / m_per_deg_lat
```

### Comparing `cropharvest-0.6.0/cropharvest/eo/eo.py` & `cropharvest-0.7.0/cropharvest/eo/eo.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,14 @@
 
         return labels
 
     @staticmethod
     def _filter_labels(
         labels: geopandas.GeoDataFrame, checkpoint: Optional[Path]
     ) -> geopandas.GeoDataFrame:
-
         # does not sort
         datasets = labels.dataset.unique()
 
         if checkpoint is None:
             # if we have no checkpoint folder, then we have no
             # downloaded files to check against
             return labels
@@ -208,15 +207,14 @@
         filename: str,
         description: str,
         drive_folder: Optional[str] = None,
         dest_bucket: Optional[str] = None,
         file_dimensions: Optional[int] = None,
         test: bool = False,
     ) -> ee.batch.Export:
-
         kwargs = dict(
             image=image.clip(region),
             description=description[:100],
             scale=10,
             region=region,
             maxPixels=1e13,
             fileDimensions=file_dimensions,
@@ -246,24 +244,23 @@
             print(f"Task not started! Got exception {e}")
             return task
 
         return task
 
     def _export_for_polygon(
         self,
-        polygon: ee.Geometry.Polygon,
+        polygon: ee.Geometry,
         polygon_identifier: Union[int, str],
         start_date: date,
         end_date: date,
         days_per_timestep: int = DAYS_PER_TIMESTEP,
         checkpoint: Optional[Path] = None,
         test: bool = False,
         file_dimensions: Optional[int] = None,
     ) -> bool:
-
         filename = str(polygon_identifier)
         if (checkpoint is not None) and (checkpoint / f"{filename}.tif").exists():
             print("File already exists! Skipping")
             return False
 
         # Description of the export cannot contain certrain characters
         description = filename.replace(".", "-").replace("=", "-").replace("/", "-")[:100]
@@ -344,17 +341,16 @@
 
         self._export(**kwargs)
         return True
 
     @classmethod
     def _labels_to_polygons_and_years(
         cls, labels: geopandas.GeoDataFrame, surrounding_metres: int
-    ) -> List[Tuple[ee.Geometry.Polygon, str, date, date]]:
-
-        output: List[ee.Geometry.Polygon] = []
+    ) -> List[Tuple[ee.Geometry, str, date, date]]:
+        output: List[Tuple[ee.Geometry, str, date, date]] = []
 
         print(f"Exporting {len(labels)} labels")
 
         for _, row in tqdm(labels.iterrows()):
             ee_bbox = EEBoundingBox.from_centre(
                 mid_lat=row[RequiredColumns.LAT],
                 mid_lon=row[RequiredColumns.LON],
@@ -377,15 +373,14 @@
                 )
             )
 
         return output
 
     @staticmethod
     def make_identifier(bbox: BBox, start_date, end_date) -> str:
-
         # Identifier is rounded to the nearest ~10m
         min_lon = round(bbox.min_lon, 4)
         min_lat = round(bbox.min_lat, 4)
         max_lon = round(bbox.max_lon, 4)
         max_lat = round(bbox.max_lat, 4)
         return (
             f"min_lat={min_lat}_min_lon={min_lon}_max_lat={max_lat}_max_lon={max_lon}_"
@@ -393,15 +388,14 @@
         )
 
     def export_for_test(
         self,
         padding_metres: int = 160,
         checkpoint: Optional[Path] = None,
     ) -> None:
-
         for identifier, bbox in TEST_REGIONS.items():
             polygon = EEBoundingBox.from_bounding_box(
                 bounding_box=bbox, padding_metres=padding_metres
             ).to_ee_polygon()
             _, _, year, _ = identifier.split("_")
             end_date = date(int(year), EXPORT_END_MONTH, EXPORT_END_DAY)
             start_date = end_date - timedelta(days=DAYS_PER_TIMESTEP * DEFAULT_NUM_TIMESTEPS)
@@ -419,15 +413,14 @@
         bbox: BBox,
         bbox_name: str,
         start_date: date,
         end_date: date,
         metres_per_polygon: Optional[int] = 10000,
         file_dimensions: Optional[int] = None,
     ) -> Dict[str, bool]:
-
         if start_date > end_date:
             raise ValueError(f"Start date {start_date} is after end date {end_date}")
 
         ee_bbox = EEBoundingBox.from_bounding_box(bounding_box=bbox, padding_metres=0)
         if metres_per_polygon is not None:
             regions = ee_bbox.to_polygons(metres_per_patch=metres_per_polygon)
             ids = [f"batch_{i}/{i}" for i in range(len(regions))]
@@ -452,15 +445,14 @@
         labels: Optional[geopandas.GeoDataFrame] = None,
         dataset: Optional[str] = None,
         num_labelled_points: Optional[int] = 3000,
         surrounding_metres: int = 80,
         checkpoint: Optional[Path] = None,
         start_from_last: bool = False,
     ) -> None:
-
         if labels is None:
             labels = self.load_default_labels(
                 dataset=dataset, start_from_last=start_from_last, checkpoint=checkpoint
             )
         else:
             if dataset is not None:
                 print("No dataset can be specified if passing a different set of labels")
```

### Comparing `cropharvest-0.6.0/cropharvest/eo/era5.py` & `cropharvest-0.7.0/cropharvest/eo/era5.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from cropharvest.bands import ERA5_BANDS as BANDS
 from .utils import date_to_string
 
 image_collection = "ECMWF/ERA5_LAND/MONTHLY"
 
 
 def get_single_image(region: ee.Geometry, start_date: date, end_date: date) -> ee.Image:
-
     # This only really works with the values currently in config.
     # What happens is that the images are associated with the first day of the month,
     # so if we just use the given start_date and end_date, then we will often get
     # the image from the following month (e.g. the start and end dates of
     # 2016-02-07, 2016-03-08 respectively return data from March 2016, even though
     # February 2016 has a much higher overlap). It also means that the final month
     # timestep, with range 2017-01-02 to 2017-02-01 was returning no data (but we'd)
```

### Comparing `cropharvest-0.6.0/cropharvest/eo/sentinel1.py` & `cropharvest-0.7.0/cropharvest/eo/sentinel1.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 image_collection = "COPERNICUS/S1_GRD"
 
 
 def get_image_collection(
     region: ee.Geometry, start_date: date, end_date: date
 ) -> Tuple[ee.ImageCollection, ee.ImageCollection]:
-
     dates = ee.DateRange(
         date_to_string(start_date),
         date_to_string(end_date),
     )
 
     startDate = ee.DateRange(dates).start()
     endDate = ee.DateRange(dates).end()
@@ -61,15 +60,14 @@
 def get_single_image(
     region: ee.Geometry,
     start_date: date,
     end_date: date,
     vv_imcol: ee.ImageCollection,
     vh_imcol: ee.ImageCollection,
 ) -> ee.Image:
-
     mid_date = start_date + ((end_date - start_date) / 2)
 
     kept_vv = _get_closest_dates(mid_date, vv_imcol)
     kept_vh = _get_closest_dates(mid_date, vh_imcol)
 
     composite = ee.Image.cat(
         [
```

### Comparing `cropharvest-0.6.0/cropharvest/eo/sentinel2.py` & `cropharvest-0.7.0/cropharvest/eo/sentinel2.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
 # images with less than this many cloud pixels will be used with normal
 # mosaicing (most recent on top)
 cloudFreeKeepThresh = 3
 
 
 def get_single_image(region: ee.Geometry, start_date: date, end_date: date) -> ee.Image:
-
     dates = ee.DateRange(
         date_to_string(start_date),
         date_to_string(end_date),
     )
 
     startDate = ee.DateRange(dates).start()
     endDate = ee.DateRange(dates).end()
```

### Comparing `cropharvest-0.6.0/cropharvest/eo/utils.py` & `cropharvest-0.7.0/cropharvest/eo/utils.py`

 * *Files identical despite different names*

### Comparing `cropharvest-0.6.0/cropharvest/inference.py` & `cropharvest-0.7.0/cropharvest/inference.py`

 * *Files identical despite different names*

### Comparing `cropharvest-0.6.0/cropharvest/utils.py` & `cropharvest-0.7.0/cropharvest/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import h5py
 from pathlib import Path
 from tqdm import tqdm
 from urllib.request import urlopen, Request
 import numpy as np
 import random
 import geopandas
-import collections
+import collections.abc
 import functools
 import tarfile
 
 from typing import Dict, List, Tuple, Optional
 
 from cropharvest.config import DATASET_URL
 
@@ -63,21 +63,19 @@
         extract_archive(targz_path)
     else:
         url = f"{DATASET_URL}/files/{file_path.name}?download=1"
         download_from_url(url, file_path_str)
 
 
 def load_normalizing_dict(path_to_dict: Path) -> Dict[str, np.ndarray]:
-
     hf = h5py.File(path_to_dict, "r")
     return {"mean": hf.get("mean")[:], "std": hf.get("std")[:]}
 
 
 def deterministic_shuffle(x: List, seed: int) -> List:
-
     output_list: List = []
     x = x.copy()
 
     if seed % 2 == 0:
         seed = -seed
     while len(x) > 0:
         if abs(seed) >= len(x):
@@ -91,15 +89,14 @@
         seed *= -1
     return output_list
 
 
 def sample_with_memory(
     indices: List[int], k: int, state: Optional[List[int]] = None
 ) -> Tuple[List[int], List[int]]:
-
     if state is None:
         state = []
 
     indices_to_sample = list(set(indices) - set(state))
     if len(indices_to_sample) < k:
         # restart the state
         state, indices_to_sample = [], indices
@@ -117,15 +114,15 @@
     """
 
     def __init__(self, func):
         self.func = func
         self.cache = {}
 
     def __call__(self, *args):
-        if not isinstance(args, collections.Hashable):
+        if not isinstance(args, collections.abc.Hashable):
             # uncacheable. a list, for instance.
             # better to not cache than blow up.
             return self.func(*args)
         if args in self.cache:
             return self.cache[args]
         else:
             value = self.func(*args)
```

### Comparing `cropharvest-0.6.0/cropharvest.egg-info/PKG-INFO` & `cropharvest-0.7.0/cropharvest.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6372 6f70  : 2.1.Name: crop
 00000020: 6861 7276 6573 740a 5665 7273 696f 6e3a  harvest.Version:
-00000030: 2030 2e36 2e30 0a53 756d 6d61 7279 3a20   0.6.0.Summary: 
+00000030: 2030 2e37 2e30 0a53 756d 6d61 7279 3a20   0.7.0.Summary: 
 00000040: 4f70 656e 2073 6f75 7263 6520 7265 6d6f  Open source remo
 00000050: 7465 2073 656e 7369 6e67 2064 6174 6173  te sensing datas
 00000060: 6574 2077 6974 6820 6265 6e63 686d 6172  et with benchmar
 00000070: 6b73 0a48 6f6d 652d 7061 6765 3a20 6874  ks.Home-page: ht
 00000080: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000090: 2f6e 6173 6168 6172 7665 7374 2f63 726f  /nasaharvest/cro
 000000a0: 7068 6172 7665 7374 0a41 7574 686f 723a  pharvest.Author:
@@ -22,527 +22,555 @@
 00000150: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
 00000160: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
 00000170: 6e64 656e 740a 5265 7175 6972 6573 2d50  ndent.Requires-P
 00000180: 7974 686f 6e3a 203e 3d33 2e36 0a44 6573  ython: >=3.6.Des
 00000190: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
 000001a0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
 000001b0: 646f 776e 0a4c 6963 656e 7365 2d46 696c  down.License-Fil
-000001c0: 653a 204c 4943 454e 5345 2e74 7874 0a0a  e: LICENSE.txt..
-000001d0: 2320 4372 6f70 4861 7276 6573 740a 0a43  # CropHarvest..C
-000001e0: 726f 7048 6172 7665 7374 2069 7320 616e  ropHarvest is an
-000001f0: 206f 7065 6e20 736f 7572 6365 2072 656d   open source rem
-00000200: 6f74 6520 7365 6e73 696e 6720 6461 7461  ote sensing data
-00000210: 7365 7420 666f 7220 6167 7269 6375 6c74  set for agricult
-00000220: 7572 6520 7769 7468 2062 656e 6368 6d61  ure with benchma
-00000230: 726b 732e 2049 7420 636f 6c6c 6563 7473  rks. It collects
-00000240: 2064 6174 6120 6672 6f6d 2061 2076 6172   data from a var
-00000250: 6965 7479 206f 6620 6167 7269 6375 6c74  iety of agricult
-00000260: 7572 616c 206c 616e 6420 7573 6520 6461  ural land use da
-00000270: 7461 7365 7473 2061 6e64 2072 656d 6f74  tasets and remot
-00000280: 6520 7365 6e73 696e 6720 7072 6f64 7563  e sensing produc
-00000290: 7473 2e0a 0a0a 5468 6520 6461 7461 7365  ts....The datase
-000002a0: 7420 636f 6e73 6973 7473 206f 6620 2a2a  t consists of **
-000002b0: 3935 2c31 3836 2a2a 2064 6174 6170 6f69  95,186** datapoi
-000002c0: 6e74 732c 206f 6620 7768 6963 6820 2a2a  nts, of which **
-000002d0: 3333 2c32 3035 2a2a 2028 3335 2529 2068  33,205** (35%) h
-000002e0: 6176 6520 6d75 6c74 6963 6c61 7373 206c  ave multiclass l
-000002f0: 6162 656c 732e 2041 6c6c 206f 7468 6572  abels. All other
-00000300: 2064 6174 6170 6f69 6e74 7320 6f6e 6c79   datapoints only
-00000310: 2068 6176 6520 6269 6e61 7279 2063 726f   have binary cro
-00000320: 7020 2f20 6e6f 6e2d 6372 6f70 206c 6162  p / non-crop lab
-00000330: 656c 732e 0a0a 2a2a 3730 2c32 3133 2a2a  els...**70,213**
-00000340: 2028 3734 2529 206f 6620 7468 6573 6520   (74%) of these 
-00000350: 6c61 6265 6c73 2061 7265 2070 6169 7265  labels are paire
-00000360: 6420 7769 7468 2072 656d 6f74 6520 7365  d with remote se
-00000370: 6e73 696e 6720 616e 6420 636c 696d 6174  nsing and climat
-00000380: 6f6c 6f67 7920 6461 7461 2c20 7370 6563  ology data, spec
-00000390: 6966 6963 616c 6c79 205b 5365 6e74 696e  ifically [Sentin
-000003a0: 656c 2d32 5d28 6874 7470 733a 2f2f 7365  el-2](https://se
-000003b0: 6e74 696e 656c 2e65 7361 2e69 6e74 2f77  ntinel.esa.int/w
-000003c0: 6562 2f73 656e 7469 6e65 6c2f 6d69 7373  eb/sentinel/miss
-000003d0: 696f 6e73 2f73 656e 7469 6e65 6c2d 3229  ions/sentinel-2)
-000003e0: 2c20 5b53 656e 7469 6e65 6c2d 315d 2868  , [Sentinel-1](h
-000003f0: 7474 7073 3a2f 2f73 656e 7469 6e65 6c2e  ttps://sentinel.
-00000400: 6573 612e 696e 742f 7765 622f 7365 6e74  esa.int/web/sent
-00000410: 696e 656c 2f6d 6973 7369 6f6e 732f 7365  inel/missions/se
-00000420: 6e74 696e 656c 2d31 2f29 2c20 7468 6520  ntinel-1/), the 
-00000430: 5b53 5254 4d20 4469 6769 7461 6c20 456c  [SRTM Digital El
-00000440: 6576 6174 696f 6e20 4d6f 6465 6c5d 2868  evation Model](h
-00000450: 7474 7073 3a2f 2f63 6769 6172 6373 692e  ttps://cgiarcsi.
-00000460: 636f 6d6d 756e 6974 792f 6461 7461 2f73  community/data/s
-00000470: 7274 6d2d 3930 6d2d 6469 6769 7461 6c2d  rtm-90m-digital-
-00000480: 656c 6576 6174 696f 6e2d 6461 7461 6261  elevation-databa
-00000490: 7365 2d76 342d 312f 2920 616e 6420 5b45  se-v4-1/) and [E
-000004a0: 5241 2035 2063 6c69 6d61 746f 6c6f 6779  RA 5 climatology
-000004b0: 2064 6174 615d 2868 7474 7073 3a2f 2f77   data](https://w
-000004c0: 7777 2e65 636d 7766 2e69 6e74 2f65 6e2f  ww.ecmwf.int/en/
-000004d0: 666f 7265 6361 7374 732f 6461 7461 7365  forecasts/datase
-000004e0: 7473 2f72 6561 6e61 6c79 7369 732d 6461  ts/reanalysis-da
-000004f0: 7461 7365 7473 2f65 7261 3529 2e0a 0a32  tasets/era5)...2
-00000500: 3120 6461 7461 7365 7473 2061 7265 2061  1 datasets are a
-00000510: 6767 7265 6761 7465 6420 696e 746f 2043  ggregated into C
-00000520: 726f 7048 6172 7665 7374 202d 2074 6865  ropHarvest - the
-00000530: 7365 2061 7265 2064 6f63 756d 656e 7465  se are documente
-00000540: 6420 5b68 6572 655d 2868 7474 7073 3a2f  d [here](https:/
-00000550: 2f67 6974 6875 622e 636f 6d2f 6e61 7361  /github.com/nasa
-00000560: 6861 7276 6573 742f 6372 6f70 6861 7276  harvest/cropharv
-00000570: 6573 742f 626c 6f62 2f6d 6169 6e2f 6461  est/blob/main/da
-00000580: 7461 7365 7473 2e6d 6429 2e0a 0a4d 6f72  tasets.md)...Mor
-00000590: 6520 6465 7461 696c 7320 6162 6f75 7420  e details about 
-000005a0: 4372 6f70 4861 7276 6573 7420 616e 6420  CropHarvest and 
-000005b0: 7468 6520 6265 6e63 686d 6172 6b73 2061  the benchmarks a
-000005c0: 7265 2061 7661 696c 6162 6c65 2069 6e20  re available in 
-000005d0: 5b74 6869 7320 7061 7065 725d 2868 7474  [this paper](htt
-000005e0: 7073 3a2f 2f6f 7065 6e72 6576 6965 772e  ps://openreview.
-000005f0: 6e65 742f 666f 7275 6d3f 6964 3d4a 746a  net/forum?id=Jtj
-00000600: 7a55 5850 4561 4375 292e 0a0a 2323 2320  zUXPEaCu)...### 
-00000610: 5069 7065 6c69 6e65 0a54 6865 2063 6f64  Pipeline.The cod
-00000620: 6520 696e 2074 6869 7320 7265 706f 7369  e in this reposi
-00000630: 746f 7279 0a0a 3129 2063 6f6d 6269 6e65  tory..1) combine
-00000640: 7320 7468 6520 636f 6e73 7469 7475 656e  s the constituen
-00000650: 7420 6461 7461 7365 7473 2069 6e74 6f20  t datasets into 
-00000660: 6120 7369 6e67 6c65 2067 656f 4a53 4f4e  a single geoJSON
-00000670: 2066 696c 652c 0a32 2920 6578 706f 7274   file,.2) export
-00000680: 7320 7468 6520 6173 736f 6369 6174 6564  s the associated
-00000690: 2073 6174 656c 6c69 7465 2064 6174 6120   satellite data 
-000006a0: 6672 6f6d 2045 6172 7468 2045 6e67 696e  from Earth Engin
-000006b0: 652c 0a33 2920 636f 6d62 696e 6573 2062  e,.3) combines b
-000006c0: 6f74 6820 6461 7461 7365 7473 2074 6f20  oth datasets to 
-000006d0: 6372 6561 7465 2060 2858 2c79 2960 2074  create `(X,y)` t
-000006e0: 7261 696e 696e 6720 7475 706c 6573 2061  raining tuples a
-000006f0: 6e64 0a34 2920 6578 706f 7365 7320 7468  nd.4) exposes th
-00000700: 6f73 6520 7475 706c 6573 2076 6961 2061  ose tuples via a
-00000710: 2060 4461 7461 7365 7460 206f 626a 6563   `Dataset` objec
-00000720: 742e 0a0a 5468 6520 7069 7065 6c69 6e65  t...The pipeline
-00000730: 2074 6872 6f75 6768 2077 6869 6368 2074   through which t
-00000740: 6869 7320 6861 7070 656e 7320 6973 2073  his happens is s
-00000750: 686f 776e 2062 656c 6f77 3a0a 0a0a 416c  hown below:...Al
-00000760: 6c20 626c 7565 2062 6f78 6573 2061 7265  l blue boxes are
-00000770: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-00000780: 2063 6f64 6520 696e 2074 6869 7320 7265   code in this re
-00000790: 706f 7369 746f 7279 2e20 416e 7974 6869  pository. Anythi
-000007a0: 6e67 2067 7265 656e 2069 7320 6461 7461  ng green is data
-000007b0: 2061 6363 6573 7369 626c 6520 7669 6120   accessible via 
-000007c0: 5b5a 656e 6f64 6f5d 2868 7474 7073 3a2f  [Zenodo](https:/
-000007d0: 2f7a 656e 6f64 6f2e 6f72 672f 7265 636f  /zenodo.org/reco
-000007e0: 7264 2f35 3832 3838 3933 292e 2042 7920  rd/5828893). By 
-000007f0: 6465 6661 756c 742c 2074 6865 205a 656e  default, the Zen
-00000800: 6f64 6f20 6461 7461 2077 696c 6c20 6765  odo data will ge
-00000810: 7420 646f 776e 6c6f 6164 6564 2074 6f20  t downloaded to 
-00000820: 7468 6520 5b64 6174 6120 666f 6c64 6572  the [data folder
-00000830: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000840: 2e63 6f6d 2f6e 6173 6168 6172 7665 7374  .com/nasaharvest
-00000850: 2f63 726f 7068 6172 7665 7374 2f74 7265  /cropharvest/tre
-00000860: 652f 6d61 696e 2f64 6174 6129 202d 2074  e/main/data) - t
-00000870: 6865 2064 6174 6120 666f 6c64 6572 2773  he data folder's
-00000880: 205b 5265 6164 6d65 5d28 6874 7470 733a   [Readme](https:
-00000890: 2f2f 6769 7468 7562 2e63 6f6d 2f6e 6173  //github.com/nas
-000008a0: 6168 6172 7665 7374 2f63 726f 7068 6172  aharvest/crophar
-000008b0: 7665 7374 2f62 6c6f 622f 6d61 696e 2f64  vest/blob/main/d
-000008c0: 6174 612f 5245 4144 4d45 2e6d 6429 2068  ata/README.md) h
-000008d0: 6173 206d 6f72 6520 696e 666f 726d 6174  as more informat
-000008e0: 696f 6e20 6162 6f75 7420 7468 6520 6578  ion about the ex
-000008f0: 6163 7420 7374 7275 6374 7572 6520 6f66  act structure of
-00000900: 2074 6865 2064 6174 612e 0a0a 5468 6572   the data...Ther
-00000910: 6520 6172 6520 756e 6971 7565 2063 6173  e are unique cas
-00000920: 6573 2077 6865 7265 2079 6f75 206d 6179  es where you may
-00000930: 206e 6565 6420 746f 2075 7365 2074 6865   need to use the
-00000940: 2060 4561 7274 6845 6e67 696e 6545 7870   `EarthEngineExp
-00000950: 6f72 7465 7260 2064 6972 6563 746c 792c  orter` directly,
-00000960: 2074 6865 7365 2075 7365 2063 6173 6573   these use cases
-00000970: 2061 7265 2064 656d 6f6e 7374 7261 7465   are demonstrate
-00000980: 6420 696e 2074 6865 205b 6064 656d 6f5f  d in the [`demo_
-00000990: 6578 706f 7274 696e 675f 6461 7461 2e69  exporting_data.i
-000009a0: 7079 6e62 605d 2868 7474 7073 3a2f 2f67  pynb`](https://g
-000009b0: 6974 6875 622e 636f 6d2f 6e61 7361 6861  ithub.com/nasaha
-000009c0: 7276 6573 742f 6372 6f70 6861 7276 6573  rvest/cropharves
-000009d0: 742f 626c 6f62 2f6d 6169 6e2f 6465 6d6f  t/blob/main/demo
-000009e0: 5f65 7870 6f72 7469 6e67 5f64 6174 612e  _exporting_data.
-000009f0: 6970 796e 6229 206e 6f74 6562 6f6f 6b2e  ipynb) notebook.
-00000a00: 0a0a 2323 2320 496e 7374 616c 6c61 7469  ..### Installati
-00000a10: 6f6e 0a4c 696e 7578 2061 6e64 204d 6163  on.Linux and Mac
-00000a20: 4f53 2075 7365 7273 2063 616e 2069 6e73  OS users can ins
-00000a30: 7461 6c6c 2074 6865 206c 6174 6573 7420  tall the latest 
-00000a40: 7665 7273 696f 6e20 6f66 2043 726f 7048  version of CropH
-00000a50: 6172 7665 7374 2077 6974 6820 7468 6520  arvest with the 
-00000a60: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
-00000a70: 643a 0a60 6060 6261 7368 0a70 6970 2069  d:.```bash.pip i
-00000a80: 6e73 7461 6c6c 2063 726f 7068 6172 7665  nstall cropharve
-00000a90: 7374 0a60 6060 0a57 696e 646f 7773 2075  st.```.Windows u
-00000aa0: 7365 7273 206d 7573 7420 696e 7374 616c  sers must instal
-00000ab0: 6c20 7468 6520 4372 6f70 4861 7276 6573  l the CropHarves
-00000ac0: 7420 7769 7468 696e 2061 205b 636f 6e64  t within a [cond
-00000ad0: 615d 2868 7474 7073 3a2f 2f64 6f63 732e  a](https://docs.
-00000ae0: 636f 6e64 612e 696f 2f65 6e2f 6c61 7465  conda.io/en/late
-00000af0: 7374 2f6d 696e 6963 6f6e 6461 2e68 746d  st/miniconda.htm
-00000b00: 6c29 2065 6e76 6972 6f6e 6d65 6e74 2074  l) environment t
-00000b10: 6f20 656e 7375 7265 2061 6c6c 2064 6570  o ensure all dep
-00000b20: 656e 6465 6e63 6965 7320 6172 6520 696e  endencies are in
-00000b30: 7374 616c 6c65 6420 636f 7272 6563 746c  stalled correctl
-00000b40: 793a 0a60 6060 6261 7368 0a63 6f6e 6461  y:.```bash.conda
-00000b50: 2069 6e73 7461 6c6c 2027 6669 6f6e 613e   install 'fiona>
-00000b60: 3d31 2e35 2720 2772 6173 7465 7269 6f3e  =1.5' 'rasterio>
-00000b70: 3d31 2e32 2e36 270a 7069 7020 696e 7374  =1.2.6'.pip inst
-00000b80: 616c 6c20 6372 6f70 6861 7276 6573 740a  all cropharvest.
-00000b90: 6060 600a 0a23 2323 2047 6574 7469 6e67  ```..### Getting
-00000ba0: 2073 7461 7274 6564 205b 215b 4f70 656e   started [![Open
-00000bb0: 2049 6e20 436f 6c61 625d 2868 7474 7073   In Colab](https
-00000bc0: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
-00000bd0: 682e 676f 6f67 6c65 2e63 6f6d 2f61 7373  h.google.com/ass
-00000be0: 6574 732f 636f 6c61 622d 6261 6467 652e  ets/colab-badge.
-00000bf0: 7376 6729 5d28 6874 7470 733a 2f2f 636f  svg)](https://co
-00000c00: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00000c10: 676c 652e 636f 6d2f 6769 7468 7562 2f6e  gle.com/github/n
-00000c20: 6173 6168 6172 7665 7374 2f63 726f 7068  asaharvest/croph
-00000c30: 6172 7665 7374 2f62 6c6f 622f 6d61 696e  arvest/blob/main
-00000c40: 2f64 656d 6f2e 6970 796e 6229 0a53 6565  /demo.ipynb).See
-00000c50: 2074 6865 205b 6064 656d 6f2e 6970 796e   the [`demo.ipyn
-00000c60: 6260 5d28 6874 7470 733a 2f2f 6769 7468  b`](https://gith
-00000c70: 7562 2e63 6f6d 2f6e 6173 6168 6172 7665  ub.com/nasaharve
-00000c80: 7374 2f63 726f 7068 6172 7665 7374 2f62  st/cropharvest/b
-00000c90: 6c6f 622f 6d61 696e 2f64 656d 6f2e 6970  lob/main/demo.ip
-00000ca0: 796e 6229 206e 6f74 6562 6f6f 6b20 666f  ynb) notebook fo
-00000cb0: 7220 616e 2065 7861 6d70 6c65 206f 6e20  r an example on 
-00000cc0: 686f 7720 746f 2064 6f77 6e6c 6f61 6420  how to download 
-00000cd0: 7468 6520 6461 7461 2066 726f 6d20 5b5a  the data from [Z
-00000ce0: 656e 6f64 6f5d 2868 7474 7073 3a2f 2f7a  enodo](https://z
-00000cf0: 656e 6f64 6f2e 6f72 672f 7265 636f 7264  enodo.org/record
-00000d00: 2f37 3235 3736 3838 2920 616e 6420 7472  /7257688) and tr
-00000d10: 6169 6e20 6120 7261 6e64 6f6d 2066 6f72  ain a random for
-00000d20: 6573 7420 6167 6169 6e73 7420 7468 6973  est against this
-00000d30: 2064 6174 612e 0a0a 466f 7220 6d6f 7265   data...For more
-00000d40: 2065 7861 6d70 6c65 7320 6f66 206d 6f64   examples of mod
-00000d50: 656c 7320 7472 6169 6e65 6420 6167 6169  els trained agai
-00000d60: 6e73 7420 7468 6973 2064 6174 6173 6574  nst this dataset
-00000d70: 2c20 7365 6520 7468 6520 5b62 656e 6368  , see the [bench
-00000d80: 6d61 726b 735d 2868 7474 7073 3a2f 2f67  marks](https://g
-00000d90: 6974 6875 622e 636f 6d2f 6e61 7361 6861  ithub.com/nasaha
-00000da0: 7276 6573 742f 6372 6f70 6861 7276 6573  rvest/cropharves
-00000db0: 742f 626c 6f62 2f6d 6169 6e2f 6265 6e63  t/blob/main/benc
-00000dc0: 686d 6172 6b73 292e 0a0a 2323 2320 436f  hmarks)...### Co
-00000dd0: 6e74 7269 6275 7469 6e67 0a49 6620 796f  ntributing.If yo
-00000de0: 7520 776f 756c 6420 6c69 6b65 2074 6f20  u would like to 
-00000df0: 636f 6e74 7269 6275 7465 2061 2064 6174  contribute a dat
-00000e00: 6173 6574 2c20 706c 6561 7365 2073 6565  aset, please see
-00000e10: 2074 6865 205b 636f 6e74 7269 6275 7469   the [contributi
-00000e20: 6e67 2072 6561 646d 655d 2868 7474 7073  ng readme](https
-00000e30: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e61  ://github.com/na
-00000e40: 7361 6861 7276 6573 742f 6372 6f70 6861  saharvest/cropha
-00000e50: 7276 6573 742f 626c 6f62 2f6d 6169 6e2f  rvest/blob/main/
-00000e60: 636f 6e74 7269 6275 7469 6e67 2e6d 6429  contributing.md)
-00000e70: 2e0a 0a23 2323 207e 7e46 4151 7e7e 2051  ...### ~~FAQ~~ Q
-00000e80: 7565 7374 696f 6e73 2061 736b 6564 2061  uestions asked a
-00000e90: 7420 6c65 6173 7420 6f6e 6365 0a0a 3c64  t least once..<d
-00000ea0: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
-00000eb0: 3e3c 6120 6872 6566 3d68 7474 7073 3a2f  ><a href=https:/
-00000ec0: 2f67 6974 6875 622e 636f 6d2f 6e61 7361  /github.com/nasa
-00000ed0: 6861 7276 6573 742f 6372 6f70 6861 7276  harvest/cropharv
-00000ee0: 6573 742f 6973 7375 6573 2f39 353e 486f  est/issues/95>Ho
-00000ef0: 7720 646f 2049 2075 7365 2043 726f 7048  w do I use CropH
-00000f00: 6172 7665 7374 2066 6f72 2061 2073 7065  arvest for a spe
-00000f10: 6369 6669 6320 6765 6f67 7261 7068 793f  cific geography?
-00000f20: 3c2f 613e 3c2f 7375 6d6d 6172 793e 0a0a  </a></summary>..
-00000f30: 416c 6c20 7468 6520 6461 7461 2069 7320  All the data is 
-00000f40: 6163 6365 7373 6962 6c65 2074 6872 6f75  accessible throu
-00000f50: 6768 2074 6865 2060 6372 6f70 6861 7276  gh the `cropharv
-00000f60: 6573 742e 6461 7461 7365 7473 2e43 726f  est.datasets.Cro
-00000f70: 7048 6172 7665 7374 6020 6f62 6a65 6374  pHarvest` object
-00000f80: 2e20 5468 6520 6d61 696e 2070 6172 616d  . The main param
-00000f90: 6574 6572 7320 7768 6963 6820 796f 7520  eters which you 
-00000fa0: 6d69 6768 7420 6265 2069 6e74 6572 6573  might be interes
-00000fb0: 7465 6420 696e 206d 616e 6970 756c 6174  ted in manipulat
-00000fc0: 696e 6720 6172 6520 636f 6e74 726f 6c6c  ing are controll
-00000fd0: 6162 6c65 2074 6872 6f75 6768 2061 2060  able through a `
-00000fe0: 6372 6f70 6861 7276 6573 742e 6461 7461  cropharvest.data
-00000ff0: 7365 7473 2e54 6173 6b60 2c20 7768 6963  sets.Task`, whic
-00001000: 6820 7461 6b65 7320 6173 2069 6e70 7574  h takes as input
-00001010: 2074 6865 2066 6f6c 6c6f 7769 6e67 2070   the following p
-00001020: 6172 616d 6574 6572 733a 0a2d 2041 2062  arameters:.- A b
-00001030: 6f75 6e64 696e 6720 626f 782c 2077 6869  ounding box, whi
-00001040: 6368 2064 6566 696e 6573 2074 6865 2073  ch defines the s
-00001050: 7061 7469 616c 2062 6f75 6e64 6172 6965  patial boundarie
-00001060: 7320 6f66 2074 6865 206c 6162 656c 7320  s of the labels 
-00001070: 7265 7472 6965 7665 730a 2d20 4120 7461  retrieves.- A ta
-00001080: 7267 6574 206c 6162 656c 2c20 7768 6963  rget label, whic
-00001090: 6820 6465 6669 6e65 7320 7468 6520 636c  h defines the cl
-000010a0: 6173 7320 6f66 2074 6865 2070 6f73 6974  ass of the posit
-000010b0: 6976 6520 6c61 6265 6c73 2028 6966 2074  ive labels (if t
-000010c0: 6869 7320 6973 206c 6566 7420 746f 2060  his is left to `
-000010d0: 4e6f 6e65 602c 2074 6865 6e20 7468 6520  None`, then the 
-000010e0: 706f 7369 7469 7665 2063 6c61 7373 2077  positive class w
-000010f0: 696c 6c20 6265 2063 726f 7073 2061 6e64  ill be crops and
-00001100: 2074 6865 206e 6567 6174 6976 6520 636c   the negative cl
-00001110: 6173 7320 7769 6c6c 2062 6520 6e6f 6e2d  ass will be non-
-00001120: 6372 6f70 7329 0a2d 2041 2062 6f6f 6c65  crops).- A boole
-00001130: 616e 2064 6566 696e 696e 6720 7768 6574  an defining whet
-00001140: 6865 7220 6f72 206e 6f74 2074 6f20 6261  her or not to ba
-00001150: 6c61 6e63 6520 7468 6520 6372 6f70 7320  lance the crops 
-00001160: 616e 6420 6e6f 6e2d 6372 6f70 7320 696e  and non-crops in
-00001170: 2074 6865 206e 6567 6174 6976 6520 636c   the negative cl
-00001180: 6173 730a 2d20 4120 7465 7374 5f69 6465  ass.- A test_ide
-00001190: 6e74 6966 6965 7220 7374 7269 6e67 2c20  ntifier string, 
-000011a0: 7768 6963 6820 7465 6c6c 7320 7468 6520  which tells the 
-000011b0: 6461 7461 7365 7420 7768 6574 6865 7220  dataset whether 
-000011c0: 6f72 206e 6f74 2074 6f20 7265 7472 6965  or not to retrie
-000011d0: 7665 2061 2066 696c 6520 6672 6f6d 2074  ve a file from t
-000011e0: 6865 2060 7465 7374 5f66 6561 7475 7265  he `test_feature
-000011f0: 7360 2066 6f6c 6465 7220 616e 6420 7265  s` folder and re
-00001200: 7475 726e 2069 7420 6173 2074 6865 2074  turn it as the t
-00001210: 6573 7420 6461 7461 2e0a 0a53 6f20 6966  est data...So if
-00001220: 2049 2077 616e 7465 6420 746f 2075 7365   I wanted to use
-00001230: 2074 6869 7320 746f 2074 7261 696e 2061   this to train a
-00001240: 206d 6f64 656c 2074 6f20 6964 656e 7469   model to identi
-00001250: 6679 2063 726f 7020 7673 2e20 6e6f 6e20  fy crop vs. non 
-00001260: 6372 6f70 2069 6e20 4672 616e 6365 2c20  crop in France, 
-00001270: 4920 6d69 6768 7420 646f 2069 7420 6c69  I might do it li
-00001280: 6b65 2074 6869 733a 0a0a 6060 6070 7974  ke this:..```pyt
-00001290: 686f 6e0a 6672 6f6d 2073 6b6c 6561 726e  hon.from sklearn
-000012a0: 2e65 6e73 656d 626c 6520 696d 706f 7274  .ensemble import
-000012b0: 2052 616e 646f 6d46 6f72 6573 7443 6c61   RandomForestCla
-000012c0: 7373 6966 6965 720a 0a66 726f 6d20 6372  ssifier..from cr
-000012d0: 6f70 6861 7276 6573 742e 6461 7461 7365  opharvest.datase
-000012e0: 7473 2069 6d70 6f72 7420 5461 736b 2c20  ts import Task, 
-000012f0: 4372 6f70 4861 7276 6573 740a 6672 6f6d  CropHarvest.from
-00001300: 2063 726f 7068 6172 7665 7374 2e63 6f75   cropharvest.cou
-00001310: 6e74 7269 6573 2069 6d70 6f72 7420 6765  ntries import ge
-00001320: 745f 636f 756e 7472 795f 6262 6f78 0a0a  t_country_bbox..
-00001330: 2320 666f 6c64 6572 2069 6e74 6f20 7768  # folder into wh
-00001340: 6963 6820 7468 6520 6461 7461 2077 696c  ich the data wil
-00001350: 6c20 6265 2064 6f77 6e6c 6f61 6465 6420  l be downloaded 
-00001360: 2f20 616c 7265 6164 7920 6578 6973 7473  / already exists
-00001370: 0a64 6174 615f 6469 7220 3d20 2264 6174  .data_dir = "dat
-00001380: 6122 0a0a 2320 6765 745f 636f 756e 7472  a"..# get_countr
-00001390: 795f 6262 6f78 2072 6574 7572 6e73 2061  y_bbox returns a
-000013a0: 206c 6973 7420 6f66 2062 6f75 6e64 696e   list of boundin
-000013b0: 6720 626f 7865 732e 0a23 2074 6865 206f  g boxes..# the o
-000013c0: 6e65 2072 6570 7265 7365 6e74 696e 6720  ne representing 
-000013d0: 4d65 7472 6f70 6f6c 6974 616e 2046 7261  Metropolitan Fra
-000013e0: 6e63 6520 6973 2074 6865 2032 6e64 2062  nce is the 2nd b
-000013f0: 6f78 0a6d 6574 726f 706f 6c69 7461 6e5f  ox.metropolitan_
-00001400: 6672 616e 6365 5f62 626f 7820 3d20 6765  france_bbox = ge
-00001410: 745f 636f 756e 7472 795f 6262 6f78 2822  t_country_bbox("
-00001420: 4672 616e 6365 2229 5b31 5d0a 0a74 6173  France")[1]..tas
-00001430: 6b20 3d20 5461 736b 2862 6f75 6e64 696e  k = Task(boundin
-00001440: 675f 626f 783d 6d65 7472 6f70 6f6c 6974  g_box=metropolit
-00001450: 616e 5f66 7261 6e63 655f 6262 6f78 2c20  an_france_bbox, 
-00001460: 6e6f 726d 616c 697a 653d 5472 7565 290a  normalize=True).
-00001470: 0a6d 795f 6461 7461 7365 7420 3d20 4372  .my_dataset = Cr
-00001480: 6f70 4861 7276 6573 7428 6461 7461 5f64  opHarvest(data_d
-00001490: 6972 2c20 7461 736b 290a 0a58 2c20 7920  ir, task)..X, y 
-000014a0: 3d20 6d79 5f64 6174 6173 6574 2e61 735f  = my_dataset.as_
-000014b0: 6172 7261 7928 666c 6174 7465 6e5f 783d  array(flatten_x=
-000014c0: 5472 7565 290a 6d6f 6465 6c20 3d20 5261  True).model = Ra
-000014d0: 6e64 6f6d 466f 7265 7374 436c 6173 7369  ndomForestClassi
-000014e0: 6669 6572 2872 616e 646f 6d5f 7374 6174  fier(random_stat
-000014f0: 653d 3029 0a6d 6f64 656c 2e66 6974 2858  e=0).model.fit(X
-00001500: 2c20 7929 0a60 6060 0a3c 2f64 6574 6169  , y).```.</detai
-00001510: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a3c  ls>..<details>.<
-00001520: 7375 6d6d 6172 793e 3c61 2068 7265 663d  summary><a href=
-00001530: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001540: 6f6d 2f6e 6173 6168 6172 7665 7374 2f63  om/nasaharvest/c
-00001550: 726f 7068 6172 7665 7374 2f69 7373 7565  ropharvest/issue
-00001560: 732f 3130 363e 486f 7720 646f 2049 206c  s/106>How do I l
-00001570: 6f61 6420 6120 7370 6563 6966 6963 2070  oad a specific p
-00001580: 6978 656c 2074 696d 6573 6572 6965 733f  ixel timeseries?
-00001590: 3c2f 613e 3c2f 7375 6d6d 6172 793e 0a0a  </a></summary>..
-000015a0: 5468 6520 3c61 2068 7265 663d 6874 7470  The <a href=http
-000015b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
-000015c0: 6173 6168 6172 7665 7374 2f63 726f 7068  asaharvest/croph
-000015d0: 6172 7665 7374 2f69 7373 7565 732f 3130  arvest/issues/10
-000015e0: 363e 7370 6563 6966 6963 2075 7365 2063  6>specific use c
-000015f0: 6173 653c 2f61 3e20 6865 7265 2069 7320  ase</a> here is 
-00001600: 746f 2072 6574 7269 6576 6520 4e44 5649  to retrieve NDVI
-00001610: 2076 616c 7565 7320 666f 7220 6120 7370   values for a sp
-00001620: 6563 6966 6963 2072 6f77 2069 6e20 7468  ecific row in th
-00001630: 6520 606c 6162 656c 732e 6765 6f6a 736f  e `labels.geojso
-00001640: 6e60 2e20 4865 7265 2069 7320 686f 7720  n`. Here is how 
-00001650: 796f 7520 6d69 6768 7420 676f 2061 626f  you might go abo
-00001660: 7574 2064 6f69 6e67 2074 6861 743a 0a0a  ut doing that:..
-00001670: 4669 7273 746c 792c 2049 2077 696c 6c20  Firstly, I will 
-00001680: 6c6f 6164 2074 6865 2067 656f 736a 6f6e  load the geosjon
-00001690: 2e20 4927 6c6c 2064 6f20 6974 2074 6872  . I'll do it thr
-000016a0: 6f75 6768 2061 2060 4372 6f70 4861 7276  ough a `CropHarv
-000016b0: 6573 744c 6162 656c 7360 206f 626a 6563  estLabels` objec
-000016c0: 742c 2077 6869 6368 2069 7320 6a75 7374  t, which is just
-000016d0: 2061 2077 7261 7070 6572 2061 726f 756e   a wrapper aroun
-000016e0: 6420 7468 6520 6765 6f6a 736f 6e20 6275  d the geojson bu
-000016f0: 7420 7072 6f76 6964 6573 2073 6f6d 6520  t provides some 
-00001700: 6e69 6365 2075 7469 6c69 7479 2066 756e  nice utility fun
-00001710: 6374 696f 6e73 2e0a 6060 6070 7974 686f  ctions..```pytho
-00001720: 6e0a 3e3e 3e20 6672 6f6d 2063 726f 7068  n.>>> from croph
-00001730: 6172 7665 7374 2e64 6174 6173 6574 7320  arvest.datasets 
-00001740: 696d 706f 7274 2043 726f 7048 6172 7665  import CropHarve
-00001750: 7374 4c61 6265 6c73 0a3e 3e3e 0a3e 3e3e  stLabels.>>>.>>>
-00001760: 206c 6162 656c 7320 3d20 4372 6f70 4861   labels = CropHa
-00001770: 7276 6573 744c 6162 656c 7328 2263 726f  rvestLabels("cro
-00001780: 7068 6172 7665 7374 2f64 6174 6122 290a  pharvest/data").
-00001790: 3e3e 3e20 6c61 6265 6c73 5f67 656f 6a73  >>> labels_geojs
-000017a0: 6f6e 203d 206c 6162 656c 732e 6173 5f67  on = labels.as_g
-000017b0: 656f 6a73 6f6e 2829 0a3e 3e3e 206c 6162  eojson().>>> lab
-000017c0: 656c 735f 6765 6f6a 736f 6e2e 6865 6164  els_geojson.head
-000017d0: 2829 0a20 2068 6172 7665 7374 5f64 6174  ().  harvest_dat
-000017e0: 6520 706c 616e 7469 6e67 5f64 6174 6520  e planting_date 
-000017f0: 202e 2e2e 2069 735f 7465 7374 2020 2020   ... is_test    
-00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001820: 2020 2020 2020 2067 656f 6d65 7472 790a         geometry.
-00001830: 3020 2020 2020 2020 2020 4e6f 6e65 2020  0         None  
-00001840: 2020 2020 2020 2020 4e6f 6e65 2020 2e2e          None  ..
-00001850: 2e20 2020 4661 6c73 6520 2050 4f4c 5947  .   False  POLYG
-00001860: 4f4e 2028 2833 372e 3038 3235 3220 3130  ON ((37.08252 10
-00001870: 2e37 3132 3734 2c20 3337 2e30 3833 3438  .71274, 37.08348
-00001880: 2031 302e 3731 3239 312e 2e2e 0a31 2020   10.71291....1  
-00001890: 2020 2020 2020 204e 6f6e 6520 2020 2020         None     
-000018a0: 2020 2020 204e 6f6e 6520 202e 2e2e 2020       None  ...  
-000018b0: 2046 616c 7365 2020 504f 4c59 474f 4e20   False  POLYGON 
-000018c0: 2828 3337 2e30 3837 3231 2031 302e 3732  ((37.08721 10.72
-000018d0: 3339 382c 2033 372e 3038 3731 3420 3130  398, 37.08714 10
-000018e0: 2e37 3234 3239 2e2e 2e0a 3220 2020 2020  .72429....2     
-000018f0: 2020 2020 4e6f 6e65 2020 2020 2020 2020      None        
-00001900: 2020 4e6f 6e65 2020 2e2e 2e20 2020 4661    None  ...   Fa
-00001910: 6c73 6520 2050 4f4c 5947 4f4e 2028 2833  lse  POLYGON ((3
-00001920: 372e 3038 3439 3820 3130 2e37 3133 3731  7.08498 10.71371
-00001930: 2c20 3337 2e30 3834 3831 2031 302e 3731  , 37.08481 10.71
-00001940: 3339 332e 2e2e 0a33 2020 2020 2020 2020  393....3        
-00001950: 204e 6f6e 6520 2020 2020 2020 2020 204e   None          N
-00001960: 6f6e 6520 202e 2e2e 2020 2046 616c 7365  one  ...   False
-00001970: 2020 504f 4c59 474f 4e20 2828 3337 2e30    POLYGON ((37.0
-00001980: 3930 3231 2031 302e 3731 3332 302c 2033  9021 10.71320, 3
-00001990: 372e 3039 3031 3420 3130 2e37 3133 3431  7.09014 10.71341
-000019a0: 2e2e 2e0a 3420 2020 2020 2020 2020 4e6f  ....4         No
-000019b0: 6e65 2020 2020 2020 2020 2020 4e6f 6e65  ne          None
-000019c0: 2020 2e2e 2e20 2020 4661 6c73 6520 2050    ...   False  P
-000019d0: 4f4c 5947 4f4e 2028 2833 372e 3038 3330  OLYGON ((37.0830
-000019e0: 3720 3130 2e37 3231 3630 2c20 3337 2e30  7 10.72160, 37.0
-000019f0: 3832 3831 2031 302e 3732 3139 372e 2e2e  8281 10.72197...
-00001a00: 0a0a 5b35 2072 6f77 7320 7820 3133 2063  ..[5 rows x 13 c
-00001a10: 6f6c 756d 6e73 5d0a 6060 600a 0a4e 6f77  olumns].```..Now
-00001a20: 2c20 4920 6361 6e20 7573 6520 7468 6520  , I can use the 
-00001a30: 606c 6162 656c 7360 206f 626a 6563 7420  `labels` object 
-00001a40: 746f 2072 6574 7269 6576 6520 7468 6520  to retrieve the 
-00001a50: 6669 6c65 7061 7468 206f 6620 7468 6520  filepath of the 
-00001a60: 7072 6f63 6573 7365 6420 7361 7465 6c6c  processed satell
-00001a70: 6974 6520 6461 7461 2066 6f72 2065 6163  ite data for eac
-00001a80: 6820 726f 7720 696e 2074 6865 206c 6162  h row in the lab
-00001a90: 656c 7320 6765 6f6a 736f 6e3a 0a60 6060  els geojson:.```
-00001aa0: 7079 7468 6f6e 0a3e 3e3e 2070 6174 685f  python.>>> path_
-00001ab0: 746f 5f66 696c 6520 3d20 6c61 6265 6c73  to_file = labels
-00001ac0: 2e5f 7061 7468 5f66 726f 6d5f 726f 7728  ._path_from_row(
-00001ad0: 6c61 6265 6c73 5f67 656f 6a73 6f6e 2e69  labels_geojson.i
-00001ae0: 6c6f 635b 305d 290a 6060 600a 5468 6973  loc[0]).```.This
-00001af0: 2070 726f 6365 7373 6564 2073 6174 656c   processed satel
-00001b00: 6c69 7465 2064 6174 6120 6973 2073 746f  lite data is sto
-00001b10: 7265 6420 6173 2060 6835 7079 6020 6669  red as `h5py` fi
-00001b20: 6c65 732c 2073 6f20 4920 6361 6e20 6c6f  les, so I can lo
-00001b30: 6164 2069 7420 7570 2061 7320 666f 6c6c  ad it up as foll
-00001b40: 6f77 733a 0a60 6060 7079 7468 6f6e 0a3e  ows:.```python.>
-00001b50: 3e3e 2069 6d70 6f72 7420 6835 7079 0a3e  >> import h5py.>
-00001b60: 3e3e 2068 3570 795f 6669 6c65 203d 2068  >> h5py_file = h
-00001b70: 3570 792e 4669 6c65 2870 6174 685f 746f  5py.File(path_to
-00001b80: 5f66 696c 652c 2022 7222 290a 3e3e 3e20  _file, "r").>>> 
-00001b90: 7820 3d20 6835 7079 5f66 696c 652e 6765  x = h5py_file.ge
-00001ba0: 7428 2261 7272 6179 2229 5b3a 5d0a 3e3e  t("array")[:].>>
-00001bb0: 3e20 782e 7368 6170 650a 2831 322c 2031  > x.shape.(12, 1
-00001bc0: 3829 0a60 6060 0a54 6865 2073 6861 7065  8).```.The shape
-00001bd0: 206f 6620 6078 6020 7265 7072 6573 656e   of `x` represen
-00001be0: 7473 2031 3220 7469 6d65 7374 6570 7320  ts 12 timesteps 
-00001bf0: 616e 6420 3138 2062 616e 6473 2e20 546f  and 18 bands. To
-00001c00: 2072 6574 7269 6576 6520 7468 6520 6261   retrieve the ba
-00001c10: 6e64 2049 2061 6d20 696e 7465 7265 7374  nd I am interest
-00001c20: 6564 2069 6e3a 0a60 6060 7079 7468 6f6e  ed in:.```python
-00001c30: 0a3e 3e3e 2066 726f 6d20 6372 6f70 6861  .>>> from cropha
-00001c40: 7276 6573 742e 6261 6e64 7320 696d 706f  rvest.bands impo
-00001c50: 7274 2042 414e 4453 0a3e 3e3e 2078 5b3a  rt BANDS.>>> x[:
-00001c60: 2c20 4241 4e44 532e 696e 6465 7828 224e  , BANDS.index("N
-00001c70: 4456 4922 295d 0a61 7272 6179 285b 302e  DVI")].array([0.
-00001c80: 3238 3939 3230 3732 2c20 302e 3238 3833  28992072, 0.2883
-00001c90: 3833 3433 2c20 302e 3236 3833 3335 3739  8343, 0.26833579
-00001ca0: 2c20 302e 3232 3537 3736 3333 2c20 302e  , 0.22577633, 0.
-00001cb0: 3237 3133 3839 3836 2c0a 2020 2020 2020  27138986,.      
-00001cc0: 2030 2e30 3635 3834 3131 342c 2030 2e34   0.06584114, 0.4
-00001cd0: 3938 3939 3820 202c 2030 2e35 3031 3437  98998  , 0.50147
-00001ce0: 3230 332c 2030 2e35 3034 3337 3734 332c  203, 0.50437743,
-00001cf0: 2030 2e34 3433 3236 3334 332c 0a20 2020   0.44326343,.   
-00001d00: 2020 2020 302e 3333 3733 3538 3439 2c20      0.33735849, 
-00001d10: 302e 3238 3337 3539 3637 5d29 0a60 6060  0.28375967]).```
-00001d20: 0a54 6865 7365 2061 7265 2031 3220 4e44  .These are 12 ND
-00001d30: 5649 2076 616c 7565 732c 2063 6f72 7265  VI values, corre
-00001d40: 7370 6f6e 6469 6e67 2074 6f20 7468 6520  sponding to the 
-00001d50: 3132 206d 6f6e 7468 7320 6361 7074 7572  12 months captur
-00001d60: 6564 2069 6e20 7468 6973 2074 696d 6573  ed in this times
-00001d70: 6572 6965 732e 2054 6f20 6669 6e64 206f  eries. To find o
-00001d80: 7574 2065 7861 6374 6c79 2077 6869 6368  ut exactly which
-00001d90: 206d 6f6e 7468 2065 6163 6820 7469 6d65   month each time
-00001da0: 7374 6570 2072 6570 7265 7365 6e74 732c  step represents,
-00001db0: 2049 2063 616e 2064 6f0a 6060 6070 7974   I can do.```pyt
-00001dc0: 686f 6e0a 3e3e 3e20 6c61 6265 6c73 5f67  hon.>>> labels_g
-00001dd0: 656f 6a73 6f6e 2e69 6c6f 635b 305d 2e65  eojson.iloc[0].e
-00001de0: 7870 6f72 745f 656e 645f 6461 7465 0a27  xport_end_date.'
-00001df0: 3230 3231 2d30 322d 3031 5430 303a 3030  2021-02-01T00:00
-00001e00: 3a30 3027 0a60 6060 0a57 6963 6820 7465  :00'.```.Wich te
-00001e10: 6c6c 7320 6d65 2074 6861 7420 7468 6520  lls me that the 
-00001e20: 6c61 7374 2074 696d 6573 7465 7020 7265  last timestep re
-00001e30: 7072 6573 656e 7473 204a 616e 7561 7279  presents January
-00001e40: 2032 3032 312e 2049 2063 616e 2077 6f72   2021. I can wor
-00001e50: 6b20 6261 636b 7761 7264 7320 6672 6f6d  k backwards from
-00001e60: 2074 6865 7265 2e0a 0a3c 2f64 6574 6169   there...</detai
-00001e70: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a3c  ls>..<details>.<
-00001e80: 7375 6d6d 6172 793e 3c61 2068 7265 663d  summary><a href=
-00001e90: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00001ea0: 636f 6d2f 6e61 7361 6861 7276 6573 742f  com/nasaharvest/
-00001eb0: 6372 6f70 6861 7276 6573 742f 6973 7375  cropharvest/issu
-00001ec0: 6573 2f38 3822 3e57 6861 7420 6973 2074  es/88">What is t
-00001ed0: 6865 2064 6174 6120 666f 726d 6174 3f3c  he data format?<
-00001ee0: 2f61 3e3c 2f73 756d 6d61 7279 3e0a 5468  /a></summary>.Th
-00001ef0: 6520 7374 7275 6374 7572 6520 6f66 2074  e structure of t
-00001f00: 6865 2064 6966 6665 7265 6e74 2064 6174  he different dat
-00001f10: 6120 6669 6c65 7320 6973 206e 6f77 2064  a files is now d
-00001f20: 6573 6372 6962 6564 2069 6e20 6465 7074  escribed in dept
-00001f30: 6820 696e 2074 6865 2064 6174 6120 666f  h in the data fo
-00001f40: 6c64 6572 2773 205b 5265 6164 6d65 5d28  lder's [Readme](
-00001f50: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001f60: 6f6d 2f6e 6173 6168 6172 7665 7374 2f63  om/nasaharvest/c
-00001f70: 726f 7068 6172 7665 7374 2f62 6c6f 622f  ropharvest/blob/
-00001f80: 6d61 696e 2f64 6174 612f 5245 4144 4d45  main/data/README
-00001f90: 2e6d 6429 0a3c 2f64 6574 6169 6c73 3e0a  .md).</details>.
-00001fa0: 0a23 2323 204c 6963 656e 7365 0a43 726f  .### License.Cro
-00001fb0: 7048 6172 7665 7374 2068 6173 2061 205b  pHarvest has a [
-00001fc0: 4372 6561 7469 7665 2043 6f6d 6d6f 6e73  Creative Commons
-00001fd0: 2041 7474 7269 6275 7469 6f6e 2d53 6861   Attribution-Sha
-00001fe0: 7265 416c 696b 6520 342e 3020 496e 7465  reAlike 4.0 Inte
-00001ff0: 726e 6174 696f 6e61 6c5d 2868 7474 7073  rnational](https
-00002000: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e61  ://github.com/na
-00002010: 7361 6861 7276 6573 742f 6372 6f70 6861  saharvest/cropha
-00002020: 7276 6573 742f 626c 6f62 2f6d 6169 6e2f  rvest/blob/main/
-00002030: 4c49 4345 4e53 452e 7478 7429 206c 6963  LICENSE.txt) lic
-00002040: 656e 7365 2e0a 0a23 2323 2043 6974 6174  ense...### Citat
-00002050: 696f 6e0a 0a49 6620 796f 7520 7573 6520  ion..If you use 
-00002060: 4372 6f70 4861 7276 6573 7420 696e 2079  CropHarvest in y
-00002070: 6f75 7220 7265 7365 6172 6368 2c20 706c  our research, pl
-00002080: 6561 7365 2075 7365 2074 6865 2066 6f6c  ease use the fol
-00002090: 6c6f 7769 6e67 2063 6974 6174 696f 6e3a  lowing citation:
-000020a0: 0a60 6060 0a40 696e 7072 6f63 6565 6469  .```.@inproceedi
-000020b0: 6e67 737b 0a20 2020 2074 7365 6e67 3230  ngs{.    tseng20
-000020c0: 3231 6372 6f70 6861 7276 6573 742c 0a20  21cropharvest,. 
-000020d0: 2020 2074 6974 6c65 3d7b 4372 6f70 4861     title={CropHa
-000020e0: 7276 6573 743a 2041 2067 6c6f 6261 6c20  rvest: A global 
-000020f0: 6461 7461 7365 7420 666f 7220 6372 6f70  dataset for crop
-00002100: 2d74 7970 6520 636c 6173 7369 6669 6361  -type classifica
-00002110: 7469 6f6e 7d2c 0a20 2020 2061 7574 686f  tion},.    autho
-00002120: 723d 7b47 6162 7269 656c 2054 7365 6e67  r={Gabriel Tseng
-00002130: 2061 6e64 2049 7661 6e20 5a76 6f6e 6b6f   and Ivan Zvonko
-00002140: 7620 616e 6420 4361 7468 6572 696e 6520  v and Catherine 
-00002150: 4c69 6c69 616e 204e 616b 616c 656d 6265  Lilian Nakalembe
-00002160: 2061 6e64 2048 616e 6e61 6820 4b65 726e   and Hannah Kern
-00002170: 6572 7d2c 0a20 2020 2062 6f6f 6b74 6974  er},.    booktit
-00002180: 6c65 3d7b 5468 6972 7479 2d66 6966 7468  le={Thirty-fifth
-00002190: 2043 6f6e 6665 7265 6e63 6520 6f6e 204e   Conference on N
-000021a0: 6575 7261 6c20 496e 666f 726d 6174 696f  eural Informatio
-000021b0: 6e20 5072 6f63 6573 7369 6e67 2053 7973  n Processing Sys
-000021c0: 7465 6d73 2044 6174 6173 6574 7320 616e  tems Datasets an
-000021d0: 6420 4265 6e63 686d 6172 6b73 2054 7261  d Benchmarks Tra
-000021e0: 636b 2028 526f 756e 6420 3229 7d2c 0a20  ck (Round 2)},. 
-000021f0: 2020 2079 6561 723d 7b32 3032 317d 2c0a     year={2021},.
-00002200: 2020 2020 7572 6c3d 7b68 7474 7073 3a2f      url={https:/
-00002210: 2f6f 7065 6e72 6576 6965 772e 6e65 742f  /openreview.net/
-00002220: 666f 7275 6d3f 6964 3d4a 746a 7a55 5850  forum?id=JtjzUXP
-00002230: 4561 4375 7d0a 7d0a 6060 600a            EaCu}.}.```.
+000001c0: 653a 204c 4943 454e 5345 2e74 7874 0a52  e: LICENSE.txt.R
+000001d0: 6571 7569 7265 732d 4469 7374 3a20 7061  equires-Dist: pa
+000001e0: 6e64 6173 3c32 2e30 2e30 0a52 6571 7569  ndas<2.0.0.Requi
+000001f0: 7265 732d 4469 7374 3a20 6765 6f70 616e  res-Dist: geopan
+00000200: 6461 733d 3d30 2e39 2e30 0a52 6571 7569  das==0.9.0.Requi
+00000210: 7265 732d 4469 7374 3a20 7861 7272 6179  res-Dist: xarray
+00000220: 3c30 2e32 302e 302c 3e3d 302e 3136 2e32  <0.20.0,>=0.16.2
+00000230: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000240: 7471 646d 3e3d 342e 3631 2e31 0a52 6571  tqdm>=4.61.1.Req
+00000250: 7569 7265 732d 4469 7374 3a20 6835 7079  uires-Dist: h5py
+00000260: 213d 332e 372e 302c 3e3d 332e 312e 300a  !=3.7.0,>=3.1.0.
+00000270: 5265 7175 6972 6573 2d44 6973 743a 2072  Requires-Dist: r
+00000280: 6173 7465 7269 6f3e 3d31 2e32 2e36 0a52  asterio>=1.2.6.R
+00000290: 6571 7569 7265 732d 4469 7374 3a20 6f70  equires-Dist: op
+000002a0: 656e 7079 786c 3e3d 322e 352e 390a 5265  enpyxl>=2.5.9.Re
+000002b0: 7175 6972 6573 2d44 6973 743a 2073 6369  quires-Dist: sci
+000002c0: 6b69 742d 6c65 6172 6e3e 3d30 2e32 322e  kit-learn>=0.22.
+000002d0: 320a 0a23 2043 726f 7048 6172 7665 7374  2..# CropHarvest
+000002e0: 0a0a 4372 6f70 4861 7276 6573 7420 6973  ..CropHarvest is
+000002f0: 2061 6e20 6f70 656e 2073 6f75 7263 6520   an open source 
+00000300: 7265 6d6f 7465 2073 656e 7369 6e67 2064  remote sensing d
+00000310: 6174 6173 6574 2066 6f72 2061 6772 6963  ataset for agric
+00000320: 756c 7475 7265 2077 6974 6820 6265 6e63  ulture with benc
+00000330: 686d 6172 6b73 2e20 4974 2063 6f6c 6c65  hmarks. It colle
+00000340: 6374 7320 6461 7461 2066 726f 6d20 6120  cts data from a 
+00000350: 7661 7269 6574 7920 6f66 2061 6772 6963  variety of agric
+00000360: 756c 7475 7261 6c20 6c61 6e64 2075 7365  ultural land use
+00000370: 2064 6174 6173 6574 7320 616e 6420 7265   datasets and re
+00000380: 6d6f 7465 2073 656e 7369 6e67 2070 726f  mote sensing pro
+00000390: 6475 6374 732e 0a0a 0a54 6865 2064 6174  ducts....The dat
+000003a0: 6173 6574 2063 6f6e 7369 7374 7320 6f66  aset consists of
+000003b0: 202a 2a39 352c 3138 362a 2a20 6461 7461   **95,186** data
+000003c0: 706f 696e 7473 2c20 6f66 2077 6869 6368  points, of which
+000003d0: 202a 2a33 332c 3230 352a 2a20 2833 3525   **33,205** (35%
+000003e0: 2920 6861 7665 206d 756c 7469 636c 6173  ) have multiclas
+000003f0: 7320 6c61 6265 6c73 2e20 416c 6c20 6f74  s labels. All ot
+00000400: 6865 7220 6461 7461 706f 696e 7473 206f  her datapoints o
+00000410: 6e6c 7920 6861 7665 2062 696e 6172 7920  nly have binary 
+00000420: 6372 6f70 202f 206e 6f6e 2d63 726f 7020  crop / non-crop 
+00000430: 6c61 6265 6c73 2e0a 0a2a 2a37 302c 3231  labels...**70,21
+00000440: 332a 2a20 2837 3425 2920 6f66 2074 6865  3** (74%) of the
+00000450: 7365 206c 6162 656c 7320 6172 6520 7061  se labels are pa
+00000460: 6972 6564 2077 6974 6820 7265 6d6f 7465  ired with remote
+00000470: 2073 656e 7369 6e67 2061 6e64 2063 6c69   sensing and cli
+00000480: 6d61 746f 6c6f 6779 2064 6174 612c 2073  matology data, s
+00000490: 7065 6369 6669 6361 6c6c 7920 5b53 656e  pecifically [Sen
+000004a0: 7469 6e65 6c2d 325d 2868 7474 7073 3a2f  tinel-2](https:/
+000004b0: 2f73 656e 7469 6e65 6c2e 6573 612e 696e  /sentinel.esa.in
+000004c0: 742f 7765 622f 7365 6e74 696e 656c 2f6d  t/web/sentinel/m
+000004d0: 6973 7369 6f6e 732f 7365 6e74 696e 656c  issions/sentinel
+000004e0: 2d32 292c 205b 5365 6e74 696e 656c 2d31  -2), [Sentinel-1
+000004f0: 5d28 6874 7470 733a 2f2f 7365 6e74 696e  ](https://sentin
+00000500: 656c 2e65 7361 2e69 6e74 2f77 6562 2f73  el.esa.int/web/s
+00000510: 656e 7469 6e65 6c2f 6d69 7373 696f 6e73  entinel/missions
+00000520: 2f73 656e 7469 6e65 6c2d 312f 292c 2074  /sentinel-1/), t
+00000530: 6865 205b 5352 544d 2044 6967 6974 616c  he [SRTM Digital
+00000540: 2045 6c65 7661 7469 6f6e 204d 6f64 656c   Elevation Model
+00000550: 5d28 6874 7470 733a 2f2f 6367 6961 7263  ](https://cgiarc
+00000560: 7369 2e63 6f6d 6d75 6e69 7479 2f64 6174  si.community/dat
+00000570: 612f 7372 746d 2d39 306d 2d64 6967 6974  a/srtm-90m-digit
+00000580: 616c 2d65 6c65 7661 7469 6f6e 2d64 6174  al-elevation-dat
+00000590: 6162 6173 652d 7634 2d31 2f29 2061 6e64  abase-v4-1/) and
+000005a0: 205b 4552 4120 3520 636c 696d 6174 6f6c   [ERA 5 climatol
+000005b0: 6f67 7920 6461 7461 5d28 6874 7470 733a  ogy data](https:
+000005c0: 2f2f 7777 772e 6563 6d77 662e 696e 742f  //www.ecmwf.int/
+000005d0: 656e 2f66 6f72 6563 6173 7473 2f64 6174  en/forecasts/dat
+000005e0: 6173 6574 732f 7265 616e 616c 7973 6973  asets/reanalysis
+000005f0: 2d64 6174 6173 6574 732f 6572 6135 292e  -datasets/era5).
+00000600: 0a0a 3231 2064 6174 6173 6574 7320 6172  ..21 datasets ar
+00000610: 6520 6167 6772 6567 6174 6564 2069 6e74  e aggregated int
+00000620: 6f20 4372 6f70 4861 7276 6573 7420 2d20  o CropHarvest - 
+00000630: 7468 6573 6520 6172 6520 646f 6375 6d65  these are docume
+00000640: 6e74 6564 205b 6865 7265 5d28 6874 7470  nted [here](http
+00000650: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
+00000660: 6173 6168 6172 7665 7374 2f63 726f 7068  asaharvest/croph
+00000670: 6172 7665 7374 2f62 6c6f 622f 6d61 696e  arvest/blob/main
+00000680: 2f64 6174 6173 6574 732e 6d64 292e 0a0a  /datasets.md)...
+00000690: 4d6f 7265 2064 6574 6169 6c73 2061 626f  More details abo
+000006a0: 7574 2043 726f 7048 6172 7665 7374 2061  ut CropHarvest a
+000006b0: 6e64 2074 6865 2062 656e 6368 6d61 726b  nd the benchmark
+000006c0: 7320 6172 6520 6176 6169 6c61 626c 6520  s are available 
+000006d0: 696e 205b 7468 6973 2070 6170 6572 5d28  in [this paper](
+000006e0: 6874 7470 733a 2f2f 6f70 656e 7265 7669  https://openrevi
+000006f0: 6577 2e6e 6574 2f66 6f72 756d 3f69 643d  ew.net/forum?id=
+00000700: 4a74 6a7a 5558 5045 6143 7529 2e0a 0a23  JtjzUXPEaCu)...#
+00000710: 2323 2050 6970 656c 696e 650a 5468 6520  ## Pipeline.The 
+00000720: 636f 6465 2069 6e20 7468 6973 2072 6570  code in this rep
+00000730: 6f73 6974 6f72 790a 0a31 2920 636f 6d62  ository..1) comb
+00000740: 696e 6573 2074 6865 2063 6f6e 7374 6974  ines the constit
+00000750: 7565 6e74 2064 6174 6173 6574 7320 696e  uent datasets in
+00000760: 746f 2061 2073 696e 676c 6520 6765 6f4a  to a single geoJ
+00000770: 534f 4e20 6669 6c65 2c0a 3229 2065 7870  SON file,.2) exp
+00000780: 6f72 7473 2074 6865 2061 7373 6f63 6961  orts the associa
+00000790: 7465 6420 7361 7465 6c6c 6974 6520 6461  ted satellite da
+000007a0: 7461 2066 726f 6d20 4561 7274 6820 456e  ta from Earth En
+000007b0: 6769 6e65 2c0a 3329 2063 6f6d 6269 6e65  gine,.3) combine
+000007c0: 7320 626f 7468 2064 6174 6173 6574 7320  s both datasets 
+000007d0: 746f 2063 7265 6174 6520 6028 582c 7929  to create `(X,y)
+000007e0: 6020 7472 6169 6e69 6e67 2074 7570 6c65  ` training tuple
+000007f0: 7320 616e 640a 3429 2065 7870 6f73 6573  s and.4) exposes
+00000800: 2074 686f 7365 2074 7570 6c65 7320 7669   those tuples vi
+00000810: 6120 6120 6044 6174 6173 6574 6020 6f62  a a `Dataset` ob
+00000820: 6a65 6374 2e0a 0a54 6865 2070 6970 656c  ject...The pipel
+00000830: 696e 6520 7468 726f 7567 6820 7768 6963  ine through whic
+00000840: 6820 7468 6973 2068 6170 7065 6e73 2069  h this happens i
+00000850: 7320 7368 6f77 6e20 6265 6c6f 773a 0a0a  s shown below:..
+00000860: 0a41 6c6c 2062 6c75 6520 626f 7865 7320  .All blue boxes 
+00000870: 6172 6520 6173 736f 6369 6174 6564 2077  are associated w
+00000880: 6974 6820 636f 6465 2069 6e20 7468 6973  ith code in this
+00000890: 2072 6570 6f73 6974 6f72 792e 2041 6e79   repository. Any
+000008a0: 7468 696e 6720 6772 6565 6e20 6973 2064  thing green is d
+000008b0: 6174 6120 6163 6365 7373 6962 6c65 2076  ata accessible v
+000008c0: 6961 205b 5a65 6e6f 646f 5d28 6874 7470  ia [Zenodo](http
+000008d0: 733a 2f2f 7a65 6e6f 646f 2e6f 7267 2f72  s://zenodo.org/r
+000008e0: 6563 6f72 642f 3538 3238 3839 3329 2e20  ecord/5828893). 
+000008f0: 4279 2064 6566 6175 6c74 2c20 7468 6520  By default, the 
+00000900: 5a65 6e6f 646f 2064 6174 6120 7769 6c6c  Zenodo data will
+00000910: 2067 6574 2064 6f77 6e6c 6f61 6465 6420   get downloaded 
+00000920: 746f 2074 6865 205b 6461 7461 2066 6f6c  to the [data fol
+00000930: 6465 725d 2868 7474 7073 3a2f 2f67 6974  der](https://git
+00000940: 6875 622e 636f 6d2f 6e61 7361 6861 7276  hub.com/nasaharv
+00000950: 6573 742f 6372 6f70 6861 7276 6573 742f  est/cropharvest/
+00000960: 7472 6565 2f6d 6169 6e2f 6461 7461 2920  tree/main/data) 
+00000970: 2d20 7468 6520 6461 7461 2066 6f6c 6465  - the data folde
+00000980: 7227 7320 5b52 6561 646d 655d 2868 7474  r's [Readme](htt
+00000990: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000009a0: 6e61 7361 6861 7276 6573 742f 6372 6f70  nasaharvest/crop
+000009b0: 6861 7276 6573 742f 626c 6f62 2f6d 6169  harvest/blob/mai
+000009c0: 6e2f 6461 7461 2f52 4541 444d 452e 6d64  n/data/README.md
+000009d0: 2920 6861 7320 6d6f 7265 2069 6e66 6f72  ) has more infor
+000009e0: 6d61 7469 6f6e 2061 626f 7574 2074 6865  mation about the
+000009f0: 2065 7861 6374 2073 7472 7563 7475 7265   exact structure
+00000a00: 206f 6620 7468 6520 6461 7461 2e0a 0a54   of the data...T
+00000a10: 6865 7265 2061 7265 2075 6e69 7175 6520  here are unique 
+00000a20: 6361 7365 7320 7768 6572 6520 796f 7520  cases where you 
+00000a30: 6d61 7920 6e65 6564 2074 6f20 7573 6520  may need to use 
+00000a40: 7468 6520 6045 6172 7468 456e 6769 6e65  the `EarthEngine
+00000a50: 4578 706f 7274 6572 6020 6469 7265 6374  Exporter` direct
+00000a60: 6c79 2c20 7468 6573 6520 7573 6520 6361  ly, these use ca
+00000a70: 7365 7320 6172 6520 6465 6d6f 6e73 7472  ses are demonstr
+00000a80: 6174 6564 2069 6e20 7468 6520 5b60 6465  ated in the [`de
+00000a90: 6d6f 5f65 7870 6f72 7469 6e67 5f64 6174  mo_exporting_dat
+00000aa0: 612e 6970 796e 6260 5d28 6874 7470 733a  a.ipynb`](https:
+00000ab0: 2f2f 6769 7468 7562 2e63 6f6d 2f6e 6173  //github.com/nas
+00000ac0: 6168 6172 7665 7374 2f63 726f 7068 6172  aharvest/crophar
+00000ad0: 7665 7374 2f62 6c6f 622f 6d61 696e 2f64  vest/blob/main/d
+00000ae0: 656d 6f5f 6578 706f 7274 696e 675f 6461  emo_exporting_da
+00000af0: 7461 2e69 7079 6e62 2920 6e6f 7465 626f  ta.ipynb) notebo
+00000b00: 6f6b 2e0a 0a23 2323 2049 6e73 7461 6c6c  ok...### Install
+00000b10: 6174 696f 6e0a 4c69 6e75 7820 616e 6420  ation.Linux and 
+00000b20: 4d61 634f 5320 7573 6572 7320 6361 6e20  MacOS users can 
+00000b30: 696e 7374 616c 6c20 7468 6520 6c61 7465  install the late
+00000b40: 7374 2076 6572 7369 6f6e 206f 6620 4372  st version of Cr
+00000b50: 6f70 4861 7276 6573 7420 7769 7468 2074  opHarvest with t
+00000b60: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00000b70: 6d61 6e64 3a0a 6060 6062 6173 680a 7069  mand:.```bash.pi
+00000b80: 7020 696e 7374 616c 6c20 6372 6f70 6861  p install cropha
+00000b90: 7276 6573 740a 6060 600a 5769 6e64 6f77  rvest.```.Window
+00000ba0: 7320 7573 6572 7320 6d75 7374 2069 6e73  s users must ins
+00000bb0: 7461 6c6c 2074 6865 2043 726f 7048 6172  tall the CropHar
+00000bc0: 7665 7374 2077 6974 6869 6e20 6120 5b63  vest within a [c
+00000bd0: 6f6e 6461 5d28 6874 7470 733a 2f2f 646f  onda](https://do
+00000be0: 6373 2e63 6f6e 6461 2e69 6f2f 656e 2f6c  cs.conda.io/en/l
+00000bf0: 6174 6573 742f 6d69 6e69 636f 6e64 612e  atest/miniconda.
+00000c00: 6874 6d6c 2920 656e 7669 726f 6e6d 656e  html) environmen
+00000c10: 7420 746f 2065 6e73 7572 6520 616c 6c20  t to ensure all 
+00000c20: 6465 7065 6e64 656e 6369 6573 2061 7265  dependencies are
+00000c30: 2069 6e73 7461 6c6c 6564 2063 6f72 7265   installed corre
+00000c40: 6374 6c79 3a0a 6060 6062 6173 680a 636f  ctly:.```bash.co
+00000c50: 6e64 6120 696e 7374 616c 6c20 2766 696f  nda install 'fio
+00000c60: 6e61 3e3d 312e 3527 2027 7261 7374 6572  na>=1.5' 'raster
+00000c70: 696f 3e3d 312e 322e 3627 0a70 6970 2069  io>=1.2.6'.pip i
+00000c80: 6e73 7461 6c6c 2063 726f 7068 6172 7665  nstall cropharve
+00000c90: 7374 0a60 6060 0a49 6e20 6164 6469 7469  st.```.In additi
+00000ca0: 6f6e 2c20 6974 205b 6d61 7920 6265 206e  on, it [may be n
+00000cb0: 6563 6573 7361 7279 5d28 6874 7470 733a  ecessary](https:
+00000cc0: 2f2f 6769 7468 7562 2e63 6f6d 2f68 3570  //github.com/h5p
+00000cd0: 792f 6835 7079 2f69 7373 7565 732f 3137  y/h5py/issues/17
+00000ce0: 3734 2920 746f 2069 6e73 7461 6c6c 2060  74) to install `
+00000cf0: 6835 7079 6020 7573 696e 6720 636f 6e64  h5py` using cond
+00000d00: 6120 6173 2077 656c 6c20 2860 636f 6e64  a as well (`cond
+00000d10: 6120 696e 7374 616c 6c20 2768 3570 793e  a install 'h5py>
+00000d20: 332e 372e 3027 6029 2070 7269 6f72 2074  3.7.0'`) prior t
+00000d30: 6f20 7069 702d 696e 7374 616c 6c69 6e67  o pip-installing
+00000d40: 2063 726f 7068 6172 7665 7374 2e0a 0a23   cropharvest...#
+00000d50: 2323 2047 6574 7469 6e67 2073 7461 7274  ## Getting start
+00000d60: 6564 205b 215b 4f70 656e 2049 6e20 436f  ed [![Open In Co
+00000d70: 6c61 625d 2868 7474 7073 3a2f 2f63 6f6c  lab](https://col
+00000d80: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
+00000d90: 6c65 2e63 6f6d 2f61 7373 6574 732f 636f  le.com/assets/co
+00000da0: 6c61 622d 6261 6467 652e 7376 6729 5d28  lab-badge.svg)](
+00000db0: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
+00000dc0: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
+00000dd0: 6d2f 6769 7468 7562 2f6e 6173 6168 6172  m/github/nasahar
+00000de0: 7665 7374 2f63 726f 7068 6172 7665 7374  vest/cropharvest
+00000df0: 2f62 6c6f 622f 6d61 696e 2f64 656d 6f2e  /blob/main/demo.
+00000e00: 6970 796e 6229 0a53 6565 2074 6865 205b  ipynb).See the [
+00000e10: 6064 656d 6f2e 6970 796e 6260 5d28 6874  `demo.ipynb`](ht
+00000e20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000e30: 2f6e 6173 6168 6172 7665 7374 2f63 726f  /nasaharvest/cro
+00000e40: 7068 6172 7665 7374 2f62 6c6f 622f 6d61  pharvest/blob/ma
+00000e50: 696e 2f64 656d 6f2e 6970 796e 6229 206e  in/demo.ipynb) n
+00000e60: 6f74 6562 6f6f 6b20 666f 7220 616e 2065  otebook for an e
+00000e70: 7861 6d70 6c65 206f 6e20 686f 7720 746f  xample on how to
+00000e80: 2064 6f77 6e6c 6f61 6420 7468 6520 6461   download the da
+00000e90: 7461 2066 726f 6d20 5b5a 656e 6f64 6f5d  ta from [Zenodo]
+00000ea0: 2868 7474 7073 3a2f 2f7a 656e 6f64 6f2e  (https://zenodo.
+00000eb0: 6f72 672f 7265 636f 7264 2f37 3235 3736  org/record/72576
+00000ec0: 3838 2920 616e 6420 7472 6169 6e20 6120  88) and train a 
+00000ed0: 7261 6e64 6f6d 2066 6f72 6573 7420 6167  random forest ag
+00000ee0: 6169 6e73 7420 7468 6973 2064 6174 612e  ainst this data.
+00000ef0: 0a0a 466f 7220 6d6f 7265 2065 7861 6d70  ..For more examp
+00000f00: 6c65 7320 6f66 206d 6f64 656c 7320 7472  les of models tr
+00000f10: 6169 6e65 6420 6167 6169 6e73 7420 7468  ained against th
+00000f20: 6973 2064 6174 6173 6574 2c20 7365 6520  is dataset, see 
+00000f30: 7468 6520 5b62 656e 6368 6d61 726b 735d  the [benchmarks]
+00000f40: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000f50: 636f 6d2f 6e61 7361 6861 7276 6573 742f  com/nasaharvest/
+00000f60: 6372 6f70 6861 7276 6573 742f 626c 6f62  cropharvest/blob
+00000f70: 2f6d 6169 6e2f 6265 6e63 686d 6172 6b73  /main/benchmarks
+00000f80: 292e 0a0a 2323 2320 436f 6e74 7269 6275  )...### Contribu
+00000f90: 7469 6e67 0a49 6620 796f 7520 776f 756c  ting.If you woul
+00000fa0: 6420 6c69 6b65 2074 6f20 636f 6e74 7269  d like to contri
+00000fb0: 6275 7465 2061 2064 6174 6173 6574 2c20  bute a dataset, 
+00000fc0: 706c 6561 7365 2073 6565 2074 6865 205b  please see the [
+00000fd0: 636f 6e74 7269 6275 7469 6e67 2072 6561  contributing rea
+00000fe0: 646d 655d 2868 7474 7073 3a2f 2f67 6974  dme](https://git
+00000ff0: 6875 622e 636f 6d2f 6e61 7361 6861 7276  hub.com/nasaharv
+00001000: 6573 742f 6372 6f70 6861 7276 6573 742f  est/cropharvest/
+00001010: 626c 6f62 2f6d 6169 6e2f 636f 6e74 7269  blob/main/contri
+00001020: 6275 7469 6e67 2e6d 6429 2e0a 0a23 2323  buting.md)...###
+00001030: 207e 7e46 4151 7e7e 2051 7565 7374 696f   ~~FAQ~~ Questio
+00001040: 6e73 2061 736b 6564 2061 7420 6c65 6173  ns asked at leas
+00001050: 7420 6f6e 6365 0a0a 3c64 6574 6169 6c73  t once..<details
+00001060: 3e0a 3c73 756d 6d61 7279 3e3c 6120 6872  >.<summary><a hr
+00001070: 6566 3d68 7474 7073 3a2f 2f67 6974 6875  ef=https://githu
+00001080: 622e 636f 6d2f 6e61 7361 6861 7276 6573  b.com/nasaharves
+00001090: 742f 6372 6f70 6861 7276 6573 742f 6973  t/cropharvest/is
+000010a0: 7375 6573 2f39 353e 486f 7720 646f 2049  sues/95>How do I
+000010b0: 2075 7365 2043 726f 7048 6172 7665 7374   use CropHarvest
+000010c0: 2066 6f72 2061 2073 7065 6369 6669 6320   for a specific 
+000010d0: 6765 6f67 7261 7068 793f 3c2f 613e 3c2f  geography?</a></
+000010e0: 7375 6d6d 6172 793e 0a0a 416c 6c20 7468  summary>..All th
+000010f0: 6520 6461 7461 2069 7320 6163 6365 7373  e data is access
+00001100: 6962 6c65 2074 6872 6f75 6768 2074 6865  ible through the
+00001110: 2060 6372 6f70 6861 7276 6573 742e 6461   `cropharvest.da
+00001120: 7461 7365 7473 2e43 726f 7048 6172 7665  tasets.CropHarve
+00001130: 7374 6020 6f62 6a65 6374 2e20 5468 6520  st` object. The 
+00001140: 6d61 696e 2070 6172 616d 6574 6572 7320  main parameters 
+00001150: 7768 6963 6820 796f 7520 6d69 6768 7420  which you might 
+00001160: 6265 2069 6e74 6572 6573 7465 6420 696e  be interested in
+00001170: 206d 616e 6970 756c 6174 696e 6720 6172   manipulating ar
+00001180: 6520 636f 6e74 726f 6c6c 6162 6c65 2074  e controllable t
+00001190: 6872 6f75 6768 2061 2060 6372 6f70 6861  hrough a `cropha
+000011a0: 7276 6573 742e 6461 7461 7365 7473 2e54  rvest.datasets.T
+000011b0: 6173 6b60 2c20 7768 6963 6820 7461 6b65  ask`, which take
+000011c0: 7320 6173 2069 6e70 7574 2074 6865 2066  s as input the f
+000011d0: 6f6c 6c6f 7769 6e67 2070 6172 616d 6574  ollowing paramet
+000011e0: 6572 733a 0a2d 2041 2062 6f75 6e64 696e  ers:.- A boundin
+000011f0: 6720 626f 782c 2077 6869 6368 2064 6566  g box, which def
+00001200: 696e 6573 2074 6865 2073 7061 7469 616c  ines the spatial
+00001210: 2062 6f75 6e64 6172 6965 7320 6f66 2074   boundaries of t
+00001220: 6865 206c 6162 656c 7320 7265 7472 6965  he labels retrie
+00001230: 7665 730a 2d20 4120 7461 7267 6574 206c  ves.- A target l
+00001240: 6162 656c 2c20 7768 6963 6820 6465 6669  abel, which defi
+00001250: 6e65 7320 7468 6520 636c 6173 7320 6f66  nes the class of
+00001260: 2074 6865 2070 6f73 6974 6976 6520 6c61   the positive la
+00001270: 6265 6c73 2028 6966 2074 6869 7320 6973  bels (if this is
+00001280: 206c 6566 7420 746f 2060 4e6f 6e65 602c   left to `None`,
+00001290: 2074 6865 6e20 7468 6520 706f 7369 7469   then the positi
+000012a0: 7665 2063 6c61 7373 2077 696c 6c20 6265  ve class will be
+000012b0: 2063 726f 7073 2061 6e64 2074 6865 206e   crops and the n
+000012c0: 6567 6174 6976 6520 636c 6173 7320 7769  egative class wi
+000012d0: 6c6c 2062 6520 6e6f 6e2d 6372 6f70 7329  ll be non-crops)
+000012e0: 0a2d 2041 2062 6f6f 6c65 616e 2064 6566  .- A boolean def
+000012f0: 696e 696e 6720 7768 6574 6865 7220 6f72  ining whether or
+00001300: 206e 6f74 2074 6f20 6261 6c61 6e63 6520   not to balance 
+00001310: 7468 6520 6372 6f70 7320 616e 6420 6e6f  the crops and no
+00001320: 6e2d 6372 6f70 7320 696e 2074 6865 206e  n-crops in the n
+00001330: 6567 6174 6976 6520 636c 6173 730a 2d20  egative class.- 
+00001340: 4120 7465 7374 5f69 6465 6e74 6966 6965  A test_identifie
+00001350: 7220 7374 7269 6e67 2c20 7768 6963 6820  r string, which 
+00001360: 7465 6c6c 7320 7468 6520 6461 7461 7365  tells the datase
+00001370: 7420 7768 6574 6865 7220 6f72 206e 6f74  t whether or not
+00001380: 2074 6f20 7265 7472 6965 7665 2061 2066   to retrieve a f
+00001390: 696c 6520 6672 6f6d 2074 6865 2060 7465  ile from the `te
+000013a0: 7374 5f66 6561 7475 7265 7360 2066 6f6c  st_features` fol
+000013b0: 6465 7220 616e 6420 7265 7475 726e 2069  der and return i
+000013c0: 7420 6173 2074 6865 2074 6573 7420 6461  t as the test da
+000013d0: 7461 2e0a 0a53 6f20 6966 2049 2077 616e  ta...So if I wan
+000013e0: 7465 6420 746f 2075 7365 2074 6869 7320  ted to use this 
+000013f0: 746f 2074 7261 696e 2061 206d 6f64 656c  to train a model
+00001400: 2074 6f20 6964 656e 7469 6679 2063 726f   to identify cro
+00001410: 7020 7673 2e20 6e6f 6e20 6372 6f70 2069  p vs. non crop i
+00001420: 6e20 4672 616e 6365 2c20 4920 6d69 6768  n France, I migh
+00001430: 7420 646f 2069 7420 6c69 6b65 2074 6869  t do it like thi
+00001440: 733a 0a0a 6060 6070 7974 686f 6e0a 6672  s:..```python.fr
+00001450: 6f6d 2073 6b6c 6561 726e 2e65 6e73 656d  om sklearn.ensem
+00001460: 626c 6520 696d 706f 7274 2052 616e 646f  ble import Rando
+00001470: 6d46 6f72 6573 7443 6c61 7373 6966 6965  mForestClassifie
+00001480: 720a 0a66 726f 6d20 6372 6f70 6861 7276  r..from cropharv
+00001490: 6573 742e 6461 7461 7365 7473 2069 6d70  est.datasets imp
+000014a0: 6f72 7420 5461 736b 2c20 4372 6f70 4861  ort Task, CropHa
+000014b0: 7276 6573 740a 6672 6f6d 2063 726f 7068  rvest.from croph
+000014c0: 6172 7665 7374 2e63 6f75 6e74 7269 6573  arvest.countries
+000014d0: 2069 6d70 6f72 7420 6765 745f 636f 756e   import get_coun
+000014e0: 7472 795f 6262 6f78 0a0a 2320 666f 6c64  try_bbox..# fold
+000014f0: 6572 2069 6e74 6f20 7768 6963 6820 7468  er into which th
+00001500: 6520 6461 7461 2077 696c 6c20 6265 2064  e data will be d
+00001510: 6f77 6e6c 6f61 6465 6420 2f20 616c 7265  ownloaded / alre
+00001520: 6164 7920 6578 6973 7473 0a64 6174 615f  ady exists.data_
+00001530: 6469 7220 3d20 2264 6174 6122 0a0a 2320  dir = "data"..# 
+00001540: 6765 745f 636f 756e 7472 795f 6262 6f78  get_country_bbox
+00001550: 2072 6574 7572 6e73 2061 206c 6973 7420   returns a list 
+00001560: 6f66 2062 6f75 6e64 696e 6720 626f 7865  of bounding boxe
+00001570: 732e 0a23 2074 6865 206f 6e65 2072 6570  s..# the one rep
+00001580: 7265 7365 6e74 696e 6720 4d65 7472 6f70  resenting Metrop
+00001590: 6f6c 6974 616e 2046 7261 6e63 6520 6973  olitan France is
+000015a0: 2074 6865 2032 6e64 2062 6f78 0a6d 6574   the 2nd box.met
+000015b0: 726f 706f 6c69 7461 6e5f 6672 616e 6365  ropolitan_france
+000015c0: 5f62 626f 7820 3d20 6765 745f 636f 756e  _bbox = get_coun
+000015d0: 7472 795f 6262 6f78 2822 4672 616e 6365  try_bbox("France
+000015e0: 2229 5b31 5d0a 0a74 6173 6b20 3d20 5461  ")[1]..task = Ta
+000015f0: 736b 2862 6f75 6e64 696e 675f 626f 783d  sk(bounding_box=
+00001600: 6d65 7472 6f70 6f6c 6974 616e 5f66 7261  metropolitan_fra
+00001610: 6e63 655f 6262 6f78 2c20 6e6f 726d 616c  nce_bbox, normal
+00001620: 697a 653d 5472 7565 290a 0a6d 795f 6461  ize=True)..my_da
+00001630: 7461 7365 7420 3d20 4372 6f70 4861 7276  taset = CropHarv
+00001640: 6573 7428 6461 7461 5f64 6972 2c20 7461  est(data_dir, ta
+00001650: 736b 290a 0a58 2c20 7920 3d20 6d79 5f64  sk)..X, y = my_d
+00001660: 6174 6173 6574 2e61 735f 6172 7261 7928  ataset.as_array(
+00001670: 666c 6174 7465 6e5f 783d 5472 7565 290a  flatten_x=True).
+00001680: 6d6f 6465 6c20 3d20 5261 6e64 6f6d 466f  model = RandomFo
+00001690: 7265 7374 436c 6173 7369 6669 6572 2872  restClassifier(r
+000016a0: 616e 646f 6d5f 7374 6174 653d 3029 0a6d  andom_state=0).m
+000016b0: 6f64 656c 2e66 6974 2858 2c20 7929 0a60  odel.fit(X, y).`
+000016c0: 6060 0a3c 2f64 6574 6169 6c73 3e0a 0a3c  ``.</details>..<
+000016d0: 6465 7461 696c 733e 0a3c 7375 6d6d 6172  details>.<summar
+000016e0: 793e 3c61 2068 7265 663d 6874 7470 733a  y><a href=https:
+000016f0: 2f2f 6769 7468 7562 2e63 6f6d 2f6e 6173  //github.com/nas
+00001700: 6168 6172 7665 7374 2f63 726f 7068 6172  aharvest/crophar
+00001710: 7665 7374 2f69 7373 7565 732f 3130 363e  vest/issues/106>
+00001720: 486f 7720 646f 2049 206c 6f61 6420 6120  How do I load a 
+00001730: 7370 6563 6966 6963 2070 6978 656c 2074  specific pixel t
+00001740: 696d 6573 6572 6965 733f 3c2f 613e 3c2f  imeseries?</a></
+00001750: 7375 6d6d 6172 793e 0a0a 5468 6520 3c61  summary>..The <a
+00001760: 2068 7265 663d 6874 7470 733a 2f2f 6769   href=https://gi
+00001770: 7468 7562 2e63 6f6d 2f6e 6173 6168 6172  thub.com/nasahar
+00001780: 7665 7374 2f63 726f 7068 6172 7665 7374  vest/cropharvest
+00001790: 2f69 7373 7565 732f 3130 363e 7370 6563  /issues/106>spec
+000017a0: 6966 6963 2075 7365 2063 6173 653c 2f61  ific use case</a
+000017b0: 3e20 6865 7265 2069 7320 746f 2072 6574  > here is to ret
+000017c0: 7269 6576 6520 4e44 5649 2076 616c 7565  rieve NDVI value
+000017d0: 7320 666f 7220 6120 7370 6563 6966 6963  s for a specific
+000017e0: 2072 6f77 2069 6e20 7468 6520 606c 6162   row in the `lab
+000017f0: 656c 732e 6765 6f6a 736f 6e60 2e20 4865  els.geojson`. He
+00001800: 7265 2069 7320 686f 7720 796f 7520 6d69  re is how you mi
+00001810: 6768 7420 676f 2061 626f 7574 2064 6f69  ght go about doi
+00001820: 6e67 2074 6861 743a 0a0a 4669 7273 746c  ng that:..Firstl
+00001830: 792c 2049 2077 696c 6c20 6c6f 6164 2074  y, I will load t
+00001840: 6865 2067 656f 736a 6f6e 2e20 4927 6c6c  he geosjon. I'll
+00001850: 2064 6f20 6974 2074 6872 6f75 6768 2061   do it through a
+00001860: 2060 4372 6f70 4861 7276 6573 744c 6162   `CropHarvestLab
+00001870: 656c 7360 206f 626a 6563 742c 2077 6869  els` object, whi
+00001880: 6368 2069 7320 6a75 7374 2061 2077 7261  ch is just a wra
+00001890: 7070 6572 2061 726f 756e 6420 7468 6520  pper around the 
+000018a0: 6765 6f6a 736f 6e20 6275 7420 7072 6f76  geojson but prov
+000018b0: 6964 6573 2073 6f6d 6520 6e69 6365 2075  ides some nice u
+000018c0: 7469 6c69 7479 2066 756e 6374 696f 6e73  tility functions
+000018d0: 2e0a 6060 6070 7974 686f 6e0a 3e3e 3e20  ..```python.>>> 
+000018e0: 6672 6f6d 2063 726f 7068 6172 7665 7374  from cropharvest
+000018f0: 2e64 6174 6173 6574 7320 696d 706f 7274  .datasets import
+00001900: 2043 726f 7048 6172 7665 7374 4c61 6265   CropHarvestLabe
+00001910: 6c73 0a3e 3e3e 0a3e 3e3e 206c 6162 656c  ls.>>>.>>> label
+00001920: 7320 3d20 4372 6f70 4861 7276 6573 744c  s = CropHarvestL
+00001930: 6162 656c 7328 2263 726f 7068 6172 7665  abels("cropharve
+00001940: 7374 2f64 6174 6122 290a 3e3e 3e20 6c61  st/data").>>> la
+00001950: 6265 6c73 5f67 656f 6a73 6f6e 203d 206c  bels_geojson = l
+00001960: 6162 656c 732e 6173 5f67 656f 6a73 6f6e  abels.as_geojson
+00001970: 2829 0a3e 3e3e 206c 6162 656c 735f 6765  ().>>> labels_ge
+00001980: 6f6a 736f 6e2e 6865 6164 2829 0a20 2068  ojson.head().  h
+00001990: 6172 7665 7374 5f64 6174 6520 706c 616e  arvest_date plan
+000019a0: 7469 6e67 5f64 6174 6520 202e 2e2e 2069  ting_date  ... i
+000019b0: 735f 7465 7374 2020 2020 2020 2020 2020  s_test          
+000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019e0: 2067 656f 6d65 7472 790a 3020 2020 2020   geometry.0     
+000019f0: 2020 2020 4e6f 6e65 2020 2020 2020 2020      None        
+00001a00: 2020 4e6f 6e65 2020 2e2e 2e20 2020 4661    None  ...   Fa
+00001a10: 6c73 6520 2050 4f4c 5947 4f4e 2028 2833  lse  POLYGON ((3
+00001a20: 372e 3038 3235 3220 3130 2e37 3132 3734  7.08252 10.71274
+00001a30: 2c20 3337 2e30 3833 3438 2031 302e 3731  , 37.08348 10.71
+00001a40: 3239 312e 2e2e 0a31 2020 2020 2020 2020  291....1        
+00001a50: 204e 6f6e 6520 2020 2020 2020 2020 204e   None          N
+00001a60: 6f6e 6520 202e 2e2e 2020 2046 616c 7365  one  ...   False
+00001a70: 2020 504f 4c59 474f 4e20 2828 3337 2e30    POLYGON ((37.0
+00001a80: 3837 3231 2031 302e 3732 3339 382c 2033  8721 10.72398, 3
+00001a90: 372e 3038 3731 3420 3130 2e37 3234 3239  7.08714 10.72429
+00001aa0: 2e2e 2e0a 3220 2020 2020 2020 2020 4e6f  ....2         No
+00001ab0: 6e65 2020 2020 2020 2020 2020 4e6f 6e65  ne          None
+00001ac0: 2020 2e2e 2e20 2020 4661 6c73 6520 2050    ...   False  P
+00001ad0: 4f4c 5947 4f4e 2028 2833 372e 3038 3439  OLYGON ((37.0849
+00001ae0: 3820 3130 2e37 3133 3731 2c20 3337 2e30  8 10.71371, 37.0
+00001af0: 3834 3831 2031 302e 3731 3339 332e 2e2e  8481 10.71393...
+00001b00: 0a33 2020 2020 2020 2020 204e 6f6e 6520  .3         None 
+00001b10: 2020 2020 2020 2020 204e 6f6e 6520 202e           None  .
+00001b20: 2e2e 2020 2046 616c 7365 2020 504f 4c59  ..   False  POLY
+00001b30: 474f 4e20 2828 3337 2e30 3930 3231 2031  GON ((37.09021 1
+00001b40: 302e 3731 3332 302c 2033 372e 3039 3031  0.71320, 37.0901
+00001b50: 3420 3130 2e37 3133 3431 2e2e 2e0a 3420  4 10.71341....4 
+00001b60: 2020 2020 2020 2020 4e6f 6e65 2020 2020          None    
+00001b70: 2020 2020 2020 4e6f 6e65 2020 2e2e 2e20        None  ... 
+00001b80: 2020 4661 6c73 6520 2050 4f4c 5947 4f4e    False  POLYGON
+00001b90: 2028 2833 372e 3038 3330 3720 3130 2e37   ((37.08307 10.7
+00001ba0: 3231 3630 2c20 3337 2e30 3832 3831 2031  2160, 37.08281 1
+00001bb0: 302e 3732 3139 372e 2e2e 0a0a 5b35 2072  0.72197.....[5 r
+00001bc0: 6f77 7320 7820 3133 2063 6f6c 756d 6e73  ows x 13 columns
+00001bd0: 5d0a 6060 600a 0a4e 6f77 2c20 4920 6361  ].```..Now, I ca
+00001be0: 6e20 7573 6520 7468 6520 606c 6162 656c  n use the `label
+00001bf0: 7360 206f 626a 6563 7420 746f 2072 6574  s` object to ret
+00001c00: 7269 6576 6520 7468 6520 6669 6c65 7061  rieve the filepa
+00001c10: 7468 206f 6620 7468 6520 7072 6f63 6573  th of the proces
+00001c20: 7365 6420 7361 7465 6c6c 6974 6520 6461  sed satellite da
+00001c30: 7461 2066 6f72 2065 6163 6820 726f 7720  ta for each row 
+00001c40: 696e 2074 6865 206c 6162 656c 7320 6765  in the labels ge
+00001c50: 6f6a 736f 6e3a 0a60 6060 7079 7468 6f6e  ojson:.```python
+00001c60: 0a3e 3e3e 2070 6174 685f 746f 5f66 696c  .>>> path_to_fil
+00001c70: 6520 3d20 6c61 6265 6c73 2e5f 7061 7468  e = labels._path
+00001c80: 5f66 726f 6d5f 726f 7728 6c61 6265 6c73  _from_row(labels
+00001c90: 5f67 656f 6a73 6f6e 2e69 6c6f 635b 305d  _geojson.iloc[0]
+00001ca0: 290a 6060 600a 5468 6973 2070 726f 6365  ).```.This proce
+00001cb0: 7373 6564 2073 6174 656c 6c69 7465 2064  ssed satellite d
+00001cc0: 6174 6120 6973 2073 746f 7265 6420 6173  ata is stored as
+00001cd0: 2060 6835 7079 6020 6669 6c65 732c 2073   `h5py` files, s
+00001ce0: 6f20 4920 6361 6e20 6c6f 6164 2069 7420  o I can load it 
+00001cf0: 7570 2061 7320 666f 6c6c 6f77 733a 0a60  up as follows:.`
+00001d00: 6060 7079 7468 6f6e 0a3e 3e3e 2069 6d70  ``python.>>> imp
+00001d10: 6f72 7420 6835 7079 0a3e 3e3e 2068 3570  ort h5py.>>> h5p
+00001d20: 795f 6669 6c65 203d 2068 3570 792e 4669  y_file = h5py.Fi
+00001d30: 6c65 2870 6174 685f 746f 5f66 696c 652c  le(path_to_file,
+00001d40: 2022 7222 290a 3e3e 3e20 7820 3d20 6835   "r").>>> x = h5
+00001d50: 7079 5f66 696c 652e 6765 7428 2261 7272  py_file.get("arr
+00001d60: 6179 2229 5b3a 5d0a 3e3e 3e20 782e 7368  ay")[:].>>> x.sh
+00001d70: 6170 650a 2831 322c 2031 3829 0a60 6060  ape.(12, 18).```
+00001d80: 0a54 6865 2073 6861 7065 206f 6620 6078  .The shape of `x
+00001d90: 6020 7265 7072 6573 656e 7473 2031 3220  ` represents 12 
+00001da0: 7469 6d65 7374 6570 7320 616e 6420 3138  timesteps and 18
+00001db0: 2062 616e 6473 2e20 546f 2072 6574 7269   bands. To retri
+00001dc0: 6576 6520 7468 6520 6261 6e64 2049 2061  eve the band I a
+00001dd0: 6d20 696e 7465 7265 7374 6564 2069 6e3a  m interested in:
+00001de0: 0a60 6060 7079 7468 6f6e 0a3e 3e3e 2066  .```python.>>> f
+00001df0: 726f 6d20 6372 6f70 6861 7276 6573 742e  rom cropharvest.
+00001e00: 6261 6e64 7320 696d 706f 7274 2042 414e  bands import BAN
+00001e10: 4453 0a3e 3e3e 2078 5b3a 2c20 4241 4e44  DS.>>> x[:, BAND
+00001e20: 532e 696e 6465 7828 224e 4456 4922 295d  S.index("NDVI")]
+00001e30: 0a61 7272 6179 285b 302e 3238 3939 3230  .array([0.289920
+00001e40: 3732 2c20 302e 3238 3833 3833 3433 2c20  72, 0.28838343, 
+00001e50: 302e 3236 3833 3335 3739 2c20 302e 3232  0.26833579, 0.22
+00001e60: 3537 3736 3333 2c20 302e 3237 3133 3839  577633, 0.271389
+00001e70: 3836 2c0a 2020 2020 2020 2030 2e30 3635  86,.       0.065
+00001e80: 3834 3131 342c 2030 2e34 3938 3939 3820  84114, 0.498998 
+00001e90: 202c 2030 2e35 3031 3437 3230 332c 2030   , 0.50147203, 0
+00001ea0: 2e35 3034 3337 3734 332c 2030 2e34 3433  .50437743, 0.443
+00001eb0: 3236 3334 332c 0a20 2020 2020 2020 302e  26343,.       0.
+00001ec0: 3333 3733 3538 3439 2c20 302e 3238 3337  33735849, 0.2837
+00001ed0: 3539 3637 5d29 0a60 6060 0a54 6865 7365  5967]).```.These
+00001ee0: 2061 7265 2031 3220 4e44 5649 2076 616c   are 12 NDVI val
+00001ef0: 7565 732c 2063 6f72 7265 7370 6f6e 6469  ues, correspondi
+00001f00: 6e67 2074 6f20 7468 6520 3132 206d 6f6e  ng to the 12 mon
+00001f10: 7468 7320 6361 7074 7572 6564 2069 6e20  ths captured in 
+00001f20: 7468 6973 2074 696d 6573 6572 6965 732e  this timeseries.
+00001f30: 2054 6f20 6669 6e64 206f 7574 2065 7861   To find out exa
+00001f40: 6374 6c79 2077 6869 6368 206d 6f6e 7468  ctly which month
+00001f50: 2065 6163 6820 7469 6d65 7374 6570 2072   each timestep r
+00001f60: 6570 7265 7365 6e74 732c 2049 2063 616e  epresents, I can
+00001f70: 2064 6f0a 6060 6070 7974 686f 6e0a 3e3e   do.```python.>>
+00001f80: 3e20 6c61 6265 6c73 5f67 656f 6a73 6f6e  > labels_geojson
+00001f90: 2e69 6c6f 635b 305d 2e65 7870 6f72 745f  .iloc[0].export_
+00001fa0: 656e 645f 6461 7465 0a27 3230 3231 2d30  end_date.'2021-0
+00001fb0: 322d 3031 5430 303a 3030 3a30 3027 0a60  2-01T00:00:00'.`
+00001fc0: 6060 0a57 6963 6820 7465 6c6c 7320 6d65  ``.Wich tells me
+00001fd0: 2074 6861 7420 7468 6520 6c61 7374 2074   that the last t
+00001fe0: 696d 6573 7465 7020 7265 7072 6573 656e  imestep represen
+00001ff0: 7473 204a 616e 7561 7279 2032 3032 312e  ts January 2021.
+00002000: 2049 2063 616e 2077 6f72 6b20 6261 636b   I can work back
+00002010: 7761 7264 7320 6672 6f6d 2074 6865 7265  wards from there
+00002020: 2e0a 0a3c 2f64 6574 6169 6c73 3e0a 0a3c  ...</details>..<
+00002030: 6465 7461 696c 733e 0a3c 7375 6d6d 6172  details>.<summar
+00002040: 793e 3c61 2068 7265 663d 2268 7474 7073  y><a href="https
+00002050: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e61  ://github.com/na
+00002060: 7361 6861 7276 6573 742f 6372 6f70 6861  saharvest/cropha
+00002070: 7276 6573 742f 6973 7375 6573 2f38 3822  rvest/issues/88"
+00002080: 3e57 6861 7420 6973 2074 6865 2064 6174  >What is the dat
+00002090: 6120 666f 726d 6174 3f3c 2f61 3e3c 2f73  a format?</a></s
+000020a0: 756d 6d61 7279 3e0a 5468 6520 7374 7275  ummary>.The stru
+000020b0: 6374 7572 6520 6f66 2074 6865 2064 6966  cture of the dif
+000020c0: 6665 7265 6e74 2064 6174 6120 6669 6c65  ferent data file
+000020d0: 7320 6973 206e 6f77 2064 6573 6372 6962  s is now describ
+000020e0: 6564 2069 6e20 6465 7074 6820 696e 2074  ed in depth in t
+000020f0: 6865 2064 6174 6120 666f 6c64 6572 2773  he data folder's
+00002100: 205b 5265 6164 6d65 5d28 6874 7470 733a   [Readme](https:
+00002110: 2f2f 6769 7468 7562 2e63 6f6d 2f6e 6173  //github.com/nas
+00002120: 6168 6172 7665 7374 2f63 726f 7068 6172  aharvest/crophar
+00002130: 7665 7374 2f62 6c6f 622f 6d61 696e 2f64  vest/blob/main/d
+00002140: 6174 612f 5245 4144 4d45 2e6d 6429 0a3c  ata/README.md).<
+00002150: 2f64 6574 6169 6c73 3e0a 0a23 2323 204c  /details>..### L
+00002160: 6963 656e 7365 0a43 726f 7048 6172 7665  icense.CropHarve
+00002170: 7374 2068 6173 2061 205b 4372 6561 7469  st has a [Creati
+00002180: 7665 2043 6f6d 6d6f 6e73 2041 7474 7269  ve Commons Attri
+00002190: 6275 7469 6f6e 2d53 6861 7265 416c 696b  bution-ShareAlik
+000021a0: 6520 342e 3020 496e 7465 726e 6174 696f  e 4.0 Internatio
+000021b0: 6e61 6c5d 2868 7474 7073 3a2f 2f67 6974  nal](https://git
+000021c0: 6875 622e 636f 6d2f 6e61 7361 6861 7276  hub.com/nasaharv
+000021d0: 6573 742f 6372 6f70 6861 7276 6573 742f  est/cropharvest/
+000021e0: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
+000021f0: 452e 7478 7429 206c 6963 656e 7365 2e0a  E.txt) license..
+00002200: 0a23 2323 2043 6974 6174 696f 6e0a 0a49  .### Citation..I
+00002210: 6620 796f 7520 7573 6520 4372 6f70 4861  f you use CropHa
+00002220: 7276 6573 7420 696e 2079 6f75 7220 7265  rvest in your re
+00002230: 7365 6172 6368 2c20 706c 6561 7365 2075  search, please u
+00002240: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
+00002250: 2063 6974 6174 696f 6e3a 0a60 6060 0a40   citation:.```.@
+00002260: 696e 7072 6f63 6565 6469 6e67 737b 0a20  inproceedings{. 
+00002270: 2020 2074 7365 6e67 3230 3231 6372 6f70     tseng2021crop
+00002280: 6861 7276 6573 742c 0a20 2020 2074 6974  harvest,.    tit
+00002290: 6c65 3d7b 4372 6f70 4861 7276 6573 743a  le={CropHarvest:
+000022a0: 2041 2067 6c6f 6261 6c20 6461 7461 7365   A global datase
+000022b0: 7420 666f 7220 6372 6f70 2d74 7970 6520  t for crop-type 
+000022c0: 636c 6173 7369 6669 6361 7469 6f6e 7d2c  classification},
+000022d0: 0a20 2020 2061 7574 686f 723d 7b47 6162  .    author={Gab
+000022e0: 7269 656c 2054 7365 6e67 2061 6e64 2049  riel Tseng and I
+000022f0: 7661 6e20 5a76 6f6e 6b6f 7620 616e 6420  van Zvonkov and 
+00002300: 4361 7468 6572 696e 6520 4c69 6c69 616e  Catherine Lilian
+00002310: 204e 616b 616c 656d 6265 2061 6e64 2048   Nakalembe and H
+00002320: 616e 6e61 6820 4b65 726e 6572 7d2c 0a20  annah Kerner},. 
+00002330: 2020 2062 6f6f 6b74 6974 6c65 3d7b 5468     booktitle={Th
+00002340: 6972 7479 2d66 6966 7468 2043 6f6e 6665  irty-fifth Confe
+00002350: 7265 6e63 6520 6f6e 204e 6575 7261 6c20  rence on Neural 
+00002360: 496e 666f 726d 6174 696f 6e20 5072 6f63  Information Proc
+00002370: 6573 7369 6e67 2053 7973 7465 6d73 2044  essing Systems D
+00002380: 6174 6173 6574 7320 616e 6420 4265 6e63  atasets and Benc
+00002390: 686d 6172 6b73 2054 7261 636b 2028 526f  hmarks Track (Ro
+000023a0: 756e 6420 3229 7d2c 0a20 2020 2079 6561  und 2)},.    yea
+000023b0: 723d 7b32 3032 317d 2c0a 2020 2020 7572  r={2021},.    ur
+000023c0: 6c3d 7b68 7474 7073 3a2f 2f6f 7065 6e72  l={https://openr
+000023d0: 6576 6965 772e 6e65 742f 666f 7275 6d3f  eview.net/forum?
+000023e0: 6964 3d4a 746a 7a55 5850 4561 4375 7d0a  id=JtjzUXPEaCu}.
+000023f0: 7d0a 6060 600a                           }.```.
```

### Comparing `cropharvest-0.6.0/cropharvest.egg-info/SOURCES.txt` & `cropharvest-0.7.0/cropharvest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cropharvest-0.6.0/setup.py` & `cropharvest-0.7.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,24 +11,25 @@
     name="cropharvest",
     description="Open source remote sensing dataset with benchmarks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Gabriel Tseng",
     author_email="gabrieltseng95@gmail.com",
     url="https://github.com/nasaharvest/cropharvest",
-    version="0.6.0",
+    version="0.7.0",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     packages=["cropharvest"] + [f"cropharvest.{f}" for f in find_packages("cropharvest")],
     install_requires=[
+        "pandas<2.0.0",
         "geopandas==0.9.0",
-        "xarray>=0.16.2",
+        "xarray>=0.16.2, <0.20.0",
         "tqdm>=4.61.1",
         # h5py 3.7.0 breaks windows, see
         # https://github.com/h5py/h5py/issues/2110
         "h5py>=3.1.0,!=3.7.0",
         "rasterio>=1.2.6",
         "openpyxl>=2.5.9",
         "scikit-learn>=0.22.2",
```

