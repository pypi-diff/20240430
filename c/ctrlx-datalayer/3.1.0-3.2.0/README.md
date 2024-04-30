# Comparing `tmp/ctrlx-datalayer-3.1.0.tar.gz` & `tmp/ctrlx_datalayer-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrlx-datalayer-3.1.0.tar", last modified: Thu Jan 25 09:16:05 2024, max compression
+gzip compressed data, was "ctrlx_datalayer-3.2.0.tar", last modified: Tue Apr 30 12:51:37 2024, max compression
```

## Comparing `ctrlx-datalayer-3.1.0.tar` & `ctrlx_datalayer-3.2.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 boschrexroth  (1001) boschrexroth  (1001)        0 2024-01-25 09:16:05.858364 ctrlx-datalayer-3.1.0/
-drwxrwxr-x   0 boschrexroth  (1001) boschrexroth  (1001)        0 2024-01-25 09:16:05.834364 ctrlx-datalayer-3.1.0/LICENSES/
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     1068 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/LICENSES/MIT.txt
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    45758 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/LICENSES/boschrexroth_tac_delivery.txt
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)   153265 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/LICENSES/tc_for_provision_of_products_free_of_charge.pdf
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)       46 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/MANIFEST.in
--rw-r--r--   0 boschrexroth  (1001) boschrexroth  (1001)     1934 2024-01-25 09:16:05.858364 ctrlx-datalayer-3.1.0/PKG-INFO
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     1222 2024-01-25 09:12:47.000000 ctrlx-datalayer-3.1.0/README.md
-drwxrwxr-x   0 boschrexroth  (1001) boschrexroth  (1001)        0 2024-01-25 09:16:05.858364 ctrlx-datalayer-3.1.0/ctrlx_datalayer.egg-info/
--rw-r--r--   0 boschrexroth  (1001) boschrexroth  (1001)     1934 2024-01-25 09:16:05.000000 ctrlx-datalayer-3.1.0/ctrlx_datalayer.egg-info/PKG-INFO
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     1686 2024-01-25 09:16:05.000000 ctrlx-datalayer-3.1.0/ctrlx_datalayer.egg-info/SOURCES.txt
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)        1 2024-01-25 09:16:05.000000 ctrlx-datalayer-3.1.0/ctrlx_datalayer.egg-info/dependency_links.txt
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)       38 2024-01-25 09:16:05.000000 ctrlx-datalayer-3.1.0/ctrlx_datalayer.egg-info/requires.txt
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)       15 2024-01-25 09:16:05.000000 ctrlx-datalayer-3.1.0/ctrlx_datalayer.egg-info/top_level.txt
-drwxrwxr-x   0 boschrexroth  (1001) boschrexroth  (1001)        0 2024-01-25 09:16:05.850364 ctrlx-datalayer-3.1.0/ctrlxdatalayer/
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)      422 2023-12-01 15:34:49.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/__init__.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)       47 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/_version.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    31023 2023-11-07 10:57:55.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/bulk.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     6509 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/bulk_util.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)      532 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     9016 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_bulk.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    12645 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_client.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     2504 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_converter.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)      956 2023-11-07 10:57:51.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_factory.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     3601 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_provider.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     3251 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_provider_node.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     1970 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_system.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    16886 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_variant.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    22388 2023-11-07 10:57:55.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/client.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     4604 2023-11-07 10:57:55.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/converter.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     1362 2023-11-07 10:57:51.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/factory.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     9421 2023-12-01 15:13:33.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/metadata_utils.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     5215 2023-11-07 10:57:51.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/provider.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     6288 2023-11-07 10:57:55.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/provider_node.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     4906 2023-11-07 10:57:55.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/subscription.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    10479 2023-11-07 10:57:55.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/subscription_async.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     6426 2023-11-07 10:57:55.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/subscription_sync.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     2978 2023-11-07 10:57:55.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/system.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    31125 2023-11-07 10:57:55.000000 ctrlx-datalayer-3.1.0/ctrlxdatalayer/variant.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)      736 2024-01-25 09:12:47.000000 ctrlx-datalayer-3.1.0/pyproject.toml
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)       38 2024-01-25 09:16:05.858364 ctrlx-datalayer-3.1.0/setup.cfg
-drwxrwxr-x   0 boschrexroth  (1001) boschrexroth  (1001)        0 2024-01-25 09:16:05.858364 ctrlx-datalayer-3.1.0/tests/
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    26071 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_bulk.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    11814 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_bulk_async.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    20246 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_client.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     6750 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_converter.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     1193 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_fbs.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     4999 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_integration_bulk.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     6264 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_integration_bulk_async.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    14848 2023-11-07 10:57:55.000000 ctrlx-datalayer-3.1.0/tests/test_integration_client.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     5333 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_integration_converter.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     3926 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_integration_provider.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    16958 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_integration_sub_async.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    12806 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_integration_sub_sync.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    12514 2023-12-01 15:13:33.000000 ctrlx-datalayer-3.1.0/tests/test_metadata_utils.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     2704 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_node.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     9470 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_provider.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     9611 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_provider_node.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    20938 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_subscription_async.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    22177 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_subscription_sync.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     7125 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_system.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     1240 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_utils.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    13224 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_variant.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    15117 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_variant_array.py
--rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    19050 2023-10-16 06:56:32.000000 ctrlx-datalayer-3.1.0/tests/test_variant_functions.py
+drwxrwxr-x   0 boschrexroth  (1001) boschrexroth  (1001)        0 2024-04-30 12:51:37.399273 ctrlx_datalayer-3.2.0/
+drwxrwxr-x   0 boschrexroth  (1001) boschrexroth  (1001)        0 2024-04-30 12:51:37.395273 ctrlx_datalayer-3.2.0/LICENSES/
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     1068 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/LICENSES/MIT.txt
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    45758 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/LICENSES/boschrexroth_tac_delivery.txt
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)   153265 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/LICENSES/tc_for_provision_of_products_free_of_charge.pdf
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)       46 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/MANIFEST.in
+-rw-r--r--   0 boschrexroth  (1001) boschrexroth  (1001)     1934 2024-04-30 12:51:37.399273 ctrlx_datalayer-3.2.0/PKG-INFO
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     1222 2024-04-30 12:39:09.000000 ctrlx_datalayer-3.2.0/README.md
+drwxrwxr-x   0 boschrexroth  (1001) boschrexroth  (1001)        0 2024-04-30 12:51:37.399273 ctrlx_datalayer-3.2.0/ctrlx_datalayer.egg-info/
+-rw-r--r--   0 boschrexroth  (1001) boschrexroth  (1001)     1934 2024-04-30 12:51:37.000000 ctrlx_datalayer-3.2.0/ctrlx_datalayer.egg-info/PKG-INFO
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     1686 2024-04-30 12:51:37.000000 ctrlx_datalayer-3.2.0/ctrlx_datalayer.egg-info/SOURCES.txt
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)        1 2024-04-30 12:51:37.000000 ctrlx_datalayer-3.2.0/ctrlx_datalayer.egg-info/dependency_links.txt
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)       38 2024-04-30 12:51:37.000000 ctrlx_datalayer-3.2.0/ctrlx_datalayer.egg-info/requires.txt
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)       15 2024-04-30 12:51:37.000000 ctrlx_datalayer-3.2.0/ctrlx_datalayer.egg-info/top_level.txt
+drwxrwxr-x   0 boschrexroth  (1001) boschrexroth  (1001)        0 2024-04-30 12:51:37.399273 ctrlx_datalayer-3.2.0/ctrlxdatalayer/
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)      422 2023-12-01 15:34:49.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/__init__.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)       47 2024-04-30 12:48:45.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/_version.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    31023 2023-11-07 10:57:55.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/bulk.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     6509 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/bulk_util.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)      532 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     9016 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_bulk.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    12645 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_client.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     2504 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_converter.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)      956 2023-11-07 10:57:51.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_factory.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     3601 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_provider.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     3251 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_provider_node.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     1970 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_system.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    16886 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_variant.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    22388 2023-11-07 10:57:55.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/client.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     4604 2023-11-07 10:57:55.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/converter.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     1362 2023-11-07 10:57:51.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/factory.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     9421 2023-12-01 15:13:33.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/metadata_utils.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     5215 2023-11-07 10:57:51.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/provider.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     6288 2023-11-07 10:57:55.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/provider_node.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     4906 2023-11-07 10:57:55.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/subscription.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    10479 2023-11-07 10:57:55.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/subscription_async.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     6426 2023-11-07 10:57:55.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/subscription_sync.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     2978 2023-11-07 10:57:55.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/system.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    31125 2023-11-07 10:57:55.000000 ctrlx_datalayer-3.2.0/ctrlxdatalayer/variant.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)      736 2024-04-30 12:48:45.000000 ctrlx_datalayer-3.2.0/pyproject.toml
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)       38 2024-04-30 12:51:37.399273 ctrlx_datalayer-3.2.0/setup.cfg
+drwxrwxr-x   0 boschrexroth  (1001) boschrexroth  (1001)        0 2024-04-30 12:51:37.399273 ctrlx_datalayer-3.2.0/tests/
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    26071 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_bulk.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    11814 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_bulk_async.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    20246 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_client.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     6750 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_converter.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     1193 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_fbs.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     4999 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_integration_bulk.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     6264 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_integration_bulk_async.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    14848 2023-11-07 10:57:55.000000 ctrlx_datalayer-3.2.0/tests/test_integration_client.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     5333 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_integration_converter.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     3926 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_integration_provider.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    16958 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_integration_sub_async.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    12806 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_integration_sub_sync.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    12514 2023-12-01 15:13:33.000000 ctrlx_datalayer-3.2.0/tests/test_metadata_utils.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     2704 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_node.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     9470 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_provider.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     9611 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_provider_node.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    20938 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_subscription_async.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    22177 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_subscription_sync.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     7125 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_system.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)     1240 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_utils.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    13224 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_variant.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    15117 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_variant_array.py
+-rw-rw-r--   0 boschrexroth  (1001) boschrexroth  (1001)    19050 2023-10-16 06:56:32.000000 ctrlx_datalayer-3.2.0/tests/test_variant_functions.py
```

### Comparing `ctrlx-datalayer-3.1.0/LICENSES/MIT.txt` & `ctrlx_datalayer-3.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/LICENSES/boschrexroth_tac_delivery.txt` & `ctrlx_datalayer-3.2.0/LICENSES/boschrexroth_tac_delivery.txt`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/LICENSES/tc_for_provision_of_products_free_of_charge.pdf` & `ctrlx_datalayer-3.2.0/LICENSES/tc_for_provision_of_products_free_of_charge.pdf`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/PKG-INFO` & `ctrlx_datalayer-3.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: ctrlx-datalayer
-Version: 3.1.0
+Version: 3.2.0
 Summary: ctrlX Data Layer API for Python
 Author-email: Bosch Rexroth AG <github@boschrexroth.com>
 Project-URL: Homepage, https://github.com/boschrexroth
 Platform: linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSES/MIT.txt
 License-File: LICENSES/boschrexroth_tac_delivery.txt
 License-File: LICENSES/tc_for_provision_of_products_free_of_charge.pdf
