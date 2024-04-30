# Comparing `tmp/openimis-be-individual-1.0.0.tar.gz` & `tmp/openimis_be_individual-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-individual-1.0.0.tar", last modified: Sat Dec 16 01:12:36 2023, max compression
+gzip compressed data, was "openimis_be_individual-1.1.0.tar", last modified: Tue Apr 30 09:00:12 2024, max compression
```

## Comparing `openimis-be-individual-1.0.0.tar` & `openimis_be_individual-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:12:36.940047 openimis-be-individual-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2023-12-16 01:12:36.940047 openimis-be-individual-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:12:36.936047 openimis-be-individual-1.0.0/individual/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:12:36.940047 openimis-be-individual-1.0.0/individual/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/migrations/0002_add_individual_rigts_for_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7511 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/migrations/0003_group_groupindividual_historicalgroup_historicalgroupindividual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/migrations/0004_add_group_rights_to_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/migrations/0005_auto_20230621_1323.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/migrations/0006_auto_20230621_1544.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/migrations/0007_auto_20230630_0950.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/migrations/0008_auto_20230724_1355.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:12:36.940047 openimis-be-individual-1.0.0/individual/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/tests/group_individual_service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/tests/group_service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/tests/individual_service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 01:12:26.000000 openimis-be-individual-1.0.0/individual/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:12:36.940047 openimis-be-individual-1.0.0/openimis_be_individual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2023-12-16 01:12:36.000000 openimis-be-individual-1.0.0/openimis_be_individual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2023-12-16 01:12:36.000000 openimis-be-individual-1.0.0/openimis_be_individual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 01:12:36.000000 openimis-be-individual-1.0.0/openimis_be_individual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-16 01:12:36.000000 openimis-be-individual-1.0.0/openimis_be_individual.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-16 01:12:36.000000 openimis-be-individual-1.0.0/openimis_be_individual.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 01:12:36.940047 openimis-be-individual-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-16 01:12:36.000000 openimis-be-individual-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:12.548458 openimis_be_individual-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-30 09:00:12.544458 openimis_be_individual-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:12.540459 openimis_be_individual-1.1.0/individual/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/custom_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13918 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:12.544458 openimis_be_individual-1.1.0/individual/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/migrations/0002_add_individual_rigts_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7511 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/migrations/0003_group_groupindividual_historicalgroup_historicalgroupindividual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/migrations/0004_add_group_rights_to_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/migrations/0005_auto_20230621_1323.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/migrations/0006_auto_20230621_1544.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/migrations/0007_auto_20230630_0950.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/migrations/0008_auto_20240105_1527.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/migrations/0009_auto_20240109_0953.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/migrations/0010_auto_20240109_1140.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/migrations/0011_auto_20240131_1015.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15120 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26327 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:12.544458 openimis_be_individual-1.1.0/individual/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8875 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/signals/on_validation_import_valid_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:12.544458 openimis_be_individual-1.1.0/individual/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/tests/create_group_and_move_individual_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/tests/group_individual_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/tests/group_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/tests/individual_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:12.544458 openimis_be_individual-1.1.0/individual/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/workflows/base_individual_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/workflows/base_individual_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/workflows/example_import_individual_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/workflows/individual_update_valid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/workflows/individual_upload_valid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-04-30 09:00:03.000000 openimis_be_individual-1.1.0/individual/workflows/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:12.544458 openimis_be_individual-1.1.0/openimis_be_individual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-30 09:00:12.000000 openimis_be_individual-1.1.0/openimis_be_individual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-30 09:00:12.000000 openimis_be_individual-1.1.0/openimis_be_individual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:00:12.000000 openimis_be_individual-1.1.0/openimis_be_individual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 09:00:12.000000 openimis_be_individual-1.1.0/openimis_be_individual.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 09:00:12.000000 openimis_be_individual-1.1.0/openimis_be_individual.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:00:12.548458 openimis_be_individual-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-30 09:00:12.000000 openimis_be_individual-1.1.0/setup.py
```

### Comparing `openimis-be-individual-1.0.0/LICENSE.md` & `openimis_be_individual-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-individual-1.0.0/PKG-INFO` & `openimis_be_individual-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-individual
-Version: 1.0.0
+Version: 1.1.0
 Summary: The openIMIS Backend individual reference module.
 Home-page: https://openimis.org/
 Author: Kamil Malinowski
 Author-email: kmalinowski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -83,7 +83,17 @@
 * gql_group_create_perms: required rights to call createGroup and addIndividualToGroup and createGroupIndividuals GraphQL Mutation (default: ["180002"])
 * gql_group_update_perms: required rights to call updateGroup and editIndividualInGroup GraphQL Mutation (default: ["180003"])
 * gql_group_delete_perms: required rights to call deleteGroup and removeIndividualFromGroup GraphQL Mutation (default: ["180004"])
 
 
 ## openIMIS Modules Dependencies
 - core
