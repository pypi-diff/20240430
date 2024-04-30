# Comparing `tmp/geonomics-1.4.0.tar.gz` & `tmp/geonomics-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geonomics-1.4.0.tar", last modified: Mon Apr  1 13:05:52 2024, max compression
+gzip compressed data, was "geonomics-1.4.1.tar", last modified: Tue Apr 30 00:22:20 2024, max compression
```

## Comparing `geonomics-1.4.0.tar` & `geonomics-1.4.1.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.293627 geonomics-1.4.0/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     1112 2024-01-03 01:50:01.000000 geonomics-1.4.0/LICENSE.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)       74 2021-03-24 04:15:31.000000 geonomics-1.4.0/MANIFEST.in
--rw-rw-r--   0 deth      (1000) deth      (1000)     9440 2024-04-01 13:05:52.293627 geonomics-1.4.0/PKG-INFO
--rw-rw-r--   0 deth      (1000) deth      (1000)     8326 2022-01-01 18:34:30.000000 geonomics-1.4.0/README.rst
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.241626 geonomics-1.4.0/geonomics/
--rwxrwxr-x   0 deth      (1000) deth      (1000)      499 2022-01-01 17:50:26.000000 geonomics-1.4.0/geonomics/__init__.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.241626 geonomics-1.4.0/geonomics/data/
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.253626 geonomics-1.4.0/geonomics/data/IBD_IBE_demo/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     1573 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/IBD_IBE_demo/MMRR.R
--rwxrwxr-x   0 deth      (1000) deth      (1000)     2807 2023-06-14 19:20:14.000000 geonomics-1.4.0/geonomics/data/IBD_IBE_demo/MMRR.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.257627 geonomics-1.4.0/geonomics/data/IBD_IBE_demo/__pycache__/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     3091 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc
--rwxrwxr-x   0 deth      (1000) deth      (1000)     3067 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc
--rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/IBD_IBE_demo/env.csv
--rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/IBD_IBE_demo/gen.csv
--rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/IBD_IBE_demo/geo.csv
--rwxrwxr-x   0 deth      (1000) deth      (1000)      898 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/IBD_IBE_demo/run_mantel.R
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.257627 geonomics-1.4.0/geonomics/data/default_models/
--rw-rw-r--   0 deth      (1000) deth      (1000)    14817 2021-10-09 01:45:22.000000 geonomics-1.4.0/geonomics/data/default_models/selection_params.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.257627 geonomics-1.4.0/geonomics/data/yosemite_demo/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35632 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.257627 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.265627 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34429 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34424 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34399 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34379 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34604 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34326 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34361 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34407 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34382 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34292 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34435 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34351 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34256 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34516 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    29050 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.277627 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35877 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36099 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35864 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35990 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35953 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35962 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36177 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35922 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35932 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35896 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36275 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36218 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36091 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36181 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35874 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36217 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36109 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.285627 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31648 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31717 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31807 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31507 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31710 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31645 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31584 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31437 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31454 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31455 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31446 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31556 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31499 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31484 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31434 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31516 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31416 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31225 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    20497 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.285627 geonomics-1.4.0/geonomics/demos/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    40012 2021-08-30 15:43:03.000000 geonomics-1.4.0/geonomics/demos/_IBD_IBE.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)       76 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/demos/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    23746 2021-08-30 20:54:50.000000 geonomics-1.4.0/geonomics/demos/_simult_select.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    40559 2021-08-30 20:54:24.000000 geonomics-1.4.0/geonomics/demos/_yosemite.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.285627 geonomics-1.4.0/geonomics/help/
--rwxrwxr-x   0 deth      (1000) deth      (1000)      728 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/help/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     2260 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/help/_memory_help.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    19956 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/help/_param_help.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    42853 2024-04-01 12:51:51.000000 geonomics-1.4.0/geonomics/main.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.289627 geonomics-1.4.0/geonomics/ops/
--rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/ops/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36149 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/ops/change.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    11576 2024-03-26 13:35:21.000000 geonomics-1.4.0/geonomics/ops/demography.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    10192 2021-09-21 22:53:47.000000 geonomics-1.4.0/geonomics/ops/mating.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     6555 2021-03-24 04:15:27.000000 geonomics-1.4.0/geonomics/ops/movement.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     8345 2024-03-29 11:47:20.000000 geonomics-1.4.0/geonomics/ops/mutation.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     5094 2021-07-09 03:11:40.000000 geonomics-1.4.0/geonomics/ops/selection.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.289627 geonomics-1.4.0/geonomics/sim/
--rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/sim/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     3405 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/sim/burnin.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    23562 2022-12-26 20:26:33.000000 geonomics-1.4.0/geonomics/sim/data.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)   142781 2024-04-01 03:38:11.000000 geonomics-1.4.0/geonomics/sim/model.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    49119 2024-04-01 12:20:05.000000 geonomics-1.4.0/geonomics/sim/params.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    19972 2023-04-13 16:46:44.000000 geonomics-1.4.0/geonomics/sim/stats.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.289627 geonomics-1.4.0/geonomics/structs/
--rwxrwxr-x   0 deth      (1000) deth      (1000)      116 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/structs/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     5433 2021-07-09 03:11:40.000000 geonomics-1.4.0/geonomics/structs/community.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    87852 2024-03-31 14:11:08.000000 geonomics-1.4.0/geonomics/structs/genome.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     8672 2021-07-09 03:11:40.000000 geonomics-1.4.0/geonomics/structs/individual.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    32817 2021-07-09 03:11:40.000000 geonomics-1.4.0/geonomics/structs/landscape.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)   153475 2024-04-01 03:44:04.000000 geonomics-1.4.0/geonomics/structs/species.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.293627 geonomics-1.4.0/geonomics/utils/
--rwxrwxr-x   0 deth      (1000) deth      (1000)       82 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/utils/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)      607 2021-03-24 04:15:28.000000 geonomics-1.4.0/geonomics/utils/_str_repr_.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    10991 2023-04-13 17:58:34.000000 geonomics-1.4.0/geonomics/utils/io.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    21410 2022-12-26 20:39:40.000000 geonomics-1.4.0/geonomics/utils/spatial.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    16746 2021-03-24 04:15:29.000000 geonomics-1.4.0/geonomics/utils/viz.py
--rw-rw-r--   0 deth      (1000) deth      (1000)       22 2024-04-01 03:57:06.000000 geonomics-1.4.0/geonomics/version.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-01 13:05:52.245627 geonomics-1.4.0/geonomics.egg-info/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     9440 2024-04-01 13:05:51.000000 geonomics-1.4.0/geonomics.egg-info/PKG-INFO
--rwxrwxr-x   0 deth      (1000) deth      (1000)     5542 2024-04-01 13:05:52.000000 geonomics-1.4.0/geonomics.egg-info/SOURCES.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)        1 2024-04-01 13:05:51.000000 geonomics-1.4.0/geonomics.egg-info/dependency_links.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)       86 2024-04-01 13:05:51.000000 geonomics-1.4.0/geonomics.egg-info/requires.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)       10 2024-04-01 13:05:51.000000 geonomics-1.4.0/geonomics.egg-info/top_level.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)      107 2024-04-01 13:05:52.293627 geonomics-1.4.0/setup.cfg
--rwxrwxr-x   0 deth      (1000) deth      (1000)     2680 2022-01-01 17:57:19.000000 geonomics-1.4.0/setup.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.556071 geonomics-1.4.1/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     1112 2024-01-03 01:50:01.000000 geonomics-1.4.1/LICENSE.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       74 2021-03-24 04:15:31.000000 geonomics-1.4.1/MANIFEST.in
+-rw-rw-r--   0 deth      (1000) deth      (1000)     9440 2024-04-30 00:22:20.556071 geonomics-1.4.1/PKG-INFO
+-rw-rw-r--   0 deth      (1000) deth      (1000)     8326 2022-01-01 18:34:30.000000 geonomics-1.4.1/README.rst
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.204071 geonomics-1.4.1/geonomics/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      499 2022-01-01 17:50:26.000000 geonomics-1.4.1/geonomics/__init__.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.200070 geonomics-1.4.1/geonomics/data/
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.216071 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     1573 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/MMRR.R
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     2807 2023-06-14 19:20:14.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/MMRR.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.216071 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/__pycache__/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     3091 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     3067 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc
+-rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/env.csv
+-rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/gen.csv
+-rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/geo.csv
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      898 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/IBD_IBE_demo/run_mantel.R
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.216071 geonomics-1.4.1/geonomics/data/default_models/
+-rw-rw-r--   0 deth      (1000) deth      (1000)    14817 2021-10-09 01:45:22.000000 geonomics-1.4.1/geonomics/data/default_models/selection_params.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.216071 geonomics-1.4.1/geonomics/data/yosemite_demo/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35632 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.220071 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.224071 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34429 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34424 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34399 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34379 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34604 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34326 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34361 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34407 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34382 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34292 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34435 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34351 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34256 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34516 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    29050 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.232071 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35877 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36099 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35864 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35990 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35953 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35962 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36177 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35922 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35932 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35896 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36275 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36218 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36091 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36181 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35874 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36217 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36109 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.240071 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31648 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31717 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31807 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31507 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31710 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31645 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31584 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31437 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31454 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31455 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31446 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31556 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31499 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31484 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31434 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31516 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31416 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31225 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    20497 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.328071 geonomics-1.4.1/geonomics/demos/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    40012 2021-08-30 15:43:03.000000 geonomics-1.4.1/geonomics/demos/_IBD_IBE.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       76 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/demos/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    23746 2021-08-30 20:54:50.000000 geonomics-1.4.1/geonomics/demos/_simult_select.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    40559 2021-08-30 20:54:24.000000 geonomics-1.4.1/geonomics/demos/_yosemite.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.328071 geonomics-1.4.1/geonomics/help/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      728 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/help/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     2260 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/help/_memory_help.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    19956 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/help/_param_help.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    42853 2024-04-01 12:51:51.000000 geonomics-1.4.1/geonomics/main.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.376071 geonomics-1.4.1/geonomics/ops/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/ops/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36149 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/ops/change.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    11576 2024-03-26 13:35:21.000000 geonomics-1.4.1/geonomics/ops/demography.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    10192 2021-09-21 22:53:47.000000 geonomics-1.4.1/geonomics/ops/mating.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     6555 2021-03-24 04:15:27.000000 geonomics-1.4.1/geonomics/ops/movement.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     8345 2024-03-29 11:47:20.000000 geonomics-1.4.1/geonomics/ops/mutation.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     5094 2021-07-09 03:11:40.000000 geonomics-1.4.1/geonomics/ops/selection.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.464071 geonomics-1.4.1/geonomics/sim/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/sim/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     3405 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/sim/burnin.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    23562 2022-12-26 20:26:33.000000 geonomics-1.4.1/geonomics/sim/data.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)   142795 2024-04-30 00:17:16.000000 geonomics-1.4.1/geonomics/sim/model.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    49119 2024-04-01 12:20:05.000000 geonomics-1.4.1/geonomics/sim/params.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    19972 2023-04-13 16:46:44.000000 geonomics-1.4.1/geonomics/sim/stats.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.512071 geonomics-1.4.1/geonomics/structs/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      116 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/structs/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     5851 2024-04-30 00:00:02.000000 geonomics-1.4.1/geonomics/structs/community.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    88196 2024-04-29 23:24:41.000000 geonomics-1.4.1/geonomics/structs/genome.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     8672 2021-07-09 03:11:40.000000 geonomics-1.4.1/geonomics/structs/individual.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    32817 2021-07-09 03:11:40.000000 geonomics-1.4.1/geonomics/structs/landscape.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)   153475 2024-04-01 03:44:04.000000 geonomics-1.4.1/geonomics/structs/species.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.556071 geonomics-1.4.1/geonomics/utils/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       82 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/utils/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      607 2021-03-24 04:15:28.000000 geonomics-1.4.1/geonomics/utils/_str_repr_.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    10991 2023-04-13 17:58:34.000000 geonomics-1.4.1/geonomics/utils/io.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    21410 2022-12-26 20:39:40.000000 geonomics-1.4.1/geonomics/utils/spatial.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    16746 2021-03-24 04:15:29.000000 geonomics-1.4.1/geonomics/utils/viz.py
+-rw-rw-r--   0 deth      (1000) deth      (1000)       22 2024-04-29 23:26:19.000000 geonomics-1.4.1/geonomics/version.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-04-30 00:22:20.204071 geonomics-1.4.1/geonomics.egg-info/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     9440 2024-04-30 00:22:19.000000 geonomics-1.4.1/geonomics.egg-info/PKG-INFO
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     5542 2024-04-30 00:22:20.000000 geonomics-1.4.1/geonomics.egg-info/SOURCES.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)        1 2024-04-30 00:22:19.000000 geonomics-1.4.1/geonomics.egg-info/dependency_links.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       86 2024-04-30 00:22:19.000000 geonomics-1.4.1/geonomics.egg-info/requires.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       10 2024-04-30 00:22:19.000000 geonomics-1.4.1/geonomics.egg-info/top_level.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      107 2024-04-30 00:22:20.556071 geonomics-1.4.1/setup.cfg
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     2680 2022-01-01 17:57:19.000000 geonomics-1.4.1/setup.py
```

### Comparing `geonomics-1.4.0/LICENSE.txt` & `geonomics-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/PKG-INFO` & `geonomics-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: geonomics
-Version: 1.4.0
+Version: 1.4.1
 Summary: A package for landscape genomic simulation
 Home-page: https://github.com/drewhart/geonomics