-Requires-Dist: ctrlx_fbs~=2.1.0
+Requires-Dist: ctrlx_fbs~=2.2.0
 Requires-Dist: flatbuffers~=23.5.26
 
 # Python Wrapper for ctrlX Data Layer
 
 This project provides ctrlX Data Layer access via Python.
 It wraps the original ctrlX Data Layer written in C++.
 
 ## Setup
 
 Set up a virtual python environment and install the packages libzmq5 and ctrlX Data Layer
 
 ```bash
 sudo apt-get update && sudo apt-get -y install virtualenv libzmq5
 
-DATALAYER_DEB_VERSION=2.4.5
-SDK_RELEASE_VERSION=2.4.0
+DATALAYER_DEB_VERSION=2.6.1
+SDK_RELEASE_VERSION=2.6.0
 
 wget --quiet https://github.com/boschrexroth/ctrlx-automation-sdk/releases/download/${SDK_RELEASE_VERSION}/ctrlx-datalayer-${DATALAYER_DEB_VERSION}.deb \
     && sudo dpkg --install ctrlx-datalayer-${DATALAYER_DEB_VERSION}.deb \
     && rm ctrlx-datalayer-${DATALAYER_DEB_VERSION}.deb
     
 virtualenv -p python3 venv && source venv/bin/activate
 ```
