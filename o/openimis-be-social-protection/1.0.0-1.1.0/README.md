# Comparing `tmp/openimis-be-social_protection-1.0.0.tar.gz` & `tmp/openimis_be_social_protection-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-social_protection-1.0.0.tar", last modified: Sat Dec 16 00:58:43 2023, max compression
+gzip compressed data, was "openimis_be_social_protection-1.1.0.tar", last modified: Tue Apr 30 09:07:40 2024, max compression
```

## Comparing `openimis-be-social_protection-1.0.0.tar` & `openimis_be_social_protection-1.1.0.tar`

### file list

```diff
@@ -1,53 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:42.995545 openimis-be-social_protection-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2023-12-16 00:58:42.995545 openimis-be-social_protection-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:42.995545 openimis-be-social_protection-1.0.0/openimis_be_social_protection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2023-12-16 00:58:42.000000 openimis-be-social_protection-1.0.0/openimis_be_social_protection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2023-12-16 00:58:42.000000 openimis-be-social_protection-1.0.0/openimis_be_social_protection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:58:42.000000 openimis-be-social_protection-1.0.0/openimis_be_social_protection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-16 00:58:42.000000 openimis-be-social_protection-1.0.0/openimis_be_social_protection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-16 00:58:42.000000 openimis-be-social_protection-1.0.0/openimis_be_social_protection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:58:42.995545 openimis-be-social_protection-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2023-12-16 00:58:42.000000 openimis-be-social_protection-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:42.991545 openimis-be-social_protection-1.0.0/social_protection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/custom_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)    14599 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:42.991545 openimis-be-social_protection-1.0.0/social_protection/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:42.991545 openimis-be-social_protection-1.0.0/social_protection/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/management/commands/add_beneficiary_data_to_opensearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:42.991545 openimis-be-social_protection-1.0.0/social_protection/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/migrations/0002_add_benefit_plan_rights_to_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/migrations/0003_beneficiary_historicalbeneficiary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/migrations/0004_add_beneficiary_rights_to_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/migrations/0005_auto_20230607_0759.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/migrations/0006_add_description_to_benefit_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/migrations/0007_auto_20230622_1015.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/migrations/0008_benefitplandatauploadrecords_historicalbenefitplandatauploadrecords.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/migrations/0009_add_schema_admin_and_schema_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/migrations/0010_auto_20230803_1735.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6613 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:42.995545 openimis-be-social_protection-1.0.0/social_protection/signals/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/signals/on_benefit_plan_data_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:42.995545 openimis-be-social_protection-1.0.0/social_protection/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/tests/beneficiary_service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/tests/benefit_plan_service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/tests/group_beneficiary_service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2023-12-16 00:58:30.000000 openimis-be-social_protection-1.0.0/social_protection/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:40.418497 openimis_be_social_protection-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18265 2024-04-30 09:07:40.418497 openimis_be_social_protection-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:40.418497 openimis_be_social_protection-1.1.0/openimis_be_social_protection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18265 2024-04-30 09:07:40.000000 openimis_be_social_protection-1.1.0/openimis_be_social_protection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-30 09:07:40.000000 openimis_be_social_protection-1.1.0/openimis_be_social_protection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:07:40.000000 openimis_be_social_protection-1.1.0/openimis_be_social_protection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 09:07:40.000000 openimis_be_social_protection-1.1.0/openimis_be_social_protection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 09:07:40.000000 openimis_be_social_protection-1.1.0/openimis_be_social_protection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:07:40.418497 openimis_be_social_protection-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-30 09:07:40.000000 openimis_be_social_protection-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:40.414497 openimis_be_social_protection-1.1.0/social_protection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/custom_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14910 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:40.414497 openimis_be_social_protection-1.1.0/social_protection/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:40.414497 openimis_be_social_protection-1.1.0/social_protection/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/management/commands/add_beneficiary_data_to_opensearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:40.414497 openimis_be_social_protection-1.1.0/social_protection/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/migrations/0002_add_benefit_plan_rights_to_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/migrations/0003_beneficiary_historicalbeneficiary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/migrations/0004_add_beneficiary_rights_to_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/migrations/0005_auto_20230607_0759.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/migrations/0006_add_description_to_benefit_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/migrations/0007_auto_20230622_1015.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/migrations/0008_benefitplandatauploadrecords_historicalbenefitplandatauploadrecords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/migrations/0009_add_schema_admin_and_schema_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/migrations/0010_auto_20230803_1735.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/migrations/0011_alter_beneficiary_date_created_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/migrations/0012_benefitplanmutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:40.414497 openimis_be_social_protection-1.1.0/social_protection/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/signals/on_confirm_enrollment_of_individual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/signals/on_validation_import_valid_items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:40.418497 openimis_be_social_protection-1.1.0/social_protection/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/tests/beneficiary_import_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/tests/beneficiary_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/tests/benefit_plan_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/tests/group_beneficiary_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:40.418497 openimis_be_social_protection-1.1.0/social_protection/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/workflows/base_beneficiary_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/workflows/base_beneficiary_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/workflows/beneficiary_update_valid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/workflows/beneficiary_upload_valid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-30 09:07:29.000000 openimis_be_social_protection-1.1.0/social_protection/workflows/utils.py
```

### Comparing `openimis-be-social_protection-1.0.0/LICENSE.md` & `openimis_be_social_protection-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/openimis_be_social_protection.egg-info/SOURCES.txt` & `openimis_be_social_protection-1.1.0/openimis_be_social_protection.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 social_protection/documents.py
 social_protection/gql_mutations.py
 social_protection/gql_queries.py
 social_protection/models.py
 social_protection/schema.py
 social_protection/services.py
 social_protection/urls.py
