# Comparing `tmp/soda_core_spark_df-3.3.2.tar.gz` & `tmp/soda_core_spark_df-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_core_spark_df-3.3.2.tar", last modified: Wed Apr 24 15:26:42 2024, max compression
+gzip compressed data, was "soda_core_spark_df-3.3.3.tar", last modified: Tue Apr 30 11:51:14 2024, max compression
```

## Comparing `soda_core_spark_df-3.3.2.tar` & `soda_core_spark_df-3.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:42.415869 soda_core_spark_df-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 15:25:40.000000 soda_core_spark_df-3.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-24 15:26:42.415869 soda_core_spark_df-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:26:42.415869 soda_core_spark_df-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-24 15:25:40.000000 soda_core_spark_df-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:42.411869 soda_core_spark_df-3.3.2/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:42.415869 soda_core_spark_df-3.3.2/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-24 15:25:40.000000 soda_core_spark_df-3.3.2/soda/data_sources/spark_df_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-24 15:25:40.000000 soda_core_spark_df-3.3.2/soda/data_sources/spark_df_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 15:25:40.000000 soda_core_spark_df-3.3.2/soda/data_sources/spark_df_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:42.415869 soda_core_spark_df-3.3.2/soda_core_spark_df.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-24 15:26:42.000000 soda_core_spark_df-3.3.2/soda_core_spark_df.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-24 15:26:42.000000 soda_core_spark_df-3.3.2/soda_core_spark_df.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:26:42.000000 soda_core_spark_df-3.3.2/soda_core_spark_df.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 15:26:42.000000 soda_core_spark_df-3.3.2/soda_core_spark_df.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:26:42.000000 soda_core_spark_df-3.3.2/soda_core_spark_df.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:42.415869 soda_core_spark_df-3.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-24 15:25:40.000000 soda_core_spark_df-3.3.2/tests/test_spark_df.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:51:14.737214 soda_core_spark_df-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 11:50:11.000000 soda_core_spark_df-3.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-30 11:51:14.737214 soda_core_spark_df-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 11:51:14.737214 soda_core_spark_df-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-30 11:50:11.000000 soda_core_spark_df-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:51:14.733214 soda_core_spark_df-3.3.3/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:51:14.733214 soda_core_spark_df-3.3.3/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-30 11:50:11.000000 soda_core_spark_df-3.3.3/soda/data_sources/spark_df_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-30 11:50:11.000000 soda_core_spark_df-3.3.3/soda/data_sources/spark_df_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-30 11:50:11.000000 soda_core_spark_df-3.3.3/soda/data_sources/spark_df_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:51:14.737214 soda_core_spark_df-3.3.3/soda_core_spark_df.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-30 11:51:14.000000 soda_core_spark_df-3.3.3/soda_core_spark_df.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-30 11:51:14.000000 soda_core_spark_df-3.3.3/soda_core_spark_df.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 11:51:14.000000 soda_core_spark_df-3.3.3/soda_core_spark_df.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-30 11:51:14.000000 soda_core_spark_df-3.3.3/soda_core_spark_df.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 11:51:14.000000 soda_core_spark_df-3.3.3/soda_core_spark_df.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:51:14.737214 soda_core_spark_df-3.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-30 11:50:11.000000 soda_core_spark_df-3.3.3/tests/test_spark_df.py
```

### Comparing `soda_core_spark_df-3.3.2/LICENSE` & `soda_core_spark_df-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_core_spark_df-3.3.2/soda/data_sources/spark_df_cursor.py` & `soda_core_spark_df-3.3.3/soda/data_sources/spark_df_cursor.py`

 * *Files identical despite different names*

### Comparing `soda_core_spark_df-3.3.2/soda/data_sources/spark_df_data_source.py` & `soda_core_spark_df-3.3.3/soda/data_sources/spark_df_data_source.py`

 * *Files identical despite different names*

### Comparing `soda_core_spark_df-3.3.2/tests/test_spark_df.py` & `soda_core_spark_df-3.3.3/tests/test_spark_df.py`

 * *Files identical despite different names*

