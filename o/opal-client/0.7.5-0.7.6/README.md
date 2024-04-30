# Comparing `tmp/opal-client-0.7.5.tar.gz` & `tmp/opal_client-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-client-0.7.5.tar", last modified: Wed Mar 13 16:42:10 2024, max compression
+gzip compressed data, was "opal_client-0.7.6.tar", last modified: Tue Apr 30 17:18:48 2024, max compression
```

## Comparing `opal-client-0.7.5.tar` & `opal_client-0.7.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.650197 opal-client-0.7.5/
--rw-r--r--   0 roekatz    (501) staff       (20)     9993 2024-03-13 16:42:10.649906 opal-client-0.7.5/PKG-INFO
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.640235 opal-client-0.7.5/opal_client/
--rw-r--r--   0 roekatz    (501) staff       (20)       31 2022-12-08 13:40:17.000000 opal-client-0.7.5/opal_client/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.642078 opal-client-0.7.5/opal_client/callbacks/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.5/opal_client/callbacks/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3034 2022-12-08 13:40:17.000000 opal-client-0.7.5/opal_client/callbacks/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4385 2024-03-06 13:35:27.000000 opal-client-0.7.5/opal_client/callbacks/register.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3729 2024-03-06 13:35:27.000000 opal-client-0.7.5/opal_client/callbacks/reporter.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2213 2023-05-29 10:10:14.000000 opal-client-0.7.5/opal_client/cli.py
--rw-r--r--   0 roekatz    (501) staff       (20)    20236 2024-03-06 13:35:27.000000 opal-client-0.7.5/opal_client/client.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12812 2024-03-13 14:22:17.000000 opal-client-0.7.5/opal_client/config.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.643122 opal-client-0.7.5/opal_client/data/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.5/opal_client/data/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      863 2022-12-08 13:40:17.000000 opal-client-0.7.5/opal_client/data/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4816 2024-03-13 14:22:17.000000 opal-client-0.7.5/opal_client/data/fetcher.py
--rw-r--r--   0 roekatz    (501) staff       (20)      842 2022-12-08 13:40:17.000000 opal-client-0.7.5/opal_client/data/rpc.py
--rw-r--r--   0 roekatz    (501) staff       (20)    21950 2024-03-13 16:32:44.000000 opal-client-0.7.5/opal_client/data/updater.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.644173 opal-client-0.7.5/opal_client/engine/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-05-29 10:10:14.000000 opal-client-0.7.5/opal_client/engine/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.644608 opal-client-0.7.5/opal_client/engine/healthcheck/
--rw-r--r--   0 roekatz    (501) staff       (20)     1123 2023-05-29 10:10:14.000000 opal-client-0.7.5/opal_client/engine/healthcheck/opal.rego
--rw-r--r--   0 roekatz    (501) staff       (20)     3032 2024-03-06 13:35:27.000000 opal-client-0.7.5/opal_client/engine/logger.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5702 2023-05-29 10:10:14.000000 opal-client-0.7.5/opal_client/engine/options.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12557 2024-03-06 13:35:27.000000 opal-client-0.7.5/opal_client/engine/runner.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2220 2022-12-08 13:40:17.000000 opal-client-0.7.5/opal_client/limiter.py
--rw-r--r--   0 roekatz    (501) staff       (20)       33 2022-12-08 13:40:17.000000 opal-client-0.7.5/opal_client/logger.py
--rw-r--r--   0 roekatz    (501) staff       (20)       96 2022-12-08 13:40:17.000000 opal-client-0.7.5/opal_client/main.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.645776 opal-client-0.7.5/opal_client/policy/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.5/opal_client/policy/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      509 2024-03-06 13:35:27.000000 opal-client-0.7.5/opal_client/policy/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4968 2023-05-29 10:10:14.000000 opal-client-0.7.5/opal_client/policy/fetcher.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1791 2024-02-28 15:15:55.000000 opal-client-0.7.5/opal_client/policy/options.py
--rw-r--r--   0 roekatz    (501) staff       (20)      596 2022-12-08 13:40:17.000000 opal-client-0.7.5/opal_client/policy/topics.py
--rw-r--r--   0 roekatz    (501) staff       (20)    15053 2024-03-06 13:35:27.000000 opal-client-0.7.5/opal_client/policy/updater.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.648413 opal-client-0.7.5/opal_client/policy_store/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.5/opal_client/policy_store/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1650 2023-05-29 10:10:14.000000 opal-client-0.7.5/opal_client/policy_store/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8442 2024-03-13 14:12:07.000000 opal-client-0.7.5/opal_client/policy_store/base_policy_store_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12318 2023-05-29 10:10:14.000000 opal-client-0.7.5/opal_client/policy_store/cedar_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3040 2024-03-06 13:35:27.000000 opal-client-0.7.5/opal_client/policy_store/mock_policy_store_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)    36976 2024-03-13 14:12:07.000000 opal-client-0.7.5/opal_client/policy_store/opa_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6605 2024-03-13 14:12:07.000000 opal-client-0.7.5/opal_client/policy_store/policy_store_client_factory.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1831 2023-06-20 17:01:29.000000 opal-client-0.7.5/opal_client/policy_store/schemas.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.649217 opal-client-0.7.5/opal_client/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.5/opal_client/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)    10553 2024-03-06 13:35:27.000000 opal-client-0.7.5/opal_client/tests/data_updater_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3973 2024-03-06 13:35:27.000000 opal-client-0.7.5/opal_client/tests/opa_client_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4542 2024-03-06 13:35:27.000000 opal-client-0.7.5/opal_client/tests/server_to_client_intergation_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)      613 2023-07-17 14:14:01.000000 opal-client-0.7.5/opal_client/utils.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.649550 opal-client-0.7.5/opal_client.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)     9993 2024-03-13 16:42:10.000000 opal-client-0.7.5/opal_client.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     1501 2024-03-13 16:42:10.000000 opal-client-0.7.5/opal_client.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2024-03-13 16:42:10.000000 opal-client-0.7.5/opal_client.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       52 2024-03-13 16:42:10.000000 opal-client-0.7.5/opal_client.egg-info/entry_points.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      456 2024-03-13 16:42:10.000000 opal-client-0.7.5/opal_client.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       12 2024-03-13 16:42:10.000000 opal-client-0.7.5/opal_client.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       38 2024-03-13 16:42:10.650246 opal-client-0.7.5/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     2834 2023-05-29 10:10:14.000000 opal-client-0.7.5/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.888325 opal_client-0.7.6/
+-rw-r--r--   0 roekatz    (501) staff       (20)    10001 2024-04-30 17:18:48.887806 opal_client-0.7.6/PKG-INFO
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.880180 opal_client-0.7.6/opal_client/
+-rw-r--r--   0 roekatz    (501) staff       (20)       31 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.881709 opal_client-0.7.6/opal_client/callbacks/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/callbacks/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3034 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/callbacks/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4385 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/callbacks/register.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3729 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/callbacks/reporter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2213 2023-05-29 10:10:14.000000 opal_client-0.7.6/opal_client/cli.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    20271 2024-04-30 13:01:51.000000 opal_client-0.7.6/opal_client/client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    12812 2024-04-30 16:48:47.000000 opal_client-0.7.6/opal_client/config.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.882507 opal_client-0.7.6/opal_client/data/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/data/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      863 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/data/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4489 2024-04-30 12:59:10.000000 opal_client-0.7.6/opal_client/data/fetcher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      842 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/data/rpc.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    23358 2024-04-30 13:01:51.000000 opal_client-0.7.6/opal_client/data/updater.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.883537 opal_client-0.7.6/opal_client/engine/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-05-29 10:10:14.000000 opal_client-0.7.6/opal_client/engine/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.883850 opal_client-0.7.6/opal_client/engine/healthcheck/
+-rw-r--r--   0 roekatz    (501) staff       (20)     1123 2023-05-29 10:10:14.000000 opal_client-0.7.6/opal_client/engine/healthcheck/opal.rego
+-rw-r--r--   0 roekatz    (501) staff       (20)     3032 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/engine/logger.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5702 2023-05-29 10:10:14.000000 opal_client-0.7.6/opal_client/engine/options.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    12557 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/engine/runner.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2220 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/limiter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)       33 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/logger.py
+-rw-r--r--   0 roekatz    (501) staff       (20)       96 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/main.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.885051 opal_client-0.7.6/opal_client/policy/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/policy/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      509 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/policy/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4678 2024-04-30 12:59:10.000000 opal_client-0.7.6/opal_client/policy/fetcher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1791 2024-02-28 15:15:55.000000 opal_client-0.7.6/opal_client/policy/options.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      596 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/policy/topics.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    15053 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/policy/updater.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.886421 opal_client-0.7.6/opal_client/policy_store/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/policy_store/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1650 2023-05-29 10:10:14.000000 opal_client-0.7.6/opal_client/policy_store/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8442 2024-03-13 14:12:07.000000 opal_client-0.7.6/opal_client/policy_store/base_policy_store_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    12318 2023-05-29 10:10:14.000000 opal_client-0.7.6/opal_client/policy_store/cedar_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3040 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/policy_store/mock_policy_store_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    36976 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/policy_store/opa_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6605 2024-03-13 14:12:07.000000 opal_client-0.7.6/opal_client/policy_store/policy_store_client_factory.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1831 2023-06-20 17:01:29.000000 opal_client-0.7.6/opal_client/policy_store/schemas.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.887034 opal_client-0.7.6/opal_client/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    10553 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/tests/data_updater_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3973 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/tests/opa_client_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4542 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/tests/server_to_client_intergation_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      613 2023-07-17 14:14:01.000000 opal_client-0.7.6/opal_client/utils.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.887306 opal_client-0.7.6/opal_client.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)    10001 2024-04-30 17:18:48.000000 opal_client-0.7.6/opal_client.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     1501 2024-04-30 17:18:48.000000 opal_client-0.7.6/opal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2024-04-30 17:18:48.000000 opal_client-0.7.6/opal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       52 2024-04-30 17:18:48.000000 opal_client-0.7.6/opal_client.egg-info/entry_points.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      426 2024-04-30 17:18:48.000000 opal_client-0.7.6/opal_client.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       12 2024-04-30 17:18:48.000000 opal_client-0.7.6/opal_client.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       38 2024-04-30 17:18:48.888400 opal_client-0.7.6/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     2886 2024-04-30 13:01:51.000000 opal_client-0.7.6/setup.py
```

### Comparing `opal-client-0.7.5/PKG-INFO` & `opal_client-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: opal-client
-Version: 0.7.5
+Version: 0.7.6
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-client is deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by connecting to an opal-server and subscribing to pub/sub updates for policy and policy data changes.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles<1,>=0.8.0
 Requires-Dist: aiohttp<4,>=3.9.2
 Requires-Dist: psutil<6,>=5.9.1
 Requires-Dist: tenacity<9,>=8.0.1
 Requires-Dist: websockets<11,>=10.3
 Requires-Dist: dpath<3,>=2.1.5
 Requires-Dist: jsonpatch<2,>=1.33