+social_protection/utils.py
 social_protection/validation.py
 social_protection/views.py
 social_protection/management/__init__.py
 social_protection/management/commands/__init__.py
 social_protection/management/commands/add_beneficiary_data_to_opensearch.py
 social_protection/migrations/0001_initial.py
 social_protection/migrations/0002_add_benefit_plan_rights_to_admin.py
@@ -28,16 +29,26 @@
 social_protection/migrations/0004_add_beneficiary_rights_to_admin.py
 social_protection/migrations/0005_auto_20230607_0759.py
 social_protection/migrations/0006_add_description_to_benefit_plan.py
 social_protection/migrations/0007_auto_20230622_1015.py
 social_protection/migrations/0008_benefitplandatauploadrecords_historicalbenefitplandatauploadrecords.py
 social_protection/migrations/0009_add_schema_admin_and_schema_roles.py
 social_protection/migrations/0010_auto_20230803_1735.py
+social_protection/migrations/0011_alter_beneficiary_date_created_and_more.py
+social_protection/migrations/0012_benefitplanmutation.py
 social_protection/migrations/__init__.py
 social_protection/signals/__init__.py
-social_protection/signals/on_benefit_plan_data_upload.py
+social_protection/signals/on_confirm_enrollment_of_individual.py
+social_protection/signals/on_validation_import_valid_items.py
 social_protection/tests/__init__.py
+social_protection/tests/beneficiary_import_service_test.py
 social_protection/tests/beneficiary_service_test.py
 social_protection/tests/benefit_plan_service_test.py
 social_protection/tests/data.py
 social_protection/tests/group_beneficiary_service_test.py
-social_protection/tests/helpers.py
+social_protection/tests/helpers.py
+social_protection/workflows/__init__.py
+social_protection/workflows/base_beneficiary_update.py
+social_protection/workflows/base_beneficiary_upload.py
+social_protection/workflows/beneficiary_update_valid.py
+social_protection/workflows/beneficiary_upload_valid.py
+social_protection/workflows/utils.py
```

### Comparing `openimis-be-social_protection-1.0.0/setup.py` & `openimis_be_social_protection-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,29 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-social_protection',
-    version='1.0.0',
+    version='v1.1.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend social_protection reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
     author='Jan Dolkowski',
     author_email='jdolkowski@soldevelo.com',
     install_requires=[
         'django',
         'django-db-signals',
         'djangorestframework',
         'openimis-be-core',
-        'jsonschema',
     ],
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.0',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3',
```

### Comparing `openimis-be-social_protection-1.0.0/social_protection/custom_filters.py` & `openimis_be_social_protection-1.1.0/social_protection/custom_filters.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/documents.py` & `openimis_be_social_protection-1.1.0/social_protection/documents.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/gql_mutations.py` & `openimis_be_social_protection-1.1.0/social_protection/gql_mutations.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from core.gql.gql_mutations.base_mutation import BaseHistoryModelCreateMutationMixin, BaseMutation, \
     BaseHistoryModelUpdateMutationMixin, BaseHistoryModelDeleteMutationMixin
 from core.schema import OpenIMISMutation
 from social_protection.apps import SocialProtectionConfig
 from social_protection.models import (
     BenefitPlan,
-    Beneficiary, GroupBeneficiary, BeneficiaryStatus
+    Beneficiary, GroupBeneficiary, BeneficiaryStatus, BenefitPlanMutation
 )
 from social_protection.services import (
     BenefitPlanService,
     BeneficiaryService, GroupBeneficiaryService
 )
 
 
