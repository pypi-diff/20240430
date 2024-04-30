# Comparing `tmp/cellmaps_vnn-0.1.0a1.tar.gz` & `tmp/cellmaps_vnn-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_vnn-0.1.0a1.tar", last modified: Fri Feb  2 00:21:16 2024, max compression
+gzip compressed data, was "cellmaps_vnn-0.1.0a2.tar", last modified: Tue Apr 30 05:56:58 2024, max compression
```

## Comparing `cellmaps_vnn-0.1.0a1.tar` & `cellmaps_vnn-0.1.0a2.tar`

### file list

```diff
@@ -1,64 +1,84 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-02 00:21:16.435412 cellmaps_vnn-0.1.0a1/
--rw-r--r--   0 churas     (504) staff       (20)      172 2024-02-02 00:14:29.000000 cellmaps_vnn-0.1.0a1/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3587 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2024-02-02 00:15:21.000000 cellmaps_vnn-0.1.0a1/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     5798 2024-02-02 00:21:16.435712 cellmaps_vnn-0.1.0a1/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     3706 2024-02-02 00:19:31.000000 cellmaps_vnn-0.1.0a1/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-02 00:21:16.418526 cellmaps_vnn-0.1.0a1/cellmaps_vnn/
--rw-r--r--   0 churas     (504) staff       (20)      275 2024-02-02 00:14:29.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1478 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn/ccc_loss.py
--rw-r--r--   0 churas     (504) staff       (20)     4315 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn/cellmaps_vnncmd.py
--rw-r--r--   0 churas     (504) staff       (20)    10726 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn/data_wrapper.py
--rw-r--r--   0 churas     (504) staff       (20)      122 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    20232 2024-02-02 00:10:57.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn/predict.py
--rw-r--r--   0 churas     (504) staff       (20)     9260 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn/runner.py
--rw-r--r--   0 churas     (504) staff       (20)     8723 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn/train.py
--rw-r--r--   0 churas     (504) staff       (20)     8951 2024-02-02 00:10:57.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn/util.py
--rw-r--r--   0 churas     (504) staff       (20)     9627 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn/vnn.py
--rw-r--r--   0 churas     (504) staff       (20)    10614 2024-02-02 00:10:57.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn/vnn_trainer.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-02 00:21:16.420475 cellmaps_vnn-0.1.0a1/cellmaps_vnn.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     5798 2024-02-02 00:21:16.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1245 2024-02-02 00:21:16.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2024-02-02 00:21:16.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2024-02-02 00:21:16.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)      110 2024-02-02 00:21:16.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       13 2024-02-02 00:21:16.000000 cellmaps_vnn-0.1.0a1/cellmaps_vnn.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-02 00:21:16.429345 cellmaps_vnn-0.1.0a1/docs/
--rw-r--r--   0 churas     (504) staff       (20)      613 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-02 00:21:16.411233 cellmaps_vnn-0.1.0a1/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-02 00:21:16.411309 cellmaps_vnn-0.1.0a1/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-02 00:21:16.430611 cellmaps_vnn-0.1.0a1/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_vnn-0.1.0a1/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_vnn-0.1.0a1/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_vnn-0.1.0a1/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1735 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/docs/cellmaps_vnn.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6063 2024-01-10 17:45:14.000000 cellmaps_vnn-0.1.0a1/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      280 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      913 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1158 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      436 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      810 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       71 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4280 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)     1000 2024-02-02 00:20:57.000000 cellmaps_vnn-0.1.0a1/docs/outputs.rst
--rw-r--r--   0 churas     (504) staff       (20)      782 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)     4650 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      395 2024-02-02 00:21:16.437594 cellmaps_vnn-0.1.0a1/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2025 2024-02-02 00:10:57.000000 cellmaps_vnn-0.1.0a1/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-02 00:21:16.435036 cellmaps_vnn-0.1.0a1/tests/
--rw-r--r--   0 churas     (504) staff       (20)       67 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     2535 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/tests/test_cellmaps_vnncmd.py
--rw-r--r--   0 churas     (504) staff       (20)     1631 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/tests/test_cellmapsvnn.py
--rw-r--r--   0 churas     (504) staff       (20)     5223 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/tests/test_datawrapper.py
--rw-r--r--   0 churas     (504) staff       (20)      737 2023-12-01 21:33:00.000000 cellmaps_vnn-0.1.0a1/tests/test_integration_cellmaps_vnn.py
--rw-r--r--   0 churas     (504) staff       (20)     2642 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/tests/test_predict.py
--rw-r--r--   0 churas     (504) staff       (20)     3981 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/tests/test_util.py
--rw-r--r--   0 churas     (504) staff       (20)     3272 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/tests/test_vnn.py
--rw-r--r--   0 churas     (504) staff       (20)     1332 2024-01-10 17:33:26.000000 cellmaps_vnn-0.1.0a1/tests/test_vnntrainer.py
+drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-04-30 05:56:58.697681 cellmaps_vnn-0.1.0a2/
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      172 2024-03-18 21:50:44.000000 cellmaps_vnn-0.1.0a2/AUTHORS.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     3587 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/CONTRIBUTING.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)       89 2024-03-18 21:50:44.000000 cellmaps_vnn-0.1.0a2/HISTORY.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1102 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/LICENSE
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      262 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/MANIFEST.in
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     4932 2024-04-30 05:56:58.697614 cellmaps_vnn-0.1.0a2/PKG-INFO
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     3706 2024-03-18 21:50:44.000000 cellmaps_vnn-0.1.0a2/README.rst
+drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-04-30 05:56:58.690750 cellmaps_vnn-0.1.0a2/cellmaps_vnn/
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      275 2024-04-30 05:50:32.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn/__init__.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)    14051 2024-04-30 05:48:22.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn/annotate.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1478 2024-01-05 00:07:13.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn/ccc_loss.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     4552 2024-04-30 05:48:22.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn/cellmaps_vnncmd.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      164 2024-04-30 05:48:22.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn/constants.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)    10726 2024-01-05 00:07:13.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn/data_wrapper.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      122 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn/exceptions.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)    24309 2024-04-30 05:48:22.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn/predict.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)    13419 2024-04-30 05:48:22.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn/rlipp_calculator.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)    10411 2024-04-30 05:48:22.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn/runner.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     9821 2024-04-30 05:48:22.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn/train.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     8951 2024-01-11 19:38:46.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn/util.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     9627 2024-01-05 00:07:13.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn/vnn.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)    10614 2024-01-11 19:38:46.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn/vnn_trainer.py
+drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-04-30 05:56:58.691422 cellmaps_vnn-0.1.0a2/cellmaps_vnn.egg-info/
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     4932 2024-04-30 05:56:58.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn.egg-info/PKG-INFO
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1786 2024-04-30 05:56:58.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn.egg-info/SOURCES.txt
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)        1 2024-04-30 05:56:58.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn.egg-info/dependency_links.txt
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)        1 2024-04-30 05:56:58.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn.egg-info/not-zip-safe
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      161 2024-04-30 05:56:58.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn.egg-info/requires.txt
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)       13 2024-04-30 05:56:58.000000 cellmaps_vnn-0.1.0a2/cellmaps_vnn.egg-info/top_level.txt
+drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-04-30 05:56:58.694423 cellmaps_vnn-0.1.0a2/docs/
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      613 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/docs/Makefile
+drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-04-30 05:56:58.687714 cellmaps_vnn-0.1.0a2/docs/_build/
+drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-04-30 05:56:58.687830 cellmaps_vnn-0.1.0a2/docs/_build/html/
+drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-04-30 05:56:58.695031 cellmaps_vnn-0.1.0a2/docs/_build/html/_images/
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)   100448 2024-03-20 20:57:52.000000 cellmaps_vnn-0.1.0a2/docs/_build/html/_images/cellmaps_vnn_general.png
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)   249389 2024-03-20 20:57:52.000000 cellmaps_vnn-0.1.0a2/docs/_build/html/_images/nest_vnn.png
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)   195888 2024-03-20 20:57:52.000000 cellmaps_vnn-0.1.0a2/docs/_build/html/_images/nestvnn_pred.png
+drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-04-30 05:56:58.695546 cellmaps_vnn-0.1.0a2/docs/_build/html/_static/
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      286 2024-01-30 22:17:04.000000 cellmaps_vnn-0.1.0a2/docs/_build/html/_static/file.png
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)       90 2024-01-30 22:17:04.000000 cellmaps_vnn-0.1.0a2/docs/_build/html/_static/minus.png
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)       90 2024-01-30 22:17:04.000000 cellmaps_vnn-0.1.0a2/docs/_build/html/_static/plus.png
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)       28 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/docs/authors.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1735 2024-01-05 00:07:13.000000 cellmaps_vnn-0.1.0a2/docs/cellmaps_vnn.rst
+-rwxr-xr-x   0 jlenkiewicz   (503) staff       (20)     6098 2024-03-18 21:50:44.000000 cellmaps_vnn-0.1.0a2/docs/conf.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)       33 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/docs/contributing.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      174 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/docs/devbranches.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      280 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/docs/developer.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     2169 2024-04-30 05:48:22.000000 cellmaps_vnn-0.1.0a2/docs/example_usage_nest_vnn.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)       28 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/docs/history.rst
+drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-04-30 05:56:58.696045 cellmaps_vnn-0.1.0a2/docs/images/
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)   100448 2024-03-20 20:57:52.000000 cellmaps_vnn-0.1.0a2/docs/images/cellmaps_vnn_general.png
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)   249389 2024-03-20 20:57:52.000000 cellmaps_vnn-0.1.0a2/docs/images/nest_vnn.png
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)   195888 2024-03-20 20:57:52.000000 cellmaps_vnn-0.1.0a2/docs/images/nestvnn_pred.png
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1993 2024-03-20 20:57:52.000000 cellmaps_vnn-0.1.0a2/docs/index.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      178 2024-03-20 20:57:52.000000 cellmaps_vnn-0.1.0a2/docs/inputs.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      665 2024-04-30 05:48:22.000000 cellmaps_vnn-0.1.0a2/docs/inputs_general.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     4748 2024-04-30 05:48:22.000000 cellmaps_vnn-0.1.0a2/docs/inputs_nestvnn.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1158 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/docs/installation.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      436 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/docs/integrationtesting.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      810 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/docs/make.bat
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)       71 2024-03-28 19:22:52.000000 cellmaps_vnn-0.1.0a2/docs/modules.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     4280 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/docs/newrelease.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1523 2024-04-30 05:48:22.000000 cellmaps_vnn-0.1.0a2/docs/outputs.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      782 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/docs/pypircfile.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      434 2024-03-20 20:57:52.000000 cellmaps_vnn-0.1.0a2/docs/usage.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     6391 2024-04-30 05:48:22.000000 cellmaps_vnn-0.1.0a2/docs/usage_command_line.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)       90 2024-03-20 20:57:52.000000 cellmaps_vnn-0.1.0a2/docs/usage_programmatically.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)       83 2024-03-20 20:57:52.000000 cellmaps_vnn-0.1.0a2/docs/usage_via_docker.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      817 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/docs/versioningscheme.rst
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      395 2024-04-30 05:56:58.697945 cellmaps_vnn-0.1.0a2/setup.cfg
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     2133 2024-04-30 05:48:22.000000 cellmaps_vnn-0.1.0a2/setup.py
+drwxr-xr-x   0 jlenkiewicz   (503) staff       (20)        0 2024-04-30 05:56:58.697338 cellmaps_vnn-0.1.0a2/tests/
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)       67 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/tests/__init__.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1161 2024-04-30 05:48:22.000000 cellmaps_vnn-0.1.0a2/tests/test_annotate.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     2535 2024-01-05 00:07:13.000000 cellmaps_vnn-0.1.0a2/tests/test_cellmaps_vnncmd.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1631 2024-01-05 00:07:13.000000 cellmaps_vnn-0.1.0a2/tests/test_cellmapsvnn.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     5223 2024-04-25 22:51:02.000000 cellmaps_vnn-0.1.0a2/tests/test_datawrapper.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)      737 2023-12-05 00:02:56.000000 cellmaps_vnn-0.1.0a2/tests/test_integration_cellmaps_vnn.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     2642 2024-01-05 00:07:13.000000 cellmaps_vnn-0.1.0a2/tests/test_predict.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     7675 2024-04-30 05:48:22.000000 cellmaps_vnn-0.1.0a2/tests/test_rlipp_calculator.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     3981 2024-01-05 00:07:13.000000 cellmaps_vnn-0.1.0a2/tests/test_util.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     3272 2024-01-05 00:07:13.000000 cellmaps_vnn-0.1.0a2/tests/test_vnn.py
+-rw-r--r--   0 jlenkiewicz   (503) staff       (20)     1332 2024-01-05 00:07:13.000000 cellmaps_vnn-0.1.0a2/tests/test_vnntrainer.py
```

### Comparing `cellmaps_vnn-0.1.0a1/CONTRIBUTING.rst` & `cellmaps_vnn-0.1.0a2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/LICENSE` & `cellmaps_vnn-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/README.rst` & `cellmaps_vnn-0.1.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/cellmaps_vnn/ccc_loss.py` & `cellmaps_vnn-0.1.0a2/cellmaps_vnn/ccc_loss.py`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/cellmaps_vnn/cellmaps_vnncmd.py` & `cellmaps_vnn-0.1.0a2/cellmaps_vnn/cellmaps_vnncmd.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import argparse
 import sys
 import logging
 import logging.config
 from cellmaps_utils import logutils
 from cellmaps_utils import constants
 import cellmaps_vnn
+from cellmaps_vnn.annotate import VNNAnnotate
 from cellmaps_vnn.predict import VNNPredict
 from cellmaps_vnn.runner import CellmapsvnnRunner
 from cellmaps_vnn.train import VNNTrain
 
 logger = logging.getLogger(__name__)
 
 
@@ -28,14 +29,15 @@
     parser = argparse.ArgumentParser(description=desc,
                                      formatter_class=constants.ArgParseFormatter)
     subparsers = parser.add_subparsers(dest='command', help='Command to run. Type <command> -h for more help')
     subparsers.required = True
 
     VNNTrain.add_subparser(subparsers)
     VNNPredict.add_subparser(subparsers)
+    VNNAnnotate.add_subparser(subparsers)
     parser.add_argument('--logconf', default=None,
                         help='Path to python logging configuration file in '
                              'this format: https://docs.python.org/3/library/'
                              'logging.config.html#logging-config-fileformat '
                              'Setting this overrides -v parameter which uses '
                              ' default logger. (default None)')
     parser.add_argument('--exitcode', help='Exit code this command will return',
@@ -86,14 +88,17 @@
     try:
         logutils.setup_cmd_logging(theargs)
 
         if theargs.command == VNNTrain.COMMAND:
             cmd = VNNTrain(theargs)
         elif theargs.command == VNNPredict.COMMAND:
             cmd = VNNPredict(theargs)
+        elif theargs.command == VNNAnnotate.COMMAND:
+            cmd = VNNAnnotate(theargs)
+            theargs.inputdir = theargs.model_predictions
         else:
             raise Exception('Invalid command: ' + str(theargs.command))
 
         runner = CellmapsvnnRunner(outdir=theargs.outdir,
                                    command=cmd,
                                    inputdir=theargs.inputdir,
                                    exitcode=theargs.exitcode,
```

