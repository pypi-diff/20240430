# Comparing `tmp/depthcharge_ms-0.4.3.tar.gz` & `tmp/depthcharge_ms-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depthcharge_ms-0.4.3.tar", last modified: Fri Apr 26 06:28:51 2024, max compression
+gzip compressed data, was "depthcharge_ms-0.4.4.tar", last modified: Mon Apr 29 22:20:03 2024, max compression
```

## Comparing `depthcharge_ms-0.4.3.tar` & `depthcharge_ms-0.4.4.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.312336 depthcharge_ms-0.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.296336 depthcharge_ms-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.300336 depthcharge_ms-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-26 06:28:51.312336 depthcharge_ms-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.300336 depthcharge_ms-0.4.3/data/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/data/TMT10-Trial-8.mgf
--rw-r--r--   0 runner    (1001) docker     (127)   333839 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/data/TMT10-Trial-8.mzML
--rw-r--r--   0 runner    (1001) docker     (127)    67798 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/data/TMT10-Trial-8.mzXML
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.300336 depthcharge_ms-0.4.3/depthcharge/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.304336 depthcharge_ms-0.4.3/depthcharge/data/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/data/analyte_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12035 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/data/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/data/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    18919 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/data/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/data/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    18688 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/data/spectrum_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.304336 depthcharge_ms-0.4.3/depthcharge/encoders/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/encoders/sinusoidal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/feedforward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.304336 depthcharge_ms-0.4.3/depthcharge/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/tokenizers/molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/tokenizers/peptides.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/tokenizers/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.304336 depthcharge_ms-0.4.3/depthcharge/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/transformers/analytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/transformers/spectra.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/depthcharge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.308336 depthcharge_ms-0.4.3/depthcharge_ms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-26 06:28:51.000000 depthcharge_ms-0.4.3/depthcharge_ms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-26 06:28:51.000000 depthcharge_ms-0.4.3/depthcharge_ms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 06:28:51.000000 depthcharge_ms-0.4.3/depthcharge_ms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-26 06:28:51.000000 depthcharge_ms-0.4.3/depthcharge_ms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 06:28:51.000000 depthcharge_ms-0.4.3/depthcharge_ms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.304336 depthcharge_ms-0.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/docs/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.304336 depthcharge_ms-0.4.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/docs/api/datasets.md
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/docs/api/encoders.md
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/docs/api/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/docs/api/primitives.md
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/docs/api/tokenizers.md
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/docs/api/transformers.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.308336 depthcharge_ms-0.4.3/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/docs/getting-started/spectra.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.308336 depthcharge_ms-0.4.3/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 06:28:51.312336 depthcharge_ms-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.308336 depthcharge_ms-0.4.3/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    50058 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/static/logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    46385 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/static/logo-light.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.308336 depthcharge_ms-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.308336 depthcharge_ms-0.4.3/tests/unit_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.308336 depthcharge_ms-0.4.3/tests/unit_tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/tests/unit_tests/test_data/test_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/tests/unit_tests/test_data/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/tests/unit_tests/test_data/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/tests/unit_tests/test_data/test_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.308336 depthcharge_ms-0.4.3/tests/unit_tests/test_encoders/
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/tests/unit_tests/test_encoders/test_sinusoidal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/tests/unit_tests/test_feedforward.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/tests/unit_tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/tests/unit_tests/test_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.308336 depthcharge_ms-0.4.3/tests/unit_tests/test_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/tests/unit_tests/test_tokenizers/test_molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/tests/unit_tests/test_tokenizers/test_peptides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:28:51.308336 depthcharge_ms-0.4.3/tests/unit_tests/test_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/tests/unit_tests/test_transformers/test_analyte_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/tests/unit_tests/test_transformers/test_spectrum_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-26 06:28:39.000000 depthcharge_ms-0.4.3/tests/unit_tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.260631 depthcharge_ms-0.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.244632 depthcharge_ms-0.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.248632 depthcharge_ms-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-29 22:20:03.260631 depthcharge_ms-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.252632 depthcharge_ms-0.4.4/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/data/TMT10-Trial-8.mgf
+-rw-r--r--   0 runner    (1001) docker     (127)   333839 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/data/TMT10-Trial-8.mzML
+-rw-r--r--   0 runner    (1001) docker     (127)    67798 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/data/TMT10-Trial-8.mzXML
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.252632 depthcharge_ms-0.4.4/depthcharge/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.252632 depthcharge_ms-0.4.4/depthcharge/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/data/analyte_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12035 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/data/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/data/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18930 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/data/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/data/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/data/spectrum_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.252632 depthcharge_ms-0.4.4/depthcharge/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/encoders/sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.252632 depthcharge_ms-0.4.4/depthcharge/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/tokenizers/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/tokenizers/peptides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/tokenizers/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.252632 depthcharge_ms-0.4.4/depthcharge/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/transformers/analytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/transformers/spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/depthcharge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.260631 depthcharge_ms-0.4.4/depthcharge_ms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-29 22:20:03.000000 depthcharge_ms-0.4.4/depthcharge_ms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-29 22:20:03.000000 depthcharge_ms-0.4.4/depthcharge_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:20:03.000000 depthcharge_ms-0.4.4/depthcharge_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-29 22:20:03.000000 depthcharge_ms-0.4.4/depthcharge_ms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 22:20:03.000000 depthcharge_ms-0.4.4/depthcharge_ms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.256631 depthcharge_ms-0.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/docs/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.256631 depthcharge_ms-0.4.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/docs/api/datasets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/docs/api/encoders.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/docs/api/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/docs/api/primitives.md
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/docs/api/tokenizers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/docs/api/transformers.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.256631 depthcharge_ms-0.4.4/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/docs/getting-started/spectra.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.256631 depthcharge_ms-0.4.4/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 22:20:03.260631 depthcharge_ms-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.256631 depthcharge_ms-0.4.4/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    50058 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/static/logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46385 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/static/logo-light.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.256631 depthcharge_ms-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.260631 depthcharge_ms-0.4.4/tests/unit_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.260631 depthcharge_ms-0.4.4/tests/unit_tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/tests/unit_tests/test_data/test_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/tests/unit_tests/test_data/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/tests/unit_tests/test_data/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/tests/unit_tests/test_data/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.260631 depthcharge_ms-0.4.4/tests/unit_tests/test_encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/tests/unit_tests/test_encoders/test_sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/tests/unit_tests/test_feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/tests/unit_tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/tests/unit_tests/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.260631 depthcharge_ms-0.4.4/tests/unit_tests/test_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/tests/unit_tests/test_tokenizers/test_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/tests/unit_tests/test_tokenizers/test_peptides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:20:03.260631 depthcharge_ms-0.4.4/tests/unit_tests/test_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/tests/unit_tests/test_transformers/test_analyte_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/tests/unit_tests/test_transformers/test_spectrum_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-29 22:19:51.000000 depthcharge_ms-0.4.4/tests/unit_tests/test_version.py
```

### Comparing `depthcharge_ms-0.4.3/.github/workflows/docs.yml` & `depthcharge_ms-0.4.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/.github/workflows/lint.yml` & `depthcharge_ms-0.4.4/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/.github/workflows/publish.yml` & `depthcharge_ms-0.4.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/.github/workflows/tests.yml` & `depthcharge_ms-0.4.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/CHANGELOG.md` & `depthcharge_ms-0.4.4/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v0.4.4]
+
+### Changed
+- Partially revert length changes to `SpectrumDataset` and `AnnotatedSpectrumDataset`. We removed `__len__` from both due to problems with PyTorch Lightning compatibility.
+- Simplify dataset code by removing redundancy with `lance.pytorch.LanceDatset`.
+- Improved warning message for skipped spectra.
+
 ## [v0.4.3]
 
 ### Changed
 - Length of the `SpectrumDataset` and `AnnotatedSpectrumDataset` now reflect the `samples` parameter of the `lance.pytorch.LanceDataset` parent class.
 
 ## [v0.4.2]
