# Comparing `tmp/openimis-be-contribution-plan-1.6.0.tar.gz` & `tmp/openimis_be_contribution_plan-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-contribution-plan-1.6.0.tar", last modified: Sat Dec 16 00:57:45 2023, max compression
+gzip compressed data, was "openimis_be_contribution_plan-1.7.0.tar", last modified: Tue Apr 30 09:06:17 2024, max compression
```

## Comparing `openimis-be-contribution-plan-1.6.0.tar` & `openimis_be_contribution_plan-1.7.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:45.866038 openimis-be-contribution-plan-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2023-12-16 00:57:45.866038 openimis-be-contribution-plan-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:45.858038 openimis-be-contribution-plan-1.6.0/contribution_plan/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:45.862038 openimis-be-contribution-plan-1.6.0/contribution_plan/gql/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/gql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:45.862038 openimis-be-contribution-plan-1.6.0/contribution_plan/gql/gql_mutations/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/gql/gql_mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/gql/gql_mutations/contribution_plan_bundle_details_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/gql/gql_mutations/contribution_plan_bundle_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/gql/gql_mutations/contribution_plan_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/gql/gql_mutations/input_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/gql/gql_mutations/payment_plan_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/gql/gql_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/gql/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:45.862038 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    14098 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)    23110 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0001_squashed_0010_payment_plan_roles_for_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0002_auto_20201204_1353.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0002_auto_20230126_0903.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0003_auto_20201204_1439.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0004_auto_20201217_0946.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0005_contributionplanbundlemutation_contributionplanmutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0006_auto_20210118_1349.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0007_auto_20210217_1302.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0008_historicalpaymentplan_paymentplan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0009_contributionplan_roles_for_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0010_payment_plan_roles_for_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0011_auto_20230126_0903.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0012_benefit_plan_generic_fk.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10311 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:45.862038 openimis-be-contribution-plan-1.6.0/contribution_plan/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:45.866038 openimis-be-contribution-plan-1.6.0/contribution_plan/tests/gql_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/tests/gql_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11827 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/tests/gql_tests/mutations_cp_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    10317 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/tests/gql_tests/mutations_cpb_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/tests/gql_tests/mutations_cpbd_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/tests/gql_tests/mutations_pp_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/tests/gql_tests/query_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/tests/helpers_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:45.866038 openimis-be-contribution-plan-1.6.0/contribution_plan/tests/services/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25215 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/tests/services/services_cp_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:33.000000 openimis-be-contribution-plan-1.6.0/contribution_plan/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:45.866038 openimis-be-contribution-plan-1.6.0/openimis_be_contribution_plan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2023-12-16 00:57:45.000000 openimis-be-contribution-plan-1.6.0/openimis_be_contribution_plan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2023-12-16 00:57:45.000000 openimis-be-contribution-plan-1.6.0/openimis_be_contribution_plan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:57:45.000000 openimis-be-contribution-plan-1.6.0/openimis_be_contribution_plan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-16 00:57:45.000000 openimis-be-contribution-plan-1.6.0/openimis_be_contribution_plan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-16 00:57:45.000000 openimis-be-contribution-plan-1.6.0/openimis_be_contribution_plan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:57:45.866038 openimis-be-contribution-plan-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-12-16 00:57:45.000000 openimis-be-contribution-plan-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:17.975193 openimis_be_contribution_plan-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-30 09:06:17.975193 openimis_be_contribution_plan-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:17.967193 openimis_be_contribution_plan-1.7.0/contribution_plan/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:17.967193 openimis_be_contribution_plan-1.7.0/contribution_plan/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/gql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:17.967193 openimis_be_contribution_plan-1.7.0/contribution_plan/gql/gql_mutations/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/gql/gql_mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/gql/gql_mutations/contribution_plan_bundle_details_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/gql/gql_mutations/contribution_plan_bundle_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/gql/gql_mutations/contribution_plan_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/gql/gql_mutations/input_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/gql/gql_mutations/payment_plan_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/gql/gql_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/gql/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:17.971193 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23110 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0001_squashed_0010_payment_plan_roles_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0002_auto_20201204_1353.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0002_auto_20230126_0903.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0003_auto_20201204_1439.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0004_auto_20201217_0946.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0005_contributionplanbundlemutation_contributionplanmutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0006_auto_20210118_1349.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0007_auto_20210217_1302.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0008_historicalpaymentplan_paymentplan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0009_contributionplan_roles_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0010_payment_plan_roles_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0011_auto_20230126_0903.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0012_benefit_plan_generic_fk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0013_alter_contributionplan_date_created_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15223 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:17.971193 openimis_be_contribution_plan-1.7.0/contribution_plan/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:17.971193 openimis_be_contribution_plan-1.7.0/contribution_plan/tests/gql_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/tests/gql_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/tests/gql_tests/mutations_cp_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/tests/gql_tests/mutations_cpb_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/tests/gql_tests/mutations_cpbd_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/tests/gql_tests/mutations_pp_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/tests/gql_tests/query_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/tests/helpers_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:17.971193 openimis_be_contribution_plan-1.7.0/contribution_plan/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25230 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/tests/services/services_cp_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:09.000000 openimis_be_contribution_plan-1.7.0/contribution_plan/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:17.971193 openimis_be_contribution_plan-1.7.0/openimis_be_contribution_plan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-30 09:06:17.000000 openimis_be_contribution_plan-1.7.0/openimis_be_contribution_plan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-30 09:06:17.000000 openimis_be_contribution_plan-1.7.0/openimis_be_contribution_plan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:06:17.000000 openimis_be_contribution_plan-1.7.0/openimis_be_contribution_plan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-30 09:06:17.000000 openimis_be_contribution_plan-1.7.0/openimis_be_contribution_plan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 09:06:17.000000 openimis_be_contribution_plan-1.7.0/openimis_be_contribution_plan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:06:17.975193 openimis_be_contribution_plan-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-30 09:06:17.000000 openimis_be_contribution_plan-1.7.0/setup.py
```

### Comparing `openimis-be-contribution-plan-1.6.0/LICENSE.md` & `openimis_be_contribution_plan-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/PKG-INFO` & `openimis_be_contribution_plan-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-contribution-plan
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Contribution Plan reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-contribution-plan-1.6.0/README.md` & `openimis_be_contribution_plan-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/apps.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/gql/gql_mutations/contribution_plan_bundle_details_mutations.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/gql/gql_mutations/contribution_plan_bundle_details_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/gql/gql_mutations/contribution_plan_bundle_mutations.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/gql/gql_mutations/contribution_plan_bundle_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/gql/gql_mutations/contribution_plan_mutations.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/gql/gql_mutations/contribution_plan_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/gql/gql_mutations/input_types.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/gql/gql_mutations/input_types.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/gql/gql_mutations/payment_plan_mutations.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/gql/gql_mutations/payment_plan_mutations.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,17 @@
 
     @classmethod
     def _validate_mutation(cls, user, **data):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
                 ContributionPlanConfig.gql_mutation_update_paymentplan_perms):
             raise ValidationError(_("mutation.authentication_required"))
 
