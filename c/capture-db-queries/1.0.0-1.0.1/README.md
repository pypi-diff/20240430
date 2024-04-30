# Comparing `tmp/capture_db_queries-1.0.0.tar.gz` & `tmp/capture_db_queries-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capture_db_queries-1.0.0.tar", last modified: Sun Apr 21 18:21:48 2024, max compression
+gzip compressed data, was "capture_db_queries-1.0.1.tar", last modified: Tue Apr 30 13:44:28 2024, max compression
```

## Comparing `capture_db_queries-1.0.0.tar` & `capture_db_queries-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 18:21:48.033347 capture_db_queries-1.0.0/
--rw-rw-rw-   0        0        0     1085 2024-04-16 14:24:28.000000 capture_db_queries-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       89 2024-04-16 20:59:30.000000 capture_db_queries-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3233 2024-04-21 18:21:48.033347 capture_db_queries-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1815 2024-04-16 21:57:12.000000 capture_db_queries-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 18:21:48.023345 capture_db_queries-1.0.0/capture_db_queries/
--rw-rw-rw-   0        0        0        0 2024-04-16 21:11:45.000000 capture_db_queries-1.0.0/capture_db_queries/__init__.py
--rw-rw-rw-   0        0        0     7141 2024-04-16 21:42:43.000000 capture_db_queries-1.0.0/capture_db_queries/decorators.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:21:48.031344 capture_db_queries-1.0.0/capture_db_queries.egg-info/
--rw-rw-rw-   0        0        0     3233 2024-04-21 18:21:47.000000 capture_db_queries-1.0.0/capture_db_queries.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2024-04-21 18:21:47.000000 capture_db_queries-1.0.0/capture_db_queries.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 18:21:47.000000 capture_db_queries-1.0.0/capture_db_queries.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-21 18:21:47.000000 capture_db_queries-1.0.0/capture_db_queries.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-21 18:21:47.000000 capture_db_queries-1.0.0/capture_db_queries.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 18:21:48.034345 capture_db_queries-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1389 2024-04-17 08:18:05.000000 capture_db_queries-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:28.624721 capture_db_queries-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:28.620721 capture_db_queries-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:28.620721 capture_db_queries-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-30 13:44:28.624721 capture_db_queries-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:44:28.624721 capture_db_queries-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:28.620721 capture_db_queries-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:28.620721 capture_db_queries-1.0.1/src/capture_db_queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/src/capture_db_queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/src/capture_db_queries/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/src/capture_db_queries/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:28.624721 capture_db_queries-1.0.1/src/capture_db_queries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-30 13:44:28.000000 capture_db_queries-1.0.1/src/capture_db_queries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-30 13:44:28.000000 capture_db_queries-1.0.1/src/capture_db_queries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:44:28.000000 capture_db_queries-1.0.1/src/capture_db_queries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-30 13:44:28.000000 capture_db_queries-1.0.1/src/capture_db_queries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-30 13:44:28.000000 capture_db_queries-1.0.1/src/capture_db_queries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 13:44:28.000000 capture_db_queries-1.0.1/src/capture_db_queries.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:28.624721 capture_db_queries-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/tests/test_decorators.py
```

