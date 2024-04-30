# Comparing `tmp/regional_mom6-0.5.0.tar.gz` & `tmp/regional_mom6-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regional_mom6-0.5.0.tar", last modified: Tue Apr 16 09:17:49 2024, max compression
+gzip compressed data, was "regional_mom6-0.5.1.tar", last modified: Tue Apr 30 13:06:49 2024, max compression
```

## Comparing `regional_mom6-0.5.0.tar` & `regional_mom6-0.5.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/
-drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.952148 regional_mom6-0.5.0/.github/
-drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.952148 regional_mom6-0.5.0/.github/workflows/
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     2024 2024-04-16 09:17:39.000000 regional_mom6-0.5.0/.github/workflows/testing.yml
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      142 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/.gitignore
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      567 2023-09-06 00:16:41.000000 regional_mom6-0.5.0/.readthedocs.yaml
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     1063 2023-09-06 00:16:41.000000 regional_mom6-0.5.0/LICENSE
--rw-r--r--   0 angusgibson  (1001) angusgibson  (1002)      504 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/PKG-INFO
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     7170 2024-04-16 09:16:37.000000 regional_mom6-0.5.0/README.md
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      306 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/codecov.yml
-drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.952148 regional_mom6-0.5.0/demos/
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)   152481 2024-04-16 09:16:37.000000 regional_mom6-0.5.0/demos/access_om2-forced.ipynb
-drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.952148 regional_mom6-0.5.0/demos/premade_run_directories/
-drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/demos/premade_run_directories/common_files/
--rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)    44918 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/MOM_input
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     2039 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/MOM_layout
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)       67 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/MOM_override
--rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)     1321 2024-04-16 09:16:37.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/SIS_input
--rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)      426 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/config.yaml
--rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)      912 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/data_table
--rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)     3255 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/diag_table
--rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)       64 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/field_table
--rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)     1398 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/input.nml
-drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/demos/premade_run_directories/era5_surface/
--rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)     1264 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/era5_surface/data_table
--rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)     1436 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/era5_surface/input.nml
-drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/demos/premade_run_directories/jra_surface/
--rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)      455 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/jra_surface/config.yaml
--rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)     1340 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/jra_surface/data_table
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      427 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/demos/premade_run_directories/readme_premade_rundirs.md
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)    14957 2024-04-16 09:16:37.000000 regional_mom6-0.5.0/demos/reanalysis-forced.ipynb
-drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/docs/
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      634 2023-09-06 00:16:41.000000 regional_mom6-0.5.0/docs/Makefile
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      312 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/docs/api.rst
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      896 2024-02-23 03:07:30.000000 regional_mom6-0.5.0/docs/conf.py
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     1997 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/docs/contributing.md
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      164 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/docs/demos.rst
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      441 2024-02-21 06:00:04.000000 regional_mom6-0.5.0/docs/index.rst
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     1899 2024-04-16 09:16:37.000000 regional_mom6-0.5.0/docs/installation.md
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)       47 2024-02-23 03:07:30.000000 regional_mom6-0.5.0/docs/requirements.txt
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)       74 2024-02-23 03:07:30.000000 regional_mom6-0.5.0/environment-ci.yml
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      870 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/pyproject.toml
-drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/regional_mom6/
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      129 2023-09-06 00:16:41.000000 regional_mom6-0.5.0/regional_mom6/__init__.py
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      411 2024-04-16 09:17:49.000000 regional_mom6-0.5.0/regional_mom6/_version.py
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)    81967 2024-04-16 09:16:37.000000 regional_mom6-0.5.0/regional_mom6/regional_mom6.py
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     6373 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/regional_mom6/utils.py
-drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/regional_mom6.egg-info/
--rw-r--r--   0 angusgibson  (1001) angusgibson  (1002)      504 2024-04-16 09:17:49.000000 regional_mom6-0.5.0/regional_mom6.egg-info/PKG-INFO
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     1458 2024-04-16 09:17:49.000000 regional_mom6-0.5.0/regional_mom6.egg-info/SOURCES.txt
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)        1 2024-04-16 09:17:49.000000 regional_mom6-0.5.0/regional_mom6.egg-info/dependency_links.txt
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      110 2024-04-16 09:17:49.000000 regional_mom6-0.5.0/regional_mom6.egg-info/requires.txt
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)       14 2024-04-16 09:17:49.000000 regional_mom6-0.5.0/regional_mom6.egg-info/top_level.txt
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)       38 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/setup.cfg
-drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/tests/
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)    12071 2024-04-16 09:16:37.000000 regional_mom6-0.5.0/tests/test_expt_class.py
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     4674 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/tests/test_grid_generation.py
--rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     1212 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.756345 regional_mom6-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.748345 regional_mom6-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.752345 regional_mom6-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/.github/workflows/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-30 13:06:49.756345 regional_mom6-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7821 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.752345 regional_mom6-0.5.1/demos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.752345 regional_mom6-0.5.1/demos/premade_run_directories/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.752345 regional_mom6-0.5.1/demos/premade_run_directories/common_files/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44918 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/MOM_input
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/MOM_layout
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/MOM_override
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1321 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/SIS_input
+-rwxr-xr-x   0 runner    (1001) docker     (127)      426 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      912 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/data_table
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3255 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/diag_table
+-rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/field_table
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1398 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/input.nml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.752345 regional_mom6-0.5.1/demos/premade_run_directories/era5_surface/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1264 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/era5_surface/data_table
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1436 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/era5_surface/input.nml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.752345 regional_mom6-0.5.1/demos/premade_run_directories/jra_surface/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/jra_surface/config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1340 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/jra_surface/data_table
+-rw-r--r--   0 runner    (1001) docker     (127)   121257 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/reanalysis-forced.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.756345 regional_mom6-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/demos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/mom6-file-structure-primer.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.756345 regional_mom6-0.5.1/regional_mom6/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/regional_mom6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 13:06:49.000000 regional_mom6-0.5.1/regional_mom6/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83821 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/regional_mom6/regional_mom6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/regional_mom6/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.756345 regional_mom6-0.5.1/regional_mom6.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-30 13:06:49.000000 regional_mom6-0.5.1/regional_mom6.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-30 13:06:49.000000 regional_mom6-0.5.1/regional_mom6.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:06:49.000000 regional_mom6-0.5.1/regional_mom6.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 13:06:49.000000 regional_mom6-0.5.1/regional_mom6.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 13:06:49.000000 regional_mom6-0.5.1/regional_mom6.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:06:49.756345 regional_mom6-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.756345 regional_mom6-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/tests/test_expt_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/tests/test_grid_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/tests/test_utils.py
```

### Comparing `regional_mom6-0.5.0/.github/workflows/testing.yml` & `regional_mom6-0.5.1/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.0/.readthedocs.yaml` & `regional_mom6-0.5.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.0/LICENSE` & `regional_mom6-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.0/README.md` & `regional_mom6-0.5.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,112 +1,131 @@
-# regional_mom6
+# regional-mom6
 
