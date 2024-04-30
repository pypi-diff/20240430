# Comparing `tmp/openimis-be-insuree-1.6.0.tar.gz` & `tmp/openimis_be_insuree-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-insuree-1.6.0.tar", last modified: Sat Dec 16 00:56:40 2023, max compression
+gzip compressed data, was "openimis_be_insuree-1.7.0.tar", last modified: Tue Apr 30 09:01:04 2024, max compression
```

## Comparing `openimis-be-insuree-1.6.0.tar` & `openimis_be_insuree-1.7.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:40.351298 openimis-be-insuree-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      915 2023-12-16 00:56:40.351298 openimis-be-insuree-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:40.347298 openimis-be-insuree-1.6.0/insuree/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    16530 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8994 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:40.347298 openimis-be-insuree-1.6.0/insuree/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:40.347298 openimis-be-insuree-1.6.0/insuree/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/management/commands/generateinsurees.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:40.347298 openimis-be-insuree-1.6.0/insuree/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0002_family_familytype_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0003_insureepolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0004_confirmationtype_education_profession_relation.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0005_identificationtype.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0006_auto_20200722_0839.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0007_auto_20200722_0940.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0008_auto_20200731_0443.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0009_familymutation_insureemutation.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0010_auto_20200731_0524.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0011_auto_20200807_1309.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0012_policyrenewaldetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0013_auto_20211103_1023.py
--rw-r--r--   0 runner    (1001) docker     (127)     9118 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0014_add_missing_fields_to_django_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0015_set_managed_to_true_in_all_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0016_alter_jsonext_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0017_auto_20230923_2238.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0018_confirmationtype_is_confirmation_number_required.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/0019_auto_20231026_1205.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17640 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:40.351298 openimis-be-insuree-1.6.0/insuree/reports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53577 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/reports/enrolled_families.py
--rw-r--r--   0 runner    (1001) docker     (127)    52789 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/reports/insuree_family_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)    65100 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/reports/insuree_missing_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)    38213 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/reports/insurees_pending_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (127)    19986 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    18386 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/services.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:40.351298 openimis-be-insuree-1.6.0/insuree/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10331 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/tests/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/tests/test_insuree_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/tests/test_insuree_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-16 00:56:32.000000 openimis-be-insuree-1.6.0/insuree/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:40.351298 openimis-be-insuree-1.6.0/openimis_be_insuree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2023-12-16 00:56:40.000000 openimis-be-insuree-1.6.0/openimis_be_insuree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2023-12-16 00:56:40.000000 openimis-be-insuree-1.6.0/openimis_be_insuree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:56:40.000000 openimis-be-insuree-1.6.0/openimis_be_insuree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-16 00:56:40.000000 openimis-be-insuree-1.6.0/openimis_be_insuree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-16 00:56:40.000000 openimis-be-insuree-1.6.0/openimis_be_insuree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:56:40.351298 openimis-be-insuree-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2023-12-16 00:56:39.000000 openimis-be-insuree-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:01:04.036430 openimis_be_insuree-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-30 09:01:04.036430 openimis_be_insuree-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:01:04.028430 openimis_be_insuree-1.7.0/insuree/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:01:04.028430 openimis_be_insuree-1.7.0/insuree/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:01:04.028430 openimis_be_insuree-1.7.0/insuree/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/management/commands/generateinsurees.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:01:04.032430 openimis_be_insuree-1.7.0/insuree/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0002_family_familytype_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0003_insureepolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0004_confirmationtype_education_profession_relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0005_identificationtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0006_auto_20200722_0839.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0007_auto_20200722_0940.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0008_auto_20200731_0443.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0009_familymutation_insureemutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0010_auto_20200731_0524.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0011_auto_20200807_1309.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0012_policyrenewaldetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0013_auto_20211103_1023.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0014_add_missing_fields_to_django_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0015_set_managed_to_true_in_all_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0016_alter_jsonext_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0017_auto_20230923_2238.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0018_confirmationtype_is_confirmation_number_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/0019_auto_20231026_1205.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17658 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:01:04.032430 openimis_be_insuree-1.7.0/insuree/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55276 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/reports/enrolled_families.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52789 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/reports/insuree_family_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65100 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/reports/insuree_missing_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38213 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/reports/insurees_pending_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20316 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20281 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6616 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:01:04.036430 openimis_be_insuree-1.7.0/insuree/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/tests/test_insuree_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/tests/test_insuree_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 09:00:54.000000 openimis_be_insuree-1.7.0/insuree/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:01:04.036430 openimis_be_insuree-1.7.0/openimis_be_insuree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-30 09:01:03.000000 openimis_be_insuree-1.7.0/openimis_be_insuree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-30 09:01:04.000000 openimis_be_insuree-1.7.0/openimis_be_insuree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:01:03.000000 openimis_be_insuree-1.7.0/openimis_be_insuree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 09:01:03.000000 openimis_be_insuree-1.7.0/openimis_be_insuree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 09:01:03.000000 openimis_be_insuree-1.7.0/openimis_be_insuree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:01:04.036430 openimis_be_insuree-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-30 09:01:03.000000 openimis_be_insuree-1.7.0/setup.py
```

### Comparing `openimis-be-insuree-1.6.0/LICENSE.md` & `openimis_be_insuree-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/PKG-INFO` & `openimis_be_insuree-1.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-insuree
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Insuree reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-insuree-1.6.0/README.md` & `openimis_be_insuree-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/apps.py` & `openimis_be_insuree-1.7.0/insuree/apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "validation_code_invalid_insuree_number_len": 3,
     "validation_code_invalid_insuree_number_checksum": 4,
     "validation_code_invalid_insuree_number_exception": 5,
     "validation_code_validator_import_error": 6,
     "validation_code_validator_function_error": 7,
     "insuree_fsp_mandatory": False,
     "insuree_as_worker": False,
-
+    "is_insuree_photo_required": False,
 }
 
 
 class InsureeConfig(AppConfig):
     name = MODULE_NAME
 
     gql_query_insurees_perms = []
@@ -70,14 +70,15 @@
     renewal_photo_age_adult = None
     renewal_photo_age_child = None
     insuree_number_validator = None
     insuree_number_length = None
     insuree_number_modulo_root = None
     insuree_fsp_mandatory = None
     insuree_as_worker = None
+    is_insuree_photo_required = None
 
     def __load_config(self, cfg):
         for field in cfg:
             if hasattr(InsureeConfig, field):
                 setattr(InsureeConfig, field, cfg[field])
 
     def ready(self):
```

### Comparing `openimis-be-insuree-1.6.0/insuree/dataloaders.py` & `openimis_be_insuree-1.7.0/insuree/dataloaders.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/gql_mutations.py` & `openimis_be_insuree-1.7.0/insuree/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/gql_queries.py` & `openimis_be_insuree-1.7.0/insuree/gql_queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,16 @@
         model = Relation
         filter_fields = {
             "code": ["exact"]
         }
 
 
 class InsureeStatusReasonGQLType(DjangoObjectType):
+    status_type = graphene.String(required=False)
+
     class Meta:
         model = InsureeStatusReason
         interfaces = (graphene.relay.Node,)
         filter_fields = {
             "code": ["exact"],
             "insuree_status_reason": ["exact", 'icontains', 'istartswith'],
             "status_type": ["exact"]
@@ -152,14 +154,15 @@
             "gender__code": ["exact", "isnull"],
             "marital": ["exact", "isnull"],
             "status": ["exact"],
             "validity_from": ["exact", "lt", "lte", "gt", "gte", "isnull"],
             "validity_to": ["exact", "lt", "lte", "gt", "gte", "isnull"],
             **prefix_filterset("photo__", PhotoGQLType._meta.filter_fields),
             "photo": ["isnull"],
+            "family": ["isnull"],
             **prefix_filterset("gender__", GenderGQLType._meta.filter_fields)
         }
         interfaces = (graphene.relay.Node,)
         connection_class = ExtendedConnection
 
     def resolve_client_mutation_id(self, info):
         if not info.context.user.has_perms(InsureeConfig.gql_query_insuree_perms):