@@ -101,21 +101,26 @@
         )
         check_perms_for_field(
             user, SocialProtectionConfig.gql_schema_create_perms, data, 'json_ext'
         )
 
     @classmethod
     def _mutate(cls, user, **data):
-        if "client_mutation_id" in data:
-            data.pop('client_mutation_id')
+        client_mutation_id = data.pop('client_mutation_id', None)
         if "client_mutation_label" in data:
             data.pop('client_mutation_label')
 
         service = BenefitPlanService(user)
         res = service.create(data)
+        if client_mutation_id and res['success']:
+            payroll_id = res['data']['id']
+            benefit_plan = BenefitPlan.objects.get(id=payroll_id)
+            BenefitPlanMutation.object_mutated(
+                user, client_mutation_id=client_mutation_id, benefit_plan=benefit_plan
+            )
         if not res['success']:
             return res
         return None
 
     class Input(CreateBenefitPlanInputType):
         pass
```

### Comparing `openimis-be-social_protection-1.0.0/social_protection/gql_queries.py` & `openimis_be_social_protection-1.1.0/social_protection/gql_queries.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import graphene
 from django.contrib.auth.models import AnonymousUser
+from graphene import ObjectType
 from graphene_django import DjangoObjectType
 
+from contribution_plan.models import PaymentPlan
 from core import prefix_filterset, ExtendedConnection
 from individual.gql_queries import IndividualGQLType, GroupGQLType, \
     IndividualDataSourceUploadGQLType
 from social_protection.apps import SocialProtectionConfig
 from social_protection.models import Beneficiary, BenefitPlan, GroupBeneficiary, BenefitPlanDataUploadRecords
 
 
@@ -22,14 +24,15 @@
         if _have_permissions(info.context.user, SocialProtectionConfig.gql_schema_search_perms):
             return self.json_ext
         return None
 
 
 class BenefitPlanGQLType(DjangoObjectType, JsonExtMixin):
     uuid = graphene.String(source='uuid')
+    has_payment_plans = graphene.Boolean()
 
     class Meta:
         model = BenefitPlan
         interfaces = (graphene.relay.Node,)
         filter_fields = {
             "id": ["exact"],
             "code": ["exact", "iexact", "startswith", "istartswith", "contains", "icontains"],
@@ -48,14 +51,17 @@
         connection_class = ExtendedConnection
 
     def resolve_beneficiary_data_schema(self, info):
         if _have_permissions(info.context.user, SocialProtectionConfig.gql_schema_search_perms):
             return self.beneficiary_data_schema
         return None
 
+    def resolve_has_payment_plans(self, info):
+        return PaymentPlan.objects.filter(benefit_plan_id=self.id).exists()
+
 
 class BeneficiaryGQLType(DjangoObjectType, JsonExtMixin):
     uuid = graphene.String(source='uuid')
 
     class Meta:
         model = Beneficiary
         interfaces = (graphene.relay.Node,)
@@ -108,7 +114,57 @@
             "is_deleted": ["exact"],
             "version": ["exact"],
             "workflow": ["exact", "iexact", "startswith", "istartswith", "contains", "icontains"],
             **prefix_filterset("data_upload__", IndividualDataSourceUploadGQLType._meta.filter_fields),
             **prefix_filterset("benefit_plan__", BenefitPlanGQLType._meta.filter_fields),
         }
         connection_class = ExtendedConnection
