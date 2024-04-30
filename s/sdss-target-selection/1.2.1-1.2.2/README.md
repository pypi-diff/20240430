# Comparing `tmp/sdss_target_selection-1.2.1.tar.gz` & `tmp/sdss_target_selection-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_target_selection-1.2.1.tar", last modified: Thu Apr 25 23:06:37 2024, max compression
+gzip compressed data, was "sdss_target_selection-1.2.2.tar", last modified: Tue Apr 30 18:59:34 2024, max compression
```

## Comparing `sdss_target_selection-1.2.1.tar` & `sdss_target_selection-1.2.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.745427 sdss_target_selection-1.2.1/
--rw-r--r--   0 gallegoj   (501) staff       (20)     1504 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/LICENSE.md
--rw-r--r--   0 gallegoj   (501) staff       (20)       79 2024-02-07 23:03:33.000000 sdss_target_selection-1.2.1/MANIFEST.in
--rw-r--r--   0 gallegoj   (501) staff       (20)     3969 2024-04-25 23:06:37.744903 sdss_target_selection-1.2.1/PKG-INFO
--rw-r--r--   0 gallegoj   (501) staff       (20)     1485 2024-04-25 14:27:13.000000 sdss_target_selection-1.2.1/README.md
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.652361 sdss_target_selection-1.2.1/bin/
--rw-r--r--   0 gallegoj   (501) staff       (20)      302 2024-02-07 23:03:33.000000 sdss_target_selection-1.2.1/bin/target_selection
--rwxr-xr-x   0 gallegoj   (501) staff       (20)     6590 2023-02-07 16:26:59.000000 sdss_target_selection-1.2.1/bin/yanny_scraper
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.644012 sdss_target_selection-1.2.1/python/
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.735895 sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/
--rw-r--r--   0 gallegoj   (501) staff       (20)     3969 2024-04-25 23:06:37.000000 sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/PKG-INFO
--rw-r--r--   0 gallegoj   (501) staff       (20)     3296 2024-04-25 23:06:37.000000 sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/SOURCES.txt
--rw-r--r--   0 gallegoj   (501) staff       (20)        1 2024-04-25 23:06:37.000000 sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/dependency_links.txt
--rw-r--r--   0 gallegoj   (501) staff       (20)        1 2024-02-07 23:06:15.000000 sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/not-zip-safe
--rw-r--r--   0 gallegoj   (501) staff       (20)      624 2024-04-25 23:06:37.000000 sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/requires.txt
--rw-r--r--   0 gallegoj   (501) staff       (20)       17 2024-04-25 23:06:37.000000 sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/top_level.txt
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.663612 sdss_target_selection-1.2.1/python/target_selection/
--rw-r--r--   0 gallegoj   (501) staff       (20)      718 2024-02-14 03:30:22.000000 sdss_target_selection-1.2.1/python/target_selection/__init__.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    11216 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/__main__.py
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.714995 sdss_target_selection-1.2.1/python/target_selection/cartons/
--rw-r--r--   0 gallegoj   (501) staff       (20)     1079 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/__init__.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    50847 2024-04-25 14:27:13.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/base.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    11674 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_aqmes.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    13826 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_csc.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    11105 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_galaxies.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    10763 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_gua.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    14152 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_rm.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    52812 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_spiders_agn.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    16838 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_spiders_clusters.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     2654 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/guide.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    12336 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_bin_gaia.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     5621 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_bin_vis.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    45489 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_cb.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     3361 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_cb_cvcandidates.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    13869 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_dust.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    13013 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_erosita.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    10863 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_galactic.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     8713 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_halo.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    50754 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_halo_gaia_dr3.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     5476 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_legacy_ir2opt.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     7694 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_magcloud_agb.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     7060 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_magcloud_rgb.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    14468 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_monitor_apogee.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     9872 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_ob.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     4055 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_planet.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    25410 2024-04-23 18:31:40.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_rv.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    17466 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_snc.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     4079 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_tess_ob.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     6738 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_tess_rgb.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     4882 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_wd.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    71200 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_yso.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     7568 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/ops_apogee_stds.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    59366 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/ops_boss_stds.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    12519 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/ops_bright_stars.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    15848 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/ops_skies.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     5789 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/skymask.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     2161 2024-04-25 14:27:13.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/too.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    21933 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/cartons/tools.py
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.721035 sdss_target_selection-1.2.1/python/target_selection/config/
--rw-r--r--   0 gallegoj   (501) staff       (20)   147249 2024-04-25 14:27:13.000000 sdss_target_selection-1.2.1/python/target_selection/config/target_selection.yml
--rw-r--r--   0 gallegoj   (501) staff       (20)     9866 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/config/target_selection_v0.yml
--rw-r--r--   0 gallegoj   (501) staff       (20)     8761 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/config/xmatch_v0.yml
--rw-r--r--   0 gallegoj   (501) staff       (20)     6480 2023-04-19 16:37:23.000000 sdss_target_selection-1.2.1/python/target_selection/config/xmatch_v0p5.yml
--rw-r--r--   0 gallegoj   (501) staff       (20)    33349 2024-04-25 21:48:29.000000 sdss_target_selection-1.2.1/python/target_selection/config/xmatch_v1.yml
--rw-r--r--   0 gallegoj   (501) staff       (20)     1383 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/exceptions.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     3148 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/mag_flux.py
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-04-25 23:06:37.734762 sdss_target_selection-1.2.1/python/target_selection/masks/
--rw-r--r--   0 gallegoj   (501) staff       (20)     4171 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/masks/AQMES_wboss_imaging_NGC_proc.ply
--rw-r--r--   0 gallegoj   (501) staff       (20)     8640 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.2.1.fits
--rw-r--r--   0 gallegoj   (501) staff       (20)     8640 2023-02-07 16:26:59.000000 sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.3.1.fits
--rw-r--r--   0 gallegoj   (501) staff       (20)    40320 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.2.1.fits
--rw-r--r--   0 gallegoj   (501) staff       (20)    40320 2023-02-07 16:26:59.000000 sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.3.1.fits
--rw-r--r--   0 gallegoj   (501) staff       (20)     8640 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_rm_v0.2.1.fits
--rw-r--r--   0 gallegoj   (501) staff       (20)   348269 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/masks/rsFields-annotated-lco-deep_proc.ply
--rw-r--r--   0 gallegoj   (501) staff       (20)   135360 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/masks/rsFields_boss_survey.fits
--rw-r--r--   0 gallegoj   (501) staff       (20)    40320 2022-11-28 16:42:41.000000 sdss_target_selection-1.2.1/python/target_selection/masks/rsFields_boss_survey_sgc.fits
--rw-r--r--   0 gallegoj   (501) staff       (20)    37638 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/skies.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    10703 2024-02-07 23:02:35.000000 sdss_target_selection-1.2.1/python/target_selection/utils.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    86826 2024-04-25 22:20:34.000000 sdss_target_selection-1.2.1/python/target_selection/xmatch.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     2541 2024-04-25 23:06:37.748657 sdss_target_selection-1.2.1/setup.cfg
--rw-r--r--   0 gallegoj   (501) staff       (20)       73 2024-02-07 23:03:33.000000 sdss_target_selection-1.2.1/setup.py
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-30 18:59:34.246263 sdss_target_selection-1.2.2/
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     1504 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.2/LICENSE.md
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)       79 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.2/MANIFEST.in
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     3969 2024-04-30 18:59:34.246263 sdss_target_selection-1.2.2/PKG-INFO
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     1485 2024-04-24 00:05:07.000000 sdss_target_selection-1.2.2/README.md
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-30 18:59:34.234263 sdss_target_selection-1.2.2/bin/
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)      302 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.2/bin/target_selection
+-rwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)     6590 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/bin/yanny_scraper
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-30 18:59:34.234263 sdss_target_selection-1.2.2/python/
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-30 18:59:34.242263 sdss_target_selection-1.2.2/python/sdss_target_selection.egg-info/
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     3969 2024-04-30 18:59:34.000000 sdss_target_selection-1.2.2/python/sdss_target_selection.egg-info/PKG-INFO
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     3296 2024-04-30 18:59:34.000000 sdss_target_selection-1.2.2/python/sdss_target_selection.egg-info/SOURCES.txt
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)        1 2024-04-30 18:59:34.000000 sdss_target_selection-1.2.2/python/sdss_target_selection.egg-info/dependency_links.txt
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)        1 2024-04-30 18:59:34.000000 sdss_target_selection-1.2.2/python/sdss_target_selection.egg-info/not-zip-safe
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)      624 2024-04-30 18:59:34.000000 sdss_target_selection-1.2.2/python/sdss_target_selection.egg-info/requires.txt
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)       17 2024-04-30 18:59:34.000000 sdss_target_selection-1.2.2/python/sdss_target_selection.egg-info/top_level.txt
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-30 18:59:34.238263 sdss_target_selection-1.2.2/python/target_selection/
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)      718 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/__init__.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    11216 2023-05-17 22:25:33.000000 sdss_target_selection-1.2.2/python/target_selection/__main__.py
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-30 18:59:34.242263 sdss_target_selection-1.2.2/python/target_selection/cartons/
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     1079 2023-06-01 13:48:09.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/__init__.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    50520 2024-04-30 18:29:12.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/base.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    11674 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/bhm_aqmes.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    13826 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/bhm_csc.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    11105 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/bhm_galaxies.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    10763 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/bhm_gua.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    14152 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/bhm_rm.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    52812 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/bhm_spiders_agn.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    16838 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/bhm_spiders_clusters.py
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     2654 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/guide.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    12336 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_bin_gaia.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     5621 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_bin_vis.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    45489 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_cb.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     3361 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_cb_cvcandidates.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    13869 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_dust.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    13013 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_erosita.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    10863 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_galactic.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     8713 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_halo.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    50754 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_halo_gaia_dr3.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     5476 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_legacy_ir2opt.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     7694 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_magcloud_agb.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     7060 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_magcloud_rgb.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    14468 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_monitor_apogee.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     9872 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_ob.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     4055 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_planet.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    25410 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_rv.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    17466 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_snc.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     4079 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_tess_ob.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     6738 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_tess_rgb.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     4882 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_wd.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    71200 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_yso.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     7568 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/ops_apogee_stds.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    59366 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/ops_boss_stds.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    12519 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/ops_bright_stars.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    15848 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/ops_skies.py
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     5789 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/skymask.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     2161 2024-04-23 23:42:23.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/too.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    21933 2023-05-18 08:21:33.000000 sdss_target_selection-1.2.2/python/target_selection/cartons/tools.py
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-30 18:59:34.242263 sdss_target_selection-1.2.2/python/target_selection/config/
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)   147249 2024-04-23 23:42:23.000000 sdss_target_selection-1.2.2/python/target_selection/config/target_selection.yml
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     9866 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/config/target_selection_v0.yml
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     8761 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/config/xmatch_v0.yml
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     6480 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/config/xmatch_v0p5.yml
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    33349 2024-04-30 18:26:57.000000 sdss_target_selection-1.2.2/python/target_selection/config/xmatch_v1.yml
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     1383 2023-06-01 20:51:59.000000 sdss_target_selection-1.2.2/python/target_selection/exceptions.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     3148 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/mag_flux.py
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-30 18:59:34.242263 sdss_target_selection-1.2.2/python/target_selection/masks/
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     4171 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.2/python/target_selection/masks/AQMES_wboss_imaging_NGC_proc.ply
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     8640 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.2/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.2.1.fits
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     8640 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.3.1.fits
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)    40320 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.2/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.2.1.fits
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    40320 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.3.1.fits
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     8640 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.2/python/target_selection/masks/candidate_target_fields_bhm_rm_v0.2.1.fits
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)   348269 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.2/python/target_selection/masks/rsFields-annotated-lco-deep_proc.ply
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)   135360 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.2/python/target_selection/masks/rsFields_boss_survey.fits
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)    40320 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.2/python/target_selection/masks/rsFields_boss_survey_sgc.fits
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    37638 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.2/python/target_selection/skies.py
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)    10703 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.2/python/target_selection/utils.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    86786 2024-04-30 18:27:11.000000 sdss_target_selection-1.2.2/python/target_selection/xmatch.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     2541 2024-04-30 18:59:34.246263 sdss_target_selection-1.2.2/setup.cfg
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)       73 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.2/setup.py
```

### Comparing `sdss_target_selection-1.2.1/LICENSE.md` & `sdss_target_selection-1.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/PKG-INFO` & `sdss_target_selection-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-target-selection
-Version: 1.2.1
+Version: 1.2.2
 Summary: Code to perform target selection for BHM/MWM using catalogdb
 Home-page: https://github.com/sdss/target_selection
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/target_selection
 Project-URL: Documentation, https://sdss-target-selection.readthedocs.org