```

### Comparing `ctrlx-datalayer-3.1.0/README.md` & `ctrlx_datalayer-3.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 ## Setup
 
 Set up a virtual python environment and install the packages libzmq5 and ctrlX Data Layer
 
 ```bash
 sudo apt-get update && sudo apt-get -y install virtualenv libzmq5
 
-DATALAYER_DEB_VERSION=2.4.5
-SDK_RELEASE_VERSION=2.4.0
+DATALAYER_DEB_VERSION=2.6.1
+SDK_RELEASE_VERSION=2.6.0
 
 wget --quiet https://github.com/boschrexroth/ctrlx-automation-sdk/releases/download/${SDK_RELEASE_VERSION}/ctrlx-datalayer-${DATALAYER_DEB_VERSION}.deb \
     && sudo dpkg --install ctrlx-datalayer-${DATALAYER_DEB_VERSION}.deb \
     && rm ctrlx-datalayer-${DATALAYER_DEB_VERSION}.deb
     
 virtualenv -p python3 venv && source venv/bin/activate
 ```
```

### Comparing `ctrlx-datalayer-3.1.0/ctrlx_datalayer.egg-info/PKG-INFO` & `ctrlx_datalayer-3.2.0/ctrlx_datalayer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: ctrlx-datalayer
-Version: 3.1.0
+Version: 3.2.0
 Summary: ctrlX Data Layer API for Python
 Author-email: Bosch Rexroth AG <github@boschrexroth.com>
 Project-URL: Homepage, https://github.com/boschrexroth
 Platform: linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSES/MIT.txt
 License-File: LICENSES/boschrexroth_tac_delivery.txt
 License-File: LICENSES/tc_for_provision_of_products_free_of_charge.pdf
