# Comparing `tmp/openimis-be-policyholder-1.6.0.tar.gz` & `tmp/openimis_be_policyholder-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-policyholder-1.6.0.tar", last modified: Sat Dec 16 00:57:47 2023, max compression
+gzip compressed data, was "openimis_be_policyholder-1.7.0.tar", last modified: Tue Apr 30 09:06:27 2024, max compression
```

## Comparing `openimis-be-policyholder-1.6.0.tar` & `openimis_be_policyholder-1.7.0.tar`

### file list

```diff
@@ -1,63 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:47.750398 openimis-be-policyholder-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2023-12-16 00:57:47.746398 openimis-be-policyholder-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:47.746398 openimis-be-policyholder-1.6.0/openimis_be_policyholder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2023-12-16 00:57:47.000000 openimis-be-policyholder-1.6.0/openimis_be_policyholder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2023-12-16 00:57:47.000000 openimis-be-policyholder-1.6.0/openimis_be_policyholder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:57:47.000000 openimis-be-policyholder-1.6.0/openimis_be_policyholder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-12-16 00:57:47.000000 openimis-be-policyholder-1.6.0/openimis_be_policyholder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-16 00:57:47.000000 openimis-be-policyholder-1.6.0/openimis_be_policyholder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:47.742397 openimis-be-policyholder-1.6.0/policyholder/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:47.742397 openimis-be-policyholder-1.6.0/policyholder/gql/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/gql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:47.742397 openimis-be-policyholder-1.6.0/policyholder/gql/gql_mutations/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/gql/gql_mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/gql/gql_mutations/create_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/gql/gql_mutations/delete_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/gql/gql_mutations/input_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/gql/gql_mutations/replace_mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/gql/gql_mutations/update_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/gql/gql_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:47.746398 openimis-be-policyholder-1.6.0/policyholder/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    21878 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0002_auto_20201214_1237.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0003_auto_20201214_1239.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0004_auto_20201214_1302.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0005_auto_20210111_1254.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0006_policyholdercontributionplanmutation_policyholderinsureemutation_policyholdermutation_policyholderus.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0007_auto_20210118_0927.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0008_auto_20210118_1109.py
--rw-r--r--   0 runner    (1001) docker     (127)     6921 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0009_auto_20210118_1127.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0010_auto_20210126_1040.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0011_auto_20210408_0937.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0012_auto_20210408_0949.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0013_auto_20210408_0951.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0014_auto_20210408_1007.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0015_auto_20210624_1243.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0016_policyholder_roles_for_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/0017_auto_20230126_0903.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8409 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10297 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    15720 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:47.746398 openimis-be-policyholder-1.6.0/policyholder/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/tests/helpers_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:47.746398 openimis-be-policyholder-1.6.0/policyholder/tests/services/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20660 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/tests/services/services_ph_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:47.746398 openimis-be-policyholder-1.6.0/policyholder/validation/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/validation/permission_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/validation/policyholder_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:39.000000 openimis-be-policyholder-1.6.0/policyholder/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:57:47.750398 openimis-be-policyholder-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2023-12-16 00:57:47.000000 openimis-be-policyholder-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:27.790035 openimis_be_policyholder-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-30 09:06:27.790035 openimis_be_policyholder-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:27.790035 openimis_be_policyholder-1.7.0/openimis_be_policyholder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-30 09:06:27.000000 openimis_be_policyholder-1.7.0/openimis_be_policyholder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-30 09:06:27.000000 openimis_be_policyholder-1.7.0/openimis_be_policyholder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:06:27.000000 openimis_be_policyholder-1.7.0/openimis_be_policyholder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 09:06:27.000000 openimis_be_policyholder-1.7.0/openimis_be_policyholder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 09:06:27.000000 openimis_be_policyholder-1.7.0/openimis_be_policyholder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:27.782034 openimis_be_policyholder-1.7.0/policyholder/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:27.782034 openimis_be_policyholder-1.7.0/policyholder/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/gql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:27.786034 openimis_be_policyholder-1.7.0/policyholder/gql/gql_mutations/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/gql/gql_mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/gql/gql_mutations/create_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/gql/gql_mutations/delete_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/gql/gql_mutations/input_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/gql/gql_mutations/replace_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/gql/gql_mutations/update_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/gql/gql_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:27.786034 openimis_be_policyholder-1.7.0/policyholder/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:27.786034 openimis_be_policyholder-1.7.0/policyholder/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/management/commands/generatepolicyholders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:27.790035 openimis_be_policyholder-1.7.0/policyholder/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    21878 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0002_auto_20201214_1237.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0003_auto_20201214_1239.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0004_auto_20201214_1302.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0005_auto_20210111_1254.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0006_policyholdercontributionplanmutation_policyholderinsureemutation_policyholdermutation_policyholderus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0007_auto_20210118_0927.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0008_auto_20210118_1109.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0009_auto_20210118_1127.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0010_auto_20210126_1040.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0011_auto_20210408_0937.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0012_auto_20210408_0949.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0013_auto_20210408_0951.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0014_auto_20210408_1007.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0015_auto_20210624_1243.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0016_policyholder_roles_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0017_auto_20230126_0903.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8374 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/0018_alter_historicalpolicyholder_date_created_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15720 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:27.790035 openimis_be_policyholder-1.7.0/policyholder/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/tests/helpers_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:27.790035 openimis_be_policyholder-1.7.0/policyholder/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20898 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/tests/services/services_ph_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:27.790035 openimis_be_policyholder-1.7.0/policyholder/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/validation/permission_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/validation/policyholder_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:16.000000 openimis_be_policyholder-1.7.0/policyholder/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:06:27.790035 openimis_be_policyholder-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-30 09:06:27.000000 openimis_be_policyholder-1.7.0/setup.py
```

### Comparing `openimis-be-policyholder-1.6.0/LICENSE.md` & `openimis_be_policyholder-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/PKG-INFO` & `openimis_be_policyholder-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-policyholder
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend PolicyHolder reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-policyholder-1.6.0/README.md` & `openimis_be_policyholder-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/openimis_be_policyholder.egg-info/PKG-INFO` & `openimis_be_policyholder-1.7.0/openimis_be_policyholder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-policyholder
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend PolicyHolder reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-policyholder-1.6.0/openimis_be_policyholder.egg-info/SOURCES.txt` & `openimis_be_policyholder-1.7.0/openimis_be_policyholder.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 policyholder/gql/gql_types.py
 policyholder/gql/gql_mutations/__init__.py
 policyholder/gql/gql_mutations/create_mutations.py
 policyholder/gql/gql_mutations/delete_mutations.py
 policyholder/gql/gql_mutations/input_types.py
 policyholder/gql/gql_mutations/replace_mutation.py
 policyholder/gql/gql_mutations/update_mutations.py
