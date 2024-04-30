# Comparing `tmp/openimis-be-payroll-1.0.0.tar.gz` & `tmp/openimis_be_payroll-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-payroll-1.0.0.tar", last modified: Sat Dec 16 01:06:48 2023, max compression
+gzip compressed data, was "openimis_be_payroll-1.1.0.tar", last modified: Tue Apr 30 09:08:01 2024, max compression
```

## Comparing `openimis-be-payroll-1.0.0.tar` & `openimis_be_payroll-1.1.0.tar`

### file list

```diff
@@ -1,53 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:06:48.469308 openimis-be-payroll-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-16 01:06:48.469308 openimis-be-payroll-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:06:48.469308 openimis-be-payroll-1.0.0/openimis_be_payroll.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-16 01:06:48.000000 openimis-be-payroll-1.0.0/openimis_be_payroll.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2023-12-16 01:06:48.000000 openimis-be-payroll-1.0.0/openimis_be_payroll.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 01:06:48.000000 openimis-be-payroll-1.0.0/openimis_be_payroll.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-12-16 01:06:48.000000 openimis-be-payroll-1.0.0/openimis_be_payroll.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-16 01:06:48.000000 openimis-be-payroll-1.0.0/openimis_be_payroll.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:06:48.465308 openimis-be-payroll-1.0.0/payroll/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:06:48.469308 openimis-be-payroll-1.0.0/payroll/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/migrations/0002_add_pp_rights_to_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/migrations/0003_historicalpayroll_historicalpayrollbill_payroll_payrollbill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/migrations/0004_add_payroll_rights_to_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/migrations/0005_change_i_user_to_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/migrations/0006_auto_20230809_1057.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/migrations/0007_auto_20230811_0734.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/migrations/0008_historicalpaymentadaptorhistory_paymentadaptorhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/migrations/0009_auto_20231006_0755.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:06:48.469308 openimis-be-payroll-1.0.0/payroll/payments_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/payments_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/payments_registry/registry_point.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/payments_registry/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:06:48.469308 openimis-be-payroll-1.0.0/payroll/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/strategies/strategy_mobile_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/strategies/strategy_of_payments_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/strategies/strategy_on_site_payments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/strategies/strategy_online_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/strategies/strategy_payment_bank_transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:06:48.469308 openimis-be-payroll-1.0.0/payroll/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/tests/payment_point_gql_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    11864 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/tests/payroll_gql_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2023-12-16 01:06:40.000000 openimis-be-payroll-1.0.0/payroll/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 01:06:48.469308 openimis-be-payroll-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-12-16 01:06:48.000000 openimis-be-payroll-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:08:01.657835 openimis_be_payroll-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-30 09:08:01.657835 openimis_be_payroll-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:08:01.657835 openimis_be_payroll-1.1.0/openimis_be_payroll.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-30 09:08:01.000000 openimis_be_payroll-1.1.0/openimis_be_payroll.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-30 09:08:01.000000 openimis_be_payroll-1.1.0/openimis_be_payroll.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:08:01.000000 openimis_be_payroll-1.1.0/openimis_be_payroll.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-30 09:08:01.000000 openimis_be_payroll-1.1.0/openimis_be_payroll.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 09:08:01.000000 openimis_be_payroll-1.1.0/openimis_be_payroll.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:08:01.649834 openimis_be_payroll-1.1.0/payroll/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:08:01.653834 openimis_be_payroll-1.1.0/payroll/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0002_add_pp_rights_to_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0003_historicalpayroll_historicalpayrollbill_payroll_payrollbill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0004_add_payroll_rights_to_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0005_change_i_user_to_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0006_auto_20230809_1057.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0007_auto_20230811_0734.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0008_historicalpaymentadaptorhistory_paymentadaptorhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0009_auto_20231006_0755.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0010_alter_paymentpoint_ppm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0010_auto_20240131_1015.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0011_auto_20240202_1140.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0012_auto_20240202_1619.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0013_merge_20240207_1633.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0013_payrollmutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13615 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0014_alter_benefitattachment_date_created_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0015_merge_20240207_1703.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0016_add_csv_rec_upload_rigth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0017_csvreconciliationupload_historicalcsvreconciliationupload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0018_auto_20240212_1355.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0019_auto_20240221_2330.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/0020_auto_20240227_0912.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:08:01.653834 openimis_be_payroll-1.1.0/payroll/payments_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/payments_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/payments_registry/registry_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/payments_registry/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13089 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17295 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:08:01.657835 openimis_be_payroll-1.1.0/payroll/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/strategies/strategy_mobile_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/strategies/strategy_of_payments_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/strategies/strategy_offline_payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/strategies/strategy_online_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/strategies/strategy_payment_bank_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:08:01.657835 openimis_be_payroll-1.1.0/payroll/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/tests/benefit_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/tests/benefit_consumption_gql_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/tests/payment_point_gql_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12831 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/tests/payroll_gql_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-30 09:07:53.000000 openimis_be_payroll-1.1.0/payroll/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:08:01.657835 openimis_be_payroll-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-30 09:08:01.000000 openimis_be_payroll-1.1.0/setup.py
```

### Comparing `openimis-be-payroll-1.0.0/LICENSE.md` & `openimis_be_payroll-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-payroll-1.0.0/PKG-INFO` & `openimis_be_payroll-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-payroll
-Version: 1.0.0
+Version: 1.1.0
 Summary: The openIMIS Backend payroll reference module.
 Home-page: https://openimis.org/
 Author: Kamil Malinowski
 Author-email: kmalinowski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -19,9 +19,10 @@
 Requires-Dist: django
 Requires-Dist: graphene-django
 Requires-Dist: django-db-signals
 Requires-Dist: djangorestframework
 Requires-Dist: openimis-be-core
 Requires-Dist: openimis-be-location
 Requires-Dist: openimis-be-invoice
