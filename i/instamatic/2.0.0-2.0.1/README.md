# Comparing `tmp/instamatic-2.0.0.tar.gz` & `tmp/instamatic-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instamatic-2.0.0.tar", last modified: Fri Jun 23 09:49:20 2023, max compression
+gzip compressed data, was "instamatic-2.0.1.tar", last modified: Tue Apr 30 09:16:16 2024, max compression
```

## Comparing `instamatic-2.0.0.tar` & `instamatic-2.0.1.tar`

### file list

```diff
@@ -1,255 +1,256 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.093809 instamatic-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-23 09:49:10.000000 instamatic-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-23 09:49:10.000000 instamatic-2.0.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-23 09:49:10.000000 instamatic-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-23 09:49:20.093809 instamatic-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-23 09:49:10.000000 instamatic-2.0.0/THANKS.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.049809 instamatic-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)   284790 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/banner.png
--rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/config.md
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/formats.md
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/gui.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/make_programs_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/merlin.md
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/network.md
--rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/programs.md
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/setup.md
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/tem_api.md
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/tvips.md
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-23 09:49:10.000000 instamatic-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-23 09:49:10.000000 instamatic-2.0.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.049809 instamatic-2.0.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/center_images_smv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/diagnose_beam_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/learn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/make_interval_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/make_serialed_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/process_dm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/process_tpx.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/process_tvips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:49:20.093809 instamatic-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.041809 instamatic-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.053809 instamatic-2.0.0/src/instamatic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.057809 instamatic-2.0.0/src/instamatic/TEMController/
--rw-r--r--   0 runner    (1001) docker     (123)    26129 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/TEMController.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/deflectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/fei_microscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/fei_simu_microscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    19456 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/jeol_microscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/lenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/microscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/microscope_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17133 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/simu_microscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/acquire_at_items.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/banner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.057809 instamatic-2.0.0/src/instamatic/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/calibrate_beamshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/calibrate_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/calibrate_directbeam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/calibrate_imageshift12.py
--rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/calibrate_stage_lowmag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/calibrate_stage_mag1.py
--rw-r--r--   0 runner    (1001) docker     (123)    16130 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/calibrate_stagematrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/center_z.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/filenames.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/fit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.065809 instamatic-2.0.0/src/instamatic/camera/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/CCDCOM.h
--rw-r--r--   0 runner    (1001) docker     (123)    22528 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x64_gatan.dll
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x64_simulation.dll
--rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x86_gatan.dll
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x86_simulation.dll
--rw-r--r--   0 runner    (1001) docker     (123)    55808 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/EMCameraObj.dll
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19013 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_emmenu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_gatan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_gatan2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_merlin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_serval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_simu.py
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_timepix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/fakevideostream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/gatansocket3.md
--rw-r--r--   0 runner    (1001) docker     (123)    25990 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/gatansocket3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/merlin_io.py
--rw-r--r--   0 runner    (1001) docker     (123)  1231360 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/mpxhwrelaxd.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/timepix.lockfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.065809 instamatic-2.0.0/src/instamatic/camera/tpx/
--rw-r--r--   0 runner    (1001) docker     (123)   262144 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/tpx/171207_with_flatfield.bpc
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/tpx/171207_with_flatfield.bpc.dacs
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/tpx/HW.dacs
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/tpx/config.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/videostream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.069809 instamatic-2.0.0/src/instamatic/config/
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.069809 instamatic-2.0.0/src/instamatic/config/alignments/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/alignments/neutral.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/autoconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.069809 instamatic-2.0.0/src/instamatic/config/calibration/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/calibration/orius.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/calibration/simulate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/calibration/timepix.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/calibration/tvips-f416.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.069809 instamatic-2.0.0/src/instamatic/config/camera/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/merlin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/orius.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/serval.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/simulate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/simulateDLL.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/timepix.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/tvips-f416.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/tvips-xf416.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/config_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/defaults.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.069809 instamatic-2.0.0/src/instamatic/config/microscope/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/microscope/fei_simu.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/microscope/fei_themisZ.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/microscope/jeol-1400.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/microscope/jeol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/microscope/simulate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/config/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/scripts/close_down.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/scripts/focus_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/scripts/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/scripts/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/scripts/search_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/experiments/autocred/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/autocred/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64494 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/autocred/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/experiments/cred/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/cred/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/cred/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/experiments/cred_gatan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/cred_gatan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15871 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/cred_gatan/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/experiments/cred_tvips/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/cred_tvips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/cred_tvips/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/experiments/red/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/red/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/red/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/experiments/serialed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/serialed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21941 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/serialed/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.077809 instamatic-2.0.0/src/instamatic/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/formats/adscimage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/formats/csvIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    22681 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/formats/mrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/formats/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/formats/xdscbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/goniotool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gridmontage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.081809 instamatic-2.0.0/src/instamatic/gui/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/about_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/autocred_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/console_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/cred_fei_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/cred_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    13899 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/cred_tvips_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/ctrl_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/debug_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/defocus_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/io_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/machine_learning_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/mpl_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/red_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/sed_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/videostream_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/imreg.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/montage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.085809 instamatic-2.0.0/src/instamatic/neural_network/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/neural_network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/neural_network/neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/neural_network/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/neural_network/preprocess_SerialRED.py
--rw-r--r--   0 runner    (1001) docker     (123)  1503408 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/neural_network/weights-py2.p
--rw-r--r--   0 runner    (1001) docker     (123)  1020951 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/neural_network/weights-py3.p
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.089809 instamatic-2.0.0/src/instamatic/processing/
--rw-r--r--   0 runner    (1001) docker     (123)    26808 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/ImgConversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/ImgConversionDM.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/ImgConversionTPX.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/ImgConversionTVIPS.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/XDS_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/XDS_templateDM.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/XDS_templateTPX.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/XDS_templateTVIPS.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/find_crystals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/find_crystals_ilastik.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/find_holes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/flatfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/stretch_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.089809 instamatic-2.0.0/src/instamatic/server/
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/TEMServer_FEI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/cam_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/cam_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/dials_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/goniotool_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/tem_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/tem_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/vm_ubuntu_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/xds_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.089809 instamatic-2.0.0/src/instamatic/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/utils/beamstop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/utils/high_precision_timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/utils/spinbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/utils/xds_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.053809 instamatic-2.0.0/src/instamatic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-23 09:49:20.000000 instamatic-2.0.0/src/instamatic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-06-23 09:49:20.000000 instamatic-2.0.0/src/instamatic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:49:20.000000 instamatic-2.0.0/src/instamatic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-23 09:49:20.000000 instamatic-2.0.0/src/instamatic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-23 09:49:20.000000 instamatic-2.0.0/src/instamatic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 09:49:20.000000 instamatic-2.0.0/src/instamatic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.093809 instamatic-2.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.093809 instamatic-2.0.0/tests/config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.093809 instamatic-2.0.0/tests/config/calibration/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/config/calibration/test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.093809 instamatic-2.0.0/tests/config/camera/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/config/camera/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/config/defaults.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.093809 instamatic-2.0.0/tests/config/microscope/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/config/microscope/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/config/settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/test_ctrl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/test_grid_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/test_merlin_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.610588 instamatic-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 09:16:10.000000 instamatic-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-30 09:16:10.000000 instamatic-2.0.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-30 09:16:10.000000 instamatic-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-30 09:16:16.610588 instamatic-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-30 09:16:10.000000 instamatic-2.0.1/THANKS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.570588 instamatic-2.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 09:16:10.000000 instamatic-2.0.1/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-30 09:16:10.000000 instamatic-2.0.1/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)   284790 2024-04-30 09:16:10.000000 instamatic-2.0.1/docs/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14386 2024-04-30 09:16:10.000000 instamatic-2.0.1/docs/config.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-30 09:16:10.000000 instamatic-2.0.1/docs/formats.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-30 09:16:10.000000 instamatic-2.0.1/docs/gonio.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-30 09:16:10.000000 instamatic-2.0.1/docs/gui.md
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 09:16:10.000000 instamatic-2.0.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-30 09:16:10.000000 instamatic-2.0.1/docs/make_programs_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-30 09:16:10.000000 instamatic-2.0.1/docs/merlin.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-30 09:16:10.000000 instamatic-2.0.1/docs/network.md
+-rw-r--r--   0 runner    (1001) docker     (127)    20578 2024-04-30 09:16:10.000000 instamatic-2.0.1/docs/programs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-30 09:16:10.000000 instamatic-2.0.1/docs/setup.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-04-30 09:16:10.000000 instamatic-2.0.1/docs/tem_api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-30 09:16:10.000000 instamatic-2.0.1/docs/tvips.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-30 09:16:10.000000 instamatic-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-30 09:16:10.000000 instamatic-2.0.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.574588 instamatic-2.0.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:10.000000 instamatic-2.0.1/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-30 09:16:10.000000 instamatic-2.0.1/scripts/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-30 09:16:10.000000 instamatic-2.0.1/scripts/center_images_smv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-30 09:16:10.000000 instamatic-2.0.1/scripts/diagnose_beam_drift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-30 09:16:10.000000 instamatic-2.0.1/scripts/learn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-30 09:16:10.000000 instamatic-2.0.1/scripts/make_interval_movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-30 09:16:10.000000 instamatic-2.0.1/scripts/make_serialed_movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-30 09:16:10.000000 instamatic-2.0.1/scripts/process_dm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-04-30 09:16:10.000000 instamatic-2.0.1/scripts/process_tpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-30 09:16:10.000000 instamatic-2.0.1/scripts/process_tvips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-30 09:16:10.000000 instamatic-2.0.1/scripts/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:16:16.610588 instamatic-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.566588 instamatic-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.574588 instamatic-2.0.1/src/instamatic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.578588 instamatic-2.0.1/src/instamatic/TEMController/
+-rw-r--r--   0 runner    (1001) docker     (127)    26129 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/TEMController/TEMController.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/TEMController/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/TEMController/deflectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15098 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/TEMController/fei_microscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/TEMController/fei_simu_microscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/TEMController/jeol_microscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/TEMController/lenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/TEMController/microscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/TEMController/microscope_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/TEMController/simu_microscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11126 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/TEMController/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/TEMController/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/acquire_at_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.578588 instamatic-2.0.1/src/instamatic/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10802 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/calibrate/calibrate_beamshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/calibrate/calibrate_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/calibrate/calibrate_directbeam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/calibrate/calibrate_imageshift12.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13839 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/calibrate/calibrate_stage_lowmag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/calibrate/calibrate_stage_mag1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/calibrate/calibrate_stagematrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/calibrate/center_z.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/calibrate/filenames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/calibrate/fit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.586588 instamatic-2.0.1/src/instamatic/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/CCDCOM.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22528 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/CCDCOM2_x64_gatan.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    10752 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/CCDCOM2_x64_simulation.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    17920 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/CCDCOM2_x86_gatan.dll
+-rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/CCDCOM2_x86_simulation.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    55808 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/EMCameraObj.dll
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/camera_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19013 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/camera_emmenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/camera_gatan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/camera_gatan2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/camera_merlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/camera_serval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/camera_simu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/camera_timepix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/fakevideostream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/gatansocket3.md
+-rw-r--r--   0 runner    (1001) docker     (127)    25990 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/gatansocket3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/merlin_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1231360 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/mpxhwrelaxd.dll
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/timepix.lockfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.586588 instamatic-2.0.1/src/instamatic/camera/tpx/
+-rw-r--r--   0 runner    (1001) docker     (127)   262144 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/tpx/171207_with_flatfield.bpc
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/tpx/171207_with_flatfield.bpc.dacs
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/tpx/HW.dacs
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/tpx/config.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/camera/videostream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.586588 instamatic-2.0.1/src/instamatic/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.586588 instamatic-2.0.1/src/instamatic/config/alignments/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/alignments/neutral.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/autoconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.586588 instamatic-2.0.1/src/instamatic/config/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/calibration/orius.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/calibration/simulate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/calibration/timepix.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/calibration/tvips-f416.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.590588 instamatic-2.0.1/src/instamatic/config/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/camera/merlin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/camera/orius.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/camera/serval.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/camera/simulate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/camera/simulateDLL.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/camera/timepix.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/camera/tvips-f416.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/camera/tvips-xf416.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/config_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/defaults.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.590588 instamatic-2.0.1/src/instamatic/config/microscope/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/microscope/fei_simu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/microscope/fei_themisZ.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/microscope/jeol-1400.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/microscope/jeol.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/microscope/simulate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.590588 instamatic-2.0.1/src/instamatic/config/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/scripts/close_down.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/scripts/focus_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/scripts/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/scripts/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/scripts/search_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.590588 instamatic-2.0.1/src/instamatic/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.590588 instamatic-2.0.1/src/instamatic/experiments/autocred/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/experiments/autocred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64494 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/experiments/autocred/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.590588 instamatic-2.0.1/src/instamatic/experiments/cred/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/experiments/cred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17207 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/experiments/cred/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.590588 instamatic-2.0.1/src/instamatic/experiments/cred_gatan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/experiments/cred_gatan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15871 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/experiments/cred_gatan/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.594588 instamatic-2.0.1/src/instamatic/experiments/cred_tvips/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/experiments/cred_tvips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20753 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/experiments/cred_tvips/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.594588 instamatic-2.0.1/src/instamatic/experiments/red/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/experiments/red/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/experiments/red/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.594588 instamatic-2.0.1/src/instamatic/experiments/serialed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/experiments/serialed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21941 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/experiments/serialed/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.594588 instamatic-2.0.1/src/instamatic/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/formats/adscimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/formats/csvIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22681 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/formats/mrc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/formats/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/formats/xdscbf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/goniotool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gridmontage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.598588 instamatic-2.0.1/src/instamatic/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/about_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14841 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/autocred_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/console_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/cred_fei_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/cred_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13899 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/cred_tvips_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/ctrl_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/debug_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/defocus_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/io_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/machine_learning_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/mpl_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/red_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/sed_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/gui/videostream_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/imreg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/montage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.598588 instamatic-2.0.1/src/instamatic/neural_network/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/neural_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/neural_network/neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/neural_network/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/neural_network/preprocess_SerialRED.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1503408 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/neural_network/weights-py2.p
+-rw-r--r--   0 runner    (1001) docker     (127)  1020951 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/neural_network/weights-py3.p
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.602588 instamatic-2.0.1/src/instamatic/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)    26808 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/processing/ImgConversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/processing/ImgConversionDM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/processing/ImgConversionTPX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/processing/ImgConversionTVIPS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/processing/XDS_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/processing/XDS_templateDM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/processing/XDS_templateTPX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/processing/XDS_templateTVIPS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/processing/find_crystals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/processing/find_crystals_ilastik.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6409 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/processing/find_holes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/processing/flatfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/processing/stretch_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.606588 instamatic-2.0.1/src/instamatic/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/server/TEMServer_FEI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/server/cam_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/server/cam_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/server/dials_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/server/goniotool_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/server/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/server/tem_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/server/tem_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/server/vm_ubuntu_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/server/xds_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.606588 instamatic-2.0.1/src/instamatic/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/utils/beamstop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/utils/high_precision_timers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/utils/spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-30 09:16:10.000000 instamatic-2.0.1/src/instamatic/utils/xds_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.610588 instamatic-2.0.1/src/instamatic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-30 09:16:16.000000 instamatic-2.0.1/src/instamatic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-04-30 09:16:16.000000 instamatic-2.0.1/src/instamatic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:16:16.000000 instamatic-2.0.1/src/instamatic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-30 09:16:16.000000 instamatic-2.0.1/src/instamatic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-30 09:16:16.000000 instamatic-2.0.1/src/instamatic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 09:16:16.000000 instamatic-2.0.1/src/instamatic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.610588 instamatic-2.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.610588 instamatic-2.0.1/tests/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.610588 instamatic-2.0.1/tests/config/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-30 09:16:10.000000 instamatic-2.0.1/tests/config/calibration/test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.610588 instamatic-2.0.1/tests/config/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-30 09:16:10.000000 instamatic-2.0.1/tests/config/camera/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-30 09:16:10.000000 instamatic-2.0.1/tests/config/defaults.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:16:16.610588 instamatic-2.0.1/tests/config/microscope/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-30 09:16:10.000000 instamatic-2.0.1/tests/config/microscope/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-30 09:16:10.000000 instamatic-2.0.1/tests/config/settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-30 09:16:10.000000 instamatic-2.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-30 09:16:10.000000 instamatic-2.0.1/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-30 09:16:10.000000 instamatic-2.0.1/tests/test_ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-30 09:16:10.000000 instamatic-2.0.1/tests/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-30 09:16:10.000000 instamatic-2.0.1/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-30 09:16:10.000000 instamatic-2.0.1/tests/test_grid_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-30 09:16:10.000000 instamatic-2.0.1/tests/test_merlin_io.py
```

### Comparing `instamatic-2.0.0/.pre-commit-config.yaml` & `instamatic-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/LICENCE` & `instamatic-2.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/MANIFEST.in` & `instamatic-2.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/THANKS.md` & `instamatic-2.0.1/THANKS.md`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/docs/banner.png` & `instamatic-2.0.1/docs/banner.png`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/docs/config.md` & `instamatic-2.0.1/docs/config.md`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/docs/formats.md` & `instamatic-2.0.1/docs/formats.md`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/docs/gui.md` & `instamatic-2.0.1/docs/gui.md`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/docs/make_programs_md.py` & `instamatic-2.0.1/docs/make_programs_md.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/docs/merlin.md` & `instamatic-2.0.1/docs/merlin.md`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/docs/network.md` & `instamatic-2.0.1/docs/network.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 cam_server_host: 10.0.0.12
 cam_server_port: 8088
 
 use_cam_server: False
 ```
 
 
-## Example 3
+## Example 2
 
 This is an example where the microscope and camera PCs should be controlled through an intermediate support PC.
 
 If your camera can be controlled directly through TCP/IP, such as the MerlinEM or ASI Cheetah (via `serval`), do not use `instamatic.camserver`, but connect directly to the IP. For example, for Merlin.
 
 1. Start Merlin software first
 2. Run `instamatic.temserver` on the Microscope PC
@@ -56,15 +56,15 @@
 
 ```yaml title="settings.yaml"
 use_tem_server: True
 tem_server_host: 10.0.0.20
 tem_server_port: 8088
 ```
 
-```yaml title = "camera/merlin.yaml"
+```yaml title="camera/merlin.yaml"
 host: 10.0.0.30
 ```
 
 On the Microscope PC:
 
 ```yaml title="settings.yaml"
 cam_server_host: 0.0.0.0
```