-Download-URL: https://github.com/drewhart/geonomics/archive/1.4.0.tar.gz
+Download-URL: https://github.com/drewhart/geonomics/archive/1.4.1.tar.gz
 Author: Drew Ellison Hart
 Author-email: drew.ellison.hart@gmail.com
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/drewhart/geonomics/blob/master/doc/built/doc.html
 Project-URL: Source, https://github.com/drewhart/geonomics
 Keywords: landscape genomics genetics ecology evolution simulation model environmental model agent-based
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geonomics-1.4.0/README.rst` & `geonomics-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/IBD_IBE_demo/MMRR.R` & `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/MMRR.R`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/IBD_IBE_demo/MMRR.py` & `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/MMRR.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc` & `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc` & `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/IBD_IBE_demo/env.csv` & `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/env.csv`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/IBD_IBE_demo/gen.csv` & `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/gen.csv`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/IBD_IBE_demo/geo.csv` & `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/geo.csv`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/IBD_IBE_demo/run_mantel.R` & `geonomics-1.4.1/geonomics/data/IBD_IBE_demo/run_mantel.R`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/default_models/selection_params.py` & `geonomics-1.4.1/geonomics/data/default_models/selection_params.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif` & `geonomics-1.4.1/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/demos/_IBD_IBE.py` & `geonomics-1.4.1/geonomics/demos/_IBD_IBE.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/demos/_simult_select.py` & `geonomics-1.4.1/geonomics/demos/_simult_select.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/demos/_yosemite.py` & `geonomics-1.4.1/geonomics/demos/_yosemite.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/help/__init__.py` & `geonomics-1.4.1/geonomics/help/__init__.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/help/_memory_help.py` & `geonomics-1.4.1/geonomics/help/_memory_help.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/help/_param_help.py` & `geonomics-1.4.1/geonomics/help/_param_help.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/main.py` & `geonomics-1.4.1/geonomics/main.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/ops/change.py` & `geonomics-1.4.1/geonomics/ops/change.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/ops/demography.py` & `geonomics-1.4.1/geonomics/ops/demography.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/ops/mating.py` & `geonomics-1.4.1/geonomics/ops/mating.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/ops/movement.py` & `geonomics-1.4.1/geonomics/ops/movement.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/ops/mutation.py` & `geonomics-1.4.1/geonomics/ops/mutation.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/ops/selection.py` & `geonomics-1.4.1/geonomics/ops/selection.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/sim/burnin.py` & `geonomics-1.4.1/geonomics/sim/burnin.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/sim/data.py` & `geonomics-1.4.1/geonomics/sim/data.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/sim/model.py` & `geonomics-1.4.1/geonomics/sim/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,15 +393,17 @@
 
     #wrapper around Species._make_change
     def _make_spp_change(self, spp_idx):
         self.comm[spp_idx]._make_change(verbose = self._verbose)
 
     #wrapper around Community._check_burned
     def _check_comm_burned(self):
-        self.comm._check_burned(burn_T = self.burn_T)
+        self.comm._check_burned(burn_T=self.burn_T,
+                                params=self.params,
+                               )
 
     ###################################################
 
     #method to wrap around landscape._make_landscape
     def _make_landscape(self, verbose=False):
         land = _make_landscape(mod=self, params=self.params,
                                verbose=verbose)
@@ -957,27 +959,26 @@
             mode, the Model will run for precisely this many timesteps. If in
             'burn' mode, it will run either until stationarity statistics
             indicate that it has burned in, or for this many timesteps,
             whichever occurs first.) Defaults to a single timestep.
             single step.
         mode : {'burn', 'main'}, optional
             The mode in which to run the Model.
-            If 'burn', it will run in burn-in mode. This entails the following:
-                - Genomes will not yet be assigned, so genomic phenomena such
-                  as crossing-over and natural selection will not occur;
-                - Any scheduled landscape and demographic changes will not
-                  occur;
-                - Statiionarity statistics will be checked at the end of each
-                  timestep, to determine if the Model has burned in (in which
-                  case the model will stop running regardless of timestep,
-                  genomes will be randomly assigned to all individuals, and
-                  the Model will be deemed ready to run in main mode)
             If 'main', it will run in main mode (i.e. all functionalities will
             be used. (Note that for a Model to run in main mode it must first
             have been burned in.)
+            If 'burn', it will run in burn-in mode. This entails the following:
+            1. Genomes will not yet be assigned, so genomic phenomena such
+            as crossing-over and natural selection will not occur;
+            2. Any scheduled landscape and demographic changes will not occur;
+            3. Stationarity statistics will be checked at the end of each
+            timestep, to determine if the Model has burned in (in which
+            case the model will stop running regardless of timestep,
+            genomes will be randomly assigned to all individuals, and
+            the Model will be deemed ready to run in main mode).
         verbose : bool, optional
             Whether or not to run the Model should provide written output.
             If True, formatted messages will be printed to STDOUT at each
             timestep. Defaults to True for `Model.walk`.
         animate : {tuple of ints, bool}, optional
             If a length-2 tuple of integers is provided, the Species indicated
             by the first number will be plotted on the Landscape Layer
@@ -3035,20 +3036,20 @@
             population from which individuals will be taken
             (or an int or str referring to that Species within this Model).
 
         source_msprime_params: dict, optional, default: None
             A dict of keyword args to be fed to `gnx.sim_msprime_individs()`,
             to parameterize the msprime source population model from which
             new Individuals will be drawn. These include:
-                recomb_rate         (required)
-                mut_rate            (required)
-                demography          (optional; default: None)
-                population_size     (optional; default: None)
-                ancestry_model      (optional; default: None)
-                random_seed         (optional; default: None)
+            - recomb_rate         (required)
+            - mut_rate            (required)
+            - demography          (optional; default: None)
+            - population_size     (optional; default: None)
+            - ancestry_model      (optional; default: None)
+            - random_seed         (optional; default: None)
             See `gnx.sim_msprime_individs` for details.
 
         individs: {tuple, list, numpy.ndarray}, optional, default: None
             A 1d numpy.ndarray or equivalent array-like containing the int indices
             of the Individuals to be taken from `source_spp` and added to
             `recip_spp`. If None
```