+
+
+class BenefitPlanSchemaFieldsGQLType(ObjectType):
+    schema_fields = graphene.List(graphene.String)
+
+    def resolve_schema_fields(self, info, **kwargs):
+        schemas = self.values_list("beneficiary_data_schema__properties", flat=True)
+        field_list = set(
+            f'json_ext__{field}'
+            for schema in schemas  # Iterate over each schema
+            if schema  # Ensure the schema is not None or empty
+            for field in schema  # Iterate over fields in the schema
+        )
+        return field_list
+
+
+class BenefitPlanHistoryGQLType(DjangoObjectType, JsonExtMixin):
+    uuid = graphene.String(source='uuid')
+    has_payment_plans = graphene.Boolean()
+
+    def resolve_user_updated(self, info):
+        return self.user_updated
+
+    class Meta:
+        model = BenefitPlan.history.model
+        interfaces = (graphene.relay.Node,)
+        filter_fields = {
+            "id": ["exact"],
+            "code": ["exact", "iexact", "startswith", "istartswith", "contains", "icontains"],
+            "name": ["exact", "iexact", "startswith", "istartswith", "contains", "icontains"],
+            "date_valid_from": ["exact", "lt", "lte", "gt", "gte"],
+            "date_valid_to": ["exact", "lt", "lte", "gt", "gte"],
+            "max_beneficiaries": ["exact", "lt", "lte", "gt", "gte"],
+            "institution": ["exact", "iexact", "startswith", "istartswith", "contains", "icontains"],
+
+            "date_created": ["exact", "lt", "lte", "gt", "gte"],
+            "date_updated": ["exact", "lt", "lte", "gt", "gte"],
+            "is_deleted": ["exact"],
+            "version": ["exact"],
+            "description": ["exact", "iexact", "startswith", "istartswith", "contains", "icontains"],
+        }
+        connection_class = ExtendedConnection
+
+    def resolve_beneficiary_data_schema(self, info):
+        if _have_permissions(info.context.user, SocialProtectionConfig.gql_schema_search_perms):
+            return self.beneficiary_data_schema
+        return None
+
+    def resolve_has_payment_plans(self, info):
+        return PaymentPlan.objects.filter(benefit_plan_id=self.id).exists()
```

### Comparing `openimis-be-social_protection-1.0.0/social_protection/management/commands/add_beneficiary_data_to_opensearch.py` & `openimis_be_social_protection-1.1.0/social_protection/management/commands/add_beneficiary_data_to_opensearch.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/migrations/0001_initial.py` & `openimis_be_social_protection-1.1.0/social_protection/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/migrations/0002_add_benefit_plan_rights_to_admin.py` & `openimis_be_social_protection-1.1.0/social_protection/migrations/0002_add_benefit_plan_rights_to_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/migrations/0003_beneficiary_historicalbeneficiary.py` & `openimis_be_social_protection-1.1.0/social_protection/migrations/0003_beneficiary_historicalbeneficiary.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/migrations/0004_add_beneficiary_rights_to_admin.py` & `openimis_be_social_protection-1.1.0/social_protection/migrations/0004_add_beneficiary_rights_to_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/migrations/0005_auto_20230607_0759.py` & `openimis_be_social_protection-1.1.0/social_protection/migrations/0005_auto_20230607_0759.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/migrations/0006_add_description_to_benefit_plan.py` & `openimis_be_social_protection-1.1.0/social_protection/migrations/0006_add_description_to_benefit_plan.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/migrations/0007_auto_20230622_1015.py` & `openimis_be_social_protection-1.1.0/social_protection/migrations/0007_auto_20230622_1015.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/migrations/0008_benefitplandatauploadrecords_historicalbenefitplandatauploadrecords.py` & `openimis_be_social_protection-1.1.0/social_protection/migrations/0008_benefitplandatauploadrecords_historicalbenefitplandatauploadrecords.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/migrations/0009_add_schema_admin_and_schema_roles.py` & `openimis_be_social_protection-1.1.0/social_protection/migrations/0009_add_schema_admin_and_schema_roles.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/migrations/0010_auto_20230803_1735.py` & `openimis_be_social_protection-1.1.0/social_protection/migrations/0010_auto_20230803_1735.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/models.py` & `openimis_be_social_protection-1.1.0/social_protection/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from django.contrib.auth.models import AnonymousUser
 from django.db import models