-        if PaymentPlanService.check_unique_code(data['code']):
+        if PaymentPlanService.check_unique_code(data['code'], data['id']):
             raise ValidationError(_("mutation.payment_plan_code_duplicated"))
 
-
     @classmethod
     def _mutate(cls, user, **data):
         if "date_valid_to" not in data:
             data['date_valid_to'] = None
         if "client_mutation_id" in data:
             data.pop('client_mutation_id')
         if "client_mutation_label" in data:
```

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/gql/gql_types.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/gql/gql_types.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/gql/util.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/gql/util.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0001_initial.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0001_squashed_0010_payment_plan_roles_for_admin.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0001_squashed_0010_payment_plan_roles_for_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0002_auto_20201204_1353.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0002_auto_20201204_1353.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0002_auto_20230126_0903.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0002_auto_20230126_0903.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0003_auto_20201204_1439.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0003_auto_20201204_1439.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0004_auto_20201217_0946.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0004_auto_20201217_0946.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0005_contributionplanbundlemutation_contributionplanmutation.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0005_contributionplanbundlemutation_contributionplanmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0006_auto_20210118_1349.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0006_auto_20210118_1349.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0007_auto_20210217_1302.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0007_auto_20210217_1302.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0008_historicalpaymentplan_paymentplan.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0008_historicalpaymentplan_paymentplan.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0009_contributionplan_roles_for_admin.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0009_contributionplan_roles_for_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0010_payment_plan_roles_for_admin.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0010_payment_plan_roles_for_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0011_auto_20230126_0903.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0011_auto_20230126_0903.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/migrations/0012_benefit_plan_generic_fk.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/migrations/0012_benefit_plan_generic_fk.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/mixins.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/mixins.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/models.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     objects = GenericPlanManager()
 
     class Meta:
         abstract = True
 
 
 _get_contribution_length_signal_params = ["grace_period"]
-get_contribution_length_signal = Signal(providing_args=_get_contribution_length_signal_params)
+get_contribution_length_signal = Signal(_get_contribution_length_signal_params)
 
 
 class ContributionPlanBundleManager(models.Manager):
     def filter(self, *args, **kwargs):
         keys = [x for x in kwargs if "itemsvc" in x]
         for key in keys:
             new_key = key.replace("itemsvc", self.model.model_prefix)
```

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/schema.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/services.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,16 +306,19 @@
             "message": "Ok",
             "detail": "",
             "old_object": json.loads(json.dumps(dict_representation, cls=DjangoJSONEncoder)),
             "uuid_new_object": str(pp_to_replace.replacement_uuid),
         }
 
     @staticmethod
