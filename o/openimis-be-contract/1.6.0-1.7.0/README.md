# Comparing `tmp/openimis-be-contract-1.6.0.tar.gz` & `tmp/openimis_be_contract-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-contract-1.6.0.tar", last modified: Sat Dec 16 00:57:56 2023, max compression
+gzip compressed data, was "openimis_be_contract-1.7.0.tar", last modified: Tue Apr 30 09:06:41 2024, max compression
```

## Comparing `openimis-be-contract-1.6.0.tar` & `openimis_be_contract-1.7.0.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:56.899674 openimis-be-contract-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2023-12-16 00:57:56.899674 openimis-be-contract-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:56.891674 openimis-be-contract-1.6.0/contract/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:56.895674 openimis-be-contract-1.6.0/contract/gql/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/gql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:56.895674 openimis-be-contract-1.6.0/contract/gql/gql_mutations/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/gql/gql_mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/gql/gql_mutations/contract_details_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/gql/gql_mutations/contract_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/gql/gql_mutations/input_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    11658 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/gql/gql_mutations/mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/gql/gql_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:56.899674 openimis-be-contract-1.6.0/contract/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    15534 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0002_auto_20201221_1547.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0003_auto_20201222_1044.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0004_auto_20201222_1424.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0005_auto_20201228_1151.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0006_auto_20201228_1218.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0007_auto_20201228_1310.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0008_auto_20201230_1052.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0009_auto_20210118_1427.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0010_auto_20210119_1204.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0011_contractmutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0012_contractdetailsmutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0013_auto_20210202_0815.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0014_auto_20210208_1236.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0015_auto_20210208_1506.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0016_auto_20210208_1508.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0017_contract_roles_for_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0018_approve_ask_for_change_perms.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0019_amend_perms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/0020_auto_20230126_0903.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6889 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    48626 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/services.py
--rw-r--r--   0 runner    (1001) docker     (127)    12303 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:56.899674 openimis-be-contract-1.6.0/contract/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:56.899674 openimis-be-contract-1.6.0/contract/tests/gql_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/tests/gql_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/tests/gql_tests/mutation_create_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    23887 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/tests/gql_tests/query_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/tests/helpers_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:56.899674 openimis-be-contract-1.6.0/contract/tests/services/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16004 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/tests/services/services_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:46.000000 openimis-be-contract-1.6.0/contract/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:56.899674 openimis-be-contract-1.6.0/openimis_be_contract.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2023-12-16 00:57:56.000000 openimis-be-contract-1.6.0/openimis_be_contract.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2023-12-16 00:57:56.000000 openimis-be-contract-1.6.0/openimis_be_contract.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:57:56.000000 openimis-be-contract-1.6.0/openimis_be_contract.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-16 00:57:56.000000 openimis-be-contract-1.6.0/openimis_be_contract.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-16 00:57:56.000000 openimis-be-contract-1.6.0/openimis_be_contract.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:57:56.899674 openimis-be-contract-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2023-12-16 00:57:56.000000 openimis-be-contract-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.752252 openimis_be_contract-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-30 09:06:41.752252 openimis_be_contract-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.744253 openimis_be_contract-1.7.0/contract/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.744253 openimis_be_contract-1.7.0/contract/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/gql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.744253 openimis_be_contract-1.7.0/contract/gql/gql_mutations/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/gql/gql_mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/gql/gql_mutations/contract_details_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/gql/gql_mutations/contract_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/gql/gql_mutations/input_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11658 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/gql/gql_mutations/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/gql/gql_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.748252 openimis_be_contract-1.7.0/contract/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    15534 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0002_auto_20201221_1547.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0003_auto_20201222_1044.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0004_auto_20201222_1424.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0005_auto_20201228_1151.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0006_auto_20201228_1218.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0007_auto_20201228_1310.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0008_auto_20201230_1052.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0009_auto_20210118_1427.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0010_auto_20210119_1204.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0011_contractmutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0012_contractdetailsmutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0013_auto_20210202_0815.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0014_auto_20210208_1236.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0015_auto_20210208_1506.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0016_auto_20210208_1508.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0017_contract_roles_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0018_approve_ask_for_change_perms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0019_amend_perms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0020_auto_20230126_0903.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/0021_alter_contract_date_created_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52894 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.748252 openimis_be_contract-1.7.0/contract/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.752252 openimis_be_contract-1.7.0/contract/tests/gql_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/tests/gql_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/tests/gql_tests/mutation_create_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23894 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/tests/gql_tests/query_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/tests/helpers_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.752252 openimis_be_contract-1.7.0/contract/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15980 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/tests/services/services_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:27.000000 openimis_be_contract-1.7.0/contract/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.752252 openimis_be_contract-1.7.0/openimis_be_contract.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-30 09:06:41.000000 openimis_be_contract-1.7.0/openimis_be_contract.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-30 09:06:41.000000 openimis_be_contract-1.7.0/openimis_be_contract.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:06:41.000000 openimis_be_contract-1.7.0/openimis_be_contract.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-30 09:06:41.000000 openimis_be_contract-1.7.0/openimis_be_contract.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 09:06:41.000000 openimis_be_contract-1.7.0/openimis_be_contract.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:06:41.752252 openimis_be_contract-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-30 09:06:41.000000 openimis_be_contract-1.7.0/setup.py
```

### Comparing `openimis-be-contract-1.6.0/LICENSE.md` & `openimis_be_contract-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/PKG-INFO` & `openimis_be_contract-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-contract
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Contract reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-contract-1.6.0/README.md` & `openimis_be_contract-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/apps.py` & `openimis_be_contract-1.7.0/contract/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/config.py` & `openimis_be_contract-1.7.0/contract/config.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/gql/gql_mutations/contract_details_mutations.py` & `openimis_be_contract-1.7.0/contract/gql/gql_mutations/contract_details_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/gql/gql_mutations/contract_mutations.py` & `openimis_be_contract-1.7.0/contract/gql/gql_mutations/contract_mutations.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,24 +84,21 @@
             if not connection:
                 raise CeleryWorkerError("Celery worker not found. Please, contact your system administrator.")
         except (IOError, OperationalError) as e:
             raise CeleryWorkerError(
                 F"Celery connection has failed. Error: {e} \n Please, contact your system administrator.")
     @classmethod
     def approve_contracts(cls, user, contracts):
-        try:
-            cls._check_celery_status(cls)
-        except CeleryWorkerError as e:
-            return F"Celery connection has failed. Please, contact your system administrator."
+
         if "uuids" in contracts:
             contracts["uuids"] = list(contracts["uuids"].values_list("id", flat=True))
-            approve_contracts.delay(user_id=f'{user.id}', contracts=contracts["uuids"])
+            return approve_contracts(user_id=f'{user.id}', contracts=contracts["uuids"])
         else:
             if "contract_uuids" in contracts:
-                approve_contracts.delay(user_id=f'{user.id}', contracts=contracts["contract_uuids"])
+                return approve_contracts(user_id=f'{user.id}', contracts=contracts["contract_uuids"])
 
     class Input(ContractApproveBulkInputType):
         pass
 
 
 class CounterContractMutation(ContractCounterMutationMixin, BaseMutation):
     _mutation_class = "CounterContractMutation"
@@ -128,18 +125,18 @@
             cls.create_contract_invoice(user=user, contracts=data)
         return None
 
     @classmethod
     def create_contract_invoice(cls, user, contracts):
         if "uuids" in contracts:
             contracts["uuids"] = list(contracts["uuids"].values_list("id", flat=True))
-            create_invoice_from_contracts.delay(user_id=f'{user.id}', contracts=contracts["uuids"])
+            return create_invoice_from_contracts(user_id=f'{user.id}', contracts=contracts["uuids"])
         else:
             if "contract_uuids" in contracts:
-                create_invoice_from_contracts.delay(user_id=f'{user.id}', contracts=contracts["contract_uuids"])
+                return create_invoice_from_contracts(user_id=f'{user.id}', contracts=contracts["contract_uuids"])
 
     class Input(ContractCreateInvoiceBulkInputType):
         pass
 
 
 class CounterContractBulkMutation(ContractCounterMutationMixin, BaseMutation):
     _mutation_class = "CounterContractBulkMutation"
@@ -157,18 +154,18 @@
             cls.counter_contracts(user=user, contracts=data)
         return None
 
     @classmethod
     def counter_contracts(cls, user, contracts):
         if "uuids" in contracts:
             contracts["uuids"] = list(contracts["uuids"].values_list("id", flat=True))
-            counter_contracts.delay(user_id=f'{user.id}', contracts=contracts["uuids"])
+            return counter_contracts(user_id=f'{user.id}', contracts=contracts["uuids"])
         else:
             if "contract_uuids" in contracts:
-                counter_contracts.delay(user_id=f'{user.id}', contracts=contracts["contract_uuids"])
+                return counter_contracts(user_id=f'{user.id}', contracts=contracts["contract_uuids"])
 
     class Input(ContractCounterBulkInputType):
         pass
 
 
 class AmendContractMutation(ContractAmendMutationMixin, BaseMutation):
     _mutation_class = "AmendContractMutation"
```

### Comparing `openimis-be-contract-1.6.0/contract/gql/gql_mutations/input_types.py` & `openimis_be_contract-1.7.0/contract/gql/gql_mutations/input_types.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/gql/gql_mutations/mutations.py` & `openimis_be_contract-1.7.0/contract/gql/gql_mutations/mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/gql/gql_types.py` & `openimis_be_contract-1.7.0/contract/gql/gql_types.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0001_initial.py` & `openimis_be_contract-1.7.0/contract/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0002_auto_20201221_1547.py` & `openimis_be_contract-1.7.0/contract/migrations/0002_auto_20201221_1547.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0003_auto_20201222_1044.py` & `openimis_be_contract-1.7.0/contract/migrations/0003_auto_20201222_1044.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0004_auto_20201222_1424.py` & `openimis_be_contract-1.7.0/contract/migrations/0004_auto_20201222_1424.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0005_auto_20201228_1151.py` & `openimis_be_contract-1.7.0/contract/migrations/0005_auto_20201228_1151.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0006_auto_20201228_1218.py` & `openimis_be_contract-1.7.0/contract/migrations/0006_auto_20201228_1218.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0007_auto_20201228_1310.py` & `openimis_be_contract-1.7.0/contract/migrations/0007_auto_20201228_1310.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0008_auto_20201230_1052.py` & `openimis_be_contract-1.7.0/contract/migrations/0008_auto_20201230_1052.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0009_auto_20210118_1427.py` & `openimis_be_contract-1.7.0/contract/migrations/0009_auto_20210118_1427.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0010_auto_20210119_1204.py` & `openimis_be_contract-1.7.0/contract/migrations/0010_auto_20210119_1204.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0011_contractmutation.py` & `openimis_be_contract-1.7.0/contract/migrations/0011_contractmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0012_contractdetailsmutation.py` & `openimis_be_contract-1.7.0/contract/migrations/0012_contractdetailsmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0013_auto_20210202_0815.py` & `openimis_be_contract-1.7.0/contract/migrations/0013_auto_20210202_0815.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0014_auto_20210208_1236.py` & `openimis_be_contract-1.7.0/contract/migrations/0014_auto_20210208_1236.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0015_auto_20210208_1506.py` & `openimis_be_contract-1.7.0/contract/migrations/0015_auto_20210208_1506.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0016_auto_20210208_1508.py` & `openimis_be_contract-1.7.0/contract/migrations/0016_auto_20210208_1508.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0017_contract_roles_for_admin.py` & `openimis_be_contract-1.7.0/contract/migrations/0017_contract_roles_for_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/migrations/0020_auto_20230126_0903.py` & `openimis_be_contract-1.7.0/contract/migrations/0020_auto_20230126_0903.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/models.py` & `openimis_be_contract-1.7.0/contract/models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/schema.py` & `openimis_be_contract-1.7.0/contract/schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/services.py` & `openimis_be_contract-1.7.0/contract/services.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import json
-
+import uuid
+import traceback
+from django.conf import settings
 from copy import copy
 
 from django.core.exceptions import ValidationError
 
 from .config import get_message_counter_contract
 
 from django.db.models.query import Q
