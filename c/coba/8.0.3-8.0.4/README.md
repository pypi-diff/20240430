# Comparing `tmp/coba-8.0.3.tar.gz` & `tmp/coba-8.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coba-8.0.3.tar", last modified: Sat Feb 24 20:11:14 2024, max compression
+gzip compressed data, was "coba-8.0.4.tar", last modified: Tue Apr 30 15:53:38 2024, max compression
```

## Comparing `coba-8.0.3.tar` & `coba-8.0.4.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 20:11:14.996173 coba-8.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-24 20:11:07.000000 coba-8.0.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-24 20:11:07.000000 coba-8.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-02-24 20:11:14.996173 coba-8.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-02-24 20:11:07.000000 coba-8.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 20:11:14.984173 coba-8.0.3/coba/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-24 20:11:07.000000 coba-8.0.3/coba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-24 20:11:07.000000 coba-8.0.3/coba/backports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 20:11:14.988173 coba-8.0.3/coba/context/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-24 20:11:07.000000 coba-8.0.3/coba/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-02-24 20:11:07.000000 coba-8.0.3/coba/context/cachers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-02-24 20:11:07.000000 coba-8.0.3/coba/context/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-02-24 20:11:07.000000 coba-8.0.3/coba/context/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-24 20:11:07.000000 coba-8.0.3/coba/contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-02-24 20:11:07.000000 coba-8.0.3/coba/encodings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 20:11:14.988173 coba-8.0.3/coba/environments/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-02-24 20:11:07.000000 coba-8.0.3/coba/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45104 2024-02-24 20:11:07.000000 coba-8.0.3/coba/environments/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    63249 2024-02-24 20:11:07.000000 coba-8.0.3/coba/environments/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12684 2024-02-24 20:11:07.000000 coba-8.0.3/coba/environments/openml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-02-24 20:11:07.000000 coba-8.0.3/coba/environments/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-02-24 20:11:07.000000 coba-8.0.3/coba/environments/serialized.py
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-02-24 20:11:07.000000 coba-8.0.3/coba/environments/supervised.py
--rw-r--r--   0 runner    (1001) docker     (127)    28185 2024-02-24 20:11:07.000000 coba-8.0.3/coba/environments/synthetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-02-24 20:11:07.000000 coba-8.0.3/coba/environments/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 20:11:14.988173 coba-8.0.3/coba/evaluators/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-24 20:11:07.000000 coba-8.0.3/coba/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-02-24 20:11:07.000000 coba-8.0.3/coba/evaluators/offline.py
--rw-r--r--   0 runner    (1001) docker     (127)    24816 2024-02-24 20:11:07.000000 coba-8.0.3/coba/evaluators/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-02-24 20:11:07.000000 coba-8.0.3/coba/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 20:11:14.992173 coba-8.0.3/coba/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-24 20:11:07.000000 coba-8.0.3/coba/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-02-24 20:11:07.000000 coba-8.0.3/coba/experiments/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-02-24 20:11:07.000000 coba-8.0.3/coba/experiments/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-02-24 20:11:07.000000 coba-8.0.3/coba/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 20:11:14.992173 coba-8.0.3/coba/learners/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-02-24 20:11:07.000000 coba-8.0.3/coba/learners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-02-24 20:11:07.000000 coba-8.0.3/coba/learners/bandit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-02-24 20:11:07.000000 coba-8.0.3/coba/learners/corral.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-02-24 20:11:07.000000 coba-8.0.3/coba/learners/lints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-02-24 20:11:07.000000 coba-8.0.3/coba/learners/linucb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-02-24 20:11:07.000000 coba-8.0.3/coba/learners/misguided.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-02-24 20:11:07.000000 coba-8.0.3/coba/learners/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    31782 2024-02-24 20:11:07.000000 coba-8.0.3/coba/learners/vowpal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-02-24 20:11:07.000000 coba-8.0.3/coba/multiprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 20:11:14.992173 coba-8.0.3/coba/pipes/
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-02-24 20:11:07.000000 coba-8.0.3/coba/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-02-24 20:11:07.000000 coba-8.0.3/coba/pipes/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14927 2024-02-24 20:11:07.000000 coba-8.0.3/coba/pipes/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-02-24 20:11:07.000000 coba-8.0.3/coba/pipes/lines.py
--rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-02-24 20:11:07.000000 coba-8.0.3/coba/pipes/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-02-24 20:11:07.000000 coba-8.0.3/coba/pipes/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19967 2024-02-24 20:11:07.000000 coba-8.0.3/coba/pipes/rows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-02-24 20:11:07.000000 coba-8.0.3/coba/pipes/sinks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-02-24 20:11:07.000000 coba-8.0.3/coba/pipes/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-24 20:11:07.000000 coba-8.0.3/coba/pipes/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    21025 2024-02-24 20:11:07.000000 coba-8.0.3/coba/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-02-24 20:11:07.000000 coba-8.0.3/coba/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-02-24 20:11:07.000000 coba-8.0.3/coba/register.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-02-24 20:11:07.000000 coba-8.0.3/coba/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 20:11:14.992173 coba-8.0.3/coba/results/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-24 20:11:07.000000 coba-8.0.3/coba/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    85858 2024-02-24 20:11:07.000000 coba-8.0.3/coba/results/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-02-24 20:11:07.000000 coba-8.0.3/coba/results/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17102 2024-02-24 20:11:07.000000 coba-8.0.3/coba/safety.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-02-24 20:11:07.000000 coba-8.0.3/coba/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-02-24 20:11:07.000000 coba-8.0.3/coba/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 20:11:14.996173 coba-8.0.3/coba.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-02-24 20:11:14.000000 coba-8.0.3/coba.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-02-24 20:11:14.000000 coba-8.0.3/coba.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 20:11:14.000000 coba-8.0.3/coba.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-24 20:11:14.000000 coba-8.0.3/coba.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-24 20:11:14.000000 coba-8.0.3/coba.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-24 20:11:14.000000 coba-8.0.3/coba.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-02-24 20:11:07.000000 coba-8.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-24 20:11:14.996173 coba-8.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.672798 coba-8.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:53:34.000000 coba-8.0.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-30 15:53:34.000000 coba-8.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-30 15:53:38.672798 coba-8.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-30 15:53:34.000000 coba-8.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.664798 coba-8.0.4/coba/
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-30 15:53:34.000000 coba-8.0.4/coba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-30 15:53:34.000000 coba-8.0.4/coba/backports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.664798 coba-8.0.4/coba/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-30 15:53:34.000000 coba-8.0.4/coba/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-04-30 15:53:34.000000 coba-8.0.4/coba/context/cachers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-30 15:53:34.000000 coba-8.0.4/coba/context/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-30 15:53:34.000000 coba-8.0.4/coba/context/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 15:53:34.000000 coba-8.0.4/coba/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-04-30 15:53:34.000000 coba-8.0.4/coba/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.668798 coba-8.0.4/coba/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45104 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63249 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12684 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/openml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/serialized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/supervised.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28215 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/synthetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.668798 coba-8.0.4/coba/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-30 15:53:34.000000 coba-8.0.4/coba/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-04-30 15:53:34.000000 coba-8.0.4/coba/evaluators/offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24816 2024-04-30 15:53:34.000000 coba-8.0.4/coba/evaluators/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-30 15:53:34.000000 coba-8.0.4/coba/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.668798 coba-8.0.4/coba/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 15:53:34.000000 coba-8.0.4/coba/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-04-30 15:53:34.000000 coba-8.0.4/coba/experiments/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-04-30 15:53:34.000000 coba-8.0.4/coba/experiments/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-30 15:53:34.000000 coba-8.0.4/coba/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.668798 coba-8.0.4/coba/learners/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/corral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/lints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/linucb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/misguided.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31782 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/vowpal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-30 15:53:34.000000 coba-8.0.4/coba/multiprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.672798 coba-8.0.4/coba/pipes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14927 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19967 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/rows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/sinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21025 2024-04-30 15:53:34.000000 coba-8.0.4/coba/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-04-30 15:53:34.000000 coba-8.0.4/coba/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-30 15:53:34.000000 coba-8.0.4/coba/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-30 15:53:34.000000 coba-8.0.4/coba/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.672798 coba-8.0.4/coba/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-30 15:53:34.000000 coba-8.0.4/coba/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85885 2024-04-30 15:53:34.000000 coba-8.0.4/coba/results/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-30 15:53:34.000000 coba-8.0.4/coba/results/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17102 2024-04-30 15:53:34.000000 coba-8.0.4/coba/safety.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-30 15:53:34.000000 coba-8.0.4/coba/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-04-30 15:53:34.000000 coba-8.0.4/coba/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.672798 coba-8.0.4/coba.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-30 15:53:38.000000 coba-8.0.4/coba.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-30 15:53:38.000000 coba-8.0.4/coba.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:53:38.000000 coba-8.0.4/coba.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-30 15:53:38.000000 coba-8.0.4/coba.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 15:53:38.000000 coba-8.0.4/coba.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 15:53:38.000000 coba-8.0.4/coba.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-30 15:53:34.000000 coba-8.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:53:38.672798 coba-8.0.4/setup.cfg
```

### Comparing `coba-8.0.3/LICENSE` & `coba-8.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/PKG-INFO` & `coba-8.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coba
-Version: 8.0.3
+Version: 8.0.4
 Summary: A contextual bandit research package
 Author-email: Mark Rucker <rucker.mark@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://coba-docs.readthedocs.io/
 Project-URL: Documentation, https://coba-docs.readthedocs.io/
 Project-URL: Repository, https://github.com/vowpalwabbit/coba
 Classifier: Intended Audience :: Science/Research
@@ -23,16 +23,16 @@
 Requires-Dist: numpy; extra == "full"
 Requires-Dist: scipy; extra == "full"
 Requires-Dist: cloudpickle; extra == "full"
 Requires-Dist: torch; extra == "full"
 
 [![codecov](https://codecov.io/gh/VowpalWabbit/coba/branch/master/graph/badge.svg?token=885XLZJ2D4)](https://codecov.io/gh/VowpalWabbit/coba)
 [![binder](https://img.shields.io/badge/launch%20example-binder-579ACA.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAB8lBMVEX///9XmsrmZYH1olJXmsr1olJXmsrmZYH1olJXmsr1olJXmsrmZYH1olL1olJXmsr1olJXmsrmZYH1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olJXmsrmZYH1olL1olL0nFf1olJXmsrmZYH1olJXmsq8dZb1olJXmsrmZYH1olJXmspXmspXmsr1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olLeaIVXmsrmZYH1olL1olL1olJXmsrmZYH1olLna31Xmsr1olJXmsr1olJXmsrmZYH1olLqoVr1olJXmsr1olJXmsrmZYH1olL1olKkfaPobXvviGabgadXmsqThKuofKHmZ4Dobnr1olJXmsr1olJXmspXmsr1olJXmsrfZ4TuhWn1olL1olJXmsqBi7X1olJXmspZmslbmMhbmsdemsVfl8ZgmsNim8Jpk8F0m7R4m7F5nLB6jbh7jbiDirOEibOGnKaMhq+PnaCVg6qWg6qegKaff6WhnpKofKGtnomxeZy3noG6dZi+n3vCcpPDcpPGn3bLb4/Mb47UbIrVa4rYoGjdaIbeaIXhoWHmZYHobXvpcHjqdHXreHLroVrsfG/uhGnuh2bwj2Hxk17yl1vzmljzm1j0nlX1olL3AJXWAAAAbXRSTlMAEBAQHx8gICAuLjAwMDw9PUBAQEpQUFBXV1hgYGBkcHBwcXl8gICAgoiIkJCQlJicnJ2goKCmqK+wsLC4usDAwMjP0NDQ1NbW3Nzg4ODi5+3v8PDw8/T09PX29vb39/f5+fr7+/z8/Pz9/v7+zczCxgAABC5JREFUeAHN1ul3k0UUBvCb1CTVpmpaitAGSLSpSuKCLWpbTKNJFGlcSMAFF63iUmRccNG6gLbuxkXU66JAUef/9LSpmXnyLr3T5AO/rzl5zj137p136BISy44fKJXuGN/d19PUfYeO67Znqtf2KH33Id1psXoFdW30sPZ1sMvs2D060AHqws4FHeJojLZqnw53cmfvg+XR8mC0OEjuxrXEkX5ydeVJLVIlV0e10PXk5k7dYeHu7Cj1j+49uKg7uLU61tGLw1lq27ugQYlclHC4bgv7VQ+TAyj5Zc/UjsPvs1sd5cWryWObtvWT2EPa4rtnWW3JkpjggEpbOsPr7F7EyNewtpBIslA7p43HCsnwooXTEc3UmPmCNn5lrqTJxy6nRmcavGZVt/3Da2pD5NHvsOHJCrdc1G2r3DITpU7yic7w/7Rxnjc0kt5GC4djiv2Sz3Fb2iEZg41/ddsFDoyuYrIkmFehz0HR2thPgQqMyQYb2OtB0WxsZ3BeG3+wpRb1vzl2UYBog8FfGhttFKjtAclnZYrRo9ryG9uG/FZQU4AEg8ZE9LjGMzTmqKXPLnlWVnIlQQTvxJf8ip7VgjZjyVPrjw1te5otM7RmP7xm+sK2Gv9I8Gi++BRbEkR9EBw8zRUcKxwp73xkaLiqQb+kGduJTNHG72zcW9LoJgqQxpP3/Tj//c3yB0tqzaml05/+orHLksVO+95kX7/7qgJvnjlrfr2Ggsyx0eoy9uPzN5SPd86aXggOsEKW2Prz7du3VID3/tzs/sSRs2w7ovVHKtjrX2pd7ZMlTxAYfBAL9jiDwfLkq55Tm7ifhMlTGPyCAs7RFRhn47JnlcB9RM5T97ASuZXIcVNuUDIndpDbdsfrqsOppeXl5Y+XVKdjFCTh+zGaVuj0d9zy05PPK3QzBamxdwtTCrzyg/2Rvf2EstUjordGwa/kx9mSJLr8mLLtCW8HHGJc2R5hS219IiF6PnTusOqcMl57gm0Z8kanKMAQg0qSyuZfn7zItsbGyO9QlnxY0eCuD1XL2ys/MsrQhltE7Ug0uFOzufJFE2PxBo/YAx8XPPdDwWN0MrDRYIZF0mSMKCNHgaIVFoBbNoLJ7tEQDKxGF0kcLQimojCZopv0OkNOyWCCg9XMVAi7ARJzQdM2QUh0gmBozjc3Skg6dSBRqDGYSUOu66Zg+I2fNZs/M3/f/Grl/XnyF1Gw3VKCez0PN5IUfFLqvgUN4C0qNqYs5YhPL+aVZYDE4IpUk57oSFnJm4FyCqqOE0jhY2SMyLFoo56zyo6becOS5UVDdj7Vih0zp+tcMhwRpBeLyqtIjlJKAIZSbI8SGSF3k0pA3mR5tHuwPFoa7N7reoq2bqCsAk1HqCu5uvI1n6JuRXI+S1Mco54YmYTwcn6Aeic+kssXi8XpXC4V3t7/ADuTNKaQJdScAAAAAElFTkSuQmCC)](https://mybinder.org/v2/gh/VowpalWabbit/Coba/HEAD?filepath=doc/source/notebooks)
-[![doc](https://readthedocs.org/projects/coba-docs/badge/?version=latest)](https://coba-docs.readthedocs.io/en/latest/?badge=latest)
-[![pypi](https://img.shields.io/badge/pypi-v8.0.2-blue)](https://pypi.org/project/coba/)
+[![doc](https://readthedocs.org/projects/coba-docs/badge/?version=latest)](https://coba-docs.readthedocs.io/?badge=v8.0.3)
+[![pypi](https://img.shields.io/badge/pypi-v8.0.3-blue)](https://pypi.org/project/coba/)
 
 # Coba
 
  ### What is it?
 
  Coba is a powerful framework built to facilitate research with online contextual bandit (CB) algorithms.
```

### Comparing `coba-8.0.3/README.md` & `coba-8.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![codecov](https://codecov.io/gh/VowpalWabbit/coba/branch/master/graph/badge.svg?token=885XLZJ2D4)](https://codecov.io/gh/VowpalWabbit/coba)
 [![binder](https://img.shields.io/badge/launch%20example-binder-579ACA.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAB8lBMVEX///9XmsrmZYH1olJXmsr1olJXmsrmZYH1olJXmsr1olJXmsrmZYH1olL1olJXmsr1olJXmsrmZYH1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olJXmsrmZYH1olL1olL0nFf1olJXmsrmZYH1olJXmsq8dZb1olJXmsrmZYH1olJXmspXmspXmsr1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olLeaIVXmsrmZYH1olL1olL1olJXmsrmZYH1olLna31Xmsr1olJXmsr1olJXmsrmZYH1olLqoVr1olJXmsr1olJXmsrmZYH1olL1olKkfaPobXvviGabgadXmsqThKuofKHmZ4Dobnr1olJXmsr1olJXmspXmsr1olJXmsrfZ4TuhWn1olL1olJXmsqBi7X1olJXmspZmslbmMhbmsdemsVfl8ZgmsNim8Jpk8F0m7R4m7F5nLB6jbh7jbiDirOEibOGnKaMhq+PnaCVg6qWg6qegKaff6WhnpKofKGtnomxeZy3noG6dZi+n3vCcpPDcpPGn3bLb4/Mb47UbIrVa4rYoGjdaIbeaIXhoWHmZYHobXvpcHjqdHXreHLroVrsfG/uhGnuh2bwj2Hxk17yl1vzmljzm1j0nlX1olL3AJXWAAAAbXRSTlMAEBAQHx8gICAuLjAwMDw9PUBAQEpQUFBXV1hgYGBkcHBwcXl8gICAgoiIkJCQlJicnJ2goKCmqK+wsLC4usDAwMjP0NDQ1NbW3Nzg4ODi5+3v8PDw8/T09PX29vb39/f5+fr7+/z8/Pz9/v7+zczCxgAABC5JREFUeAHN1ul3k0UUBvCb1CTVpmpaitAGSLSpSuKCLWpbTKNJFGlcSMAFF63iUmRccNG6gLbuxkXU66JAUef/9LSpmXnyLr3T5AO/rzl5zj137p136BISy44fKJXuGN/d19PUfYeO67Znqtf2KH33Id1psXoFdW30sPZ1sMvs2D060AHqws4FHeJojLZqnw53cmfvg+XR8mC0OEjuxrXEkX5ydeVJLVIlV0e10PXk5k7dYeHu7Cj1j+49uKg7uLU61tGLw1lq27ugQYlclHC4bgv7VQ+TAyj5Zc/UjsPvs1sd5cWryWObtvWT2EPa4rtnWW3JkpjggEpbOsPr7F7EyNewtpBIslA7p43HCsnwooXTEc3UmPmCNn5lrqTJxy6nRmcavGZVt/3Da2pD5NHvsOHJCrdc1G2r3DITpU7yic7w/7Rxnjc0kt5GC4djiv2Sz3Fb2iEZg41/ddsFDoyuYrIkmFehz0HR2thPgQqMyQYb2OtB0WxsZ3BeG3+wpRb1vzl2UYBog8FfGhttFKjtAclnZYrRo9ryG9uG/FZQU4AEg8ZE9LjGMzTmqKXPLnlWVnIlQQTvxJf8ip7VgjZjyVPrjw1te5otM7RmP7xm+sK2Gv9I8Gi++BRbEkR9EBw8zRUcKxwp73xkaLiqQb+kGduJTNHG72zcW9LoJgqQxpP3/Tj//c3yB0tqzaml05/+orHLksVO+95kX7/7qgJvnjlrfr2Ggsyx0eoy9uPzN5SPd86aXggOsEKW2Prz7du3VID3/tzs/sSRs2w7ovVHKtjrX2pd7ZMlTxAYfBAL9jiDwfLkq55Tm7ifhMlTGPyCAs7RFRhn47JnlcB9RM5T97ASuZXIcVNuUDIndpDbdsfrqsOppeXl5Y+XVKdjFCTh+zGaVuj0d9zy05PPK3QzBamxdwtTCrzyg/2Rvf2EstUjordGwa/kx9mSJLr8mLLtCW8HHGJc2R5hS219IiF6PnTusOqcMl57gm0Z8kanKMAQg0qSyuZfn7zItsbGyO9QlnxY0eCuD1XL2ys/MsrQhltE7Ug0uFOzufJFE2PxBo/YAx8XPPdDwWN0MrDRYIZF0mSMKCNHgaIVFoBbNoLJ7tEQDKxGF0kcLQimojCZopv0OkNOyWCCg9XMVAi7ARJzQdM2QUh0gmBozjc3Skg6dSBRqDGYSUOu66Zg+I2fNZs/M3/f/Grl/XnyF1Gw3VKCez0PN5IUfFLqvgUN4C0qNqYs5YhPL+aVZYDE4IpUk57oSFnJm4FyCqqOE0jhY2SMyLFoo56zyo6becOS5UVDdj7Vih0zp+tcMhwRpBeLyqtIjlJKAIZSbI8SGSF3k0pA3mR5tHuwPFoa7N7reoq2bqCsAk1HqCu5uvI1n6JuRXI+S1Mco54YmYTwcn6Aeic+kssXi8XpXC4V3t7/ADuTNKaQJdScAAAAAElFTkSuQmCC)](https://mybinder.org/v2/gh/VowpalWabbit/Coba/HEAD?filepath=doc/source/notebooks)
-[![doc](https://readthedocs.org/projects/coba-docs/badge/?version=latest)](https://coba-docs.readthedocs.io/en/latest/?badge=latest)
-[![pypi](https://img.shields.io/badge/pypi-v8.0.2-blue)](https://pypi.org/project/coba/)
+[![doc](https://readthedocs.org/projects/coba-docs/badge/?version=latest)](https://coba-docs.readthedocs.io/?badge=v8.0.3)
+[![pypi](https://img.shields.io/badge/pypi-v8.0.3-blue)](https://pypi.org/project/coba/)
 
 # Coba
 
  ### What is it?
 
  Coba is a powerful framework built to facilitate research with online contextual bandit (CB) algorithms.
```

### Comparing `coba-8.0.3/coba/__init__.py` & `coba-8.0.4/coba/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 from coba.statistics import mean
 
 from coba.primitives import is_batch, Context, Action, Actions, Categorical, Dense, Sparse
 from coba.primitives import Learner, Environment, Interaction, Evaluator, Rewards, Namespaces
 from coba.primitives import LoggedInteraction, SimulatedInteraction, GroundedInteraction
 from coba.primitives import L1Reward, HammingReward, DiscreteReward
 
-__version__ = "8.0.3"
+__version__ = "8.0.4"
```

### Comparing `coba-8.0.3/coba/context/cachers.py` & `coba-8.0.4/coba/context/cachers.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/context/core.py` & `coba-8.0.4/coba/context/core.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/context/loggers.py` & `coba-8.0.4/coba/context/loggers.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/encodings.py` & `coba-8.0.4/coba/encodings.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/environments/__init__.py` & `coba-8.0.4/coba/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/environments/core.py` & `coba-8.0.4/coba/environments/core.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/environments/filters.py` & `coba-8.0.4/coba/environments/filters.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/environments/openml.py` & `coba-8.0.4/coba/environments/openml.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/environments/results.py` & `coba-8.0.4/coba/environments/results.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/environments/serialized.py` & `coba-8.0.4/coba/environments/serialized.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/environments/supervised.py` & `coba-8.0.4/coba/environments/supervised.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/environments/synthetics.py` & `coba-8.0.4/coba/environments/synthetics.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,14 +340,16 @@
             worlds = [list(zip(context_iter,rng.randoms(n_neighborhoods))) for _ in range(n_actions)]
         else:
             worlds = [list(zip(map(add,(c or [] for c in context_iter),action_iter),rng.randoms(n_neighborhoods))) for _ in range(n_actions)]
 
         def f(x):
             return [ min(world, key=lambda w: dist(w[0],x))[1] for world in worlds ]
 
+        self.worlds = worlds
+
         for _ in range(n_interactions):
 
             context = next(context_iter)
             actions = next(actions_iter)
 
             if n_action_feats:
                 rewards = [ f((context or [])+action)[0] for action in actions]
```

### Comparing `coba-8.0.3/coba/environments/templates.py` & `coba-8.0.4/coba/environments/templates.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/evaluators/offline.py` & `coba-8.0.4/coba/evaluators/offline.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/evaluators/sequential.py` & `coba-8.0.4/coba/evaluators/sequential.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/exceptions.py` & `coba-8.0.4/coba/exceptions.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/experiments/core.py` & `coba-8.0.4/coba/experiments/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                 broken down into smaller chunks.
             seed: The seed that will determine all randomness within the experiment.
 
         Returns:
             Result of the experiment.
         """
 
-        self.config(processes,maxtasksperchunk,maxchunksperchild)
+        self.config(processes,maxchunksperchild,maxtasksperchunk)
         mp,mc,mt = self.processes,self.maxchunksperchild,self.maxtasksperchunk
 
         CobaContext.store['experiment_seed'] = seed
         is_multiproc = mp > 1 or mc != 0
 
         if is_multiproc: self._check_for_cloudpickle_dependency()
```

### Comparing `coba-8.0.3/coba/experiments/process.py` & `coba-8.0.4/coba/experiments/process.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/json.py` & `coba-8.0.4/coba/json.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/learners/__init__.py` & `coba-8.0.4/coba/learners/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/learners/bandit.py` & `coba-8.0.4/coba/learners/bandit.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/learners/corral.py` & `coba-8.0.4/coba/learners/corral.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/learners/lints.py` & `coba-8.0.4/coba/learners/lints.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/learners/linucb.py` & `coba-8.0.4/coba/learners/linucb.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/learners/misguided.py` & `coba-8.0.4/coba/learners/misguided.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/learners/utilities.py` & `coba-8.0.4/coba/learners/utilities.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/learners/vowpal.py` & `coba-8.0.4/coba/learners/vowpal.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/multiprocessing.py` & `coba-8.0.4/coba/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/pipes/__init__.py` & `coba-8.0.4/coba/pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/pipes/core.py` & `coba-8.0.4/coba/pipes/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Mapping, Union, Iterable, Callable, Any
+from typing import Mapping, Union, Iterable, Any
 
 from coba.exceptions import CobaException
 from coba.primitives import Filter, Source, Sink, Line
 
 from coba.pipes.sources import SourceFilters
 from coba.pipes.filters import FiltersFilter
 from coba.pipes.sinks   import FiltersSink
```

### Comparing `coba-8.0.3/coba/pipes/filters.py` & `coba-8.0.4/coba/pipes/filters.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/pipes/lines.py` & `coba-8.0.4/coba/pipes/lines.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/pipes/multiprocessing.py` & `coba-8.0.4/coba/pipes/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/pipes/readers.py` & `coba-8.0.4/coba/pipes/readers.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/pipes/rows.py` & `coba-8.0.4/coba/pipes/rows.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/pipes/sinks.py` & `coba-8.0.4/coba/pipes/sinks.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/pipes/sources.py` & `coba-8.0.4/coba/pipes/sources.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/primitives.py` & `coba-8.0.4/coba/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/random.py` & `coba-8.0.4/coba/random.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,43 +138,43 @@
         b=b+1
         if a == 0:
             return [floor(b*r) for r in islice(self._randu,n)]
         else:
             r_range = b-a
             return [floor(r_range*r) + a for r in islice(self._randu,n)]
 
-    def choice(self, seq: Sequence[Any], weights:Sequence[float] = None) -> Union[Any, Tuple[Any,float]]:
+    def choice(self, seq: Sequence[Any], weights:Sequence[float] = None) -> Any:
         """Choose a random item from the given sequence.
 
         Args:
             seq: The sequence to pick randomly from.
             weights: The frequency which seq is selected.
 
         Returns:
-            An item in seq.
+            A random item in seq.
         """
         if weights and len(weights) != len(seq):
             raise ValueError("The length of weights and sequence must be equal.")
 
         if weights is None:
             return seq[int(len(seq)*next(self._randu))]
         else:
             tot = sum(weights)
             if tot == 0: raise ValueError("The sum of weights cannot be zero.")
             return next(compress(seq, map((next(self._randu)*tot).__le__, accumulate(weights))))
 
-    def choicew(self, seq: Sequence[Any], weights:Sequence[float] = None) -> Union[Any, Tuple[Any,float]]:
+    def choicew(self, seq: Sequence[Any], weights:Sequence[float] = None) -> Tuple[Any,float]:
         """Choose a random item from the given sequence.
 
         Args:
             seq: The sequence to pick randomly from.
             weights: The frequency which seq is selected.
 
         Returns:
-            An random item with its weight.
+            A random item in seq with its weight.
         """
 
         if weights is None:
             return self.choice(seq),1/len(seq)
         else:
             i = self.choice(range(len(seq)),weights)
             return seq[i], weights[i]
```

### Comparing `coba-8.0.3/coba/register.py` & `coba-8.0.4/coba/register.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/registry.py` & `coba-8.0.4/coba/registry.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/results/core.py` & `coba-8.0.4/coba/results/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2599,2769 +2599,2770 @@
 0000a260: 696e 7465 7261 6374 696f 6e73 203d 206f  interactions = o
 0000a270: 6e6c 795f 6669 6e69 7368 6564 2e69 6e74  nly_finished.int
 0000a280: 6572 6163 7469 6f6e 730a 0a20 2020 2020  eractions..     
 0000a290: 2020 2066 756c 6c5f 6964 203d 205b 2765     full_id = ['e
 0000a2a0: 6e76 6972 6f6e 6d65 6e74 5f69 6427 2c27  nvironment_id','
 0000a2b0: 6c65 6172 6e65 725f 6964 272c 2765 7661  learner_id','eva
 0000a2c0: 6c75 6174 6f72 5f69 6427 5d0a 0a20 2020  luator_id']..   
-0000a2d0: 2020 2020 2067 726f 7570 7320 3d20 7365       groups = se
-0000a2e0: 6c66 2e5f 6772 6f75 7065 645f 7973 2870  lf._grouped_ys(p
-0000a2f0: 2c6c 2c66 756c 6c5f 6c2c 6675 6c6c 5f69  ,l,full_l,full_i
-0000a300: 642c 793d 792c 6675 6e63 3d27 6c69 7374  d,y=y,func='list
-0000a310: 272c 6361 7264 3d27 5327 290a 0a20 2020  ',card='S')..   
-0000a320: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0000a330: 2020 2020 2020 6772 6f75 7073 203d 2073        groups = s
-0000a340: 6f72 7465 6428 6772 6f75 7073 290a 2020  orted(groups).  
-0000a350: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-0000a360: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
-0000a370: 5f3d 4661 6c73 650a 2020 2020 2020 2020  _=False.        
-0000a380: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000a390: 2020 736f 7274 6564 5f3d 5472 7565 0a0a    sorted_=True..
-0000a3a0: 2020 2020 2020 2020 746f 5f6b 6565 702c          to_keep,
-0000a3b0: 2074 6f5f 6472 6f70 203d 205b 5d2c 205b   to_drop = [], [
-0000a3c0: 5d0a 2020 2020 2020 2020 666f 7220 5f2c  ].        for _,
-0000a3d0: 2067 726f 7570 2069 6e20 6772 6f75 7065   group in groupe
-0000a3e0: 7228 6772 6f75 7073 2c20 6b65 793d 6974  r(groups, key=it
-0000a3f0: 656d 6765 7474 6572 2830 292c 2073 6f72  emgetter(0), sor
-0000a400: 7465 645f 3d73 6f72 7465 645f 293a 0a20  ted_=sorted_):. 
-0000a410: 2020 2020 2020 2020 2020 2066 6f72 205f             for _
-0000a420: 2c20 6772 6f75 7020 696e 2067 726f 7570  , group in group
-0000a430: 6572 2867 726f 7570 2c20 6b65 793d 6974  er(group, key=it
-0000a440: 656d 6765 7474 6572 2831 292c 2073 6f72  emgetter(1), sor
-0000a450: 7465 645f 3d73 6f72 7465 645f 293a 0a20  ted_=sorted_):. 
-0000a460: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000a470: 6178 5f76 616c 2c20 6b2c 2064 203d 202d  ax_val, k, d = -
-0000a480: 666c 6f61 7428 2769 6e66 2729 2c20 5b5d  float('inf'), []
-0000a490: 2c20 5b5d 0a20 2020 2020 2020 2020 2020  , [].           
-0000a4a0: 2020 2020 2066 6f72 205f 2c20 6772 6f75       for _, grou
-0000a4b0: 7020 696e 2067 726f 7570 6572 2867 726f  p in grouper(gro
-0000a4c0: 7570 2c20 6b65 793d 6974 656d 6765 7474  up, key=itemgett
-0000a4d0: 6572 2832 292c 2073 6f72 7465 645f 3d73  er(2), sorted_=s
-0000a4e0: 6f72 7465 645f 293a 0a20 2020 2020 2020  orted_):.       
-0000a4f0: 2020 2020 2020 2020 2020 2020 2067 726f               gro
-0000a500: 7570 203d 206c 6973 7428 6772 6f75 7029  up = list(group)
-0000a510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a520: 2020 2020 2069 6473 2c76 616c 7320 3d20       ids,vals = 
-0000a530: 7a69 7028 2a28 2867 5b33 5d2c 206d 6561  zip(*((g[3], mea
-0000a540: 6e28 6973 6c69 6365 2867 5b2d 315d 2c6e  n(islice(g[-1],n
-0000a550: 2929 2920 666f 7220 6720 696e 2067 726f  ))) for g in gro
-0000a560: 7570 2929 0a20 2020 2020 2020 2020 2020  up)).           
-0000a570: 2020 2020 2020 2020 206d 6561 6e5f 7661           mean_va
-0000a580: 6c20 3d20 6d65 616e 2876 616c 7329 0a20  l = mean(vals). 
-0000a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5a0: 2020 2069 6620 6d65 616e 5f76 616c 203c     if mean_val <
-0000a5b0: 206d 6178 5f76 616c 3a0a 2020 2020 2020   max_val:.      
-0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5d0: 2020 642e 6578 7465 6e64 2869 6473 290a    d.extend(ids).
-0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a610: 2020 6d61 785f 7661 6c20 3d20 6d65 616e    max_val = mean
-0000a620: 5f76 616c 0a20 2020 2020 2020 2020 2020  _val.           
-0000a630: 2020 2020 2020 2020 2020 2020 2064 2e65               d.e
-0000a640: 7874 656e 6428 6b29 0a20 2020 2020 2020  xtend(k).       
-0000a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a660: 206b 203d 2069 6473 0a20 2020 2020 2020   k = ids.       
-0000a670: 2020 2020 2020 2020 2074 6f5f 6b65 6570           to_keep
-0000a680: 2e65 7874 656e 6428 6b29 0a20 2020 2020  .extend(k).     
-0000a690: 2020 2020 2020 2020 2020 2074 6f5f 6472             to_dr
-0000a6a0: 6f70 2e65 7874 656e 6428 6429 0a0a 2020  op.extend(d)..  
-0000a6b0: 2020 2020 2020 6966 2074 6f5f 6472 6f70        if to_drop
-0000a6c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000a6d0: 6c65 6374 203d 2073 656c 662e 5f72 656d  lect = self._rem
-0000a6e0: 6f76 6528 746f 5f64 726f 7029 0a20 2020  ove(to_drop).   
-0000a6f0: 2020 2020 2020 2020 2069 6e74 6572 6163           interac
-0000a700: 7469 6f6e 7320 3d20 5461 626c 6528 5669  tions = Table(Vi
-0000a710: 6577 2869 6e74 6572 6163 7469 6f6e 732e  ew(interactions.
-0000a720: 5f64 6174 612c 7365 6c65 6374 292c 2069  _data,select), i
-0000a730: 6e74 6572 6163 7469 6f6e 732e 636f 6c75  nteractions.colu
-0000a740: 6d6e 732c 2069 6e74 6572 6163 7469 6f6e  mns, interaction
-0000a750: 732e 696e 6465 7865 7329 0a0a 2020 2020  s.indexes)..    
-0000a760: 2020 2020 655f 6b65 6570 2c6c 5f6b 6565      e_keep,l_kee
-0000a770: 702c 765f 6b65 6570 203d 206d 6170 2873  p,v_keep = map(s
-0000a780: 6574 2c7a 6970 282a 746f 5f6b 6565 7029  et,zip(*to_keep)
-0000a790: 2920 6966 2074 6f5f 6b65 6570 2065 6c73  ) if to_keep els
-0000a7a0: 6520 285b 5d2c 5b5d 2c5b 5d29 0a20 2020  e ([],[],[]).   
-0000a7b0: 2020 2020 2069 6620 6c65 6e28 655f 6b65       if len(e_ke
-0000a7c0: 6570 2920 213d 206c 656e 2865 6e76 6972  ep) != len(envir
-0000a7d0: 6f6e 6d65 6e74 7329 3a20 656e 7669 726f  onments): enviro
-0000a7e0: 6e6d 656e 7473 203d 2065 6e76 6972 6f6e  nments = environ
-0000a7f0: 6d65 6e74 732e 7768 6572 6528 656e 7669  ments.where(envi
-0000a800: 726f 6e6d 656e 745f 6964 3d65 5f6b 6565  ronment_id=e_kee
-0000a810: 7029 0a20 2020 2020 2020 2069 6620 6c65  p).        if le
-0000a820: 6e28 6c5f 6b65 6570 2920 213d 206c 656e  n(l_keep) != len
-0000a830: 286c 6561 726e 6572 7329 2020 2020 3a20  (learners)    : 
-0000a840: 6c65 6172 6e65 7273 2020 2020 203d 206c  learners     = l
-0000a850: 6561 726e 6572 7320 2020 202e 7768 6572  earners    .wher
-0000a860: 6528 6c65 6172 6e65 725f 6964 2020 2020  e(learner_id    
-0000a870: 3d6c 5f6b 6565 7029 0a20 2020 2020 2020  =l_keep).       
-0000a880: 2069 6620 6c65 6e28 765f 6b65 6570 2920   if len(v_keep) 
-0000a890: 213d 206c 656e 2865 7661 6c75 6174 6f72  != len(evaluator
-0000a8a0: 7329 2020 3a20 6576 616c 7561 746f 7273  s)  : evaluators
-0000a8b0: 2020 203d 2065 7661 6c75 6174 6f72 7320     = evaluators 
-0000a8c0: 202e 7768 6572 6528 6576 616c 7561 746f   .where(evaluato
-0000a8d0: 725f 6964 2020 3d76 5f6b 6565 7029 0a0a  r_id  =v_keep)..
-0000a8e0: 2020 2020 2020 2020 7265 7475 726e 2052          return R
-0000a8f0: 6573 756c 7428 656e 7669 726f 6e6d 656e  esult(environmen
-0000a900: 7473 2c20 6c65 6172 6e65 7273 2c20 6576  ts, learners, ev
-0000a910: 616c 7561 746f 7273 2c20 696e 7465 7261  aluators, intera
-0000a920: 6374 696f 6e73 2c20 7365 6c66 2e65 7870  ctions, self.exp
-0000a930: 6572 696d 656e 7429 0a0a 2020 2020 6465  eriment)..    de
-0000a940: 6620 6669 6c74 6572 5f66 696e 2873 656c  f filter_fin(sel
-0000a950: 662c 0a20 2020 2020 2020 206e 3a20 556e  f,.        n: Un
-0000a960: 696f 6e5b 696e 742c 4c69 7465 7261 6c5b  ion[int,Literal[
-0000a970: 276d 696e 275d 5d20 3d20 4e6f 6e65 2c0a  'min']] = None,.
-0000a980: 2020 2020 2020 2020 6c3a 2055 6e69 6f6e          l: Union
-0000a990: 5b73 7472 2c20 5365 7175 656e 6365 5b73  [str, Sequence[s
-0000a9a0: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
-0000a9b0: 2020 2020 2070 3a20 556e 696f 6e5b 7374       p: Union[st
-0000a9c0: 722c 2053 6571 7565 6e63 655b 7374 725d  r, Sequence[str]
-0000a9d0: 5d20 3d20 4e6f 6e65 2920 2d3e 2027 5265  ] = None) -> 'Re
-0000a9e0: 7375 6c74 273a 0a20 2020 2020 2020 2022  sult':.        "
-0000a9f0: 2222 4669 6c74 6572 2074 6865 2072 6573  ""Filter the res
-0000aa00: 756c 7473 2064 6f77 6e20 746f 2065 7665  ults down to eve
-0000aa10: 6e20 6f75 7463 6f6d 6573 2073 6f20 7468  n outcomes so th
-0000aa20: 6174 2070 6c6f 7474 6564 2072 6573 756c  at plotted resul
-0000aa30: 7473 2077 696c 6c20 6265 206d 6561 6e69  ts will be meani
-0000aa40: 6e67 6675 6c2e 0a0a 2020 2020 2020 2020  ngful...        
-0000aa50: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0000aa60: 2020 6e3a 2054 6865 206e 756d 6265 7220    n: The number 
-0000aa70: 6f66 2069 6e74 6572 6163 7469 6f6e 7320  of interactions 
-0000aa80: 6120 7370 6563 6966 6963 2065 7661 6c75  a specific evalu
-0000aa90: 6174 696f 6e20 6d75 7374 2068 6176 6520  ation must have 
-0000aaa0: 284e 6f6e 6520 696e 6469 6361 7465 7320  (None indicates 
-0000aab0: 6e6f 2063 6f6e 7374 7261 696e 7429 2e0a  no constraint)..
-0000aac0: 2020 2020 2020 2020 2020 2020 6c3a 2054              l: T
-0000aad0: 6865 206c 6576 656c 2061 7420 7768 6963  he level at whic
-0000aae0: 6820 7765 2077 6973 6820 746f 2063 6f6d  h we wish to com
-0000aaf0: 7061 7265 2065 7661 6c61 7469 6f6e 206f  pare evalation o
-0000ab00: 7574 636f 6d65 732e 0a20 2020 2020 2020  utcomes..       
-0000ab10: 2020 2020 2070 3a20 5468 6520 7061 6972       p: The pair
-0000ab20: 7320 7468 6174 206d 7573 7420 6578 6973  s that must exis
-0000ab30: 7420 6163 726f 7373 2061 6c6c 2063 6f6d  t across all com
-0000ab40: 7061 7269 736f 6e20 6c65 7665 6c73 2069  parison levels i
-0000ab50: 6e20 6f72 6465 7220 746f 2062 6520 696e  n order to be in
-0000ab60: 636c 7564 6564 2e0a 2020 2020 2020 2020  cluded..        
-0000ab70: 2222 220a 0a20 2020 2020 2020 2072 6573  """..        res
-0000ab80: 756c 7420 3d20 7365 6c66 2e5f 6669 6c74  ult = self._filt
-0000ab90: 6572 5f66 696e 286e 2c6c 2c70 290a 0a20  er_fin(n,l,p).. 
-0000aba0: 2020 2020 2020 2069 6620 6c65 6e28 7265         if len(re
-0000abb0: 7375 6c74 2e69 6e74 6572 6163 7469 6f6e  sult.interaction
-0000abc0: 7329 203d 3d20 303a 0a20 2020 2020 2020  s) == 0:.       
-0000abd0: 2020 2020 2043 6f62 6143 6f6e 7465 7874       CobaContext
-0000abe0: 2e6c 6f67 6765 722e 6c6f 6728 6622 5468  .logger.log(f"Th
-0000abf0: 6572 6520 7761 7320 6e6f 207b 707d 2077  ere was no {p} w
-0000ac00: 6869 6368 2077 6173 2066 696e 6973 6865  hich was finishe
-0000ac10: 6420 666f 7220 6576 6572 7920 7b6c 7d2e  d for every {l}.
-0000ac20: 2229 0a0a 2020 2020 2020 2020 7265 7475  ")..        retu
-0000ac30: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0000ac40: 6566 2066 696c 7465 725f 656e 7628 7365  ef filter_env(se
-0000ac50: 6c66 2c20 7072 6564 3a43 616c 6c61 626c  lf, pred:Callabl
-0000ac60: 655b 5b4d 6170 7069 6e67 5b73 7472 2c41  e[[Mapping[str,A
-0000ac70: 6e79 5d5d 2c62 6f6f 6c5d 203d 204e 6f6e  ny]],bool] = Non
-0000ac80: 652c 202a 2a6b 7761 7267 733a 2041 6e79  e, **kwargs: Any
-0000ac90: 2920 2d3e 2027 5265 7375 6c74 273a 0a20  ) -> 'Result':. 
-0000aca0: 2020 2020 2020 2022 2222 4669 6c74 6572         """Filter
-0000acb0: 2074 6865 2072 6573 756c 7420 746f 206f   the result to o
-0000acc0: 6e6c 7920 636f 6e74 6169 6e20 6461 7461  nly contain data
-0000acd0: 2061 626f 7574 2073 7065 6369 6669 6320   about specific 
-0000ace0: 656e 7669 726f 6e6d 656e 7473 2e0a 0a20  environments... 
-0000acf0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0000ad00: 2020 2020 2020 2020 2070 7265 643a 2041           pred: A
-0000ad10: 2070 7265 6469 6361 7465 2074 6861 7420   predicate that 
-0000ad20: 7265 7475 726e 7320 7472 7565 2066 6f72  returns true for
-0000ad30: 206c 6561 726e 6572 2064 6963 7469 6f6e   learner diction
-0000ad40: 6172 6965 7320 7468 6174 2073 686f 756c  aries that shoul
-0000ad50: 6420 6265 206b 6570 742e 0a20 2020 2020  d be kept..     
-0000ad60: 2020 2020 2020 202a 2a6b 7761 7267 733a         **kwargs:
-0000ad70: 206b 6579 2d76 616c 7565 2070 6169 7273   key-value pairs
-0000ad80: 2074 6f20 6669 6c74 6572 206f 6e2e 2054   to filter on. T
-0000ad90: 6f20 7365 6520 6669 6c74 6572 696e 6720  o see filtering 
-0000ada0: 6f70 7469 6f6e 7320 7365 6520 5461 626c  options see Tabl
-0000adb0: 652e 6669 6c74 6572 2e0a 2020 2020 2020  e.filter..      
-0000adc0: 2020 2222 220a 0a20 2020 2020 2020 2069    """..        i
-0000add0: 6620 6c65 6e28 7365 6c66 2e65 6e76 6972  f len(self.envir
-0000ade0: 6f6e 6d65 6e74 7329 203d 3d20 303a 2072  onments) == 0: r
-0000adf0: 6574 7572 6e20 7365 6c66 0a0a 2020 2020  eturn self..    
-0000ae00: 2020 2020 656e 7669 726f 6e6d 656e 7473      environments
-0000ae10: 203d 2073 656c 662e 656e 7669 726f 6e6d   = self.environm
-0000ae20: 656e 7473 2e77 6865 7265 2870 7265 642c  ents.where(pred,
-0000ae30: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
-0000ae40: 2020 206c 6561 726e 6572 7320 2020 2020     learners     
-0000ae50: 3d20 7365 6c66 2e6c 6561 726e 6572 730a  = self.learners.
-0000ae60: 2020 2020 2020 2020 6576 616c 7561 746f          evaluato
-0000ae70: 7273 2020 203d 2073 656c 662e 6576 616c  rs   = self.eval
-0000ae80: 7561 746f 7273 0a20 2020 2020 2020 2069  uators.        i
-0000ae90: 6e74 6572 6163 7469 6f6e 7320 3d20 7365  nteractions = se
-0000aea0: 6c66 2e69 6e74 6572 6163 7469 6f6e 730a  lf.interactions.
-0000aeb0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0000aec0: 656e 7669 726f 6e6d 656e 7473 2920 3d3d  environments) ==
-0000aed0: 206c 656e 2873 656c 662e 656e 7669 726f   len(self.enviro
-0000aee0: 6e6d 656e 7473 293a 0a20 2020 2020 2020  nments):.       
-0000aef0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000af00: 0a0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
-0000af10: 2865 6e76 6972 6f6e 6d65 6e74 7329 203d  (environments) =
-0000af20: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-0000af30: 2043 6f62 6143 6f6e 7465 7874 2e6c 6f67   CobaContext.log
-0000af40: 6765 722e 6c6f 6728 6622 4e6f 2065 6e76  ger.log(f"No env
-0000af50: 6972 6f6e 6d65 6e74 7320 6d61 7463 6865  ironments matche
-0000af60: 6420 7468 6520 6769 7665 6e20 6669 6c74  d the given filt
-0000af70: 6572 2e22 290a 0a20 2020 2020 2020 2069  er.")..        i
-0000af80: 6e74 6572 6163 7469 6f6e 7320 3d20 696e  nteractions = in
-0000af90: 7465 7261 6374 696f 6e73 2e77 6865 7265  teractions.where
-0000afa0: 2865 6e76 6972 6f6e 6d65 6e74 5f69 643d  (environment_id=
-0000afb0: 7365 7428 656e 7669 726f 6e6d 656e 7473  set(environments
-0000afc0: 5b22 656e 7669 726f 6e6d 656e 745f 6964  ["environment_id
-0000afd0: 225d 2929 0a20 2020 2020 2020 206c 6561  "])).        lea
-0000afe0: 726e 6572 7320 2020 2020 3d20 6c65 6172  rners     = lear
-0000aff0: 6e65 7273 2020 2020 2e77 6865 7265 286c  ners    .where(l
-0000b000: 6561 726e 6572 5f69 6420 2020 203d 7365  earner_id    =se
-0000b010: 7428 696e 7465 7261 6374 696f 6e73 5b22  t(interactions["
-0000b020: 6c65 6172 6e65 725f 6964 225d 2929 0a20  learner_id"])). 
-0000b030: 2020 2020 2020 2065 7661 6c75 6174 6f72         evaluator
-0000b040: 7320 2020 3d20 6576 616c 7561 746f 7273  s   = evaluators
-0000b050: 2020 2e77 6865 7265 2865 7661 6c75 6174    .where(evaluat
-0000b060: 6f72 5f69 6420 203d 7365 7428 696e 7465  or_id  =set(inte
-0000b070: 7261 6374 696f 6e73 5b22 6576 616c 7561  ractions["evalua
-0000b080: 746f 725f 6964 225d 2929 0a0a 2020 2020  tor_id"]))..    
-0000b090: 2020 2020 7265 7475 726e 2052 6573 756c      return Resul
-0000b0a0: 7428 656e 7669 726f 6e6d 656e 7473 2c6c  t(environments,l
-0000b0b0: 6561 726e 6572 732c 6576 616c 7561 746f  earners,evaluato
-0000b0c0: 7273 2c69 6e74 6572 6163 7469 6f6e 732c  rs,interactions,
-0000b0d0: 7365 6c66 2e65 7870 6572 696d 656e 7429  self.experiment)
-0000b0e0: 0a0a 2020 2020 6465 6620 6669 6c74 6572  ..    def filter
-0000b0f0: 5f6c 726e 2873 656c 662c 2070 7265 643a  _lrn(self, pred:
-0000b100: 4361 6c6c 6162 6c65 5b5b 4d61 7070 696e  Callable[[Mappin
-0000b110: 675b 7374 722c 416e 795d 5d2c 626f 6f6c  g[str,Any]],bool
-0000b120: 5d20 3d20 4e6f 6e65 2c20 2a2a 6b77 6172  ] = None, **kwar
-0000b130: 6773 3a20 416e 7929 202d 3e20 2752 6573  gs: Any) -> 'Res
-0000b140: 756c 7427 3a0a 2020 2020 2020 2020 2222  ult':.        ""
-0000b150: 2246 696c 7465 7220 7468 6520 7265 7375  "Filter the resu
-0000b160: 6c74 2074 6f20 6f6e 6c79 2063 6f6e 7461  lt to only conta
-0000b170: 696e 2064 6174 6120 6162 6f75 7420 7370  in data about sp
-0000b180: 6563 6966 6963 206c 6561 726e 6572 732e  ecific learners.
-0000b190: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-0000b1a0: 2020 2020 2020 2020 2020 2020 7072 6564              pred
-0000b1b0: 3a20 4120 7072 6564 6963 6174 6520 7468  : A predicate th
-0000b1c0: 6174 2072 6574 7572 6e73 2074 7275 6520  at returns true 
-0000b1d0: 666f 7220 6c65 6172 6e65 7220 6469 6374  for learner dict
-0000b1e0: 696f 6e61 7269 6573 2074 6861 7420 7368  ionaries that sh
-0000b1f0: 6f75 6c64 2062 6520 6b65 7074 2e0a 2020  ould be kept..  
-0000b200: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-0000b210: 6773 3a20 6b65 792d 7661 6c75 6520 7061  gs: key-value pa
-0000b220: 6972 7320 746f 2066 696c 7465 7220 6f6e  irs to filter on
-0000b230: 2e20 546f 2073 6565 2066 696c 7465 7269  . To see filteri
-0000b240: 6e67 206f 7074 696f 6e73 2073 6565 2054  ng options see T
-0000b250: 6162 6c65 2e66 696c 7465 722e 0a20 2020  able.filter..   
-0000b260: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000b270: 2069 6620 6c65 6e28 7365 6c66 2e6c 6561   if len(self.lea
-0000b280: 726e 6572 7329 203d 3d20 303a 2072 6574  rners) == 0: ret
-0000b290: 7572 6e20 7365 6c66 0a0a 2020 2020 2020  urn self..      
-0000b2a0: 2020 656e 7669 726f 6e6d 656e 7473 203d    environments =
-0000b2b0: 2073 656c 662e 656e 7669 726f 6e6d 656e   self.environmen
-0000b2c0: 7473 0a20 2020 2020 2020 206c 6561 726e  ts.        learn
-0000b2d0: 6572 7320 2020 2020 3d20 7365 6c66 2e6c  ers     = self.l
-0000b2e0: 6561 726e 6572 732e 7768 6572 6528 7072  earners.where(pr
-0000b2f0: 6564 2c20 2a2a 6b77 6172 6773 290a 2020  ed, **kwargs).  
-0000b300: 2020 2020 2020 6576 616c 7561 746f 7273        evaluators
-0000b310: 2020 203d 2073 656c 662e 6576 616c 7561     = self.evalua
-0000b320: 746f 7273 0a20 2020 2020 2020 2069 6e74  tors.        int
-0000b330: 6572 6163 7469 6f6e 7320 3d20 7365 6c66  eractions = self
-0000b340: 2e69 6e74 6572 6163 7469 6f6e 730a 0a20  .interactions.. 
-0000b350: 2020 2020 2020 2069 6620 6c65 6e28 6c65         if len(le
-0000b360: 6172 6e65 7273 2920 3d3d 206c 656e 2873  arners) == len(s
-0000b370: 656c 662e 6c65 6172 6e65 7273 293a 0a20  elf.learners):. 
-0000b380: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000b390: 6e20 7365 6c66 0a0a 2020 2020 2020 2020  n self..        
-0000b3a0: 6966 206c 656e 286c 6561 726e 6572 7329  if len(learners)
-0000b3b0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-0000b3c0: 2020 2043 6f62 6143 6f6e 7465 7874 2e6c     CobaContext.l
-0000b3d0: 6f67 6765 722e 6c6f 6728 6622 4e6f 206c  ogger.log(f"No l
-0000b3e0: 6561 726e 6572 7320 6d61 7463 6865 6420  earners matched 
-0000b3f0: 7468 6520 6769 7665 6e20 6669 6c74 6572  the given filter
-0000b400: 2e22 290a 0a20 2020 2020 2020 2069 6e74  .")..        int
-0000b410: 6572 6163 7469 6f6e 7320 3d20 696e 7465  eractions = inte
-0000b420: 7261 6374 696f 6e73 2e77 6865 7265 286c  ractions.where(l
-0000b430: 6561 726e 6572 5f69 6420 2020 203d 7365  earner_id    =se
-0000b440: 7428 6c65 6172 6e65 7273 5b22 6c65 6172  t(learners["lear
-0000b450: 6e65 725f 6964 225d 2929 0a20 2020 2020  ner_id"])).     
-0000b460: 2020 2065 6e76 6972 6f6e 6d65 6e74 7320     environments 
-0000b470: 3d20 656e 7669 726f 6e6d 656e 7473 2e77  = environments.w
-0000b480: 6865 7265 2865 6e76 6972 6f6e 6d65 6e74  here(environment
-0000b490: 5f69 643d 7365 7428 696e 7465 7261 6374  _id=set(interact
-0000b4a0: 696f 6e73 5b22 656e 7669 726f 6e6d 656e  ions["environmen
-0000b4b0: 745f 6964 225d 2929 0a20 2020 2020 2020  t_id"])).       
-0000b4c0: 2065 7661 6c75 6174 6f72 7320 2020 3d20   evaluators   = 
-0000b4d0: 6576 616c 7561 746f 7273 2020 2e77 6865  evaluators  .whe
-0000b4e0: 7265 2865 7661 6c75 6174 6f72 5f69 6420  re(evaluator_id 
-0000b4f0: 203d 7365 7428 696e 7465 7261 6374 696f   =set(interactio
-0000b500: 6e73 5b22 6576 616c 7561 746f 725f 6964  ns["evaluator_id
-0000b510: 225d 2929 0a0a 2020 2020 2020 2020 7265  "]))..        re
-0000b520: 7475 726e 2052 6573 756c 7428 656e 7669  turn Result(envi
-0000b530: 726f 6e6d 656e 7473 2c6c 6561 726e 6572  ronments,learner
-0000b540: 732c 6576 616c 7561 746f 7273 2c69 6e74  s,evaluators,int
-0000b550: 6572 6163 7469 6f6e 7329 0a0a 2020 2020  eractions)..    
-0000b560: 6465 6620 6669 6c74 6572 5f76 616c 2873  def filter_val(s
-0000b570: 656c 662c 2070 7265 643a 4361 6c6c 6162  elf, pred:Callab
-0000b580: 6c65 5b5b 4d61 7070 696e 675b 7374 722c  le[[Mapping[str,
-0000b590: 416e 795d 5d2c 626f 6f6c 5d20 3d20 4e6f  Any]],bool] = No
-0000b5a0: 6e65 2c20 2a2a 6b77 6172 6773 3a20 416e  ne, **kwargs: An
-0000b5b0: 7929 202d 3e20 2752 6573 756c 7427 3a0a  y) -> 'Result':.
-0000b5c0: 2020 2020 2020 2020 2222 2246 696c 7465          """Filte
-0000b5d0: 7220 7468 6520 7265 7375 6c74 2074 6f20  r the result to 
-0000b5e0: 6f6e 6c79 2063 6f6e 7461 696e 2064 6174  only contain dat
-0000b5f0: 6120 6162 6f75 7420 7370 6563 6966 6963  a about specific
-0000b600: 2065 7661 6c75 6174 6f72 732e 0a0a 2020   evaluators...  
-0000b610: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-0000b620: 2020 2020 2020 2020 7072 6564 3a20 4120          pred: A 
-0000b630: 7072 6564 6963 6174 6520 7468 6174 2072  predicate that r
-0000b640: 6574 7572 6e73 2074 7275 6520 666f 7220  eturns true for 
-0000b650: 6c65 6172 6e65 7220 6469 6374 696f 6e61  learner dictiona
-0000b660: 7269 6573 2074 6861 7420 7368 6f75 6c64  ries that should
-0000b670: 2062 6520 6b65 7074 2e0a 2020 2020 2020   be kept..      
-0000b680: 2020 2020 2020 2a2a 6b77 6172 6773 3a20        **kwargs: 
-0000b690: 6b65 792d 7661 6c75 6520 7061 6972 7320  key-value pairs 
-0000b6a0: 746f 2066 696c 7465 7220 6f6e 2e20 546f  to filter on. To
-0000b6b0: 2073 6565 2066 696c 7465 7269 6e67 206f   see filtering o
-0000b6c0: 7074 696f 6e73 2073 6565 2054 6162 6c65  ptions see Table
-0000b6d0: 2e66 696c 7465 722e 0a20 2020 2020 2020  .filter..       
-0000b6e0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-0000b6f0: 6c65 6e28 7365 6c66 2e6c 6561 726e 6572  len(self.learner
-0000b700: 7329 203d 3d20 303a 2072 6574 7572 6e20  s) == 0: return 
-0000b710: 7365 6c66 0a0a 2020 2020 2020 2020 656e  self..        en
-0000b720: 7669 726f 6e6d 656e 7473 203d 2073 656c  vironments = sel
-0000b730: 662e 656e 7669 726f 6e6d 656e 7473 0a20  f.environments. 
-0000b740: 2020 2020 2020 206c 6561 726e 6572 7320         learners 
-0000b750: 2020 2020 3d20 7365 6c66 2e6c 6561 726e      = self.learn
-0000b760: 6572 730a 2020 2020 2020 2020 6576 616c  ers.        eval
-0000b770: 7561 746f 7273 2020 203d 2073 656c 662e  uators   = self.
-0000b780: 6576 616c 7561 746f 7273 2e77 6865 7265  evaluators.where
-0000b790: 2870 7265 642c 202a 2a6b 7761 7267 7329  (pred, **kwargs)
-0000b7a0: 0a20 2020 2020 2020 2069 6e74 6572 6163  .        interac
-0000b7b0: 7469 6f6e 7320 3d20 7365 6c66 2e69 6e74  tions = self.int
-0000b7c0: 6572 6163 7469 6f6e 730a 0a20 2020 2020  eractions..     
-0000b7d0: 2020 2069 6620 6c65 6e28 6576 616c 7561     if len(evalua
-0000b7e0: 746f 7273 2920 3d3d 206c 656e 2873 656c  tors) == len(sel
-0000b7f0: 662e 6576 616c 7561 746f 7273 293a 0a20  f.evaluators):. 
-0000b800: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000b810: 6e20 7365 6c66 0a0a 2020 2020 2020 2020  n self..        
-0000b820: 6966 206c 656e 2865 7661 6c75 6174 6f72  if len(evaluator
-0000b830: 7329 203d 3d20 303a 0a20 2020 2020 2020  s) == 0:.       
-0000b840: 2020 2020 2043 6f62 6143 6f6e 7465 7874       CobaContext
-0000b850: 2e6c 6f67 6765 722e 6c6f 6728 6622 4e6f  .logger.log(f"No
-0000b860: 2065 7661 6c75 6174 6f72 7320 6d61 7463   evaluators matc
-0000b870: 6865 6420 7468 6520 6769 7665 6e20 6669  hed the given fi
-0000b880: 6c74 6572 2e22 290a 0a20 2020 2020 2020  lter.")..       
-0000b890: 2069 6e74 6572 6163 7469 6f6e 7320 3d20   interactions = 
-0000b8a0: 696e 7465 7261 6374 696f 6e73 2e77 6865  interactions.whe
-0000b8b0: 7265 2865 7661 6c75 6174 6f72 5f69 6420  re(evaluator_id 
-0000b8c0: 203d 7365 7428 6576 616c 7561 746f 7273   =set(evaluators
-0000b8d0: 5b27 6576 616c 7561 746f 725f 6964 275d  ['evaluator_id']
-0000b8e0: 2929 0a20 2020 2020 2020 2065 6e76 6972  )).        envir
-0000b8f0: 6f6e 6d65 6e74 7320 3d20 656e 7669 726f  onments = enviro
-0000b900: 6e6d 656e 7473 2e77 6865 7265 2865 6e76  nments.where(env
-0000b910: 6972 6f6e 6d65 6e74 5f69 643d 7365 7428  ironment_id=set(
-0000b920: 696e 7465 7261 6374 696f 6e73 5b22 656e  interactions["en
-0000b930: 7669 726f 6e6d 656e 745f 6964 225d 2929  vironment_id"]))
-0000b940: 0a20 2020 2020 2020 206c 6561 726e 6572  .        learner
-0000b950: 7320 2020 2020 3d20 6c65 6172 6e65 7273  s     = learners
-0000b960: 2020 2020 2e77 6865 7265 286c 6561 726e      .where(learn
-0000b970: 6572 5f69 6420 2020 203d 7365 7428 696e  er_id    =set(in
-0000b980: 7465 7261 6374 696f 6e73 5b22 6c65 6172  teractions["lear
-0000b990: 6e65 725f 6964 225d 2929 0a0a 2020 2020  ner_id"]))..    
-0000b9a0: 2020 2020 7265 7475 726e 2052 6573 756c      return Resul
-0000b9b0: 7428 656e 7669 726f 6e6d 656e 7473 2c6c  t(environments,l
-0000b9c0: 6561 726e 6572 732c 6576 616c 7561 746f  earners,evaluato
-0000b9d0: 7273 2c69 6e74 6572 6163 7469 6f6e 7329  rs,interactions)
-0000b9e0: 0a0a 2020 2020 6465 6620 6669 6c74 6572  ..    def filter
-0000b9f0: 5f69 6e74 2873 656c 662c 2070 7265 643a  _int(self, pred:
-0000ba00: 4361 6c6c 6162 6c65 5b5b 4d61 7070 696e  Callable[[Mappin
-0000ba10: 675b 7374 722c 416e 795d 5d2c 626f 6f6c  g[str,Any]],bool
-0000ba20: 5d20 3d20 4e6f 6e65 2c20 2a2a 6b77 6172  ] = None, **kwar
-0000ba30: 6773 3a20 416e 7929 202d 3e20 2752 6573  gs: Any) -> 'Res
-0000ba40: 756c 7427 3a0a 2020 2020 2020 2020 2222  ult':.        ""
-0000ba50: 2246 696c 7465 7220 7468 6520 7265 7375  "Filter the resu
-0000ba60: 6c74 2074 6f20 6f6e 6c79 2063 6f6e 7461  lt to only conta
-0000ba70: 696e 2064 6174 6120 6162 6f75 7420 7370  in data about sp
-0000ba80: 6563 6966 6963 2069 6e74 6572 6163 7469  ecific interacti
-0000ba90: 6f6e 732e 0a0a 2020 2020 2020 2020 4172  ons...        Ar
-0000baa0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000bab0: 7072 6564 3a20 4120 7072 6564 6963 6174  pred: A predicat
-0000bac0: 6520 7468 6174 2072 6574 7572 6e73 2074  e that returns t
-0000bad0: 7275 6520 666f 7220 6c65 6172 6e65 7220  rue for learner 
-0000bae0: 6469 6374 696f 6e61 7269 6573 2074 6861  dictionaries tha
-0000baf0: 7420 7368 6f75 6c64 2062 6520 6b65 7074  t should be kept
-0000bb00: 2e0a 2020 2020 2020 2020 2020 2020 2a2a  ..            **
-0000bb10: 6b77 6172 6773 3a20 6b65 792d 7661 6c75  kwargs: key-valu
-0000bb20: 6520 7061 6972 7320 746f 2066 696c 7465  e pairs to filte
-0000bb30: 7220 6f6e 2e20 546f 2073 6565 2066 696c  r on. To see fil
-0000bb40: 7465 7269 6e67 206f 7074 696f 6e73 2073  tering options s
-0000bb50: 6565 2054 6162 6c65 2e66 696c 7465 722e  ee Table.filter.
-0000bb60: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000bb70: 2020 2020 2069 6620 6c65 6e28 7365 6c66       if len(self
-0000bb80: 2e6c 6561 726e 6572 7329 203d 3d20 303a  .learners) == 0:
-0000bb90: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
-0000bba0: 2020 2020 2020 656e 7669 726f 6e6d 656e        environmen
-0000bbb0: 7473 203d 2073 656c 662e 656e 7669 726f  ts = self.enviro
-0000bbc0: 6e6d 656e 7473 0a20 2020 2020 2020 206c  nments.        l
-0000bbd0: 6561 726e 6572 7320 2020 2020 3d20 7365  earners     = se
-0000bbe0: 6c66 2e6c 6561 726e 6572 730a 2020 2020  lf.learners.    
-0000bbf0: 2020 2020 6576 616c 7561 746f 7273 2020      evaluators  
-0000bc00: 203d 2073 656c 662e 6576 616c 7561 746f   = self.evaluato
-0000bc10: 7273 0a20 2020 2020 2020 2069 6e74 6572  rs.        inter
-0000bc20: 6163 7469 6f6e 7320 3d20 7365 6c66 2e69  actions = self.i
-0000bc30: 6e74 6572 6163 7469 6f6e 732e 7768 6572  nteractions.wher
-0000bc40: 6528 7072 6564 2c20 2a2a 6b77 6172 6773  e(pred, **kwargs
-0000bc50: 290a 0a20 2020 2020 2020 2069 6620 6c65  )..        if le
-0000bc60: 6e28 696e 7465 7261 6374 696f 6e73 2920  n(interactions) 
-0000bc70: 3d3d 206c 656e 2873 656c 662e 696e 7465  == len(self.inte
-0000bc80: 7261 6374 696f 6e73 293a 0a20 2020 2020  ractions):.     
-0000bc90: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000bca0: 6c66 0a0a 2020 2020 2020 2020 6966 206c  lf..        if l
-0000bcb0: 656e 2869 6e74 6572 6163 7469 6f6e 7329  en(interactions)
-0000bcc0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-0000bcd0: 2020 2043 6f62 6143 6f6e 7465 7874 2e6c     CobaContext.l
-0000bce0: 6f67 6765 722e 6c6f 6728 6622 4e6f 2069  ogger.log(f"No i
-0000bcf0: 6e74 6572 6163 7469 6f6e 7320 6d61 7463  nteractions matc
-0000bd00: 6865 6420 7468 6520 6769 7665 6e20 6669  hed the given fi
-0000bd10: 6c74 6572 2e22 290a 0a20 2020 2020 2020  lter.")..       
-0000bd20: 2074 6f5f 6b65 6570 203d 206c 6973 7428   to_keep = list(
-0000bd30: 696e 7465 7261 6374 696f 6e73 2e67 726f  interactions.gro
-0000bd40: 7570 6279 2833 2c73 656c 6563 743d 4e6f  upby(3,select=No
-0000bd50: 6e65 2929 0a20 2020 2020 2020 2065 6e76  ne)).        env
-0000bd60: 2c6c 726e 2c76 616c 203d 207a 6970 282a  ,lrn,val = zip(*
-0000bd70: 746f 5f6b 6565 7029 2069 6620 746f 5f6b  to_keep) if to_k
-0000bd80: 6565 7020 656c 7365 2028 5b5d 2c5b 5d2c  eep else ([],[],
-0000bd90: 5b5d 290a 0a20 2020 2020 2020 2069 6620  [])..        if 
-0000bda0: 6c65 6e28 656e 7629 2021 3d20 6c65 6e28  len(env) != len(
-0000bdb0: 656e 7669 726f 6e6d 656e 7473 293a 2065  environments): e
-0000bdc0: 6e76 6972 6f6e 6d65 6e74 7320 3d20 656e  nvironments = en
-0000bdd0: 7669 726f 6e6d 656e 7473 2e77 6865 7265  vironments.where
-0000bde0: 2865 6e76 6972 6f6e 6d65 6e74 5f69 643d  (environment_id=
-0000bdf0: 7365 7428 656e 7629 290a 2020 2020 2020  set(env)).      
-0000be00: 2020 6966 206c 656e 286c 726e 2920 213d    if len(lrn) !=
-0000be10: 206c 656e 286c 6561 726e 6572 7329 2020   len(learners)  
-0000be20: 2020 3a20 6c65 6172 6e65 7273 2020 2020    : learners    
-0000be30: 203d 206c 6561 726e 6572 7320 2020 202e   = learners    .
-0000be40: 7768 6572 6528 6c65 6172 6e65 725f 6964  where(learner_id
-0000be50: 2020 2020 3d73 6574 286c 726e 2929 0a20      =set(lrn)). 
-0000be60: 2020 2020 2020 2069 6620 6c65 6e28 7661         if len(va
-0000be70: 6c29 2021 3d20 6c65 6e28 6576 616c 7561  l) != len(evalua
-0000be80: 746f 7273 2920 203a 2065 7661 6c75 6174  tors)  : evaluat
-0000be90: 6f72 7320 2020 3d20 6576 616c 7561 746f  ors   = evaluato
-0000bea0: 7273 2020 2e77 6865 7265 2865 7661 6c75  rs  .where(evalu
-0000beb0: 6174 6f72 5f69 6420 203d 7365 7428 7661  ator_id  =set(va
-0000bec0: 6c29 290a 0a20 2020 2020 2020 2072 6574  l))..        ret
-0000bed0: 7572 6e20 5265 7375 6c74 2865 6e76 6972  urn Result(envir
-0000bee0: 6f6e 6d65 6e74 732c 6c65 6172 6e65 7273  onments,learners
-0000bef0: 2c65 7661 6c75 6174 6f72 732c 696e 7465  ,evaluators,inte
-0000bf00: 7261 6374 696f 6e73 290a 0a20 2020 2064  ractions)..    d
-0000bf10: 6566 2077 6865 7265 5f62 6573 7428 7365  ef where_best(se
-0000bf20: 6c66 2c0a 2020 2020 2020 2020 6c3a 556e  lf,.        l:Un
-0000bf30: 696f 6e5b 7374 722c 2053 6571 7565 6e63  ion[str, Sequenc
-0000bf40: 655b 7374 725d 5d2c 0a20 2020 2020 2020  e[str]],.       
-0000bf50: 2070 3a55 6e69 6f6e 5b73 7472 2c20 5365   p:Union[str, Se
-0000bf60: 7175 656e 6365 5b73 7472 5d5d 203d 2027  quence[str]] = '
-0000bf70: 656e 7669 726f 6e6d 656e 745f 6964 272c  environment_id',
-0000bf80: 0a20 2020 2020 2020 2079 3a73 7472 203d  .        y:str =
-0000bf90: 2027 7265 7761 7264 272c 0a20 2020 2020   'reward',.     
-0000bfa0: 2020 206e 3a69 6e74 203d 204e 6f6e 652c     n:int = None,
-0000bfb0: 0a20 2020 2020 2020 2066 756c 6c5f 6c3a  .        full_l:
-0000bfc0: 556e 696f 6e5b 7374 722c 2053 6571 7565  Union[str, Seque
-0000bfd0: 6e63 655b 7374 725d 5d3d 276c 6561 726e  nce[str]]='learn
-0000bfe0: 6572 5f69 6427 2c0a 2020 2020 2020 2020  er_id',.        
-0000bff0: 6675 6c6c 5f70 3a55 6e69 6f6e 5b73 7472  full_p:Union[str
-0000c000: 2c20 5365 7175 656e 6365 5b73 7472 5d5d  , Sequence[str]]
-0000c010: 3d27 656e 7669 726f 6e6d 656e 745f 6964  ='environment_id
-0000c020: 2729 202d 3e20 2752 6573 756c 7427 3a0a  ') -> 'Result':.
-0000c030: 2020 2020 2020 2020 2222 2253 656c 6563          """Selec
-0000c040: 7420 7468 6520 6265 7374 2070 6572 666f  t the best perfo
-0000c050: 726d 696e 6720 606c 6020 6f76 6572 2060  rming `l` over `
-0000c060: 7060 2e0a 0a20 2020 2020 2020 2041 7267  p`...        Arg
-0000c070: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
-0000c080: 3a20 5468 6520 6879 7065 7270 6172 616d  : The hyperparam
-0000c090: 6574 6572 2076 616c 7565 7320 7765 2077  eter values we w
-0000c0a0: 6973 6820 746f 206f 7074 696d 697a 652e  ish to optimize.
-0000c0b0: 0a20 2020 2020 2020 2020 2020 2070 3a20  .            p: 
-0000c0c0: 5468 6520 6772 6f75 7069 6e67 2076 6172  The grouping var
-0000c0d0: 6961 626c 6520 7765 2077 6973 6820 746f  iable we wish to
-0000c0e0: 206f 7074 696d 697a 6520 6f76 6572 2e0a   optimize over..
-0000c0f0: 2020 2020 2020 2020 2020 2020 793a 2054              y: T
-0000c100: 6865 2076 6172 6961 626c 6520 7765 2077  he variable we w
-0000c110: 6973 6820 746f 206f 7074 696d 697a 652e  ish to optimize.
-0000c120: 0a20 2020 2020 2020 2020 2020 206e 3a20  .            n: 
-0000c130: 5468 6520 6e75 6d62 6572 206f 6620 696e  The number of in
-0000c140: 7465 7261 6374 696f 6e73 2077 6520 7769  teractions we wi
-0000c150: 7368 2074 6f20 636f 6e73 6964 6572 2e0a  sh to consider..
-0000c160: 2020 2020 2020 2020 2020 2020 6675 6c6c              full
-0000c170: 5f6c 3a20 5468 6520 7472 7565 206c 6f77  _l: The true low
-0000c180: 6573 7420 6c65 7665 6c20 6c61 6265 6c20  est level label 
-0000c190: 2865 2e67 2e2c 206c 6561 726e 6572 5f69  (e.g., learner_i
-0000c1a0: 6429 0a20 2020 2020 2020 2020 2020 2066  d).            f
-0000c1b0: 756c 6c5f 703a 2054 6865 2074 7275 6520  ull_p: The true 
-0000c1c0: 6c6f 7765 7374 206c 6576 656c 2070 6169  lowest level pai
-0000c1d0: 7220 2865 2e67 2e2c 2065 6e76 6972 6f6e  r (e.g., environ
-0000c1e0: 6d65 6e74 5f69 6429 0a0a 2020 2020 2020  ment_id)..      
-0000c1f0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000c200: 2020 2020 2020 2041 2052 6573 756c 7420         A Result 
-0000c210: 7769 7468 2066 756c 6c20 606c 6020 616e  with full `l` an
-0000c220: 6420 6070 6020 7468 6174 2069 7320 7468  d `p` that is th
-0000c230: 6520 6f70 7469 6d61 6c20 6f76 6572 0a20  e optimal over. 
-0000c240: 2020 2020 2020 2020 2020 2020 2020 2060                 `
-0000c250: 6675 6c6c 5f6c 6020 616e 6420 6066 756c  full_l` and `ful
-0000c260: 6c5f 7060 2e20 466f 7220 6578 616d 706c  l_p`. For exampl
-0000c270: 6520 7765 2063 6f75 6c64 2073 6179 2060  e we could say `
-0000c280: 6c60 0a20 2020 2020 2020 2020 2020 2020  l`.             
-0000c290: 2020 2069 7320 2766 616d 696c 7927 2077     is 'family' w
-0000c2a0: 6869 6c65 2060 6675 6c6c 5f6c 6020 6973  hile `full_l` is
-0000c2b0: 2027 6c65 6172 6e65 725f 6964 272e 2054   'learner_id'. T
-0000c2c0: 6869 7320 776f 756c 640a 2020 2020 2020  his would.      
-0000c2d0: 2020 2020 2020 2020 2020 7069 636b 2074            pick t
-0000c2e0: 6865 2062 6573 7420 7065 7266 6f72 6d69  he best performi
-0000c2f0: 6e67 206c 6561 726e 6572 2067 726f 7570  ng learner group
-0000c300: 6564 2062 7920 6661 6d69 6c79 2066 6f72  ed by family for
-0000c310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c320: 2065 6163 6820 6070 602e 0a0a 2020 2020   each `p`...    
-0000c330: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-0000c340: 2072 6574 7572 6e20 7365 6c66 2e66 696c   return self.fil
-0000c350: 7465 725f 6265 7374 286c 2c70 2c79 2c6e  ter_best(l,p,y,n
-0000c360: 2c66 756c 6c5f 6c2c 6675 6c6c 5f70 290a  ,full_l,full_p).
-0000c370: 0a20 2020 2064 6566 2077 6865 7265 5f66  .    def where_f
-0000c380: 696e 2873 656c 662c 0a20 2020 2020 2020  in(self,.       
-0000c390: 206e 3a20 556e 696f 6e5b 696e 742c 4c69   n: Union[int,Li
-0000c3a0: 7465 7261 6c5b 276d 696e 275d 5d20 3d20  teral['min']] = 
-0000c3b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c3a  None,.        l:
-0000c3c0: 2055 6e69 6f6e 5b73 7472 2c20 5365 7175   Union[str, Sequ
-0000c3d0: 656e 6365 5b73 7472 5d5d 203d 204e 6f6e  ence[str]] = Non
-0000c3e0: 652c 0a20 2020 2020 2020 2070 3a20 556e  e,.        p: Un
-0000c3f0: 696f 6e5b 7374 722c 2053 6571 7565 6e63  ion[str, Sequenc
-0000c400: 655b 7374 725d 5d20 3d20 4e6f 6e65 2920  e[str]] = None) 
-0000c410: 2d3e 2027 5265 7375 6c74 273a 0a20 2020  -> 'Result':.   
-0000c420: 2020 2020 2022 2222 4669 6c74 6572 2074       """Filter t
-0000c430: 6865 2072 6573 756c 7473 2064 6f77 6e20  he results down 
-0000c440: 746f 2065 7665 6e20 6f75 7463 6f6d 6573  to even outcomes
-0000c450: 2073 6f20 7468 6174 2070 6c6f 7474 6564   so that plotted
-0000c460: 2072 6573 756c 7473 2077 696c 6c20 6265   results will be
-0000c470: 206d 6561 6e69 6e67 6675 6c2e 0a0a 2020   meaningful...  
-0000c480: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-0000c490: 2020 2020 2020 2020 6e3a 2054 6865 206e          n: The n
-0000c4a0: 756d 6265 7220 6f66 2069 6e74 6572 6163  umber of interac
-0000c4b0: 7469 6f6e 7320 6120 7370 6563 6966 6963  tions a specific
-0000c4c0: 2065 7661 6c75 6174 696f 6e20 6d75 7374   evaluation must
-0000c4d0: 2068 6176 6520 284e 6f6e 6520 696e 6469   have (None indi
-0000c4e0: 6361 7465 7320 6e6f 2063 6f6e 7374 7261  cates no constra
-0000c4f0: 696e 7429 2e0a 2020 2020 2020 2020 2020  int)..          
-0000c500: 2020 6c3a 2054 6865 206c 6576 656c 2061    l: The level a
-0000c510: 7420 7768 6963 6820 7765 2077 6973 6820  t which we wish 
-0000c520: 746f 2063 6f6d 7061 7265 2065 7661 6c61  to compare evala
-0000c530: 7469 6f6e 206f 7574 636f 6d65 7320 2865  tion outcomes (e
-0000c540: 2e67 2e2c 2027 6c65 6172 6e65 725f 6964  .g., 'learner_id
-0000c550: 2729 2e0a 2020 2020 2020 2020 2020 2020  ')..            
-0000c560: 703a 2054 6865 2070 6169 7273 2074 6861  p: The pairs tha
-0000c570: 7420 6d75 7374 2065 7869 7374 2061 6372  t must exist acr
-0000c580: 6f73 7320 616c 6c20 606c 6020 696e 206f  oss all `l` in o
-0000c590: 7264 6572 2074 6f20 6265 2069 6e63 6c75  rder to be inclu
-0000c5a0: 6465 6420 2865 2e67 2e2c 2027 656e 7669  ded (e.g., 'envi
-0000c5b0: 726f 6e6d 656e 745f 6964 2729 2e0a 0a20  ronment_id')... 
-0000c5c0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0000c5d0: 2020 2020 2020 2020 2020 2020 4120 6052              A `R
-0000c5e0: 6573 756c 7460 2077 6865 7265 2061 6e20  esult` where an 
-0000c5f0: 606c 6020 6578 6973 7473 2066 6f72 2065  `l` exists for e
-0000c600: 7665 7279 2060 7060 2061 6e64 2061 6c6c  very `p` and all
-0000c610: 2060 7060 2068 6176 6520 276e 2720 696e   `p` have 'n' in
-0000c620: 7465 7261 6374 696f 6e73 2e0a 2020 2020  teractions..    
-0000c630: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-0000c640: 2072 6574 7572 6e20 7365 6c66 2e66 696c   return self.fil
-0000c650: 7465 725f 6669 6e28 6e2c 6c2c 7029 0a0a  ter_fin(n,l,p)..
-0000c660: 2020 2020 6465 6620 7768 6572 6528 7365      def where(se
-0000c670: 6c66 2c20 2a2a 6b77 6172 6773 2920 2d3e  lf, **kwargs) ->
-0000c680: 2027 5265 7375 6c74 273a 0a20 2020 2020   'Result':.     
-0000c690: 2020 2022 2222 5365 6c65 6374 206c 6561     """Select lea
-0000c6a0: 726e 6572 732f 656e 7669 726f 6e6d 656e  rners/environmen
-0000c6b0: 7473 2f65 7661 6c75 6174 6f72 732e 0a0a  ts/evaluators...
-0000c6c0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0000c6d0: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
-0000c6e0: 3a20 416e 7920 636f 6c75 6d6e 2069 6e20  : Any column in 
-0000c6f0: 656e 7669 726f 6e6d 656e 7473 2c20 6c65  environments, le
-0000c700: 6172 6e65 7273 2c20 616e 6420 6576 616c  arners, and eval
-0000c710: 7561 746f 7273 2074 6f20 6669 6c74 6572  uators to filter
-0000c720: 206f 6e2e 2042 790a 2020 2020 2020 2020   on. By.        
-0000c730: 2020 2020 2020 2020 6465 6661 756c 7420          default 
-0000c740: 636f 6d70 6172 6973 6f6e 206f 7065 7261  comparison opera
-0000c750: 746f 7273 2061 7265 2065 6974 6865 7220  tors are either 
-0000c760: 2765 7175 616c 2720 6f72 2027 696e 272e  'equal' or 'in'.
-0000c770: 2046 6f72 2065 7861 6d70 6c65 2c0a 2020   For example,.  
-0000c780: 2020 2020 2020 2020 2020 2020 2020 7768                wh
-0000c790: 6572 6528 656e 7669 726f 6e6d 656e 745f  ere(environment_
-0000c7a0: 6964 3d31 2920 776f 756c 6420 7265 7475  id=1) would retu
-0000c7b0: 726e 2061 2052 6573 756c 7420 7768 6572  rn a Result wher
-0000c7c0: 6520 656e 7669 726f 6e6d 656e 7473 206f  e environments o
-0000c7d0: 6e6c 7920 636f 6e74 6169 6e73 0a20 2020  nly contains.   
-0000c7e0: 2020 2020 2020 2020 2020 2020 2065 6e76               env
-0000c7f0: 6972 6f6e 6d65 6e74 5f69 6420 312e 204f  ironment_id 1. O
-0000c800: 6e20 7468 6520 6f74 6865 7220 6861 6e64  n the other hand
-0000c810: 2077 6865 7265 2865 6e76 6972 6f6e 6d65   where(environme
-0000c820: 6e74 5f69 643d 5b31 2c32 5d29 2077 6f75  nt_id=[1,2]) wou
-0000c830: 6c64 2072 6574 7572 6e20 610a 2020 2020  ld return a.    
-0000c840: 2020 2020 2020 2020 2020 2020 5265 7375              Resu
-0000c850: 6c74 2077 6865 7265 2065 6e76 6972 6f6e  lt where environ
-0000c860: 6d65 6e74 7320 636f 6e74 6169 6e73 2065  ments contains e
-0000c870: 6e76 6972 6f6e 6d65 6e74 5f69 6420 3120  nvironment_id 1 
-0000c880: 616e 6420 322e 2054 6865 206b 6579 776f  and 2. The keywo
-0000c890: 7264 7320 6d75 7374 0a20 2020 2020 2020  rds must.       
-0000c8a0: 2020 2020 2020 2020 2069 6e64 6963 6174           indicat
-0000c8b0: 6520 6120 636f 6c75 6d6e 206e 616d 6520  e a column name 
-0000c8c0: 696e 2065 6974 6865 7220 656e 7669 726f  in either enviro
-0000c8d0: 6e6d 656e 7473 2c20 6c65 6172 6e65 7273  nments, learners
-0000c8e0: 2c20 6576 616c 7561 746f 7273 2c20 6f72  , evaluators, or
-0000c8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c900: 2069 6e74 6572 6163 7469 6f6e 732e 2053   interactions. S
-0000c910: 7570 706f 7274 6564 2063 6f6d 7061 7269  upported compari
-0000c920: 736f 6e20 6f70 6572 6174 6f72 7320 6172  son operators ar
-0000c930: 6520 273d 272c 2721 3d27 2c27 3c3d 272c  e '=','!=','<=',
-0000c940: 273c 272c 273e 272c 273e 3d27 2c0a 2020  '<','>','>=',.  
-0000c950: 2020 2020 2020 2020 2020 2020 2020 276d                'm
-0000c960: 6174 6368 272c 2769 6e27 2c27 2169 6e27  atch','in','!in'
-0000c970: 2e20 546f 2069 6e64 6963 6174 6520 616e  . To indicate an
-0000c980: 2065 7870 6c69 6369 7420 6f70 6572 6174   explicit operat
-0000c990: 6f72 2075 7365 2061 2064 6963 7469 6f6e  or use a diction
-0000c9a0: 6172 792e 2046 6f72 0a20 2020 2020 2020  ary. For.       
-0000c9b0: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
-0000c9c0: 2c20 7768 6572 6528 656e 7669 726f 6e6d  , where(environm
-0000c9d0: 656e 745f 6964 3d7b 273c 3d27 3a31 3030  ent_id={'<=':100
-0000c9e0: 7d29 2077 6f75 6c64 2072 6574 7572 6e20  }) would return 
-0000c9f0: 6120 5265 7375 6c74 2077 6974 6820 616c  a Result with al
-0000ca00: 6c0a 2020 2020 2020 2020 2020 2020 2020  l.              
-0000ca10: 2020 656e 7669 726f 6e6d 656e 7473 2077    environments w
-0000ca20: 686f 7365 2065 6e76 6972 6f6e 6d65 6e74  hose environment
-0000ca30: 5f69 6420 3c3d 2031 3030 2e20 496e 636c  _id <= 100. Incl
-0000ca40: 7564 696e 6720 6d75 6c74 6970 6c65 206b  uding multiple k
-0000ca50: 7761 7267 7320 696e 2061 0a20 2020 2020  wargs in a.     
-0000ca60: 2020 2020 2020 2020 2020 2073 696e 676c             singl
-0000ca70: 6520 7768 6572 6520 6170 706c 6965 7320  e where applies 
-0000ca80: 616e 206f 7220 636f 6e6a 7563 7469 6f6e  an or conjuction
-0000ca90: 2e20 4368 6169 6e69 6e67 2077 6865 7265  . Chaining where
-0000caa0: 2073 7461 7465 6d65 6e74 7320 6973 2065   statements is e
-0000cab0: 7175 6976 616c 656e 740a 2020 2020 2020  quivalent.      
-0000cac0: 2020 2020 2020 2020 2020 746f 2061 6e20            to an 
-0000cad0: 616e 6420 636f 6e6a 7563 746f 722e 0a0a  and conjuctor...
-0000cae0: 2020 2020 2020 2020 5265 7574 726e 733a          Reutrns:
-0000caf0: 0a20 2020 2020 2020 2020 2020 2041 2060  .            A `
-0000cb00: 5265 7375 6c74 6020 7768 6f73 6520 656e  Result` whose en
-0000cb10: 7669 726f 6e6d 656e 7473 2c20 6c65 6172  vironments, lear
-0000cb20: 6e65 7273 2c20 6576 616c 7561 746f 7273  ners, evaluators
-0000cb30: 2c20 616e 6420 696e 7465 7261 6374 696f  , and interactio
-0000cb40: 6e73 2073 6174 6973 6679 2074 6865 0a20  ns satisfy the. 
-0000cb50: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000cb60: 6865 7265 2073 656c 6563 746f 7273 2e0a  here selectors..
-0000cb70: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000cb80: 2020 2020 656e 765f 6b77 6172 6773 203d      env_kwargs =
-0000cb90: 207b 7d0a 2020 2020 2020 2020 6c72 6e5f   {}.        lrn_
-0000cba0: 6b77 6172 6773 203d 207b 7d0a 2020 2020  kwargs = {}.    
-0000cbb0: 2020 2020 7661 6c5f 6b77 6172 6773 203d      val_kwargs =
-0000cbc0: 207b 7d0a 2020 2020 2020 2020 696e 745f   {}.        int_
-0000cbd0: 6b77 6172 6773 203d 207b 7d0a 0a20 2020  kwargs = {}..   
-0000cbe0: 2020 2020 2066 6f72 206b 6579 2c61 7267       for key,arg
-0000cbf0: 2069 6e20 6b77 6172 6773 2e69 7465 6d73   in kwargs.items
-0000cc00: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000cc10: 6966 206b 6579 2069 6e20 7365 6c66 2e65  if key in self.e
-0000cc20: 6e76 6972 6f6e 6d65 6e74 732e 636f 6c75  nvironments.colu
-0000cc30: 6d6e 733a 0a20 2020 2020 2020 2020 2020  mns:.           
-0000cc40: 2020 2020 2065 6e76 5f6b 7761 7267 735b       env_kwargs[
-0000cc50: 6b65 795d 203d 2061 7267 0a20 2020 2020  key] = arg.     
-0000cc60: 2020 2020 2020 2065 6c69 6620 6b65 7920         elif key 
-0000cc70: 696e 2073 656c 662e 6c65 6172 6e65 7273  in self.learners
-0000cc80: 2e63 6f6c 756d 6e73 3a0a 2020 2020 2020  .columns:.      
-0000cc90: 2020 2020 2020 2020 2020 6c72 6e5f 6b77            lrn_kw
-0000cca0: 6172 6773 5b6b 6579 5d20 3d20 6172 670a  args[key] = arg.
-0000ccb0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0000ccc0: 206b 6579 2069 6e20 7365 6c66 2e65 7661   key in self.eva
-0000ccd0: 6c75 6174 6f72 732e 636f 6c75 6d6e 733a  luators.columns:
-0000cce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ccf0: 2076 616c 5f6b 7761 7267 735b 6b65 795d   val_kwargs[key]
-0000cd00: 203d 2061 7267 0a20 2020 2020 2020 2020   = arg.         
-0000cd10: 2020 2065 6c69 6620 6b65 7920 696e 2073     elif key in s
-0000cd20: 656c 662e 696e 7465 7261 6374 696f 6e73  elf.interactions
-0000cd30: 2e63 6f6c 756d 6e73 3a0a 2020 2020 2020  .columns:.      
-0000cd40: 2020 2020 2020 2020 2020 696e 745f 6b77            int_kw
-0000cd50: 6172 6773 5b6b 6579 5d20 3d20 6172 670a  args[key] = arg.
-0000cd60: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000cd70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000cd80: 2020 7261 6973 6520 436f 6261 4578 6365    raise CobaExce
-0000cd90: 7074 696f 6e28 2241 6e20 756e 7265 636f  ption("An unreco
-0000cda0: 676e 697a 6564 2063 6f6c 756d 6e20 7761  gnized column wa
-0000cdb0: 7320 7072 6f76 6964 6564 2074 6f20 6077  s provided to `w
-0000cdc0: 6865 7265 6020 666f 7220 6669 6c74 6572  here` for filter
-0000cdd0: 696e 672e 2229 0a0a 2020 2020 2020 2020  ing.")..        
-0000cde0: 6f75 7420 3d20 7365 6c66 0a0a 2020 2020  out = self..    
-0000cdf0: 2020 2020 6966 2065 6e76 5f6b 7761 7267      if env_kwarg
-0000ce00: 733a 206f 7574 203d 206f 7574 2e66 696c  s: out = out.fil
-0000ce10: 7465 725f 656e 7628 2a2a 656e 765f 6b77  ter_env(**env_kw
-0000ce20: 6172 6773 290a 2020 2020 2020 2020 6966  args).        if
-0000ce30: 206c 726e 5f6b 7761 7267 733a 206f 7574   lrn_kwargs: out
-0000ce40: 203d 206f 7574 2e66 696c 7465 725f 6c72   = out.filter_lr
-0000ce50: 6e28 2a2a 6c72 6e5f 6b77 6172 6773 290a  n(**lrn_kwargs).
-0000ce60: 2020 2020 2020 2020 6966 2076 616c 5f6b          if val_k
-0000ce70: 7761 7267 733a 206f 7574 203d 206f 7574  wargs: out = out
-0000ce80: 2e66 696c 7465 725f 7661 6c28 2a2a 7661  .filter_val(**va
-0000ce90: 6c5f 6b77 6172 6773 290a 2020 2020 2020  l_kwargs).      
-0000cea0: 2020 6966 2069 6e74 5f6b 7761 7267 733a    if int_kwargs:
-0000ceb0: 206f 7574 203d 206f 7574 2e66 696c 7465   out = out.filte
-0000cec0: 725f 696e 7428 2a2a 696e 745f 6b77 6172  r_int(**int_kwar
-0000ced0: 6773 290a 0a20 2020 2020 2020 2072 6574  gs)..        ret
-0000cee0: 7572 6e20 6f75 740a 0a20 2020 2064 6566  urn out..    def
-0000cef0: 2072 6177 5f6c 6561 726e 6572 7328 7365   raw_learners(se
-0000cf00: 6c66 2c0a 2020 2020 2020 2020 7820 2020  lf,.        x   
-0000cf10: 3a20 556e 696f 6e5b 7374 722c 2053 6571  : Union[str, Seq
-0000cf20: 7565 6e63 655b 7374 725d 5d20 3d20 2769  uence[str]] = 'i
-0000cf30: 6e64 6578 272c 0a20 2020 2020 2020 2079  ndex',.        y
-0000cf40: 2020 203a 2073 7472 2020 2020 2020 2020     : str        
-0000cf50: 2020 2020 2020 2020 2020 2020 2020 203d                 =
-0000cf60: 2027 7265 7761 7264 272c 0a20 2020 2020   'reward',.     
-0000cf70: 2020 206c 2020 203a 2055 6e69 6f6e 5b73     l   : Union[s
-0000cf80: 7472 2c20 5365 7175 656e 6365 5b73 7472  tr, Sequence[str
-0000cf90: 5d5d 203d 2027 6675 6c6c 5f6e 616d 6527  ]] = 'full_name'
-0000cfa0: 2c0a 2020 2020 2020 2020 7020 2020 3a20  ,.        p   : 
-0000cfb0: 556e 696f 6e5b 7374 722c 2053 6571 7565  Union[str, Seque
-0000cfc0: 6e63 655b 7374 725d 5d20 3d20 2765 6e76  nce[str]] = 'env
-0000cfd0: 6972 6f6e 6d65 6e74 5f69 6427 2c0a 2020  ironment_id',.  
-0000cfe0: 2020 2020 2020 7370 616e 3a20 696e 7420        span: int 
-0000cff0: 3d20 4e6f 6e65 2920 2d3e 2054 6162 6c65  = None) -> Table
-0000d000: 3a0a 2020 2020 2020 2020 2222 2241 2054  :.        """A T
-0000d010: 6162 6c65 2077 6974 6820 7468 6520 7261  able with the ra
-0000d020: 7720 6461 7461 2075 7365 6420 666f 7220  w data used for 
-0000d030: 706c 6f74 5f6c 6561 726e 6572 732e 0a0a  plot_learners...
-0000d040: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0000d050: 2020 2020 2020 2020 2020 783a 2054 6865            x: The
-0000d060: 2076 6172 6961 626c 6573 2074 6f20 706c   variables to pl
-0000d070: 6f74 206f 6e20 7468 6520 782d 6178 6973  ot on the x-axis
-0000d080: 2e0a 2020 2020 2020 2020 2020 2020 793a  ..            y:
-0000d090: 2054 6865 2076 6172 6961 626c 6520 746f   The variable to
-0000d0a0: 2070 6c6f 7420 6f6e 2074 6865 2079 2d61   plot on the y-a
-0000d0b0: 7869 732e 0a20 2020 2020 2020 2020 2020  xis..           
-0000d0c0: 206c 3a20 5468 6520 6c61 6265 6c73 2074   l: The labels t
-0000d0d0: 6f20 7573 6520 696e 2074 6865 2070 6c6f  o use in the plo
-0000d0e0: 7420 6c65 6765 6e64 2e0a 2020 2020 2020  t legend..      
-0000d0f0: 2020 2020 2020 703a 2054 6865 2070 6169        p: The pai
-0000d100: 7269 6e67 7320 746f 2072 6571 7569 7265  rings to require
-0000d110: 2061 6372 6f73 7320 616c 6c20 6c2e 2049   across all l. I
-0000d120: 6620 4e6f 6e65 206e 6f20 7061 6972 696e  f None no pairin
-0000d130: 6720 6368 6563 6b73 2061 7265 2070 6572  g checks are per
-0000d140: 666f 726d 6564 2e0a 2020 2020 2020 2020  formed..        
-0000d150: 2020 2020 7370 616e 3a20 5468 6520 7369      span: The si
-0000d160: 7a65 206f 6620 7468 6520 726f 6c6c 696e  ze of the rollin
-0000d170: 6720 6176 6572 6167 6520 284e 6f6e 6520  g average (None 
-0000d180: 6d65 616e 7320 7072 6f67 7265 7373 6976  means progressiv
-0000d190: 6520 6d65 616e 2e29 0a0a 2020 2020 2020  e mean.)..      
-0000d1a0: 2020 5265 7574 726e 733a 0a20 2020 2020    Reutrns:.     
-0000d1b0: 2020 2020 2020 2041 2054 6162 6c65 2077         A Table w
-0000d1c0: 6974 6820 7468 6520 7261 7720 6461 7461  ith the raw data
-0000d1d0: 2075 7365 6420 746f 2063 6f6e 7374 7275   used to constru
-0000d1e0: 6374 2070 6c6f 745f 6c65 6172 6e65 7273  ct plot_learners
-0000d1f0: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
-0000d200: 2020 2020 2020 2069 6620 703a 2070 6c6f         if p: plo
-0000d210: 7474 6162 6c65 203d 2073 656c 662e 5f70  ttable = self._p
-0000d220: 6c6f 7474 6162 6c65 2878 2c79 292e 5f66  lottable(x,y)._f
-0000d230: 696e 6973 6865 6428 782c 792c 6c2c 7029  inished(x,y,l,p)
-0000d240: 0a20 2020 2020 2020 2065 6c73 653a 2070  .        else: p
-0000d250: 6c6f 7474 6162 6c65 203d 2073 656c 662e  lottable = self.
-0000d260: 5f70 6c6f 7474 6162 6c65 2878 2c79 290a  _plottable(x,y).
-0000d270: 0a20 2020 2020 2020 2072 6f77 7320 3d20  .        rows = 
-0000d280: 706c 6f74 7461 626c 652e 5f67 726f 7570  plottable._group
-0000d290: 6564 5f79 7328 6c2c 782c 793d 792c 7370  ed_ys(l,x,y=y,sp
-0000d2a0: 616e 3d73 7061 6e29 0a0a 2020 2020 2020  an=span)..      
-0000d2b0: 2020 5873 203d 2073 6574 286d 6170 2869    Xs = set(map(i
-0000d2c0: 7465 6d67 6574 7465 7228 3129 2c72 6f77  temgetter(1),row
-0000d2d0: 7329 290a 0a20 2020 2020 2020 2074 7279  s))..        try
-0000d2e0: 3a0a 2020 2020 2020 2020 2020 2020 5873  :.            Xs
-0000d2f0: 203d 2064 6963 7428 7a69 7028 736f 7274   = dict(zip(sort
-0000d300: 6564 2858 7329 2c63 6f75 6e74 2829 2929  ed(Xs),count()))
-0000d310: 0a20 2020 2020 2020 2065 7863 6570 743a  .        except:
-0000d320: 0a20 2020 2020 2020 2020 2020 2058 7320  .            Xs 
-0000d330: 3d20 6469 6374 287a 6970 2873 6f72 7465  = dict(zip(sorte
-0000d340: 6428 5873 2c6b 6579 3d73 7472 292c 636f  d(Xs,key=str),co
-0000d350: 756e 7428 2929 290a 0a20 2020 2020 2020  unt()))..       
-0000d360: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0000d370: 2020 726f 7773 203d 2073 6f72 7465 6428    rows = sorted(
-0000d380: 726f 7773 290a 2020 2020 2020 2020 6578  rows).        ex
-0000d390: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
-0000d3a0: 2020 736f 7274 6564 5f20 3d20 4661 6c73    sorted_ = Fals
-0000d3b0: 650a 2020 2020 2020 2020 656c 7365 3a0a  e.        else:.
-0000d3c0: 2020 2020 2020 2020 2020 2020 736f 7274              sort
-0000d3d0: 6564 5f20 3d20 5472 7565 0a0a 2020 2020  ed_ = True..    
-0000d3e0: 2020 2020 6461 7461 203d 207b 2778 273a      data = {'x':
-0000d3f0: 206c 6973 7428 5873 2e6b 6579 7328 2929   list(Xs.keys())
-0000d400: 7d0a 2020 2020 2020 2020 666f 7220 5f6c  }.        for _l
-0000d410: 2c20 6772 6f75 7020 696e 2067 726f 7570  , group in group
-0000d420: 6572 2872 6f77 732c 206b 6579 3d69 7465  er(rows, key=ite
-0000d430: 6d67 6574 7465 7228 3029 2c20 7661 6c3d  mgetter(0), val=
-0000d440: 6974 656d 6765 7474 6572 2873 6c69 6365  itemgetter(slice
-0000d450: 2831 2c4e 6f6e 6529 292c 2073 6f72 7465  (1,None)), sorte
-0000d460: 645f 3d73 6f72 7465 645f 293a 0a20 2020  d_=sorted_):.   
-0000d470: 2020 2020 2020 2020 2059 203d 205b 5b66           Y = [[f
-0000d480: 6c6f 6174 2827 6e61 6e27 295d 5d2a 6c65  loat('nan')]]*le
-0000d490: 6e28 5873 290a 2020 2020 2020 2020 2020  n(Xs).          
-0000d4a0: 2020 666f 7220 5f78 2c20 6772 6f75 7020    for _x, group 
-0000d4b0: 696e 2067 726f 7570 6572 2867 726f 7570  in grouper(group
-0000d4c0: 2c20 6b65 793d 6974 656d 6765 7474 6572  , key=itemgetter
-0000d4d0: 2830 292c 2076 616c 3d69 7465 6d67 6574  (0), val=itemget
-0000d4e0: 7465 7228 3129 2c20 736f 7274 6564 5f3d  ter(1), sorted_=
-0000d4f0: 736f 7274 6564 5f29 3a0a 2020 2020 2020  sorted_):.      
-0000d500: 2020 2020 2020 2020 2020 595b 5873 5b5f            Y[Xs[_
-0000d510: 785d 5d20 3d20 6c69 7374 2863 6861 696e  x]] = list(chain
-0000d520: 2e66 726f 6d5f 6974 6572 6162 6c65 2867  .from_iterable(g
-0000d530: 726f 7570 2929 0a20 2020 2020 2020 2020  roup)).         
-0000d540: 2020 2064 6174 615b 5f6c 5d20 3d20 590a     data[_l] = Y.
-0000d550: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0000d560: 6162 6c65 2864 6174 6129 0a0a 2020 2020  able(data)..    
-0000d570: 6465 6620 7261 775f 636f 6e74 7261 7374  def raw_contrast
-0000d580: 2873 656c 662c 0a20 2020 2020 2020 206c  (self,.        l
-0000d590: 3120 203a 2041 6e79 2c0a 2020 2020 2020  1  : Any,.      
-0000d5a0: 2020 6c32 2020 3a20 416e 792c 0a20 2020    l2  : Any,.   
-0000d5b0: 2020 2020 2078 2020 203a 2055 6e69 6f6e       x   : Union
-0000d5c0: 5b73 7472 2c20 5365 7175 656e 6365 5b73  [str, Sequence[s
-0000d5d0: 7472 5d5d 203d 2027 656e 7669 726f 6e6d  tr]] = 'environm
-0000d5e0: 656e 745f 6964 272c 0a20 2020 2020 2020  ent_id',.       
-0000d5f0: 2079 2020 203a 2073 7472 2020 2020 2020   y   : str      
-0000d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d610: 203d 2027 7265 7761 7264 272c 0a20 2020   = 'reward',.   
-0000d620: 2020 2020 206c 2020 203a 2055 6e69 6f6e       l   : Union
-0000d630: 5b73 7472 2c20 5365 7175 656e 6365 5b73  [str, Sequence[s
-0000d640: 7472 5d5d 203d 2027 6c65 6172 6e65 725f  tr]] = 'learner_
-0000d650: 6964 272c 0a20 2020 2020 2020 2070 2020  id',.        p  
-0000d660: 203a 2055 6e69 6f6e 5b73 7472 2c20 5365   : Union[str, Se
-0000d670: 7175 656e 6365 5b73 7472 5d5d 203d 2027  quence[str]] = '
-0000d680: 656e 7669 726f 6e6d 656e 745f 6964 272c  environment_id',
-0000d690: 0a20 2020 2020 2020 2073 7061 6e3a 2069  .        span: i
-0000d6a0: 6e74 203d 204e 6f6e 6529 202d 3e20 5461  nt = None) -> Ta
-0000d6b0: 626c 653a 0a20 2020 2020 2020 2022 2222  ble:.        """
-0000d6c0: 4120 5461 626c 6520 7769 7468 2074 6865  A Table with the
-0000d6d0: 2072 6177 2064 6174 6120 706c 6f74 5f63   raw data plot_c
-0000d6e0: 6f6e 7472 6173 742e 0a0a 2020 2020 2020  ontrast...      
-0000d6f0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0000d700: 2020 2020 6c31 3a20 5468 6520 6669 7273      l1: The firs
-0000d710: 7420 606c 6020 7661 6c75 6520 746f 2063  t `l` value to c
-0000d720: 6f6e 7472 6173 742e 0a20 2020 2020 2020  ontrast..       
-0000d730: 2020 2020 206c 323a 2074 6865 2073 6563       l2: the sec
-0000d740: 6f6e 6420 606c 6020 7661 6c75 6520 746f  ond `l` value to
-0000d750: 2063 6f6e 7472 6173 742e 0a20 2020 2020   contrast..     
-0000d760: 2020 2020 2020 2078 3a20 5468 6520 7661         x: The va
-0000d770: 7269 6162 6c65 7320 746f 2070 6c6f 7420  riables to plot 
-0000d780: 6f6e 2074 6865 2078 2d61 7869 732e 0a20  on the x-axis.. 
-0000d790: 2020 2020 2020 2020 2020 2079 3a20 5468             y: Th
-0000d7a0: 6520 7661 7269 6162 6c65 2074 6f20 706c  e variable to pl
-0000d7b0: 6f74 206f 6e20 7468 6520 792d 6178 6973  ot on the y-axis
-0000d7c0: 2e0a 2020 2020 2020 2020 2020 2020 6c3a  ..            l:
-0000d7d0: 2054 6865 2063 6f6c 756d 6e20 6e61 6d65   The column name
-0000d7e0: 7320 7468 6174 206c 3120 616e 6420 6c32  s that l1 and l2
-0000d7f0: 2072 6570 7265 7365 6e74 2e0a 2020 2020   represent..    
-0000d800: 2020 2020 2020 2020 703a 2054 6865 2070          p: The p
-0000d810: 6169 7269 6e67 7320 746f 2072 6571 7569  airings to requi
-0000d820: 7265 2061 6372 6f73 7320 616c 6c20 6c31  re across all l1
-0000d830: 2061 6e64 206c 322e 0a20 2020 2020 2020   and l2..       
-0000d840: 2020 2020 2073 7061 6e3a 2054 6865 2073       span: The s
-0000d850: 697a 6520 6f66 2074 6865 2072 6f6c 6c69  ize of the rolli
-0000d860: 6e67 2061 7665 7261 6765 2028 4e6f 6e65  ng average (None
-0000d870: 206d 6561 6e73 2070 726f 6772 6573 7369   means progressi
-0000d880: 7665 206d 6561 6e29 2e0a 0a20 2020 2020  ve mean)...     
-0000d890: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
-0000d8a0: 2020 2020 2020 2020 2072 6177 5f63 6f6e           raw_con
-0000d8b0: 7472 6173 7428 312c 322c 783d 2765 6e76  trast(1,2,x='env
-0000d8c0: 6972 6f6e 6d65 6e74 5f69 6427 2c79 3d27  ironment_id',y='
-0000d8d0: 7265 7761 7264 272c 6c3d 276c 6561 726e  reward',l='learn
-0000d8e0: 6572 5f69 6427 2c70 3d27 656e 7669 726f  er_id',p='enviro
-0000d8f0: 6e6d 656e 745f 6964 2729 0a20 2020 2020  nment_id').     
-0000d900: 2020 2020 2020 2077 6f75 6c64 2063 6f6e         would con
-0000d910: 7472 6173 7420 6c65 6172 6e65 725f 6964  trast learner_id
-0000d920: 3d31 2061 6e64 206c 6561 726e 6572 5f69  =1 and learner_i
-0000d930: 643d 3220 696e 2074 6572 6d73 206f 6620  d=2 in terms of 
-0000d940: 7265 7761 7264 206f 6e20 616c 6c20 656e  reward on all en
-0000d950: 7669 726f 6e6d 656e 745f 6964 732e 0a0a  vironment_ids...
-0000d960: 2020 2020 2020 2020 5265 7574 726e 733a          Reutrns:
-0000d970: 0a20 2020 2020 2020 2020 2020 2041 2054  .            A T
-0000d980: 6162 6c65 2077 6974 6820 7468 6520 7261  able with the ra
-0000d990: 7720 6461 7461 2075 7365 6420 746f 2063  w data used to c
-0000d9a0: 6f6e 7374 7275 6374 2070 6c6f 745f 636f  onstruct plot_co
-0000d9b0: 6e74 7261 7374 2e0a 2020 2020 2020 2020  ntrast..        
-0000d9c0: 2222 220a 0a20 2020 2020 2020 206f 675f  """..        og_
-0000d9d0: 6c20 3d20 286c 312c 6c32 290a 0a20 2020  l = (l1,l2)..   
-0000d9e0: 2020 2020 206c 6973 745f 6c69 6b65 3d28       list_like=(
-0000d9f0: 6c69 7374 2c74 7570 6c65 290a 0a20 2020  list,tuple)..   
-0000da00: 2020 2020 2069 6620 2020 2020 6973 696e       if     isin
-0000da10: 7374 616e 6365 286c 2c6c 6973 745f 6c69  stance(l,list_li
-0000da20: 6b65 2920 616e 6420 6e6f 7420 6973 696e  ke) and not isin
-0000da30: 7374 616e 6365 286c 315b 305d 2c6c 6973  stance(l1[0],lis
-0000da40: 745f 6c69 6b65 293a 206c 3120 3d20 5b6c  t_like): l1 = [l
-0000da50: 315d 0a20 2020 2020 2020 2069 6620 2020  1].        if   
-0000da60: 2020 6973 696e 7374 616e 6365 286c 2c6c    isinstance(l,l
-0000da70: 6973 745f 6c69 6b65 2920 616e 6420 6e6f  ist_like) and no
-0000da80: 7420 6973 696e 7374 616e 6365 286c 325b  t isinstance(l2[
-0000da90: 305d 2c6c 6973 745f 6c69 6b65 293a 206c  0],list_like): l
-0000daa0: 3220 3d20 5b6c 325d 0a20 2020 2020 2020  2 = [l2].       
-0000dab0: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-0000dac0: 6365 286c 2c6c 6973 745f 6c69 6b65 2920  ce(l,list_like) 
-0000dad0: 616e 6420 6e6f 7420 6973 696e 7374 616e  and not isinstan
-0000dae0: 6365 286c 3120 2020 2c6c 6973 745f 6c69  ce(l1   ,list_li
-0000daf0: 6b65 293a 206c 3120 3d20 5b6c 315d 0a20  ke): l1 = [l1]. 
-0000db00: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-0000db10: 696e 7374 616e 6365 286c 2c6c 6973 745f  instance(l,list_
-0000db20: 6c69 6b65 2920 616e 6420 6e6f 7420 6973  like) and not is
-0000db30: 696e 7374 616e 6365 286c 3220 2020 2c6c  instance(l2   ,l
-0000db40: 6973 745f 6c69 6b65 293a 206c 3220 3d20  ist_like): l2 = 
-0000db50: 5b6c 325d 0a0a 2020 2020 2020 2020 6966  [l2]..        if
-0000db60: 2061 6e79 285f 6c31 2069 6e20 6c32 2066   any(_l1 in l2 f
-0000db70: 6f72 205f 6c31 2069 6e20 6c31 293a 0a20  or _l1 in l1):. 
-0000db80: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000db90: 2043 6f62 6145 7863 6570 7469 6f6e 2822   CobaException("
-0000dba0: 4120 7661 6c75 6520 6361 6e6e 6f74 2062  A value cannot b
-0000dbb0: 6520 696e 2062 6f74 6820 606c 3160 2061  e in both `l1` a
-0000dbc0: 6e64 2060 6c32 602e 2050 6c65 6173 6520  nd `l2`. Please 
-0000dbd0: 6d61 6b65 2061 2063 6861 6e67 6520 616e  make a change an
-0000dbe0: 6420 7275 6e20 6974 2061 6761 696e 2e22  d run it again."
-0000dbf0: 290a 0a20 2020 2020 2020 2070 6c6f 7474  )..        plott
-0000dc00: 6162 6c65 203d 2073 656c 662e 5f70 6c6f  able = self._plo
-0000dc10: 7474 6162 6c65 2878 2c79 290a 0a20 2020  ttable(x,y)..   
-0000dc20: 2020 2020 204c 312c 4c32 203d 205b 5d2c       L1,L2 = [],
-0000dc30: 5b5d 0a20 2020 2020 2020 2066 6f72 204c  [].        for L
-0000dc40: 2069 6e20 6368 6169 6e28 6c31 2c6c 3229   in chain(l1,l2)
-0000dc50: 3a0a 2020 2020 2020 2020 2020 2020 7375  :.            su
-0000dc60: 6270 6c6f 7420 3d20 706c 6f74 7461 626c  bplot = plottabl
-0000dc70: 650a 2020 2020 2020 2020 2020 2020 7768  e.            wh
-0000dc80: 6572 6573 203d 205b 2028 6c2c 4c29 205d  eres = [ (l,L) ]
-0000dc90: 2069 6620 6973 696e 7374 616e 6365 286c   if isinstance(l
-0000dca0: 2c73 7472 2920 656c 7365 207a 6970 286c  ,str) else zip(l
-0000dcb0: 2c4c 290a 0a20 2020 2020 2020 2020 2020  ,L)..           
-0000dcc0: 206f 6c64 5f6c 6f67 6765 7220 3d20 436f   old_logger = Co
-0000dcd0: 6261 436f 6e74 6578 742e 6c6f 6767 6572  baContext.logger
-0000dce0: 0a20 2020 2020 2020 2020 2020 2043 6f62  .            Cob
-0000dcf0: 6143 6f6e 7465 7874 2e6c 6f67 6765 7220  aContext.logger 
-0000dd00: 3d20 4e75 6c6c 4c6f 6767 6572 2829 0a20  = NullLogger(). 
-0000dd10: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
-0000dd20: 5f2c 765f 2069 6e20 7768 6572 6573 3a20  _,v_ in wheres: 
-0000dd30: 7375 6270 6c6f 7420 3d20 7375 6270 6c6f  subplot = subplo
-0000dd40: 742e 7768 6572 6528 2a2a 7b6c 5f3a 765f  t.where(**{l_:v_
-0000dd50: 7d29 0a20 2020 2020 2020 2020 2020 2043  }).            C
-0000dd60: 6f62 6143 6f6e 7465 7874 2e6c 6f67 6765  obaContext.logge
-0000dd70: 7220 3d20 6f6c 645f 6c6f 6767 6572 0a0a  r = old_logger..
-0000dd80: 2020 2020 2020 2020 2020 2020 2377 6520              #we 
-0000dd90: 6172 6520 6173 7375 6d69 6e67 2061 7420  are assuming at 
-0000dda0: 7468 6973 2070 6f69 6e74 2074 6861 7420  this point that 
-0000ddb0: 6f6e 6c79 2076 616c 6964 0a20 2020 2020  only valid.     
-0000ddc0: 2020 2020 2020 2023 606c 6020 6172 6520         #`l` are 
-0000ddd0: 6c65 6674 2077 6869 6368 2069 736e 2774  left which isn't
-0000dde0: 206e 6563 6573 7361 7269 6c79 2074 6865   necessarily the
-0000ddf0: 2063 6173 650a 2020 2020 2020 2020 2020   case.          
-0000de00: 2020 7661 6c75 6573 203d 2073 7562 706c    values = subpl
-0000de10: 6f74 2e5f 6772 6f75 7065 645f 7973 2870  ot._grouped_ys(p
-0000de20: 2c78 2c79 3d79 2c63 6172 643d 2753 272c  ,x,y=y,card='S',
-0000de30: 7370 616e 3d73 7061 6e29 0a0a 2020 2020  span=span)..    
-0000de40: 2020 2020 2020 2020 6966 204c 2069 6e20          if L in 
-0000de50: 6c31 3a20 4c31 2e65 7874 656e 6428 7661  l1: L1.extend(va
-0000de60: 6c75 6573 290a 2020 2020 2020 2020 2020  lues).          
-0000de70: 2020 656c 7365 2020 2020 2020 3a20 4c32    else      : L2
-0000de80: 2e65 7874 656e 6428 7661 6c75 6573 290a  .extend(values).
-0000de90: 0a20 2020 2020 2020 2023 5765 2068 6176  .        #We hav
-0000dea0: 6520 746f 206d 6174 6572 6961 6c69 7a65  e to materialize
-0000deb0: 2062 6563 6175 7365 2077 6520 6361 6e27   because we can'
-0000dec0: 7420 7265 6c79 206f 6e20 736f 7274 696e  t rely on sortin
-0000ded0: 670a 2020 2020 2020 2020 5031 203d 207b  g.        P1 = {
-0000dee0: 6b3a 6c69 7374 2876 2920 666f 7220 6b2c  k:list(v) for k,
-0000def0: 7620 696e 2067 726f 7570 6572 284c 312c  v in grouper(L1,
-0000df00: 6b65 793d 6974 656d 6765 7474 6572 2830  key=itemgetter(0
-0000df10: 2929 7d0a 2020 2020 2020 2020 5032 203d  ))}.        P2 =
-0000df20: 207b 6b3a 6c69 7374 2876 2920 666f 7220   {k:list(v) for 
-0000df30: 6b2c 7620 696e 2067 726f 7570 6572 284c  k,v in grouper(L
-0000df40: 322c 6b65 793d 6974 656d 6765 7474 6572  2,key=itemgetter
-0000df50: 2830 2929 7d0a 0a20 2020 2020 2020 2064  (0))}..        d
-0000df60: 6566 206d 616b 6578 2878 312c 7832 293a  ef makex(x1,x2):
-0000df70: 2072 6574 7572 6e20 7831 2069 6620 7831   return x1 if x1
-0000df80: 203d 3d20 7832 2065 6c73 6520 6622 7b78   == x2 else f"{x
-0000df90: 327d 2d7b 7831 7d22 0a0a 2020 2020 2020  2}-{x1}"..      
-0000dfa0: 2020 5859 203d 2064 6566 6175 6c74 6469    XY = defaultdi
-0000dfb0: 6374 286c 6973 7429 0a20 2020 2020 2020  ct(list).       
-0000dfc0: 2066 6f72 206b 2069 6e20 5031 2e6b 6579   for k in P1.key
-0000dfd0: 7328 2920 2620 5032 2e6b 6579 7328 293a  s() & P2.keys():
-0000dfe0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000dff0: 7820 3d3d 2027 696e 6465 7827 3a0a 2020  x == 'index':.  
-0000e000: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000e010: 7220 6731 5f2c 2067 325f 2069 6e20 7a69  r g1_, g2_ in zi
-0000e020: 7028 5031 5b6b 5d2c 5032 5b6b 5d29 3a0a  p(P1[k],P2[k]):.
-0000e030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e040: 2020 2020 5859 5b67 315f 5b31 5d5d 2e61      XY[g1_[1]].a
-0000e050: 7070 656e 6428 2867 315f 5b32 5d2c 6732  ppend((g1_[2],g2
-0000e060: 5f5b 325d 2929 0a20 2020 2020 2020 2020  _[2])).         
-0000e070: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000e080: 2020 2020 2020 2020 2066 6f72 2067 315f           for g1_
-0000e090: 2c67 325f 2069 6e20 7072 6f64 7563 7428  ,g2_ in product(
-0000e0a0: 5031 5b6b 5d2c 5032 5b6b 5d29 3a0a 2020  P1[k],P2[k]):.  
-0000e0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0c0: 2020 5859 5b6d 616b 6578 2867 315f 5b31    XY[makex(g1_[1
-0000e0d0: 5d2c 6732 5f5b 315d 295d 2e61 7070 656e  ],g2_[1])].appen
-0000e0e0: 6428 2867 315f 5b32 5d2c 6732 5f5b 325d  d((g1_[2],g2_[2]
-0000e0f0: 2929 0a0a 2020 2020 2020 2020 6966 206e  ))..        if n
-0000e100: 6f74 2058 593a 0a20 2020 2020 2020 2020  ot XY:.         
-0000e110: 2020 2072 6169 7365 2043 6f62 6145 7863     raise CobaExc
-0000e120: 6570 7469 6f6e 2866 2257 6520 7765 7265  eption(f"We were
-0000e130: 2075 6e61 626c 6520 746f 2063 7265 6174   unable to creat
-0000e140: 6520 616e 7920 7061 6972 696e 6773 2074  e any pairings t
-0000e150: 6f20 636f 6e74 7261 7374 2e20 4d61 6b65  o contrast. Make
-0000e160: 2073 7572 6520 6c31 3d7b 6f67 5f6c 5b30   sure l1={og_l[0
-0000e170: 5d7d 2061 6e64 206c 323d 7b6f 675f 6c5b  ]} and l2={og_l[
-0000e180: 315d 7d20 6973 2063 6f72 7265 6374 2e22  1]} is correct."
-0000e190: 290a 0a20 2020 2020 2020 206c 315f 6c61  )..        l1_la
-0000e1a0: 6265 6c20 3d20 7365 6c66 2e5f 6c72 6e5f  bel = self._lrn_
-0000e1b0: 6361 6368 655b 6c31 5b30 5d5d 5b27 6675  cache[l1[0]]['fu
-0000e1c0: 6c6c 5f6e 616d 6527 5d20 6966 206c 3d3d  ll_name'] if l==
-0000e1d0: 276c 6561 726e 6572 5f69 6427 2065 6c73  'learner_id' els
-0000e1e0: 6520 276c 3127 0a20 2020 2020 2020 206c  e 'l1'.        l
-0000e1f0: 325f 6c61 6265 6c20 3d20 7365 6c66 2e5f  2_label = self._
-0000e200: 6c72 6e5f 6361 6368 655b 6c32 5b30 5d5d  lrn_cache[l2[0]]
-0000e210: 5b27 6675 6c6c 5f6e 616d 6527 5d20 6966  ['full_name'] if
-0000e220: 206c 3d3d 276c 6561 726e 6572 5f69 6427   l=='learner_id'
-0000e230: 2065 6c73 6520 276c 3227 0a0a 2020 2020   else 'l2'..    
-0000e240: 2020 2020 582c 5920 3d20 7a69 7028 2a73      X,Y = zip(*s
-0000e250: 6f72 7465 6428 5859 2e69 7465 6d73 2829  orted(XY.items()
-0000e260: 2929 0a0a 2020 2020 2020 2020 7265 7475  ))..        retu
-0000e270: 726e 2054 6162 6c65 287b 2778 273a 2058  rn Table({'x': X
-0000e280: 2c20 286c 315f 6c61 6265 6c2c 6c32 5f6c  , (l1_label,l2_l
-0000e290: 6162 656c 293a 2059 207d 290a 0a20 2020  abel): Y })..   
-0000e2a0: 2064 6566 2070 6c6f 745f 6c65 6172 6e65   def plot_learne
-0000e2b0: 7273 2873 656c 662c 0a20 2020 2020 2020  rs(self,.       
-0000e2c0: 2078 2020 2020 2020 203a 2055 6e69 6f6e   x       : Union
-0000e2d0: 5b73 7472 2c20 5365 7175 656e 6365 5b73  [str, Sequence[s
-0000e2e0: 7472 5d5d 203d 2027 696e 6465 7827 2c0a  tr]] = 'index',.
-0000e2f0: 2020 2020 2020 2020 7920 2020 2020 2020          y       
-0000e300: 3a20 7374 7220 2020 2020 2020 2020 2020  : str           
-0000e310: 2020 2020 2020 2020 2020 2020 3d20 2772              = 'r
-0000e320: 6577 6172 6427 2c0a 2020 2020 2020 2020  eward',.        
-0000e330: 6c20 2020 2020 2020 3a20 556e 696f 6e5b  l       : Union[
-0000e340: 7374 722c 2053 6571 7565 6e63 655b 7374  str, Sequence[st
-0000e350: 725d 5d20 3d20 2766 756c 6c5f 6e61 6d65  r]] = 'full_name
-0000e360: 272c 0a20 2020 2020 2020 2070 2020 2020  ',.        p    
-0000e370: 2020 203a 2055 6e69 6f6e 5b73 7472 2c20     : Union[str, 
-0000e380: 5365 7175 656e 6365 5b73 7472 5d5d 203d  Sequence[str]] =
-0000e390: 2027 656e 7669 726f 6e6d 656e 745f 6964   'environment_id
-0000e3a0: 272c 0a20 2020 2020 2020 2073 7061 6e20  ',.        span 
-0000e3b0: 2020 203a 2069 6e74 203d 204e 6f6e 652c     : int = None,
-0000e3c0: 0a20 2020 2020 2020 2065 7272 2020 2020  .        err    
-0000e3d0: 203a 2055 6e69 6f6e 5b4c 6974 6572 616c   : Union[Literal
-0000e3e0: 5b27 7365 272c 2773 6427 2c27 6273 272c  ['se','sd','bs',
-0000e3f0: 2762 6927 5d2c 2050 6f69 6e74 416e 6449  'bi'], PointAndI
-0000e400: 6e74 6572 7661 6c5d 203d 204e 6f6e 652c  nterval] = None,
-0000e410: 0a20 2020 2020 2020 2065 7272 6576 6572  .        errever
-0000e420: 793a 2069 6e74 203d 204e 6f6e 652c 0a20  y: int = None,. 
-0000e430: 2020 2020 2020 206c 6162 656c 7320 203a         labels  :
-0000e440: 2053 6571 7565 6e63 655b 7374 725d 203d   Sequence[str] =
-0000e450: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
-0000e460: 6f6c 6f72 7320 203a 2055 6e69 6f6e 5b69  olors  : Union[i
-0000e470: 6e74 2c53 6571 7565 6e63 655b 556e 696f  nt,Sequence[Unio
-0000e480: 6e5b 7374 722c 696e 745d 5d5d 203d 204e  n[str,int]]] = N
-0000e490: 6f6e 652c 0a20 2020 2020 2020 2074 6974  one,.        tit
-0000e4a0: 6c65 2020 203a 2073 7472 203d 204e 6f6e  le   : str = Non
-0000e4b0: 652c 0a20 2020 2020 2020 2078 6c61 6265  e,.        xlabe
-0000e4c0: 6c20 203a 2073 7472 203d 204e 6f6e 652c  l  : str = None,
-0000e4d0: 0a20 2020 2020 2020 2079 6c61 6265 6c20  .        ylabel 
-0000e4e0: 203a 2073 7472 203d 204e 6f6e 652c 0a20   : str = None,. 
-0000e4f0: 2020 2020 2020 2078 6c69 6d20 2020 203a         xlim    :
-0000e500: 2054 7570 6c65 5b4f 7074 696f 6e61 6c5b   Tuple[Optional[
-0000e510: 4e75 6d62 6572 5d2c 4f70 7469 6f6e 616c  Number],Optional
-0000e520: 5b4e 756d 6265 725d 5d20 3d20 4e6f 6e65  [Number]] = None
-0000e530: 2c0a 2020 2020 2020 2020 796c 696d 2020  ,.        ylim  
-0000e540: 2020 3a20 5475 706c 655b 4f70 7469 6f6e    : Tuple[Option
-0000e550: 616c 5b4e 756d 6265 725d 2c4f 7074 696f  al[Number],Optio
-0000e560: 6e61 6c5b 4e75 6d62 6572 5d5d 203d 204e  nal[Number]] = N
-0000e570: 6f6e 652c 0a20 2020 2020 2020 2078 7469  one,.        xti
-0000e580: 636b 7320 203a 2062 6f6f 6c20 3d20 5472  cks  : bool = Tr
-0000e590: 7565 2c0a 2020 2020 2020 2020 7974 6963  ue,.        ytic
-0000e5a0: 6b73 2020 3a20 626f 6f6c 203d 2054 7275  ks  : bool = Tru
-0000e5b0: 652c 0a20 2020 2020 2020 206c 6567 656e  e,.        legen
-0000e5c0: 6420 203a 2062 6f6f 6c20 3d20 5472 7565  d  : bool = True
-0000e5d0: 2c0a 2020 2020 2020 2020 616c 7068 6120  ,.        alpha 
-0000e5e0: 2020 3a20 666c 6f61 7420 3d20 312c 0a20    : float = 1,. 
-0000e5f0: 2020 2020 2020 2078 6f72 6465 7220 203a         xorder  :
-0000e600: 204c 6974 6572 616c 5b27 2b27 2c27 2d27   Literal['+','-'
-0000e610: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000e620: 2020 746f 705f 6e20 2020 3a20 696e 7420    top_n   : int 
-0000e630: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000e640: 6f75 7420 2020 2020 3a20 556e 696f 6e5b  out     : Union[
-0000e650: 4e6f 6e65 2c4c 6974 6572 616c 5b27 7363  None,Literal['sc
-0000e660: 7265 656e 275d 2c73 7472 5d20 3d20 2773  reen'],str] = 's
-0000e670: 6372 6565 6e27 2c0a 2020 2020 2020 2020  creen',.        
-0000e680: 6178 203d 204e 6f6e 6529 202d 3e20 4e6f  ax = None) -> No
-0000e690: 6e65 3a0a 2020 2020 2020 2020 2222 2250  ne:.        """P
-0000e6a0: 6c6f 7420 7468 6520 7065 7266 6f72 6d61  lot the performa
-0000e6b0: 6e63 6520 6f66 206d 756c 7469 706c 6520  nce of multiple 
-0000e6c0: 6c65 6172 6e65 7273 206f 6e20 6d75 6c74  learners on mult
-0000e6d0: 6970 6c65 2065 6e76 6972 6f6e 6d65 6e74  iple environment
-0000e6e0: 732e 2049 7420 6769 7665 7320 6120 7365  s. It gives a se
-0000e6f0: 6e73 6520 6f66 2074 6865 0a20 2020 2020  nse of the.     
-0000e700: 2020 2065 7870 6563 7465 6420 7065 7266     expected perf
-0000e710: 6f72 6d61 6e63 6520 666f 7220 6469 6666  ormance for diff
-0000e720: 6572 656e 7420 6c65 6172 6e65 7273 2061  erent learners a
-0000e730: 6372 6f73 7320 696e 6465 7065 6e64 656e  cross independen
-0000e740: 7420 656e 7669 726f 6e6d 656e 7473 2e20  t environments. 
-0000e750: 5468 6973 2070 6c6f 7420 6973 0a20 2020  This plot is.   
-0000e760: 2020 2020 2076 616c 7561 626c 6520 696e       valuable in
-0000e770: 2067 6169 6e69 6e67 2069 6e73 6967 6874   gaining insight
-0000e780: 2069 6e74 6f20 686f 7720 7661 7269 6f75   into how variou
-0000e790: 7320 6c65 6172 6e65 7273 2070 6572 666f  s learners perfo
-0000e7a0: 726d 2069 6e20 636f 6d70 6172 6973 6f6e  rm in comparison
-0000e7b0: 2074 6f20 6f6e 6520 616e 6f74 6865 722e   to one another.
-0000e7c0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-0000e7d0: 2020 2020 2020 2020 2020 2020 783a 2054              x: T
-0000e7e0: 6865 2076 616c 7565 7320 746f 2070 6c6f  he values to plo
-0000e7f0: 7420 6f6e 2074 6865 2078 2d61 7869 732e  t on the x-axis.
-0000e800: 0a20 2020 2020 2020 2020 2020 2079 3a20  .            y: 
-0000e810: 5468 6520 7661 6c75 6520 746f 2070 6c6f  The value to plo
-0000e820: 7420 6f6e 2074 6865 2079 2d61 7869 732e  t on the y-axis.
-0000e830: 0a20 2020 2020 2020 2020 2020 206c 3a20  .            l: 
-0000e840: 5468 6520 7661 6c75 6573 2074 6f20 706c  The values to pl
-0000e850: 6f74 2069 6e20 7468 6520 6c65 6765 6e64  ot in the legend
-0000e860: 2e0a 2020 2020 2020 2020 2020 2020 703a  ..            p:
-0000e870: 2054 6865 2070 6169 7273 2074 6861 7420   The pairs that 
-0000e880: 6d75 7374 2065 7869 7374 2061 6372 6f73  must exist acros
-0000e890: 7320 616c 6c20 6974 656d 7320 696e 2074  s all items in t
-0000e8a0: 6865 206c 6567 656e 6420 696e 206f 7264  he legend in ord
-0000e8b0: 6572 2074 6f20 6265 2069 6e63 6c75 6465  er to be include
-0000e8c0: 642e 0a20 2020 2020 2020 2020 2020 2020  d..             
-0000e8d0: 2020 2049 6620 4e6f 6e65 206e 6f20 7061     If None no pa
-0000e8e0: 6972 696e 6720 2063 6865 636b 7320 6172  iring  checks ar
-0000e8f0: 6520 7065 7266 6f72 6d65 642e 0a20 2020  e performed..   
-0000e900: 2020 2020 2020 2020 2073 7061 6e3a 2054           span: T
-0000e910: 6865 206e 756d 6265 7220 6f66 2079 2076  he number of y v
-0000e920: 616c 7565 7320 746f 2073 6d6f 6f74 6820  alues to smooth 
-0000e930: 746f 6765 7468 6572 2077 6865 6e20 7265  together when re
-0000e940: 706f 7274 696e 6720 792e 2049 6620 7468  porting y. If th
-0000e950: 6973 2069 7320 4e6f 6e65 0a20 2020 2020  is is None.     
-0000e960: 2020 2020 2020 2020 2020 2074 6865 6e20             then 
-0000e970: 7468 6520 6176 6572 6167 6520 6f66 2061  the average of a
-0000e980: 6c6c 2079 2076 616c 7565 7320 7570 2074  ll y values up t
-0000e990: 6f20 6375 7272 656e 7420 6973 2073 686f  o current is sho
-0000e9a0: 776e 206f 7468 6572 7769 7365 2061 206d  wn otherwise a m
-0000e9b0: 6f76 696e 670a 2020 2020 2020 2020 2020  oving.          
-0000e9c0: 2020 2020 2020 6176 6572 6167 6520 7769        average wi
-0000e9d0: 7468 2077 696e 646f 7720 7369 7a65 206f  th window size o
-0000e9e0: 6620 7370 616e 2028 7468 6520 7769 6e64  f span (the wind
-0000e9f0: 6f77 2077 696c 6c20 6265 2073 6d61 6c6c  ow will be small
-0000ea00: 6572 2074 6861 6e20 7370 616e 2069 6e69  er than span ini
-0000ea10: 7469 616c 6c79 292e 0a20 2020 2020 2020  tially)..       
-0000ea20: 2020 2020 2065 7272 3a20 5468 6973 2064       err: This d
-0000ea30: 6574 6572 6d69 6e65 7320 7768 6174 206b  etermines what k
-0000ea40: 696e 6420 6f66 2065 7272 6f72 2062 6172  ind of error bar
-0000ea50: 7320 746f 2070 6c6f 7420 2869 6620 616e  s to plot (if an
-0000ea60: 7929 2e20 4966 2060 4e6f 6e65 6020 7468  y). If `None` th
-0000ea70: 656e 206e 6f20 6261 7273 0a20 2020 2020  en no bars.     
-0000ea80: 2020 2020 2020 2020 2020 2061 7265 2070             are p
-0000ea90: 6c6f 7474 6564 2c20 6966 2027 7365 2720  lotted, if 'se' 
-0000eaa0: 7468 6520 7374 616e 6461 7264 2065 7272  the standard err
-0000eab0: 6f72 2069 7320 7368 6f77 6e2c 2061 6e64  or is shown, and
-0000eac0: 2069 6620 2773 6427 2074 6865 2073 7461   if 'sd' the sta
-0000ead0: 6e64 6172 6420 6465 7669 6174 696f 6e0a  ndard deviation.
-0000eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaf0: 6973 2073 686f 776e 2e0a 2020 2020 2020  is shown..      
-0000eb00: 2020 2020 2020 6572 7265 7665 7279 3a20        errevery: 
-0000eb10: 5468 6973 2064 6574 6572 6d69 6e65 7320  This determines 
-0000eb20: 7468 6520 6672 6571 7565 6e63 7920 6f66  the frequency of
-0000eb30: 2065 7272 6f72 6261 7273 2e20 4966 2060   errorbars. If `
-0000eb40: 4e6f 6e65 6020 7468 6579 2061 7070 6561  None` they appea
-0000eb50: 7220 3525 206f 6620 7468 650a 2020 2020  r 5% of the.    
-0000eb60: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-0000eb70: 2e0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
-0000eb80: 6265 6c73 3a20 5468 6520 6c65 6765 6e64  bels: The legend
-0000eb90: 206c 6162 656c 7320 746f 2075 7365 2069   labels to use i
-0000eba0: 6e20 7468 6520 706c 6f74 2e20 5468 6573  n the plot. Thes
-0000ebb0: 6520 7368 6f75 6c64 2062 6520 696e 206f  e should be in o
-0000ebc0: 7264 6572 206f 6620 7468 6520 6163 7475  rder of the actu
-0000ebd0: 616c 0a20 2020 2020 2020 2020 2020 2020  al.             
-0000ebe0: 2020 206c 6567 656e 6420 6c61 6265 6c73     legend labels
-0000ebf0: 2e0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-0000ec00: 6c6f 7273 3a20 5468 6520 636f 6c6f 7273  lors: The colors
-0000ec10: 2075 7365 6420 746f 2070 6c6f 7420 7468   used to plot th
-0000ec20: 6520 6c65 6172 6e65 7273 2070 6c6f 742e  e learners plot.
-0000ec30: 0a20 2020 2020 2020 2020 2020 2074 6974  .            tit
-0000ec40: 6c65 203a 2054 6865 2074 6974 6c65 2067  le : The title g
-0000ec50: 6976 6520 7468 6520 706c 6f74 2e0a 2020  ive the plot..  
-0000ec60: 2020 2020 2020 2020 2020 786c 6162 656c            xlabel
-0000ec70: 3a20 5468 6520 6c61 6265 6c20 6f6e 2074  : The label on t
-0000ec80: 6865 2078 2d61 7869 732e 0a20 2020 2020  he x-axis..     
-0000ec90: 2020 2020 2020 2079 6c61 6265 6c3a 2054         ylabel: T
-0000eca0: 6865 206c 6162 656c 206f 6e20 7468 6520  he label on the 
-0000ecb0: 792d 6178 6973 2e0a 2020 2020 2020 2020  y-axis..        
-0000ecc0: 2020 2020 786c 696d 3a20 4465 6669 6e65      xlim: Define
-0000ecd0: 2074 6865 2078 2d61 7869 7320 6c69 6d69   the x-axis limi
-0000ece0: 7473 2074 6f20 706c 6f74 2e20 4966 2060  ts to plot. If `
-0000ecf0: 4e6f 6e65 6020 7468 6520 782d 6178 6973  None` the x-axis
-0000ed00: 206c 696d 6974 7320 7769 6c6c 2062 6520   limits will be 
-0000ed10: 696e 6665 7272 6564 2e0a 2020 2020 2020  inferred..      
-0000ed20: 2020 2020 2020 796c 696d 3a20 4465 6669        ylim: Defi
-0000ed30: 6e65 2074 6865 2079 2d61 7869 7320 6c69  ne the y-axis li
-0000ed40: 6d69 7473 2074 6f20 706c 6f74 2e20 4966  mits to plot. If
-0000ed50: 2060 4e6f 6e65 6020 7468 6520 792d 6178   `None` the y-ax
-0000ed60: 6973 206c 696d 6974 7320 7769 6c6c 2062  is limits will b
-0000ed70: 6520 696e 6665 7272 6564 2e0a 2020 2020  e inferred..    
-0000ed80: 2020 2020 2020 2020 7874 6963 6b73 3a20          xticks: 
-0000ed90: 5768 6574 6865 7220 7468 6520 782d 6178  Whether the x-ax
-0000eda0: 6973 206c 6162 656c 7320 7368 6f75 6c64  is labels should
-0000edb0: 2062 6520 6472 6177 6e2e 0a20 2020 2020   be drawn..     
-0000edc0: 2020 2020 2020 2079 7469 636b 733a 2057         yticks: W
-0000edd0: 6865 7468 6572 2074 6865 2079 2d61 7869  hether the y-axi
-0000ede0: 7320 6c61 6265 6c73 2073 686f 756c 6420  s labels should 
-0000edf0: 6265 2064 7261 776e 2e0a 2020 2020 2020  be drawn..      
-0000ee00: 2020 2020 2020 6c65 6765 6e64 3a20 5768        legend: Wh
-0000ee10: 6574 6865 7220 7468 6520 6c65 6765 6e64  ether the legend
-0000ee20: 2066 6f72 2074 6865 2070 6c6f 7420 7368   for the plot sh
-0000ee30: 6f75 6c64 2062 6520 6472 6177 6e2e 0a20  ould be drawn.. 
-0000ee40: 2020 2020 2020 2020 2020 2061 6c70 6861             alpha
-0000ee50: 3a20 5468 6520 6f70 6163 6974 7920 6f66  : The opacity of
-0000ee60: 2064 7261 776e 2064 6174 612e 0a20 2020   drawn data..   
-0000ee70: 2020 2020 2020 2020 2078 6f72 6465 723a           xorder:
-0000ee80: 2049 6e64 6963 6174 6573 2077 6865 7468   Indicates wheth
-0000ee90: 6572 2074 6865 2078 2d61 7869 7320 7368  er the x-axis sh
-0000eea0: 6f75 6c64 2062 6520 696e 2061 7363 656e  ould be in ascen
-0000eeb0: 6469 6e67 2028 2b29 206f 7220 6465 7363  ding (+) or desc
-0000eec0: 656e 6465 696e 6720 282d 2920 6f72 6465  endeing (-) orde
-0000eed0: 722e 0a20 2020 2020 2020 2020 2020 2074  r..            t
-0000eee0: 6f70 5f6e 3a20 4f6e 6c79 2070 6c6f 7420  op_n: Only plot 
-0000eef0: 7468 6520 746f 705f 6e20 6c65 6172 6e65  the top_n learne
-0000ef00: 7273 2e20 4966 2060 4e6f 6e65 6020 616c  rs. If `None` al
-0000ef10: 6c20 6c65 6172 6e65 7273 2077 696c 6c20  l learners will 
-0000ef20: 6265 2070 6c6f 7474 6564 2e20 4966 206e  be plotted. If n
-0000ef30: 6567 6174 6976 650a 2020 2020 2020 2020  egative.        
-0000ef40: 2020 2020 2020 2020 7468 6520 626f 7474          the bott
-0000ef50: 6f6d 2077 696c 6c20 6265 2070 6c6f 7474  om will be plott
-0000ef60: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-0000ef70: 6f75 743a 2049 6e64 6963 6174 6520 7768  out: Indicate wh
-0000ef80: 6572 6520 7468 6520 706c 6f74 2073 686f  ere the plot sho
-0000ef90: 756c 6420 6265 2073 656e 7420 746f 2061  uld be sent to a
-0000efa0: 6674 6572 2070 6c6f 7474 696e 6720 6973  fter plotting is
-0000efb0: 2066 696e 6973 6865 642e 2056 616c 6964   finished. Valid
-0000efc0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
-0000efd0: 2020 2020 2020 2020 6172 6520 2773 6372          are 'scr
-0000efe0: 6565 6e27 2074 6f20 7368 6f77 2069 7420  een' to show it 
-0000eff0: 6f6e 2073 6372 6565 6e2c 2061 2070 6174  on screen, a pat
-0000f000: 6820 746f 2073 6176 6520 746f 2064 6973  h to save to dis
-0000f010: 6b2c 206f 7220 4e6f 6e65 2069 6620 7468  k, or None if th
-0000f020: 6520 706c 6f74 2073 686f 756c 640a 2020  e plot should.  
-0000f030: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-0000f040: 7420 6265 206f 7574 7075 7420 616e 7977  t be output anyw
-0000f050: 6865 7265 2028 692e 652e 2c20 6b65 7074  here (i.e., kept
-0000f060: 2069 6e20 6d65 6d6f 7279 2920 696e 206f   in memory) in o
-0000f070: 7264 6572 2074 6f20 6b65 6570 2065 6469  rder to keep edi
-0000f080: 7469 6e67 2074 6865 2070 6c6f 7420 6166  ting the plot af
-0000f090: 7465 720a 2020 2020 2020 2020 2020 2020  ter.            
-0000f0a0: 2020 2020 7468 6973 2063 616c 6c2e 0a20      this call.. 
-0000f0b0: 2020 2020 2020 2020 2020 2061 783a 2050             ax: P
-0000f0c0: 726f 7669 6465 2061 6e20 6f70 7469 6f6e  rovide an option
-0000f0d0: 616c 2061 7865 7320 7468 6174 2074 6865  al axes that the
-0000f0e0: 2070 6c6f 7420 7769 6c6c 2062 6520 6472   plot will be dr
-0000f0f0: 6177 6e20 746f 2e20 4966 206e 6f74 2070  awn to. If not p
-0000f100: 726f 7669 6465 6420 6120 6e65 770a 2020  rovided a new.  
-0000f110: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-0000f120: 6775 7265 2f61 7865 7320 6973 2063 7265  gure/axes is cre
-0000f130: 6174 6564 2e0a 2020 2020 2020 2020 2222  ated..        ""
-0000f140: 220a 2020 2020 2020 2020 7472 793a 0a20  ".        try:. 
-0000f150: 2020 2020 2020 2020 2020 2078 6c69 6d20             xlim 
-0000f160: 3d20 786c 696d 206f 7220 5b4e 6f6e 652c  = xlim or [None,
-0000f170: 4e6f 6e65 5d0a 2020 2020 2020 2020 2020  None].          
-0000f180: 2020 796c 696d 203d 2079 6c69 6d20 6f72    ylim = ylim or
-0000f190: 205b 4e6f 6e65 2c4e 6f6e 655d 0a0a 2020   [None,None]..  
-0000f1a0: 2020 2020 2020 2020 2020 7261 775f 6461            raw_da
-0000f1b0: 7461 203d 2073 656c 662e 7261 775f 6c65  ta = self.raw_le
-0000f1c0: 6172 6e65 7273 2878 2c79 2c6c 2c70 2c73  arners(x,y,l,p,s
-0000f1d0: 7061 6e29 0a0a 2020 2020 2020 2020 2020  pan)..          
-0000f1e0: 2020 6572 7265 7665 7279 203d 2065 7272    errevery = err
-0000f1f0: 6576 6572 7920 6f72 206d 6178 2869 6e74  every or max(int
-0000f200: 2872 6177 5f64 6174 615b 2778 275d 5b2d  (raw_data['x'][-
-0000f210: 315d 2a30 2e30 3529 2c31 2920 6966 2078  1]*0.05),1) if x
-0000f220: 203d 3d20 2769 6e64 6578 2720 656c 7365   == 'index' else
-0000f230: 2031 0a20 2020 2020 2020 2020 2020 2073   1.            s
-0000f240: 7479 6c65 2020 2020 3d20 222d 2220 6966  tyle    = "-" if
-0000f250: 2078 203d 3d20 2769 6e64 6578 2720 656c   x == 'index' el
-0000f260: 7365 2022 2e22 0a20 2020 2020 2020 2020  se ".".         
-0000f270: 2020 2065 7272 2020 2020 2020 3d20 7365     err      = se
-0000f280: 6c66 2e5f 636f 6e66 6964 656e 6365 2865  lf._confidence(e
-0000f290: 7272 2c20 6572 7265 7665 7279 290a 0a20  rr, errevery).. 
-0000f2a0: 2020 2020 2020 2020 2020 2059 5f63 6f75             Y_cou
-0000f2b0: 6e74 203d 205b 5d0a 2020 2020 2020 2020  nt = [].        
-0000f2c0: 2020 2020 6c69 6e65 733a 204c 6973 745b      lines: List[
-0000f2d0: 506f 696e 7473 5d20 3d20 5b5d 0a20 2020  Points] = [].   
-0000f2e0: 2020 2020 2020 2020 2066 6f72 205f 6c20           for _l 
-0000f2f0: 696e 2072 6177 5f64 6174 612e 636f 6c75  in raw_data.colu
-0000f300: 6d6e 735b 313a 5d3a 0a20 2020 2020 2020  mns[1:]:.       
-0000f310: 2020 2020 2020 2020 2063 6f6c 6f72 203d           color =
-0000f320: 2073 656c 662e 5f67 6574 5f63 6f6c 6f72   self._get_color
-0000f330: 2863 6f6c 6f72 732c 2020 206c 656e 286c  (colors,   len(l
-0000f340: 696e 6573 2929 0a20 2020 2020 2020 2020  ines)).         
-0000f350: 2020 2020 2020 206c 6162 656c 203d 2073         label = s
-0000f360: 656c 662e 5f67 6574 5f6c 6162 656c 286c  elf._get_label(l
-0000f370: 6162 656c 732c 5f6c 2c6c 656e 286c 696e  abels,_l,len(lin
-0000f380: 6573 2929 0a20 2020 2020 2020 2020 2020  es)).           
-0000f390: 2020 2020 2059 5f63 6f75 6e74 2e61 7070       Y_count.app
-0000f3a0: 656e 6428 3029 0a20 2020 2020 2020 2020  end(0).         
-0000f3b0: 2020 2020 2020 206c 696e 6573 2e61 7070         lines.app
-0000f3c0: 656e 6428 506f 696e 7473 2873 7479 6c65  end(Points(style
-0000f3d0: 3d73 7479 6c65 2c63 6f6c 6f72 3d63 6f6c  =style,color=col
-0000f3e0: 6f72 2c6c 6162 656c 3d6c 6162 656c 2c61  or,label=label,a
-0000f3f0: 6c70 6861 3d61 6c70 6861 2929 0a20 2020  lpha=alpha)).   
-0000f400: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000f410: 205f 7869 2c20 285f 782c 2059 2920 696e   _xi, (_x, Y) in
-0000f420: 2065 6e75 6d65 7261 7465 287a 6970 282a   enumerate(zip(*
-0000f430: 7261 775f 6461 7461 5b5b 2778 272c 5f6c  raw_data[['x',_l
-0000f440: 5d5d 2929 3a0a 2020 2020 2020 2020 2020  ]])):.          
-0000f450: 2020 2020 2020 2020 2020 595f 636f 756e            Y_coun
-0000f460: 745b 2d31 5d20 3d20 6d61 7828 595f 636f  t[-1] = max(Y_co
-0000f470: 756e 745b 2d31 5d2c 6c65 6e28 5929 290a  unt[-1],len(Y)).
-0000f480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f490: 2020 2020 6c69 6e65 735b 2d31 5d2e 6164      lines[-1].ad
-0000f4a0: 6428 5f78 2069 6620 5f78 2069 7320 6e6f  d(_x if _x is no
-0000f4b0: 7420 4e6f 6e65 2065 6c73 6520 274e 6f6e  t None else 'Non
-0000f4c0: 6527 2c20 2a65 7272 2859 2c20 5f78 6929  e', *err(Y, _xi)
-0000f4d0: 290a 0a20 2020 2020 2020 2020 2020 206c  )..            l
-0000f4e0: 696e 6573 2020 3d20 736f 7274 6564 286c  ines  = sorted(l
-0000f4f0: 696e 6573 2c20 6b65 793d 6c61 6d62 6461  ines, key=lambda
-0000f500: 206c 696e 653a 206c 696e 652e 595b 2d31   line: line.Y[-1
-0000f510: 5d2c 2072 6576 6572 7365 3d54 7275 6529  ], reverse=True)
-0000f520: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-0000f530: 656c 7320 3d20 5b6c 2e6c 6162 656c 206f  els = [l.label o
-0000f540: 7220 7374 7228 6c2e 6c61 6265 6c29 2066  r str(l.label) f
-0000f550: 6f72 206c 2069 6e20 6c69 6e65 735d 0a20  or l in lines]. 
-0000f560: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-0000f570: 7320 3d20 5b6c 2e63 6f6c 6f72 2020 2020  s = [l.color    
-0000f580: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000f590: 206c 2069 6e20 6c69 6e65 735d 0a20 2020   l in lines].   
-0000f5a0: 2020 2020 2020 2020 2078 6c61 6265 6c20           xlabel 
-0000f5b0: 3d20 786c 6162 656c 206f 7220 2822 496e  = xlabel or ("In
-0000f5c0: 7465 7261 6374 696f 6e22 2069 6620 783d  teraction" if x=
-0000f5d0: 3d27 696e 6465 7827 2065 6c73 6520 785b  ='index' else x[
-0000f5e0: 305d 2069 6620 6c65 6e28 7829 203d 3d20  0] if len(x) == 
-0000f5f0: 3120 656c 7365 2078 290a 2020 2020 2020  1 else x).      
-0000f600: 2020 2020 2020 796c 6162 656c 203d 2079        ylabel = y
-0000f610: 6c61 6265 6c20 6f72 2028 2252 6577 6172  label or ("Rewar
-0000f620: 6422 2069 6620 793d 3d27 7265 7761 7264  d" if y=='reward
-0000f630: 2720 656c 7365 2079 2e72 6570 6c61 6365  ' else y.replace
-0000f640: 2822 5f70 6374 222c 2220 5065 7263 656e  ("_pct"," Percen
-0000f650: 7422 2929 0a0a 2020 2020 2020 2020 2020  t"))..          
-0000f660: 2020 6966 206c 656e 2873 6574 2859 5f63    if len(set(Y_c
-0000f670: 6f75 6e74 2929 203d 3d20 313a 2059 5f63  ount)) == 1: Y_c
-0000f680: 6f75 6e74 203d 2059 5f63 6f75 6e74 5b30  ount = Y_count[0
-0000f690: 5d0a 0a20 2020 2020 2020 2020 2020 2079  ]..            y
-0000f6a0: 5f6c 6f63 6174 696f 6e20 3d20 2254 6f74  _location = "Tot
-0000f6b0: 616c 2220 6966 2078 2021 3d20 2769 6e64  al" if x != 'ind
-0000f6c0: 6578 2720 656c 7365 2022 220a 2020 2020  ex' else "".    
-0000f6d0: 2020 2020 2020 2020 795f 6176 675f 7479          y_avg_ty
-0000f6e0: 7065 203d 2028 2249 6e73 7461 6e74 2220  pe = ("Instant" 
-0000f6f0: 6966 2073 7061 6e20 3d3d 2031 2065 6c73  if span == 1 els
-0000f700: 6520 6622 5370 616e 207b 7370 616e 7d22  e f"Span {span}"
-0000f710: 2069 6620 7370 616e 2065 6c73 6520 2250   if span else "P
-0000f720: 726f 6772 6573 7369 7665 2229 0a20 2020  rogressive").   
-0000f730: 2020 2020 2020 2020 2079 5f73 616d 706c           y_sampl
-0000f740: 6573 2020 3d20 6622 287b 595f 636f 756e  es  = f"({Y_coun
-0000f750: 747d 2045 6e76 6972 6f6e 6d65 6e74 7329  t} Environments)
-0000f760: 220a 2020 2020 2020 2020 2020 2020 7469  ".            ti
-0000f770: 746c 6520 2020 2020 203d 2074 6974 6c65  tle      = title
-0000f780: 2069 6620 7469 746c 6520 6973 206e 6f74   if title is not
-0000f790: 204e 6f6e 6520 656c 7365 2028 2720 272e   None else (' '.
-0000f7a0: 6a6f 696e 2866 696c 7465 7228 4e6f 6e65  join(filter(None
-0000f7b0: 2c5b 795f 6c6f 6361 7469 6f6e 2c20 795f  ,[y_location, y_
-0000f7c0: 6176 675f 7479 7065 2c20 796c 6162 656c  avg_type, ylabel
-0000f7d0: 2c20 795f 7361 6d70 6c65 735d 2929 290a  , y_samples]))).
-0000f7e0: 0a20 2020 2020 2020 2020 2020 2078 726f  .            xro
-0000f7f0: 7461 7469 6f6e 203d 2039 3020 6966 2028  tation = 90 if (
-0000f800: 7820 213d 2027 696e 6465 7827 206f 7220  x != 'index' or 
-0000f810: 786f 7264 6572 2920 616e 6420 6c65 6e28  xorder) and len(
-0000f820: 6c69 6e65 735b 305d 2e58 293e 3520 656c  lines[0].X)>5 el
-0000f830: 7365 2030 0a20 2020 2020 2020 2020 2020  se 0.           
-0000f840: 2079 726f 7461 7469 6f6e 203d 2030 0a0a   yrotation = 0..
-0000f850: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-0000f860: 6f70 5f6e 3a0a 2020 2020 2020 2020 2020  op_n:.          
-0000f870: 2020 2020 2020 6966 2061 6273 2874 6f70        if abs(top
-0000f880: 5f6e 2920 3e20 6c65 6e28 6c69 6e65 7329  _n) > len(lines)
-0000f890: 3a20 746f 705f 6e20 3d20 6c65 6e28 6c69  : top_n = len(li
-0000f8a0: 6e65 7329 2a61 6273 2874 6f70 5f6e 292f  nes)*abs(top_n)/
-0000f8b0: 746f 705f 6e0a 2020 2020 2020 2020 2020  top_n.          
-0000f8c0: 2020 2020 2020 6966 2074 6f70 5f6e 203e        if top_n >
-0000f8d0: 2030 3a20 6c69 6e65 7320 3d20 5b72 6570   0: lines = [rep
-0000f8e0: 6c61 6365 286c 2c63 6f6c 6f72 3d73 656c  lace(l,color=sel
-0000f8f0: 662e 5f67 6574 5f63 6f6c 6f72 2863 6f6c  f._get_color(col
-0000f900: 6f72 732c 6929 2c6c 6162 656c 3d73 656c  ors,i),label=sel
-0000f910: 662e 5f67 6574 5f6c 6162 656c 286c 6162  f._get_label(lab
-0000f920: 656c 732c 6c2e 6c61 6265 6c2c 6929 2920  els,l.label,i)) 
-0000f930: 666f 7220 692c 6c20 696e 2065 6e75 6d65  for i,l in enume
-0000f940: 7261 7465 286c 696e 6573 5b3a 746f 705f  rate(lines[:top_
-0000f950: 6e5d 2c30 2020 2020 2920 5d0a 2020 2020  n],0    ) ].    
-0000f960: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-0000f970: 6f70 5f6e 203c 2030 3a20 6c69 6e65 7320  op_n < 0: lines 
-0000f980: 3d20 5b72 6570 6c61 6365 286c 2c63 6f6c  = [replace(l,col
-0000f990: 6f72 3d73 656c 662e 5f67 6574 5f63 6f6c  or=self._get_col
-0000f9a0: 6f72 2863 6f6c 6f72 732c 6929 2c6c 6162  or(colors,i),lab
-0000f9b0: 656c 3d73 656c 662e 5f67 6574 5f6c 6162  el=self._get_lab
-0000f9c0: 656c 286c 6162 656c 732c 6c2e 6c61 6265  el(labels,l.labe
-0000f9d0: 6c2c 6929 2920 666f 7220 692c 6c20 696e  l,i)) for i,l in
-0000f9e0: 2065 6e75 6d65 7261 7465 286c 696e 6573   enumerate(lines
-0000f9f0: 5b74 6f70 5f6e 3a5d 2c74 6f70 5f6e 2920  [top_n:],top_n) 
-0000fa00: 5d0a 0a20 2020 2020 2020 2020 2020 2061  ]..            a
-0000fa10: 6c6c 5f78 203d 2064 6963 742e 6672 6f6d  ll_x = dict.from
-0000fa20: 6b65 7973 2863 6861 696e 2e66 726f 6d5f  keys(chain.from_
-0000fa30: 6974 6572 6162 6c65 286c 696e 652e 5820  iterable(line.X 
-0000fa40: 666f 7220 6c69 6e65 2069 6e20 6c69 6e65  for line in line
-0000fa50: 7329 290a 2020 2020 2020 2020 2020 2020  s)).            
-0000fa60: 786f 7264 6572 6564 203d 206c 6973 7428  xordered = list(
-0000fa70: 616c 6c5f 782e 6b65 7973 2829 2920 6966  all_x.keys()) if
-0000fa80: 206e 6f74 2078 6f72 6465 7220 656c 7365   not xorder else
-0000fa90: 2073 6f72 7465 6428 616c 6c5f 782c 2072   sorted(all_x, r
-0000faa0: 6576 6572 7365 3d78 6f72 6465 723d 3d27  everse=xorder=='
-0000fab0: 2d27 290a 0a20 2020 2020 2020 2020 2020  -')..           
-0000fac0: 2069 6620 7820 3d3d 2027 696e 6465 7827   if x == 'index'
-0000fad0: 2061 6e64 2078 6f72 6465 7220 696e 205b   and xorder in [
-0000fae0: 272b 272c 4e6f 6e65 5d3a 2078 6f72 6465  '+',None]: xorde
-0000faf0: 7265 6420 3d20 4e6f 6e65 0a0a 2020 2020  red = None..    
-0000fb00: 2020 2020 2020 2020 7365 6c66 2e5f 706c          self._pl
-0000fb10: 6f74 7465 722e 706c 6f74 2861 782c 206c  otter.plot(ax, l
-0000fb20: 696e 6573 2c20 7469 746c 652c 2078 6c61  ines, title, xla
-0000fb30: 6265 6c2c 2079 6c61 6265 6c2c 2078 6c69  bel, ylabel, xli
-0000fb40: 6d2c 2079 6c69 6d2c 2078 7469 636b 732c  m, ylim, xticks,
-0000fb50: 2079 7469 636b 732c 206c 6567 656e 642c   yticks, legend,
-0000fb60: 2078 726f 7461 7469 6f6e 2c20 7972 6f74   xrotation, yrot
-0000fb70: 6174 696f 6e2c 2078 6f72 6465 7265 642c  ation, xordered,
-0000fb80: 206f 7574 290a 0a20 2020 2020 2020 2065   out)..        e
-0000fb90: 7863 6570 7420 436f 6261 4578 6365 7074  xcept CobaExcept
-0000fba0: 696f 6e20 6173 2065 3a0a 2020 2020 2020  ion as e:.      
-0000fbb0: 2020 2020 2020 436f 6261 436f 6e74 6578        CobaContex
-0000fbc0: 742e 6c6f 6767 6572 2e6c 6f67 2873 7472  t.logger.log(str
-0000fbd0: 2865 2929 0a0a 2020 2020 6465 6620 706c  (e))..    def pl
-0000fbe0: 6f74 5f63 6f6e 7472 6173 7428 7365 6c66  ot_contrast(self
-0000fbf0: 2c0a 2020 2020 2020 2020 6c31 2020 2020  ,.        l1    
-0000fc00: 2020 3a20 416e 792c 0a20 2020 2020 2020    : Any,.       
-0000fc10: 206c 3220 2020 2020 203a 2041 6e79 2c0a   l2      : Any,.
-0000fc20: 2020 2020 2020 2020 7820 2020 2020 2020          x       
-0000fc30: 3a20 556e 696f 6e5b 7374 722c 2053 6571  : Union[str, Seq
-0000fc40: 7565 6e63 655b 7374 725d 5d20 3d20 2265  uence[str]] = "e
-0000fc50: 6e76 6972 6f6e 6d65 6e74 5f69 6422 2c0a  nvironment_id",.
-0000fc60: 2020 2020 2020 2020 7920 2020 2020 2020          y       
-0000fc70: 3a20 7374 7220 3d20 2272 6577 6172 6422  : str = "reward"
-0000fc80: 2c0a 2020 2020 2020 2020 6c20 2020 2020  ,.        l     
-0000fc90: 2020 3a20 556e 696f 6e5b 7374 722c 2053    : Union[str, S
-0000fca0: 6571 7565 6e63 655b 7374 725d 5d20 3d20  equence[str]] = 
-0000fcb0: 276c 6561 726e 6572 5f69 6427 2c0a 2020  'learner_id',.  
-0000fcc0: 2020 2020 2020 7020 2020 2020 2020 3a20        p       : 
-0000fcd0: 556e 696f 6e5b 7374 722c 2053 6571 7565  Union[str, Seque
-0000fce0: 6e63 655b 7374 725d 5d20 3d20 2765 6e76  nce[str]] = 'env
-0000fcf0: 6972 6f6e 6d65 6e74 5f69 6427 2c0a 2020  ironment_id',.  
-0000fd00: 2020 2020 2020 6d6f 6465 2020 2020 3a20        mode    : 
-0000fd10: 556e 696f 6e5b 4c69 7465 7261 6c5b 2264  Union[Literal["d
-0000fd20: 6966 6622 2c22 7072 6f62 225d 2c20 4361  iff","prob"], Ca
-0000fd30: 6c6c 6162 6c65 5b5b 666c 6f61 742c 666c  llable[[float,fl
-0000fd40: 6f61 745d 2c66 6c6f 6174 5d5d 203d 2022  oat],float]] = "
-0000fd50: 6469 6666 222c 0a20 2020 2020 2020 2073  diff",.        s
-0000fd60: 7061 6e20 2020 203a 2069 6e74 203d 204e  pan    : int = N
-0000fd70: 6f6e 652c 0a20 2020 2020 2020 2065 7272  one,.        err
-0000fd80: 2020 2020 203a 2055 6e69 6f6e 5b4c 6974       : Union[Lit
-0000fd90: 6572 616c 5b27 7365 272c 2773 6427 2c27  eral['se','sd','
-0000fda0: 6273 272c 2762 6927 5d2c 2050 6f69 6e74  bs','bi'], Point
-0000fdb0: 416e 6449 6e74 6572 7661 6c5d 203d 204e  AndInterval] = N
-0000fdc0: 6f6e 652c 0a20 2020 2020 2020 2065 7272  one,.        err
-0000fdd0: 6576 6572 793a 2069 6e74 203d 204e 6f6e  every: int = Non
-0000fde0: 652c 0a20 2020 2020 2020 206c 6162 656c  e,.        label
-0000fdf0: 7320 203a 2053 6571 7565 6e63 655b 7374  s  : Sequence[st
-0000fe00: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-0000fe10: 2020 2063 6f6c 6f72 7320 203a 2053 6571     colors  : Seq
-0000fe20: 7565 6e63 655b 7374 725d 203d 204e 6f6e  uence[str] = Non
-0000fe30: 652c 0a20 2020 2020 2020 2074 6974 6c65  e,.        title
-0000fe40: 2020 203a 2073 7472 203d 204e 6f6e 652c     : str = None,
-0000fe50: 0a20 2020 2020 2020 2078 6c61 6265 6c20  .        xlabel 
-0000fe60: 203a 2073 7472 203d 204e 6f6e 652c 0a20   : str = None,. 
-0000fe70: 2020 2020 2020 2079 6c61 6265 6c20 203a         ylabel  :
-0000fe80: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-0000fe90: 2020 2020 2078 6c69 6d20 2020 203a 2054       xlim    : T
-0000fea0: 7570 6c65 5b4f 7074 696f 6e61 6c5b 4e75  uple[Optional[Nu
-0000feb0: 6d62 6572 5d2c 4f70 7469 6f6e 616c 5b4e  mber],Optional[N
-0000fec0: 756d 6265 725d 5d20 3d20 4e6f 6e65 2c0a  umber]] = None,.
-0000fed0: 2020 2020 2020 2020 796c 696d 2020 2020          ylim    
-0000fee0: 3a20 5475 706c 655b 4f70 7469 6f6e 616c  : Tuple[Optional
-0000fef0: 5b4e 756d 6265 725d 2c4f 7074 696f 6e61  [Number],Optiona
-0000ff00: 6c5b 4e75 6d62 6572 5d5d 203d 204e 6f6e  l[Number]] = Non
-0000ff10: 652c 0a20 2020 2020 2020 2078 7469 636b  e,.        xtick
-0000ff20: 7320 203a 2062 6f6f 6c20 3d20 5472 7565  s  : bool = True
-0000ff30: 2c0a 2020 2020 2020 2020 7974 6963 6b73  ,.        yticks
-0000ff40: 2020 3a20 626f 6f6c 203d 2054 7275 652c    : bool = True,
-0000ff50: 0a20 2020 2020 2020 206c 6567 656e 6420  .        legend 
-0000ff60: 203a 2062 6f6f 6c20 3d20 5472 7565 2c0a   : bool = True,.
-0000ff70: 2020 2020 2020 2020 616c 7068 6120 2020          alpha   
-0000ff80: 3a20 666c 6f61 7420 3d20 312c 0a20 2020  : float = 1,.   
-0000ff90: 2020 2020 2078 6f72 6465 7220 203a 204c       xorder  : L
-0000ffa0: 6974 6572 616c 5b27 2b27 2c27 2d27 5d20  iteral['+','-'] 
-0000ffb0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000ffc0: 626f 756e 6461 7279 3a20 626f 6f6c 203d  boundary: bool =
-0000ffd0: 2054 7275 652c 0a20 2020 2020 2020 206f   True,.        o
-0000ffe0: 7574 2020 2020 203a 2055 6e69 6f6e 5b4e  ut     : Union[N
-0000fff0: 6f6e 652c 4c69 7465 7261 6c5b 2773 6372  one,Literal['scr
-00010000: 6565 6e27 5d2c 7374 725d 203d 2027 7363  een'],str] = 'sc
-00010010: 7265 656e 272c 0a20 2020 2020 2020 2061  reen',.        a
-00010020: 7820 3d20 4e6f 6e65 2920 2d3e 204e 6f6e  x = None) -> Non
-00010030: 653a 0a20 2020 2020 2020 2022 2222 506c  e:.        """Pl
-00010040: 6f74 2061 2064 6972 6563 7420 636f 6e74  ot a direct cont
-00010050: 7261 7374 206f 6620 7468 6520 7065 7266  rast of the perf
-00010060: 6f72 6d61 6e63 6520 666f 7220 7477 6f20  ormance for two 
-00010070: 6c65 6172 6e65 7273 2e0a 0a20 2020 2020  learners...     
-00010080: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00010090: 2020 2020 206c 313a 2054 6865 2066 6972       l1: The fir
-000100a0: 7374 2073 6574 206f 6620 7061 7261 6d65  st set of parame
-000100b0: 7465 7220 7661 6c75 6573 2077 6520 7761  ter values we wa
-000100c0: 6e74 2074 6f20 636f 6e74 7261 7374 2e0a  nt to contrast..
-000100d0: 2020 2020 2020 2020 2020 2020 6c32 3a20              l2: 
-000100e0: 5468 6520 7365 636f 6e64 2073 6574 206f  The second set o
-000100f0: 6620 7061 7261 6d65 7465 7220 7661 6c75  f parameter valu
-00010100: 6573 2077 6520 7761 6e74 2074 6f20 636f  es we want to co
-00010110: 6e74 7261 7374 2e0a 2020 2020 2020 2020  ntrast..        
-00010120: 2020 2020 783a 2054 6865 2076 616c 7565      x: The value
-00010130: 2074 6f20 706c 6f74 206f 6e20 7468 6520   to plot on the 
-00010140: 782d 6178 6973 2e20 5468 6973 2063 616e  x-axis. This can
-00010150: 2065 6974 6865 7220 6265 2069 6e64 6578   either be index
-00010160: 206f 7220 656e 7669 726f 6e6d 656e 7420   or environment 
-00010170: 636f 6c75 6d6e 7320 746f 2067 726f 7570  columns to group
-00010180: 2062 792e 0a20 2020 2020 2020 2020 2020   by..           
-00010190: 2079 3a20 5468 6520 7661 6c75 6520 746f   y: The value to
-000101a0: 2070 6c6f 7420 6f6e 2074 6865 2079 2d61   plot on the y-a
-000101b0: 7869 732e 0a20 2020 2020 2020 2020 2020  xis..           
-000101c0: 206c 3a20 5468 6520 6c65 7665 6c20 6174   l: The level at
-000101d0: 2077 6869 6368 2077 6520 7761 6e74 2074   which we want t
-000101e0: 6f20 636f 6e74 7261 7374 2e0a 2020 2020  o contrast..    
-000101f0: 2020 2020 2020 2020 703a 2054 6865 2070          p: The p
-00010200: 6169 7273 2074 6861 7420 6d75 7374 2065  airs that must e
-00010210: 7869 7374 2061 6372 6f73 7320 616c 6c20  xist across all 
-00010220: 636f 6d70 6172 6973 6f6e 206c 6576 656c  comparison level
-00010230: 7320 696e 206f 7264 6572 2074 6f20 6265  s in order to be
-00010240: 2069 6e63 6c75 6465 642e 0a20 2020 2020   included..     
-00010250: 2020 2020 2020 206d 6f64 653a 2027 6469         mode: 'di
-00010260: 6666 2720 2d2d 2070 6c6f 7420 7468 6520  ff' -- plot the 
-00010270: 7061 6972 7769 7365 2064 6966 6665 7265  pairwise differe
-00010280: 6e63 653b 2027 7072 6f62 2720 706c 6f74  nce; 'prob' plot
-00010290: 2074 6865 2070 726f 6261 6269 6c69 7479   the probability
-000102a0: 206f 6620 6c31 2062 6561 7469 6e67 206c   of l1 beating l
-000102b0: 322e 0a20 2020 2020 2020 2020 2020 2073  2..            s
-000102c0: 7061 6e3a 2054 6865 206e 756d 6265 7220  pan: The number 
-000102d0: 6f66 2079 2076 616c 7565 7320 746f 2073  of y values to s
-000102e0: 6d6f 6f74 6820 746f 6765 7468 6572 2077  mooth together w
-000102f0: 6865 6e20 7265 706f 7274 696e 6720 792e  hen reporting y.
-00010300: 2049 6620 7468 6973 2069 7320 4e6f 6e65   If this is None
-00010310: 2074 6865 6e20 7468 6520 6176 6572 6167   then the averag
-00010320: 6520 6f66 2061 6c6c 2079 0a20 2020 2020  e of all y.     
-00010330: 2020 2020 2020 2020 2020 2076 616c 7565             value
-00010340: 7320 7570 2074 6f20 6375 7272 656e 7420  s up to current 
-00010350: 6973 2073 686f 776e 206f 7468 6572 7769  is shown otherwi
-00010360: 7365 2061 206d 6f76 696e 6720 6176 6572  se a moving aver
-00010370: 6167 6520 7769 7468 2077 696e 646f 7720  age with window 
-00010380: 7369 7a65 206f 6620 7370 616e 2028 7468  size of span (th
-00010390: 6520 7769 6e64 6f77 2077 696c 6c20 6265  e window will be
-000103a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000103b0: 2073 6d61 6c6c 6572 2074 6861 6e20 7370   smaller than sp
-000103c0: 616e 2069 6e69 7469 616c 6c79 292e 0a20  an initially).. 
-000103d0: 2020 2020 2020 2020 2020 2065 7272 3a20             err: 
-000103e0: 5468 6973 2064 6574 6572 6d69 6e65 7320  This determines 
-000103f0: 7768 6174 206b 696e 6420 6f66 2065 7272  what kind of err
-00010400: 6f72 2062 6172 7320 746f 2070 6c6f 7420  or bars to plot 
-00010410: 2869 6620 616e 7929 2e20 4966 2060 4e6f  (if any). If `No
-00010420: 6e65 6020 7468 656e 206e 6f20 6261 7273  ne` then no bars
-00010430: 2061 7265 2070 6c6f 7474 6564 2c20 6966   are plotted, if
-00010440: 2027 7365 270a 2020 2020 2020 2020 2020   'se'.          
-00010450: 2020 2020 2020 7468 6520 7374 616e 6461        the standa
-00010460: 7264 2065 7272 6f72 2069 7320 7368 6f77  rd error is show
-00010470: 6e2c 2061 6e64 2069 6620 2773 6427 2074  n, and if 'sd' t
-00010480: 6865 2073 7461 6e64 6172 6420 6465 7669  he standard devi
-00010490: 6174 696f 6e20 6973 2073 686f 776e 2e0a  ation is shown..
-000104a0: 2020 2020 2020 2020 2020 2020 6572 7265              erre
-000104b0: 7665 7279 3a20 5468 6973 2064 6574 6572  very: This deter
-000104c0: 6d69 6e65 7320 7468 6520 6672 6571 7565  mines the freque
-000104d0: 6e63 7920 6f66 2065 7272 6f72 6261 7273  ncy of errorbars
-000104e0: 2e20 4966 2060 4e6f 6e65 6020 7468 6579  . If `None` they
-000104f0: 2061 7070 6561 7220 3525 206f 6620 7468   appear 5% of th
-00010500: 6520 7469 6d65 2e0a 2020 2020 2020 2020  e time..        
-00010510: 2020 2020 6c61 6265 6c73 3a20 5468 6520      labels: The 
-00010520: 6c65 6765 6e64 206c 6162 656c 7320 746f  legend labels to
-00010530: 2075 7365 2069 6e20 7468 6520 706c 6f74   use in the plot
-00010540: 2e20 5468 6573 6520 7368 6f75 6c64 2062  . These should b
-00010550: 6520 696e 206f 7264 6572 206f 6620 7468  e in order of th
-00010560: 6520 6163 7475 616c 206c 6567 656e 6420  e actual legend 
-00010570: 6c61 6265 6c73 2e0a 2020 2020 2020 2020  labels..        
-00010580: 2020 2020 7469 746c 6520 3a20 5468 6520      title : The 
-00010590: 7469 746c 6520 6769 7665 2074 6865 2070  title give the p
-000105a0: 6c6f 742e 0a20 2020 2020 2020 2020 2020  lot..           
-000105b0: 2063 6f6c 6f72 733a 2054 6865 2063 6f6c   colors: The col
-000105c0: 6f72 7320 7573 6564 2074 6f20 706c 6f74  ors used to plot
-000105d0: 2074 6865 206c 6561 726e 6572 7320 706c   the learners pl
-000105e0: 6f74 2e0a 2020 2020 2020 2020 2020 2020  ot..            
-000105f0: 786c 6162 656c 3a20 5468 6520 6c61 6265  xlabel: The labe
-00010600: 6c20 6f6e 2074 6865 2078 2d61 7869 732e  l on the x-axis.
-00010610: 0a20 2020 2020 2020 2020 2020 2079 6c61  .            yla
-00010620: 6265 6c3a 2054 6865 206c 6162 656c 206f  bel: The label o
-00010630: 6e20 7468 6520 792d 6178 6973 2e0a 2020  n the y-axis..  
-00010640: 2020 2020 2020 2020 2020 6c65 6765 6e64            legend
-00010650: 3a20 5768 6574 6865 7220 7468 6520 6c65  : Whether the le
-00010660: 6765 6e64 2066 6f72 2074 6865 2070 6c6f  gend for the plo
-00010670: 7420 7368 6f75 6c64 2062 6520 6472 6177  t should be draw
-00010680: 6e2e 0a20 2020 2020 2020 2020 2020 2061  n..            a
-00010690: 6c70 6861 3a20 5468 6520 6f70 6163 6974  lpha: The opacit
-000106a0: 7920 6f66 2064 7261 776e 2064 6174 612e  y of drawn data.
-000106b0: 0a20 2020 2020 2020 2020 2020 2078 6c69  .            xli
-000106c0: 6d3a 2044 6566 696e 6520 7468 6520 782d  m: Define the x-
-000106d0: 6178 6973 206c 696d 6974 7320 746f 2070  axis limits to p
-000106e0: 6c6f 742e 2049 6620 604e 6f6e 6560 2074  lot. If `None` t
-000106f0: 6865 2078 2d61 7869 7320 6c69 6d69 7473  he x-axis limits
-00010700: 2077 696c 6c20 6265 2069 6e66 6572 7265   will be inferre
-00010710: 642e 0a20 2020 2020 2020 2020 2020 2079  d..            y
-00010720: 6c69 6d3a 2044 6566 696e 6520 7468 6520  lim: Define the 
-00010730: 792d 6178 6973 206c 696d 6974 7320 746f  y-axis limits to
-00010740: 2070 6c6f 742e 2049 6620 604e 6f6e 6560   plot. If `None`
-00010750: 2074 6865 2079 2d61 7869 7320 6c69 6d69   the y-axis limi
-00010760: 7473 2077 696c 6c20 6265 2069 6e66 6572  ts will be infer
-00010770: 7265 642e 0a20 2020 2020 2020 2020 2020  red..           
-00010780: 2078 7469 636b 733a 2057 6865 7468 6572   xticks: Whether
-00010790: 2074 6865 2078 2d61 7869 7320 6c61 6265   the x-axis labe
-000107a0: 6c73 2073 686f 756c 6420 6265 2064 7261  ls should be dra
-000107b0: 776e 2e0a 2020 2020 2020 2020 2020 2020  wn..            
-000107c0: 7974 6963 6b73 3a20 5768 6574 6865 7220  yticks: Whether 
-000107d0: 7468 6520 792d 6178 6973 206c 6162 656c  the y-axis label
-000107e0: 7320 7368 6f75 6c64 2062 6520 6472 6177  s should be draw
-000107f0: 6e2e 0a20 2020 2020 2020 2020 2020 2078  n..            x
-00010800: 6f72 6465 723a 2049 6e64 6963 6174 6573  order: Indicates
-00010810: 2077 6865 7468 6572 2074 6865 2078 2d61   whether the x-a
-00010820: 7869 7320 7368 6f75 6c64 2062 6520 696e  xis should be in
-00010830: 2061 7363 656e 6469 6e67 2028 2b29 206f   ascending (+) o
-00010840: 7220 6465 7363 656e 6465 696e 6720 282d  r descendeing (-
-00010850: 2920 6f72 6465 722e 0a20 2020 2020 2020  ) order..       
-00010860: 2020 2020 2062 6f75 6e64 6172 793a 2057       boundary: W
-00010870: 6865 7468 6572 2077 6520 7761 6e74 2074  hether we want t
-00010880: 6f20 706c 6f74 2074 6865 2062 6f75 6e64  o plot the bound
-00010890: 6172 7920 6c69 6e65 2062 6574 7765 656e  ary line between
-000108a0: 2077 6869 6368 2073 6574 2069 7320 7468   which set is th
-000108b0: 6520 6265 7374 2070 6572 666f 726d 696e  e best performin
-000108c0: 672e 0a20 2020 2020 2020 2020 2020 206f  g..            o
-000108d0: 7574 3a20 496e 6469 6361 7465 2077 6865  ut: Indicate whe
-000108e0: 7265 2074 6865 2070 6c6f 7420 7368 6f75  re the plot shou
-000108f0: 6c64 2062 6520 7365 6e74 2074 6f20 6166  ld be sent to af
-00010900: 7465 7220 706c 6f74 7469 6e67 2069 7320  ter plotting is 
-00010910: 6669 6e69 7368 6564 2e20 5661 6c69 6420  finished. Valid 
-00010920: 7661 6c75 6573 2061 7265 0a20 2020 2020  values are.     
-00010930: 2020 2020 2020 2020 2020 2027 7363 7265             'scre
-00010940: 656e 2720 746f 2073 686f 7720 6974 206f  en' to show it o
-00010950: 6e20 7363 7265 656e 2c20 6120 7061 7468  n screen, a path
-00010960: 2074 6f20 7361 7665 2074 6f20 6469 736b   to save to disk
-00010970: 2c20 6f72 204e 6f6e 6520 6966 2074 6865  , or None if the
-00010980: 2070 6c6f 7420 7368 6f75 6c64 206e 6f74   plot should not
-00010990: 2062 650a 2020 2020 2020 2020 2020 2020   be.            
-000109a0: 2020 2020 6f75 7470 7574 2061 6e79 7768      output anywh
-000109b0: 6572 6520 2869 2e65 2e2c 206b 6570 7420  ere (i.e., kept 
-000109c0: 696e 206d 656d 6f72 7929 2069 6e20 6f72  in memory) in or
-000109d0: 6465 7220 746f 206b 6565 7020 6564 6974  der to keep edit
-000109e0: 696e 6720 7468 6520 706c 6f74 2061 6674  ing the plot aft
-000109f0: 6572 2074 6869 7320 6361 6c6c 2e0a 2020  er this call..  
-00010a00: 2020 2020 2020 2020 2020 6178 3a20 5072            ax: Pr
-00010a10: 6f76 6964 6520 616e 206f 7074 696f 6e61  ovide an optiona
-00010a20: 6c20 6178 6573 2074 6861 7420 7468 6520  l axes that the 
-00010a30: 706c 6f74 2077 696c 6c20 6265 2064 7261  plot will be dra
-00010a40: 776e 2074 6f2e 2049 6620 6e6f 7420 7072  wn to. If not pr
-00010a50: 6f76 6964 6564 2061 206e 6577 2066 6967  ovided a new fig
-00010a60: 7572 652f 6178 6573 2069 7320 6372 6561  ure/axes is crea
-00010a70: 7465 642e 0a20 2020 2020 2020 2022 2222  ted..        """
-00010a80: 0a0a 2020 2020 2020 2020 7472 793a 0a20  ..        try:. 
-00010a90: 2020 2020 2020 2020 2020 2078 6c69 6d20             xlim 
-00010aa0: 3d20 786c 696d 206f 7220 5b4e 6f6e 652c  = xlim or [None,
-00010ab0: 4e6f 6e65 5d0a 2020 2020 2020 2020 2020  None].          
-00010ac0: 2020 796c 696d 203d 2079 6c69 6d20 6f72    ylim = ylim or
-00010ad0: 205b 4e6f 6e65 2c4e 6f6e 655d 0a0a 2020   [None,None]..  
-00010ae0: 2020 2020 2020 2020 2020 7261 775f 6461            raw_da
-00010af0: 7461 203d 2073 656c 662e 7261 775f 636f  ta = self.raw_co
-00010b00: 6e74 7261 7374 286c 312c 6c32 2c78 2c79  ntrast(l1,l2,x,y
-00010b10: 2c6c 2c70 2c73 7061 6e29 0a0a 2020 2020  ,l,p,span)..    
-00010b20: 2020 2020 2020 2020 6c69 7374 5f6c 696b          list_lik
-00010b30: 653d 286c 6973 742c 7475 706c 6529 0a0a  e=(list,tuple)..
-00010b40: 2020 2020 2020 2020 2020 2020 6966 2020              if  
-00010b50: 2020 2069 7369 6e73 7461 6e63 6528 6c2c     isinstance(l,
-00010b60: 6c69 7374 5f6c 696b 6529 2061 6e64 206e  list_like) and n
-00010b70: 6f74 2069 7369 6e73 7461 6e63 6528 6c31  ot isinstance(l1
-00010b80: 5b30 5d2c 6c69 7374 5f6c 696b 6529 3a20  [0],list_like): 
-00010b90: 6c31 203d 205b 6c31 5d0a 2020 2020 2020  l1 = [l1].      
-00010ba0: 2020 2020 2020 6966 2020 2020 2069 7369        if     isi
-00010bb0: 6e73 7461 6e63 6528 6c2c 6c69 7374 5f6c  nstance(l,list_l
-00010bc0: 696b 6529 2061 6e64 206e 6f74 2069 7369  ike) and not isi
-00010bd0: 6e73 7461 6e63 6528 6c32 5b30 5d2c 6c69  nstance(l2[0],li
-00010be0: 7374 5f6c 696b 6529 3a20 6c32 203d 205b  st_like): l2 = [
-00010bf0: 6c32 5d0a 2020 2020 2020 2020 2020 2020  l2].            
-00010c00: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-00010c10: 6528 6c2c 6c69 7374 5f6c 696b 6529 2061  e(l,list_like) a
-00010c20: 6e64 206e 6f74 2069 7369 6e73 7461 6e63  nd not isinstanc
-00010c30: 6528 6c31 2020 202c 6c69 7374 5f6c 696b  e(l1   ,list_lik
-00010c40: 6529 3a20 6c31 203d 205b 6c31 5d0a 2020  e): l1 = [l1].  
-00010c50: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00010c60: 2069 7369 6e73 7461 6e63 6528 6c2c 6c69   isinstance(l,li
-00010c70: 7374 5f6c 696b 6529 2061 6e64 206e 6f74  st_like) and not
-00010c80: 2069 7369 6e73 7461 6e63 6528 6c32 2020   isinstance(l2  
-00010c90: 202c 6c69 7374 5f6c 696b 6529 3a20 6c32   ,list_like): l2
-00010ca0: 203d 205b 6c32 5d0a 0a20 2020 2020 2020   = [l2]..       
-00010cb0: 2020 2020 2063 6f6e 7472 6173 7465 7220       contraster 
-00010cc0: 3d20 286c 616d 6264 6120 743a 2074 5b31  = (lambda t: t[1
-00010cd0: 5d2d 745b 305d 2920 6966 206d 6f64 6520  ]-t[0]) if mode 
-00010ce0: 3d3d 2027 6469 6666 2720 656c 7365 2028  == 'diff' else (
-00010cf0: 6c61 6d62 6461 2074 3a20 696e 7428 2874  lambda t: int((t
-00010d00: 5b31 5d2d 745b 305d 293e 3029 2920 6966  [1]-t[0])>0)) if
-00010d10: 206d 6f64 653d 3d27 7072 6f62 2720 656c   mode=='prob' el
-00010d20: 7365 206d 6f64 650a 2020 2020 2020 2020  se mode.        
-00010d30: 2020 2020 5f62 6f75 6e64 6172 7920 203d      _boundary  =
-00010d40: 2030 2069 6620 6d6f 6465 203d 3d20 2764   0 if mode == 'd
-00010d50: 6966 6627 2065 6c73 6520 2e35 0a0a 2020  iff' else .5..  
-00010d60: 2020 2020 2020 2020 2020 6572 7265 7665            erreve
-00010d70: 7279 203d 2065 7272 6576 6572 7920 6f72  ry = errevery or
-00010d80: 206d 6178 2869 6e74 2872 6177 5f64 6174   max(int(raw_dat
-00010d90: 615b 2778 275d 5b2d 315d 2a30 2e30 3529  a['x'][-1]*0.05)
-00010da0: 2c31 2920 6966 2078 203d 3d20 2769 6e64  ,1) if x == 'ind
-00010db0: 6578 2720 656c 7365 2031 0a20 2020 2020  ex' else 1.     
-00010dc0: 2020 2020 2020 2073 7479 6c65 2020 2020         style    
-00010dd0: 3d20 222d 2220 6966 2078 203d 3d20 2769  = "-" if x == 'i
-00010de0: 6e64 6578 2720 656c 7365 2022 2e22 0a20  ndex' else ".". 
-00010df0: 2020 2020 2020 2020 2020 2065 7272 2020             err  
-00010e00: 2020 2020 3d20 7365 6c66 2e5f 636f 6e66      = self._conf
-00010e10: 6964 656e 6365 2865 7272 2c20 6572 7265  idence(err, erre
-00010e20: 7665 7279 290a 0a20 2020 2020 2020 2020  very)..         
-00010e30: 2020 2058 5f59 5f59 4520 3d20 5b5d 0a20     X_Y_YE = []. 
-00010e40: 2020 2020 2020 2020 2020 2066 6f72 205f             for _
-00010e50: 7869 2c20 285f 782c 2070 6169 7273 2920  xi, (_x, pairs) 
-00010e60: 696e 2065 6e75 6d65 7261 7465 2872 6177  in enumerate(raw
-00010e70: 5f64 6174 6129 3a0a 2020 2020 2020 2020  _data):.        
-00010e80: 2020 2020 2020 2020 585f 595f 5945 2e61          X_Y_YE.a
-00010e90: 7070 656e 6428 285f 782c 292b 6572 7228  ppend((_x,)+err(
-00010ea0: 6c69 7374 286d 6170 2863 6f6e 7472 6173  list(map(contras
-00010eb0: 7465 722c 7061 6972 7329 292c 5f78 6929  ter,pairs)),_xi)
-00010ec0: 290a 0a20 2020 2020 2020 2020 2020 206c  )..            l
-00010ed0: 315f 6c61 6265 6c2c 6c32 5f6c 6162 656c  1_label,l2_label
-00010ee0: 203d 2072 6177 5f64 6174 612e 636f 6c75   = raw_data.colu
-00010ef0: 6d6e 735b 315d 0a0a 2020 2020 2020 2020  mns[1]..        
-00010f00: 2020 2020 6966 2078 203d 3d20 2769 6e64      if x == 'ind
-00010f10: 6578 273a 0a20 2020 2020 2020 2020 2020  ex':.           
-00010f20: 2020 2020 2058 2c59 2c59 4520 3d20 7a69       X,Y,YE = zi
-00010f30: 7028 2a58 5f59 5f59 4529 0a20 2020 2020  p(*X_Y_YE).     
-00010f40: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-00010f50: 2020 3d20 7365 6c66 2e5f 6765 745f 636f    = self._get_co
-00010f60: 6c6f 7228 636f 6c6f 7273 2c20 2020 2020  lor(colors,     
-00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f80: 2020 2020 3029 0a20 2020 2020 2020 2020      0).         
-00010f90: 2020 2020 2020 2069 6620 6d6f 6465 203d         if mode =
-00010fa0: 3d20 2264 6966 6622 3a0a 2020 2020 2020  = "diff":.      
-00010fb0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-00010fc0: 6265 6c20 203d 2073 656c 662e 5f67 6574  bel  = self._get
-00010fd0: 5f6c 6162 656c 286c 6162 656c 732c 6627  _label(labels,f'
-00010fe0: 7b6c 325f 6c61 6265 6c7d 20e2 8094 207b  {l2_label} ... {
-00010ff0: 6c31 5f6c 6162 656c 7d27 2c30 290a 2020  l1_label}',0).  
-00011000: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00011010: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00011020: 2020 2020 2020 2020 6c61 6265 6c20 203d          label  =
-00011030: 2073 656c 662e 5f67 6574 5f6c 6162 656c   self._get_label
-00011040: 286c 6162 656c 732c 6627 505b 7b6c 325f  (labels,f'P[{l2_
-00011050: 6c61 6265 6c7d 203e 207b 6c31 5f6c 6162  label} > {l1_lab
-00011060: 656c 7d5d 272c 3029 0a0a 2020 2020 2020  el}]',0)..      
-00011070: 2020 2020 2020 2020 2020 6c61 6265 6c20            label 
-00011080: 203d 2066 227b 6c61 6265 6c7d 2220 6966   = f"{label}" if
-00011090: 206c 6567 656e 6420 656c 7365 204e 6f6e   legend else Non
-000110a0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-000110b0: 2020 6c69 6e65 7320 203d 205b 506f 696e    lines  = [Poin
-000110c0: 7473 2858 2c20 592c 204e 6f6e 652c 2059  ts(X, Y, None, Y
-000110d0: 452c 2073 7479 6c65 3d73 7479 6c65 2c20  E, style=style, 
-000110e0: 6c61 6265 6c3d 6c61 6265 6c2c 2063 6f6c  label=label, col
-000110f0: 6f72 3d63 6f6c 6f72 2c20 616c 7068 613d  or=color, alpha=
-00011100: 616c 7068 6129 5d0a 0a20 2020 2020 2020  alpha)]..       
-00011110: 2020 2020 2065 6c69 6620 7820 3d3d 206c       elif x == l
-00011120: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011130: 2020 6966 206c 656e 286c 3129 203e 2031    if len(l1) > 1
-00011140: 2061 6e64 206c 656e 286c 3229 203d 3d20   and len(l2) == 
-00011150: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-00011160: 2020 2020 2020 2023 536f 7274 2062 7920         #Sort by 
-00011170: 6c31 2e20 5765 2061 7373 756d 6520 5f78  l1. We assume _x
-00011180: 2069 7320 6622 7b6c 327d 2d7b 6c31 7d22   is f"{l2}-{l1}"
-00011190: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000111a0: 2020 2020 2020 6c32 5f6c 656e 203d 206c        l2_len = l
-000111b0: 656e 2873 7472 286c 325b 305d 2929 0a20  en(str(l2[0])). 
-000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111d0: 2020 206c 3120 3d20 6c69 7374 286d 6170     l1 = list(map
-000111e0: 2873 7472 2c6c 3129 290a 2020 2020 2020  (str,l1)).      
-000111f0: 2020 2020 2020 2020 2020 2020 2020 585f                X_
-00011200: 595f 5945 203d 2073 6f72 7465 6428 585f  Y_YE = sorted(X_
-00011210: 595f 5945 2c20 6b65 793d 6c61 6d62 6461  Y_YE, key=lambda
-00011220: 2069 7465 6d73 3a20 6c31 2e69 6e64 6578   items: l1.index
-00011230: 2869 7465 6d73 5b30 5d5b 6c32 5f6c 656e  (items[0][l2_len
-00011240: 2b31 3a5d 2929 0a20 2020 2020 2020 2020  +1:])).         
-00011250: 2020 2020 2020 2065 6c69 6620 6c65 6e28         elif len(
-00011260: 6c32 2920 3e20 3120 616e 6420 6c65 6e28  l2) > 1 and len(
-00011270: 6c31 2920 3d3d 2031 3a0a 2020 2020 2020  l1) == 1:.      
-00011280: 2020 2020 2020 2020 2020 2020 2020 2353                #S
-00011290: 6f72 7420 6279 206c 322e 2057 6520 6173  ort by l2. We as
-000112a0: 7375 6d65 205f 7820 6973 2066 227b 6c32  sume _x is f"{l2
-000112b0: 7d2d 7b6c 317d 222e 0a20 2020 2020 2020  }-{l1}"..       
-000112c0: 2020 2020 2020 2020 2020 2020 206c 315f               l1_
-000112d0: 6c65 6e20 3d20 6c65 6e28 7374 7228 6c31  len = len(str(l1
-000112e0: 5b30 5d29 290a 2020 2020 2020 2020 2020  [0])).          
-000112f0: 2020 2020 2020 2020 2020 6c32 203d 206c            l2 = l
-00011300: 6973 7428 6d61 7028 7374 722c 6c32 2929  ist(map(str,l2))
-00011310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011320: 2020 2020 2058 5f59 5f59 4520 3d20 736f       X_Y_YE = so
-00011330: 7274 6564 2858 5f59 5f59 452c 206b 6579  rted(X_Y_YE, key
-00011340: 3d6c 616d 6264 6120 6974 656d 733a 206c  =lambda items: l
-00011350: 322e 696e 6465 7828 6974 656d 735b 305d  2.index(items[0]
-00011360: 5b3a 2d28 6c31 5f6c 656e 2b31 295d 2929  [:-(l1_len+1)]))
-00011370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011380: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00011390: 2020 2020 2020 2020 2020 2058 5f59 5f59             X_Y_Y
-000113a0: 4520 3d20 736f 7274 6564 2858 5f59 5f59  E = sorted(X_Y_Y
-000113b0: 4529 0a0a 2020 2020 2020 2020 2020 2020  E)..            
-000113c0: 2020 2020 582c 592c 5945 203d 207a 6970      X,Y,YE = zip
-000113d0: 282a 585f 595f 5945 290a 2020 2020 2020  (*X_Y_YE).      
-000113e0: 2020 2020 2020 2020 2020 636f 6c6f 7220            color 
-000113f0: 203d 2073 656c 662e 5f67 6574 5f63 6f6c   = self._get_col
-00011400: 6f72 2863 6f6c 6f72 732c 2030 290a 2020  or(colors, 0).  
-00011410: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-00011420: 6e65 7320 203d 205b 506f 696e 7473 2858  nes  = [Points(X
-00011430: 2c20 592c 204e 6f6e 652c 2059 452c 2073  , Y, None, YE, s
-00011440: 7479 6c65 3d73 7479 6c65 2c20 6c61 6265  tyle=style, labe
-00011450: 6c3d 4e6f 6e65 2c20 636f 6c6f 723d 636f  l=None, color=co
-00011460: 6c6f 722c 2061 6c70 6861 3d61 6c70 6861  lor, alpha=alpha
-00011470: 295d 0a0a 2020 2020 2020 2020 2020 2020  )]..            
-00011480: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00011490: 2020 2020 2020 7570 7065 7220 3d20 6c61        upper = la
-000114a0: 6d62 6461 2079 2c79 653a 2079 2b79 655b  mbda y,ye: y+ye[
-000114b0: 315d 2069 6620 6973 696e 7374 616e 6365  1] if isinstance
-000114c0: 2879 652c 286c 6973 742c 7475 706c 6529  (ye,(list,tuple)
-000114d0: 2920 656c 7365 2079 2b79 650a 2020 2020  ) else y+ye.    
-000114e0: 2020 2020 2020 2020 2020 2020 6c6f 7765              lowe
-000114f0: 7220 3d20 6c61 6d62 6461 2079 2c79 653a  r = lambda y,ye:
-00011500: 2079 2d79 655b 305d 2069 6620 6973 696e   y-ye[0] if isin
-00011510: 7374 616e 6365 2879 652c 286c 6973 742c  stance(ye,(list,
-00011520: 7475 706c 6529 2920 656c 7365 2079 2d79  tuple)) else y-y
-00011530: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00011540: 2020 7072 6570 2020 3d20 6c61 6d62 6461    prep  = lambda
-00011550: 205f 783a 2073 7472 285f 7829 2069 6620   _x: str(_x) if 
-00011560: 6e6f 7420 786f 7264 6572 2065 6c73 6520  not xorder else 
-00011570: 5f78 0a0a 2020 2020 2020 2020 2020 2020  _x..            
-00011580: 2020 2020 2373 706c 6974 2069 6e74 6f20      #split into 
-00011590: 7769 6e2c 7469 652c 6c6f 7373 0a20 2020  win,tie,loss.   
-000115a0: 2020 2020 2020 2020 2020 2020 206c 315f               l1_
-000115b0: 7769 6e20 3d20 5b28 7072 6570 2878 292c  win = [(prep(x),
-000115c0: 792c 7965 2920 666f 7220 782c 792c 7965  y,ye) for x,y,ye
-000115d0: 2069 6e20 585f 595f 5945 2069 6620 7570   in X_Y_YE if up
-000115e0: 7065 7228 792c 7965 2920 3c20 205f 626f  per(y,ye) <  _bo
-000115f0: 756e 6461 7279 2020 2020 2020 2020 2020  undary          
-00011600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011610: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
-00011620: 2020 2020 206e 6f5f 7769 6e20 3d20 5b28       no_win = [(
-00011630: 7072 6570 2878 292c 792c 7965 2920 666f  prep(x),y,ye) fo
-00011640: 7220 782c 792c 7965 2069 6e20 585f 595f  r x,y,ye in X_Y_
-00011650: 5945 2069 6620 6c6f 7765 7228 792c 7965  YE if lower(y,ye
-00011660: 2920 3c3d 205f 626f 756e 6461 7279 2061  ) <= _boundary a
-00011670: 6e64 205f 626f 756e 6461 7279 203c 3d20  nd _boundary <= 
-00011680: 7570 7065 7228 792c 7965 295d 0a20 2020  upper(y,ye)].   
-00011690: 2020 2020 2020 2020 2020 2020 206c 325f               l2_
-000116a0: 7769 6e20 3d20 5b28 7072 6570 2878 292c  win = [(prep(x),
-000116b0: 792c 7965 2920 666f 7220 782c 792c 7965  y,ye) for x,y,ye
-000116c0: 2069 6e20 585f 595f 5945 2069 6620 2020   in X_Y_YE if   
-000116d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116e0: 2020 2020 2020 2020 2020 205f 626f 756e             _boun
-000116f0: 6461 7279 203c 2020 6c6f 7765 7228 792c  dary <  lower(y,
-00011700: 7965 295d 0a0a 2020 2020 2020 2020 2020  ye)]..          
-00011710: 2020 2020 2020 2373 6f72 7420 6279 206f        #sort by o
-00011720: 7264 6572 206f 6620 6d61 676e 6974 7564  rder of magnitud
-00011730: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00011740: 2020 6c31 5f77 696e 203d 2073 6f72 7465    l1_win = sorte
-00011750: 6428 6c31 5f77 696e 2c6b 6579 3d69 7465  d(l1_win,key=ite
-00011760: 6d67 6574 7465 7228 3129 290a 2020 2020  mgetter(1)).    
-00011770: 2020 2020 2020 2020 2020 2020 6e6f 5f77              no_w
-00011780: 696e 203d 2073 6f72 7465 6428 6e6f 5f77  in = sorted(no_w
-00011790: 696e 2c6b 6579 3d69 7465 6d67 6574 7465  in,key=itemgette
-000117a0: 7228 3129 290a 2020 2020 2020 2020 2020  r(1)).          
-000117b0: 2020 2020 2020 6c32 5f77 696e 203d 2073        l2_win = s
-000117c0: 6f72 7465 6428 6c32 5f77 696e 2c6b 6579  orted(l2_win,key
-000117d0: 3d69 7465 6d67 6574 7465 7228 3129 290a  =itemgetter(1)).
-000117e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000117f0: 206c 696e 6573 203d 205b 5d0a 0a20 2020   lines = []..   
-00011800: 2020 2020 2020 2020 2020 2020 2058 2c59               X,Y
-00011810: 2c59 4520 3d20 7a69 7028 2a6c 315f 7769  ,YE = zip(*l1_wi
-00011820: 6e29 2069 6620 6c31 5f77 696e 2065 6c73  n) if l1_win els
-00011830: 6520 2828 292c 2829 2c4e 6f6e 6529 0a20  e ((),(),None). 
-00011840: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00011850: 6f6c 6f72 2020 3d20 7365 6c66 2e5f 6765  olor  = self._ge
-00011860: 745f 636f 6c6f 7228 636f 6c6f 7273 2c20  t_color(colors, 
-00011870: 2020 2020 2020 2020 3029 0a20 2020 2020          0).     
-00011880: 2020 2020 2020 2020 2020 206c 6162 656c             label
-00011890: 2020 3d20 7365 6c66 2e5f 6765 745f 6c61    = self._get_la
-000118a0: 6265 6c28 6c61 6265 6c73 2c6c 315f 6c61  bel(labels,l1_la
-000118b0: 6265 6c2c 3029 0a20 2020 2020 2020 2020  bel,0).         
-000118c0: 2020 2020 2020 206c 6162 656c 2020 3d20         label  = 
-000118d0: 6622 7b6c 6162 656c 7d20 287b 6c65 6e28  f"{label} ({len(
-000118e0: 5829 7d29 2220 6966 206c 6567 656e 6420  X)})" if legend 
-000118f0: 656c 7365 204e 6f6e 650a 2020 2020 2020  else None.      
-00011900: 2020 2020 2020 2020 2020 6c69 6e65 732e            lines.
-00011910: 6170 7065 6e64 2850 6f69 6e74 7328 582c  append(Points(X,
-00011920: 2059 2c20 4e6f 6e65 2c20 5945 2c20 7374   Y, None, YE, st
-00011930: 796c 653d 7374 796c 652c 206c 6162 656c  yle=style, label
-00011940: 3d6c 6162 656c 2c20 636f 6c6f 723d 636f  =label, color=co
-00011950: 6c6f 722c 2061 6c70 6861 3d61 6c70 6861  lor, alpha=alpha
-00011960: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
-00011970: 2020 2020 582c 592c 5945 203d 207a 6970      X,Y,YE = zip
-00011980: 282a 6e6f 5f77 696e 2920 6966 206e 6f5f  (*no_win) if no_
-00011990: 7769 6e20 656c 7365 2028 2829 2c28 292c  win else ((),(),
-000119a0: 4e6f 6e65 290a 2020 2020 2020 2020 2020  None).          
-000119b0: 2020 2020 2020 636f 6c6f 7220 203d 2073        color  = s
-000119c0: 656c 662e 5f67 6574 5f63 6f6c 6f72 2863  elf._get_color(c
-000119d0: 6f6c 6f72 732c 2031 290a 2020 2020 2020  olors, 1).      
-000119e0: 2020 2020 2020 2020 2020 6c61 6265 6c20            label 
-000119f0: 203d 2027 5469 6527 0a20 2020 2020 2020   = 'Tie'.       
-00011a00: 2020 2020 2020 2020 206c 6162 656c 2020           label  
-00011a10: 3d20 6622 7b6c 6162 656c 7d20 287b 6c65  = f"{label} ({le
-00011a20: 6e28 5829 7d29 2220 6966 206c 6567 656e  n(X)})" if legen
-00011a30: 6420 656c 7365 204e 6f6e 650a 2020 2020  d else None.    
-00011a40: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-00011a50: 732e 6170 7065 6e64 2850 6f69 6e74 7328  s.append(Points(
-00011a60: 582c 2059 2c20 4e6f 6e65 2c20 5945 2c20  X, Y, None, YE, 
-00011a70: 7374 796c 653d 7374 796c 652c 206c 6162  style=style, lab
-00011a80: 656c 3d6c 6162 656c 2c20 636f 6c6f 723d  el=label, color=
-00011a90: 636f 6c6f 722c 2061 6c70 6861 3d61 6c70  color, alpha=alp
-00011aa0: 6861 2929 0a0a 2020 2020 2020 2020 2020  ha))..          
-00011ab0: 2020 2020 2020 582c 592c 5945 203d 207a        X,Y,YE = z
-00011ac0: 6970 282a 6c32 5f77 696e 2920 6966 206c  ip(*l2_win) if l
-00011ad0: 325f 7769 6e20 656c 7365 2028 2829 2c28  2_win else ((),(
-00011ae0: 292c 4e6f 6e65 290a 2020 2020 2020 2020  ),None).        
-00011af0: 2020 2020 2020 2020 636f 6c6f 7220 203d          color  =
-00011b00: 2073 656c 662e 5f67 6574 5f63 6f6c 6f72   self._get_color
-00011b10: 2863 6f6c 6f72 732c 2020 2020 2020 2020  (colors,        
-00011b20: 2032 290a 2020 2020 2020 2020 2020 2020   2).            
-00011b30: 2020 2020 6c61 6265 6c20 203d 2073 656c      label  = sel
-00011b40: 662e 5f67 6574 5f6c 6162 656c 286c 6162  f._get_label(lab
-00011b50: 656c 732c 6c32 5f6c 6162 656c 2c31 290a  els,l2_label,1).
-00011b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b70: 6c61 6265 6c20 203d 2066 227b 6c61 6265  label  = f"{labe
-00011b80: 6c7d 2028 7b6c 656e 2858 297d 2922 2069  l} ({len(X)})" i
-00011b90: 6620 6c65 6765 6e64 2065 6c73 6520 4e6f  f legend else No
-00011ba0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-00011bb0: 2020 206c 696e 6573 2e61 7070 656e 6428     lines.append(
-00011bc0: 506f 696e 7473 2858 2c20 592c 204e 6f6e  Points(X, Y, Non
-00011bd0: 652c 2059 452c 2073 7479 6c65 3d73 7479  e, YE, style=sty
-00011be0: 6c65 2c20 6c61 6265 6c3d 6c61 6265 6c2c  le, label=label,
-00011bf0: 2063 6f6c 6f72 3d63 6f6c 6f72 2c20 616c   color=color, al
-00011c00: 7068 613d 616c 7068 6129 290a 0a20 2020  pha=alpha))..   
-00011c10: 2020 2020 2020 2020 2078 726f 7461 7469           xrotati
-00011c20: 6f6e 203d 2039 3020 6966 2028 7820 213d  on = 90 if (x !=
-00011c30: 2027 696e 6465 7827 206f 7220 786f 7264   'index' or xord
-00011c40: 6572 2920 616e 6420 6c65 6e28 585f 595f  er) and len(X_Y_
-00011c50: 5945 293e 3520 656c 7365 2030 0a20 2020  YE)>5 else 0.   
-00011c60: 2020 2020 2020 2020 2079 726f 7461 7469           yrotati
-00011c70: 6f6e 203d 2030 0a0a 2020 2020 2020 2020  on = 0..        
-00011c80: 2020 2020 5f59 203d 2072 6177 5f64 6174      _Y = raw_dat
-00011c90: 615b 7261 775f 6461 7461 2e63 6f6c 756d  a[raw_data.colum
-00011ca0: 6e73 5b31 5d5d 5b30 5d0a 0a20 2020 2020  ns[1]][0]..     
-00011cb0: 2020 2020 2020 2078 6c61 6265 6c20 3d20         xlabel = 
-00011cc0: 786c 6162 656c 206f 7220 2822 496e 7465  xlabel or ("Inte
-00011cd0: 7261 6374 696f 6e22 2069 6620 783d 3d27  raction" if x=='
-00011ce0: 696e 6465 7827 2065 6c73 6520 785b 305d  index' else x[0]
-00011cf0: 2069 6620 6c65 6e28 7829 203d 3d20 3120   if len(x) == 1 
-00011d00: 656c 7365 2078 290a 2020 2020 2020 2020  else x).        
-00011d10: 2020 2020 796c 6162 656c 203d 2079 6c61      ylabel = yla
-00011d20: 6265 6c20 6f72 2028 6622 245c 4465 6c74  bel or (f"$\Delt
-00011d30: 6124 207b 797d 2220 6966 206d 6f64 653d  a$ {y}" if mode=
-00011d40: 3d22 6469 6666 2220 656c 7365 2066 2250  ="diff" else f"P
-00011d50: 2824 5c44 656c 7461 2420 7b79 7d20 3e20  ($\Delta$ {y} > 
-00011d60: 3029 2229 0a20 2020 2020 2020 2020 2020  0)").           
-00011d70: 2074 6974 6c65 2020 3d20 7469 746c 6520   title  = title 
-00011d80: 6966 2074 6974 6c65 2069 7320 6e6f 7420  if title is not 
-00011d90: 4e6f 6e65 2065 6c73 6520 2866 227b 796c  None else (f"{yl
-00011da0: 6162 656c 7d20 287b 6c65 6e28 5f59 297d  abel} ({len(_Y)}
-00011db0: 2045 6e76 6972 6f6e 6d65 6e74 7329 2229   Environments)")
-00011dc0: 0a0a 2020 2020 2020 2020 2020 2020 616c  ..            al
-00011dd0: 6c5f 7820 3d20 6469 6374 2e66 726f 6d6b  l_x = dict.fromk
-00011de0: 6579 7328 6368 6169 6e2e 6672 6f6d 5f69  eys(chain.from_i
-00011df0: 7465 7261 626c 6528 6c69 6e65 2e58 2066  terable(line.X f
-00011e00: 6f72 206c 696e 6520 696e 206c 696e 6573  or line in lines
-00011e10: 2929 0a20 2020 2020 2020 2020 2020 2078  )).            x
-00011e20: 6f72 6465 7265 6420 3d20 6c69 7374 2861  ordered = list(a
-00011e30: 6c6c 5f78 2e6b 6579 7328 2929 2069 6620  ll_x.keys()) if 
-00011e40: 6e6f 7420 786f 7264 6572 2065 6c73 6520  not xorder else 
-00011e50: 736f 7274 6564 2861 6c6c 5f78 2c20 7265  sorted(all_x, re
-00011e60: 7665 7273 653d 786f 7264 6572 3d3d 272d  verse=xorder=='-
-00011e70: 2729 0a0a 2020 2020 2020 2020 2020 2020  ')..            
-00011e80: 6966 2062 6f75 6e64 6172 793a 0a20 2020  if boundary:.   
-00011e90: 2020 2020 2020 2020 2020 2020 206c 696e               lin
-00011ea0: 6573 2e61 7070 656e 6428 506f 696e 7473  es.append(Points
-00011eb0: 2828 786f 7264 6572 6564 5b30 5d2c 786f  ((xordered[0],xo
-00011ec0: 7264 6572 6564 5b2d 315d 292c 285f 626f  rdered[-1]),(_bo
-00011ed0: 756e 6461 7279 2c5f 626f 756e 6461 7279  undary,_boundary
-00011ee0: 292c 204e 6f6e 652c 204e 6f6e 6520 2c20  ), None, None , 
-00011ef0: 2223 3838 3822 2c20 312c 204e 6f6e 652c  "#888", 1, None,
-00011f00: 2027 2d27 2c2e 3529 290a 0a20 2020 2020   '-',.5))..     
-00011f10: 2020 2020 2020 2069 6620 7820 3d3d 2027         if x == '
-00011f20: 696e 6465 7827 2061 6e64 2078 6f72 6465  index' and xorde
-00011f30: 7220 696e 205b 272b 272c 4e6f 6e65 5d3a  r in ['+',None]:
-00011f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011f50: 2078 6f72 6465 7265 6420 3d20 4e6f 6e65   xordered = None
-00011f60: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00011f70: 6c66 2e5f 706c 6f74 7465 722e 706c 6f74  lf._plotter.plot
-00011f80: 2861 782c 206c 696e 6573 2c20 7469 746c  (ax, lines, titl
-00011f90: 652c 2078 6c61 6265 6c2c 2079 6c61 6265  e, xlabel, ylabe
-00011fa0: 6c2c 2078 6c69 6d2c 2079 6c69 6d2c 2078  l, xlim, ylim, x
-00011fb0: 7469 636b 732c 2079 7469 636b 732c 206c  ticks, yticks, l
-00011fc0: 6567 656e 642c 2078 726f 7461 7469 6f6e  egend, xrotation
-00011fd0: 2c20 7972 6f74 6174 696f 6e2c 2078 6f72  , yrotation, xor
-00011fe0: 6465 7265 642c 206f 7574 290a 0a20 2020  dered, out)..   
-00011ff0: 2020 2020 2065 7863 6570 7420 436f 6261       except Coba
-00012000: 4578 6365 7074 696f 6e20 6173 2065 3a0a  Exception as e:.
-00012010: 2020 2020 2020 2020 2020 2020 436f 6261              Coba
-00012020: 436f 6e74 6578 742e 6c6f 6767 6572 2e6c  Context.logger.l
-00012030: 6f67 2873 7472 2865 2929 0a0a 2020 2020  og(str(e))..    
-00012040: 6465 6620 5f5f 7374 725f 5f28 7365 6c66  def __str__(self
-00012050: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-00012060: 2020 7265 7475 726e 2073 7472 287b 224c    return str({"L
-00012070: 6561 726e 6572 7322 3a20 6c65 6e28 7365  earners": len(se
-00012080: 6c66 2e5f 6c65 6172 6e65 7273 292c 2022  lf._learners), "
-00012090: 456e 7669 726f 6e6d 656e 7473 223a 206c  Environments": l
-000120a0: 656e 2873 656c 662e 5f65 6e76 6972 6f6e  en(self._environ
-000120b0: 6d65 6e74 7329 2c20 2249 6e74 6572 6163  ments), "Interac
-000120c0: 7469 6f6e 7322 3a20 6c65 6e28 7365 6c66  tions": len(self
-000120d0: 2e5f 696e 7465 7261 6374 696f 6e73 2920  ._interactions) 
-000120e0: 7d29 0a0a 2020 2020 6465 6620 5f5f 6571  })..    def __eq
-000120f0: 5f5f 2873 656c 662c 206f 3a20 6f62 6a65  __(self, o: obje
-00012100: 6374 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ct) -> bool:.   
-00012110: 2020 2020 2072 6574 7572 6e20 6973 696e       return isin
-00012120: 7374 616e 6365 286f 2c52 6573 756c 7429  stance(o,Result)
-00012130: 205c 0a20 2020 2020 2020 2020 2020 616e   \.           an
-00012140: 6420 6f2e 656e 7669 726f 6e6d 656e 7473  d o.environments
-00012150: 203d 3d20 7365 6c66 2e65 6e76 6972 6f6e   == self.environ
-00012160: 6d65 6e74 7320 5c0a 2020 2020 2020 2020  ments \.        
-00012170: 2020 2061 6e64 206f 2e6c 6561 726e 6572     and o.learner
-00012180: 7320 3d3d 2073 656c 662e 6c65 6172 6e65  s == self.learne
-00012190: 7273 205c 0a20 2020 2020 2020 2020 2020  rs \.           
-000121a0: 616e 6420 6f2e 6576 616c 7561 746f 7273  and o.evaluators
-000121b0: 203d 3d20 7365 6c66 2e65 7661 6c75 6174   == self.evaluat
-000121c0: 6f72 730a 0a20 2020 2064 6566 205f 6970  ors..    def _ip
-000121d0: 7974 686f 6e5f 6469 7370 6c61 795f 2873  ython_display_(s
-000121e0: 656c 6629 3a0a 2020 2020 2020 2020 2370  elf):.        #p
-000121f0: 7265 7474 7920 7072 696e 7420 696e 206a  retty print in j
-00012200: 7570 7974 6572 206e 6f74 6562 6f6f 6b20  upyter notebook 
-00012210: 2868 7474 7073 3a2f 2f69 7079 7468 6f6e  (https://ipython
-00012220: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00012230: 656e 2f73 7461 626c 652f 636f 6e66 6967  en/stable/config
-00012240: 2f69 6e74 6567 7261 7469 6e67 2e68 746d  /integrating.htm
-00012250: 6c29 0a20 2020 2020 2020 2070 7269 6e74  l).        print
-00012260: 2873 7472 2873 656c 6629 290a 0a20 2020  (str(self))..   
-00012270: 2064 6566 205f 6765 745f 636f 6c6f 7228   def _get_color(
-00012280: 7365 6c66 2c20 636f 6c6f 7273 3a55 6e69  self, colors:Uni
-00012290: 6f6e 5b4e 6f6e 652c 5365 7175 656e 6365  on[None,Sequence
-000122a0: 5b55 6e69 6f6e 5b73 7472 2c69 6e74 5d5d  [Union[str,int]]
-000122b0: 5d2c 2069 3a69 6e74 2920 2d3e 2055 6e69  ], i:int) -> Uni
-000122c0: 6f6e 5b73 7472 2c69 6e74 5d3a 0a20 2020  on[str,int]:.   
-000122d0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-000122e0: 2020 2020 2020 7265 7475 726e 2063 6f6c        return col
-000122f0: 6f72 7320 6966 2069 7369 6e73 7461 6e63  ors if isinstanc
-00012300: 6528 636f 6c6f 7273 2c73 7472 2920 656c  e(colors,str) el
-00012310: 7365 2063 6f6c 6f72 735b 695d 2069 6620  se colors[i] if 
-00012320: 636f 6c6f 7273 2065 6c73 6520 690a 2020  colors else i.  
-00012330: 2020 2020 2020 6578 6365 7074 2049 6e64        except Ind
-00012340: 6578 4572 726f 723a 0a20 2020 2020 2020  exError:.       
-00012350: 2020 2020 2072 6574 7572 6e20 692b 6d61       return i+ma
-00012360: 7828 636f 6c6f 7273 2920 6966 2069 7369  x(colors) if isi
-00012370: 6e73 7461 6e63 6528 636f 6c6f 7273 5b30  nstance(colors[0
-00012380: 5d2c 2869 6e74 2c66 6c6f 6174 2929 2065  ],(int,float)) e
-00012390: 6c73 6520 690a 2020 2020 2020 2020 6578  lse i.        ex
-000123a0: 6365 7074 2054 7970 6545 7272 6f72 3a0a  cept TypeError:.
-000123b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000123c0: 726e 2069 2b63 6f6c 6f72 730a 0a20 2020  rn i+colors..   
-000123d0: 2064 6566 205f 6765 745f 6c61 6265 6c28   def _get_label(
-000123e0: 7365 6c66 2c20 6c61 6265 6c73 3a53 6571  self, labels:Seq
-000123f0: 7565 6e63 655b 7374 725d 2c20 6c61 6265  uence[str], labe
-00012400: 6c3a 7374 722c 2069 3a69 6e74 2920 2d3e  l:str, i:int) ->
-00012410: 2073 7472 3a0a 2020 2020 2020 2020 7472   str:.        tr
-00012420: 793a 0a20 2020 2020 2020 2020 2020 206c  y:.            l
-00012430: 6162 656c 203d 206c 6162 656c 7320 6966  abel = labels if
-00012440: 2069 7369 6e73 7461 6e63 6528 6c61 6265   isinstance(labe
-00012450: 6c73 2c73 7472 2920 656c 7365 206c 6162  ls,str) else lab
-00012460: 656c 735b 695d 2069 6620 6c61 6265 6c73  els[i] if labels
-00012470: 2065 6c73 6520 6c61 6265 6c0a 2020 2020   else label.    
-00012480: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
-00012490: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-000124a0: 2020 2020 2072 6574 7572 6e20 7374 7228       return str(
-000124b0: 6c61 6265 6c29 0a0a 2020 2020 6465 6620  label)..    def 
-000124c0: 5f70 6c6f 7474 6162 6c65 2873 656c 662c  _plottable(self,
-000124d0: 2078 3a53 6571 7565 6e63 655b 7374 725d   x:Sequence[str]
-000124e0: 2c20 793a 7374 7229 202d 3e20 2752 6573  , y:str) -> 'Res
-000124f0: 756c 7427 3a0a 0a20 2020 2020 2020 2069  ult':..        i
-00012500: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-00012510: 2878 2c73 7472 2920 616e 6420 2769 6e64  (x,str) and 'ind
-00012520: 6578 2720 696e 2078 2061 6e64 206c 656e  ex' in x and len
-00012530: 2878 2920 3e20 313a 0a20 2020 2020 2020  (x) > 1:.       
-00012540: 2020 2020 2072 6169 7365 2043 6f62 6145       raise CobaE
-00012550: 7863 6570 7469 6f6e 2827 5468 6520 782d  xception('The x-
-00012560: 6178 6973 2063 616e 6e6f 7420 636f 6e74  axis cannot cont
-00012570: 6169 6e20 626f 7468 2069 6e64 6578 6573  ain both indexes
-00012580: 2061 6e64 2070 6172 616d 6574 6572 732e   and parameters.
-00012590: 2729 0a0a 2020 2020 2020 2020 6966 206c  ')..        if l
-000125a0: 656e 2873 656c 662e 696e 7465 7261 6374  en(self.interact
-000125b0: 696f 6e73 2920 3d3d 2030 3a0a 2020 2020  ions) == 0:.    
-000125c0: 2020 2020 2020 2020 7261 6973 6520 436f          raise Co
-000125d0: 6261 4578 6365 7074 696f 6e28 2254 6869  baException("Thi
-000125e0: 7320 7265 7375 6c74 2064 6f65 7320 6e6f  s result does no
-000125f0: 7420 636f 6e74 6169 6e20 616e 7920 6461  t contain any da
-00012600: 7461 2074 6f20 706c 6f74 2e22 290a 0a20  ta to plot.").. 
-00012610: 2020 2020 2020 2069 6620 7920 6e6f 7420         if y not 
-00012620: 696e 2073 656c 662e 696e 7465 7261 6374  in self.interact
-00012630: 696f 6e73 2e63 6f6c 756d 6e73 3a0a 2020  ions.columns:.  
-00012640: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00012650: 436f 6261 4578 6365 7074 696f 6e28 6622  CobaException(f"
-00012660: 5468 6973 2072 6573 756c 7420 646f 6573  This result does
-00012670: 206e 6f74 2063 6f6e 7461 696e 2063 6f6c   not contain col
-00012680: 756d 6e20 277b 797d 2720 696e 2069 6e74  umn '{y}' in int
-00012690: 6572 6163 7469 6f6e 732e 2229 0a0a 2020  eractions.")..  
-000126a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000126b0: 660a 0a20 2020 2064 6566 205f 6669 6e69  f..    def _fini
-000126c0: 7368 6564 2873 656c 662c 2078 3a53 6571  shed(self, x:Seq
-000126d0: 7565 6e63 655b 7374 725d 2c20 793a 7374  uence[str], y:st
-000126e0: 722c 206c 3a53 6571 7565 6e63 655b 7374  r, l:Sequence[st
-000126f0: 725d 2c20 703a 5365 7175 656e 6365 5b73  r], p:Sequence[s
-00012700: 7472 5d29 202d 3e20 2752 6573 756c 7427  tr]) -> 'Result'
-00012710: 3a0a 2020 2020 2020 2020 6f6e 6c79 5f66  :.        only_f
-00012720: 696e 6973 6865 6420 3d20 7365 6c66 2e5f  inished = self._
-00012730: 6669 6c74 6572 5f66 696e 2827 6d69 6e27  filter_fin('min'
-00012740: 2069 6620 7820 3d3d 2027 696e 6465 7827   if x == 'index'
-00012750: 2065 6c73 6520 4e6f 6e65 2c20 6c2c 2070   else None, l, p
-00012760: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
-00012770: 286f 6e6c 795f 6669 6e69 7368 6564 2e6c  (only_finished.l
-00012780: 6561 726e 6572 7329 203d 3d20 303a 0a20  earners) == 0:. 
-00012790: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000127a0: 2043 6f62 6145 7863 6570 7469 6f6e 2866   CobaException(f
-000127b0: 2254 6869 7320 7265 7375 6c74 2064 6f65  "This result doe
-000127c0: 7320 6e6f 7420 636f 6e74 6169 6e20 6120  s not contain a 
-000127d0: 7b70 7d20 7468 6174 2068 6173 2062 6565  {p} that has bee
-000127e0: 6e20 6669 6e69 7368 6564 2066 6f72 2065  n finished for e
-000127f0: 7665 7279 207b 6c7d 2e22 290a 2020 2020  very {l}.").    
-00012800: 2020 2020 7265 7475 726e 206f 6e6c 795f      return only_
-00012810: 6669 6e69 7368 6564 0a0a 2020 2020 6465  finished..    de
-00012820: 6620 5f63 6f6e 6669 6465 6e63 6528 7365  f _confidence(se
-00012830: 6c66 2c20 6572 723a 2055 6e69 6f6e 5b73  lf, err: Union[s
-00012840: 7472 2c50 6f69 6e74 416e 6449 6e74 6572  tr,PointAndInter
-00012850: 7661 6c5d 2c20 6572 7265 7665 7279 3a69  val], errevery:i
-00012860: 6e74 203d 2031 293a 0a0a 2020 2020 2020  nt = 1):..      
-00012870: 2020 6966 2065 7272 203d 3d20 2773 6527    if err == 'se'
-00012880: 3a0a 2020 2020 2020 2020 2020 2020 6369  :.            ci
-00012890: 203d 2053 7464 4572 7243 4928 2e39 3529   = StdErrCI(.95)
-000128a0: 0a20 2020 2020 2020 2065 6c69 6620 6572  .        elif er
-000128b0: 7220 3d3d 2027 6273 273a 0a20 2020 2020  r == 'bs':.     
-000128c0: 2020 2020 2020 2063 6920 3d20 426f 6f74         ci = Boot
-000128d0: 7374 7261 7043 4928 2e39 352c 206d 6561  strapCI(.95, mea
-000128e0: 6e29 0a20 2020 2020 2020 2065 6c69 6620  n).        elif 
-000128f0: 6572 7220 3d3d 2027 6269 273a 0a20 2020  err == 'bi':.   
-00012900: 2020 2020 2020 2020 2063 6920 3d20 4269           ci = Bi
-00012910: 6e6f 6d69 616c 4349 2827 7769 6c73 6f6e  nomialCI('wilson
-00012920: 2729 0a20 2020 2020 2020 2065 6c69 6620  ').        elif 
-00012930: 6572 7220 3d3d 2027 7364 273a 0a20 2020  err == 'sd':.   
-00012940: 2020 2020 2020 2020 2063 6920 3d20 5374           ci = St
-00012950: 6444 6576 4349 2829 0a20 2020 2020 2020  dDevCI().       
-00012960: 2065 6c69 6620 6572 7220 6973 204e 6f6e   elif err is Non
-00012970: 6520 6f72 2069 7369 6e73 7461 6e63 6528  e or isinstance(
-00012980: 6572 722c 7374 7229 3a0a 2020 2020 2020  err,str):.      
-00012990: 2020 2020 2020 6369 203d 204e 6f6e 650a        ci = None.
-000129a0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000129b0: 2020 2020 2020 2020 2020 6369 203d 2065            ci = e
-000129c0: 7272 0a0a 2020 2020 2020 2020 6465 6620  rr..        def 
-000129d0: 6361 6c63 5f63 6928 5a3a 5365 7175 656e  calc_ci(Z:Sequen
-000129e0: 6365 5b66 6c6f 6174 5d2c 2069 3a69 6e74  ce[float], i:int
-000129f0: 203d 202d 3129 3a0a 2020 2020 2020 2020   = -1):.        
-00012a00: 2020 2020 6966 2063 6920 6973 204e 6f6e      if ci is Non
-00012a10: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00012a20: 2020 2072 6574 7572 6e20 286d 6561 6e28     return (mean(
-00012a30: 5a29 2c30 290a 2020 2020 2020 2020 2020  Z),0).          
-00012a40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00012a50: 2020 2020 2020 2020 736b 6970 5f65 7272          skip_err
-00012a60: 203d 2028 692b 3129 2565 7272 6576 6572   = (i+1)%errever
-00012a70: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-00012a80: 2020 7265 7475 726e 2028 6369 2e70 6f69    return (ci.poi
-00012a90: 6e74 285a 292c 2028 302c 3029 2920 6966  nt(Z), (0,0)) if
-00012aa0: 2073 6b69 705f 6572 7220 656c 7365 2063   skip_err else c
-00012ab0: 692e 706f 696e 745f 696e 7465 7276 616c  i.point_interval
-00012ac0: 285a 290a 0a20 2020 2020 2020 2072 6574  (Z)..        ret
-00012ad0: 7572 6e20 6361 6c63 5f63 690a 0a20 2020  urn calc_ci..   
-00012ae0: 2064 6566 205f 6772 6f75 7065 645f 7973   def _grouped_ys
-00012af0: 2873 656c 662c 202a 6b65 7973 3a20 7374  (self, *keys: st
-00012b00: 722c 2079 3a4f 7074 696f 6e61 6c5b 7374  r, y:Optional[st
-00012b10: 725d 2c20 6675 6e63 3a20 4c69 7465 7261  r], func: Litera
-00012b20: 6c5b 276c 6173 7427 2c27 6c69 7374 275d  l['last','list']
-00012b30: 203d 204e 6f6e 652c 2063 6172 643a 204c   = None, card: L
-00012b40: 6974 6572 616c 5b27 4727 2c27 5327 5d20  iteral['G','S'] 
-00012b50: 3d20 2747 272c 2073 7061 6e3a 4f70 7469  = 'G', span:Opti
-00012b60: 6f6e 616c 5b69 6e74 5d3d 3129 202d 3e20  onal[int]=1) -> 
-00012b70: 5365 7175 656e 6365 5b54 7570 6c65 5d3a  Sequence[Tuple]:
-00012b80: 0a0a 2020 2020 2020 2020 656e 765f 6361  ..        env_ca
-00012b90: 6368 6520 3d20 7365 6c66 2e5f 656e 765f  che = self._env_
-00012ba0: 6361 6368 650a 2020 2020 2020 2020 6c72  cache.        lr
-00012bb0: 6e5f 6361 6368 6520 3d20 7365 6c66 2e5f  n_cache = self._
-00012bc0: 6c72 6e5f 6361 6368 650a 2020 2020 2020  lrn_cache.      
-00012bd0: 2020 7661 6c5f 6361 6368 6520 3d20 7365    val_cache = se
-00012be0: 6c66 2e5f 7661 6c5f 6361 6368 650a 0a20  lf._val_cache.. 
-00012bf0: 2020 2020 2020 206e 6565 645f 6861 7368         need_hash
-00012c00: 6572 203d 204e 6f6e 650a 0a20 2020 2020  er = None..     
-00012c10: 2020 2044 203d 2064 6963 7428 2920 6966     D = dict() if
-00012c20: 2063 6172 6420 3d3d 2027 5327 2065 6c73   card == 'S' els
-00012c30: 6520 6465 6661 756c 7464 6963 7428 6c69  e defaultdict(li
-00012c40: 7374 290a 0a20 2020 2020 2020 2064 6566  st)..        def
-00012c50: 2069 735f 6963 6f6c 286b 6579 293a 0a20   is_icol(key):. 
-00012c60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00012c70: 6e20 6b65 7920 6e6f 7420 696e 205b 2765  n key not in ['e
-00012c80: 6e76 6972 6f6e 6d65 6e74 5f69 6427 2c27  nvironment_id','
-00012c90: 6c65 6172 6e65 725f 6964 272c 2765 7661  learner_id','eva
-00012ca0: 6c75 6174 6f72 5f69 6427 5d20 616e 6420  luator_id'] and 
-00012cb0: 6b65 7920 696e 2073 656c 662e 696e 7465  key in self.inte
-00012cc0: 7261 6374 696f 6e73 2e63 6f6c 756d 6e73  ractions.columns
-00012cd0: 0a0a 2020 2020 2020 2020 6465 6620 6765  ..        def ge
-00012ce0: 745f 6963 6f6c 7328 6b65 7973 293a 0a20  t_icols(keys):. 
-00012cf0: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-00012d00: 6579 2069 6e20 6b65 7973 3a0a 2020 2020  ey in keys:.    
-00012d10: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00012d20: 7369 6e73 7461 6e63 6528 6b65 792c 286c  sinstance(key,(l
-00012d30: 6973 742c 7475 706c 6529 293a 0a20 2020  ist,tuple)):.   
-00012d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d50: 2079 6965 6c64 2066 726f 6d20 6765 745f   yield from get_
-00012d60: 6963 6f6c 7328 6b65 7929 0a20 2020 2020  icols(key).     
-00012d70: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00012d80: 6973 5f69 636f 6c28 6b65 7929 3a0a 2020  is_icol(key):.  
-00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012da0: 2020 7969 656c 6420 6b65 790a 0a20 2020    yield key..   
-00012db0: 2020 2020 2064 6566 206d 616b 655f 6765       def make_ge
-00012dc0: 7473 2863 6f6c 7329 3a0a 2020 2020 2020  ts(cols):.      
-00012dd0: 2020 2020 2020 666f 7220 636f 6c20 696e        for col in
-00012de0: 2063 6f6c 733a 0a20 2020 2020 2020 2020   cols:.         
-00012df0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00012e00: 616e 6365 2863 6f6c 2c28 7475 706c 652c  ance(col,(tuple,
-00012e10: 6c69 7374 2929 3a0a 2020 2020 2020 2020  list)):.        
-00012e20: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
-00012e30: 6420 6c61 6d62 6461 2065 2c6c 2c76 2c73  d lambda e,l,v,s
-00012e40: 2c4e 2c47 3d6c 6973 7428 6d61 6b65 5f67  ,N,G=list(make_g
-00012e50: 6574 7328 636f 6c29 293a 207a 6970 282a  ets(col)): zip(*
-00012e60: 6d61 7028 6d65 7468 6f64 6361 6c6c 6572  map(methodcaller
-00012e70: 2827 5f5f 6361 6c6c 5f5f 272c 652c 6c2c  ('__call__',e,l,
-00012e80: 762c 732c 4e29 2c47 2929 2069 6620 4e20  v,s,N),G)) if N 
-00012e90: 213d 2030 2065 6c73 6520 7475 706c 6528  != 0 else tuple(
-00012ea0: 6d61 7028 6d65 7468 6f64 6361 6c6c 6572  map(methodcaller
-00012eb0: 2827 5f5f 6361 6c6c 5f5f 272c 652c 6c2c  ('__call__',e,l,
-00012ec0: 762c 732c 4e29 2c47 2929 0a20 2020 2020  v,s,N),G)).     
-00012ed0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00012ee0: 636f 6c20 696e 2073 656c 662e 656e 7669  col in self.envi
-00012ef0: 726f 6e6d 656e 7473 2e63 6f6c 756d 6e73  ronments.columns
-00012f00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012f10: 2020 2020 2020 7969 656c 6420 6c61 6d62        yield lamb
-00012f20: 6461 2065 2c6c 2c76 2c73 2c4e 2c63 6f6c  da e,l,v,s,N,col
-00012f30: 3d63 6f6c 3a20 7265 7065 6174 2865 5b63  =col: repeat(e[c
-00012f40: 6f6c 5d2c 4e29 2069 6620 4e20 213d 2030  ol],N) if N != 0
-00012f50: 2065 6c73 6520 655b 636f 6c5d 0a20 2020   else e[col].   
-00012f60: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00012f70: 6620 636f 6c20 696e 2073 656c 662e 6c65  f col in self.le
-00012f80: 6172 6e65 7273 2e63 6f6c 756d 6e73 206f  arners.columns o
-00012f90: 7220 636f 6c20 3d3d 2027 6675 6c6c 5f6e  r col == 'full_n
-00012fa0: 616d 6527 3a0a 2020 2020 2020 2020 2020  ame':.          
-00012fb0: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
-00012fc0: 6c61 6d62 6461 2065 2c6c 2c76 2c73 2c4e  lambda e,l,v,s,N
-00012fd0: 2c63 6f6c 3d63 6f6c 3a20 7265 7065 6174  ,col=col: repeat
-00012fe0: 286c 5b63 6f6c 5d2c 4e29 2069 6620 4e20  (l[col],N) if N 
-00012ff0: 213d 2030 2065 6c73 6520 6c5b 636f 6c5d  != 0 else l[col]
-00013000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013010: 2065 6c69 6620 636f 6c20 696e 2073 656c   elif col in sel
-00013020: 662e 6576 616c 7561 746f 7273 2e63 6f6c  f.evaluators.col
-00013030: 756d 6e73 3a0a 2020 2020 2020 2020 2020  umns:.          
-00013040: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
-00013050: 6c61 6d62 6461 2065 2c6c 2c76 2c73 2c4e  lambda e,l,v,s,N
-00013060: 2c63 6f6c 3d63 6f6c 3a20 7265 7065 6174  ,col=col: repeat
-00013070: 2876 5b63 6f6c 5d2c 4e29 2069 6620 4e20  (v[col],N) if N 
-00013080: 213d 2030 2065 6c73 6520 765b 636f 6c5d  != 0 else v[col]
-00013090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000130a0: 2065 6c69 6620 636f 6c20 696e 2073 656c   elif col in sel
-000130b0: 662e 696e 7465 7261 6374 696f 6e73 2e63  f.interactions.c
-000130c0: 6f6c 756d 6e73 3a0a 2020 2020 2020 2020  olumns:.        
-000130d0: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
-000130e0: 6420 6c61 6d62 6461 2065 2c6c 2c76 2c73  d lambda e,l,v,s
-000130f0: 2c4e 2c63 6f6c 3d63 6f6c 3a20 6974 6572  ,N,col=col: iter
-00013100: 2873 2e70 6f70 2829 290a 0a20 2020 2020  (s.pop())..     
-00013110: 2020 2067 6574 7320 203d 206c 6973 7428     gets  = list(
-00013120: 6d61 6b65 5f67 6574 7328 6b65 7973 2929  make_gets(keys))
-00013130: 0a20 2020 2020 2020 2069 636f 6c73 203d  .        icols =
-00013140: 206c 6973 7428 6765 745f 6963 6f6c 7328   list(get_icols(
-00013150: 6b65 7973 2929 0a20 2020 2020 2020 2069  keys)).        i
-00013160: 636f 6c73 2e72 6576 6572 7365 2829 0a0a  cols.reverse()..
-00013170: 2020 2020 2020 2020 6966 2079 3a20 6963          if y: ic
-00013180: 6f6c 7320 2b3d 205b 795d 0a20 2020 2020  ols += [y].     
-00013190: 2020 2066 6f72 2028 6569 642c 6c69 642c     for (eid,lid,
-000131a0: 7669 6429 2c20 7365 6c20 696e 2073 656c  vid), sel in sel
-000131b0: 662e 696e 7465 7261 6374 696f 6e73 2e67  f.interactions.g
-000131c0: 726f 7570 6279 2833 2c69 636f 6c73 293a  roupby(3,icols):
-000131d0: 0a0a 2020 2020 2020 2020 2020 2020 656e  ..            en
-000131e0: 7620 3d20 656e 765f 6361 6368 655b 6569  v = env_cache[ei
-000131f0: 645d 0a20 2020 2020 2020 2020 2020 206c  d].            l
-00013200: 726e 203d 206c 726e 5f63 6163 6865 5b6c  rn = lrn_cache[l
-00013210: 6964 5d0a 2020 2020 2020 2020 2020 2020  id].            
-00013220: 7661 6c20 3d20 7661 6c5f 6361 6368 655b  val = val_cache[
-00013230: 7669 645d 0a0a 2020 2020 2020 2020 2020  vid]..          
-00013240: 2020 5920 3d20 7365 6c2e 706f 7028 2920    Y = sel.pop() 
-00013250: 6966 2079 2065 6c73 6520 4e6f 6e65 0a20  if y else None. 
-00013260: 2020 2020 2020 2020 2020 204e 203d 2030             N = 0
-00013270: 2069 6620 6e6f 7420 7365 6c20 656c 7365   if not sel else
-00013280: 206c 656e 2873 656c 5b30 5d29 0a0a 2020   len(sel[0])..  
-00013290: 2020 2020 2020 2020 2020 6f75 7473 203d            outs =
-000132a0: 2074 7570 6c65 286d 6170 286d 6574 686f   tuple(map(metho
-000132b0: 6463 616c 6c65 7228 275f 5f63 616c 6c5f  dcaller('__call_
-000132c0: 5f27 2c65 6e76 2c6c 726e 2c76 616c 2c73  _',env,lrn,val,s
-000132d0: 656c 2c4e 292c 6765 7473 2929 0a0a 2020  el,N),gets))..  
-000132e0: 2020 2020 2020 2020 2020 6966 204e 2021            if N !
-000132f0: 3d20 303a 206f 7574 7320 3d20 7a69 7028  = 0: outs = zip(
-00013300: 2a6f 7574 7329 0a20 2020 2020 2020 2020  *outs).         
-00013310: 2020 2069 6620 4e20 3d3d 2030 2061 6e64     if N == 0 and
-00013320: 2066 756e 6320 6973 204e 6f6e 6520 616e   func is None an
-00013330: 6420 7920 6973 206e 6f74 204e 6f6e 653a  d y is not None:
-00013340: 2066 756e 6320 3d20 276c 6173 7427 0a0a   func = 'last'..
-00013350: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00013360: 6565 645f 6861 7368 6572 2069 7320 4e6f  eed_hasher is No
-00013370: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00013380: 2020 2020 6f75 742c 206f 7574 7320 3d20      out, outs = 
-00013390: 286f 7574 732c 206f 7574 7329 2069 6620  (outs, outs) if 
-000133a0: 4e20 3d3d 2030 2065 6c73 6520 7065 656b  N == 0 else peek
-000133b0: 5f66 6972 7374 286f 7574 7329 0a20 2020  _first(outs).   
-000133c0: 2020 2020 2020 2020 2020 2020 206e 6565               nee
-000133d0: 645f 6861 7368 6572 203d 2074 7279 5f65  d_hasher = try_e
-000133e0: 6c73 6528 6c61 6d62 6461 3a20 6e6f 7420  lse(lambda: not 
-000133f0: 626f 6f6c 2868 6173 6828 6f75 7429 292c  bool(hash(out)),
-00013400: 2054 7275 6529 0a20 2020 2020 2020 2020   True).         
-00013410: 2020 2020 2020 2069 6620 6e65 6564 5f68         if need_h
-00013420: 6173 6865 723a 0a20 2020 2020 2020 2020  asher:.         
-00013430: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00013440: 2043 6f62 6145 7863 6570 7469 6f6e 2822   CobaException("
-00013450: 5265 7375 6c74 2072 6571 7569 7265 7320  Result requires 
-00013460: 616c 6c20 6461 7461 2074 6f20 6265 2068  all data to be h
-00013470: 6173 6861 626c 652e 2229 0a0a 2020 2020  ashable.")..    
-00013480: 2020 2020 2020 2020 6966 204e 203d 3d20          if N == 
-00013490: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-000134a0: 2020 2069 6620 7920 6973 204e 6f6e 653a     if y is None:
-000134b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000134c0: 2020 2020 2076 203d 204e 6f6e 650a 2020       v = None.  
-000134d0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000134e0: 6966 2066 756e 6320 3d3d 2027 6c61 7374  if func == 'last
-000134f0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-00013500: 2020 2020 2020 2076 203d 2059 5b2d 315d         v = Y[-1]
-00013510: 2069 6620 7370 616e 203d 3d20 3120 656c   if span == 1 el
-00013520: 7365 206d 6561 6e28 595b 2d73 7061 6e3a  se mean(Y[-span:
-00013530: 5d29 2069 6620 7370 616e 2065 6c73 6520  ]) if span else 
-00013540: 6d65 616e 2859 290a 2020 2020 2020 2020  mean(Y).        
-00013550: 2020 2020 2020 2020 656c 6966 2066 756e          elif fun
-00013560: 6320 3d3d 2027 6c69 7374 273a 0a20 2020  c == 'list':.   
-00013570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013580: 2076 203d 2059 0a20 2020 2020 2020 2020   v = Y.         
-00013590: 2020 2020 2020 2069 6620 6361 7264 203d         if card =
-000135a0: 3d20 2747 273a 0a20 2020 2020 2020 2020  = 'G':.         
-000135b0: 2020 2020 2020 2020 2020 2044 5b6f 7574             D[out
-000135c0: 735d 2e61 7070 656e 6428 7629 0a20 2020  s].append(v).   
-000135d0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000135e0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000135f0: 2020 2020 2020 2044 5b6f 7574 735d 203d         D[outs] =
-00013600: 2076 0a20 2020 2020 2020 2020 2020 2065   v.            e
-00013610: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00013620: 2020 2020 2069 6620 7920 6973 204e 6f6e       if y is Non
-00013630: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00013640: 2020 2020 2020 2076 203d 2072 6570 6561         v = repea
-00013650: 7428 4e6f 6e65 290a 2020 2020 2020 2020  t(None).        
-00013660: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00013670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013680: 2020 7620 3d20 6d6f 7669 6e67 5f61 7665    v = moving_ave
-00013690: 7261 6765 2859 2c73 7061 6e29 0a20 2020  rage(Y,span).   
-000136a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000136b0: 6361 7264 203d 3d20 2747 273a 0a20 2020  card == 'G':.   
-000136c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136d0: 2066 6f72 206f 2c79 5f20 696e 207a 6970   for o,y_ in zip
-000136e0: 286f 7574 732c 7629 3a0a 2020 2020 2020  (outs,v):.      
-000136f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013700: 2020 445b 6f5d 2e61 7070 656e 6428 795f    D[o].append(y_
-00013710: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00013720: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00013730: 2020 2020 2020 2020 2020 2020 442e 7570              D.up
-00013740: 6461 7465 287a 6970 286f 7574 732c 7629  date(zip(outs,v)
-00013750: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00013760: 6e20 5b6b 202b 2028 762c 2920 666f 7220  n [k + (v,) for 
-00013770: 6b2c 7620 696e 2044 2e69 7465 6d73 2829  k,v in D.items()
-00013780: 5d0a 0a20 2020 2064 6566 205f 676c 6f62  ]..    def _glob
-00013790: 616c 5f6e 2873 656c 662c 206e 3a20 556e  al_n(self, n: Un
-000137a0: 696f 6e5b 696e 742c 4c69 7465 7261 6c5b  ion[int,Literal[
-000137b0: 276d 696e 275d 5d29 3a0a 0a20 2020 2020  'min']]):..     
-000137c0: 2020 2065 6e76 6972 6f6e 6d65 6e74 7320     environments 
-000137d0: 3d20 7365 6c66 2e65 6e76 6972 6f6e 6d65  = self.environme
-000137e0: 6e74 730a 2020 2020 2020 2020 6c65 6172  nts.        lear
-000137f0: 6e65 7273 2020 2020 203d 2073 656c 662e  ners     = self.
-00013800: 6c65 6172 6e65 7273 0a20 2020 2020 2020  learners.       
-00013810: 2065 7661 6c75 6174 6f72 7320 2020 3d20   evaluators   = 
-00013820: 7365 6c66 2e65 7661 6c75 6174 6f72 730a  self.evaluators.
-00013830: 2020 2020 2020 2020 696e 7465 7261 6374          interact
-00013840: 696f 6e73 203d 2073 656c 662e 696e 7465  ions = self.inte
-00013850: 7261 6374 696f 6e73 0a0a 2020 2020 2020  ractions..      
-00013860: 2020 656e 765f 6c65 6e67 7468 7320 3d20    env_lengths = 
-00013870: 5b5d 0a20 2020 2020 2020 2074 6f5f 6472  [].        to_dr
-00013880: 6f70 2020 2020 203d 205b 5d0a 2020 2020  op     = [].    
-00013890: 2020 2020 746f 5f6b 6565 7020 2020 2020      to_keep     
-000138a0: 3d20 5b5d 0a20 2020 2020 2020 2069 6620  = [].        if 
-000138b0: 6e20 3d3d 2027 6d69 6e27 3a0a 2020 2020  n == 'min':.    
-000138c0: 2020 2020 2020 2020 666f 7220 656e 765f          for env_
-000138d0: 6964 782c 2065 6e76 5f6c 656e 2069 6e20  idx, env_len in 
-000138e0: 7365 6c66 2e69 6e74 6572 6163 7469 6f6e  self.interaction
-000138f0: 732e 6772 6f75 7062 7928 332c 2763 6f75  s.groupby(3,'cou
-00013900: 6e74 2729 3a0a 2020 2020 2020 2020 2020  nt'):.          
-00013910: 2020 2020 2020 656e 765f 6c65 6e67 7468        env_length
-00013920: 732e 6170 7065 6e64 2865 6e76 5f6c 656e  s.append(env_len
-00013930: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00013940: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00013950: 656e 765f 6964 782c 2065 6e76 5f6c 656e  env_idx, env_len
-00013960: 2069 6e20 7365 6c66 2e69 6e74 6572 6163   in self.interac
-00013970: 7469 6f6e 732e 6772 6f75 7062 7928 332c  tions.groupby(3,
-00013980: 2763 6f75 6e74 2729 3a0a 2020 2020 2020  'count'):.      
-00013990: 2020 2020 2020 2020 2020 6966 2065 6e76            if env
-000139a0: 5f6c 656e 203c 206e 3a0a 2020 2020 2020  _len < n:.      
-000139b0: 2020 2020 2020 2020 2020 2020 2020 746f                to
-000139c0: 5f64 726f 702e 6170 7065 6e64 2865 6e76  _drop.append(env
-000139d0: 5f69 6478 290a 2020 2020 2020 2020 2020  _idx).          
-000139e0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000139f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a00: 656e 765f 6c65 6e67 7468 732e 6170 7065  env_lengths.appe
-00013a10: 6e64 2865 6e76 5f6c 656e 290a 2020 2020  nd(env_len).    
-00013a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a30: 746f 5f6b 6565 702e 6170 7065 6e64 2865  to_keep.append(e
-00013a40: 6e76 5f69 6478 290a 0a20 2020 2020 2020  nv_idx)..       
-00013a50: 2069 6620 746f 5f64 726f 703a 0a20 2020   if to_drop:.   
-00013a60: 2020 2020 2020 2020 206e 5f64 726f 7070           n_dropp
-00013a70: 6564 203d 206c 656e 2874 6f5f 6472 6f70  ed = len(to_drop
-00013a80: 290a 2020 2020 2020 2020 2020 2020 696e  ).            in
-00013a90: 7465 7261 6374 696f 6e73 203d 2054 6162  teractions = Tab
-00013aa0: 6c65 2856 6965 7728 696e 7465 7261 6374  le(View(interact
-00013ab0: 696f 6e73 2e5f 6461 7461 2c73 656c 662e  ions._data,self.
-00013ac0: 5f72 656d 6f76 6528 746f 5f64 726f 702c  _remove(to_drop,
-00013ad0: 6e29 292c 2069 6e74 6572 6163 7469 6f6e  n)), interaction
-00013ae0: 732e 636f 6c75 6d6e 732c 2069 6e74 6572  s.columns, inter
-00013af0: 6163 7469 6f6e 732e 696e 6465 7865 7329  actions.indexes)
-00013b00: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00013b10: 6e5f 6472 6f70 7065 643d 3d31 3a20 436f  n_dropped==1: Co
-00013b20: 6261 436f 6e74 6578 742e 6c6f 6767 6572  baContext.logger
-00013b30: 2e6c 6f67 2866 2257 6520 7265 6d6f 7665  .log(f"We remove
-00013b40: 6420 7b6e 5f64 726f 7070 6564 7d20 6c65  d {n_dropped} le
-00013b50: 6172 6e65 7220 6576 616c 7561 7469 6f6e  arner evaluation
-00013b60: 2062 6563 6175 7365 2069 7420 7761 7320   because it was 
-00013b70: 7368 6f72 7465 7220 7468 616e 207b 6e7d  shorter than {n}
-00013b80: 2069 6e74 6572 6163 7469 6f6e 732e 2229   interactions.")
-00013b90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00013ba0: 6e5f 6472 6f70 7065 643e 3d32 3a20 436f  n_dropped>=2: Co
-00013bb0: 6261 436f 6e74 6578 742e 6c6f 6767 6572  baContext.logger
-00013bc0: 2e6c 6f67 2866 2257 6520 7265 6d6f 7665  .log(f"We remove
-00013bd0: 6420 7b6e 5f64 726f 7070 6564 7d20 6c65  d {n_dropped} le
-00013be0: 6172 6e65 7220 6576 616c 7561 7469 6f6e  arner evaluation
-00013bf0: 7320 6265 6361 7573 6520 7468 6579 2077  s because they w
-00013c00: 6572 6520 7368 6f72 7465 7220 7468 616e  ere shorter than
-00013c10: 207b 6e7d 2069 6e74 6572 6163 7469 6f6e   {n} interaction
-00013c20: 732e 2229 0a0a 2020 2020 2020 2020 656e  s.")..        en
-00013c30: 765f 6c65 6e67 7468 7320 3d20 636f 6c6c  v_lengths = coll
-00013c40: 6563 7469 6f6e 732e 436f 756e 7465 7228  ections.Counter(
-00013c50: 656e 765f 6c65 6e67 7468 7329 0a20 2020  env_lengths).   
-00013c60: 2020 2020 2073 686f 7274 656e 5f74 6f20       shorten_to 
-00013c70: 3d20 6d69 6e28 656e 765f 6c65 6e67 7468  = min(env_length
-00013c80: 7329 2069 6620 6e3d 3d27 6d69 6e27 2061  s) if n=='min' a
-00013c90: 6e64 2065 6e76 5f6c 656e 6774 6873 2065  nd env_lengths e
-00013ca0: 6c73 6520 6e0a 2020 2020 2020 2020 6966  lse n.        if
-00013cb0: 206c 656e 2865 6e76 5f6c 656e 6774 6873   len(env_lengths
-00013cc0: 2920 3e20 3120 6f72 2065 6e76 5f6c 656e  ) > 1 or env_len
-00013cd0: 6774 6873 2e76 616c 7565 7328 2920 213d  gths.values() !=
-00013ce0: 207b 7368 6f72 7465 6e5f 746f 7d3a 0a20   {shorten_to}:. 
-00013cf0: 2020 2020 2020 2020 2020 206e 5f73 686f             n_sho
-00013d00: 7274 656e 6564 203d 2073 756d 2876 2066  rtened = sum(v f
-00013d10: 6f72 206b 2c76 2069 6e20 656e 765f 6c65  or k,v in env_le
-00013d20: 6e67 7468 732e 6974 656d 7328 2920 6966  ngths.items() if
-00013d30: 206b 203e 2073 686f 7274 656e 5f74 6f29   k > shorten_to)
-00013d40: 0a20 2020 2020 2020 2020 2020 2069 6e74  .            int
-00013d50: 6572 6163 7469 6f6e 7320 3d20 696e 7465  eractions = inte
-00013d60: 7261 6374 696f 6e73 2e77 6865 7265 2869  ractions.where(i
-00013d70: 6e64 6578 3d7b 273c 3d27 3a73 686f 7274  ndex={'<=':short
-00013d80: 656e 5f74 6f7d 2920 232e 340a 2020 2020  en_to}) #.4.    
-00013d90: 2020 2020 2020 2020 6966 206e 5f73 686f          if n_sho
-00013da0: 7274 656e 6564 3d3d 313a 2043 6f62 6143  rtened==1: CobaC
-00013db0: 6f6e 7465 7874 2e6c 6f67 6765 722e 6c6f  ontext.logger.lo
-00013dc0: 6728 6622 5765 2073 686f 7274 656e 6564  g(f"We shortened
-00013dd0: 207b 6e5f 7368 6f72 7465 6e65 647d 206c   {n_shortened} l
-00013de0: 6561 726e 6572 2065 7661 6c75 6174 696f  earner evaluatio
-00013df0: 6e20 6265 6361 7573 6520 6974 2077 6173  n because it was
-00013e00: 206c 6f6e 6765 7220 7468 616e 2074 6865   longer than the
-00013e10: 2073 686f 7274 6573 7420 656e 7669 726f   shortest enviro
-00013e20: 6e6d 656e 742e 2229 0a20 2020 2020 2020  nment.").       
-00013e30: 2020 2020 2069 6620 6e5f 7368 6f72 7465       if n_shorte
-00013e40: 6e65 643e 3d32 3a20 436f 6261 436f 6e74  ned>=2: CobaCont
-00013e50: 6578 742e 6c6f 6767 6572 2e6c 6f67 2866  ext.logger.log(f
-00013e60: 2257 6520 7368 6f72 7465 6e65 6420 7b6e  "We shortened {n
-00013e70: 5f73 686f 7274 656e 6564 7d20 6c65 6172  _shortened} lear
-00013e80: 6e65 7220 6576 616c 7561 7469 6f6e 7320  ner evaluations 
-00013e90: 6265 6361 7573 6520 7468 6579 2077 6572  because they wer
-00013ea0: 6520 6c6f 6e67 6572 2074 6861 6e20 7468  e longer than th
-00013eb0: 6520 7368 6f72 7465 7374 2065 6e76 6972  e shortest envir
-00013ec0: 6f6e 6d65 6e74 2e22 290a 0a20 2020 2020  onment.")..     
-00013ed0: 2020 206b 6565 705f 656e 7673 2c6b 6565     keep_envs,kee
-00013ee0: 705f 6c72 6e73 2c6b 6565 705f 7661 6c73  p_lrns,keep_vals
-00013ef0: 203d 206d 6170 2873 6574 2c7a 6970 282a   = map(set,zip(*
-00013f00: 746f 5f6b 6565 7029 2920 6966 2074 6f5f  to_keep)) if to_
-00013f10: 6b65 6570 2065 6c73 6520 285b 5d2c 5b5d  keep else ([],[]
-00013f20: 2c5b 5d29 0a0a 2020 2020 2020 2020 6966  ,[])..        if
-00013f30: 2074 6f5f 6472 6f70 2061 6e64 206c 656e   to_drop and len
-00013f40: 286b 6565 705f 656e 7673 2920 213d 206c  (keep_envs) != l
-00013f50: 656e 2865 6e76 6972 6f6e 6d65 6e74 7329  en(environments)
-00013f60: 3a0a 2020 2020 2020 2020 2020 2020 656e  :.            en
-00013f70: 7669 726f 6e6d 656e 7473 203d 2065 6e76  vironments = env
-00013f80: 6972 6f6e 6d65 6e74 732e 7768 6572 6528  ironments.where(
-00013f90: 656e 7669 726f 6e6d 656e 745f 6964 3d6b  environment_id=k
-00013fa0: 6565 705f 656e 7673 290a 0a20 2020 2020  eep_envs)..     
-00013fb0: 2020 2069 6620 746f 5f64 726f 7020 616e     if to_drop an
-00013fc0: 6420 6c65 6e28 6b65 6570 5f6c 726e 7329  d len(keep_lrns)
-00013fd0: 2021 3d20 6c65 6e28 6c65 6172 6e65 7273   != len(learners
-00013fe0: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
-00013ff0: 6561 726e 6572 7320 3d20 6c65 6172 6e65  earners = learne
-00014000: 7273 2e77 6865 7265 286c 6561 726e 6572  rs.where(learner
-00014010: 5f69 643d 6b65 6570 5f6c 726e 7329 0a0a  _id=keep_lrns)..
-00014020: 2020 2020 2020 2020 6966 2074 6f5f 6472          if to_dr
-00014030: 6f70 2061 6e64 206c 656e 286b 6565 705f  op and len(keep_
-00014040: 7661 6c73 2920 213d 206c 656e 2865 7661  vals) != len(eva
-00014050: 6c75 6174 6f72 7329 3a0a 2020 2020 2020  luators):.      
-00014060: 2020 2020 2020 6576 616c 7561 746f 7273        evaluators
-00014070: 203d 2065 7661 6c75 6174 6f72 732e 7768   = evaluators.wh
-00014080: 6572 6528 6576 616c 7561 746f 725f 6964  ere(evaluator_id
-00014090: 3d6b 6565 705f 7661 6c73 290a 0a20 2020  =keep_vals)..   
-000140a0: 2020 2020 2072 6574 7572 6e20 5265 7375       return Resu
-000140b0: 6c74 2865 6e76 6972 6f6e 6d65 6e74 732c  lt(environments,
-000140c0: 206c 6561 726e 6572 732c 2065 7661 6c75   learners, evalu
-000140d0: 6174 6f72 732c 2069 6e74 6572 6163 7469  ators, interacti
-000140e0: 6f6e 732c 2073 656c 662e 6578 7065 7269  ons, self.experi
-000140f0: 6d65 6e74 290a 0a20 2020 2064 6566 205f  ment)..    def _
-00014100: 6772 6f75 705f 7028 7365 6c66 2c20 6c3a  group_p(self, l:
-00014110: 556e 696f 6e5b 7374 722c 2053 6571 7565  Union[str, Seque
-00014120: 6e63 655b 7374 725d 5d2c 2070 3a55 6e69  nce[str]], p:Uni
-00014130: 6f6e 5b73 7472 2c20 5365 7175 656e 6365  on[str, Sequence
-00014140: 5b73 7472 5d5d 293a 0a0a 2020 2020 2020  [str]]):..      
-00014150: 2020 656e 7669 726f 6e6d 656e 7473 203d    environments =
-00014160: 2073 656c 662e 656e 7669 726f 6e6d 656e   self.environmen
-00014170: 7473 0a20 2020 2020 2020 206c 6561 726e  ts.        learn
-00014180: 6572 7320 2020 2020 3d20 7365 6c66 2e6c  ers     = self.l
-00014190: 6561 726e 6572 730a 2020 2020 2020 2020  earners.        
-000141a0: 6576 616c 7561 746f 7273 2020 203d 2073  evaluators   = s
-000141b0: 656c 662e 6576 616c 7561 746f 7273 0a20  elf.evaluators. 
-000141c0: 2020 2020 2020 2069 6e74 6572 6163 7469         interacti
-000141d0: 6f6e 7320 3d20 7365 6c66 2e69 6e74 6572  ons = self.inter
-000141e0: 6163 7469 6f6e 730a 0a20 2020 2020 2020  actions..       
-000141f0: 2069 6e64 6578 6573 2020 3d20 6c69 7374   indexes  = list
-00014200: 2873 656c 662e 5f67 726f 7570 6564 5f79  (self._grouped_y
-00014210: 7328 702c 6c2c 2765 6e76 6972 6f6e 6d65  s(p,l,'environme
-00014220: 6e74 5f69 6427 2c27 6c65 6172 6e65 725f  nt_id','learner_
-00014230: 6964 272c 2765 7661 6c75 6174 6f72 5f69  id','evaluator_i
-00014240: 6427 2c79 3d4e 6f6e 652c 6361 7264 3d27  d',y=None,card='
-00014250: 5327 2929 0a20 2020 2020 2020 206e 5f6c  S')).        n_l
-00014260: 6576 656c 7320 3d20 6c65 6e28 7365 7428  evels = len(set(
-00014270: 6d61 7028 6974 656d 6765 7474 6572 2831  map(itemgetter(1
-00014280: 292c 696e 6465 7865 7329 2929 0a0a 2020  ),indexes)))..  
-00014290: 2020 2020 2020 746f 5f6b 6565 702c 2074        to_keep, t
-000142a0: 6f5f 7265 6d6f 7665 2c20 6e5f 6c61 7267  o_remove, n_larg
-000142b0: 6572 2c20 6e5f 736d 616c 6c65 7220 3d20  er, n_smaller = 
-000142c0: 5b5d 2c20 5b5d 2c20 302c 2030 0a20 2020  [], [], 0, 0.   
-000142d0: 2020 2020 2066 6f72 205f 2c20 6772 6f75       for _, grou
-000142e0: 7020 696e 2067 726f 7570 6279 2869 6e64  p in groupby(ind
-000142f0: 6578 6573 2c6b 6579 3d69 7465 6d67 6574  exes,key=itemget
-00014300: 7465 7228 3029 293a 0a20 2020 2020 2020  ter(0)):.       
-00014310: 2020 2020 2067 726f 7570 203d 206c 6973       group = lis
-00014320: 7428 6772 6f75 7029 0a20 2020 2020 2020  t(group).       
-00014330: 2020 2020 2069 6620 6c65 6e28 6772 6f75       if len(grou
-00014340: 7029 203e 206e 5f6c 6576 656c 733a 0a20  p) > n_levels:. 
-00014350: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00014360: 5f6c 6172 6765 7220 2b3d 2031 0a20 2020  _larger += 1.   
-00014370: 2020 2020 2020 2020 2020 2020 2074 6f5f               to_
-00014380: 7265 6d6f 7665 2e65 7874 656e 6428 675b  remove.extend(g[
-00014390: 323a 355d 2066 6f72 2067 2069 6e20 6772  2:5] for g in gr
-000143a0: 6f75 7029 0a20 2020 2020 2020 2020 2020  oup).           
-000143b0: 2065 6c69 6620 6c65 6e28 6772 6f75 7029   elif len(group)
-000143c0: 203c 206e 5f6c 6576 656c 733a 0a20 2020   < n_levels:.   
-000143d0: 2020 2020 2020 2020 2020 2020 206e 5f73               n_s
-000143e0: 6d61 6c6c 6572 202b 3d20 310a 2020 2020  maller += 1.    
-000143f0: 2020 2020 2020 2020 2020 2020 746f 5f72              to_r
-00014400: 656d 6f76 652e 6578 7465 6e64 2867 5b32  emove.extend(g[2
-00014410: 3a35 5d20 666f 7220 6720 696e 2067 726f  :5] for g in gro
-00014420: 7570 290a 2020 2020 2020 2020 2020 2020  up).            
-00014430: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00014440: 2020 2020 2020 746f 5f6b 6565 702e 6578        to_keep.ex
-00014450: 7465 6e64 2867 5b32 3a35 5d20 666f 7220  tend(g[2:5] for 
-00014460: 6720 696e 2067 726f 7570 290a 0a20 2020  g in group)..   
-00014470: 2020 2020 2069 6620 6e5f 6c61 7267 6572       if n_larger
-00014480: 3a0a 2020 2020 2020 2020 2020 2020 436f  :.            Co
-00014490: 6261 436f 6e74 6578 742e 6c6f 6767 6572  baContext.logger
-000144a0: 2e6c 6f67 2866 2257 6520 7265 6d6f 7665  .log(f"We remove
-000144b0: 6420 7b6e 5f6c 6172 6765 727d 207b 707d  d {n_larger} {p}
-000144c0: 2062 6563 6175 7365 206d 6f72 6520 7468   because more th
-000144d0: 616e 206f 6e65 2065 7869 7374 6564 2066  an one existed f
-000144e0: 6f72 2065 6163 6820 7b6c 7d2e 2229 0a0a  or each {l}.")..
-000144f0: 2020 2020 2020 2020 6966 206e 5f73 6d61          if n_sma
-00014500: 6c6c 6572 3a0a 2020 2020 2020 2020 2020  ller:.          
-00014510: 2020 436f 6261 436f 6e74 6578 742e 6c6f    CobaContext.lo
-00014520: 6767 6572 2e6c 6f67 2866 2257 6520 7265  gger.log(f"We re
-00014530: 6d6f 7665 6420 7b6e 5f73 6d61 6c6c 6572  moved {n_smaller
-00014540: 7d20 7b70 7d20 6265 6361 7573 6520 7b27  } {p} because {'
-00014550: 7468 6579 2720 6966 206e 5f73 6d61 6c6c  they' if n_small
-00014560: 6572 3e31 2065 6c73 6520 2769 7427 7d20  er>1 else 'it'} 
-00014570: 6469 6420 6e6f 7420 6578 6973 7420 666f  did not exist fo
-00014580: 7220 6576 6572 7920 7b6c 7d2e 2229 0a0a  r every {l}.")..
-00014590: 2020 2020 2020 2020 6966 2074 6f5f 7265          if to_re
-000145a0: 6d6f 7665 3a0a 2020 2020 2020 2020 2020  move:.          
-000145b0: 2020 7365 6c65 6374 203d 2073 656c 662e    select = self.
-000145c0: 5f72 656d 6f76 6528 746f 5f72 656d 6f76  _remove(to_remov
-000145d0: 6529 0a20 2020 2020 2020 2020 2020 2069  e).            i
-000145e0: 6e74 6572 6163 7469 6f6e 7320 3d20 5461  nteractions = Ta
-000145f0: 626c 6528 5669 6577 2869 6e74 6572 6163  ble(View(interac
-00014600: 7469 6f6e 732e 5f64 6174 612c 7365 6c65  tions._data,sele
-00014610: 6374 292c 2069 6e74 6572 6163 7469 6f6e  ct), interaction
-00014620: 732e 636f 6c75 6d6e 732c 2069 6e74 6572  s.columns, inter
-00014630: 6163 7469 6f6e 732e 696e 6465 7865 7329  actions.indexes)
-00014640: 0a0a 2020 2020 2020 2020 655f 6b65 6570  ..        e_keep
-00014650: 2c6c 5f6b 6565 702c 765f 6b65 6570 203d  ,l_keep,v_keep =
-00014660: 206d 6170 2873 6574 2c7a 6970 282a 746f   map(set,zip(*to
-00014670: 5f6b 6565 7029 2920 6966 2074 6f5f 6b65  _keep)) if to_ke
-00014680: 6570 2065 6c73 6520 285b 5d2c 5b5d 2c5b  ep else ([],[],[
-00014690: 5d29 0a20 2020 2020 2020 2069 6620 6c65  ]).        if le
-000146a0: 6e28 655f 6b65 6570 2920 213d 206c 656e  n(e_keep) != len
-000146b0: 2865 6e76 6972 6f6e 6d65 6e74 7329 3a20  (environments): 
-000146c0: 656e 7669 726f 6e6d 656e 7473 203d 2065  environments = e
-000146d0: 6e76 6972 6f6e 6d65 6e74 732e 7768 6572  nvironments.wher
-000146e0: 6528 656e 7669 726f 6e6d 656e 745f 6964  e(environment_id
-000146f0: 3d65 5f6b 6565 7029 0a20 2020 2020 2020  =e_keep).       
-00014700: 2069 6620 6c65 6e28 6c5f 6b65 6570 2920   if len(l_keep) 
-00014710: 213d 206c 656e 286c 6561 726e 6572 7329  != len(learners)
-00014720: 2020 2020 3a20 6c65 6172 6e65 7273 2020      : learners  
-00014730: 2020 203d 206c 6561 726e 6572 7320 2020     = learners   
-00014740: 202e 7768 6572 6528 6c65 6172 6e65 725f   .where(learner_
-00014750: 6964 2020 2020 3d6c 5f6b 6565 7029 0a20  id    =l_keep). 
-00014760: 2020 2020 2020 2069 6620 6c65 6e28 765f         if len(v_
-00014770: 6b65 6570 2920 213d 206c 656e 2865 7661  keep) != len(eva
-00014780: 6c75 6174 6f72 7329 2020 3a20 6576 616c  luators)  : eval
-00014790: 7561 746f 7273 2020 203d 2065 7661 6c75  uators   = evalu
-000147a0: 6174 6f72 7320 202e 7768 6572 6528 6576  ators  .where(ev
-000147b0: 616c 7561 746f 725f 6964 2020 3d76 5f6b  aluator_id  =v_k
-000147c0: 6565 7029 0a0a 2020 2020 2020 2020 7265  eep)..        re
-000147d0: 7475 726e 2052 6573 756c 7428 656e 7669  turn Result(envi
-000147e0: 726f 6e6d 656e 7473 2c20 6c65 6172 6e65  ronments, learne
-000147f0: 7273 2c20 6576 616c 7561 746f 7273 2c20  rs, evaluators, 
-00014800: 696e 7465 7261 6374 696f 6e73 2c20 7365  interactions, se
-00014810: 6c66 2e65 7870 6572 696d 656e 7429 0a0a  lf.experiment)..
-00014820: 2020 2020 6465 6620 5f66 696c 7465 725f      def _filter_
-00014830: 6669 6e28 7365 6c66 2c0a 2020 2020 2020  fin(self,.      
-00014840: 2020 6e3a 2055 6e69 6f6e 5b69 6e74 2c4c    n: Union[int,L
-00014850: 6974 6572 616c 5b27 6d69 6e27 5d2c 204e  iteral['min'], N
-00014860: 6f6e 655d 2c0a 2020 2020 2020 2020 6c3a  one],.        l:
-00014870: 2055 6e69 6f6e 5b73 7472 2c20 5365 7175   Union[str, Sequ
-00014880: 656e 6365 5b73 7472 5d2c 204e 6f6e 655d  ence[str], None]
-00014890: 2c0a 2020 2020 2020 2020 703a 2055 6e69  ,.        p: Uni
-000148a0: 6f6e 5b73 7472 2c20 5365 7175 656e 6365  on[str, Sequence
-000148b0: 5b73 7472 5d2c 204e 6f6e 655d 2920 2d3e  [str], None]) ->
-000148c0: 2027 5265 7375 6c74 273a 0a20 2020 2020   'Result':.     
-000148d0: 2020 2022 2222 4669 6c74 6572 2074 6865     """Filter the
-000148e0: 2072 6573 756c 7473 2064 6f77 6e20 746f   results down to
-000148f0: 2065 7665 6e20 6f75 7463 6f6d 6573 2073   even outcomes s
-00014900: 6f20 7468 6174 2070 6c6f 7474 6564 2072  o that plotted r
-00014910: 6573 756c 7473 2077 696c 6c20 6265 206d  esults will be m
-00014920: 6561 6e69 6e67 6675 6c2e 0a0a 2020 2020  eaningful...    
-00014930: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00014940: 2020 2020 2020 6e3a 2054 6865 206e 756d        n: The num
-00014950: 6265 7220 6f66 2069 6e74 6572 6163 7469  ber of interacti
-00014960: 6f6e 7320 6120 7370 6563 6966 6963 2065  ons a specific e
-00014970: 7661 6c75 6174 696f 6e20 6d75 7374 2068  valuation must h
-00014980: 6176 6520 284e 6f6e 6520 696e 6469 6361  ave (None indica
-00014990: 7465 7320 6e6f 2063 6f6e 7374 7261 696e  tes no constrain
-000149a0: 7429 2e0a 2020 2020 2020 2020 2020 2020  t)..            
-000149b0: 6c3a 2054 6865 206c 6576 656c 2061 7420  l: The level at 
-000149c0: 7768 6963 6820 7765 2077 6973 6820 746f  which we wish to
-000149d0: 2063 6f6d 7061 7265 2065 7661 6c61 7469   compare evalati
-000149e0: 6f6e 206f 7574 636f 6d65 732e 0a20 2020  on outcomes..   
-000149f0: 2020 2020 2020 2020 2070 3a20 5468 6520           p: The 
-00014a00: 7061 6972 7320 7468 6174 206d 7573 7420  pairs that must 
-00014a10: 6578 6973 7420 6163 726f 7373 2061 6c6c  exist across all
-00014a20: 2063 6f6d 7061 7269 736f 6e20 6c65 7665   comparison leve
-00014a30: 6c73 2069 6e20 6f72 6465 7220 746f 2062  ls in order to b
-00014a40: 6520 696e 636c 7564 6564 2e0a 2020 2020  e included..    
-00014a50: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00014a60: 2072 6573 756c 7420 3d20 7365 6c66 2e63   result = self.c
-00014a70: 6f70 7928 290a 2020 2020 2020 2020 6966  opy().        if
-00014a80: 206c 206f 7220 703a 2072 6573 756c 7420   l or p: result 
-00014a90: 3d20 7265 7375 6c74 2e5f 6772 6f75 705f  = result._group_
-00014aa0: 7028 6c2c 7029 0a20 2020 2020 2020 2069  p(l,p).        i
-00014ab0: 6620 6e20 2020 2020 3a20 7265 7375 6c74  f n     : result
-00014ac0: 203d 2072 6573 756c 742e 5f67 6c6f 6261   = result._globa
-00014ad0: 6c5f 6e28 6e29 0a20 2020 2020 2020 2072  l_n(n).        r
-00014ae0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-00014af0: 2020 6465 6620 5f72 656d 6f76 6528 7365    def _remove(se
-00014b00: 6c66 2c20 6964 733a 2053 6571 7565 6e63  lf, ids: Sequenc
-00014b10: 655b 5475 706c 655b 696e 742c 696e 742c  e[Tuple[int,int,
-00014b20: 696e 745d 5d2c 206e 3d30 2920 2d3e 2053  int]], n=0) -> S
-00014b30: 6571 7565 6e63 655b 696e 745d 3a0a 2020  equence[int]:.  
-00014b40: 2020 2020 2020 2374 6869 7320 6973 206d        #this is m
-00014b50: 7563 6820 6661 7374 6572 2074 6861 6e20  uch faster than 
-00014b60: 616e 7920 6275 696c 7420 696e 2054 6162  any built in Tab
-00014b70: 6c65 206d 6574 686f 6473 0a20 2020 2020  le methods.     
-00014b80: 2020 2023 746f 2077 6f72 6b20 696e 7465     #to work inte
-00014b90: 7261 6374 696f 6e73 206d 7573 7420 6265  ractions must be
-00014ba0: 2073 6f72 7465 6420 6279 2065 6e76 5f69   sorted by env_i
-00014bb0: 642c 6c72 6e5f 6964 2c76 616c 5f69 640a  d,lrn_id,val_id.
-00014bc0: 2020 2020 2020 2020 6c6f 6320 2020 2020          loc     
-00014bd0: 2020 2020 2020 203d 2030 0a20 2020 2020         = 0.     
-00014be0: 2020 2073 656c 6563 7420 2020 2020 2020     select       
-00014bf0: 2020 3d20 5b5d 0a20 2020 2020 2020 206e    = [].        n
-00014c00: 5f69 6e74 6572 6163 7469 6f6e 7320 3d20  _interactions = 
-00014c10: 6c65 6e28 7365 6c66 2e69 6e74 6572 6163  len(self.interac
-00014c20: 7469 6f6e 7329 0a20 2020 2020 2020 2065  tions).        e
-00014c30: 6e76 5f69 6473 2c6c 726e 5f69 6473 2c76  nv_ids,lrn_ids,v
-00014c40: 616c 5f69 6473 203d 2073 656c 662e 696e  al_ids = self.in
-00014c50: 7465 7261 6374 696f 6e73 5b5b 2765 6e76  teractions[['env
-00014c60: 6972 6f6e 6d65 6e74 5f69 6427 2c27 6c65  ironment_id','le
-00014c70: 6172 6e65 725f 6964 272c 2765 7661 6c75  arner_id','evalu
-00014c80: 6174 6f72 5f69 6427 5d5d 0a20 2020 2020  ator_id']].     
-00014c90: 2020 2069 6473 203d 2073 6f72 7465 6428     ids = sorted(
-00014ca0: 6964 7329 0a20 2020 2020 2020 2066 6f72  ids).        for
-00014cb0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-00014cc0: 6964 7329 293a 0a20 2020 2020 2020 2020  ids)):.         
-00014cd0: 2020 2065 2c6c 2c76 203d 2069 6473 5b69     e,l,v = ids[i
-00014ce0: 5d0a 2020 2020 2020 2020 2020 2020 6c6f  ].            lo
-00014cf0: 3120 3d20 6d79 5f62 6973 6563 745f 6c65  1 = my_bisect_le
-00014d00: 6674 2028 656e 765f 6964 732c 652c 6c6f  ft (env_ids,e,lo
-00014d10: 632c 6e5f 696e 7465 7261 6374 696f 6e73  c,n_interactions
-00014d20: 290a 2020 2020 2020 2020 2020 2020 6869  ).            hi
-00014d30: 3120 3d20 6d79 5f62 6973 6563 745f 7269  1 = my_bisect_ri
-00014d40: 6768 7428 656e 765f 6964 732c 652c 6c6f  ght(env_ids,e,lo
-00014d50: 632c 6e5f 696e 7465 7261 6374 696f 6e73  c,n_interactions
-00014d60: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00014d70: 206c 6f31 3d3d 6869 313a 2063 6f6e 7469   lo1==hi1: conti
-00014d80: 6e75 6520 2374 6865 2067 6976 656e 2069  nue #the given i
-00014d90: 6473 2061 7265 6e27 7420 696e 2069 6e74  ds aren't in int
-00014da0: 6572 6163 7469 6f6e 730a 2020 2020 2020  eractions.      
-00014db0: 2020 2020 2020 6c6f 3220 3d20 6d79 5f62        lo2 = my_b
-00014dc0: 6973 6563 745f 6c65 6674 2028 6c72 6e5f  isect_left (lrn_
-00014dd0: 6964 732c 6c2c 6c6f 312c 6869 3129 0a20  ids,l,lo1,hi1). 
-00014de0: 2020 2020 2020 2020 2020 2068 6932 203d             hi2 =
-00014df0: 206d 795f 6269 7365 6374 5f72 6967 6874   my_bisect_right
-00014e00: 286c 726e 5f69 6473 2c6c 2c6c 6f31 2c68  (lrn_ids,l,lo1,h
-00014e10: 6931 290a 2020 2020 2020 2020 2020 2020  i1).            
-00014e20: 6966 206c 6f32 3d3d 6869 323a 2063 6f6e  if lo2==hi2: con
-00014e30: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-00014e40: 2020 6c6f 3320 3d20 6d79 5f62 6973 6563    lo3 = my_bisec
-00014e50: 745f 6c65 6674 2028 7661 6c5f 6964 732c  t_left (val_ids,
-00014e60: 762c 6c6f 322c 6869 3229 0a20 2020 2020  v,lo2,hi2).     
-00014e70: 2020 2020 2020 2068 6933 203d 206d 795f         hi3 = my_
-00014e80: 6269 7365 6374 5f72 6967 6874 2876 616c  bisect_right(val
-00014e90: 5f69 6473 2c76 2c6c 6f32 2c68 6932 290a  _ids,v,lo2,hi2).
-00014ea0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00014eb0: 6f33 3d3d 6869 333a 2063 6f6e 7469 6e75  o3==hi3: continu
-00014ec0: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
-00014ed0: 6c65 6374 2e65 7874 656e 6428 7261 6e67  lect.extend(rang
-00014ee0: 6528 6c6f 632c 6c6f 332b 286e 2069 6620  e(loc,lo3+(n if 
-00014ef0: 6869 332d 6c6f 333e 6e20 656c 7365 2030  hi3-lo3>n else 0
-00014f00: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-00014f10: 6c6f 6320 3d20 6869 330a 0a20 2020 2020  loc = hi3..     
-00014f20: 2020 2073 656c 6563 742e 6578 7465 6e64     select.extend
-00014f30: 2872 616e 6765 286c 6f63 2c6e 5f69 6e74  (range(loc,n_int
-00014f40: 6572 6163 7469 6f6e 7329 290a 2020 2020  eractions)).    
-00014f50: 2020 2020 7265 7475 726e 2073 656c 6563      return selec
-00014f60: 740a                                     t.
+0000a2d0: 2020 2020 2067 726f 7570 7320 3d20 6f6e       groups = on
+0000a2e0: 6c79 5f66 696e 6973 6865 642e 5f67 726f  ly_finished._gro
+0000a2f0: 7570 6564 5f79 7328 702c 6c2c 6675 6c6c  uped_ys(p,l,full
+0000a300: 5f6c 2c66 756c 6c5f 6964 2c79 3d79 2c66  _l,full_id,y=y,f
+0000a310: 756e 633d 276c 6973 7427 2c63 6172 643d  unc='list',card=
+0000a320: 2753 2729 0a0a 2020 2020 2020 2020 7472  'S')..        tr
+0000a330: 793a 0a20 2020 2020 2020 2020 2020 2067  y:.            g
+0000a340: 726f 7570 7320 3d20 736f 7274 6564 2867  roups = sorted(g
+0000a350: 726f 7570 7329 0a20 2020 2020 2020 2065  roups).        e
+0000a360: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
+0000a370: 2020 2073 6f72 7465 645f 3d46 616c 7365     sorted_=False
+0000a380: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000a390: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
+0000a3a0: 645f 3d54 7275 650a 0a20 2020 2020 2020  d_=True..       
+0000a3b0: 2074 6f5f 6b65 6570 2c20 746f 5f64 726f   to_keep, to_dro
+0000a3c0: 7020 3d20 5b5d 2c20 5b5d 0a20 2020 2020  p = [], [].     
+0000a3d0: 2020 2066 6f72 205f 2c20 6772 6f75 7020     for _, group 
+0000a3e0: 696e 2067 726f 7570 6572 2867 726f 7570  in grouper(group
+0000a3f0: 732c 206b 6579 3d69 7465 6d67 6574 7465  s, key=itemgette
+0000a400: 7228 3029 2c20 736f 7274 6564 5f3d 736f  r(0), sorted_=so
+0000a410: 7274 6564 5f29 3a0a 2020 2020 2020 2020  rted_):.        
+0000a420: 2020 2020 666f 7220 5f2c 2067 726f 7570      for _, group
+0000a430: 2069 6e20 6772 6f75 7065 7228 6772 6f75   in grouper(grou
+0000a440: 702c 206b 6579 3d69 7465 6d67 6574 7465  p, key=itemgette
+0000a450: 7228 3129 2c20 736f 7274 6564 5f3d 736f  r(1), sorted_=so
+0000a460: 7274 6564 5f29 3a0a 2020 2020 2020 2020  rted_):.        
+0000a470: 2020 2020 2020 2020 6d61 785f 7661 6c2c          max_val,
+0000a480: 206b 2c20 6420 3d20 2d66 6c6f 6174 2827   k, d = -float('
+0000a490: 696e 6627 292c 205b 5d2c 205b 5d0a 2020  inf'), [], [].  
+0000a4a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000a4b0: 7220 5f2c 2067 726f 7570 2069 6e20 6772  r _, group in gr
+0000a4c0: 6f75 7065 7228 6772 6f75 702c 206b 6579  ouper(group, key
+0000a4d0: 3d69 7465 6d67 6574 7465 7228 3229 2c20  =itemgetter(2), 
+0000a4e0: 736f 7274 6564 5f3d 736f 7274 6564 5f29  sorted_=sorted_)
+0000a4f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000a500: 2020 2020 2020 6772 6f75 7020 3d20 6c69        group = li
+0000a510: 7374 2867 726f 7570 290a 2020 2020 2020  st(group).      
+0000a520: 2020 2020 2020 2020 2020 2020 2020 6964                id
+0000a530: 732c 7661 6c73 203d 207a 6970 282a 2828  s,vals = zip(*((
+0000a540: 675b 335d 2c20 6d65 616e 2869 736c 6963  g[3], mean(islic
+0000a550: 6528 675b 2d31 5d2c 6e29 2929 2066 6f72  e(g[-1],n))) for
+0000a560: 2067 2069 6e20 6772 6f75 7029 290a 2020   g in group)).  
+0000a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a580: 2020 6d65 616e 5f76 616c 203d 206d 6561    mean_val = mea
+0000a590: 6e28 7661 6c73 290a 2020 2020 2020 2020  n(vals).        
+0000a5a0: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+0000a5b0: 6561 6e5f 7661 6c20 3c20 6d61 785f 7661  ean_val < max_va
+0000a5c0: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+0000a5d0: 2020 2020 2020 2020 2020 2064 2e65 7874             d.ext
+0000a5e0: 656e 6428 6964 7329 0a20 2020 2020 2020  end(ids).       
+0000a5f0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000a600: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000a610: 2020 2020 2020 2020 2020 206d 6178 5f76             max_v
+0000a620: 616c 203d 206d 6561 6e5f 7661 6c0a 2020  al = mean_val.  
+0000a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a640: 2020 2020 2020 642e 6578 7465 6e64 286b        d.extend(k
+0000a650: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000a660: 2020 2020 2020 2020 2020 6b20 3d20 6964            k = id
+0000a670: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0000a680: 2020 746f 5f6b 6565 702e 6578 7465 6e64    to_keep.extend
+0000a690: 286b 290a 2020 2020 2020 2020 2020 2020  (k).            
+0000a6a0: 2020 2020 746f 5f64 726f 702e 6578 7465      to_drop.exte
+0000a6b0: 6e64 2864 290a 0a20 2020 2020 2020 2069  nd(d)..        i
+0000a6c0: 6620 746f 5f64 726f 703a 0a20 2020 2020  f to_drop:.     
+0000a6d0: 2020 2020 2020 2073 656c 6563 7420 3d20         select = 
+0000a6e0: 6f6e 6c79 5f66 696e 6973 6865 642e 5f72  only_finished._r
+0000a6f0: 656d 6f76 6528 746f 5f64 726f 7029 0a20  emove(to_drop). 
+0000a700: 2020 2020 2020 2020 2020 2069 6e74 6572             inter
+0000a710: 6163 7469 6f6e 7320 3d20 5461 626c 6528  actions = Table(
+0000a720: 5669 6577 2869 6e74 6572 6163 7469 6f6e  View(interaction
+0000a730: 732e 5f64 6174 612c 7365 6c65 6374 292c  s._data,select),
+0000a740: 2069 6e74 6572 6163 7469 6f6e 732e 636f   interactions.co
+0000a750: 6c75 6d6e 732c 2069 6e74 6572 6163 7469  lumns, interacti
+0000a760: 6f6e 732e 696e 6465 7865 7329 0a0a 2020  ons.indexes)..  
+0000a770: 2020 2020 2020 655f 6b65 6570 2c6c 5f6b        e_keep,l_k
+0000a780: 6565 702c 765f 6b65 6570 203d 206d 6170  eep,v_keep = map
+0000a790: 2873 6574 2c7a 6970 282a 746f 5f6b 6565  (set,zip(*to_kee
+0000a7a0: 7029 2920 6966 2074 6f5f 6b65 6570 2065  p)) if to_keep e
+0000a7b0: 6c73 6520 285b 5d2c 5b5d 2c5b 5d29 0a20  lse ([],[],[]). 
+0000a7c0: 2020 2020 2020 2069 6620 6c65 6e28 655f         if len(e_
+0000a7d0: 6b65 6570 2920 213d 206c 656e 2865 6e76  keep) != len(env
+0000a7e0: 6972 6f6e 6d65 6e74 7329 3a20 656e 7669  ironments): envi
+0000a7f0: 726f 6e6d 656e 7473 203d 2065 6e76 6972  ronments = envir
+0000a800: 6f6e 6d65 6e74 732e 7768 6572 6528 656e  onments.where(en
+0000a810: 7669 726f 6e6d 656e 745f 6964 3d65 5f6b  vironment_id=e_k
+0000a820: 6565 7029 0a20 2020 2020 2020 2069 6620  eep).        if 
+0000a830: 6c65 6e28 6c5f 6b65 6570 2920 213d 206c  len(l_keep) != l
+0000a840: 656e 286c 6561 726e 6572 7329 2020 2020  en(learners)    
+0000a850: 3a20 6c65 6172 6e65 7273 2020 2020 203d  : learners     =
+0000a860: 206c 6561 726e 6572 7320 2020 202e 7768   learners    .wh
+0000a870: 6572 6528 6c65 6172 6e65 725f 6964 2020  ere(learner_id  
+0000a880: 2020 3d6c 5f6b 6565 7029 0a20 2020 2020    =l_keep).     
+0000a890: 2020 2069 6620 6c65 6e28 765f 6b65 6570     if len(v_keep
+0000a8a0: 2920 213d 206c 656e 2865 7661 6c75 6174  ) != len(evaluat
+0000a8b0: 6f72 7329 2020 3a20 6576 616c 7561 746f  ors)  : evaluato
+0000a8c0: 7273 2020 203d 2065 7661 6c75 6174 6f72  rs   = evaluator
+0000a8d0: 7320 202e 7768 6572 6528 6576 616c 7561  s  .where(evalua
+0000a8e0: 746f 725f 6964 2020 3d76 5f6b 6565 7029  tor_id  =v_keep)
+0000a8f0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000a900: 2052 6573 756c 7428 656e 7669 726f 6e6d   Result(environm
+0000a910: 656e 7473 2c20 6c65 6172 6e65 7273 2c20  ents, learners, 
+0000a920: 6576 616c 7561 746f 7273 2c20 696e 7465  evaluators, inte
+0000a930: 7261 6374 696f 6e73 2c20 6f6e 6c79 5f66  ractions, only_f
+0000a940: 696e 6973 6865 642e 6578 7065 7269 6d65  inished.experime
+0000a950: 6e74 290a 0a20 2020 2064 6566 2066 696c  nt)..    def fil
+0000a960: 7465 725f 6669 6e28 7365 6c66 2c0a 2020  ter_fin(self,.  
+0000a970: 2020 2020 2020 6e3a 2055 6e69 6f6e 5b69        n: Union[i
+0000a980: 6e74 2c4c 6974 6572 616c 5b27 6d69 6e27  nt,Literal['min'
+0000a990: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+0000a9a0: 2020 206c 3a20 556e 696f 6e5b 7374 722c     l: Union[str,
+0000a9b0: 2053 6571 7565 6e63 655b 7374 725d 5d20   Sequence[str]] 
+0000a9c0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000a9d0: 703a 2055 6e69 6f6e 5b73 7472 2c20 5365  p: Union[str, Se
+0000a9e0: 7175 656e 6365 5b73 7472 5d5d 203d 204e  quence[str]] = N
+0000a9f0: 6f6e 6529 202d 3e20 2752 6573 756c 7427  one) -> 'Result'
+0000aa00: 3a0a 2020 2020 2020 2020 2222 2246 696c  :.        """Fil
+0000aa10: 7465 7220 7468 6520 7265 7375 6c74 7320  ter the results 
+0000aa20: 646f 776e 2074 6f20 6576 656e 206f 7574  down to even out
+0000aa30: 636f 6d65 7320 736f 2074 6861 7420 706c  comes so that pl
+0000aa40: 6f74 7465 6420 7265 7375 6c74 7320 7769  otted results wi
+0000aa50: 6c6c 2062 6520 6d65 616e 696e 6766 756c  ll be meaningful
+0000aa60: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+0000aa70: 0a20 2020 2020 2020 2020 2020 206e 3a20  .            n: 
+0000aa80: 5468 6520 6e75 6d62 6572 206f 6620 696e  The number of in
+0000aa90: 7465 7261 6374 696f 6e73 2061 2073 7065  teractions a spe
+0000aaa0: 6369 6669 6320 6576 616c 7561 7469 6f6e  cific evaluation
+0000aab0: 206d 7573 7420 6861 7665 2028 4e6f 6e65   must have (None
+0000aac0: 2069 6e64 6963 6174 6573 206e 6f20 636f   indicates no co
+0000aad0: 6e73 7472 6169 6e74 292e 0a20 2020 2020  nstraint)..     
+0000aae0: 2020 2020 2020 206c 3a20 5468 6520 6c65         l: The le
+0000aaf0: 7665 6c20 6174 2077 6869 6368 2077 6520  vel at which we 
+0000ab00: 7769 7368 2074 6f20 636f 6d70 6172 6520  wish to compare 
+0000ab10: 6576 616c 6174 696f 6e20 6f75 7463 6f6d  evalation outcom
+0000ab20: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
+0000ab30: 703a 2054 6865 2070 6169 7273 2074 6861  p: The pairs tha
+0000ab40: 7420 6d75 7374 2065 7869 7374 2061 6372  t must exist acr
+0000ab50: 6f73 7320 616c 6c20 636f 6d70 6172 6973  oss all comparis
+0000ab60: 6f6e 206c 6576 656c 7320 696e 206f 7264  on levels in ord
+0000ab70: 6572 2074 6f20 6265 2069 6e63 6c75 6465  er to be include
+0000ab80: 642e 0a20 2020 2020 2020 2022 2222 0a0a  d..        """..
+0000ab90: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0000aba0: 2073 656c 662e 5f66 696c 7465 725f 6669   self._filter_fi
+0000abb0: 6e28 6e2c 6c2c 7029 0a0a 2020 2020 2020  n(n,l,p)..      
+0000abc0: 2020 6966 206c 656e 2872 6573 756c 742e    if len(result.
+0000abd0: 696e 7465 7261 6374 696f 6e73 2920 3d3d  interactions) ==
+0000abe0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0000abf0: 436f 6261 436f 6e74 6578 742e 6c6f 6767  CobaContext.logg
+0000ac00: 6572 2e6c 6f67 2866 2254 6865 7265 2077  er.log(f"There w
+0000ac10: 6173 206e 6f20 7b70 7d20 7768 6963 6820  as no {p} which 
+0000ac20: 7761 7320 6669 6e69 7368 6564 2066 6f72  was finished for
+0000ac30: 2065 7665 7279 207b 6c7d 2e22 290a 0a20   every {l}.").. 
+0000ac40: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0000ac50: 7375 6c74 0a0a 2020 2020 6465 6620 6669  sult..    def fi
+0000ac60: 6c74 6572 5f65 6e76 2873 656c 662c 2070  lter_env(self, p
+0000ac70: 7265 643a 4361 6c6c 6162 6c65 5b5b 4d61  red:Callable[[Ma
+0000ac80: 7070 696e 675b 7374 722c 416e 795d 5d2c  pping[str,Any]],
+0000ac90: 626f 6f6c 5d20 3d20 4e6f 6e65 2c20 2a2a  bool] = None, **
+0000aca0: 6b77 6172 6773 3a20 416e 7929 202d 3e20  kwargs: Any) -> 
+0000acb0: 2752 6573 756c 7427 3a0a 2020 2020 2020  'Result':.      
+0000acc0: 2020 2222 2246 696c 7465 7220 7468 6520    """Filter the 
+0000acd0: 7265 7375 6c74 2074 6f20 6f6e 6c79 2063  result to only c
+0000ace0: 6f6e 7461 696e 2064 6174 6120 6162 6f75  ontain data abou
+0000acf0: 7420 7370 6563 6966 6963 2065 6e76 6972  t specific envir
+0000ad00: 6f6e 6d65 6e74 732e 0a0a 2020 2020 2020  onments...      
+0000ad10: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000ad20: 2020 2020 7072 6564 3a20 4120 7072 6564      pred: A pred
+0000ad30: 6963 6174 6520 7468 6174 2072 6574 7572  icate that retur
+0000ad40: 6e73 2074 7275 6520 666f 7220 6c65 6172  ns true for lear
+0000ad50: 6e65 7220 6469 6374 696f 6e61 7269 6573  ner dictionaries
+0000ad60: 2074 6861 7420 7368 6f75 6c64 2062 6520   that should be 
+0000ad70: 6b65 7074 2e0a 2020 2020 2020 2020 2020  kept..          
+0000ad80: 2020 2a2a 6b77 6172 6773 3a20 6b65 792d    **kwargs: key-
+0000ad90: 7661 6c75 6520 7061 6972 7320 746f 2066  value pairs to f
+0000ada0: 696c 7465 7220 6f6e 2e20 546f 2073 6565  ilter on. To see
+0000adb0: 2066 696c 7465 7269 6e67 206f 7074 696f   filtering optio
+0000adc0: 6e73 2073 6565 2054 6162 6c65 2e66 696c  ns see Table.fil
+0000add0: 7465 722e 0a20 2020 2020 2020 2022 2222  ter..        """
+0000ade0: 0a0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+0000adf0: 2873 656c 662e 656e 7669 726f 6e6d 656e  (self.environmen
+0000ae00: 7473 2920 3d3d 2030 3a20 7265 7475 726e  ts) == 0: return
+0000ae10: 2073 656c 660a 0a20 2020 2020 2020 2065   self..        e
+0000ae20: 6e76 6972 6f6e 6d65 6e74 7320 3d20 7365  nvironments = se
+0000ae30: 6c66 2e65 6e76 6972 6f6e 6d65 6e74 732e  lf.environments.
+0000ae40: 7768 6572 6528 7072 6564 2c20 2a2a 6b77  where(pred, **kw
+0000ae50: 6172 6773 290a 2020 2020 2020 2020 6c65  args).        le
+0000ae60: 6172 6e65 7273 2020 2020 203d 2073 656c  arners     = sel
+0000ae70: 662e 6c65 6172 6e65 7273 0a20 2020 2020  f.learners.     
+0000ae80: 2020 2065 7661 6c75 6174 6f72 7320 2020     evaluators   
+0000ae90: 3d20 7365 6c66 2e65 7661 6c75 6174 6f72  = self.evaluator
+0000aea0: 730a 2020 2020 2020 2020 696e 7465 7261  s.        intera
+0000aeb0: 6374 696f 6e73 203d 2073 656c 662e 696e  ctions = self.in
+0000aec0: 7465 7261 6374 696f 6e73 0a0a 2020 2020  teractions..    
+0000aed0: 2020 2020 6966 206c 656e 2865 6e76 6972      if len(envir
+0000aee0: 6f6e 6d65 6e74 7329 203d 3d20 6c65 6e28  onments) == len(
+0000aef0: 7365 6c66 2e65 6e76 6972 6f6e 6d65 6e74  self.environment
+0000af00: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+0000af10: 7265 7475 726e 2073 656c 660a 0a20 2020  return self..   
+0000af20: 2020 2020 2069 6620 6c65 6e28 656e 7669       if len(envi
+0000af30: 726f 6e6d 656e 7473 2920 3d3d 2030 3a0a  ronments) == 0:.
+0000af40: 2020 2020 2020 2020 2020 2020 436f 6261              Coba
+0000af50: 436f 6e74 6578 742e 6c6f 6767 6572 2e6c  Context.logger.l
+0000af60: 6f67 2866 224e 6f20 656e 7669 726f 6e6d  og(f"No environm
+0000af70: 656e 7473 206d 6174 6368 6564 2074 6865  ents matched the
+0000af80: 2067 6976 656e 2066 696c 7465 722e 2229   given filter.")
+0000af90: 0a0a 2020 2020 2020 2020 696e 7465 7261  ..        intera
+0000afa0: 6374 696f 6e73 203d 2069 6e74 6572 6163  ctions = interac
+0000afb0: 7469 6f6e 732e 7768 6572 6528 656e 7669  tions.where(envi
+0000afc0: 726f 6e6d 656e 745f 6964 3d73 6574 2865  ronment_id=set(e
+0000afd0: 6e76 6972 6f6e 6d65 6e74 735b 2265 6e76  nvironments["env
+0000afe0: 6972 6f6e 6d65 6e74 5f69 6422 5d29 290a  ironment_id"])).
+0000aff0: 2020 2020 2020 2020 6c65 6172 6e65 7273          learners
+0000b000: 2020 2020 203d 206c 6561 726e 6572 7320       = learners 
+0000b010: 2020 202e 7768 6572 6528 6c65 6172 6e65     .where(learne
+0000b020: 725f 6964 2020 2020 3d73 6574 2869 6e74  r_id    =set(int
+0000b030: 6572 6163 7469 6f6e 735b 226c 6561 726e  eractions["learn
+0000b040: 6572 5f69 6422 5d29 290a 2020 2020 2020  er_id"])).      
+0000b050: 2020 6576 616c 7561 746f 7273 2020 203d    evaluators   =
+0000b060: 2065 7661 6c75 6174 6f72 7320 202e 7768   evaluators  .wh
+0000b070: 6572 6528 6576 616c 7561 746f 725f 6964  ere(evaluator_id
+0000b080: 2020 3d73 6574 2869 6e74 6572 6163 7469    =set(interacti
+0000b090: 6f6e 735b 2265 7661 6c75 6174 6f72 5f69  ons["evaluator_i
+0000b0a0: 6422 5d29 290a 0a20 2020 2020 2020 2072  d"]))..        r
+0000b0b0: 6574 7572 6e20 5265 7375 6c74 2865 6e76  eturn Result(env
+0000b0c0: 6972 6f6e 6d65 6e74 732c 6c65 6172 6e65  ironments,learne
+0000b0d0: 7273 2c65 7661 6c75 6174 6f72 732c 696e  rs,evaluators,in
+0000b0e0: 7465 7261 6374 696f 6e73 2c73 656c 662e  teractions,self.
+0000b0f0: 6578 7065 7269 6d65 6e74 290a 0a20 2020  experiment)..   
+0000b100: 2064 6566 2066 696c 7465 725f 6c72 6e28   def filter_lrn(
+0000b110: 7365 6c66 2c20 7072 6564 3a43 616c 6c61  self, pred:Calla
+0000b120: 626c 655b 5b4d 6170 7069 6e67 5b73 7472  ble[[Mapping[str
+0000b130: 2c41 6e79 5d5d 2c62 6f6f 6c5d 203d 204e  ,Any]],bool] = N
+0000b140: 6f6e 652c 202a 2a6b 7761 7267 733a 2041  one, **kwargs: A
+0000b150: 6e79 2920 2d3e 2027 5265 7375 6c74 273a  ny) -> 'Result':
+0000b160: 0a20 2020 2020 2020 2022 2222 4669 6c74  .        """Filt
+0000b170: 6572 2074 6865 2072 6573 756c 7420 746f  er the result to
+0000b180: 206f 6e6c 7920 636f 6e74 6169 6e20 6461   only contain da
+0000b190: 7461 2061 626f 7574 2073 7065 6369 6669  ta about specifi
+0000b1a0: 6320 6c65 6172 6e65 7273 2e0a 0a20 2020  c learners...   
+0000b1b0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000b1c0: 2020 2020 2020 2070 7265 643a 2041 2070         pred: A p
+0000b1d0: 7265 6469 6361 7465 2074 6861 7420 7265  redicate that re
+0000b1e0: 7475 726e 7320 7472 7565 2066 6f72 206c  turns true for l
+0000b1f0: 6561 726e 6572 2064 6963 7469 6f6e 6172  earner dictionar
+0000b200: 6965 7320 7468 6174 2073 686f 756c 6420  ies that should 
+0000b210: 6265 206b 6570 742e 0a20 2020 2020 2020  be kept..       
+0000b220: 2020 2020 202a 2a6b 7761 7267 733a 206b       **kwargs: k
+0000b230: 6579 2d76 616c 7565 2070 6169 7273 2074  ey-value pairs t
+0000b240: 6f20 6669 6c74 6572 206f 6e2e 2054 6f20  o filter on. To 
+0000b250: 7365 6520 6669 6c74 6572 696e 6720 6f70  see filtering op
+0000b260: 7469 6f6e 7320 7365 6520 5461 626c 652e  tions see Table.
+0000b270: 6669 6c74 6572 2e0a 2020 2020 2020 2020  filter..        
+0000b280: 2222 220a 2020 2020 2020 2020 6966 206c  """.        if l
+0000b290: 656e 2873 656c 662e 6c65 6172 6e65 7273  en(self.learners
+0000b2a0: 2920 3d3d 2030 3a20 7265 7475 726e 2073  ) == 0: return s
+0000b2b0: 656c 660a 0a20 2020 2020 2020 2065 6e76  elf..        env
+0000b2c0: 6972 6f6e 6d65 6e74 7320 3d20 7365 6c66  ironments = self
+0000b2d0: 2e65 6e76 6972 6f6e 6d65 6e74 730a 2020  .environments.  
+0000b2e0: 2020 2020 2020 6c65 6172 6e65 7273 2020        learners  
+0000b2f0: 2020 203d 2073 656c 662e 6c65 6172 6e65     = self.learne
+0000b300: 7273 2e77 6865 7265 2870 7265 642c 202a  rs.where(pred, *
+0000b310: 2a6b 7761 7267 7329 0a20 2020 2020 2020  *kwargs).       
+0000b320: 2065 7661 6c75 6174 6f72 7320 2020 3d20   evaluators   = 
+0000b330: 7365 6c66 2e65 7661 6c75 6174 6f72 730a  self.evaluators.
+0000b340: 2020 2020 2020 2020 696e 7465 7261 6374          interact
+0000b350: 696f 6e73 203d 2073 656c 662e 696e 7465  ions = self.inte
+0000b360: 7261 6374 696f 6e73 0a0a 2020 2020 2020  ractions..      
+0000b370: 2020 6966 206c 656e 286c 6561 726e 6572    if len(learner
+0000b380: 7329 203d 3d20 6c65 6e28 7365 6c66 2e6c  s) == len(self.l
+0000b390: 6561 726e 6572 7329 3a0a 2020 2020 2020  earners):.      
+0000b3a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000b3b0: 660a 0a20 2020 2020 2020 2069 6620 6c65  f..        if le
+0000b3c0: 6e28 6c65 6172 6e65 7273 2920 3d3d 2030  n(learners) == 0
+0000b3d0: 3a0a 2020 2020 2020 2020 2020 2020 436f  :.            Co
+0000b3e0: 6261 436f 6e74 6578 742e 6c6f 6767 6572  baContext.logger
+0000b3f0: 2e6c 6f67 2866 224e 6f20 6c65 6172 6e65  .log(f"No learne
+0000b400: 7273 206d 6174 6368 6564 2074 6865 2067  rs matched the g
+0000b410: 6976 656e 2066 696c 7465 722e 2229 0a0a  iven filter.")..
+0000b420: 2020 2020 2020 2020 696e 7465 7261 6374          interact
+0000b430: 696f 6e73 203d 2069 6e74 6572 6163 7469  ions = interacti
+0000b440: 6f6e 732e 7768 6572 6528 6c65 6172 6e65  ons.where(learne
+0000b450: 725f 6964 2020 2020 3d73 6574 286c 6561  r_id    =set(lea
+0000b460: 726e 6572 735b 226c 6561 726e 6572 5f69  rners["learner_i
+0000b470: 6422 5d29 290a 2020 2020 2020 2020 656e  d"])).        en
+0000b480: 7669 726f 6e6d 656e 7473 203d 2065 6e76  vironments = env
+0000b490: 6972 6f6e 6d65 6e74 732e 7768 6572 6528  ironments.where(
+0000b4a0: 656e 7669 726f 6e6d 656e 745f 6964 3d73  environment_id=s
+0000b4b0: 6574 2869 6e74 6572 6163 7469 6f6e 735b  et(interactions[
+0000b4c0: 2265 6e76 6972 6f6e 6d65 6e74 5f69 6422  "environment_id"
+0000b4d0: 5d29 290a 2020 2020 2020 2020 6576 616c  ])).        eval
+0000b4e0: 7561 746f 7273 2020 203d 2065 7661 6c75  uators   = evalu
+0000b4f0: 6174 6f72 7320 202e 7768 6572 6528 6576  ators  .where(ev
+0000b500: 616c 7561 746f 725f 6964 2020 3d73 6574  aluator_id  =set
+0000b510: 2869 6e74 6572 6163 7469 6f6e 735b 2265  (interactions["e
+0000b520: 7661 6c75 6174 6f72 5f69 6422 5d29 290a  valuator_id"])).
+0000b530: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000b540: 5265 7375 6c74 2865 6e76 6972 6f6e 6d65  Result(environme
+0000b550: 6e74 732c 6c65 6172 6e65 7273 2c65 7661  nts,learners,eva
+0000b560: 6c75 6174 6f72 732c 696e 7465 7261 6374  luators,interact
+0000b570: 696f 6e73 290a 0a20 2020 2064 6566 2066  ions)..    def f
+0000b580: 696c 7465 725f 7661 6c28 7365 6c66 2c20  ilter_val(self, 
+0000b590: 7072 6564 3a43 616c 6c61 626c 655b 5b4d  pred:Callable[[M
+0000b5a0: 6170 7069 6e67 5b73 7472 2c41 6e79 5d5d  apping[str,Any]]
+0000b5b0: 2c62 6f6f 6c5d 203d 204e 6f6e 652c 202a  ,bool] = None, *
+0000b5c0: 2a6b 7761 7267 733a 2041 6e79 2920 2d3e  *kwargs: Any) ->
+0000b5d0: 2027 5265 7375 6c74 273a 0a20 2020 2020   'Result':.     
+0000b5e0: 2020 2022 2222 4669 6c74 6572 2074 6865     """Filter the
+0000b5f0: 2072 6573 756c 7420 746f 206f 6e6c 7920   result to only 
+0000b600: 636f 6e74 6169 6e20 6461 7461 2061 626f  contain data abo
+0000b610: 7574 2073 7065 6369 6669 6320 6576 616c  ut specific eval
+0000b620: 7561 746f 7273 2e0a 0a20 2020 2020 2020  uators...       
+0000b630: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0000b640: 2020 2070 7265 643a 2041 2070 7265 6469     pred: A predi
+0000b650: 6361 7465 2074 6861 7420 7265 7475 726e  cate that return
+0000b660: 7320 7472 7565 2066 6f72 206c 6561 726e  s true for learn
+0000b670: 6572 2064 6963 7469 6f6e 6172 6965 7320  er dictionaries 
+0000b680: 7468 6174 2073 686f 756c 6420 6265 206b  that should be k
+0000b690: 6570 742e 0a20 2020 2020 2020 2020 2020  ept..           
+0000b6a0: 202a 2a6b 7761 7267 733a 206b 6579 2d76   **kwargs: key-v
+0000b6b0: 616c 7565 2070 6169 7273 2074 6f20 6669  alue pairs to fi
+0000b6c0: 6c74 6572 206f 6e2e 2054 6f20 7365 6520  lter on. To see 
+0000b6d0: 6669 6c74 6572 696e 6720 6f70 7469 6f6e  filtering option
+0000b6e0: 7320 7365 6520 5461 626c 652e 6669 6c74  s see Table.filt
+0000b6f0: 6572 2e0a 2020 2020 2020 2020 2222 220a  er..        """.
+0000b700: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
+0000b710: 656c 662e 6c65 6172 6e65 7273 2920 3d3d  elf.learners) ==
+0000b720: 2030 3a20 7265 7475 726e 2073 656c 660a   0: return self.
+0000b730: 0a20 2020 2020 2020 2065 6e76 6972 6f6e  .        environ
+0000b740: 6d65 6e74 7320 3d20 7365 6c66 2e65 6e76  ments = self.env
+0000b750: 6972 6f6e 6d65 6e74 730a 2020 2020 2020  ironments.      
+0000b760: 2020 6c65 6172 6e65 7273 2020 2020 203d    learners     =
+0000b770: 2073 656c 662e 6c65 6172 6e65 7273 0a20   self.learners. 
+0000b780: 2020 2020 2020 2065 7661 6c75 6174 6f72         evaluator
+0000b790: 7320 2020 3d20 7365 6c66 2e65 7661 6c75  s   = self.evalu
+0000b7a0: 6174 6f72 732e 7768 6572 6528 7072 6564  ators.where(pred
+0000b7b0: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
+0000b7c0: 2020 2020 696e 7465 7261 6374 696f 6e73      interactions
+0000b7d0: 203d 2073 656c 662e 696e 7465 7261 6374   = self.interact
+0000b7e0: 696f 6e73 0a0a 2020 2020 2020 2020 6966  ions..        if
+0000b7f0: 206c 656e 2865 7661 6c75 6174 6f72 7329   len(evaluators)
+0000b800: 203d 3d20 6c65 6e28 7365 6c66 2e65 7661   == len(self.eva
+0000b810: 6c75 6174 6f72 7329 3a0a 2020 2020 2020  luators):.      
+0000b820: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000b830: 660a 0a20 2020 2020 2020 2069 6620 6c65  f..        if le
+0000b840: 6e28 6576 616c 7561 746f 7273 2920 3d3d  n(evaluators) ==
+0000b850: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0000b860: 436f 6261 436f 6e74 6578 742e 6c6f 6767  CobaContext.logg
+0000b870: 6572 2e6c 6f67 2866 224e 6f20 6576 616c  er.log(f"No eval
+0000b880: 7561 746f 7273 206d 6174 6368 6564 2074  uators matched t
+0000b890: 6865 2067 6976 656e 2066 696c 7465 722e  he given filter.
+0000b8a0: 2229 0a0a 2020 2020 2020 2020 696e 7465  ")..        inte
+0000b8b0: 7261 6374 696f 6e73 203d 2069 6e74 6572  ractions = inter
+0000b8c0: 6163 7469 6f6e 732e 7768 6572 6528 6576  actions.where(ev
+0000b8d0: 616c 7561 746f 725f 6964 2020 3d73 6574  aluator_id  =set
+0000b8e0: 2865 7661 6c75 6174 6f72 735b 2765 7661  (evaluators['eva
+0000b8f0: 6c75 6174 6f72 5f69 6427 5d29 290a 2020  luator_id'])).  
+0000b900: 2020 2020 2020 656e 7669 726f 6e6d 656e        environmen
+0000b910: 7473 203d 2065 6e76 6972 6f6e 6d65 6e74  ts = environment
+0000b920: 732e 7768 6572 6528 656e 7669 726f 6e6d  s.where(environm
+0000b930: 656e 745f 6964 3d73 6574 2869 6e74 6572  ent_id=set(inter
+0000b940: 6163 7469 6f6e 735b 2265 6e76 6972 6f6e  actions["environ
+0000b950: 6d65 6e74 5f69 6422 5d29 290a 2020 2020  ment_id"])).    
+0000b960: 2020 2020 6c65 6172 6e65 7273 2020 2020      learners    
+0000b970: 203d 206c 6561 726e 6572 7320 2020 202e   = learners    .
+0000b980: 7768 6572 6528 6c65 6172 6e65 725f 6964  where(learner_id
+0000b990: 2020 2020 3d73 6574 2869 6e74 6572 6163      =set(interac
+0000b9a0: 7469 6f6e 735b 226c 6561 726e 6572 5f69  tions["learner_i
+0000b9b0: 6422 5d29 290a 0a20 2020 2020 2020 2072  d"]))..        r
+0000b9c0: 6574 7572 6e20 5265 7375 6c74 2865 6e76  eturn Result(env
+0000b9d0: 6972 6f6e 6d65 6e74 732c 6c65 6172 6e65  ironments,learne
+0000b9e0: 7273 2c65 7661 6c75 6174 6f72 732c 696e  rs,evaluators,in
+0000b9f0: 7465 7261 6374 696f 6e73 290a 0a20 2020  teractions)..   
+0000ba00: 2064 6566 2066 696c 7465 725f 696e 7428   def filter_int(
+0000ba10: 7365 6c66 2c20 7072 6564 3a43 616c 6c61  self, pred:Calla
+0000ba20: 626c 655b 5b4d 6170 7069 6e67 5b73 7472  ble[[Mapping[str
+0000ba30: 2c41 6e79 5d5d 2c62 6f6f 6c5d 203d 204e  ,Any]],bool] = N
+0000ba40: 6f6e 652c 202a 2a6b 7761 7267 733a 2041  one, **kwargs: A
+0000ba50: 6e79 2920 2d3e 2027 5265 7375 6c74 273a  ny) -> 'Result':
+0000ba60: 0a20 2020 2020 2020 2022 2222 4669 6c74  .        """Filt
+0000ba70: 6572 2074 6865 2072 6573 756c 7420 746f  er the result to
+0000ba80: 206f 6e6c 7920 636f 6e74 6169 6e20 6461   only contain da
+0000ba90: 7461 2061 626f 7574 2073 7065 6369 6669  ta about specifi
+0000baa0: 6320 696e 7465 7261 6374 696f 6e73 2e0a  c interactions..
+0000bab0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+0000bac0: 2020 2020 2020 2020 2020 2070 7265 643a             pred:
+0000bad0: 2041 2070 7265 6469 6361 7465 2074 6861   A predicate tha
+0000bae0: 7420 7265 7475 726e 7320 7472 7565 2066  t returns true f
+0000baf0: 6f72 206c 6561 726e 6572 2064 6963 7469  or learner dicti
+0000bb00: 6f6e 6172 6965 7320 7468 6174 2073 686f  onaries that sho
+0000bb10: 756c 6420 6265 206b 6570 742e 0a20 2020  uld be kept..   
+0000bb20: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
+0000bb30: 733a 206b 6579 2d76 616c 7565 2070 6169  s: key-value pai
+0000bb40: 7273 2074 6f20 6669 6c74 6572 206f 6e2e  rs to filter on.
+0000bb50: 2054 6f20 7365 6520 6669 6c74 6572 696e   To see filterin
+0000bb60: 6720 6f70 7469 6f6e 7320 7365 6520 5461  g options see Ta
+0000bb70: 626c 652e 6669 6c74 6572 2e0a 2020 2020  ble.filter..    
+0000bb80: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000bb90: 6966 206c 656e 2873 656c 662e 6c65 6172  if len(self.lear
+0000bba0: 6e65 7273 2920 3d3d 2030 3a20 7265 7475  ners) == 0: retu
+0000bbb0: 726e 2073 656c 660a 0a20 2020 2020 2020  rn self..       
+0000bbc0: 2065 6e76 6972 6f6e 6d65 6e74 7320 3d20   environments = 
+0000bbd0: 7365 6c66 2e65 6e76 6972 6f6e 6d65 6e74  self.environment
+0000bbe0: 730a 2020 2020 2020 2020 6c65 6172 6e65  s.        learne
+0000bbf0: 7273 2020 2020 203d 2073 656c 662e 6c65  rs     = self.le
+0000bc00: 6172 6e65 7273 0a20 2020 2020 2020 2065  arners.        e
+0000bc10: 7661 6c75 6174 6f72 7320 2020 3d20 7365  valuators   = se
+0000bc20: 6c66 2e65 7661 6c75 6174 6f72 730a 2020  lf.evaluators.  
+0000bc30: 2020 2020 2020 696e 7465 7261 6374 696f        interactio
+0000bc40: 6e73 203d 2073 656c 662e 696e 7465 7261  ns = self.intera
+0000bc50: 6374 696f 6e73 2e77 6865 7265 2870 7265  ctions.where(pre
+0000bc60: 642c 202a 2a6b 7761 7267 7329 0a0a 2020  d, **kwargs)..  
+0000bc70: 2020 2020 2020 6966 206c 656e 2869 6e74        if len(int
+0000bc80: 6572 6163 7469 6f6e 7329 203d 3d20 6c65  eractions) == le
+0000bc90: 6e28 7365 6c66 2e69 6e74 6572 6163 7469  n(self.interacti
+0000bca0: 6f6e 7329 3a0a 2020 2020 2020 2020 2020  ons):.          
+0000bcb0: 2020 7265 7475 726e 2073 656c 660a 0a20    return self.. 
+0000bcc0: 2020 2020 2020 2069 6620 6c65 6e28 696e         if len(in
+0000bcd0: 7465 7261 6374 696f 6e73 2920 3d3d 2030  teractions) == 0
+0000bce0: 3a0a 2020 2020 2020 2020 2020 2020 436f  :.            Co
+0000bcf0: 6261 436f 6e74 6578 742e 6c6f 6767 6572  baContext.logger
+0000bd00: 2e6c 6f67 2866 224e 6f20 696e 7465 7261  .log(f"No intera
+0000bd10: 6374 696f 6e73 206d 6174 6368 6564 2074  ctions matched t
+0000bd20: 6865 2067 6976 656e 2066 696c 7465 722e  he given filter.
+0000bd30: 2229 0a0a 2020 2020 2020 2020 746f 5f6b  ")..        to_k
+0000bd40: 6565 7020 3d20 6c69 7374 2869 6e74 6572  eep = list(inter
+0000bd50: 6163 7469 6f6e 732e 6772 6f75 7062 7928  actions.groupby(
+0000bd60: 332c 7365 6c65 6374 3d4e 6f6e 6529 290a  3,select=None)).
+0000bd70: 2020 2020 2020 2020 656e 762c 6c72 6e2c          env,lrn,
+0000bd80: 7661 6c20 3d20 7a69 7028 2a74 6f5f 6b65  val = zip(*to_ke
+0000bd90: 6570 2920 6966 2074 6f5f 6b65 6570 2065  ep) if to_keep e
+0000bda0: 6c73 6520 285b 5d2c 5b5d 2c5b 5d29 0a0a  lse ([],[],[])..
+0000bdb0: 2020 2020 2020 2020 6966 206c 656e 2865          if len(e
+0000bdc0: 6e76 2920 213d 206c 656e 2865 6e76 6972  nv) != len(envir
+0000bdd0: 6f6e 6d65 6e74 7329 3a20 656e 7669 726f  onments): enviro
+0000bde0: 6e6d 656e 7473 203d 2065 6e76 6972 6f6e  nments = environ
+0000bdf0: 6d65 6e74 732e 7768 6572 6528 656e 7669  ments.where(envi
+0000be00: 726f 6e6d 656e 745f 6964 3d73 6574 2865  ronment_id=set(e
+0000be10: 6e76 2929 0a20 2020 2020 2020 2069 6620  nv)).        if 
+0000be20: 6c65 6e28 6c72 6e29 2021 3d20 6c65 6e28  len(lrn) != len(
+0000be30: 6c65 6172 6e65 7273 2920 2020 203a 206c  learners)    : l
+0000be40: 6561 726e 6572 7320 2020 2020 3d20 6c65  earners     = le
+0000be50: 6172 6e65 7273 2020 2020 2e77 6865 7265  arners    .where
+0000be60: 286c 6561 726e 6572 5f69 6420 2020 203d  (learner_id    =
+0000be70: 7365 7428 6c72 6e29 290a 2020 2020 2020  set(lrn)).      
+0000be80: 2020 6966 206c 656e 2876 616c 2920 213d    if len(val) !=
+0000be90: 206c 656e 2865 7661 6c75 6174 6f72 7329   len(evaluators)
+0000bea0: 2020 3a20 6576 616c 7561 746f 7273 2020    : evaluators  
+0000beb0: 203d 2065 7661 6c75 6174 6f72 7320 202e   = evaluators  .
+0000bec0: 7768 6572 6528 6576 616c 7561 746f 725f  where(evaluator_
+0000bed0: 6964 2020 3d73 6574 2876 616c 2929 0a0a  id  =set(val))..
+0000bee0: 2020 2020 2020 2020 7265 7475 726e 2052          return R
+0000bef0: 6573 756c 7428 656e 7669 726f 6e6d 656e  esult(environmen
+0000bf00: 7473 2c6c 6561 726e 6572 732c 6576 616c  ts,learners,eval
+0000bf10: 7561 746f 7273 2c69 6e74 6572 6163 7469  uators,interacti
+0000bf20: 6f6e 7329 0a0a 2020 2020 6465 6620 7768  ons)..    def wh
+0000bf30: 6572 655f 6265 7374 2873 656c 662c 0a20  ere_best(self,. 
+0000bf40: 2020 2020 2020 206c 3a55 6e69 6f6e 5b73         l:Union[s
+0000bf50: 7472 2c20 5365 7175 656e 6365 5b73 7472  tr, Sequence[str
+0000bf60: 5d5d 2c0a 2020 2020 2020 2020 703a 556e  ]],.        p:Un
+0000bf70: 696f 6e5b 7374 722c 2053 6571 7565 6e63  ion[str, Sequenc
+0000bf80: 655b 7374 725d 5d20 3d20 2765 6e76 6972  e[str]] = 'envir
+0000bf90: 6f6e 6d65 6e74 5f69 6427 2c0a 2020 2020  onment_id',.    
+0000bfa0: 2020 2020 793a 7374 7220 3d20 2772 6577      y:str = 'rew
+0000bfb0: 6172 6427 2c0a 2020 2020 2020 2020 6e3a  ard',.        n:
+0000bfc0: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
+0000bfd0: 2020 2020 6675 6c6c 5f6c 3a55 6e69 6f6e      full_l:Union
+0000bfe0: 5b73 7472 2c20 5365 7175 656e 6365 5b73  [str, Sequence[s
+0000bff0: 7472 5d5d 3d27 6c65 6172 6e65 725f 6964  tr]]='learner_id
+0000c000: 272c 0a20 2020 2020 2020 2066 756c 6c5f  ',.        full_
+0000c010: 703a 556e 696f 6e5b 7374 722c 2053 6571  p:Union[str, Seq
+0000c020: 7565 6e63 655b 7374 725d 5d3d 2765 6e76  uence[str]]='env
+0000c030: 6972 6f6e 6d65 6e74 5f69 6427 2920 2d3e  ironment_id') ->
+0000c040: 2027 5265 7375 6c74 273a 0a20 2020 2020   'Result':.     
+0000c050: 2020 2022 2222 5365 6c65 6374 2074 6865     """Select the
+0000c060: 2062 6573 7420 7065 7266 6f72 6d69 6e67   best performing
+0000c070: 2060 6c60 206f 7665 7220 6070 602e 0a0a   `l` over `p`...
+0000c080: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000c090: 2020 2020 2020 2020 2020 6c3a 2054 6865            l: The
+0000c0a0: 2068 7970 6572 7061 7261 6d65 7465 7220   hyperparameter 
+0000c0b0: 7661 6c75 6573 2077 6520 7769 7368 2074  values we wish t
+0000c0c0: 6f20 6f70 7469 6d69 7a65 2e0a 2020 2020  o optimize..    
+0000c0d0: 2020 2020 2020 2020 703a 2054 6865 2067          p: The g
+0000c0e0: 726f 7570 696e 6720 7661 7269 6162 6c65  rouping variable
+0000c0f0: 2077 6520 7769 7368 2074 6f20 6f70 7469   we wish to opti
+0000c100: 6d69 7a65 206f 7665 722e 0a20 2020 2020  mize over..     
+0000c110: 2020 2020 2020 2079 3a20 5468 6520 7661         y: The va
+0000c120: 7269 6162 6c65 2077 6520 7769 7368 2074  riable we wish t
+0000c130: 6f20 6f70 7469 6d69 7a65 2e0a 2020 2020  o optimize..    
+0000c140: 2020 2020 2020 2020 6e3a 2054 6865 206e          n: The n
+0000c150: 756d 6265 7220 6f66 2069 6e74 6572 6163  umber of interac
+0000c160: 7469 6f6e 7320 7765 2077 6973 6820 746f  tions we wish to
+0000c170: 2063 6f6e 7369 6465 722e 0a20 2020 2020   consider..     
+0000c180: 2020 2020 2020 2066 756c 6c5f 6c3a 2054         full_l: T
+0000c190: 6865 2074 7275 6520 6c6f 7765 7374 206c  he true lowest l
+0000c1a0: 6576 656c 206c 6162 656c 2028 652e 672e  evel label (e.g.
+0000c1b0: 2c20 6c65 6172 6e65 725f 6964 290a 2020  , learner_id).  
+0000c1c0: 2020 2020 2020 2020 2020 6675 6c6c 5f70            full_p
+0000c1d0: 3a20 5468 6520 7472 7565 206c 6f77 6573  : The true lowes
+0000c1e0: 7420 6c65 7665 6c20 7061 6972 2028 652e  t level pair (e.
+0000c1f0: 672e 2c20 656e 7669 726f 6e6d 656e 745f  g., environment_
+0000c200: 6964 290a 0a20 2020 2020 2020 2052 6574  id)..        Ret
+0000c210: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+0000c220: 2020 4120 5265 7375 6c74 2077 6974 6820    A Result with 
+0000c230: 6675 6c6c 2060 6c60 2061 6e64 2060 7060  full `l` and `p`
+0000c240: 2074 6861 7420 6973 2074 6865 206f 7074   that is the opt
+0000c250: 696d 616c 206f 7665 720a 2020 2020 2020  imal over.      
+0000c260: 2020 2020 2020 2020 2020 6066 756c 6c5f            `full_
+0000c270: 6c60 2061 6e64 2060 6675 6c6c 5f70 602e  l` and `full_p`.
+0000c280: 2046 6f72 2065 7861 6d70 6c65 2077 6520   For example we 
+0000c290: 636f 756c 6420 7361 7920 606c 600a 2020  could say `l`.  
+0000c2a0: 2020 2020 2020 2020 2020 2020 2020 6973                is
+0000c2b0: 2027 6661 6d69 6c79 2720 7768 696c 6520   'family' while 
+0000c2c0: 6066 756c 6c5f 6c60 2069 7320 276c 6561  `full_l` is 'lea
+0000c2d0: 726e 6572 5f69 6427 2e20 5468 6973 2077  rner_id'. This w
+0000c2e0: 6f75 6c64 0a20 2020 2020 2020 2020 2020  ould.           
+0000c2f0: 2020 2020 2070 6963 6b20 7468 6520 6265       pick the be
+0000c300: 7374 2070 6572 666f 726d 696e 6720 6c65  st performing le
+0000c310: 6172 6e65 7220 6772 6f75 7065 6420 6279  arner grouped by
+0000c320: 2066 616d 696c 7920 666f 720a 2020 2020   family for.    
+0000c330: 2020 2020 2020 2020 2020 2020 6561 6368              each
+0000c340: 2060 7060 2e0a 0a20 2020 2020 2020 2022   `p`...        "
+0000c350: 2222 0a0a 2020 2020 2020 2020 7265 7475  ""..        retu
+0000c360: 726e 2073 656c 662e 6669 6c74 6572 5f62  rn self.filter_b
+0000c370: 6573 7428 6c2c 702c 792c 6e2c 6675 6c6c  est(l,p,y,n,full
+0000c380: 5f6c 2c66 756c 6c5f 7029 0a0a 2020 2020  _l,full_p)..    
+0000c390: 6465 6620 7768 6572 655f 6669 6e28 7365  def where_fin(se
+0000c3a0: 6c66 2c0a 2020 2020 2020 2020 6e3a 2055  lf,.        n: U
+0000c3b0: 6e69 6f6e 5b69 6e74 2c4c 6974 6572 616c  nion[int,Literal
+0000c3c0: 5b27 6d69 6e27 5d5d 203d 204e 6f6e 652c  ['min']] = None,
+0000c3d0: 0a20 2020 2020 2020 206c 3a20 556e 696f  .        l: Unio
+0000c3e0: 6e5b 7374 722c 2053 6571 7565 6e63 655b  n[str, Sequence[
+0000c3f0: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
+0000c400: 2020 2020 2020 703a 2055 6e69 6f6e 5b73        p: Union[s
+0000c410: 7472 2c20 5365 7175 656e 6365 5b73 7472  tr, Sequence[str
+0000c420: 5d5d 203d 204e 6f6e 6529 202d 3e20 2752  ]] = None) -> 'R
+0000c430: 6573 756c 7427 3a0a 2020 2020 2020 2020  esult':.        
+0000c440: 2222 2246 696c 7465 7220 7468 6520 7265  """Filter the re
+0000c450: 7375 6c74 7320 646f 776e 2074 6f20 6576  sults down to ev
+0000c460: 656e 206f 7574 636f 6d65 7320 736f 2074  en outcomes so t
+0000c470: 6861 7420 706c 6f74 7465 6420 7265 7375  hat plotted resu
+0000c480: 6c74 7320 7769 6c6c 2062 6520 6d65 616e  lts will be mean
+0000c490: 696e 6766 756c 2e0a 0a20 2020 2020 2020  ingful...       
+0000c4a0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0000c4b0: 2020 206e 3a20 5468 6520 6e75 6d62 6572     n: The number
+0000c4c0: 206f 6620 696e 7465 7261 6374 696f 6e73   of interactions
+0000c4d0: 2061 2073 7065 6369 6669 6320 6576 616c   a specific eval
+0000c4e0: 7561 7469 6f6e 206d 7573 7420 6861 7665  uation must have
+0000c4f0: 2028 4e6f 6e65 2069 6e64 6963 6174 6573   (None indicates
+0000c500: 206e 6f20 636f 6e73 7472 6169 6e74 292e   no constraint).
+0000c510: 0a20 2020 2020 2020 2020 2020 206c 3a20  .            l: 
+0000c520: 5468 6520 6c65 7665 6c20 6174 2077 6869  The level at whi
+0000c530: 6368 2077 6520 7769 7368 2074 6f20 636f  ch we wish to co
+0000c540: 6d70 6172 6520 6576 616c 6174 696f 6e20  mpare evalation 
+0000c550: 6f75 7463 6f6d 6573 2028 652e 672e 2c20  outcomes (e.g., 
+0000c560: 276c 6561 726e 6572 5f69 6427 292e 0a20  'learner_id').. 
+0000c570: 2020 2020 2020 2020 2020 2070 3a20 5468             p: Th
+0000c580: 6520 7061 6972 7320 7468 6174 206d 7573  e pairs that mus
+0000c590: 7420 6578 6973 7420 6163 726f 7373 2061  t exist across a
+0000c5a0: 6c6c 2060 6c60 2069 6e20 6f72 6465 7220  ll `l` in order 
+0000c5b0: 746f 2062 6520 696e 636c 7564 6564 2028  to be included (
+0000c5c0: 652e 672e 2c20 2765 6e76 6972 6f6e 6d65  e.g., 'environme
+0000c5d0: 6e74 5f69 6427 292e 0a0a 2020 2020 2020  nt_id')...      
+0000c5e0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0000c5f0: 2020 2020 2020 2041 2060 5265 7375 6c74         A `Result
+0000c600: 6020 7768 6572 6520 616e 2060 6c60 2065  ` where an `l` e
+0000c610: 7869 7374 7320 666f 7220 6576 6572 7920  xists for every 
+0000c620: 6070 6020 616e 6420 616c 6c20 6070 6020  `p` and all `p` 
+0000c630: 6861 7665 2027 6e27 2069 6e74 6572 6163  have 'n' interac
+0000c640: 7469 6f6e 732e 0a20 2020 2020 2020 2022  tions..        "
+0000c650: 2222 0a0a 2020 2020 2020 2020 7265 7475  ""..        retu
+0000c660: 726e 2073 656c 662e 6669 6c74 6572 5f66  rn self.filter_f
+0000c670: 696e 286e 2c6c 2c70 290a 0a20 2020 2064  in(n,l,p)..    d
+0000c680: 6566 2077 6865 7265 2873 656c 662c 202a  ef where(self, *
+0000c690: 2a6b 7761 7267 7329 202d 3e20 2752 6573  *kwargs) -> 'Res
+0000c6a0: 756c 7427 3a0a 2020 2020 2020 2020 2222  ult':.        ""
+0000c6b0: 2253 656c 6563 7420 6c65 6172 6e65 7273  "Select learners
+0000c6c0: 2f65 6e76 6972 6f6e 6d65 6e74 732f 6576  /environments/ev
+0000c6d0: 616c 7561 746f 7273 2e0a 0a20 2020 2020  aluators...     
+0000c6e0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000c6f0: 2020 2020 206b 7761 7267 733a 2041 6e79       kwargs: Any
+0000c700: 2063 6f6c 756d 6e20 696e 2065 6e76 6972   column in envir
+0000c710: 6f6e 6d65 6e74 732c 206c 6561 726e 6572  onments, learner
+0000c720: 732c 2061 6e64 2065 7661 6c75 6174 6f72  s, and evaluator
+0000c730: 7320 746f 2066 696c 7465 7220 6f6e 2e20  s to filter on. 
+0000c740: 4279 0a20 2020 2020 2020 2020 2020 2020  By.             
+0000c750: 2020 2064 6566 6175 6c74 2063 6f6d 7061     default compa
+0000c760: 7269 736f 6e20 6f70 6572 6174 6f72 7320  rison operators 
+0000c770: 6172 6520 6569 7468 6572 2027 6571 7561  are either 'equa
+0000c780: 6c27 206f 7220 2769 6e27 2e20 466f 7220  l' or 'in'. For 
+0000c790: 6578 616d 706c 652c 0a20 2020 2020 2020  example,.       
+0000c7a0: 2020 2020 2020 2020 2077 6865 7265 2865           where(e
+0000c7b0: 6e76 6972 6f6e 6d65 6e74 5f69 643d 3129  nvironment_id=1)
+0000c7c0: 2077 6f75 6c64 2072 6574 7572 6e20 6120   would return a 
+0000c7d0: 5265 7375 6c74 2077 6865 7265 2065 6e76  Result where env
+0000c7e0: 6972 6f6e 6d65 6e74 7320 6f6e 6c79 2063  ironments only c
+0000c7f0: 6f6e 7461 696e 730a 2020 2020 2020 2020  ontains.        
+0000c800: 2020 2020 2020 2020 656e 7669 726f 6e6d          environm
+0000c810: 656e 745f 6964 2031 2e20 4f6e 2074 6865  ent_id 1. On the
+0000c820: 206f 7468 6572 2068 616e 6420 7768 6572   other hand wher
+0000c830: 6528 656e 7669 726f 6e6d 656e 745f 6964  e(environment_id
+0000c840: 3d5b 312c 325d 2920 776f 756c 6420 7265  =[1,2]) would re
+0000c850: 7475 726e 2061 0a20 2020 2020 2020 2020  turn a.         
+0000c860: 2020 2020 2020 2052 6573 756c 7420 7768         Result wh
+0000c870: 6572 6520 656e 7669 726f 6e6d 656e 7473  ere environments
+0000c880: 2063 6f6e 7461 696e 7320 656e 7669 726f   contains enviro
+0000c890: 6e6d 656e 745f 6964 2031 2061 6e64 2032  nment_id 1 and 2
+0000c8a0: 2e20 5468 6520 6b65 7977 6f72 6473 206d  . The keywords m
+0000c8b0: 7573 740a 2020 2020 2020 2020 2020 2020  ust.            
+0000c8c0: 2020 2020 696e 6469 6361 7465 2061 2063      indicate a c
+0000c8d0: 6f6c 756d 6e20 6e61 6d65 2069 6e20 6569  olumn name in ei
+0000c8e0: 7468 6572 2065 6e76 6972 6f6e 6d65 6e74  ther environment
+0000c8f0: 732c 206c 6561 726e 6572 732c 2065 7661  s, learners, eva
+0000c900: 6c75 6174 6f72 732c 206f 720a 2020 2020  luators, or.    
+0000c910: 2020 2020 2020 2020 2020 2020 696e 7465              inte
+0000c920: 7261 6374 696f 6e73 2e20 5375 7070 6f72  ractions. Suppor
+0000c930: 7465 6420 636f 6d70 6172 6973 6f6e 206f  ted comparison o
+0000c940: 7065 7261 746f 7273 2061 7265 2027 3d27  perators are '='
+0000c950: 2c27 213d 272c 273c 3d27 2c27 3c27 2c27  ,'!=','<=','<','
+0000c960: 3e27 2c27 3e3d 272c 0a20 2020 2020 2020  >','>=',.       
+0000c970: 2020 2020 2020 2020 2027 6d61 7463 6827           'match'
+0000c980: 2c27 696e 272c 2721 696e 272e 2054 6f20  ,'in','!in'. To 
+0000c990: 696e 6469 6361 7465 2061 6e20 6578 706c  indicate an expl
+0000c9a0: 6963 6974 206f 7065 7261 746f 7220 7573  icit operator us
+0000c9b0: 6520 6120 6469 6374 696f 6e61 7279 2e20  e a dictionary. 
+0000c9c0: 466f 720a 2020 2020 2020 2020 2020 2020  For.            
+0000c9d0: 2020 2020 6578 616d 706c 652c 2077 6865      example, whe
+0000c9e0: 7265 2865 6e76 6972 6f6e 6d65 6e74 5f69  re(environment_i
+0000c9f0: 643d 7b27 3c3d 273a 3130 307d 2920 776f  d={'<=':100}) wo
+0000ca00: 756c 6420 7265 7475 726e 2061 2052 6573  uld return a Res
+0000ca10: 756c 7420 7769 7468 2061 6c6c 0a20 2020  ult with all.   
+0000ca20: 2020 2020 2020 2020 2020 2020 2065 6e76               env
+0000ca30: 6972 6f6e 6d65 6e74 7320 7768 6f73 6520  ironments whose 
+0000ca40: 656e 7669 726f 6e6d 656e 745f 6964 203c  environment_id <
+0000ca50: 3d20 3130 302e 2049 6e63 6c75 6469 6e67  = 100. Including
+0000ca60: 206d 756c 7469 706c 6520 6b77 6172 6773   multiple kwargs
+0000ca70: 2069 6e20 610a 2020 2020 2020 2020 2020   in a.          
+0000ca80: 2020 2020 2020 7369 6e67 6c65 2077 6865        single whe
+0000ca90: 7265 2061 7070 6c69 6573 2061 6e20 6f72  re applies an or
+0000caa0: 2063 6f6e 6a75 6374 696f 6e2e 2043 6861   conjuction. Cha
+0000cab0: 696e 696e 6720 7768 6572 6520 7374 6174  ining where stat
+0000cac0: 656d 656e 7473 2069 7320 6571 7569 7661  ements is equiva
+0000cad0: 6c65 6e74 0a20 2020 2020 2020 2020 2020  lent.           
+0000cae0: 2020 2020 2074 6f20 616e 2061 6e64 2063       to an and c
+0000caf0: 6f6e 6a75 6374 6f72 2e0a 0a20 2020 2020  onjuctor...     
+0000cb00: 2020 2052 6575 7472 6e73 3a0a 2020 2020     Reutrns:.    
+0000cb10: 2020 2020 2020 2020 4120 6052 6573 756c          A `Resul
+0000cb20: 7460 2077 686f 7365 2065 6e76 6972 6f6e  t` whose environ
+0000cb30: 6d65 6e74 732c 206c 6561 726e 6572 732c  ments, learners,
+0000cb40: 2065 7661 6c75 6174 6f72 732c 2061 6e64   evaluators, and
+0000cb50: 2069 6e74 6572 6163 7469 6f6e 7320 7361   interactions sa
+0000cb60: 7469 7366 7920 7468 650a 2020 2020 2020  tisfy the.      
+0000cb70: 2020 2020 2020 2020 2020 7768 6572 6520            where 
+0000cb80: 7365 6c65 6374 6f72 732e 0a20 2020 2020  selectors..     
+0000cb90: 2020 2022 2222 0a20 2020 2020 2020 2065     """.        e
+0000cba0: 6e76 5f6b 7761 7267 7320 3d20 7b7d 0a20  nv_kwargs = {}. 
+0000cbb0: 2020 2020 2020 206c 726e 5f6b 7761 7267         lrn_kwarg
+0000cbc0: 7320 3d20 7b7d 0a20 2020 2020 2020 2076  s = {}.        v
+0000cbd0: 616c 5f6b 7761 7267 7320 3d20 7b7d 0a20  al_kwargs = {}. 
+0000cbe0: 2020 2020 2020 2069 6e74 5f6b 7761 7267         int_kwarg
+0000cbf0: 7320 3d20 7b7d 0a0a 2020 2020 2020 2020  s = {}..        
+0000cc00: 666f 7220 6b65 792c 6172 6720 696e 206b  for key,arg in k
+0000cc10: 7761 7267 732e 6974 656d 7328 293a 0a20  wargs.items():. 
+0000cc20: 2020 2020 2020 2020 2020 2069 6620 6b65             if ke
+0000cc30: 7920 696e 2073 656c 662e 656e 7669 726f  y in self.enviro
+0000cc40: 6e6d 656e 7473 2e63 6f6c 756d 6e73 3a0a  nments.columns:.
+0000cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc60: 656e 765f 6b77 6172 6773 5b6b 6579 5d20  env_kwargs[key] 
+0000cc70: 3d20 6172 670a 2020 2020 2020 2020 2020  = arg.          
+0000cc80: 2020 656c 6966 206b 6579 2069 6e20 7365    elif key in se
+0000cc90: 6c66 2e6c 6561 726e 6572 732e 636f 6c75  lf.learners.colu
+0000cca0: 6d6e 733a 0a20 2020 2020 2020 2020 2020  mns:.           
+0000ccb0: 2020 2020 206c 726e 5f6b 7761 7267 735b       lrn_kwargs[
+0000ccc0: 6b65 795d 203d 2061 7267 0a20 2020 2020  key] = arg.     
+0000ccd0: 2020 2020 2020 2065 6c69 6620 6b65 7920         elif key 
+0000cce0: 696e 2073 656c 662e 6576 616c 7561 746f  in self.evaluato
+0000ccf0: 7273 2e63 6f6c 756d 6e73 3a0a 2020 2020  rs.columns:.    
+0000cd00: 2020 2020 2020 2020 2020 2020 7661 6c5f              val_
+0000cd10: 6b77 6172 6773 5b6b 6579 5d20 3d20 6172  kwargs[key] = ar
+0000cd20: 670a 2020 2020 2020 2020 2020 2020 656c  g.            el
+0000cd30: 6966 206b 6579 2069 6e20 7365 6c66 2e69  if key in self.i
+0000cd40: 6e74 6572 6163 7469 6f6e 732e 636f 6c75  nteractions.colu
+0000cd50: 6d6e 733a 0a20 2020 2020 2020 2020 2020  mns:.           
+0000cd60: 2020 2020 2069 6e74 5f6b 7761 7267 735b       int_kwargs[
+0000cd70: 6b65 795d 203d 2061 7267 0a20 2020 2020  key] = arg.     
+0000cd80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000cd90: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+0000cda0: 7365 2043 6f62 6145 7863 6570 7469 6f6e  se CobaException
+0000cdb0: 2822 416e 2075 6e72 6563 6f67 6e69 7a65  ("An unrecognize
+0000cdc0: 6420 636f 6c75 6d6e 2077 6173 2070 726f  d column was pro
+0000cdd0: 7669 6465 6420 746f 2060 7768 6572 6560  vided to `where`
+0000cde0: 2066 6f72 2066 696c 7465 7269 6e67 2e22   for filtering."
+0000cdf0: 290a 0a20 2020 2020 2020 206f 7574 203d  )..        out =
+0000ce00: 2073 656c 660a 0a20 2020 2020 2020 2069   self..        i
+0000ce10: 6620 656e 765f 6b77 6172 6773 3a20 6f75  f env_kwargs: ou
+0000ce20: 7420 3d20 6f75 742e 6669 6c74 6572 5f65  t = out.filter_e
+0000ce30: 6e76 282a 2a65 6e76 5f6b 7761 7267 7329  nv(**env_kwargs)
+0000ce40: 0a20 2020 2020 2020 2069 6620 6c72 6e5f  .        if lrn_
+0000ce50: 6b77 6172 6773 3a20 6f75 7420 3d20 6f75  kwargs: out = ou
+0000ce60: 742e 6669 6c74 6572 5f6c 726e 282a 2a6c  t.filter_lrn(**l
+0000ce70: 726e 5f6b 7761 7267 7329 0a20 2020 2020  rn_kwargs).     
+0000ce80: 2020 2069 6620 7661 6c5f 6b77 6172 6773     if val_kwargs
+0000ce90: 3a20 6f75 7420 3d20 6f75 742e 6669 6c74  : out = out.filt
+0000cea0: 6572 5f76 616c 282a 2a76 616c 5f6b 7761  er_val(**val_kwa
+0000ceb0: 7267 7329 0a20 2020 2020 2020 2069 6620  rgs).        if 
+0000cec0: 696e 745f 6b77 6172 6773 3a20 6f75 7420  int_kwargs: out 
+0000ced0: 3d20 6f75 742e 6669 6c74 6572 5f69 6e74  = out.filter_int
+0000cee0: 282a 2a69 6e74 5f6b 7761 7267 7329 0a0a  (**int_kwargs)..
+0000cef0: 2020 2020 2020 2020 7265 7475 726e 206f          return o
+0000cf00: 7574 0a0a 2020 2020 6465 6620 7261 775f  ut..    def raw_
+0000cf10: 6c65 6172 6e65 7273 2873 656c 662c 0a20  learners(self,. 
+0000cf20: 2020 2020 2020 2078 2020 203a 2055 6e69         x   : Uni
+0000cf30: 6f6e 5b73 7472 2c20 5365 7175 656e 6365  on[str, Sequence
+0000cf40: 5b73 7472 5d5d 203d 2027 696e 6465 7827  [str]] = 'index'
+0000cf50: 2c0a 2020 2020 2020 2020 7920 2020 3a20  ,.        y   : 
+0000cf60: 7374 7220 2020 2020 2020 2020 2020 2020  str             
+0000cf70: 2020 2020 2020 2020 2020 3d20 2772 6577            = 'rew
+0000cf80: 6172 6427 2c0a 2020 2020 2020 2020 6c20  ard',.        l 
+0000cf90: 2020 3a20 556e 696f 6e5b 7374 722c 2053    : Union[str, S
+0000cfa0: 6571 7565 6e63 655b 7374 725d 5d20 3d20  equence[str]] = 
+0000cfb0: 2766 756c 6c5f 6e61 6d65 272c 0a20 2020  'full_name',.   
+0000cfc0: 2020 2020 2070 2020 203a 2055 6e69 6f6e       p   : Union
+0000cfd0: 5b73 7472 2c20 5365 7175 656e 6365 5b73  [str, Sequence[s
+0000cfe0: 7472 5d5d 203d 2027 656e 7669 726f 6e6d  tr]] = 'environm
+0000cff0: 656e 745f 6964 272c 0a20 2020 2020 2020  ent_id',.       
+0000d000: 2073 7061 6e3a 2069 6e74 203d 204e 6f6e   span: int = Non
+0000d010: 6529 202d 3e20 5461 626c 653a 0a20 2020  e) -> Table:.   
+0000d020: 2020 2020 2022 2222 4120 5461 626c 6520       """A Table 
+0000d030: 7769 7468 2074 6865 2072 6177 2064 6174  with the raw dat
+0000d040: 6120 7573 6564 2066 6f72 2070 6c6f 745f  a used for plot_
+0000d050: 6c65 6172 6e65 7273 2e0a 0a20 2020 2020  learners...     
+0000d060: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000d070: 2020 2020 2078 3a20 5468 6520 7661 7269       x: The vari
+0000d080: 6162 6c65 7320 746f 2070 6c6f 7420 6f6e  ables to plot on
+0000d090: 2074 6865 2078 2d61 7869 732e 0a20 2020   the x-axis..   
+0000d0a0: 2020 2020 2020 2020 2079 3a20 5468 6520           y: The 
+0000d0b0: 7661 7269 6162 6c65 2074 6f20 706c 6f74  variable to plot
+0000d0c0: 206f 6e20 7468 6520 792d 6178 6973 2e0a   on the y-axis..
+0000d0d0: 2020 2020 2020 2020 2020 2020 6c3a 2054              l: T
+0000d0e0: 6865 206c 6162 656c 7320 746f 2075 7365  he labels to use
+0000d0f0: 2069 6e20 7468 6520 706c 6f74 206c 6567   in the plot leg
+0000d100: 656e 642e 0a20 2020 2020 2020 2020 2020  end..           
+0000d110: 2070 3a20 5468 6520 7061 6972 696e 6773   p: The pairings
+0000d120: 2074 6f20 7265 7175 6972 6520 6163 726f   to require acro
+0000d130: 7373 2061 6c6c 206c 2e20 4966 204e 6f6e  ss all l. If Non
+0000d140: 6520 6e6f 2070 6169 7269 6e67 2063 6865  e no pairing che
+0000d150: 636b 7320 6172 6520 7065 7266 6f72 6d65  cks are performe
+0000d160: 642e 0a20 2020 2020 2020 2020 2020 2073  d..            s
+0000d170: 7061 6e3a 2054 6865 2073 697a 6520 6f66  pan: The size of
+0000d180: 2074 6865 2072 6f6c 6c69 6e67 2061 7665   the rolling ave
+0000d190: 7261 6765 2028 4e6f 6e65 206d 6561 6e73  rage (None means
+0000d1a0: 2070 726f 6772 6573 7369 7665 206d 6561   progressive mea
+0000d1b0: 6e2e 290a 0a20 2020 2020 2020 2052 6575  n.)..        Reu
+0000d1c0: 7472 6e73 3a0a 2020 2020 2020 2020 2020  trns:.          
+0000d1d0: 2020 4120 5461 626c 6520 7769 7468 2074    A Table with t
+0000d1e0: 6865 2072 6177 2064 6174 6120 7573 6564  he raw data used
+0000d1f0: 2074 6f20 636f 6e73 7472 7563 7420 706c   to construct pl
+0000d200: 6f74 5f6c 6561 726e 6572 732e 0a20 2020  ot_learners..   
+0000d210: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+0000d220: 2020 6966 2070 3a20 706c 6f74 7461 626c    if p: plottabl
+0000d230: 6520 3d20 7365 6c66 2e5f 706c 6f74 7461  e = self._plotta
+0000d240: 626c 6528 782c 7929 2e5f 6669 6e69 7368  ble(x,y)._finish
+0000d250: 6564 2878 2c79 2c6c 2c70 290a 2020 2020  ed(x,y,l,p).    
+0000d260: 2020 2020 656c 7365 3a20 706c 6f74 7461      else: plotta
+0000d270: 626c 6520 3d20 7365 6c66 2e5f 706c 6f74  ble = self._plot
+0000d280: 7461 626c 6528 782c 7929 0a0a 2020 2020  table(x,y)..    
+0000d290: 2020 2020 726f 7773 203d 2070 6c6f 7474      rows = plott
+0000d2a0: 6162 6c65 2e5f 6772 6f75 7065 645f 7973  able._grouped_ys
+0000d2b0: 286c 2c78 2c79 3d79 2c73 7061 6e3d 7370  (l,x,y=y,span=sp
+0000d2c0: 616e 290a 0a20 2020 2020 2020 2058 7320  an)..        Xs 
+0000d2d0: 3d20 7365 7428 6d61 7028 6974 656d 6765  = set(map(itemge
+0000d2e0: 7474 6572 2831 292c 726f 7773 2929 0a0a  tter(1),rows))..
+0000d2f0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+0000d300: 2020 2020 2020 2020 2058 7320 3d20 6469           Xs = di
+0000d310: 6374 287a 6970 2873 6f72 7465 6428 5873  ct(zip(sorted(Xs
+0000d320: 292c 636f 756e 7428 2929 290a 2020 2020  ),count())).    
+0000d330: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
+0000d340: 2020 2020 2020 2020 5873 203d 2064 6963          Xs = dic
+0000d350: 7428 7a69 7028 736f 7274 6564 2858 732c  t(zip(sorted(Xs,
+0000d360: 6b65 793d 7374 7229 2c63 6f75 6e74 2829  key=str),count()
+0000d370: 2929 0a0a 2020 2020 2020 2020 7472 793a  ))..        try:
+0000d380: 0a20 2020 2020 2020 2020 2020 2072 6f77  .            row
+0000d390: 7320 3d20 736f 7274 6564 2872 6f77 7329  s = sorted(rows)
+0000d3a0: 0a20 2020 2020 2020 2065 7863 6570 743a  .        except:
+0000d3b0: 0a20 2020 2020 2020 2020 2020 2073 6f72  .            sor
+0000d3c0: 7465 645f 203d 2046 616c 7365 0a20 2020  ted_ = False.   
+0000d3d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000d3e0: 2020 2020 2020 2073 6f72 7465 645f 203d         sorted_ =
+0000d3f0: 2054 7275 650a 0a20 2020 2020 2020 2064   True..        d
+0000d400: 6174 6120 3d20 7b27 7827 3a20 6c69 7374  ata = {'x': list
+0000d410: 2858 732e 6b65 7973 2829 297d 0a20 2020  (Xs.keys())}.   
+0000d420: 2020 2020 2066 6f72 205f 6c2c 2067 726f       for _l, gro
+0000d430: 7570 2069 6e20 6772 6f75 7065 7228 726f  up in grouper(ro
+0000d440: 7773 2c20 6b65 793d 6974 656d 6765 7474  ws, key=itemgett
+0000d450: 6572 2830 292c 2076 616c 3d69 7465 6d67  er(0), val=itemg
+0000d460: 6574 7465 7228 736c 6963 6528 312c 4e6f  etter(slice(1,No
+0000d470: 6e65 2929 2c20 736f 7274 6564 5f3d 736f  ne)), sorted_=so
+0000d480: 7274 6564 5f29 3a0a 2020 2020 2020 2020  rted_):.        
+0000d490: 2020 2020 5920 3d20 5b5b 666c 6f61 7428      Y = [[float(
+0000d4a0: 276e 616e 2729 5d5d 2a6c 656e 2858 7329  'nan')]]*len(Xs)
+0000d4b0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000d4c0: 205f 782c 2067 726f 7570 2069 6e20 6772   _x, group in gr
+0000d4d0: 6f75 7065 7228 6772 6f75 702c 206b 6579  ouper(group, key
+0000d4e0: 3d69 7465 6d67 6574 7465 7228 3029 2c20  =itemgetter(0), 
+0000d4f0: 7661 6c3d 6974 656d 6765 7474 6572 2831  val=itemgetter(1
+0000d500: 292c 2073 6f72 7465 645f 3d73 6f72 7465  ), sorted_=sorte
+0000d510: 645f 293a 0a20 2020 2020 2020 2020 2020  d_):.           
+0000d520: 2020 2020 2059 5b58 735b 5f78 5d5d 203d       Y[Xs[_x]] =
+0000d530: 206c 6973 7428 6368 6169 6e2e 6672 6f6d   list(chain.from
+0000d540: 5f69 7465 7261 626c 6528 6772 6f75 7029  _iterable(group)
+0000d550: 290a 2020 2020 2020 2020 2020 2020 6461  ).            da
+0000d560: 7461 5b5f 6c5d 203d 2059 0a20 2020 2020  ta[_l] = Y.     
+0000d570: 2020 2072 6574 7572 6e20 5461 626c 6528     return Table(
+0000d580: 6461 7461 290a 0a20 2020 2064 6566 2072  data)..    def r
+0000d590: 6177 5f63 6f6e 7472 6173 7428 7365 6c66  aw_contrast(self
+0000d5a0: 2c0a 2020 2020 2020 2020 6c31 2020 3a20  ,.        l1  : 
+0000d5b0: 416e 792c 0a20 2020 2020 2020 206c 3220  Any,.        l2 
+0000d5c0: 203a 2041 6e79 2c0a 2020 2020 2020 2020   : Any,.        
+0000d5d0: 7820 2020 3a20 556e 696f 6e5b 7374 722c  x   : Union[str,
+0000d5e0: 2053 6571 7565 6e63 655b 7374 725d 5d20   Sequence[str]] 
+0000d5f0: 3d20 2765 6e76 6972 6f6e 6d65 6e74 5f69  = 'environment_i
+0000d600: 6427 2c0a 2020 2020 2020 2020 7920 2020  d',.        y   
+0000d610: 3a20 7374 7220 2020 2020 2020 2020 2020  : str           
+0000d620: 2020 2020 2020 2020 2020 2020 3d20 2772              = 'r
+0000d630: 6577 6172 6427 2c0a 2020 2020 2020 2020  eward',.        
+0000d640: 6c20 2020 3a20 556e 696f 6e5b 7374 722c  l   : Union[str,
+0000d650: 2053 6571 7565 6e63 655b 7374 725d 5d20   Sequence[str]] 
+0000d660: 3d20 276c 6561 726e 6572 5f69 6427 2c0a  = 'learner_id',.
+0000d670: 2020 2020 2020 2020 7020 2020 3a20 556e          p   : Un
+0000d680: 696f 6e5b 7374 722c 2053 6571 7565 6e63  ion[str, Sequenc
+0000d690: 655b 7374 725d 5d20 3d20 2765 6e76 6972  e[str]] = 'envir
+0000d6a0: 6f6e 6d65 6e74 5f69 6427 2c0a 2020 2020  onment_id',.    
+0000d6b0: 2020 2020 7370 616e 3a20 696e 7420 3d20      span: int = 
+0000d6c0: 4e6f 6e65 2920 2d3e 2054 6162 6c65 3a0a  None) -> Table:.
+0000d6d0: 2020 2020 2020 2020 2222 2241 2054 6162          """A Tab
+0000d6e0: 6c65 2077 6974 6820 7468 6520 7261 7720  le with the raw 
+0000d6f0: 6461 7461 2070 6c6f 745f 636f 6e74 7261  data plot_contra
+0000d700: 7374 2e0a 0a20 2020 2020 2020 2041 7267  st...        Arg
+0000d710: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
+0000d720: 313a 2054 6865 2066 6972 7374 2060 6c60  1: The first `l`
+0000d730: 2076 616c 7565 2074 6f20 636f 6e74 7261   value to contra
+0000d740: 7374 2e0a 2020 2020 2020 2020 2020 2020  st..            
+0000d750: 6c32 3a20 7468 6520 7365 636f 6e64 2060  l2: the second `
+0000d760: 6c60 2076 616c 7565 2074 6f20 636f 6e74  l` value to cont
+0000d770: 7261 7374 2e0a 2020 2020 2020 2020 2020  rast..          
+0000d780: 2020 783a 2054 6865 2076 6172 6961 626c    x: The variabl
+0000d790: 6573 2074 6f20 706c 6f74 206f 6e20 7468  es to plot on th
+0000d7a0: 6520 782d 6178 6973 2e0a 2020 2020 2020  e x-axis..      
+0000d7b0: 2020 2020 2020 793a 2054 6865 2076 6172        y: The var
+0000d7c0: 6961 626c 6520 746f 2070 6c6f 7420 6f6e  iable to plot on
+0000d7d0: 2074 6865 2079 2d61 7869 732e 0a20 2020   the y-axis..   
+0000d7e0: 2020 2020 2020 2020 206c 3a20 5468 6520           l: The 
+0000d7f0: 636f 6c75 6d6e 206e 616d 6573 2074 6861  column names tha
+0000d800: 7420 6c31 2061 6e64 206c 3220 7265 7072  t l1 and l2 repr
+0000d810: 6573 656e 742e 0a20 2020 2020 2020 2020  esent..         
+0000d820: 2020 2070 3a20 5468 6520 7061 6972 696e     p: The pairin
+0000d830: 6773 2074 6f20 7265 7175 6972 6520 6163  gs to require ac
+0000d840: 726f 7373 2061 6c6c 206c 3120 616e 6420  ross all l1 and 
+0000d850: 6c32 2e0a 2020 2020 2020 2020 2020 2020  l2..            
+0000d860: 7370 616e 3a20 5468 6520 7369 7a65 206f  span: The size o
+0000d870: 6620 7468 6520 726f 6c6c 696e 6720 6176  f the rolling av
+0000d880: 6572 6167 6520 284e 6f6e 6520 6d65 616e  erage (None mean
+0000d890: 7320 7072 6f67 7265 7373 6976 6520 6d65  s progressive me
+0000d8a0: 616e 292e 0a0a 2020 2020 2020 2020 4578  an)...        Ex
+0000d8b0: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
+0000d8c0: 2020 2020 7261 775f 636f 6e74 7261 7374      raw_contrast
+0000d8d0: 2831 2c32 2c78 3d27 656e 7669 726f 6e6d  (1,2,x='environm
+0000d8e0: 656e 745f 6964 272c 793d 2772 6577 6172  ent_id',y='rewar
+0000d8f0: 6427 2c6c 3d27 6c65 6172 6e65 725f 6964  d',l='learner_id
+0000d900: 272c 703d 2765 6e76 6972 6f6e 6d65 6e74  ',p='environment
+0000d910: 5f69 6427 290a 2020 2020 2020 2020 2020  _id').          
+0000d920: 2020 776f 756c 6420 636f 6e74 7261 7374    would contrast
+0000d930: 206c 6561 726e 6572 5f69 643d 3120 616e   learner_id=1 an
+0000d940: 6420 6c65 6172 6e65 725f 6964 3d32 2069  d learner_id=2 i
+0000d950: 6e20 7465 726d 7320 6f66 2072 6577 6172  n terms of rewar
+0000d960: 6420 6f6e 2061 6c6c 2065 6e76 6972 6f6e  d on all environ
+0000d970: 6d65 6e74 5f69 6473 2e0a 0a20 2020 2020  ment_ids...     
+0000d980: 2020 2052 6575 7472 6e73 3a0a 2020 2020     Reutrns:.    
+0000d990: 2020 2020 2020 2020 4120 5461 626c 6520          A Table 
+0000d9a0: 7769 7468 2074 6865 2072 6177 2064 6174  with the raw dat
+0000d9b0: 6120 7573 6564 2074 6f20 636f 6e73 7472  a used to constr
+0000d9c0: 7563 7420 706c 6f74 5f63 6f6e 7472 6173  uct plot_contras
+0000d9d0: 742e 0a20 2020 2020 2020 2022 2222 0a0a  t..        """..
+0000d9e0: 2020 2020 2020 2020 6f67 5f6c 203d 2028          og_l = (
+0000d9f0: 6c31 2c6c 3229 0a0a 2020 2020 2020 2020  l1,l2)..        
+0000da00: 6c69 7374 5f6c 696b 653d 286c 6973 742c  list_like=(list,
+0000da10: 7475 706c 6529 0a0a 2020 2020 2020 2020  tuple)..        
+0000da20: 6966 2020 2020 2069 7369 6e73 7461 6e63  if     isinstanc
+0000da30: 6528 6c2c 6c69 7374 5f6c 696b 6529 2061  e(l,list_like) a
+0000da40: 6e64 206e 6f74 2069 7369 6e73 7461 6e63  nd not isinstanc
+0000da50: 6528 6c31 5b30 5d2c 6c69 7374 5f6c 696b  e(l1[0],list_lik
+0000da60: 6529 3a20 6c31 203d 205b 6c31 5d0a 2020  e): l1 = [l1].  
+0000da70: 2020 2020 2020 6966 2020 2020 2069 7369        if     isi
+0000da80: 6e73 7461 6e63 6528 6c2c 6c69 7374 5f6c  nstance(l,list_l
+0000da90: 696b 6529 2061 6e64 206e 6f74 2069 7369  ike) and not isi
+0000daa0: 6e73 7461 6e63 6528 6c32 5b30 5d2c 6c69  nstance(l2[0],li
+0000dab0: 7374 5f6c 696b 6529 3a20 6c32 203d 205b  st_like): l2 = [
+0000dac0: 6c32 5d0a 2020 2020 2020 2020 6966 206e  l2].        if n
+0000dad0: 6f74 2069 7369 6e73 7461 6e63 6528 6c2c  ot isinstance(l,
+0000dae0: 6c69 7374 5f6c 696b 6529 2061 6e64 206e  list_like) and n
+0000daf0: 6f74 2069 7369 6e73 7461 6e63 6528 6c31  ot isinstance(l1
+0000db00: 2020 202c 6c69 7374 5f6c 696b 6529 3a20     ,list_like): 
+0000db10: 6c31 203d 205b 6c31 5d0a 2020 2020 2020  l1 = [l1].      
+0000db20: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
+0000db30: 6e63 6528 6c2c 6c69 7374 5f6c 696b 6529  nce(l,list_like)
+0000db40: 2061 6e64 206e 6f74 2069 7369 6e73 7461   and not isinsta
+0000db50: 6e63 6528 6c32 2020 202c 6c69 7374 5f6c  nce(l2   ,list_l
+0000db60: 696b 6529 3a20 6c32 203d 205b 6c32 5d0a  ike): l2 = [l2].
+0000db70: 0a20 2020 2020 2020 2069 6620 616e 7928  .        if any(
+0000db80: 5f6c 3120 696e 206c 3220 666f 7220 5f6c  _l1 in l2 for _l
+0000db90: 3120 696e 206c 3129 3a0a 2020 2020 2020  1 in l1):.      
+0000dba0: 2020 2020 2020 7261 6973 6520 436f 6261        raise Coba
+0000dbb0: 4578 6365 7074 696f 6e28 2241 2076 616c  Exception("A val
+0000dbc0: 7565 2063 616e 6e6f 7420 6265 2069 6e20  ue cannot be in 
+0000dbd0: 626f 7468 2060 6c31 6020 616e 6420 606c  both `l1` and `l
+0000dbe0: 3260 2e20 506c 6561 7365 206d 616b 6520  2`. Please make 
+0000dbf0: 6120 6368 616e 6765 2061 6e64 2072 756e  a change and run
+0000dc00: 2069 7420 6167 6169 6e2e 2229 0a0a 2020   it again.")..  
+0000dc10: 2020 2020 2020 706c 6f74 7461 626c 6520        plottable 
+0000dc20: 3d20 7365 6c66 2e5f 706c 6f74 7461 626c  = self._plottabl
+0000dc30: 6528 782c 7929 0a0a 2020 2020 2020 2020  e(x,y)..        
+0000dc40: 4c31 2c4c 3220 3d20 5b5d 2c5b 5d0a 2020  L1,L2 = [],[].  
+0000dc50: 2020 2020 2020 666f 7220 4c20 696e 2063        for L in c
+0000dc60: 6861 696e 286c 312c 6c32 293a 0a20 2020  hain(l1,l2):.   
+0000dc70: 2020 2020 2020 2020 2073 7562 706c 6f74           subplot
+0000dc80: 203d 2070 6c6f 7474 6162 6c65 0a20 2020   = plottable.   
+0000dc90: 2020 2020 2020 2020 2077 6865 7265 7320           wheres 
+0000dca0: 3d20 5b20 286c 2c4c 2920 5d20 6966 2069  = [ (l,L) ] if i
+0000dcb0: 7369 6e73 7461 6e63 6528 6c2c 7374 7229  sinstance(l,str)
+0000dcc0: 2065 6c73 6520 7a69 7028 6c2c 4c29 0a0a   else zip(l,L)..
+0000dcd0: 2020 2020 2020 2020 2020 2020 6f6c 645f              old_
+0000dce0: 6c6f 6767 6572 203d 2043 6f62 6143 6f6e  logger = CobaCon
+0000dcf0: 7465 7874 2e6c 6f67 6765 720a 2020 2020  text.logger.    
+0000dd00: 2020 2020 2020 2020 436f 6261 436f 6e74          CobaCont
+0000dd10: 6578 742e 6c6f 6767 6572 203d 204e 756c  ext.logger = Nul
+0000dd20: 6c4c 6f67 6765 7228 290a 2020 2020 2020  lLogger().      
+0000dd30: 2020 2020 2020 666f 7220 6c5f 2c76 5f20        for l_,v_ 
+0000dd40: 696e 2077 6865 7265 733a 2073 7562 706c  in wheres: subpl
+0000dd50: 6f74 203d 2073 7562 706c 6f74 2e77 6865  ot = subplot.whe
+0000dd60: 7265 282a 2a7b 6c5f 3a76 5f7d 290a 2020  re(**{l_:v_}).  
+0000dd70: 2020 2020 2020 2020 2020 436f 6261 436f            CobaCo
+0000dd80: 6e74 6578 742e 6c6f 6767 6572 203d 206f  ntext.logger = o
+0000dd90: 6c64 5f6c 6f67 6765 720a 0a20 2020 2020  ld_logger..     
+0000dda0: 2020 2020 2020 2023 7765 2061 7265 2061         #we are a
+0000ddb0: 7373 756d 696e 6720 6174 2074 6869 7320  ssuming at this 
+0000ddc0: 706f 696e 7420 7468 6174 206f 6e6c 7920  point that only 
+0000ddd0: 7661 6c69 640a 2020 2020 2020 2020 2020  valid.          
+0000dde0: 2020 2360 6c60 2061 7265 206c 6566 7420    #`l` are left 
+0000ddf0: 7768 6963 6820 6973 6e27 7420 6e65 6365  which isn't nece
+0000de00: 7373 6172 696c 7920 7468 6520 6361 7365  ssarily the case
+0000de10: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+0000de20: 7565 7320 3d20 7375 6270 6c6f 742e 5f67  ues = subplot._g
+0000de30: 726f 7570 6564 5f79 7328 702c 782c 793d  rouped_ys(p,x,y=
+0000de40: 792c 6361 7264 3d27 5327 2c73 7061 6e3d  y,card='S',span=
+0000de50: 7370 616e 290a 0a20 2020 2020 2020 2020  span)..         
+0000de60: 2020 2069 6620 4c20 696e 206c 313a 204c     if L in l1: L
+0000de70: 312e 6578 7465 6e64 2876 616c 7565 7329  1.extend(values)
+0000de80: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000de90: 6520 2020 2020 203a 204c 322e 6578 7465  e      : L2.exte
+0000dea0: 6e64 2876 616c 7565 7329 0a0a 2020 2020  nd(values)..    
+0000deb0: 2020 2020 2357 6520 6861 7665 2074 6f20      #We have to 
+0000dec0: 6d61 7465 7269 616c 697a 6520 6265 6361  materialize beca
+0000ded0: 7573 6520 7765 2063 616e 2774 2072 656c  use we can't rel
+0000dee0: 7920 6f6e 2073 6f72 7469 6e67 0a20 2020  y on sorting.   
+0000def0: 2020 2020 2050 3120 3d20 7b6b 3a6c 6973       P1 = {k:lis
+0000df00: 7428 7629 2066 6f72 206b 2c76 2069 6e20  t(v) for k,v in 
+0000df10: 6772 6f75 7065 7228 4c31 2c6b 6579 3d69  grouper(L1,key=i
+0000df20: 7465 6d67 6574 7465 7228 3029 297d 0a20  temgetter(0))}. 
+0000df30: 2020 2020 2020 2050 3220 3d20 7b6b 3a6c         P2 = {k:l
+0000df40: 6973 7428 7629 2066 6f72 206b 2c76 2069  ist(v) for k,v i
+0000df50: 6e20 6772 6f75 7065 7228 4c32 2c6b 6579  n grouper(L2,key
+0000df60: 3d69 7465 6d67 6574 7465 7228 3029 297d  =itemgetter(0))}
+0000df70: 0a0a 2020 2020 2020 2020 6465 6620 6d61  ..        def ma
+0000df80: 6b65 7828 7831 2c78 3229 3a20 7265 7475  kex(x1,x2): retu
+0000df90: 726e 2078 3120 6966 2078 3120 3d3d 2078  rn x1 if x1 == x
+0000dfa0: 3220 656c 7365 2066 227b 7832 7d2d 7b78  2 else f"{x2}-{x
+0000dfb0: 317d 220a 0a20 2020 2020 2020 2058 5920  1}"..        XY 
+0000dfc0: 3d20 6465 6661 756c 7464 6963 7428 6c69  = defaultdict(li
+0000dfd0: 7374 290a 2020 2020 2020 2020 666f 7220  st).        for 
+0000dfe0: 6b20 696e 2050 312e 6b65 7973 2829 2026  k in P1.keys() &
+0000dff0: 2050 322e 6b65 7973 2829 3a0a 2020 2020   P2.keys():.    
+0000e000: 2020 2020 2020 2020 6966 2078 203d 3d20          if x == 
+0000e010: 2769 6e64 6578 273a 0a20 2020 2020 2020  'index':.       
+0000e020: 2020 2020 2020 2020 2066 6f72 2067 315f           for g1_
+0000e030: 2c20 6732 5f20 696e 207a 6970 2850 315b  , g2_ in zip(P1[
+0000e040: 6b5d 2c50 325b 6b5d 293a 0a20 2020 2020  k],P2[k]):.     
+0000e050: 2020 2020 2020 2020 2020 2020 2020 2058                 X
+0000e060: 595b 6731 5f5b 315d 5d2e 6170 7065 6e64  Y[g1_[1]].append
+0000e070: 2828 6731 5f5b 325d 2c67 325f 5b32 5d29  ((g1_[2],g2_[2])
+0000e080: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000e090: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000e0a0: 2020 2020 666f 7220 6731 5f2c 6732 5f20      for g1_,g2_ 
+0000e0b0: 696e 2070 726f 6475 6374 2850 315b 6b5d  in product(P1[k]
+0000e0c0: 2c50 325b 6b5d 293a 0a20 2020 2020 2020  ,P2[k]):.       
+0000e0d0: 2020 2020 2020 2020 2020 2020 2058 595b               XY[
+0000e0e0: 6d61 6b65 7828 6731 5f5b 315d 2c67 325f  makex(g1_[1],g2_
+0000e0f0: 5b31 5d29 5d2e 6170 7065 6e64 2828 6731  [1])].append((g1
+0000e100: 5f5b 325d 2c67 325f 5b32 5d29 290a 0a20  _[2],g2_[2])).. 
+0000e110: 2020 2020 2020 2069 6620 6e6f 7420 5859         if not XY
+0000e120: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0000e130: 6973 6520 436f 6261 4578 6365 7074 696f  ise CobaExceptio
+0000e140: 6e28 6622 5765 2077 6572 6520 756e 6162  n(f"We were unab
+0000e150: 6c65 2074 6f20 6372 6561 7465 2061 6e79  le to create any
+0000e160: 2070 6169 7269 6e67 7320 746f 2063 6f6e   pairings to con
+0000e170: 7472 6173 742e 204d 616b 6520 7375 7265  trast. Make sure
+0000e180: 206c 313d 7b6f 675f 6c5b 305d 7d20 616e   l1={og_l[0]} an
+0000e190: 6420 6c32 3d7b 6f67 5f6c 5b31 5d7d 2069  d l2={og_l[1]} i
+0000e1a0: 7320 636f 7272 6563 742e 2229 0a0a 2020  s correct.")..  
+0000e1b0: 2020 2020 2020 6c31 5f6c 6162 656c 203d        l1_label =
+0000e1c0: 2073 656c 662e 5f6c 726e 5f63 6163 6865   self._lrn_cache
+0000e1d0: 5b6c 315b 305d 5d5b 2766 756c 6c5f 6e61  [l1[0]]['full_na
+0000e1e0: 6d65 275d 2069 6620 6c3d 3d27 6c65 6172  me'] if l=='lear
+0000e1f0: 6e65 725f 6964 2720 656c 7365 2027 6c31  ner_id' else 'l1
+0000e200: 270a 2020 2020 2020 2020 6c32 5f6c 6162  '.        l2_lab
+0000e210: 656c 203d 2073 656c 662e 5f6c 726e 5f63  el = self._lrn_c
+0000e220: 6163 6865 5b6c 325b 305d 5d5b 2766 756c  ache[l2[0]]['ful
+0000e230: 6c5f 6e61 6d65 275d 2069 6620 6c3d 3d27  l_name'] if l=='
+0000e240: 6c65 6172 6e65 725f 6964 2720 656c 7365  learner_id' else
+0000e250: 2027 6c32 270a 0a20 2020 2020 2020 2058   'l2'..        X
+0000e260: 2c59 203d 207a 6970 282a 736f 7274 6564  ,Y = zip(*sorted
+0000e270: 2858 592e 6974 656d 7328 2929 290a 0a20  (XY.items())).. 
+0000e280: 2020 2020 2020 2072 6574 7572 6e20 5461         return Ta
+0000e290: 626c 6528 7b27 7827 3a20 582c 2028 6c31  ble({'x': X, (l1
+0000e2a0: 5f6c 6162 656c 2c6c 325f 6c61 6265 6c29  _label,l2_label)
+0000e2b0: 3a20 5920 7d29 0a0a 2020 2020 6465 6620  : Y })..    def 
+0000e2c0: 706c 6f74 5f6c 6561 726e 6572 7328 7365  plot_learners(se
+0000e2d0: 6c66 2c0a 2020 2020 2020 2020 7820 2020  lf,.        x   
+0000e2e0: 2020 2020 3a20 556e 696f 6e5b 7374 722c      : Union[str,
+0000e2f0: 2053 6571 7565 6e63 655b 7374 725d 5d20   Sequence[str]] 
+0000e300: 3d20 2769 6e64 6578 272c 0a20 2020 2020  = 'index',.     
+0000e310: 2020 2079 2020 2020 2020 203a 2073 7472     y       : str
+0000e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e330: 2020 2020 2020 203d 2027 7265 7761 7264         = 'reward
+0000e340: 272c 0a20 2020 2020 2020 206c 2020 2020  ',.        l    
+0000e350: 2020 203a 2055 6e69 6f6e 5b73 7472 2c20     : Union[str, 
+0000e360: 5365 7175 656e 6365 5b73 7472 5d5d 203d  Sequence[str]] =
+0000e370: 2027 6675 6c6c 5f6e 616d 6527 2c0a 2020   'full_name',.  
+0000e380: 2020 2020 2020 7020 2020 2020 2020 3a20        p       : 
+0000e390: 556e 696f 6e5b 7374 722c 2053 6571 7565  Union[str, Seque
+0000e3a0: 6e63 655b 7374 725d 5d20 3d20 2765 6e76  nce[str]] = 'env
+0000e3b0: 6972 6f6e 6d65 6e74 5f69 6427 2c0a 2020  ironment_id',.  
+0000e3c0: 2020 2020 2020 7370 616e 2020 2020 3a20        span    : 
+0000e3d0: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
+0000e3e0: 2020 2020 6572 7220 2020 2020 3a20 556e      err     : Un
+0000e3f0: 696f 6e5b 4c69 7465 7261 6c5b 2773 6527  ion[Literal['se'
+0000e400: 2c27 7364 272c 2762 7327 2c27 6269 275d  ,'sd','bs','bi']
+0000e410: 2c20 506f 696e 7441 6e64 496e 7465 7276  , PointAndInterv
+0000e420: 616c 5d20 3d20 4e6f 6e65 2c0a 2020 2020  al] = None,.    
+0000e430: 2020 2020 6572 7265 7665 7279 3a20 696e      errevery: in
+0000e440: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
+0000e450: 2020 6c61 6265 6c73 2020 3a20 5365 7175    labels  : Sequ
+0000e460: 656e 6365 5b73 7472 5d20 3d20 4e6f 6e65  ence[str] = None
+0000e470: 2c0a 2020 2020 2020 2020 636f 6c6f 7273  ,.        colors
+0000e480: 2020 3a20 556e 696f 6e5b 696e 742c 5365    : Union[int,Se
+0000e490: 7175 656e 6365 5b55 6e69 6f6e 5b73 7472  quence[Union[str
+0000e4a0: 2c69 6e74 5d5d 5d20 3d20 4e6f 6e65 2c0a  ,int]]] = None,.
+0000e4b0: 2020 2020 2020 2020 7469 746c 6520 2020          title   
+0000e4c0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0000e4d0: 2020 2020 2020 786c 6162 656c 2020 3a20        xlabel  : 
+0000e4e0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+0000e4f0: 2020 2020 796c 6162 656c 2020 3a20 7374      ylabel  : st
+0000e500: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+0000e510: 2020 786c 696d 2020 2020 3a20 5475 706c    xlim    : Tupl
+0000e520: 655b 4f70 7469 6f6e 616c 5b4e 756d 6265  e[Optional[Numbe
+0000e530: 725d 2c4f 7074 696f 6e61 6c5b 4e75 6d62  r],Optional[Numb
+0000e540: 6572 5d5d 203d 204e 6f6e 652c 0a20 2020  er]] = None,.   
+0000e550: 2020 2020 2079 6c69 6d20 2020 203a 2054       ylim    : T
+0000e560: 7570 6c65 5b4f 7074 696f 6e61 6c5b 4e75  uple[Optional[Nu
+0000e570: 6d62 6572 5d2c 4f70 7469 6f6e 616c 5b4e  mber],Optional[N
+0000e580: 756d 6265 725d 5d20 3d20 4e6f 6e65 2c0a  umber]] = None,.
+0000e590: 2020 2020 2020 2020 7874 6963 6b73 2020          xticks  
+0000e5a0: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
+0000e5b0: 2020 2020 2020 2079 7469 636b 7320 203a         yticks  :
+0000e5c0: 2062 6f6f 6c20 3d20 5472 7565 2c0a 2020   bool = True,.  
+0000e5d0: 2020 2020 2020 6c65 6765 6e64 2020 3a20        legend  : 
+0000e5e0: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
+0000e5f0: 2020 2020 2061 6c70 6861 2020 203a 2066       alpha   : f
+0000e600: 6c6f 6174 203d 2031 2c0a 2020 2020 2020  loat = 1,.      
+0000e610: 2020 786f 7264 6572 2020 3a20 4c69 7465    xorder  : Lite
+0000e620: 7261 6c5b 272b 272c 272d 275d 203d 204e  ral['+','-'] = N
+0000e630: 6f6e 652c 0a20 2020 2020 2020 2074 6f70  one,.        top
+0000e640: 5f6e 2020 203a 2069 6e74 203d 204e 6f6e  _n   : int = Non
+0000e650: 652c 0a20 2020 2020 2020 206f 7574 2020  e,.        out  
+0000e660: 2020 203a 2055 6e69 6f6e 5b4e 6f6e 652c     : Union[None,
+0000e670: 4c69 7465 7261 6c5b 2773 6372 6565 6e27  Literal['screen'
+0000e680: 5d2c 7374 725d 203d 2027 7363 7265 656e  ],str] = 'screen
+0000e690: 272c 0a20 2020 2020 2020 2061 7820 3d20  ',.        ax = 
+0000e6a0: 4e6f 6e65 2920 2d3e 204e 6f6e 653a 0a20  None) -> None:. 
+0000e6b0: 2020 2020 2020 2022 2222 506c 6f74 2074         """Plot t
+0000e6c0: 6865 2070 6572 666f 726d 616e 6365 206f  he performance o
+0000e6d0: 6620 6d75 6c74 6970 6c65 206c 6561 726e  f multiple learn
+0000e6e0: 6572 7320 6f6e 206d 756c 7469 706c 6520  ers on multiple 
+0000e6f0: 656e 7669 726f 6e6d 656e 7473 2e20 4974  environments. It
+0000e700: 2067 6976 6573 2061 2073 656e 7365 206f   gives a sense o
+0000e710: 6620 7468 650a 2020 2020 2020 2020 6578  f the.        ex
+0000e720: 7065 6374 6564 2070 6572 666f 726d 616e  pected performan
+0000e730: 6365 2066 6f72 2064 6966 6665 7265 6e74  ce for different
+0000e740: 206c 6561 726e 6572 7320 6163 726f 7373   learners across
+0000e750: 2069 6e64 6570 656e 6465 6e74 2065 6e76   independent env
+0000e760: 6972 6f6e 6d65 6e74 732e 2054 6869 7320  ironments. This 
+0000e770: 706c 6f74 2069 730a 2020 2020 2020 2020  plot is.        
+0000e780: 7661 6c75 6162 6c65 2069 6e20 6761 696e  valuable in gain
+0000e790: 696e 6720 696e 7369 6768 7420 696e 746f  ing insight into
+0000e7a0: 2068 6f77 2076 6172 696f 7573 206c 6561   how various lea
+0000e7b0: 726e 6572 7320 7065 7266 6f72 6d20 696e  rners perform in
+0000e7c0: 2063 6f6d 7061 7269 736f 6e20 746f 206f   comparison to o
+0000e7d0: 6e65 2061 6e6f 7468 6572 2e0a 0a20 2020  ne another...   
+0000e7e0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000e7f0: 2020 2020 2020 2078 3a20 5468 6520 7661         x: The va
+0000e800: 6c75 6573 2074 6f20 706c 6f74 206f 6e20  lues to plot on 
+0000e810: 7468 6520 782d 6178 6973 2e0a 2020 2020  the x-axis..    
+0000e820: 2020 2020 2020 2020 793a 2054 6865 2076          y: The v
+0000e830: 616c 7565 2074 6f20 706c 6f74 206f 6e20  alue to plot on 
+0000e840: 7468 6520 792d 6178 6973 2e0a 2020 2020  the y-axis..    
+0000e850: 2020 2020 2020 2020 6c3a 2054 6865 2076          l: The v
+0000e860: 616c 7565 7320 746f 2070 6c6f 7420 696e  alues to plot in
+0000e870: 2074 6865 206c 6567 656e 642e 0a20 2020   the legend..   
+0000e880: 2020 2020 2020 2020 2070 3a20 5468 6520           p: The 
+0000e890: 7061 6972 7320 7468 6174 206d 7573 7420  pairs that must 
+0000e8a0: 6578 6973 7420 6163 726f 7373 2061 6c6c  exist across all
+0000e8b0: 2069 7465 6d73 2069 6e20 7468 6520 6c65   items in the le
+0000e8c0: 6765 6e64 2069 6e20 6f72 6465 7220 746f  gend in order to
+0000e8d0: 2062 6520 696e 636c 7564 6564 2e0a 2020   be included..  
+0000e8e0: 2020 2020 2020 2020 2020 2020 2020 4966                If
+0000e8f0: 204e 6f6e 6520 6e6f 2070 6169 7269 6e67   None no pairing
+0000e900: 2020 6368 6563 6b73 2061 7265 2070 6572    checks are per
+0000e910: 666f 726d 6564 2e0a 2020 2020 2020 2020  formed..        
+0000e920: 2020 2020 7370 616e 3a20 5468 6520 6e75      span: The nu
+0000e930: 6d62 6572 206f 6620 7920 7661 6c75 6573  mber of y values
+0000e940: 2074 6f20 736d 6f6f 7468 2074 6f67 6574   to smooth toget
+0000e950: 6865 7220 7768 656e 2072 6570 6f72 7469  her when reporti
+0000e960: 6e67 2079 2e20 4966 2074 6869 7320 6973  ng y. If this is
+0000e970: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+0000e980: 2020 2020 2020 7468 656e 2074 6865 2061        then the a
+0000e990: 7665 7261 6765 206f 6620 616c 6c20 7920  verage of all y 
+0000e9a0: 7661 6c75 6573 2075 7020 746f 2063 7572  values up to cur
+0000e9b0: 7265 6e74 2069 7320 7368 6f77 6e20 6f74  rent is shown ot
+0000e9c0: 6865 7277 6973 6520 6120 6d6f 7669 6e67  herwise a moving
+0000e9d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e9e0: 2061 7665 7261 6765 2077 6974 6820 7769   average with wi
+0000e9f0: 6e64 6f77 2073 697a 6520 6f66 2073 7061  ndow size of spa
+0000ea00: 6e20 2874 6865 2077 696e 646f 7720 7769  n (the window wi
+0000ea10: 6c6c 2062 6520 736d 616c 6c65 7220 7468  ll be smaller th
+0000ea20: 616e 2073 7061 6e20 696e 6974 6961 6c6c  an span initiall
+0000ea30: 7929 2e0a 2020 2020 2020 2020 2020 2020  y)..            
+0000ea40: 6572 723a 2054 6869 7320 6465 7465 726d  err: This determ
+0000ea50: 696e 6573 2077 6861 7420 6b69 6e64 206f  ines what kind o
+0000ea60: 6620 6572 726f 7220 6261 7273 2074 6f20  f error bars to 
+0000ea70: 706c 6f74 2028 6966 2061 6e79 292e 2049  plot (if any). I
+0000ea80: 6620 604e 6f6e 6560 2074 6865 6e20 6e6f  f `None` then no
+0000ea90: 2062 6172 730a 2020 2020 2020 2020 2020   bars.          
+0000eaa0: 2020 2020 2020 6172 6520 706c 6f74 7465        are plotte
+0000eab0: 642c 2069 6620 2773 6527 2074 6865 2073  d, if 'se' the s
+0000eac0: 7461 6e64 6172 6420 6572 726f 7220 6973  tandard error is
+0000ead0: 2073 686f 776e 2c20 616e 6420 6966 2027   shown, and if '
+0000eae0: 7364 2720 7468 6520 7374 616e 6461 7264  sd' the standard
+0000eaf0: 2064 6576 6961 7469 6f6e 0a20 2020 2020   deviation.     
+0000eb00: 2020 2020 2020 2020 2020 2069 7320 7368             is sh
+0000eb10: 6f77 6e2e 0a20 2020 2020 2020 2020 2020  own..           
+0000eb20: 2065 7272 6576 6572 793a 2054 6869 7320   errevery: This 
+0000eb30: 6465 7465 726d 696e 6573 2074 6865 2066  determines the f
+0000eb40: 7265 7175 656e 6379 206f 6620 6572 726f  requency of erro
+0000eb50: 7262 6172 732e 2049 6620 604e 6f6e 6560  rbars. If `None`
+0000eb60: 2074 6865 7920 6170 7065 6172 2035 2520   they appear 5% 
+0000eb70: 6f66 2074 6865 0a20 2020 2020 2020 2020  of the.         
+0000eb80: 2020 2020 2020 2074 696d 652e 0a20 2020         time..   
+0000eb90: 2020 2020 2020 2020 206c 6162 656c 733a           labels:
+0000eba0: 2054 6865 206c 6567 656e 6420 6c61 6265   The legend labe
+0000ebb0: 6c73 2074 6f20 7573 6520 696e 2074 6865  ls to use in the
+0000ebc0: 2070 6c6f 742e 2054 6865 7365 2073 686f   plot. These sho
+0000ebd0: 756c 6420 6265 2069 6e20 6f72 6465 7220  uld be in order 
+0000ebe0: 6f66 2074 6865 2061 6374 7561 6c0a 2020  of the actual.  
+0000ebf0: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+0000ec00: 6765 6e64 206c 6162 656c 732e 0a20 2020  gend labels..   
+0000ec10: 2020 2020 2020 2020 2063 6f6c 6f72 733a           colors:
+0000ec20: 2054 6865 2063 6f6c 6f72 7320 7573 6564   The colors used
+0000ec30: 2074 6f20 706c 6f74 2074 6865 206c 6561   to plot the lea
+0000ec40: 726e 6572 7320 706c 6f74 2e0a 2020 2020  rners plot..    
+0000ec50: 2020 2020 2020 2020 7469 746c 6520 3a20          title : 
+0000ec60: 5468 6520 7469 746c 6520 6769 7665 2074  The title give t
+0000ec70: 6865 2070 6c6f 742e 0a20 2020 2020 2020  he plot..       
+0000ec80: 2020 2020 2078 6c61 6265 6c3a 2054 6865       xlabel: The
+0000ec90: 206c 6162 656c 206f 6e20 7468 6520 782d   label on the x-
+0000eca0: 6178 6973 2e0a 2020 2020 2020 2020 2020  axis..          
+0000ecb0: 2020 796c 6162 656c 3a20 5468 6520 6c61    ylabel: The la
+0000ecc0: 6265 6c20 6f6e 2074 6865 2079 2d61 7869  bel on the y-axi
+0000ecd0: 732e 0a20 2020 2020 2020 2020 2020 2078  s..            x
+0000ece0: 6c69 6d3a 2044 6566 696e 6520 7468 6520  lim: Define the 
+0000ecf0: 782d 6178 6973 206c 696d 6974 7320 746f  x-axis limits to
+0000ed00: 2070 6c6f 742e 2049 6620 604e 6f6e 6560   plot. If `None`
+0000ed10: 2074 6865 2078 2d61 7869 7320 6c69 6d69   the x-axis limi
+0000ed20: 7473 2077 696c 6c20 6265 2069 6e66 6572  ts will be infer
+0000ed30: 7265 642e 0a20 2020 2020 2020 2020 2020  red..           
+0000ed40: 2079 6c69 6d3a 2044 6566 696e 6520 7468   ylim: Define th
+0000ed50: 6520 792d 6178 6973 206c 696d 6974 7320  e y-axis limits 
+0000ed60: 746f 2070 6c6f 742e 2049 6620 604e 6f6e  to plot. If `Non
+0000ed70: 6560 2074 6865 2079 2d61 7869 7320 6c69  e` the y-axis li
+0000ed80: 6d69 7473 2077 696c 6c20 6265 2069 6e66  mits will be inf
+0000ed90: 6572 7265 642e 0a20 2020 2020 2020 2020  erred..         
+0000eda0: 2020 2078 7469 636b 733a 2057 6865 7468     xticks: Wheth
+0000edb0: 6572 2074 6865 2078 2d61 7869 7320 6c61  er the x-axis la
+0000edc0: 6265 6c73 2073 686f 756c 6420 6265 2064  bels should be d
+0000edd0: 7261 776e 2e0a 2020 2020 2020 2020 2020  rawn..          
+0000ede0: 2020 7974 6963 6b73 3a20 5768 6574 6865    yticks: Whethe
+0000edf0: 7220 7468 6520 792d 6178 6973 206c 6162  r the y-axis lab
+0000ee00: 656c 7320 7368 6f75 6c64 2062 6520 6472  els should be dr
+0000ee10: 6177 6e2e 0a20 2020 2020 2020 2020 2020  awn..           
+0000ee20: 206c 6567 656e 643a 2057 6865 7468 6572   legend: Whether
+0000ee30: 2074 6865 206c 6567 656e 6420 666f 7220   the legend for 
+0000ee40: 7468 6520 706c 6f74 2073 686f 756c 6420  the plot should 
+0000ee50: 6265 2064 7261 776e 2e0a 2020 2020 2020  be drawn..      
+0000ee60: 2020 2020 2020 616c 7068 613a 2054 6865        alpha: The
+0000ee70: 206f 7061 6369 7479 206f 6620 6472 6177   opacity of draw
+0000ee80: 6e20 6461 7461 2e0a 2020 2020 2020 2020  n data..        
+0000ee90: 2020 2020 786f 7264 6572 3a20 496e 6469      xorder: Indi
+0000eea0: 6361 7465 7320 7768 6574 6865 7220 7468  cates whether th
+0000eeb0: 6520 782d 6178 6973 2073 686f 756c 6420  e x-axis should 
+0000eec0: 6265 2069 6e20 6173 6365 6e64 696e 6720  be in ascending 
+0000eed0: 282b 2920 6f72 2064 6573 6365 6e64 6569  (+) or descendei
+0000eee0: 6e67 2028 2d29 206f 7264 6572 2e0a 2020  ng (-) order..  
+0000eef0: 2020 2020 2020 2020 2020 746f 705f 6e3a            top_n:
+0000ef00: 204f 6e6c 7920 706c 6f74 2074 6865 2074   Only plot the t
+0000ef10: 6f70 5f6e 206c 6561 726e 6572 732e 2049  op_n learners. I
+0000ef20: 6620 604e 6f6e 6560 2061 6c6c 206c 6561  f `None` all lea
+0000ef30: 726e 6572 7320 7769 6c6c 2062 6520 706c  rners will be pl
+0000ef40: 6f74 7465 642e 2049 6620 6e65 6761 7469  otted. If negati
+0000ef50: 7665 0a20 2020 2020 2020 2020 2020 2020  ve.             
+0000ef60: 2020 2074 6865 2062 6f74 746f 6d20 7769     the bottom wi
+0000ef70: 6c6c 2062 6520 706c 6f74 7465 642e 0a20  ll be plotted.. 
+0000ef80: 2020 2020 2020 2020 2020 206f 7574 3a20             out: 
+0000ef90: 496e 6469 6361 7465 2077 6865 7265 2074  Indicate where t
+0000efa0: 6865 2070 6c6f 7420 7368 6f75 6c64 2062  he plot should b
+0000efb0: 6520 7365 6e74 2074 6f20 6166 7465 7220  e sent to after 
+0000efc0: 706c 6f74 7469 6e67 2069 7320 6669 6e69  plotting is fini
+0000efd0: 7368 6564 2e20 5661 6c69 6420 7661 6c75  shed. Valid valu
+0000efe0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+0000eff0: 2020 2061 7265 2027 7363 7265 656e 2720     are 'screen' 
+0000f000: 746f 2073 686f 7720 6974 206f 6e20 7363  to show it on sc
+0000f010: 7265 656e 2c20 6120 7061 7468 2074 6f20  reen, a path to 
+0000f020: 7361 7665 2074 6f20 6469 736b 2c20 6f72  save to disk, or
+0000f030: 204e 6f6e 6520 6966 2074 6865 2070 6c6f   None if the plo
+0000f040: 7420 7368 6f75 6c64 0a20 2020 2020 2020  t should.       
+0000f050: 2020 2020 2020 2020 206e 6f74 2062 6520           not be 
+0000f060: 6f75 7470 7574 2061 6e79 7768 6572 6520  output anywhere 
+0000f070: 2869 2e65 2e2c 206b 6570 7420 696e 206d  (i.e., kept in m
+0000f080: 656d 6f72 7929 2069 6e20 6f72 6465 7220  emory) in order 
+0000f090: 746f 206b 6565 7020 6564 6974 696e 6720  to keep editing 
+0000f0a0: 7468 6520 706c 6f74 2061 6674 6572 0a20  the plot after. 
+0000f0b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000f0c0: 6869 7320 6361 6c6c 2e0a 2020 2020 2020  his call..      
+0000f0d0: 2020 2020 2020 6178 3a20 5072 6f76 6964        ax: Provid
+0000f0e0: 6520 616e 206f 7074 696f 6e61 6c20 6178  e an optional ax
+0000f0f0: 6573 2074 6861 7420 7468 6520 706c 6f74  es that the plot
+0000f100: 2077 696c 6c20 6265 2064 7261 776e 2074   will be drawn t
+0000f110: 6f2e 2049 6620 6e6f 7420 7072 6f76 6964  o. If not provid
+0000f120: 6564 2061 206e 6577 0a20 2020 2020 2020  ed a new.       
+0000f130: 2020 2020 2020 2020 2066 6967 7572 652f           figure/
+0000f140: 6178 6573 2069 7320 6372 6561 7465 642e  axes is created.
+0000f150: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000f160: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0000f170: 2020 2020 2020 786c 696d 203d 2078 6c69        xlim = xli
+0000f180: 6d20 6f72 205b 4e6f 6e65 2c4e 6f6e 655d  m or [None,None]
+0000f190: 0a20 2020 2020 2020 2020 2020 2079 6c69  .            yli
+0000f1a0: 6d20 3d20 796c 696d 206f 7220 5b4e 6f6e  m = ylim or [Non
+0000f1b0: 652c 4e6f 6e65 5d0a 0a20 2020 2020 2020  e,None]..       
+0000f1c0: 2020 2020 2072 6177 5f64 6174 6120 3d20       raw_data = 
+0000f1d0: 7365 6c66 2e72 6177 5f6c 6561 726e 6572  self.raw_learner
+0000f1e0: 7328 782c 792c 6c2c 702c 7370 616e 290a  s(x,y,l,p,span).
+0000f1f0: 0a20 2020 2020 2020 2020 2020 2065 7272  .            err
+0000f200: 6576 6572 7920 3d20 6572 7265 7665 7279  every = errevery
+0000f210: 206f 7220 6d61 7828 696e 7428 7261 775f   or max(int(raw_
+0000f220: 6461 7461 5b27 7827 5d5b 2d31 5d2a 302e  data['x'][-1]*0.
+0000f230: 3035 292c 3129 2069 6620 7820 3d3d 2027  05),1) if x == '
+0000f240: 696e 6465 7827 2065 6c73 6520 310a 2020  index' else 1.  
+0000f250: 2020 2020 2020 2020 2020 7374 796c 6520            style 
+0000f260: 2020 203d 2022 2d22 2069 6620 7820 3d3d     = "-" if x ==
+0000f270: 2027 696e 6465 7827 2065 6c73 6520 222e   'index' else ".
+0000f280: 220a 2020 2020 2020 2020 2020 2020 6572  ".            er
+0000f290: 7220 2020 2020 203d 2073 656c 662e 5f63  r      = self._c
+0000f2a0: 6f6e 6669 6465 6e63 6528 6572 722c 2065  onfidence(err, e
+0000f2b0: 7272 6576 6572 7929 0a0a 2020 2020 2020  rrevery)..      
+0000f2c0: 2020 2020 2020 595f 636f 756e 7420 3d20        Y_count = 
+0000f2d0: 5b5d 0a20 2020 2020 2020 2020 2020 206c  [].            l
+0000f2e0: 696e 6573 3a20 4c69 7374 5b50 6f69 6e74  ines: List[Point
+0000f2f0: 735d 203d 205b 5d0a 2020 2020 2020 2020  s] = [].        
+0000f300: 2020 2020 666f 7220 5f6c 2069 6e20 7261      for _l in ra
+0000f310: 775f 6461 7461 2e63 6f6c 756d 6e73 5b31  w_data.columns[1
+0000f320: 3a5d 3a0a 2020 2020 2020 2020 2020 2020  :]:.            
+0000f330: 2020 2020 636f 6c6f 7220 3d20 7365 6c66      color = self
+0000f340: 2e5f 6765 745f 636f 6c6f 7228 636f 6c6f  ._get_color(colo
+0000f350: 7273 2c20 2020 6c65 6e28 6c69 6e65 7329  rs,   len(lines)
+0000f360: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000f370: 2020 6c61 6265 6c20 3d20 7365 6c66 2e5f    label = self._
+0000f380: 6765 745f 6c61 6265 6c28 6c61 6265 6c73  get_label(labels
+0000f390: 2c5f 6c2c 6c65 6e28 6c69 6e65 7329 290a  ,_l,len(lines)).
+0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3b0: 595f 636f 756e 742e 6170 7065 6e64 2830  Y_count.append(0
+0000f3c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000f3d0: 2020 6c69 6e65 732e 6170 7065 6e64 2850    lines.append(P
+0000f3e0: 6f69 6e74 7328 7374 796c 653d 7374 796c  oints(style=styl
+0000f3f0: 652c 636f 6c6f 723d 636f 6c6f 722c 6c61  e,color=color,la
+0000f400: 6265 6c3d 6c61 6265 6c2c 616c 7068 613d  bel=label,alpha=
+0000f410: 616c 7068 6129 290a 2020 2020 2020 2020  alpha)).        
+0000f420: 2020 2020 2020 2020 666f 7220 5f78 692c          for _xi,
+0000f430: 2028 5f78 2c20 5929 2069 6e20 656e 756d   (_x, Y) in enum
+0000f440: 6572 6174 6528 7a69 7028 2a72 6177 5f64  erate(zip(*raw_d
+0000f450: 6174 615b 5b27 7827 2c5f 6c5d 5d29 293a  ata[['x',_l]])):
+0000f460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f470: 2020 2020 2059 5f63 6f75 6e74 5b2d 315d       Y_count[-1]
+0000f480: 203d 206d 6178 2859 5f63 6f75 6e74 5b2d   = max(Y_count[-
+0000f490: 315d 2c6c 656e 2859 2929 0a20 2020 2020  1],len(Y)).     
+0000f4a0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000f4b0: 696e 6573 5b2d 315d 2e61 6464 285f 7820  ines[-1].add(_x 
+0000f4c0: 6966 205f 7820 6973 206e 6f74 204e 6f6e  if _x is not Non
+0000f4d0: 6520 656c 7365 2027 4e6f 6e65 272c 202a  e else 'None', *
+0000f4e0: 6572 7228 592c 205f 7869 2929 0a0a 2020  err(Y, _xi))..  
+0000f4f0: 2020 2020 2020 2020 2020 6c69 6e65 7320            lines 
+0000f500: 203d 2073 6f72 7465 6428 6c69 6e65 732c   = sorted(lines,
+0000f510: 206b 6579 3d6c 616d 6264 6120 6c69 6e65   key=lambda line
+0000f520: 3a20 6c69 6e65 2e59 5b2d 315d 2c20 7265  : line.Y[-1], re
+0000f530: 7665 7273 653d 5472 7565 290a 2020 2020  verse=True).    
+0000f540: 2020 2020 2020 2020 6c61 6265 6c73 203d          labels =
+0000f550: 205b 6c2e 6c61 6265 6c20 6f72 2073 7472   [l.label or str
+0000f560: 286c 2e6c 6162 656c 2920 666f 7220 6c20  (l.label) for l 
+0000f570: 696e 206c 696e 6573 5d0a 2020 2020 2020  in lines].      
+0000f580: 2020 2020 2020 636f 6c6f 7273 203d 205b        colors = [
+0000f590: 6c2e 636f 6c6f 7220 2020 2020 2020 2020  l.color         
+0000f5a0: 2020 2020 2020 2020 666f 7220 6c20 696e          for l in
+0000f5b0: 206c 696e 6573 5d0a 2020 2020 2020 2020   lines].        
+0000f5c0: 2020 2020 786c 6162 656c 203d 2078 6c61      xlabel = xla
+0000f5d0: 6265 6c20 6f72 2028 2249 6e74 6572 6163  bel or ("Interac
+0000f5e0: 7469 6f6e 2220 6966 2078 3d3d 2769 6e64  tion" if x=='ind
+0000f5f0: 6578 2720 656c 7365 2078 5b30 5d20 6966  ex' else x[0] if
+0000f600: 206c 656e 2878 2920 3d3d 2031 2065 6c73   len(x) == 1 els
+0000f610: 6520 7829 0a20 2020 2020 2020 2020 2020  e x).           
+0000f620: 2079 6c61 6265 6c20 3d20 796c 6162 656c   ylabel = ylabel
+0000f630: 206f 7220 2822 5265 7761 7264 2220 6966   or ("Reward" if
+0000f640: 2079 3d3d 2772 6577 6172 6427 2065 6c73   y=='reward' els
+0000f650: 6520 792e 7265 706c 6163 6528 225f 7063  e y.replace("_pc
+0000f660: 7422 2c22 2050 6572 6365 6e74 2229 290a  t"," Percent")).
+0000f670: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000f680: 6c65 6e28 7365 7428 595f 636f 756e 7429  len(set(Y_count)
+0000f690: 2920 3d3d 2031 3a20 595f 636f 756e 7420  ) == 1: Y_count 
+0000f6a0: 3d20 595f 636f 756e 745b 305d 0a0a 2020  = Y_count[0]..  
+0000f6b0: 2020 2020 2020 2020 2020 795f 6c6f 6361            y_loca
+0000f6c0: 7469 6f6e 203d 2022 546f 7461 6c22 2069  tion = "Total" i
+0000f6d0: 6620 7820 213d 2027 696e 6465 7827 2065  f x != 'index' e
+0000f6e0: 6c73 6520 2222 0a20 2020 2020 2020 2020  lse "".         
+0000f6f0: 2020 2079 5f61 7667 5f74 7970 6520 3d20     y_avg_type = 
+0000f700: 2822 496e 7374 616e 7422 2069 6620 7370  ("Instant" if sp
+0000f710: 616e 203d 3d20 3120 656c 7365 2066 2253  an == 1 else f"S
+0000f720: 7061 6e20 7b73 7061 6e7d 2220 6966 2073  pan {span}" if s
+0000f730: 7061 6e20 656c 7365 2022 5072 6f67 7265  pan else "Progre
+0000f740: 7373 6976 6522 290a 2020 2020 2020 2020  ssive").        
+0000f750: 2020 2020 795f 7361 6d70 6c65 7320 203d      y_samples  =
+0000f760: 2066 2228 7b59 5f63 6f75 6e74 7d20 456e   f"({Y_count} En
+0000f770: 7669 726f 6e6d 656e 7473 2922 0a20 2020  vironments)".   
+0000f780: 2020 2020 2020 2020 2074 6974 6c65 2020           title  
+0000f790: 2020 2020 3d20 7469 746c 6520 6966 2074      = title if t
+0000f7a0: 6974 6c65 2069 7320 6e6f 7420 4e6f 6e65  itle is not None
+0000f7b0: 2065 6c73 6520 2827 2027 2e6a 6f69 6e28   else (' '.join(
+0000f7c0: 6669 6c74 6572 284e 6f6e 652c 5b79 5f6c  filter(None,[y_l
+0000f7d0: 6f63 6174 696f 6e2c 2079 5f61 7667 5f74  ocation, y_avg_t
+0000f7e0: 7970 652c 2079 6c61 6265 6c2c 2079 5f73  ype, ylabel, y_s
+0000f7f0: 616d 706c 6573 5d29 2929 0a0a 2020 2020  amples])))..    
+0000f800: 2020 2020 2020 2020 7872 6f74 6174 696f          xrotatio
+0000f810: 6e20 3d20 3930 2069 6620 2878 2021 3d20  n = 90 if (x != 
+0000f820: 2769 6e64 6578 2720 6f72 2078 6f72 6465  'index' or xorde
+0000f830: 7229 2061 6e64 206c 656e 286c 696e 6573  r) and len(lines
+0000f840: 5b30 5d2e 5829 3e35 2065 6c73 6520 300a  [0].X)>5 else 0.
+0000f850: 2020 2020 2020 2020 2020 2020 7972 6f74              yrot
+0000f860: 6174 696f 6e20 3d20 300a 0a20 2020 2020  ation = 0..     
+0000f870: 2020 2020 2020 2069 6620 746f 705f 6e3a         if top_n:
+0000f880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f890: 2069 6620 6162 7328 746f 705f 6e29 203e   if abs(top_n) >
+0000f8a0: 206c 656e 286c 696e 6573 293a 2074 6f70   len(lines): top
+0000f8b0: 5f6e 203d 206c 656e 286c 696e 6573 292a  _n = len(lines)*
+0000f8c0: 6162 7328 746f 705f 6e29 2f74 6f70 5f6e  abs(top_n)/top_n
+0000f8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f8e0: 2069 6620 746f 705f 6e20 3e20 303a 206c   if top_n > 0: l
+0000f8f0: 696e 6573 203d 205b 7265 706c 6163 6528  ines = [replace(
+0000f900: 6c2c 636f 6c6f 723d 7365 6c66 2e5f 6765  l,color=self._ge
+0000f910: 745f 636f 6c6f 7228 636f 6c6f 7273 2c69  t_color(colors,i
+0000f920: 292c 6c61 6265 6c3d 7365 6c66 2e5f 6765  ),label=self._ge
+0000f930: 745f 6c61 6265 6c28 6c61 6265 6c73 2c6c  t_label(labels,l
+0000f940: 2e6c 6162 656c 2c69 2929 2066 6f72 2069  .label,i)) for i
+0000f950: 2c6c 2069 6e20 656e 756d 6572 6174 6528  ,l in enumerate(
+0000f960: 6c69 6e65 735b 3a74 6f70 5f6e 5d2c 3020  lines[:top_n],0 
+0000f970: 2020 2029 205d 0a20 2020 2020 2020 2020     ) ].         
+0000f980: 2020 2020 2020 2069 6620 746f 705f 6e20         if top_n 
+0000f990: 3c20 303a 206c 696e 6573 203d 205b 7265  < 0: lines = [re
+0000f9a0: 706c 6163 6528 6c2c 636f 6c6f 723d 7365  place(l,color=se
+0000f9b0: 6c66 2e5f 6765 745f 636f 6c6f 7228 636f  lf._get_color(co
+0000f9c0: 6c6f 7273 2c69 292c 6c61 6265 6c3d 7365  lors,i),label=se
+0000f9d0: 6c66 2e5f 6765 745f 6c61 6265 6c28 6c61  lf._get_label(la
+0000f9e0: 6265 6c73 2c6c 2e6c 6162 656c 2c69 2929  bels,l.label,i))
+0000f9f0: 2066 6f72 2069 2c6c 2069 6e20 656e 756d   for i,l in enum
+0000fa00: 6572 6174 6528 6c69 6e65 735b 746f 705f  erate(lines[top_
+0000fa10: 6e3a 5d2c 746f 705f 6e29 205d 0a0a 2020  n:],top_n) ]..  
+0000fa20: 2020 2020 2020 2020 2020 616c 6c5f 7820            all_x 
+0000fa30: 3d20 6469 6374 2e66 726f 6d6b 6579 7328  = dict.fromkeys(
+0000fa40: 6368 6169 6e2e 6672 6f6d 5f69 7465 7261  chain.from_itera
+0000fa50: 626c 6528 6c69 6e65 2e58 2066 6f72 206c  ble(line.X for l
+0000fa60: 696e 6520 696e 206c 696e 6573 2929 0a20  ine in lines)). 
+0000fa70: 2020 2020 2020 2020 2020 2078 6f72 6465             xorde
+0000fa80: 7265 6420 3d20 6c69 7374 2861 6c6c 5f78  red = list(all_x
+0000fa90: 2e6b 6579 7328 2929 2069 6620 6e6f 7420  .keys()) if not 
+0000faa0: 786f 7264 6572 2065 6c73 6520 736f 7274  xorder else sort
+0000fab0: 6564 2861 6c6c 5f78 2c20 7265 7665 7273  ed(all_x, revers
+0000fac0: 653d 786f 7264 6572 3d3d 272d 2729 0a0a  e=xorder=='-')..
+0000fad0: 2020 2020 2020 2020 2020 2020 6966 2078              if x
+0000fae0: 203d 3d20 2769 6e64 6578 2720 616e 6420   == 'index' and 
+0000faf0: 786f 7264 6572 2069 6e20 5b27 2b27 2c4e  xorder in ['+',N
+0000fb00: 6f6e 655d 3a20 786f 7264 6572 6564 203d  one]: xordered =
+0000fb10: 204e 6f6e 650a 0a20 2020 2020 2020 2020   None..         
+0000fb20: 2020 2073 656c 662e 5f70 6c6f 7474 6572     self._plotter
+0000fb30: 2e70 6c6f 7428 6178 2c20 6c69 6e65 732c  .plot(ax, lines,
+0000fb40: 2074 6974 6c65 2c20 786c 6162 656c 2c20   title, xlabel, 
+0000fb50: 796c 6162 656c 2c20 786c 696d 2c20 796c  ylabel, xlim, yl
+0000fb60: 696d 2c20 7874 6963 6b73 2c20 7974 6963  im, xticks, ytic
+0000fb70: 6b73 2c20 6c65 6765 6e64 2c20 7872 6f74  ks, legend, xrot
+0000fb80: 6174 696f 6e2c 2079 726f 7461 7469 6f6e  ation, yrotation
+0000fb90: 2c20 786f 7264 6572 6564 2c20 6f75 7429  , xordered, out)
+0000fba0: 0a0a 2020 2020 2020 2020 6578 6365 7074  ..        except
+0000fbb0: 2043 6f62 6145 7863 6570 7469 6f6e 2061   CobaException a
+0000fbc0: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
+0000fbd0: 2043 6f62 6143 6f6e 7465 7874 2e6c 6f67   CobaContext.log
+0000fbe0: 6765 722e 6c6f 6728 7374 7228 6529 290a  ger.log(str(e)).
+0000fbf0: 0a20 2020 2064 6566 2070 6c6f 745f 636f  .    def plot_co
+0000fc00: 6e74 7261 7374 2873 656c 662c 0a20 2020  ntrast(self,.   
+0000fc10: 2020 2020 206c 3120 2020 2020 203a 2041       l1      : A
+0000fc20: 6e79 2c0a 2020 2020 2020 2020 6c32 2020  ny,.        l2  
+0000fc30: 2020 2020 3a20 416e 792c 0a20 2020 2020      : Any,.     
+0000fc40: 2020 2078 2020 2020 2020 203a 2055 6e69     x       : Uni
+0000fc50: 6f6e 5b73 7472 2c20 5365 7175 656e 6365  on[str, Sequence
+0000fc60: 5b73 7472 5d5d 203d 2022 656e 7669 726f  [str]] = "enviro
+0000fc70: 6e6d 656e 745f 6964 222c 0a20 2020 2020  nment_id",.     
+0000fc80: 2020 2079 2020 2020 2020 203a 2073 7472     y       : str
+0000fc90: 203d 2022 7265 7761 7264 222c 0a20 2020   = "reward",.   
+0000fca0: 2020 2020 206c 2020 2020 2020 203a 2055       l       : U
+0000fcb0: 6e69 6f6e 5b73 7472 2c20 5365 7175 656e  nion[str, Sequen
+0000fcc0: 6365 5b73 7472 5d5d 203d 2027 6c65 6172  ce[str]] = 'lear
+0000fcd0: 6e65 725f 6964 272c 0a20 2020 2020 2020  ner_id',.       
+0000fce0: 2070 2020 2020 2020 203a 2055 6e69 6f6e   p       : Union
+0000fcf0: 5b73 7472 2c20 5365 7175 656e 6365 5b73  [str, Sequence[s
+0000fd00: 7472 5d5d 203d 2027 656e 7669 726f 6e6d  tr]] = 'environm
+0000fd10: 656e 745f 6964 272c 0a20 2020 2020 2020  ent_id',.       
+0000fd20: 206d 6f64 6520 2020 203a 2055 6e69 6f6e   mode    : Union
+0000fd30: 5b4c 6974 6572 616c 5b22 6469 6666 222c  [Literal["diff",
+0000fd40: 2270 726f 6222 5d2c 2043 616c 6c61 626c  "prob"], Callabl
+0000fd50: 655b 5b66 6c6f 6174 2c66 6c6f 6174 5d2c  e[[float,float],
+0000fd60: 666c 6f61 745d 5d20 3d20 2264 6966 6622  float]] = "diff"
+0000fd70: 2c0a 2020 2020 2020 2020 7370 616e 2020  ,.        span  
+0000fd80: 2020 3a20 696e 7420 3d20 4e6f 6e65 2c0a    : int = None,.
+0000fd90: 2020 2020 2020 2020 6572 7220 2020 2020          err     
+0000fda0: 3a20 556e 696f 6e5b 4c69 7465 7261 6c5b  : Union[Literal[
+0000fdb0: 2773 6527 2c27 7364 272c 2762 7327 2c27  'se','sd','bs','
+0000fdc0: 6269 275d 2c20 506f 696e 7441 6e64 496e  bi'], PointAndIn
+0000fdd0: 7465 7276 616c 5d20 3d20 4e6f 6e65 2c0a  terval] = None,.
+0000fde0: 2020 2020 2020 2020 6572 7265 7665 7279          errevery
+0000fdf0: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+0000fe00: 2020 2020 2020 6c61 6265 6c73 2020 3a20        labels  : 
+0000fe10: 5365 7175 656e 6365 5b73 7472 5d20 3d20  Sequence[str] = 
+0000fe20: 4e6f 6e65 2c0a 2020 2020 2020 2020 636f  None,.        co
+0000fe30: 6c6f 7273 2020 3a20 5365 7175 656e 6365  lors  : Sequence
+0000fe40: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0000fe50: 2020 2020 2020 7469 746c 6520 2020 3a20        title   : 
+0000fe60: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+0000fe70: 2020 2020 786c 6162 656c 2020 3a20 7374      xlabel  : st
+0000fe80: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+0000fe90: 2020 796c 6162 656c 2020 3a20 7374 7220    ylabel  : str 
+0000fea0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000feb0: 786c 696d 2020 2020 3a20 5475 706c 655b  xlim    : Tuple[
+0000fec0: 4f70 7469 6f6e 616c 5b4e 756d 6265 725d  Optional[Number]
+0000fed0: 2c4f 7074 696f 6e61 6c5b 4e75 6d62 6572  ,Optional[Number
+0000fee0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+0000fef0: 2020 2079 6c69 6d20 2020 203a 2054 7570     ylim    : Tup
+0000ff00: 6c65 5b4f 7074 696f 6e61 6c5b 4e75 6d62  le[Optional[Numb
+0000ff10: 6572 5d2c 4f70 7469 6f6e 616c 5b4e 756d  er],Optional[Num
+0000ff20: 6265 725d 5d20 3d20 4e6f 6e65 2c0a 2020  ber]] = None,.  
+0000ff30: 2020 2020 2020 7874 6963 6b73 2020 3a20        xticks  : 
+0000ff40: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
+0000ff50: 2020 2020 2079 7469 636b 7320 203a 2062       yticks  : b
+0000ff60: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
+0000ff70: 2020 2020 6c65 6765 6e64 2020 3a20 626f      legend  : bo
+0000ff80: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
+0000ff90: 2020 2061 6c70 6861 2020 203a 2066 6c6f     alpha   : flo
+0000ffa0: 6174 203d 2031 2c0a 2020 2020 2020 2020  at = 1,.        
+0000ffb0: 786f 7264 6572 2020 3a20 4c69 7465 7261  xorder  : Litera
+0000ffc0: 6c5b 272b 272c 272d 275d 203d 204e 6f6e  l['+','-'] = Non
+0000ffd0: 652c 0a20 2020 2020 2020 2062 6f75 6e64  e,.        bound
+0000ffe0: 6172 793a 2062 6f6f 6c20 3d20 5472 7565  ary: bool = True
+0000fff0: 2c0a 2020 2020 2020 2020 6f75 7420 2020  ,.        out   
+00010000: 2020 3a20 556e 696f 6e5b 4e6f 6e65 2c4c    : Union[None,L
+00010010: 6974 6572 616c 5b27 7363 7265 656e 275d  iteral['screen']
+00010020: 2c73 7472 5d20 3d20 2773 6372 6565 6e27  ,str] = 'screen'
+00010030: 2c0a 2020 2020 2020 2020 6178 203d 204e  ,.        ax = N
+00010040: 6f6e 6529 202d 3e20 4e6f 6e65 3a0a 2020  one) -> None:.  
+00010050: 2020 2020 2020 2222 2250 6c6f 7420 6120        """Plot a 
+00010060: 6469 7265 6374 2063 6f6e 7472 6173 7420  direct contrast 
+00010070: 6f66 2074 6865 2070 6572 666f 726d 616e  of the performan
+00010080: 6365 2066 6f72 2074 776f 206c 6561 726e  ce for two learn
+00010090: 6572 732e 0a0a 2020 2020 2020 2020 4172  ers...        Ar
+000100a0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+000100b0: 6c31 3a20 5468 6520 6669 7273 7420 7365  l1: The first se
+000100c0: 7420 6f66 2070 6172 616d 6574 6572 2076  t of parameter v
+000100d0: 616c 7565 7320 7765 2077 616e 7420 746f  alues we want to
+000100e0: 2063 6f6e 7472 6173 742e 0a20 2020 2020   contrast..     
+000100f0: 2020 2020 2020 206c 323a 2054 6865 2073         l2: The s
+00010100: 6563 6f6e 6420 7365 7420 6f66 2070 6172  econd set of par
+00010110: 616d 6574 6572 2076 616c 7565 7320 7765  ameter values we
+00010120: 2077 616e 7420 746f 2063 6f6e 7472 6173   want to contras
+00010130: 742e 0a20 2020 2020 2020 2020 2020 2078  t..            x
+00010140: 3a20 5468 6520 7661 6c75 6520 746f 2070  : The value to p
+00010150: 6c6f 7420 6f6e 2074 6865 2078 2d61 7869  lot on the x-axi
+00010160: 732e 2054 6869 7320 6361 6e20 6569 7468  s. This can eith
+00010170: 6572 2062 6520 696e 6465 7820 6f72 2065  er be index or e
+00010180: 6e76 6972 6f6e 6d65 6e74 2063 6f6c 756d  nvironment colum
+00010190: 6e73 2074 6f20 6772 6f75 7020 6279 2e0a  ns to group by..
+000101a0: 2020 2020 2020 2020 2020 2020 793a 2054              y: T
+000101b0: 6865 2076 616c 7565 2074 6f20 706c 6f74  he value to plot
+000101c0: 206f 6e20 7468 6520 792d 6178 6973 2e0a   on the y-axis..
+000101d0: 2020 2020 2020 2020 2020 2020 6c3a 2054              l: T
+000101e0: 6865 206c 6576 656c 2061 7420 7768 6963  he level at whic
+000101f0: 6820 7765 2077 616e 7420 746f 2063 6f6e  h we want to con
+00010200: 7472 6173 742e 0a20 2020 2020 2020 2020  trast..         
+00010210: 2020 2070 3a20 5468 6520 7061 6972 7320     p: The pairs 
+00010220: 7468 6174 206d 7573 7420 6578 6973 7420  that must exist 
+00010230: 6163 726f 7373 2061 6c6c 2063 6f6d 7061  across all compa
+00010240: 7269 736f 6e20 6c65 7665 6c73 2069 6e20  rison levels in 
+00010250: 6f72 6465 7220 746f 2062 6520 696e 636c  order to be incl
+00010260: 7564 6564 2e0a 2020 2020 2020 2020 2020  uded..          
+00010270: 2020 6d6f 6465 3a20 2764 6966 6627 202d    mode: 'diff' -
+00010280: 2d20 706c 6f74 2074 6865 2070 6169 7277  - plot the pairw
+00010290: 6973 6520 6469 6666 6572 656e 6365 3b20  ise difference; 
+000102a0: 2770 726f 6227 2070 6c6f 7420 7468 6520  'prob' plot the 
+000102b0: 7072 6f62 6162 696c 6974 7920 6f66 206c  probability of l
+000102c0: 3120 6265 6174 696e 6720 6c32 2e0a 2020  1 beating l2..  
+000102d0: 2020 2020 2020 2020 2020 7370 616e 3a20            span: 
+000102e0: 5468 6520 6e75 6d62 6572 206f 6620 7920  The number of y 
+000102f0: 7661 6c75 6573 2074 6f20 736d 6f6f 7468  values to smooth
+00010300: 2074 6f67 6574 6865 7220 7768 656e 2072   together when r
+00010310: 6570 6f72 7469 6e67 2079 2e20 4966 2074  eporting y. If t
+00010320: 6869 7320 6973 204e 6f6e 6520 7468 656e  his is None then
+00010330: 2074 6865 2061 7665 7261 6765 206f 6620   the average of 
+00010340: 616c 6c20 790a 2020 2020 2020 2020 2020  all y.          
+00010350: 2020 2020 2020 7661 6c75 6573 2075 7020        values up 
+00010360: 746f 2063 7572 7265 6e74 2069 7320 7368  to current is sh
+00010370: 6f77 6e20 6f74 6865 7277 6973 6520 6120  own otherwise a 
+00010380: 6d6f 7669 6e67 2061 7665 7261 6765 2077  moving average w
+00010390: 6974 6820 7769 6e64 6f77 2073 697a 6520  ith window size 
+000103a0: 6f66 2073 7061 6e20 2874 6865 2077 696e  of span (the win
+000103b0: 646f 7720 7769 6c6c 2062 650a 2020 2020  dow will be.    
+000103c0: 2020 2020 2020 2020 2020 2020 736d 616c              smal
+000103d0: 6c65 7220 7468 616e 2073 7061 6e20 696e  ler than span in
+000103e0: 6974 6961 6c6c 7929 2e0a 2020 2020 2020  itially)..      
+000103f0: 2020 2020 2020 6572 723a 2054 6869 7320        err: This 
+00010400: 6465 7465 726d 696e 6573 2077 6861 7420  determines what 
+00010410: 6b69 6e64 206f 6620 6572 726f 7220 6261  kind of error ba
+00010420: 7273 2074 6f20 706c 6f74 2028 6966 2061  rs to plot (if a
+00010430: 6e79 292e 2049 6620 604e 6f6e 6560 2074  ny). If `None` t
+00010440: 6865 6e20 6e6f 2062 6172 7320 6172 6520  hen no bars are 
+00010450: 706c 6f74 7465 642c 2069 6620 2773 6527  plotted, if 'se'
+00010460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010470: 2074 6865 2073 7461 6e64 6172 6420 6572   the standard er
+00010480: 726f 7220 6973 2073 686f 776e 2c20 616e  ror is shown, an
+00010490: 6420 6966 2027 7364 2720 7468 6520 7374  d if 'sd' the st
+000104a0: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
+000104b0: 2069 7320 7368 6f77 6e2e 0a20 2020 2020   is shown..     
+000104c0: 2020 2020 2020 2065 7272 6576 6572 793a         errevery:
+000104d0: 2054 6869 7320 6465 7465 726d 696e 6573   This determines
+000104e0: 2074 6865 2066 7265 7175 656e 6379 206f   the frequency o
+000104f0: 6620 6572 726f 7262 6172 732e 2049 6620  f errorbars. If 
+00010500: 604e 6f6e 6560 2074 6865 7920 6170 7065  `None` they appe
+00010510: 6172 2035 2520 6f66 2074 6865 2074 696d  ar 5% of the tim
+00010520: 652e 0a20 2020 2020 2020 2020 2020 206c  e..            l
+00010530: 6162 656c 733a 2054 6865 206c 6567 656e  abels: The legen
+00010540: 6420 6c61 6265 6c73 2074 6f20 7573 6520  d labels to use 
+00010550: 696e 2074 6865 2070 6c6f 742e 2054 6865  in the plot. The
+00010560: 7365 2073 686f 756c 6420 6265 2069 6e20  se should be in 
+00010570: 6f72 6465 7220 6f66 2074 6865 2061 6374  order of the act
+00010580: 7561 6c20 6c65 6765 6e64 206c 6162 656c  ual legend label
+00010590: 732e 0a20 2020 2020 2020 2020 2020 2074  s..            t
+000105a0: 6974 6c65 203a 2054 6865 2074 6974 6c65  itle : The title
+000105b0: 2067 6976 6520 7468 6520 706c 6f74 2e0a   give the plot..
+000105c0: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
+000105d0: 7273 3a20 5468 6520 636f 6c6f 7273 2075  rs: The colors u
+000105e0: 7365 6420 746f 2070 6c6f 7420 7468 6520  sed to plot the 
+000105f0: 6c65 6172 6e65 7273 2070 6c6f 742e 0a20  learners plot.. 
+00010600: 2020 2020 2020 2020 2020 2078 6c61 6265             xlabe
+00010610: 6c3a 2054 6865 206c 6162 656c 206f 6e20  l: The label on 
+00010620: 7468 6520 782d 6178 6973 2e0a 2020 2020  the x-axis..    
+00010630: 2020 2020 2020 2020 796c 6162 656c 3a20          ylabel: 
+00010640: 5468 6520 6c61 6265 6c20 6f6e 2074 6865  The label on the
+00010650: 2079 2d61 7869 732e 0a20 2020 2020 2020   y-axis..       
+00010660: 2020 2020 206c 6567 656e 643a 2057 6865       legend: Whe
+00010670: 7468 6572 2074 6865 206c 6567 656e 6420  ther the legend 
+00010680: 666f 7220 7468 6520 706c 6f74 2073 686f  for the plot sho
+00010690: 756c 6420 6265 2064 7261 776e 2e0a 2020  uld be drawn..  
+000106a0: 2020 2020 2020 2020 2020 616c 7068 613a            alpha:
+000106b0: 2054 6865 206f 7061 6369 7479 206f 6620   The opacity of 
+000106c0: 6472 6177 6e20 6461 7461 2e0a 2020 2020  drawn data..    
+000106d0: 2020 2020 2020 2020 786c 696d 3a20 4465          xlim: De
+000106e0: 6669 6e65 2074 6865 2078 2d61 7869 7320  fine the x-axis 
+000106f0: 6c69 6d69 7473 2074 6f20 706c 6f74 2e20  limits to plot. 
+00010700: 4966 2060 4e6f 6e65 6020 7468 6520 782d  If `None` the x-
+00010710: 6178 6973 206c 696d 6974 7320 7769 6c6c  axis limits will
+00010720: 2062 6520 696e 6665 7272 6564 2e0a 2020   be inferred..  
+00010730: 2020 2020 2020 2020 2020 796c 696d 3a20            ylim: 
+00010740: 4465 6669 6e65 2074 6865 2079 2d61 7869  Define the y-axi
+00010750: 7320 6c69 6d69 7473 2074 6f20 706c 6f74  s limits to plot
+00010760: 2e20 4966 2060 4e6f 6e65 6020 7468 6520  . If `None` the 
+00010770: 792d 6178 6973 206c 696d 6974 7320 7769  y-axis limits wi
+00010780: 6c6c 2062 6520 696e 6665 7272 6564 2e0a  ll be inferred..
+00010790: 2020 2020 2020 2020 2020 2020 7874 6963              xtic
+000107a0: 6b73 3a20 5768 6574 6865 7220 7468 6520  ks: Whether the 
+000107b0: 782d 6178 6973 206c 6162 656c 7320 7368  x-axis labels sh
+000107c0: 6f75 6c64 2062 6520 6472 6177 6e2e 0a20  ould be drawn.. 
+000107d0: 2020 2020 2020 2020 2020 2079 7469 636b             ytick
+000107e0: 733a 2057 6865 7468 6572 2074 6865 2079  s: Whether the y
+000107f0: 2d61 7869 7320 6c61 6265 6c73 2073 686f  -axis labels sho
+00010800: 756c 6420 6265 2064 7261 776e 2e0a 2020  uld be drawn..  
+00010810: 2020 2020 2020 2020 2020 786f 7264 6572            xorder
+00010820: 3a20 496e 6469 6361 7465 7320 7768 6574  : Indicates whet
+00010830: 6865 7220 7468 6520 782d 6178 6973 2073  her the x-axis s
+00010840: 686f 756c 6420 6265 2069 6e20 6173 6365  hould be in asce
+00010850: 6e64 696e 6720 282b 2920 6f72 2064 6573  nding (+) or des
+00010860: 6365 6e64 6569 6e67 2028 2d29 206f 7264  cendeing (-) ord
+00010870: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
+00010880: 626f 756e 6461 7279 3a20 5768 6574 6865  boundary: Whethe
+00010890: 7220 7765 2077 616e 7420 746f 2070 6c6f  r we want to plo
+000108a0: 7420 7468 6520 626f 756e 6461 7279 206c  t the boundary l
+000108b0: 696e 6520 6265 7477 6565 6e20 7768 6963  ine between whic
+000108c0: 6820 7365 7420 6973 2074 6865 2062 6573  h set is the bes
+000108d0: 7420 7065 7266 6f72 6d69 6e67 2e0a 2020  t performing..  
+000108e0: 2020 2020 2020 2020 2020 6f75 743a 2049            out: I
+000108f0: 6e64 6963 6174 6520 7768 6572 6520 7468  ndicate where th
+00010900: 6520 706c 6f74 2073 686f 756c 6420 6265  e plot should be
+00010910: 2073 656e 7420 746f 2061 6674 6572 2070   sent to after p
+00010920: 6c6f 7474 696e 6720 6973 2066 696e 6973  lotting is finis
+00010930: 6865 642e 2056 616c 6964 2076 616c 7565  hed. Valid value
+00010940: 7320 6172 650a 2020 2020 2020 2020 2020  s are.          
+00010950: 2020 2020 2020 2773 6372 6565 6e27 2074        'screen' t
+00010960: 6f20 7368 6f77 2069 7420 6f6e 2073 6372  o show it on scr
+00010970: 6565 6e2c 2061 2070 6174 6820 746f 2073  een, a path to s
+00010980: 6176 6520 746f 2064 6973 6b2c 206f 7220  ave to disk, or 
+00010990: 4e6f 6e65 2069 6620 7468 6520 706c 6f74  None if the plot
+000109a0: 2073 686f 756c 6420 6e6f 7420 6265 0a20   should not be. 
+000109b0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+000109c0: 7574 7075 7420 616e 7977 6865 7265 2028  utput anywhere (
+000109d0: 692e 652e 2c20 6b65 7074 2069 6e20 6d65  i.e., kept in me
+000109e0: 6d6f 7279 2920 696e 206f 7264 6572 2074  mory) in order t
+000109f0: 6f20 6b65 6570 2065 6469 7469 6e67 2074  o keep editing t
+00010a00: 6865 2070 6c6f 7420 6166 7465 7220 7468  he plot after th
+00010a10: 6973 2063 616c 6c2e 0a20 2020 2020 2020  is call..       
+00010a20: 2020 2020 2061 783a 2050 726f 7669 6465       ax: Provide
+00010a30: 2061 6e20 6f70 7469 6f6e 616c 2061 7865   an optional axe
+00010a40: 7320 7468 6174 2074 6865 2070 6c6f 7420  s that the plot 
+00010a50: 7769 6c6c 2062 6520 6472 6177 6e20 746f  will be drawn to
+00010a60: 2e20 4966 206e 6f74 2070 726f 7669 6465  . If not provide
+00010a70: 6420 6120 6e65 7720 6669 6775 7265 2f61  d a new figure/a
+00010a80: 7865 7320 6973 2063 7265 6174 6564 2e0a  xes is created..
+00010a90: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00010aa0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00010ab0: 2020 2020 2020 786c 696d 203d 2078 6c69        xlim = xli
+00010ac0: 6d20 6f72 205b 4e6f 6e65 2c4e 6f6e 655d  m or [None,None]
+00010ad0: 0a20 2020 2020 2020 2020 2020 2079 6c69  .            yli
+00010ae0: 6d20 3d20 796c 696d 206f 7220 5b4e 6f6e  m = ylim or [Non
+00010af0: 652c 4e6f 6e65 5d0a 0a20 2020 2020 2020  e,None]..       
+00010b00: 2020 2020 2072 6177 5f64 6174 6120 3d20       raw_data = 
+00010b10: 7365 6c66 2e72 6177 5f63 6f6e 7472 6173  self.raw_contras
+00010b20: 7428 6c31 2c6c 322c 782c 792c 6c2c 702c  t(l1,l2,x,y,l,p,
+00010b30: 7370 616e 290a 0a20 2020 2020 2020 2020  span)..         
+00010b40: 2020 206c 6973 745f 6c69 6b65 3d28 6c69     list_like=(li
+00010b50: 7374 2c74 7570 6c65 290a 0a20 2020 2020  st,tuple)..     
+00010b60: 2020 2020 2020 2069 6620 2020 2020 6973         if     is
+00010b70: 696e 7374 616e 6365 286c 2c6c 6973 745f  instance(l,list_
+00010b80: 6c69 6b65 2920 616e 6420 6e6f 7420 6973  like) and not is
+00010b90: 696e 7374 616e 6365 286c 315b 305d 2c6c  instance(l1[0],l
+00010ba0: 6973 745f 6c69 6b65 293a 206c 3120 3d20  ist_like): l1 = 
+00010bb0: 5b6c 315d 0a20 2020 2020 2020 2020 2020  [l1].           
+00010bc0: 2069 6620 2020 2020 6973 696e 7374 616e   if     isinstan
+00010bd0: 6365 286c 2c6c 6973 745f 6c69 6b65 2920  ce(l,list_like) 
+00010be0: 616e 6420 6e6f 7420 6973 696e 7374 616e  and not isinstan
+00010bf0: 6365 286c 325b 305d 2c6c 6973 745f 6c69  ce(l2[0],list_li
+00010c00: 6b65 293a 206c 3220 3d20 5b6c 325d 0a20  ke): l2 = [l2]. 
+00010c10: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00010c20: 7420 6973 696e 7374 616e 6365 286c 2c6c  t isinstance(l,l
+00010c30: 6973 745f 6c69 6b65 2920 616e 6420 6e6f  ist_like) and no
+00010c40: 7420 6973 696e 7374 616e 6365 286c 3120  t isinstance(l1 
+00010c50: 2020 2c6c 6973 745f 6c69 6b65 293a 206c    ,list_like): l
+00010c60: 3120 3d20 5b6c 315d 0a20 2020 2020 2020  1 = [l1].       
+00010c70: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
+00010c80: 7374 616e 6365 286c 2c6c 6973 745f 6c69  stance(l,list_li
+00010c90: 6b65 2920 616e 6420 6e6f 7420 6973 696e  ke) and not isin
+00010ca0: 7374 616e 6365 286c 3220 2020 2c6c 6973  stance(l2   ,lis
+00010cb0: 745f 6c69 6b65 293a 206c 3220 3d20 5b6c  t_like): l2 = [l
+00010cc0: 325d 0a0a 2020 2020 2020 2020 2020 2020  2]..            
+00010cd0: 636f 6e74 7261 7374 6572 203d 2028 6c61  contraster = (la
+00010ce0: 6d62 6461 2074 3a20 745b 315d 2d74 5b30  mbda t: t[1]-t[0
+00010cf0: 5d29 2069 6620 6d6f 6465 203d 3d20 2764  ]) if mode == 'd
+00010d00: 6966 6627 2065 6c73 6520 286c 616d 6264  iff' else (lambd
+00010d10: 6120 743a 2069 6e74 2828 745b 315d 2d74  a t: int((t[1]-t
+00010d20: 5b30 5d29 3e30 2929 2069 6620 6d6f 6465  [0])>0)) if mode
+00010d30: 3d3d 2770 726f 6227 2065 6c73 6520 6d6f  =='prob' else mo
+00010d40: 6465 0a20 2020 2020 2020 2020 2020 205f  de.            _
+00010d50: 626f 756e 6461 7279 2020 3d20 3020 6966  boundary  = 0 if
+00010d60: 206d 6f64 6520 3d3d 2027 6469 6666 2720   mode == 'diff' 
+00010d70: 656c 7365 202e 350a 0a20 2020 2020 2020  else .5..       
+00010d80: 2020 2020 2065 7272 6576 6572 7920 3d20       errevery = 
+00010d90: 6572 7265 7665 7279 206f 7220 6d61 7828  errevery or max(
+00010da0: 696e 7428 7261 775f 6461 7461 5b27 7827  int(raw_data['x'
+00010db0: 5d5b 2d31 5d2a 302e 3035 292c 3129 2069  ][-1]*0.05),1) i
+00010dc0: 6620 7820 3d3d 2027 696e 6465 7827 2065  f x == 'index' e
+00010dd0: 6c73 6520 310a 2020 2020 2020 2020 2020  lse 1.          
+00010de0: 2020 7374 796c 6520 2020 203d 2022 2d22    style    = "-"
+00010df0: 2069 6620 7820 3d3d 2027 696e 6465 7827   if x == 'index'
+00010e00: 2065 6c73 6520 222e 220a 2020 2020 2020   else ".".      
+00010e10: 2020 2020 2020 6572 7220 2020 2020 203d        err      =
+00010e20: 2073 656c 662e 5f63 6f6e 6669 6465 6e63   self._confidenc
+00010e30: 6528 6572 722c 2065 7272 6576 6572 7929  e(err, errevery)
+00010e40: 0a0a 2020 2020 2020 2020 2020 2020 585f  ..            X_
+00010e50: 595f 5945 203d 205b 5d0a 2020 2020 2020  Y_YE = [].      
+00010e60: 2020 2020 2020 666f 7220 5f78 692c 2028        for _xi, (
+00010e70: 5f78 2c20 7061 6972 7329 2069 6e20 656e  _x, pairs) in en
+00010e80: 756d 6572 6174 6528 7261 775f 6461 7461  umerate(raw_data
+00010e90: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00010ea0: 2020 2058 5f59 5f59 452e 6170 7065 6e64     X_Y_YE.append
+00010eb0: 2828 5f78 2c29 2b65 7272 286c 6973 7428  ((_x,)+err(list(
+00010ec0: 6d61 7028 636f 6e74 7261 7374 6572 2c70  map(contraster,p
+00010ed0: 6169 7273 2929 2c5f 7869 2929 0a0a 2020  airs)),_xi))..  
+00010ee0: 2020 2020 2020 2020 2020 6c31 5f6c 6162            l1_lab
+00010ef0: 656c 2c6c 325f 6c61 6265 6c20 3d20 7261  el,l2_label = ra
+00010f00: 775f 6461 7461 2e63 6f6c 756d 6e73 5b31  w_data.columns[1
+00010f10: 5d0a 0a20 2020 2020 2020 2020 2020 2069  ]..            i
+00010f20: 6620 7820 3d3d 2027 696e 6465 7827 3a0a  f x == 'index':.
+00010f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f40: 582c 592c 5945 203d 207a 6970 282a 585f  X,Y,YE = zip(*X_
+00010f50: 595f 5945 290a 2020 2020 2020 2020 2020  Y_YE).          
+00010f60: 2020 2020 2020 636f 6c6f 7220 203d 2073        color  = s
+00010f70: 656c 662e 5f67 6574 5f63 6f6c 6f72 2863  elf._get_color(c
+00010f80: 6f6c 6f72 732c 2020 2020 2020 2020 2020  olors,          
+00010f90: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+00010fa0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00010fb0: 2020 6966 206d 6f64 6520 3d3d 2022 6469    if mode == "di
+00010fc0: 6666 223a 0a20 2020 2020 2020 2020 2020  ff":.           
+00010fd0: 2020 2020 2020 2020 206c 6162 656c 2020           label  
+00010fe0: 3d20 7365 6c66 2e5f 6765 745f 6c61 6265  = self._get_labe
+00010ff0: 6c28 6c61 6265 6c73 2c66 277b 6c32 5f6c  l(labels,f'{l2_l
+00011000: 6162 656c 7d20 e280 9420 7b6c 315f 6c61  abel} ... {l1_la
+00011010: 6265 6c7d 272c 3029 0a20 2020 2020 2020  bel}',0).       
+00011020: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011040: 2020 206c 6162 656c 2020 3d20 7365 6c66     label  = self
+00011050: 2e5f 6765 745f 6c61 6265 6c28 6c61 6265  ._get_label(labe
+00011060: 6c73 2c66 2750 5b7b 6c32 5f6c 6162 656c  ls,f'P[{l2_label
+00011070: 7d20 3e20 7b6c 315f 6c61 6265 6c7d 5d27  } > {l1_label}]'
+00011080: 2c30 290a 0a20 2020 2020 2020 2020 2020  ,0)..           
+00011090: 2020 2020 206c 6162 656c 2020 3d20 6622       label  = f"
+000110a0: 7b6c 6162 656c 7d22 2069 6620 6c65 6765  {label}" if lege
+000110b0: 6e64 2065 6c73 6520 4e6f 6e65 0a20 2020  nd else None.   
+000110c0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+000110d0: 6573 2020 3d20 5b50 6f69 6e74 7328 582c  es  = [Points(X,
+000110e0: 2059 2c20 4e6f 6e65 2c20 5945 2c20 7374   Y, None, YE, st
+000110f0: 796c 653d 7374 796c 652c 206c 6162 656c  yle=style, label
+00011100: 3d6c 6162 656c 2c20 636f 6c6f 723d 636f  =label, color=co
+00011110: 6c6f 722c 2061 6c70 6861 3d61 6c70 6861  lor, alpha=alpha
+00011120: 295d 0a0a 2020 2020 2020 2020 2020 2020  )]..            
+00011130: 656c 6966 2078 203d 3d20 6c3a 0a20 2020  elif x == l:.   
+00011140: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00011150: 6c65 6e28 6c31 2920 3e20 3120 616e 6420  len(l1) > 1 and 
+00011160: 6c65 6e28 6c32 2920 3d3d 2031 3a0a 2020  len(l2) == 1:.  
+00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011180: 2020 2353 6f72 7420 6279 206c 312e 2057    #Sort by l1. W
+00011190: 6520 6173 7375 6d65 205f 7820 6973 2066  e assume _x is f
+000111a0: 227b 6c32 7d2d 7b6c 317d 222e 0a20 2020  "{l2}-{l1}"..   
+000111b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111c0: 206c 325f 6c65 6e20 3d20 6c65 6e28 7374   l2_len = len(st
+000111d0: 7228 6c32 5b30 5d29 290a 2020 2020 2020  r(l2[0])).      
+000111e0: 2020 2020 2020 2020 2020 2020 2020 6c31                l1
+000111f0: 203d 206c 6973 7428 6d61 7028 7374 722c   = list(map(str,
+00011200: 6c31 2929 0a20 2020 2020 2020 2020 2020  l1)).           
+00011210: 2020 2020 2020 2020 2058 5f59 5f59 4520           X_Y_YE 
+00011220: 3d20 736f 7274 6564 2858 5f59 5f59 452c  = sorted(X_Y_YE,
+00011230: 206b 6579 3d6c 616d 6264 6120 6974 656d   key=lambda item
+00011240: 733a 206c 312e 696e 6465 7828 6974 656d  s: l1.index(item
+00011250: 735b 305d 5b6c 325f 6c65 6e2b 313a 5d29  s[0][l2_len+1:])
+00011260: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011270: 2020 656c 6966 206c 656e 286c 3229 203e    elif len(l2) >
+00011280: 2031 2061 6e64 206c 656e 286c 3129 203d   1 and len(l1) =
+00011290: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+000112a0: 2020 2020 2020 2020 2023 536f 7274 2062           #Sort b
+000112b0: 7920 6c32 2e20 5765 2061 7373 756d 6520  y l2. We assume 
+000112c0: 5f78 2069 7320 6622 7b6c 327d 2d7b 6c31  _x is f"{l2}-{l1
+000112d0: 7d22 2e0a 2020 2020 2020 2020 2020 2020  }"..            
+000112e0: 2020 2020 2020 2020 6c31 5f6c 656e 203d          l1_len =
+000112f0: 206c 656e 2873 7472 286c 315b 305d 2929   len(str(l1[0]))
+00011300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011310: 2020 2020 206c 3220 3d20 6c69 7374 286d       l2 = list(m
+00011320: 6170 2873 7472 2c6c 3229 290a 2020 2020  ap(str,l2)).    
+00011330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011340: 585f 595f 5945 203d 2073 6f72 7465 6428  X_Y_YE = sorted(
+00011350: 585f 595f 5945 2c20 6b65 793d 6c61 6d62  X_Y_YE, key=lamb
+00011360: 6461 2069 7465 6d73 3a20 6c32 2e69 6e64  da items: l2.ind
+00011370: 6578 2869 7465 6d73 5b30 5d5b 3a2d 286c  ex(items[0][:-(l
+00011380: 315f 6c65 6e2b 3129 5d29 290a 2020 2020  1_len+1)])).    
+00011390: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000113a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000113b0: 2020 2020 2020 585f 595f 5945 203d 2073        X_Y_YE = s
+000113c0: 6f72 7465 6428 585f 595f 5945 290a 0a20  orted(X_Y_YE).. 
+000113d0: 2020 2020 2020 2020 2020 2020 2020 2058                 X
+000113e0: 2c59 2c59 4520 3d20 7a69 7028 2a58 5f59  ,Y,YE = zip(*X_Y
+000113f0: 5f59 4529 0a20 2020 2020 2020 2020 2020  _YE).           
+00011400: 2020 2020 2063 6f6c 6f72 2020 3d20 7365       color  = se
+00011410: 6c66 2e5f 6765 745f 636f 6c6f 7228 636f  lf._get_color(co
+00011420: 6c6f 7273 2c20 3029 0a20 2020 2020 2020  lors, 0).       
+00011430: 2020 2020 2020 2020 206c 696e 6573 2020           lines  
+00011440: 3d20 5b50 6f69 6e74 7328 582c 2059 2c20  = [Points(X, Y, 
+00011450: 4e6f 6e65 2c20 5945 2c20 7374 796c 653d  None, YE, style=
+00011460: 7374 796c 652c 206c 6162 656c 3d4e 6f6e  style, label=Non
+00011470: 652c 2063 6f6c 6f72 3d63 6f6c 6f72 2c20  e, color=color, 
+00011480: 616c 7068 613d 616c 7068 6129 5d0a 0a20  alpha=alpha)].. 
+00011490: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000114a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000114b0: 2075 7070 6572 203d 206c 616d 6264 6120   upper = lambda 
+000114c0: 792c 7965 3a20 792b 7965 5b31 5d20 6966  y,ye: y+ye[1] if
+000114d0: 2069 7369 6e73 7461 6e63 6528 7965 2c28   isinstance(ye,(
+000114e0: 6c69 7374 2c74 7570 6c65 2929 2065 6c73  list,tuple)) els
+000114f0: 6520 792b 7965 0a20 2020 2020 2020 2020  e y+ye.         
+00011500: 2020 2020 2020 206c 6f77 6572 203d 206c         lower = l
+00011510: 616d 6264 6120 792c 7965 3a20 792d 7965  ambda y,ye: y-ye
+00011520: 5b30 5d20 6966 2069 7369 6e73 7461 6e63  [0] if isinstanc
+00011530: 6528 7965 2c28 6c69 7374 2c74 7570 6c65  e(ye,(list,tuple
+00011540: 2929 2065 6c73 6520 792d 7965 0a20 2020  )) else y-ye.   
+00011550: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+00011560: 7020 203d 206c 616d 6264 6120 5f78 3a20  p  = lambda _x: 
+00011570: 7374 7228 5f78 2920 6966 206e 6f74 2078  str(_x) if not x
+00011580: 6f72 6465 7220 656c 7365 205f 780a 0a20  order else _x.. 
+00011590: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000115a0: 7370 6c69 7420 696e 746f 2077 696e 2c74  split into win,t
+000115b0: 6965 2c6c 6f73 730a 2020 2020 2020 2020  ie,loss.        
+000115c0: 2020 2020 2020 2020 6c31 5f77 696e 203d          l1_win =
+000115d0: 205b 2870 7265 7028 7829 2c79 2c79 6529   [(prep(x),y,ye)
+000115e0: 2066 6f72 2078 2c79 2c79 6520 696e 2058   for x,y,ye in X
+000115f0: 5f59 5f59 4520 6966 2075 7070 6572 2879  _Y_YE if upper(y
+00011600: 2c79 6529 203c 2020 5f62 6f75 6e64 6172  ,ye) <  _boundar
+00011610: 7920 2020 2020 2020 2020 2020 2020 2020  y               
+00011620: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
+00011630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011640: 6e6f 5f77 696e 203d 205b 2870 7265 7028  no_win = [(prep(
+00011650: 7829 2c79 2c79 6529 2066 6f72 2078 2c79  x),y,ye) for x,y
+00011660: 2c79 6520 696e 2058 5f59 5f59 4520 6966  ,ye in X_Y_YE if
+00011670: 206c 6f77 6572 2879 2c79 6529 203c 3d20   lower(y,ye) <= 
+00011680: 5f62 6f75 6e64 6172 7920 616e 6420 5f62  _boundary and _b
+00011690: 6f75 6e64 6172 7920 3c3d 2075 7070 6572  oundary <= upper
+000116a0: 2879 2c79 6529 5d0a 2020 2020 2020 2020  (y,ye)].        
+000116b0: 2020 2020 2020 2020 6c32 5f77 696e 203d          l2_win =
+000116c0: 205b 2870 7265 7028 7829 2c79 2c79 6529   [(prep(x),y,ye)
+000116d0: 2066 6f72 2078 2c79 2c79 6520 696e 2058   for x,y,ye in X
+000116e0: 5f59 5f59 4520 6966 2020 2020 2020 2020  _Y_YE if        
+000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011700: 2020 2020 2020 5f62 6f75 6e64 6172 7920        _boundary 
+00011710: 3c20 206c 6f77 6572 2879 2c79 6529 5d0a  <  lower(y,ye)].
+00011720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011730: 2023 736f 7274 2062 7920 6f72 6465 7220   #sort by order 
+00011740: 6f66 206d 6167 6e69 7475 6465 0a20 2020  of magnitude.   
+00011750: 2020 2020 2020 2020 2020 2020 206c 315f               l1_
+00011760: 7769 6e20 3d20 736f 7274 6564 286c 315f  win = sorted(l1_
+00011770: 7769 6e2c 6b65 793d 6974 656d 6765 7474  win,key=itemgett
+00011780: 6572 2831 2929 0a20 2020 2020 2020 2020  er(1)).         
+00011790: 2020 2020 2020 206e 6f5f 7769 6e20 3d20         no_win = 
+000117a0: 736f 7274 6564 286e 6f5f 7769 6e2c 6b65  sorted(no_win,ke
+000117b0: 793d 6974 656d 6765 7474 6572 2831 2929  y=itemgetter(1))
+000117c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000117d0: 206c 325f 7769 6e20 3d20 736f 7274 6564   l2_win = sorted
+000117e0: 286c 325f 7769 6e2c 6b65 793d 6974 656d  (l2_win,key=item
+000117f0: 6765 7474 6572 2831 2929 0a0a 2020 2020  getter(1))..    
+00011800: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+00011810: 7320 3d20 5b5d 0a0a 2020 2020 2020 2020  s = []..        
+00011820: 2020 2020 2020 2020 582c 592c 5945 203d          X,Y,YE =
+00011830: 207a 6970 282a 6c31 5f77 696e 2920 6966   zip(*l1_win) if
+00011840: 206c 315f 7769 6e20 656c 7365 2028 2829   l1_win else (()
+00011850: 2c28 292c 4e6f 6e65 290a 2020 2020 2020  ,(),None).      
+00011860: 2020 2020 2020 2020 2020 636f 6c6f 7220            color 
+00011870: 203d 2073 656c 662e 5f67 6574 5f63 6f6c   = self._get_col
+00011880: 6f72 2863 6f6c 6f72 732c 2020 2020 2020  or(colors,      
+00011890: 2020 2030 290a 2020 2020 2020 2020 2020     0).          
+000118a0: 2020 2020 2020 6c61 6265 6c20 203d 2073        label  = s
+000118b0: 656c 662e 5f67 6574 5f6c 6162 656c 286c  elf._get_label(l
+000118c0: 6162 656c 732c 6c31 5f6c 6162 656c 2c30  abels,l1_label,0
+000118d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000118e0: 2020 6c61 6265 6c20 203d 2066 227b 6c61    label  = f"{la
+000118f0: 6265 6c7d 2028 7b6c 656e 2858 297d 2922  bel} ({len(X)})"
+00011900: 2069 6620 6c65 6765 6e64 2065 6c73 6520   if legend else 
+00011910: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00011920: 2020 2020 206c 696e 6573 2e61 7070 656e       lines.appen
+00011930: 6428 506f 696e 7473 2858 2c20 592c 204e  d(Points(X, Y, N
+00011940: 6f6e 652c 2059 452c 2073 7479 6c65 3d73  one, YE, style=s
+00011950: 7479 6c65 2c20 6c61 6265 6c3d 6c61 6265  tyle, label=labe
+00011960: 6c2c 2063 6f6c 6f72 3d63 6f6c 6f72 2c20  l, color=color, 
+00011970: 616c 7068 613d 616c 7068 6129 290a 0a20  alpha=alpha)).. 
+00011980: 2020 2020 2020 2020 2020 2020 2020 2058                 X
+00011990: 2c59 2c59 4520 3d20 7a69 7028 2a6e 6f5f  ,Y,YE = zip(*no_
+000119a0: 7769 6e29 2069 6620 6e6f 5f77 696e 2065  win) if no_win e
+000119b0: 6c73 6520 2828 292c 2829 2c4e 6f6e 6529  lse ((),(),None)
+000119c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000119d0: 2063 6f6c 6f72 2020 3d20 7365 6c66 2e5f   color  = self._
+000119e0: 6765 745f 636f 6c6f 7228 636f 6c6f 7273  get_color(colors
+000119f0: 2c20 3129 0a20 2020 2020 2020 2020 2020  , 1).           
+00011a00: 2020 2020 206c 6162 656c 2020 3d20 2754       label  = 'T
+00011a10: 6965 270a 2020 2020 2020 2020 2020 2020  ie'.            
+00011a20: 2020 2020 6c61 6265 6c20 203d 2066 227b      label  = f"{
+00011a30: 6c61 6265 6c7d 2028 7b6c 656e 2858 297d  label} ({len(X)}
+00011a40: 2922 2069 6620 6c65 6765 6e64 2065 6c73  )" if legend els
+00011a50: 6520 4e6f 6e65 0a20 2020 2020 2020 2020  e None.         
+00011a60: 2020 2020 2020 206c 696e 6573 2e61 7070         lines.app
+00011a70: 656e 6428 506f 696e 7473 2858 2c20 592c  end(Points(X, Y,
+00011a80: 204e 6f6e 652c 2059 452c 2073 7479 6c65   None, YE, style
+00011a90: 3d73 7479 6c65 2c20 6c61 6265 6c3d 6c61  =style, label=la
+00011aa0: 6265 6c2c 2063 6f6c 6f72 3d63 6f6c 6f72  bel, color=color
+00011ab0: 2c20 616c 7068 613d 616c 7068 6129 290a  , alpha=alpha)).
+00011ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011ad0: 2058 2c59 2c59 4520 3d20 7a69 7028 2a6c   X,Y,YE = zip(*l
+00011ae0: 325f 7769 6e29 2069 6620 6c32 5f77 696e  2_win) if l2_win
+00011af0: 2065 6c73 6520 2828 292c 2829 2c4e 6f6e   else ((),(),Non
+00011b00: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00011b10: 2020 2063 6f6c 6f72 2020 3d20 7365 6c66     color  = self
+00011b20: 2e5f 6765 745f 636f 6c6f 7228 636f 6c6f  ._get_color(colo
+00011b30: 7273 2c20 2020 2020 2020 2020 3229 0a20  rs,         2). 
+00011b40: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00011b50: 6162 656c 2020 3d20 7365 6c66 2e5f 6765  abel  = self._ge
+00011b60: 745f 6c61 6265 6c28 6c61 6265 6c73 2c6c  t_label(labels,l
+00011b70: 325f 6c61 6265 6c2c 3129 0a20 2020 2020  2_label,1).     
+00011b80: 2020 2020 2020 2020 2020 206c 6162 656c             label
+00011b90: 2020 3d20 6622 7b6c 6162 656c 7d20 287b    = f"{label} ({
+00011ba0: 6c65 6e28 5829 7d29 2220 6966 206c 6567  len(X)})" if leg
+00011bb0: 656e 6420 656c 7365 204e 6f6e 650a 2020  end else None.  
+00011bc0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+00011bd0: 6e65 732e 6170 7065 6e64 2850 6f69 6e74  nes.append(Point
+00011be0: 7328 582c 2059 2c20 4e6f 6e65 2c20 5945  s(X, Y, None, YE
+00011bf0: 2c20 7374 796c 653d 7374 796c 652c 206c  , style=style, l
+00011c00: 6162 656c 3d6c 6162 656c 2c20 636f 6c6f  abel=label, colo
+00011c10: 723d 636f 6c6f 722c 2061 6c70 6861 3d61  r=color, alpha=a
+00011c20: 6c70 6861 2929 0a0a 2020 2020 2020 2020  lpha))..        
+00011c30: 2020 2020 7872 6f74 6174 696f 6e20 3d20      xrotation = 
+00011c40: 3930 2069 6620 2878 2021 3d20 2769 6e64  90 if (x != 'ind
+00011c50: 6578 2720 6f72 2078 6f72 6465 7229 2061  ex' or xorder) a
+00011c60: 6e64 206c 656e 2858 5f59 5f59 4529 3e35  nd len(X_Y_YE)>5
+00011c70: 2065 6c73 6520 300a 2020 2020 2020 2020   else 0.        
+00011c80: 2020 2020 7972 6f74 6174 696f 6e20 3d20      yrotation = 
+00011c90: 300a 0a20 2020 2020 2020 2020 2020 205f  0..            _
+00011ca0: 5920 3d20 7261 775f 6461 7461 5b72 6177  Y = raw_data[raw
+00011cb0: 5f64 6174 612e 636f 6c75 6d6e 735b 315d  _data.columns[1]
+00011cc0: 5d5b 305d 0a0a 2020 2020 2020 2020 2020  ][0]..          
+00011cd0: 2020 786c 6162 656c 203d 2078 6c61 6265    xlabel = xlabe
+00011ce0: 6c20 6f72 2028 2249 6e74 6572 6163 7469  l or ("Interacti
+00011cf0: 6f6e 2220 6966 2078 3d3d 2769 6e64 6578  on" if x=='index
+00011d00: 2720 656c 7365 2078 5b30 5d20 6966 206c  ' else x[0] if l
+00011d10: 656e 2878 2920 3d3d 2031 2065 6c73 6520  en(x) == 1 else 
+00011d20: 7829 0a20 2020 2020 2020 2020 2020 2079  x).            y
+00011d30: 6c61 6265 6c20 3d20 796c 6162 656c 206f  label = ylabel o
+00011d40: 7220 2866 2224 5c44 656c 7461 2420 7b79  r (f"$\Delta$ {y
+00011d50: 7d22 2069 6620 6d6f 6465 3d3d 2264 6966  }" if mode=="dif
+00011d60: 6622 2065 6c73 6520 6622 5028 245c 4465  f" else f"P($\De
+00011d70: 6c74 6124 207b 797d 203e 2030 2922 290a  lta$ {y} > 0)").
+00011d80: 2020 2020 2020 2020 2020 2020 7469 746c              titl
+00011d90: 6520 203d 2074 6974 6c65 2069 6620 7469  e  = title if ti
+00011da0: 746c 6520 6973 206e 6f74 204e 6f6e 6520  tle is not None 
+00011db0: 656c 7365 2028 6622 7b79 6c61 6265 6c7d  else (f"{ylabel}
+00011dc0: 2028 7b6c 656e 285f 5929 7d20 456e 7669   ({len(_Y)} Envi
+00011dd0: 726f 6e6d 656e 7473 2922 290a 0a20 2020  ronments)")..   
+00011de0: 2020 2020 2020 2020 2061 6c6c 5f78 203d           all_x =
+00011df0: 2064 6963 742e 6672 6f6d 6b65 7973 2863   dict.fromkeys(c
+00011e00: 6861 696e 2e66 726f 6d5f 6974 6572 6162  hain.from_iterab
+00011e10: 6c65 286c 696e 652e 5820 666f 7220 6c69  le(line.X for li
+00011e20: 6e65 2069 6e20 6c69 6e65 7329 290a 2020  ne in lines)).  
+00011e30: 2020 2020 2020 2020 2020 786f 7264 6572            xorder
+00011e40: 6564 203d 206c 6973 7428 616c 6c5f 782e  ed = list(all_x.
+00011e50: 6b65 7973 2829 2920 6966 206e 6f74 2078  keys()) if not x
+00011e60: 6f72 6465 7220 656c 7365 2073 6f72 7465  order else sorte
+00011e70: 6428 616c 6c5f 782c 2072 6576 6572 7365  d(all_x, reverse
+00011e80: 3d78 6f72 6465 723d 3d27 2d27 290a 0a20  =xorder=='-').. 
+00011e90: 2020 2020 2020 2020 2020 2069 6620 626f             if bo
+00011ea0: 756e 6461 7279 3a0a 2020 2020 2020 2020  undary:.        
+00011eb0: 2020 2020 2020 2020 6c69 6e65 732e 6170          lines.ap
+00011ec0: 7065 6e64 2850 6f69 6e74 7328 2878 6f72  pend(Points((xor
+00011ed0: 6465 7265 645b 305d 2c78 6f72 6465 7265  dered[0],xordere
+00011ee0: 645b 2d31 5d29 2c28 5f62 6f75 6e64 6172  d[-1]),(_boundar
+00011ef0: 792c 5f62 6f75 6e64 6172 7929 2c20 4e6f  y,_boundary), No
+00011f00: 6e65 2c20 4e6f 6e65 202c 2022 2338 3838  ne, None , "#888
+00011f10: 222c 2031 2c20 4e6f 6e65 2c20 272d 272c  ", 1, None, '-',
+00011f20: 2e35 2929 0a0a 2020 2020 2020 2020 2020  .5))..          
+00011f30: 2020 6966 2078 203d 3d20 2769 6e64 6578    if x == 'index
+00011f40: 2720 616e 6420 786f 7264 6572 2069 6e20  ' and xorder in 
+00011f50: 5b27 2b27 2c4e 6f6e 655d 3a0a 2020 2020  ['+',None]:.    
+00011f60: 2020 2020 2020 2020 2020 2020 786f 7264              xord
+00011f70: 6572 6564 203d 204e 6f6e 650a 0a20 2020  ered = None..   
+00011f80: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
+00011f90: 6c6f 7474 6572 2e70 6c6f 7428 6178 2c20  lotter.plot(ax, 
+00011fa0: 6c69 6e65 732c 2074 6974 6c65 2c20 786c  lines, title, xl
+00011fb0: 6162 656c 2c20 796c 6162 656c 2c20 786c  abel, ylabel, xl
+00011fc0: 696d 2c20 796c 696d 2c20 7874 6963 6b73  im, ylim, xticks
+00011fd0: 2c20 7974 6963 6b73 2c20 6c65 6765 6e64  , yticks, legend
+00011fe0: 2c20 7872 6f74 6174 696f 6e2c 2079 726f  , xrotation, yro
+00011ff0: 7461 7469 6f6e 2c20 786f 7264 6572 6564  tation, xordered
+00012000: 2c20 6f75 7429 0a0a 2020 2020 2020 2020  , out)..        
+00012010: 6578 6365 7074 2043 6f62 6145 7863 6570  except CobaExcep
+00012020: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
+00012030: 2020 2020 2020 2043 6f62 6143 6f6e 7465         CobaConte
+00012040: 7874 2e6c 6f67 6765 722e 6c6f 6728 7374  xt.logger.log(st
+00012050: 7228 6529 290a 0a20 2020 2064 6566 205f  r(e))..    def _
+00012060: 5f73 7472 5f5f 2873 656c 6629 202d 3e20  _str__(self) -> 
+00012070: 7374 723a 0a20 2020 2020 2020 2072 6574  str:.        ret
+00012080: 7572 6e20 7374 7228 7b22 4c65 6172 6e65  urn str({"Learne
+00012090: 7273 223a 206c 656e 2873 656c 662e 5f6c  rs": len(self._l
+000120a0: 6561 726e 6572 7329 2c20 2245 6e76 6972  earners), "Envir
+000120b0: 6f6e 6d65 6e74 7322 3a20 6c65 6e28 7365  onments": len(se
+000120c0: 6c66 2e5f 656e 7669 726f 6e6d 656e 7473  lf._environments
+000120d0: 292c 2022 496e 7465 7261 6374 696f 6e73  ), "Interactions
+000120e0: 223a 206c 656e 2873 656c 662e 5f69 6e74  ": len(self._int
+000120f0: 6572 6163 7469 6f6e 7329 207d 290a 0a20  eractions) }).. 
+00012100: 2020 2064 6566 205f 5f65 715f 5f28 7365     def __eq__(se
+00012110: 6c66 2c20 6f3a 206f 626a 6563 7429 202d  lf, o: object) -
+00012120: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00012130: 7265 7475 726e 2069 7369 6e73 7461 6e63  return isinstanc
+00012140: 6528 6f2c 5265 7375 6c74 2920 5c0a 2020  e(o,Result) \.  
+00012150: 2020 2020 2020 2020 2061 6e64 206f 2e65           and o.e
+00012160: 6e76 6972 6f6e 6d65 6e74 7320 3d3d 2073  nvironments == s
+00012170: 656c 662e 656e 7669 726f 6e6d 656e 7473  elf.environments
+00012180: 205c 0a20 2020 2020 2020 2020 2020 616e   \.           an
+00012190: 6420 6f2e 6c65 6172 6e65 7273 203d 3d20  d o.learners == 
+000121a0: 7365 6c66 2e6c 6561 726e 6572 7320 5c0a  self.learners \.
+000121b0: 2020 2020 2020 2020 2020 2061 6e64 206f             and o
+000121c0: 2e65 7661 6c75 6174 6f72 7320 3d3d 2073  .evaluators == s
+000121d0: 656c 662e 6576 616c 7561 746f 7273 0a0a  elf.evaluators..
+000121e0: 2020 2020 6465 6620 5f69 7079 7468 6f6e      def _ipython
+000121f0: 5f64 6973 706c 6179 5f28 7365 6c66 293a  _display_(self):
+00012200: 0a20 2020 2020 2020 2023 7072 6574 7479  .        #pretty
+00012210: 2070 7269 6e74 2069 6e20 6a75 7079 7465   print in jupyte
+00012220: 7220 6e6f 7465 626f 6f6b 2028 6874 7470  r notebook (http
+00012230: 733a 2f2f 6970 7974 686f 6e2e 7265 6164  s://ipython.read
+00012240: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
+00012250: 6162 6c65 2f63 6f6e 6669 672f 696e 7465  able/config/inte
+00012260: 6772 6174 696e 672e 6874 6d6c 290a 2020  grating.html).  
+00012270: 2020 2020 2020 7072 696e 7428 7374 7228        print(str(
+00012280: 7365 6c66 2929 0a0a 2020 2020 6465 6620  self))..    def 
+00012290: 5f67 6574 5f63 6f6c 6f72 2873 656c 662c  _get_color(self,
+000122a0: 2063 6f6c 6f72 733a 556e 696f 6e5b 4e6f   colors:Union[No
+000122b0: 6e65 2c53 6571 7565 6e63 655b 556e 696f  ne,Sequence[Unio
+000122c0: 6e5b 7374 722c 696e 745d 5d5d 2c20 693a  n[str,int]]], i:
+000122d0: 696e 7429 202d 3e20 556e 696f 6e5b 7374  int) -> Union[st
+000122e0: 722c 696e 745d 3a0a 2020 2020 2020 2020  r,int]:.        
+000122f0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00012300: 2072 6574 7572 6e20 636f 6c6f 7273 2069   return colors i
+00012310: 6620 6973 696e 7374 616e 6365 2863 6f6c  f isinstance(col
+00012320: 6f72 732c 7374 7229 2065 6c73 6520 636f  ors,str) else co
+00012330: 6c6f 7273 5b69 5d20 6966 2063 6f6c 6f72  lors[i] if color
+00012340: 7320 656c 7365 2069 0a20 2020 2020 2020  s else i.       
+00012350: 2065 7863 6570 7420 496e 6465 7845 7272   except IndexErr
+00012360: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+00012370: 7265 7475 726e 2069 2b6d 6178 2863 6f6c  return i+max(col
+00012380: 6f72 7329 2069 6620 6973 696e 7374 616e  ors) if isinstan
+00012390: 6365 2863 6f6c 6f72 735b 305d 2c28 696e  ce(colors[0],(in
+000123a0: 742c 666c 6f61 7429 2920 656c 7365 2069  t,float)) else i
+000123b0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+000123c0: 5479 7065 4572 726f 723a 0a20 2020 2020  TypeError:.     
+000123d0: 2020 2020 2020 2072 6574 7572 6e20 692b         return i+
+000123e0: 636f 6c6f 7273 0a0a 2020 2020 6465 6620  colors..    def 
+000123f0: 5f67 6574 5f6c 6162 656c 2873 656c 662c  _get_label(self,
+00012400: 206c 6162 656c 733a 5365 7175 656e 6365   labels:Sequence
+00012410: 5b73 7472 5d2c 206c 6162 656c 3a73 7472  [str], label:str
+00012420: 2c20 693a 696e 7429 202d 3e20 7374 723a  , i:int) -> str:
+00012430: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00012440: 2020 2020 2020 2020 2020 6c61 6265 6c20            label 
+00012450: 3d20 6c61 6265 6c73 2069 6620 6973 696e  = labels if isin
+00012460: 7374 616e 6365 286c 6162 656c 732c 7374  stance(labels,st
+00012470: 7229 2065 6c73 6520 6c61 6265 6c73 5b69  r) else labels[i
+00012480: 5d20 6966 206c 6162 656c 7320 656c 7365  ] if labels else
+00012490: 206c 6162 656c 0a20 2020 2020 2020 2065   label.        e
+000124a0: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
+000124b0: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
+000124c0: 7265 7475 726e 2073 7472 286c 6162 656c  return str(label
+000124d0: 290a 0a20 2020 2064 6566 205f 706c 6f74  )..    def _plot
+000124e0: 7461 626c 6528 7365 6c66 2c20 783a 5365  table(self, x:Se
+000124f0: 7175 656e 6365 5b73 7472 5d2c 2079 3a73  quence[str], y:s
+00012500: 7472 2920 2d3e 2027 5265 7375 6c74 273a  tr) -> 'Result':
+00012510: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00012520: 2069 7369 6e73 7461 6e63 6528 782c 7374   isinstance(x,st
+00012530: 7229 2061 6e64 2027 696e 6465 7827 2069  r) and 'index' i
+00012540: 6e20 7820 616e 6420 6c65 6e28 7829 203e  n x and len(x) >
+00012550: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00012560: 7261 6973 6520 436f 6261 4578 6365 7074  raise CobaExcept
+00012570: 696f 6e28 2754 6865 2078 2d61 7869 7320  ion('The x-axis 
+00012580: 6361 6e6e 6f74 2063 6f6e 7461 696e 2062  cannot contain b
+00012590: 6f74 6820 696e 6465 7865 7320 616e 6420  oth indexes and 
+000125a0: 7061 7261 6d65 7465 7273 2e27 290a 0a20  parameters.').. 
+000125b0: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
+000125c0: 6c66 2e69 6e74 6572 6163 7469 6f6e 7329  lf.interactions)
+000125d0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+000125e0: 2020 2072 6169 7365 2043 6f62 6145 7863     raise CobaExc
+000125f0: 6570 7469 6f6e 2822 5468 6973 2072 6573  eption("This res
+00012600: 756c 7420 646f 6573 206e 6f74 2063 6f6e  ult does not con
+00012610: 7461 696e 2061 6e79 2064 6174 6120 746f  tain any data to
+00012620: 2070 6c6f 742e 2229 0a0a 2020 2020 2020   plot.")..      
+00012630: 2020 6966 2079 206e 6f74 2069 6e20 7365    if y not in se
+00012640: 6c66 2e69 6e74 6572 6163 7469 6f6e 732e  lf.interactions.
+00012650: 636f 6c75 6d6e 733a 0a20 2020 2020 2020  columns:.       
+00012660: 2020 2020 2072 6169 7365 2043 6f62 6145       raise CobaE
+00012670: 7863 6570 7469 6f6e 2866 2254 6869 7320  xception(f"This 
+00012680: 7265 7375 6c74 2064 6f65 7320 6e6f 7420  result does not 
+00012690: 636f 6e74 6169 6e20 636f 6c75 6d6e 2027  contain column '
+000126a0: 7b79 7d27 2069 6e20 696e 7465 7261 6374  {y}' in interact
+000126b0: 696f 6e73 2e22 290a 0a20 2020 2020 2020  ions.")..       
+000126c0: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
+000126d0: 2020 6465 6620 5f66 696e 6973 6865 6428    def _finished(
+000126e0: 7365 6c66 2c20 783a 5365 7175 656e 6365  self, x:Sequence
+000126f0: 5b73 7472 5d2c 2079 3a73 7472 2c20 6c3a  [str], y:str, l:
+00012700: 5365 7175 656e 6365 5b73 7472 5d2c 2070  Sequence[str], p
+00012710: 3a53 6571 7565 6e63 655b 7374 725d 2920  :Sequence[str]) 
+00012720: 2d3e 2027 5265 7375 6c74 273a 0a20 2020  -> 'Result':.   
+00012730: 2020 2020 206f 6e6c 795f 6669 6e69 7368       only_finish
+00012740: 6564 203d 2073 656c 662e 5f66 696c 7465  ed = self._filte
+00012750: 725f 6669 6e28 276d 696e 2720 6966 2078  r_fin('min' if x
+00012760: 203d 3d20 2769 6e64 6578 2720 656c 7365   == 'index' else
+00012770: 204e 6f6e 652c 206c 2c20 7029 0a20 2020   None, l, p).   
+00012780: 2020 2020 2069 6620 6c65 6e28 6f6e 6c79       if len(only
+00012790: 5f66 696e 6973 6865 642e 6c65 6172 6e65  _finished.learne
+000127a0: 7273 2920 3d3d 2030 3a0a 2020 2020 2020  rs) == 0:.      
+000127b0: 2020 2020 2020 7261 6973 6520 436f 6261        raise Coba
+000127c0: 4578 6365 7074 696f 6e28 6622 5468 6973  Exception(f"This
+000127d0: 2072 6573 756c 7420 646f 6573 206e 6f74   result does not
+000127e0: 2063 6f6e 7461 696e 2061 207b 707d 2074   contain a {p} t
+000127f0: 6861 7420 6861 7320 6265 656e 2066 696e  hat has been fin
+00012800: 6973 6865 6420 666f 7220 6576 6572 7920  ished for every 
+00012810: 7b6c 7d2e 2229 0a20 2020 2020 2020 2072  {l}.").        r
+00012820: 6574 7572 6e20 6f6e 6c79 5f66 696e 6973  eturn only_finis
+00012830: 6865 640a 0a20 2020 2064 6566 205f 636f  hed..    def _co
+00012840: 6e66 6964 656e 6365 2873 656c 662c 2065  nfidence(self, e
+00012850: 7272 3a20 556e 696f 6e5b 7374 722c 506f  rr: Union[str,Po
+00012860: 696e 7441 6e64 496e 7465 7276 616c 5d2c  intAndInterval],
+00012870: 2065 7272 6576 6572 793a 696e 7420 3d20   errevery:int = 
+00012880: 3129 3a0a 0a20 2020 2020 2020 2069 6620  1):..        if 
+00012890: 6572 7220 3d3d 2027 7365 273a 0a20 2020  err == 'se':.   
+000128a0: 2020 2020 2020 2020 2063 6920 3d20 5374           ci = St
+000128b0: 6445 7272 4349 282e 3935 290a 2020 2020  dErrCI(.95).    
+000128c0: 2020 2020 656c 6966 2065 7272 203d 3d20      elif err == 
+000128d0: 2762 7327 3a0a 2020 2020 2020 2020 2020  'bs':.          
+000128e0: 2020 6369 203d 2042 6f6f 7473 7472 6170    ci = Bootstrap
+000128f0: 4349 282e 3935 2c20 6d65 616e 290a 2020  CI(.95, mean).  
+00012900: 2020 2020 2020 656c 6966 2065 7272 203d        elif err =
+00012910: 3d20 2762 6927 3a0a 2020 2020 2020 2020  = 'bi':.        
+00012920: 2020 2020 6369 203d 2042 696e 6f6d 6961      ci = Binomia
+00012930: 6c43 4928 2777 696c 736f 6e27 290a 2020  lCI('wilson').  
+00012940: 2020 2020 2020 656c 6966 2065 7272 203d        elif err =
+00012950: 3d20 2773 6427 3a0a 2020 2020 2020 2020  = 'sd':.        
+00012960: 2020 2020 6369 203d 2053 7464 4465 7643      ci = StdDevC
+00012970: 4928 290a 2020 2020 2020 2020 656c 6966  I().        elif
+00012980: 2065 7272 2069 7320 4e6f 6e65 206f 7220   err is None or 
+00012990: 6973 696e 7374 616e 6365 2865 7272 2c73  isinstance(err,s
+000129a0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+000129b0: 2063 6920 3d20 4e6f 6e65 0a20 2020 2020   ci = None.     
+000129c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000129d0: 2020 2020 2063 6920 3d20 6572 720a 0a20       ci = err.. 
+000129e0: 2020 2020 2020 2064 6566 2063 616c 635f         def calc_
+000129f0: 6369 285a 3a53 6571 7565 6e63 655b 666c  ci(Z:Sequence[fl
+00012a00: 6f61 745d 2c20 693a 696e 7420 3d20 2d31  oat], i:int = -1
+00012a10: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00012a20: 6620 6369 2069 7320 4e6f 6e65 3a0a 2020  f ci is None:.  
+00012a30: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00012a40: 7475 726e 2028 6d65 616e 285a 292c 3029  turn (mean(Z),0)
+00012a50: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00012a60: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00012a70: 2020 2073 6b69 705f 6572 7220 3d20 2869     skip_err = (i
+00012a80: 2b31 2925 6572 7265 7665 7279 0a20 2020  +1)%errevery.   
+00012a90: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00012aa0: 7572 6e20 2863 692e 706f 696e 7428 5a29  urn (ci.point(Z)
+00012ab0: 2c20 2830 2c30 2929 2069 6620 736b 6970  , (0,0)) if skip
+00012ac0: 5f65 7272 2065 6c73 6520 6369 2e70 6f69  _err else ci.poi
+00012ad0: 6e74 5f69 6e74 6572 7661 6c28 5a29 0a0a  nt_interval(Z)..
+00012ae0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00012af0: 616c 635f 6369 0a0a 2020 2020 6465 6620  alc_ci..    def 
+00012b00: 5f67 726f 7570 6564 5f79 7328 7365 6c66  _grouped_ys(self
+00012b10: 2c20 2a6b 6579 733a 2073 7472 2c20 793a  , *keys: str, y:
+00012b20: 4f70 7469 6f6e 616c 5b73 7472 5d2c 2066  Optional[str], f
+00012b30: 756e 633a 204c 6974 6572 616c 5b27 6c61  unc: Literal['la
+00012b40: 7374 272c 276c 6973 7427 5d20 3d20 4e6f  st','list'] = No
+00012b50: 6e65 2c20 6361 7264 3a20 4c69 7465 7261  ne, card: Litera
+00012b60: 6c5b 2747 272c 2753 275d 203d 2027 4727  l['G','S'] = 'G'
+00012b70: 2c20 7370 616e 3a4f 7074 696f 6e61 6c5b  , span:Optional[
+00012b80: 696e 745d 3d31 2920 2d3e 2053 6571 7565  int]=1) -> Seque
+00012b90: 6e63 655b 5475 706c 655d 3a0a 0a20 2020  nce[Tuple]:..   
+00012ba0: 2020 2020 2065 6e76 5f63 6163 6865 203d       env_cache =
+00012bb0: 2073 656c 662e 5f65 6e76 5f63 6163 6865   self._env_cache
+00012bc0: 0a20 2020 2020 2020 206c 726e 5f63 6163  .        lrn_cac
+00012bd0: 6865 203d 2073 656c 662e 5f6c 726e 5f63  he = self._lrn_c
+00012be0: 6163 6865 0a20 2020 2020 2020 2076 616c  ache.        val
+00012bf0: 5f63 6163 6865 203d 2073 656c 662e 5f76  _cache = self._v
+00012c00: 616c 5f63 6163 6865 0a0a 2020 2020 2020  al_cache..      
+00012c10: 2020 6e65 6564 5f68 6173 6865 7220 3d20    need_hasher = 
+00012c20: 4e6f 6e65 0a0a 2020 2020 2020 2020 4420  None..        D 
+00012c30: 3d20 6469 6374 2829 2069 6620 6361 7264  = dict() if card
+00012c40: 203d 3d20 2753 2720 656c 7365 2064 6566   == 'S' else def
+00012c50: 6175 6c74 6469 6374 286c 6973 7429 0a0a  aultdict(list)..
+00012c60: 2020 2020 2020 2020 6465 6620 6973 5f69          def is_i
+00012c70: 636f 6c28 6b65 7929 3a0a 2020 2020 2020  col(key):.      
+00012c80: 2020 2020 2020 7265 7475 726e 206b 6579        return key
+00012c90: 206e 6f74 2069 6e20 5b27 656e 7669 726f   not in ['enviro
+00012ca0: 6e6d 656e 745f 6964 272c 276c 6561 726e  nment_id','learn
+00012cb0: 6572 5f69 6427 2c27 6576 616c 7561 746f  er_id','evaluato
+00012cc0: 725f 6964 275d 2061 6e64 206b 6579 2069  r_id'] and key i
+00012cd0: 6e20 7365 6c66 2e69 6e74 6572 6163 7469  n self.interacti
+00012ce0: 6f6e 732e 636f 6c75 6d6e 730a 0a20 2020  ons.columns..   
+00012cf0: 2020 2020 2064 6566 2067 6574 5f69 636f       def get_ico
+00012d00: 6c73 286b 6579 7329 3a0a 2020 2020 2020  ls(keys):.      
+00012d10: 2020 2020 2020 666f 7220 6b65 7920 696e        for key in
+00012d20: 206b 6579 733a 0a20 2020 2020 2020 2020   keys:.         
+00012d30: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00012d40: 616e 6365 286b 6579 2c28 6c69 7374 2c74  ance(key,(list,t
+00012d50: 7570 6c65 2929 3a0a 2020 2020 2020 2020  uple)):.        
+00012d60: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
+00012d70: 6420 6672 6f6d 2067 6574 5f69 636f 6c73  d from get_icols
+00012d80: 286b 6579 290a 2020 2020 2020 2020 2020  (key).          
+00012d90: 2020 2020 2020 656c 6966 2069 735f 6963        elif is_ic
+00012da0: 6f6c 286b 6579 293a 0a20 2020 2020 2020  ol(key):.       
+00012db0: 2020 2020 2020 2020 2020 2020 2079 6965               yie
+00012dc0: 6c64 206b 6579 0a0a 2020 2020 2020 2020  ld key..        
+00012dd0: 6465 6620 6d61 6b65 5f67 6574 7328 636f  def make_gets(co
+00012de0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00012df0: 2066 6f72 2063 6f6c 2069 6e20 636f 6c73   for col in cols
+00012e00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012e10: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00012e20: 636f 6c2c 2874 7570 6c65 2c6c 6973 7429  col,(tuple,list)
+00012e30: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00012e40: 2020 2020 2020 2079 6965 6c64 206c 616d         yield lam
+00012e50: 6264 6120 652c 6c2c 762c 732c 4e2c 473d  bda e,l,v,s,N,G=
+00012e60: 6c69 7374 286d 616b 655f 6765 7473 2863  list(make_gets(c
+00012e70: 6f6c 2929 3a20 7a69 7028 2a6d 6170 286d  ol)): zip(*map(m
+00012e80: 6574 686f 6463 616c 6c65 7228 275f 5f63  ethodcaller('__c
+00012e90: 616c 6c5f 5f27 2c65 2c6c 2c76 2c73 2c4e  all__',e,l,v,s,N
+00012ea0: 292c 4729 2920 6966 204e 2021 3d20 3020  ),G)) if N != 0 
+00012eb0: 656c 7365 2074 7570 6c65 286d 6170 286d  else tuple(map(m
+00012ec0: 6574 686f 6463 616c 6c65 7228 275f 5f63  ethodcaller('__c
+00012ed0: 616c 6c5f 5f27 2c65 2c6c 2c76 2c73 2c4e  all__',e,l,v,s,N
+00012ee0: 292c 4729 290a 2020 2020 2020 2020 2020  ),G)).          
+00012ef0: 2020 2020 2020 656c 6966 2063 6f6c 2069        elif col i
+00012f00: 6e20 7365 6c66 2e65 6e76 6972 6f6e 6d65  n self.environme
+00012f10: 6e74 732e 636f 6c75 6d6e 733a 0a20 2020  nts.columns:.   
+00012f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f30: 2079 6965 6c64 206c 616d 6264 6120 652c   yield lambda e,
+00012f40: 6c2c 762c 732c 4e2c 636f 6c3d 636f 6c3a  l,v,s,N,col=col:
+00012f50: 2072 6570 6561 7428 655b 636f 6c5d 2c4e   repeat(e[col],N
+00012f60: 2920 6966 204e 2021 3d20 3020 656c 7365  ) if N != 0 else
+00012f70: 2065 5b63 6f6c 5d0a 2020 2020 2020 2020   e[col].        
+00012f80: 2020 2020 2020 2020 656c 6966 2063 6f6c          elif col
+00012f90: 2069 6e20 7365 6c66 2e6c 6561 726e 6572   in self.learner
+00012fa0: 732e 636f 6c75 6d6e 7320 6f72 2063 6f6c  s.columns or col
+00012fb0: 203d 3d20 2766 756c 6c5f 6e61 6d65 273a   == 'full_name':
+00012fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012fd0: 2020 2020 2079 6965 6c64 206c 616d 6264       yield lambd
+00012fe0: 6120 652c 6c2c 762c 732c 4e2c 636f 6c3d  a e,l,v,s,N,col=
+00012ff0: 636f 6c3a 2072 6570 6561 7428 6c5b 636f  col: repeat(l[co
+00013000: 6c5d 2c4e 2920 6966 204e 2021 3d20 3020  l],N) if N != 0 
+00013010: 656c 7365 206c 5b63 6f6c 5d0a 2020 2020  else l[col].    
+00013020: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00013030: 2063 6f6c 2069 6e20 7365 6c66 2e65 7661   col in self.eva
+00013040: 6c75 6174 6f72 732e 636f 6c75 6d6e 733a  luators.columns:
+00013050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013060: 2020 2020 2079 6965 6c64 206c 616d 6264       yield lambd
+00013070: 6120 652c 6c2c 762c 732c 4e2c 636f 6c3d  a e,l,v,s,N,col=
+00013080: 636f 6c3a 2072 6570 6561 7428 765b 636f  col: repeat(v[co
+00013090: 6c5d 2c4e 2920 6966 204e 2021 3d20 3020  l],N) if N != 0 
+000130a0: 656c 7365 2076 5b63 6f6c 5d0a 2020 2020  else v[col].    
+000130b0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+000130c0: 2063 6f6c 2069 6e20 7365 6c66 2e69 6e74   col in self.int
+000130d0: 6572 6163 7469 6f6e 732e 636f 6c75 6d6e  eractions.column
+000130e0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000130f0: 2020 2020 2020 2079 6965 6c64 206c 616d         yield lam
+00013100: 6264 6120 652c 6c2c 762c 732c 4e2c 636f  bda e,l,v,s,N,co
+00013110: 6c3d 636f 6c3a 2069 7465 7228 732e 706f  l=col: iter(s.po
+00013120: 7028 2929 0a0a 2020 2020 2020 2020 6765  p())..        ge
+00013130: 7473 2020 3d20 6c69 7374 286d 616b 655f  ts  = list(make_
+00013140: 6765 7473 286b 6579 7329 290a 2020 2020  gets(keys)).    
+00013150: 2020 2020 6963 6f6c 7320 3d20 6c69 7374      icols = list
+00013160: 2867 6574 5f69 636f 6c73 286b 6579 7329  (get_icols(keys)
+00013170: 290a 2020 2020 2020 2020 6963 6f6c 732e  ).        icols.
+00013180: 7265 7665 7273 6528 290a 0a20 2020 2020  reverse()..     
+00013190: 2020 2069 6620 793a 2069 636f 6c73 202b     if y: icols +
+000131a0: 3d20 5b79 5d0a 2020 2020 2020 2020 666f  = [y].        fo
+000131b0: 7220 2865 6964 2c6c 6964 2c76 6964 292c  r (eid,lid,vid),
+000131c0: 2073 656c 2069 6e20 7365 6c66 2e69 6e74   sel in self.int
+000131d0: 6572 6163 7469 6f6e 732e 6772 6f75 7062  eractions.groupb
+000131e0: 7928 332c 6963 6f6c 7329 3a0a 0a20 2020  y(3,icols):..   
+000131f0: 2020 2020 2020 2020 2065 6e76 203d 2065           env = e
+00013200: 6e76 5f63 6163 6865 5b65 6964 5d0a 2020  nv_cache[eid].  
+00013210: 2020 2020 2020 2020 2020 6c72 6e20 3d20            lrn = 
+00013220: 6c72 6e5f 6361 6368 655b 6c69 645d 0a20  lrn_cache[lid]. 
+00013230: 2020 2020 2020 2020 2020 2076 616c 203d             val =
+00013240: 2076 616c 5f63 6163 6865 5b76 6964 5d0a   val_cache[vid].
+00013250: 0a20 2020 2020 2020 2020 2020 2059 203d  .            Y =
+00013260: 2073 656c 2e70 6f70 2829 2069 6620 7920   sel.pop() if y 
+00013270: 656c 7365 204e 6f6e 650a 2020 2020 2020  else None.      
+00013280: 2020 2020 2020 4e20 3d20 3020 6966 206e        N = 0 if n
+00013290: 6f74 2073 656c 2065 6c73 6520 6c65 6e28  ot sel else len(
+000132a0: 7365 6c5b 305d 290a 0a20 2020 2020 2020  sel[0])..       
+000132b0: 2020 2020 206f 7574 7320 3d20 7475 706c       outs = tupl
+000132c0: 6528 6d61 7028 6d65 7468 6f64 6361 6c6c  e(map(methodcall
+000132d0: 6572 2827 5f5f 6361 6c6c 5f5f 272c 656e  er('__call__',en
+000132e0: 762c 6c72 6e2c 7661 6c2c 7365 6c2c 4e29  v,lrn,val,sel,N)
+000132f0: 2c67 6574 7329 290a 0a20 2020 2020 2020  ,gets))..       
+00013300: 2020 2020 2069 6620 4e20 213d 2030 3a20       if N != 0: 
+00013310: 6f75 7473 203d 207a 6970 282a 6f75 7473  outs = zip(*outs
+00013320: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00013330: 204e 203d 3d20 3020 616e 6420 6675 6e63   N == 0 and func
+00013340: 2069 7320 4e6f 6e65 2061 6e64 2079 2069   is None and y i
+00013350: 7320 6e6f 7420 4e6f 6e65 3a20 6675 6e63  s not None: func
+00013360: 203d 2027 6c61 7374 270a 0a20 2020 2020   = 'last'..     
+00013370: 2020 2020 2020 2069 6620 6e65 6564 5f68         if need_h
+00013380: 6173 6865 7220 6973 204e 6f6e 653a 0a20  asher is None:. 
+00013390: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+000133a0: 7574 2c20 6f75 7473 203d 2028 6f75 7473  ut, outs = (outs
+000133b0: 2c20 6f75 7473 2920 6966 204e 203d 3d20  , outs) if N == 
+000133c0: 3020 656c 7365 2070 6565 6b5f 6669 7273  0 else peek_firs
+000133d0: 7428 6f75 7473 290a 2020 2020 2020 2020  t(outs).        
+000133e0: 2020 2020 2020 2020 6e65 6564 5f68 6173          need_has
+000133f0: 6865 7220 3d20 7472 795f 656c 7365 286c  her = try_else(l
+00013400: 616d 6264 613a 206e 6f74 2062 6f6f 6c28  ambda: not bool(
+00013410: 6861 7368 286f 7574 2929 2c20 5472 7565  hash(out)), True
+00013420: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00013430: 2020 6966 206e 6565 645f 6861 7368 6572    if need_hasher
+00013440: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013450: 2020 2020 2020 7261 6973 6520 436f 6261        raise Coba
+00013460: 4578 6365 7074 696f 6e28 2252 6573 756c  Exception("Resul
+00013470: 7420 7265 7175 6972 6573 2061 6c6c 2064  t requires all d
+00013480: 6174 6120 746f 2062 6520 6861 7368 6162  ata to be hashab
+00013490: 6c65 2e22 290a 0a20 2020 2020 2020 2020  le.")..         
+000134a0: 2020 2069 6620 4e20 3d3d 2030 3a0a 2020     if N == 0:.  
+000134b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000134c0: 2079 2069 7320 4e6f 6e65 3a0a 2020 2020   y is None:.    
+000134d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134e0: 7620 3d20 4e6f 6e65 0a20 2020 2020 2020  v = None.       
+000134f0: 2020 2020 2020 2020 2065 6c69 6620 6675           elif fu
+00013500: 6e63 203d 3d20 276c 6173 7427 3a0a 2020  nc == 'last':.  
+00013510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013520: 2020 7620 3d20 595b 2d31 5d20 6966 2073    v = Y[-1] if s
+00013530: 7061 6e20 3d3d 2031 2065 6c73 6520 6d65  pan == 1 else me
+00013540: 616e 2859 5b2d 7370 616e 3a5d 2920 6966  an(Y[-span:]) if
+00013550: 2073 7061 6e20 656c 7365 206d 6561 6e28   span else mean(
+00013560: 5929 0a20 2020 2020 2020 2020 2020 2020  Y).             
+00013570: 2020 2065 6c69 6620 6675 6e63 203d 3d20     elif func == 
+00013580: 276c 6973 7427 3a0a 2020 2020 2020 2020  'list':.        
+00013590: 2020 2020 2020 2020 2020 2020 7620 3d20              v = 
+000135a0: 590a 2020 2020 2020 2020 2020 2020 2020  Y.              
+000135b0: 2020 6966 2063 6172 6420 3d3d 2027 4727    if card == 'G'
+000135c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000135d0: 2020 2020 2020 445b 6f75 7473 5d2e 6170        D[outs].ap
+000135e0: 7065 6e64 2876 290a 2020 2020 2020 2020  pend(v).        
+000135f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00013600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013610: 2020 445b 6f75 7473 5d20 3d20 760a 2020    D[outs] = v.  
+00013620: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00013630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013640: 6966 2079 2069 7320 4e6f 6e65 3a0a 2020  if y is None:.  
+00013650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013660: 2020 7620 3d20 7265 7065 6174 284e 6f6e    v = repeat(Non
+00013670: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00013680: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00013690: 2020 2020 2020 2020 2020 2020 2076 203d               v =
+000136a0: 206d 6f76 696e 675f 6176 6572 6167 6528   moving_average(
+000136b0: 592c 7370 616e 290a 2020 2020 2020 2020  Y,span).        
+000136c0: 2020 2020 2020 2020 6966 2063 6172 6420          if card 
+000136d0: 3d3d 2027 4727 3a0a 2020 2020 2020 2020  == 'G':.        
+000136e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000136f0: 6f2c 795f 2069 6e20 7a69 7028 6f75 7473  o,y_ in zip(outs
+00013700: 2c76 293a 0a20 2020 2020 2020 2020 2020  ,v):.           
+00013710: 2020 2020 2020 2020 2020 2020 2044 5b6f               D[o
+00013720: 5d2e 6170 7065 6e64 2879 5f29 0a20 2020  ].append(y_).   
+00013730: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00013740: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00013750: 2020 2020 2020 2044 2e75 7064 6174 6528         D.update(
+00013760: 7a69 7028 6f75 7473 2c76 2929 0a0a 2020  zip(outs,v))..  
+00013770: 2020 2020 2020 7265 7475 726e 205b 6b20        return [k 
+00013780: 2b20 2876 2c29 2066 6f72 206b 2c76 2069  + (v,) for k,v i
+00013790: 6e20 442e 6974 656d 7328 295d 0a0a 2020  n D.items()]..  
+000137a0: 2020 6465 6620 5f67 6c6f 6261 6c5f 6e28    def _global_n(
+000137b0: 7365 6c66 2c20 6e3a 2055 6e69 6f6e 5b69  self, n: Union[i
+000137c0: 6e74 2c4c 6974 6572 616c 5b27 6d69 6e27  nt,Literal['min'
+000137d0: 5d5d 293a 0a0a 2020 2020 2020 2020 656e  ]]):..        en
+000137e0: 7669 726f 6e6d 656e 7473 203d 2073 656c  vironments = sel
+000137f0: 662e 656e 7669 726f 6e6d 656e 7473 0a20  f.environments. 
+00013800: 2020 2020 2020 206c 6561 726e 6572 7320         learners 
+00013810: 2020 2020 3d20 7365 6c66 2e6c 6561 726e      = self.learn
+00013820: 6572 730a 2020 2020 2020 2020 6576 616c  ers.        eval
+00013830: 7561 746f 7273 2020 203d 2073 656c 662e  uators   = self.
+00013840: 6576 616c 7561 746f 7273 0a20 2020 2020  evaluators.     
+00013850: 2020 2069 6e74 6572 6163 7469 6f6e 7320     interactions 
+00013860: 3d20 7365 6c66 2e69 6e74 6572 6163 7469  = self.interacti
+00013870: 6f6e 730a 0a20 2020 2020 2020 2065 6e76  ons..        env
+00013880: 5f6c 656e 6774 6873 203d 205b 5d0a 2020  _lengths = [].  
+00013890: 2020 2020 2020 746f 5f64 726f 7020 2020        to_drop   
+000138a0: 2020 3d20 5b5d 0a20 2020 2020 2020 2074    = [].        t
+000138b0: 6f5f 6b65 6570 2020 2020 203d 205b 5d0a  o_keep     = [].
+000138c0: 2020 2020 2020 2020 6966 206e 203d 3d20          if n == 
+000138d0: 276d 696e 273a 0a20 2020 2020 2020 2020  'min':.         
+000138e0: 2020 2066 6f72 2065 6e76 5f69 6478 2c20     for env_idx, 
+000138f0: 656e 765f 6c65 6e20 696e 2073 656c 662e  env_len in self.
+00013900: 696e 7465 7261 6374 696f 6e73 2e67 726f  interactions.gro
+00013910: 7570 6279 2833 2c27 636f 756e 7427 293a  upby(3,'count'):
+00013920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013930: 2065 6e76 5f6c 656e 6774 6873 2e61 7070   env_lengths.app
+00013940: 656e 6428 656e 765f 6c65 6e29 0a20 2020  end(env_len).   
+00013950: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00013960: 2020 2020 2020 2066 6f72 2065 6e76 5f69         for env_i
+00013970: 6478 2c20 656e 765f 6c65 6e20 696e 2073  dx, env_len in s
+00013980: 656c 662e 696e 7465 7261 6374 696f 6e73  elf.interactions
+00013990: 2e67 726f 7570 6279 2833 2c27 636f 756e  .groupby(3,'coun
+000139a0: 7427 293a 0a20 2020 2020 2020 2020 2020  t'):.           
+000139b0: 2020 2020 2069 6620 656e 765f 6c65 6e20       if env_len 
+000139c0: 3c20 6e3a 0a20 2020 2020 2020 2020 2020  < n:.           
+000139d0: 2020 2020 2020 2020 2074 6f5f 6472 6f70           to_drop
+000139e0: 2e61 7070 656e 6428 656e 765f 6964 7829  .append(env_idx)
+000139f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013a00: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00013a10: 2020 2020 2020 2020 2020 2065 6e76 5f6c             env_l
+00013a20: 656e 6774 6873 2e61 7070 656e 6428 656e  engths.append(en
+00013a30: 765f 6c65 6e29 0a20 2020 2020 2020 2020  v_len).         
+00013a40: 2020 2020 2020 2020 2020 2074 6f5f 6b65             to_ke
+00013a50: 6570 2e61 7070 656e 6428 656e 765f 6964  ep.append(env_id
+00013a60: 7829 0a0a 2020 2020 2020 2020 6966 2074  x)..        if t
+00013a70: 6f5f 6472 6f70 3a0a 2020 2020 2020 2020  o_drop:.        
+00013a80: 2020 2020 6e5f 6472 6f70 7065 6420 3d20      n_dropped = 
+00013a90: 6c65 6e28 746f 5f64 726f 7029 0a20 2020  len(to_drop).   
+00013aa0: 2020 2020 2020 2020 2069 6e74 6572 6163           interac
+00013ab0: 7469 6f6e 7320 3d20 5461 626c 6528 5669  tions = Table(Vi
+00013ac0: 6577 2869 6e74 6572 6163 7469 6f6e 732e  ew(interactions.
+00013ad0: 5f64 6174 612c 7365 6c66 2e5f 7265 6d6f  _data,self._remo
+00013ae0: 7665 2874 6f5f 6472 6f70 2c6e 2929 2c20  ve(to_drop,n)), 
+00013af0: 696e 7465 7261 6374 696f 6e73 2e63 6f6c  interactions.col
+00013b00: 756d 6e73 2c20 696e 7465 7261 6374 696f  umns, interactio
+00013b10: 6e73 2e69 6e64 6578 6573 290a 2020 2020  ns.indexes).    
+00013b20: 2020 2020 2020 2020 6966 206e 5f64 726f          if n_dro
+00013b30: 7070 6564 3d3d 313a 2043 6f62 6143 6f6e  pped==1: CobaCon
+00013b40: 7465 7874 2e6c 6f67 6765 722e 6c6f 6728  text.logger.log(
+00013b50: 6622 5765 2072 656d 6f76 6564 207b 6e5f  f"We removed {n_
+00013b60: 6472 6f70 7065 647d 206c 6561 726e 6572  dropped} learner
+00013b70: 2065 7661 6c75 6174 696f 6e20 6265 6361   evaluation beca
+00013b80: 7573 6520 6974 2077 6173 2073 686f 7274  use it was short
+00013b90: 6572 2074 6861 6e20 7b6e 7d20 696e 7465  er than {n} inte
+00013ba0: 7261 6374 696f 6e73 2e22 290a 2020 2020  ractions.").    
+00013bb0: 2020 2020 2020 2020 6966 206e 5f64 726f          if n_dro
+00013bc0: 7070 6564 3e3d 323a 2043 6f62 6143 6f6e  pped>=2: CobaCon
+00013bd0: 7465 7874 2e6c 6f67 6765 722e 6c6f 6728  text.logger.log(
+00013be0: 6622 5765 2072 656d 6f76 6564 207b 6e5f  f"We removed {n_
+00013bf0: 6472 6f70 7065 647d 206c 6561 726e 6572  dropped} learner
+00013c00: 2065 7661 6c75 6174 696f 6e73 2062 6563   evaluations bec
+00013c10: 6175 7365 2074 6865 7920 7765 7265 2073  ause they were s
+00013c20: 686f 7274 6572 2074 6861 6e20 7b6e 7d20  horter than {n} 
+00013c30: 696e 7465 7261 6374 696f 6e73 2e22 290a  interactions.").
+00013c40: 0a20 2020 2020 2020 2065 6e76 5f6c 656e  .        env_len
+00013c50: 6774 6873 203d 2063 6f6c 6c65 6374 696f  gths = collectio
+00013c60: 6e73 2e43 6f75 6e74 6572 2865 6e76 5f6c  ns.Counter(env_l
+00013c70: 656e 6774 6873 290a 2020 2020 2020 2020  engths).        
+00013c80: 7368 6f72 7465 6e5f 746f 203d 206d 696e  shorten_to = min
+00013c90: 2865 6e76 5f6c 656e 6774 6873 2920 6966  (env_lengths) if
+00013ca0: 206e 3d3d 276d 696e 2720 616e 6420 656e   n=='min' and en
+00013cb0: 765f 6c65 6e67 7468 7320 656c 7365 206e  v_lengths else n
+00013cc0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00013cd0: 656e 765f 6c65 6e67 7468 7329 203e 2031  env_lengths) > 1
+00013ce0: 206f 7220 656e 765f 6c65 6e67 7468 732e   or env_lengths.
+00013cf0: 7661 6c75 6573 2829 2021 3d20 7b73 686f  values() != {sho
+00013d00: 7274 656e 5f74 6f7d 3a0a 2020 2020 2020  rten_to}:.      
+00013d10: 2020 2020 2020 6e5f 7368 6f72 7465 6e65        n_shortene
+00013d20: 6420 3d20 7375 6d28 7620 666f 7220 6b2c  d = sum(v for k,
+00013d30: 7620 696e 2065 6e76 5f6c 656e 6774 6873  v in env_lengths
+00013d40: 2e69 7465 6d73 2829 2069 6620 6b20 3e20  .items() if k > 
+00013d50: 7368 6f72 7465 6e5f 746f 290a 2020 2020  shorten_to).    
+00013d60: 2020 2020 2020 2020 696e 7465 7261 6374          interact
+00013d70: 696f 6e73 203d 2069 6e74 6572 6163 7469  ions = interacti
+00013d80: 6f6e 732e 7768 6572 6528 696e 6465 783d  ons.where(index=
+00013d90: 7b27 3c3d 273a 7368 6f72 7465 6e5f 746f  {'<=':shorten_to
+00013da0: 7d29 2023 2e34 0a20 2020 2020 2020 2020  }) #.4.         
+00013db0: 2020 2069 6620 6e5f 7368 6f72 7465 6e65     if n_shortene
+00013dc0: 643d 3d31 3a20 436f 6261 436f 6e74 6578  d==1: CobaContex
+00013dd0: 742e 6c6f 6767 6572 2e6c 6f67 2866 2257  t.logger.log(f"W
+00013de0: 6520 7368 6f72 7465 6e65 6420 7b6e 5f73  e shortened {n_s
+00013df0: 686f 7274 656e 6564 7d20 6c65 6172 6e65  hortened} learne
+00013e00: 7220 6576 616c 7561 7469 6f6e 2062 6563  r evaluation bec
+00013e10: 6175 7365 2069 7420 7761 7320 6c6f 6e67  ause it was long
+00013e20: 6572 2074 6861 6e20 7468 6520 7368 6f72  er than the shor
+00013e30: 7465 7374 2065 6e76 6972 6f6e 6d65 6e74  test environment
+00013e40: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+00013e50: 6966 206e 5f73 686f 7274 656e 6564 3e3d  if n_shortened>=
+00013e60: 323a 2043 6f62 6143 6f6e 7465 7874 2e6c  2: CobaContext.l
+00013e70: 6f67 6765 722e 6c6f 6728 6622 5765 2073  ogger.log(f"We s
+00013e80: 686f 7274 656e 6564 207b 6e5f 7368 6f72  hortened {n_shor
+00013e90: 7465 6e65 647d 206c 6561 726e 6572 2065  tened} learner e
+00013ea0: 7661 6c75 6174 696f 6e73 2062 6563 6175  valuations becau
+00013eb0: 7365 2074 6865 7920 7765 7265 206c 6f6e  se they were lon
+00013ec0: 6765 7220 7468 616e 2074 6865 2073 686f  ger than the sho
+00013ed0: 7274 6573 7420 656e 7669 726f 6e6d 656e  rtest environmen
+00013ee0: 742e 2229 0a0a 2020 2020 2020 2020 6b65  t.")..        ke
+00013ef0: 6570 5f65 6e76 732c 6b65 6570 5f6c 726e  ep_envs,keep_lrn
+00013f00: 732c 6b65 6570 5f76 616c 7320 3d20 6d61  s,keep_vals = ma
+00013f10: 7028 7365 742c 7a69 7028 2a74 6f5f 6b65  p(set,zip(*to_ke
+00013f20: 6570 2929 2069 6620 746f 5f6b 6565 7020  ep)) if to_keep 
+00013f30: 656c 7365 2028 5b5d 2c5b 5d2c 5b5d 290a  else ([],[],[]).
+00013f40: 0a20 2020 2020 2020 2069 6620 746f 5f64  .        if to_d
+00013f50: 726f 7020 616e 6420 6c65 6e28 6b65 6570  rop and len(keep
+00013f60: 5f65 6e76 7329 2021 3d20 6c65 6e28 656e  _envs) != len(en
+00013f70: 7669 726f 6e6d 656e 7473 293a 0a20 2020  vironments):.   
+00013f80: 2020 2020 2020 2020 2065 6e76 6972 6f6e           environ
+00013f90: 6d65 6e74 7320 3d20 656e 7669 726f 6e6d  ments = environm
+00013fa0: 656e 7473 2e77 6865 7265 2865 6e76 6972  ents.where(envir
+00013fb0: 6f6e 6d65 6e74 5f69 643d 6b65 6570 5f65  onment_id=keep_e
+00013fc0: 6e76 7329 0a0a 2020 2020 2020 2020 6966  nvs)..        if
+00013fd0: 2074 6f5f 6472 6f70 2061 6e64 206c 656e   to_drop and len
+00013fe0: 286b 6565 705f 6c72 6e73 2920 213d 206c  (keep_lrns) != l
+00013ff0: 656e 286c 6561 726e 6572 7329 3a0a 2020  en(learners):.  
+00014000: 2020 2020 2020 2020 2020 6c65 6172 6e65            learne
+00014010: 7273 203d 206c 6561 726e 6572 732e 7768  rs = learners.wh
+00014020: 6572 6528 6c65 6172 6e65 725f 6964 3d6b  ere(learner_id=k
+00014030: 6565 705f 6c72 6e73 290a 0a20 2020 2020  eep_lrns)..     
+00014040: 2020 2069 6620 746f 5f64 726f 7020 616e     if to_drop an
+00014050: 6420 6c65 6e28 6b65 6570 5f76 616c 7329  d len(keep_vals)
+00014060: 2021 3d20 6c65 6e28 6576 616c 7561 746f   != len(evaluato
+00014070: 7273 293a 0a20 2020 2020 2020 2020 2020  rs):.           
+00014080: 2065 7661 6c75 6174 6f72 7320 3d20 6576   evaluators = ev
+00014090: 616c 7561 746f 7273 2e77 6865 7265 2865  aluators.where(e
+000140a0: 7661 6c75 6174 6f72 5f69 643d 6b65 6570  valuator_id=keep
+000140b0: 5f76 616c 7329 0a0a 2020 2020 2020 2020  _vals)..        
+000140c0: 7265 7475 726e 2052 6573 756c 7428 656e  return Result(en
+000140d0: 7669 726f 6e6d 656e 7473 2c20 6c65 6172  vironments, lear
+000140e0: 6e65 7273 2c20 6576 616c 7561 746f 7273  ners, evaluators
+000140f0: 2c20 696e 7465 7261 6374 696f 6e73 2c20  , interactions, 
+00014100: 7365 6c66 2e65 7870 6572 696d 656e 7429  self.experiment)
+00014110: 0a0a 2020 2020 6465 6620 5f67 726f 7570  ..    def _group
+00014120: 5f70 2873 656c 662c 206c 3a55 6e69 6f6e  _p(self, l:Union
+00014130: 5b73 7472 2c20 5365 7175 656e 6365 5b73  [str, Sequence[s
+00014140: 7472 5d5d 2c20 703a 556e 696f 6e5b 7374  tr]], p:Union[st
+00014150: 722c 2053 6571 7565 6e63 655b 7374 725d  r, Sequence[str]
+00014160: 5d29 3a0a 0a20 2020 2020 2020 2065 6e76  ]):..        env
+00014170: 6972 6f6e 6d65 6e74 7320 3d20 7365 6c66  ironments = self
+00014180: 2e65 6e76 6972 6f6e 6d65 6e74 730a 2020  .environments.  
+00014190: 2020 2020 2020 6c65 6172 6e65 7273 2020        learners  
+000141a0: 2020 203d 2073 656c 662e 6c65 6172 6e65     = self.learne
+000141b0: 7273 0a20 2020 2020 2020 2065 7661 6c75  rs.        evalu
+000141c0: 6174 6f72 7320 2020 3d20 7365 6c66 2e65  ators   = self.e
+000141d0: 7661 6c75 6174 6f72 730a 2020 2020 2020  valuators.      
+000141e0: 2020 696e 7465 7261 6374 696f 6e73 203d    interactions =
+000141f0: 2073 656c 662e 696e 7465 7261 6374 696f   self.interactio
+00014200: 6e73 0a0a 2020 2020 2020 2020 696e 6465  ns..        inde
+00014210: 7865 7320 203d 206c 6973 7428 7365 6c66  xes  = list(self
+00014220: 2e5f 6772 6f75 7065 645f 7973 2870 2c6c  ._grouped_ys(p,l
+00014230: 2c27 656e 7669 726f 6e6d 656e 745f 6964  ,'environment_id
+00014240: 272c 276c 6561 726e 6572 5f69 6427 2c27  ','learner_id','
+00014250: 6576 616c 7561 746f 725f 6964 272c 793d  evaluator_id',y=
+00014260: 4e6f 6e65 2c63 6172 643d 2753 2729 290a  None,card='S')).
+00014270: 2020 2020 2020 2020 6e5f 6c65 7665 6c73          n_levels
+00014280: 203d 206c 656e 2873 6574 286d 6170 2869   = len(set(map(i
+00014290: 7465 6d67 6574 7465 7228 3129 2c69 6e64  temgetter(1),ind
+000142a0: 6578 6573 2929 290a 0a20 2020 2020 2020  exes)))..       
+000142b0: 2074 6f5f 6b65 6570 2c20 746f 5f72 656d   to_keep, to_rem
+000142c0: 6f76 652c 206e 5f6c 6172 6765 722c 206e  ove, n_larger, n
+000142d0: 5f73 6d61 6c6c 6572 203d 205b 5d2c 205b  _smaller = [], [
+000142e0: 5d2c 2030 2c20 300a 2020 2020 2020 2020  ], 0, 0.        
+000142f0: 666f 7220 5f2c 2067 726f 7570 2069 6e20  for _, group in 
+00014300: 6772 6f75 7062 7928 696e 6465 7865 732c  groupby(indexes,
+00014310: 6b65 793d 6974 656d 6765 7474 6572 2830  key=itemgetter(0
+00014320: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+00014330: 6772 6f75 7020 3d20 6c69 7374 2867 726f  group = list(gro
+00014340: 7570 290a 2020 2020 2020 2020 2020 2020  up).            
+00014350: 6966 206c 656e 2867 726f 7570 2920 3e20  if len(group) > 
+00014360: 6e5f 6c65 7665 6c73 3a0a 2020 2020 2020  n_levels:.      
+00014370: 2020 2020 2020 2020 2020 6e5f 6c61 7267            n_larg
+00014380: 6572 202b 3d20 310a 2020 2020 2020 2020  er += 1.        
+00014390: 2020 2020 2020 2020 746f 5f72 656d 6f76          to_remov
+000143a0: 652e 6578 7465 6e64 2867 5b32 3a35 5d20  e.extend(g[2:5] 
+000143b0: 666f 7220 6720 696e 2067 726f 7570 290a  for g in group).
+000143c0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+000143d0: 206c 656e 2867 726f 7570 2920 3c20 6e5f   len(group) < n_
+000143e0: 6c65 7665 6c73 3a0a 2020 2020 2020 2020  levels:.        
+000143f0: 2020 2020 2020 2020 6e5f 736d 616c 6c65          n_smalle
+00014400: 7220 2b3d 2031 0a20 2020 2020 2020 2020  r += 1.         
+00014410: 2020 2020 2020 2074 6f5f 7265 6d6f 7665         to_remove
+00014420: 2e65 7874 656e 6428 675b 323a 355d 2066  .extend(g[2:5] f
+00014430: 6f72 2067 2069 6e20 6772 6f75 7029 0a20  or g in group). 
+00014440: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00014450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014460: 2074 6f5f 6b65 6570 2e65 7874 656e 6428   to_keep.extend(
+00014470: 675b 323a 355d 2066 6f72 2067 2069 6e20  g[2:5] for g in 
+00014480: 6772 6f75 7029 0a0a 2020 2020 2020 2020  group)..        
+00014490: 6966 206e 5f6c 6172 6765 723a 0a20 2020  if n_larger:.   
+000144a0: 2020 2020 2020 2020 2043 6f62 6143 6f6e           CobaCon
+000144b0: 7465 7874 2e6c 6f67 6765 722e 6c6f 6728  text.logger.log(
+000144c0: 6622 5765 2072 656d 6f76 6564 207b 6e5f  f"We removed {n_
+000144d0: 6c61 7267 6572 7d20 7b70 7d20 6265 6361  larger} {p} beca
+000144e0: 7573 6520 6d6f 7265 2074 6861 6e20 6f6e  use more than on
+000144f0: 6520 6578 6973 7465 6420 666f 7220 6561  e existed for ea
+00014500: 6368 207b 6c7d 2e22 290a 0a20 2020 2020  ch {l}.")..     
+00014510: 2020 2069 6620 6e5f 736d 616c 6c65 723a     if n_smaller:
+00014520: 0a20 2020 2020 2020 2020 2020 2043 6f62  .            Cob
+00014530: 6143 6f6e 7465 7874 2e6c 6f67 6765 722e  aContext.logger.
+00014540: 6c6f 6728 6622 5765 2072 656d 6f76 6564  log(f"We removed
+00014550: 207b 6e5f 736d 616c 6c65 727d 207b 707d   {n_smaller} {p}
+00014560: 2062 6563 6175 7365 207b 2774 6865 7927   because {'they'
+00014570: 2069 6620 6e5f 736d 616c 6c65 723e 3120   if n_smaller>1 
+00014580: 656c 7365 2027 6974 277d 2064 6964 206e  else 'it'} did n
+00014590: 6f74 2065 7869 7374 2066 6f72 2065 7665  ot exist for eve
+000145a0: 7279 207b 6c7d 2e22 290a 0a20 2020 2020  ry {l}.")..     
+000145b0: 2020 2069 6620 746f 5f72 656d 6f76 653a     if to_remove:
+000145c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000145d0: 6563 7420 3d20 7365 6c66 2e5f 7265 6d6f  ect = self._remo
+000145e0: 7665 2874 6f5f 7265 6d6f 7665 290a 2020  ve(to_remove).  
+000145f0: 2020 2020 2020 2020 2020 696e 7465 7261            intera
+00014600: 6374 696f 6e73 203d 2054 6162 6c65 2856  ctions = Table(V
+00014610: 6965 7728 696e 7465 7261 6374 696f 6e73  iew(interactions
+00014620: 2e5f 6461 7461 2c73 656c 6563 7429 2c20  ._data,select), 
+00014630: 696e 7465 7261 6374 696f 6e73 2e63 6f6c  interactions.col
+00014640: 756d 6e73 2c20 696e 7465 7261 6374 696f  umns, interactio
+00014650: 6e73 2e69 6e64 6578 6573 290a 0a20 2020  ns.indexes)..   
+00014660: 2020 2020 2065 5f6b 6565 702c 6c5f 6b65       e_keep,l_ke
+00014670: 6570 2c76 5f6b 6565 7020 3d20 6d61 7028  ep,v_keep = map(
+00014680: 7365 742c 7a69 7028 2a74 6f5f 6b65 6570  set,zip(*to_keep
+00014690: 2929 2069 6620 746f 5f6b 6565 7020 656c  )) if to_keep el
+000146a0: 7365 2028 5b5d 2c5b 5d2c 5b5d 290a 2020  se ([],[],[]).  
+000146b0: 2020 2020 2020 6966 206c 656e 2865 5f6b        if len(e_k
+000146c0: 6565 7029 2021 3d20 6c65 6e28 656e 7669  eep) != len(envi
+000146d0: 726f 6e6d 656e 7473 293a 2065 6e76 6972  ronments): envir
+000146e0: 6f6e 6d65 6e74 7320 3d20 656e 7669 726f  onments = enviro
+000146f0: 6e6d 656e 7473 2e77 6865 7265 2865 6e76  nments.where(env
+00014700: 6972 6f6e 6d65 6e74 5f69 643d 655f 6b65  ironment_id=e_ke
+00014710: 6570 290a 2020 2020 2020 2020 6966 206c  ep).        if l
+00014720: 656e 286c 5f6b 6565 7029 2021 3d20 6c65  en(l_keep) != le
+00014730: 6e28 6c65 6172 6e65 7273 2920 2020 203a  n(learners)    :
+00014740: 206c 6561 726e 6572 7320 2020 2020 3d20   learners     = 
+00014750: 6c65 6172 6e65 7273 2020 2020 2e77 6865  learners    .whe
+00014760: 7265 286c 6561 726e 6572 5f69 6420 2020  re(learner_id   
+00014770: 203d 6c5f 6b65 6570 290a 2020 2020 2020   =l_keep).      
+00014780: 2020 6966 206c 656e 2876 5f6b 6565 7029    if len(v_keep)
+00014790: 2021 3d20 6c65 6e28 6576 616c 7561 746f   != len(evaluato
+000147a0: 7273 2920 203a 2065 7661 6c75 6174 6f72  rs)  : evaluator
+000147b0: 7320 2020 3d20 6576 616c 7561 746f 7273  s   = evaluators
+000147c0: 2020 2e77 6865 7265 2865 7661 6c75 6174    .where(evaluat
+000147d0: 6f72 5f69 6420 203d 765f 6b65 6570 290a  or_id  =v_keep).
+000147e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000147f0: 5265 7375 6c74 2865 6e76 6972 6f6e 6d65  Result(environme
+00014800: 6e74 732c 206c 6561 726e 6572 732c 2065  nts, learners, e
+00014810: 7661 6c75 6174 6f72 732c 2069 6e74 6572  valuators, inter
+00014820: 6163 7469 6f6e 732c 2073 656c 662e 6578  actions, self.ex
+00014830: 7065 7269 6d65 6e74 290a 0a20 2020 2064  periment)..    d
+00014840: 6566 205f 6669 6c74 6572 5f66 696e 2873  ef _filter_fin(s
+00014850: 656c 662c 0a20 2020 2020 2020 206e 3a20  elf,.        n: 
+00014860: 556e 696f 6e5b 696e 742c 4c69 7465 7261  Union[int,Litera
+00014870: 6c5b 276d 696e 275d 2c20 4e6f 6e65 5d2c  l['min'], None],
+00014880: 0a20 2020 2020 2020 206c 3a20 556e 696f  .        l: Unio
+00014890: 6e5b 7374 722c 2053 6571 7565 6e63 655b  n[str, Sequence[
+000148a0: 7374 725d 2c20 4e6f 6e65 5d2c 0a20 2020  str], None],.   
+000148b0: 2020 2020 2070 3a20 556e 696f 6e5b 7374       p: Union[st
+000148c0: 722c 2053 6571 7565 6e63 655b 7374 725d  r, Sequence[str]
+000148d0: 2c20 4e6f 6e65 5d29 202d 3e20 2752 6573  , None]) -> 'Res
+000148e0: 756c 7427 3a0a 2020 2020 2020 2020 2222  ult':.        ""
+000148f0: 2246 696c 7465 7220 7468 6520 7265 7375  "Filter the resu
+00014900: 6c74 7320 646f 776e 2074 6f20 6576 656e  lts down to even
+00014910: 206f 7574 636f 6d65 7320 736f 2074 6861   outcomes so tha
+00014920: 7420 706c 6f74 7465 6420 7265 7375 6c74  t plotted result
+00014930: 7320 7769 6c6c 2062 6520 6d65 616e 696e  s will be meanin
+00014940: 6766 756c 2e0a 0a20 2020 2020 2020 2041  gful...        A
+00014950: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00014960: 206e 3a20 5468 6520 6e75 6d62 6572 206f   n: The number o
+00014970: 6620 696e 7465 7261 6374 696f 6e73 2061  f interactions a
+00014980: 2073 7065 6369 6669 6320 6576 616c 7561   specific evalua
+00014990: 7469 6f6e 206d 7573 7420 6861 7665 2028  tion must have (
+000149a0: 4e6f 6e65 2069 6e64 6963 6174 6573 206e  None indicates n
+000149b0: 6f20 636f 6e73 7472 6169 6e74 292e 0a20  o constraint).. 
+000149c0: 2020 2020 2020 2020 2020 206c 3a20 5468             l: Th
+000149d0: 6520 6c65 7665 6c20 6174 2077 6869 6368  e level at which
+000149e0: 2077 6520 7769 7368 2074 6f20 636f 6d70   we wish to comp
+000149f0: 6172 6520 6576 616c 6174 696f 6e20 6f75  are evalation ou
+00014a00: 7463 6f6d 6573 2e0a 2020 2020 2020 2020  tcomes..        
+00014a10: 2020 2020 703a 2054 6865 2070 6169 7273      p: The pairs
+00014a20: 2074 6861 7420 6d75 7374 2065 7869 7374   that must exist
+00014a30: 2061 6372 6f73 7320 616c 6c20 636f 6d70   across all comp
+00014a40: 6172 6973 6f6e 206c 6576 656c 7320 696e  arison levels in
+00014a50: 206f 7264 6572 2074 6f20 6265 2069 6e63   order to be inc
+00014a60: 6c75 6465 642e 0a20 2020 2020 2020 2022  luded..        "
+00014a70: 2222 0a0a 2020 2020 2020 2020 7265 7375  ""..        resu
+00014a80: 6c74 203d 2073 656c 662e 636f 7079 2829  lt = self.copy()
+00014a90: 0a20 2020 2020 2020 2069 6620 6c20 6f72  .        if l or
+00014aa0: 2070 3a20 7265 7375 6c74 203d 2072 6573   p: result = res
+00014ab0: 756c 742e 5f67 726f 7570 5f70 286c 2c70  ult._group_p(l,p
+00014ac0: 290a 2020 2020 2020 2020 6966 206e 2020  ).        if n  
+00014ad0: 2020 203a 2072 6573 756c 7420 3d20 7265     : result = re
+00014ae0: 7375 6c74 2e5f 676c 6f62 616c 5f6e 286e  sult._global_n(n
+00014af0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00014b00: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00014b10: 205f 7265 6d6f 7665 2873 656c 662c 2069   _remove(self, i
+00014b20: 6473 3a20 5365 7175 656e 6365 5b54 7570  ds: Sequence[Tup
+00014b30: 6c65 5b69 6e74 2c69 6e74 2c69 6e74 5d5d  le[int,int,int]]
+00014b40: 2c20 6e3d 3029 202d 3e20 5365 7175 656e  , n=0) -> Sequen
+00014b50: 6365 5b69 6e74 5d3a 0a20 2020 2020 2020  ce[int]:.       
+00014b60: 2023 7468 6973 2069 7320 6d75 6368 2066   #this is much f
+00014b70: 6173 7465 7220 7468 616e 2061 6e79 2062  aster than any b
+00014b80: 7569 6c74 2069 6e20 5461 626c 6520 6d65  uilt in Table me
+00014b90: 7468 6f64 730a 2020 2020 2020 2020 2374  thods.        #t
+00014ba0: 6f20 776f 726b 2069 6e74 6572 6163 7469  o work interacti
+00014bb0: 6f6e 7320 6d75 7374 2062 6520 736f 7274  ons must be sort
+00014bc0: 6564 2062 7920 656e 765f 6964 2c6c 726e  ed by env_id,lrn
+00014bd0: 5f69 642c 7661 6c5f 6964 0a20 2020 2020  _id,val_id.     
+00014be0: 2020 206c 6f63 2020 2020 2020 2020 2020     loc          
+00014bf0: 2020 3d20 300a 2020 2020 2020 2020 7365    = 0.        se
+00014c00: 6c65 6374 2020 2020 2020 2020 203d 205b  lect         = [
+00014c10: 5d0a 2020 2020 2020 2020 6e5f 696e 7465  ].        n_inte
+00014c20: 7261 6374 696f 6e73 203d 206c 656e 2873  ractions = len(s
+00014c30: 656c 662e 696e 7465 7261 6374 696f 6e73  elf.interactions
+00014c40: 290a 2020 2020 2020 2020 656e 765f 6964  ).        env_id
+00014c50: 732c 6c72 6e5f 6964 732c 7661 6c5f 6964  s,lrn_ids,val_id
+00014c60: 7320 3d20 7365 6c66 2e69 6e74 6572 6163  s = self.interac
+00014c70: 7469 6f6e 735b 5b27 656e 7669 726f 6e6d  tions[['environm
+00014c80: 656e 745f 6964 272c 276c 6561 726e 6572  ent_id','learner
+00014c90: 5f69 6427 2c27 6576 616c 7561 746f 725f  _id','evaluator_
+00014ca0: 6964 275d 5d0a 2020 2020 2020 2020 6964  id']].        id
+00014cb0: 7320 3d20 736f 7274 6564 2869 6473 290a  s = sorted(ids).
+00014cc0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00014cd0: 2072 616e 6765 286c 656e 2869 6473 2929   range(len(ids))
+00014ce0: 3a0a 2020 2020 2020 2020 2020 2020 652c  :.            e,
+00014cf0: 6c2c 7620 3d20 6964 735b 695d 0a20 2020  l,v = ids[i].   
+00014d00: 2020 2020 2020 2020 206c 6f31 203d 206d           lo1 = m
+00014d10: 795f 6269 7365 6374 5f6c 6566 7420 2865  y_bisect_left (e
+00014d20: 6e76 5f69 6473 2c65 2c6c 6f63 2c6e 5f69  nv_ids,e,loc,n_i
+00014d30: 6e74 6572 6163 7469 6f6e 7329 0a20 2020  nteractions).   
+00014d40: 2020 2020 2020 2020 2068 6931 203d 206d           hi1 = m
+00014d50: 795f 6269 7365 6374 5f72 6967 6874 2865  y_bisect_right(e
+00014d60: 6e76 5f69 6473 2c65 2c6c 6f63 2c6e 5f69  nv_ids,e,loc,n_i
+00014d70: 6e74 6572 6163 7469 6f6e 7329 0a20 2020  nteractions).   
+00014d80: 2020 2020 2020 2020 2069 6620 6c6f 313d           if lo1=
+00014d90: 3d68 6931 3a20 636f 6e74 696e 7565 2023  =hi1: continue #
+00014da0: 7468 6520 6769 7665 6e20 6964 7320 6172  the given ids ar
+00014db0: 656e 2774 2069 6e20 696e 7465 7261 6374  en't in interact
+00014dc0: 696f 6e73 0a20 2020 2020 2020 2020 2020  ions.           
+00014dd0: 206c 6f32 203d 206d 795f 6269 7365 6374   lo2 = my_bisect
+00014de0: 5f6c 6566 7420 286c 726e 5f69 6473 2c6c  _left (lrn_ids,l
+00014df0: 2c6c 6f31 2c68 6931 290a 2020 2020 2020  ,lo1,hi1).      
+00014e00: 2020 2020 2020 6869 3220 3d20 6d79 5f62        hi2 = my_b
+00014e10: 6973 6563 745f 7269 6768 7428 6c72 6e5f  isect_right(lrn_
+00014e20: 6964 732c 6c2c 6c6f 312c 6869 3129 0a20  ids,l,lo1,hi1). 
+00014e30: 2020 2020 2020 2020 2020 2069 6620 6c6f             if lo
+00014e40: 323d 3d68 6932 3a20 636f 6e74 696e 7565  2==hi2: continue
+00014e50: 0a20 2020 2020 2020 2020 2020 206c 6f33  .            lo3
+00014e60: 203d 206d 795f 6269 7365 6374 5f6c 6566   = my_bisect_lef
+00014e70: 7420 2876 616c 5f69 6473 2c76 2c6c 6f32  t (val_ids,v,lo2
+00014e80: 2c68 6932 290a 2020 2020 2020 2020 2020  ,hi2).          
+00014e90: 2020 6869 3320 3d20 6d79 5f62 6973 6563    hi3 = my_bisec
+00014ea0: 745f 7269 6768 7428 7661 6c5f 6964 732c  t_right(val_ids,
+00014eb0: 762c 6c6f 322c 6869 3229 0a20 2020 2020  v,lo2,hi2).     
+00014ec0: 2020 2020 2020 2069 6620 6c6f 333d 3d68         if lo3==h
+00014ed0: 6933 3a20 636f 6e74 696e 7565 0a20 2020  i3: continue.   
+00014ee0: 2020 2020 2020 2020 2073 656c 6563 742e           select.
+00014ef0: 6578 7465 6e64 2872 616e 6765 286c 6f63  extend(range(loc
+00014f00: 2c6c 6f33 2b28 6e20 6966 2068 6933 2d6c  ,lo3+(n if hi3-l
+00014f10: 6f33 3e6e 2065 6c73 6520 3029 2929 0a20  o3>n else 0))). 
+00014f20: 2020 2020 2020 2020 2020 206c 6f63 203d             loc =
+00014f30: 2068 6933 0a0a 2020 2020 2020 2020 7365   hi3..        se
+00014f40: 6c65 6374 2e65 7874 656e 6428 7261 6e67  lect.extend(rang
+00014f50: 6528 6c6f 632c 6e5f 696e 7465 7261 6374  e(loc,n_interact
+00014f60: 696f 6e73 2929 0a20 2020 2020 2020 2072  ions)).        r
+00014f70: 6574 7572 6e20 7365 6c65 6374 0a         eturn select.
```

### Comparing `coba-8.0.3/coba/results/errors.py` & `coba-8.0.4/coba/results/errors.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/safety.py` & `coba-8.0.4/coba/safety.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/statistics.py` & `coba-8.0.4/coba/statistics.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/coba/utilities.py` & `coba-8.0.4/coba/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import warnings
 import importlib.util
 
 from math import isfinite
 from itertools import chain, islice, groupby
 from collections import defaultdict
-from typing import TypeVar, Iterable, Tuple, Union, Sequence, Any, Callable, Hashable, Mapping
+from typing import TypeVar, Iterable, Tuple, Union, Sequence, Any, Callable, Hashable
 
 from coba.exceptions import CobaExit
 
 def coba_exit(message:str):
     #we ignore warnings before exiting in order to make jupyter's output a little cleaner
     warnings.filterwarnings("ignore",message="To exit: use 'exit', 'quit', or Ctrl-D.")
     raise CobaExit(message) from None
```

### Comparing `coba-8.0.3/coba.egg-info/PKG-INFO` & `coba-8.0.4/coba.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coba
-Version: 8.0.3
+Version: 8.0.4
 Summary: A contextual bandit research package
 Author-email: Mark Rucker <rucker.mark@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://coba-docs.readthedocs.io/
 Project-URL: Documentation, https://coba-docs.readthedocs.io/
 Project-URL: Repository, https://github.com/vowpalwabbit/coba
 Classifier: Intended Audience :: Science/Research
@@ -23,16 +23,16 @@
 Requires-Dist: numpy; extra == "full"
 Requires-Dist: scipy; extra == "full"
 Requires-Dist: cloudpickle; extra == "full"
 Requires-Dist: torch; extra == "full"
 
 [![codecov](https://codecov.io/gh/VowpalWabbit/coba/branch/master/graph/badge.svg?token=885XLZJ2D4)](https://codecov.io/gh/VowpalWabbit/coba)
 [![binder](https://img.shields.io/badge/launch%20example-binder-579ACA.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAB8lBMVEX///9XmsrmZYH1olJXmsr1olJXmsrmZYH1olJXmsr1olJXmsrmZYH1olL1olJXmsr1olJXmsrmZYH1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olJXmsrmZYH1olL1olL0nFf1olJXmsrmZYH1olJXmsq8dZb1olJXmsrmZYH1olJXmspXmspXmsr1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olLeaIVXmsrmZYH1olL1olL1olJXmsrmZYH1olLna31Xmsr1olJXmsr1olJXmsrmZYH1olLqoVr1olJXmsr1olJXmsrmZYH1olL1olKkfaPobXvviGabgadXmsqThKuofKHmZ4Dobnr1olJXmsr1olJXmspXmsr1olJXmsrfZ4TuhWn1olL1olJXmsqBi7X1olJXmspZmslbmMhbmsdemsVfl8ZgmsNim8Jpk8F0m7R4m7F5nLB6jbh7jbiDirOEibOGnKaMhq+PnaCVg6qWg6qegKaff6WhnpKofKGtnomxeZy3noG6dZi+n3vCcpPDcpPGn3bLb4/Mb47UbIrVa4rYoGjdaIbeaIXhoWHmZYHobXvpcHjqdHXreHLroVrsfG/uhGnuh2bwj2Hxk17yl1vzmljzm1j0nlX1olL3AJXWAAAAbXRSTlMAEBAQHx8gICAuLjAwMDw9PUBAQEpQUFBXV1hgYGBkcHBwcXl8gICAgoiIkJCQlJicnJ2goKCmqK+wsLC4usDAwMjP0NDQ1NbW3Nzg4ODi5+3v8PDw8/T09PX29vb39/f5+fr7+/z8/Pz9/v7+zczCxgAABC5JREFUeAHN1ul3k0UUBvCb1CTVpmpaitAGSLSpSuKCLWpbTKNJFGlcSMAFF63iUmRccNG6gLbuxkXU66JAUef/9LSpmXnyLr3T5AO/rzl5zj137p136BISy44fKJXuGN/d19PUfYeO67Znqtf2KH33Id1psXoFdW30sPZ1sMvs2D060AHqws4FHeJojLZqnw53cmfvg+XR8mC0OEjuxrXEkX5ydeVJLVIlV0e10PXk5k7dYeHu7Cj1j+49uKg7uLU61tGLw1lq27ugQYlclHC4bgv7VQ+TAyj5Zc/UjsPvs1sd5cWryWObtvWT2EPa4rtnWW3JkpjggEpbOsPr7F7EyNewtpBIslA7p43HCsnwooXTEc3UmPmCNn5lrqTJxy6nRmcavGZVt/3Da2pD5NHvsOHJCrdc1G2r3DITpU7yic7w/7Rxnjc0kt5GC4djiv2Sz3Fb2iEZg41/ddsFDoyuYrIkmFehz0HR2thPgQqMyQYb2OtB0WxsZ3BeG3+wpRb1vzl2UYBog8FfGhttFKjtAclnZYrRo9ryG9uG/FZQU4AEg8ZE9LjGMzTmqKXPLnlWVnIlQQTvxJf8ip7VgjZjyVPrjw1te5otM7RmP7xm+sK2Gv9I8Gi++BRbEkR9EBw8zRUcKxwp73xkaLiqQb+kGduJTNHG72zcW9LoJgqQxpP3/Tj//c3yB0tqzaml05/+orHLksVO+95kX7/7qgJvnjlrfr2Ggsyx0eoy9uPzN5SPd86aXggOsEKW2Prz7du3VID3/tzs/sSRs2w7ovVHKtjrX2pd7ZMlTxAYfBAL9jiDwfLkq55Tm7ifhMlTGPyCAs7RFRhn47JnlcB9RM5T97ASuZXIcVNuUDIndpDbdsfrqsOppeXl5Y+XVKdjFCTh+zGaVuj0d9zy05PPK3QzBamxdwtTCrzyg/2Rvf2EstUjordGwa/kx9mSJLr8mLLtCW8HHGJc2R5hS219IiF6PnTusOqcMl57gm0Z8kanKMAQg0qSyuZfn7zItsbGyO9QlnxY0eCuD1XL2ys/MsrQhltE7Ug0uFOzufJFE2PxBo/YAx8XPPdDwWN0MrDRYIZF0mSMKCNHgaIVFoBbNoLJ7tEQDKxGF0kcLQimojCZopv0OkNOyWCCg9XMVAi7ARJzQdM2QUh0gmBozjc3Skg6dSBRqDGYSUOu66Zg+I2fNZs/M3/f/Grl/XnyF1Gw3VKCez0PN5IUfFLqvgUN4C0qNqYs5YhPL+aVZYDE4IpUk57oSFnJm4FyCqqOE0jhY2SMyLFoo56zyo6becOS5UVDdj7Vih0zp+tcMhwRpBeLyqtIjlJKAIZSbI8SGSF3k0pA3mR5tHuwPFoa7N7reoq2bqCsAk1HqCu5uvI1n6JuRXI+S1Mco54YmYTwcn6Aeic+kssXi8XpXC4V3t7/ADuTNKaQJdScAAAAAElFTkSuQmCC)](https://mybinder.org/v2/gh/VowpalWabbit/Coba/HEAD?filepath=doc/source/notebooks)
-[![doc](https://readthedocs.org/projects/coba-docs/badge/?version=latest)](https://coba-docs.readthedocs.io/en/latest/?badge=latest)
-[![pypi](https://img.shields.io/badge/pypi-v8.0.2-blue)](https://pypi.org/project/coba/)
+[![doc](https://readthedocs.org/projects/coba-docs/badge/?version=latest)](https://coba-docs.readthedocs.io/?badge=v8.0.3)
+[![pypi](https://img.shields.io/badge/pypi-v8.0.3-blue)](https://pypi.org/project/coba/)
 
 # Coba
 
  ### What is it?
 
  Coba is a powerful framework built to facilitate research with online contextual bandit (CB) algorithms.
```

### Comparing `coba-8.0.3/coba.egg-info/SOURCES.txt` & `coba-8.0.4/coba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coba-8.0.3/pyproject.toml` & `coba-8.0.4/pyproject.toml`

 * *Files identical despite different names*

