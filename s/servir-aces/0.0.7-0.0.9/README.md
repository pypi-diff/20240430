# Comparing `tmp/servir_aces-0.0.7.tar.gz` & `tmp/servir_aces-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servir_aces-0.0.7.tar", last modified: Tue Apr 16 15:28:27 2024, max compression
+gzip compressed data, was "servir_aces-0.0.9.tar", last modified: Tue Apr 16 15:34:16 2024, max compression
```

## Comparing `servir_aces-0.0.7.tar` & `servir_aces-0.0.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.990435 servir_aces-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.974435 servir_aces-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.978435 servir_aces-0.0.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.978435 servir_aces-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-16 15:28:17.000000 servir_aces-0.0.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-16 15:28:17.000000 servir_aces-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 15:28:17.000000 servir_aces-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-16 15:28:27.990435 servir_aces-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-16 15:28:17.000000 servir_aces-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.982435 servir_aces-0.0.7/aces/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25100 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    21671 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/ee_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    20238 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/model_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)    16644 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/remote_sensing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.982435 servir_aces-0.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/config.md
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/data_processor.md
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/ee_utils.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/metrics.md
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/model_builder.md
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/model_trainer.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.982435 servir_aces-0.0.7/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/remote_sensing.md
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.982435 servir_aces-0.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:17.000000 servir_aces-0.0.7/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-16 15:28:17.000000 servir_aces-0.0.7/examples/count_sample_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-16 15:28:17.000000 servir_aces-0.0.7/examples/run_model_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-16 15:28:17.000000 servir_aces-0.0.7/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.986435 servir_aces-0.0.7/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)  2316819 2024-04-16 15:28:17.000000 servir_aces-0.0.7/notebook/aces_rice_classification_paro_2021.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    57598 2024-04-16 15:28:17.000000 servir_aces-0.0.7/notebook/count_sample_size.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    61100 2024-04-16 15:28:17.000000 servir_aces-0.0.7/notebook/prediction_dnn.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    81476 2024-04-16 15:28:17.000000 servir_aces-0.0.7/notebook/prediction_unet.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-16 15:28:17.000000 servir_aces-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 15:28:17.000000 servir_aces-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-16 15:28:17.000000 servir_aces-0.0.7/requirements_dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.990435 servir_aces-0.0.7/servir_aces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-16 15:28:27.000000 servir_aces-0.0.7/servir_aces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-16 15:28:27.000000 servir_aces-0.0.7/servir_aces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:28:27.000000 servir_aces-0.0.7/servir_aces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 15:28:27.000000 servir_aces-0.0.7/servir_aces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 15:28:27.000000 servir_aces-0.0.7/servir_aces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:28:27.990435 servir_aces-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.986435 servir_aces-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-16 15:28:17.000000 servir_aces-0.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.974435 servir_aces-0.0.7/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.986435 servir_aces-0.0.7/workflow/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v1/1.s1_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.990435 servir_aces-0.0.7/workflow/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/1.planet_composites.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/2.generate_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/4.export_image_for_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/5.prediction_dnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/5.prediction_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    18247 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/generate_training_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/host_vertex_ai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:16.660453 servir_aces-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-16 15:34:05.000000 servir_aces-0.0.9/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:16.644453 servir_aces-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:16.648453 servir_aces-0.0.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-16 15:34:05.000000 servir_aces-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-16 15:34:05.000000 servir_aces-0.0.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-16 15:34:05.000000 servir_aces-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:16.648453 servir_aces-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-16 15:34:05.000000 servir_aces-0.0.9/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-16 15:34:05.000000 servir_aces-0.0.9/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-16 15:34:05.000000 servir_aces-0.0.9/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-16 15:34:05.000000 servir_aces-0.0.9/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-16 15:34:05.000000 servir_aces-0.0.9/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-16 15:34:05.000000 servir_aces-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-16 15:34:05.000000 servir_aces-0.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-16 15:34:05.000000 servir_aces-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 15:34:05.000000 servir_aces-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-16 15:34:16.660453 servir_aces-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-16 15:34:05.000000 servir_aces-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:16.652453 servir_aces-0.0.9/aces/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-16 15:34:05.000000 servir_aces-0.0.9/aces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-16 15:34:05.000000 servir_aces-0.0.9/aces/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25100 2024-04-16 15:34:05.000000 servir_aces-0.0.9/aces/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21671 2024-04-16 15:34:05.000000 servir_aces-0.0.9/aces/ee_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-16 15:34:05.000000 servir_aces-0.0.9/aces/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-04-16 15:34:05.000000 servir_aces-0.0.9/aces/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20238 2024-04-16 15:34:05.000000 servir_aces-0.0.9/aces/model_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-16 15:34:05.000000 servir_aces-0.0.9/aces/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    16644 2024-04-16 15:34:05.000000 servir_aces-0.0.9/aces/remote_sensing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-16 15:34:05.000000 servir_aces-0.0.9/aces/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:16.652453 servir_aces-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 15:34:05.000000 servir_aces-0.0.9/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 15:34:05.000000 servir_aces-0.0.9/docs/config.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-16 15:34:05.000000 servir_aces-0.0.9/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 15:34:05.000000 servir_aces-0.0.9/docs/data_processor.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 15:34:05.000000 servir_aces-0.0.9/docs/ee_utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 15:34:05.000000 servir_aces-0.0.9/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-16 15:34:05.000000 servir_aces-0.0.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 15:34:05.000000 servir_aces-0.0.9/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 15:34:05.000000 servir_aces-0.0.9/docs/metrics.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 15:34:05.000000 servir_aces-0.0.9/docs/model_builder.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 15:34:05.000000 servir_aces-0.0.9/docs/model_trainer.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:16.652453 servir_aces-0.0.9/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-16 15:34:05.000000 servir_aces-0.0.9/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 15:34:05.000000 servir_aces-0.0.9/docs/remote_sensing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-16 15:34:05.000000 servir_aces-0.0.9/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-16 15:34:05.000000 servir_aces-0.0.9/docs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:16.656453 servir_aces-0.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:05.000000 servir_aces-0.0.9/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-16 15:34:05.000000 servir_aces-0.0.9/examples/count_sample_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-16 15:34:05.000000 servir_aces-0.0.9/examples/run_model_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-16 15:34:05.000000 servir_aces-0.0.9/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:16.656453 servir_aces-0.0.9/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)  2316819 2024-04-16 15:34:05.000000 servir_aces-0.0.9/notebook/aces_rice_classification_paro_2021.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    57598 2024-04-16 15:34:05.000000 servir_aces-0.0.9/notebook/count_sample_size.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    61100 2024-04-16 15:34:05.000000 servir_aces-0.0.9/notebook/prediction_dnn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    81476 2024-04-16 15:34:05.000000 servir_aces-0.0.9/notebook/prediction_unet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-16 15:34:05.000000 servir_aces-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 15:34:05.000000 servir_aces-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-16 15:34:05.000000 servir_aces-0.0.9/requirements_dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:16.660453 servir_aces-0.0.9/servir_aces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-16 15:34:16.000000 servir_aces-0.0.9/servir_aces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-16 15:34:16.000000 servir_aces-0.0.9/servir_aces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:34:16.000000 servir_aces-0.0.9/servir_aces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 15:34:16.000000 servir_aces-0.0.9/servir_aces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 15:34:16.000000 servir_aces-0.0.9/servir_aces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:34:16.660453 servir_aces-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:16.660453 servir_aces-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-16 15:34:05.000000 servir_aces-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:16.648453 servir_aces-0.0.9/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:16.660453 servir_aces-0.0.9/workflow/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-16 15:34:05.000000 servir_aces-0.0.9/workflow/v1/1.s1_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-16 15:34:05.000000 servir_aces-0.0.9/workflow/v1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:16.660453 servir_aces-0.0.9/workflow/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-16 15:34:05.000000 servir_aces-0.0.9/workflow/v2/1.planet_composites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-16 15:34:05.000000 servir_aces-0.0.9/workflow/v2/2.generate_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-16 15:34:05.000000 servir_aces-0.0.9/workflow/v2/4.export_image_for_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-04-16 15:34:05.000000 servir_aces-0.0.9/workflow/v2/5.prediction_dnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-16 15:34:05.000000 servir_aces-0.0.9/workflow/v2/5.prediction_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-16 15:34:05.000000 servir_aces-0.0.9/workflow/v2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18247 2024-04-16 15:34:05.000000 servir_aces-0.0.9/workflow/v2/generate_training_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-16 15:34:05.000000 servir_aces-0.0.9/workflow/v2/host_vertex_ai.py
```

### Comparing `servir_aces-0.0.7/.env.example` & `servir_aces-0.0.9/.env.example`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/.github/workflows/docs.yml` & `servir_aces-0.0.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/.github/workflows/macos.yml` & `servir_aces-0.0.9/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/.github/workflows/pypi.yml` & `servir_aces-0.0.9/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/.github/workflows/ubuntu.yml` & `servir_aces-0.0.9/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/.github/workflows/windows.yml` & `servir_aces-0.0.9/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/.gitignore` & `servir_aces-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/CODE_OF_CONDUCT.md` & `servir_aces-0.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/LICENSE` & `servir_aces-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/PKG-INFO` & `servir_aces-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servir-aces
-Version: 0.0.7
+Version: 0.0.9
 Summary: Agricultural Classification and Estimation Service (ACES)
 Author-email: Biplov Bhandari <bionicbiplov45@gmail.com>
 License: GNU General Public License v3.0
 Project-URL: Homepage, https://github.com/SERVIR/servir-aces
 Keywords: remote sensing,agriculture,machine learning,deep learning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `servir_aces-0.0.7/README.md` & `servir_aces-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/aces/config.py` & `servir_aces-0.0.9/aces/config.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/aces/data_processor.py` & `servir_aces-0.0.9/aces/data_processor.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/aces/ee_utils.py` & `servir_aces-0.0.9/aces/ee_utils.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/aces/metrics.py` & `servir_aces-0.0.9/aces/metrics.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/aces/model_builder.py` & `servir_aces-0.0.9/aces/model_builder.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/aces/model_trainer.py` & `servir_aces-0.0.9/aces/model_trainer.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/aces/refs.bib` & `servir_aces-0.0.9/aces/refs.bib`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/aces/remote_sensing.py` & `servir_aces-0.0.9/aces/remote_sensing.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/aces/utils.py` & `servir_aces-0.0.9/aces/utils.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/docs/contributing.md` & `servir_aces-0.0.9/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/docs/index.md` & `servir_aces-0.0.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/examples/count_sample_size.py` & `servir_aces-0.0.9/examples/count_sample_size.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/examples/run_model_example.py` & `servir_aces-0.0.9/examples/run_model_example.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/mkdocs.yml` & `servir_aces-0.0.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/notebook/aces_rice_classification_paro_2021.ipynb` & `servir_aces-0.0.9/notebook/aces_rice_classification_paro_2021.ipynb`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/notebook/count_sample_size.ipynb` & `servir_aces-0.0.9/notebook/count_sample_size.ipynb`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/notebook/prediction_dnn.ipynb` & `servir_aces-0.0.9/notebook/prediction_dnn.ipynb`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/notebook/prediction_unet.ipynb` & `servir_aces-0.0.9/notebook/prediction_unet.ipynb`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/pyproject.toml` & `servir_aces-0.0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "servir-aces"
-version = "0.0.7"
+version = "0.0.9"
 dynamic = [
     "dependencies",
 ]
 description = "Agricultural Classification and Estimation Service (ACES)"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = [
@@ -37,15 +37,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.7"
+current_version = "0.0.9"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `servir_aces-0.0.7/servir_aces.egg-info/PKG-INFO` & `servir_aces-0.0.9/servir_aces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servir-aces
-Version: 0.0.7
+Version: 0.0.9
 Summary: Agricultural Classification and Estimation Service (ACES)
 Author-email: Biplov Bhandari <bionicbiplov45@gmail.com>
 License: GNU General Public License v3.0
 Project-URL: Homepage, https://github.com/SERVIR/servir-aces
 Keywords: remote sensing,agriculture,machine learning,deep learning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `servir_aces-0.0.7/servir_aces.egg-info/SOURCES.txt` & `servir_aces-0.0.9/servir_aces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/workflow/v1/1.s1_preprocess.py` & `servir_aces-0.0.9/workflow/v1/1.s1_preprocess.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/workflow/v2/1.planet_composites.py` & `servir_aces-0.0.9/workflow/v2/1.planet_composites.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/workflow/v2/2.generate_samples.py` & `servir_aces-0.0.9/workflow/v2/2.generate_samples.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/workflow/v2/4.export_image_for_prediction.py` & `servir_aces-0.0.9/workflow/v2/4.export_image_for_prediction.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/workflow/v2/5.prediction_dnn.py` & `servir_aces-0.0.9/workflow/v2/5.prediction_dnn.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/workflow/v2/5.prediction_unet.py` & `servir_aces-0.0.9/workflow/v2/5.prediction_unet.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/workflow/v2/README.md` & `servir_aces-0.0.9/workflow/v2/README.md`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/workflow/v2/generate_training_patches.py` & `servir_aces-0.0.9/workflow/v2/generate_training_patches.py`

 * *Files identical despite different names*

### Comparing `servir_aces-0.0.7/workflow/v2/host_vertex_ai.py` & `servir_aces-0.0.9/workflow/v2/host_vertex_ai.py`

 * *Files identical despite different names*