-Requires-Dist: opal-common==0.7.5
-Requires-Dist: charset-normalizer<3,>=2.0.12
+Requires-Dist: opal-common==0.7.6
 Requires-Dist: idna<4,>=3.3
 Requires-Dist: typer<1,>=0.4.1
 Requires-Dist: fastapi<1,>=0.109.1
 Requires-Dist: fastapi_websocket_pubsub==0.3.7
 Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<21,>=20.1.0
+Requires-Dist: gunicorn<23,>=22.0.0
 Requires-Dist: pydantic[email]<2,>=1.9.1
 Requires-Dist: typing-extensions; python_version < "3.8"
 Requires-Dist: uvicorn[standard]<1,>=0.17.6
 Requires-Dist: fastapi-utils<1,>=0.2.1
 Requires-Dist: setuptools>=65.5.1
 
 <p  align="center">
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: opal-client Version: 0.7.5 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-client Version: 0.7.6 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-client is
 deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by
 connecting to an opal-server and subscribing to pub/sub updates for policy and
 policy data changes. Home-page: https://github.com/permitio/opal Author: Or
 Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Classifier:
 Operating System :: OS Independent Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP
-:: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-
-Python: >=3.7 Description-Content-Type: text/markdown Requires-Dist:
-aiofiles<1,>=0.8.0 Requires-Dist: aiohttp<4,>=3.9.2 Requires-Dist:
-psutil<6,>=5.9.1 Requires-Dist: tenacity<9,>=8.0.1 Requires-Dist:
-websockets<11,>=10.3 Requires-Dist: dpath<3,>=2.1.5 Requires-Dist:
-jsonpatch<2,>=1.33 Requires-Dist: opal-common==0.7.5 Requires-Dist: charset-
-normalizer<3,>=2.0.12 Requires-Dist: idna<4,>=3.3 Requires-Dist:
-typer<1,>=0.4.1 Requires-Dist: fastapi<1,>=0.109.1 Requires-Dist:
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-Python: >=3.9
+Description-Content-Type: text/markdown Requires-Dist: aiofiles<1,>=0.8.0
+Requires-Dist: aiohttp<4,>=3.9.2 Requires-Dist: psutil<6,>=5.9.1 Requires-Dist:
+tenacity<9,>=8.0.1 Requires-Dist: websockets<11,>=10.3 Requires-Dist:
+dpath<3,>=2.1.5 Requires-Dist: jsonpatch<2,>=1.33 Requires-Dist: opal-
+common==0.7.6 Requires-Dist: idna<4,>=3.3 Requires-Dist: typer<1,>=0.4.1
+Requires-Dist: fastapi<1,>=0.109.1 Requires-Dist:
 fastapi_websocket_pubsub==0.3.7 Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<21,>=20.1.0 Requires-Dist: pydantic[email]<2,>=1.9.1