```

### Comparing `depthcharge_ms-0.4.3/CODE_OF_CONDUCT.md` & `depthcharge_ms-0.4.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/CONTRIBUTING.md` & `depthcharge_ms-0.4.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/LICENSE` & `depthcharge_ms-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/PKG-INFO` & `depthcharge_ms-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge-ms
-Version: 0.4.3
+Version: 0.4.4
 Summary: A mass spectrometry toolkit for deep learning with Transformer models.
 Author-email: "William E. Fondrie" <fondriew@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/wfondrie/depthcharge
 Project-URL: Documentation, https://wfondrie.github.io/depthcharge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `depthcharge_ms-0.4.3/README.md` & `depthcharge_ms-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/data/TMT10-Trial-8.mgf` & `depthcharge_ms-0.4.4/data/TMT10-Trial-8.mgf`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/data/TMT10-Trial-8.mzML` & `depthcharge_ms-0.4.4/data/TMT10-Trial-8.mzML`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/data/TMT10-Trial-8.mzXML` & `depthcharge_ms-0.4.4/data/TMT10-Trial-8.mzXML`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/__init__.py` & `depthcharge_ms-0.4.4/depthcharge/__init__.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/data/analyte_datasets.py` & `depthcharge_ms-0.4.4/depthcharge/data/analyte_datasets.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/data/arrow.py` & `depthcharge_ms-0.4.4/depthcharge/data/arrow.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/data/fields.py` & `depthcharge_ms-0.4.4/depthcharge/data/fields.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/data/parsers.py` & `depthcharge_ms-0.4.4/depthcharge/data/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Mass spectrometry data parsers."""
 
 from __future__ import annotations
 
 import logging