+policyholder/management/__init__.py
+policyholder/management/commands/__init__.py
+policyholder/management/commands/generatepolicyholders.py
 policyholder/migrations/0001_initial.py
 policyholder/migrations/0002_auto_20201214_1237.py
 policyholder/migrations/0003_auto_20201214_1239.py
 policyholder/migrations/0004_auto_20201214_1302.py
 policyholder/migrations/0005_auto_20210111_1254.py
 policyholder/migrations/0006_policyholdercontributionplanmutation_policyholderinsureemutation_policyholdermutation_policyholderus.py
 policyholder/migrations/0007_auto_20210118_0927.py
@@ -37,14 +40,15 @@
 policyholder/migrations/0011_auto_20210408_0937.py
 policyholder/migrations/0012_auto_20210408_0949.py
 policyholder/migrations/0013_auto_20210408_0951.py
 policyholder/migrations/0014_auto_20210408_1007.py
 policyholder/migrations/0015_auto_20210624_1243.py
 policyholder/migrations/0016_policyholder_roles_for_admin.py
 policyholder/migrations/0017_auto_20230126_0903.py
+policyholder/migrations/0018_alter_historicalpolicyholder_date_created_and_more.py
 policyholder/migrations/__init__.py
 policyholder/tests/__init__.py
 policyholder/tests/helpers.py
 policyholder/tests/helpers_tests.py
 policyholder/tests/services/__init__.py
 policyholder/tests/services/services_ph_tests.py
 policyholder/validation/__init__.py