-Requires-Dist: ctrlx_fbs~=2.1.0
+Requires-Dist: ctrlx_fbs~=2.2.0
 Requires-Dist: flatbuffers~=23.5.26
 
 # Python Wrapper for ctrlX Data Layer
 
 This project provides ctrlX Data Layer access via Python.
 It wraps the original ctrlX Data Layer written in C++.
 
 ## Setup
 
 Set up a virtual python environment and install the packages libzmq5 and ctrlX Data Layer
 
 ```bash
 sudo apt-get update && sudo apt-get -y install virtualenv libzmq5
 
-DATALAYER_DEB_VERSION=2.4.5
-SDK_RELEASE_VERSION=2.4.0
+DATALAYER_DEB_VERSION=2.6.1
+SDK_RELEASE_VERSION=2.6.0
 
 wget --quiet https://github.com/boschrexroth/ctrlx-automation-sdk/releases/download/${SDK_RELEASE_VERSION}/ctrlx-datalayer-${DATALAYER_DEB_VERSION}.deb \
     && sudo dpkg --install ctrlx-datalayer-${DATALAYER_DEB_VERSION}.deb \
     && rm ctrlx-datalayer-${DATALAYER_DEB_VERSION}.deb
     
 virtualenv -p python3 venv && source venv/bin/activate
 ```