### Comparing `geonomics-1.4.0/geonomics/sim/params.py` & `geonomics-1.4.1/geonomics/sim/params.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/sim/stats.py` & `geonomics-1.4.1/geonomics/sim/stats.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/structs/community.py` & `geonomics-1.4.1/geonomics/structs/community.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,26 +100,35 @@
         self.t += 1
 
     #method to reset the self.t attribute (the timestep counter)
     def _reset_t(self):
         self.t = -1
 
     #method to check if all species have burned in
-    def _check_burned(self, burn_T):
-        #check minimum burn-in time has passed
-        burnin_status= np.all([len(spp.Nt) >= burn_T for spp in self.values()])
-        #if so, then check all burn-in tests for all spps
-        if burnin_status:
-            adf_tests = np.all([burnin._test_adf_threshold(spp, burn_T) for
-                                spp in self.values()])
-            t_tests = np.all([burnin._test_t_threshold(spp, burn_T) for
-                                spp in self.values()])
-            spat_tests = np.all([spp._do_spatial_burnin_test(burn_T) for
-                                 spp in self.values()])
-            burnin_status = adf_tests and t_tests and spat_tests
+    def _check_burned(self,
+                      burn_T,
+                      params,
+                     ):
+        # if pop will be replaced by msprime individs then short-circuit burn-in
+        all_msprime = np.all(['msprime' in spp_params['init'] for
+                              spp_params in params['comm']['species'].values()])
+        if all_msprime:
+            burnin_status = True
+        else:
+            #check minimum burn-in time has passed
+            burnin_status= np.all([len(spp.Nt) >= burn_T for spp in self.values()])
+            #if so, then check all burn-in tests for all spps
+            if burnin_status:
+                adf_tests = np.all([burnin._test_adf_threshold(spp, burn_T) for
+                                    spp in self.values()])
+                t_tests = np.all([burnin._test_t_threshold(spp, burn_T) for
+                                    spp in self.values()])
+                spat_tests = np.all([spp._do_spatial_burnin_test(burn_T) for
+                                     spp in self.values()])
+                burnin_status = adf_tests and t_tests and spat_tests
         #set the community burn-in tracker
         self.burned = burnin_status
         #and set the spps' burn-in trackers
         [setattr(spp, 'burned', burnin_status) for spp in self.values()]
 
 
 ######################################