```

### Comparing `openimis-be-policyholder-1.6.0/policyholder/apps.py` & `openimis_be_policyholder-1.7.0/policyholder/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/gql/gql_mutations/create_mutations.py` & `openimis_be_policyholder-1.7.0/policyholder/gql/gql_mutations/create_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/gql/gql_mutations/delete_mutations.py` & `openimis_be_policyholder-1.7.0/policyholder/gql/gql_mutations/delete_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/gql/gql_mutations/input_types.py` & `openimis_be_policyholder-1.7.0/policyholder/gql/gql_mutations/input_types.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/gql/gql_mutations/replace_mutation.py` & `openimis_be_policyholder-1.7.0/policyholder/gql/gql_mutations/replace_mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/gql/gql_mutations/update_mutations.py` & `openimis_be_policyholder-1.7.0/policyholder/gql/gql_mutations/update_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/gql/gql_types.py` & `openimis_be_policyholder-1.7.0/policyholder/gql/gql_types.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/migrations/0001_initial.py` & `openimis_be_policyholder-1.7.0/policyholder/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/migrations/0002_auto_20201214_1237.py` & `openimis_be_policyholder-1.7.0/policyholder/migrations/0002_auto_20201214_1237.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/migrations/0003_auto_20201214_1239.py` & `openimis_be_policyholder-1.7.0/policyholder/migrations/0003_auto_20201214_1239.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/migrations/0004_auto_20201214_1302.py` & `openimis_be_policyholder-1.7.0/policyholder/migrations/0004_auto_20201214_1302.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/migrations/0005_auto_20210111_1254.py` & `openimis_be_policyholder-1.7.0/policyholder/migrations/0005_auto_20210111_1254.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/migrations/0006_policyholdercontributionplanmutation_policyholderinsureemutation_policyholdermutation_policyholderus.py` & `openimis_be_policyholder-1.7.0/policyholder/migrations/0006_policyholdercontributionplanmutation_policyholderinsureemutation_policyholdermutation_policyholderus.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/migrations/0007_auto_20210118_0927.py` & `openimis_be_policyholder-1.7.0/policyholder/migrations/0007_auto_20210118_0927.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/migrations/0008_auto_20210118_1109.py` & `openimis_be_policyholder-1.7.0/policyholder/migrations/0008_auto_20210118_1109.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/migrations/0009_auto_20210118_1127.py` & `openimis_be_policyholder-1.7.0/policyholder/migrations/0009_auto_20210118_1127.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/migrations/0010_auto_20210126_1040.py` & `openimis_be_policyholder-1.7.0/policyholder/migrations/0010_auto_20210126_1040.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/migrations/0015_auto_20210624_1243.py` & `openimis_be_policyholder-1.7.0/policyholder/migrations/0015_auto_20210624_1243.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/migrations/0016_policyholder_roles_for_admin.py` & `openimis_be_policyholder-1.7.0/policyholder/migrations/0016_policyholder_roles_for_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/migrations/0017_auto_20230126_0903.py` & `openimis_be_policyholder-1.7.0/policyholder/migrations/0017_auto_20230126_0903.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/models.py` & `openimis_be_policyholder-1.7.0/policyholder/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import uuid
 
 from contribution_plan.models import ContributionPlanBundle
 from django.conf import settings
 from django.db import models
 from core import models as core_models, fields
 from graphql import ResolveInfo
