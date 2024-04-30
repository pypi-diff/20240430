# Comparing `tmp/openimis-be-claim-1.6.0.tar.gz` & `tmp/openimis_be_claim-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-claim-1.6.0.tar", last modified: Sat Dec 16 00:57:16 2023, max compression
+gzip compressed data, was "openimis_be_claim-1.7.0.tar", last modified: Tue Apr 30 09:05:49 2024, max compression
```

## Comparing `openimis-be-claim-1.6.0.tar` & `openimis_be_claim-1.7.0.tar`

### file list

```diff
@@ -1,75 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:16.814524 openimis-be-claim-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-12-16 00:57:16.814524 openimis-be-claim-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:16.802524 openimis-be-claim-1.6.0/claim/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    45989 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:16.802524 openimis-be-claim-1.6.0/claim/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:16.802524 openimis-be-claim-1.6.0/claim/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/management/commands/generateclaimadmins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/management/commands/generateclaims.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:16.806524 openimis-be-claim-1.6.0/claim/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0002_batchrun.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0003_claimofficer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0004_claimattachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0005_claimmutation.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0006_claimattachment_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0007_auto_20200318_1443.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0008_create_claim_attachments_count_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0009_auto_20200421_1657.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0010_auto_20200611_0601.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0011_auto_20201126_1244.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0012_item_service_jsonExtField.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0013_feedbackprompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0014_change_code_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0015_prohibit_interaction_for_enrolment_officer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11532 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0016_update_django_scheme_with_missing_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0017_set_managed_to_true.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0018_alter_jsonext_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0019_auto_20230615_1055.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0020_alter_claim_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0021_auto_20230818_0914.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0022_alter_feedbackprompt_phone_number.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0023_claim_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0024_add_claim_restore_perms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0025_auto_20231205_1455.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/0026_add_sequences.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26474 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:16.810524 openimis-be-claim-1.6.0/claim/reports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   112176 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/reports/claim.py
--rw-r--r--   0 runner    (1001) docker     (127)   340417 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/reports/claim_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    45285 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/reports/claim_percentage_referrals.py
--rw-r--r--   0 runner    (1001) docker     (127)   340381 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/reports/claims_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)   228066 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/reports/claims_primary_operational_indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11756 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    14599 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:16.810524 openimis-be-claim-1.6.0/claim/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    14300 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)    46484 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/tests/test_validations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    67577 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/validations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2023-12-16 00:57:00.000000 openimis-be-claim-1.6.0/claim/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:16.810524 openimis-be-claim-1.6.0/openimis_be_claim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-12-16 00:57:16.000000 openimis-be-claim-1.6.0/openimis_be_claim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2023-12-16 00:57:16.000000 openimis-be-claim-1.6.0/openimis_be_claim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:57:16.000000 openimis-be-claim-1.6.0/openimis_be_claim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-16 00:57:16.000000 openimis-be-claim-1.6.0/openimis_be_claim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-16 00:57:16.000000 openimis-be-claim-1.6.0/openimis_be_claim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:57:16.814524 openimis-be-claim-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-12-16 00:57:16.000000 openimis-be-claim-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:49.008041 openimis_be_claim-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-30 09:05:49.008041 openimis_be_claim-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:48.996041 openimis_be_claim-1.7.0/claim/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:49.000041 openimis_be_claim-1.7.0/claim/attachment_strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/attachment_strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/attachment_strategies/handle_claimdoc_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43093 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:49.000041 openimis_be_claim-1.7.0/claim/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:49.000041 openimis_be_claim-1.7.0/claim/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/management/commands/generateclaimadmins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/management/commands/generateclaims.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:49.004041 openimis_be_claim-1.7.0/claim/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0002_batchrun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0003_claimofficer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0004_claimattachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0005_claimmutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0006_claimattachment_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0007_auto_20200318_1443.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0008_create_claim_attachments_count_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0009_auto_20200421_1657.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0010_auto_20200611_0601.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0011_auto_20201126_1244.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0012_item_service_jsonExtField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0013_feedbackprompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0014_change_code_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0015_prohibit_interaction_for_enrolment_officer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0016_update_django_scheme_with_missing_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0017_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0018_alter_jsonext_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0019_auto_20230615_1055.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0020_alter_claim_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0021_auto_20230818_0914.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0022_alter_feedbackprompt_phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0023_claim_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0024_add_claim_restore_perms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0025_auto_20231205_1455.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0026_add_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0027_auto_20240203_2339.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0028_claimattachmenttype_claimattachment_predefined_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0028_claimserviceitem_claimserviceservice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0029_rename_pcpdate_claimserviceitem_created_date_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/0030_merge_20240318_1324.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29920 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:49.008041 openimis_be_claim-1.7.0/claim/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112176 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/reports/claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)   340417 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/reports/claim_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47457 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/reports/claim_percentage_referrals.py
+-rw-r--r--   0 runner    (1001) docker     (127)   340561 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/reports/claims_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)   228065 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/reports/claims_primary_operational_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12754 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29402 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:49.008041 openimis_be_claim-1.7.0/claim/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52362 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/tests/test_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17487 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/tests/tests_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72313 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-30 09:05:40.000000 openimis_be_claim-1.7.0/claim/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:49.008041 openimis_be_claim-1.7.0/openimis_be_claim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-30 09:05:48.000000 openimis_be_claim-1.7.0/openimis_be_claim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-30 09:05:48.000000 openimis_be_claim-1.7.0/openimis_be_claim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:05:48.000000 openimis_be_claim-1.7.0/openimis_be_claim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-30 09:05:48.000000 openimis_be_claim-1.7.0/openimis_be_claim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 09:05:48.000000 openimis_be_claim-1.7.0/openimis_be_claim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:05:49.008041 openimis_be_claim-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-30 09:05:48.000000 openimis_be_claim-1.7.0/setup.py
```

### Comparing `openimis-be-claim-1.6.0/LICENSE.md` & `openimis_be_claim-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/PKG-INFO` & `openimis_be_claim-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-claim
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Claim reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-claim-1.6.0/README.md` & `openimis_be_claim-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/apps.py` & `openimis_be_claim-1.7.0/claim/apps.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     "claim_attachments_root_path": None,
     "claim_uspUpdateClaimFromPhone_intermediate_sets": 2,
     "autogenerated_claim_code_config": {'code_length': 8},
     "max_claim_length": 20,
     "claim_validation_multiple_services_explanation_required": True,
     "autogenerate_func": 'claim.utils.autogenerate_nepali_claim_code',
     "additional_diagnosis_number_allowed": 4,
-    "claim_max_restore": None
+    "claim_max_restore": None,
+    "allowed_domains_attachments": [],
+    "native_code_for_services": True
 }
 
 
 class ClaimConfig(AppConfig):
     name = MODULE_NAME
 
     default_validations_disabled = None
@@ -58,21 +60,23 @@
     gql_mutation_process_claims_perms = []
     gql_mutation_restore_claims_perms = []
     gql_mutation_delete_claims_perms = []
     claim_print_perms = []
     claim_attachments_root_path = None
     claim_uspUpdateClaimFromPhone_intermediate_sets = None
     autogenerated_claim_code_config = {}
+    native_code_for_services = True
     # cannot be set in the model, since migration has to be able to handle all implementations
     max_claim_length = None
     claim_max_restore = None
     claim_validation_multiple_services_explanation_required = None
     # Provide absolute path to autogenerating function for claim code
     autogenerate_func = None
     additional_diagnosis_number_allowed = None  # Currently code supports 4 diagnoses maximum, going above will not work
+    allowed_domains_attachments = None
 
     def __load_config(self, cfg):
         for field in cfg:
             if hasattr(ClaimConfig, field):
                 setattr(ClaimConfig, field, cfg[field])
 
     def ready(self):
```

### Comparing `openimis-be-claim-1.6.0/claim/gql_mutations.py` & `openimis_be_claim-1.7.0/claim/gql_mutations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 import logging
+import os
+import urllib.parse
 import uuid
 import pathlib
 import base64
+from urllib.parse import urlparse
 from typing import Callable, Dict
 
 import graphene
 import importlib
 import graphene_django_optimizer
-from django.db.models import Count, Case, When, IntegerField, Q
+from django.db.models import Count, Case, When, IntegerField, Q, Prefetch
 
 from core.models import MutationLog, Officer
 from .apps import ClaimConfig
 from claim.validations import validate_claim, get_claim_category, validate_assign_prod_to_claimitems_and_services, \
     process_dedrem, approved_amount
 from core import filter_validity, assert_string_length
 from core.schema import TinyInt, SmallInt, OpenIMISMutation
 from core.gql.gql_mutations import mutation_on_uuids_from_filter
 from django.conf import settings
 from django.contrib.auth.models import AnonymousUser
 from django.core.exceptions import ValidationError, PermissionDenied, ObjectDoesNotExist
 from django.utils.translation import gettext as _
 from graphene import InputObjectType
-
 from claim.gql_queries import ClaimGQLType
 from claim.models import Claim, Feedback, FeedbackPrompt, ClaimDetail, ClaimItem, ClaimService, ClaimAttachment, \
-    ClaimDedRem
+    ClaimDedRem, GeneralClaimAttachmentType, ClaimAttachmentType,ClaimServiceService
+from claim.attachment_strategies import *
+
 from product.models import ProductItemOrService
+from medical.models import Item, Service
 
 from claim.utils import process_items_relations, process_services_relations
-from .services import check_unique_claim_code
+from claim.services import validate_claim_data as service_validate_claim_data, \
+        update_or_create_claim as service_update_or_create_claim, check_unique_claim_code, submit_claim,\
+            validate_and_process_dedrem_claim as service_validate_and_process_dedrem_claim,\
+            create_feedback_prompt as service_create_feedback_prompt, update_claims_dedrems,\
+                set_feedback_prompt_validity_to_to_current_date, set_claims_status
 from django.db import transaction
+import requests
 
 logger = logging.getLogger(__name__)
 
 
 class ClaimItemInputType(InputObjectType):
     id = graphene.Int(required=False)
     item_id = graphene.Int(required=True)
@@ -65,14 +75,34 @@
         max_digits=18, decimal_places=2, required=False)
     exceed_ceiling_amount = graphene.Decimal(
         max_digits=18, decimal_places=2, required=False)
     price_origin = graphene.String(required=False)
     exceed_ceiling_amount_category = graphene.Decimal(
         max_digits=18, decimal_places=2, required=False)
 
+class ClaimSubServiceInputType(InputObjectType):
+    id = graphene.Int(required=False)
+    sub_service_code = graphene.String(required=True)
+    qty_provided = graphene.Decimal(
+        max_digits=18, decimal_places=2, required=False)
+    qty_asked = graphene.Decimal(
+        max_digits=18, decimal_places=2, required=False)
+    price_asked = graphene.Decimal(
+        max_digits=18, decimal_places=2, required=False)
+
+
+class ClaimSubItemInputType(InputObjectType):
+    id = graphene.Int(required=False)
+    sub_item_code = graphene.String(required=True)
+    qty_provided = graphene.Decimal(
+        max_digits=18, decimal_places=2, required=False)
+    qty_asked = graphene.Decimal(
+        max_digits=18, decimal_places=2, required=False)
+    price_asked = graphene.Decimal(
+        max_digits=18, decimal_places=2, required=False)
 
 class ClaimServiceInputType(InputObjectType):
     id = graphene.Int(required=False)
     legacy_id = graphene.Int(required=False)
     service_id = graphene.Int(required=True)
     status = TinyInt(required=True)
     qty_provided = graphene.Decimal(
@@ -104,14 +134,16 @@
         max_digits=18, decimal_places=2, required=False,
         description="deductable is spelled with a, not deductible")
     exceed_ceiling_amount = graphene.Decimal(
         max_digits=18, decimal_places=2, required=False)
     price_origin = graphene.String(max_length=1, required=False)
     exceed_ceiling_amount_category = graphene.Decimal(
         max_digits=18, decimal_places=2, required=False)
+    service_item_set = graphene.List(ClaimSubItemInputType, required=False)
+    service_service_set = graphene.List(ClaimSubServiceInputType, required=False)
 
 
 class FeedbackInputType(InputObjectType):
     id = graphene.Int(required=False, read_only=True)
     care_rendered = graphene.Boolean(required=False)
     payment_asked = graphene.Boolean(required=False)
     drug_prescribed = graphene.Boolean(required=False)
@@ -162,14 +194,16 @@
 class BaseAttachment:
     id = graphene.String(required=False, read_only=True)
     type = graphene.String(required=False)
     title = graphene.String(required=False)
     date = graphene.Date(required=False)
     filename = graphene.String(required=False)
     mime = graphene.String(required=False)
+    general_type = graphene.String(required=False)
+    predefined_type = graphene.String(required=False)
     url = graphene.String(required=False)
 
 
 class BaseAttachmentInputType(BaseAttachment, OpenIMISMutation.Input):
     """
     Claim attachment (without the document), used on its own
     """
@@ -227,30 +261,19 @@
     feedback = graphene.Field(FeedbackInputType, required=False)
     care_type = graphene.String(required=False)
 
     items = graphene.List(ClaimItemInputType, required=False)
     services = graphene.List(ClaimServiceInputType, required=False)
 
 
+
 class CreateClaimInputType(ClaimInputType):
     attachments = graphene.List(ClaimAttachmentInputType, required=False)
 
 