+Requires-Dist: gunicorn<23,>=22.0.0 Requires-Dist: pydantic[email]<2,>=1.9.1
 Requires-Dist: typing-extensions; python_version < "3.8" Requires-Dist: uvicorn
 [standard]<1,>=0.17.6 Requires-Dist: fastapi-utils<1,>=0.2.1 Requires-Dist:
 setuptools>=65.5.1
                                     [opal]
                            ************ ?â??¡OOPPAALL?â??¡ ************
                  ********** OOppeenn PPoolliiccyy AAddmmiinniissttrraattiioonn LLaayyeerr **********
 _[_T_e_s_t_s_]_[_P_a_c_k_a_g_e_]_[_P_a_c_k_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_c_k_e_r_ _p_u_l_l_s_]_[_J_o_i_n_ _o_u_r_ _S_l_a_c_k_!_]_[_h_t_t_p_s_:_/_/
```

### Comparing `opal-client-0.7.5/opal_client/callbacks/api.py` & `opal_client-0.7.6/opal_client/callbacks/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/callbacks/register.py` & `opal_client-0.7.6/opal_client/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/callbacks/reporter.py` & `opal_client-0.7.6/opal_client/callbacks/reporter.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/cli.py` & `opal_client-0.7.6/opal_client/cli.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/client.py` & `opal_client-0.7.6/opal_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,15 +458,16 @@
             logger.error(
                 "Critical: OPA health-check policy is enabled, but cannot find policy at {path}",
                 path=healthcheck_policy_path,
             )
             raise ValueError("OPA health check policy not found!")
 
         try:
-            healthcheck_policy_code = open(healthcheck_policy_path, "r").read()
+            with open(healthcheck_policy_path, "r") as file:
+                healthcheck_policy_code = file.read()
         except IOError as err:
             logger.error(
                 "Critical: Cannot read healthcheck policy: {err}", err=repr(err)
             )
             raise
 
         try:
```

### Comparing `opal-client-0.7.5/opal_client/config.py` & `opal_client-0.7.6/opal_client/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         },
         description="retry options when connecting to the base data source (e.g. an external API server which returns data snapshot)",
     )
 
     POLICY_STORE_POLICY_PATHS_TO_IGNORE = confi.list(
         "POLICY_STORE_POLICY_PATHS_TO_IGNORE",
         [],
-        description="When loading policies manually or otherwise externally into the policy store, use this list of glob patterns to have OPAL ignore and not delete or override them, end paths (without any wildcards in the middle) with '\**' to indicate you want all nested under the path to be ignored",
+        description="When loading policies manually or otherwise externally into the policy store, use this list of glob patterns to have OPAL ignore and not delete or override them, end paths (without any wildcards in the middle) with '/**' to indicate you want all nested under the path to be ignored",
     )
 
     POLICY_UPDATER_ENABLED = confi.bool(
         "POLICY_UPDATER_ENABLED",
         True,
         description="If set to False, opal client will not listen to dynamic policy updates."
         "Policy update fetching will be completely disabled.",
```

### Comparing `opal-client-0.7.5/opal_client/data/api.py` & `opal_client-0.7.6/opal_client/data/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/data/fetcher.py` & `opal_client-0.7.6/opal_client/data/fetcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,40 +10,34 @@
 from opal_common.logger import logger
 from opal_common.utils import get_authorization_header, tuple_to_dict
 
 
 class DataFetcher:
     """fetches policy data from backend."""
 
-    # Use as default config the configuration provider by opal_client_config.DATA_UPDATER_CONN_RETRY
-    # Add reraise as true (an option not available for control from the higher-level config)
-    DEFAULT_RETRY_CONFIG = opal_client_config.DATA_UPDATER_CONN_RETRY.toTenacityConfig()
-    DEFAULT_RETRY_CONFIG["reraise"] = True
-
-    def __init__(
-        self, default_data_url: str = None, token: str = None, retry_config=None
-    ):
+    def __init__(self, default_data_url: str = None, token: str = None):
         """
 
         Args:
             default_data_url (str, optional): The URL used to fetch data if no specific url is given in a fetch request. Defaults to DEFAULT_DATA_URL.
             token (str, optional): default auth token. Defaults to CLIENT_TOKEN.
         """
         # defaults
         default_data_url: str = default_data_url or opal_client_config.DEFAULT_DATA_URL
         token: str = token or opal_client_config.CLIENT_TOKEN
-        self._retry_config = (
-            retry_config if retry_config is not None else self.DEFAULT_RETRY_CONFIG
-        )
+
+        retry_config = opal_client_config.DATA_UPDATER_CONN_RETRY.toTenacityConfig()
+        retry_config["reraise"] = True  # This is currently not configurable
+
         # The underlying fetching engine
         self._engine = FetchingEngine(
             worker_count=opal_common_config.FETCHING_WORKER_COUNT,
             callback_timeout=opal_common_config.FETCHING_CALLBACK_TIMEOUT,
             enqueue_timeout=opal_common_config.FETCHING_ENQUEUE_TIMEOUT,
-            retry_config=self._retry_config,
+            retry_config=retry_config,
         )
         self._data_url = default_data_url
         self._token = token
         self._auth_headers = tuple_to_dict(get_authorization_header(token))
         self._default_fetcher_config = HttpFetcherConfig(
             headers=self._auth_headers, is_json=True
         )
```

### Comparing `opal-client-0.7.5/opal_client/data/rpc.py` & `opal_client-0.7.6/opal_client/data/rpc.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/data/updater.py` & `opal_client-0.7.6/opal_client/data/updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import hashlib
 import itertools
 import json
 import uuid
+from functools import partial
 from typing import Any, Dict, List, Optional, Tuple
 
 import aiohttp
 from aiohttp.client import ClientError, ClientSession
 from fastapi_websocket_pubsub import PubSubClient
 from fastapi_websocket_rpc.rpc_channel import RpcChannel
 from opal_client.callbacks.register import CallbacksRegister
@@ -18,15 +19,15 @@
 from opal_client.policy_store.base_policy_store_client import (
     BasePolicyStoreClient,
     JsonableValue,
 )
 from opal_client.policy_store.policy_store_client_factory import (
     DEFAULT_POLICY_STORE_GETTER,
 )
-from opal_common.async_utils import TakeANumberQueue, TasksPool
+from opal_common.async_utils import TakeANumberQueue, TasksPool, repeated_call
 from opal_common.config import opal_common_config
 from opal_common.fetcher.events import FetcherConfig
 from opal_common.http import is_http_error_response
 from opal_common.schemas.data import (
     DataEntryReport,
     DataSourceConfig,
     DataSourceEntry,
@@ -126,14 +127,15 @@
         self._ssl_context_kwargs = (
             {"ssl": self._custom_ssl_context}
             if self._custom_ssl_context is not None
             else {}
         )
         self._updates_storing_queue = TakeANumberQueue(logger)
         self._tasks = TasksPool()
+        self._polling_update_tasks = []
 
     async def __aenter__(self):
         await self.start()
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         """Context handler to terminate internal tasks."""
@@ -198,20 +200,43 @@
         Args:
             config_url (str, optional): URL to retrieve data sources config from. Defaults to None ( self._data_sources_config_url).
             data_fetch_reason (str, optional): Reason to log for the update operation. Defaults to "Initial load".
         """
         logger.info(
             "Performing data configuration, reason: {reason}", reason=data_fetch_reason
         )
+        await self._stop_polling_update_tasks()  # If this is a reconnect - should stop previously received periodic updates
         sources_config = await self.get_policy_data_config(url=config_url)
-        # translate config to a data update
-        entries = sources_config.entries
-        update = DataUpdate(reason=data_fetch_reason, entries=entries)
+
+        init_entries, periodic_entries = [], []
+        for entry in sources_config.entries:
+            (
+                periodic_entries
+                if (entry.periodic_update_interval is not None)
+                else init_entries
+            ).append(entry)
+
+        # Process one time entries now
+        update = DataUpdate(reason=data_fetch_reason, entries=init_entries)
         await self.trigger_data_update(update)
 
+        # Schedule repeated processing of periodic polling entries
+        async def _trigger_update_with_entry(entry):
+            await self.trigger_data_update(
+                DataUpdate(reason="Periodic Update", entries=[entry])
+            )
+
+        for entry in periodic_entries:
+            repeat_process_entry = repeated_call(
+                partial(_trigger_update_with_entry, entry),
+                entry.periodic_update_interval,
+                logger=logger,
+            )
+            self._polling_update_tasks.append(asyncio.create_task(repeat_process_entry))
+
     async def on_connect(self, client: PubSubClient, channel: RpcChannel):
         """Pub/Sub on_connect callback On connection to backend, whether its
         the first connection, or reconnecting after downtime, refetch the state
         opa needs.
 
         As long as the connection is alive we know we are in sync with
         the server, when the connection is lost we assume we need to
@@ -258,27 +283,37 @@
             keep_alive=opal_client_config.KEEP_ALIVE_INTERVAL,
             server_uri=self._server_url,
             **self._ssl_context_kwargs,
         )
         async with self._client:
             await self._client.wait_until_done()
 
+    async def _stop_polling_update_tasks(self):
+        if len(self._polling_update_tasks) > 0:
+            for task in self._polling_update_tasks:
+                task.cancel()
+            await asyncio.gather(*self._polling_update_tasks, return_exceptions=True)
+            self._polling_update_tasks = []
+
     async def stop(self):
         self._stopping = True
         logger.info("Stopping data updater")
 
         # disconnect from Pub/Sub
         if self._client is not None:
             try:
                 await asyncio.wait_for(self._client.disconnect(), timeout=3)
             except asyncio.TimeoutError:
                 logger.debug(
                     "Timeout waiting for DataUpdater pubsub client to disconnect"
                 )
 
+        # stop periodic updates
+        await self._stop_polling_update_tasks()
+
         # stop subscriber task
         if self._subscriber_task is not None:
             logger.debug("Cancelling DataUpdater subscriber task")
             self._subscriber_task.cancel()
             try:
                 await self._subscriber_task
             except asyncio.CancelledError as exc:
```

### Comparing `opal-client-0.7.5/opal_client/engine/healthcheck/opal.rego` & `opal_client-0.7.6/opal_client/engine/healthcheck/opal.rego`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/engine/logger.py` & `opal_client-0.7.6/opal_client/engine/logger.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/engine/options.py` & `opal_client-0.7.6/opal_client/engine/options.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/engine/runner.py` & `opal_client-0.7.6/opal_client/engine/runner.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/limiter.py` & `opal_client-0.7.6/opal_client/limiter.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/policy/fetcher.py` & `opal_client-0.7.6/opal_client/policy/fetcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,33 +24,28 @@
         )
         raise
 
 
 class PolicyFetcher:
     """fetches policy from backend."""
 
-    # Use as default config the configuration provider by opal_client_config.POLICY_UPDATER_CONN_RETRY
-    # Add reraise as true (an option not available for control from the higher-level config)
-    DEFAULT_RETRY_CONFIG = (
-        opal_client_config.POLICY_UPDATER_CONN_RETRY.toTenacityConfig()
-    )
-    DEFAULT_RETRY_CONFIG["reraise"] = True
-
-    def __init__(self, backend_url=None, token=None, retry_config=None):
+    def __init__(self, backend_url=None, token=None):
         """
         Args:
             backend_url (str): Defaults to opal_client_config.SERVER_URL.
             token ([type], optional): [description]. Defaults to opal_client_config.CLIENT_TOKEN.
         """
         self._token = token or opal_client_config.CLIENT_TOKEN
         self._backend_url = backend_url or opal_client_config.SERVER_URL
         self._auth_headers = tuple_to_dict(get_authorization_header(self._token))
+
         self._retry_config = (
-            retry_config if retry_config is not None else self.DEFAULT_RETRY_CONFIG
+            opal_client_config.POLICY_UPDATER_CONN_RETRY.toTenacityConfig()
         )
+        self._retry_config["reraise"] = True  # This is currently not configurable
 
         scope_id = opal_client_config.SCOPE_ID
 
         if scope_id != "default":
             self._policy_endpoint_url = f"{self._backend_url}/scopes/{scope_id}/policy"
         else:
             self._policy_endpoint_url = f"{self._backend_url}/policy"
```

### Comparing `opal-client-0.7.5/opal_client/policy/options.py` & `opal_client-0.7.6/opal_client/policy/options.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/policy/topics.py` & `opal_client-0.7.6/opal_client/policy/topics.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/policy/updater.py` & `opal_client-0.7.6/opal_client/policy/updater.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/policy_store/api.py` & `opal_client-0.7.6/opal_client/policy_store/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/policy_store/base_policy_store_client.py` & `opal_client-0.7.6/opal_client/policy_store/base_policy_store_client.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/policy_store/cedar_client.py` & `opal_client-0.7.6/opal_client/policy_store/cedar_client.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/policy_store/mock_policy_store_client.py` & `opal_client-0.7.6/opal_client/policy_store/mock_policy_store_client.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/policy_store/opa_client.py` & `opal_client-0.7.6/opal_client/policy_store/opa_client.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/policy_store/policy_store_client_factory.py` & `opal_client-0.7.6/opal_client/policy_store/policy_store_client_factory.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/policy_store/schemas.py` & `opal_client-0.7.6/opal_client/policy_store/schemas.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/tests/data_updater_test.py` & `opal_client-0.7.6/opal_client/tests/data_updater_test.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/tests/opa_client_test.py` & `opal_client-0.7.6/opal_client/tests/opa_client_test.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/tests/server_to_client_intergation_test.py` & `opal_client-0.7.6/opal_client/tests/server_to_client_intergation_test.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client/utils.py` & `opal_client-0.7.6/opal_client/utils.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/opal_client.egg-info/PKG-INFO` & `opal_client-0.7.6/opal_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: opal-client
-Version: 0.7.5
+Version: 0.7.6
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-client is deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by connecting to an opal-server and subscribing to pub/sub updates for policy and policy data changes.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles<1,>=0.8.0
 Requires-Dist: aiohttp<4,>=3.9.2
 Requires-Dist: psutil<6,>=5.9.1
 Requires-Dist: tenacity<9,>=8.0.1
 Requires-Dist: websockets<11,>=10.3
 Requires-Dist: dpath<3,>=2.1.5
 Requires-Dist: jsonpatch<2,>=1.33
-Requires-Dist: opal-common==0.7.5
-Requires-Dist: charset-normalizer<3,>=2.0.12
+Requires-Dist: opal-common==0.7.6
 Requires-Dist: idna<4,>=3.3
 Requires-Dist: typer<1,>=0.4.1
 Requires-Dist: fastapi<1,>=0.109.1
 Requires-Dist: fastapi_websocket_pubsub==0.3.7
 Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<21,>=20.1.0
+Requires-Dist: gunicorn<23,>=22.0.0
 Requires-Dist: pydantic[email]<2,>=1.9.1
 Requires-Dist: typing-extensions; python_version < "3.8"
 Requires-Dist: uvicorn[standard]<1,>=0.17.6
 Requires-Dist: fastapi-utils<1,>=0.2.1
 Requires-Dist: setuptools>=65.5.1
 
 <p  align="center">
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: opal-client Version: 0.7.5 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-client Version: 0.7.6 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-client is
 deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by
 connecting to an opal-server and subscribing to pub/sub updates for policy and
 policy data changes. Home-page: https://github.com/permitio/opal Author: Or
 Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Classifier:
 Operating System :: OS Independent Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP
-:: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-
-Python: >=3.7 Description-Content-Type: text/markdown Requires-Dist:
-aiofiles<1,>=0.8.0 Requires-Dist: aiohttp<4,>=3.9.2 Requires-Dist:
-psutil<6,>=5.9.1 Requires-Dist: tenacity<9,>=8.0.1 Requires-Dist:
-websockets<11,>=10.3 Requires-Dist: dpath<3,>=2.1.5 Requires-Dist:
-jsonpatch<2,>=1.33 Requires-Dist: opal-common==0.7.5 Requires-Dist: charset-
-normalizer<3,>=2.0.12 Requires-Dist: idna<4,>=3.3 Requires-Dist:
-typer<1,>=0.4.1 Requires-Dist: fastapi<1,>=0.109.1 Requires-Dist:
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-Python: >=3.9
+Description-Content-Type: text/markdown Requires-Dist: aiofiles<1,>=0.8.0
+Requires-Dist: aiohttp<4,>=3.9.2 Requires-Dist: psutil<6,>=5.9.1 Requires-Dist:
+tenacity<9,>=8.0.1 Requires-Dist: websockets<11,>=10.3 Requires-Dist:
+dpath<3,>=2.1.5 Requires-Dist: jsonpatch<2,>=1.33 Requires-Dist: opal-
+common==0.7.6 Requires-Dist: idna<4,>=3.3 Requires-Dist: typer<1,>=0.4.1
+Requires-Dist: fastapi<1,>=0.109.1 Requires-Dist:
 fastapi_websocket_pubsub==0.3.7 Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<21,>=20.1.0 Requires-Dist: pydantic[email]<2,>=1.9.1
+Requires-Dist: gunicorn<23,>=22.0.0 Requires-Dist: pydantic[email]<2,>=1.9.1
 Requires-Dist: typing-extensions; python_version < "3.8" Requires-Dist: uvicorn
 [standard]<1,>=0.17.6 Requires-Dist: fastapi-utils<1,>=0.2.1 Requires-Dist:
 setuptools>=65.5.1
                                     [opal]
                            ************ ?â??¡OOPPAALL?â??¡ ************
                  ********** OOppeenn PPoolliiccyy AAddmmiinniissttrraattiioonn LLaayyeerr **********
 _[_T_e_s_t_s_]_[_P_a_c_k_a_g_e_]_[_P_a_c_k_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_c_k_e_r_ _p_u_l_l_s_]_[_J_o_i_n_ _o_u_r_ _S_l_a_c_k_!_]_[_h_t_t_p_s_:_/_/
```

### Comparing `opal-client-0.7.5/opal_client.egg-info/SOURCES.txt` & `opal_client-0.7.6/opal_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.5/setup.py` & `opal_client-0.7.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,20 +60,21 @@
         "": ["engine/healthcheck/opal.rego"],
     },
     classifiers=[
         "Operating System :: OS Independent",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
         "Topic :: Internet :: WWW/HTTP :: WSGI",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.9",
     install_requires=client_install_requires + about.get_install_requires(project_root),
     entry_points="""
     [console_scripts]
         opal-client=opal_client.cli:cli
     """,
 )
```