@@ -11,17 +13,19 @@
 from django.contrib.auth.models import AnonymousUser
 from django.core.serializers.json import DjangoJSONEncoder
 from django.core.mail import send_mail, BadHeaderError
 from django.forms.models import model_to_dict
 
 from contract.apps import ContractConfig
 from contract.signals import signal_contract, signal_contract_approve
-from contract.models import Contract as ContractModel, \
-    ContractDetails as ContractDetailsModel, \
-    ContractContributionPlanDetails as ContractContributionPlanDetailsModel
+from contract.models import (
+    Contract as ContractModel,
+    ContractDetails as ContractDetailsModel,
+    ContractContributionPlanDetails as ContractContributionPlanDetailsModel,
+)
 from calculation.services import run_calculation_rules
 
 from policyholder.models import PolicyHolderInsuree
 from contribution.models import Premium
 from contribution_plan.models import ContributionPlanBundleDetails, ContributionPlan
 
 from policy.models import Policy
@@ -66,462 +70,624 @@
 
     def __init__(self, user):
         self.user = user
 
     @check_authentication
     def create(self, contract):
         try:
-            incoming_code = contract.get('code')
+            incoming_code = contract.get("code")
             if check_unique_code(incoming_code):
-                raise ValidationError(("Contract code %s already exists" % incoming_code))
-            if not self.user.has_perms(ContractConfig.gql_mutation_create_contract_perms):
+                raise ValidationError(
+                    ("Contract code %s already exists" % incoming_code)
+                )
+            if not self.user.has_perms(
+                ContractConfig.gql_mutation_create_contract_perms
+            ):
                 raise PermissionError("Unauthorized")
             c = ContractModel(**contract)
             c.state = ContractModel.STATE_DRAFT
             c.save(username=self.user.username)
             uuid_string = f"{c.id}"
             # check if the PH is set
             if "policy_holder_id" in contract:
                 # run services updateFromPHInsuree and Contract Valuation
                 cd = ContractDetails(user=self.user)
-                result_ph_insuree = cd.update_from_ph_insuree(contract_details={
-                    "policy_holder_id": contract["policy_holder_id"],
-                    "contract_id": uuid_string,
-                    "amendment": 0,
-                })
+                result_ph_insuree = cd.update_from_ph_insuree(
+                    contract_details={
+                        "policy_holder_id": contract["policy_holder_id"],
+                        "contract_id": uuid_string,
+                        "amendment": 0,
+                    }
+                )
                 total_amount = self.evaluate_contract_valuation(
                     contract_details_result=result_ph_insuree,
                 )["total_amount"]
                 c.amount_notified = total_amount
             historical_record = c.history.all().last()
             c.json_ext = _save_json_external(
                 user_id=str(historical_record.user_updated.id),
                 datetime=str(historical_record.date_updated),
-                message=f"create contract status {historical_record.state}"
+                message=f"create contract status {historical_record.state}",
             )
             c.save(username=self.user.username)
             dict_representation = model_to_dict(c)
-            dict_representation['id'], dict_representation['uuid'] = (str(uuid_string), str(uuid_string))
+            dict_representation["id"], dict_representation["uuid"] = (
+                str(uuid_string),
+                str(uuid_string),
+            )
         except Exception as exc:
-            return _output_exception(model_name="Contract", method="create", exception=exc)
+            return _output_exception(
+                model_name="Contract", method="create", exception=exc
+            )
         return _output_result_success(dict_representation=dict_representation)
 
     def evaluate_contract_valuation(self, contract_details_result, save=False):
         ccpd = ContractContributionPlanDetails(user=self.user)
         result_contract_valuation = ccpd.contract_valuation(
             contract_contribution_plan_details={
                 "contract_details": contract_details_result["data"],
                 "save": save,
             }
         )
-        if not result_contract_valuation or result_contract_valuation["success"] is False:
+        if (
+            not result_contract_valuation
+            or result_contract_valuation["success"] is False
+        ):
             logger.error("contract valuation failed %s", str(result_contract_valuation))
-            raise Exception("contract valuation failed " + str(result_contract_valuation))
+            raise Exception(
+                "contract valuation failed " + str(result_contract_valuation)
+            )
         return result_contract_valuation["data"]
 
     # TODO update contract scenario according to wiki page
     @check_authentication
     def update(self, contract):
         try:
             # check rights for contract / amendments
-            if not (self.user.has_perms(ContractConfig.gql_mutation_update_contract_perms) or self.user.has_perms(
-                    ContractConfig.gql_mutation_approve_ask_for_change_contract_perms)):
+            if not (
+                self.user.has_perms(ContractConfig.gql_mutation_update_contract_perms)
+                or self.user.has_perms(
+                    ContractConfig.gql_mutation_approve_ask_for_change_contract_perms
+                )
+            ):
                 raise PermissionError("Unauthorized")
-            updated_contract = ContractModel.objects.filter(id=contract['id']).first()
+            updated_contract = ContractModel.objects.filter(id=contract["id"]).first()
             # updatable scenario
             if self.__check_rights_by_status(updated_contract.state) == "updatable":
                 if "code" in contract:
-                    raise ContractUpdateError("That fields are not editable in that permission!")
+                    raise ContractUpdateError(
+                        "That fields are not editable in that permission!"
+                    )
                 return _output_result_success(
                     dict_representation=self.__update_contract_fields(
-                        contract_input=contract,
-                        updated_contract=updated_contract
+                        contract_input=contract, updated_contract=updated_contract
                     )
                 )
             # approvable scenario
             if self.__check_rights_by_status(updated_contract.state) == "approvable":
                 # in “Negotiable” changes are possible only with the authority “Approve/ask for change”
-                if not self.user.has_perms(ContractConfig.gql_mutation_approve_ask_for_change_contract_perms):
+                if not self.user.has_perms(
+                    ContractConfig.gql_mutation_approve_ask_for_change_contract_perms
+                ):
                     raise PermissionError("Unauthorized")
                 return _output_result_success(
                     dict_representation=self.__update_contract_fields(
-                        contract_input=contract,
-                        updated_contract=updated_contract
+                        contract_input=contract, updated_contract=updated_contract
                     )
                 )
             if self.__check_rights_by_status(updated_contract.state) == "cannot_update":
                 raise ContractUpdateError("In that state you cannot update!")
         except Exception as exc:
-            return _output_exception(model_name="Contract", method="update", exception=exc)
+            return _output_exception(
+                model_name="Contract", method="update", exception=exc
+            )
 
     def __check_rights_by_status(self, status):
         state = "cannot_update"
-        if status in [ContractModel.STATE_DRAFT, ContractModel.STATE_REQUEST_FOR_INFORMATION,
-                      ContractModel.STATE_COUNTER]:
+        if status in [
+            ContractModel.STATE_DRAFT,
+            ContractModel.STATE_REQUEST_FOR_INFORMATION,
+            ContractModel.STATE_COUNTER,
+        ]:
             state = "updatable"
         if status == ContractModel.STATE_NEGOTIABLE:
             state = "approvable"
         return state
 
     def __update_contract_fields(self, contract_input, updated_contract):
         # get the current policy_holder value
         current_policy_holder_id = updated_contract.policy_holder_id
         [setattr(updated_contract, key, contract_input[key]) for key in contract_input]
         # check if PH is set and not changed
         if current_policy_holder_id:
-            if "policy_holder" in updated_contract.get_dirty_fields(check_relationship=True):
-                raise ContractUpdateError("You cannot update already set PolicyHolder in Contract!")
+            if "policy_holder" in updated_contract.get_dirty_fields(
+                check_relationship=True
+            ):
+                raise ContractUpdateError(
+                    "You cannot update already set PolicyHolder in Contract!"
+                )
         updated_contract.save(username=self.user.username)
         # save the communication
         historical_record = updated_contract.history.all().first()
         updated_contract.json_ext = _save_json_external(
             user_id=str(historical_record.user_updated.id),
             datetime=str(historical_record.date_updated),
-            message="update contract status " + str(historical_record.state)
+            message="update contract status " + str(historical_record.state),
         )
         updated_contract.save(username=self.user.username)
         uuid_string = f"{updated_contract.id}"
         dict_representation = model_to_dict(updated_contract)
-        dict_representation["id"], dict_representation["uuid"] = (str(uuid_string), str(uuid_string))
+        dict_representation["id"], dict_representation["uuid"] = (
+            str(uuid_string),
+            str(uuid_string),
+        )
         return dict_representation
 
     @check_authentication
     def submit(self, contract):
         try:
             # check for submittion right perms/authorites
-            if not self.user.has_perms(ContractConfig.gql_mutation_submit_contract_perms):
+            if not self.user.has_perms(
+                ContractConfig.gql_mutation_submit_contract_perms
+            ):
                 raise PermissionError("Unauthorized")
 
             contract_id = f"{contract['id']}"
             contract_to_submit = ContractModel.objects.filter(id=contract_id).first()
             contract_details_list = {}
             contract_details_list["data"] = self.__gather_policy_holder_insuree(
                 self.__validate_submission(contract_to_submit=contract_to_submit),
                 contract_to_submit.amendment,
                 contract_date_valid_from=None,
             )
             # contract valuation
             contract_contribution_plan_details = self.evaluate_contract_valuation(
                 contract_details_result=contract_details_list,
             )
-            contract_to_submit.amount_rectified = contract_contribution_plan_details["total_amount"]
+            contract_to_submit.amount_rectified = contract_contribution_plan_details[
+                "total_amount"
+            ]
             # send signal
             contract_to_submit.state = ContractModel.STATE_NEGOTIABLE
-            signal_contract.send(sender=ContractModel, contract=contract_to_submit, user=self.user)
+            signal_contract.send(
+                sender=ContractModel, contract=contract_to_submit, user=self.user
+            )
             dict_representation = model_to_dict(contract_to_submit)
-            dict_representation["id"], dict_representation["uuid"] = (contract_id, contract_id)
+            dict_representation["id"], dict_representation["uuid"] = (
+                contract_id,
+                contract_id,
+            )
             return _output_result_success(dict_representation=dict_representation)
         except Exception as exc:
-            return _output_exception(model_name="Contract", method="submit", exception=exc)
+            return _output_exception(
+                model_name="Contract", method="submit", exception=exc
+            )
 
     def __validate_submission(self, contract_to_submit):
         # check if we have a PolicyHoldes and any ContractDetails
         if not contract_to_submit.policy_holder:
             raise ContractUpdateError("The contract does not contain PolicyHolder!")
-        contract_details = ContractDetailsModel.objects.filter(contract_id=contract_to_submit.id)
+        contract_details = ContractDetailsModel.objects.filter(
+            contract_id=contract_to_submit.id
+        )
         if contract_details.count() == 0:
             raise ContractUpdateError("The contract does not contain any insuree!")
         # variable to check if we have right for submit
         state_right = self.__check_rights_by_status(contract_to_submit.state)
         # check if we can submit
         if state_right == "cannot_update":
-            raise ContractUpdateError("The contract cannot be submitted because of current state!")
+            raise ContractUpdateError(
+                "The contract cannot be submitted because of current state!"
+            )
         if state_right == "approvable":
             raise ContractUpdateError("The contract has been already submitted!")
         return list(contract_details.values())
 
-    def __gather_policy_holder_insuree(self, contract_details, amendment, contract_date_valid_from=None):
+    def __gather_policy_holder_insuree(
+        self, contract_details, amendment, contract_date_valid_from=None
+    ):
         result = []
         for cd in contract_details:
             ph_insuree = PolicyHolderInsuree.objects.filter(
-                Q(insuree_id=cd['insuree_id'], last_policy__isnull=False)).first()
+                Q(insuree_id=cd["insuree_id"], last_policy__isnull=False)
+            ).first()
             policy_id = ph_insuree.last_policy.id if ph_insuree else None