+import warnings
 from abc import ABC, abstractmethod
 from collections.abc import Callable, Iterable
 from os import PathLike
 from typing import Any
 
 import pyarrow as pa
 from cloudpathlib import AnyPath
@@ -219,18 +220,18 @@
                     yield self._yield_batch()
 
             # Get the remainder:
             if self._batch is not None:
                 yield self._yield_batch()
 
         if n_skipped:
-            LOGGER.warning(
-                "Skipped %d spectra with invalid information", n_skipped
+            warnings.warn(
+                f"Skipped {n_skipped} spectra with invalid information."
+                f"Last error was: \n {str(last_exc)}"
             )
-            LOGGER.debug("Last error: %s", str(last_exc))
 
     def _update_batch(self, entry: dict) -> None:
         """Update the batch.
 
         Parameters
         ----------
         entry : dict
```

### Comparing `depthcharge_ms-0.4.3/depthcharge/data/preprocessing.py` & `depthcharge_ms-0.4.4/depthcharge/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/data/spectrum_datasets.py` & `depthcharge_ms-0.4.4/depthcharge/data/spectrum_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Serve mass spectra to neural networks."""
 
 from __future__ import annotations
 
 import copy
 import logging
-import math
 import uuid
 from collections.abc import Generator, Iterable
 from os import PathLike
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Any
 
@@ -73,14 +72,16 @@
         Keyword arguments to initialize a
         `[lance.torch.data.LanceDataset](https://lancedb.github.io/lance/api/python/lance.torch.html#lance.torch.data.LanceDataset)`.
 
     Attributes
     ----------
     peak_files : list of str
     path : Path
+    n_spectra : int
+    dataset : lance.LanceDataset
 
     """
 
     def __init__(
         self,
         spectra: pl.DataFrame | PathLike | Iterable[PathLike],
         batch_size: int,
@@ -114,19 +115,19 @@
                 mode="overwrite" if self._path.exists() else "create",
                 schema=batch.schema,
             )
 
         elif not self._path.exists():
             raise ValueError("No spectra were provided")
 
-        self._dataset = lance.dataset(str(self._path))
+        dataset = lance.dataset(str(self._path))
         if "to_tensor_fn" not in kwargs:
             kwargs["to_tensor_fn"] = self._to_tensor
 
-        super().__init__(self._dataset, batch_size, **kwargs)
+        super().__init__(dataset, batch_size, **kwargs)
 
     def add_spectra(
         self,
         spectra: pl.DataFrame | PathLike | Iterable[PathLike],
     ) -> SpectrumDataset:
         """Add mass spectrometry data to the lance dataset.
 
@@ -140,15 +141,15 @@
             with `depthcharge.spectra_to_df()`, parquet files created with
             `depthcharge.spectra_to_parquet()`, or a peak file in the mzML,
             mzXML, or MGF format.
 
         """
         spectra = utils.listify(spectra)
         batch = next(_get_records(spectra, **self._init_kwargs))
-        self._dataset = lance.write_dataset(
+        self.dataset = lance.write_dataset(
             _get_records(spectra, **self._parse_kwargs),
             self._path,
             mode="append",
             schema=batch.schema,
         )
 
         return self
@@ -166,34 +167,31 @@
         dict
             A dictionary representing a row of the dataset. Each
             key is a column and the value is the value for that
             row. List columns are automatically converted to
             PyTorch tensors if the nested data type is compatible.
 
         """
-        return self._to_tensor(self._dataset.take(utils.listify(idx)))
-
-    def __len__(self) -> int:
-        """The number of batches in the lance dataset."""
-        num = self._dataset.count_rows()
-        if self.samples:
-            num = min(self.samples, num)
-
-        return math.ceil(num / self.batch_size)
+        return self._to_tensor(self.dataset.take(utils.listify(idx)))
 
     def __del__(self) -> None:
         """Cleanup the temporary directory."""
         if self._tmpdir is not None:
             self._tmpdir.cleanup()
 
     @property
+    def n_spectra(self) -> int:
+        """The number of spectra in the Lance dataset."""
+        return self.dataset.count_rows()
+
+    @property
     def peak_files(self) -> list[str]:
         """The files currently in the lance dataset."""
         return (
-            self._dataset.to_table(columns=["peak_file"])
+            self.dataset.to_table(columns=["peak_file"])
             .column(0)
             .unique()
             .to_pylist()
         )
 
     @property
     def path(self) -> Path:
@@ -316,14 +314,16 @@
         Keyword arguments to initialize a
         `[lance.torch.data.LanceDataset](https://lancedb.github.io/lance/api/python/lance.torch.html#lance.torch.data.LanceDataset)`.
 
     Attributes
     ----------
     peak_files : list of str
     path : Path
+    n_spectra : int
+    dataset : lance.LanceDataset
     tokenizer : PeptideTokenizer
         The tokenizer for the annotations.
     annotations : str
         The annotation column in the dataset.
 
     """
```

### Comparing `depthcharge_ms-0.4.3/depthcharge/encoders/sinusoidal.py` & `depthcharge_ms-0.4.4/depthcharge/encoders/sinusoidal.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/feedforward.py` & `depthcharge_ms-0.4.4/depthcharge/feedforward.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/mixins.py` & `depthcharge_ms-0.4.4/depthcharge/mixins.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/primitives.py` & `depthcharge_ms-0.4.4/depthcharge/primitives.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/testing.py` & `depthcharge_ms-0.4.4/depthcharge/testing.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/tokenizers/molecules.py` & `depthcharge_ms-0.4.4/depthcharge/tokenizers/molecules.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/tokenizers/peptides.py` & `depthcharge_ms-0.4.4/depthcharge/tokenizers/peptides.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/tokenizers/tokenizer.py` & `depthcharge_ms-0.4.4/depthcharge/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/transformers/analytes.py` & `depthcharge_ms-0.4.4/depthcharge/transformers/analytes.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/transformers/spectra.py` & `depthcharge_ms-0.4.4/depthcharge/transformers/spectra.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge/utils.py` & `depthcharge_ms-0.4.4/depthcharge/utils.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/depthcharge_ms.egg-info/PKG-INFO` & `depthcharge_ms-0.4.4/depthcharge_ms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge-ms
-Version: 0.4.3
+Version: 0.4.4
 Summary: A mass spectrometry toolkit for deep learning with Transformer models.
 Author-email: "William E. Fondrie" <fondriew@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/wfondrie/depthcharge
 Project-URL: Documentation, https://wfondrie.github.io/depthcharge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `depthcharge_ms-0.4.3/depthcharge_ms.egg-info/SOURCES.txt` & `depthcharge_ms-0.4.4/depthcharge_ms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/docs/CHANGELOG.md` & `depthcharge_ms-0.4.4/docs/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v0.4.4]
+
+### Changed
+- Partially revert length changes to `SpectrumDataset` and `AnnotatedSpectrumDataset`. We removed `__len__` from both due to problems with PyTorch Lightning compatibility.
+- Simplify dataset code by removing redundancy with `lance.pytorch.LanceDatset`.
+- Improved warning message for skipped spectra.
+
 ## [v0.4.3]
 
 ### Changed
 - Length of the `SpectrumDataset` and `AnnotatedSpectrumDataset` now reflect the `samples` parameter of the `lance.pytorch.LanceDataset` parent class.
 
 ## [v0.4.2]
```

### Comparing `depthcharge_ms-0.4.3/docs/CODE_OF_CONDUCT.md` & `depthcharge_ms-0.4.4/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/docs/CONTRIBUTING.md` & `depthcharge_ms-0.4.4/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/docs/api/index.md` & `depthcharge_ms-0.4.4/docs/api/index.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/docs/getting-started/installation.md` & `depthcharge_ms-0.4.4/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/docs/getting-started/spectra.qmd` & `depthcharge_ms-0.4.4/docs/getting-started/spectra.qmd`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/docs/index.md` & `depthcharge_ms-0.4.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/docs/stylesheets/extra.css` & `depthcharge_ms-0.4.4/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/mkdocs.yml` & `depthcharge_ms-0.4.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/pyproject.toml` & `depthcharge_ms-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/static/icon.svg` & `depthcharge_ms-0.4.4/static/icon.svg`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/static/logo-dark.png` & `depthcharge_ms-0.4.4/static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/static/logo-light.png` & `depthcharge_ms-0.4.4/static/logo-light.png`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/tests/conftest.py` & `depthcharge_ms-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/tests/unit_tests/test_data/test_arrow.py` & `depthcharge_ms-0.4.4/tests/unit_tests/test_data/test_arrow.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/tests/unit_tests/test_data/test_datasets.py` & `depthcharge_ms-0.4.4/tests/unit_tests/test_data/test_datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,18 @@
     """Use a tokenizer for every test."""
     return PeptideTokenizer()
 
 
 def test_addition(mgf_small, tmp_path):
     """Testing adding a file."""
     dataset = SpectrumDataset(mgf_small, path=tmp_path / "test", batch_size=1)
-    assert len(dataset) == 2
+    assert dataset.n_spectra == 2
 
     dataset = dataset.add_spectra(mgf_small)
-    assert len(dataset) == 4
+    assert dataset.n_spectra == 4
 
 
 def test_indexing(tokenizer, mgf_small, tmp_path):
     """Test retrieving spectra."""
     mgf_small2 = tmp_path / "mgf_small2.mgf"
     shutil.copy(mgf_small, mgf_small2)
 
@@ -193,15 +193,15 @@
     pkl_file = tmp_path / "test.pkl"
     with pkl_file.open("wb+") as pkl:
         pickle.dump(dataset, pkl)
 
     with pkl_file.open("rb") as pkl:
         loaded = pickle.load(pkl)
 
-    assert len(dataset) == len(loaded)
+    assert dataset.n_spectra == loaded.n_spectra
 
     dataset = AnnotatedSpectrumDataset(
         [mgf_small],
         tokenizer,
         "seq",
         batch_size=1,
         path=tmp_path / "test.lance",
@@ -210,8 +210,8 @@
 
     with pkl_file.open("wb+") as pkl:
         pickle.dump(dataset, pkl)
 
     with pkl_file.open("rb") as pkl:
         loaded = pickle.load(pkl)
 
-    assert len(dataset) == len(loaded)
+    assert dataset.n_spectra == loaded.n_spectra
```

### Comparing `depthcharge_ms-0.4.3/tests/unit_tests/test_data/test_loaders.py` & `depthcharge_ms-0.4.4/tests/unit_tests/test_data/test_loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         mgf_small,
         batch_size=1,
         path=tmp_path / "test",
         samples=samples,
     )
 
     loaded = list(DataLoader(dset))
-    assert len(dset) == batches
+    assert dset.n_spectra == 2
     assert len(loaded) == batches
 
 
 def test_streaming_spectrum_loader(mgf_small, tmp_path):
     """Test streaming spectra."""
     streamer = StreamingSpectrumDataset(mgf_small, batch_size=2)
     loader = DataLoader(streamer)
```

### Comparing `depthcharge_ms-0.4.3/tests/unit_tests/test_data/test_parsers.py` & `depthcharge_ms-0.4.4/tests/unit_tests/test_data/test_parsers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/tests/unit_tests/test_encoders/test_sinusoidal.py` & `depthcharge_ms-0.4.4/tests/unit_tests/test_encoders/test_sinusoidal.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/tests/unit_tests/test_feedforward.py` & `depthcharge_ms-0.4.4/tests/unit_tests/test_feedforward.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/tests/unit_tests/test_primitives.py` & `depthcharge_ms-0.4.4/tests/unit_tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/tests/unit_tests/test_testing.py` & `depthcharge_ms-0.4.4/tests/unit_tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/tests/unit_tests/test_tokenizers/test_molecules.py` & `depthcharge_ms-0.4.4/tests/unit_tests/test_tokenizers/test_molecules.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/tests/unit_tests/test_tokenizers/test_peptides.py` & `depthcharge_ms-0.4.4/tests/unit_tests/test_tokenizers/test_peptides.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/tests/unit_tests/test_transformers/test_analyte_transformers.py` & `depthcharge_ms-0.4.4/tests/unit_tests/test_transformers/test_analyte_transformers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/tests/unit_tests/test_transformers/test_spectrum_transformers.py` & `depthcharge_ms-0.4.4/tests/unit_tests/test_transformers/test_spectrum_transformers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.3/tests/unit_tests/test_version.py` & `depthcharge_ms-0.4.4/tests/unit_tests/test_version.py`

 * *Files identical despite different names*

