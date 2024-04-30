# Comparing `tmp/maxgcp-0.1.0.tar.gz` & `tmp/maxgcp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxgcp-0.1.0.tar", last modified: Tue Apr 30 17:21:44 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `maxgcp-0.1.0.tar` & `maxgcp-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,13 @@
-drwxr-xr-x   0 zietzm     (501) staff       (20)        0 2024-04-30 17:21:44.806846 maxgcp-0.1.0/
--rw-r--r--   0 zietzm     (501) staff       (20)     1073 2024-04-30 17:21:44.806339 maxgcp-0.1.0/PKG-INFO
--rw-r--r--   0 zietzm     (501) staff       (20)      801 2023-10-31 00:44:54.000000 maxgcp-0.1.0/README.md
--rw-r--r--   0 zietzm     (501) staff       (20)      492 2024-04-30 17:21:13.000000 maxgcp-0.1.0/pyproject.toml
--rw-r--r--   0 zietzm     (501) staff       (20)       38 2024-04-30 17:21:44.806982 maxgcp-0.1.0/setup.cfg
-drwxr-xr-x   0 zietzm     (501) staff       (20)        0 2024-04-30 17:21:44.801254 maxgcp-0.1.0/src/
-drwxr-xr-x   0 zietzm     (501) staff       (20)        0 2024-04-30 17:21:44.803007 maxgcp-0.1.0/src/maxgcp/
--rw-r--r--   0 zietzm     (501) staff       (20)      124 2024-01-11 19:05:54.000000 maxgcp-0.1.0/src/maxgcp/__init__.py
--rw-r--r--   0 zietzm     (501) staff       (20)     4154 2024-04-30 17:20:33.000000 maxgcp-0.1.0/src/maxgcp/estimators.py
--rw-r--r--   0 zietzm     (501) staff       (20)        0 2024-01-17 15:37:33.000000 maxgcp-0.1.0/src/maxgcp/py.typed
--rw-r--r--   0 zietzm     (501) staff       (20)     1205 2024-01-17 15:37:27.000000 maxgcp-0.1.0/src/maxgcp/summary.py
-drwxr-xr-x   0 zietzm     (501) staff       (20)        0 2024-04-30 17:21:44.805368 maxgcp-0.1.0/src/maxgcp.egg-info/
--rw-r--r--   0 zietzm     (501) staff       (20)     1073 2024-04-30 17:21:44.000000 maxgcp-0.1.0/src/maxgcp.egg-info/PKG-INFO
--rw-r--r--   0 zietzm     (501) staff       (20)      283 2024-04-30 17:21:44.000000 maxgcp-0.1.0/src/maxgcp.egg-info/SOURCES.txt
--rw-r--r--   0 zietzm     (501) staff       (20)        1 2024-04-30 17:21:44.000000 maxgcp-0.1.0/src/maxgcp.egg-info/dependency_links.txt
--rw-r--r--   0 zietzm     (501) staff       (20)       28 2024-04-30 17:21:44.000000 maxgcp-0.1.0/src/maxgcp.egg-info/requires.txt
--rw-r--r--   0 zietzm     (501) staff       (20)        7 2024-04-30 17:21:44.000000 maxgcp-0.1.0/src/maxgcp.egg-info/top_level.txt
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 maxgcp-0.1.1/requirements-dev.lock
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 maxgcp-0.1.1/requirements.lock
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 maxgcp-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 maxgcp-0.1.1/src/maxgcp/__init__.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 maxgcp-0.1.1/src/maxgcp/estimators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maxgcp-0.1.1/src/maxgcp/py.typed
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 maxgcp-0.1.1/src/maxgcp/summary.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maxgcp-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 maxgcp-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 maxgcp-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 maxgcp-0.1.1/README.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 maxgcp-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 maxgcp-0.1.1/PKG-INFO
```

### Comparing `maxgcp-0.1.0/README.md` & `maxgcp-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Maximum genetic component phenotyping
 
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Actions status](https://img.shields.io/github/actions/workflow/status/tatonetti-lab/maxgcp/test.yml?branch=main&label=actions)](https://github.com/tatonetti-lab/maxgcp/actions)
 
 `maxgcp` is a Python package that implements maximum genetic component phenotyping (MaxGCP), a method that optimizes a linear phenotype definition to maximize its heritability and genetic correlation with a trait of interest.
 In short, this method results in a phenotype definition that is, close to the genetic component of the trait of interest, on the individual level.
 This phenotype definition can be used in various applications, including enhancement of statistical power in genome-wide association studies (GWAS).
 `maxgcp` requires only estimates of genetic and phenotypic covariances, which can be obtained from GWAS summary statistics.
```

### Comparing `maxgcp-0.1.0/src/maxgcp/estimators.py` & `maxgcp-0.1.1/src/maxgcp/estimators.py`

 * *Files identical despite different names*

### Comparing `maxgcp-0.1.0/src/maxgcp/summary.py` & `maxgcp-0.1.1/src/maxgcp/summary.py`

 * *Files identical despite different names*