-from location.models import Location, UserDistrict
+from location.models import Location, LocationManager
 from insuree.models import Insuree
 from policy.models import Policy
 
 
 class PolicyHolderManager(core_models.HistoryModelManager):
     def filter(self, *args, **kwargs):
         keys = [x for x in kwargs if "itemsvc" in x]
@@ -40,18 +40,15 @@
     def get_queryset(cls, queryset, user):
         queryset = cls.filter_queryset(queryset)
         if isinstance(user, ResolveInfo):
             user = user.context.user
         if settings.ROW_SECURITY and user.is_anonymous:
             return queryset.filter(id=None)
         if settings.ROW_SECURITY:
-            dist = UserDistrict.get_user_districts(user._u)
-            return queryset.filter(
-                locations__parent__parent_id__in=[l.location_id for l in dist]
-            )
+            return LocationManager().build_user_location_filter_query(user._u, queryset=queryset, prefix='locations')
         return queryset
 
     class Meta:
         db_table = 'tblPolicyHolder'
 
 
 class PolicyHolderInsureeManager(core_models.HistoryModelManager):
```

### Comparing `openimis-be-policyholder-1.6.0/policyholder/schema.py` & `openimis_be_policyholder-1.7.0/policyholder/schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/services.py` & `openimis_be_policyholder-1.7.0/policyholder/services.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/signals.py` & `openimis_be_policyholder-1.7.0/policyholder/signals.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/tests/helpers.py` & `openimis_be_policyholder-1.7.0/policyholder/tests/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,25 +7,14 @@
 from policyholder.models import PolicyHolder, PolicyHolderInsuree, PolicyHolderUser
 
 from product.test_helpers import create_test_product
 
 PH_DATA = {
     'code': 'PHCode',
     'trade_name': 'CompanyTest',
-    'address': {"region": "APAC", "street": "test"},
-    'phone': '111000111',
-    'fax': 'Fax',
-    'email': 'policy_holder@mail.com',
-    'contact_name': {"name": "test", "surname": "test-test"},
-    'legal_form': 1,
-    'activity_code': 2,
-    'accountancy_account': '128903719082739810273',
-    'bank_account': {"IBAN": "PL00 0000 2345 0000 1000 2345 2345"},
-    'payment_reference': 'PolicyHolderPaymentReference',
-    'json_ext': {},
 }
 
 
 def create_test_policy_holder(locations=None, custom_props={}):
     user = __get_or_create_simple_policy_holder_user()
 
     object_data = {
@@ -48,18 +37,18 @@
                                       last_policy=None, custom_props={}):
     if not policy_holder:
         policy_holder = create_test_policy_holder()
     if not insuree:
         insuree = create_test_insuree()
     if not contribution_plan_bundle:
         contribution_plan_bundle = create_test_contribution_plan_bundle()
-    if not last_policy:
-        last_policy = create_test_policy(
-            product=create_test_product("TestCode", custom_props={"insurance_period": 12, }),
-            insuree=insuree)
+    #if not last_policy:
+    #    last_policy = create_test_policy(
+    #        product=create_test_product("TestCode", custom_props={"insurance_period": 12, }),
+    #        insuree=insuree)
 
     user = __get_or_create_simple_policy_holder_user()
 
     object_data = {
         'policy_holder': policy_holder,
         'insuree': insuree,
         'contribution_plan_bundle': contribution_plan_bundle,
```

### Comparing `openimis-be-policyholder-1.6.0/policyholder/tests/helpers_tests.py` & `openimis_be_policyholder-1.7.0/policyholder/tests/helpers_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/policyholder/tests/services/services_ph_tests.py` & `openimis_be_policyholder-1.7.0/policyholder/tests/services/services_ph_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.test import TestCase
 
 from policyholder.services import PolicyHolder as PolicyHolderService, \
     PolicyHolderInsuree as PolicyHolderInsureeService, \
     PolicyHolderContributionPlan as PolicyHolderContributionPlanService
 from policyholder.models import PolicyHolder, PolicyHolderInsuree, PolicyHolderContributionPlan
-from policyholder.tests.helpers import create_test_policy_holder, create_test_policy_holder_insuree
+from policyholder.tests.helpers import create_test_policy_holder, create_test_policy_holder_insuree, PH_DATA as POLICY_HOLDER_MINI
 
 from contribution_plan.tests.helpers_tests import create_test_contribution_plan_bundle
 from insuree.test_helpers import create_test_insuree
 from core.models import User
 
 from policyholder.validation import PolicyHolderValidation
 
@@ -28,83 +28,88 @@
         'bank_account': {"IBAN": "PL00 0000 2345 0000 1000 2345 2345"},
         'payment_reference': 'PolicyHolderPaymentReference',
     }
 
     @classmethod
     def setUpClass(cls):
         super(ServiceTestPolicyHolder, cls).setUpClass()