+Requires-Dist: openimis-be-payment_cycle
 
 # openIMIS Backend payroll reference module
```

### Comparing `openimis-be-payroll-1.0.0/openimis_be_payroll.egg-info/PKG-INFO` & `openimis_be_payroll-1.1.0/openimis_be_payroll.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-payroll
-Version: 1.0.0
+Version: 1.1.0
 Summary: The openIMIS Backend payroll reference module.
 Home-page: https://openimis.org/
 Author: Kamil Malinowski
 Author-email: kmalinowski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -19,9 +19,10 @@
 Requires-Dist: django
 Requires-Dist: graphene-django
 Requires-Dist: django-db-signals
 Requires-Dist: djangorestframework
 Requires-Dist: openimis-be-core
 Requires-Dist: openimis-be-location
 Requires-Dist: openimis-be-invoice
+Requires-Dist: openimis-be-payment_cycle
 
 # openIMIS Backend payroll reference module
```

### Comparing `openimis-be-payroll-1.0.0/openimis_be_payroll.egg-info/SOURCES.txt` & `openimis_be_payroll-1.1.0/openimis_be_payroll.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 openimis_be_payroll.egg-info/SOURCES.txt
 openimis_be_payroll.egg-info/dependency_links.txt
 openimis_be_payroll.egg-info/requires.txt
 openimis_be_payroll.egg-info/top_level.txt
 payroll/__init__.py
 payroll/admin.py
 payroll/apps.py
+payroll/documents.py
 payroll/gql_mutations.py
 payroll/gql_queries.py
 payroll/models.py
 payroll/schema.py
 payroll/services.py
 payroll/signals.py
 payroll/urls.py
@@ -23,22 +24,37 @@
 payroll/migrations/0003_historicalpayroll_historicalpayrollbill_payroll_payrollbill.py
 payroll/migrations/0004_add_payroll_rights_to_admin.py
 payroll/migrations/0005_change_i_user_to_user.py
 payroll/migrations/0006_auto_20230809_1057.py
 payroll/migrations/0007_auto_20230811_0734.py
 payroll/migrations/0008_historicalpaymentadaptorhistory_paymentadaptorhistory.py
 payroll/migrations/0009_auto_20231006_0755.py