+from django.db.models import Func
 from django.utils.translation import gettext as _
 from pydantic.error_wrappers import ValidationError
 
 from core import models as core_models
+from core.models import UUIDModel, ObjectMutation, MutationLog
 from individual.models import Individual, Group, IndividualDataSourceUpload
 
 
 class BeneficiaryStatus(models.TextChoices):
     POTENTIAL = "POTENTIAL", _("POTENTIAL")
     ACTIVE = "ACTIVE", _("ACTIVE")
     GRADUATED = "GRADUATED", _("GRADUATED")
@@ -31,20 +33,26 @@
         max_length=100, choices=BenefitPlanType.choices, default=BenefitPlanType.INDIVIDUAL_TYPE, null=False
     )
     description = models.CharField(max_length=1024, null=True, blank=True)
 
     def __str__(self):
         return f'Benefit Plan {self.code}'
 
+
+class BenefitPlanMutation(UUIDModel, ObjectMutation):
+    benefit_plan = models.ForeignKey(BenefitPlan, models.DO_NOTHING, related_name='mutations')
+    mutation = models.ForeignKey(MutationLog, models.DO_NOTHING, related_name='benefit_plan')
+
+
 class Beneficiary(core_models.HistoryBusinessModel):
     individual = models.ForeignKey(Individual, models.DO_NOTHING, null=False)
     benefit_plan = models.ForeignKey(BenefitPlan, models.DO_NOTHING, null=False)
     status = models.CharField(max_length=100, choices=BeneficiaryStatus.choices, null=False)
 
-    json_ext = models.JSONField(db_column="Json_ext", default=dict)
+    json_ext = models.JSONField(db_column="Json_ext", blank=True, default=dict)
 
     def clean(self):
         if self.benefit_plan.type != BenefitPlan.BenefitPlanType.INDIVIDUAL_TYPE:
             raise ValidationError(_("Beneficiary must be associated with an individual benefit plan."))
         super().clean()
 
     def __str__(self):
@@ -52,20 +60,28 @@
 
 
 class BenefitPlanDataUploadRecords(core_models.HistoryModel):
     data_upload = models.ForeignKey(IndividualDataSourceUpload, models.DO_NOTHING, null=False)
     benefit_plan = models.ForeignKey(BenefitPlan, models.DO_NOTHING, null=False)
     workflow = models.CharField(max_length=50)
 
+    def __str__(self):
+        return f"{self.benefit_plan.code} {self.data_upload.source_name} {self.workflow} {self.date_created}"
+
 
 class GroupBeneficiary(core_models.HistoryBusinessModel):
     group = models.ForeignKey(Group, models.DO_NOTHING, null=False)
     benefit_plan = models.ForeignKey(BenefitPlan, models.DO_NOTHING, null=False)
     status = models.CharField(max_length=100, choices=BeneficiaryStatus.choices, null=False)
 
-    json_ext = models.JSONField(db_column="Json_ext", default=dict)
+    json_ext = models.JSONField(db_column="Json_ext", blank=True, default=dict)
 
     def clean(self):
         if self.benefit_plan.type != BenefitPlan.BenefitPlanType.GROUP_TYPE:
             raise ValidationError(_("Group beneficiary must be associated with a group benefit plan."))
 
         super().clean()
+
+
+class JSONUpdate(Func):
+    function = 'JSONB_SET'
+    arity = 3
```

### Comparing `openimis-be-social_protection-1.0.0/social_protection/schema.py` & `openimis_be_social_protection-1.1.0/social_protection/schema.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 import graphene
 import pandas as pd
-import re
 
 from django.contrib.auth.models import AnonymousUser
 from django.db.models import Q
 from django.core.exceptions import PermissionDenied
 
 from core.gql.export_mixin import ExportableQueryMixin
 
 from django.utils.translation import gettext as _
 from core.custom_filters import CustomFilterWizardStorage
 from core.gql_queries import ValidationMessageGQLType
 from core.schema import OrderedDjangoFilterConnectionField