-        PolicyHolder.objects.filter(code=cls.POLICY_HOLDER['code']).delete()
         if not User.objects.filter(username='admin').exists():
             User.objects.create_superuser(username='admin', password='S\/pe®Pąßw0rd™')
         cls.user = User.objects.filter(username='admin').first()
         cls.policy_holder_service = PolicyHolderService(cls.user)
         cls.policy_holder_insuree_service = PolicyHolderInsureeService(cls.user)
         cls.policy_holder_contribution_plan_service = PolicyHolderContributionPlanService(cls.user)
 
-        cls.test_policy_holder = create_test_policy_holder()
-        cls.test_policy_holder_insuree = create_test_policy_holder_insuree()
-
-        cls.test_insuree = cls.test_policy_holder_insuree.insuree
+        cls.test_policy_holder = create_test_policy_holder(custom_props=cls.POLICY_HOLDER)
+        cls.test_policy_holder_mini = create_test_policy_holder()
+        cls.test_insuree = create_test_insuree()
+        cls.test_policy_holder_insuree = create_test_policy_holder_insuree(policy_holder=cls.test_policy_holder, insuree=cls.test_insuree)
+        cls.test_policy_holder_insuree = create_test_policy_holder_insuree(policy_holder=cls.test_policy_holder_mini, insuree=cls.test_insuree)
+        
+        
         cls.test_insuree_to_change = create_test_insuree()
         cls.test_contribution_plan_bundle = cls.test_policy_holder_insuree.contribution_plan_bundle
         cls.test_last_policy = cls.test_policy_holder_insuree.last_policy
         cls.test_contribution_plan_bundle_to_replace = create_test_contribution_plan_bundle()
 
     def test_policy_holder_create(self):
+        self.POLICY_HOLDER['code']='test_policy_holder_create'
+
         response = self.policy_holder_service.create(self.POLICY_HOLDER)
 
         # tear down the test data
-        PolicyHolder.objects.filter(id=response["data"]["id"]).delete()
 
         self.assertEqual(
             (
                 True,
                 "Ok",
                 "",
-                "TT_Code",
-                "COTO",
+                self.POLICY_HOLDER['code'],
+                self.POLICY_HOLDER['trade_name'],
                 1,
-                {"IBAN": "PL00 0000 2345 0000 1000 2345 2345"},
-                "128903719082739810273",
+                self.POLICY_HOLDER['bank_account'],
+                self.POLICY_HOLDER['accountancy_account'],
             ),
             (
                 response['success'],
                 response['message'],
                 response['detail'],
                 response['data']['code'],
                 response['data']['trade_name'],
                 response['data']['version'],
                 response['data']['bank_account'],
                 response['data']['accountancy_account'],
             )
         )
 
     def test_duplicate_policy_holder_exception(self):
+
+        self.POLICY_HOLDER['code']='qwerqwre'
         first = self.policy_holder_service.create(self.POLICY_HOLDER)
         second = self.policy_holder_service.create(self.POLICY_HOLDER)