+payroll/migrations/0010_alter_paymentpoint_ppm.py
+payroll/migrations/0010_auto_20240131_1015.py
+payroll/migrations/0011_auto_20240202_1140.py
+payroll/migrations/0012_auto_20240202_1619.py
+payroll/migrations/0013_merge_20240207_1633.py
+payroll/migrations/0013_payrollmutation.py
+payroll/migrations/0014_alter_benefitattachment_date_created_and_more.py
+payroll/migrations/0015_merge_20240207_1703.py
+payroll/migrations/0016_add_csv_rec_upload_rigth.py
+payroll/migrations/0017_csvreconciliationupload_historicalcsvreconciliationupload.py
+payroll/migrations/0018_auto_20240212_1355.py
+payroll/migrations/0019_auto_20240221_2330.py
+payroll/migrations/0020_auto_20240227_0912.py
 payroll/migrations/__init__.py
 payroll/payments_registry/__init__.py
 payroll/payments_registry/registry_point.py
 payroll/payments_registry/storage.py
 payroll/strategies/__init__.py
 payroll/strategies/strategy_mobile_payment.py
 payroll/strategies/strategy_of_payments_interface.py
-payroll/strategies/strategy_on_site_payments.py
+payroll/strategies/strategy_offline_payments.py
 payroll/strategies/strategy_online_payment.py
 payroll/strategies/strategy_payment_bank_transfer.py
 payroll/tests/__init__.py
+payroll/tests/benefit_consumption.py
+payroll/tests/benefit_consumption_gql_tests.py
 payroll/tests/data.py
 payroll/tests/helpers.py
 payroll/tests/payment_point_gql_tests.py
 payroll/tests/payroll_gql_tests.py
```

### Comparing `openimis-be-payroll-1.0.0/payroll/gql_mutations.py` & `openimis_be_payroll-1.1.0/payroll/gql_mutations.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from django.core.exceptions import ValidationError
 from django.db import transaction
 
 from core.gql.gql_mutations.base_mutation import BaseHistoryModelCreateMutationMixin, BaseMutation, \
     BaseHistoryModelUpdateMutationMixin, BaseHistoryModelDeleteMutationMixin
 from core.schema import OpenIMISMutation
 from payroll.apps import PayrollConfig
-from payroll.models import PaymentPoint, Payroll, PayrollStatus
+from payroll.models import PaymentPoint, Payroll, PayrollStatus, PayrollMutation
 from payroll.services import PaymentPointService, PayrollService
 
 
 class CreatePaymentPointInputType(OpenIMISMutation.Input):
     name = graphene.String(required=True, max_length=255)
     location_id = graphene.Int(required=True)
     ppm_id = graphene.UUID(required=True)
@@ -24,35 +24,40 @@
 
 class DeletePaymentPointInputType(OpenIMISMutation.Input):
     ids = graphene.List(graphene.UUID, required=True)
 
 
 class CreatePayrollInput(OpenIMISMutation.Input):
     class PayrollStatusEnum(graphene.Enum):
-        CREATED = PayrollStatus.CREATED
-        ONGOING = PayrollStatus.ONGOING
-        AWAITING_FOR_RECONCILIATION = PayrollStatus.AWAITING_FOR_RECONCILIATION
-        RECONCILIATED = PayrollStatus.RECONCILIATED
+        PENDING_APPROVAL = PayrollStatus.PENDING_APPROVAL
+        APPROVE_FOR_PAYMENT = PayrollStatus.APPROVE_FOR_PAYMENT
+        REJECTED = PayrollStatus.REJECTED
+        RECONCILED = PayrollStatus.RECONCILED
 
     name = graphene.String(required=True, max_length=255)
-    benefit_plan_id = graphene.UUID(required=True)
+    payment_plan_id = graphene.UUID(required=True)
     payment_point_id = graphene.UUID(required=False)
+    payment_cycle_id = graphene.UUID(required=False)
     status = graphene.Field(PayrollStatusEnum, required=True)
     payment_method = graphene.String(required=True, max_length=255)
-    included_unpaid = graphene.Boolean(required=True)
+    from_failed_invoices_payroll_id = graphene.UUID(required=False)
 
     date_valid_from = graphene.Date(required=False)
     date_valid_to = graphene.Date(required=False)
     json_ext = graphene.JSONString(required=False)
 
 
 class DeletePayrollInputType(DeletePaymentPointInputType):
     pass
 
 
+class ClosePayrollInputType(DeletePaymentPointInputType):
+    pass
+
+
 class CreatePaymentPointMutation(BaseHistoryModelCreateMutationMixin, BaseMutation):
     _mutation_class = "CreatePaymentPointMutation"
     _mutation_module = PayrollConfig.name
     _model = PaymentPoint
 
     @classmethod
     def _validate_mutation(cls, user, **data):