+
+
+## Enabling Python Workflows
+Module comes with simple workflows for individual data upload. 
+They should be used for the development purposes, not in production environment. 
+To activate these Python workflows, a configuration change is required. 
+Specifically, the `enable_python_workflows` parameter to `true` within module config.
+
+Workflows: 
+ * individual upload
```

### Comparing `openimis-be-individual-1.0.0/README.md` & `openimis_be_individual-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,7 +60,17 @@
 * gql_group_create_perms: required rights to call createGroup and addIndividualToGroup and createGroupIndividuals GraphQL Mutation (default: ["180002"])
 * gql_group_update_perms: required rights to call updateGroup and editIndividualInGroup GraphQL Mutation (default: ["180003"])
 * gql_group_delete_perms: required rights to call deleteGroup and removeIndividualFromGroup GraphQL Mutation (default: ["180004"])
 
 
 ## openIMIS Modules Dependencies
 - core
+
+
+## Enabling Python Workflows
+Module comes with simple workflows for individual data upload. 
+They should be used for the development purposes, not in production environment. 
+To activate these Python workflows, a configuration change is required. 
+Specifically, the `enable_python_workflows` parameter to `true` within module config.
+
+Workflows: 
+ * individual upload
```

### Comparing `openimis-be-individual-1.0.0/individual/gql_mutations.py` & `openimis_be_individual-1.1.0/individual/gql_mutations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import graphene
-from django.contrib.auth.models import AnonymousUser
 from django.core.exceptions import ValidationError
 from django.db import transaction
 
 from core.gql.gql_mutations.base_mutation import BaseHistoryModelDeleteMutationMixin, BaseMutation, \
     BaseHistoryModelUpdateMutationMixin, BaseHistoryModelCreateMutationMixin
 from core.schema import OpenIMISMutation
 from individual.apps import IndividualConfig
 from individual.models import Individual, Group, GroupIndividual
-from individual.services import IndividualService, GroupService, GroupIndividualService
+from individual.services import IndividualService, GroupService, GroupIndividualService, \
+    CreateGroupAndMoveIndividualService
+from individual.tasks import (
+    task_import_individual_workflow,
+    task_import_individual_workflow_valid
+)
 
 
 class CreateIndividualInputType(OpenIMISMutation.Input):
     first_name = graphene.String(required=True, max_length=255)
     last_name = graphene.String(required=True, max_length=255)
     dob = graphene.Date(required=True)
     json_ext = graphene.types.json.JSONString(required=False)
@@ -30,86 +34,99 @@
     id = graphene.UUID(required=True)
 
 
 class CreateGroupIndividualInputType(OpenIMISMutation.Input):
     class RoleEnum(graphene.Enum):
         HEAD = GroupIndividual.Role.HEAD
         RECIPIENT = GroupIndividual.Role.RECIPIENT
+
     group_id = graphene.UUID(required=True)
     individual_id = graphene.UUID(required=True)
     role = graphene.Field(RoleEnum, required=False)
 
     def resolve_role(self, info):
         return self.role
 
 
 class UpdateGroupIndividualInputType(CreateGroupIndividualInputType):
     id = graphene.UUID(required=True)
 
 