```

### Comparing `sdss_target_selection-1.2.1/README.md` & `sdss_target_selection-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/bin/yanny_scraper` & `sdss_target_selection-1.2.2/bin/yanny_scraper`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/PKG-INFO` & `sdss_target_selection-1.2.2/python/sdss_target_selection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-target-selection
-Version: 1.2.1
+Version: 1.2.2
 Summary: Code to perform target selection for BHM/MWM using catalogdb
 Home-page: https://github.com/sdss/target_selection
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/target_selection
 Project-URL: Documentation, https://sdss-target-selection.readthedocs.org
```

### Comparing `sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/SOURCES.txt` & `sdss_target_selection-1.2.2/python/sdss_target_selection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/sdss_target_selection.egg-info/requires.txt` & `sdss_target_selection-1.2.2/python/sdss_target_selection.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/__init__.py` & `sdss_target_selection-1.2.2/python/target_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/__main__.py` & `sdss_target_selection-1.2.2/python/target_selection/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/__init__.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/base.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 from sdssdb.peewee import BaseModel
 from sdssdb.peewee.sdss5db import catalogdb as cdb
 from sdssdb.peewee.sdss5db import targetdb as tdb
 from sdsstools import read_yaml_file
 from sdsstools._vendor.color_print import color_text
 
 from target_selection import __version__, config, log