-            result.append({
-                "id": f"{cd['id']}",
-                "contribution_plan_bundle": f"{cd['contribution_plan_bundle_id']}",
-                "policy_id": policy_id,
-                "json_ext": cd['json_ext'],
-                "contract_date_valid_from": contract_date_valid_from,
-                "insuree_id": cd['insuree_id'],
-                "amendment": amendment
-            })
+            result.append(
+                {
+                    "id": f"{cd['id']}",
+                    "contribution_plan_bundle": f"{cd['contribution_plan_bundle_id']}",
+                    "policy_id": policy_id,
+                    "json_ext": cd["json_ext"],
+                    "contract_date_valid_from": contract_date_valid_from,
+                    "insuree_id": cd["insuree_id"],
+                    "amendment": amendment,
+                }
+            )
         return result
 
     @check_authentication
     def approve(self, contract):
         try:
             # check for approve/ask for change right perms/authorites
-            if not self.user.has_perms(ContractConfig.gql_mutation_approve_ask_for_change_contract_perms):
+            if not self.user.has_perms(
+                ContractConfig.gql_mutation_approve_ask_for_change_contract_perms
+            ):
                 raise PermissionError("Unauthorized")
             contract_id = f"{contract['id']}"
             contract_to_approve = ContractModel.objects.filter(id=contract_id).first()
             # variable to check if we have right to approve
             state_right = self.__check_rights_by_status(contract_to_approve.state)
             # check if we can submit
             if state_right != "approvable":
-                raise ContractUpdateError("You cannot approve this contract! The status of contract is not Negotiable!")
+                raise ContractUpdateError(
+                    "You cannot approve this contract! The status of contract is not Negotiable!"
+                )
             contract_details_list = {}
             contract_details_list["data"] = self.__gather_policy_holder_insuree(
-                list(ContractDetailsModel.objects.filter(contract_id=contract_to_approve.id).values()),
+                list(
+                    ContractDetailsModel.objects.filter(
+                        contract=contract_to_approve
+                    ).values()
+                ),
                 contract_to_approve.amendment,
                 contract_to_approve.date_valid_from,
             )
             # send signal - approve contract
             ccpd_service = ContractContributionPlanDetails(user=self.user)
             payment_service = PaymentService(user=self.user)
             signal_contract_approve.send(
                 sender=ContractModel,
                 contract=contract_to_approve,
                 user=self.user,
                 contract_details_list=contract_details_list,
                 service_object=self,
                 payment_service=payment_service,
-                ccpd_service=ccpd_service
+                ccpd_service=ccpd_service,
             )
             # ccpd.create_contribution(contract_contribution_plan_details)
             dict_representation = {}
             id_contract_approved = f"{contract_to_approve.id}"
-            dict_representation["id"], dict_representation["uuid"] = id_contract_approved, id_contract_approved
+            dict_representation["id"], dict_representation["uuid"] = (
+                id_contract_approved,
+                id_contract_approved,
+            )
             return _output_result_success(dict_representation=dict_representation)
         except Exception as exc:
-            return _output_exception(model_name="Contract", method="approve", exception=exc)
+            return _output_exception(
+                model_name="Contract", method="approve", exception=exc
+            )
 
     @check_authentication
     def counter(self, contract):
         try:
             # check for approve/ask for change right perms/authorites
-            if not self.user.has_perms(ContractConfig.gql_mutation_approve_ask_for_change_contract_perms):
+            if not self.user.has_perms(
+                ContractConfig.gql_mutation_approve_ask_for_change_contract_perms
+            ):
                 raise PermissionError("Unauthorized")
             contract_id = f"{contract['id']}"
             contract_to_counter = ContractModel.objects.filter(id=contract_id).first()
             # variable to check if we have right to approve
             state_right = self.__check_rights_by_status(contract_to_counter.state)
             # check if we can submit
             if state_right != "approvable":
-                raise ContractUpdateError("You cannot counter this contract! The status of contract is not Negotiable!")
+                raise ContractUpdateError(
+                    "You cannot counter this contract! The status of contract is not Negotiable!"
+                )
             contract_to_counter.state = ContractModel.STATE_COUNTER
-            signal_contract.send(sender=ContractModel, contract=contract_to_counter, user=self.user)
+            signal_contract.send(
+                sender=ContractModel, contract=contract_to_counter, user=self.user
+            )
             dict_representation = model_to_dict(contract_to_counter)
-            dict_representation["id"], dict_representation["uuid"] = (contract_id, contract_id)
+            dict_representation["id"], dict_representation["uuid"] = (
+                contract_id,
+                contract_id,
+            )
             email = _send_email_notify_counter(
                 code=contract_to_counter.code,
                 name=contract_to_counter.policy_holder.trade_name,
                 contact_name=contract_to_counter.policy_holder.contact_name,
                 email=contract_to_counter.policy_holder.email,
             )
             return _output_result_success(dict_representation=dict_representation)
         except Exception as exc:
-            return _output_exception(model_name="Contract", method="counter", exception=exc)
+            return _output_exception(
+                model_name="Contract", method="counter", exception=exc
+            )
 
     @check_authentication
     def amend(self, contract):
         try:
             # check for amend right perms/authorites
-            if not self.user.has_perms(ContractConfig.gql_mutation_amend_contract_perms):
+            if not self.user.has_perms(
+                ContractConfig.gql_mutation_amend_contract_perms
+            ):
                 raise PermissionError("Unauthorized")
             contract_id = f"{contract['id']}"
             contract_to_amend = ContractModel.objects.filter(id=contract_id).first()
             # variable to check if we have right to amend contract
             state_right = self.__check_rights_by_status(contract_to_amend.state)
             # check if we can amend
-            if state_right != "cannot_update" and contract_to_amend.state != ContractModel.STATE_TERMINATED:
+            if (
+                state_right != "cannot_update"
+                and contract_to_amend.state != ContractModel.STATE_TERMINATED
+            ):
                 raise ContractUpdateError("You cannot amend this contract!")
             # create copy of the contract
             amended_contract = copy(contract_to_amend)
             amended_contract.id = None
             amended_contract.amendment += 1
             amended_contract.state = ContractModel.STATE_DRAFT
             contract_to_amend.state = ContractModel.STATE_ADDENDUM
             from core import datetime
+
             contract_to_amend.date_valid_to = datetime.datetime.now()
             # update contract - also copy contract details etc
             contract.pop("id")
             [setattr(amended_contract, key, contract[key]) for key in contract]
             # check if chosen fields are not edited
-            if any(dirty_field in ["policy_holder", "code", "date_valid_from"] for dirty_field in
-                   amended_contract.get_dirty_fields(check_relationship=True)):
-                raise ContractUpdateError("You cannot update this field during amend contract!")
-            signal_contract.send(sender=ContractModel, contract=contract_to_amend, user=self.user)
-            signal_contract.send(sender=ContractModel, contract=amended_contract, user=self.user)
+            if any(
+                dirty_field in ["policy_holder", "code", "date_valid_from"]
+                for dirty_field in amended_contract.get_dirty_fields(
+                    check_relationship=True
+                )
+            ):
+                raise ContractUpdateError(
+                    "You cannot update this field during amend contract!"
+                )
+            signal_contract.send(
+                sender=ContractModel, contract=contract_to_amend, user=self.user
+            )
+            signal_contract.send(
+                sender=ContractModel, contract=amended_contract, user=self.user
+            )
             # copy also contract details
-            self.__copy_details(contract_id=contract_id, modified_contract=amended_contract)
+            self.__copy_details(
+                contract_id=contract_id, modified_contract=amended_contract
+            )
             # evaluate amended contract amount notified
             contract_details_list = {}
             contract_details_list["data"] = self.__gather_policy_holder_insuree(
-                list(ContractDetailsModel.objects.filter(contract_id=amended_contract.id).values()),
+                list(
+                    ContractDetailsModel.objects.filter(
+                        contract_id=amended_contract.id
+                    ).values()
+                ),
                 contract_to_amend.amendment,
             )
             contract_contribution_plan_details = self.evaluate_contract_valuation(
-                contract_details_result=contract_details_list,
-                save=False
+                contract_details_result=contract_details_list, save=False
             )
-            amended_contract.amount_notified = contract_contribution_plan_details["total_amount"]
+            amended_contract.amount_notified = contract_contribution_plan_details[
+                "total_amount"
+            ]
             if "amount_notified" in amended_contract.get_dirty_fields():
-                signal_contract.send(sender=ContractModel, contract=amended_contract, user=self.user)
+                signal_contract.send(
+                    sender=ContractModel, contract=amended_contract, user=self.user
+                )
             amended_contract_dict = model_to_dict(amended_contract)
             id_new_amended = f"{amended_contract.id}"
-            amended_contract_dict["id"], amended_contract_dict["uuid"] = (id_new_amended, id_new_amended)
+            amended_contract_dict["id"], amended_contract_dict["uuid"] = (
+                id_new_amended,
+                id_new_amended,
+            )
             return _output_result_success(dict_representation=amended_contract_dict)
         except Exception as exc:
-            return _output_exception(model_name="Contract", method="amend", exception=exc)
+            return _output_exception(
+                model_name="Contract", method="amend", exception=exc
+            )
 
     def __copy_details(self, contract_id, modified_contract):
-        list_cd = list(ContractDetailsModel.objects.filter(contract_id=contract_id).all())
+        list_cd = list(
+            ContractDetailsModel.objects.filter(contract_id=contract_id).all()
+        )
         for cd in list_cd:
             cd_new = copy(cd)
             cd_new.id = None
             cd_new.contract = modified_contract
             cd_new.save(username=self.user.username)
 
     @check_authentication
     def renew(self, contract):
         try:
             # check rights for renew contract
-            if not self.user.has_perms(ContractConfig.gql_mutation_renew_contract_perms):
+            if not self.user.has_perms(
+                ContractConfig.gql_mutation_renew_contract_perms
+            ):
                 raise PermissionError("Unauthorized")
             from core import datetime, datetimedelta
+
             contract_to_renew = ContractModel.objects.filter(id=contract["id"]).first()
             contract_id = contract["id"]
             # block renewing contract not in Updateable or Approvable state
             state_right = self.__check_rights_by_status(contract_to_renew.state)
             # check if we can renew
-            if state_right != "cannot_update" and contract_to_renew.state != ContractModel.STATE_TERMINATED:
+            if (
+                state_right != "cannot_update"
+                and contract_to_renew.state != ContractModel.STATE_TERMINATED
+            ):
                 raise ContractUpdateError("You cannot renew this contract!")
             # create copy of the contract - later we also copy contract detail
             renewed_contract = copy(contract_to_renew)
             # TO DO : if a policyholder is set, the contract details must be removed and PHinsuree imported again
             renewed_contract.id = None
             # Date to (the previous contract) became date From of the new contract (TBC if we need to add 1 day)
             # Date To of the new contract is calculated by DateFrom new contract + “Duration in month of previous contract“
-            length_contract = (contract_to_renew.date_valid_to.year - contract_to_renew.date_valid_from.year) * 12 \
-                              + (contract_to_renew.date_valid_to.month - contract_to_renew.date_valid_from.month)
-            renewed_contract.date_valid_from = contract_to_renew.date_valid_to + datetimedelta(days=1)
-            renewed_contract.date_valid_to = contract_to_renew.date_valid_to + datetimedelta(months=length_contract)
-            renewed_contract.state, renewed_contract.version = (ContractModel.STATE_DRAFT, 1)
+            length_contract = (
+                contract_to_renew.date_valid_to.year
+                - contract_to_renew.date_valid_from.year
+            ) * 12 + (
+                contract_to_renew.date_valid_to.month
+                - contract_to_renew.date_valid_from.month
+            )
+            renewed_contract.date_valid_from = (
+                contract_to_renew.date_valid_to + datetimedelta(days=1)
+            )
+            renewed_contract.date_valid_to = (
+                contract_to_renew.date_valid_to + datetimedelta(months=length_contract)
+            )
+            renewed_contract.state, renewed_contract.version = (
+                ContractModel.STATE_DRAFT,
+                1,
+            )
             renewed_contract.amount_rectified, renewed_contract.amount_due = (0, 0)
             renewed_contract.save(username=self.user.username)
             historical_record = renewed_contract.history.all().first()
             renewed_contract.json_ext = _save_json_external(
                 user_id=str(historical_record.user_updated.id),
                 datetime=str(historical_record.date_updated),
-                message=f"contract renewed - state "
-                        f"{historical_record.state}"
+                message=f"contract renewed - state " f"{historical_record.state}",
             )
             renewed_contract.save(username=self.user.username)
             # copy also contract details