-def reset_claim_before_update(claim):
-    claim.date_to = None
-    claim.icd_1 = None
-    claim.icd_2 = None
-    claim.icd_3 = None
-    claim.icd_4 = None
-    claim.guarantee_id = None
-    claim.explanation = None
-    claim.adjustment = None
-    claim.json_ext = None
-
-
 def create_file(date, claim_id, document):
     date_iso = date.isoformat()
     root = ClaimConfig.claim_attachments_root_path
     file_dir = '%s/%s/%s/%s' % (
         date_iso[0:4],
         date_iso[5:7],
         date_iso[8:10],
@@ -264,136 +287,53 @@
     return file_path
 
 
 def create_attachment(claim_id, data):
     data["claim_id"] = claim_id
     from core import datetime
     now = datetime.datetime.now()
-    if ClaimConfig.claim_attachments_root_path:
-        # don't use data date as it may be updated by user afterwards!
-        data['url'] = create_file(now, claim_id, data.pop('document'))
+    general_type = data['general_type']
+    data['module'] = 'claim'
+    if general_type == GeneralClaimAttachmentType.URL:
+        parsed_url = urlparse(data['url'])
+        if (ClaimConfig.allowed_domains_attachments and
+                not any(domain in parsed_url.path for domain in ClaimConfig.allowed_domains_attachments)):
+            raise ValidationError(_("mutation.attachment_url_domain_not_allowed"))
+        if data['predefined_type'] in attachment_strategies_dict:
+            data['url'] = attachment_strategies_dict[data['predefined_type']].handler(data)
+            data['document'] = data['url']
+        data['predefined_type'] = ClaimAttachmentType.objects.get(validity_to__isnull=True, claim_general_type="URL",
+                                                                  claim_attachment_type=data['predefined_type'])
+    elif general_type == GeneralClaimAttachmentType.FILE:
+        if ClaimConfig.claim_attachments_root_path:
+            # don't use data date as it may be updated by user afterwards!
+            data['url'] = create_file(now, claim_id, data.pop('document'))
+        data['predefined_type'] = ClaimAttachmentType.objects.get(validity_to__isnull=True, claim_general_type="FILE",
+                                                                  claim_attachment_type=data['predefined_type'])
+    else:
+        raise ValidationError(_("mutation.attachment_general_type_incorrect"))
     data['validity_from'] = now
     ClaimAttachment.objects.create(**data)
 
 
 def create_attachments(claim_id, attachments):
     for attachment in attachments:
         create_attachment(claim_id, attachment)
 
 
 def validate_claim_data(data, user):
-    services = data.get('services') if 'services' in data else []
-    incoming_code = data.get('code')
-    claim_uuid = data.get("uuid", None)
-    restore = data.get('restore', None)
-    current_claim = Claim.objects.filter(uuid=claim_uuid).first()
-    current_code = current_claim.code if current_claim else None
-    
- 
-
-    if restore:
-        restored_qs = Claim.objects.filter(uuid=restore)
-        restored_from_claim = restored_qs.first()
-        restored_count = Claim.objects.filter(restore=restored_from_claim).count()
-        if not restored_qs.exists():
-            raise ValidationError(_("mutation.restored_from_does_not_exist"))
-        if not restored_from_claim.status == Claim.STATUS_REJECTED:
-            raise ValidationError(_("mutation.cannot_restore_not_rejected_claim"))
-        if not user.has_perms(ClaimConfig.gql_mutation_restore_claims_perms):
-            raise ValidationError(_("mutation.no_restore_rights"))
-        if ClaimConfig.claim_max_restore and restored_count >= ClaimConfig.claim_max_restore:
-            raise ValidationError(_("mutation.max_restored_claim") % {
-                "max_restore": ClaimConfig.claim_max_restore
-            })
-           
-    elif current_claim is not None and current_claim.status not in (Claim.STATUS_CHECKED, Claim.STATUS_ENTERED):
-        raise ValidationError(_("mutation.claim_not_editable")) 
-
-    if not validate_number_of_additional_diagnoses(data):
-        raise ValidationError(_("mutation.claim_too_many_additional_diagnoses"))
-
-    if ClaimConfig.claim_validation_multiple_services_explanation_required:
-        for service in services:
-            if service["qty_provided"] > 1 and not service.get("explanation"):
-                raise ValidationError(_("mutation.service_explanation_required"))
-
-    if len(incoming_code) > ClaimConfig.max_claim_length:
-        raise ValidationError(_("mutation.code_name_too_long"))
-
-    if not restore and current_code != incoming_code and check_unique_claim_code(incoming_code):
-        raise ValidationError(_("mutation.code_name_duplicated"))
-
+    return service_validate_claim_data(data, user)
 
 @transaction.atomic
 def update_or_create_claim(data, user):
-    validate_claim_data(data, user)
-    items = data.pop('items') if 'items' in data else []
-    services = data.pop('services') if 'services' in data else []
-    claim_uuid = data.pop("uuid", None)
-    autogenerate_code = data.pop('autogenerate', None)
-    restore = data.pop('restore', None)
-    if restore:
-        restored_qs = Claim.objects.filter(uuid=restore)
-        restored_from_claim = restored_qs.first()
-        data["restore"] = restored_from_claim
-    if autogenerate_code:
-        data['code'] = __autogenerate_claim_code()
     if "client_mutation_id" in data:
         data.pop('client_mutation_id')
     if "client_mutation_label" in data:
-        data.pop('client_mutation_label')
-    # update_or_create(uuid=claim_uuid, ...)
-    # doesn't work because of explicit attempt to set null to uuid!
-    if claim_uuid:
-        claim = Claim.objects.get(uuid=claim_uuid)
-        claim.save_history()
-        # reset the non required fields
-        # (each update is 'complete', necessary to be able to set 'null')
-        reset_claim_before_update(claim)
-        [setattr(claim, key, data[key]) for key in data]
-    else:
-        claim = Claim.objects.create(**data)
-    from core.utils import TimeUtils
-    claimed = 0
-    claim.items.update(validity_to=TimeUtils.now())
-    claimed += process_items_relations(user, claim, items)
-    claim.services.update(validity_to=TimeUtils.now())
-    claimed += process_services_relations(user, claim, services)
-
-    claim.claimed = claimed
-    claim.save()
-    return claim
-
-
-def validate_number_of_additional_diagnoses(incoming_data):
-    additional_diagnoses_count = 0
-    for key in incoming_data.keys():
-        if key.startswith("icd_") and key.endswith("_id") and key != "icd_id":
-            additional_diagnoses_count += 1
-
-    return additional_diagnoses_count <= ClaimConfig.additional_diagnosis_number_allowed
-
-
-def __autogenerate_claim_code():
-    module_name, function_name = '[undefined]', '[undefined]'
-    try:
-        claim_code_function = _get_autogenerating_func()
-        return claim_code_function(ClaimConfig.autogenerated_claim_code_config)
-    except ImportError as e:
-        logger.error(f"Error: Could not import module '{module_name}' for claim code autogeneration")
-        raise e
-    except AttributeError as e:
-        logger.error(f"Error: Could not find function '{function_name}' in module '{module_name}' for claim code autogeneration")
-        raise e
-
-
-def _get_autogenerating_func() -> Callable[[Dict], Callable]:
-    module_name, function_name = ClaimConfig.autogenerate_func.rsplit('.', 1)
-    module = importlib.import_module(module_name)
-    return getattr(module, function_name)
+        data.pop('client_mutation_label') 
+    return service_update_or_create_claim(data, user)
 
 
 class CreateClaimMutation(OpenIMISMutation):
     """
     Create a new claim. The claim items and services can all be entered with this call
     """
     _mutation_module = "claim"
@@ -408,15 +348,14 @@
             # TODO move this verification to OIMutation
             if type(user) is AnonymousUser or not user.id:
                 raise ValidationError(
                     _("mutation.authentication_required"))
             if not user.has_perms(ClaimConfig.gql_mutation_create_claims_perms):
                 raise PermissionDenied(_("unauthorized"))
             is_claim_code_autogenerated = data.get("autogenerate", False)
-            data['audit_user_id'] = user.id_for_audit
             data['status'] = Claim.STATUS_ENTERED
             from core.utils import TimeUtils
             data['validity_from'] = TimeUtils.now()
             attachments = data.pop('attachments') if 'attachments' in data else None
             claim = update_or_create_claim(data, user)
             if attachments:
                 create_attachments(claim.id, attachments)
@@ -500,22 +439,44 @@
     @classmethod
     def async_mutate(cls, user, **data):
         try:
             if not user.has_perms(ClaimConfig.gql_mutation_update_claims_perms):
                 raise PermissionDenied(_("unauthorized"))
             queryset = ClaimAttachment.objects.filter(*filter_validity())
             if settings.ROW_SECURITY:
-                from location.schema import  LocationManager
+                from location.schema import LocationManager
                 queryset = LocationManager().build_user_location_filter_query( user._u, prefix='claim__health_facility__location', queryset = queryset.select_related("claim"), loc_types=['D'])
 
             attachment = queryset \
                 .filter(id=data['id']) \
                 .first()
             if not attachment:
                 raise PermissionDenied(_("unauthorized"))
+            general_type = data['general_type']
+            data['module'] = 'claim'
+            from core import datetime
+            now = datetime.datetime.now()
+            if general_type == GeneralClaimAttachmentType.URL:
+                parsed_url = urlparse(data['url'])
+                if (ClaimConfig.allowed_domains_attachments and
+                        not any(domain in parsed_url.path for domain in ClaimConfig.allowed_domains_attachments)):
+                    raise ValidationError(_("mutation.attachment_url_domain_not_allowed"))
+                if data['predefined_type'] in attachment_strategies_dict:
+                    data['url'] = attachment_strategies_dict[data['predefined_type']].handler(data)
+                    data['document'] = data['url']
+                data['predefined_type'] = ClaimAttachmentType.objects.get(validity_to__isnull=True,
+                                                                          claim_general_type="URL",
+                                                                          claim_attachment_type=data['predefined_type'])
+            elif general_type == GeneralClaimAttachmentType.FILE:
+                if ClaimConfig.claim_attachments_root_path:
+                    # don't use data date as it may be updated by user afterwards!
+                    data['url'] = create_file(now, claim_id, data.pop('document'))
+                data['predefined_type'] = ClaimAttachmentType.objects.get(validity_to__isnull=True,
+                                                                          claim_general_type="FILE",
+                                                                          claim_attachment_type=data['predefined_type'])
             attachment.save_history()
             data['audit_user_id'] = user.id_for_audit
             [setattr(attachment, key, data[key]) for key in data]
             attachment.save()
             return None
         except Exception as exc:
             return [{
@@ -631,134 +592,48 @@
     @mutation_on_uuids_from_filter(Claim, ClaimGQLType, 'additional_filters', __filter_handlers)
     def async_mutate(cls, user, **data):
         if not user.has_perms(ClaimConfig.gql_mutation_submit_claims_perms):
             raise PermissionDenied(_("unauthorized"))
         errors = []
         uuids = data.get("uuids", [])
         client_mutation_id = data.get("client_mutation_id", None)
-
-        for claim_uuid in uuids:
-            c_errors = []
-            claim = Claim.objects \
-                .filter(uuid=claim_uuid,
+        c_errors = []
+        claims = Claim.objects \
+                .filter(uuid__in=uuids,
                         validity_to__isnull=True) \
-                .prefetch_related("items") \
-                .prefetch_related("services") \
-                .first()
-            if claim is None:
-                errors += {
-                    'title': claim_uuid,
-                    'list': [
-                        {'message': _(
-                            "claim.validation.id_does_not_exist") % {'id': claim_uuid}}
-                    ]
-                }
-                continue
-            claim.save_history()
-            logger.debug("SubmitClaimsMutation: validating claim %s", claim_uuid)
-            c_errors += validate_claim(claim, True)
-            logger.debug("SubmitClaimsMutation: claim %s validated, nb of errors: %s", claim_uuid, len(c_errors))
-            if len(c_errors) == 0:
-                c_errors = validate_assign_prod_to_claimitems_and_services(claim)
-                logger.debug("SubmitClaimsMutation: claim %s assigned, nb of errors: %s", claim_uuid, len(c_errors))
-                c_errors += process_dedrem(claim, user.id_for_audit, False)
-                logger.debug("SubmitClaimsMutation: claim %s processed for dedrem, nb of errors: %s", claim_uuid,
-                             len(errors))
-            c_errors += set_claim_submitted(claim, c_errors, user)
-            logger.debug("SubmitClaimsMutation: claim %s set submitted", claim_uuid)
+            .prefetch_related(Prefetch('items', queryset=ClaimItem.objects.filter(
+                *filter_validity(), 
+                Q(Q(rejection_reason=0) | Q(rejection_reason__isnull=True))))) \
+            .prefetch_related(Prefetch('services', queryset=ClaimService.objects.filter(
+                *filter_validity(),
+                Q(Q(rejection_reason=0) | Q(rejection_reason__isnull=True))))) 
+        remaining_uuid = list(map(str.upper,uuids))
+        for claim in claims:
+            remaining_uuid.remove(claim.uuid.upper())
+            c_errors += submit_claim(claim, user)
             if c_errors:
                 errors.append({
                     'title': claim.code,
                     'list': c_errors
                 })
+        if len(remaining_uuid):
+            c_errors.append( {'code': REJECTION_REASON_INVALID_CLAIM,
+                            'message': _("claim.validation.claim_uuid_not_found") + ','.join(remaining_uuid) })
         if len(errors) == 1:
             errors = errors[0]['list']
         cls.add_submission_stats_to_mutation_log(client_mutation_id, uuids)
         logger.debug("SubmitClaimsMutation: claim done, errors: %s", len(errors))
         return errors
 
 
-def set_claims_status(uuids, field, status, audit_data=None, user=None):
-    errors = []
-    for claim_uuid in uuids:
-        claim = Claim.objects \
-            .filter(uuid=claim_uuid,
-                    validity_to__isnull=True) \
-            .first()
-        if claim is None:
-            errors += [{'message': _(
-                "claim.validation.id_does_not_exist") % {'id': claim_uuid}}]
-            continue
-        try:
-            claim.save_history()
-            setattr(claim, field, status)
-            # creating/cancelling feedback prompts
-            if field == 'feedback_status':
-                if status == Claim.FEEDBACK_SELECTED:
-                    create_feedback_prompt(claim_uuid, user)
-                elif status in [Claim.FEEDBACK_NOT_SELECTED, Claim.FEEDBACK_BYPASSED]:
-                    set_feedback_prompt_validity_to_to_current_date(claim_uuid)
-            if audit_data:
-                for k, v in audit_data.items():
-                    setattr(claim, k, v)
-            claim.save()
-        except Exception as exc:
-            errors += [
-                {'message': _("claim.mutation.failed_to_change_status_of_claim") %
-                            {'code': claim.code}}]
-
-    return errors
-
 
 def create_feedback_prompt(claim_uuid, user):
     current_claim = Claim.objects.get(uuid=claim_uuid)
-    feedback_prompt = {}
-    from core.utils import TimeUtils
-    feedback_prompt['feedback_prompt_date'] = TimeUtils.date()
-    feedback_prompt['validity_from'] = TimeUtils.now()
-    feedback_prompt['claim'] = current_claim
-    villages = []
-    if current_claim.insuree.current_village:
-        villages.append(current_claim.insuree.current_village)
-    if current_claim.insuree.family.location:
-        villages.append(current_claim.insuree.family.location)
-    officer = Officer.objects.filter(
-        *filter_validity(),
-        officer_villages__location__in=villages
-    ).first()
-    if not officer:
-        raise RuntimeError(f"No officer found for the insuree village code {', '.join([str(v.code) for v in villages ])}")
-    feedback_prompt['officer_id'] = officer.id
-    feedback_prompt['audit_user_id'] = user.id_for_audit
-    FeedbackPrompt.objects.create(
-        **feedback_prompt
-    )
-
-
-
-def set_feedback_prompt_validity_to_to_current_date(claim_uuid):
-    try:
-        claim = Claim.objects.get(uuid=claim_uuid).id
-        feedback_prompt_id = FeedbackPrompt.objects.get(claim=claim, validity_to=None).id
-        from core.utils import TimeUtils
-        current_feedback_prompt = FeedbackPrompt.objects.get(id=feedback_prompt_id)
-        current_feedback_prompt.validity_to = TimeUtils.now()
-        current_feedback_prompt.save()
-    except ObjectDoesNotExist:
-        return "No such feedback prompt exist."
-
-
-def update_claims_dedrems(uuids, user):
-    # We could do it in one query with filter(claim__uuid__in=uuids) but we'd loose the logging
-    errors = []
-    for uuid in uuids:
-        logger.debug(f"delivering review on {uuid}, reprocessing dedrem ({user})")
-        claim = Claim.objects.get(uuid=uuid)
-        errors += validate_and_process_dedrem_claim(claim, user, False)
-    return errors
+    return service_create_feedback_prompt(current_claim, user)
+    
 
 
 class SelectClaimsForFeedbackMutation(OpenIMISMutation):
     """
     Select one or several claims for feedback.
     """
     _mutation_module = "claim"
@@ -961,20 +836,63 @@
             all_rejected = True
             for item in items:
                 item_id = item.pop('id')
                 claim.items.filter(id=item_id).update(**item)
                 if item['status'] == ClaimItem.STATUS_PASSED:
                     all_rejected = False
             services = data.pop('services') if 'services' in data else []
+            claimed = 0
+            claim_service_elements = []
             for service in services:
                 service_id = service.pop('id')
+                service_linked = service.pop('service_service_set', [])
+                logger.debug("service_linked ", service_linked)
+                service_service_set = service.pop('service_service_set', [])
+                logger.debug("service_service_set ", service_service_set)
                 claim.services.filter(id=service_id).update(**service)
+                if ClaimConfig.native_code_for_services == False:
+                    for claim_service_service in service_service_set:
+                        claim_service_code = claim_service_service.pop('subServiceCode')
+                        claim_service = claim.services.filter(id=service_id).first()
+                        if claim_service:
+                            service_element = Service.objects.filter(*filter_validity(), code=claim_service_code).first()
+                            if service_element:
+                                claim_service_to_update = claim_service.services.filter(service=service_element.id)
+                                logger.debug("claim_service_to_update ", claim_service_to_update)
+                                if claim_service_to_update:
+                                    qty_asked = claim_service_service.pop('qty_asked', 0)
+                                    price_asked = claim_service_service.pop('price_asked', 0)
+                                    claim_service_service['qty_displayed'] = qty_asked
+                                    price = qty_asked * price_asked
+                                    claimed += price
+                                    claim_service_to_update.update(**claim_service_service)
+                            claim_service_elements.append(claim_service)
+                    for claim_service_item in service_linked:
+                        claim_item_code = claim_service_item.pop('subItemCode')
+                        claim_service = claim.services.filter(id=service_id).first()
+                        if claim_service:
+                            item_element = Item.objects.filter(*filter_validity(), code=claim_item_code).first()
+                            if item_element:
+                                claim_item_to_update = claim_service.items.filter(item=item_element.id)
+                                logger.debug("claim_item_to_update ", claim_item_to_update)
+                                if claim_item_to_update:
+                                    qty_asked = claim_service_item.pop('qty_asked', 0)
+                                    price_asked = claim_service_item.pop('price_asked', 0)
+                                    claim_service_item['qty_displayed'] = qty_asked
+                                    price = qty_asked * price_asked
+                                    claimed += price
+                                    claim_item_to_update.update(**claim_service_item)
+
                 if service['status'] == ClaimService.STATUS_PASSED:
                     all_rejected = False
             claim.approved = approved_amount(claim)
+            if ClaimConfig.native_code_for_services == False:
+                claim.claimed = claimed
+                for claimservice in claim_service_elements:
+                    setattr(claimservice, 'price_adjusted', claimed)
             claim.audit_user_id_review = user.id_for_audit
             if all_rejected:
                 claim.status = Claim.STATUS_REJECTED
             claim.save()
             return None
         except Exception as exc:
             return [{
@@ -1006,41 +924,44 @@
     @classmethod
     def async_mutate(cls, user, **data):
         if not user.has_perms(ClaimConfig.gql_mutation_process_claims_perms):
             raise PermissionDenied(_("unauthorized"))
         errors = []
         uuids = data.get("uuids", None)
         client_mutation_id = data.get("client_mutation_id", None)
-        for claim_uuid in uuids:
-            logger.debug("ProcessClaimsMutation: processing %s", claim_uuid)
+        claims = Claim.objects \
+                .filter(uuid__in=uuids) \
+                .prefetch_related(Prefetch('items', queryset=ClaimItem.objects.filter(*filter_validity())))\
+                .prefetch_related(Prefetch('services', queryset=ClaimService.objects.filter(*filter_validity())))
+        remaining_uuid = list(map(str.upper,uuids))
+        for claim in claims:
+            remaining_uuid.remove(claim.uuid.upper())
+            
+
+            logger.debug("ProcessClaimsMutation: processing %s", claim.uuid)
             c_errors = []
-            claim = Claim.objects \
-                .filter(uuid=claim_uuid) \
-                .prefetch_related("items") \
-                .prefetch_related("services") \
-                .first()
-            if claim is None:
-                errors += {
-                    'title': claim_uuid,
-                    'list': [{'message': _(
-                        "claim.validation.id_does_not_exist") % {'id': claim_uuid}}]
-                }
-                continue
+     
             claim.save_history()
             claim.audit_user_id_process = user.id_for_audit
-            logger.debug("ProcessClaimsMutation: validating claim %s", claim_uuid)
+            logger.debug("ProcessClaimsMutation: validating claim %s", claim.uuid)
             c_errors += validate_and_process_dedrem_claim(claim, user, True)
 
-            logger.debug("ProcessClaimsMutation: claim %s set processed or valuated", claim_uuid)
+            logger.debug("ProcessClaimsMutation: claim %s set processed or valuated", claim.uuid)
             if c_errors:
                 errors.append({
                     'title': claim.code,
                     'list': c_errors
                 })
-
+                
+        if len(remaining_uuid):
+                errors += {
+                    'title': _('error'),
+                    'list': [{'message': _(
+                        "claim.validation.id_does_not_exist") % {'id': ','.join(remaining_uuid)}}]
+                }
         if len(errors) == 1:
             errors = errors[0]['list']
         cls.add_submission_stats_to_mutation_log(client_mutation_id, uuids)
         logger.debug("ProcessClaimsMutation: claims %s done, errors: %s", data["uuids"], len(errors))
         return errors
 
 
@@ -1059,50 +980,31 @@
     def async_mutate(cls, user, **data):
         if not user.has_perms(ClaimConfig.gql_mutation_delete_claims_perms):
             raise PermissionDenied(_("unauthorized"))
         errors = []
         for claim_uuid in data["uuids"]:
             claim = Claim.objects \
                 .filter(uuid=claim_uuid) \
-                .prefetch_related("items") \
-                .prefetch_related("services") \
+                .prefetch_related(Prefetch('items', queryset=ClaimItem.objects.filter(*filter_validity())))\
+                .prefetch_related(Prefetch('services', queryset=ClaimService.objects.filter(*filter_validity())))\
                 .first()
             if claim is None:
                 errors += {
                     'title': claim_uuid,
                     'list': [{'message': _(
                         "claim.validation.id_does_not_exist") % {'id': claim_uuid}}]
                 }
                 continue
             errors += set_claim_deleted(claim)
         if len(errors) == 1:
             errors = errors[0]['list']
         return errors
 
 
-def set_claim_submitted(claim, errors, user):
-    try:
-        claim.audit_user_id_submit = user.id_for_audit
-        if errors:
-            claim.status = Claim.STATUS_REJECTED
-        else:
-            claim.approved = approved_amount(claim)
-            claim.status = Claim.STATUS_CHECKED
-            from core.utils import TimeUtils
-            claim.submit_stamp = TimeUtils.now()
-            claim.category = get_claim_category(claim)
-        claim.save()
-        return []
-    except Exception as exc:
-        return {
-            'title': claim.code,
-            'list': [{
-                'message': _("claim.mutation.failed_to_change_status_of_claim") % {'code': claim.code},
-                'detail': claim.uuid}]
-        }
+
 
 
 def set_claim_deleted(claim):
     try:
         claim.delete_history()
         return []
     except Exception as exc:
@@ -1110,53 +1012,11 @@
             'title': claim.code,
             'list': [{
                 'message': _("claim.mutation.failed_to_change_status_of_claim") % {'code': claim.code},
                 'detail': claim.uuid}]
         }
 
 
-def details_with_relative_prices(details):
-    return details.filter(status=ClaimDetail.STATUS_PASSED) \
-        .filter(price_origin=ProductItemOrService.ORIGIN_RELATIVE) \
-        .exists()
-
-
-def with_relative_prices(claim):
-    return details_with_relative_prices(claim.items) or details_with_relative_prices(claim.services)
-
-
-def set_claim_processed_or_valuated(claim, errors, user):
-    try:
-        if errors:
-            claim.status = Claim.STATUS_REJECTED
-        else:
-            claim.status = Claim.STATUS_PROCESSED if with_relative_prices(claim) else Claim.STATUS_VALUATED
-            claim.audit_user_id_process = user.id_for_audit
-            from core.utils import TimeUtils
-            claim.process_stamp = TimeUtils.now()
-        claim.save()
-        return []
-    except Exception as ex:
-        return {
-            'title': claim.code,
-            'list': [{'message': _("claim.mutation.failed_to_change_status_of_claim") % {'code': claim.code},
-                      'detail': claim.uuid}]
-        }
 
 
 def validate_and_process_dedrem_claim(claim, user, is_process):
-    errors = validate_claim(claim, False)
-    logger.debug("ProcessClaimsMutation: claim %s validated, nb of errors: %s", claim.uuid, len(errors))
-    if len(errors) == 0:
-        errors = validate_assign_prod_to_claimitems_and_services(claim)
-        logger.debug("ProcessClaimsMutation: claim %s assigned, nb of errors: %s", claim.uuid, len(errors))
-        errors += process_dedrem(claim, user.id_for_audit, is_process)
-        logger.debug("ProcessClaimsMutation: claim %s processed for dedrem, nb of errors: %s", claim.uuid,
-                     len(errors))
-    else:
-        # OMT-208 the claim is invalid. If there is a dedrem, we need to clear it (caused by a review)
-        deleted_dedrems = ClaimDedRem.objects.filter(claim=claim).delete()
-        if deleted_dedrems:
-            logger.debug(f"Claim {claim.uuid} is invalid, we deleted its dedrem ({deleted_dedrems})")
-    if is_process:
-        errors += set_claim_processed_or_valuated(claim, errors, user)
-    return errors
+    return service_validate_and_process_dedrem_claim(claim, user, is_process)
```

### Comparing `openimis-be-claim-1.6.0/claim/gql_queries.py` & `openimis_be_claim-1.7.0/claim/gql_queries.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from graphene.utils.deduplicator import deflate
 from graphene_django import DjangoObjectType
 from insuree.schema import InsureeGQLType
 from location.schema import HealthFacilityGQLType
 from medical.schema import DiagnosisGQLType
 from claim_batch.schema import BatchRunGQLType
 from .apps import ClaimConfig
-from .models import ClaimDedRem, Claim, ClaimAdmin, Feedback, ClaimItem, ClaimService, ClaimAttachment
+from claim.models import (ClaimDedRem, Claim, ClaimAdmin, Feedback, ClaimItem, ClaimService, ClaimAttachment,
+                          ClaimAttachmentType, ClaimServiceService, ClaimServiceItem)
 from django.utils.translation import gettext as _
 from django.core.exceptions import PermissionDenied
 
 
 class ClaimDedRemGQLType(DjangoObjectType):
     """
     Details about Claim demands and remunerated amounts
@@ -51,15 +52,16 @@
     The filters are possible on BatchRun, Insuree, HealthFacility, Admin and ICD in addition to the Claim fields
     themselves.
     """
 
     attachments_count = graphene.Int()
     client_mutation_id = graphene.String()
     date_processed_to = graphene.Date()
-
+    restore_id = graphene.Int()
+    
     def resolve_insuree(self, info):
         if not info.context.user.has_perms(ClaimConfig.gql_query_claims_perms):
             raise PermissionDenied(_("unauthorized"))
         if "insuree_loader" in info.context.dataloaders and self.insuree_id:
             return info.context.dataloaders["insuree_loader"].load(self.insuree_id)
         return self.insuree
 
@@ -70,15 +72,19 @@
             "health_facility_loader" in info.context.dataloaders
             and self.health_facility_id
         ):
             return info.context.dataloaders["health_facility_loader"].load(
                 self.health_facility_id
             )
         return self.health_facility
-
+    
+    def resolve_restore_id(self, info):
+        return self.restore_id
+        
+        
     class Meta:
         model = Claim
         interfaces = (graphene.relay.Node,)
         filter_fields = {
             "uuid": ["exact"],
             "code": ["exact", "istartswith", "icontains", "iexact"],
             "status": ["exact", "gt"],
@@ -123,39 +129,50 @@
         return claim_mutation.mutation.client_mutation_id if claim_mutation else None
 
     @classmethod
     def get_queryset(cls, queryset, info):
         return Claim.get_queryset(queryset, info).all()
 
 
-
 class ClaimAttachmentGQLType(DjangoObjectType):
     doc = graphene.String()
 
     class Meta:
         model = ClaimAttachment
         interfaces = (graphene.relay.Node,)
         filter_fields = {
             "id": ["exact"],
             "type": ["exact", "icontains"],
             "title": ["exact", "icontains"],
             "date": ["exact", "lt", "lte", "gt", "gte"],
             "filename": ["exact", "icontains"],
             "mime": ["exact", "icontains"],
+            "general_type": ["exact", "icontains"],
             "url": ["exact", "icontains"],
             **prefix_filterset("claim__", ClaimGQLType._meta.filter_fields),
         }
         connection_class = ExtendedConnection
 
     @classmethod
     def get_queryset(cls, queryset, info):
         queryset = queryset.filter(*filter_validity())
         return queryset
 
 
+class ClaimAttachmentTypeGQLType(DjangoObjectType):
+    class Meta:
+        model = ClaimAttachmentType
+        interfaces = (graphene.relay.Node,)
+        filter_fields = {
+            "id": ["exact"],
+            "claim_general_type": ["exact"]
+        }
+        connection_class = ExtendedConnection
+
+
 class FeedbackGQLType(DjangoObjectType):
     class Meta:
         model = Feedback
 
 
 class ClaimItemGQLType(DjangoObjectType):
     """
@@ -169,7 +186,23 @@
 class ClaimServiceGQLType(DjangoObjectType):
     """
     Contains the services within a specific Claim
     """
 
     class Meta:
         model = ClaimService
+
+class ClaimServiceServiceGQLType(DjangoObjectType):
+    """
+    Contains the Claim services within a specific Claim
+    """
+
+    class Meta:
+        model = ClaimServiceService
+
+class ClaimServiceItemGQLType(DjangoObjectType):
+    """
+    Contains the Claim services within a specific Claim
+    """
+
+    class Meta:
+        model = ClaimServiceItem
```

### Comparing `openimis-be-claim-1.6.0/claim/management/commands/generateclaimadmins.py` & `openimis_be_claim-1.7.0/claim/management/commands/generateclaimadmins.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,14 +40,15 @@
                 "code": ''.join(random.choices(string.ascii_uppercase + string.digits, k=8)),
                 "last_name": fake.last_name(),
                 "other_names": fake.first_name(),
                 "email_id": fake.ascii_email(),
                 "phone": "+" + fake.msisdn(),
                 "health_facility_id": hf})
             if verbose:
-                print(admin_num, "created claim admin", claim_admin, "for HF", hf, "with code", claim_admin.code)
+                logger.debug(f"{admin_num} created claim admin {claim_admin} for HF {hf} \
+                    with code {claim_admin.code}")
 
     def get_random_hf(self):
         if not self.hfs:
             from location.models import HealthFacility
             self.hfs = HealthFacility.objects.filter(validity_to__isnull=True).values_list("pk", flat=True)
         return random.choice(self.hfs)
```

### Comparing `openimis-be-claim-1.6.0/claim/management/commands/generateclaims.py` & `openimis_be_claim-1.7.0/claim/management/commands/generateclaims.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,34 +38,34 @@
             claim_admin = self.get_random_claim_admin()
             hf = self.get_random_hf()
             claim = create_test_claim({"insuree_id": insuree,
                                        "code": ''.join(random.choices(string.ascii_uppercase + string.digits, k=8)),
                                        "admin_id": claim_admin,
                                        "health_facility_id": hf})
             if verbose:
-                print(claim_num, "created claim", claim, "for insuree", insuree, "with code", claim.code)
+                logger.debug(f"{claim_num} created claim {claim} for insuree {insuree} with code {claim.code}")
             for svc_num in range(1, nb_services + 1):
                 service = self.get_random_service()
                 claim_service = create_test_claimservice(claim, custom_props={
                     "service_id": service,
                     "qty_provided": random.randint(1, 10),
                     "price_asked": random.randint(1, 1000),
                 })
                 if verbose:
-                    print(claim_num, svc_num, "Created claim service", claim_service, "for service", service)
+                    logger.debug(f"{claim_num} {svc_num} Created claim service {claim_service} for service {service}")
             for item_num in range(1, nb_items + 1):
                 item = self.get_random_item()
                 claim_item = create_test_claimitem(claim, "D", custom_props=
                 {
                     "item_id": item,
                     "qty_provided": random.randint(1, 10),
                     "price_asked": random.randint(1, 1000),
                 })
                 if verbose:
-                    print(claim_num, item_num, "Created claim item", claim_item, "for item", item)
+                    logger.debug(f"{claim_num} {item_num} Created claim item {claim_item} for item {item}")
 
     def get_random_insuree(self):
         if not self.insurees:
             self.insurees = Insuree.objects.filter(validity_to__isnull=True).values_list("pk", flat=True)
         return random.choice(self.insurees)
 
     def get_random_service(self):
```

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0001_initial.py` & `openimis_be_claim-1.7.0/claim/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0002_batchrun.py` & `openimis_be_claim-1.7.0/claim/migrations/0002_batchrun.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0003_claimofficer.py` & `openimis_be_claim-1.7.0/claim/migrations/0003_claimofficer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0004_claimattachment.py` & `openimis_be_claim-1.7.0/claim/migrations/0004_claimattachment.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0005_claimmutation.py` & `openimis_be_claim-1.7.0/claim/migrations/0005_claimmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0009_auto_20200421_1657.py` & `openimis_be_claim-1.7.0/claim/migrations/0009_auto_20200421_1657.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0010_auto_20200611_0601.py` & `openimis_be_claim-1.7.0/claim/migrations/0010_auto_20200611_0601.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0012_item_service_jsonExtField.py` & `openimis_be_claim-1.7.0/claim/migrations/0012_item_service_jsonExtField.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0013_feedbackprompt.py` & `openimis_be_claim-1.7.0/claim/migrations/0013_feedbackprompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     operations = [
         migrations.CreateModel(
             name='FeedbackPrompt',
             fields=[
                 ('id', models.AutoField(db_column='FeedbackPromptID', primary_key=True, serialize=False)),
                 ('feedback_prompt_date', core.fields.DateField(blank=True, db_column='FeedbackPromptDate', null=True)),
                 ('officer_id', models.IntegerField(blank=True, db_column='OfficerID', null=True)),
-                ('phone_number', models.CharField(db_column='PhoneNumber', max_length=36, unique=True)),
+                ('phone_number', models.CharField(db_column='PhoneNumber', max_length=36, null=True, blank=True)),
                 ('sms_status', models.IntegerField(blank=True, db_column='SMSStatus', null=True)),
                 ('validity_from', core.fields.DateTimeField(blank=True, db_column='ValidityFrom', null=True)),
                 ('validity_to', core.fields.DateTimeField(blank=True, db_column='ValidityTo', null=True)),
                 ('legacy_id', models.IntegerField(blank=True, db_column='LegacyID', null=True)),
                 ('audit_user_id', models.IntegerField(blank=True, db_column='AuditUserID', null=True)),
             ],
             options={
```

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0015_prohibit_interaction_for_enrolment_officer.py` & `openimis_be_claim-1.7.0/claim/migrations/0015_prohibit_interaction_for_enrolment_officer.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,35 +3,36 @@
 from django.db import migrations
 from core.models import RoleRight, Role
 
 
 def forwards_func(apps, schema_editor):
     # Delete enrollment officer right to interact with claim data
     # Enrollment officer is predefined system role with id 1
-    eo_role = Role.objects.filter(is_system=1, validity_to__isnull=True).get()
+    eo_roles = Role.objects.filter(is_system=1, validity_to__isnull=True)
     # Prohibited Roles ID are gql_query_claims_perms (111001)
     # and gql_mutation_deliver_claim_feedback_perms (111009)
     rights_id = [111001, 111009]
     for right_id in rights_id:
         RoleRight.objects.filter(
-            role_id=eo_role.id,
+            role__in=eo_roles,
             right_id=right_id,
             validity_to__isnull=True
         ).delete()
 
 
 def reverse_func(apps, schema_editor):
-    eo_role = Role.objects.filter(is_system=1, validity_to__isnull=True).get()
+    eo_roles = Role.objects.filter(is_system=1, validity_to__isnull=True)
     rights_id = [111001, 111009]
-    for right_id in rights_id:
-        RoleRight(
-            role_id=eo_role.id,
-            right_id=right_id,
-            audit_user_id=None,
-        ).save()
+    for eo_role in v:
+        for right_id in rights_id:
+            RoleRight(
+                role_id=eo_role.id,
+                right_id=right_id,
+                audit_user_id=None,
+            ).save()
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ("claim", "0014_change_code_limit"),
     ]
```

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0016_update_django_scheme_with_missing_fields.py` & `openimis_be_claim-1.7.0/claim/migrations/0016_update_django_scheme_with_missing_fields.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0017_set_managed_to_true.py` & `openimis_be_claim-1.7.0/claim/migrations/0017_set_managed_to_true.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0018_alter_jsonext_column.py` & `openimis_be_claim-1.7.0/claim/migrations/0018_alter_jsonext_column.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0019_auto_20230615_1055.py` & `openimis_be_claim-1.7.0/claim/migrations/0019_auto_20230615_1055.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 # Generated by Django 3.2.16 on 2023-06-15 10:55
 
 from django.db import migrations, models
 import django.db.models.deletion
+from claim.models import Claim
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('location', '0015_set_managed_to_true'),
         ('claim', '0018_alter_jsonext_column'),
     ]
 
-    operations = [
-        migrations.AddField(
+    operations = []
+    try:
+        Claim.objects.filter(pk__lt=10).aggregate(sum=models.Count('refer_from'))
+    except:
+        operations.append(migrations.AddField(
             model_name='claim',
             name='refer_from',
             field=models.ForeignKey(blank=True, db_column='ReferFrom', null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name='referFromHF', to='location.healthfacility'),
-        ),
-        migrations.AddField(
+        ))
+    try:
+        Claim.objects.filter(pk__lt=10).aggregate(sum=models.Count('refer_to'))
+    except:    
+        operations.append(migrations.AddField(
             model_name='claim',
             name='refer_to',
             field=models.ForeignKey(blank=True, db_column='ReferTo', null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name='referToHF', to='location.healthfacility'),
-        ),
-    ]
+        ))
+
```

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0023_claim_restore.py` & `openimis_be_claim-1.7.0/claim/migrations/0023_claim_restore.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0024_add_claim_restore_perms.py` & `openimis_be_claim-1.7.0/claim/migrations/0024_add_claim_restore_perms.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0025_auto_20231205_1455.py` & `openimis_be_claim-1.7.0/claim/migrations/0025_auto_20231205_1455.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/migrations/0026_add_sequences.py` & `openimis_be_claim-1.7.0/claim/migrations/0026_add_sequences.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/models.py` & `openimis_be_claim-1.7.0/claim/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 from core import models as core_models
 from django import dispatch
 from django.conf import settings
 from django.db import models
 from graphql import ResolveInfo
 from insuree import models as insuree_models
 from location import models as location_models
-from location.models import  LocationManager
+from location.models import LocationManager
 from medical import models as medical_models
 from policy import models as policy_models
 from product import models as product_models
 from django.apps import apps
+from django.utils import timezone as django_tz
 
 core_config = apps.get_app_config('core')
 
 
 class ClaimAdmin(core_models.VersionedModel):
     id = models.AutoField(db_column='ClaimAdminId', primary_key=True)
     uuid = models.CharField(db_column='ClaimAdminUUID', max_length=36, default=uuid.uuid4, unique=True)
 
-    code = models.CharField(db_column='ClaimAdminCode', max_length=core_config.user_username_and_code_length_limit,
+    code = models.CharField(db_column='ClaimAdminCode', max_length=50,
                             blank=True, null=True)
     last_name = models.CharField(db_column='LastName', max_length=100, blank=True, null=True)
     other_names = models.CharField(db_column='OtherNames', max_length=100, blank=True, null=True)
     dob = models.DateField(db_column='DOB', blank=True, null=True)
     email_id = models.CharField(db_column='EmailId', max_length=200, blank=True, null=True)
     phone = models.CharField(db_column='Phone', max_length=50, blank=True, null=True)
     health_facility = models.ForeignKey(
@@ -44,16 +45,17 @@
         queryset = cls.filter_queryset(queryset)
         # GraphQL calls with an info object while Rest calls with the user itself
         if isinstance(user, ResolveInfo):
             user = user.context.user
         if settings.ROW_SECURITY and user.is_anonymous:
             return queryset.filter(id=-1)
         if settings.ROW_SECURITY:
-            from location.schema import  LocationManager
-            queryset =  LocationManager().build_user_location_filter_query( user._u, prefix='health_facility__location', queryset=queryset, loc_types = ['D'])    
+            from location.schema import LocationManager
+            queryset = LocationManager().build_user_location_filter_query(
+                user._u, prefix='health_facility__location', queryset=queryset, loc_types=['D'])
         return queryset
 
     @property
     def id_for_audit(self):
         return self.audit_user_id
 
     @property
@@ -122,20 +124,21 @@
         queryset = cls.filter_queryset(queryset)
         # GraphQL calls with an info object while Rest calls with the user itself
         if isinstance(user, ResolveInfo):
             user = user.context.user
         if settings.ROW_SECURITY and user.is_anonymous:
             return queryset.filter(id=-1)
         if settings.ROW_SECURITY:
-            queryset =  LocationManager().build_user_location_filter_query( user._u, prefix='health_facility__location', queryset=queryset, loc_types=['D'])    
+            queryset = LocationManager().build_user_location_filter_query(
+                user._u, prefix='health_facility__location', queryset=queryset, loc_types=['D'])
         return queryset
 
 
 
-signal_claim_rejection = dispatch.Signal(providing_args=["claim"])
+signal_claim_rejection = dispatch.Signal(["claim"])
 
 
 class Claim(core_models.VersionedModel, core_models.ExtendableModel):
     id = models.AutoField(db_column='ClaimID', primary_key=True)
     uuid = models.CharField(db_column='ClaimUUID',
                             max_length=36, default=uuid.uuid4, unique=True)
     category = models.CharField(
@@ -296,30 +299,32 @@
         if isinstance(user, ResolveInfo):
             user = user.context.user
         if settings.ROW_SECURITY and user.is_anonymous:
             return queryset.filter(id=-1)
         if settings.ROW_SECURITY:
             # TechnicalUsers don't have health_facility_id attribute
             if hasattr(user._u, 'health_facility_id') and user._u.health_facility_id:
-                queryset =  queryset.filter(
+                queryset = queryset.filter(
                     health_facility_id=user._u.health_facility_id
                 )
             else:
                 if not isinstance(user._u, core_models.TechnicalUser):
-                    queryset = LocationManager().build_user_location_filter_query( user._u, prefix='health_facility__location', queryset = queryset, loc_types=['D'])
+                    queryset = LocationManager().build_user_location_filter_query(
+                        user._u, prefix='health_facility__location', queryset=queryset, loc_types=['D'])
         return queryset
-      
+
+
 class FeedbackPrompt(core_models.VersionedModel):
     id = models.AutoField(db_column='FeedbackPromptID', primary_key=True)
     feedback_prompt_date = fields.DateField(db_column='FeedbackPromptDate', blank=True, null=True)
     claim = models.ForeignKey(
-        Claim, models.DO_NOTHING, db_column='ClaimID', blank=True, null=True, related_name="+")   
+        Claim, models.DO_NOTHING, db_column='ClaimID', blank=True, null=True, related_name="+")
     officer = models.ForeignKey(
-        core_models.Officer , models.DO_NOTHING, db_column="OfficerID", blank=True, null=True)
-    phone_number = models.CharField(db_column='PhoneNumber', max_length=50)
+        core_models.Officer, models.DO_NOTHING, db_column="OfficerID", blank=True, null=True)
+    phone_number = models.CharField(db_column='PhoneNumber', max_length=50, blank=True, null=True)
     sms_status = models.IntegerField(db_column='SMSStatus', blank=True, null=True)
     validity_from = fields.DateTimeField(db_column='ValidityFrom', blank=True, null=True)
     validity_to = fields.DateTimeField(db_column='ValidityTo', blank=True, null=True)
     legacy_id = models.IntegerField(db_column='LegacyID', blank=True, null=True)
     audit_user_id = models.IntegerField(db_column='AuditUserID', blank=True, null=True)
 
     class Meta:
@@ -331,15 +336,16 @@
         queryset = cls.filter_queryset(queryset)
         # GraphQL calls with an info object while Rest calls with the user itself
         if isinstance(user, ResolveInfo):
             user = user.context.user
         if settings.ROW_SECURITY and user.is_anonymous:
             return queryset.filter(id=-1)
         if settings.ROW_SECURITY:
-            queryset =  LocationManager().build_user_location_filter_query( user._u, prefix='health_facility__location', queryset=queryset, loc_types=['D'])    
+            queryset = LocationManager().build_user_location_filter_query(
+                user._u, prefix='health_facility__location', queryset=queryset, loc_types=['D'])
 
         return queryset
 
 
 
 class ClaimAttachmentsCount(models.Model):
     claim = models.OneToOneField(Claim, primary_key=True, related_name='attachments_count', on_delete=models.DO_NOTHING)
@@ -447,22 +453,46 @@
     objects = ClaimDetailManager()
 
     class Meta:
         managed = True
         db_table = 'tblClaimItems'
 
 
+class GeneralClaimAttachmentType(models.TextChoices):
+    URL = "URL"
+    FILE = "FILE"
+
+
+class ClaimAttachmentType(core_models.VersionedModel):
+    id = models.SmallIntegerField(db_column='ClaimAttachmentTypeId', primary_key=True)
+    claim_attachment_type = models.CharField(db_column='ClaimAttachmentType', max_length=50)
+    is_autogenerated = models.BooleanField(default=False)
+    claim_general_type = models.CharField(max_length=10, default=GeneralClaimAttachmentType.FILE,
+                                          choices=GeneralClaimAttachmentType.choices)
+
+    class Meta:
+        managed = True
+        db_table = 'claim_ClaimAttachment_ClaimAttachmentType'
+
+
 class ClaimAttachment(core_models.UUIDModel, core_models.UUIDVersionedModel):
     claim = models.ForeignKey(
         Claim, models.DO_NOTHING, related_name='attachments')
+    general_type = models.CharField(max_length=4, choices=GeneralClaimAttachmentType.choices,
+                                    default=GeneralClaimAttachmentType.FILE)
     type = models.TextField(blank=True, null=True)
+    predefined_type = models.ForeignKey(ClaimAttachmentType, models.DO_NOTHING, related_name='type_dropdown', null=True,
+                                        blank=True)
     title = models.TextField(blank=True, null=True)
     date = fields.DateField(blank=True, default=TimeUtils.now)
     filename = models.TextField(blank=True, null=True)
     mime = models.TextField(blank=True, null=True)
+    # this is not needed at the moment, but we want to move attachment to core
+    # in that case module information is needed, and we want to avoid writing additional migration
+    module = models.TextField(blank=False, null=True)
     # frontend contributions may lead to externalized (nas) storage for documents
     url = models.TextField(blank=True, null=True)
     # Support of BinaryField is database-related: prefer to stick to b64-encoded
     document = models.TextField(blank=True, null=True)
 
     class Meta:
         managed = True
@@ -518,21 +548,56 @@
         db_column='DeductableAmount', max_digits=18, decimal_places=2, blank=True, null=True)
     exceed_ceiling_amount = models.DecimalField(
         db_column='ExceedCeilingAmount', max_digits=18, decimal_places=2, blank=True, null=True)
     price_origin = models.CharField(
         db_column='PriceOrigin', max_length=1, blank=True, null=True)
     exceed_ceiling_amount_category = models.DecimalField(
         db_column='ExceedCeilingAmountCategory', max_digits=18, decimal_places=2, blank=True, null=True)
-
     objects = ClaimDetailManager()
 
     class Meta:
         managed = True
         db_table = 'tblClaimServices'
 
+class ClaimServiceItem(models.Model):
+    id = models.AutoField(primary_key=True, db_column='idCsi')
+    item = models.ForeignKey(medical_models.Item, models.DO_NOTHING, db_column='ItemID', related_name="service_items")                           
+    claim_service = models.ForeignKey( ClaimService,
+                                          models.DO_NOTHING, db_column="ClaimServiceID",related_name='items')
+    qty_provided = models.IntegerField(db_column="qty_provided",
+                                      blank=True, null=True)
+    qty_displayed = models.IntegerField(db_column="qty_displayed",
+                                      blank=True, null=True)
+    created_date = models.DateTimeField(db_column="created_date", default=django_tz.now,
+                                   blank=True, null=True)
+    price_asked = models.DecimalField(db_column="price",
+                                   max_digits=18, decimal_places=2, blank=True, null=True)
+                                   
+    class Meta:
+        managed = True
+        db_table = 'tblClaimServicesItems'
+
+class ClaimServiceService(models.Model):
+    id = models.AutoField(primary_key=True, db_column='idCss')
+    service = models.ForeignKey(medical_models.Service, models.DO_NOTHING,
+                              db_column='ServiceId', related_name='service_services')
+    claim_service = models.ForeignKey( ClaimService,
+                                          models.DO_NOTHING, db_column="claimServiceID", related_name='services')
+    qty_provided = models.IntegerField(db_column="qty_provided",
+                                      blank=True, null=True)
+    qty_displayed = models.IntegerField(db_column="qty_displayed",
+                                      blank=True, null=True)
+    created_date = models.DateTimeField(db_column="created_date", default=django_tz.now,
+                                   blank=True, null=True)
+    price_asked = models.DecimalField(db_column="price",
+                                   max_digits=18, decimal_places=2, blank=True, null=True)
+    
+    class Meta:
+        managed = True
+        db_table = 'tblClaimServicesService'
 
 class ClaimDedRem(core_models.VersionedModel):
     id = models.AutoField(db_column='ExpenditureID', primary_key=True)
 
     policy = models.ForeignKey('policy.Policy', models.DO_NOTHING, db_column='PolicyID', blank=True, null=True,
                                related_name='claim_ded_rems')
     insuree = models.ForeignKey('insuree.Insuree', models.DO_NOTHING, db_column='InsureeID', blank=True, null=True,
```

### Comparing `openimis-be-claim-1.6.0/claim/report.py` & `openimis_be_claim-1.7.0/claim/report.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/reports/claim.py` & `openimis_be_claim-1.7.0/claim/reports/claim.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/reports/claim_history.py` & `openimis_be_claim-1.7.0/claim/reports/claim_history.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.6.0/claim/reports/claim_percentage_referrals.py` & `openimis_be_claim-1.7.0/claim/reports/claim_percentage_referrals.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-from claim.models import Claim
 from django.db import connection
-from django.db.models import Q, F, Count
-from django.db.models.functions import Coalesce
-from location.models import HealthFacility, Location
 from tools.utils import dictfetchall
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 template = """
@@ -395,17 +391,17 @@
                     "pageBreak": false,
                     "repeatGroupHeader": false,
                     "columnData": [
                         {
                             "elementType": "table_text",
                             "id": 277,
                             "width": 304,
-                            "content": "${HF}",
+                            "content": "${hf}",
                             "eval": false,
-                            "colspan": "",  
+                            "colspan": "",
                             "styleId": "",
                             "bold": false,
                             "italic": false,
                             "underline": false,
                             "strikethrough": false,
                             "horizontalAlignment": "left",
                             "verticalAlignment": "middle",
@@ -441,15 +437,15 @@
                             "borderWidth": 1,
                             "growWeight": 0
                         },
                         {
                             "elementType": "table_text",
                             "id": 278,
                             "width": 90,
-                            "content": "${TotalClaims}",
+                            "content": "${totalclaims}",
                             "eval": false,
                             "colspan": "",
                             "styleId": "",
                             "bold": false,
                             "italic": false,
                             "underline": false,
                             "strikethrough": false,
@@ -487,15 +483,15 @@
                             "borderWidth": 1,
                             "growWeight": 0
                         },
                         {
                             "elementType": "table_text",
                             "id": 283,
                             "width": 90,
-                            "content": "${TotalOP}",
+                            "content": "${totalop}",
                             "eval": false,
                             "colspan": "",
                             "styleId": "",
                             "bold": false,
                             "italic": false,
                             "underline": false,
                             "strikethrough": false,
@@ -533,15 +529,15 @@
                             "borderWidth": 1,
                             "growWeight": 0
                         },
                         {
                             "elementType": "table_text",
                             "id": 286,
                             "width": 90,
-                        "content": "${TotalIP}",
+                            "content": "${totalip}",
                             "eval": false,
                             "colspan": "",
                             "styleId": "",
                             "bold": false,
                             "italic": false,
                             "underline": false,
                             "strikethrough": false,
@@ -977,51 +973,51 @@
                     "pattern": "",
                     "expression": "",
                     "showOnlyNameType": true,
                     "testData": ""
                 },
                 {
                     "id": 235,
-                    "name": "HF",
+                    "name": "hf",
                     "type": "string",
                     "arrayItemType": "string",
                     "eval": false,
                     "nullable": false,
                     "pattern": "",
                     "expression": "",
                     "showOnlyNameType": false,
                     "testData": ""
                 },
                 {
                     "id": 236,
-                    "name": "TotalClaims",
+                    "name": "totalclaims",
                     "type": "number",
                     "arrayItemType": "string",
                     "eval": false,
                     "nullable": true,
                     "pattern": "#,##0",
                     "expression": "",
                     "showOnlyNameType": false,
                     "testData": ""
                 },
                 {
                     "id": 262,
-                    "name": "TotalOP",
+                    "name": "totalop",
                     "type": "number",
                     "arrayItemType": "string",
                     "eval": false,
                     "nullable": true,
                     "pattern": "#,##0",
                     "expression": "",
                     "showOnlyNameType": false,
                     "testData": ""
                 },
                 {
                     "id": 271,
-                    "name": "TotalIP",
+                    "name": "totalip",
                     "type": "number",
                     "arrayItemType": "string",
                     "eval": false,
                     "nullable": true,
                     "pattern": "#,##0",
                     "expression": "",
                     "showOnlyNameType": false,
@@ -1130,61 +1126,77 @@
         "footerDisplay": "always",
         "patternLocale": "en",
         "patternCurrencySymbol": "$"
     }
 }
 """
 
-
-def claim_percentage_referrals_query(user, region_id=0, district_id=0, date_start="2019-01-01", date_end="2022-12-31", **kwargs):
-    result_set = []
-
-    try:
-        health_facilities = HealthFacility.objects.filter(
-            validity_to__isnull=True,
-            level__in=['D', 'C'],
-            location__id=district_id
-        )
-
-        for hf in health_facilities:
-            total_claims = Claim.objects.filter(
-                health_facility=hf,
-                validity_to__isnull=True,
-                date_claimed__range=[date_start, date_end]
-            ).count()
-
-            total_op = Claim.objects.filter(
-                Q(date_to__isnull=True) | Q(date_to=F("date_from")),
-                health_facility=hf,
-                validity_to__isnull=True,
-                visit_type="R",
-                date_claimed__range=[date_start, date_end]
-            ).count()
-
-            total_ip = Claim.objects.filter(
-                ~Q(date_from=F("date_to")),
-                health_facility=hf,
-                validity_to__isnull=True,
-                visit_type="R",
-                date_claimed__range=[date_start, date_end]
-            ).count()
-
+# TODO transform the SQL query into a Django ORM query
+percentage_referrals_sql = """
+SELECT CONCAT(HF."HFCode", ' - ', HF."HFName") HF, TotalClaim.TotalClaims, RefOP.TotalOP, RefIP.TotalIP
+FROM (SELECT HF."HfID", HF."HFCode", HF."HFName"
+      FROM "tblHF" HF
+               INNER JOIN "uvwLocations" L ON L."LocationId" = HF."LocationId"
+      WHERE HF."ValidityTo" Is NULL
+        AND HF."HFLevel" IN ('D', 'C')
+        AND (L."RegionId" = %(region_id)s OR %(region_id)s = 0 OR L."LocationId" IS NULL)
+        AND (L."DistrictId" = %(district_id)s OR %(district_id)s = 0 OR L."DistrictId" IS NULL)
+      ) HF
+         LEFT OUTER JOIN (SELECT COUNT(1) TotalClaims, "HFID"
+                          FROM "tblClaim"
+                          WHERE "ValidityTo" Is NULL
+                          AND "DateClaimed" BETWEEN %(date_start)s AND %(date_end)s
+                          GROUP BY "HFID") TotalClaim ON HF."HfID" = TotalClaim."HFID"
+         LEFT OUTER JOIN (SELECT I."HFID", COUNT(C."ClaimID") TotalOP
+                          FROM "tblClaim" C
+                                   INNER JOIN "tblInsuree" I ON C."InsureeID" = I."InsureeID"
+                                   INNER JOIN "tblHF" HF ON C."HFID" = HF."HfID"
+                                   INNER JOIN "uvwLocations" L ON L."LocationId" = HF."LocationId"
+                          WHERE C."ValidityTo" Is NULL
+                            AND I."ValidityTo" IS NULL
+                            AND HF."ValidityTo" IS NULL
+                            AND (C."DateTo" is null OR C."DateFrom" = C."DateTo")
+                            AND HF."HfID" <> I."HFID"
+                            AND C."VisitType" = N'R'
+                            AND (L."RegionId" = %(region_id)s OR %(region_id)s = 0 OR L."LocationId" IS NULL)
+                            AND (L."DistrictId" = %(district_id)s OR %(district_id)s = 0 OR L."DistrictId" IS NULL)
+                            AND C."DateClaimed" BETWEEN %(date_start)s AND %(date_end)s
+                          GROUP BY I."HFID") RefOP ON HF."HfID" = RefOP."HFID"
+         LEFT OUTER JOIN (SELECT I."HFID", COUNT(C."ClaimID") TotalIP
+                          FROM "tblClaim" C
+                                   INNER JOIN "tblInsuree" I ON C."InsureeID" = I."InsureeID"
+                                   INNER JOIN "tblHF" HF ON C."HFID" = HF."HfID"
+                                   INNER JOIN "uvwLocations" L ON L."LocationId" = HF."LocationId"
+                          WHERE C."ValidityTo" Is NULL
+                            AND I."ValidityTo" IS NULL
+                            AND HF."ValidityTo" IS NULL
+                            AND C."DateTo" is not null and C."DateFrom" <> C."DateTo"
+                            AND HF."HfID" <> I."HFID"
+                            AND C."VisitType" = N'R'
+                            AND (L."RegionId" = %(region_id)s OR %(region_id)s = 0 OR L."LocationId" IS NULL)
+                            AND (L."DistrictId" = %(district_id)s OR %(district_id)s = 0 OR L."DistrictId" IS NULL)
+                            AND C."DateClaimed" BETWEEN %(date_start)s AND %(date_end)s
+                          GROUP BY I."HFID") RefIP ON HF."HfID" = RefIP."HFID"
+"""
 
 
-            result_set.append(
+def claim_percentage_referrals_query(user, region_id=0, district_id=0, date_start="2019-01-01", date_end="2022-12-31",
+                                     **kwargs):
+    with connection.cursor() as cur:
+        try:
+            cur.execute(
+                percentage_referrals_sql,
                 {
-                    "HF": f"{hf.code} - {hf.name}",
-                    "TotalClaims": total_claims,
-                    "TotalOP": total_op,
-                    "TotalIP": total_ip
-                }
+                    "region_id": region_id,
+                    "district_id": district_id,
+                    "date_start": date_start,
+                    "date_end": date_end,
+                },
             )
-
-
-        return {"data": result_set}
-
-    except Exception as e:
-        logger.exception("Error fetching claim percentage referrals query")
-        raise e
+            data = dictfetchall(cur)
+            return {"data": data}
+        except Exception as e:
+            logger.exception("Error fetching claim percentage referrals query")
+            raise e
 
     logger.error("Claim percentage referrals query arrived at end of function")
     return {"data": None}
```

### Comparing `openimis-be-claim-1.6.0/claim/reports/claims_overview.py` & `openimis_be_claim-1.7.0/claim/reports/claims_overview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from _decimal import Decimal
 from typing import Dict, Union
 
-from django.db.models import Q
+from django.db.models import Q, Prefetch
 
+from core.utils import filter_validity
 from location.models import Location, HealthFacility
 from product.models import Product
 from claim.models import Claim, ClaimItem, ClaimService
 
 import logging
 
 logger = logging.getLogger(__name__)
@@ -7541,18 +7542,18 @@
     # If this report has to be generated with an MSSQL database, this part will need to be changed.
     # An easy way would be to make a set of claim codes - during the for loop, check if the code is in the set:
     # if it's not in the set -> process the claim and add its code to the set
     # if it's already in the set -> continue
     claim_queryset = Claim.objects.filter(claim_filters) \
                                   .distinct("date_claimed", "insuree__chf_id", "code") \
                                   .order_by("date_claimed", "insuree__chf_id", "code") \
-                                  .prefetch_related("items") \
+                                  .prefetch_related(Prefetch('items', queryset=ClaimItem.objects.filter(*filter_validity())))\
                                   .prefetch_related("items__item") \
                                   .prefetch_related("insuree") \
-                                  .prefetch_related("services") \
+                                  .prefetch_related(Prefetch('services', queryset=ClaimService.objects.filter(*filter_validity())))\
                                   .prefetch_related("services__service") \
                                   .prefetch_related("admin")
 
     total_claimed = Decimal(0.0)
     total_approved = Decimal(0.0)
     total_adjusted = Decimal(0.0)
     total_paid = Decimal(0.0)
```

### Comparing `openimis-be-claim-1.6.0/claim/reports/claims_primary_operational_indicators.py` & `openimis_be_claim-1.7.0/claim/reports/claims_primary_operational_indicators.py`

 * *Files 0% similar despite different names*

```diff
@@ -4961,15 +4961,15 @@
         "headerDisplay": "always",
         "footer": true,
         "footerSize": "30",
         "footerDisplay": "always",
         "patternLocale": "en",
         "patternCurrencySymbol": "$"
     }
-}7
+}
 """
 
 CATEGORY_TOTAL = "T"
 CATEGORY_PAID = "P"
 CATEGORY_REJECTED = "R"
 
 NO_DATA_CODE = "????????"
```

### Comparing `openimis-be-claim-1.6.0/claim/schema.py` & `openimis_be_claim-1.7.0/claim/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,18 +31,20 @@
         orderBy=graphene.List(of_type=graphene.String),
         items=graphene.List(of_type=graphene.String),
         services=graphene.List(of_type=graphene.String),
         json_ext=graphene.JSONString(),
         attachment_status=graphene.Int(required=False),
         care_type=graphene.String(required=False),
         show_restored=graphene.Boolean(required=False)
-    )
+        )
 
     claim = graphene.Field(
-        ClaimGQLType, id=graphene.Int(), uuid=graphene.UUID()
+        ClaimGQLType, 
+        id=graphene.Int(), 
+        uuid=graphene.UUID()
     )
 
     claim_attachments = DjangoFilterConnectionField(
         ClaimAttachmentGQLType
     )
     claim_admins = DjangoFilterConnectionField(
         ClaimAdminGQLType,
@@ -59,22 +61,32 @@
     )
 
     validate_claim_code = graphene.Field(
         graphene.Boolean,
         claim_code=graphene.String(required=True),
         description="Checks that the specified claim code is unique."
     )
+    fsp_from_claim = graphene.Field(
+        HealthFacilityGQLType,
+        insuree_code=graphene.String(required=True),
+        date_claimed=graphene.Date(required=True),
+        description="Return FSP of insuree during creation of the claim."
+    )
 
     claim_with_same_diagnosis = OrderedDjangoFilterConnectionField(
         ClaimGQLType,
         icd=graphene.String(required=True),
         chfid=graphene.String(required=True),
         description="Return last claim (date claimed) with identical diagnosis for given insuree."
     )
 
+    claim_attachment_type = DjangoFilterConnectionField(
+        ClaimAttachmentTypeGQLType
+    )
+
     def resolve_insuree_name_by_chfid(self, info, **kwargs):
         if not info.context.user.has_perms(ClaimConfig.gql_mutation_create_claims_perms)\
                 and not info.context.user.has_perms(ClaimConfig.gql_mutation_update_claims_perms):
             raise PermissionDenied(_("unauthorized"))
         chf_id = kwargs.get('chfId')
         insuree = Insuree.objects\
             .filter(validity_to__isnull=True, chf_id=chf_id)\
@@ -101,60 +113,55 @@
 
         if id is not None:
             return Claim.objects.get(id=id)
         if uuid is not None:
             return Claim.objects.get(uuid=uuid)
 
     def resolve_claims(self, info, **kwargs):
+        class AttachmentStatusEnum(Enum):
+            NONE = 0
+            WITH = 1
+            WITHOUT = 2
         if (
             not info.context.user.has_perms(ClaimConfig.gql_query_claims_perms)
             and settings.ROW_SECURITY
         ):
             raise PermissionDenied(_("unauthorized"))
-        query = Claim.objects.all()
-        code_is_not = kwargs.get("code_is_not", None)
-        if code_is_not:
-            query = query.exclude(code=code_is_not)
-        variance = kwargs.get("diagnosisVariance", None)
+        query = Claim.objects
+        filters = []
 
         show_restored = kwargs.get("show_restored", None)
         if show_restored:
-            query = query.filter(restore__isnull=False)
+            filters.append(Q(restore__isnull=False))
 
         items = kwargs.get("items", None)
         services = kwargs.get("services", None)
 
         if items:
-            query = query.filter(items__item__code__in=items)
+            filters.append(Q(items__item__code__in=items))
 
         if services:
-            query = query.filter(services__service__code__in=services)
+            filters.append(Q(services__service__code__in=services))
 
         attachment_status = kwargs.get("attachment_status", 0)
-
-        class AttachmentStatusEnum(Enum):
-            NONE = 0
-            WITH = 1
-            WITHOUT = 2
-
         if attachment_status == AttachmentStatusEnum.WITH.value:
-            query = query.filter(attachments__isnull=False)
+            filters.append(Q(attachments__isnull=False))
         elif attachment_status == AttachmentStatusEnum.WITHOUT.value:
-            query = query.filter(attachments__isnull=True)
+            filters.append(Q(attachments__isnull=True))
 
         care_type = kwargs.get("care_type", None)
 
         if care_type:
-            query = query.filter(care_type=care_type)
+            filters.append(Q(care_type=care_type))
 
         json_ext = kwargs.get("json_ext", None)
 
         if json_ext:
-            query = query.filter(json_ext__jsoncontains=json_ext)
-
+            filters.append(Q(json_ext__jsoncontains=json_ext))
+        variance = kwargs.get("diagnosisVariance", None)
         if variance:
             from core import datetime, datetimedelta
 
             last_year = datetime.date.today() + datetimedelta(years=-1)
             diag_avg = (
                 Claim.objects.filter(*filter_validity(**kwargs))
                 .filter(date_claimed__gt=last_year)
@@ -168,22 +175,30 @@
             if not ClaimConfig.gql_query_claim_diagnosis_variance_only_on_existing:
                 diags = (
                     Claim.objects.filter(*filter_validity(**kwargs))
                     .filter(date_claimed__gt=last_year)
                     .values("icd__code")
                     .distinct()
                 )
-                variance_filter = variance_filter | ~Q(icd__code__in=diags)
-            query = query.filter(variance_filter)
+                variance_filter = Q(variance_filter | ~Q(icd__code__in=diags))
+            filters.append(variance_filter)    
         #filtered already in get_queryser
         #query = query.filter(
         #            LocationManager().build_user_location_filter_query( info.context.user._u, prefix='health_facility__location') 
         #        )
-
-        return gql_optimizer.query(query.all(), info)
+        code_is_not = kwargs.get("code_is_not", None)
+        
+        if len(filters):
+            query = query.filter(*filters)   
+        if code_is_not:
+            query = query.exclude(code=code_is_not)
+        
+        if len(filters) == 0 and not code_is_not:
+            query = query.all()
+        return gql_optimizer.query(query, info)
 
     def resolve_claim_attachments(self, info, **kwargs):
         if not info.context.user.has_perms(ClaimConfig.gql_query_claims_perms):
             raise PermissionDenied(_("unauthorized"))
 
     def resolve_claim_admins(
             self,
@@ -231,14 +246,23 @@
             qs = qs.filter(
                 Q(code__icontains=search)
                 | Q(last_name__icontains=search)
                 | Q(other_names__icontains=search)
             )
         return qs
 
+    def resolve_fsp_from_claim(self, info, **kwargs):
+        if not info.context.user.has_perms(ClaimConfig.gql_query_claim_officers_perms):
+            raise PermissionDenied(_("unauthorized"))
+        result = Insuree.objects.filter(
+            chf_id=kwargs['insuree_code'],
+            *filter_validity(validity=kwargs['date_claimed']),
+        ).first().health_facility
+        return result
+
     def resolve_claim_with_same_diagnosis(self, info, **kwargs):
         if not info.context.user.has_perms(ClaimConfig.gql_query_claim_officers_perms):
             raise PermissionDenied(_("unauthorized"))
 
         qs = Claim.objects.filter(icd__code=kwargs['icd'], icd__validity_to__isnull=True,
                                   insuree__chf_id=kwargs['chfid'], insuree__validity_to__isnull=True,
                                   validity_to__isnull=True).order_by("date_claimed")
@@ -285,14 +309,15 @@
     elif kwargs.get('mutation_class', None) != 'CreateClaimMutation':
         return []
     if 'data' in kwargs and kwargs['data'].get('autogenerate'):
         try:
             mutation_client_id = kwargs.get('data')['client_mutation_id']
             mutation_log = MutationLog.objects.filter(client_mutation_id=mutation_client_id).first()
             mutation_log.client_mutation_label = kwargs['data']['client_mutation_label']
+            mutation_log.autogenerated_code = kwargs['data']['code']
             mutation_log.save()
             return []
         except KeyError as e:
             logger.error("Client Mutation ID not found in claim signal after mutation, error: ", e)
     return []
```

### Comparing `openimis-be-claim-1.6.0/claim/test_helpers.py` & `openimis_be_claim-1.7.0/claim/test_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,74 @@
 from claim.models import Claim, ClaimService, ClaimItem, ClaimDedRem, ClaimAdmin
 from claim.validations import get_claim_category, approved_amount
+from claim.services import claim_create, update_sum_claims
 from medical.test_helpers import get_item_of_type, get_service_of_category
 from uuid import uuid4
 
-def create_test_claim(custom_props={}):
+class DummyUser:
+    def __init__(self):
+      self.id_for_audit = 1  
+
+def create_test_claim(custom_props={}, user = DummyUser() ):
     from core import datetime
-    return Claim.objects.create(
-        **{
+    if 'insuree' not in custom_props and 'insuree_id' not in custom_props:
+        custom_props["insuree_id"]= 2
+
+    return claim_create(
+        {
             "health_facility_id": 18,
             "icd_id": 116,
             "date_from": datetime.datetime(2019, 6, 1),
             "date_claimed": datetime.datetime(2019, 6, 1),
             "date_to": datetime.datetime(2019, 6, 1),
-            "audit_user_id": 1,
-            "insuree_id": 2,
             "status": 2,
             "validity_from": datetime.datetime(2019, 6, 1),
+            "code":  str(uuid4()),
             **custom_props
-        }
+        }, user
     )
 
 
 def create_test_claimitem(claim, item_type, valid=True, custom_props={}):
-    return ClaimItem.objects.create(
+    item =  ClaimItem.objects.create(
         **{
             "claim": claim,
             "qty_provided": 7,
             "price_asked": 11,
             "item_id": get_item_of_type(item_type).id if item_type else 23,  # Atropine
             "status": 1,
             "availability": True,
             "validity_from": "2019-06-01",
             "validity_to": None if valid else "2019-06-01",
             "audit_user_id": -1,
             **custom_props
            }
     )
+    update_sum_claims(claim)
+    return item
+
 
 
 def create_test_claimservice(claim, category=None, valid=True, custom_props={}):
-    return ClaimService.objects.create(
+    service =  ClaimService.objects.create(
         **{
             "claim": claim,
             "qty_provided": 7,
             "price_asked": 11,
             "service_id": get_service_of_category(category).id if category else 23,  # Skin graft, no cat
             "status": 1,
             "validity_from": "2019-06-01",
             "validity_to": None if valid else "2019-06-01",
             "audit_user_id": -1,
             **custom_props
         }
-    )
+    )    
+    update_sum_claims(claim)
+    return service
+
 
 
 def mark_test_claim_as_processed(claim, status=Claim.STATUS_CHECKED, audit_user_id=-1):
     claim.approved = approved_amount(claim)
     claim.status = status
     claim.audit_user_id_submit = audit_user_id
     from core.utils import TimeUtils
```

### Comparing `openimis-be-claim-1.6.0/claim/tests/test_services.py` & `openimis_be_claim-1.7.0/claim/tests/tests_services.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,94 @@
 from django.test import TestCase
 from unittest import mock
-from location.test_helpers import create_test_location, create_test_health_facility, create_test_village
+from location.test_helpers import create_test_location, create_test_health_facility,create_test_village
 from insuree.test_helpers import create_test_insuree
-from claim.test_helpers import create_test_claim_admin
-from claim.models import Claim, ClaimItem, ClaimService, ClaimDetail
-from medical.models import Diagnosis, Item, Service
+from claim.test_helpers import create_test_claim_admin, create_test_claim
+from claim.models import Claim, ClaimItem, ClaimService,ClaimDetail
+from medical.models import  Diagnosis, Item, Service
 from medical.test_helpers import create_test_item, create_test_service
 
 from core.services import create_or_update_interactive_user, create_or_update_core_user
 import datetime
 from claim.services import *
 import core
-
+from medical.test_helpers import create_test_service, create_test_item
+from claim.utils import service_create_hook, calcul_amount_service, service_update_hook
+from claim.test_helpers import create_test_claim
+from claim.models import ClaimServiceItem, ClaimServiceService
 
 class ClaimSubmitServiceTestCase(TestCase):
     test_hf = None
 
-    test_insuree = None
+    test_insuree =None
     test_claim_admin = None
     test_icd = None
     test_claim = None
     test_claim_item = None
     test_claim_service = None
     test_region = None
     test_district = None
     test_village = None
     test_ward = None
-
+    
 
     @classmethod
     def setUpTestData(cls):
         if cls.test_region is None:
-            cls.test_village = create_test_village()
-            cls.test_ward = cls.test_village.parent
-            cls.test_region = cls.test_village.parent.parent.parent
+            cls.test_village  =create_test_village( )
+            cls.test_ward =cls.test_village.parent
+            cls.test_region =cls.test_village.parent.parent.parent
             cls.test_district = cls.test_village.parent.parent
 
-        cls.test_hf = create_test_health_facility("1", cls.test_district.id, valid=True)
+        cls.test_hf=create_test_health_facility("1", cls.test_district.id, valid=True)
         props = dict(
             last_name="name",
             other_names="surname",
             dob=core.datetime.date(2000, 1, 13),
             chf_id="884930485",
         )
         family_props = dict(
             location=cls.test_village,
         )
-        cls.test_insuree = create_test_insuree(is_head=True, custom_props=props, family_custom_props=family_props)
-        cls.test_claim_admin = create_test_claim_admin()
+        cls.test_insuree= create_test_insuree(is_head=True, custom_props=props, family_custom_props=family_props)
+        cls.test_claim_admin= create_test_claim_admin()
         cls.test_icd = Diagnosis(code='ICD00I', name='diag test', audit_user_id=-1)
         cls.test_icd.save()
         cls.test_claim = Claim.objects.create(
             date_claimed=core.datetime.date(2020, 1, 9),
-            code="code_ABVCD",
+            code="code_ABVC",
             icd=cls.test_icd,
             claimed=2000,
             date_from=core.datetime.date(2020, 1, 13),
             admin=cls.test_claim_admin,
             insuree=cls.test_insuree,
             health_facility=cls.test_hf,
             status=Claim.STATUS_ENTERED,
             audit_user_id=-1
         )
-
+        
         cls.test_claim_item = ClaimItem.objects.create(
-            claim=cls.test_claim,
-            item=create_test_item(
+            claim = cls.test_claim,
+            item =create_test_item(
                 'D',
-                custom_props={"code": "cCode", "price": 1000}
+                custom_props={"code": "cCode", "price" :1000}
             ),
-            price_asked=1000,
+            price_asked = 1000,
             qty_provided=1,
             audit_user_id=-1,
             status=ClaimDetail.STATUS_PASSED,
             availability=True
         )
         cls.test_claim_service = ClaimService.objects.create(
-            claim=cls.test_claim,
-            service=create_test_service(
+            claim = cls.test_claim,
+            service = create_test_service(
                 'D',
-                custom_props={"code": "sCode", "price": 1000}
+                custom_props={"code": "sCode", "price" :1000}
             ),
-            price_asked=1000,
+            price_asked = 1000,
             qty_provided=1,
             audit_user_id=-1,
             status=ClaimDetail.STATUS_PASSED
         )
 
     def test_minimal_item_claim_submit_xml(self):
         items = [
@@ -171,35 +174,35 @@
             start_date=core.datetime.date(2020, 1, 13),
             claim_admin_code=self.test_claim_admin.code,
             insuree_chf_id=self.test_insuree.chf_id,
             health_facility_code=self.test_hf.code,
             item_submits=items,
             service_submits=services
         )
-
+          
         details = "<Details>"
         details = details + "<ClaimDate>09/01/2020</ClaimDate>"
         details = details + f"<HFCode>{self.test_hf.code}</HFCode>"
         details = details + f"<ClaimAdmin>{self.test_claim_admin.code}</ClaimAdmin>"
         details = details + "<ClaimCode>code_ABVC</ClaimCode>"
-        details = details + f"<CHFID>{self.test_insuree.chf_id}</CHFID>"
+        details = details + f"<CHFID>{self.test_insuree.chf_id}</CHFID>"        
         details = details + "<StartDate>13/01/2020</StartDate>"
         details = details + f"<ICDCode>{self.test_icd.code}</ICDCode>"
         details = details + "<Total>334</Total>"
         details = details + "</Details>"
         expected = "<Claim>%s" % details
         expected = expected + "<Items>%s%s</Items>" % (item_a, item_b)
         expected = expected + \
-            "<Services>%s%s</Services>" % (service_a, service_b)
+                   "<Services>%s%s</Services>" % (service_a, service_b)
         expected = expected + "</Claim>"
         self.assertEquals(expected, claim.to_xml())
 
     @mock.patch('django.db.connections')
     def test_claim_submit_error(self, mock_connections):
-        if connection.vendor != 'mssql':
+        if connection.vendor != 'microsoft':
             self.skipTest("This test can only be executed for MSSQL database")
         with mock.patch("claim.services.ClaimSubmitService.hf_scope_check") as mock_security:
             mock_security.return_value = None
             query_result = [2]
             mock_connections.__getitem__.return_value.cursor.return_value \
                 .__enter__.return_value.fetchone.return_value = query_result
             mock_user = mock.Mock(is_anonymous=False)
@@ -215,27 +218,30 @@
                 health_facility_code=self.test_hf.code,
             )
             service = ClaimSubmitService(user=mock_user)
             with self.assertRaises(ClaimSubmitError) as cm:
                 service.submit(claim)
             self.assertNotEqual(cm.exception.code, 0)
 
-    def test_claim_submit_allgood_xml(self):
+    @mock.patch('django.db.connections')
+    def test_claim_submit_allgood_xml(self, mock_connections):
+        if connection.vendor != 'microsoft':
+            self.skipTest("This test can only be executed for MSSQL database")
         with mock.patch("django.db.backends.utils.CursorWrapper") as mock_cursor:
             # required for all modules tests
             mock_cursor.return_value.description = None
             # required for claim module tests
             mock_cursor.return_value.__enter__.return_value.description = None
             with mock.patch("claim.services.ClaimSubmitService.hf_scope_check") as mock_security:
                 mock_security.return_value = None
                 mock_user = mock.Mock(is_anonymous=False)
                 mock_user.has_perm = mock.MagicMock(return_value=True)
                 claim = ClaimSubmit(
                     date=core.datetime.date(2020, 1, 9),
-                    code="code_ABVC",
+                    code="code_ABVCD",
                     icd_code=self.test_icd.code,
                     total=334,
                     start_date=core.datetime.date(2020, 1, 13),
                     claim_admin_code=self.test_claim_admin.code,
                     insuree_chf_id=self.test_insuree.chf_id,
                     health_facility_code=self.test_hf.code,
                 )
@@ -276,39 +282,86 @@
         service = ClaimSubmitService(user=mock_user)
 
         service.enter_and_submit(claim, False)
 
         with self.assertRaises(ValidationError):
             service.enter_and_submit(claim, False)
 
+    def test_service_create_hook(self):
+        item = create_test_item("D", custom_props={})
+        service = create_test_service("V")
+        claim = create_test_claim()
+        service_items_dict = {
+            "qty_provided": 7, "price_asked": 11, "service_id": 23,
+            "status": 1, "validity_from": "2019-06-01", "validity_to": None, "audit_user_id": -1,
+            "service_item_set": [{"sub_item_code": item.code, "qty_asked":1, "qty_provided": 7, "price_asked": 11}],
+            "service_service_set": [{"sub_service_code": service.code, "qty_asked":2, "qty_provided": 3, "price_asked": 20}]
+        }
+        service_create_hook(claim.id, service_items_dict)
+        claim_service_item = ClaimServiceItem.objects.filter(item=item.id)
+        self.assertTrue(len(claim_service_item) > 0)
+        claim_service_item = claim_service_item.first()
+        self.assertEquals(claim_service_item.qty_displayed, 1)
+        self.assertEquals(claim_service_item.qty_provided, 7)
+        self.assertEquals(claim_service_item.price_asked, 11)
+
+        claim_service_service = ClaimServiceService.objects.filter(service=service.id)
+        self.assertTrue(len(claim_service_service) > 0)
+        claim_service_service = claim_service_service.first()
+        self.assertEquals(claim_service_service.qty_displayed, 2)
+        self.assertEquals(claim_service_service.qty_provided, 3)
+        self.assertEquals(claim_service_service.price_asked, 20)
+
+        service_items_dict["service_item_set"] = [{"qty_asked": 90, "sub_item_code": item.code}]
+        service_items_dict["service_service_set"] = [{"qty_asked": 100, "sub_service_code": service.code}]
+            
+        service_update_hook(claim.id, service_items_dict)
+        claim_service_service.refresh_from_db()
+        self.assertEqual(100, claim_service_service.qty_displayed)
+        
+        claim_service_item.refresh_from_db()
+        self.assertEqual(90, claim_service_item.qty_displayed)
+    
+    def test_calcul_amount_service(self):
+        item = create_test_item("D", custom_props={})
+        service = create_test_service("V")
+        service_items_dict = {
+            "qty_provided": 5, "price_asked": 50, "service_id": 23,
+            "status": 1, "validity_from": "2019-06-01", "validity_to": None, "audit_user_id": -1,
+            "service_item_set": [{"sub_item_code": item.code, "qty_asked":1, "qty_provided": 7, "price_asked": 11}],
+            "service_service_set": [{"sub_service_code": service.code, "qty_asked":2, "qty_provided": 3, "price_asked": 20}]
+        }
+        result = calcul_amount_service(service_items_dict)
+        self.assertEqual(result, 51)
+
     def _get_test_dict(self, code=None):
         return {
-            "health_facility_id": self.test_claim.health_facility_id,
-            "icd_id": self.test_icd.id,
-            "date_from": self.test_claim.date_from,
+            "health_facility_id": self.test_claim.health_facility_id, 
+            "icd_id": self.test_icd.id, 
+            "date_from": self.test_claim.date_from, 
             "code": self.test_claim.code if code is None else code,
-            "date_claimed": self.test_claim.date_claimed,
+            "date_claimed": self.test_claim.date_claimed, 
             "date_to": self.test_claim.date_to,
-            "audit_user_id": self.test_claim.audit_user_id,
-            "insuree_id": self.test_claim.insuree_id,
-            "status": self.test_claim.status,
+            "audit_user_id": self.test_claim.audit_user_id, 
+            "insuree_id": self.test_claim.insuree_id, 
+            "status": self.test_claim.status, 
             "validity_from": self.test_claim.validity_from,
             "items": [{
-                "qty_provided": self.test_claim_item.qty_provided,
-                "price_asked": self.test_claim_item.price_asked,
-                "item_id": self.test_claim_item.item_id,
-                "status": self.test_claim_item.status,
+                "qty_provided": self.test_claim_item.qty_provided, 
+                "price_asked": self.test_claim_item.price_asked, 
+                "item_id": self.test_claim_item.item_id, 
+                "status": self.test_claim_item.status, 
                 "availability": self.test_claim_item.availability,
-                "validity_from": self.test_claim_item.validity_from,
-                "validity_to": self.test_claim_item.validity_to,
+                "validity_from": self.test_claim_item.validity_from, 
+                "validity_to": self.test_claim_item.validity_to, 
                 "audit_user_id": self.test_claim_item.audit_user_id
             }],
             "services": [{
-                "qty_provided": self.test_claim_service.qty_provided,
-                "price_asked": self.test_claim_service.price_asked,
-                "service_id": self.test_claim_service.service_id,
-                "status": self.test_claim_service.status,
-                "validity_from": self.test_claim_service.validity_from,
-                "validity_to": self.test_claim_service.validity_to,
+                "qty_provided": self.test_claim_service.qty_provided, 
+                "price_asked": self.test_claim_service.price_asked, 
+                "service_id": self.test_claim_service.service_id, 
+                "status": self.test_claim_service.status, 
+                "validity_from": self.test_claim_service.validity_from, 
+                "validity_to": self.test_claim_service.validity_to, 
                 "audit_user_id": self.test_claim_service.audit_user_id
             }]
         }
```

### Comparing `openimis-be-claim-1.6.0/claim/tests/test_validations.py` & `openimis_be_claim-1.7.0/claim/tests/test_validations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-from claim.gql_mutations import set_claims_status, update_claims_dedrems
-from claim.models import Claim, ClaimDedRem, ClaimItem, ClaimDetail, ClaimService
+from claim.services import update_claims_dedrems, set_claims_status
+from claim.models import Claim, ClaimDedRem, ClaimItem, ClaimDetail, ClaimService, ClaimServiceItem, ClaimServiceService
 from claim.test_helpers import create_test_claim, create_test_claimservice, create_test_claimitem, \
     mark_test_claim_as_processed, delete_claim_with_itemsvc_dedrem_and_history
+from core.test_helpers import create_test_officer
+
 from claim.validations import get_claim_category, validate_claim, validate_assign_prod_to_claimitems_and_services, \
     process_dedrem, REJECTION_REASON_WAITING_PERIOD_FAIL, REJECTION_REASON_INVALID_ITEM_OR_SERVICE
 from core.models import User, InteractiveUser
 from django.test import TestCase
 from insuree.models import Family, Insuree
 from insuree.test_helpers import create_test_insuree
 from location.models import HealthFacility
+from medical_pricelist.test_helpers import add_service_to_hf_pricelist, add_item_to_hf_pricelist
+from medical.models import ServiceItem, ServiceService
+from product.models import ProductItemOrService
 from medical.test_helpers import create_test_service, create_test_item
 from medical_pricelist.test_helpers import add_service_to_hf_pricelist, add_item_to_hf_pricelist, \
     update_pricelist_service_detail_in_hf_pricelist, update_pricelist_item_detail_in_hf_pricelist
 from policy.test_helpers import create_test_policy
+ 
 
 # default arguments should not pass a list or a dict because they're mutable but we don't risk mutating them here:
 # noinspection PyDefaultArgument,DuplicatedCode
 from product.test_helpers import create_test_product, create_test_product_service, create_test_product_item
 
 
 class ValidationTest(TestCase):
@@ -256,15 +262,15 @@
         # The insuree has a patient_category of 6, not matching the service category
         claim1 = create_test_claim({"insuree_id": insuree.id})
         service1 = create_test_claimservice(claim1, custom_props={"service_id": service.id})
         errors = validate_claim(claim1, True)
 
         # Then
         claim1.refresh_from_db()
-        self.assertEquals(len(errors), 1)
+        self.assertEquals(len(errors), 2)
         self.assertEquals(errors[0]['code'], 1)  # claimed rejected because all services are rejected
         self.assertEquals(claim1.services.first().rejection_reason, 4)  # reason is wrong insuree mask
 
         # tearDown
         service1.delete()
         claim1.delete()
         policy.insuree_policies.first().delete()
@@ -541,15 +547,15 @@
         pricelist_detail = add_service_to_hf_pricelist(service)
 
         # A first claim for a visit within the waiting period should be refused
         claim1 = create_test_claim({"insuree_id": insuree.id})
         service1 = create_test_claimservice(claim1, custom_props={"service_id": service.id})
         errors = validate_claim(claim1, True)
 
-        self.assertEqual(len(errors), 1, "An adult visit within the waiting period should be refused")
+        self.assertEqual(len(errors), 2, "An adult visit within the waiting period should be refused")
         self.assertEqual(claim1.services.first().rejection_reason, REJECTION_REASON_WAITING_PERIOD_FAIL)
 
         # a visit after the waiting period should be fine
         claim2 = create_test_claim({
             "insuree_id": insuree.id,
             "date_from": datetime.datetime(2020, 2, 1),
             "date_to": datetime.datetime(2020, 2, 1),
@@ -924,15 +930,15 @@
 
         set_claims_status([claim1.uuid], "review_status", Claim.REVIEW_DELIVERED)
         update_claims_dedrems([claim1.uuid], self.user)
 
         # Then dedrem should have been updated
         dedrem = ClaimDedRem.objects.filter(claim=claim1).first()
         self.assertIsNotNone(dedrem)
-        self.assertEquals(dedrem.rem_g, 37 + 53)
+        self.assertEquals(dedrem.rem_g, 200)  # 100*1 + 100*1
 
         # tearDown
         # dedrem.delete() # already done if the test passed
         delete_claim_with_itemsvc_dedrem_and_history(claim1)
         policy.insuree_policies.first().delete()
         policy.delete()
         product_item.delete()
@@ -1111,14 +1117,146 @@
         product_item.delete()
         product_service.delete()
         pricelist_detail1.delete()
         pricelist_detail2.delete()
         service.delete()
         item.delete()
         product.delete()
+
     def test_set_status(self):
         class DummyUser:
             id_for_audit=-1
-        claim = create_test_claim(custom_props={'status':Claim.STATUS_CHECKED})
-        set_claims_status([claim.uuid], 'feedback_status', Claim.FEEDBACK_SELECTED, user = DummyUser())
+        insuree = create_test_insuree()
+        officer = create_test_officer(villages=[insuree.current_village or insuree.family.location])
+        claim = create_test_claim(custom_props={'status':Claim.STATUS_CHECKED, 
+                                                'insuree':insuree})
+        restult =set_claims_status([claim.uuid], 'feedback_status', Claim.FEEDBACK_SELECTED, user = DummyUser())
         claim.refresh_from_db()
         self.assertEqual(claim.feedback_status, Claim.FEEDBACK_SELECTED)
+    
+    def test_submit_claim_with_different_packatypes(self):
+        from claim.apps import ClaimConfig
+        ClaimConfig.native_code_for_services=False
+        insuree = create_test_insuree()
+        self.assertIsNotNone(insuree)
+        product = create_test_product("VISIT", custom_props={})
+        policy = create_test_policy(product, insuree, link=True)
+        service = create_test_service("V", custom_props={"packagetype": "F"})
+        item = create_test_item("D", custom_props={})
+        product_service = create_test_product_service(product, service)
+        product_service.price_origin = ProductItemOrService.ORIGIN_CLAIM
+        product_service.save()
+        product_item = create_test_product_item(product, item)
+        product_item.price_origin = ProductItemOrService.ORIGIN_CLAIM
+        product_item.save()
+        pricelist_detail1 = add_service_to_hf_pricelist(service)
+        pricelist_detail2 = add_item_to_hf_pricelist(item)
+
+        claim1 = create_test_claim({"insuree_id": insuree.id})
+        claimservice1 = create_test_claimservice(
+            claim1, custom_props={"service_id": service.id})
+        clalimitem1 = create_test_claimitem(
+            claim1, "D", custom_props={"item_id": item.id})
+        # Set the price_adjusted to 4000
+        claimservice1.price_adjusted = 4000
+        claimservice1.save()
+        # set the service price to 1000 lower than the price_adjusted
+        service.price = 1000
+        service.save()
+        service.refresh_from_db()
+        errors = validate_claim(claim1, True)
+        errors = validate_assign_prod_to_claimitems_and_services(claim1)
+        errors += process_dedrem(claim1, -1, True)
+        self.assertEqual(len(errors), 0)
+        # The claimservice1's price_adjusted should be the service price
+        # because the price_adjusted is greater than the service (4000 > 1000)
+        claimservice1.refresh_from_db()
+        self.assertEqual(claimservice1.price_adjusted, 1000)
+
+        # Set the price_adjusted to None
+        claimservice1.price_adjusted = None
+        claimservice1.price_asked = 6000
+        service.price = 750
+        service.save()
+        claimservice1.save()
+        validate_claim(claim1, True)
+        validate_assign_prod_to_claimitems_and_services(claim1)
+        process_dedrem(claim1, -1, True)
+        claimservice1.refresh_from_db()
+        service.refresh_from_db()
+        # The claimservice1's price_adjusted should also be the service's price
+        # because the price_asked is now also greater than the service (6000 > 750)
+        self.assertEqual(claimservice1.price_adjusted, 750)
+
+        # Change the price_origin
+        product_service.price_origin = ProductItemOrService.ORIGIN_PRICELIST
+        product_service.save()
+        product_item.price_origin = ProductItemOrService.ORIGIN_PRICELIST
+        product_item.save()
+        service.packagetype = "P"
+        service.save()
+        # serviceservice = ServiceService.objects.create(
+        #     servicelinkedService=service,
+        #     service_id = claimservice1.service_id,
+        #     price_asked = 3,
+        #     qty_provided = 2
+        # )
+        claimserviceservice = ClaimServiceService.objects.create(
+            service = service,
+            claim_service = claimservice1,
+            qty_displayed = 5,
+            qty_provided = 4,
+            price_asked = 300,
+        )
+        claimserviceitem = ClaimServiceItem.objects.create(
+            item = item,
+            claim_service = claimservice1,
+            qty_displayed = 2,
+            qty_provided = 3,
+            price_asked = 500,
+        )
+        serviceitem = ServiceItem.objects.create(
+            servicelinkedItem=service,
+            item = clalimitem1.item,
+            price_asked = 12,
+            qty_provided = 11
+        )
+
+        validate_claim(claim1, True)
+        validate_assign_prod_to_claimitems_and_services(claim1)
+        process_dedrem(claim1, -1, True)
+        claimservice1.refresh_from_db()
+        # claimservicesitem.qty_provided 2 is not equal to qty_displayed on the claimserviceservice
+        # so the price_adjusted is set to 0
+        self.assertEqual(claimservice1.price_adjusted, 0)
+
+        claimserviceservice.qty_displayed = 2
+        claimserviceservice.save()
+        claimserviceservice.refresh_from_db
+        validate_claim(claim1, True)
+        validate_assign_prod_to_claimitems_and_services(claim1)
+        process_dedrem(claim1, -1, True)
+        claimservice1.refresh_from_db()
+        # service item.qty_provided 11 is not equal to qty_displayed on the claimserviceitem
+        # so the price_adjusted is set to 0
+        self.assertEqual(claimservice1.price_adjusted, 0)
+
+        dedrem_qs = ClaimDedRem.objects.filter(claim=claim1)
+        # tearDown
+        dedrem_qs.delete()
+        # serviceservice.delete()
+        claimserviceservice.delete()
+        claimserviceitem.delete()
+        claimservice1.delete()
+        serviceitem.delete()
+        clalimitem1.delete()
+        claim1.delete()
+        policy.insuree_policies.first().delete()
+        policy.delete()
+        product_item.delete()
+        product_service.delete()
+        pricelist_detail1.delete()
+        pricelist_detail2.delete()
+        service.delete()
+        item.delete()
+        product.delete()
+        ClaimConfig.native_code_for_services=True
```

### Comparing `openimis-be-claim-1.6.0/claim/tests/tests.py` & `openimis_be_claim-1.7.0/claim/tests/tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import base64
 import json
 from dataclasses import dataclass
 from core.models import User
+from core.models.openimis_graphql_test_case import openIMISGraphQLTestCase
 from core.utils import filter_validity
 from core.test_helpers import create_test_interactive_user
 from django.conf import settings
 from graphene_django.utils.testing import GraphQLTestCase
 from graphql_jwt.shortcuts import get_token
 #credits https://docs.graphene-python.org/projects/django/en/latest/testing/
 from claim import schema as claim_schema
@@ -25,16 +26,15 @@
 from medical_pricelist.test_helpers import add_service_to_hf_pricelist
 
 @dataclass
 class DummyContext:
     """ Just because we need a context to generate. """
     user: User
 
-class ClaimGraphQLTestCase(GraphQLTestCase):
-    GRAPHQL_URL = f'/{settings.SITE_ROOT()}graphql'
+class ClaimGraphQLTestCase(openIMISGraphQLTestCase):
     # This is required by some version of graphene but is never used. It should be set to the schema but the import
     # is shown as an error in the IDE, so leaving it as True.
     GRAPHQL_SCHEMA = True
     admin_user = None
     graph_client = None
     schema = None      
     officer= None
@@ -73,15 +73,15 @@
                 {
                     totalCount
                     pageInfo { hasNextPage, hasPreviousPage, startCursor, endCursor}
                     edges
                     {
                         node
                         {
-                            uuid,code,jsonExt,dateClaimed,dateProcessed,feedbackStatus,reviewStatus,claimed,approved,status,restore {id},healthFacility { id uuid name code },insuree{id, uuid, chfId, lastName, otherNames, dob},attachmentsCount
+                            uuid,code,jsonExt,dateClaimed,dateProcessed,feedbackStatus,reviewStatus,claimed,approved,status,restoreId,healthFacility { id uuid name code },insuree{id, uuid, chfId, lastName, otherNames, dob},attachmentsCount
                         }
                     }
                 }
             }
             ''',
             headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_token}"},
         )
@@ -102,15 +102,15 @@
                 {
                     totalCount
                     pageInfo { hasNextPage, hasPreviousPage, startCursor, endCursor}
                     edges
                     {
                         node
                         {
-                            uuid,code,jsonExt,dateClaimed,dateProcessed,feedbackStatus,reviewStatus,claimed,approved,status,restore {id},healthFacility { id uuid name code },insuree{id, uuid, chfId, lastName, otherNames, dob},attachmentsCount
+                            uuid,code,jsonExt,dateClaimed,dateProcessed,feedbackStatus,reviewStatus,claimed,approved,status,restoreId,healthFacility { id uuid name code },insuree{id, uuid, chfId, lastName, otherNames, dob},attachmentsCount
                         }
                     }
                 }
             }
             ''',
             headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_token}"},
             variables={'status': 2, 'first':10}
@@ -148,109 +148,114 @@
                 visitType: "O"
                 services: [
                 {{
                 
                 serviceId: {self.service.id}
                 priceAsked: "10.00"
                 qtyProvided: "1.00"
-                status: 1
+                status: 1,
+                serviceItemSet: [],
+                serviceServiceSet: []
             }}
                 ]
                 items: [
                 ]
                     }}
                 ) {{
                     clientMutationId
                     internalId
                 }}
             }}
                 ''',
             headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_token}"})
-        
-        #wait 
-        
-        response = self.query('''
-        
-        {
-        mutationLogs(clientMutationId: "3a90436a-d5ea-48e7-bde4-0bcff0240260")
-        {
-            
-        pageInfo { hasNextPage, hasPreviousPage, startCursor, endCursor}
-        edges
-        {
-        node
-        {
-            id,status,error,clientMutationId,clientMutationLabel,clientMutationDetails,requestDateTime,jsonExt
-        }
-        }
-        }
-        }
-        
-        ''',
-            headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_token}"})
-        
-        
+        self.get_mutation_result('3a90436a-d5ea-48e7-bde4-0bcff0240260', self.admin_token )
         claim = Claim.objects.filter(code = 'm-c-claim').first()
         self.assertIsNotNone(claim)
         self.assertEqual(claim.status, Claim.STATUS_ENTERED)
-        
+        response = self.query(
+            f'''
+            mutation {{
+                updateClaim(
+                    input: {{
+                    clientMutationId: "3a90436b-d5ea-48e7-bde4-0bcff0240260"
+                    clientMutationLabel: "Update Claim - m-c-claim" 
+                    code: "m-c-claim"
+                autogenerate: false
+                uuid: "{str(claim.uuid)}"
+                insureeId: {self.insuree.id}
+                adminId: {self.claim_admin.id}
+                dateFrom: "2023-11-06"  
+                icdId: 2 
+                jsonExt: "{{}}"
+                feedbackStatus: 1
+                reviewStatus: 1
+                dateClaimed: "2023-12-06"
+                healthFacilityId: {self.claim_admin.health_facility.id}
+                visitType: "O"
+                services: [
+                {{
+                
+                serviceId: {self.service.id}
+                priceAsked: "10.00"
+                qtyProvided: "1.00"
+                status: 1,
+                serviceItemSet: [],
+                serviceServiceSet: []
+            }}
+                ]
+                items: [
+                ]
+                    }}
+                ) {{
+                    clientMutationId
+                    internalId
+                }}
+            }}
+                ''',
+            headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_token}"})
+        self.get_mutation_result('3a90436b-d5ea-48e7-bde4-0bcff0240260', self.admin_token )
+                
         #submit claim 
         response = self.query(f'''
             mutation {{
             submitClaims(
                 input: {{
-                clientMutationId: "d02fff0a-dd95-4413-a2f6-4cf2189dc0d6"
+                clientMutationId: "d02fff0a-dd95-4413-a2f4-4cf2189dc0d6"
                 clientMutationLabel: "Submit claim erterwtw"
                 
                 uuids: ["{claim.uuid}"]
                 }}
             ) {{
                 clientMutationId
                 internalId
             }}
             }}
             ''',
             headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_token}"})
         self.assertResponseNoErrors(response)
-
+        self.get_mutation_result('d02fff0a-dd95-4413-a2f4-4cf2189dc0d6', self.admin_token )
         # select for feeback
         claim = Claim.objects.filter(code = 'm-c-claim').first()
+        create_test_officer(villages=[claim.insuree.family.location])
         self.assertEqual(claim.status, Claim.STATUS_CHECKED)
         response = self.query(f'''
             mutation {{
             selectClaimsForFeedback(
                 input: {{
-                clientMutationId: "f0585e2b-d72d-4001-905a-1cf10e9f1722"
+                clientMutationId: "f0585e2b-d72d-4001-915a-1cf10e9f1722"
                 clientMutationLabel: "Select claim sadddfas for feedback"
                 
                 uuids: ["{claim.uuid}"]
                 }}
             ) {{
                 clientMutationId
                 internalId
             }}
             }}
         ''' ,
             headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_token}"})
         self.assertResponseNoErrors(response)
-
+        self.get_mutation_result('f0585e2b-d72d-4001-915a-1cf10e9f1722', self.admin_token )
         ## check the mutation answer
-        response = self.query('''
-        {
-        mutationLogs(clientMutationId: "f0585e2b-d72d-4001-905a-1cf10e9f1722")
-        {
-            
-        pageInfo { hasNextPage, hasPreviousPage, startCursor, endCursor}
-        edges
-        {
-        node
-        {
-            id,status,error,clientMutationId,clientMutationLabel,clientMutationDetails,requestDateTime,jsonExt
-        }
-        }
-        }
-        }
-            ''',
-            headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_token}"})
-        self.assertResponseNoErrors(response)
+        
         claim = Claim.objects.filter(code = 'm-c-claim').first()
         self.assertEqual(claim.feedback_status, Claim.FEEDBACK_SELECTED)
```

### Comparing `openimis-be-claim-1.6.0/claim/validations.py` & `openimis_be_claim-1.7.0/claim/validations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import itertools
 import logging
 from collections import namedtuple
 
-from claim.models import ClaimItem, Claim, ClaimService, ClaimDedRem, ClaimDetail
+from claim.models import ClaimItem, Claim, ClaimService, ClaimDedRem, ClaimDetail, ClaimServiceService, ClaimServiceItem
 from core import utils
 from core.datetimes.shared import datetimedelta
+from core.utils import filter_validity
 from django.db import connection
 from django.db.models import Sum, Q
 from django.db.models.functions import Coalesce
 from django.utils.translation import gettext as _
 from insuree.models import InsureePolicy
-from medical.models import Service
+from medical.models import Service, ServiceService, ServiceItem
 from medical_pricelist.models import ItemsPricelistDetail, ServicesPricelistDetail
 from policy.models import Policy
 from product.models import Product, ProductItem, ProductService, ProductItemOrService
 
 from .apps import ClaimConfig
 from .utils import get_queryset_valid_at_date
 
@@ -34,15 +35,15 @@
 REJECTION_REASON_MAX_VISITS = 12
 REJECTION_REASON_MAX_CONSULTATIONS = 13
 REJECTION_REASON_MAX_SURGERIES = 14
 REJECTION_REASON_MAX_DELIVERIES = 15
 REJECTION_REASON_QTY_OVER_LIMIT = 16
 REJECTION_REASON_WAITING_PERIOD_FAIL = 17
 REJECTION_REASON_MAX_ANTENATAL = 19
-
+REJECTION_REASON_INVALID_CLAIM = 20
 
 def validate_claim(claim, check_max):
     """
     Based on the legacy validation, this method returns standard codes along with details
     :param claim: claim to be verified
     :param check_max: max amount to validate. Everything above will be rejected
     :return: (result_code, error_details)
@@ -95,86 +96,86 @@
         .update(status=ClaimService.STATUS_PASSED)
 
     if rtn_items_passed + rtn_services_passed == 0:
         errors += [{'code': REJECTION_REASON_INVALID_ITEM_OR_SERVICE,
                     'message': _("claim.validation.all_items_and_services_rejected") % {
                         'code': claim.code},
                     'detail': claim.uuid}]
+        if len(detail_errors)>0:
+            errors += detail_errors
         claim.status = Claim.STATUS_REJECTED
         claim.rejection_reason = REJECTION_REASON_INVALID_ITEM_OR_SERVICE
         claim.save()
     logger.debug(f"Validation found {len(errors)} error(s)")
     return errors
 
 
 def validate_claimitems(claim):
     errors = []
     target_date = claim.date_from if claim.date_from else claim.date_to
-    for claimitem in claim.items \
-            .filter(validity_to__isnull=True) \
-            .filter(Q(rejection_reason=0) | Q(rejection_reason__isnull=True)):
-        errors += validate_claimitem_validity(claim, claimitem)
-        if not claimitem.rejection_reason:
-            errors += validate_claimitem_in_price_list(claim, claimitem)
-        if not claimitem.rejection_reason:
-            errors += validate_claimdetail_care_type(claim, claimitem)
-        if not claimitem.rejection_reason:
-            errors += validate_claimdetail_limitation_fail(claim, claimitem)
+    for claimitem in claim.items.all():
         if not claimitem.rejection_reason:
-            errors += validate_claimitem_frequency(claim, claimitem)
-        if not claimitem.rejection_reason:
-            errors += validate_item_product_family(
-                claimitem=claimitem,
-                target_date=target_date,
-                item=claimitem.item,
-                insuree_id=claim.insuree_id,
-                adult=claim.insuree.is_adult(target_date)
-            )
-        if claimitem.rejection_reason:
-            claimitem.status = ClaimItem.STATUS_REJECTED
-        else:
-            claimitem.rejection_reason = 0
-            claimitem.status = ClaimItem.STATUS_PASSED
-        claimitem.save()
+            errors += validate_claimitem_validity(claim, claimitem)
+            if not claimitem.rejection_reason:
+                errors += validate_claimitem_in_price_list(claim, claimitem)
+            if not claimitem.rejection_reason:
+                errors += validate_claimdetail_care_type(claim, claimitem)
+            if not claimitem.rejection_reason:
+                errors += validate_claimdetail_limitation_fail(claim, claimitem)
+            if not claimitem.rejection_reason:
+                errors += validate_claimitem_frequency(claim, claimitem)
+            if not claimitem.rejection_reason:
+                errors += validate_item_product_family(
+                    claimitem=claimitem,
+                    target_date=target_date,
+                    item=claimitem.item,
+                    insuree_id=claim.insuree_id,
+                    adult=claim.insuree.is_adult(target_date)
+                )
+            if claimitem.rejection_reason:
+                claimitem.status = ClaimItem.STATUS_REJECTED
+            else:
+                claimitem.rejection_reason = 0
+                claimitem.status = ClaimItem.STATUS_PASSED
+            claimitem.save()
     return errors
 
 
 def validate_claimservices(claim):
     errors = []
     target_date = claim.date_from if claim.date_from else claim.date_to
     base_category = get_claim_category(claim)
 
-    for claimservice in claim.services \
-            .filter(validity_to__isnull=True) \
-            .filter(Q(rejection_reason=0) | Q(rejection_reason__isnull=True)):
-        errors += validate_claimservice_validity(claim, claimservice)
+    for claimservice in claim.services.all():
         if not claimservice.rejection_reason:
-            errors += validate_claimservice_in_price_list(claim, claimservice)
-        if not claimservice.rejection_reason:
-            errors += validate_claimdetail_care_type(claim, claimservice)
-        if not claimservice.rejection_reason:
-            errors += validate_claimservice_frequency(claim, claimservice)
-        if not claimservice.rejection_reason:
-            errors += validate_claimdetail_limitation_fail(claim, claimservice)
-        if not claimservice.rejection_reason:
-            errors += validate_service_product_family(
-                claimservice=claimservice,
-                target_date=target_date,
-                service=claimservice.service,
-                insuree_id=claim.insuree_id,
-                adult=claim.insuree.is_adult(target_date),
-                base_category=base_category,
-                claim=claim,
-            )
-        if claimservice.rejection_reason:
-            claimservice.status = ClaimService.STATUS_REJECTED
-        else:
-            claimservice.rejection_reason = 0
-            claimservice.status = ClaimService.STATUS_PASSED
-        claimservice.save()
+            errors += validate_claimservice_validity(claim, claimservice)
+            if not claimservice.rejection_reason:
+                errors += validate_claimservice_in_price_list(claim, claimservice)
+            if not claimservice.rejection_reason:
+                errors += validate_claimdetail_care_type(claim, claimservice)
+            if not claimservice.rejection_reason:
+                errors += validate_claimservice_frequency(claim, claimservice)
+            if not claimservice.rejection_reason:
+                errors += validate_claimdetail_limitation_fail(claim, claimservice)
+            if not claimservice.rejection_reason:
+                errors += validate_service_product_family(
+                    claimservice=claimservice,
+                    target_date=target_date,
+                    service=claimservice.service,
+                    insuree_id=claim.insuree_id,
+                    adult=claim.insuree.is_adult(target_date),
+                    base_category=base_category,
+                    claim=claim,
+                )
+            if claimservice.rejection_reason:
+                claimservice.status = ClaimService.STATUS_REJECTED
+            else:
+                claimservice.rejection_reason = 0
+                claimservice.status = ClaimService.STATUS_PASSED
+            claimservice.save()
     return errors
 
 
 def validate_claimitem_validity(claim, claimitem):
     # In the stored procedure, this check used a complex query to get the latest item but the latest item seems to
     # always be updated.
     # select *
@@ -301,15 +302,14 @@
                 validity_to__isnull=True,
                 target_date__gte=td - delta,
                 status=ClaimDetail.STATUS_PASSED,
                 claim__insuree_id=claim.insuree_id,
                 claim__status__gt=Claim.STATUS_ENTERED
                 ) \
         .exclude(claim__uuid=claim.uuid) \
-        .order_by('-claim__date_from') \
         .exists()
 
 
 def validate_claimitem_frequency(claim, claimitem):
     errors = []
     if claimitem.item.frequency and \
             frequency_check(ClaimItem.objects.filter(item=claimitem.item), claim, claimitem.item):
@@ -930,32 +930,30 @@
     # TODO: it is not clear in the original code which policy_id was actually used, the latest one apparently...
     policy = None
     ceiling_interpretation = None
 
     # The original code has a pretty complex query here called product_loop that refers to policies while it is
     # actually looping on ClaimItem and ClaimService.
     items_query = claim.items.filter(
-        Q(item__validity_to__isnull=True) | Q(item__validity_to__gte=target_date),
-        validity_to__isnull=True,
+        *filter_validity(validity=target_date, prefix='item__'),
+        *filter_validity(),
+        *filter_validity(prefix='product__'),
         rejection_reason=0,
-        item__validity_from__lte=target_date,
-        product__isnull=False,
-        product__validity_to__isnull=True
     ).values("policy_id", "product_id")
     services_query = claim.services.filter(
-        Q(service__validity_to__isnull=True) | Q(service__validity_to__gte=target_date),
-        validity_to__isnull=True,
+        *filter_validity(validity=target_date, prefix='service__'),
+        *filter_validity(),
+        *filter_validity(prefix='product__'),
         rejection_reason=0,
-        service__validity_from__date__lte=target_date,
-        product__isnull=False, product__validity_to__isnull=True
     ).values("policy_id", "product_id")
     if items_query.count() == 0 and services_query.count() == 0:
         logger.warning(f"claim {claim.uuid} did not have any item or service to valuate.")
     for policy_product in items_query.union(services_query, all=True):
-        product = Product.objects.get(id=policy_product["product_id"])
+        product = Product.objects.get(*filter_validity(validity=target_date), 
+                Q(Q(id=policy_product["product_id"])|Q(legacy_id=policy_product["product_id"])))
         policy_members = InsureePolicy.objects.filter(
             policy_id=policy_product["policy_id"],
             effective_date__isnull=False,
             effective_date__lte=target_date,
             expiry_date__gte=target_date,
             validity_to__isnull=True
         ).count()
@@ -1084,19 +1082,19 @@
                         )
 
         # Loop through items
         deducted = 0
         remunerated = 0
         for claim_detail in itertools.chain(
                 claim.items
-                        .filter(validity_to__isnull=True)
-                        .filter(status=ClaimItem.STATUS_PASSED),
+                        .filter(validity_to__isnull=True,
+                                status=ClaimItem.STATUS_PASSED),
                 claim.services
-                        .filter(validity_to__isnull=True)
-                        .filter(status=ClaimService.STATUS_PASSED)):
+                        .filter(validity_to__isnull=True,
+                                status=ClaimService.STATUS_PASSED)):
             detail_is_item = isinstance(claim_detail, ClaimItem)
             itemsvc_quantity = claim_detail.qty_approved \
                 if claim_detail.qty_approved is not None else claim_detail.qty_provided
             set_price_deducted = 0
             exceed_ceiling_amount = 0
             exceed_ceiling_amount_category = 0
             # TODO make sure that this does not return more than one row ?
@@ -1127,21 +1125,81 @@
                     raise ValueError("Product Service not found")
 
             pl_price = itemsvc_pricelist_detail.price_overrule if itemsvc_pricelist_detail.price_overrule \
                 else claim_detail.itemsvc.price
 
             if claim_detail.price_approved is not None:
                 set_price_adjusted = claim_detail.price_approved
+            if claim_detail.price_origin == ProductItemOrService.ORIGIN_CLAIM:
+                set_price_adjusted = claim_detail.price_asked
+                if ClaimConfig.native_code_for_services == False:
+                    try:
+                        if claim_detail.service.packagetype == 'F':
+                            service_price = claim_detail.service.price
+                            if claim_detail.price_adjusted is not None:
+                                logger.debug(f"compare {claim_detail.price_adjusted} and {service_price}")
+                                if claim_detail.price_adjusted > service_price:
+                                    set_price_adjusted = service_price
+                            else:
+                                logger.debug(f"compare {claim_detail.price_asked} and {service_price}")
+                                if claim_detail.price_asked > service_price:
+                                    set_price_adjusted = service_price
+                    except:
+                        logger.debug("This it an item element")
             else:
-                if claim_detail.price_origin == ProductItemOrService.ORIGIN_CLAIM:
-                    set_price_adjusted = claim_detail.price_asked
-                else:
-                    set_price_adjusted = pl_price
+                set_price_adjusted = pl_price
+                if ClaimConfig.native_code_for_services == False:
+                    try:
+                        contunue_service_check = True
+                        if claim_detail.service.packagetype == 'P':
+                            service_services = ServiceService.objects.filter(servicelinkedService=claim_detail.service.id).all()
+                            claim_service_services = ClaimServiceService.objects.filter(claim_service=claim_detail.id).all()
+                            if len(service_services) == len(claim_service_services):
+                                for servservice in service_services:
+                                    for claimserviceservice in claim_service_services:
+                                        if servservice.service.id == claimserviceservice.service.id:
+                                            logger.debug(f"comparing serviceservice qty {servservice.qty_provided}\
+                                                and claimserviceservice qty {claimserviceservice.qty_displayed}")
+                                            if servservice.qty_provided != claimserviceservice.qty_displayed:
+                                                set_price_adjusted = 0
+                                                contunue_service_check = False
+                                                break
+                                    if contunue_service_check == False:
+                                        break
+                            else:
+                                # user misconfiguration !
+                                set_price_adjusted = 0
+                                contunue_service_check = False
+                            logger.debug(f"set_price_adjusted after service check {set_price_adjusted}")
+                            if contunue_service_check:
+                                contunue_item_check = True
+                                service_items = ServiceItem.objects.filter(servicelinkedItem=claim_detail.service.id).all()
+                                claim_service_items = ClaimServiceItem.objects.filter(claim_service=claim_detail.id).all()
+                                logger.debug(f"service_items: {service_items}")
+                                logger.debug(f"claim_service_items: {claim_service_items}")
+                                if len(service_items) == len(claim_service_items):
+                                    for serviceitem in service_items:
+                                        for claimservicesitem in claim_service_items:
+                                            if serviceitem.item.id == claimservicesitem.item.id:
+                                                logger.debug(f"comparing serviceitem qty {serviceitem.qty_provided}\
+                                                 and claimservicesitem qty {claimservicesitem.qty_displayed}")
+                                                if serviceitem.qty_provided != claimservicesitem.qty_displayed:
+                                                    set_price_adjusted = 0
+                                                    contunue_item_check = False
+                                                    break
+                                        if contunue_item_check == False:
+                                            break
+                                else:
+                                    # user misconfiguration !
+                                    set_price_adjusted = 0
+                                logger.debug(f"set_price_adjusted after items check {set_price_adjusted}")
+                    except:
+                        logger.debug("This is a ClaimItem element, not a ClaimService")
 
-            work_value = itemsvc_quantity * set_price_adjusted
+            work_value = int(itemsvc_quantity * set_price_adjusted)
 
             if claim_detail.limitation == ProductItemOrService.LIMIT_FIXED_AMOUNT \
                     and claim_detail.limitation_value \
                     and (itemsvc_quantity * claim_detail.limitation_value) < work_value:
                 work_value = itemsvc_quantity * claim_detail.limitation_value
 
             if deductible and deductible.amount - prev_deductible - deducted > 0:
```

### Comparing `openimis-be-claim-1.6.0/claim/views.py` & `openimis_be_claim-1.7.0/claim/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import base64
 from django.conf import settings
 from django.core.exceptions import PermissionDenied
 from django.http import HttpResponse
 from rest_framework.decorators import api_view, permission_classes
-from location.models import  LocationManager
+from location.models import LocationManager
 from report.services import ReportService
-from tools.views import checkUserWithRights
+from core.security import checkUserWithRights
 from .services import ClaimReportService
 from .reports import claim
 from .apps import ClaimConfig
 from .models import ClaimAttachment
 from django.utils.translation import gettext as _
 import core
 
@@ -32,15 +32,16 @@
         )
     ]
 )
 def attach(request):
     queryset = ClaimAttachment.objects.filter(*core.filter_validity())
     if settings.ROW_SECURITY:
         from location.models import LocationManager
-        queryset = LocationManager().build_user_location_filter_query( request.user._u, prefix='health_facility__location', queryset = queryset.select_related("claim"), loc_types=['D'])
+        queryset = LocationManager().build_user_location_filter_query(request.user._u, prefix='health_facility__location',
+                                                                      queryset=queryset.select_related("claim"), loc_types=['D'])
     attachment = queryset\
         .filter(id=request.GET['id'])\
         .first()
     if not attachment:
         raise PermissionDenied(_("unauthorized"))
 
     if ClaimConfig.claim_attachments_root_path and attachment.url is None:
```

### Comparing `openimis-be-claim-1.6.0/openimis_be_claim.egg-info/PKG-INFO` & `openimis_be_claim-1.7.0/openimis_be_claim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-claim
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Claim reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-claim-1.6.0/setup.py` & `openimis_be_claim-1.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-claim',
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Claim reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

