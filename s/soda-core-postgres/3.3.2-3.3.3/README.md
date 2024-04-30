# Comparing `tmp/soda_core_postgres-3.3.2.tar.gz` & `tmp/soda_core_postgres-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_core_postgres-3.3.2.tar", last modified: Wed Apr 24 15:26:26 2024, max compression
+gzip compressed data, was "soda_core_postgres-3.3.3.tar", last modified: Tue Apr 30 11:50:56 2024, max compression
```

## Comparing `soda_core_postgres-3.3.2.tar` & `soda_core_postgres-3.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:26.747805 soda_core_postgres-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 15:25:40.000000 soda_core_postgres-3.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 15:26:26.747805 soda_core_postgres-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:26:26.751805 soda_core_postgres-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-24 15:25:40.000000 soda_core_postgres-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:26.747805 soda_core_postgres-3.3.2/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:26.747805 soda_core_postgres-3.3.2/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-04-24 15:25:40.000000 soda_core_postgres-3.3.2/soda/data_sources/postgres_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:26.747805 soda_core_postgres-3.3.2/soda_core_postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 15:26:26.000000 soda_core_postgres-3.3.2/soda_core_postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-24 15:26:26.000000 soda_core_postgres-3.3.2/soda_core_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:26:26.000000 soda_core_postgres-3.3.2/soda_core_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 15:26:26.000000 soda_core_postgres-3.3.2/soda_core_postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:26:26.000000 soda_core_postgres-3.3.2/soda_core_postgres.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:26.747805 soda_core_postgres-3.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-24 15:25:40.000000 soda_core_postgres-3.3.2/tests/test_postgres_connection_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-24 15:25:40.000000 soda_core_postgres-3.3.2/tests/test_postgres_specific_stuff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:56.165087 soda_core_postgres-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 11:50:11.000000 soda_core_postgres-3.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 11:50:56.165087 soda_core_postgres-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 11:50:56.165087 soda_core_postgres-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-30 11:50:11.000000 soda_core_postgres-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:56.161087 soda_core_postgres-3.3.3/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:56.161087 soda_core_postgres-3.3.3/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-04-30 11:50:11.000000 soda_core_postgres-3.3.3/soda/data_sources/postgres_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:56.165087 soda_core_postgres-3.3.3/soda_core_postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 11:50:56.000000 soda_core_postgres-3.3.3/soda_core_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-30 11:50:56.000000 soda_core_postgres-3.3.3/soda_core_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 11:50:56.000000 soda_core_postgres-3.3.3/soda_core_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-30 11:50:56.000000 soda_core_postgres-3.3.3/soda_core_postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 11:50:56.000000 soda_core_postgres-3.3.3/soda_core_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:56.165087 soda_core_postgres-3.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-30 11:50:11.000000 soda_core_postgres-3.3.3/tests/test_postgres_connection_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-30 11:50:11.000000 soda_core_postgres-3.3.3/tests/test_postgres_specific_stuff.py
```

### Comparing `soda_core_postgres-3.3.2/LICENSE` & `soda_core_postgres-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_core_postgres-3.3.2/soda/data_sources/postgres_data_source.py` & `soda_core_postgres-3.3.3/soda/data_sources/postgres_data_source.py`

 * *Files identical despite different names*

### Comparing `soda_core_postgres-3.3.2/tests/test_postgres_connection_validation.py` & `soda_core_postgres-3.3.3/tests/test_postgres_connection_validation.py`

 * *Files identical despite different names*

### Comparing `soda_core_postgres-3.3.2/tests/test_postgres_specific_stuff.py` & `soda_core_postgres-3.3.3/tests/test_postgres_specific_stuff.py`

 * *Files identical despite different names*