-            self.__copy_details(contract_id=contract_id, modified_contract=renewed_contract)
+            self.__copy_details(
+                contract_id=contract_id, modified_contract=renewed_contract
+            )
             renewed_contract_dict = model_to_dict(renewed_contract)
             id_new_renewed = f"{renewed_contract.id}"
-            renewed_contract_dict["id"], renewed_contract_dict["uuid"] = (id_new_renewed, id_new_renewed)
+            renewed_contract_dict["id"], renewed_contract_dict["uuid"] = (
+                id_new_renewed,
+                id_new_renewed,
+            )
             return _output_result_success(dict_representation=renewed_contract_dict)
         except Exception as exc:
-            return _output_exception(model_name="Contract", method="renew", exception=exc)
+            return _output_exception(
+                model_name="Contract", method="renew", exception=exc
+            )
 
     @check_authentication
     def delete(self, contract):
         try:
             # check rights for delete contract
-            if not self.user.has_perms(ContractConfig.gql_mutation_delete_contract_perms):
+            if not self.user.has_perms(
+                ContractConfig.gql_mutation_delete_contract_perms
+            ):
                 raise PermissionError("Unauthorized")
             contract_to_delete = ContractModel.objects.filter(id=contract["id"]).first()
             # block deleting contract not in Updateable or Approvable state
-            if self.__check_rights_by_status(contract_to_delete.state) == "cannot_update":
+            if (
+                self.__check_rights_by_status(contract_to_delete.state)
+                == "cannot_update"
+            ):
                 raise ContractUpdateError("Contract in that state cannot be deleted")
             contract_to_delete.delete(username=self.user.username)
             return {
                 "success": True,
                 "message": "Ok",
                 "detail": "",
             }
         except Exception as exc:
-            return _output_exception(model_name="Contract", method="delete", exception=exc)
+            return _output_exception(
+                model_name="Contract", method="delete", exception=exc
+            )
 
     @check_authentication
     def terminate_contract(self):
         try:
             # TODO - add this service to the tasks.py in apscheduler once a day
             #  to check if contract might be terminated
             from core import datetime
-            contracts_to_terminate = list(ContractModel.objects.filter(
-                Q(date_valid_to__lt=datetime.datetime.now(), state=7)
-            ))
+
+            contracts_to_terminate = list(
+                ContractModel.objects.filter(
+                    Q(date_valid_to__lt=datetime.datetime.now(), state=7)
+                )
+            )
             if len(contracts_to_terminate) > 0:
                 for contract in contracts_to_terminate:
                     # we can marked that contract as a terminated
                     contract.state = ContractModel.STATE_TERMINATED
                     contract.save(username=self.user.username)
                     historical_record = contract.history.all().first()
                     contract.json_ext = _save_json_external(
                         user_id=str(historical_record.user_updated.id),
                         datetime=str(historical_record.date_updated),
                         message=f"contract terminated - state "
-                                f"{historical_record.state}"
+                        f"{historical_record.state}",
                     )
                     contract.save(username=self.user.username)
                 return {
                     "success": True,
                     "message": "Ok",
                     "detail": "",
                 }
             else:
                 return {
                     "success": False,
                     "message": "No contracts to terminate!",
                     "detail": "We do not have any contract to be terminated!",
                 }
         except Exception as exc:
-            return _output_exception(model_name="Contract", method="terminateContract", exception=exc)
+            return _output_exception(
+                model_name="Contract", method="terminateContract", exception=exc
+            )
 
     @check_authentication
     def get_negative_amount_amendment(self, credit_note):
         try:
             if not self.user.has_perms(ContractConfig.gql_query_contract_perms):
                 raise PermissionError("Unauthorized")
 
             contract_output_list = []
-            payment_detail = PaymentDetail.get_queryset(PaymentDetail.objects.filter(
-                payment__id=credit_note["id"]
-            )).prefetch_related(
-                'premium__contract_contribution_plan_details__contract_details__contract'
-            ).prefetch_related(
-                'premium__contract_contribution_plan_details'
-            ).filter(premium__contract_contribution_plan_details__isnull=False)
+            payment_detail = (
+                PaymentDetail.get_queryset(
+                    PaymentDetail.objects.filter(payment__id=credit_note["id"])
+                )
+                .prefetch_related(
+                    "premium__contract_contribution_plan_details__contract_details__contract"
+                )
+                .prefetch_related("premium__contract_contribution_plan_details")
+                .filter(premium__contract_contribution_plan_details__isnull=False)
+            )
 
             if len(list(payment_detail)) > 0:
                 contribution_list_id = [pd.premium.id for pd in payment_detail]
                 contract_list = ContractModel.objects.filter(
                     contractdetails__contractcontributionplandetails__contribution__id__in=contribution_list_id
                 ).distinct()
                 for contract in contract_list:
                     # look for approved contract (amendement)
-                    if contract.state in [ContractModel.STATE_EFFECTIVE,
-                                          ContractModel.STATE_EXECUTABLE] and contract.amendment > 0:
+                    if (
+                        contract.state
+                        in [
+                            ContractModel.STATE_EFFECTIVE,
+                            ContractModel.STATE_EXECUTABLE,
+                        ]
+                        and contract.amendment > 0
+                    ):
                         # get the contract which has the negative amount due
                         if contract.amount_due < 0:
                             contract_dict = model_to_dict(contract)
                             contract_id = f"{contract.id}"
-                            contract_dict["id"], contract_dict["uuid"] = (contract_id, contract_id)
+                            contract_dict["id"], contract_dict["uuid"] = (
+                                contract_id,
+                                contract_id,
+                            )
                             contract_output_list.append(contract_dict)
             # TODO not only get that contracts - but also do another things (it must be specified on wiki page)
             return _output_result_success(dict_representation=contract_output_list)
         except Exception as exc:
-            return _output_exception(model_name="Contract", method="getNegativeAmountAmendment", exception=exc)
+            return _output_exception(
+                model_name="Contract",
+                method="getNegativeAmountAmendment",
+                exception=exc,
+            )
 
 
 class ContractDetails(object):
 
     def __init__(self, user):
         self.user = user
 
     @check_authentication
     def update_from_ph_insuree(self, contract_details):
         try:
             contract_insuree_list = []
             policy_holder_insuree = PolicyHolderInsuree.objects.filter(
-                policy_holder__id=contract_details['policy_holder_id'],
+                policy_holder__id=contract_details["policy_holder_id"],
             )
             for phi in policy_holder_insuree:
                 # TODO add the validity condition also!
                 if phi.is_deleted is False and phi.contribution_plan_bundle:
                     cd = ContractDetailsModel(
                         **{
                             "contract_id": contract_details["contract_id"],
@@ -530,69 +696,91 @@
                             "json_ext": phi.json_ext,
                         }
                     )
                     # TODO add only the caclulation_rule section
                     cd.save(username=self.user.username)
                     uuid_string = f"{cd.id}"
                     dict_representation = model_to_dict(cd)
-                    dict_representation["id"], dict_representation["uuid"] = (uuid_string, uuid_string)
-                    dict_representation["policy_id"] = phi.last_policy.id if phi.last_policy else None
+                    dict_representation["id"], dict_representation["uuid"] = (
+                        uuid_string,
+                        uuid_string,
+                    )
+                    dict_representation["policy_id"] = (
+                        phi.last_policy.id if phi.last_policy else None
+                    )
                     dict_representation["amendment"] = contract_details["amendment"]
-                    dict_representation["contract_date_valid_from"] = cd.contract.date_valid_from
+                    dict_representation["contract_date_valid_from"] = (
+                        cd.contract.date_valid_from
+                    )
                     contract_insuree_list.append(dict_representation)
         except Exception as exc:
-            return _output_exception(model_name="ContractDetails", method="updateFromPHInsuree", exception=exc)
+            return _output_exception(
+                model_name="ContractDetails",
+                method="updateFromPHInsuree",
+                exception=exc,
+            )
         return _output_result_success(dict_representation=contract_insuree_list)
 
     @check_authentication
     def ph_insuree_to_contract_details(self, contract, ph_insuree):
         try:
             phi = PolicyHolderInsuree.objects.get(id=f'{ph_insuree["id"]}')
             # check for update contract right perms/authorites
-            if not self.user.has_perms(ContractConfig.gql_mutation_update_contract_perms):
+            if not self.user.has_perms(
+                ContractConfig.gql_mutation_update_contract_perms
+            ):
                 raise PermissionError("Unauthorized")
             if phi.is_deleted is False and phi.contribution_plan_bundle:
                 updated_contract = ContractModel.objects.get(id=f'{contract["id"]}')
-                if updated_contract.state not in [ContractModel.STATE_DRAFT,
-                                                  ContractModel.STATE_REQUEST_FOR_INFORMATION,
-                                                  ContractModel.STATE_COUNTER]:
+                if updated_contract.state not in [
+                    ContractModel.STATE_DRAFT,
+                    ContractModel.STATE_REQUEST_FOR_INFORMATION,
+                    ContractModel.STATE_COUNTER,
+                ]:
                     raise ContractUpdateError(
                         "You cannot update contract by adding insuree - contract not in updatable state!"
                     )
                 if updated_contract.policy_holder is None:
-                    raise ContractUpdateError(
-                        "There is no policy holder in contract!"
-                    )
+                    raise ContractUpdateError("There is no policy holder in contract!")
                 cd = ContractDetailsModel(
                     **{
                         "contract_id": contract["id"],
                         "insuree_id": phi.insuree.id,
                         "contribution_plan_bundle_id": f"{phi.contribution_plan_bundle.id}",
                     }
                 )
                 cd.save(username=self.user.username)
                 uuid_string = f"{cd.id}"
                 dict_representation = model_to_dict(cd)
-                dict_representation["id"], dict_representation["uuid"] = (uuid_string, uuid_string)
+                dict_representation["id"], dict_representation["uuid"] = (
+                    uuid_string,
+                    uuid_string,
+                )
                 return _output_result_success(dict_representation=dict_representation)
             else:
-                raise ContractUpdateError("You cannot insuree - is deleted or not enough data to create contract!")
+                raise ContractUpdateError(
+                    "You cannot insuree - is deleted or not enough data to create contract!"
+                )
         except Exception as exc:
-            return _output_exception(model_name="ContractDetails", method="PHInsureToCDetatils", exception=exc)
+            return _output_exception(
+                model_name="ContractDetails",
+                method="PHInsureToCDetatils",
+                exception=exc,
+            )
 
 
 class ContractContributionPlanDetails(object):
 
     def __init__(self, user):
         self.user = user
 
     @check_authentication
     def create_ccpd(self, ccpd, insuree_id):