+class ConfirmIndividualEnrollmentInputType(OpenIMISMutation.Input):
+    custom_filters = graphene.List(required=False, of_type=graphene.String)
+    benefit_plan_id = graphene.String(required=True, max_lenght=255)
+    status = graphene.String(required=True, max_lenght=255)
+
+
 class CreateIndividualMutation(BaseHistoryModelCreateMutationMixin, BaseMutation):
     _mutation_class = "CreateIndividualMutation"
     _mutation_module = "individual"
     _model = Individual
 
     @classmethod
     def _validate_mutation(cls, user, **data):
-        if type(user) is AnonymousUser or not user.id or not user.has_perms(
+        super()._validate_mutation(user, **data)
+        if not user.has_perms(
                 IndividualConfig.gql_individual_create_perms):
             raise ValidationError("mutation.authentication_required")
 
     @classmethod
     def _mutate(cls, user, **data):
         if "client_mutation_id" in data:
             data.pop('client_mutation_id')
         if "client_mutation_label" in data:
             data.pop('client_mutation_label')
 
         service = IndividualService(user)
-        service.create(data)
+        result = service.create(data)
+        return result if not result['success'] else None
 
     class Input(CreateIndividualInputType):
         pass
 
 
 class UpdateIndividualMutation(BaseHistoryModelUpdateMutationMixin, BaseMutation):
     _mutation_class = "UpdateIndividualMutation"
     _mutation_module = "individual"
     _model = Individual
 
     @classmethod
     def _validate_mutation(cls, user, **data):
-        if type(user) is AnonymousUser or not user.id or not user.has_perms(
+        super()._validate_mutation(user, **data)
+        if not user.has_perms(
                 IndividualConfig.gql_individual_update_perms):
             raise ValidationError("mutation.authentication_required")
 
     @classmethod
     def _mutate(cls, user, **data):
-        if "date_valid_to" not in data:
-            data['date_valid_to'] = None
         if "client_mutation_id" in data:
             data.pop('client_mutation_id')
         if "client_mutation_label" in data:
             data.pop('client_mutation_label')
 
         service = IndividualService(user)
-        service.update(data)
+        if IndividualConfig.check_individual_update:
+            result = service.create_update_task(data)
+        else:
+            result = service.update(data)
+        return result if not result['success'] else None
 
     class Input(UpdateIndividualInputType):
         pass
 
 
 class DeleteIndividualMutation(BaseHistoryModelDeleteMutationMixin, BaseMutation):
     _mutation_class = "DeleteIndividualMutation"
     _mutation_module = "individual"
     _model = Individual
 
     @classmethod
     def _validate_mutation(cls, user, **data):
-        if type(user) is AnonymousUser or not user.id or not user.has_perms(
+        super()._validate_mutation(user, **data)
+        if not user.has_perms(
                 IndividualConfig.gql_individual_delete_perms):
             raise ValidationError("mutation.authentication_required")
 
     @classmethod
     def _mutate(cls, user, **data):
         if "client_mutation_id" in data:
             data.pop('client_mutation_id')
@@ -131,68 +148,70 @@
 class CreateGroupMutation(BaseHistoryModelCreateMutationMixin, BaseMutation):
     _mutation_class = "CreateGroupMutation"
     _mutation_module = "individual"
     _model = Group
 
     @classmethod
     def _validate_mutation(cls, user, **data):
-        if type(user) is AnonymousUser or not user.has_perms(
+        super()._validate_mutation(user, **data)
+        if not user.has_perms(
                 IndividualConfig.gql_group_create_perms):
             raise ValidationError("mutation.authentication_required")
 
     @classmethod
     def _mutate(cls, user, **data):
         if "client_mutation_id" in data:
             data.pop('client_mutation_id')
         if "client_mutation_label" in data:
             data.pop('client_mutation_label')
 
         service = GroupService(user)
-        service.create(data)
+        result = service.create(data)
+        return result if not result['success'] else None
 
     class Input(CreateGroupInputType):
         pass
 
 
 class UpdateGroupMutation(BaseHistoryModelUpdateMutationMixin, BaseMutation):
     _mutation_class = "UpdateGroupMutation"
     _mutation_module = "individual"
     _model = Group
 
     @classmethod
     def _validate_mutation(cls, user, **data):
         super()._validate_mutation(user, **data)
-        if type(user) is AnonymousUser or not user.has_perms(
+        if not user.has_perms(
                 IndividualConfig.gql_group_update_perms):
             raise ValidationError("mutation.authentication_required")
 
     @classmethod
     def _mutate(cls, user, **data):
-        if "date_valid_to" not in data:
-            data['date_valid_to'] = None
         if "client_mutation_id" in data:
             data.pop('client_mutation_id')
         if "client_mutation_label" in data:
             data.pop('client_mutation_label')
 
         service = GroupService(user)
-        service.update(data)
+        result = service.update(data)
+        return result if not result['success'] else None
 
     class Input(UpdateGroupInputType):
         pass
 
 
 class DeleteGroupMutation(BaseHistoryModelDeleteMutationMixin, BaseMutation):
     _mutation_class = "DeleteGroupMutation"
     _mutation_module = "social_protection"
     _model = Group
 
     @classmethod
     def _validate_mutation(cls, user, **data):
-        if type(user) is AnonymousUser or not user.id or not user.has_perms(
+        super()._validate_mutation(user, **data)
+        if not user.has_perms(
                 IndividualConfig.gql_group_delete_perms):
             raise ValidationError("mutation.authentication_required")
 
     @classmethod
     def _mutate(cls, user, **data):
         if "client_mutation_id" in data:
             data.pop('client_mutation_id')
@@ -214,68 +233,73 @@
 class CreateGroupIndividualMutation(BaseHistoryModelCreateMutationMixin, BaseMutation):
     _mutation_class = "CreateGroupIndividualMutation"
     _mutation_module = "individual"
     _model = GroupIndividual
 
     @classmethod
     def _validate_mutation(cls, user, **data):
-        if type(user) is AnonymousUser or not user.has_perms(
+        super()._validate_mutation(user, **data)
+        if not user.has_perms(
                 IndividualConfig.gql_group_create_perms):
             raise ValidationError("mutation.authentication_required")
 
     @classmethod
     def _mutate(cls, user, **data):
         if "client_mutation_id" in data:
             data.pop('client_mutation_id')
         if "client_mutation_label" in data:
             data.pop('client_mutation_label')
 
         service = GroupIndividualService(user)
-        service.create(data)
+        result = service.create(data)
+        return result if not result['success'] else None
 
     class Input(CreateGroupIndividualInputType):
         pass
 
 
 class UpdateGroupIndividualMutation(BaseHistoryModelUpdateMutationMixin, BaseMutation):
     _mutation_class = "UpdateGroupIndividualMutation"
     _mutation_module = "individual"
     _model = GroupIndividual
 
     @classmethod
     def _validate_mutation(cls, user, **data):
         super()._validate_mutation(user, **data)
-        if type(user) is AnonymousUser or not user.has_perms(
+        if not user.has_perms(
                 IndividualConfig.gql_group_update_perms):
             raise ValidationError("mutation.authentication_required")
 
     @classmethod
     def _mutate(cls, user, **data):
-        if "date_valid_to" not in data:
-            data['date_valid_to'] = None
         if "client_mutation_id" in data:
             data.pop('client_mutation_id')
         if "client_mutation_label" in data:
             data.pop('client_mutation_label')
 
         service = GroupIndividualService(user)
-        service.update(data)
+        if IndividualConfig.check_group_individual_update:
+            result = service.create_update_task(data)
+        else:
+            result = service.update(data)
+        return result if not result['success'] else None
 
     class Input(UpdateGroupIndividualInputType):
         pass
 
 
 class DeleteGroupIndividualMutation(BaseHistoryModelDeleteMutationMixin, BaseMutation):
     _mutation_class = "DeleteGroupIndividualMutation"
     _mutation_module = "individual"
     _model = GroupIndividual
 
     @classmethod
     def _validate_mutation(cls, user, **data):
-        if type(user) is AnonymousUser or not user.id or not user.has_perms(
+        super()._validate_mutation(user, **data)
+        if not user.has_perms(
                 IndividualConfig.gql_group_delete_perms):
             raise ValidationError("mutation.authentication_required")
 
     @classmethod
     def _mutate(cls, user, **data):
         if "client_mutation_id" in data:
             data.pop('client_mutation_id')
@@ -297,23 +321,90 @@
 class CreateGroupIndividualsMutation(BaseHistoryModelCreateMutationMixin, BaseMutation):
     _mutation_class = "CreateGroupIndividualsMutation"
     _mutation_module = "individual"
     _model = Group
 
     @classmethod
     def _validate_mutation(cls, user, **data):
-        if type(user) is AnonymousUser or not user.id or not user.has_perms(
+        super()._validate_mutation(user, **data)
+        if not user.has_perms(
                 IndividualConfig.gql_group_create_perms):
             raise ValidationError("mutation.authentication_required")
 
     @classmethod
     def _mutate(cls, user, **data):
         if "client_mutation_id" in data:
             data.pop('client_mutation_id')
         if "client_mutation_label" in data:
             data.pop('client_mutation_label')
 
         service = GroupService(user)
-        service.create_group_individuals(data)
+        result = service.create_group_individuals(data)
+        return result if not result['success'] else None
 
     class Input(CreateGroupInputType):
-        individual_ids = graphene.List(graphene.UUID)
+        individual_ids = graphene.List(graphene.UUID, required=True)
+
+
+class CreateGroupAndMoveIndividualMutation(BaseHistoryModelCreateMutationMixin, BaseMutation):
+    _mutation_class = "CreateGroupAndMoveIndividualMutation"
+    _mutation_module = "individual"
+    _model = Group
+
+    @classmethod
+    def _validate_mutation(cls, user, **data):
+        super()._validate_mutation(user, **data)
+
+        required_perms = IndividualConfig.gql_group_create_perms + IndividualConfig.gql_group_update_perms
+        if not user.has_perms(required_perms):
+            raise ValidationError("mutation.authentication_required")
+
+    @classmethod
+    def _mutate(cls, user, **data):
+        if "client_mutation_id" in data:
+            data.pop('client_mutation_id')
+        if "client_mutation_label" in data:
+            data.pop('client_mutation_label')
+
+        service = CreateGroupAndMoveIndividualService(user)
+        if IndividualConfig.check_group_individual_update or IndividualConfig.check_group_create:
+            result = service.create_create_task(data)
+        else:
+            result = service.create(data)
+        return result if not result['success'] else None
+
+    class Input(CreateGroupInputType):
+        group_individual_id = graphene.UUID(required=True)
+
+
+class ConfirmIndividualEnrollmentMutation(BaseHistoryModelCreateMutationMixin, BaseMutation):
+    _mutation_class = "ConfirmIndividualEnrollmentMutation"
+    _mutation_module = "individual"
+    _model = Individual
+
+    @classmethod
+    def _validate_mutation(cls, user, **data):
+        super()._validate_mutation(user, **data)
+        if not user.has_perms(
+                IndividualConfig.gql_group_create_perms):
+            raise ValidationError("mutation.authentication_required")
+
+    @classmethod
+    def _mutate(cls, user, **data):
+        if "client_mutation_id" in data:
+            data.pop('client_mutation_id')
+        if "client_mutation_label" in data:
+            data.pop('client_mutation_label')
+        custom_filters = data.pop('custom_filters', None)
+        benefit_plan_id = data.pop('benefit_plan_id', None)
+        status = data.pop('status', "ACTIVE")
+        service = IndividualService(user)
+        service.select_individuals_to_benefit_plan(
+            custom_filters,
+            benefit_plan_id,
+            status,
+            user,
+        )
+        return None
+
+    class Input(ConfirmIndividualEnrollmentInputType):
+        pass
```

### Comparing `openimis-be-individual-1.0.0/individual/migrations/0001_initial.py` & `openimis_be_individual-1.1.0/individual/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-individual-1.0.0/individual/migrations/0002_add_individual_rigts_for_admin.py` & `openimis_be_individual-1.1.0/individual/migrations/0002_add_individual_rigts_for_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-individual-1.0.0/individual/migrations/0003_group_groupindividual_historicalgroup_historicalgroupindividual.py` & `openimis_be_individual-1.1.0/individual/migrations/0003_group_groupindividual_historicalgroup_historicalgroupindividual.py`

 * *Files identical despite different names*

### Comparing `openimis-be-individual-1.0.0/individual/migrations/0004_add_group_rights_to_admin.py` & `openimis_be_individual-1.1.0/individual/migrations/0004_add_group_rights_to_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-individual-1.0.0/individual/migrations/0005_auto_20230621_1323.py` & `openimis_be_individual-1.1.0/individual/migrations/0005_auto_20230621_1323.py`

 * *Files identical despite different names*

### Comparing `openimis-be-individual-1.0.0/individual/migrations/0006_auto_20230621_1544.py` & `openimis_be_individual-1.1.0/individual/migrations/0006_auto_20230621_1544.py`

 * *Files identical despite different names*

### Comparing `openimis-be-individual-1.0.0/individual/migrations/0007_auto_20230630_0950.py` & `openimis_be_individual-1.1.0/individual/migrations/0007_auto_20230630_0950.py`

 * *Files identical despite different names*

### Comparing `openimis-be-individual-1.0.0/individual/tests/data.py` & `openimis_be_individual-1.1.0/individual/tests/data.py`

 * *Files identical despite different names*

### Comparing `openimis-be-individual-1.0.0/individual/tests/group_individual_service_test.py` & `openimis_be_individual-1.1.0/individual/tests/group_individual_service_test.py`

 * *Files identical despite different names*

### Comparing `openimis-be-individual-1.0.0/individual/tests/group_service_test.py` & `openimis_be_individual-1.1.0/individual/tests/group_service_test.py`

 * *Files identical despite different names*

### Comparing `openimis-be-individual-1.0.0/individual/tests/helpers.py` & `openimis_be_individual-1.1.0/individual/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-individual-1.0.0/individual/tests/individual_service_test.py` & `openimis_be_individual-1.1.0/individual/tests/individual_service_test.py`

 * *Files identical despite different names*

### Comparing `openimis-be-individual-1.0.0/openimis_be_individual.egg-info/PKG-INFO` & `openimis_be_individual-1.1.0/openimis_be_individual.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-individual
-Version: 1.0.0
+Version: 1.1.0
 Summary: The openIMIS Backend individual reference module.
 Home-page: https://openimis.org/
 Author: Kamil Malinowski
 Author-email: kmalinowski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -83,7 +83,17 @@
 * gql_group_create_perms: required rights to call createGroup and addIndividualToGroup and createGroupIndividuals GraphQL Mutation (default: ["180002"])
 * gql_group_update_perms: required rights to call updateGroup and editIndividualInGroup GraphQL Mutation (default: ["180003"])
 * gql_group_delete_perms: required rights to call deleteGroup and removeIndividualFromGroup GraphQL Mutation (default: ["180004"])
 
 
 ## openIMIS Modules Dependencies
 - core
+
+
+## Enabling Python Workflows
+Module comes with simple workflows for individual data upload. 
+They should be used for the development purposes, not in production environment. 
+To activate these Python workflows, a configuration change is required. 
+Specifically, the `enable_python_workflows` parameter to `true` within module config.
+
+Workflows: 
+ * individual upload
```

### Comparing `openimis-be-individual-1.0.0/setup.py` & `openimis_be_individual-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-individual',
-    version='1.0.0',
+    version='v1.1.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend individual reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