### Comparing `cellmaps_vnn-0.1.0a1/cellmaps_vnn/data_wrapper.py` & `cellmaps_vnn-0.1.0a2/cellmaps_vnn/data_wrapper.py`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/cellmaps_vnn/predict.py` & `cellmaps_vnn-0.1.0a2/cellmaps_vnn/predict.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import os
 import logging
+import shutil
 from datetime import date
 from tqdm import tqdm
 import numpy as np
 import pandas as pd
 import torch
 import torch.utils.data as du
 from torch.autograd import Variable
 from cellmaps_utils import constants
+import cellmaps_vnn.constants as vnnconstants
+from ndex2.cx2 import RawCX2NetworkFactory
 
 import cellmaps_vnn
 from cellmaps_vnn import util
 from cellmaps_vnn.exceptions import CellmapsvnnError
+from cellmaps_vnn.rlipp_calculator import RLIPPCalculator
 
 logger = logging.getLogger(__name__)
 
 
 class VNNPredict:
     COMMAND = 'predict'
 
@@ -53,14 +57,19 @@
         parser.add_argument('--cn_amplifications', required=True, help='Copy number amplifications for cell lines',
                             type=str)
         parser.add_argument('--batchsize', help='Batchsize', type=int, default=1000)
         parser.add_argument('--cuda', help='Specify GPU', type=int, default=0)
         parser.add_argument('--zscore_method', help='zscore method (zscore/robustz)', type=str, default='auc')
         parser.add_argument('--std', help='Standardization File (if not set standardization file from RO-Crate '
                                           'will be used)', type=str)