-        """"
-            method to create contract contribution plan details
+        """ "
+        method to create contract contribution plan details
         """
         # get the relevant policy from the related product of contribution plan
         # policy objects get all related to this product
         insuree = Insuree.objects.filter(id=insuree_id).first()
         policies = self.__get_policy(
             insuree=insuree,
             date_valid_from=ccpd.date_valid_from,
@@ -617,61 +805,77 @@
             ccpd.policy = policies[1]
             ccpd_new.save(username=self.user.username)
             ccpd.save(username=self.user.username)
             return [ccpd_new, ccpd]
 
     def __get_policy(self, insuree, date_valid_from, date_valid_to, product):
         from core import datetime
+
         policy_output = []
         # get all policies related to the product and insuree
-        policies = Policy.objects.filter(product=product) \
-            .filter(family__head_insuree=insuree) \
+        policies = (
+            Policy.objects.filter(product=product)
+            .filter(family__head_insuree=insuree)
             .filter(start_date__lte=date_valid_to, expiry_date__gte=date_valid_from)
+        )
         # get covered policy, use count to run a COUNT query
         if policies.count() > 0:
-            policies_covered = list(policies.order_by('start_date'))
+            policies_covered = list(policies.order_by("start_date"))
         else:
             policies_covered = []
         missing_coverage = []
-        # make sure the policies covers the contract : 
+        # make sure the policies covers the contract :
         last_date_covered = date_valid_from
         # get the start date of the new contract by updating last_date_covered to the policy.stop_date
         while last_date_covered < date_valid_to and len(policies_covered) > 0:
             cur_policy = policies_covered.pop()
             # to check if it does take the first
             if cur_policy.start_date <= last_date_covered:
                 # Really unlikely we might create a policy that stop at curPolicy.startDate
                 # (start at curPolicy.startDate - product length) and add it to policy_output
                 last_date_covered = cur_policy.expiry_date
                 policy_output.append(cur_policy)
             elif cur_policy.expiry_date <= date_valid_to:
-                missing_coverage.append({'start': cur_policy.start_date, 'stop': last_date_covered})
+                missing_coverage.append(
+                    {"start": cur_policy.start_date, "stop": last_date_covered}
+                )
                 last_date_covered = cur_policy.expiry_date
                 policy_output.append(cur_policy)
 
         for data in missing_coverage:
-            policy_created, last_date_covered = self.create_contract_details_policies(insuree, product, data['start'],
-                                                                                      data['stop'])
+            policy_created, last_date_covered = self.create_contract_details_policies(
+                insuree, product, data["start"], data["stop"]
+            )
             if policy_created is not None and len(policy_created) > 0:
                 policy_output += policy_created
 
         # now we create new policy
         while last_date_covered < date_valid_to:
-            policy_created, last_date_covered = self.create_contract_details_policies(insuree, product,
-                                                                                      last_date_covered, date_valid_to)
+            policy_created, last_date_covered = self.create_contract_details_policies(
+                insuree, product, last_date_covered, date_valid_to
+            )
             if policy_created is not None and len(policy_created) > 0:
                 policy_output += policy_created
         return policy_output
 
-    def create_contract_details_policies(self, insuree, product, last_date_covered, date_valid_to):
+    def create_contract_details_policies(
+        self, insuree, product, last_date_covered, date_valid_to
+    ):
         # create policy for insuree familly
         # TODO Policy with status - new open=32 in policy-be_py module
         policy_output = []
+        # TODO support familyless insuree
+        if not insuree.family:
+            raise ValidationError(
+                f"insuree {insuree.chf_id} does not have a family, this is mandatory"
+            )
         while last_date_covered < date_valid_to:
-            expiry_date = last_date_covered + relativedelta(months=product.insurance_period)
+            expiry_date = last_date_covered + relativedelta(
+                months=product.insurance_period
+            )
             cur_policy = Policy.objects.create(
                 **{
                     "family": insuree.family,
                     "product": product,
                     "status": Policy.STATUS_ACTIVE,
                     "stage": Policy.STAGE_NEW,
                     "enroll_date": last_date_covered,
@@ -690,268 +894,320 @@
     @check_authentication
     def contract_valuation(self, contract_contribution_plan_details):
         try:
             dict_representation = {}
             ccpd_list = []
             total_amount = 0
             amendment = 0
-            for contract_details in contract_contribution_plan_details["contract_details"]:
+            for contract_details in contract_contribution_plan_details[
+                "contract_details"
+            ]:
                 cpbd_list = ContributionPlanBundleDetails.objects.filter(
-                    contribution_plan_bundle__id=str(contract_details["contribution_plan_bundle"])
+                    contribution_plan_bundle__id=str(
+                        contract_details["contribution_plan_bundle"]
+                    )
                 )
                 amendment = contract_details["amendment"]
                 for cpbd in cpbd_list:
                     ccpd = ContractContributionPlanDetailsModel(
                         **{
                             "contract_details_id": contract_details["id"],
                             "contribution_plan_id": f"{cpbd.contribution_plan.id}",
                             "policy_id": contract_details["policy_id"],
                         }
                     )
                     # rc - result of calculation
                     calculated_amount = 0
                     rc = run_calculation_rules(ccpd, "create", self.user)
                     if rc:
-                        calculated_amount = rc[0][1] if rc[0][1] not in [None, False] else 0
+                        calculated_amount = (
+                            rc[0][1] if rc[0][1] not in [None, False] else 0
+                        )
                         total_amount += calculated_amount
                     ccpd_record = model_to_dict(ccpd)
                     ccpd_record["calculated_amount"] = calculated_amount
                     if contract_contribution_plan_details["save"]:
-                        ccpd_list, total_amount, ccpd_record = self.__append_contract_cpd_to_list(
-                            ccpd=ccpd,
-                            cp=cpbd.contribution_plan,
-                            date_valid_from=contract_details["contract_date_valid_from"],
-                            insuree_id=contract_details["insuree_id"],
-                            total_amount=total_amount,
-                            calculated_amount=calculated_amount,
-                            ccpd_list=ccpd_list,
-                            ccpd_record=ccpd_record
+                        ccpd_list, total_amount, ccpd_record = (
+                            self.__append_contract_cpd_to_list(
+                                ccpd=ccpd,
+                                cp=cpbd.contribution_plan,
+                                date_valid_from=contract_details[
+                                    "contract_date_valid_from"
+                                ],
+                                insuree_id=contract_details["insuree_id"],
+                                total_amount=total_amount,
+                                calculated_amount=calculated_amount,
+                                ccpd_list=ccpd_list,
+                                ccpd_record=ccpd_record,
+                            )
                         )
                     if "id" not in ccpd_record:
                         ccpd_list.append(ccpd_record)
             if amendment > 0:
                 # get the payment from the previous version of the contract
-                contract_detail_id = contract_contribution_plan_details["contract_details"][0]["id"]
+                contract_detail_id = contract_contribution_plan_details[
+                    "contract_details"
+                ][0]["id"]
                 cd = ContractDetailsModel.objects.get(id=contract_detail_id)
                 contract_previous = ContractModel.objects.filter(
                     Q(amendment=amendment - 1, code=cd.contract.code)
                 ).first()
-                premium = ContractContributionPlanDetailsModel.objects.filter(
-                    contract_details__contract__id=f'{contract_previous.id}'
-                ).first().contribution
-                payment_detail_contribution = PaymentDetail.objects.filter(premium=premium).first()
+                premium = (
+                    ContractContributionPlanDetailsModel.objects.filter(
+                        contract_details__contract__id=f"{contract_previous.id}"
+                    )
+                    .first()
+                    .contribution
+                )
+                payment_detail_contribution = PaymentDetail.objects.filter(
+                    premium=premium
+                ).first()
                 payment_id = payment_detail_contribution.payment.id
                 payment_object = Payment.objects.get(id=payment_id)
-                received_amount = payment_object.received_amount if payment_object.received_amount else 0
+                received_amount = (
+                    payment_object.received_amount
+                    if payment_object.received_amount
+                    else 0
+                )
                 total_amount = float(total_amount) - float(received_amount)
-            dict_representation['total_amount'] = total_amount
-            dict_representation['contribution_plan_details'] = ccpd_list
+            dict_representation["total_amount"] = total_amount
+            dict_representation["contribution_plan_details"] = ccpd_list
             return _output_result_success(dict_representation=dict_representation)
         except Exception as exc:
             return _output_exception(
                 model_name="ContractContributionPlanDetails",
                 method="contractValuation",
-                exception=exc
+                exception=exc,
             )
 
-    def __append_contract_cpd_to_list(self, ccpd, cp, date_valid_from, insuree_id, total_amount,
-                                      calculated_amount, ccpd_list, ccpd_record):
+    def __append_contract_cpd_to_list(
+        self,
+        ccpd,
+        cp,
+        date_valid_from,
+        insuree_id,
+        total_amount,
+        calculated_amount,
+        ccpd_list,
+        ccpd_record,
+    ):
         """helper private function to gather results to the list
