# Comparing `tmp/gilda-1.1.0.tar.gz` & `tmp/gilda-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gilda-1.1.0.tar", last modified: Tue Feb  6 19:47:15 2024, max compression
+gzip compressed data, was "gilda-1.2.0.tar", last modified: Tue Apr 30 20:06:36 2024, max compression
```

## Comparing `gilda-1.1.0.tar` & `gilda-1.2.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-02-06 19:47:15.621072 gilda-1.1.0/
--rw-r--r--   0 ben        (503) staff       (20)     1346 2021-02-10 19:17:08.000000 gilda-1.1.0/LICENSE
--rw-r--r--   0 ben        (503) staff       (20)      155 2023-06-30 15:07:59.000000 gilda-1.1.0/MANIFEST.in
--rw-r--r--   0 ben        (503) staff       (20)     7134 2024-02-06 19:47:15.620950 gilda-1.1.0/PKG-INFO
--rw-r--r--   0 ben        (503) staff       (20)     6431 2024-02-06 19:46:02.000000 gilda-1.1.0/README.md
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-02-06 19:47:15.615921 gilda-1.1.0/doc/
--rw-r--r--   0 ben        (503) staff       (20)      634 2021-02-10 19:17:08.000000 gilda-1.1.0/doc/Makefile
--rw-r--r--   0 ben        (503) staff       (20)     5514 2023-06-30 15:07:59.000000 gilda-1.1.0/doc/conf.py
--rw-r--r--   0 ben        (503) staff       (20)      341 2022-04-26 22:20:20.000000 gilda-1.1.0/doc/index.rst
--rw-r--r--   0 ben        (503) staff       (20)      795 2021-02-10 19:17:08.000000 gilda-1.1.0/doc/make.bat
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-02-06 19:47:15.616024 gilda-1.1.0/doc/modules/
--rw-r--r--   0 ben        (503) staff       (20)      674 2023-06-30 15:07:59.000000 gilda-1.1.0/doc/modules/index.rst
--rw-r--r--   0 ben        (503) staff       (20)      128 2023-06-30 15:07:59.000000 gilda-1.1.0/doc/requirements.txt
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-02-06 19:47:15.617145 gilda-1.1.0/gilda/
--rw-r--r--   0 ben        (503) staff       (20)      768 2024-02-06 19:46:02.000000 gilda-1.1.0/gilda/__init__.py
--rw-r--r--   0 ben        (503) staff       (20)     8879 2024-02-06 19:46:02.000000 gilda-1.1.0/gilda/api.py
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-02-06 19:47:15.618400 gilda-1.1.0/gilda/app/
--rw-r--r--   0 ben        (503) staff       (20)      412 2023-06-30 15:07:59.000000 gilda-1.1.0/gilda/app/__init__.py
--rw-r--r--   0 ben        (503) staff       (20)       59 2021-09-05 00:38:55.000000 gilda-1.1.0/gilda/app/__main__.py
--rw-r--r--   0 ben        (503) staff       (20)    11668 2024-02-06 19:46:02.000000 gilda-1.1.0/gilda/app/app.py
--rw-r--r--   0 ben        (503) staff       (20)      378 2024-02-06 19:46:02.000000 gilda-1.1.0/gilda/app/proxies.py
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-02-06 19:47:15.618932 gilda-1.1.0/gilda/app/templates/
--rw-r--r--   0 ben        (503) staff       (20)     6663 2024-02-06 19:46:02.000000 gilda-1.1.0/gilda/app/templates/base.html
--rw-r--r--   0 ben        (503) staff       (20)       92 2023-06-30 15:07:59.000000 gilda-1.1.0/gilda/app/templates/home.html
--rw-r--r--   0 ben        (503) staff       (20)     2235 2023-06-30 15:07:59.000000 gilda-1.1.0/gilda/app/templates/matches.html
--rw-r--r--   0 ben        (503) staff       (20)       96 2023-06-30 15:07:59.000000 gilda-1.1.0/gilda/app/templates/ner_home.html
--rw-r--r--   0 ben        (503) staff       (20)     1838 2023-06-30 15:07:59.000000 gilda-1.1.0/gilda/app/templates/ner_matches.html
--rw-r--r--   0 ben        (503) staff       (20)     3707 2024-02-06 19:46:02.000000 gilda-1.1.0/gilda/app/ui.py
--rw-r--r--   0 ben        (503) staff       (20)    28683 2024-02-06 19:46:02.000000 gilda-1.1.0/gilda/generate_terms.py
--rwxr-xr-x   0 ben        (503) staff       (20)     1584 2022-04-26 22:20:20.000000 gilda-1.1.0/gilda/greek_alphabet.py
--rw-r--r--   0 ben        (503) staff       (20)    29133 2024-02-06 19:46:02.000000 gilda-1.1.0/gilda/grounder.py
--rw-r--r--   0 ben        (503) staff       (20)     6898 2024-02-06 19:46:02.000000 gilda-1.1.0/gilda/ner.py
--rw-r--r--   0 ben        (503) staff       (20)     3170 2024-02-06 19:46:02.000000 gilda-1.1.0/gilda/pandas_utils.py
--rw-r--r--   0 ben        (503) staff       (20)     7755 2023-06-30 15:07:59.000000 gilda-1.1.0/gilda/process.py
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-02-06 19:47:15.619711 gilda-1.1.0/gilda/resources/
--rw-r--r--   0 ben        (503) staff       (20)     2846 2022-06-21 14:02:33.000000 gilda-1.1.0/gilda/resources/__init__.py
--rw-r--r--   0 ben        (503) staff       (20)      130 2021-09-05 00:38:55.000000 gilda-1.1.0/gilda/resources/__main__.py
--rw-r--r--   0 ben        (503) staff       (20)    29081 2021-02-10 19:17:08.000000 gilda-1.1.0/gilda/resources/mesh_ambig_mappings.tsv
--rw-r--r--   0 ben        (503) staff       (20)   362152 2021-02-10 19:17:08.000000 gilda-1.1.0/gilda/resources/mesh_mappings.tsv
--rw-r--r--   0 ben        (503) staff       (20)     3331 2023-06-30 15:07:59.000000 gilda-1.1.0/gilda/resources/sqlite_adapter.py
--rw-r--r--   0 ben        (503) staff       (20)     8205 2023-06-30 15:07:59.000000 gilda-1.1.0/gilda/scorer.py
--rw-r--r--   0 ben        (503) staff       (20)     6602 2024-02-06 19:46:02.000000 gilda-1.1.0/gilda/term.py
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-02-06 19:47:15.620778 gilda-1.1.0/gilda/tests/
--rw-r--r--   0 ben        (503) staff       (20)       47 2021-02-10 19:17:08.000000 gilda-1.1.0/gilda/tests/__init__.py
--rw-r--r--   0 ben        (503) staff       (20)     2022 2022-04-26 22:20:20.000000 gilda-1.1.0/gilda/tests/test_api.py
--rw-r--r--   0 ben        (503) staff       (20)     2972 2024-02-06 19:46:02.000000 gilda-1.1.0/gilda/tests/test_app.py
--rw-r--r--   0 ben        (503) staff       (20)     5846 2023-06-30 15:07:59.000000 gilda-1.1.0/gilda/tests/test_generate_terms.py
--rw-r--r--   0 ben        (503) staff       (20)     9552 2024-02-06 19:46:02.000000 gilda-1.1.0/gilda/tests/test_grounder.py
--rw-r--r--   0 ben        (503) staff       (20)     2666 2024-02-06 19:46:02.000000 gilda-1.1.0/gilda/tests/test_ner.py
--rw-r--r--   0 ben        (503) staff       (20)      543 2023-06-30 15:07:59.000000 gilda-1.1.0/gilda/tests/test_pandas_utils.py
--rw-r--r--   0 ben        (503) staff       (20)     1644 2023-06-30 15:07:59.000000 gilda-1.1.0/gilda/tests/test_process.py
--rw-r--r--   0 ben        (503) staff       (20)     1566 2021-02-10 19:17:08.000000 gilda-1.1.0/gilda/tests/test_scorer.py
--rw-r--r--   0 ben        (503) staff       (20)     1238 2022-04-26 22:20:20.000000 gilda-1.1.0/gilda/tests/test_term.py
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-02-06 19:47:15.617844 gilda-1.1.0/gilda.egg-info/
--rw-r--r--   0 ben        (503) staff       (20)     7134 2024-02-06 19:47:15.000000 gilda-1.1.0/gilda.egg-info/PKG-INFO
--rw-r--r--   0 ben        (503) staff       (20)     1187 2024-02-06 19:47:15.000000 gilda-1.1.0/gilda.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (503) staff       (20)        1 2024-02-06 19:47:15.000000 gilda-1.1.0/gilda.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (503) staff       (20)       41 2024-02-06 19:47:15.000000 gilda-1.1.0/gilda.egg-info/entry_points.txt
--rw-r--r--   0 ben        (503) staff       (20)      340 2024-02-06 19:47:15.000000 gilda-1.1.0/gilda.egg-info/requires.txt
--rw-r--r--   0 ben        (503) staff       (20)        6 2024-02-06 19:47:15.000000 gilda-1.1.0/gilda.egg-info/top_level.txt
--rw-r--r--   0 ben        (503) staff       (20)       38 2024-02-06 19:47:15.621105 gilda-1.1.0/setup.cfg
--rw-r--r--   0 ben        (503) staff       (20)     2300 2024-02-06 19:46:02.000000 gilda-1.1.0/setup.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-04-30 20:06:36.109643 gilda-1.2.0/
+-rw-r--r--   0 ben        (503) staff       (20)     1346 2021-02-10 19:17:08.000000 gilda-1.2.0/LICENSE
+-rw-r--r--   0 ben        (503) staff       (20)      155 2023-06-30 15:07:59.000000 gilda-1.2.0/MANIFEST.in
+-rw-r--r--   0 ben        (503) staff       (20)     8222 2024-04-30 20:06:36.109473 gilda-1.2.0/PKG-INFO
+-rw-r--r--   0 ben        (503) staff       (20)     7519 2024-04-30 19:26:28.000000 gilda-1.2.0/README.md
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-04-30 20:06:36.104249 gilda-1.2.0/doc/
+-rw-r--r--   0 ben        (503) staff       (20)      634 2021-02-10 19:17:08.000000 gilda-1.2.0/doc/Makefile
+-rw-r--r--   0 ben        (503) staff       (20)     5514 2023-06-30 15:07:59.000000 gilda-1.2.0/doc/conf.py
+-rw-r--r--   0 ben        (503) staff       (20)      341 2022-04-26 22:20:20.000000 gilda-1.2.0/doc/index.rst
+-rw-r--r--   0 ben        (503) staff       (20)      795 2021-02-10 19:17:08.000000 gilda-1.2.0/doc/make.bat
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-04-30 20:06:36.104358 gilda-1.2.0/doc/modules/
+-rw-r--r--   0 ben        (503) staff       (20)      674 2023-06-30 15:07:59.000000 gilda-1.2.0/doc/modules/index.rst
+-rw-r--r--   0 ben        (503) staff       (20)      128 2023-06-30 15:07:59.000000 gilda-1.2.0/doc/requirements.txt
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-04-30 20:06:36.105535 gilda-1.2.0/gilda/
+-rw-r--r--   0 ben        (503) staff       (20)      768 2024-04-30 20:06:34.000000 gilda-1.2.0/gilda/__init__.py
+-rw-r--r--   0 ben        (503) staff       (20)     8879 2024-02-06 19:46:02.000000 gilda-1.2.0/gilda/api.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-04-30 20:06:36.106847 gilda-1.2.0/gilda/app/
+-rw-r--r--   0 ben        (503) staff       (20)      412 2023-06-30 15:07:59.000000 gilda-1.2.0/gilda/app/__init__.py
+-rw-r--r--   0 ben        (503) staff       (20)       59 2021-09-05 00:38:55.000000 gilda-1.2.0/gilda/app/__main__.py
+-rw-r--r--   0 ben        (503) staff       (20)    11668 2024-02-06 19:46:02.000000 gilda-1.2.0/gilda/app/app.py
+-rw-r--r--   0 ben        (503) staff       (20)      378 2024-02-06 19:46:02.000000 gilda-1.2.0/gilda/app/proxies.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-04-30 20:06:36.107443 gilda-1.2.0/gilda/app/templates/
+-rw-r--r--   0 ben        (503) staff       (20)     6663 2024-02-06 19:46:02.000000 gilda-1.2.0/gilda/app/templates/base.html
+-rw-r--r--   0 ben        (503) staff       (20)       92 2023-06-30 15:07:59.000000 gilda-1.2.0/gilda/app/templates/home.html
+-rw-r--r--   0 ben        (503) staff       (20)     2235 2023-06-30 15:07:59.000000 gilda-1.2.0/gilda/app/templates/matches.html
+-rw-r--r--   0 ben        (503) staff       (20)       96 2023-06-30 15:07:59.000000 gilda-1.2.0/gilda/app/templates/ner_home.html
+-rw-r--r--   0 ben        (503) staff       (20)     1838 2023-06-30 15:07:59.000000 gilda-1.2.0/gilda/app/templates/ner_matches.html
+-rw-r--r--   0 ben        (503) staff       (20)     3707 2024-02-06 19:46:02.000000 gilda-1.2.0/gilda/app/ui.py
+-rw-r--r--   0 ben        (503) staff       (20)    28683 2024-02-06 19:46:02.000000 gilda-1.2.0/gilda/generate_terms.py
+-rwxr-xr-x   0 ben        (503) staff       (20)     1584 2022-04-26 22:20:20.000000 gilda-1.2.0/gilda/greek_alphabet.py
+-rw-r--r--   0 ben        (503) staff       (20)    29560 2024-04-30 19:26:28.000000 gilda-1.2.0/gilda/grounder.py
+-rw-r--r--   0 ben        (503) staff       (20)     6898 2024-02-06 19:46:02.000000 gilda-1.2.0/gilda/ner.py
+-rw-r--r--   0 ben        (503) staff       (20)     3170 2024-02-06 19:46:02.000000 gilda-1.2.0/gilda/pandas_utils.py
+-rw-r--r--   0 ben        (503) staff       (20)     7755 2023-06-30 15:07:59.000000 gilda-1.2.0/gilda/process.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-04-30 20:06:36.108231 gilda-1.2.0/gilda/resources/
+-rw-r--r--   0 ben        (503) staff       (20)     2846 2022-06-21 14:02:33.000000 gilda-1.2.0/gilda/resources/__init__.py
+-rw-r--r--   0 ben        (503) staff       (20)      130 2021-09-05 00:38:55.000000 gilda-1.2.0/gilda/resources/__main__.py
+-rw-r--r--   0 ben        (503) staff       (20)    29081 2021-02-10 19:17:08.000000 gilda-1.2.0/gilda/resources/mesh_ambig_mappings.tsv
+-rw-r--r--   0 ben        (503) staff       (20)   362152 2021-02-10 19:17:08.000000 gilda-1.2.0/gilda/resources/mesh_mappings.tsv
+-rw-r--r--   0 ben        (503) staff       (20)     3331 2023-06-30 15:07:59.000000 gilda-1.2.0/gilda/resources/sqlite_adapter.py
+-rw-r--r--   0 ben        (503) staff       (20)     8205 2023-06-30 15:07:59.000000 gilda-1.2.0/gilda/scorer.py
+-rw-r--r--   0 ben        (503) staff       (20)     6602 2024-02-06 19:46:02.000000 gilda-1.2.0/gilda/term.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-04-30 20:06:36.109312 gilda-1.2.0/gilda/tests/
+-rw-r--r--   0 ben        (503) staff       (20)       47 2021-02-10 19:17:08.000000 gilda-1.2.0/gilda/tests/__init__.py
+-rw-r--r--   0 ben        (503) staff       (20)     2022 2022-04-26 22:20:20.000000 gilda-1.2.0/gilda/tests/test_api.py
+-rw-r--r--   0 ben        (503) staff       (20)     2972 2024-02-06 19:46:02.000000 gilda-1.2.0/gilda/tests/test_app.py
+-rw-r--r--   0 ben        (503) staff       (20)     5846 2023-06-30 15:07:59.000000 gilda-1.2.0/gilda/tests/test_generate_terms.py
+-rw-r--r--   0 ben        (503) staff       (20)     9552 2024-02-06 19:46:02.000000 gilda-1.2.0/gilda/tests/test_grounder.py
+-rw-r--r--   0 ben        (503) staff       (20)     2666 2024-02-06 19:46:02.000000 gilda-1.2.0/gilda/tests/test_ner.py
+-rw-r--r--   0 ben        (503) staff       (20)      543 2023-06-30 15:07:59.000000 gilda-1.2.0/gilda/tests/test_pandas_utils.py
+-rw-r--r--   0 ben        (503) staff       (20)     1644 2023-06-30 15:07:59.000000 gilda-1.2.0/gilda/tests/test_process.py
+-rw-r--r--   0 ben        (503) staff       (20)     1566 2021-02-10 19:17:08.000000 gilda-1.2.0/gilda/tests/test_scorer.py
+-rw-r--r--   0 ben        (503) staff       (20)     1238 2022-04-26 22:20:20.000000 gilda-1.2.0/gilda/tests/test_term.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-04-30 20:06:36.106262 gilda-1.2.0/gilda.egg-info/
+-rw-r--r--   0 ben        (503) staff       (20)     8222 2024-04-30 20:06:36.000000 gilda-1.2.0/gilda.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (503) staff       (20)     1187 2024-04-30 20:06:36.000000 gilda-1.2.0/gilda.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (503) staff       (20)        1 2024-04-30 20:06:36.000000 gilda-1.2.0/gilda.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (503) staff       (20)       41 2024-04-30 20:06:36.000000 gilda-1.2.0/gilda.egg-info/entry_points.txt
+-rw-r--r--   0 ben        (503) staff       (20)      340 2024-04-30 20:06:36.000000 gilda-1.2.0/gilda.egg-info/requires.txt
+-rw-r--r--   0 ben        (503) staff       (20)        6 2024-04-30 20:06:36.000000 gilda-1.2.0/gilda.egg-info/top_level.txt
+-rw-r--r--   0 ben        (503) staff       (20)       38 2024-04-30 20:06:36.109679 gilda-1.2.0/setup.cfg
+-rw-r--r--   0 ben        (503) staff       (20)     2300 2024-02-06 19:46:02.000000 gilda-1.2.0/setup.py
```

### Comparing `gilda-1.1.0/LICENSE` & `gilda-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/PKG-INFO` & `gilda-1.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: gilda
-Version: 1.1.0
-Summary: Grounding for biomedical entities with contextual disambiguation
-Home-page: https://github.com/indralab/gilda
-Author: Benjamin M. Gyori, Harvard Medical School
-Author-email: benjamin_gyori@hms.harvard.edu
-Keywords: nlp,biology
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: terms
-Provides-Extra: benchmarks
-Provides-Extra: ui
-Provides-Extra: docs
-License-File: LICENSE
-
 # Gilda: Grounding Integrating Learned Disambiguation
 [![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Build](https://github.com/indralab/gilda/actions/workflows/tests.yml/badge.svg)](https://github.com/indralab/gilda/actions)
 [![Documentation](https://readthedocs.org/projects/gilda/badge/?version=latest)](https://gilda.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/gilda.svg)](https://badge.fury.io/py/gilda)
 [![DOI](https://img.shields.io/badge/DOI-10.1093/bioadv/vbac034-green.svg)](https://doi.org/10.1093/bioadv/vbac034)
 
@@ -161,14 +140,31 @@
 Alternatively, you can use `docker-compose` to do both the initial build and
 run the container based on the `docker-compose.yml` configuration:
 
 ```shell
 $ docker-compose up
 ```
 
+## Default grounding resources
+
+Gilda is customizable with terms coming from different vocabularies. However,
+Gilda comes with a default set of resources from which terms are collected
+(almost 2 million entries as of v1.1.0), without any additional configuration
+needed. These resources include:
+- [HGNC](https://bioregistry.io/hgnc) (human genes)
+- [UniProt](https://bioregistry.io/uniprot) (human and model organism proteins)
+- [FamPlex](https://bioregistry.io/famplex) (human protein families and complexes)
+- [CHeBI](https://bioregistry.io/chebi) (small molecules, metabolites, etc.)
+- [GO](https://bioregistry.io/go) (biological processes, molecular functions, complexes)
+- [DOID](https://bioregistry.io/doid) (diseases)
+- [EFO](https://bioregistry.io/efo) (experimental factors: cell lines, cell types, anatomical entities, etc.)
+- [HP](https://bioregistry.io/hp) (human phenotypes)
+- [MeSH](https://bioregistry.io/mesh) (general: diseases, proteins, small molecules, cell types, etc.)
+- [Adeft](https://github.com/gyorilab/adeft) (misc. terms corresponding to ambiguous acronyms)
+
 ## Citation
 
 ```bibtex
 @article{gyori2022gilda,
     author = {Gyori, Benjamin M and Hoyt, Charles Tapley and Steppi, Albert},
     title = "{{Gilda: biomedical entity text normalization with machine-learned disambiguation as a service}}",
     journal = {Bioinformatics Advances},
```

### Comparing `gilda-1.1.0/README.md` & `gilda-1.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: gilda
+Version: 1.2.0
+Summary: Grounding for biomedical entities with contextual disambiguation
+Home-page: https://github.com/indralab/gilda
+Author: Benjamin M. Gyori, Harvard Medical School
+Author-email: benjamin_gyori@hms.harvard.edu
+Keywords: nlp,biology
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: terms
+Provides-Extra: benchmarks
+Provides-Extra: ui
+Provides-Extra: docs
+License-File: LICENSE
+
 # Gilda: Grounding Integrating Learned Disambiguation
 [![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Build](https://github.com/indralab/gilda/actions/workflows/tests.yml/badge.svg)](https://github.com/indralab/gilda/actions)
 [![Documentation](https://readthedocs.org/projects/gilda/badge/?version=latest)](https://gilda.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/gilda.svg)](https://badge.fury.io/py/gilda)
 [![DOI](https://img.shields.io/badge/DOI-10.1093/bioadv/vbac034-green.svg)](https://doi.org/10.1093/bioadv/vbac034)
 
@@ -140,14 +161,31 @@
 Alternatively, you can use `docker-compose` to do both the initial build and
 run the container based on the `docker-compose.yml` configuration:
 
 ```shell
 $ docker-compose up
 ```
 
+## Default grounding resources
+
+Gilda is customizable with terms coming from different vocabularies. However,
+Gilda comes with a default set of resources from which terms are collected
+(almost 2 million entries as of v1.1.0), without any additional configuration
+needed. These resources include:
+- [HGNC](https://bioregistry.io/hgnc) (human genes)
+- [UniProt](https://bioregistry.io/uniprot) (human and model organism proteins)
+- [FamPlex](https://bioregistry.io/famplex) (human protein families and complexes)
+- [CHeBI](https://bioregistry.io/chebi) (small molecules, metabolites, etc.)
+- [GO](https://bioregistry.io/go) (biological processes, molecular functions, complexes)
+- [DOID](https://bioregistry.io/doid) (diseases)
+- [EFO](https://bioregistry.io/efo) (experimental factors: cell lines, cell types, anatomical entities, etc.)
+- [HP](https://bioregistry.io/hp) (human phenotypes)
+- [MeSH](https://bioregistry.io/mesh) (general: diseases, proteins, small molecules, cell types, etc.)
+- [Adeft](https://github.com/gyorilab/adeft) (misc. terms corresponding to ambiguous acronyms)
+
 ## Citation
 
 ```bibtex
 @article{gyori2022gilda,
     author = {Gyori, Benjamin M and Hoyt, Charles Tapley and Steppi, Albert},
     title = "{{Gilda: biomedical entity text normalization with machine-learned disambiguation as a service}}",
     journal = {Bioinformatics Advances},
```

### Comparing `gilda-1.1.0/doc/Makefile` & `gilda-1.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/doc/conf.py` & `gilda-1.2.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/doc/make.bat` & `gilda-1.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/doc/modules/index.rst` & `gilda-1.2.0/doc/modules/index.rst`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/__init__.py` & `gilda-1.2.0/gilda/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.1.0'
+__version__ = '1.2.0'
 
 import logging
 
 from .api import get_grounder, get_models, get_names, ground, make_grounder, annotate
 from .grounder import Grounder, ScoredMatch
 from .pandas_utils import ground_df, ground_df_map
 from .term import Term, dump_terms
```

### Comparing `gilda-1.1.0/gilda/api.py` & `gilda-1.2.0/gilda/api.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/app/app.py` & `gilda-1.2.0/gilda/app/app.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/app/templates/base.html` & `gilda-1.2.0/gilda/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/app/templates/matches.html` & `gilda-1.2.0/gilda/app/templates/matches.html`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/app/templates/ner_matches.html` & `gilda-1.2.0/gilda/app/templates/ner_matches.html`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/app/ui.py` & `gilda-1.2.0/gilda/app/ui.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/generate_terms.py` & `gilda-1.2.0/gilda/generate_terms.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/greek_alphabet.py` & `gilda-1.2.0/gilda/greek_alphabet.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/grounder.py` & `gilda-1.2.0/gilda/grounder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import os
 import csv
 import json
 import gzip
 import logging
 import itertools
 import collections.abc
+import tempfile
 from pathlib import Path
 from collections import defaultdict, Counter
 from textwrap import dedent
 from typing import Iterator, List, Mapping, Optional, Set, Tuple, Union, Iterable
+from urllib.request import urlretrieve
+
 from adeft.disambiguate import load_disambiguator
 from adeft.modeling.classify import load_model_info
 from adeft import available_shortforms as available_adeft_models
 from .term import Term, get_identifiers_curie, get_identifiers_url
 from .process import normalize, replace_dashes, replace_greek_uni, \
     replace_greek_latin, replace_greek_spelled_out, depluralize, \
     replace_roman_arabic
@@ -49,15 +52,15 @@
     terms :
         Specifies the grounding terms that should be loaded in the Grounder.
 
         - If ``None``, the default grounding terms are loaded from the
           versioned resource folder.
         - If :class:`str` or :class:`pathlib.Path`, it is interpreted
           as a path to a grounding terms gzipped TSV file which is then
-          loaded.
+          loaded. If it's a str and looks like a URL, will be downloaded from the internet
         - If :class:`dict`, it is assumed to be a grounding terms dict with
           normalized entity strings as keys and :class:`gilda.term.Term`
           instances as values.
         - If :class:`list`, :class:`set`, :class:`tuple`, or any other iterable,
           it is assumed to be a flat list of
           :class:`gilda.term.Term` instances.
     namespace_priority :
@@ -76,15 +79,20 @@
         terms: Optional[GrounderInput] = None,
         *,
         namespace_priority: Optional[List[str]] = None,
     ):
         if terms is None:
             terms = get_grounding_terms()
 
-        if isinstance(terms, (str, Path)):
+        if isinstance(terms, str) and terms.startswith("http"):
+            with tempfile.TemporaryDirectory() as directory:
+                path = Path(directory).joinpath("terms.tsv.gz")
+                urlretrieve(terms, path)  # noqa:S310
+                self.entries = load_terms_file(path)
+        elif isinstance(terms, (str, Path)):
             extension = os.path.splitext(terms)[1]
             if extension == '.db':
                 from .resources.sqlite_adapter import SqliteEntries
                 self.entries = SqliteEntries(terms)
             else:
                 self.entries = load_terms_file(terms)
         elif isinstance(terms, dict):
```

### Comparing `gilda-1.1.0/gilda/ner.py` & `gilda-1.2.0/gilda/ner.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/pandas_utils.py` & `gilda-1.2.0/gilda/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/process.py` & `gilda-1.2.0/gilda/process.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/resources/__init__.py` & `gilda-1.2.0/gilda/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/resources/mesh_ambig_mappings.tsv` & `gilda-1.2.0/gilda/resources/mesh_ambig_mappings.tsv`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/resources/mesh_mappings.tsv` & `gilda-1.2.0/gilda/resources/mesh_mappings.tsv`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/resources/sqlite_adapter.py` & `gilda-1.2.0/gilda/resources/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/scorer.py` & `gilda-1.2.0/gilda/scorer.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/term.py` & `gilda-1.2.0/gilda/term.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/tests/test_api.py` & `gilda-1.2.0/gilda/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/tests/test_app.py` & `gilda-1.2.0/gilda/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/tests/test_generate_terms.py` & `gilda-1.2.0/gilda/tests/test_generate_terms.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/tests/test_grounder.py` & `gilda-1.2.0/gilda/tests/test_grounder.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/tests/test_ner.py` & `gilda-1.2.0/gilda/tests/test_ner.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/tests/test_pandas_utils.py` & `gilda-1.2.0/gilda/tests/test_pandas_utils.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/tests/test_process.py` & `gilda-1.2.0/gilda/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/tests/test_scorer.py` & `gilda-1.2.0/gilda/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda/tests/test_term.py` & `gilda-1.2.0/gilda/tests/test_term.py`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/gilda.egg-info/PKG-INFO` & `gilda-1.2.0/gilda.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gilda
-Version: 1.1.0
+Version: 1.2.0
 Summary: Grounding for biomedical entities with contextual disambiguation
 Home-page: https://github.com/indralab/gilda
 Author: Benjamin M. Gyori, Harvard Medical School
 Author-email: benjamin_gyori@hms.harvard.edu
 Keywords: nlp,biology
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -161,14 +161,31 @@
 Alternatively, you can use `docker-compose` to do both the initial build and
 run the container based on the `docker-compose.yml` configuration:
 
 ```shell
 $ docker-compose up
 ```
 
+## Default grounding resources
+
+Gilda is customizable with terms coming from different vocabularies. However,
+Gilda comes with a default set of resources from which terms are collected
+(almost 2 million entries as of v1.1.0), without any additional configuration
+needed. These resources include:
+- [HGNC](https://bioregistry.io/hgnc) (human genes)
+- [UniProt](https://bioregistry.io/uniprot) (human and model organism proteins)
+- [FamPlex](https://bioregistry.io/famplex) (human protein families and complexes)
+- [CHeBI](https://bioregistry.io/chebi) (small molecules, metabolites, etc.)
+- [GO](https://bioregistry.io/go) (biological processes, molecular functions, complexes)
+- [DOID](https://bioregistry.io/doid) (diseases)
+- [EFO](https://bioregistry.io/efo) (experimental factors: cell lines, cell types, anatomical entities, etc.)
+- [HP](https://bioregistry.io/hp) (human phenotypes)
+- [MeSH](https://bioregistry.io/mesh) (general: diseases, proteins, small molecules, cell types, etc.)
+- [Adeft](https://github.com/gyorilab/adeft) (misc. terms corresponding to ambiguous acronyms)
+
 ## Citation
 
 ```bibtex
 @article{gyori2022gilda,
     author = {Gyori, Benjamin M and Hoyt, Charles Tapley and Steppi, Albert},
     title = "{{Gilda: biomedical entity text normalization with machine-learned disambiguation as a service}}",
     journal = {Bioinformatics Advances},
```

### Comparing `gilda-1.1.0/gilda.egg-info/SOURCES.txt` & `gilda-1.2.0/gilda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gilda-1.1.0/setup.py` & `gilda-1.2.0/setup.py`

 * *Files identical despite different names*