+        parser.add_argument('--cpu_count', help='No of available cores', type=int, default=1)
+        parser.add_argument('--drug_count', help='No of top performing drugs', type=int, default=0)
+        parser.add_argument('--genotype_hiddens',
+                            help='Mapping for the number of neurons in each term in genotype parts', type=int,
+                            default=4)
         return parser
 
     def run(self):
         """
         The logic for running predictions with the model. It executes the prediction process
         using the trained model and input data.
 
@@ -83,14 +92,26 @@
             if not os.path.exists(hidden_dir):
                 os.mkdir(hidden_dir)
 
             # Perform prediction
             self.predict(predict_data, model, hidden_dir, self._theargs.batchsize,
                          cell_features)
 
+            hierarchy_file = os.path.join(self._theargs.inputdir, 'hierarchy.cx2')
+            factory = RawCX2NetworkFactory()
+            hierarchy = factory.get_cx2network(hierarchy_file)
+            rlipp_file = os.path.join(self._theargs.outdir, vnnconstants.RLIPP_OUTPUT_FILE)
+            gene_rho_file = os.path.join(self._theargs.outdir, 'gene_rho.out')
+            # Perform interpretation
+            calc = RLIPPCalculator(hierarchy, self._theargs.predict_data, self._get_predict_dest_file(),
+                                   self._theargs.gene2id, self._theargs.cell2id, hidden_dir,
+                                   rlipp_file, gene_rho_file, self._theargs.cpu_count, self._theargs.genotype_hiddens,
+                                   self._theargs.drug_count)
+            calc.calc_scores()
+
         except Exception as e:
             logger.error(f"Error in prediction flow: {e}")
             raise CellmapsvnnError(f"Encountered problem in prediction flow: {e}")
 
     def _prepare_predict_data(self, test_file, cell2id_mapping_file, zscore_method, std_file):
         """
         Prepares the prediction data for the model.