-*Python package for automatic generation of regional configurations for the [Modular Ocean Model 6](https://github.com/mom-ocean/MOM6).*
+*Python package for automatic generation of regional configurations for the [Modular Ocean Model version 6](https://github.com/mom-ocean/MOM6) (MOM6)*
 
 [![Repo status](https://www.repostatus.org/badges/latest/active.svg?style=flat-square)](https://www.repostatus.org/#active)
 [![conda forge](https://img.shields.io/conda/vn/conda-forge/regional-mom6.svg)](https://anaconda.org/conda-forge/regional-mom6)
 [![pypi](https://badge.fury.io/py/regional-mom6.svg)](https://badge.fury.io/py/regional-mom6)
+[![status](https://joss.theoj.org/papers/d396435c09aae4c2f4b62cdbc1493c1e/status.svg)](https://joss.theoj.org/papers/d396435c09aae4c2f4b62cdbc1493c1e)
+[![Documentation Status](https://readthedocs.org/projects/regional-mom6/badge/?version=latest)](https://regional-mom6.readthedocs.io/en/latest/?badge=latest)
+
 [![License](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](https://mit-license.org)
 [![codecov](https://codecov.io/gh/COSIMA/regional-mom6/branch/main/graph/badge.svg?token=7OEZ1UZRY4)](https://codecov.io/gh/COSIMA/regional-mom6)
-[![Documentation Status](https://readthedocs.org/projects/regional-mom6/badge/?version=latest)](https://regional-mom6.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Users just need to provide some information about where, when, and how big their domain is and also where raw input forcing files are. The package sorts out all the boring details and creates a set of MOM6-friendly input files along with setup directories ready to go! 
 
 The idea behind this package is that it should let the user sidestep some of the tricky issues with getting the model to run in the first place. This removes some of the steep learning curve for people new to working with MOM6. Note that the resultant model configuration might still need some tweaking (e.g., fiddling with timestep to avoid CFL-related numerical stability issues or fiddling with bathymetry to deal with very narrow fjords or channels that may exist).
 
-Limitations: Currently the package supports only one horizontal grid type (that is equally spaced in longitude); there are plans to add more grid options. We have designed the package in a way that it is modular so, for example, one needs to implement just another method for a different type of grid and the rest should be good to go.
 
-If you find this package useful and have any suggestions please feel free to open an [issue](https://github.com/COSIMA/regional-mom6/issues) or a [discussion](https://github.com/COSIMA/regional-mom6/discussions). We'd love to have [new contributors](https://regional-mom6.readthedocs.io/en/latest/contributing.html) and we are very keen to help you out along the way!
+## Features
+
+- Automatic grid generation at chosen vertical and horizontal grid spacing.
+- Automatic removal of non-advective cells from the bathymetry that cause the model to crash.
+- Handle slicing across 'seams' in of the forcing input datasets (e.g., when the regional
+  configuration includes longitude 180 and the forcing longitude is defined in [-180, 180]).
+- Handles metadata encoding.
+- Creates directory structure with the configuration files as expected by MOM6.
+- Handles interpolation and interpretation of input data. No pre-processing of forcing datasets is required. (In some cases, slicing the forcing dataset before helps with hitting limitations related to the machine's available memory.)
+
+## Limitations
+
+- Only generates regional horizontal grids with uniform spacing in longitude and latitude.
+  However, users can provide their own non-uniform grid, or ideally
+  [open a pull request](https://github.com/COSIMA/regional-mom6/pulls) with a method that
+  generates other types of horizontal grids.
+- Only supports boundary segments that are parallel to either lines of constant longitude or
+  lines of constant latitude.
+
+
+## We want to hear from you
+
+If you have any suggestions please feel free to open an [issue](https://github.com/COSIMA/regional-mom6/issues) or start a [discussion](https://github.com/COSIMA/regional-mom6/discussions). We welcome any [new contributors](https://regional-mom6.readthedocs.io/en/latest/contributing.html) and we are very keen to help you out along the way!
+
 
 ## What you need to get started:
+
 1. a cool idea for a new regional MOM6 domain,
 2. a working MOM6 executable on a machine of your choice, 
 3. a bathymetry file that at least covers your domain,
 4. 3D ocean forcing files *of any resolution* on your choice of A, B, or C Arakawa grid,
 5. surface forcing files (e.g., from ERA or JRA reanalysis), and
 6. [GFDL's FRE tools](https://github.com/NOAA-GFDL/FRE-NCtools) be downloaded and compiled on the machine you are using.
 
 Check out the [documentation](https://regional-mom6.readthedocs.io/en/latest/) and browse through the [demos](https://regional-mom6.readthedocs.io/en/latest/demos.html).
 
+
 ## Installation
 
-#### Easy, clean, one liner
+We encourage creating a new or using an existing conda environment.
 
-The easiest way is to install `regional-mom6` via [`conda`](https://anaconda.org/conda-forge/regional-mom6).
-We encourage creating a new or using an existing conda environment and then simply
+#### Easy, clean, one liner via conda
+
+The easiest way to install `regional-mom6` is via [`conda`](https://anaconda.org/conda-forge/regional-mom6).
 
 ```bash
 conda install conda-forge::regional-mom6
 ```
 
 That's it -- now enjoy!
 
-#### "*But I want `pip`, can't I install with `pip`*?"
+#### "*But I want pip, can't I install with pip*?"
 
-We can install via `pip` but it's a bit more cumbersome.
-Again, we encourage creating a new or using an existing conda environment.
+To install via `pip` is a bit more cumbersome.
 
-A prerequisite is the binary `esmpy` dependency, which provides regridding capabilities.
+A prerequisite is the binary `esmpy` dependency, which provides re-gridding capabilities.
 The easiest way to install `esmpy` is via conda:
 
 ```bash
 conda install -c conda-forge esmpy
 ```
 
 Alternatively, to install `esmpy` in a Conda-free way, follow the instructions for [installing ESMPy from
 source](https://earthsystemmodeling.org/esmpy_doc/release/latest/html/install.html#installing-esmpy-from-source).
-With `esmpy` available, we can then install `regional_mom6` via pip. (If we don't have have pip, then
+With `esmpy` available, we can then install `regional-mom6` via pip. (If we don't have have pip, then
 `conda install pip` should do the job.)
 
 With `esmpy` installed we can now install `regional-mom6` via [`pip`](https://pypi.org/project/regional-mom6/):
 
 ```bash
 pip install regional-mom6
 ```
 
 The above installs the version of `regional-mom6` (plus any required dependencies) that corresponds to the latest tagged release of the package.
 
-#### "*I'd like to be on the cutting edge of the development*?"
+#### "*I want to live on the edge! I want the latest developments*"
 
-Alternatively, we can install directly `regional-mom6` directly via GitHub using `pip`.
-First install `esmpy` as described above and then:
+To install `regional-mom6` directly from the [GitHub repository](https://github.com/COSIMA/regional-mom6/) using `pip`, first install `esmpy` as described above. Then:
 
 ```bash
 pip install git+https://github.com/COSIMA/regional-mom6.git
 ```
 
 to get the version that corresponds to the latest commit in GitHub.
-Or, install the version that corresponds to a particular git commit using
+Alternatively, install the version that corresponds to a particular git commit using, for example,
 
 ```bash
 pip install git+https://github.com/COSIMA/regional-mom6.git@061b0ef80c7cbc04de0566df329c4ea472002f7e
 ```
 
 ## MOM6 Configuration and Version Requirements
 
-The package and demos assume a coupled SIS2-MOM6 configuration.
-The examples could work for an ocean-only MOM6 run but this has not been tested. 
+The package and demos assume a coupled MOM6-SIS2 configuration, but also work for MOM6 ocean-only configuration after appropriate changes in the `input.nml` and `MOM_input` files.
+
+Additionally, regional configurations require that the MOM6 executable _must_ be compiled with **symmetric memory**.
 
 The current release of this package assumes the latest source code of all components needed to run MOM6 as of
 January 2024. A forked version of the [`setup-mom6-nci`](https://github.com/ashjbarnes/setup-mom6-nci) repository
 contains scripts for compiling MOM6 and, furthermore, its [`src`](https://github.com/ashjbarnes/setup-mom6-nci/tree/setup-mom6/src)
 directory lists the particular commits that were used to compile MOM6 and its submodules for this package.
 
 Note that the commits used for MOM6 submodules (e.g., Flexible Modelling System (FMS), coupler, SIS2) are _not_
 necessarily those used by the GFDL's [`MOM6_examples`](https://github.com/NOAA-GFDL/MOM6-examples) repository.
 
-## Getting started
 
+## Getting started
 
 The [example notebooks](https://regional-mom6.readthedocs.io/en/latest/demos.html) walk you through how to use
 the package using two different sets of input datasets.
-Please ensure that you can get at least one of these working on your setup with your MOM6 executable before trying modify the example to suit your domain with your bathymethry, forcing, and boundary conditions.
-
-You can download the notebooks [from Github](https://github.com/COSIMA/regional-mom6/tree/ncc/installation/demos) or by clicking on the download <img width="22" alt="download" src="https://github.com/COSIMA/regional-mom6/assets/7112768/2c1ae149-c6a8-4395-ab09-2f77588008d9"> button, e.g., at the top-right of the [regional tasmania forced by ERA5 example](https://regional-mom6.readthedocs.io/en/latest/demo_notebooks/reanalysis-forced.html).
-
-**Note**
+Please ensure that you can get at least one of these working on your setup with your MOM6 executable before trying to modify the example to suit your domain with your bathymetry, forcing, and boundary conditions.
 
-The `xesmf` the package attempts to regrid in parallel, and if it's not able to do so, it throws a warning and
-runs in serial. You also get a print out of the relevant `mpirun` command which you could use as a backup.
-Depending on your setup of your machine, you may need to write scripts that implement the package to access more
-computational resources than might be available, e.g., on the HPC machine of you are working on.
+You can download the notebooks [from Github](https://github.com/COSIMA/regional-mom6/tree/main/demos) or by clicking on the download <img width="22" alt="download" src="https://github.com/COSIMA/regional-mom6/assets/7112768/2c1ae149-c6a8-4395-ab09-2f77588008d9"> button, e.g., at the top-right of the [regional Tasmania forced by ERA5 example](https://regional-mom6.readthedocs.io/en/latest/demo_notebooks/reanalysis-forced.html).
```

### Comparing `regional_mom6-0.5.0/demos/premade_run_directories/common_files/MOM_input` & `regional_mom6-0.5.1/demos/premade_run_directories/common_files/MOM_input`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.0/demos/premade_run_directories/common_files/MOM_layout` & `regional_mom6-0.5.1/demos/premade_run_directories/common_files/MOM_layout`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.0/demos/premade_run_directories/common_files/SIS_input` & `regional_mom6-0.5.1/demos/premade_run_directories/common_files/SIS_input`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.0/demos/premade_run_directories/common_files/data_table` & `regional_mom6-0.5.1/demos/premade_run_directories/common_files/data_table`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.0/demos/premade_run_directories/common_files/diag_table` & `regional_mom6-0.5.1/demos/premade_run_directories/common_files/diag_table`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.0/demos/premade_run_directories/common_files/input.nml` & `regional_mom6-0.5.1/demos/premade_run_directories/common_files/input.nml`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.0/demos/premade_run_directories/era5_surface/data_table` & `regional_mom6-0.5.1/demos/premade_run_directories/era5_surface/data_table`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.0/demos/premade_run_directories/era5_surface/input.nml` & `regional_mom6-0.5.1/demos/premade_run_directories/era5_surface/input.nml`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.0/demos/premade_run_directories/jra_surface/data_table` & `regional_mom6-0.5.1/demos/premade_run_directories/jra_surface/data_table`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.0/docs/Makefile` & `regional_mom6-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.0/docs/conf.py` & `regional_mom6-0.5.1/docs/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
-project = "Regional MOM6"
-copyright = "2023, Ashley Barnes & COSIMA Contributors"
-author = "Ashley Barnes & COSIMA Contributors"
+project = "regional-mom6"
+copyright = "2024, COSIMA community and outside contributors"
+author = "COSIMA community and outside contributors"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
```

### Comparing `regional_mom6-0.5.0/docs/contributing.md` & `regional_mom6-0.5.1/docs/contributing.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,74 +6,76 @@
 introduced. Also, sometimes it's also a good idea to build the documentation locally to see
 how new docstrings or any new bits of documentation that you may have added look like.
 
 
 ## Testing
 
 To run the tests from a local clone of the repository we first need to create a conda
-environment with all the dependencies required. From the repositories local clone main
-directory do
+environment with all the required dependencies.
+
+We create the environment by calling
 
 ```{code-block} bash
 conda env create --prefix ./env --file environment-ci.yml
 ```
 
-and then activate it
+from the repository's local clone main directory. Then we activate it via
 
 ```{code-block} bash
 conda activate ./env
 ```
 
-Now we need to install the package in this environment as well as `pytest`
+We then install both the package in this environment as well as the `pytest` package:
 
 ```{code-block} bash
 python -m pip install .
 python -m pip install pytest
 ```
 
 Now we can run the tests with
 
 ```{code-block} bash
 python -m pytest tests/
 ```
 
-If we also want to run the doctests (tests that appear as examples in various docstrings), we
-can use
+If we also want to run the doctests (that is, the tests that appear as examples in
+various docstrings), we can use
 
 ```{code-block} bash
 python -m pytest --doctest-modules tests/ regional_mom6/
 ```
 
 ## Documentation
 
 To build the docs from a local clone of the repository we first need to create a conda
-environment. Navigate to the `docs` directory of your local repository clone (e.g., `cd docs`)
-and then 
+environment after we first navigate to the `docs` directory of our local repository clone.
 
 ```{code-block} bash
 cd docs
 conda create --name docs-env --file requirements.txt
 ```
 
-Then activate this environment and install the package itself as an editable install (`pip install -e`).
+We activate this environment and install the package itself as an editable install (`pip install -e`).
 
 ```{code-block} bash
 conda activate docs-env
 pip install -e ..
 ```
 
-Now we can make the docs
+Now we can build the docs via `make`:
 
 ```{code-block} bash
 make html
 ```
 
-and open `_build/html/index.html` in your favorite browser.
+and upon successful build, we preview the documentation by opening `_build/html/index.html`
+in our favorite browser.
 
-Alternatively, we can install the dependencies needed for the docs via `pip`; the rest is same, that is
+Alternatively, instead of creating a conda environment, we can install the required
+dependencies for the docs via `pip`; the rest is same, that is
 
 ```{code-block} bash
 cd docs
 pip install -r requirements.txt
 pip install -e ..
 make html
 ```
```

### Comparing `regional_mom6-0.5.0/docs/installation.md` & `regional_mom6-0.5.1/docs/installation.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Installation
 ============
 
-#### Easy, clean, one liner
+We encourage creating a new or using an existing conda environment.
 
-The easiest way is to install `regional-mom6` via [`conda`](https://anaconda.org/conda-forge/regional-mom6).
-We encourage creating a new or using an existing conda environment and then simply
+## Easy, clean, one liner via conda
+
+The easiest way to install `regional-mom6` is via [`conda`](https://anaconda.org/conda-forge/regional-mom6).
 
 ```bash
 conda install conda-forge::regional-mom6
 ```
 
 That's it -- now enjoy!
 
-#### "*But I want `pip`, can't I install with `pip`*?"
+## "*But I want pip, can't I install with pip*?"
 
-We can install via `pip` but it's a bit more cumbersome.
-Again, we encourage creating a new or using an existing conda environment.
+To install via `pip` is a bit more cumbersome.
 
-A prerequisite is the binary `esmpy` dependency, which provides regridding capabilities.
+A prerequisite is the binary `esmpy` dependency, which provides re-gridding capabilities.
 The easiest way to install `esmpy` is via conda:
 
 ```bash
 conda install -c conda-forge esmpy
 ```
 
 Alternatively, to install `esmpy` in a Conda-free way, follow the instructions for [installing ESMPy from
@@ -33,22 +33,21 @@
 
 ```bash
 pip install regional-mom6
 ```
 
 The above installs the version of `regional-mom6` (plus any required dependencies) that corresponds to the latest tagged release of the package.
 
-#### "*I'd like to be on the cutting edge of the development*?"
+## "*I want to live on the edge! I want the latest developments*"
 
-Alternatively, we can install directly `regional-mom6` directly via GitHub using `pip`.
-First install `esmpy` as described above and then:
+To install `regional-mom6` directly from the [GitHub repository](https://github.com/COSIMA/regional-mom6/) using `pip`, first install `esmpy` as described above. Then:
 
 ```bash
 pip install git+https://github.com/COSIMA/regional-mom6.git
 ```
 
 to get the version that corresponds to the latest commit in GitHub.
-Or, install the version that corresponds to a particular git commit using
+Alternatively, install the version that corresponds to a particular git commit using, for example,
 
 ```bash
 pip install git+https://github.com/COSIMA/regional-mom6.git@061b0ef80c7cbc04de0566df329c4ea472002f7e
 ```
```

### Comparing `regional_mom6-0.5.0/pyproject.toml` & `regional_mom6-0.5.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [project]
 name = "regional_mom6"
-description = "Automatic generation of regional configurations for Modular Ocean Model 6"
-keywords = ["mom6", "regional", "ocean modeling"]
+description = "Automatic generation of regional configurations for Modular Ocean Model v6"
+keywords = ["mom6", "regional", "ocean modeling", "python"]
 authors = [
-  {name = "Ashley Barnes, COSIMA community, and contributors"},
+  {name = "COSIMA community and outside contributors"},
 ]
 dynamic = ["version"]
+readme = "README.md"
 dependencies = [
   "bottleneck",
   "dask[array]",
   "dask[distributed]",
   "netCDF4",
   "numpy >= 1.17.0",
   "scipy >= 1.2.0",
```

### Comparing `regional_mom6-0.5.0/regional_mom6/regional_mom6.py` & `regional_mom6-0.5.1/regional_mom6/regional_mom6.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,16 +29,17 @@
 
 
 ## Auxiliary functions
 
 
 def longitude_slicer(data, longitude_extent, longitude_coords):
     """
-    Slice longitudes, handling periodicity and 'seams' where the
-    data wraps around (commonly either in domain [0, 360], [-180, 180], or [-270, 90]).
+    Slice longitudes while handling periodicity and the 'seams', that is the
+    longitude values where the data wraps around in a global domain (for example,
+    longitudes are defined, usually, within domain [0, 360] or [-180, 180]).
 
     The algorithm works in five steps:
 
     - Determine whether we need to add or subtract 360 to get the middle of the
       ``longitude_extent`` to lie within ``data``'s longitude range (hereby ``old_lon``).
 
     - Shift the dataset so that its midpoint matches the midpoint of
@@ -46,19 +47,19 @@
       does not increase monotonically from West to East since the 'seam'
       has moved.
 
     - Fix ``old_lon`` to make it monotonically increasing again. This uses
       the information we have about the way the dataset was shifted/rolled.
 
     - Slice the ``data`` index-wise. We know that ``|longitude_extent[1] - longitude_extent[0]| / 360``
-      multiplied by the number of discrete longitude points will give
-      the total width of our slice, and we've already set the midpoint
+      multiplied by the number of discrete longitude points in the global input data gives
+      the number of longitude points in our slice, and we've already set the midpoint
       to be the middle of the target domain.
 
-    - Finally re-add the right multiple of 360 so the whole domain matches
+    - Finally re-add the correct multiple of 360 so the whole domain matches
       the target.
 
     Args:
         data (xarray.Dataset): The global data you want to slice in longitude.
         longitude_extent (Tuple[float, float]): The target longitudes (in degrees)
             we want to slice to. Must be in increasing order.
         longitude_coords (Union[str, list[str]): The name or list of names of the
@@ -116,15 +117,15 @@
                     new_lon[0:new_seam_index] -= 360
 
                 if shift < 0:
                     new_seam_index = data[lon].shape[0] + shift
 
                     new_lon[new_seam_index:] += 360
 
-                ## new_x is used to recentre the midpoint to match that of target domain
+                ## new_lon is used to re-centre the midpoint to match that of target domain
                 new_lon -= i * 360
 
                 new_data = new_data.assign_coords({lon: new_lon})
 
                 ## Choose the number of lon points to take from the middle, including a buffer.
                 ## Use this to index the new global dataset
                 num_lonpoints = (
@@ -159,15 +160,15 @@
     Positive parameter ``ratio`` prescribes (approximately) the ratio of the thickness
     of the bottom-most layer to the top-most layer. The final ratio of the bottom-most
     layer to the top-most layer ends up a bit different from the prescribed ``ratio``.
     In particular, the final ratio of the bottom over the top-most layer thickness is
     ``(1 + ratio * exp(2π)) / (ratio + exp(2π))``. This slight departure comes about
     because of the value of the hyperbolic tangent profile at the end-points ``tanh(π)``,
     which is approximately 0.9963 and not 1. Note that because ``exp(2π)`` is much greater
-    than 1, the value of the actual ratio is not that different from prescribed value
+    than 1, the value of the actual ratio is not that different from the prescribed value
     ``ratio``, e.g., for ``ratio`` values between 1/100 and 100 the final ratio of the
     bottom-most layer to the top-most layer only departs from the prescribed ``ratio``
     by ±20%.
 
     Args:
         nlayers (int): Number of vertical layers.
         ratio (float): The desired value of the ratio of bottom-most to
@@ -258,16 +259,16 @@
     assert np.isclose(total_depth, sum_of_thicknesses, atol=atol)  # just checking ;)
 
     return layer_thicknesses
 
 
 def rectangular_hgrid(λ, φ):
     """
-    Construct a horizontal grid with all the metadata required by MOM6 provided
-    an array of longitudes (``λ``) and latitudes (``φ``) on the supergrid.
+    Construct a horizontal grid with all the metadata required by MOM6, based on
+    arrays of longitudes (``λ``) and latitudes (``φ``) on the supergrid.
     Here, 'supergrid' refers to both cell edges and centres, meaning that there
     are twice as many points along each axis than for any individual field.
 
     Caution:
         It is assumed the grid's boundaries are lines of constant latitude and
         longitude. Rotated grids need to be handled differently.
 
@@ -291,15 +292,15 @@
     # compute longitude spacing and ensure that longitudes are uniformly spaced
     dλ = λ[1] - λ[0]
 
     assert np.allclose(
         np.diff(λ), dλ * np.ones(np.size(λ) - 1)
     ), "provided array of longitudes must be uniformly spaced"
 
-    # dx = R * cos(φ) * np.deg2rad(dλ) / 2
+    # dx = R * cos(np.deg2rad(φ)) * np.deg2rad(dλ) / 2
     # Note: division by 2 because we're on the supergrid
     dx = np.broadcast_to(
         R * np.cos(np.deg2rad(φ)) * np.deg2rad(dλ) / 2,
         (λ.shape[0] - 1, φ.shape[0]),
     ).T
 
     # dy = R * np.deg2rad(dφ) / 2
@@ -318,23 +319,23 @@
             "discretization": "logically_rectangular",
             "conformal": "true",
         },
         "x": {"standard_name": "geographic_longitude", "units": "degree_east"},
         "y": {"standard_name": "geographic_latitude", "units": "degree_north"},
         "dx": {
             "standard_name": "grid_edge_x_distance",
-            "units": "metres",
+            "units": "meters",
         },
         "dy": {
             "standard_name": "grid_edge_y_distance",
-            "units": "metres",
+            "units": "meters",
         },
         "area": {
             "standard_name": "grid_cell_area",
-            "units": "m2",
+            "units": "m**2",
         },
         "angle_dx": {
             "standard_name": "grid_vertex_x_angle_WRT_geographic_east",
             "units": "degrees_east",
         },
         "arcx": {
             "standard_name": "grid_edge_x_arc_type",
@@ -359,41 +360,45 @@
 class experiment:
     """The main class for setting up a regional experiment.
 
     Everything about the regional experiment.
 
     Methods in this class generate the various input files needed for a MOM6
     experiment forced with open boundary conditions (OBCs). The code is agnostic
-    to the user's choice of boundary forcing, bathymetry and surface forcing;
+    to the user's choice of boundary forcing, bathymetry, and surface forcing;
     users need to prescribe what variables are all called via mapping dictionaries
     from MOM6 variable/coordinate name to the name in the input dataset.
 
     The class can be used to generate the grids for a new experiment, or to read in
-    an existing one by providing with ``read_existing_grids=True``.
+    an existing one (when ``read_existing_grids=True``; see argument description below).
 
     Args:
-        longitude_extent (Tuple[float]): Extent of the region in longitude in degrees.
-        latitude_extent (Tuple[float]): Extent of the region in latitude in degrees.
-        date_range (Tuple[str]): Start and end dates of the boundary forcing window.
-        resolution (float): Lateral resolution of the domain, in degrees.
+        longitude_extent (Tuple[float]): Extent of the region in longitude (in degrees). For
+            example: ``(40.5, 50.0)``.
+        latitude_extent (Tuple[float]): Extent of the region in latitude (in degrees). For
+            example: ``(-20.0, 30.0)``.
+        date_range (Tuple[str]): Start and end dates of the boundary forcing window. For
+            example: ``("2003-01-01", "2003-01-31")``.
+        resolution (float): Lateral resolution of the domain (in degrees).
         number_vertical_layers (int): Number of vertical layers.
         layer_thickness_ratio (float): Ratio of largest to smallest layer thickness;
             used as input in :func:`~hyperbolictan_thickness_profile`.
         depth (float): Depth of the domain.
         mom_run_dir (str): Path of the MOM6 control directory.
         mom_input_dir (str): Path of the MOM6 input directory, to receive the forcing files.
         toolpath_dir (str): Path of GFDL's FRE tools (https://github.com/NOAA-GFDL/FRE-NCtools)
             binaries.
         grid_type (Optional[str]): Type of horizontal grid to generate.
             Currently, only ``'even_spacing'`` is supported.
         repeat_year_forcing (Optional[bool]): When ``True`` the experiment runs with
             repeat-year forcing. When ``False`` (default) then inter-annual forcing is used.
         read_existing_grids (Optional[Bool]): When ``True``, instead of generating the grids,
-            reads the grids and ocean mask from ``mom_input_dir`` and ``mom_run_dir``. Useful
-            for modifying or troubleshooting experiments. Default: ``False``.
+            the grids and the ocean mask are being read from within the ``mom_input_dir`` and
+            ``mom_run_dir`` directories. Useful for modifying or troubleshooting experiments.
+            Default: ``False``.
     """
 
     def __init__(
         self,
         *,
         longitude_extent,
         latitude_extent,
@@ -412,37 +417,38 @@
         ## in case list was given, convert to tuples
         self.longitude_extent = tuple(longitude_extent)
         self.latitude_extent = tuple(latitude_extent)
         self.date_range = tuple(date_range)
 
         self.mom_run_dir = Path(mom_run_dir)
         self.mom_input_dir = Path(mom_input_dir)
+        self.toolpath_dir = Path(toolpath_dir)
 
         self.mom_run_dir.mkdir(exist_ok=True)
         self.mom_input_dir.mkdir(exist_ok=True)
 
         self.date_range = [
             dt.datetime.strptime(date_range[0], "%Y-%m-%d %H:%M:%S"),
             dt.datetime.strptime(date_range[1], "%Y-%m-%d %H:%M:%S"),
         ]
         self.resolution = resolution
         self.number_vertical_layers = number_vertical_layers
         self.layer_thickness_ratio = layer_thickness_ratio
         self.depth = depth
-        self.toolpath_dir = Path(toolpath_dir)
         self.grid_type = grid_type
         self.repeat_year_forcing = repeat_year_forcing
         self.ocean_mask = None
         if read_existing_grids:
             try:
                 self.hgrid = xr.open_dataset(self.mom_input_dir / "hgrid.nc")
                 self.vgrid = xr.open_dataset(self.mom_input_dir / "vcoord.nc")
             except:
                 print(
-                    "Error in reading in existing grids. Make sure you've got files called `hgrid.nc` and `vcoord.nc` in {self.mom_input_dir}"
+                    "Error while reading in existing grids!\n\n"
+                    + f"Make sure `hgrid.nc` and `vcoord.nc` exists in {self.mom_input_dir} directory."
                 )
                 raise ValueError
         else:
             self.hgrid = self._make_hgrid()
             self.vgrid = self._make_vgrid()
         # create additional directories and links
         (self.mom_input_dir / "weights").mkdir(exist_ok=True)
@@ -456,38 +462,42 @@
             input_rundir.symlink_to(self.mom_run_dir.resolve())
 
     def __getattr__(self, name):
         available_methods = [
             method for method in dir(self) if not method.startswith("__")
         ]
         error_message = (
-            f"'{name}' method not found. Available methods are: {available_methods}"
+            f"{name} method not found. Available methods are: {available_methods}"
         )
         raise AttributeError(error_message)
 
     def _make_hgrid(self):
         """
         Set up a horizontal grid based on user's specification of the domain.
-        The default behaviour provides with a grid evenly spaced both in
-        longitude and in latitude.
+        The default behaviour generates a grid evenly spaced both in longitude
+        and in latitude.
 
-        The latitudinal resolution is scaled with the cosine of the central latitude of
-        the domain, i.e., ``Δφ = cos(φ_central) * Δλ``, where ``Δλ`` is the longitudinal
-        spacing. This way, and given that the domain is small enough, the linear
-        distances between grid points are nearly identical: ``Δx = R * cos(φ) * Δλ``
-        and ``Δy = R * Δφ = R * cos(φ_central) * Δλ``. That is, given that the domain is
-        small enough so that so that ``cos(φ_North_Side)`` is not much different from
-        ``cos(φ_South_Side)`` then ``Δx`` and ``Δy`` are similar.
+        The latitudinal resolution is scaled with the cosine of the central
+        latitude of the domain, i.e., ``Δφ = cos(φ_central) * Δλ``, where ``Δλ``
+        is the longitudinal spacing. This way, for a sufficiently small domain,
+        the linear distances between grid points are nearly identical:
+        ``Δx = R * cos(φ) * Δλ`` and ``Δy = R * Δφ = R * cos(φ_central) * Δλ``
+        (here ``R`` is Earth's radius and ``φ``, ``φ_central``, ``Δλ``, and ``Δφ``
+        are all expressed in radians).
+        That is, if the domain is small enough that so that ``cos(φ_North_Side)``
+        is not much different from ``cos(φ_South_Side)``, then ``Δx`` and ``Δy``
+        are similar.
 
         Note:
-            The intention is for the horizontal grid (``hgrid``) generation to be very flexible.
+            The intention is for the horizontal grid (``hgrid``) generation to be flexible.
             For now, there is only one implemented horizontal grid included in the package,
-            but you can customise it by simply overwriting the ``hgrid.nc`` file in the ``rundir``
-            after initialising an ``experiment``. To conserve the metadata, it might be easiest
-            to read the file in, then modify the fields before re-saving.
+            but you can customise it by simply overwriting the ``hgrid.nc`` file in the
+            ``mom_run_dir`` directory after initialising an ``experiment``. To preserve the
+            metadata, it might be easiest to read the file in, then modify the fields before
+            re-saving.
         """
 
         assert (
             self.grid_type == "even_spacing"
         ), "only even_spacing grid type is implemented"
 
         if self.grid_type == "even_spacing":
@@ -528,17 +538,18 @@
             hgrid = rectangular_hgrid(λ, φ)
             hgrid.to_netcdf(self.mom_input_dir / "hgrid.nc")
 
             return hgrid
 
     def _make_vgrid(self):
         """
-        Generate a vertical grid based on the number of layers ``nlayers`` and
-        the prescribed ratio of the vertical layer thicknesses (``layer_thickness_ratio``)
-        specified at the class level.
+        Generates a vertical grid based on the ``number_vertical_layers``, the ratio
+        of largest to smallest layer thickness (``layer_thickness_ratio``) and the
+        total ``depth`` parameters.
+        (All these parameters are specified at the class level.)
         """
 
         thicknesses = hyperbolictan_thickness_profile(
             self.number_vertical_layers, self.layer_thickness_ratio, self.depth
         )
 
         zi = np.cumsum(thicknesses)
@@ -551,63 +562,66 @@
         vcoord["zi"].attrs = {"units": "meters"}
         vcoord["zl"].attrs = {"units": "meters"}
 
         vcoord.to_netcdf(self.mom_input_dir / "vcoord.nc")
 
         return vcoord
 
-    def initial_condition(self, ic_path, varnames, gridtype="A", vcoord_type="height"):
+    def initial_condition(
+        self, ic_path, varnames, arakawa_grid="A", vcoord_type="height"
+    ):
         """
-        Read the initial condition files, interpolates to the model grid fixes
-        up metadata and saves to the input directory.
+        Reads the initial condition from files in ``ic_path``, interpolates to the
+        model grid, fixes up metadata, and saves back to the input directory.
 
         Args:
             ic_path (Union[str, Path]): Path to initial condition file.
             varnames (Dict[str, str]): Mapping from MOM6 variable/coordinate names to the names
                 in the input dataset. For example, ``{'xq': 'lonq', 'yh': 'lath', 'salt': 'so', ...}``.
-            gridtype (Optional[str]): Arakawa grid staggering of input; either ``'A'``, ``'B'``,
-                or ``'C'``.
+            arakawa_grid (Optional[str]): Arakawa grid staggering type of the initial condition.
+                Either ``'A'`` (default), ``'B'``, or ``'C'``.
             vcoord_type (Optional[str]): The type of vertical coordinate used in the forcing files.
                 Either ``'height'`` or ``'thickness'``.
         """
 
-        # Remove time dimension if present in the IC. Assume that the first time dim is the intended on if more than one is present
+        # Remove time dimension if present in the IC.
+        # Assume that the first time dim is the intended on if more than one is present
 
         ic_raw = xr.open_dataset(ic_path)
         if varnames["time"] in ic_raw.dims:
             ic_raw = ic_raw.isel({varnames["time"]: 0})
         if varnames["time"] in ic_raw.coords:
             ic_raw = ic_raw.drop(varnames["time"])
 
         # Separate out tracers from two velocity fields of IC
         try:
             ic_raw_tracers = ic_raw[
                 [varnames["tracers"][i] for i in varnames["tracers"]]
             ]
         except:
             raise ValueError(
-                "Error in reading in initial condition tracers. Terminating"
+                "Error in reading in initial condition tracers. Terminating!"
             )
         try:
             ic_raw_u = ic_raw[varnames["u"]]
             ic_raw_v = ic_raw[varnames["v"]]
         except:
             raise ValueError(
-                "Error in reading in initial condition tracers. Terminating"
+                "Error in reading in initial condition tracers. Terminating!"
             )
 
         try:
             ic_raw_eta = ic_raw[varnames["eta"]]
         except:
             raise ValueError(
-                "Error in reading in initial condition tracers. Terminating"
+                "Error in reading in initial condition tracers. Terminating!"
             )
 
         # Rename all coordinates to have 'lon' and 'lat' to work with the xesmf regridder
-        if gridtype == "A":
+        if arakawa_grid == "A":
             if (
                 "xh" in varnames.keys() and "yh" in varnames.keys()
             ):  ## Handle case where user has provided xh and yh rather than x & y
                 # Rename xh with x in dictionary
                 varnames["x"] = varnames["xh"]
                 varnames["y"] = varnames["yh"]
 
@@ -618,17 +632,20 @@
                 ic_raw_u = ic_raw_u.rename({varnames["x"]: "lon", varnames["y"]: "lat"})
                 ic_raw_v = ic_raw_v.rename({varnames["x"]: "lon", varnames["y"]: "lat"})
                 ic_raw_eta = ic_raw_eta.rename(
                     {varnames["x"]: "lon", varnames["y"]: "lat"}
                 )
             else:
                 raise ValueError(
-                    "Can't find required coordinates in initial condition. Given that gridtype is 'A' the 'x' and 'y' coordinates should be provided in the varnames dictionary. E.g., {'x': 'lon','y': 'lat'}. Terminating"
+                    "Can't find required coordinates in initial condition.\n\n"
+                    + "Given that arakawa_grid is 'A' the 'x' and 'y' coordinates should be provided"
+                    + "in the varnames dictionary. For example, {'x': 'lon', 'y': 'lat'}.\n\n"
+                    + "Terminating!"
                 )
-        if gridtype == "B":
+        if arakawa_grid == "B":
             if (
                 "xq" in varnames.keys()
                 and "yq" in varnames.keys()
                 and "xh" in varnames.keys()
                 and "yh" in varnames.keys()
             ):
                 ic_raw_tracers = ic_raw_tracers.rename(
@@ -641,17 +658,21 @@
                     {varnames["xq"]: "lon", varnames["yq"]: "lat"}
                 )
                 ic_raw_v = ic_raw_v.rename(
                     {varnames["xq"]: "lon", varnames["yq"]: "lat"}
                 )
             else:
                 raise ValueError(
-                    "Can't find coordinates in initial condition. Given that gridtype is 'B' the names of the cell centre ('xh' & 'yh') as well as the cell edge ('xq' & 'yq') coordinates should be provided in the varnames dictionary. E.g {'xh':'lonh','yh':'lath' etc }. Terminating"
+                    "Can't find coordinates in initial condition.\n\n"
+                    + "Given that arakawa_grid is 'B' the names of the cell centers ('xh' & 'yh')"
+                    + "as well as the cell edges ('xq' & 'yq') coordinates should be provided in "
+                    + "the varnames dictionary. For example, {'xh': 'lonh', 'yh': 'lath', ...}.\n\n"
+                    + "Terminating!"
                 )
-        if gridtype == "C":
+        if arakawa_grid == "C":
             if (
                 "xq" in varnames.keys()
                 and "yq" in varnames.keys()
                 and "xh" in varnames.keys()
                 and "yh" in varnames.keys()
             ):
                 ic_raw_tracers = ic_raw_tracers.rename(
@@ -664,46 +685,51 @@
                     {varnames["xq"]: "lon", varnames["yh"]: "lat"}
                 )
                 ic_raw_v = ic_raw_v.rename(
                     {varnames["xh"]: "lon", varnames["yq"]: "lat"}
                 )
             else:
                 raise ValueError(
-                    "Can't find coordinates in initial condition. Given that gridtype is 'C' the names of the cell centre ('xh' & 'yh') as well as the cell edge ('xq' & 'yq') coordinates should be provided in the varnames dictionary. E.g {'xh':'lonh','yh':'lath' etc }. Terminating"
+                    "Can't find coordinates in initial condition.\n\n"
+                    + "Given that arakawa_grid is 'C' the names of the cell centers ('xh' & 'yh')"
+                    + "as well as the cell edges ('xq' & 'yq') coordinates should be provided in "
+                    + "in the varnames dictionary. For example, {'xh': 'lonh', 'yh': 'lath', ...}.\n\n"
+                    + "Terminating!"
                 )
-        ## Construct the xq,yh and xh yq grids
+        ## Construct the xq, yh and xh, yq grids
         ugrid = (
             self.hgrid[["x", "y"]]
             .isel(nxp=slice(None, None, 2), nyp=slice(1, None, 2))
             .rename({"x": "lon", "y": "lat"})
             .set_coords(["lat", "lon"])
         )
         vgrid = (
             self.hgrid[["x", "y"]]
             .isel(nxp=slice(1, None, 2), nyp=slice(None, None, 2))
             .rename({"x": "lon", "y": "lat"})
             .set_coords(["lat", "lon"])
         )
 
-        ## Construct the cell centre grid for tracers (xh,yh).
+        ## Construct the cell centre grid for tracers (xh, yh).
         tgrid = xr.Dataset(
             {
                 "lon": (
                     ["lon"],
                     self.hgrid.x.isel(nxp=slice(1, None, 2), nyp=1).values,
                 ),
                 "lat": (
                     ["lat"],
                     self.hgrid.y.isel(nxp=1, nyp=slice(1, None, 2)).values,
                 ),
             }
         )
 
         ### Drop NaNs to be re-added later
-        # NaNs might be here from the land mask of the model that the IC has come from. If they're not removed then the coastlines from this other grid will be retained!
+        # NaNs might be here from the land mask of the model that the IC has come from.
+        # If they're not removed then the coastlines from this other grid will be retained!
         ic_raw_tracers = (
             ic_raw_tracers.interpolate_na("lon", method="linear")
             .ffill("lon")
             .bfill("lon")
             .ffill("lat")
             .bfill("lat")
             .ffill(varnames["zl"])
@@ -795,14 +821,16 @@
         for i in varnames["tracers"]:
             tracers_out[i].attrs = ic_raw_tracers[varnames["tracers"][i]].attrs
 
         eta_out.xh.attrs = ic_raw_tracers.lon.attrs
         eta_out.yh.attrs = ic_raw_tracers.lat.attrs
         eta_out.attrs = ic_raw_eta.attrs
 
+        ## if min(temp) > 100 then assume that units must be degrees K
+        ## (otherwise we can't be on Earth) and convert to degrees C
         if np.min(tracers_out["temp"].isel({"zl": 0})) > 100:
             tracers_out["temp"] -= 273.15
 
         ## Regrid the fields vertically
 
         if (
             vcoord_type == "thickness"
@@ -853,56 +881,56 @@
         self.ic_vels = vel_out
         return
 
     def rectangular_boundary(
         self, path_to_bc, varnames, orientation, segment_number, arakawa_grid="A"
     ):
         """
-        Setup a boundary forcing file for a given orientation. Here the term 'rectangular'
-        implies boundaries along lines of constant latitude or longitude.
+        Set up a boundary forcing file for a given orientation. Here the term 'rectangular'
+        means boundaries along lines of constant latitude or longitude.
 
         Args:
             path_to_bc (str): Path to boundary forcing file. Ideally this should be a pre cut-out
                 netCDF file containing only the boundary region and 3 extra boundary points on either
                 side. Users can also provide a large dataset containing their entire domain but this
                 will be slower.
             varnames (Dict[str, str]): Mapping from MOM6 variable/coordinate names to the name in the
                 input dataset.
             orientation (str): Orientation of boundary forcing file, i.e., ``'east'``, ``'west'``,
                 ``'north'``, or ``'south'``.
             segment_number (int): Number the segments according to how they'll be specified in
                 the ``MOM_input``.
-            arakawa_grid (Optional[str]): Arakawa grid staggering of input; either ``'A'``, ``'B'``,
-                or ``'C'``.
+            arakawa_grid (Optional[str]): Arakawa grid staggering type of the boundary forcing.
+                Either ``'A'`` (default), ``'B'``, or ``'C'``.
         """
 
         print("Processing {} boundary...".format(orientation), end="")
 
         seg = segment(
-            self.hgrid,
-            path_to_bc,  # location of raw boundary
-            self.mom_input_dir,
-            varnames,
-            "segment_{:03d}".format(segment_number),
-            orientation,  # orienataion
-            self.date_range[0],
-            gridtype=arakawa_grid,
+            hgrid=self.hgrid,
+            infile=path_to_bc,  # location of raw boundary
+            outfolder=self.mom_input_dir,
+            varnames=varnames,
+            segment_name="segment_{:03d}".format(segment_number),
+            orientation=orientation,  # orienataion
+            startdate=self.date_range[0],
+            arakawa_grid=arakawa_grid,
             repeat_year_forcing=self.repeat_year_forcing,
         )
 
         seg.rectangular_brushcut()
         print("Done.")
         return
 
     def setup_bathymetry(
         self,
         *,
         bathymetry_path,
-        longitude_coordinate_name="lat",
-        latitude_coordinate_name="lon",
+        longitude_coordinate_name="lon",
+        latitude_coordinate_name="lat",
         vertical_coordinate_name="elevation",
         fill_channels=False,
         minimum_layers=3,
         positive_down=False,
         chunks="auto",
     ):
         """
@@ -914,17 +942,17 @@
 
         Output is saved in the input directory of the experiment.
 
         Args:
             bathymetry_path (str): Path to the netCDF file with the bathymetry.
             longitude_coordinate_name (Optional[str]): The name of the longitude coordinate in the bathymetry
                 dataset at ``bathymetry_path``. For example, for GEBCO bathymetry: ``'lon'`` (default).
-            latitude_coordinate_name (Optional[str]): The name of the longitude coordinate in the bathymetry
+            latitude_coordinate_name (Optional[str]): The name of the latitude coordinate in the bathymetry
                 dataset at ``bathymetry_path``. For example, for GEBCO bathymetry: ``'lat'`` (default).
-            vertical_coordinate_name (Optional[str]): The name of the longitude coordinate in the bathymetry
+            vertical_coordinate_name (Optional[str]): The name of the vertical coordinate in the bathymetry
                 dataset at ``bathymetry_path``. For example, for GEBCO bathymetry: ``'elevation'`` (default).
             fill_channels (Optional[bool]): Whether or not to fill in
                 diagonal channels. This removes more narrow inlets,
                 but can also connect extra islands to land. Default: ``False``.
             minimum_layers (Optional[int]): The minimum depth allowed as an integer
                 number of layers. Anything shallower than the ``minimum_layers``
                 (as specified by the vertical coordinate file ``vcoord.nc``) is deemed land.
@@ -1002,15 +1030,15 @@
 
         bathymetry_output = bathymetry_output.rename(
             {coordinate_names["xh"]: "lon", coordinate_names["yh"]: "lat"}
         )
         bathymetry_output.lon.attrs["units"] = "degrees_east"
         bathymetry_output.lat.attrs["units"] = "degrees_north"
         bathymetry_output.elevation.attrs["_FillValue"] = -1e20
-        bathymetry_output.elevation.attrs["units"] = "m"
+        bathymetry_output.elevation.attrs["units"] = "meters"
         bathymetry_output.elevation.attrs["standard_name"] = (
             "height_above_reference_ellipsoid"
         )
         bathymetry_output.elevation.attrs["long_name"] = (
             "Elevation relative to sea level"
         )
         bathymetry_output.elevation.attrs["coordinates"] = "lon lat"
@@ -1061,30 +1089,30 @@
             }
 
         tgrid = tgrid.chunk(chunks)
         tgrid.lon.attrs["units"] = "degrees_east"
         tgrid.lon.attrs["_FillValue"] = 1e20
         tgrid.lat.attrs["units"] = "degrees_north"
         tgrid.lat.attrs["_FillValue"] = 1e20
-        tgrid.elevation.attrs["units"] = "m"
+        tgrid.elevation.attrs["units"] = "meters"
         tgrid.elevation.attrs["coordinates"] = "lon lat"
         tgrid.to_netcdf(
             self.mom_input_dir / "bathymetry_unfinished.nc", mode="w", engine="netcdf4"
         )
         tgrid.close()
 
         ## Replace subprocess run with regular regridder
         print(
             "Begin regridding bathymetry...\n\n"
             + "If this process hangs it means that the chosen domain might be too big to handle this way. "
             + "After ensuring access to appropriate computational resources, try calling ESMF "
             + "directly from a terminal in the input directory via\n\n"
             + "mpirun ESMF_Regrid -s bathymetry_original.nc -d bathymetry_unfinished.nc -m bilinear --src_var elevation --dst_var elevation --netcdf4 --src_regional --dst_regional\n\n"
             + "For details see https://xesmf.readthedocs.io/en/latest/large_problems_on_HPC.html\n\n"
-            + "Aftewards, we run 'tidy_bathymetry' method to skip the expensive interpolation step, and finishing metadata, encoding and cleanup."
+            + "Afterwards, we run 'tidy_bathymetry' method to skip the expensive interpolation step, and finishing metadata, encoding and cleanup."
         )
 
         # If we have a domain large enough for chunks, we'll run regridder with parallel=True
         parallel = True
         if len(tgrid.chunks) != 2:
             parallel = False
         print(f"Regridding in parallel: {parallel}")
@@ -1109,42 +1137,42 @@
     ):
         """
         An auxiliary function for bathymetry used to fix up the metadata and remove inland
         lakes after regridding the bathymetry. Having `tidy_bathymetry` as a separate
         method from :func:`~setup_bathymetry` allows for the regridding to be done separately,
         since regridding can be really expensive for large domains.
 
-        If the bathymetry is already regridded and what is left to be done is fixing the metadata,
-        or fill in some channels then call this function directly to read in the existing
+        If the bathymetry is already regridded and what is left to be done is fixing the metadata
+        or fill in some channels, then call this function directly to read in the existing
         ``bathymetry_unfinished.nc`` file that should be in the input directory.
 
         Args:
-            fill_channels (Optional[bool]): Whether or not to fill in
+            fill_channels (Optional[bool]): Whether to fill in
                 diagonal channels. This removes more narrow inlets,
                 but can also connect extra islands to land. Default: ``False``.
             minimum_layers (Optional[int]): The minimum depth allowed
                 as an integer number of layers. The default value of ``3``
                 layers means that anything shallower than the 3rd
                 layer (as specified by the ``vcoord``) is deemed land.
-            positive_down (Optional[bool]): If ``True`` (default), it assumes that
+            positive_down (Optional[bool]): If ``True`` (default), assume that
                 bathymetry vertical coordinate is positive down.
         """
 
         ## reopen bathymetry to modify
         print("Reading in regridded bathymetry to fix up metadata...", end="")
         bathymetry = xr.open_dataset(
             self.mom_input_dir / "bathymetry_unfinished.nc", engine="netcdf4"
         )
 
         ## Ensure correct encoding
         bathymetry = xr.Dataset(
             {"depth": (["ny", "nx"], bathymetry["elevation"].values)}
         )
         bathymetry.attrs["depth"] = "meters"
-        bathymetry.attrs["standard_name"] = "bathymetryraphic depth at T-cell centers"
+        bathymetry.attrs["standard_name"] = "bathymetric depth at T-cell centers"
         bathymetry.attrs["coordinates"] = "zi"
 
         bathymetry.expand_dims("tiles", 0)
 
         if not positive_down:
             ## Ensure that coordinate is positive down!
             bathymetry["depth"] *= -1
@@ -1308,15 +1336,15 @@
         User provides processor ``layout`` tuple of processing units.
         """
 
         print(
             "Running GFDL's FRE Tools. The following information is all printed by the FRE tools themselves"
         )
         if not (self.mom_input_dir / "bathymetry.nc").exists():
-            print("No bathymetry file! Need to run .setup_bathymetry method first")
+            print("No bathymetry file! Need to run setup_bathymetry method first")
             return
 
         for p in self.mom_input_dir.glob("mask_table*"):
             p.unlink()
 
         print(
             "OUTPUT FROM MAKE SOLO MOSAIC:",
@@ -1364,20 +1392,18 @@
     def setup_run_directory(
         self,
         surface_forcing=None,
         using_payu=False,
         overwrite=False,
     ):
         """
-        Setup the run directory for MOM6. Either copy a pre-made set of files, or modify
+        Set up the run directory for MOM6. Either copy a pre-made set of files, or modify
         existing files in the 'rundir' directory for the experiment.
 
         Args:
-            regional_mom6_path (str): Path to the regional MOM6 source code that was cloned
-                from GitHub. Default is current path, ``'.'``.
             surface_forcing (Optional[str]): Specify the choice of surface forcing, one
                 of: ``'jra'`` or ``'era5'``. If not prescribed then constant fluxes are used.
             using_payu (Optional[bool]): Whether or not to use payu (https://github.com/payu-org/payu)
                 to run the model. If ``True``, a payu configuration file will be created.
                 Default: ``False``.
             overwrite (Optional[bool]): Whether or not to overwrite existing files in the
                 run directory. If ``False`` (default), will only modify the ``MOM_layout`` file and will
@@ -1389,15 +1415,16 @@
             importlib.resources.files("regional_mom6") / "demos/premade_run_directories"
         )
 
         # Define the locations of the directories we'll copy files across from. Base contains most of the files, and overwrite replaces files in the base directory.
         base_run_dir = premade_rundir_path / "common_files"
         if not premade_rundir_path.exists():
             raise ValueError(
-                f"Cannot find the premade run directory files at \n{premade_rundir_path}\n. Something is not right about how the package has been installed as these files are missing!"
+                f"Cannot find the premade run directory files at {premade_rundir_path}.\n\n"
+                + "These files missing might be indicating an error during the package installation!"
             )
         if surface_forcing:
             overwrite_run_dir = premade_rundir_path / f"{surface_forcing}_surface"
             if not overwrite_run_dir.exists():
                 available = [x for x in premade_rundir_path.iterdir() if x.is_dir()]
                 raise ValueError(
                     f"Surface forcing {surface_forcing} not available. Please choose from {str(available)}"  ##Here print all available run directories
@@ -1450,19 +1477,22 @@
 
             _, masked, layout = p.name.split(".")
             mask_table = p.name
             x, y = (int(v) for v in layout.split("x"))
             ncpus = (x * y) - int(masked)
         if mask_table == None:
             print(
-                "No mask table found! This suggests the domain is mostly water, so there are no `non compute` cells that are entirely land. If this doesn't seem right, ensure you've already run .FRE_tools()."
+                "No mask table found! This suggests the domain is mostly water, so there are "
+                + "no `non compute` cells that are entirely land. If this doesn't seem right, "
+                + "ensure you've already run `FRE_tools`."
             )
             if not hasattr(self, "layout"):
                 raise AttributeError(
-                    "No layout information found. This suggests you haven't run .FRE_tools() yet. Please do so first so I know how many processors you'd like to use."
+                    "No layout information found. This suggests that `FRE_tools()` hasn't been called yet. "
+                    + "Please do so, in order for the number of processors required is computed."
                 )
             ncpus = self.layout[0] * self.layout[1]
         print("Number of CPUs required: ", ncpus)
 
         ## Modify the input namelists to give the correct layouts
         # TODO Re-implement with package that works for this file type? or at least tidy up code
         with open(self.mom_run_dir / "MOM_layout", "r") as file:
@@ -1538,93 +1568,94 @@
             ["2t", "10u", "10v", "sp", "2d", "msdwswrf", "msdwlwrf", "lsrr", "crr"],
             ["t2m", "u10", "v10", "sp", "d2m", "msdwswrf", "msdwlwrf", "lsrr", "crr"],
         ):
             ## Load data from all relevant years
             years = [
                 i for i in range(self.date_range[0].year, self.date_range[1].year + 1)
             ]
-            # Loop through each year and read the corresponding files
-            for year in years:
-                ds = xr.open_mfdataset(
-                    f"{era5_path}/{fname}/{year}/{fname}*",
-                    decode_times=False,
-                    chunks={"longitude": 100, "latitude": 100},
-                )
-
-                ## Cut out this variable to our domain size
-                rawdata[fname] = longitude_slicer(
-                    ds,
-                    self.longitude_extent,
-                    "longitude",
-                ).sel(
-                    latitude=slice(
-                        self.longitude_extent[1], self.longitude_extent[0]
-                    )  ## This is because ERA5 has latitude in decreasing order (??)
-                )
-
-                ## Now fix up the latitude and time dimensions
-
-                rawdata[fname] = (
-                    rawdata[fname]
-                    .isel(latitude=slice(None, None, -1))  ## Flip latitude
-                    .assign_coords(
-                        time=np.arange(
-                            0, rawdata[fname].time.shape[0], dtype=float
-                        )  ## Set the zero date of forcing to start of run
-                    )
+            # construct a list of all paths for all years to use for open_mfdataset
+            paths_per_year = [Path(f"{era5_path}/{fname}/{year}/") for year in years]
+            all_files = []
+            for path in paths_per_year:
+                # Use glob to find all files that match the pattern
+                files = list(path.glob(f"{fname}*.nc"))
+                # Add the files to the all_files list
+                all_files.extend(files)
+
+            ds = xr.open_mfdataset(
+                all_files,
+                decode_times=False,
+                chunks={"longitude": 100, "latitude": 100},
+            )
+
+            ## Cut out this variable to our domain size
+            rawdata[fname] = longitude_slicer(
+                ds,
+                self.longitude_extent,
+                "longitude",
+            ).sel(
+                latitude=slice(
+                    self.latitude_extent[1], self.latitude_extent[0]
+                )  ## This is because ERA5 has latitude in decreasing order (??)
+            )
+
+            ## Now fix up the latitude and time dimensions
+
+            rawdata[fname] = (
+                rawdata[fname]
+                .isel(latitude=slice(None, None, -1))  ## Flip latitude
+                .assign_coords(
+                    time=np.arange(
+                        0, rawdata[fname].time.shape[0], dtype=float
+                    )  ## Set the zero date of forcing to start of run
+                )
+            )
+
+            rawdata[fname].time.attrs = {
+                "calendar": "julian",
+                "units": f"hours since {self.date_range[0].strftime('%Y-%m-%d %H:%M:%S')}",
+            }  ## Fix up calendar to match
+
+            if fname == "2d":
+                ## Calculate specific humidity from dewpoint temperature
+                dewpoint = 8.07131 - 1730.63 / (233.426 + rawdata["2d"]["d2m"] - 273.15)
+                humidity = (0.622 / rawdata["sp"]["sp"]) * (10**dewpoint) * 101325 / 760
+                q = xr.Dataset(data_vars={"q": humidity})
+
+                q.q.attrs = {"long_name": "Specific Humidity", "units": "kg/kg"}
+                q.to_netcdf(
+                    f"{self.mom_input_dir}/forcing/q_ERA5.nc",
+                    unlimited_dims="time",
+                    encoding={"q": {"dtype": "double"}},
+                )
+            elif fname == "crr":
+                ## Calculate total rain rate from convective and total
+                trr = xr.Dataset(
+                    data_vars={"trr": rawdata["crr"]["crr"] + rawdata["lsrr"]["lsrr"]}
+                )
+
+                trr.trr.attrs = {
+                    "long_name": "Total Rain Rate",
+                    "units": "kg m**-2 s**-1",
+                }
+                trr.to_netcdf(
+                    f"{self.mom_input_dir}/forcing/trr_ERA5.nc",
+                    unlimited_dims="time",
+                    encoding={"trr": {"dtype": "double"}},
                 )
 
-                rawdata[fname].time.attrs = {
-                    "calendar": "julian",
-                    "units": f"hours since {self.date_range[0].strftime('%Y-%m-%d %H:%M:%S')}",
-                }  ## Fix up calendar to match
-
-                if fname == "2d":
-                    ## Calculate specific humidity from dewpoint temperature
-                    dewpoint = 8.07131 - 1730.63 / (
-                        233.426 + rawdata["2d"]["d2m"] - 273.15
-                    )
-                    humidity = (
-                        (0.622 / rawdata["sp"]["sp"]) * (10**dewpoint) * 101325 / 760
-                    )
-                    q = xr.Dataset(data_vars={"q": humidity})
-
-                    q.q.attrs = {"long_name": "Specific Humidity", "units": "kg/kg"}
-                    q.to_netcdf(
-                        f"{self.mom_input_dir}/forcing/q_ERA5.nc",
-                        unlimited_dims="time",
-                        encoding={"q": {"dtype": "double"}},
-                    )
-                elif fname == "crr":
-                    ## Calculate total rain rate from convective and total
-                    trr = xr.Dataset(
-                        data_vars={
-                            "trr": rawdata["crr"]["crr"] + rawdata["lsrr"]["lsrr"]
-                        }
-                    )
-
-                    trr.trr.attrs = {
-                        "long_name": "Total Rain Rate",
-                        "units": "kg m**-2 s**-1",
-                    }
-                    trr.to_netcdf(
-                        f"{self.mom_input_dir}/forcing/trr_ERA5-{year}.nc",
-                        unlimited_dims="time",
-                        encoding={"trr": {"dtype": "double"}},
-                    )
-
-                elif fname == "lsrr":
-                    ## This is handled by crr as both are added together to calculate total rain rate.
-                    pass
-                else:
-                    rawdata[fname].to_netcdf(
-                        f"{self.mom_input_dir}/forcing/{fname}_ERA5-{year}.nc",
-                        unlimited_dims="time",
-                        encoding={vname: {"dtype": "double"}},
-                    )
+            elif fname == "lsrr":
+                ## This is handled by crr as both are added together to calculate total rain rate.
+                pass
+            else:
+                rawdata[fname].to_netcdf(
+                    f"{self.mom_input_dir}/forcing/{fname}_ERA5.nc",
+                    unlimited_dims="time",
+                    encoding={vname: {"dtype": "double"}},
+                )
 
 
 class segment:
     """
     Class to turn raw boundary segment data into MOM6 boundary
     segments.
 
@@ -1632,61 +1663,64 @@
     segment. No horizontal chunking is done here, so big fat segments
     will process slowly.
 
     Data should be at daily temporal resolution, iterating upwards
     from the provided startdate. Function ignores the time metadata
     and puts it on Julian calendar.
 
-    Only supports z-star (z*) vertical coordinate!
+    Note:
+        Only supports z-star (z*) vertical coordinate.
 
     Args:
         hgrid (xarray.Dataset): The horizontal grid used for domain.
         infile (Union[str, Path]): Path to the raw, unprocessed boundary segment.
         outfolder (Union[str, Path]): Path to folder where the model inputs will
             be stored.
         varnames (Dict[str, str]): Mapping between the variable/dimension names and
-            standard naming convension of this pipeline, e.g., ``{"xq": "longitude,
+            standard naming convention of this pipeline, e.g., ``{"xq": "longitude,
             "yh": "latitude", "salt": "salinity", ...}``. Key "tracers" points to nested
             dictionary of tracers to include in boundary.
-        seg_name (str): Name of the segment, e.g., ``'segment_001'``.
-        orientation (str): Cardinal direction (lowercase) of the boundary segment.
+        segment_name (str): Name of the segment, e.g., ``'segment_001'``.
+        orientation (str): Cardinal direction (lowercase) of the boundary segment,
+            i.e., ``'east'``, ``'west'``, ``'north'``, or ``'south'``.
         startdate (str): The starting date to use in the segment calendar.
-        gridtype (Optional[str]): Arakawa staggering of input grid, one of ``'A'``, ``'B'``,
-            or ``'C'``
+        arakawa_grid (Optional[str]): Arakawa grid staggering type of the boundary forcing.
+                Either ``'A'`` (default), ``'B'``, or ``'C'``.
         time_units (str): The units used by the raw forcing files, e.g., ``hours``,
             ``days`` (default).
         tidal_constituents (Optional[int]): An integer determining the number of tidal
             constituents to be included from the list: *M*:sub:`2`, *S*:sub:`2`, *N*:sub:`2`,
             *K*:sub:`2`, *K*:sub:`1`, *O*:sub:`2`, *P*:sub:`1`, *Q*:sub:`1`, *Mm*,
             *Mf*, and *M*:sub:`4`. For example, specifying ``1`` only includes *M*:sub:`2`;
             specifying ``2`` includes *M*:sub:`2` and *S*:sub:`2`, etc. Default: ``None``.
         repeat_year_forcing (Optional[bool]): When ``True`` the experiment runs with repeat-year
             forcing. When ``False`` (default) then inter-annual forcing is used.
     """
 
     def __init__(
         self,
+        *,
         hgrid,
         infile,
         outfolder,
         varnames,
-        seg_name,
+        segment_name,
         orientation,
         startdate,
-        gridtype="A",
+        arakawa_grid="A",
         time_units="days",
         tidal_constituents=None,
         repeat_year_forcing=False,
     ):
         ## Store coordinate names
-        if gridtype == "A":
+        if arakawa_grid == "A":
             self.x = varnames["x"]
             self.y = varnames["y"]
 
-        elif gridtype in ("B", "C"):
+        elif arakawa_grid in ("B", "C"):
             self.xq = varnames["xq"]
             self.xh = varnames["xh"]
             self.yq = varnames["yq"]
             self.yh = varnames["yh"]
 
         ## Store velocity names
         self.u = varnames["u"]
@@ -1697,28 +1731,36 @@
         self.startdate = startdate
 
         ## Store tracer names
         self.tracers = varnames["tracers"]
         self.time_units = time_units
 
         ## Store other data
+        orientation = orientation.lower()
+        if orientation not in ("north", "south", "east", "west"):
+            raise ValueError(
+                "orientation must be one of: 'north', 'south', 'east', or 'west'"
+            )
+        self.orientation = orientation
+
+        if arakawa_grid not in ("A", "B", "C"):
+            raise ValueError("arakawa_grid must be one of: 'A', 'B', or 'C'")
+        self.arakawa_grid = arakawa_grid
+
         self.infile = infile
         self.outfolder = outfolder
-        self.orientation = orientation.lower()  ## might not be needed? NSEW
-        self.grid = gridtype
         self.hgrid = hgrid
-        self.seg_name = seg_name
+        self.segment_name = segment_name
         self.tidal_constituents = tidal_constituents
         self.repeat_year_forcing = repeat_year_forcing
 
     def rectangular_brushcut(self):
         """
-        Cut out and interpolates tracers. This method assumes that the boundary
-        is a simple Northern, Southern, Eastern, or Western boundary. Cuts out
-        and interpolates tracers.
+        Cut out and interpolate tracers. ``rectangular_brushcut`` assumes that the boundary
+        is a simple Northern, Southern, Eastern, or Western boundary.
         """
         if self.orientation == "north":
             self.hgrid_seg = self.hgrid.isel(nyp=[-1])
             self.perpendicular = "ny"
             self.parallel = "nx"
 
         if self.orientation == "south":
@@ -1742,27 +1784,27 @@
         else:
             self.axis_to_expand = 3
 
         ## Grid for interpolating our fields
         self.interp_grid = xr.Dataset(
             {
                 "lat": (
-                    [f"{self.parallel}_{self.seg_name}"],
+                    [f"{self.parallel}_{self.segment_name}"],
                     self.hgrid_seg.y.squeeze().data,
                 ),
                 "lon": (
-                    [f"{self.parallel}_{self.seg_name}"],
+                    [f"{self.parallel}_{self.segment_name}"],
                     self.hgrid_seg.x.squeeze().data,
                 ),
             }
         ).set_coords(["lat", "lon"])
 
         rawseg = xr.open_dataset(self.infile, decode_times=False, engine="netcdf4")
 
-        if self.grid == "A":
+        if self.arakawa_grid == "A":
             rawseg = rawseg.rename({self.x: "lon", self.y: "lat"})
             ## In this case velocities and tracers all on same points
             regridder = xe.Regridder(
                 rawseg[self.u],
                 self.interp_grid,
                 "bilinear",
                 locstream_out=True,
@@ -1778,15 +1820,15 @@
                             [self.u, self.v, self.eta]
                             + [self.tracers[i] for i in self.tracers]
                         ]
                     )
                 ]
             )
 
-        if self.grid == "B":
+        if self.arakawa_grid == "B":
             ## All tracers on one grid, all velocities on another
             regridder_velocity = xe.Regridder(
                 rawseg[self.u].rename({self.xq: "lon", self.yq: "lat"}),
                 self.interp_grid,
                 "bilinear",
                 locstream_out=True,
                 reuse_weights=False,
@@ -1815,15 +1857,15 @@
                         rawseg[
                             [self.eta] + [self.tracers[i] for i in self.tracers]
                         ].rename({self.xh: "lon", self.yh: "lat"})
                     ),
                 ]
             )
 
-        if self.grid == "C":
+        if self.arakawa_grid == "C":
             ## All tracers on one grid, all velocities on another
             regridder_uvelocity = xe.Regridder(
                 rawseg[self.u].rename({self.xq: "lon", self.yh: "lat"}),
                 self.interp_grid,
                 "bilinear",
                 locstream_out=True,
                 reuse_weights=False,
@@ -1872,17 +1914,17 @@
             > 100
         ):
             segment_out[self.tracers["temp"]] -= 273.15
 
         # fill in NaNs
         segment_out = (
             segment_out.ffill(self.z)
-            .interpolate_na(f"{self.parallel}_{self.seg_name}")
-            .ffill(f"{self.parallel}_{self.seg_name}")
-            .bfill(f"{self.parallel}_{self.seg_name}")
+            .interpolate_na(f"{self.parallel}_{self.segment_name}")
+            .ffill(f"{self.parallel}_{self.segment_name}")
+            .bfill(f"{self.parallel}_{self.segment_name}")
         )
 
         time = np.arange(
             0,  #! Indexing everything from start of experiment = simple but maybe counterintutive?
             segment_out[self.time].shape[
                 0
             ],  ## Time is indexed from start date of window
@@ -1895,62 +1937,68 @@
             "units": f"{self.time_units} since {self.startdate}",
         }
         # Dictionary we built for encoding the netcdf at end
         encoding_dict = {
             "time": {
                 "dtype": "double",
             },
-            f"nx_{self.seg_name}": {
+            f"nx_{self.segment_name}": {
                 "dtype": "int32",
             },
-            f"ny_{self.seg_name}": {
+            f"ny_{self.segment_name}": {
                 "dtype": "int32",
             },
         }
 
-        ### Generate our dz variable. This needs to be in layer thicknesses
+        ### Generate the dz variable; needs to be in layer thicknesses
         dz = segment_out[self.z].diff(self.z)
         dz.name = "dz"
         dz = xr.concat([dz, dz[-1]], dim=self.z)
 
-        # Here, keep in mind that 'var' keeps track of the mom6 variable names we want, and self.tracers[var] will return the name of the variable from the original data
+        # Here, keep in mind that 'var' keeps track of the mom6 variable names we want, and self.tracers[var]
+        # will return the name of the variable from the original data
 
         allfields = {
             **self.tracers,
             "u": self.u,
             "v": self.v,
         }  ## Combine all fields into one flattened dictionary to iterate over as we fix metadata
 
         for (
             var
         ) in (
             allfields
         ):  ## Replace with more generic list of tracer variables that might be included?
-            v = f"{var}_{self.seg_name}"
+            v = f"{var}_{self.segment_name}"
             ## Rename each variable in dataset
             segment_out = segment_out.rename({allfields[var]: v})
 
             ## Rename vertical coordinate for this variable
-            segment_out[f"{var}_{self.seg_name}"] = segment_out[
-                f"{var}_{self.seg_name}"
-            ].rename({self.z: f"nz_{self.seg_name}_{var}"})
+            segment_out[f"{var}_{self.segment_name}"] = segment_out[
+                f"{var}_{self.segment_name}"
+            ].rename({self.z: f"nz_{self.segment_name}_{var}"})
 
             ## Replace the old depth coordinates with incremental integers
-            segment_out[f"nz_{self.seg_name}_{var}"] = np.arange(
-                segment_out[f"nz_{self.seg_name}_{var}"].size
+            segment_out[f"nz_{self.segment_name}_{var}"] = np.arange(
+                segment_out[f"nz_{self.segment_name}_{var}"].size
             )
 
             ## Re-add the secondary dimension (even though it represents one value..)
             segment_out[v] = segment_out[v].expand_dims(
-                f"{self.perpendicular}_{self.seg_name}", axis=self.axis_to_expand
+                f"{self.perpendicular}_{self.segment_name}", axis=self.axis_to_expand
             )
 
             ## Add the layer thicknesses
             segment_out[f"dz_{v}"] = (
-                ["time", f"nz_{v}", f"ny_{self.seg_name}", f"nx_{self.seg_name}"],
+                [
+                    "time",
+                    f"nz_{v}",
+                    f"ny_{self.segment_name}",
+                    f"nx_{self.segment_name}",
+                ],
                 da.broadcast_to(
                     dz.data[None, :, None, None],
                     segment_out[v].shape,
                     chunks=(
                         1,
                         None,
                         None,
@@ -1967,56 +2015,56 @@
             encoding_dict[f"dz_{v}"] = {
                 "_FillValue": netCDF4.default_fillvals["f8"],
                 "zlib": True,
                 # "chunksizes": tuple(s),
             }
 
             ## appears to be another variable just with integers??
-            encoding_dict[f"nz_{self.seg_name}_{var}"] = {"dtype": "int32"}
+            encoding_dict[f"nz_{self.segment_name}_{var}"] = {"dtype": "int32"}
 
         ## Treat eta separately since it has no vertical coordinate. Do the same things as for the surface variables above
-        segment_out = segment_out.rename({self.eta: f"eta_{self.seg_name}"})
-        encoding_dict[f"eta_{self.seg_name}"] = {
+        segment_out = segment_out.rename({self.eta: f"eta_{self.segment_name}"})
+        encoding_dict[f"eta_{self.segment_name}"] = {
             "_FillValue": netCDF4.default_fillvals["f8"],
         }
-        segment_out[f"eta_{self.seg_name}"] = segment_out[
-            f"eta_{self.seg_name}"
+        segment_out[f"eta_{self.segment_name}"] = segment_out[
+            f"eta_{self.segment_name}"
         ].expand_dims(
-            f"{self.perpendicular}_{self.seg_name}", axis=self.axis_to_expand - 1
+            f"{self.perpendicular}_{self.segment_name}", axis=self.axis_to_expand - 1
         )
 
         # Overwrite the actual lat/lon values in the dimensions, replace with incrementing integers
-        segment_out[f"{self.parallel}_{self.seg_name}"] = np.arange(
-            segment_out[f"{self.parallel}_{self.seg_name}"].size
+        segment_out[f"{self.parallel}_{self.segment_name}"] = np.arange(
+            segment_out[f"{self.parallel}_{self.segment_name}"].size
         )
-        segment_out[f"{self.perpendicular}_{self.seg_name}"] = [0]
+        segment_out[f"{self.perpendicular}_{self.segment_name}"] = [0]
 
         # Store actual lat/lon values here as variables rather than coordinates
-        segment_out[f"lon_{self.seg_name}"] = (
-            [f"ny_{self.seg_name}", f"nx_{self.seg_name}"],
+        segment_out[f"lon_{self.segment_name}"] = (
+            [f"ny_{self.segment_name}", f"nx_{self.segment_name}"],
             self.hgrid_seg.x.data,
         )
-        segment_out[f"lat_{self.seg_name}"] = (
-            [f"ny_{self.seg_name}", f"nx_{self.seg_name}"],
+        segment_out[f"lat_{self.segment_name}"] = (
+            [f"ny_{self.segment_name}", f"nx_{self.segment_name}"],
             self.hgrid_seg.y.data,
         )
 
         # Add units to the lat / lon to keep the `categorize_axis_from_units` checker happy
-        segment_out[f"lat_{self.seg_name}"].attrs = {
+        segment_out[f"lat_{self.segment_name}"].attrs = {
             "units": "degrees_north",
         }
-        segment_out[f"lon_{self.seg_name}"].attrs = {
+        segment_out[f"lon_{self.segment_name}"].attrs = {
             "units": "degrees_east",
         }
 
         # If repeat-year forcing, add modulo coordinate
         if self.repeat_year_forcing:
             segment_out["time"] = segment_out["time"].assign_attrs({"modulo": " "})
 
         with ProgressBar():
             segment_out.load().to_netcdf(
-                self.outfolder / f"forcing/forcing_obc_{self.seg_name}.nc",
+                self.outfolder / f"forcing/forcing_obc_{self.segment_name}.nc",
                 encoding=encoding_dict,
                 unlimited_dims="time",
             )
 
         return segment_out, encoding_dict
```

### Comparing `regional_mom6-0.5.0/regional_mom6/utils.py` & `regional_mom6-0.5.1/regional_mom6/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 
 def vecdot(v1, v2):
     """Return the dot product of vectors ``v1`` and ``v2``.
     ``v1`` and ``v2`` can be either numpy vectors or numpy.ndarrays
     in which case the last dimension is considered the dimension
-    over which the dot product is taken of.
+    over which the dot product is taken.
     """
     return np.sum(v1 * v2, axis=-1)
 
 
 def angle_between(v1, v2, v3):
     """Return the angle ``v2``-``v1``-``v3`` (in radians), where
     ``v1``, ``v2``, ``v3`` are 3-vectors. That is, the angle that
@@ -84,15 +84,15 @@
     a3 = angle_between(v3, v4, v2)
     a4 = angle_between(v4, v1, v3)
 
     return (a1 + a2 + a3 + a4 - 2 * np.pi) * R**2
 
 
 def latlon_to_cartesian(lat, lon, R=1):
-    """Convert latitude-longitude (in degrees) to Cartesian coordinates on
+    """Convert latitude and longitude (in degrees) to Cartesian coordinates on
     a sphere of radius ``R``. By default ``R = 1``.
 
     Args:
         lat (float): Latitude (in degrees).
         lon (float): Longitude (in degrees).
         R (float): The radius of the sphere; default: 1.
 
@@ -132,15 +132,15 @@
         lat (numpy.array): Array of latitude points (in degrees).
         lon (numpy.array): Array of longitude points (in degrees).
         R (float): The radius of the sphere; default: 1.
 
     Returns:
         numpy.array: Array with the areas of the quadrilaterals defined by the ``lat``-``lon`` grid
         provided. If the provided ``lat``, ``lon`` arrays are of dimension *m* :math:`\\times` *n*
-        then return areas array is of dimension (*m-1*) :math:`\\times` (*n-1*).
+        then returned areas array is of dimension (*m-1*) :math:`\\times` (*n-1*).
 
     Example:
 
         Let's construct a lat-lon grid on the sphere with 60 degree spacing.
         Then we compute the areas of each grid cell and confirm that the
         sum of the areas gives us the total area of the sphere.
```

### Comparing `regional_mom6-0.5.0/regional_mom6.egg-info/SOURCES.txt` & `regional_mom6-0.5.1/regional_mom6.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 .gitignore
 .readthedocs.yaml
 LICENSE
 README.md
 codecov.yml
 environment-ci.yml
 pyproject.toml
+.github/workflows/package.yml
 .github/workflows/testing.yml
-demos/access_om2-forced.ipynb
 demos/reanalysis-forced.ipynb
-demos/premade_run_directories/readme_premade_rundirs.md
+demos/premade_run_directories/README.md
 demos/premade_run_directories/common_files/MOM_input
 demos/premade_run_directories/common_files/MOM_layout
 demos/premade_run_directories/common_files/MOM_override
 demos/premade_run_directories/common_files/SIS_input
 demos/premade_run_directories/common_files/config.yaml
 demos/premade_run_directories/common_files/data_table
 demos/premade_run_directories/common_files/diag_table
@@ -26,14 +26,15 @@
 docs/api.rst
 docs/conf.py
 docs/contributing.md
 docs/demo_notebooks
 docs/demos.rst
 docs/index.rst
 docs/installation.md
+docs/mom6-file-structure-primer.md
 docs/requirements.txt
 regional_mom6/__init__.py
 regional_mom6/_version.py
 regional_mom6/regional_mom6.py
 regional_mom6/utils.py
 regional_mom6.egg-info/PKG-INFO
 regional_mom6.egg-info/SOURCES.txt
```

### Comparing `regional_mom6-0.5.0/tests/test_expt_class.py` & `regional_mom6-0.5.1/tests/test_expt_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
         "v": "v",
         "tracers": {"temp": "temp", "salt": "salt"},
     }
 
     expt.initial_condition(
         tmp_path / "ic_unprocessed",
         varnames,
-        gridtype="A",
+        arakawa_grid="A",
     )
 
 
 @pytest.mark.parametrize(
     (
         "longitude_extent",
         "latitude_extent",
```

### Comparing `regional_mom6-0.5.0/tests/test_grid_generation.py` & `regional_mom6-0.5.1/tests/test_grid_generation.py`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.0/tests/test_utils.py` & `regional_mom6-0.5.1/tests/test_utils.py`

 * *Files identical despite different names*