@@ -132,21 +137,26 @@
     def _validate_mutation(cls, user, **data):
         if type(user) is AnonymousUser or not user.has_perms(
                 PayrollConfig.gql_payroll_create_perms):
             raise ValidationError("mutation.authentication_required")
 
     @classmethod
     def _mutate(cls, user, **data):
-        if "client_mutation_id" in data:
-            data.pop('client_mutation_id')
+        client_mutation_id = data.pop('client_mutation_id', None)
         if "client_mutation_label" in data:
             data.pop('client_mutation_label')
 
         service = PayrollService(user)
         response = service.create(data)
+        if client_mutation_id and response['success']:
+            payroll_id = response['data']['id']
+            payroll = Payroll.objects.get(id=payroll_id)
+            PayrollMutation.object_mutated(
+                user, client_mutation_id=client_mutation_id, payroll=payroll
+            )
         if not response['success']:
             return response
         return None
 
     class Input(CreatePayrollInput):
         pass
 
@@ -174,7 +184,65 @@
         if ids:
             with transaction.atomic():
                 for id in ids:
                     service.delete({'id': id})
 
     class Input(DeletePayrollInputType):
         pass
+
+
+class ClosePayrollMutation(BaseHistoryModelDeleteMutationMixin, BaseMutation):
+    _mutation_class = "ClosePayrollMutation"
+    _mutation_module = "payroll"
+    _model = Payroll
+
+    @classmethod
+    def _validate_mutation(cls, user, **data):
+        if type(user) is AnonymousUser or not user.has_perms(
+                PayrollConfig.gql_payroll_delete_perms):
+            raise ValidationError("mutation.authentication_required")
+
+    @classmethod
+    def _mutate(cls, user, **data):
+        if "client_mutation_id" in data:
+            data.pop('client_mutation_id')
+        if "client_mutation_label" in data:
+            data.pop('client_mutation_label')
+
+        service = PayrollService(user)
+        ids = data.get('ids')
+        if ids:
+            with transaction.atomic():
+                for id in ids:
+                    service.close_payroll({'id': id})
+
+    class Input(DeletePayrollInputType):
+        pass
+
+
+class RejectPayrollMutation(BaseHistoryModelDeleteMutationMixin, BaseMutation):
+    _mutation_class = "RejectPayrollMutation"
+    _mutation_module = "payroll"
+    _model = Payroll
+
+    @classmethod
+    def _validate_mutation(cls, user, **data):
+        if type(user) is AnonymousUser or not user.has_perms(
+                PayrollConfig.gql_payroll_delete_perms):
+            raise ValidationError("mutation.authentication_required")
+
+    @classmethod
+    def _mutate(cls, user, **data):
+        if "client_mutation_id" in data:
+            data.pop('client_mutation_id')
+        if "client_mutation_label" in data:
+            data.pop('client_mutation_label')
+
+        service = PayrollService(user)
+        ids = data.get('ids')
+        if ids:
+            with transaction.atomic():
+                for id in ids:
+                    service.reject_approved_payroll({'id': id})
+
+    class Input(DeletePayrollInputType):
+        pass
```

### Comparing `openimis-be-payroll-1.0.0/payroll/migrations/0001_initial.py` & `openimis_be_payroll-1.1.0/payroll/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payroll-1.0.0/payroll/migrations/0002_add_pp_rights_to_admin.py` & `openimis_be_payroll-1.1.0/payroll/migrations/0002_add_pp_rights_to_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payroll-1.0.0/payroll/migrations/0003_historicalpayroll_historicalpayrollbill_payroll_payrollbill.py` & `openimis_be_payroll-1.1.0/payroll/migrations/0003_historicalpayroll_historicalpayrollbill_payroll_payrollbill.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payroll-1.0.0/payroll/migrations/0004_add_payroll_rights_to_admin.py` & `openimis_be_payroll-1.1.0/payroll/migrations/0004_add_payroll_rights_to_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payroll-1.0.0/payroll/migrations/0005_change_i_user_to_user.py` & `openimis_be_payroll-1.1.0/payroll/migrations/0005_change_i_user_to_user.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payroll-1.0.0/payroll/migrations/0006_auto_20230809_1057.py` & `openimis_be_payroll-1.1.0/payroll/migrations/0006_auto_20230809_1057.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payroll-1.0.0/payroll/migrations/0007_auto_20230811_0734.py` & `openimis_be_payroll-1.1.0/payroll/migrations/0007_auto_20230811_0734.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payroll-1.0.0/payroll/migrations/0008_historicalpaymentadaptorhistory_paymentadaptorhistory.py` & `openimis_be_payroll-1.1.0/payroll/migrations/0008_historicalpaymentadaptorhistory_paymentadaptorhistory.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payroll-1.0.0/payroll/migrations/0009_auto_20231006_0755.py` & `openimis_be_payroll-1.1.0/payroll/migrations/0009_auto_20231006_0755.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payroll-1.0.0/payroll/payments_registry/registry_point.py` & `openimis_be_payroll-1.1.0/payroll/payments_registry/registry_point.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payroll-1.0.0/payroll/payments_registry/storage.py` & `openimis_be_payroll-1.1.0/payroll/payments_registry/storage.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payroll-1.0.0/payroll/strategies/strategy_online_payment.py` & `openimis_be_payroll-1.1.0/payroll/strategies/strategy_online_payment.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payroll-1.0.0/payroll/tests/helpers.py` & `openimis_be_payroll-1.1.0/payroll/tests/helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,15 +28,17 @@
             user_id=None, data={**self._TEST_DATA_USER, **kwargs}, audit_user_id=999, connected=False)
         create_or_update_core_user(
             user_uuid=None, username={**self._TEST_DATA_USER, **kwargs}["username"], i_user=i_user)
         return DbManagerUtils.get_object_or_none(User, username={**self._TEST_DATA_USER, **kwargs}["username"])
 
 
 class PaymentPointHelper:
-    _TEST_DATA_PAYMENT_POINT = {
+    _TEST_DATA_PAYMENT_POINT = None
+    def __init__(self):
+        self._TEST_DATA_PAYMENT_POINT=        {
         "name": "TestPaymentPoint",
         "location": Location.objects.filter(validity_to__isnull=True, type='V').first()
     }
 
     def get_or_create_payment_point_api(self, **kwargs):
         payment_point = PaymentPoint.objects.filter(name={**self._TEST_DATA_PAYMENT_POINT, **kwargs}["name"]).first()
         if payment_point is None:
```

### Comparing `openimis-be-payroll-1.0.0/payroll/tests/payment_point_gql_tests.py` & `openimis_be_payroll-1.1.0/payroll/tests/payment_point_gql_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payroll-1.0.0/payroll/tests/payroll_gql_tests.py` & `openimis_be_payroll-1.1.0/payroll/tests/payroll_gql_tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import json
+import uuid
 from datetime import datetime, timedelta
+from core.models import MutationLog
 
-from graphene import Schema
+from graphene import JSONString, Schema
 from graphene.test import Client
 from django.test import TestCase
 from django.contrib.contenttypes.models import ContentType
 from django.db.models import Q
 
+from contribution_plan.models import PaymentPlan
 from individual.models import Individual
 from individual.tests.data import service_add_individual_payload
 from invoice.models import Bill
-from payroll.models import Payroll, PayrollBill
+from payment_cycle.models import PaymentCycle
+from payroll.models import Payroll, PayrollBill, PayrollStatus
 from payroll.tests.data import gql_payroll_create, gql_payroll_query, gql_payroll_delete, \
     gql_payroll_create_no_json_ext
 from payroll.tests.helpers import LogInHelper, PaymentPointHelper
 from payroll.schema import Query, Mutation
 from social_protection.models import BenefitPlan, Beneficiary
 from social_protection.tests.data import service_add_payload
 
@@ -40,75 +44,84 @@
             query=Query,
             mutation=Mutation
         )
         cls.gql_client = Client(gql_schema)
         cls.gql_context = cls.GQLContext(cls.user)
         cls.gql_context_unauthorized = cls.GQLContext(cls.user_unauthorized)
         cls.name = "TestCreatePayroll"