@@ -341,14 +362,15 @@
         :return: A list of dataset IDs for the registered files.
         """
         output_ids = list()
         output_ids.append(self._register_predict_file(outdir, description, keywords, provenance_utils))
         for i in range(self._number_feature_grads):
             output_ids.append(self._register_feature_grad_file(outdir, description, keywords, provenance_utils, i))
         output_ids.extend(self._register_hidden_files(outdir, description, keywords, provenance_utils))
+        output_ids.append(self._copy_and_register_hierarchy(outdir, description, keywords, provenance_utils))
         return output_ids
 
     def _register_predict_file(self, outdir, description, keywords, provenance_utils):
         """
         Registers the prediction result file with the FAIRSCAPE service for data provenance.
 
         :param outdir: The output directory where the outputs are stored.
@@ -436,7 +458,53 @@
             hidden_files_ids.append(dataset_id)
             cntr += 1
             if cntr > 5:
                 # Todo: https://github.com/fairscape/fairscape-cli/issues/9
                 logger.error('FAIRSCAPE cannot handle too many files, skipping rest')
                 break
         return hidden_files_ids
+
+    def _copy_and_register_hierarchy(self, outdir, description, keywords, provenance_utils):
+        hierarchy_out_file = os.path.join(outdir, 'hierarchy.cx2')
+        shutil.copy(os.path.join(self._theargs.inputdir, 'hierarchy.cx2'), hierarchy_out_file)
+
+        data_dict = {'name': os.path.basename(hierarchy_out_file) + ' Hierarchy network file',
+                     'description': description + ' Hierarchy network file',
+                     'keywords': keywords,
+                     'data-format': 'CX2',
+                     'author': cellmaps_vnn.__name__,
+                     'version': cellmaps_vnn.__version__,
+                     'date-published': date.today().strftime('%m-%d-%Y')}
+        dataset_id = provenance_utils.register_dataset(outdir,
+                                                       source_file=hierarchy_out_file,
+                                                       data_dict=data_dict)
+        return dataset_id
+
+    def _register_rlipp_file(self, outdir, description, keywords, provenance_utils):
+        rlipp_file = os.path.join(outdir, vnnconstants.RLIPP_OUTPUT_FILE)
+
+        data_dict = {'name': os.path.basename(rlipp_file) + ' RLIPP output file',
+                     'description': description + ' RLIPP output file',
+                     'keywords': keywords,
+                     'data-format': 'txt',
+                     'author': cellmaps_vnn.__name__,
+                     'version': cellmaps_vnn.__version__,
+                     'date-published': date.today().strftime('%m-%d-%Y')}
+        dataset_id = provenance_utils.register_dataset(outdir,
+                                                       source_file=rlipp_file,
+                                                       data_dict=data_dict)
+        return dataset_id
+
+    def _register_gene_rho_file(self, outdir, description, keywords, provenance_utils):
+        gene_rho_file = os.path.join(outdir, 'gene_rho.out')
+
+        data_dict = {'name': os.path.basename(gene_rho_file) + ' Gene Rho file',
+                     'description': description + ' Gene Rho file',
+                     'keywords': keywords,
+                     'data-format': 'txt',
+                     'author': cellmaps_vnn.__name__,
+                     'version': cellmaps_vnn.__version__,
+                     'date-published': date.today().strftime('%m-%d-%Y')}
+        dataset_id = provenance_utils.register_dataset(outdir,
+                                                       source_file=gene_rho_file,
+                                                       data_dict=data_dict)
+        return dataset_id
```

### Comparing `cellmaps_vnn-0.1.0a1/cellmaps_vnn/runner.py` & `cellmaps_vnn-0.1.0a2/cellmaps_vnn/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #! /usr/bin/env python
 
 import os
 import time
 import logging
