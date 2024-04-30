# Comparing `tmp/FileTAO-2.1.0.tar.gz` & `tmp/FileTAO-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FileTAO-2.1.0.tar", last modified: Tue Mar 12 16:00:57 2024, max compression
+gzip compressed data, was "FileTAO-3.0.0.tar", last modified: Tue Apr 30 03:15:26 2024, max compression
```

## Comparing `FileTAO-2.1.0.tar` & `FileTAO-3.0.0.tar`

### file list

```diff
@@ -1,90 +1,98 @@
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-12 16:00:57.941162 FileTAO-2.1.0/
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-12 16:00:57.937162 FileTAO-2.1.0/FileTAO.egg-info/
--rw-r--r--   0 phil      (1007) phil      (1008)    66664 2024-03-12 16:00:57.000000 FileTAO-2.1.0/FileTAO.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1007) phil      (1008)     1916 2024-03-12 16:00:57.000000 FileTAO-2.1.0/FileTAO.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1007) phil      (1008)        1 2024-03-12 16:00:57.000000 FileTAO-2.1.0/FileTAO.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1007) phil      (1008)       52 2024-03-12 16:00:57.000000 FileTAO-2.1.0/FileTAO.egg-info/entry_points.txt
--rw-rw-r--   0 phil      (1007) phil      (1008)      299 2024-03-12 16:00:57.000000 FileTAO-2.1.0/FileTAO.egg-info/requires.txt
--rw-rw-r--   0 phil      (1007) phil      (1008)       22 2024-03-12 16:00:57.000000 FileTAO-2.1.0/FileTAO.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1007) phil      (1008)     1069 2024-02-20 00:19:28.000000 FileTAO-2.1.0/LICENSE
--rw-rw-r--   0 phil      (1007) phil      (1008)    66664 2024-03-12 16:00:57.941162 FileTAO-2.1.0/PKG-INFO
--rw-rw-r--   0 phil      (1007) phil      (1008)    65628 2024-03-12 15:06:47.000000 FileTAO-2.1.0/README.md
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-12 16:00:57.937162 FileTAO-2.1.0/neurons/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-2.1.0/neurons/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    18421 2024-03-12 15:56:01.000000 FileTAO-2.1.0/neurons/api.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    44074 2024-03-12 15:56:01.000000 FileTAO-2.1.0/neurons/miner.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    16620 2024-03-12 15:56:01.000000 FileTAO-2.1.0/neurons/validator.py
--rw-rw-r--   0 phil      (1007) phil      (1008)       38 2024-03-12 16:00:57.941162 FileTAO-2.1.0/setup.cfg
--rw-rw-r--   0 phil      (1007) phil      (1008)     3912 2024-03-12 15:33:30.000000 FileTAO-2.1.0/setup.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-12 16:00:57.937162 FileTAO-2.1.0/storage/
--rw-rw-r--   0 phil      (1007) phil      (1008)     2342 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/__init__.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-12 16:00:57.937162 FileTAO-2.1.0/storage/api/
--rw-rw-r--   0 phil      (1007) phil      (1008)      133 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/api/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     2246 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/api/example.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     3968 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/api/retrieve_api.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5567 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/api/store_api.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     3991 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/api/utils.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-12 16:00:57.937162 FileTAO-2.1.0/storage/cli/
--rw-rw-r--   0 phil      (1007) phil      (1008)     1199 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/cli/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     8690 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/cli/cli.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     1602 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/cli/default_values.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     6742 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/cli/listcommand.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     2274 2024-02-27 03:13:35.000000 FileTAO-2.1.0/storage/cli/neuroncommand.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     9528 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/cli/retrievecommand.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     4711 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/cli/statscommand.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    10520 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/cli/storecommand.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     1372 2024-03-12 14:58:37.000000 FileTAO-2.1.0/storage/constants.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-12 16:00:57.937162 FileTAO-2.1.0/storage/miner/
--rw-rw-r--   0 phil      (1007) phil      (1008)     1240 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/miner/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    10531 2024-03-06 23:48:11.000000 FileTAO-2.1.0/storage/miner/config.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    15278 2024-02-22 21:12:16.000000 FileTAO-2.1.0/storage/miner/database.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     4041 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/miner/run.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     4619 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/miner/set_weights.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    14477 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/miner/utils.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-12 16:00:57.937162 FileTAO-2.1.0/storage/plot/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/plot/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     6672 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/plot/utils.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     7564 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/protocol.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-12 16:00:57.937162 FileTAO-2.1.0/storage/shared/
--rw-rw-r--   0 phil      (1007) phil      (1008)     1200 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/shared/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     4310 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/shared/checks.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     7290 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/shared/ecc.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    17746 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/shared/merkle.py
--rw-rw-r--   0 phil      (1007) phil      (1008)      923 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/shared/subtensor.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     6050 2024-03-03 21:47:24.000000 FileTAO-2.1.0/storage/shared/utils.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     3434 2024-03-04 01:56:44.000000 FileTAO-2.1.0/storage/shared/weights.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-12 16:00:57.941162 FileTAO-2.1.0/storage/validator/
--rw-rw-r--   0 phil      (1007) phil      (1008)     1492 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/validator/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    13665 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/validator/bonding.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    10538 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/validator/challenge.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5864 2024-02-22 21:12:16.000000 FileTAO-2.1.0/storage/validator/cid.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    12036 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/validator/config.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    38740 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/validator/database.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     3211 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/validator/distribute.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    15435 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/validator/encryption.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     3046 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/validator/event.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     6223 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/validator/forward.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     9341 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/validator/network.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5072 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/validator/rebalance.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    16213 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/validator/retrieve.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    11988 2024-03-12 13:26:36.000000 FileTAO-2.1.0/storage/validator/reward.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     8798 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/validator/state.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    23045 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/validator/store.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    32277 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/validator/utils.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     8315 2024-02-20 00:19:28.000000 FileTAO-2.1.0/storage/validator/verify.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     6957 2024-03-11 21:33:06.000000 FileTAO-2.1.0/storage/validator/weights.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-12 16:00:57.941162 FileTAO-2.1.0/tests/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-2.1.0/tests/__init__.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-12 16:00:57.941162 FileTAO-2.1.0/tests/integration/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-2.1.0/tests/integration/__init__.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-12 16:00:57.941162 FileTAO-2.1.0/tests/unit/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-2.1.0/tests/unit/__init__.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-12 16:00:57.941162 FileTAO-2.1.0/tests/unit/cli/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-2.1.0/tests/unit/cli/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)      407 2024-02-20 00:19:28.000000 FileTAO-2.1.0/tests/unit/cli/test_cli.py
--rw-rw-r--   0 phil      (1007) phil      (1008)      442 2024-02-27 03:13:35.000000 FileTAO-2.1.0/tests/unit/cli/test_neuroncommand.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-12 16:00:57.941162 FileTAO-2.1.0/tests/unit/validator/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-2.1.0/tests/unit/validator/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)      863 2024-02-20 00:19:28.000000 FileTAO-2.1.0/tests/unit/validator/test_challenge.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     1529 2024-02-20 00:19:28.000000 FileTAO-2.1.0/tests/unit/validator/test_encryption.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     1118 2024-02-20 00:19:28.000000 FileTAO-2.1.0/tests/unit/validator/test_state.py
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.004255 FileTAO-3.0.0/
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:25.996255 FileTAO-3.0.0/FileTAO.egg-info/
+-rw-r--r--   0 phil      (1007) phil      (1008)    67427 2024-04-30 03:15:25.000000 FileTAO-3.0.0/FileTAO.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1007) phil      (1008)     2099 2024-04-30 03:15:25.000000 FileTAO-3.0.0/FileTAO.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1007) phil      (1008)        1 2024-04-30 03:15:25.000000 FileTAO-3.0.0/FileTAO.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1007) phil      (1008)       52 2024-04-30 03:15:25.000000 FileTAO-3.0.0/FileTAO.egg-info/entry_points.txt
+-rw-rw-r--   0 phil      (1007) phil      (1008)      385 2024-04-30 03:15:25.000000 FileTAO-3.0.0/FileTAO.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1007) phil      (1008)       22 2024-04-30 03:15:25.000000 FileTAO-3.0.0/FileTAO.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1007) phil      (1008)     1069 2024-02-20 00:19:28.000000 FileTAO-3.0.0/LICENSE
+-rw-r--r--   0 phil      (1007) phil      (1008)    67427 2024-04-30 03:15:26.004255 FileTAO-3.0.0/PKG-INFO
+-rw-rw-r--   0 phil      (1007) phil      (1008)    65567 2024-04-29 21:23:35.000000 FileTAO-3.0.0/README.md
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:25.996255 FileTAO-3.0.0/neurons/
+-rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-3.0.0/neurons/__init__.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    21877 2024-04-30 03:12:19.000000 FileTAO-3.0.0/neurons/api.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    44346 2024-04-28 20:19:43.000000 FileTAO-3.0.0/neurons/miner.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    16973 2024-04-28 20:19:43.000000 FileTAO-3.0.0/neurons/validator.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)       38 2024-04-30 03:15:26.004255 FileTAO-3.0.0/setup.cfg
+-rw-rw-r--   0 phil      (1007) phil      (1008)     3962 2024-04-26 15:16:51.000000 FileTAO-3.0.0/setup.py
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:25.996255 FileTAO-3.0.0/storage/
+-rw-rw-r--   0 phil      (1007) phil      (1008)     2364 2024-04-27 21:32:42.000000 FileTAO-3.0.0/storage/__init__.py
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:25.996255 FileTAO-3.0.0/storage/api/
+-rw-rw-r--   0 phil      (1007) phil      (1008)      179 2024-04-28 20:19:49.000000 FileTAO-3.0.0/storage/api/__init__.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     3431 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/api/base.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     4975 2024-04-28 20:19:49.000000 FileTAO-3.0.0/storage/api/delete_api.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     2552 2024-04-28 20:19:49.000000 FileTAO-3.0.0/storage/api/example.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     5923 2024-04-28 20:19:49.000000 FileTAO-3.0.0/storage/api/retrieve_api.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     6841 2024-04-29 05:21:26.000000 FileTAO-3.0.0/storage/api/store_api.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     3991 2024-03-17 16:11:41.000000 FileTAO-3.0.0/storage/api/utils.py
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.000255 FileTAO-3.0.0/storage/cli/
+-rw-rw-r--   0 phil      (1007) phil      (1008)     1199 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/cli/__init__.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     8728 2024-04-29 21:23:35.000000 FileTAO-3.0.0/storage/cli/cli.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     1602 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/cli/default_values.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     6742 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/cli/listcommand.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     2274 2024-03-17 16:11:41.000000 FileTAO-3.0.0/storage/cli/neuroncommand.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     9067 2024-04-29 21:23:35.000000 FileTAO-3.0.0/storage/cli/retrievecommand.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     4711 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/cli/statscommand.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     9471 2024-04-29 21:23:35.000000 FileTAO-3.0.0/storage/cli/storecommand.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     2136 2024-04-28 21:03:18.000000 FileTAO-3.0.0/storage/constants.py
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.000255 FileTAO-3.0.0/storage/indexer/
+-rw-rw-r--   0 phil      (1007) phil      (1008)     8064 2024-04-30 03:12:19.000000 FileTAO-3.0.0/storage/indexer/__init__.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     8100 2024-04-30 03:12:19.000000 FileTAO-3.0.0/storage/indexer/endpoint.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    10255 2024-04-29 16:40:25.000000 FileTAO-3.0.0/storage/indexer/redis.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)      675 2024-04-27 21:32:42.000000 FileTAO-3.0.0/storage/indexer/sqlite.py
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.000255 FileTAO-3.0.0/storage/miner/
+-rw-rw-r--   0 phil      (1007) phil      (1008)     1240 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/miner/__init__.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    10763 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/miner/config.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    15278 2024-02-22 21:12:16.000000 FileTAO-3.0.0/storage/miner/database.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     4204 2024-04-28 17:54:08.000000 FileTAO-3.0.0/storage/miner/run.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     4619 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/miner/set_weights.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    14477 2024-03-17 16:50:11.000000 FileTAO-3.0.0/storage/miner/utils.py
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.000255 FileTAO-3.0.0/storage/plot/
+-rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-03-17 16:11:41.000000 FileTAO-3.0.0/storage/plot/__init__.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     6672 2024-03-17 16:11:41.000000 FileTAO-3.0.0/storage/plot/utils.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     7921 2024-04-28 20:19:49.000000 FileTAO-3.0.0/storage/protocol.py
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.000255 FileTAO-3.0.0/storage/shared/
+-rw-rw-r--   0 phil      (1007) phil      (1008)     1200 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/shared/__init__.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     5413 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/shared/checks.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     7290 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/shared/ecc.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    17746 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/shared/merkle.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)      923 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/shared/subtensor.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     7992 2024-04-28 20:19:49.000000 FileTAO-3.0.0/storage/shared/utils.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     3436 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/shared/weights.py
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.004255 FileTAO-3.0.0/storage/validator/
+-rw-rw-r--   0 phil      (1007) phil      (1008)     1514 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/__init__.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    14756 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/bonding.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    10538 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/challenge.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     5864 2024-02-22 21:12:16.000000 FileTAO-3.0.0/storage/validator/cid.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    12139 2024-04-30 03:12:19.000000 FileTAO-3.0.0/storage/validator/config.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    43538 2024-04-28 20:19:49.000000 FileTAO-3.0.0/storage/validator/database.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     3113 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/dendrite.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     3211 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/validator/distribute.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    15435 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/validator/encryption.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     3046 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/validator/event.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     6223 2024-03-17 16:11:41.000000 FileTAO-3.0.0/storage/validator/forward.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     9417 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/network.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     5072 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/validator/rebalance.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    16215 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/retrieve.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    12356 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/reward.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     8798 2024-03-17 16:11:41.000000 FileTAO-3.0.0/storage/validator/state.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    23047 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/store.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)    32272 2024-04-28 17:54:08.000000 FileTAO-3.0.0/storage/validator/utils.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     8315 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/validator/verify.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     6961 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/weights.py
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.004255 FileTAO-3.0.0/tests/
+-rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/__init__.py
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.004255 FileTAO-3.0.0/tests/integration/
+-rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/integration/__init__.py
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.004255 FileTAO-3.0.0/tests/unit/
+-rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/unit/__init__.py
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.004255 FileTAO-3.0.0/tests/unit/cli/
+-rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/unit/cli/__init__.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)      407 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/unit/cli/test_cli.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)      442 2024-03-17 16:11:41.000000 FileTAO-3.0.0/tests/unit/cli/test_neuroncommand.py
+drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.004255 FileTAO-3.0.0/tests/unit/validator/
+-rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/unit/validator/__init__.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)      863 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/unit/validator/test_challenge.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     1529 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/unit/validator/test_encryption.py
+-rw-rw-r--   0 phil      (1007) phil      (1008)     1118 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/unit/validator/test_state.py
```

### Comparing `FileTAO-2.1.0/FileTAO.egg-info/PKG-INFO` & `FileTAO-3.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,22 @@
-Metadata-Version: 2.1
-Name: FileTAO
-Version: 2.1.0
-Summary: Philanthropic storage for the masses. (FileTAO)
-Home-page: https://github.com/ifrit98/storage-subnet
-Author: philanthrope
-Author-email: ifrit98@gmail.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9,<3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # FileTAO
 
 [![Latest Version](https://img.shields.io/pypi/v/filetao.svg)](https://pypi.org/project/filetao/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/filetao)](https://pypi.org/project/filetao)
 [![License](https://img.shields.io/pypi/l/filetao.svg)](https://github.com/ifrit98/storage-subnet/blob/master/LICENSE)
 
 ![Subnet21](assets/Subnet21.png)
 
 FileTAO (Bittensor Subnet 21) implements a novel, multi-layered zero-knowledge interactive proof-of-spacetime algorithm by cleverly using Pedersen commitments, random challenges leveraging elliptic curve cryptography, sequential seed-based chained hash verification, and merkle proofs to achieve an efficient, robust, secure, and highly available decetralized storage system on the Bittensor network. The system validates on encrypted user data, such that miners are unaware of what data they are storing, and only end-users may encrypt/decrypt the data they provide with their bittensor wallet coldkey.
 
 We consider this system to be an important stepping stone so that bittensor can fulfill its mission of democratizing intelligence, and a decentralized AWS platform is a key brick in this wall. 
 
 **NOTICE**: Using this software, you **must** agree to the Terms and Agreements provided in the [terms and conditions](TERMS.md) document. By downloading and running this software, you implicitly agree to these terms and conditions.
 
-Currently supporting `python>=3.9,<3.11`.
+Currently supporting `python>=3.9,<3.12`.
 
 > Note: The storage subnet is in an alpha stage and is subject to rapid development.
 
 # Table of Contents for Subnet 21 (FileTAO)
 1. [FileTAO Overview](#filetao)
 2. [Installation](#installation)
    - [Install Redis](#install-redis)
@@ -75,28 +49,36 @@
    - [Advanced Cryptographic Techniques](#advanced-cryptographic-techniques)
    - [User-Centric Approach](#user-centric-approach)
 7. [Zero Knowledge Proof-of-Spacetime](#zero-knowledge-proof-of-spacetime)
    - [Storage Phase](#storage-phase)
    - [Challenge Phase](#challenge-phase)
    - [Retrieval Phase](#retrieval-phase)
 8. [Reward System](#reward-system)
+   - [Overview and Justification](#overview-and-justification)
    - [Speed and Reliability in Decentralized Storage Mining](#speed-and-reliability-in-decentralized-storage-mining)
+   - [Viewing Wandb Runs](#viewing-wandb-runs)
 9. [Epoch UID Selection](#epoch-uid-selection)
 10. [Running FileTAO](#running-filetao)
     - [Running a Miner](#running-a-miner)
     - [Running a Validator](#running-a-validator)
     - [Running the API](#running-the-api)
     - [Setup WandB](#setup-wandb)
+    - [Testnet](#testnet)
 11. [Local Subtensor](#local-subtensor)
 12. [Database Schema Migration](#database-schema-migration)
 13. [Disable RDB](#disable-rdb)
-
+14. [FileTAO Docker](#filetao-docker)
+15. [Demos](#demo-notebooks-and-examples)
 
 ## Installation
 ```bash
+# Please install torch-cpu if you do not need a gpu. (GPU not required for FileTAO)
+pip install torch==2.3.0+cpu -f https://download.pytorch.org/whl/torch_stable.html
+
+# Clone and Install the FileTAO repo.
 git clone https://github.com/ifrit98/storage-subnet
 cd storage-subnet
 python -m pip install -e .
 ```
 
 ### Install Redis
 Install Redis on your host system.
@@ -139,41 +121,19 @@
 Nov 16 22:35:42 user systemd[1]: Started Advanced key-value store.
 ```
 
 ### Secure Redis Configuration
 
 In order to securely run a node, whether a miner or validator, you must run ensure your redis instance is secure from the outside internet and is password-protected.
 
-The following steps are **mandatory** for secure communication on the network:
+The following steps are **recommended** for secure communication on the network and data integrity:
 
-1. Closing the default redis port
 1. Password protecting redis
-1. Enabling persistence
-
-#### Close external traffic to Redis 
+1. Enabling redis persistence
 
-> Note: **EXPOSING THE REDIS PORT IS A MAJOR SECURITY RISK**
-
-This Bash script is designed to configure UFW (Uncomplicated Firewall) to manage access to default Redis port 6379. The script's primary function is to block all external traffic to port 6379, typically used by Redis, while allowing local processes to still access this port.
-
-##### Usage
-To run the script, use the following command in the terminal:
-```bash
-sudo ./scripts/redis/create_redis_firewall.sh
-```
-Running this script will:
-- Check if UFW is installed and active. If UFW is not active, the script will attempt to enable it.
-- Set UFW rules to deny all external access to port 6379.
-- Set UFW rules to allow all local access to port 6379.
-- Apply the changes by reloading UFW.
-
-##### Important Considerations
-- **Test Before Production**: Always test the script in a controlled environment before deploying it in a production setting.
-- **Existing Rules**: If there are existing rules for port 6379, review the script to ensure compatibility.
-- **Firewall Management**: This script is specifically for systems using UFW. If another firewall management tool is in use, this script will not be compatible.
 
 #### Automated Redis Password Configuration
 To enhance security, our system now automatically generates a strong password for Redis. This is **REQUIRED**. This is handled by the `set_redis_password.sh` script. Follow these steps to set up Redis with an automated password:
 
 1. **Run the Redis Start Script**: 
     ```bash
     bash scripts/redis/set_redis_password.sh
@@ -266,22 +226,22 @@
 from storage.api import store, retrieve
 
 # Store data
 wallet = bt.wallet()
 subtensor = bt.subtensor()
 
 data = b"Some bytestring data!"
-cid, hotkeys = await store(data, wallet, subtensor, netuid=22)
+cid, hotkeys = await store(data, wallet, subtensor, netuid=21)
 print("Stored {} with {} hotkeys".format(cid, hotkeys))
 > Stored bafkreid6mhmfptdpfvljyavss77zmo6b2oert2pula2gy4tosekupm4nqa with validator hotkeys [5CaFuijc2ucdoWhkjLaYgnzYrpv62KGt1fWWtUxhFHXPA3KK, 5FKwbwguHU1SVQiGot5YKSTQ6fWGVv2wRHFrWfwp9X9nWbyU]
 ```
 
 Now you can retrieve the data using the content identifier `CID` and the `hotkey`s directly:
 ```python
-data = await retrieve(cid, wallet, subtensor, netuid=22, hotkeys=hotkeys)
+data = await retrieve(cid, wallet, subtensor, netuid=21, hotkeys=hotkeys)
 print(data)
 > b"Some bytestring data!"
 ```
 
 ### Using SubnetsAPI 
 In addition to the convenience wrappers and command-line interface, FileTao can be accessed via the bittensor subnets python API.
 
@@ -615,153 +575,194 @@
 In each phase, cryptographic primitives ensure data integrity and confidentiality. The encryption and commitment schemes ensure the data's security, while Merkle trees and random challenges provide a robust method for verifying data possession without revealing the actual data.
 
 In each phase, cryptographic primitives like hashing, commitment schemes (e.g., Elliptic Curve Cryptography and Pedersen commitments), and data structures like Merkle trees are employed to ensure the integrity, confidentiality, and availability of the data. The use of seeds and randomness in commitments adds an additional layer of security and ensures that each instance of data storage and retrieval is unique and verifiable. See [here](https://kndrck.co/posts/efficient-merkletrees-zk-proofs/) for more information.
 
 
 ## Reward System
 
+There are several components to the reward mechanism and is multi-layered. In a nutshell, the goals are as follows:
+
+- Incentivize data durability and salience via cryptographic proof system. (E.g. don't lose data.)
+- Incentivize good performance over a long period of time. (Tier system to reward based on reputation.)
+- Incentivize fast response times. We want to retrieve user data quickly and ensure that it is over high network bandwidth.
+
 In FileTAO's decentralized storage system, optimal behavior is crucial for the overall health and efficiency of the network. Miners play a vital role in maintaining this ecosystem, and their actions directly impact their rewards and standing within the subnet. We have implemented a tier-based reward system to encourage proper behavior, successful challenge completions, and consistent performance.
 
 Failing to pass either challenge or retrieval verifications incur negative rewards. This is doubly destructive, as rolling statistics are continuously logged to periodically compute which tier a given miner hotkey belongs to. When a miner achieves the threshold for the next tier, the rewards that miner receives proportionally increase. Conversely, when a miner drops below the threshold of the previous tier, that miner's rewards are slashed such that they receive rewards proportionally to the immediately lower tier.
 
+### Overview and Justification
+FileTAO's Multi-dimensional reward mechanism is spread across 4 main axes:
+(1) Availability: Is the miner reachable when requested? Incentivizes uptime.
+(2) Speed (performant): how fast was the normalized response time?
+(3) Correctness (reliable): did the proof succeed? y/n
+(4) Trustworthiness (correctness over time): Tier definitions encapsulate consistenty and trustworthiness over time. A miner that rarely fails challenges and faithfully returns data when requested will receive an initial higher proportional reward.
+
+The main drivers behind the reward mechanism are to model meritocratic systems as seen in the academic realm and in the business world that scales trust across time and observation of output. For example, we create various "tiers" in education, Undergraduate, Masters, PhD, Post Doc, or in software, Junior Engineer, Senior Engineer, Principal Engineer, Staff Engineer, etc where each subsequent level achieved has proportionally greater expecetations on performance and qualification of the individual. 
+
+However, performance of the individual must match the expectations of the pedigree, and behavior that is inconsistent with a given level will be adjusted. If, for example, a Junior Engineer proves their output is substantial and over time completes projects that provide value, that engineer will be promoted to Senior Engineer over time, and pontentially beyond. Conversely, a Principal Engineer that consistently underperforms expectations will be demoted to a role with lower expectations until able to prove otherwise. The same logic applies to miners in FileTAO (SN21).
+
+Tier (class) mobility is at the heart of the mechanism, and provides a balance between competition and trust, where over time competitiveness breeds a degree of trust on which we can associate a degree of reliability with a given entity (or miner).
+
 **Why Optimal Behavior Matters:**
 1. **Reliability:** Miners who consistently store, retrieve, and pass challenges with high Wilson Scores ensure the reliability and integrity of the network.
 2. **Trust:** High-performing miners build trust in the network, attracting more users and increasing the overall value of the system.
 3. **Efficiency:** Optimal behavior leads to a more efficient network, reducing the likelihood of data loss and ensuring fast, reliable access to stored information.
 
 **Tier-Based Reward System:**
 - **Tiers:** We classify miners into four tiers – Diamond, Gold, Silver, and Bronze – based on their performance metrics.
 - **Performance Metrics:** These include the Wilson Score in storage, retrieval, and challenge tasks, as well as the total number of successful operations.
 - **Higher Rewards for Higher Tiers:** Miners in higher tiers receive a greater proportion of the rewards, reflecting their superior performance and contribution to the network.
 
 ### **Wilson Score**
-A measure of confidence is required to assess reliability in low sample environments. For miners who have less history, it is unfair to expect perfection early on and is account for by using a statistical tool, the `Wilson Score`. 
+
+A measure of confidence is required to assess reliability in low sample environments. For miners who have less history, it is unfair to expect perfection early on and is account for by using a statistical tool, the `Wilson Score`. An asymmetric approximation of the confidence interval suited for low sample sizes given a particular z-score target, the `Wilson score` doesn't suffer from problems of overshoot and zero-width intervals that afflict the normal interval approximation.
+
+See: https://en.wikipedia.org/wiki/Binomial_proportion_confidence_interval#Wilson_score_interval for more information.
 
 For example, if a miner succeeds 4/5 times, it has a success rate of 80%. However it may not be indicative of true performance and reliability. Thus we have added Wilson Scores to accomodate low sample populations to get a more balanced approach to scoring miners.
 
 This effectively allows for forgiveness for early failures and facilitates miners who are faithful actors to still rise through the tier system without being perpetually punished for early mistakes or poor optimization.
 
 The equivalent wilson score for 4 of 5 attempts is `0.77`, which indicates with 95% statistical confidence that this miner is AT least this successful 80% of the time. Functionally, this allows for lowering of the tier requirements while having statistical confidence that over time, the miner may continue to improve performance from there while being considered reliable.
 
-**Moving Up Tiers:**
-- To ascend to a higher tier, a miner must maintain high Wilson Scores and achieve a set number of total successes.
-- This progression system incentivizes continuous improvement and excellence in mining operations.
-
-**Graphical Representation:**
-- The graph below illustrates how rewards increase as miners advance through the tiers. It visually represents the potential growth in earnings as miners optimize their operations and maintain high standards of performance.
-
-<div align="center">
-   <img src="assets/reward-tiers-vert.png" alt="Bonding Curves" width="650"/>
-</div>
+More concretely, given `N` trials, the wilson score establishes a lower bound for the confidence interval on miner success rates given low sample or population sizes. E.g., if a miner responds successfuly 8 of 9 times, it's lower bound on success rate is roughly `0.8701769999681506`. In other words, `wilson_score(8,9) == 0.8701769999681506`, suggesting that 87% of the time, this miner is expected to succeed on average. 
+
+This calculation is used as the lower bound to determine tier eligibility and establishes a "minimium trust level" for the miner. If a miner continues to have failed challenges, the wilson score lower bound will cross below the current tier threshold, and when the tiers are recalculated, that miner will move down a tier (e.g. `Diamond -> Gold`.)
 
-#### Tier System:
+### **monitor**
+Miners are also incentivized to be available, and are punshed for not being online, (e.g. failed `n` pings) by the `monitor` protocol. Periodically (every `m` steps) validators ping a set of `k` miners (default is 40), and after 5 successive failed attempts to ping a specific UID, that miner will be negatively rewarded for unavailability.
+
+### Tier System:
 The tier system classifies miners into five distinct categories, each with specific requirements and storage limits. These tiers are designed to reward miners based on their performance, reliability, and the total volume of data they can store.
 
 Importance of Tier System:
 - **Encourages High Performance:** Higher tiers reward miners with greater benefits, motivating them to maintain high Wilson Scores.
 - **Enhances Network Reliability:** The tier system ensures that only the most reliable and efficient miners handle significant volumes of data, enhancing the overall reliability of the network.
 - **Fair Reward Distribution:** The reward factors are proportional to the miners' tier, ensuring a fair distribution of rewards based on performance.
 
 1. 🎇 **Super Saiyan Tier:** 
-   - **Storage Limit:** 1 Exabyte (EB)
-   - **Store Wilson Score:** 0.88
-   - **Minimum Successes Required:** 10,000
+   - **Storage Limit:** 50 Petabytes (PB)
+   - **Store Wilson Score:** 0.9
+   - **Minimum Successes Required:** 15,000
    - **Reward Factor:** 1.0 (100% rewards)
 
-2. 💎 **Diamond Tier:**
-   - **Storage Limit:** 1 Petabyte (PB)
-   - **Store Wilson Score:**  0.77
-   - **Minimum Successes Required:** 5,000
-   - **Reward Factor:** 0.9 (90% rewards)
-
-3. 🥇 **Gold Tier:**
-   - **Storage Limit:** 100 Terabytes (TB)
-   - **Store Wilson Score:** 0.66
-   - **Minimum Successes Required:** 2,000
+2. 🌹 **Ruby Tier**
+   - **Storage Limit:** 20 Petabytes (PB)
+   - **Store Wilson Score:** 0.85
+   - **Minimum Successes Required:** 10,000
+   - **Rewrd Factor:** 0.9 (90% rewards)
+
+3. 🔮 **Emerald Tier**
+   - **Storage Limit:** 10 Petabytes (PB)
+   - **Store Wilson Score:** 0.8
+   - **Minimum Successes Required:** 8,000
+   - **Rewrd Factor:** 0.85 (85% rewards)
+
+4. 💠 **Diamond Tier:**
+   - **Storage Limit:** 5 Petabytes (PB)
+   - **Store Wilson Score:**  0.75
+   - **Minimum Successes Required:** 6,000
    - **Reward Factor:** 0.8 (80% rewards)
 
-4. 🥈 **Silver Tier:**
-   - **Storage Limit:** 10 Terabytes (TB)
-   - **Store Wilson Score:** 0.55
-   - **Minimum Successes Required:** 1,000
+5. 🔗 **Platinum Tier**
+   - **Storage Limit:** 1 Petabyte (PB)
+   - **Store Wilson Score:** 0.65
+   - **Minimum Successes Required:** 4,000
+   - **Reward Factor:** 0.75 (75% rewards) 
+
+6. 🥇 **Gold Tier:**
+   - **Storage Limit:** 200 Terabytes (TB)
+   - **Store Wilson Score:** 0.65
+   - **Minimum Successes Required:** 2,000
    - **Reward Factor:** 0.7 (70% rewards)
 
-5. 🥉 **Bronze Tier:**
-   - **Storage Limit:** 1 Terabyte (TB)
+7. 🥈 **Silver Tier:**
+   - **Storage Limit:** 50 Terabytes (TB)
+   - **Store Wilson Score:** 0.6
+   - **Minimum Successes Required:** 500
+   - **Reward Factor:** 0.65 (65% rewards)
+
+8. 🥉 **Bronze Tier:**
+   - **Storage Limit:** 10 Terabytes (TB)
    - **Store Wilson Score:** Not specifically defined for this tier
    - **Minimum Successes Required:** Not specifically defined for this tier
    - **Reward Factor:** 0.6 (60% rewards)
 
 #### Maintaining and Advancing Tiers:
 - To advance to a higher tier, miners must consistently achieve the required minimum Wilson Scores in their operations.
-- Periodic evaluations are conducted to ensure miners maintain the necessary performance standards to stay in their respective tiers.
-- Advancing to a higher tier takes time. In order to ascend to the first higher tier (Silver), it takes at least 1000 successful requests, whether they are challenge requests, store requests, or retry requests and must maintain a 95% Wilson Score in all categories. 
-- Depending on how often a miner is queried, how many validators are operating at one given time, and primarily the performance of the miner, this can take several hours to several days. Assuming full 64 validator slots are occupied, this should take a matter of hours.
+- Periodic evaluations are conducted to ensure miners maintain the necessary performance standards to stay in their respective tiers, or move up or down tiers.
+- Advancing to a higher tier takes time. In order to ascend to the first higher tier (Silver), it takes at least 1000 successful requests, whether they are challenge requests, store requests, or retry requests and must maintain the minimum Wilson Score for successes / attempts. 
+- Depending on how often a miner is queried, how many validators are operating at one given time, and primarily the performance of the miner, this can take several hours to several days. Assuming full 64 validator slots are occupied, this should take ~100 hours.
 
-Here is a distribution of UIDs queried over 1000 blocks based on block hash:
-![uid-dist](assets/uid_dist.png)
+As miners move up tiers, their responsibility increases proportionally. Thus, miners who move from Silver -> Gold are expected to be able to store up to 200 Terabytes (TB) of data, a 4x the storage cap for Silver. Similarly, it must maintain a minimum wilson score of 0.66 over it's lifetime, increasing the lower bound for expected performance and reliability. It also means that this miner will now receive a higher percentage of rewards for each successful query, going from 65% -> 70%. This does not mean that the miner may rest on its laurels, and may move right back down a tier (or more) if it does not meed the minimum requirements for Gold.
 
 Assuming perfect performance, that out of ~200 miner UIDs, each of which is queried roughly 34 times every 1000 rounds, namely a 3.4% chance every query round, one can expect to reach the next tier within 
-
 ```bash
-hours = total_successes / prob_of_query_per_round * time_per_round / 3600
-hours = 98 # roughly 4 days at perfect performance to top tier (no challenge failures)
+hours = total_successes / prob_of_query_per_round * time_per_round / 3600 / num_active_validators
+hours = 4.9 # roughly 5 hours at perfect performance to next (Silver) tier (assuming no challenge failures)
 ```
 
 #### Miner Advancement Program
 The top two (2) performers per batch of `store`, `challenge` or `retrieve` requests will recieve a one-time tier appropriate boost. These tier-specific boosts decrease as you ascend the tier structure, and are defined in `constants.py`. For example:
 
 ```bash
 TIER_BOOSTS = {
     b"Super Saiyan": 1.02, # 2%  -> 1.02
-    b"Diamond": 1.05,      # 5%  -> 0.945
-    b"Gold": 1.1,          # 10% -> 0.88
-    b"Silver": 1.15,       # 15% -> 0.805
+    b"Ruby": 1.04,         # 4%  -> 0.936
+    b"Emerald": 1.05,      # 6%  -> 0.918
+    b"Diamond": 1.08,      # 8%  -> 0.864
+    b"Platinum": 1.1,      # 10% -> 0.825
+    b"Gold": 1.12,         # 12% -> 0.784
+    b"Silver": 1.16,       # 16% -> 0.754
     b"Bronze": 1.2,        # 20% -> 0.72
 }
 ```
 
 Concretely, a `Bronze` miner who is one of the top 2 within a batch of requests will receive a proportionally larger boost than a `Diamond` miner who is also in the top 2.
 
 ```
 REWARD = TIER * REWARD * BOOST
 Bronze  -> 0.72 = 0.6 * 1.0 * 1.2
 Diamond -> 0.84 = 0.8 * 1.0 * 1.05
 ```
 
-This mechansim *significantly* closes the gap for newer miners who perform well and should be able to ascned the tier structure honestly and faithfully.
+This mechanism *significantly* closes the gap for newer miners who perform well and should be able to ascend the tier structure honestly and faithfully. This is such that miners who consistently perform well but are lower tiers can more readily survive immunity period to make it to successively higher tiers and not "gate" access to the older miners. This directly negates the "grandfathering" effect. Higher tier miners that are in the top 2 are boosted significantly less than those Bronze or lower tier miners who make the top 2.
+
 
 #### Periodic Statistics Rollover
 
-Statistics for `store_successes/attempts`, `challenge_attempts/successes`, and `retrieve_attempts/successes` are reset every epoch, while the `total_successes` are carried over for accurate tier computation. This "sliding window" of the previous 360 blocks of `N` successes vs `M` attempts effectively resets the `N / M` ratio and applies Wilson Scoring. This facilitates a less punishing tier calculation for early failures that then have to be "outpaced", while simultaneously discouraging grandfathering in of older miners who were able to succeed early and cement their status in a higher tier. The net effect is greater mobility across the tiers, keeping the network competitive while incentivizing reliability and consistency.
+Statistics for `store_successes/attempts`, `challenge_attempts/successes`, and `retrieve_attempts/successes` are reset every 2 epochs (720 blocks), while the `total_successes` are carried over for accurate tier computation. This "sliding window" of the previous 720 blocks of `N` successes vs `M` attempts effectively resets the `N / M` ratio and applies Wilson Scoring. This facilitates a less punishing tier calculation for early failures that would otherwise have to be "outpaced", while simultaneously discourages grandfathering older miners who were able to succeed early and cemented their status in a higher tier. The net effect is greater mobility across the tiers, keeping the network competitive while incentivizing reliability and consistency.
 
 For example:
 ```bash
 store_successes = 2
 store_attempts = 2
 challenge_successes = 3
 challenge_attempts = 5
 retrieve_successes = 1
 retireve_attempts = 1
-total_successes_epoch = 6
-total_attempts_epoch = 8
-wilson_score = 0.73 # would qualify for Diamond tier this round
+total_successes_epoch = 7
+total_attempts_epoch = 9
+total_successes = 6842
+wilson_score = 0.79
 ```
 
 The scores are then reset, while keeping the total successes for tier recognition:
 ```bash
 store_attempts = 0
 store_successes = 0
 challenge_successes = 0
 challenge_attempts = 0
 retrieve_successes = 0
 retrieve_attempts = 0
-total_successes = 6
+total_successes = 6851 # + 9 by aggregating total successs previous 2 epochs
 ```
 
+> This miner would qualify for Diamond tier this round, as it has passed the minimum threshold for total successes (5000) and wilson score (0.77).
+
 ### Speed and Reliability in Decentralized Storage Mining
 
 In the context of FileTAO's decentralized storage system, speed and reliability are critical factors that significantly influence the performance and reputation of miners. These factors not only affect the efficiency of data storage and retrieval but also play a crucial role in the overall user experience and the robustness of the network.
 
 #### Importance of Speed:
 1. **Quick Data Access:** Fast response times in data storage and retrieval operations are essential for a seamless user experience. Miners with quicker response times enhance the network's ability to serve data efficiently.
 2. **Improved Network Performance:** Speedy processing of tasks contributes to the overall performance of the network, reducing bottlenecks and ensuring smooth data flow.
@@ -781,26 +782,28 @@
 2. **Tier-Based Reward Factors:** Each tier has an associated reward factor, which determines the proportion of rewards received by the miner. Higher tiers, achieved through consistent performance, offer greater rewards. Miner rewards and punishments are symmetrically scaled by their tier. Miners who have a lower tier are penalized proportionally less than miners who have a higher tier. This encourages top miners to have higher Wilson Scores, and allows for lower tier miners the ability to work their way up the ladder.
 
 e.g.
 ```python
 reward = 1.0 * TIER_FACTOR if task_successful else TASK_NEGATIVE_REWARD * TIER_FACTOR
 
 # For Bronze and challenges
-reward = 1.0 * 0.555 if challenge_successful else -0.05 * 0.555
+reward = 1.0 * 0.5 if challenge_successful else -0.05 * 0.5
 reward
-> 0.555 | -0.02775 # lighter punishment for lower tier failure
+> 0.5 | -0.025 # lighter punishment for lower tier failure
 
 # However for Gold
-reward = 1.0 * 0.777 if challenge_successful else -0.05 * 0.777
+reward = 1.0 * 0.7 if challenge_successful else -0.05 * 0.7
 reward
-> 0.777 | -0.03885 # harsher punishment for higher tier failure
+> 0.7 | -0.035 # harsher punishment for higher tier failure
 ```
 
 The tier system in FileTAO's decentralized storage network plays a pivotal role in ensuring the network's efficiency and reliability. By setting clear performance benchmarks and rewarding miners accordingly, the system fosters a competitive yet fair environment. This encourages continuous improvement among miners, ultimately leading to a robust and trustworthy decentralized storage solution.
 
+### Viewing Wandb Runs
+You can view validator provided run data on wandb by viewing the project found at this [link](https://wandb.ai/philanthrope/philanthropic-thunder/table). This provides information on miner statistics and tier level available to the public.
 
 ## Epoch UID selection
 Miners are chosen pseudorandomly using the current block hash as a random seed. This allows for public verification of which miners are selected for each challenge round (3 blocks).
 
 
 For example:
 ```python
@@ -836,56 +839,14 @@
 ```bash
 pm2 start /home/user/storage-subnet/neurons/miner.py --interpreter /home/user/miniconda3/envs/sn21/bin/python --name miner -- --netuid 21 --wandb.off --wallet.name default --wallet.hotkey miner  --axon.port 8888 --logging.debug
 ```
 
 > Make sure to use absolute paths when executing your pm2 command.
 
 
-#### Options
-
-- `--netuid`: Specifies the chain subnet uid. Default: 21.
-- `--miner.name`: Name of the miner, used for organizing logs and data. Default: "core_storage_miner".
-- `--miner.device`: Device to run the miner on, e.g., "cuda" for GPUs or "cpu" for CPU. Default depends on CUDA availability.
-- `--miner.verbose`: Enables verbose logging. Default: False.
-
-- `--database.host`: Hostname of the redis database. Default: "localhost".
-- `--database.port`: Port for the redis database. Default: 6379.
-- `--database.index`: Redis database index. Default: 0.
-- `--database.directory`: Directory to store local data. Default: "~/.data".
-
-- `--miner.set_weights_wait_for_inclusion`: Wether to wait for the set_weights extrinsic to enter a block. Default: False.
-- `--miner.set_weights_wait_for_finalization`: Wether to wait for the set_weights extrinsic to be finalized on the chain. Default: False.
-
-- `--blacklist.blacklist_hotkeys`: List of hotkeys to blacklist. Default: [].
-- `--blacklist.whitelist_hotkeys`: List of hotkeys to whitelist. Default: [].
-- `--blacklist.force_validator_permit`: If True, only allows requests from validators. Default: False.
-- `--blacklist.allow_non_registered`: If True, allows non-registered hotkeys to mine. Default: False.
-- `--blacklist.minimum_stake_requirement`: Minimum stake requirement for participating hotkeys. Default: 0.0.
-- `--blacklist.min_request_period`: Time period (in minutes) to serve a maximum number of requests per hotkey. Default: 5.
-
-- `--miner.priority.default`: Default priority for non-registered requests. Default: 0.0.
-- `--miner.priority.time_stake_multiplicate`: Time (in minutes) to double the importance of stake in the priority queue. Default: 10.
-- `--miner.priority.len_request_timestamps`: Number of historical request timestamps to record. Default: 50.
-
-- `--miner.no_set_weights`: If True, the miner does not set weights on the chain. Default: False.
-- `--miner.no_serve`: If True, the miner does not serve requests. Default: False.
-- `--miner.no_start_axon`: If True, the miner does not start the axon server. Default: False.
-
-- `--miner.mock_subtensor`: If True, uses a mock subtensor for testing. Default: False.
-
-- `--wandb.off`: Disables Weight and Biases logging. Default: False.
-- `--wandb.project_name`: Project name for WandB logging. Default: "philanthropic-thunder".
-- `--wandb.entity`: WandB entity (username or team name) for the run. Default: "philanthrope".
-- `--wandb.offline`: Runs WandB in offline mode. Default: False.
-- `--wandb.weights_step_length`: Steps interval for logging weights to WandB. Default: 10.
-- `--wandb.run_step_length`: Steps interval for a new run rollover in WandB. Default: 1500.
-- `--wandb.notes`: Notes to add to the WandB run. Default: "".
-
-These options allow you to configure the miner's behavior, database connections, blacklist/whitelist settings, priority handling, and integration with monitoring tools like WandB. Adjust these settings based on your mining setup and requirements.
-
 
 #### Data migration
 If for whatever reason you need to migrate the data in your hard drive configured with `--database.directory` to a new directory than is reflected in the Redis index, then you can do it by simply running the script in `scripts/migrate_database_directory.sh`. 
 
 When should you run the migration script?:
 - if you want to specify a different --database.directory
 - if your data has moved but your redis index has not reflected this change
@@ -952,40 +913,14 @@
 For example,
 ```bash
 REBALANCE_SCRIPT_PATH=/home/user/storage-subnet/scripts/rebalance_deregistration.sh
 ```
 
 This way you are able to run your process from anywhere and not rely on relative path resolution to ensure proper functioning of the validator.
 
-#### Options
-
-- `--neuron.name`: Specifies the name of the validator neuron. Default: "core_storage_validator".
-- `--neuron.device`: The device to run the validator on (e.g., "cuda" for GPU, "cpu" for CPU). Default: "cuda" if CUDA is available, else "cpu".
-- `--neuron.curve`: The elliptic curve used for cryptography. Only "P-256" is currently available.
-- `--neuron.maxsize`: The maximum size of random data to store. If `None`, a lognormal random Gaussian distribution is used (default: `None`).
-- `--neuron.min_chunk_size`: The minimum chunk size of random data for challenges. Default: 256.
-- `--neuron.disable_log_rewards`: If set, disables all reward logging to suppress function values from being logged (e.g., to WandB). Default: False.
-- `--neuron.chunk_factor`: The factor to divide data into chunks. Default: 4.
-- `--neuron.num_concurrent_forwards`: The number of concurrent forward requests running at any time. Default: 1.
-- `--neuron.disable_set_weights`: If set, disables setting weights on the chain. Default: False.
-- `--neuron.semaphore_size`: The limit on concurrent asynchronous calls. Default: 256.
-- `--neuron.checkpoint_block_length`: Blocks before a checkpoint is saved. Default: 100.
-- `--neuron.events_retention_size`: File size for retaining event logs (e.g., "2 GB"). Default: "2 GB".
-- `--neuron.dont_save_events`: If set, event logs will not be saved to a file. Default: False.
-- `--neuron.vpermit_tao_limit`: The maximum TAO allowed for querying a validator with a vpermit. Default: 500.
-- `--neuron.verbose`: If set, detailed verbose logs will be printed. Default: False.
-- `--neuron.log_responses`: If set, all responses will be logged. Note: These logs can be extensive. Default: False.
-- `--neuron.data_ttl`: The number of blocks before stored challenge data expires. Default: 50000 (approximately 7 days).
-- `--neuron.profile`: If set, network and I/O actions will be profiled. Default: False.
-
-- `--database.host`: Hostname of the Redis database. Default: "localhost".
-- `--database.port`: Port of the Redis database. Default: 6379.
-- `--database.index`: The database number for the Redis instance. Default: 1.
-
-These options allow you to fine-tune the behavior, storage, and network interaction of the validator neuron. Adjust these settings based on your specific requirements and infrastructure.
 
 > Note: Challenge data lives by default for 5000 blocks in the validator index. This means after 7 days the data is removed and is no longer queried by the validator. This allows miners to recover who have lost challenge data
 
 ### Running the API
 
 Running an API node at `neurons.api.py` allows you to create an entry node into the FileTao network for storing data. This can be connected to a back-end service, or used similarly to an IPFS node as an entrypoint for public use.
 
@@ -1059,28 +994,29 @@
    ```bash
    echo 'export WANDB_API_KEY=your_api_key' >> ~/.bashrc
    source ~/.bashrc
    ```
 
    Replace `your_api_key` with the actual API key. This method automatically authenticates you with wandb every time you open a new terminal session.
 
-#### Tips and Best Practices
-
-- **Security**: Keep your API key confidential. Do not share it or commit it to public repositories.
-- **Troubleshooting**: If you encounter issues, check for common problems like incorrect API key entry or network issues.
-- **Usage in Scripts**: For using WANDB in your Python scripts, refer to the WANDB documentation for proper initialization and usage patterns.
-
-Following these steps, you should be able to successfully log into WANDB and set up your API key on your Ubuntu machine, enabling seamless integration of WANDB in your machine learning workflows.
 
 #### Compute Requirements
 No GPU is currently required to run either a validator or miner. This may change in the future for accelerating the proof and/or verification system.
 
 See [`min_compute.yml`](min_compute.yml) for complete details on minimum and recommended requirements.
 
 
+### Testnet
+FileTao runs a testnet to deploy miners and try out miners on `netuid 22`. 
+
+You can access this testnet by adding these to your script:
+```
+--subtensor.network test --netuid 22
+```
+
 ### Local Subtensor
 
 Availability is *critical* in storage in general and SN21, specifically. The reward mechanism punishes failed challenges and retrievals, even if the reason for that failure is unavailability, not only explicitly incorrect proofs or intentionally malicious behavior. It is possible to experience intermittent connectivity with the free provided endpoints for subtensor connections.
 
 It is *highly* recommended that all miners and validators run their own local subtensor node. This will resolve the many issues commonly found with intermittent connectivity across all subnets.
 
 To start your miner/validator using your local node, include the flag `--subtensor.network local` into your startup parameters.
@@ -1224,7 +1160,41 @@
 This will remove the `save` argument for RDB in the `etc/reids/redis.conf` file. 
 
 Please ensure to path the path to your redis.conf file if it is differen from the default:
 ```bash
 REDIS_PATH="/path/to/redis.conf"
 bash ./scripts/redis/disable_rdb.sh $REDIS_PATH
 ```
+
+
+## FileTAO Docker
+
+FileTao is now able to run with docker with miner, validator, and api nodes. If running a validator, API nodes are *automatically* deployed in a separate container.
+
+You are free to use this provided docker convenience but may still run nodes on bare-metal. However, it is recommended to upgrade to build and use these docker images, as they are generally more secure and convenient to use.
+
+### Run filetao with docker
+
+To run the suite of services (miner, validator, and redis), first run:
+
+```sh
+cp example.env .env
+```
+
+and populate the environment variables as appropriate. Ensure that each node has its own wallet, and is registered on SN21.
+
+To run the entire stack, use the following commands:
+
+```sh
+docker-compose build
+docker-compose up
+```
+
+To run only an individual service (e.g. miner and validator), use:
+
+```
+docker compose up --build {filetao-miner, filetao-validator}
+```
+
+### Demo notebooks and examples
+
+See [`storage/api/demo_notebook.ipynb`]("docs/api_demo.ipynb") and [`storage/api/example.py`]("storage/api/example.py") To learn different ways to query the subnet.
```

### Comparing `FileTAO-2.1.0/FileTAO.egg-info/SOURCES.txt` & `FileTAO-3.0.0/FileTAO.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,26 +11,32 @@
 neurons/api.py
 neurons/miner.py
 neurons/validator.py
 storage/__init__.py
 storage/constants.py
 storage/protocol.py
 storage/api/__init__.py
+storage/api/base.py
+storage/api/delete_api.py
 storage/api/example.py
 storage/api/retrieve_api.py
 storage/api/store_api.py
 storage/api/utils.py
 storage/cli/__init__.py
 storage/cli/cli.py
 storage/cli/default_values.py
 storage/cli/listcommand.py
 storage/cli/neuroncommand.py
 storage/cli/retrievecommand.py
 storage/cli/statscommand.py
 storage/cli/storecommand.py
+storage/indexer/__init__.py
+storage/indexer/endpoint.py
+storage/indexer/redis.py
+storage/indexer/sqlite.py
 storage/miner/__init__.py
 storage/miner/config.py
 storage/miner/database.py
 storage/miner/run.py
 storage/miner/set_weights.py
 storage/miner/utils.py
 storage/plot/__init__.py
@@ -44,14 +50,15 @@
 storage/shared/weights.py
 storage/validator/__init__.py
 storage/validator/bonding.py
 storage/validator/challenge.py
 storage/validator/cid.py
 storage/validator/config.py
 storage/validator/database.py
+storage/validator/dendrite.py
 storage/validator/distribute.py
 storage/validator/encryption.py
 storage/validator/event.py
 storage/validator/forward.py
 storage/validator/network.py
 storage/validator/rebalance.py
 storage/validator/retrieve.py
```

### Comparing `FileTAO-2.1.0/LICENSE` & `FileTAO-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/PKG-INFO` & `FileTAO-3.0.0/FileTAO.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,55 @@
 Metadata-Version: 2.1
 Name: FileTAO
-Version: 2.1.0
+Version: 3.0.0
 Summary: Philanthropic storage for the masses. (FileTAO)
 Home-page: https://github.com/ifrit98/storage-subnet
 Author: philanthrope
 Author-email: ifrit98@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<3.12
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: torch>=1.13.0
+Requires-Dist: bcrypt==3.2.0
+Requires-Dist: bittensor==6.11.0
+Requires-Dist: redis==5.0.1
+Requires-Dist: pycryptodome==3.20.0
+Requires-Dist: pyinstrument==4.6.1
+Requires-Dist: wandb==0.16.0
+Requires-Dist: morphys==1.0
+Requires-Dist: py-multibase==1.0.3
+Requires-Dist: py-multicodec==0.2.1
+Requires-Dist: py-multihash==2.0.1
+Requires-Dist: ipfs-cid==1.0.0
+Requires-Dist: python-jose==3.3.0
+Requires-Dist: passlib==1.7.4
+Requires-Dist: python-multipart==0.0.9
+Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: loguru==0.7.0
+Requires-Dist: pandas==2.2.0
+Provides-Extra: dev
+Requires-Dist: pytest==7.4.3; extra == "dev"
+Requires-Dist: pytest-cov==4.1.0; extra == "dev"
+Requires-Dist: parameterized==0.9.0; extra == "dev"
+Requires-Dist: flake8==7.0.0; extra == "dev"
 
 # FileTAO
 
 [![Latest Version](https://img.shields.io/pypi/v/filetao.svg)](https://pypi.org/project/filetao/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/filetao)](https://pypi.org/project/filetao)
 [![License](https://img.shields.io/pypi/l/filetao.svg)](https://github.com/ifrit98/storage-subnet/blob/master/LICENSE)
 
@@ -34,15 +57,15 @@
 
 FileTAO (Bittensor Subnet 21) implements a novel, multi-layered zero-knowledge interactive proof-of-spacetime algorithm by cleverly using Pedersen commitments, random challenges leveraging elliptic curve cryptography, sequential seed-based chained hash verification, and merkle proofs to achieve an efficient, robust, secure, and highly available decetralized storage system on the Bittensor network. The system validates on encrypted user data, such that miners are unaware of what data they are storing, and only end-users may encrypt/decrypt the data they provide with their bittensor wallet coldkey.
 
 We consider this system to be an important stepping stone so that bittensor can fulfill its mission of democratizing intelligence, and a decentralized AWS platform is a key brick in this wall. 
 
 **NOTICE**: Using this software, you **must** agree to the Terms and Agreements provided in the [terms and conditions](TERMS.md) document. By downloading and running this software, you implicitly agree to these terms and conditions.
 
-Currently supporting `python>=3.9,<3.11`.
+Currently supporting `python>=3.9,<3.12`.
 
 > Note: The storage subnet is in an alpha stage and is subject to rapid development.
 
 # Table of Contents for Subnet 21 (FileTAO)
 1. [FileTAO Overview](#filetao)
 2. [Installation](#installation)
    - [Install Redis](#install-redis)
@@ -75,28 +98,36 @@
    - [Advanced Cryptographic Techniques](#advanced-cryptographic-techniques)
    - [User-Centric Approach](#user-centric-approach)
 7. [Zero Knowledge Proof-of-Spacetime](#zero-knowledge-proof-of-spacetime)
    - [Storage Phase](#storage-phase)
    - [Challenge Phase](#challenge-phase)
    - [Retrieval Phase](#retrieval-phase)
 8. [Reward System](#reward-system)
+   - [Overview and Justification](#overview-and-justification)
    - [Speed and Reliability in Decentralized Storage Mining](#speed-and-reliability-in-decentralized-storage-mining)
+   - [Viewing Wandb Runs](#viewing-wandb-runs)
 9. [Epoch UID Selection](#epoch-uid-selection)
 10. [Running FileTAO](#running-filetao)
     - [Running a Miner](#running-a-miner)
     - [Running a Validator](#running-a-validator)
     - [Running the API](#running-the-api)
     - [Setup WandB](#setup-wandb)
+    - [Testnet](#testnet)
 11. [Local Subtensor](#local-subtensor)
 12. [Database Schema Migration](#database-schema-migration)
 13. [Disable RDB](#disable-rdb)
-
+14. [FileTAO Docker](#filetao-docker)
+15. [Demos](#demo-notebooks-and-examples)
 
 ## Installation
 ```bash
+# Please install torch-cpu if you do not need a gpu. (GPU not required for FileTAO)
+pip install torch==2.3.0+cpu -f https://download.pytorch.org/whl/torch_stable.html
+
+# Clone and Install the FileTAO repo.
 git clone https://github.com/ifrit98/storage-subnet
 cd storage-subnet
 python -m pip install -e .
 ```
 
 ### Install Redis
 Install Redis on your host system.
@@ -139,41 +170,19 @@
 Nov 16 22:35:42 user systemd[1]: Started Advanced key-value store.
 ```
 
 ### Secure Redis Configuration
 
 In order to securely run a node, whether a miner or validator, you must run ensure your redis instance is secure from the outside internet and is password-protected.
 
-The following steps are **mandatory** for secure communication on the network:
+The following steps are **recommended** for secure communication on the network and data integrity:
 
-1. Closing the default redis port
 1. Password protecting redis
-1. Enabling persistence
+1. Enabling redis persistence
 
-#### Close external traffic to Redis 
-
-> Note: **EXPOSING THE REDIS PORT IS A MAJOR SECURITY RISK**
-
-This Bash script is designed to configure UFW (Uncomplicated Firewall) to manage access to default Redis port 6379. The script's primary function is to block all external traffic to port 6379, typically used by Redis, while allowing local processes to still access this port.
-
-##### Usage
-To run the script, use the following command in the terminal:
-```bash
-sudo ./scripts/redis/create_redis_firewall.sh
-```
-Running this script will:
-- Check if UFW is installed and active. If UFW is not active, the script will attempt to enable it.
-- Set UFW rules to deny all external access to port 6379.
-- Set UFW rules to allow all local access to port 6379.
-- Apply the changes by reloading UFW.
-
-##### Important Considerations
-- **Test Before Production**: Always test the script in a controlled environment before deploying it in a production setting.
-- **Existing Rules**: If there are existing rules for port 6379, review the script to ensure compatibility.
-- **Firewall Management**: This script is specifically for systems using UFW. If another firewall management tool is in use, this script will not be compatible.
 
 #### Automated Redis Password Configuration
 To enhance security, our system now automatically generates a strong password for Redis. This is **REQUIRED**. This is handled by the `set_redis_password.sh` script. Follow these steps to set up Redis with an automated password:
 
 1. **Run the Redis Start Script**: 
     ```bash
     bash scripts/redis/set_redis_password.sh
@@ -266,22 +275,22 @@
 from storage.api import store, retrieve
 
 # Store data
 wallet = bt.wallet()
 subtensor = bt.subtensor()
 
 data = b"Some bytestring data!"
-cid, hotkeys = await store(data, wallet, subtensor, netuid=22)
+cid, hotkeys = await store(data, wallet, subtensor, netuid=21)
 print("Stored {} with {} hotkeys".format(cid, hotkeys))
 > Stored bafkreid6mhmfptdpfvljyavss77zmo6b2oert2pula2gy4tosekupm4nqa with validator hotkeys [5CaFuijc2ucdoWhkjLaYgnzYrpv62KGt1fWWtUxhFHXPA3KK, 5FKwbwguHU1SVQiGot5YKSTQ6fWGVv2wRHFrWfwp9X9nWbyU]
 ```
 
 Now you can retrieve the data using the content identifier `CID` and the `hotkey`s directly:
 ```python
-data = await retrieve(cid, wallet, subtensor, netuid=22, hotkeys=hotkeys)
+data = await retrieve(cid, wallet, subtensor, netuid=21, hotkeys=hotkeys)
 print(data)
 > b"Some bytestring data!"
 ```
 
 ### Using SubnetsAPI 
 In addition to the convenience wrappers and command-line interface, FileTao can be accessed via the bittensor subnets python API.
 
@@ -615,153 +624,194 @@
 In each phase, cryptographic primitives ensure data integrity and confidentiality. The encryption and commitment schemes ensure the data's security, while Merkle trees and random challenges provide a robust method for verifying data possession without revealing the actual data.
 
 In each phase, cryptographic primitives like hashing, commitment schemes (e.g., Elliptic Curve Cryptography and Pedersen commitments), and data structures like Merkle trees are employed to ensure the integrity, confidentiality, and availability of the data. The use of seeds and randomness in commitments adds an additional layer of security and ensures that each instance of data storage and retrieval is unique and verifiable. See [here](https://kndrck.co/posts/efficient-merkletrees-zk-proofs/) for more information.
 
 
 ## Reward System
 
+There are several components to the reward mechanism and is multi-layered. In a nutshell, the goals are as follows:
+
+- Incentivize data durability and salience via cryptographic proof system. (E.g. don't lose data.)
+- Incentivize good performance over a long period of time. (Tier system to reward based on reputation.)
+- Incentivize fast response times. We want to retrieve user data quickly and ensure that it is over high network bandwidth.
+
 In FileTAO's decentralized storage system, optimal behavior is crucial for the overall health and efficiency of the network. Miners play a vital role in maintaining this ecosystem, and their actions directly impact their rewards and standing within the subnet. We have implemented a tier-based reward system to encourage proper behavior, successful challenge completions, and consistent performance.
 
 Failing to pass either challenge or retrieval verifications incur negative rewards. This is doubly destructive, as rolling statistics are continuously logged to periodically compute which tier a given miner hotkey belongs to. When a miner achieves the threshold for the next tier, the rewards that miner receives proportionally increase. Conversely, when a miner drops below the threshold of the previous tier, that miner's rewards are slashed such that they receive rewards proportionally to the immediately lower tier.
 
+### Overview and Justification
+FileTAO's Multi-dimensional reward mechanism is spread across 4 main axes:
+(1) Availability: Is the miner reachable when requested? Incentivizes uptime.
+(2) Speed (performant): how fast was the normalized response time?
+(3) Correctness (reliable): did the proof succeed? y/n
+(4) Trustworthiness (correctness over time): Tier definitions encapsulate consistenty and trustworthiness over time. A miner that rarely fails challenges and faithfully returns data when requested will receive an initial higher proportional reward.
+
+The main drivers behind the reward mechanism are to model meritocratic systems as seen in the academic realm and in the business world that scales trust across time and observation of output. For example, we create various "tiers" in education, Undergraduate, Masters, PhD, Post Doc, or in software, Junior Engineer, Senior Engineer, Principal Engineer, Staff Engineer, etc where each subsequent level achieved has proportionally greater expecetations on performance and qualification of the individual. 
+
+However, performance of the individual must match the expectations of the pedigree, and behavior that is inconsistent with a given level will be adjusted. If, for example, a Junior Engineer proves their output is substantial and over time completes projects that provide value, that engineer will be promoted to Senior Engineer over time, and pontentially beyond. Conversely, a Principal Engineer that consistently underperforms expectations will be demoted to a role with lower expectations until able to prove otherwise. The same logic applies to miners in FileTAO (SN21).
+
+Tier (class) mobility is at the heart of the mechanism, and provides a balance between competition and trust, where over time competitiveness breeds a degree of trust on which we can associate a degree of reliability with a given entity (or miner).
+
 **Why Optimal Behavior Matters:**
 1. **Reliability:** Miners who consistently store, retrieve, and pass challenges with high Wilson Scores ensure the reliability and integrity of the network.
 2. **Trust:** High-performing miners build trust in the network, attracting more users and increasing the overall value of the system.
 3. **Efficiency:** Optimal behavior leads to a more efficient network, reducing the likelihood of data loss and ensuring fast, reliable access to stored information.
 
 **Tier-Based Reward System:**
 - **Tiers:** We classify miners into four tiers – Diamond, Gold, Silver, and Bronze – based on their performance metrics.
 - **Performance Metrics:** These include the Wilson Score in storage, retrieval, and challenge tasks, as well as the total number of successful operations.
 - **Higher Rewards for Higher Tiers:** Miners in higher tiers receive a greater proportion of the rewards, reflecting their superior performance and contribution to the network.
 
 ### **Wilson Score**
-A measure of confidence is required to assess reliability in low sample environments. For miners who have less history, it is unfair to expect perfection early on and is account for by using a statistical tool, the `Wilson Score`. 
+
+A measure of confidence is required to assess reliability in low sample environments. For miners who have less history, it is unfair to expect perfection early on and is account for by using a statistical tool, the `Wilson Score`. An asymmetric approximation of the confidence interval suited for low sample sizes given a particular z-score target, the `Wilson score` doesn't suffer from problems of overshoot and zero-width intervals that afflict the normal interval approximation.
+
+See: https://en.wikipedia.org/wiki/Binomial_proportion_confidence_interval#Wilson_score_interval for more information.
 
 For example, if a miner succeeds 4/5 times, it has a success rate of 80%. However it may not be indicative of true performance and reliability. Thus we have added Wilson Scores to accomodate low sample populations to get a more balanced approach to scoring miners.
 
 This effectively allows for forgiveness for early failures and facilitates miners who are faithful actors to still rise through the tier system without being perpetually punished for early mistakes or poor optimization.
 
 The equivalent wilson score for 4 of 5 attempts is `0.77`, which indicates with 95% statistical confidence that this miner is AT least this successful 80% of the time. Functionally, this allows for lowering of the tier requirements while having statistical confidence that over time, the miner may continue to improve performance from there while being considered reliable.
 
-**Moving Up Tiers:**
-- To ascend to a higher tier, a miner must maintain high Wilson Scores and achieve a set number of total successes.
-- This progression system incentivizes continuous improvement and excellence in mining operations.
-
-**Graphical Representation:**
-- The graph below illustrates how rewards increase as miners advance through the tiers. It visually represents the potential growth in earnings as miners optimize their operations and maintain high standards of performance.
-
-<div align="center">
-   <img src="assets/reward-tiers-vert.png" alt="Bonding Curves" width="650"/>
-</div>
+More concretely, given `N` trials, the wilson score establishes a lower bound for the confidence interval on miner success rates given low sample or population sizes. E.g., if a miner responds successfuly 8 of 9 times, it's lower bound on success rate is roughly `0.8701769999681506`. In other words, `wilson_score(8,9) == 0.8701769999681506`, suggesting that 87% of the time, this miner is expected to succeed on average. 
+
+This calculation is used as the lower bound to determine tier eligibility and establishes a "minimium trust level" for the miner. If a miner continues to have failed challenges, the wilson score lower bound will cross below the current tier threshold, and when the tiers are recalculated, that miner will move down a tier (e.g. `Diamond -> Gold`.)
+
+### **monitor**
+Miners are also incentivized to be available, and are punshed for not being online, (e.g. failed `n` pings) by the `monitor` protocol. Periodically (every `m` steps) validators ping a set of `k` miners (default is 40), and after 5 successive failed attempts to ping a specific UID, that miner will be negatively rewarded for unavailability.
 
-#### Tier System:
+### Tier System:
 The tier system classifies miners into five distinct categories, each with specific requirements and storage limits. These tiers are designed to reward miners based on their performance, reliability, and the total volume of data they can store.
 
 Importance of Tier System:
 - **Encourages High Performance:** Higher tiers reward miners with greater benefits, motivating them to maintain high Wilson Scores.
 - **Enhances Network Reliability:** The tier system ensures that only the most reliable and efficient miners handle significant volumes of data, enhancing the overall reliability of the network.
 - **Fair Reward Distribution:** The reward factors are proportional to the miners' tier, ensuring a fair distribution of rewards based on performance.
 
 1. 🎇 **Super Saiyan Tier:** 
-   - **Storage Limit:** 1 Exabyte (EB)
-   - **Store Wilson Score:** 0.88
-   - **Minimum Successes Required:** 10,000
+   - **Storage Limit:** 50 Petabytes (PB)
+   - **Store Wilson Score:** 0.9
+   - **Minimum Successes Required:** 15,000
    - **Reward Factor:** 1.0 (100% rewards)
 
-2. 💎 **Diamond Tier:**
-   - **Storage Limit:** 1 Petabyte (PB)
-   - **Store Wilson Score:**  0.77
-   - **Minimum Successes Required:** 5,000
-   - **Reward Factor:** 0.9 (90% rewards)
-
-3. 🥇 **Gold Tier:**
-   - **Storage Limit:** 100 Terabytes (TB)
-   - **Store Wilson Score:** 0.66
-   - **Minimum Successes Required:** 2,000
+2. 🌹 **Ruby Tier**
+   - **Storage Limit:** 20 Petabytes (PB)
+   - **Store Wilson Score:** 0.85
+   - **Minimum Successes Required:** 10,000
+   - **Rewrd Factor:** 0.9 (90% rewards)
+
+3. 🔮 **Emerald Tier**
+   - **Storage Limit:** 10 Petabytes (PB)
+   - **Store Wilson Score:** 0.8
+   - **Minimum Successes Required:** 8,000
+   - **Rewrd Factor:** 0.85 (85% rewards)
+
+4. 💠 **Diamond Tier:**
+   - **Storage Limit:** 5 Petabytes (PB)
+   - **Store Wilson Score:**  0.75
+   - **Minimum Successes Required:** 6,000
    - **Reward Factor:** 0.8 (80% rewards)
 
-4. 🥈 **Silver Tier:**
-   - **Storage Limit:** 10 Terabytes (TB)
-   - **Store Wilson Score:** 0.55
-   - **Minimum Successes Required:** 1,000
+5. 🔗 **Platinum Tier**
+   - **Storage Limit:** 1 Petabyte (PB)
+   - **Store Wilson Score:** 0.65
+   - **Minimum Successes Required:** 4,000
+   - **Reward Factor:** 0.75 (75% rewards) 
+
+6. 🥇 **Gold Tier:**
+   - **Storage Limit:** 200 Terabytes (TB)
+   - **Store Wilson Score:** 0.65
+   - **Minimum Successes Required:** 2,000
    - **Reward Factor:** 0.7 (70% rewards)
 
-5. 🥉 **Bronze Tier:**
-   - **Storage Limit:** 1 Terabyte (TB)
+7. 🥈 **Silver Tier:**
+   - **Storage Limit:** 50 Terabytes (TB)
+   - **Store Wilson Score:** 0.6
+   - **Minimum Successes Required:** 500
+   - **Reward Factor:** 0.65 (65% rewards)
+
+8. 🥉 **Bronze Tier:**
+   - **Storage Limit:** 10 Terabytes (TB)
    - **Store Wilson Score:** Not specifically defined for this tier
    - **Minimum Successes Required:** Not specifically defined for this tier
    - **Reward Factor:** 0.6 (60% rewards)
 
 #### Maintaining and Advancing Tiers:
 - To advance to a higher tier, miners must consistently achieve the required minimum Wilson Scores in their operations.
-- Periodic evaluations are conducted to ensure miners maintain the necessary performance standards to stay in their respective tiers.
-- Advancing to a higher tier takes time. In order to ascend to the first higher tier (Silver), it takes at least 1000 successful requests, whether they are challenge requests, store requests, or retry requests and must maintain a 95% Wilson Score in all categories. 
-- Depending on how often a miner is queried, how many validators are operating at one given time, and primarily the performance of the miner, this can take several hours to several days. Assuming full 64 validator slots are occupied, this should take a matter of hours.
+- Periodic evaluations are conducted to ensure miners maintain the necessary performance standards to stay in their respective tiers, or move up or down tiers.
+- Advancing to a higher tier takes time. In order to ascend to the first higher tier (Silver), it takes at least 1000 successful requests, whether they are challenge requests, store requests, or retry requests and must maintain the minimum Wilson Score for successes / attempts. 
+- Depending on how often a miner is queried, how many validators are operating at one given time, and primarily the performance of the miner, this can take several hours to several days. Assuming full 64 validator slots are occupied, this should take ~100 hours.
 
-Here is a distribution of UIDs queried over 1000 blocks based on block hash:
-![uid-dist](assets/uid_dist.png)
+As miners move up tiers, their responsibility increases proportionally. Thus, miners who move from Silver -> Gold are expected to be able to store up to 200 Terabytes (TB) of data, a 4x the storage cap for Silver. Similarly, it must maintain a minimum wilson score of 0.66 over it's lifetime, increasing the lower bound for expected performance and reliability. It also means that this miner will now receive a higher percentage of rewards for each successful query, going from 65% -> 70%. This does not mean that the miner may rest on its laurels, and may move right back down a tier (or more) if it does not meed the minimum requirements for Gold.
 
 Assuming perfect performance, that out of ~200 miner UIDs, each of which is queried roughly 34 times every 1000 rounds, namely a 3.4% chance every query round, one can expect to reach the next tier within 
-
 ```bash
-hours = total_successes / prob_of_query_per_round * time_per_round / 3600
-hours = 98 # roughly 4 days at perfect performance to top tier (no challenge failures)
+hours = total_successes / prob_of_query_per_round * time_per_round / 3600 / num_active_validators
+hours = 4.9 # roughly 5 hours at perfect performance to next (Silver) tier (assuming no challenge failures)
 ```
 
 #### Miner Advancement Program
 The top two (2) performers per batch of `store`, `challenge` or `retrieve` requests will recieve a one-time tier appropriate boost. These tier-specific boosts decrease as you ascend the tier structure, and are defined in `constants.py`. For example:
 
 ```bash
 TIER_BOOSTS = {
     b"Super Saiyan": 1.02, # 2%  -> 1.02
-    b"Diamond": 1.05,      # 5%  -> 0.945
-    b"Gold": 1.1,          # 10% -> 0.88
-    b"Silver": 1.15,       # 15% -> 0.805
+    b"Ruby": 1.04,         # 4%  -> 0.936
+    b"Emerald": 1.05,      # 6%  -> 0.918
+    b"Diamond": 1.08,      # 8%  -> 0.864
+    b"Platinum": 1.1,      # 10% -> 0.825
+    b"Gold": 1.12,         # 12% -> 0.784
+    b"Silver": 1.16,       # 16% -> 0.754
     b"Bronze": 1.2,        # 20% -> 0.72
 }
 ```
 
 Concretely, a `Bronze` miner who is one of the top 2 within a batch of requests will receive a proportionally larger boost than a `Diamond` miner who is also in the top 2.
 
 ```
 REWARD = TIER * REWARD * BOOST
 Bronze  -> 0.72 = 0.6 * 1.0 * 1.2
 Diamond -> 0.84 = 0.8 * 1.0 * 1.05
 ```
 
-This mechansim *significantly* closes the gap for newer miners who perform well and should be able to ascned the tier structure honestly and faithfully.
+This mechanism *significantly* closes the gap for newer miners who perform well and should be able to ascend the tier structure honestly and faithfully. This is such that miners who consistently perform well but are lower tiers can more readily survive immunity period to make it to successively higher tiers and not "gate" access to the older miners. This directly negates the "grandfathering" effect. Higher tier miners that are in the top 2 are boosted significantly less than those Bronze or lower tier miners who make the top 2.
+
 
 #### Periodic Statistics Rollover
 
-Statistics for `store_successes/attempts`, `challenge_attempts/successes`, and `retrieve_attempts/successes` are reset every epoch, while the `total_successes` are carried over for accurate tier computation. This "sliding window" of the previous 360 blocks of `N` successes vs `M` attempts effectively resets the `N / M` ratio and applies Wilson Scoring. This facilitates a less punishing tier calculation for early failures that then have to be "outpaced", while simultaneously discouraging grandfathering in of older miners who were able to succeed early and cement their status in a higher tier. The net effect is greater mobility across the tiers, keeping the network competitive while incentivizing reliability and consistency.
+Statistics for `store_successes/attempts`, `challenge_attempts/successes`, and `retrieve_attempts/successes` are reset every 2 epochs (720 blocks), while the `total_successes` are carried over for accurate tier computation. This "sliding window" of the previous 720 blocks of `N` successes vs `M` attempts effectively resets the `N / M` ratio and applies Wilson Scoring. This facilitates a less punishing tier calculation for early failures that would otherwise have to be "outpaced", while simultaneously discourages grandfathering older miners who were able to succeed early and cemented their status in a higher tier. The net effect is greater mobility across the tiers, keeping the network competitive while incentivizing reliability and consistency.
 
 For example:
 ```bash
 store_successes = 2
 store_attempts = 2
 challenge_successes = 3
 challenge_attempts = 5
 retrieve_successes = 1
 retireve_attempts = 1
-total_successes_epoch = 6
-total_attempts_epoch = 8
-wilson_score = 0.73 # would qualify for Diamond tier this round
+total_successes_epoch = 7
+total_attempts_epoch = 9
+total_successes = 6842
+wilson_score = 0.79
 ```
 
 The scores are then reset, while keeping the total successes for tier recognition:
 ```bash
 store_attempts = 0
 store_successes = 0
 challenge_successes = 0
 challenge_attempts = 0
 retrieve_successes = 0
 retrieve_attempts = 0
-total_successes = 6
+total_successes = 6851 # + 9 by aggregating total successs previous 2 epochs
 ```
 
+> This miner would qualify for Diamond tier this round, as it has passed the minimum threshold for total successes (5000) and wilson score (0.77).
+
 ### Speed and Reliability in Decentralized Storage Mining
 
 In the context of FileTAO's decentralized storage system, speed and reliability are critical factors that significantly influence the performance and reputation of miners. These factors not only affect the efficiency of data storage and retrieval but also play a crucial role in the overall user experience and the robustness of the network.
 
 #### Importance of Speed:
 1. **Quick Data Access:** Fast response times in data storage and retrieval operations are essential for a seamless user experience. Miners with quicker response times enhance the network's ability to serve data efficiently.
 2. **Improved Network Performance:** Speedy processing of tasks contributes to the overall performance of the network, reducing bottlenecks and ensuring smooth data flow.
@@ -781,26 +831,28 @@
 2. **Tier-Based Reward Factors:** Each tier has an associated reward factor, which determines the proportion of rewards received by the miner. Higher tiers, achieved through consistent performance, offer greater rewards. Miner rewards and punishments are symmetrically scaled by their tier. Miners who have a lower tier are penalized proportionally less than miners who have a higher tier. This encourages top miners to have higher Wilson Scores, and allows for lower tier miners the ability to work their way up the ladder.
 
 e.g.
 ```python
 reward = 1.0 * TIER_FACTOR if task_successful else TASK_NEGATIVE_REWARD * TIER_FACTOR
 
 # For Bronze and challenges
-reward = 1.0 * 0.555 if challenge_successful else -0.05 * 0.555
+reward = 1.0 * 0.5 if challenge_successful else -0.05 * 0.5
 reward
-> 0.555 | -0.02775 # lighter punishment for lower tier failure
+> 0.5 | -0.025 # lighter punishment for lower tier failure
 
 # However for Gold
-reward = 1.0 * 0.777 if challenge_successful else -0.05 * 0.777
+reward = 1.0 * 0.7 if challenge_successful else -0.05 * 0.7
 reward
-> 0.777 | -0.03885 # harsher punishment for higher tier failure
+> 0.7 | -0.035 # harsher punishment for higher tier failure
 ```
 
 The tier system in FileTAO's decentralized storage network plays a pivotal role in ensuring the network's efficiency and reliability. By setting clear performance benchmarks and rewarding miners accordingly, the system fosters a competitive yet fair environment. This encourages continuous improvement among miners, ultimately leading to a robust and trustworthy decentralized storage solution.
 
+### Viewing Wandb Runs
+You can view validator provided run data on wandb by viewing the project found at this [link](https://wandb.ai/philanthrope/philanthropic-thunder/table). This provides information on miner statistics and tier level available to the public.
 
 ## Epoch UID selection
 Miners are chosen pseudorandomly using the current block hash as a random seed. This allows for public verification of which miners are selected for each challenge round (3 blocks).
 
 
 For example:
 ```python
@@ -836,56 +888,14 @@
 ```bash
 pm2 start /home/user/storage-subnet/neurons/miner.py --interpreter /home/user/miniconda3/envs/sn21/bin/python --name miner -- --netuid 21 --wandb.off --wallet.name default --wallet.hotkey miner  --axon.port 8888 --logging.debug
 ```
 
 > Make sure to use absolute paths when executing your pm2 command.
 
 
-#### Options
-
-- `--netuid`: Specifies the chain subnet uid. Default: 21.
-- `--miner.name`: Name of the miner, used for organizing logs and data. Default: "core_storage_miner".
-- `--miner.device`: Device to run the miner on, e.g., "cuda" for GPUs or "cpu" for CPU. Default depends on CUDA availability.
-- `--miner.verbose`: Enables verbose logging. Default: False.
-
-- `--database.host`: Hostname of the redis database. Default: "localhost".
-- `--database.port`: Port for the redis database. Default: 6379.
-- `--database.index`: Redis database index. Default: 0.
-- `--database.directory`: Directory to store local data. Default: "~/.data".
-
-- `--miner.set_weights_wait_for_inclusion`: Wether to wait for the set_weights extrinsic to enter a block. Default: False.
-- `--miner.set_weights_wait_for_finalization`: Wether to wait for the set_weights extrinsic to be finalized on the chain. Default: False.
-
-- `--blacklist.blacklist_hotkeys`: List of hotkeys to blacklist. Default: [].
-- `--blacklist.whitelist_hotkeys`: List of hotkeys to whitelist. Default: [].
-- `--blacklist.force_validator_permit`: If True, only allows requests from validators. Default: False.
-- `--blacklist.allow_non_registered`: If True, allows non-registered hotkeys to mine. Default: False.
-- `--blacklist.minimum_stake_requirement`: Minimum stake requirement for participating hotkeys. Default: 0.0.
-- `--blacklist.min_request_period`: Time period (in minutes) to serve a maximum number of requests per hotkey. Default: 5.
-
-- `--miner.priority.default`: Default priority for non-registered requests. Default: 0.0.
-- `--miner.priority.time_stake_multiplicate`: Time (in minutes) to double the importance of stake in the priority queue. Default: 10.
-- `--miner.priority.len_request_timestamps`: Number of historical request timestamps to record. Default: 50.
-
-- `--miner.no_set_weights`: If True, the miner does not set weights on the chain. Default: False.
-- `--miner.no_serve`: If True, the miner does not serve requests. Default: False.
-- `--miner.no_start_axon`: If True, the miner does not start the axon server. Default: False.
-
-- `--miner.mock_subtensor`: If True, uses a mock subtensor for testing. Default: False.
-
-- `--wandb.off`: Disables Weight and Biases logging. Default: False.
-- `--wandb.project_name`: Project name for WandB logging. Default: "philanthropic-thunder".
-- `--wandb.entity`: WandB entity (username or team name) for the run. Default: "philanthrope".
-- `--wandb.offline`: Runs WandB in offline mode. Default: False.
-- `--wandb.weights_step_length`: Steps interval for logging weights to WandB. Default: 10.
-- `--wandb.run_step_length`: Steps interval for a new run rollover in WandB. Default: 1500.
-- `--wandb.notes`: Notes to add to the WandB run. Default: "".
-
-These options allow you to configure the miner's behavior, database connections, blacklist/whitelist settings, priority handling, and integration with monitoring tools like WandB. Adjust these settings based on your mining setup and requirements.
-
 
 #### Data migration
 If for whatever reason you need to migrate the data in your hard drive configured with `--database.directory` to a new directory than is reflected in the Redis index, then you can do it by simply running the script in `scripts/migrate_database_directory.sh`. 
 
 When should you run the migration script?:
 - if you want to specify a different --database.directory
 - if your data has moved but your redis index has not reflected this change
@@ -952,40 +962,14 @@
 For example,
 ```bash
 REBALANCE_SCRIPT_PATH=/home/user/storage-subnet/scripts/rebalance_deregistration.sh
 ```
 
 This way you are able to run your process from anywhere and not rely on relative path resolution to ensure proper functioning of the validator.
 
-#### Options
-
-- `--neuron.name`: Specifies the name of the validator neuron. Default: "core_storage_validator".
-- `--neuron.device`: The device to run the validator on (e.g., "cuda" for GPU, "cpu" for CPU). Default: "cuda" if CUDA is available, else "cpu".
-- `--neuron.curve`: The elliptic curve used for cryptography. Only "P-256" is currently available.
-- `--neuron.maxsize`: The maximum size of random data to store. If `None`, a lognormal random Gaussian distribution is used (default: `None`).
-- `--neuron.min_chunk_size`: The minimum chunk size of random data for challenges. Default: 256.
-- `--neuron.disable_log_rewards`: If set, disables all reward logging to suppress function values from being logged (e.g., to WandB). Default: False.
-- `--neuron.chunk_factor`: The factor to divide data into chunks. Default: 4.
-- `--neuron.num_concurrent_forwards`: The number of concurrent forward requests running at any time. Default: 1.
-- `--neuron.disable_set_weights`: If set, disables setting weights on the chain. Default: False.
-- `--neuron.semaphore_size`: The limit on concurrent asynchronous calls. Default: 256.
-- `--neuron.checkpoint_block_length`: Blocks before a checkpoint is saved. Default: 100.
-- `--neuron.events_retention_size`: File size for retaining event logs (e.g., "2 GB"). Default: "2 GB".
-- `--neuron.dont_save_events`: If set, event logs will not be saved to a file. Default: False.
-- `--neuron.vpermit_tao_limit`: The maximum TAO allowed for querying a validator with a vpermit. Default: 500.
-- `--neuron.verbose`: If set, detailed verbose logs will be printed. Default: False.
-- `--neuron.log_responses`: If set, all responses will be logged. Note: These logs can be extensive. Default: False.
-- `--neuron.data_ttl`: The number of blocks before stored challenge data expires. Default: 50000 (approximately 7 days).
-- `--neuron.profile`: If set, network and I/O actions will be profiled. Default: False.
-
-- `--database.host`: Hostname of the Redis database. Default: "localhost".
-- `--database.port`: Port of the Redis database. Default: 6379.
-- `--database.index`: The database number for the Redis instance. Default: 1.
-
-These options allow you to fine-tune the behavior, storage, and network interaction of the validator neuron. Adjust these settings based on your specific requirements and infrastructure.
 
 > Note: Challenge data lives by default for 5000 blocks in the validator index. This means after 7 days the data is removed and is no longer queried by the validator. This allows miners to recover who have lost challenge data
 
 ### Running the API
 
 Running an API node at `neurons.api.py` allows you to create an entry node into the FileTao network for storing data. This can be connected to a back-end service, or used similarly to an IPFS node as an entrypoint for public use.
 
@@ -1059,28 +1043,29 @@
    ```bash
    echo 'export WANDB_API_KEY=your_api_key' >> ~/.bashrc
    source ~/.bashrc
    ```
 
    Replace `your_api_key` with the actual API key. This method automatically authenticates you with wandb every time you open a new terminal session.
 
-#### Tips and Best Practices
-
-- **Security**: Keep your API key confidential. Do not share it or commit it to public repositories.
-- **Troubleshooting**: If you encounter issues, check for common problems like incorrect API key entry or network issues.
-- **Usage in Scripts**: For using WANDB in your Python scripts, refer to the WANDB documentation for proper initialization and usage patterns.
-
-Following these steps, you should be able to successfully log into WANDB and set up your API key on your Ubuntu machine, enabling seamless integration of WANDB in your machine learning workflows.
 
 #### Compute Requirements
 No GPU is currently required to run either a validator or miner. This may change in the future for accelerating the proof and/or verification system.
 
 See [`min_compute.yml`](min_compute.yml) for complete details on minimum and recommended requirements.
 
 
+### Testnet
+FileTao runs a testnet to deploy miners and try out miners on `netuid 22`. 
+
+You can access this testnet by adding these to your script:
+```
+--subtensor.network test --netuid 22
+```
+
 ### Local Subtensor
 
 Availability is *critical* in storage in general and SN21, specifically. The reward mechanism punishes failed challenges and retrievals, even if the reason for that failure is unavailability, not only explicitly incorrect proofs or intentionally malicious behavior. It is possible to experience intermittent connectivity with the free provided endpoints for subtensor connections.
 
 It is *highly* recommended that all miners and validators run their own local subtensor node. This will resolve the many issues commonly found with intermittent connectivity across all subnets.
 
 To start your miner/validator using your local node, include the flag `--subtensor.network local` into your startup parameters.
@@ -1224,7 +1209,41 @@
 This will remove the `save` argument for RDB in the `etc/reids/redis.conf` file. 
 
 Please ensure to path the path to your redis.conf file if it is differen from the default:
 ```bash
 REDIS_PATH="/path/to/redis.conf"
 bash ./scripts/redis/disable_rdb.sh $REDIS_PATH
 ```
+
+
+## FileTAO Docker
+
+FileTao is now able to run with docker with miner, validator, and api nodes. If running a validator, API nodes are *automatically* deployed in a separate container.
+
+You are free to use this provided docker convenience but may still run nodes on bare-metal. However, it is recommended to upgrade to build and use these docker images, as they are generally more secure and convenient to use.
+
+### Run filetao with docker
+
+To run the suite of services (miner, validator, and redis), first run:
+
+```sh
+cp example.env .env
+```
+
+and populate the environment variables as appropriate. Ensure that each node has its own wallet, and is registered on SN21.
+
+To run the entire stack, use the following commands:
+
+```sh
+docker-compose build
+docker-compose up
+```
+
+To run only an individual service (e.g. miner and validator), use:
+
+```
+docker compose up --build {filetao-miner, filetao-validator}
+```
+
+### Demo notebooks and examples
+
+See [`storage/api/demo_notebook.ipynb`]("docs/api_demo.ipynb") and [`storage/api/example.py`]("storage/api/example.py") To learn different ways to query the subnet.
```

### Comparing `FileTAO-2.1.0/README.md` & `FileTAO-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,71 @@
+Metadata-Version: 2.1
+Name: FileTAO
+Version: 3.0.0
+Summary: Philanthropic storage for the masses. (FileTAO)
+Home-page: https://github.com/ifrit98/storage-subnet
+Author: philanthrope
+Author-email: ifrit98@gmail.com
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.9,<3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch>=1.13.0
+Requires-Dist: bcrypt==3.2.0
+Requires-Dist: bittensor==6.11.0
+Requires-Dist: redis==5.0.1
+Requires-Dist: pycryptodome==3.20.0
+Requires-Dist: pyinstrument==4.6.1
+Requires-Dist: wandb==0.16.0
+Requires-Dist: morphys==1.0
+Requires-Dist: py-multibase==1.0.3
+Requires-Dist: py-multicodec==0.2.1
+Requires-Dist: py-multihash==2.0.1
+Requires-Dist: ipfs-cid==1.0.0
+Requires-Dist: python-jose==3.3.0
+Requires-Dist: passlib==1.7.4
+Requires-Dist: python-multipart==0.0.9
+Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: loguru==0.7.0
+Requires-Dist: pandas==2.2.0
+Provides-Extra: dev
+Requires-Dist: pytest==7.4.3; extra == "dev"
+Requires-Dist: pytest-cov==4.1.0; extra == "dev"
+Requires-Dist: parameterized==0.9.0; extra == "dev"
+Requires-Dist: flake8==7.0.0; extra == "dev"
+
 # FileTAO
 
 [![Latest Version](https://img.shields.io/pypi/v/filetao.svg)](https://pypi.org/project/filetao/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/filetao)](https://pypi.org/project/filetao)
 [![License](https://img.shields.io/pypi/l/filetao.svg)](https://github.com/ifrit98/storage-subnet/blob/master/LICENSE)
 
 ![Subnet21](assets/Subnet21.png)
 
 FileTAO (Bittensor Subnet 21) implements a novel, multi-layered zero-knowledge interactive proof-of-spacetime algorithm by cleverly using Pedersen commitments, random challenges leveraging elliptic curve cryptography, sequential seed-based chained hash verification, and merkle proofs to achieve an efficient, robust, secure, and highly available decetralized storage system on the Bittensor network. The system validates on encrypted user data, such that miners are unaware of what data they are storing, and only end-users may encrypt/decrypt the data they provide with their bittensor wallet coldkey.
 
 We consider this system to be an important stepping stone so that bittensor can fulfill its mission of democratizing intelligence, and a decentralized AWS platform is a key brick in this wall. 
 
 **NOTICE**: Using this software, you **must** agree to the Terms and Agreements provided in the [terms and conditions](TERMS.md) document. By downloading and running this software, you implicitly agree to these terms and conditions.
 
-Currently supporting `python>=3.9,<3.11`.
+Currently supporting `python>=3.9,<3.12`.
 
 > Note: The storage subnet is in an alpha stage and is subject to rapid development.
 
 # Table of Contents for Subnet 21 (FileTAO)
 1. [FileTAO Overview](#filetao)
 2. [Installation](#installation)
    - [Install Redis](#install-redis)
@@ -49,28 +98,36 @@
    - [Advanced Cryptographic Techniques](#advanced-cryptographic-techniques)
    - [User-Centric Approach](#user-centric-approach)
 7. [Zero Knowledge Proof-of-Spacetime](#zero-knowledge-proof-of-spacetime)
    - [Storage Phase](#storage-phase)
    - [Challenge Phase](#challenge-phase)
    - [Retrieval Phase](#retrieval-phase)
 8. [Reward System](#reward-system)
+   - [Overview and Justification](#overview-and-justification)
    - [Speed and Reliability in Decentralized Storage Mining](#speed-and-reliability-in-decentralized-storage-mining)
+   - [Viewing Wandb Runs](#viewing-wandb-runs)
 9. [Epoch UID Selection](#epoch-uid-selection)
 10. [Running FileTAO](#running-filetao)
     - [Running a Miner](#running-a-miner)
     - [Running a Validator](#running-a-validator)
     - [Running the API](#running-the-api)
     - [Setup WandB](#setup-wandb)
+    - [Testnet](#testnet)
 11. [Local Subtensor](#local-subtensor)
 12. [Database Schema Migration](#database-schema-migration)
 13. [Disable RDB](#disable-rdb)
-
+14. [FileTAO Docker](#filetao-docker)
+15. [Demos](#demo-notebooks-and-examples)
 
 ## Installation
 ```bash
+# Please install torch-cpu if you do not need a gpu. (GPU not required for FileTAO)
+pip install torch==2.3.0+cpu -f https://download.pytorch.org/whl/torch_stable.html
+
+# Clone and Install the FileTAO repo.
 git clone https://github.com/ifrit98/storage-subnet
 cd storage-subnet
 python -m pip install -e .
 ```
 
 ### Install Redis
 Install Redis on your host system.
@@ -113,41 +170,19 @@
 Nov 16 22:35:42 user systemd[1]: Started Advanced key-value store.
 ```
 
 ### Secure Redis Configuration
 
 In order to securely run a node, whether a miner or validator, you must run ensure your redis instance is secure from the outside internet and is password-protected.
 
-The following steps are **mandatory** for secure communication on the network:
+The following steps are **recommended** for secure communication on the network and data integrity:
 
-1. Closing the default redis port
 1. Password protecting redis
-1. Enabling persistence
-
-#### Close external traffic to Redis 
+1. Enabling redis persistence
 
-> Note: **EXPOSING THE REDIS PORT IS A MAJOR SECURITY RISK**
-
-This Bash script is designed to configure UFW (Uncomplicated Firewall) to manage access to default Redis port 6379. The script's primary function is to block all external traffic to port 6379, typically used by Redis, while allowing local processes to still access this port.
-
-##### Usage
-To run the script, use the following command in the terminal:
-```bash
-sudo ./scripts/redis/create_redis_firewall.sh
-```
-Running this script will:
-- Check if UFW is installed and active. If UFW is not active, the script will attempt to enable it.
-- Set UFW rules to deny all external access to port 6379.
-- Set UFW rules to allow all local access to port 6379.
-- Apply the changes by reloading UFW.
-
-##### Important Considerations
-- **Test Before Production**: Always test the script in a controlled environment before deploying it in a production setting.
-- **Existing Rules**: If there are existing rules for port 6379, review the script to ensure compatibility.
-- **Firewall Management**: This script is specifically for systems using UFW. If another firewall management tool is in use, this script will not be compatible.
 
 #### Automated Redis Password Configuration
 To enhance security, our system now automatically generates a strong password for Redis. This is **REQUIRED**. This is handled by the `set_redis_password.sh` script. Follow these steps to set up Redis with an automated password:
 
 1. **Run the Redis Start Script**: 
     ```bash
     bash scripts/redis/set_redis_password.sh
@@ -240,22 +275,22 @@
 from storage.api import store, retrieve
 
 # Store data
 wallet = bt.wallet()
 subtensor = bt.subtensor()
 
 data = b"Some bytestring data!"
-cid, hotkeys = await store(data, wallet, subtensor, netuid=22)
+cid, hotkeys = await store(data, wallet, subtensor, netuid=21)
 print("Stored {} with {} hotkeys".format(cid, hotkeys))
 > Stored bafkreid6mhmfptdpfvljyavss77zmo6b2oert2pula2gy4tosekupm4nqa with validator hotkeys [5CaFuijc2ucdoWhkjLaYgnzYrpv62KGt1fWWtUxhFHXPA3KK, 5FKwbwguHU1SVQiGot5YKSTQ6fWGVv2wRHFrWfwp9X9nWbyU]
 ```
 
 Now you can retrieve the data using the content identifier `CID` and the `hotkey`s directly:
 ```python
-data = await retrieve(cid, wallet, subtensor, netuid=22, hotkeys=hotkeys)
+data = await retrieve(cid, wallet, subtensor, netuid=21, hotkeys=hotkeys)
 print(data)
 > b"Some bytestring data!"
 ```
 
 ### Using SubnetsAPI 
 In addition to the convenience wrappers and command-line interface, FileTao can be accessed via the bittensor subnets python API.
 
@@ -589,153 +624,194 @@
 In each phase, cryptographic primitives ensure data integrity and confidentiality. The encryption and commitment schemes ensure the data's security, while Merkle trees and random challenges provide a robust method for verifying data possession without revealing the actual data.
 
 In each phase, cryptographic primitives like hashing, commitment schemes (e.g., Elliptic Curve Cryptography and Pedersen commitments), and data structures like Merkle trees are employed to ensure the integrity, confidentiality, and availability of the data. The use of seeds and randomness in commitments adds an additional layer of security and ensures that each instance of data storage and retrieval is unique and verifiable. See [here](https://kndrck.co/posts/efficient-merkletrees-zk-proofs/) for more information.
 
 
 ## Reward System
 
+There are several components to the reward mechanism and is multi-layered. In a nutshell, the goals are as follows:
+
+- Incentivize data durability and salience via cryptographic proof system. (E.g. don't lose data.)
+- Incentivize good performance over a long period of time. (Tier system to reward based on reputation.)
+- Incentivize fast response times. We want to retrieve user data quickly and ensure that it is over high network bandwidth.
+
 In FileTAO's decentralized storage system, optimal behavior is crucial for the overall health and efficiency of the network. Miners play a vital role in maintaining this ecosystem, and their actions directly impact their rewards and standing within the subnet. We have implemented a tier-based reward system to encourage proper behavior, successful challenge completions, and consistent performance.
 
 Failing to pass either challenge or retrieval verifications incur negative rewards. This is doubly destructive, as rolling statistics are continuously logged to periodically compute which tier a given miner hotkey belongs to. When a miner achieves the threshold for the next tier, the rewards that miner receives proportionally increase. Conversely, when a miner drops below the threshold of the previous tier, that miner's rewards are slashed such that they receive rewards proportionally to the immediately lower tier.
 
+### Overview and Justification
+FileTAO's Multi-dimensional reward mechanism is spread across 4 main axes:
+(1) Availability: Is the miner reachable when requested? Incentivizes uptime.
+(2) Speed (performant): how fast was the normalized response time?
+(3) Correctness (reliable): did the proof succeed? y/n
+(4) Trustworthiness (correctness over time): Tier definitions encapsulate consistenty and trustworthiness over time. A miner that rarely fails challenges and faithfully returns data when requested will receive an initial higher proportional reward.
+
+The main drivers behind the reward mechanism are to model meritocratic systems as seen in the academic realm and in the business world that scales trust across time and observation of output. For example, we create various "tiers" in education, Undergraduate, Masters, PhD, Post Doc, or in software, Junior Engineer, Senior Engineer, Principal Engineer, Staff Engineer, etc where each subsequent level achieved has proportionally greater expecetations on performance and qualification of the individual. 
+
+However, performance of the individual must match the expectations of the pedigree, and behavior that is inconsistent with a given level will be adjusted. If, for example, a Junior Engineer proves their output is substantial and over time completes projects that provide value, that engineer will be promoted to Senior Engineer over time, and pontentially beyond. Conversely, a Principal Engineer that consistently underperforms expectations will be demoted to a role with lower expectations until able to prove otherwise. The same logic applies to miners in FileTAO (SN21).
+
+Tier (class) mobility is at the heart of the mechanism, and provides a balance between competition and trust, where over time competitiveness breeds a degree of trust on which we can associate a degree of reliability with a given entity (or miner).
+
 **Why Optimal Behavior Matters:**
 1. **Reliability:** Miners who consistently store, retrieve, and pass challenges with high Wilson Scores ensure the reliability and integrity of the network.
 2. **Trust:** High-performing miners build trust in the network, attracting more users and increasing the overall value of the system.
 3. **Efficiency:** Optimal behavior leads to a more efficient network, reducing the likelihood of data loss and ensuring fast, reliable access to stored information.
 
 **Tier-Based Reward System:**
 - **Tiers:** We classify miners into four tiers – Diamond, Gold, Silver, and Bronze – based on their performance metrics.
 - **Performance Metrics:** These include the Wilson Score in storage, retrieval, and challenge tasks, as well as the total number of successful operations.
 - **Higher Rewards for Higher Tiers:** Miners in higher tiers receive a greater proportion of the rewards, reflecting their superior performance and contribution to the network.
 
 ### **Wilson Score**
-A measure of confidence is required to assess reliability in low sample environments. For miners who have less history, it is unfair to expect perfection early on and is account for by using a statistical tool, the `Wilson Score`. 
+
+A measure of confidence is required to assess reliability in low sample environments. For miners who have less history, it is unfair to expect perfection early on and is account for by using a statistical tool, the `Wilson Score`. An asymmetric approximation of the confidence interval suited for low sample sizes given a particular z-score target, the `Wilson score` doesn't suffer from problems of overshoot and zero-width intervals that afflict the normal interval approximation.
+
+See: https://en.wikipedia.org/wiki/Binomial_proportion_confidence_interval#Wilson_score_interval for more information.
 
 For example, if a miner succeeds 4/5 times, it has a success rate of 80%. However it may not be indicative of true performance and reliability. Thus we have added Wilson Scores to accomodate low sample populations to get a more balanced approach to scoring miners.
 
 This effectively allows for forgiveness for early failures and facilitates miners who are faithful actors to still rise through the tier system without being perpetually punished for early mistakes or poor optimization.
 
 The equivalent wilson score for 4 of 5 attempts is `0.77`, which indicates with 95% statistical confidence that this miner is AT least this successful 80% of the time. Functionally, this allows for lowering of the tier requirements while having statistical confidence that over time, the miner may continue to improve performance from there while being considered reliable.
 
-**Moving Up Tiers:**
-- To ascend to a higher tier, a miner must maintain high Wilson Scores and achieve a set number of total successes.
-- This progression system incentivizes continuous improvement and excellence in mining operations.
-
-**Graphical Representation:**
-- The graph below illustrates how rewards increase as miners advance through the tiers. It visually represents the potential growth in earnings as miners optimize their operations and maintain high standards of performance.
-
-<div align="center">
-   <img src="assets/reward-tiers-vert.png" alt="Bonding Curves" width="650"/>
-</div>
+More concretely, given `N` trials, the wilson score establishes a lower bound for the confidence interval on miner success rates given low sample or population sizes. E.g., if a miner responds successfuly 8 of 9 times, it's lower bound on success rate is roughly `0.8701769999681506`. In other words, `wilson_score(8,9) == 0.8701769999681506`, suggesting that 87% of the time, this miner is expected to succeed on average. 
+
+This calculation is used as the lower bound to determine tier eligibility and establishes a "minimium trust level" for the miner. If a miner continues to have failed challenges, the wilson score lower bound will cross below the current tier threshold, and when the tiers are recalculated, that miner will move down a tier (e.g. `Diamond -> Gold`.)
 
-#### Tier System:
+### **monitor**
+Miners are also incentivized to be available, and are punshed for not being online, (e.g. failed `n` pings) by the `monitor` protocol. Periodically (every `m` steps) validators ping a set of `k` miners (default is 40), and after 5 successive failed attempts to ping a specific UID, that miner will be negatively rewarded for unavailability.
+
+### Tier System:
 The tier system classifies miners into five distinct categories, each with specific requirements and storage limits. These tiers are designed to reward miners based on their performance, reliability, and the total volume of data they can store.
 
 Importance of Tier System:
 - **Encourages High Performance:** Higher tiers reward miners with greater benefits, motivating them to maintain high Wilson Scores.
 - **Enhances Network Reliability:** The tier system ensures that only the most reliable and efficient miners handle significant volumes of data, enhancing the overall reliability of the network.
 - **Fair Reward Distribution:** The reward factors are proportional to the miners' tier, ensuring a fair distribution of rewards based on performance.
 
 1. 🎇 **Super Saiyan Tier:** 
-   - **Storage Limit:** 1 Exabyte (EB)
-   - **Store Wilson Score:** 0.88
-   - **Minimum Successes Required:** 10,000
+   - **Storage Limit:** 50 Petabytes (PB)
+   - **Store Wilson Score:** 0.9
+   - **Minimum Successes Required:** 15,000
    - **Reward Factor:** 1.0 (100% rewards)
 
-2. 💎 **Diamond Tier:**
-   - **Storage Limit:** 1 Petabyte (PB)
-   - **Store Wilson Score:**  0.77
-   - **Minimum Successes Required:** 5,000
-   - **Reward Factor:** 0.9 (90% rewards)
-
-3. 🥇 **Gold Tier:**
-   - **Storage Limit:** 100 Terabytes (TB)
-   - **Store Wilson Score:** 0.66
-   - **Minimum Successes Required:** 2,000
+2. 🌹 **Ruby Tier**
+   - **Storage Limit:** 20 Petabytes (PB)
+   - **Store Wilson Score:** 0.85
+   - **Minimum Successes Required:** 10,000
+   - **Rewrd Factor:** 0.9 (90% rewards)
+
+3. 🔮 **Emerald Tier**
+   - **Storage Limit:** 10 Petabytes (PB)
+   - **Store Wilson Score:** 0.8
+   - **Minimum Successes Required:** 8,000
+   - **Rewrd Factor:** 0.85 (85% rewards)
+
+4. 💠 **Diamond Tier:**
+   - **Storage Limit:** 5 Petabytes (PB)
+   - **Store Wilson Score:**  0.75
+   - **Minimum Successes Required:** 6,000
    - **Reward Factor:** 0.8 (80% rewards)
 
-4. 🥈 **Silver Tier:**
-   - **Storage Limit:** 10 Terabytes (TB)
-   - **Store Wilson Score:** 0.55
-   - **Minimum Successes Required:** 1,000
+5. 🔗 **Platinum Tier**
+   - **Storage Limit:** 1 Petabyte (PB)
+   - **Store Wilson Score:** 0.65
+   - **Minimum Successes Required:** 4,000
+   - **Reward Factor:** 0.75 (75% rewards) 
+
+6. 🥇 **Gold Tier:**
+   - **Storage Limit:** 200 Terabytes (TB)
+   - **Store Wilson Score:** 0.65
+   - **Minimum Successes Required:** 2,000
    - **Reward Factor:** 0.7 (70% rewards)
 
-5. 🥉 **Bronze Tier:**
-   - **Storage Limit:** 1 Terabyte (TB)
+7. 🥈 **Silver Tier:**
+   - **Storage Limit:** 50 Terabytes (TB)
+   - **Store Wilson Score:** 0.6
+   - **Minimum Successes Required:** 500
+   - **Reward Factor:** 0.65 (65% rewards)
+
+8. 🥉 **Bronze Tier:**
+   - **Storage Limit:** 10 Terabytes (TB)
    - **Store Wilson Score:** Not specifically defined for this tier
    - **Minimum Successes Required:** Not specifically defined for this tier
    - **Reward Factor:** 0.6 (60% rewards)
 
 #### Maintaining and Advancing Tiers:
 - To advance to a higher tier, miners must consistently achieve the required minimum Wilson Scores in their operations.
-- Periodic evaluations are conducted to ensure miners maintain the necessary performance standards to stay in their respective tiers.
-- Advancing to a higher tier takes time. In order to ascend to the first higher tier (Silver), it takes at least 1000 successful requests, whether they are challenge requests, store requests, or retry requests and must maintain a 95% Wilson Score in all categories. 
-- Depending on how often a miner is queried, how many validators are operating at one given time, and primarily the performance of the miner, this can take several hours to several days. Assuming full 64 validator slots are occupied, this should take a matter of hours.
+- Periodic evaluations are conducted to ensure miners maintain the necessary performance standards to stay in their respective tiers, or move up or down tiers.
+- Advancing to a higher tier takes time. In order to ascend to the first higher tier (Silver), it takes at least 1000 successful requests, whether they are challenge requests, store requests, or retry requests and must maintain the minimum Wilson Score for successes / attempts. 
+- Depending on how often a miner is queried, how many validators are operating at one given time, and primarily the performance of the miner, this can take several hours to several days. Assuming full 64 validator slots are occupied, this should take ~100 hours.
 
-Here is a distribution of UIDs queried over 1000 blocks based on block hash:
-![uid-dist](assets/uid_dist.png)
+As miners move up tiers, their responsibility increases proportionally. Thus, miners who move from Silver -> Gold are expected to be able to store up to 200 Terabytes (TB) of data, a 4x the storage cap for Silver. Similarly, it must maintain a minimum wilson score of 0.66 over it's lifetime, increasing the lower bound for expected performance and reliability. It also means that this miner will now receive a higher percentage of rewards for each successful query, going from 65% -> 70%. This does not mean that the miner may rest on its laurels, and may move right back down a tier (or more) if it does not meed the minimum requirements for Gold.
 
 Assuming perfect performance, that out of ~200 miner UIDs, each of which is queried roughly 34 times every 1000 rounds, namely a 3.4% chance every query round, one can expect to reach the next tier within 
-
 ```bash
-hours = total_successes / prob_of_query_per_round * time_per_round / 3600
-hours = 98 # roughly 4 days at perfect performance to top tier (no challenge failures)
+hours = total_successes / prob_of_query_per_round * time_per_round / 3600 / num_active_validators
+hours = 4.9 # roughly 5 hours at perfect performance to next (Silver) tier (assuming no challenge failures)
 ```
 
 #### Miner Advancement Program
 The top two (2) performers per batch of `store`, `challenge` or `retrieve` requests will recieve a one-time tier appropriate boost. These tier-specific boosts decrease as you ascend the tier structure, and are defined in `constants.py`. For example:
 
 ```bash
 TIER_BOOSTS = {
     b"Super Saiyan": 1.02, # 2%  -> 1.02
-    b"Diamond": 1.05,      # 5%  -> 0.945
-    b"Gold": 1.1,          # 10% -> 0.88
-    b"Silver": 1.15,       # 15% -> 0.805
+    b"Ruby": 1.04,         # 4%  -> 0.936
+    b"Emerald": 1.05,      # 6%  -> 0.918
+    b"Diamond": 1.08,      # 8%  -> 0.864
+    b"Platinum": 1.1,      # 10% -> 0.825
+    b"Gold": 1.12,         # 12% -> 0.784
+    b"Silver": 1.16,       # 16% -> 0.754
     b"Bronze": 1.2,        # 20% -> 0.72
 }
 ```
 
 Concretely, a `Bronze` miner who is one of the top 2 within a batch of requests will receive a proportionally larger boost than a `Diamond` miner who is also in the top 2.
 
 ```
 REWARD = TIER * REWARD * BOOST
 Bronze  -> 0.72 = 0.6 * 1.0 * 1.2
 Diamond -> 0.84 = 0.8 * 1.0 * 1.05
 ```
 
-This mechansim *significantly* closes the gap for newer miners who perform well and should be able to ascned the tier structure honestly and faithfully.
+This mechanism *significantly* closes the gap for newer miners who perform well and should be able to ascend the tier structure honestly and faithfully. This is such that miners who consistently perform well but are lower tiers can more readily survive immunity period to make it to successively higher tiers and not "gate" access to the older miners. This directly negates the "grandfathering" effect. Higher tier miners that are in the top 2 are boosted significantly less than those Bronze or lower tier miners who make the top 2.
+
 
 #### Periodic Statistics Rollover
 
-Statistics for `store_successes/attempts`, `challenge_attempts/successes`, and `retrieve_attempts/successes` are reset every epoch, while the `total_successes` are carried over for accurate tier computation. This "sliding window" of the previous 360 blocks of `N` successes vs `M` attempts effectively resets the `N / M` ratio and applies Wilson Scoring. This facilitates a less punishing tier calculation for early failures that then have to be "outpaced", while simultaneously discouraging grandfathering in of older miners who were able to succeed early and cement their status in a higher tier. The net effect is greater mobility across the tiers, keeping the network competitive while incentivizing reliability and consistency.
+Statistics for `store_successes/attempts`, `challenge_attempts/successes`, and `retrieve_attempts/successes` are reset every 2 epochs (720 blocks), while the `total_successes` are carried over for accurate tier computation. This "sliding window" of the previous 720 blocks of `N` successes vs `M` attempts effectively resets the `N / M` ratio and applies Wilson Scoring. This facilitates a less punishing tier calculation for early failures that would otherwise have to be "outpaced", while simultaneously discourages grandfathering older miners who were able to succeed early and cemented their status in a higher tier. The net effect is greater mobility across the tiers, keeping the network competitive while incentivizing reliability and consistency.
 
 For example:
 ```bash
 store_successes = 2
 store_attempts = 2
 challenge_successes = 3
 challenge_attempts = 5
 retrieve_successes = 1
 retireve_attempts = 1
-total_successes_epoch = 6
-total_attempts_epoch = 8
-wilson_score = 0.73 # would qualify for Diamond tier this round
+total_successes_epoch = 7
+total_attempts_epoch = 9
+total_successes = 6842
+wilson_score = 0.79
 ```
 
 The scores are then reset, while keeping the total successes for tier recognition:
 ```bash
 store_attempts = 0
 store_successes = 0
 challenge_successes = 0
 challenge_attempts = 0
 retrieve_successes = 0
 retrieve_attempts = 0
-total_successes = 6
+total_successes = 6851 # + 9 by aggregating total successs previous 2 epochs
 ```
 
+> This miner would qualify for Diamond tier this round, as it has passed the minimum threshold for total successes (5000) and wilson score (0.77).
+
 ### Speed and Reliability in Decentralized Storage Mining
 
 In the context of FileTAO's decentralized storage system, speed and reliability are critical factors that significantly influence the performance and reputation of miners. These factors not only affect the efficiency of data storage and retrieval but also play a crucial role in the overall user experience and the robustness of the network.
 
 #### Importance of Speed:
 1. **Quick Data Access:** Fast response times in data storage and retrieval operations are essential for a seamless user experience. Miners with quicker response times enhance the network's ability to serve data efficiently.
 2. **Improved Network Performance:** Speedy processing of tasks contributes to the overall performance of the network, reducing bottlenecks and ensuring smooth data flow.
@@ -755,26 +831,28 @@
 2. **Tier-Based Reward Factors:** Each tier has an associated reward factor, which determines the proportion of rewards received by the miner. Higher tiers, achieved through consistent performance, offer greater rewards. Miner rewards and punishments are symmetrically scaled by their tier. Miners who have a lower tier are penalized proportionally less than miners who have a higher tier. This encourages top miners to have higher Wilson Scores, and allows for lower tier miners the ability to work their way up the ladder.
 
 e.g.
 ```python
 reward = 1.0 * TIER_FACTOR if task_successful else TASK_NEGATIVE_REWARD * TIER_FACTOR
 
 # For Bronze and challenges
-reward = 1.0 * 0.555 if challenge_successful else -0.05 * 0.555
+reward = 1.0 * 0.5 if challenge_successful else -0.05 * 0.5
 reward
-> 0.555 | -0.02775 # lighter punishment for lower tier failure
+> 0.5 | -0.025 # lighter punishment for lower tier failure
 
 # However for Gold
-reward = 1.0 * 0.777 if challenge_successful else -0.05 * 0.777
+reward = 1.0 * 0.7 if challenge_successful else -0.05 * 0.7
 reward
-> 0.777 | -0.03885 # harsher punishment for higher tier failure
+> 0.7 | -0.035 # harsher punishment for higher tier failure
 ```
 
 The tier system in FileTAO's decentralized storage network plays a pivotal role in ensuring the network's efficiency and reliability. By setting clear performance benchmarks and rewarding miners accordingly, the system fosters a competitive yet fair environment. This encourages continuous improvement among miners, ultimately leading to a robust and trustworthy decentralized storage solution.
 
+### Viewing Wandb Runs
+You can view validator provided run data on wandb by viewing the project found at this [link](https://wandb.ai/philanthrope/philanthropic-thunder/table). This provides information on miner statistics and tier level available to the public.
 
 ## Epoch UID selection
 Miners are chosen pseudorandomly using the current block hash as a random seed. This allows for public verification of which miners are selected for each challenge round (3 blocks).
 
 
 For example:
 ```python
@@ -810,56 +888,14 @@
 ```bash
 pm2 start /home/user/storage-subnet/neurons/miner.py --interpreter /home/user/miniconda3/envs/sn21/bin/python --name miner -- --netuid 21 --wandb.off --wallet.name default --wallet.hotkey miner  --axon.port 8888 --logging.debug
 ```
 
 > Make sure to use absolute paths when executing your pm2 command.
 
 
-#### Options
-
-- `--netuid`: Specifies the chain subnet uid. Default: 21.
-- `--miner.name`: Name of the miner, used for organizing logs and data. Default: "core_storage_miner".
-- `--miner.device`: Device to run the miner on, e.g., "cuda" for GPUs or "cpu" for CPU. Default depends on CUDA availability.
-- `--miner.verbose`: Enables verbose logging. Default: False.
-
-- `--database.host`: Hostname of the redis database. Default: "localhost".
-- `--database.port`: Port for the redis database. Default: 6379.
-- `--database.index`: Redis database index. Default: 0.
-- `--database.directory`: Directory to store local data. Default: "~/.data".
-
-- `--miner.set_weights_wait_for_inclusion`: Wether to wait for the set_weights extrinsic to enter a block. Default: False.
-- `--miner.set_weights_wait_for_finalization`: Wether to wait for the set_weights extrinsic to be finalized on the chain. Default: False.
-
-- `--blacklist.blacklist_hotkeys`: List of hotkeys to blacklist. Default: [].
-- `--blacklist.whitelist_hotkeys`: List of hotkeys to whitelist. Default: [].
-- `--blacklist.force_validator_permit`: If True, only allows requests from validators. Default: False.
-- `--blacklist.allow_non_registered`: If True, allows non-registered hotkeys to mine. Default: False.
-- `--blacklist.minimum_stake_requirement`: Minimum stake requirement for participating hotkeys. Default: 0.0.
-- `--blacklist.min_request_period`: Time period (in minutes) to serve a maximum number of requests per hotkey. Default: 5.
-
-- `--miner.priority.default`: Default priority for non-registered requests. Default: 0.0.
-- `--miner.priority.time_stake_multiplicate`: Time (in minutes) to double the importance of stake in the priority queue. Default: 10.
-- `--miner.priority.len_request_timestamps`: Number of historical request timestamps to record. Default: 50.
-
-- `--miner.no_set_weights`: If True, the miner does not set weights on the chain. Default: False.
-- `--miner.no_serve`: If True, the miner does not serve requests. Default: False.
-- `--miner.no_start_axon`: If True, the miner does not start the axon server. Default: False.
-
-- `--miner.mock_subtensor`: If True, uses a mock subtensor for testing. Default: False.
-
-- `--wandb.off`: Disables Weight and Biases logging. Default: False.
-- `--wandb.project_name`: Project name for WandB logging. Default: "philanthropic-thunder".
-- `--wandb.entity`: WandB entity (username or team name) for the run. Default: "philanthrope".
-- `--wandb.offline`: Runs WandB in offline mode. Default: False.
-- `--wandb.weights_step_length`: Steps interval for logging weights to WandB. Default: 10.
-- `--wandb.run_step_length`: Steps interval for a new run rollover in WandB. Default: 1500.
-- `--wandb.notes`: Notes to add to the WandB run. Default: "".
-
-These options allow you to configure the miner's behavior, database connections, blacklist/whitelist settings, priority handling, and integration with monitoring tools like WandB. Adjust these settings based on your mining setup and requirements.
-
 
 #### Data migration
 If for whatever reason you need to migrate the data in your hard drive configured with `--database.directory` to a new directory than is reflected in the Redis index, then you can do it by simply running the script in `scripts/migrate_database_directory.sh`. 
 
 When should you run the migration script?:
 - if you want to specify a different --database.directory
 - if your data has moved but your redis index has not reflected this change
@@ -926,40 +962,14 @@
 For example,
 ```bash
 REBALANCE_SCRIPT_PATH=/home/user/storage-subnet/scripts/rebalance_deregistration.sh
 ```
 
 This way you are able to run your process from anywhere and not rely on relative path resolution to ensure proper functioning of the validator.
 
-#### Options
-
-- `--neuron.name`: Specifies the name of the validator neuron. Default: "core_storage_validator".
-- `--neuron.device`: The device to run the validator on (e.g., "cuda" for GPU, "cpu" for CPU). Default: "cuda" if CUDA is available, else "cpu".
-- `--neuron.curve`: The elliptic curve used for cryptography. Only "P-256" is currently available.
-- `--neuron.maxsize`: The maximum size of random data to store. If `None`, a lognormal random Gaussian distribution is used (default: `None`).
-- `--neuron.min_chunk_size`: The minimum chunk size of random data for challenges. Default: 256.
-- `--neuron.disable_log_rewards`: If set, disables all reward logging to suppress function values from being logged (e.g., to WandB). Default: False.
-- `--neuron.chunk_factor`: The factor to divide data into chunks. Default: 4.
-- `--neuron.num_concurrent_forwards`: The number of concurrent forward requests running at any time. Default: 1.
-- `--neuron.disable_set_weights`: If set, disables setting weights on the chain. Default: False.
-- `--neuron.semaphore_size`: The limit on concurrent asynchronous calls. Default: 256.
-- `--neuron.checkpoint_block_length`: Blocks before a checkpoint is saved. Default: 100.
-- `--neuron.events_retention_size`: File size for retaining event logs (e.g., "2 GB"). Default: "2 GB".
-- `--neuron.dont_save_events`: If set, event logs will not be saved to a file. Default: False.
-- `--neuron.vpermit_tao_limit`: The maximum TAO allowed for querying a validator with a vpermit. Default: 500.
-- `--neuron.verbose`: If set, detailed verbose logs will be printed. Default: False.
-- `--neuron.log_responses`: If set, all responses will be logged. Note: These logs can be extensive. Default: False.
-- `--neuron.data_ttl`: The number of blocks before stored challenge data expires. Default: 50000 (approximately 7 days).
-- `--neuron.profile`: If set, network and I/O actions will be profiled. Default: False.
-
-- `--database.host`: Hostname of the Redis database. Default: "localhost".
-- `--database.port`: Port of the Redis database. Default: 6379.
-- `--database.index`: The database number for the Redis instance. Default: 1.
-
-These options allow you to fine-tune the behavior, storage, and network interaction of the validator neuron. Adjust these settings based on your specific requirements and infrastructure.
 
 > Note: Challenge data lives by default for 5000 blocks in the validator index. This means after 7 days the data is removed and is no longer queried by the validator. This allows miners to recover who have lost challenge data
 
 ### Running the API
 
 Running an API node at `neurons.api.py` allows you to create an entry node into the FileTao network for storing data. This can be connected to a back-end service, or used similarly to an IPFS node as an entrypoint for public use.
 
@@ -1033,28 +1043,29 @@
    ```bash
    echo 'export WANDB_API_KEY=your_api_key' >> ~/.bashrc
    source ~/.bashrc
    ```
 
    Replace `your_api_key` with the actual API key. This method automatically authenticates you with wandb every time you open a new terminal session.
 
-#### Tips and Best Practices
-
-- **Security**: Keep your API key confidential. Do not share it or commit it to public repositories.
-- **Troubleshooting**: If you encounter issues, check for common problems like incorrect API key entry or network issues.
-- **Usage in Scripts**: For using WANDB in your Python scripts, refer to the WANDB documentation for proper initialization and usage patterns.
-
-Following these steps, you should be able to successfully log into WANDB and set up your API key on your Ubuntu machine, enabling seamless integration of WANDB in your machine learning workflows.
 
 #### Compute Requirements
 No GPU is currently required to run either a validator or miner. This may change in the future for accelerating the proof and/or verification system.
 
 See [`min_compute.yml`](min_compute.yml) for complete details on minimum and recommended requirements.
 
 
+### Testnet
+FileTao runs a testnet to deploy miners and try out miners on `netuid 22`. 
+
+You can access this testnet by adding these to your script:
+```
+--subtensor.network test --netuid 22
+```
+
 ### Local Subtensor
 
 Availability is *critical* in storage in general and SN21, specifically. The reward mechanism punishes failed challenges and retrievals, even if the reason for that failure is unavailability, not only explicitly incorrect proofs or intentionally malicious behavior. It is possible to experience intermittent connectivity with the free provided endpoints for subtensor connections.
 
 It is *highly* recommended that all miners and validators run their own local subtensor node. This will resolve the many issues commonly found with intermittent connectivity across all subnets.
 
 To start your miner/validator using your local node, include the flag `--subtensor.network local` into your startup parameters.
@@ -1198,7 +1209,41 @@
 This will remove the `save` argument for RDB in the `etc/reids/redis.conf` file. 
 
 Please ensure to path the path to your redis.conf file if it is differen from the default:
 ```bash
 REDIS_PATH="/path/to/redis.conf"
 bash ./scripts/redis/disable_rdb.sh $REDIS_PATH
 ```
+
+
+## FileTAO Docker
+
+FileTao is now able to run with docker with miner, validator, and api nodes. If running a validator, API nodes are *automatically* deployed in a separate container.
+
+You are free to use this provided docker convenience but may still run nodes on bare-metal. However, it is recommended to upgrade to build and use these docker images, as they are generally more secure and convenient to use.
+
+### Run filetao with docker
+
+To run the suite of services (miner, validator, and redis), first run:
+
+```sh
+cp example.env .env
+```
+
+and populate the environment variables as appropriate. Ensure that each node has its own wallet, and is registered on SN21.
+
+To run the entire stack, use the following commands:
+
+```sh
+docker-compose build
+docker-compose up
+```
+
+To run only an individual service (e.g. miner and validator), use:
+
+```
+docker compose up --build {filetao-miner, filetao-validator}
+```
+
+### Demo notebooks and examples
+
+See [`storage/api/demo_notebook.ipynb`]("docs/api_demo.ipynb") and [`storage/api/example.py`]("storage/api/example.py") To learn different ways to query the subnet.
```

### Comparing `FileTAO-2.1.0/neurons/api.py` & `FileTAO-3.0.0/neurons/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,17 +33,19 @@
 from storage.shared.utils import get_redis_password
 from storage.shared.subtensor import get_current_block
 from storage.validator.config import config, check_config, add_args
 from storage.validator.state import should_checkpoint
 from storage.validator.encryption import encrypt_data, setup_encryption_wallet
 from storage.validator.store import store_broadband
 from storage.validator.retrieve import retrieve_broadband
-from storage.validator.database import retrieve_encryption_payload, get_ordered_metadata
+from storage.validator.database import retrieve_encryption_payload, get_ordered_metadata, delete_file_from_database
 from storage.validator.cid import generate_cid_string
 from storage.validator.encryption import decrypt_data_with_private_key
+from storage.validator.dendrite import timed_dendrite
+from storage.indexer import run_indexer_thread
 
 
 def MockDendrite():
     pass
 
 
 class neuron:
@@ -75,16 +77,22 @@
 
     def __init__(self):
         self.config = neuron.config()
         self.check_config(self.config)
         bt.logging(config=self.config, logging_dir=self.config.neuron.full_path)
         print(self.config)
 
+        redis_password = get_redis_password(self.config.database.redis_password)
         try:
-            asyncio.run(check_environment(self.config.database.redis_conf_path))
+            asyncio.run(check_environment(
+                self.config.database.redis_conf_path,
+                self.config.database.host,
+                self.config.database.port,
+                redis_password
+            ))
         except AssertionError as e:
             bt.logging.warning(
                 f"Something is missing in your environment: {e}. Please check your configuration, use the README for help, and try again."
             )
 
         bt.logging.info("neuron.__init__()")
 
@@ -127,15 +135,14 @@
             netuid=self.config.netuid, network=self.subtensor.network, sync=False
         )  # Make sure not to sync without passing subtensor
         self.metagraph.sync(subtensor=self.subtensor)  # Sync metagraph with subtensor.
         bt.logging.debug(str(self.metagraph))
 
         # Setup database
         bt.logging.info("loading database")
-        redis_password = get_redis_password(self.config.database.redis_password)
         self.database = aioredis.StrictRedis(
             host=self.config.database.host,
             port=self.config.database.port,
             db=self.config.database.index,
             socket_keepalive=True,
             socket_connect_timeout=300,
             password=redis_password,
@@ -146,51 +153,55 @@
         bt.logging.debug("loading moving_averaged_scores")
         self.moving_averaged_scores = torch.zeros((self.metagraph.n)).to(self.device)
         bt.logging.debug(str(self.moving_averaged_scores))
 
         self.my_subnet_uid = self.metagraph.hotkeys.index(
             self.wallet.hotkey.ss58_address
         )
-        bt.logging.info(f"Running validator on uid: {self.my_subnet_uid}")
+        bt.logging.info(f"Running validator (api) on uid: {self.my_subnet_uid}")
 
         bt.logging.debug("serving ip to chain...")
         try:
             self.axon = bt.axon(wallet=self.wallet, config=self.config)
 
             self.axon.attach(
                 forward_fn=self.store_user_data,
                 blacklist_fn=self.store_blacklist,
                 priority_fn=self.store_priority,
             ).attach(
                 forward_fn=self.retrieve_user_data,
                 blacklist_fn=self.retrieve_blacklist,
                 priority_fn=self.retrieve_priority,
+            ).attach(
+                forward_fn=self.delete_user_data,
+                blacklist_fn=self.delete_blacklist,
+                priority_fn=self.delete_priority,
             )
 
             try:
                 self.subtensor.serve_axon(
                     netuid=self.config.netuid,
                     axon=self.axon,
                 )
-                self.axon.start()
-
             except Exception as e:
                 bt.logging.error(f"Failed to serve Axon: {e}")
                 pass
 
+            self.axon.start()
+
         except Exception as e:
             bt.logging.error(f"Failed to create Axon initialize: {e}")
             pass
 
         # Dendrite pool for querying the network.
         bt.logging.debug("loading dendrite_pool")
         if self.config.neuron.mock:
             self.dendrite = MockDendrite()  # TODO: fix this import error
         else:
-            self.dendrite = bt.dendrite(wallet=self.wallet)
+            self.dendrite = timed_dendrite(wallet=self.wallet)
         bt.logging.debug(str(self.dendrite))
 
         # Init the event loop.
         self.loop = asyncio.get_event_loop()
 
         self.prev_step_block = get_current_block(self.subtensor)
 
@@ -277,23 +288,29 @@
         # Otherwise, reject.
         return (
             True,
             f"Hotkey {synapse.dendrite.hotkey} not whitelisted or in top n% stake.",
         )
 
     async def store_priority(self, synapse: protocol.StoreUser) -> float:
+        if self.config.api.open_access or synapse.dendrite.hotkey in self.config.api.whitelisted_hotkeys:
+            return 1.0
+
         caller_uid = self.metagraph.hotkeys.index(
             synapse.dendrite.hotkey
         )  # Get the caller index.
+
         priority = float(
             self.metagraph.S[caller_uid]
         )  # Return the stake as the priority.
+
         bt.logging.trace(
             f"Prioritizing {synapse.dendrite.hotkey} with value: ", priority
         )
+
         return priority
 
     async def retrieve_user_data(
         self, synapse: protocol.RetrieveUser
     ) -> protocol.RetrieveUser:
         """
         Asynchronously handles the retrieval of user data from the network based on a given hash.
@@ -355,23 +372,97 @@
         # Otherwise, reject.
         return (
             True,
             f"Hotkey {synapse.dendrite.hotkey} not whitelisted or in top n% stake.",
         )
 
     async def retrieve_priority(self, synapse: protocol.RetrieveUser) -> float:
+        if self.config.api.open_access or synapse.dendrite.hotkey in self.config.api.whitelisted_hotkeys:
+            return 1.0
+
+        caller_uid = self.metagraph.hotkeys.index(
+            synapse.dendrite.hotkey
+        )  # Get the caller index.
+
+        priority = float(
+            self.metagraph.S[caller_uid]
+        )  # Return the stake as the priority.
+
+        bt.logging.trace(
+            f"Prioritizing {synapse.dendrite.hotkey} with value: ", priority
+        )
+
+        return priority
+
+    async def delete_user_data(self, synapse: protocol.DeleteUser) -> protocol.DeleteUser:
+        """
+        Asynchronously handles the deletion of user data from the network based on a given hash.
+        It deletes the data and updates the synapse object with the deletion status.
+
+        Parameters:
+            synapse (protocol.DeleteUser): An instance of the DeleteUser protocol class containing
+                                        the hash of the data to be deleted.
+
+        Returns:
+            protocol.DeleteUser: The updated instance of the DeleteUser protocol class with the
+                                deletion status.
+
+        Note:
+            - The function is part of a larger protocol for data deletion in a distributed network.
+            - It utilizes the 'delete_broadband' method to perform the actual data deletion based
+            on the provided data hash.
+            - The method logs the deletion process and the resulting status for monitoring and debugging.
+        """
+        metadata = await get_ordered_metadata(synapse.data_hash, self.database)
+
+        if not metadata:
+            bt.logging.warning(f"Hash {synapse.data_hash} does not exist on the network.")
+            synapse.deleted = False
+            return synapse
+
+        bt.logging.trace(metadata)
+
+        await delete_file_from_database(synapse.data_hash, self.database)
+        synapse.deleted = True
+
+        return synapse
+
+    async def delete_blacklist(
+        self, synapse: protocol.DeleteUser
+    ) -> typing.Tuple[bool, str]:
+        # If debug mode, whitelist everything (NOT RECOMMENDED)
+        if self.config.api.open_access:
+            return False, "Open access: WARNING all whitelisted"
+
+        # If explicitly whitelisted hotkey, allow.
+        if synapse.dendrite.hotkey in self.config.api.whitelisted_hotkeys:
+            return False, f"Hotkey {synapse.dendrite.hotkey} whitelisted."
+
+        # Otherwise, reject.
+        return (
+            True,
+            f"Hotkey {synapse.dendrite.hotkey} not whitelisted or in top n% stake.",
+        )
+
+    async def delete_priority(self, synapse: protocol.DeleteUser) -> float:
+        if self.config.api.open_access or synapse.dendrite.hotkey in self.config.api.whitelisted_hotkeys:
+            return 1.0
+
         caller_uid = self.metagraph.hotkeys.index(
             synapse.dendrite.hotkey
         )  # Get the caller index.
+
         priority = float(
             self.metagraph.S[caller_uid]
         )  # Return the stake as the priority.
+
         bt.logging.trace(
             f"Prioritizing {synapse.dendrite.hotkey} with value: ", priority
         )
+
         return priority
 
     def run(self):
         bt.logging.info("run()")
         if self.wallet.hotkey.ss58_address not in self.metagraph.hotkeys:
             raise Exception(
                 f"API is not registered - hotkey {self.wallet.hotkey.ss58_address} not in metagraph"
@@ -458,12 +549,14 @@
             traceback: A traceback object encoding the stack trace.
                        None if the context was exited without an exception.
         """
         self.stop_run_thread()
 
 
 def run_api():
-    neuron().run()
+    neuron_obj = neuron()
+    run_indexer_thread(neuron_obj.config)
+    neuron_obj.run()
 
 
 if __name__ == "__main__":
     run_api()
```

### Comparing `FileTAO-2.1.0/neurons/miner.py` & `FileTAO-3.0.0/neurons/miner.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,20 +126,29 @@
 
     def __init__(self):
         self.config = miner.config()
         self.check_config(self.config)
         bt.logging(config=self.config, logging_dir=self.config.miner.full_path)
         bt.logging.info(f"{self.config}")
 
-        try:
-            asyncio.run(check_environment(self.config.database.redis_conf_path))
-        except AssertionError as e:
-            bt.logging.warning(
-                f"Something is missing in your environment: {e}. Please check your configuration, use the README for help, and try again."
-            )
+        redis_password = get_redis_password(self.config.database.redis_password)
+        if self.config.database.native_environment_check:
+            try:
+                asyncio.run(check_environment(
+                    self.config.database.redis_conf_path,
+                    self.config.database.host,
+                    self.config.database.port,
+                    redis_password
+                ))
+            except AssertionError as e:
+                bt.logging.warning(
+                    f"Something is missing in your environment: {e}. Please check your configuration, use the README for help, and try again."
+                )
+        else:
+            bt.logging.info("Skipping environment checks.")
 
         bt.logging.info("miner.__init__()")
 
         # Init device.
         bt.logging.debug("loading device")
         self.device = torch.device(self.config.miner.device)
         bt.logging.debug(str(self.device))
@@ -165,15 +174,14 @@
             netuid=self.config.netuid, network=self.subtensor.network, sync=False
         )  # Make sure not to sync without passing subtensor
         self.metagraph.sync(subtensor=self.subtensor)  # Sync metagraph with subtensor.
         bt.logging.debug(str(self.metagraph))
 
         # Setup database
         bt.logging.info("loading database")
-        redis_password = get_redis_password(self.config.database.redis_password)
         self.database = aioredis.StrictRedis(
             host=self.config.database.host,
             port=self.config.database.port,
             db=self.config.database.index,
             socket_keepalive=True,
             socket_connect_timeout=300,
             password=redis_password,
@@ -720,14 +728,16 @@
         data = await get_chunk_metadata(
             r=self.database,
             chunk_hash=synapse.challenge_hash,
             hotkey=synapse.dendrite.hotkey,
         )
         if data is None:
             bt.logging.error(f"No data found for {synapse.challenge_hash}")
+            synapse.axon.status_code = 404
+            synapse.axon.status_message = "File metadata not found"
             return synapse
 
         bt.logging.trace(f"retrieved data: {pformat(data)}")
 
         # Chunk the data according to the specified (random) chunk size
         filepath = data.get("filepath", None)
         if filepath is None:
@@ -769,18 +779,17 @@
             return synapse
 
         # Construct the next commitment hash using previous commitment and hash
         # of the data to prove storage over time
         prev_seed = data.get("seed", "").encode()
         bt.logging.debug(f"challenge() prev_seed: {prev_seed}")
         if prev_seed is None:
-            # TODO: this should raise an error that would trigger a 404 response in the axon
-            # Currently, the synapse logs show this as successful, because axon recieves a synapse without
-            # errors. This is a bug and should be addressed in bittensor.
             bt.logging.error(f"No seed found for {synapse.challenge_hash}")
+            synapse.axon.status_code = 404
+            synapse.axon.status_message = "Previous seed not found"
             return synapse
 
         bt.logging.trace("entering comput_subsequent_commitment()...")
         new_seed = synapse.seed.encode()
         next_commitment, proof = compute_subsequent_commitment(
             encrypted_data_bytes, prev_seed, new_seed, verbose=self.config.miner.verbose
         )
@@ -789,15 +798,15 @@
             bt.logging.debug(f"new seed  : {new_seed}")
             bt.logging.debug(f"proof     : {proof}")
             bt.logging.debug(f"commitment: {next_commitment}\n")
         synapse.commitment_hash = next_commitment
         synapse.commitment_proof = proof
 
         # update the commitment seed challenge hash in storage
-        bt.logging.trace(f"udpating challenge miner storage: {pformat(data)}")
+        bt.logging.trace(f"updating challenge miner storage: {pformat(data)}")
         await update_seed_info(
             self.database,
             chunk_hash=synapse.challenge_hash,
             hotkey=synapse.dendrite.hotkey,
             seed=new_seed.decode("utf-8"),
         )
 
@@ -941,15 +950,15 @@
         bt.logging.trace("entering update_seed_info()")
         await update_seed_info(
             self.database,
             chunk_hash=synapse.data_hash,
             hotkey=synapse.dendrite.hotkey,
             seed=synapse.seed,
         )
-        bt.logging.debug(f"udpated retrieve miner storage: {pformat(data)}")
+        bt.logging.debug(f"updated retrieve miner storage: {pformat(data)}")
 
         # Return base64 data
         bt.logging.trace("entering b64_encode()")
         synapse.data = base64.b64encode(encrypted_data_bytes)
         bt.logging.info(f"returning retrieved data {synapse.data[:24]}...")
         return synapse
```

### Comparing `FileTAO-2.1.0/neurons/validator.py` & `FileTAO-3.0.0/neurons/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     log_event,
 )
 from storage.validator.weights import (
     set_weights_for_validator,
 )
 from storage.validator.forward import forward
 from storage.validator.encryption import setup_encryption_wallet
+from storage.validator.dendrite import timed_dendrite
 
 load_dotenv()
 
 
 def MockDendrite():
     pass
 
@@ -96,16 +97,22 @@
 
     def __init__(self):
         self.config = neuron.config()
         self.check_config(self.config)
         bt.logging(config=self.config, logging_dir=self.config.neuron.full_path)
         print(self.config)
 
+        redis_password = get_redis_password(self.config.database.redis_password)
         try:
-            asyncio.run(check_environment(self.config.database.redis_conf_path))
+            asyncio.run(check_environment(
+                self.config.database.redis_conf_path,
+                self.config.database.host,
+                self.config.database.port,
+                redis_password
+            ))
         except AssertionError as e:
             bt.logging.warning(
                 f"Something is missing in your environment: {e}. Please check your configuration, use the README for help, and try again."
             )
 
         bt.logging.info("neuron.__init__()")
 
@@ -151,15 +158,14 @@
         bt.logging.debug(str(self.metagraph))
 
         # Get initial block
         self.current_block = self.subtensor.get_current_block()
 
         # Setup database
         bt.logging.info("loading database")
-        redis_password = get_redis_password(self.config.database.redis_password)
         self.database = aioredis.StrictRedis(
             host=self.config.database.host,
             port=self.config.database.port,
             db=self.config.database.index,
             password=redis_password,
         )
         self.db_semaphore = asyncio.Semaphore()
@@ -175,15 +181,16 @@
         bt.logging.info(f"Running validator on uid: {self.my_subnet_uid}")
 
         # Dendrite pool for querying the network.
         bt.logging.debug("loading dendrite_pool")
         if self.config.neuron.mock_dendrite_pool:
             self.dendrite = MockDendrite()
         else:
-            self.dendrite = bt.dendrite(wallet=self.wallet)
+            self.dendrite = timed_dendrite(wallet=self.wallet)
+
         bt.logging.debug(str(self.dendrite))
 
         # Init the event loop.
         self.loop = asyncio.get_event_loop()
 
         self.wandb = None
 
@@ -351,23 +358,24 @@
             block_hash = substrate.get_block_hash(block_id=block_no)
             bt.logging.debug(f"subscription block hash: {block_hash}")
             events = substrate.get_events(block_hash)
 
             for event in events:
                 event_dict = event["event"].decode()
                 if event_dict["event_id"] == "NeuronRegistered":
-                    netuid, uid, hotkey = event_dict["attributes"]
+                    netuid, uid, new_hotkey = event_dict["attributes"]
                     if int(netuid) == 21:
                         self.log(
                             f"NeuronRegistered Event {uid}! Rebalancing data...\n"
                             f"{pformat(event_dict)}\n"
                         )
-
+                        replaced_hotkey = self.metagraph.hotkeys[uid]
                         self.last_registered_block = block_no
-                        self.rebalance_queue.append(hotkey)
+                        self.rebalance_queue.append(replaced_hotkey)
+                        self.metagraph.hotkeys[uid] = new_hotkey
 
             # If we have some hotkeys deregistered, and it's been 5 blocks since we've caught a registration: rebalance
             if (
                 len(self.rebalance_queue) > 0
                 and self.last_registered_block + 5 <= block_no
             ):
                 hotkeys = deepcopy(self.rebalance_queue)
```

### Comparing `FileTAO-2.1.0/setup.py` & `FileTAO-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     long_description_content_type="text/markdown",
     url="https://github.com/ifrit98/storage-subnet",
     author="philanthrope",
     packages=find_packages(),
     include_package_data=True,
     author_email="ifrit98@gmail.com",
     license="MIT",
-    python_requires=">=3.9,<3.11",
+    python_requires=">=3.9,<3.12",
     entry_points={
         "console_scripts": [
             "filetao=storage.cli.cli:filetao"
         ]
     },
     install_requires=requirements,
     extras_require={"dev": extra_requirements_dev},
@@ -84,14 +84,15 @@
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
```

### Comparing `FileTAO-2.1.0/storage/__init__.py` & `FileTAO-3.0.0/storage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,18 +47,19 @@
         return (self.major, self.minor, self.patch) < (
             other.major,
             other.minor,
             other.patch,
         )
 
 
-__version__ = "2.1.0"
+__version__ = "3.0.0"
 version = StorageVersion.from_string(__version__)
 __spec_version__ = version.to_spec_version()
 
 # Import all submodules.
 from . import protocol
 from . import validator
 from . import miner
 from . import plot
 from . import cli
-from . import api
+from . import api
+from . import indexer
```

### Comparing `FileTAO-2.1.0/storage/api/example.py` & `FileTAO-3.0.0/storage/api/example.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 import random
 import bittensor as bt
-from storage.api import store, retrieve
+from storage.api import store, retrieve, delete
 from storage.api import StoreUserAPI, RetrieveUserAPI, get_query_api_axons
 bt.trace()
 
 # Example usage
 async def test_storage_abstraction():
     # setup wallet and subtensor connection
     wallet = bt.wallet()
@@ -53,21 +53,29 @@
     print("Stored {} with {} hotkeys".format(cid, hotkeys))
 
     time.sleep(5)
     bt.logging.info(f"Now retrieving data with CID: {cid}")
     retrieve_handler = RetrieveUserAPI(wallet)
     rdata = await retrieve_handler(
         axons=axons,
-        # Arugmnts for the proper synapse
+        # Arguments for the proper synapse
         cid=cid,
         timeout=60,
     )
     print(rdata)
     assert raw_data == rdata
 
 
+async def test_delete():
+    cid = "bafkreiej3j74ywl3j2nsjxlrzj2jkyz2di7yahy4ilnfjjnkerrv76js6m"
+    hotkeys = ["5C86aJ2uQawR6P6veaJQXNK9HaWh6NMbUhTiLs65kq4ZW3NH"]
+    wallet = bt.wallet()
+    subtensor = bt.subtensor("test")
+    await delete(cid, wallet, subtensor, hotkeys=hotkeys, netuid=22)
+
+
 if __name__ == "__main__":
     import asyncio
     print("Starting test of high level storage abstraction")
     asyncio.run(test_storage_abstraction())
     print("Starting test of storage primitives")
     asyncio.run(test_storage_primitives())
```

### Comparing `FileTAO-2.1.0/storage/api/store_api.py` & `FileTAO-3.0.0/storage/api/store_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,27 +13,32 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
+import os
 import torch
 import base64
 import random
+import asyncio
 import bittensor as bt
 from abc import ABC, abstractmethod
 from typing import Any, List, Union
 from storage.protocol import StoreUser
 from storage.validator.cid import generate_cid_string
 from storage.validator.encryption import encrypt_data
+from storage.api.base import Subnet21API
 from storage.api.utils import get_query_api_axons
+from storage.cli.default_values import defaults
+from storage.shared.utils import get_coldkey_wallets_for_path, get_hash_mapping, save_hash_mapping
 
 
-class StoreUserAPI(bt.SubnetsAPI):
+class StoreUserAPI(Subnet21API):
     def __init__(self, wallet: "bt.wallet"):
         super().__init__(wallet)
         self.netuid = 21
 
     def prepare_synapse(
         self, data: bytes, encrypt=False, ttl=60 * 60 * 24 * 30, encoding="utf-8"
     ) -> StoreUser:
@@ -92,53 +97,72 @@
     wallet: "bt.wallet",
     subtensor: "bt.subtensor" = None,
     chain_endpoint: str = "finney",
     netuid: int = 21,
     ttl: int = 60 * 60 * 24 * 30,
     encrypt: bool = False,
     encoding: str = "utf-8",
-    timeout: int = 60,
+    timeout: int = 100,
     uid: int = None,
+    metadata_path: str = None,
+    name: str = None,
+    max_retries: int = 3,
+    backoff_factor: float = 2.0,
 ):
 
     """
-    Stores data on the Bittensor network.
+    Stores data on the FileTAO network.
     
     Args:
         data (bytes): The data to store.
         wallet (bittensor.wallet): The wallet instance to use for storing data.
         subtensor (bittensor.subtensor, optional): The subtensor instance to use for storing data. Defaults to None.
         chain_endpoint (str, optional): The chain endpoint to use for storing data. Defaults to "finney".
         netuid (int, optional): The netuid to use for storing data. Defaults to 21.
         ttl (int, optional): The time-to-live for the stored data. Defaults to 60 * 60 * 24 * 30.
         encrypt (bool, optional): Whether to encrypt the data. Defaults to False.
         encoding (str, optional): The encoding of the data. Defaults to "utf-8".
         timeout (int, optional): The timeout in seconds for storing data. Defaults to 60.
         uid (int, optional): The UID of a specific API node to use for storing data. Defaults to None.
+        metadata_path (str, optionla): The path to store the metadata object for associating hotkeys.
+        name (str, optional): String name of the data to associate with metadata.
 
     Returns:
         str: The CID of the stored data.
         hotkeys: The hotkeys of the successfully stored data.
     """
-    store_handler = StoreUserAPI(wallet)
+    retry_count = 0
+    delay = 2
 
-    subtensor = subtensor or bt.subtensor(chain_endpoint)
-    metagraph = subtensor.metagraph(netuid=netuid)
+    while retry_count < max_retries:
+        try:
+            store_handler = StoreUserAPI(wallet)
+            subtensor = subtensor or bt.subtensor(chain_endpoint)
+            metagraph = subtensor.metagraph(netuid=netuid)
+
+            uids = [uid] if uid is not None else None
+            all_axons = await get_query_api_axons(wallet=wallet, metagraph=metagraph, uids=uids)
+            axons = random.choices(all_axons, k=min(3, len(all_axons)))
+
+            cid, hotkeys = await store_handler(
+                axons=axons,
+                data=data,
+                encrypt=encrypt,
+                ttl=ttl,
+                encoding=encoding,
+                uid=uid,
+                timeout=timeout,
+            )
 
-    uids = None
-    if uid is not None:
-        uids = [uid]
-
-    all_axons = await get_query_api_axons(wallet=wallet, metagraph=metagraph, uids=uids)
-    axons = random.choices(all_axons, k=3)
-
-    cid, hotkeys = await store_handler(
-        axons=axons,
-        data=data,
-        encrypt=encrypt,
-        ttl=ttl,
-        encoding=encoding,
-        uid=uid,
-        timeout=timeout,
-    )
+            if cid != "" and hotkeys:
+                metadata_path = os.path.expanduser(metadata_path or defaults.hash_basepath)
+                hash_filepath = os.path.join(metadata_path, wallet.name + ".json")
+                save_hash_mapping(hash_filepath, name or cid, cid, hotkeys)
+                return cid, hotkeys
+        except Exception as e:
+            print(f"Attempt {retry_count + 1} failed: {str(e)}")
+
+        await asyncio.sleep(delay)
+        delay *= backoff_factor
+        retry_count += 1
 
-    return cid, hotkeys
+    raise Exception("Maximum retry limit reached without success.")
```

### Comparing `FileTAO-2.1.0/storage/api/utils.py` & `FileTAO-3.0.0/storage/api/utils.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/cli/__init__.py` & `FileTAO-3.0.0/storage/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/cli/cli.py` & `FileTAO-3.0.0/storage/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,23 +70,23 @@
         "aliases": ["m", "miner"],
         "help": "Commands for retrieving statistics from the Bittensor network.",
         "commands": {
             "stats": ListMinerStats,  # lists all miner stats associated with hotkey
         },
     },
     "run": {
-         "name": "run",
-         "aliases": ["n", "run"],
-         "help": "Commands for running neurons in this subnetwork.",
-         "commands": {
-             "miner": RunMiner,
-             "validator": RunValidator,
-             "api": RunApi,
-         },
-     },
+        "name": "run",
+        "aliases": ["n", "run"],
+        "help": "Commands for running neurons in this subnetwork.",
+        "commands": {
+            "miner": RunMiner,
+            "validator": RunValidator,
+            "api": RunApi,
+        },
+    },
 }
 
 
 class cli:
     """
     Implementation of the Command Line Interface (CLI) class for the Bittensor protocol.
     This class handles operations like key management (hotkey and coldkey) and token transfer.
@@ -228,13 +228,14 @@
                 await command_data["commands"][self.config["subcommand"]].run(self)
             else:
                 await command_data.run(self)
         else:
             print(f":cross_mark:[red]Unknown command: {self.config.command}[/red]")
             sys.exit()
 
-async def async_main(args):
-    await cli(args=args).run()
+async def async_main(config):
+    await cli(config=config).run()
 
 def filetao():
     args = sys.argv[1:]
-    asyncio.run(async_main(args=args))
+    config = cli.create_config(args)
+    asyncio.run(async_main(config=config))
```

### Comparing `FileTAO-2.1.0/storage/cli/default_values.py` & `FileTAO-3.0.0/storage/cli/default_values.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/cli/listcommand.py` & `FileTAO-3.0.0/storage/cli/listcommand.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/cli/neuroncommand.py` & `FileTAO-3.0.0/storage/cli/neuroncommand.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/cli/retrievecommand.py` & `FileTAO-3.0.0/storage/cli/retrievecommand.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,54 +21,28 @@
 import torch
 import base64
 import argparse
 
 import storage
 from storage.validator.encryption import decrypt_data_with_private_key
 from storage.api.retrieve_api import retrieve
+from storage.shared.utils import list_all_hashes
 
 import bittensor
 
 from typing import List
 from rich.prompt import Prompt
 
 from .default_values import defaults
 
 
 # Create a console instance for CLI display.
 console = bittensor.__console__
 
 
-def list_all_hashes(hash_file):
-    try:
-        with open(os.path.expanduser(hash_file), "r") as file:
-            hashes = json.load(file)
-            return hashes
-    except (FileNotFoundError, json.JSONDecodeError):
-        return {}
-
-
-def get_coldkey_wallets_for_path(path: str) -> List["bittensor.wallet"]:
-    try:
-        wallet_names = next(os.walk(os.path.expanduser(path)))[1]
-        return [bittensor.wallet(path=path, name=name) for name in wallet_names]
-    except StopIteration:
-        # No wallet files found.
-        wallets = []
-    return wallets
-
-
-def get_hash_mapping(hash_file, filename):
-    try:
-        with open(os.path.expanduser(hash_file), "r") as file:
-            hashes = json.load(file)
-            return hashes.get(filename)
-    except (FileNotFoundError, json.JSONDecodeError):
-        return None
-
 
 class RetrieveData:
     """
     Executes the 'get' command to retrieve data from the Bittensor network using a specific data hash.
     This command is crucial for users who wish to access data stored on the network using its unique identifier.
 
     Usage:
@@ -125,14 +99,18 @@
                 bittensor.logging.debug(f"hashes dict: {hashes_dict}")
                 reverse_hashes_dict = {v: k for k, v in hashes_dict.items() if "hotkeys" not in k}
                 if cli.config.cid in reverse_hashes_dict:
                     filename = reverse_hashes_dict[cli.config.cid]
                     outpath = os.path.join(base_outpath, filename)
                     bittensor.logging.debug(f"set filename: {filename}")
                     hotkeys = hashes_dict[filename + "_hotkeys"]
+                else:
+                    hotkeys = []
+            else:
+                hotkeys = []
 
         except Exception as e:
             bittensor.logging.warning(
                 "Failed to lookup filename for CID: {} ".format(e),
                 "Reverting to hash value as filename {outpath}",
             )
 
@@ -156,14 +134,15 @@
 
             data = await retrieve(
                 cli.config.cid,
                 wallet,
                 sub,
                 netuid=cli.config.netuid,
                 hotkeys=hotkeys,
+                uids=cli.config.uids,
             )
 
             success = True
 
         if success:
             # Save the data
             with open(outpath, "wb") as f:
@@ -235,11 +214,17 @@
         )
         retrieve_parser.add_argument(
             "--netuid",
             type=str,
             default=defaults.netuid,
             help="Network identifier for the Bittensor network.",
         )
+        retrieve_parser.add_argument(
+            "--uids",
+            type=int,
+            nargs="+",
+            help="Validator API UID to ping directly if known apriori.",
+        )
 
         bittensor.wallet.add_args(retrieve_parser)
         bittensor.subtensor.add_args(retrieve_parser)
         bittensor.logging.add_args(retrieve_parser)
```

### Comparing `FileTAO-2.1.0/storage/cli/statscommand.py` & `FileTAO-3.0.0/storage/cli/statscommand.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/cli/storecommand.py` & `FileTAO-3.0.0/storage/cli/storecommand.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import argparse
 
 import storage
 from storage.validator.encryption import encrypt_data
 from storage.validator.cid import generate_cid_string
 from storage.shared.ecc import hash_data
 from storage.api.store_api import store
+from storage.shared.utils import get_coldkey_wallets_for_path, get_hash_mapping, save_hash_mapping
 
 import bittensor
 
 from typing import List
 from rich.prompt import Prompt
 from storage.validator.utils import get_all_validators
 
@@ -40,59 +41,14 @@
 bittensor.trace()
 
 
 # Create a console instance for CLI display.
 console = bittensor.__console__
 
 
-def get_coldkey_wallets_for_path(path: str) -> List["bittensor.wallet"]:
-    try:
-        wallet_names = next(os.walk(os.path.expanduser(path)))[1]
-        return [bittensor.wallet(path=path, name=name) for name in wallet_names]
-    except StopIteration:
-        # No wallet files found.
-        wallets = []
-    return wallets
-
-
-def get_hash_mapping(hash_file, filename):
-    try:
-        with open(os.path.expanduser(hash_file), "r") as file:
-            hashes = json.load(file)
-            return hashes.get(filename)
-    except (FileNotFoundError, json.JSONDecodeError):
-        return None
-
-
-def save_hash_mapping(hash_file: str, filename: str, data_hash: str, hotkeys: List[str]):
-    base_dir = os.path.basename(hash_file)
-    if not os.path.exists(base_dir):
-        os.makedirs(base_dir)
-
-    try:
-        with open(hash_file, "r") as file:
-            hashes = json.load(file)
-    except (FileNotFoundError, json.JSONDecodeError):
-        hashes = {}
-
-    hashes[filename] = data_hash
-    hashes[filename + "_hotkeys"] = hotkeys
-
-    with open(hash_file, "w") as file:
-        json.dump(hashes, file)
-
-
-def list_all_hashes(hash_file):
-    try:
-        with open(hash_file, "r") as file:
-            hashes = json.load(file)
-            return hashes
-    except (FileNotFoundError, json.JSONDecodeError):
-        return {}
-
 
 class StoreData:
     """
     Executes the 'put' command to store data from the local disk on the Bittensor network.
     This command is essential for users who wish to upload and store data securely on the network.
 
     Usage:
@@ -170,14 +126,15 @@
                     wallet=wallet,
                     subtensor=subtensor,
                     netuid=cli.config.netuid,
                     ttl=cli.config.ttl,
                     encrypt=cli.config.encrypt,
                     encoding=cli.config.encoding,
                     timeout=cli.config.timeout,
+                    uid=cli.config.uid,
                 )
 
             if len(stored_hotkeys) > 0:
                 bittensor.logging.info(
                     f"Stored data with hotkeys: {stored_hotkeys}."
                 )
                 success = True
@@ -273,11 +230,16 @@
         )
         store_parser.add_argument(
             "--timeout",
             type=int,
             default=180,
             help="Timeout for the complete storage request on the Bittensor network.",
         )
+        store_parser.add_argument(
+            "--uid",
+            type=int,
+            help="UID of validator API to ping directly",
+        )
 
         bittensor.wallet.add_args(store_parser)
         bittensor.subtensor.add_args(store_parser)
         bittensor.logging.add_args(store_parser)
```

### Comparing `FileTAO-2.1.0/storage/constants.py` & `FileTAO-3.0.0/storage/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,51 @@
 # Failure mode negative rewards
 STORE_FAILURE_REWARD = 0
 CHALLENGE_FAILURE_REWARD = 0
 MONITOR_FAILURE_REWARD = -0.005  # Incentivize uptime
 RETRIEVAL_FAILURE_REWARD = -0.01 # Incentivize keeping all data
 
 # Constants for storage limits in bytes
-STORAGE_LIMIT_SUPER_SAIYAN = 1024**6 * 1  # 1 EB
-STORAGE_LIMIT_DIAMOND = 1024**5 * 1       # 1 PB
-STORAGE_LIMIT_GOLD = 1024**4 * 100        # 100 TB
-STORAGE_LIMIT_SILVER = 1024**4 * 10       # 10 TB
-STORAGE_LIMIT_BRONZE = 1024**4 * 1        # 1 TB
+STORAGE_LIMIT_SUPER_SAIYAN = 1024**5 * 50 # 50 PB
+STORAGE_LIMIT_RUBY = 1024**5 * 20         # 20 PB
+STORAGE_LIMIT_EMERALD = 1024**5 * 10      # 10 PB
+STORAGE_LIMIT_DIAMOND = 1024**5 * 5       # 5 PB
+STORAGE_LIMIT_PLATINUM = 1024**5 * 1      # 1 PB
+STORAGE_LIMIT_GOLD = 1024**4 * 200        # 200 TB
+STORAGE_LIMIT_SILVER = 1024**4 * 50       # 50 TB
+STORAGE_LIMIT_BRONZE = 1024**4 * 10       # 10 TB
 
 SUPER_SAIYAN_TIER_REWARD_FACTOR = 1.0
-DIAMOND_TIER_REWARD_FACTOR = 0.9
-GOLD_TIER_REWARD_FACTOR = 0.8
-SILVER_TIER_REWARD_FACTOR = 0.7
+RUBY_TIER_REWARD_FACTOR = 0.9
+EMERALD_TIER_REWARD_FACTOR = 0.85
+DIAMOND_TIER_REWARD_FACTOR = 0.8
+PLATINUM_TIER_REWARD_FACTOR = 0.75
+GOLD_TIER_REWARD_FACTOR = 0.7
+SILVER_TIER_REWARD_FACTOR = 0.65
 BRONZE_TIER_REWARD_FACTOR = 0.6
 
-SUPER_SAIYAN_TIER_TOTAL_SUCCESSES = 10**4  # 10,000 (estimated 30 epochs to reach this tier)
-DIAMOND_TIER_TOTAL_SUCCESSES = 10**3 * 5   # 5,000  (estimated 15 epochs to reach this tier)
-GOLD_TIER_TOTAL_SUCCESSES = 10**3 * 2      # 2,000  (estimated 6  epochs to reach this tier)
-SILVER_TIER_TOTAL_SUCCESSES = 10**3        # 1,000  (estimated 3  epochs to reach this tier)
+SUPER_SAIYAN_TIER_TOTAL_SUCCESSES = 10**3 * 15 # 15,000 (estimated 72 epochs to reach this tier)
+RUBY_TIER_TOTAL_SUCCESSES = 10**3 * 10         # 10,000 (estimated 56 epochs to reach this tier)
+EMERALD_TIER_TOTAL_SUCCESSES = 10**3 * 7       # 8,000  (estimated 48 epochs to reach this tier)
+DIAMOND_TIER_TOTAL_SUCCESSES = 10**3 * 5       # 6,000  (estimated 36 epochs to reach this tier)
+PLATINUM_TIER_TOTAL_SUCCESSES = 10**3 * 3      # 4,000  (estimated 24 epochs to reach this tier)
+GOLD_TIER_TOTAL_SUCCESSES = 10**3 * 2          # 2,000  (estimated 12 epochs to reach this tier)
+SILVER_TIER_TOTAL_SUCCESSES = 10**2 * 5        # 500    (estimated 3  epochs to reach this tier)
 
-SUPER_SAIYAN_WILSON_SCORE = 0.88
-DIAMOND_WILSON_SCORE = 0.77
-GOLD_WILSON_SCORE = 0.66
+SUPER_SAIYAN_WILSON_SCORE = 0.85
+RUBY_WILSON_SCORE = 0.8
+EMERALD_WILSON_SCORE = 0.75
+DIAMOND_WILSON_SCORE = 0.7
+PLATINUM_WILSON_SCORE = 0.65
+GOLD_WILSON_SCORE = 0.6
 SILVER_WILSON_SCORE = 0.55
 
 TIER_BOOSTS = {
     b"Super Saiyan": 1.02, # 2%  -> 1.02
-    b"Diamond": 1.05,      # 5%  -> 0.945
-    b"Gold": 1.1,          # 10% -> 0.88
-    b"Silver": 1.15,       # 15% -> 0.805
+    b"Ruby": 1.04,         # 4%  -> 0.936
+    b"Emerald": 1.05,      # 6%  -> 0.918
+    b"Diamond": 1.08,      # 8%  -> 0.864
+    b"Platinum": 1.1,      # 10% -> 0.825
+    b"Gold": 1.12,         # 12% -> 0.784
+    b"Silver": 1.16,       # 16% -> 0.754
     b"Bronze": 1.2,        # 20% -> 0.72
 }
```

### Comparing `FileTAO-2.1.0/storage/miner/__init__.py` & `FileTAO-3.0.0/storage/miner/__init__.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/miner/config.py` & `FileTAO-3.0.0/storage/miner/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,21 @@
     )
     parser.add_argument(
         "--database.redis_conf_path",
         type=str,
         help="Redis configuration path.",
         default="/etc/redis/redis.conf",
     )
+    parser.add_argument(
+        "--database.skip_native_environment_check",
+        dest="database.native_environment_check",
+        action="store_false",
+        default=True,
+        help="Skip native environment check.",
+    )
 
     # Run config.
     parser.add_argument(
         "--miner.set_weights_wait_for_inclusion",
         action="store_true",
         help="Wether to wait for the set_weights extrinsic to enter a block",
         default=False,
```

### Comparing `FileTAO-2.1.0/storage/miner/database.py` & `FileTAO-3.0.0/storage/miner/database.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/miner/run.py` & `FileTAO-3.0.0/storage/miner/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
+import os
 import bittensor as bt
 from substrateinterface import SubstrateInterface
 from storage.shared.checks import check_registration
 from .utils import update_storage_stats
 
 
 def run(self):
@@ -43,14 +44,19 @@
         - The function leverages the global configurations set during the initialization of the miner.
         - The miner's axon serves as its interface to the Bittensor network, handling incoming and outgoing requests.
 
     Raises:
         KeyboardInterrupt: If the miner is stopped by a manual interruption.
         Exception: For unforeseen errors during the miner's operation, which are logged for diagnosis.
     """
+
+    data_directory = os.path.expanduser(self.config.database.directory)
+    if not os.path.exists(data_directory):
+        os.makedirs(data_directory)
+
     block_handler_substrate = SubstrateInterface(
         ss58_format=bt.__ss58_format__,
         use_remote_preset=True,
         url=self.subtensor.chain_endpoint,
         type_registry=bt.__type_registry__,
     )
```

### Comparing `FileTAO-2.1.0/storage/miner/set_weights.py` & `FileTAO-3.0.0/storage/miner/set_weights.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/miner/utils.py` & `FileTAO-3.0.0/storage/miner/utils.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/plot/utils.py` & `FileTAO-3.0.0/storage/plot/utils.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/protocol.py` & `FileTAO-3.0.0/storage/protocol.py`

 * *Files 3% similar despite different names*

```diff
@@ -194,7 +194,21 @@
 
     required_hash_fields: typing.List[str] = pydantic.Field(
         ["data_hash"],
         title="Required Hash Fields",
         description="A list of required fields for the hash.",
         allow_mutation=False,
     )
+
+
+class DeleteUser(bt.Synapse):
+    # Where to find the data
+    data_hash: str  # Miner storage lookup key
+
+    deleted: bool = False
+
+    required_hash_fields: typing.List[str] = pydantic.Field(
+        ["data_hash"],
+        title="Required Hash Fields",
+        description="A list of required fields for the hash.",
+        allow_mutation=False,
+    )
```

### Comparing `FileTAO-2.1.0/storage/shared/__init__.py` & `FileTAO-3.0.0/storage/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/shared/checks.py` & `FileTAO-3.0.0/storage/shared/checks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,95 @@
+from __future__ import annotations
+
 import subprocess
 import time
 import asyncio
 import re
 import os
 import bittensor as bt
 from redis import asyncio as aioredis
 
+from storage.shared.utils import is_running_in_docker
+
 
-async def check_environment(redis_conf_path: str = "/etc/redis/redis.conf"):
-    redis_port = 6379
-    _check_redis_config(redis_conf_path)
-    _check_redis_settings(redis_conf_path)
-    _assert_setting_exists(redis_conf_path, "requirepass")
-    await _check_redis_connection(redis_conf_path, redis_port)
-    await _check_data_persistence(redis_conf_path, redis_port)
+async def check_environment(
+    redis_conf_path: str | None = "/etc/redis/redis.conf",
+    redis_host: str = "localhost",
+    redis_port: int = 6379,
+    redis_password: str = "nopasswd",
+    skip_native_env_redis_checks: bool = False,
+):
+    """
+    Check the environment for the required settings and configurations.
+
+    :param redis_conf_path: The path to the Redis configuration file. Can be `None` if non-local Redis is used.
+    :param redis_host: The host name of the Redis server.
+    :param redis_port: The port number of the Redis server.
+    :param redis_password: The password to use when connecting to Redis.
+    :param skip_native_env_redis_checks: Skip the native environment checks that assume Redis is running on
+                                         the same machine.
+    """
+    await _check_redis_connection(redis_conf_path, redis_host, redis_port, redis_password)
+    skip_native_env_redis_checks = skip_native_env_redis_checks or is_running_in_docker()
+    if redis_conf_path and not skip_native_env_redis_checks:
+        _check_redis_config(redis_conf_path)
+        _check_redis_settings(redis_conf_path)
+        _assert_setting_exists(redis_conf_path, "requirepass")
+        await _check_data_persistence(redis_conf_path, redis_host, redis_port, redis_password)
 
 
 def _check_redis_config(path):
+    cmd = ["test", "-f", path] if is_running_in_docker() else ["sudo", "test", "-f", path]
     try:
-        subprocess.run(["sudo", "test", "-f", path], check=True)
+        subprocess.run(cmd, check=True)
     except subprocess.CalledProcessError:
         raise AssertionError(f"Redis config file path: '{path}' does not exist.")
 
 
 def _check_redis_settings(redis_conf_path):
     settings_to_check = [
         ("appendonly", ["appendonly yes"]),
-        ("save", ['save ""']),
     ]
 
     for setting, expected_values in settings_to_check:
         _check_redis_setting(redis_conf_path, setting, expected_values)
 
 
-async def _check_redis_connection(redis_conf_path, port):
-    redis_password = _get_redis_password(redis_conf_path)
-
+async def _check_redis_connection(redis_conf_path, host, port, passwd):
     assert port is not None, "Redis server port not found"
     try:
         client = aioredis.StrictRedis(
-            port=port, db=0, password=redis_password, socket_connect_timeout=1
+            host=host,
+            port=port, db=0,
+            password=passwd, socket_connect_timeout=1
         )
         await client.ping()
     except Exception as e:
         assert False, f"Redis connection failed. ConnectionError'{e}'"
 
 
-async def _check_data_persistence(redis_conf_path, port):
-    redis_password = _get_redis_password(redis_conf_path)
-
+async def _check_data_persistence(redis_conf_path, host, port, passwd):
     assert port is not None, "Redis server port not found"
-    client = aioredis.StrictRedis(port=port, db=0, password=redis_password)
+    client = aioredis.StrictRedis(host=host, port=port, db=0, password=passwd)
 
     # Insert data into Redis
     await client.set("testkey", "Hello, Redis!")
 
     # Restart Redis server
-    subprocess.run(["sudo", "systemctl", "restart", "redis-server.service"], check=True)
+    cmd = [
+        "sudo", "systemctl", "restart", "redis-server.service"
+    ]
+    subprocess.run(cmd, check=True)
 
     # Wait a bit to ensure Redis has restarted
     await asyncio.sleep(5)
 
     # Reconnect to Redis
     assert port is not None, "Redis server port not found after restart"
-    new_redis = aioredis.StrictRedis(port=port, db=0, password=redis_password)
+    new_redis = aioredis.StrictRedis(port=port, db=0, password=passwd)
 
     # Retrieve data from Redis
     value = await new_redis.get("testkey")
 
     # Clean up
     await new_redis.delete("testkey")
 
@@ -92,17 +114,20 @@
     actual_values = _get_redis_setting(file_path, setting)
     assert actual_values is not None, f"Redis config missing setting '{setting}'"
     return actual_values
 
 
 def _get_redis_setting(file_path, setting):
     """Retrieve specific settings from the Redis configuration file."""
+    cmd = ["grep", f"^{setting}", file_path] if is_running_in_docker() else [
+        "sudo", "grep", f"^{setting}", file_path
+    ]
     try:
         result = subprocess.check_output(
-            ["sudo", "grep", f"^{setting}", file_path], text=True
+            cmd, text=True
         )
         return result.strip().split("\n")
     except subprocess.CalledProcessError:
         return None
 
 
 def _get_redis_password(redis_conf_path):
```

### Comparing `FileTAO-2.1.0/storage/shared/ecc.py` & `FileTAO-3.0.0/storage/shared/ecc.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/shared/merkle.py` & `FileTAO-3.0.0/storage/shared/merkle.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/shared/subtensor.py` & `FileTAO-3.0.0/storage/shared/subtensor.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/shared/utils.py` & `FileTAO-3.0.0/storage/shared/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,14 +22,24 @@
 import base64
 import subprocess
 import bittensor as bt
 from typing import List, Union
 from redis import asyncio as aioredis
 
 
+def is_running_in_docker():
+    if os.path.exists('/.dockerenv'):
+        return True
+    try:
+        with open('/proc/self/cgroup', 'rt') as f:
+            return any('docker' in line or 'kubepods' in line for line in f)
+    except Exception:
+        return False
+
+
 async def safe_key_search(database: aioredis.Redis, pattern: str) -> List[str]:
     """
     Safely search for keys in the database that doesn't block.
     `scan_iter` uses cursor under the hood.
     """
     return [key async for key in database.scan_iter(pattern)]
 
@@ -132,24 +142,78 @@
 
 def get_redis_password(
     redis_password: str = None, redis_conf: str = "/etc/redis/redis.conf"
 ) -> str:
     redis_password = os.getenv("REDIS_PASSWORD") or redis_password
     if redis_password is None:
         try:
+            cmd = ["grep", "-Po", "^requirepass \K.*", redis_conf] if is_running_in_docker() else ["sudo", "grep", "-Po", "^requirepass \K.*", redis_conf]
             redis_password = subprocess.check_output(
-                ["sudo", "grep", "-Po", "^requirepass \K.*", redis_conf],
+                cmd,
                 text=True,
             ).strip()
         except Exception as e:
-            bt.logging.error(
+            bt.logging.warning(
                 f"No Redis password set in Redis config file: {redis_conf}"
             )
     if redis_password == "" or redis_password is None:
-        bt.logging.error(
+        bt.logging.warning(
             "Redis password not found! This must be set as either an env var `REDIS_PASSWORD`, passed via CLI in `--database.redis_pasword`, or parsed from /etc/redis/redis.conf."
             "Please ensure it is set by running `. ./scripts/redis/set_redis_password.sh` and try again."
             f"You may also run: `sudo grep -Po '^requirepass \K.*' {redis_conf}` to discover this manually and pass to the cli."
         )
-        exit(1)
+        return None
 
     return redis_password
+
+
+def list_all_hashes(hash_file):
+    try:
+        with open(os.path.expanduser(hash_file), "r") as file:
+            hashes = json.load(file)
+            return hashes
+    except (FileNotFoundError, json.JSONDecodeError):
+        return {}
+
+
+def get_coldkey_wallets_for_path(path: str) -> List["bt.wallet"]:
+    try:
+        wallet_names = next(os.walk(os.path.expanduser(path)))[1]
+        return [bt.wallet(path=path, name=name) for name in wallet_names]
+    except StopIteration:
+        # No wallet files found.
+        wallets = []
+    return wallets
+
+
+def get_hash_mapping(hash_file, filename):
+    try:
+        with open(os.path.expanduser(hash_file), "r") as file:
+            hashes = json.load(file)
+            return hashes.get(filename)
+    except (FileNotFoundError, json.JSONDecodeError):
+        return None
+
+    try:
+        with open(os.path.expanduser(hash_file), "r") as file:
+            hashes = json.load(file)
+            return hashes.get(filename)
+    except (FileNotFoundError, json.JSONDecodeError):
+        return None
+
+
+def save_hash_mapping(hash_file: str, filename: str, data_hash: str, hotkeys: List[str]):
+    base_dir = os.path.dirname(hash_file)
+    if not os.path.exists(base_dir):
+        os.makedirs(base_dir)
+
+    try:
+        with open(hash_file, "r") as file:
+            hashes = json.load(file)
+    except (FileNotFoundError, json.JSONDecodeError):
+        hashes = {}
+
+    hashes[filename] = data_hash
+    hashes[filename + "_hotkeys"] = hotkeys
+
+    with open(hash_file, "w") as file:
+        json.dump(hashes, file)
```

### Comparing `FileTAO-2.1.0/storage/shared/weights.py` & `FileTAO-3.0.0/storage/shared/weights.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,20 +52,20 @@
         subtensor (bt.subtensor): The Bittensor object managing the blockchain connection.
         wallet (bt.wallet): The miner's wallet holding cryptographic information.
         netuid (int): The unique identifier for the chain subnet.
         uids (torch.Tensor): miners UIDs on the network.
         weights (torch.Tensor): weights to sent for UIDs on the network.
         metagraph (bt.metagraph): Bittensor metagraph.
         wandb_on (bool, optional): Flag to determine if logging to Weights & Biases is enabled. Defaults to False.
-        wait_for_inclusion (bool, optional): Wether to wait for the extrinsic to enter a block.
-        wait_for_finalization (bool, optional): Wether to wait for the extrinsic to be finalized on the chain.
+        wait_for_inclusion (bool, optional): Whether to wait for the extrinsic to enter a block.
+        wait_for_finalization (bool, optional): Whether to wait for the extrinsic to be finalized on the chain.
 
     Returns:
         success (bool):
-            flag is true if extrinsic was finalized or uncluded in the block.
+            flag is true if extrinsic was finalized or included in the block.
             If we did not wait for finalization / inclusion, the response is true.
         message (str):
             message returned by the chain.
 
     Raises:
         Exception: If there's an error while setting weights, the exception is logged for diagnosis.
     """
```

### Comparing `FileTAO-2.1.0/storage/validator/__init__.py` & `FileTAO-3.0.0/storage/validator/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,7 +28,8 @@
 from . import rebalance
 from . import challenge
 from . import retrieve
 from . import distribute
 from . import store
 from . import forward
 from . import cid
+from . import dendrite
```

### Comparing `FileTAO-2.1.0/storage/validator/bonding.py` & `FileTAO-3.0.0/storage/validator/bonding.py`

 * *Files 4% similar despite different names*

```diff
@@ -233,20 +233,38 @@
     if (
         current_wilson_score >= SUPER_SAIYAN_WILSON_SCORE
         and total_successes >= SUPER_SAIYAN_TIER_TOTAL_SUCCESSES
     ):
         bt.logging.trace(f"Setting {stats_key} to Super Saiyan tier.")
         tier = "Super Saiyan"
     elif (
+        current_wilson_score >= RUBY_WILSON_SCORE
+        and total_successes >= RUBY_TIER_TOTAL_SUCCESSES
+    ):
+        bt.logging.trace(f"Setting {stats_key} to Ruby tier.")
+        tier = "Ruby"
+    elif (
+        current_wilson_score >= EMERALD_WILSON_SCORE
+        and total_successes >= EMERALD_TIER_TOTAL_SUCCESSES
+    ):
+        bt.logging.trace(f"Setting {stats_key} to Emerald tier.")
+        tier = "Emerald"
+    elif (
         current_wilson_score >= DIAMOND_WILSON_SCORE
         and total_successes >= DIAMOND_TIER_TOTAL_SUCCESSES
     ):
         bt.logging.trace(f"Setting {stats_key} to Diamond tier.")
         tier = "Diamond"
     elif (
+        current_wilson_score >= PLATINUM_WILSON_SCORE
+        and total_successes >= PLATINUM_TIER_TOTAL_SUCCESSES
+    ):
+        bt.logging.trace(f"Setting {stats_key} to Platinum tier.")
+        tier = "Platinum"
+    elif (
         current_wilson_score >= GOLD_WILSON_SCORE
         and total_successes >= GOLD_TIER_TOTAL_SUCCESSES
     ):
         bt.logging.trace(f"Setting {stats_key} to Gold tier.")
         tier = "Gold"
     elif (
         current_wilson_score >= SILVER_WILSON_SCORE
@@ -260,16 +278,22 @@
 
     # Update the tier in the database
     await database.hset(stats_key, "tier", tier)
 
     # Update storage limit based on tier
     if tier == "Super Saiyan":
         storage_limit = STORAGE_LIMIT_SUPER_SAIYAN
+    elif tier == "Ruby":
+        storage_limit = STORAGE_LIMIT_RUBY
+    elif tier == "Emerald":
+        storage_limit = STORAGE_LIMIT_EMERALD
     elif tier == "Diamond":
         storage_limit = STORAGE_LIMIT_DIAMOND
+    elif tier == "Platinum":
+        storage_limit = STORAGE_LIMIT_PLATINUM
     elif tier == "Gold":
         storage_limit = STORAGE_LIMIT_GOLD
     elif tier == "Silver":
         storage_limit = STORAGE_LIMIT_SILVER
     else:  # Bronze
         storage_limit = STORAGE_LIMIT_BRONZE
 
@@ -321,16 +345,22 @@
     tier = await database.hget(f"stats:{ss58_address}", "tier")
 
     if tier is None:
         return BRONZE_TIER_REWARD_FACTOR
 
     if tier == b"Super Saiyan":
         factor = SUPER_SAIYAN_TIER_REWARD_FACTOR
+    elif tier == b"Ruby":
+        factor = RUBY_TIER_REWARD_FACTOR
+    elif tier == b"Emerald":
+        factor = EMERALD_TIER_REWARD_FACTOR
     elif tier == b"Diamond":
         factor = DIAMOND_TIER_REWARD_FACTOR
+    elif tier == b"Platinum":
+        factor = PLATINUM_TIER_REWARD_FACTOR
     elif tier == b"Gold":
         factor = GOLD_TIER_REWARD_FACTOR
     elif tier == b"Silver":
         factor = SILVER_TIER_REWARD_FACTOR
     else:
         factor = BRONZE_TIER_REWARD_FACTOR
```

### Comparing `FileTAO-2.1.0/storage/validator/challenge.py` & `FileTAO-3.0.0/storage/validator/challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
     axon = self.metagraph.axons[uid]
 
     response = await self.dendrite(
         [axon],
         synapse,
         deserialize=True,
-        timeout=30,
+        timeout=45,
     )
     verified = verify_challenge_with_seed(response[0], synapse.seed)
 
     if verified:
         data["prev_seed"] = synapse.seed
         await update_metadata_for_data_hash(hotkey, data_hash, data, self.database)
```

### Comparing `FileTAO-2.1.0/storage/validator/cid.py` & `FileTAO-3.0.0/storage/validator/cid.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/validator/config.py` & `FileTAO-3.0.0/storage/validator/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,21 +313,21 @@
     )
 
     # API specific
     parser.add_argument(
         "--api.store_timeout",
         type=int,
         help="Store data query timeout.",
-        default=60,
+        default=600,
     )
     parser.add_argument(
         "--api.retrieve_timeout",
         type=int,
         help="Retrieve data query timeout.",
-        default=60,
+        default=600,
     )
     parser.add_argument(
         "--api.ping_timeout",
         type=int,
         help="Ping data query timeout.",
         default=5,
     )
@@ -337,17 +337,17 @@
         type=list,
         help="List of blacklisted hotkeys.",
         default=[],
     )
     parser.add_argument(
         "--api.whitelisted_hotkeys",
         nargs="+",
-        type=list,
+        type=str,
         help="List of whitelisted hotkeys.",
-        default=[],
+        default=["5HBATntUR9FUyvrGaewMht9pU66qUbcEL9VadXF69EQhKLaZ", "5GhV9ZEY76jovhYc5cuYXPS867aY5Dinuc2GkxFGwLd62hqw"],
     )
     parser.add_argument(
         "--api.open_access",
         action="store_true",
         help="If set, we whitelist all hotkeys by default to test easily. (NOT RECOMMENDED FOR PRODUCTION)",
     )
```

### Comparing `FileTAO-2.1.0/storage/validator/database.py` & `FileTAO-3.0.0/storage/validator/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # DEALINGS IN THE SOFTWARE.
 
 import json
 import time
 from redis import asyncio as aioredis
 import asyncio
 import bittensor as bt
-from typing import Dict, List, Any, Union, Optional
+from typing import Dict, List, Any, Union, Optional, Tuple
 
 
 async def set_ttl_for_hash_and_hotkey(
     data_hash: str,
     ss58_address: str,
     database: aioredis.Redis,
     ttl: int = 60 * 60 * 24 * 30,
@@ -281,15 +281,15 @@
 async def get_metadata_for_hotkey_and_hash(
     ss58_address: str, data_hash: str, database: aioredis.Redis, verbose: bool = False
 ) -> Optional[Dict[str, Any]]:
     """
     Retrieves specific metadata from a hash in Redis for the given field_key.
 
     Parameters:
-        ss58_address (str): The hotkey assoicated.
+        ss58_address (str): The hotkey associated.
         data_hash (str): The data hash associated.
         databse (aioredis.Redis): The Redis client instance.
 
     Returns:
         The deserialized metadata as a dictionary, or None if not found.
     """
     # Get the JSON string from Redis
@@ -343,16 +343,15 @@
     Parameters:
         database (aioredis.Redis): The Redis client instance.
 
     Returns:
         A dictionary where keys are data hashes and values are lists of hotkeys associated with each data hash.
     """
     data_hashes = []
-    keys = await database.scan_iter("*")
-    for key in keys:
+    async for key in database.scan_iter("*"):
         if not key.startswith(b"file:"):
             continue
         data_hashes.append(key.decode("utf-8").split(":")[1])
 
     return data_hashes
 
 
@@ -459,21 +458,22 @@
                 f"Hotkey {hotkey} has {(limit - total_storage) // 1024**3} GB free."
             )
         return False
 
 
 async def cache_hotkeys_capacity(
     hotkeys: List[str], database: aioredis.Redis, verbose: bool = False
-):
+) -> Dict[str, Tuple[int, Optional[int]]]:
     """
     Caches the capacity information for a list of hotkeys.
 
     Parameters:
         hotkeys (list): List of hotkey strings to check.
         database (aioredis.Redis): The Redis client instance.
+        verbose (bool): A flag indicating if verbose logging is enabled.
 
     Returns:
         dict: A dictionary with hotkeys as keys and a tuple of (total_storage, limit) as values.
     """
     hotkeys_capacity = {}
 
     for hotkey in hotkeys:
@@ -493,15 +493,15 @@
                 limit = None
 
         hotkeys_capacity[hotkey] = (total_storage, limit)
 
     return hotkeys_capacity
 
 
-async def check_hotkeys_capacity(hotkeys_capacity, hotkey: str, verbose: bool = False):
+async def check_hotkeys_capacity(hotkeys_capacity, hotkey: str, verbose: bool = False) -> bool:
     """
     Checks if a hotkey is at capacity using the cached information.
 
     Parameters:
         hotkeys_capacity (dict): Dictionary with cached capacity information.
         hotkey (str): The key representing the hotkey.
 
@@ -590,15 +590,15 @@
     Calculates the total approximate size of all keys in a Redis database.
     Parameters:
         database (int): Redis database
     Returns:
         int: Total size of all keys in bytes
     """
     total_size = 0
-    async for key in await database.scan_iter("*"):
+    async for key in database.scan_iter("*"):
         size = await database.execute_command("MEMORY USAGE", key)
         if size:
             total_size += size
     return total_size
 
 
 async def store_file_chunk_mapping_ordered(
@@ -855,15 +855,15 @@
     if chunks_info is None:
         return None
 
     ordered_chunks = sorted(chunks_info.items(), key=lambda x: x[0])
     return [chunk_info for _, chunk_info in ordered_chunks]
 
 
-# Function to grab mutually exclusiv UIDs for a specific full_hash (get chunks of non-overlapping UIDs)
+# Function to grab mutually exclusive UIDs for a specific full_hash (get chunks of non-overlapping UIDs)
 async def retrieve_mutually_exclusive_hotkeys_full_hash(
     full_hash: str, database: aioredis.Redis
 ) -> Dict[str, List[str]]:
     """
     Retrieve a list of mutually exclusive hotkeys for a specific full hash.
 
     This function retrieves the metadata for all chunks of a file and then sorts them based on their
@@ -1059,15 +1059,164 @@
 
     # Test getting the chunk hash back
     chunk_data = await get_all_chunks_for_file(file_hash, database)
     if chunk_data == {}:
         bt.logging.debug(f"all chunks deleted for file {file_hash}.")
         await database.delete(f"file:{file_hash}")
 
+    bt.logging.trace(f"File {file_hash} deleted!")
+
 
-def get_hash_keys(ss58_address, r):
+async def get_hash_keys(ss58_address: str, database: aioredis.Redis) -> List[str]:
     """
     Filter out the ttl: hashes from the hotkey hashes and return the list of keys.
     """
     return [
-        key for key in r.hkeys(f"hotkey:{ss58_address}") if not key.startswith(b"ttl:")
+        key for key in await database.hkeys(f"hotkey:{ss58_address}") if not key.startswith(b"ttl:")
+    ]
+
+
+async def active_hotkeys(database: aioredis.Redis) -> List[str]:
+    """
+    Returns a list of all active hotkeys in the database.
+    """
+    return [
+        x.decode().split(":")[-1] async for x in database.scan_iter("hotkey:*")
     ]
+
+
+async def get_network_capacity(database) -> int:
+    """
+    Get the total storage capacity of the network in bytes.
+    """
+    cap = 0
+    for k,v in (await get_miner_statistics(database)).items():
+        cap += int(v.get('storage_limit', 0))
+
+    return cap
+
+
+async def current_validator_storage(database) -> int:
+    """
+    Get the current storage capacity of the network in bytes.
+    """
+    hotkeys = await active_hotkeys(database)
+
+    current_storage = 0
+    for k, (cur, _) in (await cache_hotkeys_capacity(hotkeys, database)).items():
+        current_storage += cur
+
+    return current_storage
+
+
+async def tier_statistics(database: aioredis.Redis, by_tier: bool = False) -> Dict[str, Dict[str, int]]:
+    tier_counts = {
+        "Super Saiyan": 0,
+        "Diamond": 0,
+        "Gold": 0,
+        "Silver": 0,
+        "Bronze": 0,
+    } 
+    tier_capacity = {
+        "Super Saiyan": 0,
+        "Diamond": 0,
+        "Gold": 0,
+        "Silver": 0,
+        "Bronze": 0,
+    }
+    tier_usage = {
+        "Super Saiyan": 0,
+        "Diamond": 0,
+        "Gold": 0,
+        "Silver": 0,
+        "Bronze": 0,
+    }
+
+    for k,v in (await get_miner_statistics(database)).items():
+        tier = v.get('tier', None)
+        if tier:
+            hotkey = k.split(":")[-1]
+            tier_counts[tier] += 1
+            tier_capacity[tier] += int(v.get('storage_limit', 0))
+            tier_usage[tier] += await total_hotkey_storage(hotkey, database, False)
+
+    tier_percent_usage = {
+        k: 100 * (v / tier_capacity[k]) if tier_capacity[k] > 0 else 0
+        for k,v in tier_usage.items()
+    }
+
+    type_dict = {
+        "counts": tier_counts, 
+        "capacity": tier_capacity, 
+        "usage": tier_usage,
+        "percent_usage": tier_percent_usage
+    }
+
+    if by_tier:
+        inverted_dict = {}
+
+        for category, tier_dict in type_dict.items():
+            for tier, value in tier_dict.items():
+                if tier not in inverted_dict:
+                    inverted_dict[tier] = {}
+                inverted_dict[tier][category] = value
+
+        return inverted_dict
+
+    return type_dict
+
+async def total_successful_requests(database: aioredis.Redis) -> int:
+    return sum(
+        [
+            int(v.get('total_successes', 0))
+            for k,v in (await get_miner_statistics(database)).items()
+        ]
+    )
+
+
+async def compute_by_tier_stats(database):
+
+    stats = await get_miner_statistics(database)
+
+    tier_stats = {}
+
+    for _, d in stats.items():
+        tier = d.get('tier', "Bronze")
+
+        if tier not in tier_stats:
+            tier_stats[tier] = {
+                'store_attempts': 0,
+                'store_successes': 0,
+                'challenge_attempts': 0,
+                'challenge_successes': 0,
+                'retrieve_attempts': 0,
+                'retrieve_successes': 0,
+                'total_current_attempts': 0,
+                'total_current_successes': 0,
+                'total_global_successes': 0,
+            }
+
+        tier_stats[tier]['store_attempts'] += int(d.get('store_attempts', 0))
+        tier_stats[tier]['store_successes'] += int(d.get('store_successes', 0))
+        tier_stats[tier]['challenge_attempts'] += int(d.get('challenge_attempts', 0))
+        tier_stats[tier]['challenge_successes'] += int(d.get('challenge_successes', 0))
+        tier_stats[tier]['retrieve_attempts'] += int(d.get('retrieve_attempts', 0))
+        tier_stats[tier]['retrieve_successes'] += int(d.get('retrieve_successes', 0))
+
+        tier_stats[tier]['total_current_attempts'] = sum([
+            tier_stats[tier]['store_attempts'], 
+            tier_stats[tier]['challenge_attempts'], 
+            tier_stats[tier]['retrieve_attempts']
+        ])
+        tier_stats[tier]['total_current_successes'] = sum([
+            tier_stats[tier]['store_successes'], 
+            tier_stats[tier]['challenge_successes'], 
+            tier_stats[tier]['retrieve_successes']
+        ])
+        tier_stats[tier]['total_global_successes'] += int(d.get('total_successes', 0))
+
+        total_attempts = tier_stats[tier]['total_current_attempts']
+        total_successes = tier_stats[tier]['total_current_successes']
+        success_rate = (total_successes / total_attempts * 100) if total_attempts else 0
+        tier_stats[tier]['success_rate'] = success_rate
+
+    return tier_stats
```

### Comparing `FileTAO-2.1.0/storage/validator/distribute.py` & `FileTAO-3.0.0/storage/validator/distribute.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/validator/encryption.py` & `FileTAO-3.0.0/storage/validator/encryption.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/validator/event.py` & `FileTAO-3.0.0/storage/validator/event.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/validator/forward.py` & `FileTAO-3.0.0/storage/validator/forward.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/validator/network.py` & `FileTAO-3.0.0/storage/validator/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -157,28 +157,27 @@
         # Ping all UIDs
         current_successful_uids, current_failed_uids = await ping_uids(self, uids)
         successful_uids.update(current_successful_uids)
         failed_uids.update(current_failed_uids)
 
         # If enough UIDs are successful, select the first k items
         if len(successful_uids) >= k:
-            uids = list(successful_uids)[:k]
             break
 
         # Reroll for k UIDs excluding the successful ones
-        new_uids = await get_available_query_miners(
+        uids = await get_available_query_miners(
             self, k=k, exclude=list(successful_uids.union(failed_uids))
         )
-        bt.logging.debug(f"ping_and_retry() new uids: {new_uids}")
+        bt.logging.debug(f"ping_and_retry() new uids: {uids}")
         retries += 1
 
     # Log if the maximum retries are reached without enough successful UIDs
     if len(successful_uids) < k:
         bt.logging.warning(
-            f"Insufficient successful UIDs for k: {k} Success UIDs {successful_uids} Failed UIDs: {failed_uids}"
+            f"Insufficient successful UIDs for k: {k} Success UIDs {len(successful_uids)} : {successful_uids} Failed UIDs {len(failed_uids)} : {failed_uids}"
         )
 
     return list(successful_uids)[:k], failed_uids
 
 
 # Monitor all UIDs by ping and keep track of how many failures
 async def monitor(self):
@@ -191,14 +190,16 @@
     query_uids = await get_available_query_miners(self, k=40)
     bt.logging.debug(f"monitor() uids: {query_uids}")
     _, failed_uids = await ping_uids(self, query_uids)
     bt.logging.debug(f"monitor() failed uids: {failed_uids}")
 
     down_uids = []
     for uid in failed_uids:
+        if uid not in self.monitor_lookup:
+            self.monitor_lookup[uid] = 0
         self.monitor_lookup[uid] += 1
         if self.monitor_lookup[uid] > 5:
             self.monitor_lookup[uid] = 0
             down_uids.append(uid)
     bt.logging.debug(f"monitor() down uids: {down_uids}")
     bt.logging.trace(f"monitor() monitor_lookup: {self.monitor_lookup}")
```

### Comparing `FileTAO-2.1.0/storage/validator/rebalance.py` & `FileTAO-3.0.0/storage/validator/rebalance.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/validator/retrieve.py` & `FileTAO-3.0.0/storage/validator/retrieve.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         data_hash=data_hash,
         seed=get_random_bytes(32).hex(),
     )
     response = await self.dendrite(
         [axon],
         synapse,
         deserialize=False,
-        timeout=60,
+        timeout=100,
     )
 
     try:
         bt.logging.trace(f"Fetching AES payload from UID: {uid}")
 
         # Load the data for this miner from validator storage
         data = await get_metadata_for_hotkey_and_hash(
@@ -318,15 +318,15 @@
         )
 
         axons = [self.metagraph.axons[uid] for uid in uids]
         responses = await self.dendrite(
             axons,
             synapse,
             deserialize=False,
-            timeout=60,
+            timeout=100,
         )
 
         # Compute the rewards for the responses given proc time.
         rewards: torch.FloatTensor = torch.zeros(
             len(responses), dtype=torch.float32
         ).to(self.device)
```

### Comparing `FileTAO-2.1.0/storage/validator/reward.py` & `FileTAO-3.0.0/storage/validator/reward.py`

 * *Files 6% similar despite different names*

```diff
@@ -147,30 +147,36 @@
     """
     max_time = max(
         [
             response.dendrite.process_time for response in responses
             if response.dendrite.process_time is not None
         ] or [1] # nobody responded successfully
     )
+    bt.logging.trace(f"max response time: {max_time}")
 
     sorted_axon_times = get_sorted_response_times(uids, responses, max_time=max_time)
 
     # Extract only the process times
     process_times = [proc_time for _, proc_time in sorted_axon_times]
+    bt.logging.trace(f"process times: {process_times}")
+    if process_times == []: # is empty
+        bt.logging.warning(f"No one returned successfully. 0 reward across the board.")
+        return [0.0 for _ in rewards]
 
     # Apply logarithmic scaling to data sizes
     bt.logging.trace(f"Unnormalized data sizes: {data_sizes}")
     log_data_sizes_np = np.log1p(data_sizes)
     bt.logging.trace(f"Logarithmically scaled data sizes: {log_data_sizes_np}")
 
     # Normalize the response times by data size (unit time)
     data_normalized_process_times = np.asarray(np.array(process_times) / log_data_sizes_np)
 
     # Normalize the response times
-    normalized_times = sigmoid_normalize(data_normalized_process_times, max(data_normalized_process_times))
+    bt.logging.trace(f"data_normalized_process_times: {data_normalized_process_times}")
+    normalized_times = sigmoid_normalize(data_normalized_process_times, max(data_normalized_process_times) * 2)
 
     # Create a dictionary mapping UIDs to normalized times
     uid_to_normalized_time = {
         uid: normalized_time
         for (uid, _), normalized_time in zip(sorted_axon_times, normalized_times)
     }
```

### Comparing `FileTAO-2.1.0/storage/validator/state.py` & `FileTAO-3.0.0/storage/validator/state.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/validator/store.py` & `FileTAO-3.0.0/storage/validator/store.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             failed_uids = []
 
         # Broadcast the query to selected miners on the network.
         responses = await self.dendrite(
             axons,
             synapse,
             deserialize=False,
-            timeout=60,
+            timeout=100,
         )
 
         # Compute the rewards for the responses given proc time.
         rewards: torch.FloatTensor = torch.zeros(
             len(responses), dtype=torch.float32
         ).to(self.device)
 
@@ -336,15 +336,15 @@
         ]
 
         axons = [self.metagraph.axons[uid] for uid in uids]
         responses = await self.dendrite(
             axons,
             synapse,
             deserialize=False,
-            timeout=60,
+            timeout=100,
         )
 
         # Compute the rewards for the responses given proc time.
         rewards: torch.FloatTensor = torch.zeros(
             len(responses), dtype=torch.float32
         ).to(self.device)
```

### Comparing `FileTAO-2.1.0/storage/validator/utils.py` & `FileTAO-3.0.0/storage/validator/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 
 from storage.shared.ecc import hash_data
 from storage.validator.database import hotkey_at_capacity
 
 import bittensor as bt
 
 
-MIN_CHUNK_SIZE = 64 * 1024 * 1024  # 128 MB
-MAX_CHUNK_SIZE = 512 * 1024 * 1024  # 512 MB
+MIN_CHUNK_SIZE = 64 * 1024 * 1024   # 64 MB
+MAX_CHUNK_SIZE = 256 * 1024 * 1024  # 256 MB
 
 
 def chunk_data_generator(data, chunk_size):
     """
     Generator that yields chunks of data.
 
     Args:
@@ -176,15 +176,15 @@
     """
     try:
         block_hash: str = self.subtensor.get_block_hash(self.subtensor.get_current_block())
         if block_hash is not None:
             return block_hash
     except Exception as e:
         bt.logging.warning(f"Failed to get block hash: {e}. Returning a random hash value.")
-    return int(str(random.randint(2 << 32, 2 << 64)))
+    return str(random.randint(2 << 32, 2 << 64))
 
 def get_block_seed(self):
     """
     Get the block seed for the current block.
 
     Args:
         subtensor (bittensor.subtensor.Subtensor): The subtensor instance to use for getting the block seed.
```

### Comparing `FileTAO-2.1.0/storage/validator/verify.py` & `FileTAO-3.0.0/storage/validator/verify.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/storage/validator/weights.py` & `FileTAO-3.0.0/storage/validator/weights.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,20 +49,20 @@
         wallet (bt.wallet): The miner's wallet holding cryptographic information.
         netuid (int): The unique identifier for the chain subnet.
         uids (torch.Tensor): miners UIDs on the network.
         metagraph (bt.metagraph): Bittensor metagraph.
         moving_averaged_scores (torch.Tensor): .
         wandb_on (bool, optional): Flag to determine if logging to Weights & Biases is enabled. Defaults to False.
         tempo (int): Tempo for 'netuid' subnet.
-        wait_for_inclusion (bool, optional): Wether to wait for the extrinsic to enter a block
-        wait_for_finalization (bool, optional): Wether to wait for the extrinsic to be finalized on the chain
+        wait_for_inclusion (bool, optional): Whether to wait for the extrinsic to enter a block
+        wait_for_finalization (bool, optional): Whether to wait for the extrinsic to be finalized on the chain
 
     Returns:
         success (bool):
-            flag is true if extrinsic was finalized or uncluded in the block.
+            flag is true if extrinsic was finalized or included in the block.
             If we did not wait for finalization / inclusion, the response is true.
 
     Raises:
         Exception: If there's an error while setting weights, the exception is logged for diagnosis.
     """
     # Calculate the average reward for each uid across non-zero values.
     # Replace any NaN values with 0.
@@ -84,15 +84,15 @@
     # Make all values positive
     if minimum < 0:
         positive_moving_averaged_scores = moving_averaged_scores_no_nan - minimum
     else:
         positive_moving_averaged_scores = moving_averaged_scores_no_nan
     bt.logging.debug(f"Positive scores", positive_moving_averaged_scores)
 
-    # Push all orinally negative indices to zero
+    # Push all originally negative indices to zero
     positive_moving_averaged_scores[neg_idxs] = 0
 
     # Normalize, ensuring no division by zero or NaNs occur
     sum_scores = positive_moving_averaged_scores.sum()
     bt.logging.info(f"Score sum: {sum_scores}")
     if sum_scores > 0:
         raw_weights = torch.nn.functional.normalize(positive_moving_averaged_scores, p=1, dim=0)
```

### Comparing `FileTAO-2.1.0/tests/unit/validator/test_challenge.py` & `FileTAO-3.0.0/tests/unit/validator/test_challenge.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/tests/unit/validator/test_encryption.py` & `FileTAO-3.0.0/tests/unit/validator/test_encryption.py`

 * *Files identical despite different names*

### Comparing `FileTAO-2.1.0/tests/unit/validator/test_state.py` & `FileTAO-3.0.0/tests/unit/validator/test_state.py`

 * *Files identical despite different names*