-        cls.status = "CREATED"
+        cls.status = PayrollStatus.CREATED
         cls.payment_method = "TestPaymentMethod"
         cls.date_valid_from, cls.date_valid_to = cls.__get_start_and_end_of_current_month()
         cls.payment_point = PaymentPointHelper().get_or_create_payment_point_api()
         cls.benefit_plan = cls.__create_benefit_plan()
         cls.individual = cls.__create_individual()
         cls.subject_type = ContentType.objects.get_for_model(Beneficiary)
+        cls.payment_plan = cls.__create_payment_plan(cls.benefit_plan)
+        cls.payment_cycle = cls.__create_payment_cycle()
         cls.beneficiary = cls.__create_beneficiary()
         cls.bill = cls.__create_bill()
-        cls.json_ext_able_bodied_false = """{\\"advanced_criteria\\": [{\\"custom_filter_condition\\": \\"able_bodied__boolean=False\\"}]}"""
-        cls.json_ext_able_bodied_true = """{\\"advanced_criteria\\": [{\\"custom_filter_condition\\": \\"able_bodied__boolean=True\\"}]}"""
+        cls.json_ext_able_bodied_false = """{"advanced_criteria": [{"custom_filter_condition": "able_bodied__boolean=False"}]}"""
+        cls.json_ext_able_bodied_true = """{"advanced_criteria": [{"custom_filter_condition": "able_bodied__boolean=True"}]}"""
+        cls.includedUnpaid = False
 
     def test_query(self):
         output = self.gql_client.execute(gql_payroll_query, context=self.gql_context)
         result = output.get('data', {}).get('payroll', {})
         self.assertTrue(result)
 
     def test_query_unauthorized(self):
         output = self.gql_client.execute(gql_payroll_query, context=self.gql_context_unauthorized)
         error = next(iter(output.get('errors', [])), {}).get('message', None)
         self.assertTrue(error)
 
     def create_payroll(self, name, json_ext):
-        payload = gql_payroll_create % (
-            name,
-            self.benefit_plan.id,
-            self.payment_point.id,
-            self.payment_method,
-            self.status,
-            self.date_valid_from,
-            self.date_valid_to,
-            json_ext,
-        )
-        output = self.gql_client.execute(payload, context=self.gql_context)
+        variables = {
+            "name": name,
+            "paymentCycleId": str(self.payment_cycle.id),
+            "paymentPlanId": str(self.payment_plan.id),
+            "paymentMethod": self.payment_method,
+            "status": PayrollStatus.PENDING_APPROVAL,
+            "dateValidFrom": self.date_valid_from,
+            "dateValidTo": self.date_valid_to,
+            "jsonExt": json_ext,
+            "clientMutationId": str(uuid.uuid4())
+        }
+
+        output = self.gql_client.execute(gql_payroll_create, context=self.gql_context, variable_values=variables)
+
         payroll = Payroll.objects.filter(
             name=name,
-            benefit_plan_id=self.benefit_plan.id,
+            payment_plan_id=self.payment_plan.id,
+            payment_cycle_id=self.payment_cycle.id,
             payment_point_id=self.payment_point.id,
             payment_method=self.payment_method,
             status=self.status,
             date_valid_from=self.date_valid_from,
             date_valid_to=self.date_valid_to,
             is_deleted=False,
         )
         return payroll
 
     def create_payroll_no_json_ext(self, name):
         payload = gql_payroll_create_no_json_ext % (
             name,
-            self.benefit_plan.id,
+            self.payment_cycle.id,
+            self.payment_plan.id,
             self.payment_point.id,
             self.payment_method,
             self.status,
             self.date_valid_from,
             self.date_valid_to,
         )
         output = self.gql_client.execute(payload, context=self.gql_context)
         payroll = Payroll.objects.filter(
             name=name,
-            benefit_plan_id=self.benefit_plan.id,
+            payment_plan_id=self.payment_plan.id,
             payment_point_id=self.payment_point.id,
+            payment_cycle_id=self.payment_cycle.id,
             payment_method=self.payment_method,
             status=self.status,
             date_valid_from=self.date_valid_from,
             date_valid_to=self.date_valid_to,
             is_deleted=False,
         )
         return payroll
@@ -147,109 +160,117 @@
 
         payroll = self.create_payroll(self.name, self.json_ext_able_bodied_true)
         self.assertFalse(payroll.exists())
 
         self.delete_payroll_and_check_bill(payroll_tmp)
 
     def test_create_unauthorized(self):