-from target_selection.exceptions import (TargetSelectionError,
-                                         TargetSelectionUserWarning)
+from target_selection.exceptions import TargetSelectionError
 from target_selection.utils import Timer
 
 
 EPOCH = 2016.0
 
 
 class BaseCarton(metaclass=abc.ABCMeta):
@@ -628,16 +627,15 @@
         n_empty = (Model
                    .select()
                    .where(Model.g.is_null() | Model.r.is_null() | Model.i.is_null())
                    .where(Model.selected >> True)
                    .count())
 
         if n_empty > 0:
-            warnings.warn(f'Found {n_empty} entries with empty magnitudes.',
-                          TargetSelectionUserWarning)
+            log.warning(f'Found {n_empty} entries with empty magnitudes.')
 
     def post_process(self, model, **kwargs):
         """Post-processes the temporary table.
 
         This method provides a framework for applying non-SQL operations on
         carton query. It receives the model for the temporary table and can
         perform any operation on it, including modifying the ``selected``
@@ -807,27 +805,24 @@
             Equivalent to setting ``mode='overwrite'``. This option is deprecated and
             will raise a warning.
 
         """
 
         if overwrite:
             mode = 'overwrite'
-            warnings.warn(
+            log.warning(
                 'The `overwrite` option is deprecated and will be removed in a future version. '
-                'Use `mode="overwrite"` instead.',
-                TargetSelectionUserWarning)
+                'Use `mode="overwrite"` instead.')
 
         if self.check_targets():
             if mode == 'overwrite':