```

### Comparing `openimis-be-insuree-1.6.0/insuree/management/commands/generateinsurees.py` & `openimis_be_insuree-1.7.0/insuree/management/commands/generateinsurees.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0001_initial.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0002_family_familytype_photo.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0002_family_familytype_photo.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0003_insureepolicy.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0003_insureepolicy.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0004_confirmationtype_education_profession_relation.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0004_confirmationtype_education_profession_relation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0005_identificationtype.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0005_identificationtype.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0007_auto_20200722_0940.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0007_auto_20200722_0940.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0009_familymutation_insureemutation.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0009_familymutation_insureemutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0010_auto_20200731_0524.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0010_auto_20200731_0524.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0011_auto_20200807_1309.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0011_auto_20200807_1309.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0012_policyrenewaldetail.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0012_policyrenewaldetail.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0013_auto_20211103_1023.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0013_auto_20211103_1023.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0014_add_missing_fields_to_django_scheme.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0014_add_missing_fields_to_django_scheme.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0015_set_managed_to_true_in_all_models.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0015_set_managed_to_true_in_all_models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0016_alter_jsonext_column.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0016_alter_jsonext_column.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0017_auto_20230923_2238.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0017_auto_20230923_2238.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/migrations/0019_auto_20231026_1205.py` & `openimis_be_insuree-1.7.0/insuree/migrations/0019_auto_20231026_1205.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/models.py` & `openimis_be_insuree-1.7.0/insuree/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,16 +352,16 @@
         if isinstance(user, ResolveInfo):
             user = user.context.user
         if settings.ROW_SECURITY and user.is_anonymous:
             return queryset.filter(id=-1)
         if settings.ROW_SECURITY and not user.is_imis_admin:
                         # Limit the list by the logged in user location mapping
             return queryset.filter(                
-                Q(LocationManager().build_user_location_filter_query(user._u, prefix='current_village__parent__parent', loc_types=['D']) |
-                    LocationManager().build_user_location_filter_query(user._u, prefix='family__location__parent__parent', loc_types=['D']))
+                Q(LocationManager().build_user_location_filter_query(user._u, prefix='insuree__current_village__parent__parent', loc_types=['D']) |
+                    LocationManager().build_user_location_filter_query(user._u, prefix='insuree__family__location__parent__parent', loc_types=['D']))
             )
  
         return queryset
 
     class Meta:
         managed = True
         db_table = 'tblInsureePolicy'
```

### Comparing `openimis-be-insuree-1.6.0/insuree/report.py` & `openimis_be_insuree-1.7.0/insuree/report.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/reports/enrolled_families.py` & `openimis_be_insuree-1.7.0/insuree/reports/insuree_family_overview.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from report.services import run_stored_proc_report
+from django.conf import settings
+from django.db.models import Q, F
 
 # If manually pasting from reportbro and you have test data, search and replace \" with \\"
 template = """
 {
   "docElements": [
     {
       "elementType": "text",
       "id": 3,
       "containerId": "0_header",
       "x": 0,
       "y": 20,
       "width": 575,
       "height": 40,
-      "content": "Enrollment Report",
+      "content": "Families and Insurees",
       "eval": false,
       "styleId": "",
       "bold": true,
       "italic": false,
       "underline": false,
       "strikethrough": false,
       "horizontalAlignment": "center",
@@ -369,15 +370,15 @@
           "printIf": "",
           "alwaysPrintOnSamePage": true,
           "columnData": [
             {
               "elementType": "table_text",
               "id": 258,
               "width": 160,
-              "content": "${DistrictName}",
+              "content": "${district}",
               "eval": false,
               "colspan": "4",
               "styleId": "33",
               "bold": true,
               "italic": false,
               "underline": false,
               "strikethrough": false,
@@ -557,15 +558,15 @@
           "printIf": "",
           "alwaysPrintOnSamePage": true,
           "columnData": [
             {
               "elementType": "table_text",
               "id": 253,
               "width": 160,
-              "content": "   ${WardName}",
+              "content": "   ${ward}",
               "eval": false,
               "colspan": "4",
               "styleId": "33",
               "bold": true,
               "italic": false,
               "underline": false,
               "strikethrough": false,
@@ -745,15 +746,15 @@
           "printIf": "",
           "alwaysPrintOnSamePage": true,
           "columnData": [
             {
               "elementType": "table_text",
               "id": 246,
               "width": 160,
-              "content": "      ${VillageName}",
+              "content": "      ${village}",
               "eval": false,
               "colspan": "4",
               "styleId": "33",
               "bold": true,
               "italic": false,
               "underline": false,
               "strikethrough": false,
@@ -933,15 +934,15 @@
           "printIf": "",
           "alwaysPrintOnSamePage": false,
           "columnData": [
             {
               "elementType": "table_text",
               "id": 200,
               "width": 160,
-              "content": "${CHFID}",
+              "content": "${chf_id}",
               "eval": false,
               "colspan": "",
               "styleId": "",
               "bold": false,
               "italic": false,
               "underline": false,
               "strikethrough": false,
@@ -977,15 +978,15 @@
               "cs_paddingBottom": 2,
               "borderWidth": 1
             },
             {
               "elementType": "table_text",
               "id": 208,
               "width": 175,
-              "content": "${OtherNames} + ' ' + ${LastName}",
+              "content": "${other_names} + ' ' + ${last_name}",
               "eval": true,
               "colspan": "",
               "styleId": "",
               "bold": false,
               "italic": false,
               "underline": false,
               "strikethrough": false,
@@ -1021,15 +1022,15 @@
               "cs_paddingBottom": 2,
               "borderWidth": 1
             },
             {
               "elementType": "table_text",
               "id": 209,
               "width": 168,
-              "content": "${EnrolDate}",
+              "content": "${enroll_date}",
               "eval": false,
               "colspan": "",
               "styleId": "",
               "bold": false,
               "italic": false,
               "underline": false,
               "strikethrough": false,
@@ -1065,15 +1066,15 @@
               "cs_paddingBottom": 2,
               "borderWidth": 1
             },
             {
               "elementType": "table_text",
               "id": 240,
               "width": 71,
-              "content": "${PolicyStatusDesc}",
+              "content": "${status}",
               "eval": false,
               "colspan": "",
               "styleId": "",
               "bold": false,
               "italic": false,
               "underline": false,
               "strikethrough": false,
@@ -1475,15 +1476,15 @@
       "type": "array",
       "arrayItemType": "string",
       "eval": false,
       "nullable": false,
       "pattern": "",
       "expression": "",
       "showOnlyNameType": false,
-      "testData": "[{\\"FamilyID\\":\\"1234567\\",\\"LocationId\\":\\"123\\",\\"RegionName\\":\\"Reg\\",\\"DistrictName\\":\\"Dist\\",\\"WardName\\":\\"Wrd\\",\\"VillageName\\":\\"Vil\\",\\"IsHead\\":\\"1\\",\\"CHFID\\":\\"132434654\\",\\"LastName\\":\\"Doe\\",\\"OtherNames\\":\\"John\\",\\"EnrolDate\\":\\"2022-01-01\\",\\"PolicyStatus\\":\\"1\\",\\"PolicyStatusDesc\\":\\"READY\\"}]",
+      "testData": "[{\\"chf_id\\":\\"1234567\\",\\"other_names\\":\\"oth\\",\\"last_name\\":\\"last\\",\\"enroll_date\\":\\"2022-01-01\\",\\"status\\":\\"READY\\",\\"village\\":\\"foo\\",\\"ward\\":\\"bar\\",\\"district\\":\\"klet\\"}]",
       "children": [
         {
           "id": 234,
           "name": "row_number",
           "type": "number",
           "arrayItemType": "string",
           "eval": false,
@@ -1491,159 +1492,99 @@
           "pattern": "",
           "expression": "",
           "showOnlyNameType": true,
           "testData": ""
         },
         {
           "id": 235,
-          "name": "FamilyID",
-          "type": "number",
+          "name": "chf_id",
+          "type": "string",
           "arrayItemType": "string",
           "eval": false,
           "nullable": true,
           "pattern": "",
           "expression": "",
           "showOnlyNameType": false,
           "testData": ""
         },
         {
           "id": 236,
-          "name": "LocationId",
-          "type": "number",
+          "name": "other_names",
+          "type": "string",
           "arrayItemType": "string",
           "eval": false,
           "nullable": true,
           "pattern": "",
           "expression": "",
           "showOnlyNameType": false,
           "testData": ""
         },
         {
           "id": 262,
-          "name": "RegionName",
+          "name": "last_name",
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
           "id": 237,
-          "name": "DistrictName",
-          "type": "string",
+          "name": "enroll_date",
+          "type": "date",
           "arrayItemType": "string",
           "eval": false,
           "nullable": true,
           "pattern": "",
           "expression": "",
           "showOnlyNameType": false,
           "testData": ""
         },
         {
           "id": 242,
-          "name": "WardName",
+          "name": "status",
           "type": "string",
           "arrayItemType": "string",
           "eval": false,
           "nullable": true,
           "pattern": "",
           "expression": "",
           "showOnlyNameType": false,
           "testData": ""
         },
         {
           "id": 244,
-          "name": "VillageName",
+          "name": "village",
           "type": "string",
           "arrayItemType": "string",
           "eval": false,
           "nullable": true,
           "pattern": "",
           "expression": "",
           "showOnlyNameType": false,
           "testData": ""
         },
         {
           "id": 250,
-          "name": "IsHead",
-          "type": "boolean",
-          "arrayItemType": "string",
-          "eval": false,
-          "nullable": true,
-          "pattern": "",
-          "expression": "",
-          "showOnlyNameType": false,
-          "testData": ""
-        },
-        {
-          "id": 251,
-          "name": "CHFID",
+          "name": "ward",
           "type": "string",
           "arrayItemType": "string",
           "eval": false,
-          "nullable": false,
-          "pattern": "",
-          "expression": "",
-          "showOnlyNameType": false,
-          "testData": ""
-        },
-        {
-          "id": 263,
-          "name": "LastName",
-          "type": "string",
-          "arrayItemType": "string",
-          "eval": false,
-          "nullable": false,
-          "pattern": "",
-          "expression": "",
-          "showOnlyNameType": false,
-          "testData": ""
-        },
-        {
-          "id": 264,
-          "name": "OtherNames",
-          "type": "string",
-          "arrayItemType": "string",
-          "eval": false,
-          "nullable": true,
-          "pattern": "",
-          "expression": "",
-          "showOnlyNameType": false,
-          "testData": ""
-        },
-        {
-          "id": 265,
-          "name": "EnrolDate",
-          "type": "date",
-          "arrayItemType": "string",
-          "eval": false,
           "nullable": true,
           "pattern": "",
           "expression": "",
           "showOnlyNameType": false,
           "testData": ""
         },
         {
-          "id": 266,
-          "name": "PolicyStatus",
-          "type": "number",
-          "arrayItemType": "string",
-          "eval": false,
-          "nullable": true,
-          "pattern": "",
-          "expression": "",
-          "showOnlyNameType": false,
-          "testData": ""
-        },
-        {
-          "id": 267,
-          "name": "PolicyStatusDesc",
+          "id": 251,
+          "name": "district",
           "type": "string",
           "arrayItemType": "string",
           "eval": false,
           "nullable": true,
           "pattern": "",
           "expression": "",
           "showOnlyNameType": false,
@@ -1750,21 +1691,40 @@
     "footer": true,
     "footerSize": "30",
     "footerDisplay": "always",
     "patternLocale": "en",
     "patternCurrencySymbol": "$"
   }
 }
-
 """
 
 