-from cellmaps_utils import logutils
+from cellmaps_utils import logutils, constants
 from cellmaps_utils.provenance import ProvenanceUtil
 
 import cellmaps_vnn
 from cellmaps_vnn.exceptions import CellmapsvnnError
 
 logger = logging.getLogger(__name__)
 
@@ -67,35 +67,51 @@
 
     def _update_provenance_fields(self):
         """
         Updates the provenance attributes by merging the ROCrate provenance attributes
         from the input directory with optional overrides for the name, project name, and organization name
         and additional keywords.
         """
-        prov_attrs = self._provenance_utils.get_merged_rocrate_provenance_attrs(self._inputdir,
-                                                                                override_name=self._name,
-                                                                                override_project_name=
-                                                                                self._project_name,
-                                                                                override_organization_name=
-                                                                                self._organization_name,
-                                                                                extra_keywords=[
-                                                                                    'VNN',
-                                                                                    'Visible Neural Network',
-                                                                                    self._command.COMMAND
-                                                                                ])
-        if self._name is None:
-            self._name = prov_attrs.get_name()
-
-        if self._organization_name is None:
-            self._organization_name = prov_attrs.get_organization_name()
-
-        if self._project_name is None:
-            self._project_name = prov_attrs.get_project_name()
-        self._keywords = prov_attrs.get_keywords()
-        self._description = prov_attrs.get_description()
+        rocrate_dirs = []
+        dirs = []
+        if isinstance(self._inputdir, str):
+            dirs = [self._inputdir]
+        elif isinstance(self._inputdir, list):
+            dirs = self._inputdir
+        for entry in dirs:
+            if os.path.exists(os.path.join(entry, constants.RO_CRATE_METADATA_FILE)):
+                rocrate_dirs.append(entry)
+        if len(rocrate_dirs) > 0:
+            prov_attrs = self._provenance_utils.get_merged_rocrate_provenance_attrs(rocrate_dirs,
+                                                                                    override_name=self._name,
+                                                                                    override_project_name=
+                                                                                    self._project_name,
+                                                                                    override_organization_name=
+                                                                                    self._organization_name,
+                                                                                    extra_keywords=[
+                                                                                        'VNN',
+                                                                                        'Visible Neural Network',
+                                                                                        self._command.COMMAND
+                                                                                    ])
+            if self._name is None:
+                self._name = prov_attrs.get_name()
+
+            if self._organization_name is None:
+                self._organization_name = prov_attrs.get_organization_name()
+
+            if self._project_name is None:
+                self._project_name = prov_attrs.get_project_name()
+            self._keywords = prov_attrs.get_keywords()
+            self._description = prov_attrs.get_description()
+        else:
+            self._name = 'VNN tool'
+            self._organization_name = 'Example'
+            self._project_name = 'Example'
+            self._keywords = ['vnn']
+            self._description = 'Example input dataset VNN'
 
     def _create_rocrate(self):
         """
         Creates rocrate for output directory
 
         :raises CellMapsProvenanceError: If there is an error
         """