### Comparing `instamatic-2.0.0/docs/programs.md` & `instamatic-2.0.1/docs/programs.md`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/docs/setup.md` & `instamatic-2.0.1/docs/setup.md`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/docs/tem_api.md` & `instamatic-2.0.1/docs/tem_api.md`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/docs/tvips.md` & `instamatic-2.0.1/docs/tvips.md`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/pyproject.toml` & `instamatic-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 [project]
 name = "instamatic"
-version = "2.0.0"
+version = "2.0.1"
 description = "Python program for automated electron diffraction data collection"
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
 	{name = "Stef Smeets", email = "s.smeets@esciencecenter.nl"},
 ]
 keywords = [
```

### Comparing `instamatic-2.0.0/scripts/browser.py` & `instamatic-2.0.1/scripts/browser.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/scripts/center_images_smv.py` & `instamatic-2.0.1/scripts/center_images_smv.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/scripts/diagnose_beam_drift.py` & `instamatic-2.0.1/scripts/diagnose_beam_drift.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/scripts/learn.py` & `instamatic-2.0.1/scripts/learn.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/scripts/make_interval_movie.py` & `instamatic-2.0.1/scripts/make_interval_movie.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/scripts/make_serialed_movie.py` & `instamatic-2.0.1/scripts/make_serialed_movie.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/scripts/process_dm.py` & `instamatic-2.0.1/scripts/process_dm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 from pathlib import Path
 
 import numpy as np
+from skimage.exposure import rescale_intensity
 from PIL import Image
 
 from instamatic.processing.ImgConversionDM import ImgConversionDM as ImgConversion
 
 # Script to process cRED data collecting using the DigitalMicrograph script `insteaDMatic`
 # https://github.com/instamatic-dev/InsteaDMatic
 #
@@ -117,21 +118,24 @@
         p = Path(s)
         return int(p.stem.split('_')[-1])
 
     for i, fn in enumerate(image_fns):
         j = extract_image_number(fn)
         img = np.array(Image.open(fn))
 
-        if img.dtype != np.uint16:
-            # cast to 16 bit uint16
-            img = (2**16 - 1) * (img - img.min()) / (img.max() - img.min())
-
         h = {'ImageGetTime': timestamp, 'ImageExposureTime': exposure_time}
         buffer.append((j, img, h))
 
+    if img.dtype != np.uint16:
+        max_val = max(img.max() for _, img, _ in buffer)
+        min_val = min(img.min() for _, img, _ in buffer)
+        for item in buffer:
+            # cast to 16 bit uint16
+            item[1] = rescale_intensity(item[1], out_range='uint16', in_range=(min_val, max_val))
+
     img_conv = ImgConversion(buffer=buffer,
                              osc_angle=osc_angle,
                              start_angle=start_angle,
                              end_angle=end_angle,
                              rotation_axis=rotation_axis,
                              acquisition_time=acquisition_time,
                              flatfield=None,
```

### Comparing `instamatic-2.0.0/scripts/process_tpx.py` & `instamatic-2.0.1/scripts/process_tpx.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/scripts/process_tvips.py` & `instamatic-2.0.1/scripts/process_tvips.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/scripts/viewer.py` & `instamatic-2.0.1/scripts/viewer.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/TEMController/TEMController.py` & `instamatic-2.0.1/src/instamatic/TEMController/TEMController.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/TEMController/deflectors.py` & `instamatic-2.0.1/src/instamatic/TEMController/deflectors.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/TEMController/fei_microscope.py` & `instamatic-2.0.1/src/instamatic/TEMController/fei_microscope.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/TEMController/fei_simu_microscope.py` & `instamatic-2.0.1/src/instamatic/TEMController/fei_simu_microscope.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/TEMController/jeol_microscope.py` & `instamatic-2.0.1/src/instamatic/TEMController/jeol_microscope.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/TEMController/lenses.py` & `instamatic-2.0.1/src/instamatic/TEMController/lenses.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/TEMController/microscope.py` & `instamatic-2.0.1/src/instamatic/TEMController/microscope.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/TEMController/microscope_client.py` & `instamatic-2.0.1/src/instamatic/TEMController/microscope_client.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/TEMController/simu_microscope.py` & `instamatic-2.0.1/src/instamatic/TEMController/simu_microscope.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/TEMController/stage.py` & `instamatic-2.0.1/src/instamatic/TEMController/stage.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/TEMController/states.py` & `instamatic-2.0.1/src/instamatic/TEMController/states.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/__init__.py` & `instamatic-2.0.1/src/instamatic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #   | | '_ \/ __| __/ _` | '_ ` _ \ / _` | __| |/ __|   #
 #   | | | | \__ \ || (_| | | | | | | (_| | |_| | (__    #
 #   |_|_| |_|___/\__\__,_|_| |_| |_|\__,_|\__|_|\___|   #
 #                                                       #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 """
 
-__version__ = '2.0.0'
+__version__ = '2.0.1'
 __title__ = 'instamatic'
 __long_title__ = f'{__title__} v{__version__}'
 __author__ = 'Stef Smeets'
 __author_email__ = 's.smeets@esciencecenter.nl'
 __description__ = 'Python program for automated serial electron diffraction data collection'
 __license__ = 'GPLv3'
 __url__ = 'https://github.com/instamatic-dev/instamatic'
```

### Comparing `instamatic-2.0.0/src/instamatic/acquire_at_items.py` & `instamatic-2.0.1/src/instamatic/acquire_at_items.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/banner.py` & `instamatic-2.0.1/src/instamatic/banner.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/browser.py` & `instamatic-2.0.1/src/instamatic/browser.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/calibrate/calibrate_beamshift.py` & `instamatic-2.0.1/src/instamatic/calibrate/calibrate_beamshift.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/calibrate/calibrate_brightness.py` & `instamatic-2.0.1/src/instamatic/calibrate/calibrate_brightness.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/calibrate/calibrate_directbeam.py` & `instamatic-2.0.1/src/instamatic/calibrate/calibrate_directbeam.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/calibrate/calibrate_imageshift12.py` & `instamatic-2.0.1/src/instamatic/calibrate/calibrate_imageshift12.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/calibrate/calibrate_stage_lowmag.py` & `instamatic-2.0.1/src/instamatic/calibrate/calibrate_stage_lowmag.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/calibrate/calibrate_stage_mag1.py` & `instamatic-2.0.1/src/instamatic/calibrate/calibrate_stage_mag1.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/calibrate/calibrate_stagematrix.py` & `instamatic-2.0.1/src/instamatic/calibrate/calibrate_stagematrix.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/calibrate/center_z.py` & `instamatic-2.0.1/src/instamatic/calibrate/center_z.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/calibrate/fit.py` & `instamatic-2.0.1/src/instamatic/calibrate/fit.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/CCDCOM.h` & `instamatic-2.0.1/src/instamatic/camera/CCDCOM.h`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x64_gatan.dll` & `instamatic-2.0.1/src/instamatic/camera/CCDCOM2_x64_gatan.dll`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x64_simulation.dll` & `instamatic-2.0.1/src/instamatic/camera/CCDCOM2_x64_simulation.dll`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x86_gatan.dll` & `instamatic-2.0.1/src/instamatic/camera/CCDCOM2_x86_gatan.dll`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x86_simulation.dll` & `instamatic-2.0.1/src/instamatic/camera/CCDCOM2_x86_simulation.dll`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/EMCameraObj.dll` & `instamatic-2.0.1/src/instamatic/camera/EMCameraObj.dll`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/camera.py` & `instamatic-2.0.1/src/instamatic/camera/camera.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/camera_client.py` & `instamatic-2.0.1/src/instamatic/camera/camera_client.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/camera_emmenu.py` & `instamatic-2.0.1/src/instamatic/camera/camera_emmenu.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/camera_gatan.py` & `instamatic-2.0.1/src/instamatic/camera/camera_gatan.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/camera_gatan2.py` & `instamatic-2.0.1/src/instamatic/camera/camera_gatan2.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/camera_merlin.py` & `instamatic-2.0.1/src/instamatic/camera/camera_merlin.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/camera_serval.py` & `instamatic-2.0.1/src/instamatic/camera/camera_serval.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/camera_simu.py` & `instamatic-2.0.1/src/instamatic/camera/camera_simu.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/camera_timepix.py` & `instamatic-2.0.1/src/instamatic/camera/camera_timepix.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/fakevideostream.py` & `instamatic-2.0.1/src/instamatic/camera/fakevideostream.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/gatansocket3.md` & `instamatic-2.0.1/src/instamatic/camera/gatansocket3.md`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/gatansocket3.py` & `instamatic-2.0.1/src/instamatic/camera/gatansocket3.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/merlin_io.py` & `instamatic-2.0.1/src/instamatic/camera/merlin_io.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/mpxhwrelaxd.dll` & `instamatic-2.0.1/src/instamatic/camera/mpxhwrelaxd.dll`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/tpx/171207_with_flatfield.bpc` & `instamatic-2.0.1/src/instamatic/camera/tpx/171207_with_flatfield.bpc`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/tpx/171207_with_flatfield.bpc.dacs` & `instamatic-2.0.1/src/instamatic/camera/tpx/171207_with_flatfield.bpc.dacs`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/camera/videostream.py` & `instamatic-2.0.1/src/instamatic/camera/videostream.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/__init__.py` & `instamatic-2.0.1/src/instamatic/config/__init__.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/autoconfig.py` & `instamatic-2.0.1/src/instamatic/config/autoconfig.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/calibration/orius.yaml` & `instamatic-2.0.1/src/instamatic/config/calibration/orius.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/calibration/simulate.yaml` & `instamatic-2.0.1/src/instamatic/config/calibration/simulate.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/calibration/timepix.yaml` & `instamatic-2.0.1/src/instamatic/config/calibration/timepix.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/calibration/tvips-f416.yaml` & `instamatic-2.0.1/src/instamatic/config/calibration/tvips-f416.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/camera/serval.yaml` & `instamatic-2.0.1/src/instamatic/config/camera/serval.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/config_updater.py` & `instamatic-2.0.1/src/instamatic/config/config_updater.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/microscope/fei_simu.yaml` & `instamatic-2.0.1/src/instamatic/config/microscope/fei_simu.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/microscope/fei_themisZ.yaml` & `instamatic-2.0.1/src/instamatic/config/microscope/fei_themisZ.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/microscope/jeol-1400.yaml` & `instamatic-2.0.1/src/instamatic/config/microscope/jeol-1400.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/microscope/jeol.yaml` & `instamatic-2.0.1/src/instamatic/config/microscope/jeol.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/microscope/simulate.yaml` & `instamatic-2.0.1/src/instamatic/config/microscope/simulate.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/scripts/readme.md` & `instamatic-2.0.1/src/instamatic/config/scripts/readme.md`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/settings.yaml` & `instamatic-2.0.1/src/instamatic/config/settings.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/config/utils.py` & `instamatic-2.0.1/src/instamatic/config/utils.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/exceptions.py` & `instamatic-2.0.1/src/instamatic/exceptions.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/experiments/autocred/experiment.py` & `instamatic-2.0.1/src/instamatic/experiments/autocred/experiment.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/experiments/cred/experiment.py` & `instamatic-2.0.1/src/instamatic/experiments/cred/experiment.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/experiments/cred_gatan/experiment.py` & `instamatic-2.0.1/src/instamatic/experiments/cred_gatan/experiment.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/experiments/cred_tvips/experiment.py` & `instamatic-2.0.1/src/instamatic/experiments/cred_tvips/experiment.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/experiments/red/experiment.py` & `instamatic-2.0.1/src/instamatic/experiments/red/experiment.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/experiments/serialed/experiment.py` & `instamatic-2.0.1/src/instamatic/experiments/serialed/experiment.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/formats/__init__.py` & `instamatic-2.0.1/src/instamatic/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/formats/adscimage.py` & `instamatic-2.0.1/src/instamatic/formats/adscimage.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/formats/csvIO.py` & `instamatic-2.0.1/src/instamatic/formats/csvIO.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/formats/mrc.py` & `instamatic-2.0.1/src/instamatic/formats/mrc.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/formats/util.py` & `instamatic-2.0.1/src/instamatic/formats/util.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/formats/xdscbf.py` & `instamatic-2.0.1/src/instamatic/formats/xdscbf.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/goniotool.py` & `instamatic-2.0.1/src/instamatic/goniotool.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gridmontage.py` & `instamatic-2.0.1/src/instamatic/gridmontage.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/about_frame.py` & `instamatic-2.0.1/src/instamatic/gui/about_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/autocred_frame.py` & `instamatic-2.0.1/src/instamatic/gui/autocred_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/base_module.py` & `instamatic-2.0.1/src/instamatic/gui/base_module.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/console_frame.py` & `instamatic-2.0.1/src/instamatic/gui/console_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/cred_fei_frame.py` & `instamatic-2.0.1/src/instamatic/gui/cred_fei_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/cred_frame.py` & `instamatic-2.0.1/src/instamatic/gui/cred_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/cred_tvips_frame.py` & `instamatic-2.0.1/src/instamatic/gui/cred_tvips_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/ctrl_frame.py` & `instamatic-2.0.1/src/instamatic/gui/ctrl_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/debug_frame.py` & `instamatic-2.0.1/src/instamatic/gui/debug_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/defocus_button.py` & `instamatic-2.0.1/src/instamatic/gui/defocus_button.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/gui.py` & `instamatic-2.0.1/src/instamatic/gui/gui.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/io_frame.py` & `instamatic-2.0.1/src/instamatic/gui/io_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/jobs.py` & `instamatic-2.0.1/src/instamatic/gui/jobs.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/machine_learning_frame.py` & `instamatic-2.0.1/src/instamatic/gui/machine_learning_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/modules.py` & `instamatic-2.0.1/src/instamatic/gui/modules.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/mpl_frame.py` & `instamatic-2.0.1/src/instamatic/gui/mpl_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/red_frame.py` & `instamatic-2.0.1/src/instamatic/gui/red_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/sed_frame.py` & `instamatic-2.0.1/src/instamatic/gui/sed_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/gui/videostream_frame.py` & `instamatic-2.0.1/src/instamatic/gui/videostream_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/image_utils.py` & `instamatic-2.0.1/src/instamatic/image_utils.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/imreg.py` & `instamatic-2.0.1/src/instamatic/imreg.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/io.py` & `instamatic-2.0.1/src/instamatic/io.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/main.py` & `instamatic-2.0.1/src/instamatic/main.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/montage.py` & `instamatic-2.0.1/src/instamatic/montage.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/neural_network/neural_network.py` & `instamatic-2.0.1/src/instamatic/neural_network/neural_network.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/neural_network/preprocess.py` & `instamatic-2.0.1/src/instamatic/neural_network/preprocess.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/neural_network/preprocess_SerialRED.py` & `instamatic-2.0.1/src/instamatic/neural_network/preprocess_SerialRED.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/neural_network/weights-py2.p` & `instamatic-2.0.1/src/instamatic/neural_network/weights-py2.p`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/neural_network/weights-py3.p` & `instamatic-2.0.1/src/instamatic/neural_network/weights-py3.p`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/processing/ImgConversion.py` & `instamatic-2.0.1/src/instamatic/processing/ImgConversion.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/processing/ImgConversionDM.py` & `instamatic-2.0.1/src/instamatic/processing/ImgConversionDM.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/processing/ImgConversionTPX.py` & `instamatic-2.0.1/src/instamatic/processing/ImgConversionTPX.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/processing/ImgConversionTVIPS.py` & `instamatic-2.0.1/src/instamatic/processing/ImgConversionTVIPS.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/processing/XDS_template.py` & `instamatic-2.0.1/src/instamatic/processing/XDS_template.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/processing/XDS_templateDM.py` & `instamatic-2.0.1/src/instamatic/processing/XDS_templateDM.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/processing/XDS_templateTPX.py` & `instamatic-2.0.1/src/instamatic/processing/XDS_templateTPX.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/processing/XDS_templateTVIPS.py` & `instamatic-2.0.1/src/instamatic/processing/XDS_templateTVIPS.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/processing/find_crystals.py` & `instamatic-2.0.1/src/instamatic/processing/find_crystals.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/processing/find_crystals_ilastik.py` & `instamatic-2.0.1/src/instamatic/processing/find_crystals_ilastik.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/processing/find_holes.py` & `instamatic-2.0.1/src/instamatic/processing/find_holes.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/processing/flatfield.py` & `instamatic-2.0.1/src/instamatic/processing/flatfield.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/processing/stretch_correction.py` & `instamatic-2.0.1/src/instamatic/processing/stretch_correction.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/server/TEMServer_FEI.py` & `instamatic-2.0.1/src/instamatic/server/TEMServer_FEI.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/server/cam_server.py` & `instamatic-2.0.1/src/instamatic/server/cam_server.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/server/dials_server.py` & `instamatic-2.0.1/src/instamatic/server/dials_server.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/server/goniotool_server.py` & `instamatic-2.0.1/src/instamatic/server/goniotool_server.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/server/serializer.py` & `instamatic-2.0.1/src/instamatic/server/serializer.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/server/tem_server.py` & `instamatic-2.0.1/src/instamatic/server/tem_server.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/server/vm_ubuntu_server.py` & `instamatic-2.0.1/src/instamatic/server/vm_ubuntu_server.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/server/xds_server.py` & `instamatic-2.0.1/src/instamatic/server/xds_server.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/tools.py` & `instamatic-2.0.1/src/instamatic/tools.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/utils/beamstop.py` & `instamatic-2.0.1/src/instamatic/utils/beamstop.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/utils/high_precision_timers.py` & `instamatic-2.0.1/src/instamatic/utils/high_precision_timers.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/utils/progress.py` & `instamatic-2.0.1/src/instamatic/utils/progress.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/utils/spinbox.py` & `instamatic-2.0.1/src/instamatic/utils/spinbox.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic/utils/xds_parser.py` & `instamatic-2.0.1/src/instamatic/utils/xds_parser.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/src/instamatic.egg-info/SOURCES.txt` & `instamatic-2.0.1/src/instamatic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 pyproject.toml
 requirements.txt
 docs/CODE_OF_CONDUCT.md
 docs/CONTRIBUTING.md
 docs/banner.png
 docs/config.md
 docs/formats.md
+docs/gonio.md
 docs/gui.md
 docs/index.md
 docs/make_programs_md.py
 docs/merlin.md
 docs/network.md
 docs/programs.md
 docs/setup.md
```

### Comparing `instamatic-2.0.0/src/instamatic.egg-info/entry_points.txt` & `instamatic-2.0.1/src/instamatic.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/tests/config/calibration/test.yaml` & `instamatic-2.0.1/tests/config/calibration/test.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/tests/config/microscope/test.yaml` & `instamatic-2.0.1/tests/config/microscope/test.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/tests/test_ctrl.py` & `instamatic-2.0.1/tests/test_ctrl.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/tests/test_experiments.py` & `instamatic-2.0.1/tests/test_experiments.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/tests/test_formats.py` & `instamatic-2.0.1/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `instamatic-2.0.0/tests/test_merlin_io.py` & `instamatic-2.0.1/tests/test_merlin_io.py`

 * *Files identical despite different names*