-from core.utils import append_validity_filter
+from core.utils import append_validity_filter, validate_json_schema
 from social_protection.apps import SocialProtectionConfig
 from social_protection.gql_mutations import (
     CreateBenefitPlanMutation,
     UpdateBenefitPlanMutation,
     DeleteBenefitPlanMutation,
     CreateBeneficiaryMutation,
     UpdateBeneficiaryMutation,
     DeleteBeneficiaryMutation, CreateGroupBeneficiaryMutation, UpdateGroupBeneficiaryMutation,
     DeleteGroupBeneficiaryMutation
 )
 from social_protection.gql_queries import (
     BenefitPlanGQLType,
-    BeneficiaryGQLType, GroupBeneficiaryGQLType, BenefitPlanDataUploadQGLType
+    BeneficiaryGQLType, GroupBeneficiaryGQLType,
+    BenefitPlanDataUploadQGLType, BenefitPlanSchemaFieldsGQLType,
+    BenefitPlanHistoryGQLType
 )
 from social_protection.models import (
     BenefitPlan,
     Beneficiary, GroupBeneficiary, BenefitPlanDataUploadRecords
 )
-from social_protection.validation import validate_bf_unique_code, validate_bf_unique_name, validate_json_schema
+from social_protection.validation import validate_bf_unique_code, validate_bf_unique_name
 import graphene_django_optimizer as gql_optimizer
 
 
 def patch_details(beneficiary_df: pd.DataFrame):
     # Transform extension to DF columns 
     df_unfolded = pd.json_normalize(beneficiary_df['json_ext'])
     # Merge unfolded DataFrame with the original DataFrame
     df_final = pd.concat([beneficiary_df, df_unfolded], axis=1)
     df_final = df_final.drop('json_ext', axis=1)
     return df_final
 
 