-           ccpd - contract contribution plan details
-           cp - contribution plan
-           return ccpd list and total amount
+        ccpd - contract contribution plan details
+        cp - contribution plan
+        return ccpd list and total amount
         """
         from core import datetime, datetimedelta
+
         # TODO - catch grace period from calculation rule if is defined
         #  grace_period = cp.calculation_rule etc
         #  length = cp.get_contribution_length(grace_period)
         length = cp.get_contribution_length()
         ccpd.date_valid_from = date_valid_from
         ccpd.date_valid_to = date_valid_from + datetimedelta(months=length)
         # TODO: calculate the number of CCPD to create in order to cover the contract lenght
         ccpd_results = self.create_ccpd(ccpd, insuree_id)
         ccpd_record = model_to_dict(ccpd)
         ccpd_record["calculated_amount"] = calculated_amount
         # TODO: support more that 2 CCPD
         # case 1 - single contribution
         if len(ccpd_results) == 1:
             uuid_string = f"{ccpd_results[0].id}"
-            ccpd_record['id'], ccpd_record['uuid'] = (uuid_string, uuid_string)
+            ccpd_record["id"], ccpd_record["uuid"] = (uuid_string, uuid_string)
             ccpd_list.append(ccpd_record)
         # case 2 - 2 contributions with 2 policies
         else:
             # there is additional contribution - we have to calculate/recalculate
             total_amount = total_amount - calculated_amount
             for ccpd_result in ccpd_results:
-                length_ccpd = float((ccpd_result.date_valid_to.year - ccpd_result.date_valid_from.year) * 12 \
-                                    + (ccpd_result.date_valid_to.month - ccpd_result.date_valid_from.month))
+                length_ccpd = float(
+                    (ccpd_result.date_valid_to.year - ccpd_result.date_valid_from.year)
+                    * 12
+                    + (
+                        ccpd_result.date_valid_to.month
+                        - ccpd_result.date_valid_from.month
+                    )
+                )
                 periodicity = float(ccpd_result.contribution_plan.periodicity)
                 # time part of splited as a fraction to count contribution value for that splited period properly
                 part_time_period = length_ccpd / periodicity
                 # rc - result calculation
                 rc = run_calculation_rules(ccpd, "update", self.user)
                 if rc:
-                    calculated_amount = rc[0][1] * part_time_period if rc[0][1] not in [None, False] else 0
+                    calculated_amount = (
+                        rc[0][1] * part_time_period
+                        if rc[0][1] not in [None, False]
+                        else 0
+                    )
                     total_amount += calculated_amount
                 ccpd_record = model_to_dict(ccpd_result)
                 ccpd_record["calculated_amount"] = calculated_amount
                 uuid_string = f"{ccpd_result.id}"
-                ccpd_record['id'], ccpd_record['uuid'] = (uuid_string, uuid_string)
+                ccpd_record["id"], ccpd_record["uuid"] = (uuid_string, uuid_string)
                 ccpd_list.append(ccpd_record)
         return ccpd_list, total_amount, ccpd_record
 
     @check_authentication
     def create_contribution(self, contract_contribution_plan_details):
         try:
             dict_representation = {}
             contribution_list = []
             from core import datetime
+
             now = datetime.datetime.now()
             for ccpd in contract_contribution_plan_details["contribution_plan_details"]:
-                contract_details = ContractDetailsModel.objects.get(id=f"{ccpd['contract_details']}")
+                contract_details = ContractDetailsModel.objects.get(
+                    id=f"{ccpd['contract_details']}"
+                )
                 # create the contributions based on the ContractContributionPlanDetails
                 if ccpd["contribution"] is None:
                     contribution = Premium.objects.create(
                         **{
                             "policy_id": ccpd["policy"],
                             "amount": ccpd["calculated_amount"],
                             "audit_user_id": -1,
                             "pay_date": now,
                             # TODO Temporary value pay_type - I have to get to know about this field what should be here
                             #  also ask about audit_user_id and pay_date value
                             "pay_type": " ",
+                            "receipt": str(uuid.uuid4()),
                         }
                     )
-                    ccpd_object = ContractContributionPlanDetailsModel.objects.get(id=ccpd["id"])
+                    ccpd_object = ContractContributionPlanDetailsModel.objects.get(
+                        id=ccpd["id"]
+                    )
                     ccpd_object.contribution = contribution
                     ccpd_object.save(username=self.user.username)
                     contribution_record = model_to_dict(contribution)
                     contribution_list.append(contribution_record)
                     dict_representation["contributions"] = contribution_list
             return _output_result_success(dict_representation=dict_representation)
         except Exception as exc:
             return _output_exception(
                 model_name="ContractContributionPlanDetails",
                 method="createContribution",
-                exception=exc
+                exception=exc,
             )
 
 
 class PaymentService(object):
 
     def __init__(self, user):
         self.user = user
 
     @check_authentication
     def create(self, payment, payment_details=None):
         try:
             dict_representation = {}
             payment_list = []
             from core import datetime
+
             now = datetime.datetime.now()
             p = update_or_create_payment(data=payment, user=self.user)
             dict_representation = model_to_dict(p)
-            dict_representation['id'], dict_representation['uuid'] = (p.id, p.uuid)
+            dict_representation["id"], dict_representation["uuid"] = (p.id, p.uuid)
             if payment_details:
                 for payment_detail in payment_details:
                     pd = PaymentDetail.objects.create(
                         payment=Payment.objects.get(id=p.id),
                         audit_user_id=-1,
                         validity_from=now,
                         product_code=payment_detail["product_code"],
                         insurance_number=payment_detail["insurance_number"],
                         expected_amount=payment_detail["expected_amount"],
-                        premium=payment_detail["premium"]
+                        premium=payment_detail["premium"],
                     )
                     pd_record = model_to_dict(pd)
-                    pd_record['id'] = pd.id
+                    pd_record["id"] = pd.id
                     payment_list.append(pd_record)
             dict_representation["payment_details"] = payment_list
             return _output_result_success(dict_representation=dict_representation)
         except Exception as exc:
             return _output_exception(
-                model_name="Payment",
-                method="createPayment",
-                exception=exc
+                model_name="Payment", method="createPayment", exception=exc
             )
 
     @check_authentication
     def collect_payment_details(self, contract_contribution_plan_details):
         payment_details_data = []
         for ccpd in contract_contribution_plan_details:
-            product_code = ContributionPlan.objects.get(id=ccpd["contribution_plan"]).benefit_plan.code
-            insurance_number = ContractDetailsModel.objects.get(id=ccpd["contract_details"]).insuree.chf_id
-            contribution = ContractContributionPlanDetailsModel.objects.get(id=ccpd["id"]).contribution
+            product_code = ContributionPlan.objects.get(
+                id=ccpd["contribution_plan"]
+            ).benefit_plan.code
+            insurance_number = ContractDetailsModel.objects.get(
+                id=ccpd["contract_details"]
+            ).insuree.chf_id
+            contribution = ContractContributionPlanDetailsModel.objects.get(
+                id=ccpd["id"]
+            ).contribution
             expected_amount = ccpd["calculated_amount"]
-            payment_details_data.append({
-                "product_code": product_code,
-                "insurance_number": insurance_number,
-                "expected_amount": expected_amount,
-                "premium": contribution
-            })
+            payment_details_data.append(
+                {
+                    "product_code": product_code,
+                    "insurance_number": insurance_number,
+                    "expected_amount": expected_amount,
+                    "premium": contribution,
+                }
+            )
         return payment_details_data
 
 
 class ContractToInvoiceService(object):
 
     def __init__(self, user):
         self.user = user
 
     @classmethod
-    @register_service_signal('create_invoice_from_contract')
+    @register_service_signal("create_invoice_from_contract")
     def create_invoice(self, instance, convert_to="Invoice", **kwargs):
-        """ run convert the ContractContributionPlanDetails of the contract to invoice lines"""
+        """run convert the ContractContributionPlanDetails of the contract to invoice lines"""
         pass
 
 
 def _output_exception(model_name, method, exception):
     return {
         "success": False,
         "message": f"Failed to {method} {model_name}",
         "detail": f"{exception}",
-        "data": "",
+        "data": traceback.format_exc() if settings.DEBUG else "",
     }
 
 
 def _output_result_success(dict_representation):
     return {
         "success": True,
         "message": "Ok",
         "detail": "",
         "data": json.loads(json.dumps(dict_representation, cls=DjangoJSONEncoder)),
     }
 
 
 def _save_json_external(user_id, datetime, message):
     return {
-        "comments": [{
-            "From": "Portal/webapp",
-            "user": user_id,
-            "date": datetime,
-            "msg": message
-        }]
+        "comments": [
+            {"From": "Portal/webapp", "user": user_id, "date": datetime, "msg": message}
+        ]
     }
 
 
 def _send_email_notify_counter(code, name, contact_name, email):
     try:
         email_to_send = send_mail(
-            subject='Contract counter notification',
+            subject="Contract counter notification",
             message=get_message_counter_contract(
-                language=settings.LANGUAGE_CODE.split('-')[0],
+                language=settings.LANGUAGE_CODE.split("-")[0],
                 code=code,
                 name=name,
                 contact_name=contact_name,
             ),
             from_email=settings.EMAIL_HOST_USER,
             recipient_list=[email],
             fail_silently=False,
         )
         return email_to_send
     except BadHeaderError:
-        return ValueError('Invalid header found.')
+        return ValueError("Invalid header found.")
 
 
 def check_unique_code(code):
     if ContractModel.objects.filter(code=code, is_deleted=False).exists():
         return [{"message": "Contract code %s already exists" % code}]
     return []
```

### Comparing `openimis-be-contract-1.6.0/contract/signals.py` & `openimis_be_contract-1.7.0/contract/signals.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from policyholder.apps import PolicyholderConfig
 from policyholder.models import PolicyHolderUser
 from insuree.models import InsureePolicy
 
 _contract_signal_params = ["contract", "user"]
 _contract_approve_signal_params = ["contract", "user", "contract_details_list", "service_object", "payment_service",
                                    "ccpd_service"]
-signal_contract = Signal(providing_args=_contract_signal_params)
-signal_contract_approve = Signal(providing_args=_contract_signal_params)
+signal_contract = Signal(_contract_signal_params)
+signal_contract_approve = Signal(_contract_signal_params)
 
 
 def on_contract_signal(sender, **kwargs):
     contract = kwargs["contract"]
     user = kwargs["user"]
     __save_or_update_contract(contract=contract, user=user)
     return f"contract updated - state {contract.state}"
@@ -48,51 +48,57 @@
     result_payment = __create_payment(contract_to_approve, payment_service, contract_contribution_plan_details)
     # STATE_EXECUTABLE
     from core import datetime
     now = datetime.datetime.now()
     contract_to_approve.date_approved = now
     contract_to_approve.state = 5
     approved_contract = __save_or_update_contract(contract=contract_to_approve, user=user)
-    email_contact_name = contract_to_approve.policy_holder.contact_name["contactName"] \
-        if "contactName" in contract_to_approve.policy_holder.contact_name \
-        else contract_to_approve.policy_holder.contact_name
-    email = __send_email_notify_payment(
-        code=contract_to_approve.code,
-        name=contract_to_approve.policy_holder.trade_name,
-        contact_name=email_contact_name,
-        amount_due=contract_to_approve.amount_due,
-        payment_reference=contract_to_approve.payment_reference,
-        email=contract_to_approve.policy_holder.email,
-    )
+    if contract_to_approve.policy_holder.email:
+        email_contact_name = contract_to_approve.policy_holder.contact_name["contactName"] \
+            if (contract_to_approve.policy_holder.contact_name and "contactName" in contract_to_approve.policy_holder.contact_name) \
+            else contract_to_approve.policy_holder.trade_name or contract_to_approve.policy_holder.code
+        email = __send_email_notify_payment(
+            code=contract_to_approve.code,
+            name=contract_to_approve.policy_holder.trade_name,
+            contact_name=email_contact_name,
+            amount_due=contract_to_approve.amount_due,
+            payment_reference=contract_to_approve.payment_reference,
+            email=contract_to_approve.policy_holder.email,
+        )
     return approved_contract
 
 
 # additional filters for payment in 'contract' tab
 def append_contract_filter(sender, **kwargs):
     user = kwargs.get("user", None)
     additional_filter = kwargs.get('additional_filter', None)
     if "contract" in additional_filter:
         # then check perms
         if user.has_perms(PaymentConfig.gql_query_payments_perms) or user.has_perms(
                 PolicyholderConfig.gql_query_payment_portal_perms):
             contract_id = additional_filter["contract"]
             contract_to_process = Contract.objects.filter(id=contract_id).first()
+
+            if not contract_to_process or not contract_to_process.policy_holder:
+                return Q(pk=-1)
             # check if user is linked to ph in policy holder user table
             type_user = f"{user}"
             # related to user object output (i) or (t)
             # check if we have interactive user from current context
             if '(i)' in type_user:
                 from core import datetime
                 now = datetime.datetime.now()
+
                 ph_user = PolicyHolderUser.objects.filter(
                     Q(policy_holder__id=contract_to_process.policy_holder.id, user__id=user.id)
                 ).filter(
                     Q(date_valid_from=None) | Q(date_valid_from__lte=now),
                     Q(date_valid_to=None) | Q(date_valid_to__gte=now)
                 ).first()
+
                 if ph_user or user.has_perms(PaymentConfig.gql_query_payments_perms):
                     return Q(
                         payment_details__premium__contract_contribution_plan_details__contract_details__contract__id=contract_id
                     )
 
 
 # additional filters for InsureePolicy in contract
@@ -101,39 +107,44 @@
     additional_filter = kwargs.get('additional_filter', None)
     if "contract" in additional_filter:
         # then check perms
         if user.has_perms(InsureeConfig.gql_query_insuree_policy_perms) or user.has_perms(
                 PolicyholderConfig.gql_query_insuree_policy_portal_perms):
             contract_id = additional_filter["contract"]
             contract_to_process = Contract.objects.filter(id=contract_id).first()
+            if not contract_to_process or not contract_to_process.policy_holder:
+                return Q(pk=-1)
             # check if user is linked to ph in policy holder user table
             type_user = f"{user}"
             # related to user object output (i) or (t)
             # check if we have interactive user from current context
             if '(i)' in type_user:
                 from core import datetime
                 now = datetime.datetime.now()
                 ph_user = PolicyHolderUser.objects.filter(
                     Q(policy_holder__id=contract_to_process.policy_holder.id, user__id=user.id)
                 ).filter(
                     Q(date_valid_from=None) | Q(date_valid_from__lte=now),
                     Q(date_valid_to=None) | Q(date_valid_to__gte=now)
                 ).first()
+
                 if ph_user or user.has_perms(InsureeConfig.gql_query_insuree_policy_perms):
                     policies = list(
                         ContractContributionPlanDetails.objects.filter(
                             contract_details__contract__id=contract_id).values_list("policy", flat=True)
                     )
+
                     return Q(
                         start_date__gte=contract_to_process.date_valid_from,
                         start_date__lte=contract_to_process.date_valid_to,
                         policy__in=policies
                     )
 
 
+
 # check if policy is related to formal sector contract
 def formal_sector_policies(sender, **kwargs):
     policy_id = kwargs.get('policy_id', None)
     ccpd = ContractContributionPlanDetails.objects.filter(policy__id=policy_id, is_deleted=False).first()
     if ccpd:
         cd = ccpd.contract_details
         contract = cd.contract
```

### Comparing `openimis-be-contract-1.6.0/contract/tasks.py` & `openimis_be_contract-1.7.0/contract/tasks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import logging
 
-from celery import shared_task
 from core.models import User
 from contract.models import Contract, ContractContributionPlanDetails
 from contract.services import Contract as ContractService, ContractToInvoiceService
 
 
 logger = logging.getLogger(__name__)
 
 
-@shared_task
 def approve_contracts(user_id, contracts):
+    output = []
     user = User.objects.get(id=user_id)
     contract_service = ContractService(user=user)
     for contract in contracts:
-        output = contract_service.approve(contract={"id": contract})
+        output.append(contract_service.approve(contract={"id": contract}))
+    return output
 
-
-@shared_task
 def counter_contracts(user_id, contracts):
+    output = []
     user = User.objects.get(id=user_id)
     contract_service = ContractService(user=user)
     for contract in contracts:
-        output = contract_service.counter(contract={"id": contract})
-
+        output.append(contract_service.counter(contract={"id": contract}))
+    return output
 
-@shared_task
 def create_invoice_from_contracts(user_id, contracts):
+    output = []
     user = User.objects.get(id=user_id)
     contract_service = ContractToInvoiceService(user=user)
     for contract in contracts:
         contract_instance = Contract.objects.filter(id=contract)
         if contract_instance:
             contract_instance = contract_instance.first()
             ccpd_list = ContractContributionPlanDetails.objects.filter(contract_details__contract=contract_instance)
-            output = contract_service.create_invoice(
+            output.append(contract_service.create_invoice(
                 instance=contract_instance,
                 convert_to="InvoiceLine",
                 user=user,
                 ccpd_list=ccpd_list
-            )
+            ))
+    return output
```

### Comparing `openimis-be-contract-1.6.0/contract/tests/gql_tests/mutation_create_tests.py` & `openimis_be_contract-1.7.0/contract/tests/gql_tests/mutation_create_tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,176 +2,222 @@
 from unittest import mock
 from django.test import TestCase
 
 import graphene
 from contract.tests.helpers import *
 from contract.models import Contract, ContractDetails
 from core.models import TechnicalUser
-from core.test_helpers import create_test_technical_user
+from core.models.openimis_graphql_test_case import openIMISGraphQLTestCase
+from core.test_helpers import create_test_interactive_user
 from policyholder.tests.helpers import *
-from contribution_plan.tests.helpers import create_test_contribution_plan, \
-    create_test_contribution_plan_bundle, create_test_contribution_plan_bundle_details
+from contribution_plan.tests.helpers import (
+    create_test_contribution_plan,
+    create_test_contribution_plan_bundle,
+    create_test_contribution_plan_bundle_details,
+)
 from contract import schema as contract_schema
 from graphene import Schema
 from graphene.test import Client
+from graphene_django.utils.testing import GraphQLTestCase
+from django.conf import settings
+import json
+import uuid
+from graphql_jwt.shortcuts import get_token
+
+
+class MutationTestContract(openIMISGraphQLTestCase):
+    GRAPHQL_URL = f"/{settings.SITE_ROOT()}graphql"
+    # This is required by some version of graphene but is never used. It should be set to the schema but the import
+    # is shown as an error in the IDE, so leaving it as True.
+    GRAPHQL_SCHEMA = True
+    admin_user = None
+    schema = Schema(
+        query=contract_schema.Query,
+    )
 
-
-class MutationTestContract(TestCase):
     class BaseTestContext:
         def __init__(self, user):
             self.user = user
 
     class AnonymousUserContext:
         user = mock.Mock(is_anonymous=True)
 
     @classmethod
     def setUpClass(cls):
         super(MutationTestContract, cls).setUpClass()
-        if not TechnicalUser.objects.filter(username='admin').exists():
-            create_test_technical_user(username='admin', password='S\/pe®Pąßw0rd™', super_user=True)
-        cls.user = User.objects.filter(username='admin').first()
+        cls.user = User.objects.filter(username="admin", i_user__isnull=False).first()
+        if not cls.user:
+            cls.user = create_test_interactive_user(username="admin")
         # some test data so as to created contract properly
+        cls.user_token = get_token(cls.user, cls.BaseTestContext(user=cls.user))
+
         cls.income = 500
         cls.rate = 5
         cls.number_of_insuree = 2
         cls.policy_holder = create_test_policy_holder()
         cls.policy_holder2 = create_test_policy_holder()
         # create contribution plans etc
         cls.contribution_plan_bundle = create_test_contribution_plan_bundle()
         cls.contribution_plan = create_test_contribution_plan(
             custom_props={"json_ext": {"calculation_rule": {"rate": cls.rate}}}
         )
-        cls.contribution_plan_bundle_details = create_test_contribution_plan_bundle_details(
-            contribution_plan=cls.contribution_plan,
-            contribution_plan_bundle=cls.contribution_plan_bundle
+        cls.contribution_plan_bundle_details = (
+            create_test_contribution_plan_bundle_details(
+                contribution_plan=cls.contribution_plan,
+                contribution_plan_bundle=cls.contribution_plan_bundle,
+            )
         )
         from core import datetime
+
         # create policy holder insuree for that test policy holder
         for i in range(0, cls.number_of_insuree):
             ph_insuree = create_test_policy_holder_insuree(
                 policy_holder=cls.policy_holder,
                 contribution_plan_bundle=cls.contribution_plan_bundle,
                 custom_props={
                     "last_policy": None,
-                    "json_ext": {"calculation_rule": {"income": cls.income}}
-                }
+                    "json_ext": {"calculation_rule": {"income": cls.income}},
+                },
             )
             create_test_policy(
                 cls.contribution_plan.benefit_plan,
                 ph_insuree.insuree,
                 custom_props={
                     "start_date": datetime.datetime(2016, 3, 1),
-                    "expiry_date": datetime.datetime(2021, 7, 1)
-                }
+                    "expiry_date": datetime.datetime(2021, 7, 1),
+                },
             )
-
+        # TODO support familyless insuree
+        # cls.insuree_wo_family = create_test_insuree(with_family=False)
+        cls.insuree_wo_family = create_test_insuree(with_family=True)
         cls.policy_holder_insuree = create_test_policy_holder_insuree(
+            insuree=cls.insuree_wo_family,
             policy_holder=cls.policy_holder,
-            contribution_plan_bundle=cls.contribution_plan_bundle
+            contribution_plan_bundle=cls.contribution_plan_bundle,
         )
         cls.policy_holder_insuree2 = create_test_policy_holder_insuree(
             policy_holder=cls.policy_holder,
-            contribution_plan_bundle=cls.contribution_plan_bundle
+            contribution_plan_bundle=cls.contribution_plan_bundle,
         )
 
         cls.schema = Schema(
-            query=contract_schema.Query,
-            mutation=contract_schema.Mutation
+            query=contract_schema.Query, mutation=contract_schema.Mutation
         )
         cls.graph_client = Client(cls.schema)
 
     def test_mutation_contract_create_without_policy_holder(self):
         time_stamp = datetime.datetime.now()
         input_param = {
             "code": "XYZ:" + str(time_stamp),
         }
-        self.add_mutation("createContract", input_param)
+        self.add_mutation("createContract", input_param, self.user_token)
         result = self.find_by_exact_attributes_query(
             "contract",
             params=input_param,
         )["edges"]
-        converted_id = base64.b64decode(result[0]['node']['id']).decode('utf-8').split(':')[1]
+        # converted_id = base64.b64decode(result[0]['node']['id']).decode('utf-8').split(':')[1]
         # tear down the test data
-        Contract.objects.filter(id=str(converted_id)).delete()
-        self.assertEqual(
-            (
-                "XYZ:" + str(time_stamp),
-            )
-            ,
-            (
-                result[0]['node']['code'],
-            )
-        )
+        # Contract.objects.filter(id=str(converted_id)).delete()
+        self.assertEqual(("XYZ:" + str(time_stamp),), (result[0]["node"]["code"],))
 
     def test_mutation_contract_create_with_policy_holder(self):
         time_stamp = datetime.datetime.now()
         input_param = {
             "code": "XYZ:" + str(time_stamp),
-            "policyHolderId": str(self.policy_holder.id)
+            "policyHolderId": str(self.policy_holder.id),
+            "clientMutationId": str(uuid.uuid4()),
         }
-        self.add_mutation("createContract", input_param)
+        content = self.send_mutation("createContract", input_param, self.user_token)
+        self.assertEqual(
+            content["data"]["mutationLogs"]["edges"][0]["node"]["status"], 2
+        )
+        del input_param["clientMutationId"]
         result = self.find_by_exact_attributes_query(
             "contract",
             params=input_param,
         )["edges"]
-        converted_id = base64.b64decode(result[0]['node']['id']).decode('utf-8').split(':')[1]
-        # tear down the test data
-        ContractDetails.objects.filter(contract_id=str(converted_id)).delete()
-        Contract.objects.filter(id=str(converted_id)).delete()
+        converted_id = (
+            base64.b64decode(result[0]["node"]["id"]).decode("utf-8").split(":")[1]
+        )
 
+        # SUBMIT
+        input_param = {"id": converted_id, "clientMutationId": str(uuid.uuid4())}
+        content = self.send_mutation("submitContract", input_param, self.user_token)
+        content = self.assertEqual(
+            content["data"]["mutationLogs"]["edges"][0]["node"]["status"], 2
+        )
+
+        # COUNTER
+        input_param = {"id": converted_id, "clientMutationId": str(uuid.uuid4())}
+        content = self.send_mutation("counterContract", input_param, self.user_token)
+
+        content = self.assertEqual(
+            content["data"]["mutationLogs"]["edges"][0]["node"]["status"], 2
+        )
+
+        # reSUBMIT
+        input_param = {"id": converted_id, "clientMutationId": str(uuid.uuid4())}
+        content = self.send_mutation("submitContract", input_param, self.user_token)
         self.assertEqual(
-            (
-                "XYZ:" + str(time_stamp),
-            )
-            ,
-            (
-                result[0]['node']['code'],
-            )
+            content["data"]["mutationLogs"]["edges"][0]["node"]["status"], 2
         )
+        # Approve
+        input_param = {"id": converted_id, "clientMutationId": str(uuid.uuid4())}
+        content = self.send_mutation("approveContract", input_param, self.user_token)
+
+        self.assertEqual(
+            content["data"]["mutationLogs"]["edges"][0]["node"]["status"], 2
+        )
+
+        # tear down the test data (TODO FK conflict with mutation )
+        # ContractDetails.objects.filter(contract_id=str(converted_id)).delete()
+        # Contract.objects.filter(id=str(converted_id)).delete()
 
     def find_by_id_query(self, query_type, id, context=None):
-        query = F'''
+        query = f"""
         {{
             {query_type}(id:"{id}") {{
                 totalCount
                 edges {{
                   node {{
                     id
                     version
                   }}
                   cursor
                 }}
           }}
         }}
