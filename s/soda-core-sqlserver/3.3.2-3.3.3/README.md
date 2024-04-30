# Comparing `tmp/soda_core_sqlserver-3.3.2.tar.gz` & `tmp/soda_core_sqlserver-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_core_sqlserver-3.3.2.tar", last modified: Wed Apr 24 15:26:46 2024, max compression
+gzip compressed data, was "soda_core_sqlserver-3.3.3.tar", last modified: Tue Apr 30 11:51:17 2024, max compression
```

## Comparing `soda_core_sqlserver-3.3.2.tar` & `soda_core_sqlserver-3.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:46.431885 soda_core_sqlserver-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 15:25:40.000000 soda_core_sqlserver-3.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 15:26:46.431885 soda_core_sqlserver-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:26:46.431885 soda_core_sqlserver-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-24 15:25:40.000000 soda_core_sqlserver-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:46.431885 soda_core_sqlserver-3.3.2/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:46.431885 soda_core_sqlserver-3.3.2/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)    17504 2024-04-24 15:25:40.000000 soda_core_sqlserver-3.3.2/soda/data_sources/sqlserver_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:46.431885 soda_core_sqlserver-3.3.2/soda_core_sqlserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 15:26:46.000000 soda_core_sqlserver-3.3.2/soda_core_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-24 15:26:46.000000 soda_core_sqlserver-3.3.2/soda_core_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:26:46.000000 soda_core_sqlserver-3.3.2/soda_core_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 15:26:46.000000 soda_core_sqlserver-3.3.2/soda_core_sqlserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:26:46.000000 soda_core_sqlserver-3.3.2/soda_core_sqlserver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:46.431885 soda_core_sqlserver-3.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-24 15:25:40.000000 soda_core_sqlserver-3.3.2/tests/test_sqlserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:51:17.609236 soda_core_sqlserver-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 11:50:11.000000 soda_core_sqlserver-3.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-30 11:51:17.609236 soda_core_sqlserver-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 11:51:17.609236 soda_core_sqlserver-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-30 11:50:11.000000 soda_core_sqlserver-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:51:17.605236 soda_core_sqlserver-3.3.3/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:51:17.605236 soda_core_sqlserver-3.3.3/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)    17504 2024-04-30 11:50:11.000000 soda_core_sqlserver-3.3.3/soda/data_sources/sqlserver_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:51:17.609236 soda_core_sqlserver-3.3.3/soda_core_sqlserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-30 11:51:17.000000 soda_core_sqlserver-3.3.3/soda_core_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-30 11:51:17.000000 soda_core_sqlserver-3.3.3/soda_core_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 11:51:17.000000 soda_core_sqlserver-3.3.3/soda_core_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 11:51:17.000000 soda_core_sqlserver-3.3.3/soda_core_sqlserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 11:51:17.000000 soda_core_sqlserver-3.3.3/soda_core_sqlserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:51:17.609236 soda_core_sqlserver-3.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-30 11:50:11.000000 soda_core_sqlserver-3.3.3/tests/test_sqlserver.py
```

### Comparing `soda_core_sqlserver-3.3.2/LICENSE` & `soda_core_sqlserver-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_core_sqlserver-3.3.2/soda/data_sources/sqlserver_data_source.py` & `soda_core_sqlserver-3.3.3/soda/data_sources/sqlserver_data_source.py`

 * *Files identical despite different names*