-        payload = gql_payroll_create % (
-            self.name,
-            self.benefit_plan.id,
-            self.payment_point.id,
-            self.payment_method,
-            self.status,
-            self.date_valid_from,
-            self.date_valid_to,
-            self.json_ext_able_bodied_false,
-        )
-        output = self.gql_client.execute(payload, context=self.gql_context_unauthorized)
+        variables = {
+            "name": self.name,
+            "paymentCycleId": str(self.payment_cycle.id),
+            "paymentPlanId": str(self.payment_plan.id),
+            "paymentMethod": self.payment_method,
+            "status": PayrollStatus.PENDING_APPROVAL,
+            "dateValidFrom": self.date_valid_from,
+            "dateValidTo": self.date_valid_to,
+            "jsonExt": self.json_ext_able_bodied_false,
+            "clientMutationId": str(uuid.uuid4())
+        }
+
+        output = self.gql_client.execute(
+            gql_payroll_create, context=self.gql_context_unauthorized, variable_values=variables)
         self.assertFalse(
             Payroll.objects.filter(
                 name=self.name,
-                benefit_plan_id=self.benefit_plan.id,
+                payment_plan_id=self.benefit_plan.id,
+                payment_cycle_id=self.payment_cycle.id,
                 payment_point_id=self.payment_point.id,
                 payment_method=self.payment_method,
                 status=self.status,
                 date_valid_from=self.date_valid_from,
                 date_valid_to=self.date_valid_to,
                 json_ext=self.json_ext_able_bodied_false,
                 is_deleted=False,
             ).exists()
         )
 
     def test_delete(self):
         payroll = Payroll(name=self.name,
-                          benefit_plan_id=self.benefit_plan.id,
+                          payment_plan_id=self.payment_plan.id,
                           payment_point_id=self.payment_point.id,
+                          payment_cycle_id=self.payment_cycle.id,
                           payment_method=self.payment_method,
                           status=self.status,
                           date_valid_from=self.date_valid_from,
                           date_valid_to=self.date_valid_to,
-                          json_ext=self.json_ext_able_bodied_false,
+                          json_ext=json.loads(self.json_ext_able_bodied_false),
                           )
         payroll.save(username=self.user.username)
         payroll_bill = PayrollBill(payroll=payroll, bill=self.bill)
         payroll_bill.save(username=self.user.username)
         payload = gql_payroll_delete % json.dumps([str(payroll.id)])
         output = self.gql_client.execute(payload, context=self.gql_context)
         self.assertTrue(Payroll.objects.filter(id=payroll.id, is_deleted=True).exists())
         self.assertEqual(PayrollBill.objects.filter(payroll=payroll, bill=self.bill).count(), 0)
 
     def test_delete_unauthorized(self):
         payroll = Payroll(name=self.name,
-                          benefit_plan_id=self.benefit_plan.id,
+                          payment_plan_id=self.payment_plan.id,
+                          payment_cycle_id=self.payment_cycle.id,
                           payment_point_id=self.payment_point.id,
                           payment_method=self.payment_method,
                           status=self.status,
                           date_valid_from=self.date_valid_from,
                           date_valid_to=self.date_valid_to,
-                          json_ext=self.json_ext_able_bodied_true,
+                          json_ext=json.loads(self.json_ext_able_bodied_true),
                           )
         payroll.save(username=self.user.username)
         payroll_bill = PayrollBill(payroll=payroll, bill=self.bill)
         payroll_bill.save(username=self.user.username)
         payload = gql_payroll_delete % json.dumps([str(payroll.id)])
         output = self.gql_client.execute(payload, context=self.gql_context_unauthorized)
         self.assertTrue(Payroll.objects.filter(id=payroll.id, is_deleted=False).exists())
         self.assertEqual(PayrollBill.objects.filter(payroll=payroll, bill=self.bill).count(), 1)
         payroll_bill.delete(username=self.user.username)
         self.assertTrue(PayrollBill.objects.filter(payroll=payroll, bill=self.bill, is_deleted=True))
 