+class BfTypeEnum(graphene.Enum):
+    INDIVIDUAL = BenefitPlan.BenefitPlanType.INDIVIDUAL_TYPE
+    GROUP = BenefitPlan.BenefitPlanType.GROUP_TYPE
+
+
 class Query(ExportableQueryMixin, graphene.ObjectType):
     export_patches = {
         'beneficiary': [
             patch_details
         ],
         'group_beneficiary': [
             patch_details
@@ -108,14 +114,32 @@
         description="Checks that the specified Benefit Plan name is valid"
     )
     bf_schema_validity = graphene.Field(
         ValidationMessageGQLType,
         bf_schema=graphene.String(required=True),
         description="Checks that the specified Benefit Plan schema is valid"
     )
+    benefit_plan_schema_field = graphene.Field(
+        BenefitPlanSchemaFieldsGQLType,
+        bf_type=graphene.Argument(BfTypeEnum),
+        description="Endpoint responsible for getting all fields from all BF schemas"
+    )
+    benefit_plan_history = OrderedDjangoFilterConnectionField(
+        BenefitPlanHistoryGQLType,
+        orderBy=graphene.List(of_type=graphene.String),
+        dateValidFrom__Gte=graphene.DateTime(),
+        dateValidTo__Lte=graphene.DateTime(),
+        applyDefaultValidityFilter=graphene.Boolean(),
+        client_mutation_id=graphene.String(),
+        individual_id=graphene.String(),
+        group_id=graphene.String(),
+        beneficiary_status=graphene.String(),
+        search=graphene.String(),
+        sort_alphabetically=graphene.Boolean(),
+    )
 
     def resolve_bf_code_validity(self, info, **kwargs):
         if not info.context.user.has_perms(SocialProtectionConfig.gql_benefit_plan_search_perms):
             raise PermissionDenied(_("unauthorized"))
         errors = validate_bf_unique_code(kwargs['bf_code'])
         if errors:
             return ValidationMessageGQLType(False, error_message=errors[0]['message'])
@@ -212,33 +236,101 @@
         Query._check_permissions(
             info.context.user,
             SocialProtectionConfig.gql_beneficiary_search_perms
         )
         query = GroupBeneficiary.objects.filter(*filters)
         return gql_optimizer.query(query, info)
 
+    def resolve_awaiting_beneficiary(self, info, **kwargs):
+        filters = append_validity_filter(**kwargs)
+
+        client_mutation_id = kwargs.get("client_mutation_id", None)
+        if client_mutation_id:
+            filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
+
+        Query._check_permissions(
+            info.context.user,
+            SocialProtectionConfig.gql_beneficiary_search_perms
+        )
+        query = GroupBeneficiary.objects.filter(*filters)
+        return gql_optimizer.query(query, info)
+
     def resolve_beneficiary_data_upload_history(self, info, **kwargs):
         filters = append_validity_filter(**kwargs)
 
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
             filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
 
         Query._check_permissions(
             info.context.user,
             SocialProtectionConfig.gql_beneficiary_search_perms
         )
         query = BenefitPlanDataUploadRecords.objects.filter(*filters)
         return gql_optimizer.query(query, info)
 
+    def resolve_benefit_plan_schema_field(self, info, **kwargs):
+        filters = append_validity_filter(**kwargs)
+
+        Query._check_permissions(
+            info.context.user,
+            SocialProtectionConfig.gql_schema_search_perms
+        )
+
+        bf_type = kwargs.get("bf_type", None)
+        if bf_type:
+            filters.append(Q(type=bf_type))
+
+        query = BenefitPlan.objects.filter(*filters)
+        return gql_optimizer.query(query, info)
+
     @staticmethod
     def _check_permissions(user, permission):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(permission):
             raise PermissionError("Unauthorized")
 
+    def resolve_benefit_plan_history(self, info, **kwargs):
+        filters = append_validity_filter(**kwargs)
+
+        search = kwargs.get("search", None)
+        if search:
+            search_terms = search.split(' ')
+            search_queries = Q()
+            for term in search_terms:
+                search_queries |= Q(code__icontains=term) | Q(name__icontains=term)
+            filters.append(search_queries)
+
+        client_mutation_id = kwargs.get("client_mutation_id", None)
+        if client_mutation_id:
+            filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
+
+        individual_id = kwargs.get("individual_id", None)
+        if individual_id:
+            filters.append(Q(beneficiary__individual__id=individual_id))
+
+        group_id = kwargs.get("group_id", None)
+        if group_id:
+            filters.append(Q(groupbeneficiary__group__id=group_id))
+
+        beneficiary_status = kwargs.get("beneficiary_status", None)
+        if beneficiary_status:
+            filters.append(Q(beneficiary__status=beneficiary_status) | Q(groupbeneficiary__status=beneficiary_status))
+
+        Query._check_permissions(
+            info.context.user,
+            SocialProtectionConfig.gql_benefit_plan_search_perms
+        )
+
+        query = BenefitPlan.history.filter(*filters)
+
+        sort_alphabetically = kwargs.get("sort_alphabetically", None)
+        if sort_alphabetically:
+            query = query.order_by('code')
+        return gql_optimizer.query(query, info)
+
 
 class Mutation(graphene.ObjectType):
     create_benefit_plan = CreateBenefitPlanMutation.Field()
     update_benefit_plan = UpdateBenefitPlanMutation.Field()
     delete_benefit_plan = DeleteBenefitPlanMutation.Field()
 
     create_beneficiary = CreateBeneficiaryMutation.Field()
```

### Comparing `openimis-be-social_protection-1.0.0/social_protection/signals/__init__.py` & `openimis_be_social_protection-1.1.0/social_protection/signals/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 import logging
 
 from core.service_signals import ServiceSignalBindType
 from core.signals import bind_service_signal
 from social_protection.services import BenefitPlanService, BeneficiaryService, GroupBeneficiaryService
 
-from social_protection.signals.on_benefit_plan_data_upload import on_benefit_plan_data_upload
+from social_protection.signals.on_validation_import_valid_items import on_task_complete_import_validated, \
+    on_task_resolve
+
+from social_protection.signals.on_confirm_enrollment_of_individual import on_confirm_enrollment_of_individual
+from social_protection.signals.on_validation_import_valid_items import on_task_complete_import_validated, \
+    on_task_resolve
+
 from tasks_management.services import on_task_complete_service_handler
 
 logger = logging.getLogger(__name__)
 
 
 def bind_service_signals():
     bind_service_signal(
-        'benefit_plan.import_beneficiaries',
-        on_benefit_plan_data_upload,
-        bind_type=ServiceSignalBindType.AFTER
-    )
-    bind_service_signal(
         'task_service.complete_task',
         on_task_complete_service_handler(BenefitPlanService),
         bind_type=ServiceSignalBindType.AFTER
     )
     bind_service_signal(
         'task_service.complete_task',
         on_task_complete_service_handler(BeneficiaryService),
         bind_type=ServiceSignalBindType.AFTER
     )
     bind_service_signal(
         'task_service.complete_task',
         on_task_complete_service_handler(GroupBeneficiaryService),
         bind_type=ServiceSignalBindType.AFTER
     )
+    bind_service_signal(
+        'task_service.complete_task',
+        on_task_complete_import_validated,
+        bind_type=ServiceSignalBindType.AFTER
+    )
+    bind_service_signal(
+        'task_service.resolve_task',
+        on_task_resolve,
+        bind_type=ServiceSignalBindType.AFTER
+    )
+    bind_service_signal(
+        'individual_service.select_individuals_to_benefit_plan',
+        on_confirm_enrollment_of_individual,
+        bind_type=ServiceSignalBindType.AFTER
+    )
```

### Comparing `openimis-be-social_protection-1.0.0/social_protection/tests/beneficiary_service_test.py` & `openimis_be_social_protection-1.1.0/social_protection/tests/beneficiary_service_test.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/tests/benefit_plan_service_test.py` & `openimis_be_social_protection-1.1.0/social_protection/tests/benefit_plan_service_test.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/tests/data.py` & `openimis_be_social_protection-1.1.0/social_protection/tests/data.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/tests/group_beneficiary_service_test.py` & `openimis_be_social_protection-1.1.0/social_protection/tests/group_beneficiary_service_test.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/tests/helpers.py` & `openimis_be_social_protection-1.1.0/social_protection/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-social_protection-1.0.0/social_protection/validation.py` & `openimis_be_social_protection-1.1.0/social_protection/validation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import json
-
-import jsonschema
-
 from django.core.exceptions import ValidationError
 from django.utils.translation import gettext as _
 
+from core.utils import validate_json_schema
 from core.validation import BaseModelValidation
 from social_protection.models import Beneficiary, BenefitPlan
 
 
 class BenefitPlanValidation(BaseModelValidation):
     OBJECT_TYPE = BenefitPlan
 
@@ -44,47 +41,31 @@
     if beneficiary_data_schema:
         validations.extend(validate_json_schema(beneficiary_data_schema))
 
     return validations
 
 
 def validate_bf_unique_code(code, uuid=None):
-    instance = BenefitPlan.objects.filter(code=code, is_deleted=False).first()
-    if instance and str(instance.uuid) != uuid:
+    instance = BenefitPlan.objects.filter(code=code, is_deleted=False).exclude(id=uuid).first()
+    if instance:
         return [{"message": _("social_protection.validation.benefit_plan.code_exists" % {
             'code': code
         })}]
     return []
 
 
 def validate_bf_unique_name(name, uuid=None):
-    instance = BenefitPlan.objects.filter(name=name, is_deleted=False).first()
-    if instance and str(instance.uuid) != uuid:
+    instance = BenefitPlan.objects.filter(name=name, is_deleted=False).exclude(id=uuid).first()
+    if instance:
         return [{"message": _("social_protection.validation.benefit_plan.name_exists" % {
             'name': name
         })}]
     return []
 
 
-def validate_json_schema(schema):
-    try:
-        if not isinstance(schema, dict):
-            schema = json.loads(schema)
-        jsonschema.Draft7Validator.check_schema(schema)
-        return []
-    except jsonschema.exceptions.SchemaError as schema_error:
-        return [{"message": _("social_protection.validation.benefit_plan.invalid_schema" % {
-            'error': str(schema_error)
-        })}]
-    except ValueError as json_error:
-        return [{"message": _("social_protection.validation.benefit_plan.invalid_json" % {
-            'error': str(json_error)
-        })}]
-
-
 def validate_not_empty_field(string, field):
     if not string:
         return [{"message": _("social_protection.validation.field_empty") % {
             'field': field
         }}]
     return []
```