-        '''
+        """
 
         query_result = self.execute_query(query, context=context)
-        records = query_result[query_type]['edges']
+        records = query_result[query_type]["edges"]
 
         if len(records) > 1:
-            raise ValueError(F"Ambiguous id {id} for query {query_type}")
+            raise ValueError(f"Ambiguous id {id} for query {query_type}")
 
         return records
 
     def find_by_exact_attributes_query(self, query_type, params, context=None):
         if "dateValidFrom" in params:
-            params.pop('dateValidFrom')
+            params.pop("dateValidFrom")
+        if "clientMutationId" in params:
+            params.pop("clientMutationId")
         if "dateValidTo" in params:
-            params.pop('dateValidTo')
+            params.pop("dateValidTo")
         if "policyHolderId" in params:
-            params.pop('policyHolderId')
+            params.pop("policyHolderId")
         if "contributionPlanBundleId" in params:
-            params.pop('contributionPlanBundleId')
+            params.pop("contributionPlanBundleId")
         if "insureeId" in params:
-            params.pop('insureeId')
+            params.pop("insureeId")
         if "uuids" in params:
             params["id"] = params["uuids"][0]
             params.pop("uuids")
-        node_content_str = "\n".join(params.keys()) if query_type == "contract" else ''
-        query = F'''
+        node_content_str = "\n".join(params.keys()) if query_type == "contract" else ""
+        query = f"""
         {{
             {query_type}({'contract_Id: "' + str(params["contractId"]) + '", orderBy: ["-dateCreated"]' if "contractId" in params else self.build_params(params)}) {{
                 totalCount
                 edges {{
                   node {{
                     id
                     {node_content_str}
@@ -182,59 +228,68 @@
                     {'state' if query_type == 'contract' else ''}
                     {'paymentReference' if query_type == 'contract' else ''}
                   }}
                   cursor
                 }}
           }}
         }}
-        '''
+        """
         query_result = self.execute_query(query, context=context)
         records = query_result[query_type]
         return records
 
     def execute_query(self, query, context=None):
         if context is None:
             context = self.BaseTestContext(self.user)
 
         query_result = self.graph_client.execute(query, context=context)
-        query_data = query_result['data']
+        query_data = query_result["data"]
         return query_data
 
     def add_mutation(self, mutation_type, input_params, context=None):