```

### Comparing `geonomics-1.4.0/geonomics/structs/genome.py` & `geonomics-1.4.1/geonomics/structs/genome.py`

 * *Files 0% similar despite different names*

```diff
@@ -871,15 +871,19 @@
     # get the genome parameters
     g_params = spp_params.gen_arch
     # get the custom genomic-architecture file, if provided
     gen_arch_file = None
     if 'gen_arch_file' in g_params.keys():
         if g_params.gen_arch_file is not None:
             gen_arch_file = pd.read_csv(g_params.gen_arch_file)
-
+            # check that the genome length matches the params file
+            assert len(gen_arch_file) == g_params.L, ("The length of the "
+                        "custom genomic architecture file must match the "
+                        "genome length provided to the parameter 'L' in "
+                        "Geonomics parameters file.")
             # check that each trait is assigned an alpha value
             for trt_val, alpha_val in zip(gen_arch_file['trait'],
                                           gen_arch_file['alpha']):
                 if pd.notnull(trt_val):
                     assert pd.notnull(alpha_val), ("All trait-associated loci "
                                                    "specified in a custom "
                                                    "genomic architecture file "
```

### Comparing `geonomics-1.4.0/geonomics/structs/individual.py` & `geonomics-1.4.1/geonomics/structs/individual.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/structs/landscape.py` & `geonomics-1.4.1/geonomics/structs/landscape.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/structs/species.py` & `geonomics-1.4.1/geonomics/structs/species.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/utils/_str_repr_.py` & `geonomics-1.4.1/geonomics/utils/_str_repr_.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/utils/io.py` & `geonomics-1.4.1/geonomics/utils/io.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/utils/spatial.py` & `geonomics-1.4.1/geonomics/utils/spatial.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics/utils/viz.py` & `geonomics-1.4.1/geonomics/utils/viz.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/geonomics.egg-info/PKG-INFO` & `geonomics-1.4.1/geonomics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: geonomics
-Version: 1.4.0
+Version: 1.4.1
 Summary: A package for landscape genomic simulation
 Home-page: https://github.com/drewhart/geonomics
-Download-URL: https://github.com/drewhart/geonomics/archive/1.4.0.tar.gz
+Download-URL: https://github.com/drewhart/geonomics/archive/1.4.1.tar.gz
 Author: Drew Ellison Hart
 Author-email: drew.ellison.hart@gmail.com
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/drewhart/geonomics/blob/master/doc/built/doc.html
 Project-URL: Source, https://github.com/drewhart/geonomics
 Keywords: landscape genomics genetics ecology evolution simulation model environmental model agent-based
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geonomics-1.4.0/geonomics.egg-info/SOURCES.txt` & `geonomics-1.4.1/geonomics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.0/setup.py` & `geonomics-1.4.1/setup.py`

 * *Files identical despite different names*