@@ -137,22 +153,30 @@
 
         :param generated_dataset_ids: List of IDs for the datasets generated during the computation.
         :type generated_dataset_ids: list
         # Todo: added in used dataset, software and what is being generated
         :return:
         """
         logger.debug('Getting id of input rocrate')
-        input_dataset_id = self._provenance_utils.get_id_of_rocrate(self._inputdir)
+        used_dataset = []
+        if isinstance(self._inputdir, str):
+            if os.path.exists(os.path.join(self._inputdir, constants.RO_CRATE_METADATA_FILE)):
+                used_dataset = [self._provenance_utils.get_id_of_rocrate(self._inputdir)]
+        elif isinstance(self._inputdir, list):
+            for entry in self._inputdir:
+                if os.path.exists(os.path.join(entry, constants.RO_CRATE_METADATA_FILE)):
+                    used_dataset.append(self._provenance_utils.get_id_of_rocrate(entry))
+
         self._provenance_utils.register_computation(self._outdir,
                                                     name=cellmaps_vnn.__name__ + ' computation',
                                                     run_by=str(self._provenance_utils.get_login()),
                                                     command=str(self._input_data_dict),
                                                     description='run of ' + cellmaps_vnn.__name__,
                                                     used_software=[self._softwareid],
-                                                    used_dataset=[input_dataset_id],
+                                                    used_dataset=used_dataset,
                                                     generated=generated_dataset_ids)
 
     def run(self):
         """
         Runs cellmaps_vnn
 
         :return:
```

### Comparing `cellmaps_vnn-0.1.0a1/cellmaps_vnn/train.py` & `cellmaps_vnn-0.1.0a2/cellmaps_vnn/train.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # train.py
 import os
+import shutil
 from datetime import date
 
 from cellmaps_utils import constants
 import logging
 
 import cellmaps_vnn
 from cellmaps_vnn.data_wrapper import TrainingDataWrapper
@@ -38,15 +39,15 @@
         directory specified by the user.
         """
         parser = subparsers.add_parser(VNNTrain.COMMAND,
                                        help='Train a Visual Neural Network',
                                        description=desc,
                                        formatter_class=constants.ArgParseFormatter)
         parser.add_argument('outdir', help='Directory to write results to')
-        parser.add_argument('--inputdir', required=True, help='Path to RO-Crate with hierarchy.cx2 file.')
+        parser.add_argument('--inputdir', required=True, help='Path to directory or RO-Crate with hierarchy.cx2 file.')
         parser.add_argument('--training_data', required=True, help='Training data')
         parser.add_argument('--gene2id', required=True, help='Gene to ID mapping file', type=str)
         parser.add_argument('--cell2id', required=True, help='Cell to ID mapping file', type=str)
         parser.add_argument('--mutations', required=True, help='Mutation information for cell lines', type=str)
         parser.add_argument('--cn_deletions', required=True, help='Copy number deletions for cell lines', type=str)
         parser.add_argument('--cn_amplifications', required=True, help='Copy number amplifications for cell lines',
                             type=str)
@@ -110,15 +111,16 @@
         :param keywords: List of keywords associated with the files.
         :param provenance_utils: The utility class for provenance registration.
 
         :return: A list of dataset IDs for the registered model and standard deviation files.
         """
         id_model = self._register_model_file(outdir, description, keywords, provenance_utils)
         id_std = self._register_std_file(outdir, description, keywords, provenance_utils)