-    def check_unique_code(code):
-        if PaymentPlanModel.objects.filter(code=code, is_deleted=False).exists():
+    def check_unique_code(code, uuid=None):
+        qs = PaymentPlanModel.objects.filter(code=code, is_deleted=False)
+        if uuid:
+            qs = qs.exclude(id=uuid)
+        if qs:
             return [{"message": "Payment plan code %s already exists" % code}]
         return []
 
 
 def _output_exception(model_name, method, exception):
     return {
         "success": False,
```

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/tests/gql_tests/mutations_cp_tests.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/tests/gql_tests/mutations_cp_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/tests/gql_tests/mutations_cpb_tests.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/tests/gql_tests/mutations_cpb_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/tests/gql_tests/mutations_cpbd_tests.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/tests/gql_tests/mutations_cpbd_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/tests/gql_tests/mutations_pp_tests.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/tests/gql_tests/mutations_pp_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/tests/gql_tests/query_tests.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/tests/gql_tests/query_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/tests/helpers.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/tests/helpers_tests.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/tests/helpers_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/tests/services/services_cp_tests.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/tests/services/services_cp_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                 True,
                 "Ok",
                 "",
                 "CP SERVICE",
                 "Contribution Plan Name Service",
                 1,
                 6,
-                self.test_product.id,
+                str(self.test_product.id),
                 str(self.calculation),
             ),
             (
                 response['success'],
                 response['message'],
                 response['detail'],
                 response['data']['code'],
@@ -163,15 +163,15 @@
         self.assertEqual(
             (
                 True,
                 "Ok",
                 "",
                 3,
                 2,
-                self.test_product2.id,
+                str(self.test_product2.id),
             ),
             (
                 response['success'],
                 response['message'],
                 response['detail'],
                 response['data']['periodicity'],
                 response['data']['version'],
@@ -644,15 +644,15 @@
                 True,
                 "Ok",
                 "",
                 "PP SERVICE",
                 "Payment Plan Name Service",
                 1,
                 6,
-                self.test_product.id,
+                str(self.test_product.id),
                 str(self.calculation),
             ),
             (
                 response['success'],
                 response['message'],
                 response['detail'],
                 response['data']['code'],
```

### Comparing `openimis-be-contribution-plan-1.6.0/contribution_plan/utils.py` & `openimis_be_contribution_plan-1.7.0/contribution_plan/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.6.0/openimis_be_contribution_plan.egg-info/PKG-INFO` & `openimis_be_contribution_plan-1.7.0/openimis_be_contribution_plan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-contribution-plan
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Contribution Plan reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-contribution-plan-1.6.0/openimis_be_contribution_plan.egg-info/SOURCES.txt` & `openimis_be_contribution_plan-1.7.0/openimis_be_contribution_plan.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 contribution_plan/migrations/0006_auto_20210118_1349.py
 contribution_plan/migrations/0007_auto_20210217_1302.py
 contribution_plan/migrations/0008_historicalpaymentplan_paymentplan.py
 contribution_plan/migrations/0009_contributionplan_roles_for_admin.py
 contribution_plan/migrations/0010_payment_plan_roles_for_admin.py
 contribution_plan/migrations/0011_auto_20230126_0903.py
 contribution_plan/migrations/0012_benefit_plan_generic_fk.py
+contribution_plan/migrations/0013_alter_contributionplan_date_created_and_more.py
 contribution_plan/migrations/__init__.py
 contribution_plan/tests/__init__.py
 contribution_plan/tests/helpers.py
 contribution_plan/tests/helpers_tests.py
 contribution_plan/tests/gql_tests/__init__.py
 contribution_plan/tests/gql_tests/mutations_cp_tests.py
 contribution_plan/tests/gql_tests/mutations_cpb_tests.py
```

### Comparing `openimis-be-contribution-plan-1.6.0/setup.py` & `openimis_be_contribution_plan-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-contribution-plan',
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Contribution Plan reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