-    def test_check_bill_included_unpaid(self):
-        self.bill.json_ext = {"unpaid": True}
-        self.bill.save(username=self.user.username)
-        bills_queryset_not_paid = Bill.objects.filter(json_ext__unpaid=True)
-        bills_queryset = Bill.objects.filter(
-            Q(json_ext__unpaid=False) |
-            Q(json_ext__unpaid__isnull=True)
-        )
-        self.assertGreaterEqual(bills_queryset_not_paid.count(), 1)
-        self.assertEqual(bills_queryset.count(), 0)
-
-    def test_check_bill_not_included_unpaid(self):
-        bills_queryset_not_paid = Bill.objects.filter(json_ext__unpaid=True)
-        bills_queryset = Bill.objects.filter(
-            Q(json_ext__unpaid=False) |
-            Q(json_ext__unpaid__isnull=True)
-        )
-        self.assertEqual(bills_queryset_not_paid.count(), 0)
-        self.assertGreaterEqual(bills_queryset.count(), 1)
-
     @classmethod
     def __create_benefit_plan(cls):
         object_data = {
             **service_add_payload
         }
 
         benefit_plan = BenefitPlan(**object_data)
         benefit_plan.save(username=cls.user.username)
 
         return benefit_plan
 
     @classmethod
+    def __create_payment_plan(cls, benefit_plan):
+        object_data = {
+            'is_deleted': False,
+            'code': "PP-E",
+            'name': "Example Payment Plan",
+            'benefit_plan': benefit_plan,
+            'periodicity': 1,
+            'calculation': "32d96b58-898a-460a-b357-5fd4b95cd87c",
+            'json_ext': {},
+        }
+
+        payment_plan = PaymentPlan(**object_data)
+        payment_plan.save(username=cls.user.username)
+        return payment_plan
+
+    @classmethod
+    def __create_payment_cycle(cls):
+        pc = PaymentCycle(run_year=2023, run_month=2, type=ContentType.objects.get_for_model(BenefitPlan))
+        pc.save(username=cls.user.username)
+        return pc
+
+    @classmethod
     def __create_individual(cls):
         object_data = {
             **service_add_individual_payload
         }
 
         individual = Individual(**object_data)
         individual.save(username=cls.user.username)
```

### Comparing `openimis-be-payroll-1.0.0/payroll/validation.py` & `openimis_be_payroll-1.1.0/payroll/validation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.core.exceptions import ValidationError
 from django.utils.translation import gettext as _
 
 from core.validation import BaseModelValidation
-from payroll.models import PaymentPoint, Payroll, PayrollBill
+from payroll.models import PaymentPoint, Payroll, PayrollBill, BenefitConsumption
 
 
 class PaymentPointValidation(BaseModelValidation):
     OBJECT_TYPE = PaymentPoint
 
     @classmethod
     def validate_create(cls, user, **data):
@@ -28,14 +28,22 @@
     def validate_create(cls, user, **data):
         errors = validate_payroll(data)
         if errors:
             raise ValidationError(errors)
         super().validate_create(user, **data)
 
 
+class BenefitConsumptionValidation(BaseModelValidation):
+    OBJECT_TYPE = BenefitConsumption
+
+    @classmethod
+    def validate_create(cls, user, **data):
+        super().validate_create(user, **data)
+
+
 def validate_payroll(data):
     return [
         *are_bills_in_data(data),
         *validate_one_payroll_per_bill(data),
         *validate_payroll_unique_name(data, uuid=None),
         *validate_not_empty_field(data, 'name')
     ]
@@ -58,15 +66,15 @@
         }}]
     return []
 
 
 def validate_payroll_unique_name(data, uuid=None):
     name = data.get("name")
     instance = Payroll.objects.filter(name=name, is_deleted=False).first()
-    if instance and str(instance.uuid) != uuid:
+    if instance and instance.uuid != uuid:
         return [{"message": _("payroll.validation.payroll.name_exists" % {
             'name': name
         })}]
     return []
 
 
 def validate_not_empty_field(data, field):
```

### Comparing `openimis-be-payroll-1.0.0/setup.py` & `openimis_be_payroll-1.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-payroll',
-    version='1.0.0',
+    version='v1.1.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend payroll reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
@@ -22,15 +22,16 @@
     install_requires=[
         'django',
         'graphene-django',
         'django-db-signals',
         'djangorestframework',
         'openimis-be-core',
         'openimis-be-location',
-        'openimis-be-invoice'
+        'openimis-be-invoice',
+        'openimis-be-payment_cycle',
     ],
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.0',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3',
```