```

### Comparing `ctrlx-datalayer-3.1.0/ctrlx_datalayer.egg-info/SOURCES.txt` & `ctrlx_datalayer-3.2.0/ctrlx_datalayer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/bulk.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/bulk.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/bulk_util.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/bulk_util.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_bulk.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_bulk.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_client.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_client.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_converter.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_converter.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_factory.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_factory.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_provider.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_provider.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_provider_node.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_provider_node.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_system.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_system.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/clib_variant.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/clib_variant.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/client.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/client.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/converter.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/converter.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/factory.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/factory.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/metadata_utils.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/provider.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/provider.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/provider_node.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/provider_node.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/subscription.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/subscription.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/subscription_async.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/subscription_async.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/subscription_sync.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/subscription_sync.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/system.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/system.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/ctrlxdatalayer/variant.py` & `ctrlx_datalayer-3.2.0/ctrlxdatalayer/variant.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/pyproject.toml` & `ctrlx_datalayer-3.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ctrlx-datalayer"
-version = "3.1.0"
+version = "3.2.0"
 authors = [
   { name="Bosch Rexroth AG", email="github@boschrexroth.com" },
 ]
 description = "ctrlX Data Layer API for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
 ]
 
 dependencies = [
-"ctrlx_fbs~=2.1.0", 
+"ctrlx_fbs~=2.2.0", 
 "flatbuffers~=23.5.26"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/boschrexroth"
 
 [tool.setuptools]
```

### Comparing `ctrlx-datalayer-3.1.0/tests/test_bulk.py` & `ctrlx_datalayer-3.2.0/tests/test_bulk.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_bulk_async.py` & `ctrlx_datalayer-3.2.0/tests/test_bulk_async.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_client.py` & `ctrlx_datalayer-3.2.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_converter.py` & `ctrlx_datalayer-3.2.0/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_fbs.py` & `ctrlx_datalayer-3.2.0/tests/test_fbs.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_integration_bulk.py` & `ctrlx_datalayer-3.2.0/tests/test_integration_bulk.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_integration_bulk_async.py` & `ctrlx_datalayer-3.2.0/tests/test_integration_bulk_async.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_integration_client.py` & `ctrlx_datalayer-3.2.0/tests/test_integration_client.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_integration_converter.py` & `ctrlx_datalayer-3.2.0/tests/test_integration_converter.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_integration_provider.py` & `ctrlx_datalayer-3.2.0/tests/test_integration_provider.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_integration_sub_async.py` & `ctrlx_datalayer-3.2.0/tests/test_integration_sub_async.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_integration_sub_sync.py` & `ctrlx_datalayer-3.2.0/tests/test_integration_sub_sync.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_metadata_utils.py` & `ctrlx_datalayer-3.2.0/tests/test_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_node.py` & `ctrlx_datalayer-3.2.0/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_provider.py` & `ctrlx_datalayer-3.2.0/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_provider_node.py` & `ctrlx_datalayer-3.2.0/tests/test_provider_node.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_subscription_async.py` & `ctrlx_datalayer-3.2.0/tests/test_subscription_async.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_subscription_sync.py` & `ctrlx_datalayer-3.2.0/tests/test_subscription_sync.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_system.py` & `ctrlx_datalayer-3.2.0/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_utils.py` & `ctrlx_datalayer-3.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_variant.py` & `ctrlx_datalayer-3.2.0/tests/test_variant.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_variant_array.py` & `ctrlx_datalayer-3.2.0/tests/test_variant_array.py`

 * *Files identical despite different names*

### Comparing `ctrlx-datalayer-3.1.0/tests/test_variant_functions.py` & `ctrlx_datalayer-3.2.0/tests/test_variant_functions.py`

 * *Files identical despite different names*