-def enrolled_families_query(user, date_from=None, date_to=None, location_id=None, **kwargs):
-    data = run_stored_proc_report(
-        "uspSSRSEnroledFamilies",
-        LocationId=location_id,
-        StartDate=date_from,
-        EndDate=date_to,
+def insuree_family_overview_query(user, date_from=None, date_to=None, **kwargs):
+    from ..models import Insuree
+    from core import datetimedelta
+
+    filters = Q(legacy_id__isnull=True) & Q(family__legacy_id__isnull=True)
+    # TODO verify that we should use the validity_from and not the enrolment_date
+    # TODO verify the day+1 approach
+    if date_from:
+        filters &= Q(validity_from__gte=date_from)
+    if date_to:
+        filters &= Q(validity_from__lte=date_to + datetimedelta(days=1))
+    queryset = Insuree.objects
+    if settings.ROW_SECURITY:
+        from location.models import LocationManager
+        queryset = LocationManager().build_user_location_filter_query(user._u, queryset = queryset, loc_types = ['V'] )   
+    queryset = (
+        queryset.filter(filters)
+        .values(
+            "chf_id",
+            "other_names",
+            "last_name",
+            enroll_date=F("validity_from"),
+            village=F("family__location__name"),
+            ward=F("family__location__parent__name"),
+            district=F("family__location__parent__parent__name"),
+        )
+        .order_by("district", "ward", "village", "chf_id")
     )
-    return {
-        "data": data
-    }
+
+    return {"data": list(queryset)}
```

### Comparing `openimis-be-insuree-1.6.0/insuree/reports/insuree_family_overview.py` & `openimis_be_insuree-1.7.0/insuree/reports/enrolled_families.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-from django.conf import settings
-from django.db.models import Q, F
+from insuree.models import Family, Insuree
+from report.services import run_stored_proc_report
+from django.db.models import F, Case, When, Value
+from django.db.models.functions import Cast, Rank
+from django.db.models.expressions import Window
 
 # If manually pasting from reportbro and you have test data, search and replace \" with \\"
 template = """
 {
   "docElements": [
     {
       "elementType": "text",
       "id": 3,
       "containerId": "0_header",
       "x": 0,
       "y": 20,
       "width": 575,
       "height": 40,
-      "content": "Families and Insurees",
+      "content": "Enrollment Report",
       "eval": false,
       "styleId": "",
       "bold": true,
       "italic": false,
       "underline": false,
       "strikethrough": false,
       "horizontalAlignment": "center",
@@ -370,15 +373,15 @@
           "printIf": "",
           "alwaysPrintOnSamePage": true,
           "columnData": [
             {
               "elementType": "table_text",
               "id": 258,
               "width": 160,
-              "content": "${district}",
+              "content": "${DistrictName}",
               "eval": false,
               "colspan": "4",
               "styleId": "33",
               "bold": true,
               "italic": false,
               "underline": false,
               "strikethrough": false,
@@ -558,15 +561,15 @@
           "printIf": "",
           "alwaysPrintOnSamePage": true,
           "columnData": [
             {
               "elementType": "table_text",
               "id": 253,
               "width": 160,
-              "content": "   ${ward}",
+              "content": "   ${WardName}",
               "eval": false,
               "colspan": "4",
               "styleId": "33",
               "bold": true,
               "italic": false,
               "underline": false,
               "strikethrough": false,
@@ -746,15 +749,15 @@
           "printIf": "",
           "alwaysPrintOnSamePage": true,
           "columnData": [
             {
               "elementType": "table_text",
               "id": 246,
               "width": 160,
-              "content": "      ${village}",
+              "content": "      ${VillageName}",
               "eval": false,
               "colspan": "4",
               "styleId": "33",
               "bold": true,
               "italic": false,
               "underline": false,
               "strikethrough": false,
@@ -934,15 +937,15 @@
           "printIf": "",
           "alwaysPrintOnSamePage": false,
           "columnData": [
             {
               "elementType": "table_text",
               "id": 200,
               "width": 160,
-              "content": "${chf_id}",
+              "content": "${CHFID}",
               "eval": false,
               "colspan": "",
               "styleId": "",
               "bold": false,
               "italic": false,
               "underline": false,
               "strikethrough": false,
@@ -978,15 +981,15 @@
               "cs_paddingBottom": 2,
               "borderWidth": 1
             },
             {
               "elementType": "table_text",
               "id": 208,
               "width": 175,
-              "content": "${other_names} + ' ' + ${last_name}",
+              "content": "${OtherNames} + ' ' + ${LastName}",
               "eval": true,
               "colspan": "",
               "styleId": "",
               "bold": false,
               "italic": false,
               "underline": false,
               "strikethrough": false,
@@ -1022,15 +1025,15 @@
               "cs_paddingBottom": 2,
               "borderWidth": 1
             },
             {
               "elementType": "table_text",
               "id": 209,
               "width": 168,
-              "content": "${enroll_date}",
+              "content": "${EnrolDate}",
               "eval": false,
               "colspan": "",
               "styleId": "",
               "bold": false,
               "italic": false,
               "underline": false,
               "strikethrough": false,
@@ -1041,15 +1044,15 @@
               "font": "helvetica",
               "fontSize": 12,
               "lineSpacing": 1,
               "paddingLeft": 2,
               "paddingTop": 2,
               "paddingRight": 2,
               "paddingBottom": 2,
-              "pattern": "yyyy/MM/dd",
+              "pattern": "dd/MM/yyyy",
               "link": "",
               "cs_condition": "",
               "cs_styleId": "",
               "cs_bold": false,
               "cs_italic": false,
               "cs_underline": false,
               "cs_strikethrough": false,
@@ -1066,15 +1069,15 @@
               "cs_paddingBottom": 2,
               "borderWidth": 1
             },
             {
               "elementType": "table_text",
               "id": 240,
               "width": 71,
-              "content": "${status}",
+              "content": "${PolicyStatusDesc}",
               "eval": false,
               "colspan": "",
               "styleId": "",
               "bold": false,
               "italic": false,
               "underline": false,
               "strikethrough": false,
@@ -1476,15 +1479,15 @@
       "type": "array",
       "arrayItemType": "string",
       "eval": false,
       "nullable": false,
       "pattern": "",
       "expression": "",
       "showOnlyNameType": false,
-      "testData": "[{\\"chf_id\\":\\"1234567\\",\\"other_names\\":\\"oth\\",\\"last_name\\":\\"last\\",\\"enroll_date\\":\\"2022-01-01\\",\\"status\\":\\"READY\\",\\"village\\":\\"foo\\",\\"ward\\":\\"bar\\",\\"district\\":\\"klet\\"}]",
+      "testData": "[{\\"FamilyID\\":\\"1234567\\",\\"LocationId\\":\\"123\\",\\"RegionName\\":\\"Reg\\",\\"DistrictName\\":\\"Dist\\",\\"WardName\\":\\"Wrd\\",\\"VillageName\\":\\"Vil\\",\\"IsHead\\":\\"1\\",\\"CHFID\\":\\"132434654\\",\\"LastName\\":\\"Doe\\",\\"OtherNames\\":\\"John\\",\\"EnrolDate\\":\\"2022-01-01\\",\\"PolicyStatus\\":\\"1\\",\\"PolicyStatusDesc\\":\\"READY\\"}]",
       "children": [
         {
           "id": 234,
           "name": "row_number",
           "type": "number",
           "arrayItemType": "string",
           "eval": false,
@@ -1492,99 +1495,159 @@
           "pattern": "",
           "expression": "",
           "showOnlyNameType": true,
           "testData": ""
         },
         {
           "id": 235,
-          "name": "chf_id",
-          "type": "string",
+          "name": "FamilyID",
+          "type": "number",
           "arrayItemType": "string",
           "eval": false,
           "nullable": true,
           "pattern": "",
           "expression": "",
           "showOnlyNameType": false,
           "testData": ""
         },
         {
           "id": 236,
-          "name": "other_names",
-          "type": "string",
+          "name": "LocationId",
+          "type": "number",
           "arrayItemType": "string",
           "eval": false,
           "nullable": true,
           "pattern": "",
           "expression": "",
           "showOnlyNameType": false,
           "testData": ""
         },
         {
           "id": 262,
-          "name": "last_name",
+          "name": "RegionName",
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
           "id": 237,
-          "name": "enroll_date",
-          "type": "date",
+          "name": "DistrictName",
+          "type": "string",
           "arrayItemType": "string",
           "eval": false,
           "nullable": true,
           "pattern": "",
           "expression": "",
           "showOnlyNameType": false,
           "testData": ""
         },
         {
           "id": 242,
-          "name": "status",
+          "name": "WardName",
           "type": "string",
           "arrayItemType": "string",
           "eval": false,
           "nullable": true,
           "pattern": "",
           "expression": "",
           "showOnlyNameType": false,
           "testData": ""
         },
         {
           "id": 244,
-          "name": "village",
+          "name": "VillageName",
           "type": "string",
           "arrayItemType": "string",
           "eval": false,
           "nullable": true,
           "pattern": "",
           "expression": "",
           "showOnlyNameType": false,
           "testData": ""
         },
         {
           "id": 250,
-          "name": "ward",
-          "type": "string",
+          "name": "IsHead",
+          "type": "boolean",
           "arrayItemType": "string",
           "eval": false,
           "nullable": true,
           "pattern": "",
           "expression": "",
           "showOnlyNameType": false,
           "testData": ""
         },
         {
           "id": 251,
-          "name": "district",
+          "name": "CHFID",
+          "type": "string",
+          "arrayItemType": "string",
+          "eval": false,
+          "nullable": false,
+          "pattern": "",
+          "expression": "",
+          "showOnlyNameType": false,
+          "testData": ""
+        },
+        {
+          "id": 263,
+          "name": "LastName",
+          "type": "string",
+          "arrayItemType": "string",
+          "eval": false,
+          "nullable": false,
+          "pattern": "",
+          "expression": "",
+          "showOnlyNameType": false,
+          "testData": ""
+        },
+        {
+          "id": 264,
+          "name": "OtherNames",
+          "type": "string",
+          "arrayItemType": "string",
+          "eval": false,
+          "nullable": true,
+          "pattern": "",
+          "expression": "",
+          "showOnlyNameType": false,
+          "testData": ""
+        },
+        {
+          "id": 265,
+          "name": "EnrolDate",
+          "type": "date",
+          "arrayItemType": "string",
+          "eval": false,
+          "nullable": true,
+          "pattern": "",
+          "expression": "",
+          "showOnlyNameType": false,
+          "testData": ""
+        },
+        {
+          "id": 266,
+          "name": "PolicyStatus",
+          "type": "number",
+          "arrayItemType": "string",
+          "eval": false,
+          "nullable": true,
+          "pattern": "",
+          "expression": "",
+          "showOnlyNameType": false,
+          "testData": ""
+        },
+        {
+          "id": 267,
+          "name": "PolicyStatusDesc",
           "type": "string",
           "arrayItemType": "string",
           "eval": false,
           "nullable": true,
           "pattern": "",
           "expression": "",
           "showOnlyNameType": false,
@@ -1691,40 +1754,59 @@
     "footer": true,
     "footerSize": "30",
     "footerDisplay": "always",
     "patternLocale": "en",
     "patternCurrencySymbol": "$"
   }
 }
+
 """
 
 
-def insuree_family_overview_query(user, date_from=None, date_to=None, **kwargs):
-    from ..models import Insuree
-    from core import datetimedelta
+def enrolled_families_query(user, dateFrom=None, dateTo=None, locationId=None, **kwargs):
 
-    filters = Q(legacy_id__isnull=True) & Q(family__legacy_id__isnull=True)
-    # TODO verify that we should use the validity_from and not the enrolment_date
-    # TODO verify the day+1 approach
-    if date_from:
-        filters &= Q(validity_from__gte=date_from)
-    if date_to:
-        filters &= Q(validity_from__lte=date_to + datetimedelta(days=1))
-    queryset = Insuree.objects
-    if settings.ROW_SECURITY:
-        from location.models import LocationManager
-        queryset = LocationManager().build_user_location_filter_query(user._u, queryset = queryset, loc_types = ['V'] )   
-    queryset = (
-        queryset.filter(filters)
-        .values(
-            "chf_id",
-            "other_names",
-            "last_name",
-            enroll_date=F("validity_from"),
-            village=F("family__location__name"),
-            ward=F("family__location__parent__name"),
-            district=F("family__location__parent__parent__name"),
+    report_data = Insuree.objects.filter(
+        family__location_id=locationId,
+        validity_to__isnull=True,
+        validity_from__date__range=(dateFrom, dateTo),
+        family__location__parent__parent__parent__validity_to__isnull=True,
+        family__location__parent__parent__validity_to__isnull=True,
+        family__location__parent__validity_to__isnull=True,
+        family__location__validity_to__isnull=True,
+        family__policies__validity_to__isnull=True
+    ).annotate(
+        RegionName=F('family__location__parent__parent__parent__name'),
+        DistrictName=F('family__location__parent__parent__name'),
+        WardName=F('family__location__parent__name'),
+        VillageName=F('family__location__name'),
+        IsHead=F('family__head_insuree__head'),
+        CHFID=F('chf_id'),
+        LastName=F('last_name'),
+        OtherNames=F('other_names'),
+        EnrolDate=F('validity_from__date'),
+        PolicyStatusDesc=Case(
+            When(family__policies__status=1, then=Value('Idle')),
+            When(family__policies__status=2, then=Value('Active')),
+            When(family__policies__status=4, then=Value('Suspended')),
+            When(family__policies__status=8, then=Value('Expired'))
+        ),
+        rank=Window(
+            expression=Rank(),
+            partition_by=F('family__id'),
+            order_by=F('family__policies__validity_from').desc()
         )
-        .order_by("district", "ward", "village", "chf_id")
+    ).filter(rank=1).values(
+        'RegionName',
+        'DistrictName',
+        'WardName',
+        'VillageName',
+        'IsHead',
+        'CHFID',
+        'LastName',
+        'OtherNames',
+        'EnrolDate',
+        'PolicyStatusDesc'
     )
 
-    return {"data": list(queryset)}
+    return {
+        "data": list(report_data)
+    }
```

### Comparing `openimis-be-insuree-1.6.0/insuree/reports/insuree_missing_photo.py` & `openimis_be_insuree-1.7.0/insuree/reports/insuree_missing_photo.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/reports/insurees_pending_enrollment.py` & `openimis_be_insuree-1.7.0/insuree/reports/insurees_pending_enrollment.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/schema.py` & `openimis_be_insuree-1.7.0/insuree/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import graphene
 
 from claim.apps import ClaimConfig
+from core.gql.export_mixin import ExportableQueryMixin
 from core.schema import signal_mutation_module_validate
 from core.utils import filter_validity
 from django.db.models import Q
 from django.core.exceptions import PermissionDenied
 from django.dispatch import Signal
 from graphene_django.filter import DjangoFilterConnectionField
 import graphene_django_optimizer as gql_optimizer
@@ -54,15 +55,18 @@
                 Q(head_insuree__validity_to__isnull=True), **head_insuree_filters)
         if len(members_filters):
             qs = qs.filter(Q(members__validity_to__isnull=True),
                            **members_filters)
         return OrderedDjangoFilterConnectionField.orderBy(qs, args)
 
 
-class Query(graphene.ObjectType):
+class Query(ExportableQueryMixin, graphene.ObjectType):
+    exportable_fields = ['insurees']
+
+
     can_add_insuree = graphene.Field(
         graphene.List(graphene.String),
         family_id=graphene.Int(required=True),
         description="Checks that the specified family id is allowed to add more insurees (like a Policy limitation)"
     )
     insuree_genders = graphene.List(GenderGQLType)
     insurees = OrderedDjangoFilterConnectionField(
@@ -271,15 +275,16 @@
             for i in range(len(LocationConfig.location_types) - parent_location_level - 1):
                 f = "parent__" + f
             f = "location__" + f
             filters += [Q(**{f: parent_location})]
 
         # Limit the list by the logged in user location mapping
         if not info.context.user._u.is_imis_admin:
-            filters += [LocationManager().build_user_location_filter_query(info.context.user._u, prefix= 'location__parent__parent', loc_types = ['D'])]
+            filters += [LocationManager().build_user_location_filter_query(info.context.user._u,
+                                                                           prefix='location__parent__parent', loc_types=['D'])]
 
         # Duplicates cannot be removed with distinct, as TEXT field is not comparable
         ids = Family.objects.filter(*filters).values_list('id')
         dinstinct_queryset = Family.objects.filter(id__in=ids)
         return gql_optimizer.query(dinstinct_queryset.all(), info)
 
     def resolve_insuree_officers(self, info, **kwargs):
@@ -307,18 +312,18 @@
             parent_location_level = kwargs.get('parent_location_level')
             if parent_location_level is None:
                 raise NotImplementedError(
                     "Missing parentLocationLevel argument when filtering on parentLocation")
             f = "uuid"
             for i in range(len(LocationConfig.location_types) - parent_location_level - 1):
                 f = "parent__" + f
-            current_village = "current_village__" + f
-            family_location = "family__location__" + f
-            filters += [(Q(current_village__isnull=False) & Q(**{current_village: parent_location})) |
-                        (Q(current_village__isnull=True) & Q(**{family_location: parent_location}))]
+            current_village = "insuree__current_village__" + f
+            family_location = "insuree__family__location__" + f
+            filters += [(Q(insuree__current_village__isnull=False) & Q(**{current_village: parent_location})) |
+                        (Q(insuree__current_village__isnull=True) & Q(**{family_location: parent_location}))]
         return gql_optimizer.query(InsureePolicy.objects.filter(*filters).all(), info)
 
 
 class Mutation(graphene.ObjectType):
     create_family = CreateFamilyMutation.Field()
     update_family = UpdateFamilyMutation.Field()
     delete_families = DeleteFamiliesMutation.Field()
@@ -409,27 +414,32 @@
 
 
 def bind_signals():
     signal_mutation_module_validate["insuree"].connect(on_mutation)
 
 
 def _insuree_additional_filters(sender, additional_filter, user):
-    return _get_additional_filter(sender, additional_filter, user, signal_before_insuree_policy_query)
+    return _get_additional_filter(sender or Insuree, additional_filter, user, signal_before_insuree_policy_query)
+
 
 def _insuree_insuree_additional_filters(sender, additional_filter, user):
-    return _get_additional_filter(sender, additional_filter, user, signal_before_insuree_search_query)
+    return _get_additional_filter(sender or InsureePolicy, additional_filter, user, signal_before_insuree_search_query)
 
 
 def _family_additional_filters(sender, additional_filter, user):
-    return _get_additional_filter(sender, additional_filter, user, signal_before_family_query)
+    return _get_additional_filter(sender or Family, additional_filter, user, signal_before_family_query)
 
 
 def _get_additional_filter(sender, additional_filter, user, signal: Signal):
     # function to retrieve additional filters from signal
     filters_from_signal = []
+
+    if sender is None:
+        raise Exception("Missing sender")
+
     if additional_filter:
         # send signal to append additional filter
         results_signal = signal.send(
             sender=sender, additional_filter=additional_filter, user=user,
         )
         filters_from_signal = _read_signal_results(results_signal)
     return filters_from_signal
```

### Comparing `openimis-be-insuree-1.6.0/insuree/services.py` & `openimis_be_insuree-1.7.0/insuree/services.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 from django.utils.translation import gettext as _
 
 from core.signals import register_service_signal
 from insuree.apps import InsureeConfig
 from insuree.models import (InsureePhoto, PolicyRenewalDetail, Insuree, Family, InsureePolicy, InsureeStatus,
                             InsureeStatusReason)
 from django.core.exceptions import ValidationError
-from core.models import filter_validity
+from core.models import filter_validity, resolved_id_reference
 
 logger = logging.getLogger(__name__)
 
 
 def create_insuree_renewal_detail(policy_renewal):
     from core import datetime, datetimedelta
     now = datetime.datetime.now()
     adult_birth_date = now - datetimedelta(years=CoreConfig.age_of_majority)
     photo_renewal_date_adult = now - \
-                               datetimedelta(months=InsureeConfig.renewal_photo_age_adult)  # 60
+        datetimedelta(months=InsureeConfig.renewal_photo_age_adult)  # 60
     photo_renewal_date_child = now - \
-                               datetimedelta(months=InsureeConfig.renewal_photo_age_child)  # 12
+        datetimedelta(months=InsureeConfig.renewal_photo_age_child)  # 12
     photos_to_renew = InsureePhoto.objects.filter(insuree__family=policy_renewal.insuree.family) \
         .filter(insuree__validity_to__isnull=True) \
         .filter(Q(insuree__photo_date__isnull=True)
                 | Q(insuree__photo_date__lte=photo_renewal_date_adult)
                 | (Q(insuree__photo_date__lte=photo_renewal_date_child)
                    & Q(insuree__dob__gt=adult_birth_date)
                    )
@@ -59,19 +59,19 @@
                  "message": _("validator_module_import_error")}]
 
     except AttributeError:
         return [{"errorCode": InsureeConfig.validation_code_validator_function_error,
                  "message": _("validator_function_not_found")}]
 
 
-def validate_insuree_number(insuree_number, uuid=None):
+def validate_insuree_number(insuree_number, insuree_uuid=None):
     query = Insuree.objects.filter(
         chf_id=insuree_number, validity_to__isnull=True)
     insuree = query.first()
-    if insuree and str(insuree.uuid) != str(uuid):
+    if insuree_uuid and insuree and uuid.UUID(insuree.uuid) != uuid.UUID(insuree_uuid):
         return [{"errorCode": InsureeConfig.validation_code_taken_insuree_number,
                  "message": "Insuree number has to be unique, %s exists in system" % insuree_number}]
 
     if InsureeConfig.get_insuree_number_validator():
         return custom_insuree_number_validation(insuree_number)
     if InsureeConfig.get_insuree_number_length():
         if not insuree_number:
@@ -168,19 +168,19 @@
     insuree_photo = None
     if not photo_changed(existing_insuree_photo, data):
         return None
     data['audit_user_id'] = user.id_for_audit
     data['validity_from'] = now
     data['insuree_id'] = insuree.id
     if 'uuid' not in data or (existing_insuree_photo and data['uuid'] == existing_insuree_photo.uuid):
-        data['uuid'] =  str(uuid.uuid4())
+        data['uuid'] = str(uuid.uuid4())
     photo_bin = data.get('photo', None)
     if photo_bin and InsureeConfig.insuree_photos_root_path \
             and (existing_insuree_photo is None or existing_insuree_photo.photo != photo_bin):
-        (file_dir, file_name) = create_file(now, insuree.id, photo_bin,data['uuid'] )
+        (file_dir, file_name) = create_file(now, insuree.id, photo_bin, data['uuid'])
         data['folder'] = file_dir
         data['filename'] = file_name
         insuree_photo = InsureePhoto(**data)
 
     if existing_insuree_photo and insuree_photo:
         existing_insuree_photo.save_history()
         insuree_photo.id = existing_insuree_photo.id
@@ -211,15 +211,15 @@
 
 def _create_dir(file_dir):
     root = InsureeConfig.insuree_photos_root_path
     pathlib.Path(path.join(root, file_dir)) \
         .mkdir(parents=True, exist_ok=True)
 
 
-def create_file(date, insuree_id, photo_bin, name ):
+def create_file(date, insuree_id, photo_bin, name):
     file_dir = path.join(str(date.year), str(date.month),
                          str(date.day), str(insuree_id))
     file_name = name
 
     _create_dir(file_dir)
     with open(_photo_dir(file_dir, file_name), "xb") as f:
         f.write(base64.b64decode(photo_bin))
@@ -292,52 +292,79 @@
         from core import datetime
         now = datetime.datetime.now()
         data['audit_user_id'] = self.user.id_for_audit
         data['validity_from'] = now
         status = data.get('status', InsureeStatus.ACTIVE)
         if status not in [choice[0] for choice in InsureeStatus.choices]:
             raise ValidationError(_("mutation.insuree.wrong_status"))
+        if InsureeConfig.is_insuree_photo_required and photo_data is None:
+            raise ValidationError(_("mutation.insuree.no_required_photo"))
         if status in [InsureeStatus.INACTIVE, InsureeStatus.DEAD]:
             status_reason = InsureeStatusReason.objects.get(code=data.get('status_reason', None),
                                                             validity_to__isnull=True)
             if status_reason is None or status_reason.status_type != status:
                 raise ValidationError(_("mutation.insuree.wrong_status"))
             data['status_reason'] = status_reason
+            if "uuid" in data:
+                insuree = Insuree.objects.get(uuid=data["uuid"])
+                self.disable_policies_of_insuree(insuree=insuree, status_date=data['status_date'])
+        elif "uuid" in data:
+            insuree = Insuree.objects.filter(uuid=data["uuid"]).first()
+            if not insuree:
+                insuree = Insuree.objects.create(**data)
+            self.activate_policies_of_insuree(insuree, audit_user_id=data['audit_user_id'])
         if InsureeConfig.insuree_fsp_mandatory and 'health_facility_id' not in data:
             raise ValidationError("mutation.insuree.fsp_required")
-    
+
         insuree = Insuree(**data)
         return self._create_or_update(insuree, photo_data)
 
-    
-    def _create_or_update(self, insuree, photo_data = None):    
+    def disable_policies_of_insuree(self, insuree, status_date):
+        policies_to_cancel = InsureePolicy.objects.filter(insuree=insuree.id, validity_to__isnull=True).all()
+        for policy in policies_to_cancel:
+            policy.expiry_date = status_date
+            policy.save()
+
+    def activate_policies_of_insuree(self, insuree, audit_user_id):
+        from core import datetime
+        now = datetime.date.today()
+        from policy.models import Policy
+        policies_to_activate = Policy.objects.filter(family=insuree.family, validity_to__isnull=True)
+        for policy in policies_to_activate:
+            if policy.expiry_date >= now:
+                current_policy_dict = {"effective_date": now, "expiry_date": policy.expiry_date,
+                                       "audit_user_id": audit_user_id, "offline": policy.offline,
+                                       "start_date": policy.start_date, "policy": policy, "insuree": insuree,
+                                       "enrollment_date": policy.enroll_date}
+                current_policy = InsureePolicy(**current_policy_dict)
+                current_policy.save()
+
+    def _create_or_update(self, insuree, photo_data=None):
         validate_insuree(insuree)
         if insuree.id:
-            filters = Q(id = insuree.id )
+            filters = Q(id=insuree.id)
             # remove it from now3 to avoid id at creation
             insuree.id = None
         elif insuree.uuid:
-            filters = Q(uuid = (insuree.uuid) )
+            filters = Q(uuid=(insuree.uuid))
         else:
-            filters = None   
+            filters = None
         existing_insuree = Insuree.objects.filter(filters).prefetch_related(
-                    "photo").first() if filters else None
+            "photo").first() if filters else None
         if existing_insuree:
             existing_insuree.save_history()
             insuree.id = existing_insuree.id
         insuree.save()
         if photo_data:
             photo = handle_insuree_photo(self.user, insuree.validity_from, insuree, photo_data)
             if photo:
                 insuree.photo = photo
                 insuree.photo_date = photo.date
                 insuree.save()
         return insuree
-            
-
 
     def remove(self, insuree):
         try:
             insuree.save_history()
             insuree.family = None
             insuree.save()
             return []
@@ -411,56 +438,61 @@
 
 
 class FamilyService:
     def __init__(self, user):
         self.user = user
 
     def create_or_update(self, data):
-        # this should be in the mutation file
-        head_insuree_data = data.pop('head_insuree')
-        head_insuree_data["head"] = True
-        head_insuree = InsureeService(
-            self.user).create_or_update(head_insuree_data)
-        data["head_insuree"] = head_insuree
+        head_insuree_data = data.pop('head_insuree', None)
+        
+        if head_insuree_data:
+            head_insuree_data["head"] = True
+            head_insuree = InsureeService(
+                self.user).create_or_update(head_insuree_data)
+            data["head_insuree_id"] = head_insuree.id
+        
+        elif 'head_insuree_id' not in data:
+            raise Exception(f'no head insuree found')
         from core import datetime
 
         now = datetime.datetime.now()
 
         data['audit_user_id'] = self.user.id_for_audit
         data['validity_from'] = now
         family = Family(**data)
         return self._create_or_update(family)
-        
+
     def _create_or_update(self, family):
         if family.id:
-            filters = Q(id = family.id )
+            filters = Q(id=family.id)
             # remove it from now3 to avoid id at creation
             family.id = None
         elif family.uuid:
-            filters = Q(uuid = (family.uuid) )
+            filters = Q(uuid=(family.uuid))
         else:
-            filters = None   
-        existing_family = Family.objects.filter(*filter_validity(),filters).first() if filters else None            
+            filters = None
+        existing_family = Family.objects.filter(*filter_validity(), filters).first() if filters else None
         if existing_family:
             return self._update(existing_family, family)
         else:
             return self._create(family)
-        
+
     def _create(self, family):
         family.save()
         family.head_insuree.family = family
         family.head_insuree.save()
         return family
-        
-    def _update(self, existing_family, family):     
+
+    def _update(self, existing_family, family):
         existing_family.save_history()
         family.id = existing_family.id
         family.save()
-        head_insuree.family = family
-        head_insuree.save()
+        if family.head_insuree.family != family:
+            family.head_insuree.family = family
+            family.head_insuree.save()
         return family
 
     def set_deleted(self, family, delete_members):
         try:
             [self.handle_member_on_family_delete(member, delete_members)
              for member in family.members.filter(validity_to__isnull=True).all()]
             family.delete_history()
```

### Comparing `openimis-be-insuree-1.6.0/insuree/signals.py` & `openimis_be_insuree-1.7.0/insuree/signals.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from core.signals import Signal
 
 
 _insuree_policy_before_query_signal_params = ["user", "additional_filter"]
-signal_before_insuree_policy_query = Signal(providing_args=_insuree_policy_before_query_signal_params)
-signal_before_family_query = Signal(providing_args=_insuree_policy_before_query_signal_params)
-signal_before_insuree_search_query = Signal(providing_args=_insuree_policy_before_query_signal_params)
+signal_before_insuree_policy_query = Signal(_insuree_policy_before_query_signal_params)
+signal_before_family_query = Signal(_insuree_policy_before_query_signal_params)
+signal_before_insuree_search_query = Signal(_insuree_policy_before_query_signal_params)
 
 
 def _read_signal_results(result_signal):
     # signal result is a representation of list of tuple (function, result)
     return [result[1] for result in result_signal if result[1] is not None]
```

### Comparing `openimis-be-insuree-1.6.0/insuree/test_helpers.py` & `openimis_be_insuree-1.7.0/insuree/test_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from insuree.apps import InsureeConfig
 from insuree.models import Insuree, Family, Gender, InsureePhoto
 from insuree.services import validate_insuree_number
 from location.models import Location
 import random
-
+import re
+from datetime import datetime
+    
 def create_test_insuree(with_family=True, is_head=False, custom_props=None, family_custom_props=None):
     # insuree has a mandatory reference to family and family has a mandatory reference to insuree
     # So we first insert the family with a dummy id and then update it
     #loof if it exists
     family = None
     location = None
     village = None
@@ -37,15 +39,15 @@
             village=qs_location.first()
     
         family = get_from_custom_props(custom_props, 'family',  None)
         
 
         
         insuree = Insuree.objects.create(
-                last_name = get_from_custom_props(custom_props, 'last_name',"last" ),
+                last_name = get_from_custom_props(custom_props, 'last_name',"Test Last" ),
                 other_names= get_from_custom_props(custom_props, 'other_names', "First Second"),
                 family= family,
                 gender= get_from_custom_props(custom_props, 'gender', Gender.objects.get(code='M')),
                 dob=  get_from_custom_props(custom_props, 'dob', '1972-08-09'),
                 chf_id= ref,
                 head= is_head,
                 card_issued= get_from_custom_props(custom_props, 'card_issued', True),
@@ -102,15 +104,25 @@
 gkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWmp6ipqrKztLW2t7i5usLD
 xMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/8QAHwEAAwEBAQEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ
 3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eH
 l6goOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3uLm6wsPExcbHyMnK0tPU1dbX2Nna4uPk5ebn6Onq8vP09fb3+Pn6/9oADAMBAAIRAxEAPwD3+
 iiigD//2Q==
 """
 def get_from_custom_props( custom_props, elm, default):
-    return custom_props.pop(elm) if custom_props and elm in custom_props else default
+
+    value= custom_props.pop(elm) if custom_props and elm in custom_props else default
+
+    regex = re.compile("^[0-9]{4}-[0-9]{2}-[0-9]{2}$")
+    regex_dt = re.compile("^[0-9]{4}-[0-9]{2}-[0-9]{2}T[0-9]{2}:[0-9]{2}:[0-9]{2}$")
+    if isinstance(value, str) and regex.match(value):
+        value = datetime.strptime(value, "%Y-%m-%d")
+    elif isinstance(value, str) and regex_dt.match(value):
+        value = datetime.strptime(value, "%Y-%m-%dT%H:%M:%S")
+    return value
+    
 
 def create_test_photo(insuree_id, officer_id, custom_props=None):
     photo = InsureePhoto.objects.create(
         **{
             "insuree_id": insuree_id,
             "folder": InsureeConfig.insuree_photos_root_path,
             "officer_id": officer_id,
```

### Comparing `openimis-be-insuree-1.6.0/insuree/tests/test_graphql.py` & `openimis_be_insuree-1.7.0/insuree/tests/test_graphql.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import base64
 import json
+import time
+import uuid
 from dataclasses import dataclass
 from django.utils.translation import gettext as _
 from core.models import User, filter_validity
+from core.models.openimis_graphql_test_case import openIMISGraphQLTestCase
 from core.test_helpers import create_test_interactive_user
 from django.conf import settings
 from graphene_django.utils.testing import GraphQLTestCase
 from graphql_jwt.shortcuts import get_token
 from location.models import Location
 from location.test_helpers import create_test_location, assign_user_districts
 from rest_framework import status
@@ -20,19 +23,17 @@
 
 @dataclass
 class DummyContext:
     """ Just because we need a context to generate. """
     user: User
 
 
-class InsureeGQLTestCase(GraphQLTestCase):
-    GRAPHQL_URL = f'/{settings.SITE_ROOT()}graphql'
-    # This is required by some version of graphene but is never used. It should be set to the schema but the import
-    # is shown as an error in the IDE, so leaving it as True.
-    GRAPHQL_SCHEMA = True
+
+class InsureeGQLTestCase(openIMISGraphQLTestCase):
+
     admin_user = None
     ca_user = None
     ca_token = None
     test_village = None
     test_insuree = None
     test_photo = None
     @classmethod
@@ -194,28 +195,29 @@
 
       content = json.loads(response.content)
 
     # This validates the status code and if you get errors
       self.assertResponseNoErrors(response)
 
     def test_create_insuree(self):
+      muuid = 'ffa465c5-6807-4de0-847e-202b7f42122b'
       response = self.query(f'''
     mutation {{
       createInsuree(
         input: {{
-          clientMutationId: "ffa465c5-6807-4de0-847e-202b7f42122b"
+          clientMutationId: "{muuid}"
           clientMutationLabel: "Create insuree - 12343456234"
           
           chfId: "12343456234"
     lastName: "test"
     otherNames: "create insuree"
     genderId: "M"
     dob: "1951-12-05"
     head: false
-    marital: "N"
+    marital: "M"
     currentVillageId: {self.test_village.id}
     photo:{{
     officerId: 1
     date: "2023-12-15"
     photo: "{self.photo_base64}"
   }}
     cardIssued:false
@@ -230,23 +232,25 @@
             headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_dist_token}"},
         )
 
       content = json.loads(response.content)
 
     # This validates the status code and if you get errors
       self.assertResponseNoErrors(response)
-      
+      self.get_mutation_result(muuid, self.admin_dist_token )
       
       
     def test_create_family(self):
+      muuid='50f8f2c9-7685-4cd5-a7d8-b1fa78d46470'
+      fuuid='50f8f2c9-7685-4cd5-a770-b1fa34d46470'
       response = self.query(f'''
     mutation {{
       createFamily(
         input: {{
-          clientMutationId: "50f8f2c9-7685-4cd5-a7d8-b1fa78d46470"
+          clientMutationId: "{muuid}"
           clientMutationLabel: "Create Family - test create family (445566778899)"
           headInsuree: {{
     chfId: "4455667788"
     lastName: "test"
     otherNames: "create family"
     genderId: "M"
     uuid: "50f8f2c9-7685-4cd5-a778-b1fa78d46470"
@@ -259,15 +263,15 @@
 
   }}
     cardIssued:false
     status: "AC"
   }}
     locationId: {self.test_village.id}
     poverty: false
-    uuid: "50f8f2c9-7685-4cd5-a7d8-b1fa78d46475"
+    uuid: "{fuuid}"
     jsonExt: "{{}}"
         }}
       ) {{
         clientMutationId
         internalId
       }}
     }}
@@ -275,21 +279,22 @@
             headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_dist_token}"},
         )
 
       content = json.loads(response.content)
 
     # This validates the status code and if you get errors
       self.assertResponseNoErrors(response)
-      
+      self.get_mutation_result(muuid, self.admin_dist_token )
+      mmuid = '50f8f2c9-7685-4cd5-a778-b1fa78d46471'
       # update
       response = self.query(f'''
     mutation {{
       updateFamily(
         input: {{
-          clientMutationId: "50f8f2c9-7685-4cd5-a778-b1fa78d46470"
+          clientMutationId: "{muuid}"
           clientMutationLabel: "Update Family - test create family (445566778899)"
           headInsuree: {{
     chfId: "4455667788"
     uuid: "50f8f2c9-7685-4cd5-a778-b1fa78d46470"
     lastName: "test"
     otherNames: "create family"
     genderId: "M"
@@ -302,15 +307,15 @@
 
   }}
     cardIssued:false
     status: "AC"
   }}
     locationId: {self.test_village.id}
     poverty: true
-    uuid: "50f8f2c9-7685-4cd5-a7d8-b1fa78d46475"
+    uuid: "{fuuid}"
     jsonExt: "{{}}"
         }}
       ) {{
         clientMutationId
         internalId
       }}
     }}
@@ -318,12 +323,115 @@
             headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_dist_token}"},
         )
 
       content = json.loads(response.content)
 
     # This validates the status code and if you get errors
       self.assertResponseNoErrors(response)
-            
-      family = Family.objects.filter(*filter_validity(),uuid= "50f8f2c9-7685-4cd5-a7d8-b1fa78d46475").first()
+      content=  self.get_mutation_result(muuid, self.admin_dist_token )
+      family = Family.objects.filter(*filter_validity(),uuid= uuid.UUID(fuuid)).first()
       self.assertEqual(family.poverty, True)
 
-      
+      
+      
+    def test_inquire(self):
+      response = self.query("""
+query GetInsureeInquire($chfId: String) {
+  insurees(chfId: $chfId) {
+    __typename
+    edges {
+      __typename
+      node {
+        __typename
+        chfId
+        lastName
+        otherNames
+        dob
+        gender {
+          __typename
+          gender
+        }
+        photos {
+          __typename
+          folder
+          filename
+          photo
+        }
+        insureePolicies {
+          __typename
+          edges {
+            __typename
+            node {
+              __typename
+              policy {
+                __typename
+                product {
+                  __typename
+                  name
+                  code
+                  ceiling
+                  ceilingIp
+                  ceilingOp
+                  deductible
+                  deductibleIp
+                  deductibleOp
+                  maxNoAntenatal
+                  maxAmountAntenatal
+                  maxNoSurgery
+                  maxAmountSurgery
+                  maxNoConsultation
+                  maxAmountConsultation
+                  maxNoDelivery
+                  maxAmountDelivery
+                  maxNoHospitalization
+                  maxAmountHospitalization
+                  maxMembers
+                  maxNoVisits
+                  maxInstallments
+                  maxCeilingPolicy
+                  maxCeilingPolicyIp
+                  maxCeilingPolicyOp
+                  maxPolicyExtraMember
+                  maxPolicyExtraMemberIp
+                  maxPolicyExtraMemberOp
+                }
+                enrollDate
+                expiryDate
+                status
+                value
+              }
+            }
+          }
+        }
+      }
+    }
+  }
+}
+     
+      """,
+            headers={"HTTP_AUTHORIZATION": f"Bearer {self.ca_token}"},
+        )
+
+      content = json.loads(response.content)
+
+    # This validates the status code and if you get errors
+      self.assertResponseNoErrors(response)
+      
+      
+    def test_validate_number_validditiy_with_variables(self):
+        response = self.query(
+            '''
+    query ($insuranceNumber: String!) {
+      insureeNumberValidity(insureeNumber: $insuranceNumber) {
+        isValid
+        errorCode
+        errorMessage
+      }
+    }
+            ''',
+            headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_token}"},
+            variables={"insuranceNumber": "070707070"}        )
+
+        content = json.loads(response.content)
+
+        # This validates the status code and if you get errors
+        self.assertResponseNoErrors(response)
```

### Comparing `openimis-be-insuree-1.6.0/insuree/tests/test_insuree_photo.py` & `openimis_be_insuree-1.7.0/insuree/tests/test_insuree_photo.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/tests/test_insuree_validation.py` & `openimis_be_insuree-1.7.0/insuree/tests/test_insuree_validation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/insuree/utils.py` & `openimis_be_insuree-1.7.0/insuree/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/openimis_be_insuree.egg-info/PKG-INFO` & `openimis_be_insuree-1.7.0/openimis_be_insuree.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-insuree
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Insuree reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-insuree-1.6.0/openimis_be_insuree.egg-info/SOURCES.txt` & `openimis_be_insuree-1.7.0/openimis_be_insuree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.6.0/setup.py` & `openimis_be_insuree-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-insuree',
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Insuree reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