-                warnings.warn(
+                log.warning(
                     f'Carton {self.name!r} with plan {self.plan!r} '
                     f'already has targets loaded. '
-                    'Dropping carton-to-target entries.',
-                    TargetSelectionUserWarning,
-                )
+                    'Dropping carton-to-target entries.')
                 self.drop_carton()
             elif mode == 'append':
                 pass
             elif mode == 'fail':
                 raise TargetSelectionError(
                     f'Found existing targets for '
                     f'carton {self.name!r} with plan '
@@ -845,26 +840,25 @@
             raise TargetSelectionError(
                 f'No temporary table found {self.full}. Did you call run()?'
             )
 
         has_targets = RModel.select().where(RModel.selected >> True).exists()
 
         if not has_targets:
-            warnings.warn('No targets found in intermediate table.',
-                          TargetSelectionUserWarning)
+            log.warning('No targets found in intermediate table.')
 
         with self.database.atomic():
             self.setup_transaction()
             self._create_carton_metadata()
             self._load_targets(RModel)
             self._load_carton_to_target(RModel)
             if self.load_magnitudes:
                 self._load_magnitudes(RModel)
             else:
-                warnings.warn('Skipping magnitude load.', TargetSelectionUserWarning)
+                log.warning('Skipping magnitude load.')
 
             self.log.debug('Committing records and checking constraints.')
 
     def check_targets(self):
         """Check if data has been loaded for this carton and targeting plan."""
 
         has_targets = (
```

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_aqmes.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/bhm_aqmes.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_csc.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/bhm_csc.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_galaxies.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/bhm_galaxies.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_gua.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/bhm_gua.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_rm.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/bhm_rm.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_spiders_agn.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/bhm_spiders_agn.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/bhm_spiders_clusters.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/bhm_spiders_clusters.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/guide.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/guide.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_bin_gaia.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_bin_gaia.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_bin_vis.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_bin_vis.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_cb.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_cb.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_cb_cvcandidates.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_cb_cvcandidates.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_dust.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_dust.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_erosita.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_erosita.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_galactic.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_galactic.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_halo.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_halo.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_halo_gaia_dr3.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_halo_gaia_dr3.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_legacy_ir2opt.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_legacy_ir2opt.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_magcloud_agb.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_magcloud_agb.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_magcloud_rgb.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_magcloud_rgb.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_monitor_apogee.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_monitor_apogee.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_ob.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_ob.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_planet.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_planet.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_rv.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_rv.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_snc.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_snc.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_tess_ob.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_tess_ob.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_tess_rgb.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_tess_rgb.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_wd.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_wd.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/mwm_yso.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/mwm_yso.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/ops_apogee_stds.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/ops_apogee_stds.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/ops_boss_stds.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/ops_boss_stds.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/ops_bright_stars.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/ops_bright_stars.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/ops_skies.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/ops_skies.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/skymask.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/skymask.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/too.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/too.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/cartons/tools.py` & `sdss_target_selection-1.2.2/python/target_selection/cartons/tools.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/config/target_selection.yml` & `sdss_target_selection-1.2.2/python/target_selection/config/target_selection.yml`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/config/target_selection_v0.yml` & `sdss_target_selection-1.2.2/python/target_selection/config/target_selection_v0.yml`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/config/xmatch_v0.yml` & `sdss_target_selection-1.2.2/python/target_selection/config/xmatch_v0.yml`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/config/xmatch_v0p5.yml` & `sdss_target_selection-1.2.2/python/target_selection/config/xmatch_v0p5.yml`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/config/xmatch_v1.yml` & `sdss_target_selection-1.2.2/python/target_selection/config/xmatch_v1.yml`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/exceptions.py` & `sdss_target_selection-1.2.2/python/target_selection/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/mag_flux.py` & `sdss_target_selection-1.2.2/python/target_selection/mag_flux.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/masks/AQMES_wboss_imaging_NGC_proc.ply` & `sdss_target_selection-1.2.2/python/target_selection/masks/AQMES_wboss_imaging_NGC_proc.ply`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.2.1.fits` & `sdss_target_selection-1.2.2/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.2.1.fits`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.3.1.fits` & `sdss_target_selection-1.2.2/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.3.1.fits`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.2.1.fits` & `sdss_target_selection-1.2.2/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.2.1.fits`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.3.1.fits` & `sdss_target_selection-1.2.2/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.3.1.fits`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/masks/candidate_target_fields_bhm_rm_v0.2.1.fits` & `sdss_target_selection-1.2.2/python/target_selection/masks/candidate_target_fields_bhm_rm_v0.2.1.fits`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/masks/rsFields-annotated-lco-deep_proc.ply` & `sdss_target_selection-1.2.2/python/target_selection/masks/rsFields-annotated-lco-deep_proc.ply`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/masks/rsFields_boss_survey.fits` & `sdss_target_selection-1.2.2/python/target_selection/masks/rsFields_boss_survey.fits`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/masks/rsFields_boss_survey_sgc.fits` & `sdss_target_selection-1.2.2/python/target_selection/masks/rsFields_boss_survey_sgc.fits`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/skies.py` & `sdss_target_selection-1.2.2/python/target_selection/skies.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/utils.py` & `sdss_target_selection-1.2.2/python/target_selection/utils.py`

 * *Files identical despite different names*

### Comparing `sdss_target_selection-1.2.1/python/target_selection/xmatch.py` & `sdss_target_selection-1.2.2/python/target_selection/xmatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1749,15 +1749,14 @@
                     ~fn.EXISTS(
                         rel_model_sb.select(SQL('1')).where(
                             rel_model_sb.version_id == self.version_id,
                             rel_model_sb.target_id == model_pk,
                             rel_model_sb.best >> True))))
 
         if rel_model.table_exists():
-            print('Im here', rel_model)
             unmatched = unmatched.where(
                 ~fn.EXISTS(
                     rel_model.select(SQL('1')).where(
                         rel_model.version_id == self.version_id,
                         rel_model.target_id == model_pk,
                         rel_model.best >> True)))
```

### Comparing `sdss_target_selection-1.2.1/setup.cfg` & `sdss_target_selection-1.2.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sdss-target-selection
-version = 1.2.1
+version = 1.2.2
 author = José Sánchez-Gallego
 author_email = gallegoj@uw.edu
 description = Code to perform target selection for BHM/MWM using catalogdb
 url = https://github.com/sdss/target_selection
 project_urls = 
 	Repository = https://github.com/sdss/target_selection
 	Documentation = https://sdss-target-selection.readthedocs.org
```