-        PolicyHolder.objects.filter(id=first["data"]["id"]).delete()
 
         expected_error_message = PolicyHolderValidation.UNIQUE_DISPLAY_NAME_VALIDATION_ERROR \
             .format(self.POLICY_HOLDER['code'], self.POLICY_HOLDER['trade_name'])
 
         self.assertFalse(second['success'])
         self.assertTrue(expected_error_message in second['detail'])
 
     def test_policy_holder_create_update(self):
+        self.POLICY_HOLDER['code']='ddsdfsdffff'
         response = self.policy_holder_service.create(self.POLICY_HOLDER)
         policy_holder_object = PolicyHolder.objects.get(id=response['data']['id'])
         version = policy_holder_object.version
         policy_holder = {
             'id': str(policy_holder_object.id),
             'address': {"region": "TEST", "street": "TEST"},
         }
         response = self.policy_holder_service.update(policy_holder)
 
         # tear down the test data
-        PolicyHolder.objects.filter(id=response["data"]["id"]).delete()
+        PolicyHolder.objects.filter(code=self.POLICY_HOLDER['code']).delete()
 
         self.assertEqual(
             (
                 True,
                 "Ok",
                 "",
                 {"region": "TEST", "street": "TEST"},
@@ -116,14 +121,15 @@
                 response['detail'],
                 response['data']['address'],
                 response['data']['version'],
             )
         )
 
     def test_policy_holder_update_without_changing_field(self):
+        self.POLICY_HOLDER['code']='ddsseedfth'
         ph = self.policy_holder_service.create(self.POLICY_HOLDER)
         policy_holder_object = PolicyHolder.objects.filter(id=ph['data']['id']).first()
         policy_holder = {
             'id': str(policy_holder_object.id),
             'address': policy_holder_object.address,
         }
         response = self.policy_holder_service.update(policy_holder)
@@ -138,27 +144,27 @@
                 response['success'],
                 response['message'],
                 response['detail']
             )
         )
 
     def test_update_policy_holder_with_duplicated_display(self):
+        self.POLICY_HOLDER['code']='ddfdsffewdfd'
+
         first = self.policy_holder_service.create(self.POLICY_HOLDER)
 
         second = self.policy_holder_service.create({
             **self.POLICY_HOLDER,
-            'trade_name': 'COTO2'
+            'trade_name': 'COTO2',
         })
 
         policy_holder = {'id': str(first['data']['id']), 'trade_name': second['data']['trade_name']}
 
         response = self.policy_holder_service.update(policy_holder)
 
-        PolicyHolder.objects.filter(id=first["data"]["id"]).delete()
-        PolicyHolder.objects.filter(id=second["data"]["id"]).delete()
 
         expected_error_message = PolicyHolderValidation.UNIQUE_DISPLAY_NAME_VALIDATION_ERROR \
             .format(self.POLICY_HOLDER['code'], second['data']['trade_name'])
 
         self.assertFalse(response['success'])
         self.assertTrue(expected_error_message in response['detail'])
 
@@ -175,24 +181,24 @@
             (
                 response['success'],
                 response['message'],
             )
         )
 
     def test_policy_holder_create_delete(self):
+        self.POLICY_HOLDER['code']='qqeeyyaaf'
         response = self.policy_holder_service.create(self.POLICY_HOLDER)
-        policy_holder_object = PolicyHolder.objects.get(id=response['data']['id'])
+        policy_holder_object = PolicyHolder.objects.filter(id=response['data']['id']).first()
+
         version = policy_holder_object.version
         policy_holder = {
             'id': str(policy_holder_object.id),
         }
         response = self.policy_holder_service.delete(policy_holder)
 
-        # tear down the test data
-        PolicyHolder.objects.filter(id=str(policy_holder_object.id)).delete()
 
         self.assertEqual(
             (
                 True,
                 "Ok",
                 "",
             ),
```

### Comparing `openimis-be-policyholder-1.6.0/policyholder/validation/policyholder_validation.py` & `openimis_be_policyholder-1.7.0/policyholder/validation/policyholder_validation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.6.0/setup.py` & `openimis_be_policyholder-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-policyholder',
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend PolicyHolder reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