-        mutation = f'''
+
+        if "clientMutationId" not in input_params:
+            input_params["clientMutationId"] = str(uuid.uuid4())
+        mutation = f"""
         mutation 
         {{
             {mutation_type}(input: {{
                {self.build_params(input_params)}
             }})  
 
           {{
             internalId
             clientMutationId
           }}
         }}
-        '''
-        mutation_result = self.execute_mutation(mutation, context=context)
-        return mutation_result
+        """
+        mutation_result = self.query(
+            mutation,
+            headers={"HTTP_AUTHORIZATION": f"Bearer {self.user_token}"},
+        )
+        self.assertResponseNoErrors(mutation_result)
+        content = json.loads(mutation_result.content)
+        return content
 
     def execute_mutation(self, mutation, context=None):
         if context is None:
             context = self.BaseTestContext(self.user)
 
         mutation_result = self.graph_client.execute(mutation, context=context)
         return mutation_result
 
     def build_params(self, params):
         def wrap_arg(v):
             if isinstance(v, str):
-                return F'"{v}"'
+                return f'"{v}"'
             if isinstance(v, list):
                 return json.dumps(v)
             if isinstance(v, bool):
                 return str(v).lower()
             if isinstance(v, datetime.date):
                 return graphene.DateTime.serialize(
-                    datetime.datetime.fromordinal(v.toordinal()))
+                    datetime.datetime.fromordinal(v.toordinal())
+                )
             return v
 
-        params_as_args = [f'{k}:{wrap_arg(v)}' for k, v in params.items()]
+        params_as_args = [f"{k}:{wrap_arg(v)}" for k, v in params.items()]
         return ", ".join(params_as_args)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openimis-be-contract-1.6.0/contract/tests/gql_tests/query_tests.py` & `openimis_be_contract-1.7.0/contract/tests/gql_tests/query_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,15 @@
         query_result = self.execute_query(query)
         result = query_result['contractContributionPlanDetails']['edges'][0]['node']
         converted_id = base64.b64decode(result['id']).decode('utf-8').split(':')[1]
         self.assertEqual(UUID(converted_id), id)
 
     def test_find_contract_by_contract_code_date_valid_from_gte(self):
         code = self.test_contract.code
-        date_valid_from = str(self.test_contract.date_valid_from) + 'T00:00:00'
+        date_valid_from = str(self.test_contract.date_valid_from.date()) + 'T00:00:00'
         id = self.test_contract.id
         query = F'''
         {{
             contract(
                 code: "{code}", dateValidFrom_Gte: "{date_valid_from}"){{
                 totalCount
                 edges {{
```

### Comparing `openimis-be-contract-1.6.0/contract/tests/helpers.py` & `openimis_be_contract-1.7.0/contract/tests/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
                 "policy_id": policy.id,
                 "payer_id": None,
                 "amount": 1000,
                 "receipt": "Test receipt",
                 "pay_date": "2019-01-01",
                 "validity_from": "2019-01-01",
                 "audit_user_id": -1,
+                "pay_type": 'C'
             }
         )
 
     user = __get_or_create_simple_contract_user()
     object_data = {
         'contribution_plan': contribution_plan,
         'policy': policy,
```

### Comparing `openimis-be-contract-1.6.0/contract/tests/helpers_tests.py` & `openimis_be_contract-1.7.0/contract/tests/helpers_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/contract/tests/services/services_tests.py` & `openimis_be_contract-1.7.0/contract/tests/services/services_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     def test_contract_create_without_policy_holder(self):
         contract = {
             'code': 'AAAAAA',
         }
         response = self.contract_service.create(contract)
         # tear down the test data
-        Contract.objects.filter(id=response["data"]["id"]).delete()
+        #Contract.objects.filter(id=response["data"]["id"]).delete()
         self.assertEqual(
             (
                 True,
                 "Ok",
                 "",
                 "AAAAAA",
                 0,
@@ -87,16 +87,16 @@
     def test_contract_create_with_policy_holder(self):
         contract = {
             'code': 'TESTONE',
             'policy_holder_id': self.policy_holder.id
         }
         response = self.contract_service.create(contract)
         # tear down the test data
-        ContractDetails.objects.filter(contract_id=response["data"]["id"]).delete()
-        Contract.objects.filter(id=response["data"]["id"]).delete()
+        #ContractDetails.objects.filter(contract_id=response["data"]["id"]).delete()
+        #Contract.objects.filter(id=response["data"]["id"]).delete()
         self.assertEqual(
             (
                 True,
                 "Ok",
                 "",
                 "TESTONE",
                 0,
@@ -128,16 +128,16 @@
         contract = {
             "id": contract_id,
         }
         response = self.contract_service.delete(contract)
         is_deleted = response['success']
 
         # tear down the test data
-        ContractDetails.objects.filter(contract_id=contract_id).delete()
-        Contract.objects.filter(id=contract_id).delete()
+        #ContractDetails.objects.filter(contract_id=contract_id).delete()
+        #Contract.objects.filter(id=contract_id).delete()
 
         self.assertEqual(
             ("payment_one xxxxxxxx", True),
             (updated_payment_reference, is_deleted)
         )
 
     def test_contract_create_update_failed_ph(self):
@@ -152,16 +152,16 @@
             "id": contract_id,
             "policy_holder_id": str(self.policy_holder2.id),
         }
         response = self.contract_service.update(contract)
         failed = response['detail']
 
         # tear down the test data
-        ContractDetails.objects.filter(contract_id=contract_id).delete()
-        Contract.objects.filter(id=contract_id).delete()
+        #ContractDetails.objects.filter(contract_id=contract_id).delete()
+        #Contract.objects.filter(id=contract_id).delete()
 
         self.assertEqual(
             "ContractUpdateError: You cannot update already set PolicyHolder in Contract!", failed,
         )
 
     def test_contract_create_submit_fail_scenarios(self):
         contract = {
@@ -195,16 +195,16 @@
 
         response = self.contract_service.submit(contract)
         result_message3 = response["detail"]
         expected_message3 = "ContractUpdateError: The contract does not contain PolicyHolder!"
 
         # tear down the test data
         list_cd = list(ContractDetails.objects.filter(contract_id=contract_id).values('id', 'json_ext'))
-        ContractDetails.objects.filter(contract_id=contract_id).delete()
-        Contract.objects.filter(id=contract_id).delete()
+        #ContractDetails.objects.filter(contract_id=contract_id).delete()
+        #Contract.objects.filter(id=contract_id).delete()
 
         self.assertEqual(
             (
                 expected_message,
                 expected_message2,
                 expected_message3
             ),
@@ -229,18 +229,18 @@
         self.contract_service.submit(contract)
         response = self.contract_service.counter(contract)
         result_state = response["data"]["state"]
         expected_state = 11
 
         # tear down the test data
         list_cd = list(ContractDetails.objects.filter(contract_id=contract_id).values('id'))
-        for cd in list_cd:
-            ccpd = ContractContributionPlanDetails.objects.filter(contract_details__id=f"{cd['id']}").delete()
-        ContractDetails.objects.filter(contract_id=contract_id).delete()
-        Contract.objects.filter(id=contract_id).delete()
+        #for cd in list_cd:
+        #    ccpd = ContractContributionPlanDetails.objects.filter(contract_details__id=f"{cd['id']}").delete()
+        #ContractDetails.objects.filter(contract_id=contract_id).delete()
+        #Contract.objects.filter(id=contract_id).delete()
 
         self.assertEqual(
             expected_state, result_state
         )
 
     def test_contract_create_submit(self):
         from core import datetime
@@ -256,16 +256,16 @@
         response = self.contract_service.submit(contract)
         expected_state = 4
         result_state = response["data"]["state"]
         # tear down the test data
         list_cd = list(ContractDetails.objects.filter(contract_id=contract_id).values('id'))
         for cd in list_cd:
             ContractContributionPlanDetails.objects.filter(contract_details__id=f"{cd['id']}").delete()
-        ContractDetails.objects.filter(contract_id=contract_id).delete()
-        Contract.objects.filter(id=contract_id).delete()
+        #ContractDetails.objects.filter(contract_id=contract_id).delete()
+        #Contract.objects.filter(id=contract_id).delete()
         self.assertEqual(
             expected_state, result_state
         )
 
     def test_contract_create_cd_from_phi(self):
         from core import datetime
         ph_insuree2 = create_test_policy_holder_insuree(
@@ -284,16 +284,16 @@
         contract = {"id": contract_id, }
         ph_insuree_input = {"id": f'{ph_insuree2.id}', }
         response = self.contract_details_service.ph_insuree_to_contract_details(
             contract=contract,
             ph_insuree=ph_insuree_input
         )
         # tear down the test data
-        ContractDetails.objects.filter(contract_id=contract_id).delete()
-        Contract.objects.filter(id=contract_id).delete()
+        #ContractDetails.objects.filter(contract_id=contract_id).delete()
+        #Contract.objects.filter(id=contract_id).delete()
 
         self.assertEqual(
             True, response["success"]
         )
 
 
 class CalculationContractTest(TestCase):
@@ -342,15 +342,15 @@
         class_name = "PolicyHolderInsuree"
         class_name2 = "ContributionPlan"
         result = get_rule_details(class_name=class_name)[0][1]
         result2 = get_rule_details(class_name=class_name2)[0][1]
         result_param = [param["name"] for param in result["parameters"]]
         result2_param = [param["name"] for param in result2["parameters"]]
         self.assertEqual(
-            (class_name, class_name2, ["income"], ["rate", "includeFamilly"]),
+            (class_name, class_name2, ["income"], ["rate", "includeFamily"]),
             (result["class"], result2["class"], result_param, result2_param)
         )
 
     def test_get_rule_details_not_existing(self):
         class_name = "xxxxxxxxxxxxxxx"
         result = get_rule_details(class_name=class_name)
         self.assertEqual(None, result[0][1])
@@ -373,19 +373,20 @@
             'policy_holder_id': self.policy_holder.id
         }
 
         response = self.contract_service.create(contract)
         # after creating contract - we can get contract details so as to get params
         # run calculation rules etc
         cd = ContractDetails.objects.filter(contract__id=response["data"]["id"]).first()
+        c = Contract.objects.filter(id=response["data"]["id"]).first()
         result_params = get_parameters("PolicyHolderInsuree", cd)
 
         # tear down the contract test data
-        ContractDetails.objects.filter(contract_id=response["data"]["id"]).delete()
-        Contract.objects.filter(id=response["data"]["id"]).delete()
+        #cd.delete()
+        #c.delete()
 
         # we want to assert name of param related to the contract details (should be 'income')
         # and also the value of contract (all contributions)
         # for that test should be income=500, 5 insurees, default rate=5 %
         # income*rate*number of contributions = according to Contribution Valuation Rule
         self.assertEqual(
             ("income", self.income * (float(self.rate / 100)) * self.number_of_insuree),
```

### Comparing `openimis-be-contract-1.6.0/contract/utils.py` & `openimis_be_contract-1.7.0/contract/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.6.0/openimis_be_contract.egg-info/PKG-INFO` & `openimis_be_contract-1.7.0/openimis_be_contract.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-contract
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Contract reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-contract-1.6.0/openimis_be_contract.egg-info/SOURCES.txt` & `openimis_be_contract-1.7.0/openimis_be_contract.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 contract/migrations/0014_auto_20210208_1236.py
 contract/migrations/0015_auto_20210208_1506.py
 contract/migrations/0016_auto_20210208_1508.py
 contract/migrations/0017_contract_roles_for_admin.py
 contract/migrations/0018_approve_ask_for_change_perms.py
 contract/migrations/0019_amend_perms.py
 contract/migrations/0020_auto_20230126_0903.py
+contract/migrations/0021_alter_contract_date_created_and_more.py
 contract/migrations/__init__.py
 contract/tests/__init__.py
 contract/tests/helpers.py
 contract/tests/helpers_tests.py
 contract/tests/gql_tests/__init__.py
 contract/tests/gql_tests/mutation_create_tests.py
 contract/tests/gql_tests/query_tests.py
```

### Comparing `openimis-be-contract-1.6.0/setup.py` & `openimis_be_contract-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-contract',
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Contract reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