-        return [id_model,  id_std]
+        id_hierarchy = self._copy_and_register_hierarchy(outdir, description, keywords, provenance_utils)
+        return [id_model, id_std, id_hierarchy]
 
     def _register_model_file(self, outdir, description, keywords, provenance_utils):
         """
         Registers the trained model file with the FAIRSCAPE service for data provenance.
 
         :param outdir: The output directory where the model file is stored.
         :param description: Description of the model file for provenance registration.
@@ -168,7 +170,22 @@
                      'version': cellmaps_vnn.__version__,
                      'date-published': date.today().strftime(provenance_utils.get_default_date_format_str())}
         dataset_id = provenance_utils.register_dataset(outdir,
                                                        source_file=dest_path,
                                                        data_dict=data_dict)
         return dataset_id
 
+    def _copy_and_register_hierarchy(self, outdir, description, keywords, provenance_utils):
+        hierarchy_out_file = os.path.join(outdir, 'hierarchy.cx2')
+        shutil.copy(os.path.join(self._theargs.inputdir, 'hierarchy.cx2'), hierarchy_out_file)
+
+        data_dict = {'name': os.path.basename(hierarchy_out_file) + ' Hierarchy network file',
+                     'description': description + ' Hierarchy network file',
+                     'keywords': keywords,
+                     'data-format': 'CX2',
+                     'author': cellmaps_vnn.__name__,
+                     'version': cellmaps_vnn.__version__,
+                     'date-published': date.today().strftime('%m-%d-%Y')}
+        dataset_id = provenance_utils.register_dataset(outdir,
+                                                       source_file=hierarchy_out_file,
+                                                       data_dict=data_dict)
+        return dataset_id
```

### Comparing `cellmaps_vnn-0.1.0a1/cellmaps_vnn/util.py` & `cellmaps_vnn-0.1.0a2/cellmaps_vnn/util.py`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/cellmaps_vnn/vnn.py` & `cellmaps_vnn-0.1.0a2/cellmaps_vnn/vnn.py`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/cellmaps_vnn/vnn_trainer.py` & `cellmaps_vnn-0.1.0a2/cellmaps_vnn/vnn_trainer.py`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/docs/Makefile` & `cellmaps_vnn-0.1.0a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/docs/cellmaps_vnn.rst` & `cellmaps_vnn-0.1.0a2/docs/cellmaps_vnn.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/docs/conf.py` & `cellmaps_vnn-0.1.0a2/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = ['sphinx.ext.autodoc',
               'sphinx.ext.intersphinx',
               'sphinx.ext.autosectionlabel',
-              'sphinx.ext.viewcode']
+              'sphinx.ext.viewcode',
+              'sphinx_copybutton']
 
 # intersphinx mapping
 intersphinx_mapping = {"python": ("https://docs.python.org/3", None),
                        "requests": ("https://requests.readthedocs.io/en/latest/", None),
                        "networkx": ("http://networkx.org/documentation/stable/", None),
                        "pandas": ("https://pandas.pydata.org/docs/", None),
                        "numpy": ("https://numpy.org/doc/stable/", None),
```

### Comparing `cellmaps_vnn-0.1.0a1/docs/installation.rst` & `cellmaps_vnn-0.1.0a2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/docs/make.bat` & `cellmaps_vnn-0.1.0a2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/docs/newrelease.rst` & `cellmaps_vnn-0.1.0a2/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/docs/outputs.rst` & `cellmaps_vnn-0.1.0a2/docs/outputs.rst`

 * *Files 20% similar despite different names*

```diff
@@ -22,14 +22,30 @@
 
 - ``predict_feature_grad_0.txt`` (``predict_feature_grad_1.txt``, ``predict_feature_grad_2.txt``):
     Files containing the gradients for each feature.
 
 - ``hidden`` directory:
     Directory with files containing the gradients of the hidden layer outputs.
 
+- ``rlipp.out``:
+    Output file with interpretation of predictions made by VNN.
+
+- ``gene_rho.out``:
+    Output file with Spearman correlation between gene embeddings and predicted AUC.
+
+Annotation
+-----------
+
+- ``hierarchy.cx2``:
+    File with hierarchy in HCX format annotated with interpretation results that will help determine importance of
+    the subsystems in the hierarchical network.
+
+- ``rlipp.out``:
+    Aggregated interpretation scores of each provided RO-crates with prediction and interpretation results.
+
 Logs and Metadata
 -----------------
 
 - ``output.log``:
     A standard log file recording events, errors, and other messages during the execution of the tool.
 
 - ``error.log``:
```

### Comparing `cellmaps_vnn-0.1.0a1/docs/pypircfile.rst` & `cellmaps_vnn-0.1.0a2/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/docs/versioningscheme.rst` & `cellmaps_vnn-0.1.0a2/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/setup.py` & `cellmaps_vnn-0.1.0a2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,25 @@
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = ['cellmaps_utils==0.1.0a23',
-                'ndex2>=3.7.0,<4.0.0',
+                'cellmaps_generate_hierarchy==0.1.0a20',
+                'ndex2>=3.8.0,<4.0.0',
                 'optuna',
                 'scikit-learn',
                 'networkx',
                 'pandas',
                 'torch',
                 'torchvision',
-                'torchaudio'
+                'torchaudio',
+                'scipy',
+                'joblib'
                 ]
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
```

### Comparing `cellmaps_vnn-0.1.0a1/tests/test_cellmaps_vnncmd.py` & `cellmaps_vnn-0.1.0a2/tests/test_cellmaps_vnncmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/tests/test_cellmapsvnn.py` & `cellmaps_vnn-0.1.0a2/tests/test_cellmapsvnn.py`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/tests/test_datawrapper.py` & `cellmaps_vnn-0.1.0a2/tests/test_datawrapper.py`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/tests/test_integration_cellmaps_vnn.py` & `cellmaps_vnn-0.1.0a2/tests/test_integration_cellmaps_vnn.py`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/tests/test_predict.py` & `cellmaps_vnn-0.1.0a2/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/tests/test_util.py` & `cellmaps_vnn-0.1.0a2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/tests/test_vnn.py` & `cellmaps_vnn-0.1.0a2/tests/test_vnn.py`

 * *Files identical despite different names*

### Comparing `cellmaps_vnn-0.1.0a1/tests/test_vnntrainer.py` & `cellmaps_vnn-0.1.0a2/tests/test_vnntrainer.py`

 * *Files identical despite different names*

