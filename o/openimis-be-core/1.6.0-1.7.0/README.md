# Comparing `tmp/openimis-be-core-1.6.0.tar.gz` & `tmp/openimis_be_core-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-core-1.6.0.tar", last modified: Sat Dec 16 00:55:25 2023, max compression
+gzip compressed data, was "openimis_be_core-1.7.0.tar", last modified: Tue Apr 30 05:52:20 2024, max compression
```

## Comparing `openimis-be-core-1.6.0.tar` & `openimis_be_core-1.7.0.tar`

### file list

```diff
@@ -1,127 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.533663 openimis-be-core-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-12-16 00:55:25.533663 openimis-be-core-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20949 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.521663 openimis-be-core-1.6.0/core/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/abs_calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9169 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.521663 openimis-be-core-1.6.0/core/calendars/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/calendars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/calendars/ad_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/calendars/ne_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/calendars/test_ad_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/calendars/test_ne_calendar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.521663 openimis-be-core-1.6.0/core/custom_filters/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/custom_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/custom_filters/custom_filter_registry_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/custom_filters/custom_filter_wizard_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/custom_filters/custom_filter_wizard_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/custom_lookups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.525663 openimis-be-core-1.6.0/core/datetimes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/datetimes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/datetimes/ad_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/datetimes/ne_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/datetimes/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/datetimes/test_ad_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)    14463 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/datetimes/test_ne_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/datetimes/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.525663 openimis-be-core-1.6.0/core/gql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/gql/custom_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/gql/export_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.525663 openimis-be-core-1.6.0/core/gql/gql_mutations/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/gql/gql_mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9327 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/gql/gql_mutations/base_mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/gql/gql_mutations/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/gql/gql_mutations/input_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10223 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/gql/gql_mutations/mutation_by_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/gql_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/jwt_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.525663 openimis-be-core-1.6.0/core/migration_to_history_model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migration_to_history_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migration_to_history_model/create_temp_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migration_to_history_model/patch_table_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.529663 openimis-be-core-1.6.0/core/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0002_auto_20190726_0701.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0003_control_mutationlog.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0004_auto_20190830_1625.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0005_group_usergroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0006_fieldcontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0007_auto_20191008_0923.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0008_officer_role_roleright_userrole.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0009_mutationlog_client_mutation_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0010_rolemutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0011_auto_20210324_1528.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0012_users_officers_admins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0013_users_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0014_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0015_missing_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0016_add_last_login_on_interactive_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0017_exportablequerymodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0018_auto_20230318_1551.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0019_extended_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     9704 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0020_add_missing_fields_to_django_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0021_set_managed_to_true.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0022_auto_20230516_1742.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0023_alter_jsonext_column_in_tblOfficer.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0024_alter_usergroup_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/0025_mutationlog_json_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41899 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.529663 openimis-be-core-1.6.0/core/reports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   197363 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/reports/registers_status.py
--rw-r--r--   0 runner    (1001) docker     (127)   138570 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/reports/user_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    63507 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/service_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.529663 openimis-be-core-1.6.0/core/services/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/services/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/services/roleServices.py
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/services/userServices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.529663 openimis-be-core-1.6.0/core/services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/services/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/services/utils/serviceUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.533663 openimis-be-core-1.6.0/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/templates/password_reset.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/test_security.py
--rw-r--r--   0 runner    (1001) docker     (127)    19637 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9164 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.533663 openimis-be-core-1.6.0/core/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/validation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/validation/objectExistsValidationMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/validation/obligatoryFieldValidation.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/validation/uniqueCodeValidationMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.533663 openimis-be-core-1.6.0/core/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/websocket/abstract_websocket_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/websocket/async_websocket_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-12-16 00:55:14.000000 openimis-be-core-1.6.0/core/websocket/base_websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:55:25.533663 openimis-be-core-1.6.0/openimis_be_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-12-16 00:55:25.000000 openimis-be-core-1.6.0/openimis_be_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2023-12-16 00:55:25.000000 openimis-be-core-1.6.0/openimis_be_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:55:25.000000 openimis-be-core-1.6.0/openimis_be_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-16 00:55:25.000000 openimis-be-core-1.6.0/openimis_be_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-16 00:55:25.000000 openimis-be-core-1.6.0/openimis_be_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:55:25.533663 openimis-be-core-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-12-16 00:55:25.000000 openimis-be-core-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.649644 openimis_be_core-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-30 05:52:20.649644 openimis_be_core-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20949 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.633644 openimis_be_core-1.7.0/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/abs_calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.637644 openimis_be_core-1.7.0/core/calendars/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/calendars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/calendars/ad_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/calendars/ne_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/calendars/test_ad_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/calendars/test_ne_calendar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.637644 openimis_be_core-1.7.0/core/custom_filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/custom_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/custom_filters/custom_filter_registry_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/custom_filters/custom_filter_wizard_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/custom_filters/custom_filter_wizard_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/custom_lookups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.637644 openimis_be_core-1.7.0/core/datetimes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/datetimes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/datetimes/ad_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/datetimes/ne_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/datetimes/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/datetimes/test_ad_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14463 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/datetimes/test_ne_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/datetimes/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.637644 openimis_be_core-1.7.0/core/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/gql/custom_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/gql/export_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.637644 openimis_be_core-1.7.0/core/gql/gql_mutations/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/gql/gql_mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9327 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/gql/gql_mutations/base_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/gql/gql_mutations/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/gql/gql_mutations/input_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10223 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/gql/gql_mutations/mutation_by_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/gql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/jwt_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.641645 openimis_be_core-1.7.0/core/migration_to_history_model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migration_to_history_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migration_to_history_model/create_temp_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migration_to_history_model/patch_table_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.645645 openimis_be_core-1.7.0/core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0002_auto_20190726_0701.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0003_control_mutationlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0004_auto_20190830_1625.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0005_group_usergroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0006_fieldcontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0007_auto_20191008_0923.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0008_officer_role_roleright_userrole.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0009_mutationlog_client_mutation_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0010_rolemutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0011_auto_20210324_1528.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0012_users_officers_admins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0013_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0014_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0015_missing_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0016_add_last_login_on_interactive_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0017_exportablequerymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0018_auto_20230318_1551.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0019_extended_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0020_add_missing_fields_to_django_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0021_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0022_auto_20230516_1742.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0023_alter_jsonext_column_in_tblOfficer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0024_alter_usergroup_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0025_mutationlog_json_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0026_mutationlog_autogenerated_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0027_alter_interactiveuser_last_login_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/0028_alter_moduleconfiguration_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.645645 openimis_be_core-1.7.0/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/models/base_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/models/history_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/models/openimis_graphql_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22303 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/models/user_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/models/versioned_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.645645 openimis_be_core-1.7.0/core/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   197363 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/reports/registers_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138570 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/reports/user_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66610 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/service_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.645645 openimis_be_core-1.7.0/core/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/services/roleServices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10978 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/services/userServices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.645645 openimis_be_core-1.7.0/core/services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/services/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/services/utils/serviceUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.649644 openimis_be_core-1.7.0/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/templates/password_reset.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19699 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12732 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.649644 openimis_be_core-1.7.0/core/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/validation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/validation/objectExistsValidationMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/validation/obligatoryFieldValidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/validation/stringFieldValidationMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/validation/uniqueCodeValidationMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.649644 openimis_be_core-1.7.0/core/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/websocket/abstract_websocket_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/websocket/async_websocket_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-30 05:52:11.000000 openimis_be_core-1.7.0/core/websocket/base_websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:20.649644 openimis_be_core-1.7.0/openimis_be_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-30 05:52:20.000000 openimis_be_core-1.7.0/openimis_be_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-30 05:52:20.000000 openimis_be_core-1.7.0/openimis_be_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 05:52:20.000000 openimis_be_core-1.7.0/openimis_be_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-30 05:52:20.000000 openimis_be_core-1.7.0/openimis_be_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 05:52:20.000000 openimis_be_core-1.7.0/openimis_be_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 05:52:20.649644 openimis_be_core-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-30 05:52:20.000000 openimis_be_core-1.7.0/setup.py
```

### Comparing `openimis-be-core-1.6.0/LICENSE.md` & `openimis_be_core-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/PKG-INFO` & `openimis_be_core-1.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-core
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Core reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -23,7 +23,8 @@
 Requires-Dist: django-db-signals
 Requires-Dist: djangorestframework
 Requires-Dist: cached-property
 Requires-Dist: nepalicalendar
 Requires-Dist: django-simple-history
 Requires-Dist: django-dirtyfields
 Requires-Dist: websocket-client
+Requires-Dist: jsonschema
```

### Comparing `openimis-be-core-1.6.0/README.md` & `openimis_be_core-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/abs_calculation_rule.py` & `openimis_be_core-1.7.0/core/abs_calculation_rule.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/apps.py` & `openimis_be_core-1.7.0/core/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import sys
 import os
 import importlib
 import logging
 from django.apps import AppConfig
 from django.conf import settings
 
-
 logger = logging.getLogger(__name__)
 
 MODULE_NAME = "core"
 
 this = sys.modules[MODULE_NAME]
 
 DEFAULT_CFG = {
     "username_code_length": "8",  # cannot be bigger than 50 unless modified length limit
-    "user_username_and_code_length_limit": "50",
+    "username_changeable": True,
     "auto_provisioning_user_group": "user",
     "calendar_package": "core",
     "calendar_module": ".calendars.ad_calendar",
     "datetime_package": "core",
     "datetime_module": ".datetimes.ad_datetime",
     "shortstrfdate": "%d/%m/%Y",
     "longstrfdate": "%a %d %B %Y",
     "iso_raw_date": "False",
     "age_of_majority": "18",
-    "async_mutations": "False",
+    "async_mutations": "True" if os.environ.get("ASYNC", os.environ.get("MODE", "PROD")) == "PROD" else "False",
     "password_reset_template": "password_reset.txt",
     "currency": "$",
     "gql_query_users_perms": ["121701"],
     "gql_mutation_create_users_perms": ["121702"],
     "gql_mutation_update_users_perms": ["121703"],
     "gql_mutation_delete_users_perms": ["121704"],
     "gql_query_roles_perms": ["122001"],
@@ -47,23 +46,24 @@
     "gql_query_claim_administrator_perms": ["121601"],
     "gql_mutation_create_claim_administrator_perms": ["121602"],
     "gql_mutation_update_claim_administrator_perms": ["121603"],
     "gql_mutation_delete_claim_administrator_perms": ["121604"],
     "fields_controls_user": {},
     "fields_controls_eo": {},
     "is_valid_health_facility_contract_required": False,
-    "secondary_calendar": None
+    "secondary_calendar": None,
+    "locked_user_password_hash": 'locked'
 }
 
 
 class CoreConfig(AppConfig):
     default_auto_field = 'django.db.models.AutoField'  # Django 3.1+
     name = MODULE_NAME
     username_code_length = 8
-    user_username_and_code_length_limit = 50
+    username_changeable = True
     age_of_majority = 18
     password_reset_template = "password_reset.txt"
     gql_query_roles_perms = []
     gql_mutation_create_roles_perms = []
     gql_mutation_update_roles_perms = []
     gql_mutation_replace_roles_perms = []
     gql_mutation_duplicate_roles_perms = []
@@ -80,14 +80,15 @@
     gql_mutation_update_enrolment_officers_perms = []
     gql_mutation_delete_enrolment_officers_perms = []
     gql_query_claim_administrator_perms = []
     gql_mutation_create_claim_administrator_perms = []
     gql_mutation_update_claim_administrator_perms = []
     gql_mutation_delete_claim_administrator_perms = []
     is_valid_health_facility_contract_required = None
+    locked_user_password_hash = None
 
     fields_controls_user = {}
     fields_controls_eo = {}
     secondary_calendar = None
 
     def _import_module(self, cfg, k):
         logger.info('import %s.%s' %
@@ -105,19 +106,19 @@
             this.datetime = self._import_module(cfg, "datetime")
         except Exception:
             logger.error('Failed to configure calendar, using default!\n%s: %s' % (
                 sys.exc_info()[0].__name__, sys.exc_info()[1]))
             this.calendar = self._import_module(DEFAULT_CFG, "calendar")
             this.datetime = self._import_module(DEFAULT_CFG, "datetime")
 
-    def _configure_username_code_length(self, cfg):
+    def _configure_user_config(self, cfg):
         this.username_code_length = int(cfg["username_code_length"])
-
-    def _configure_user_username_and_code_length_limit(self, cfg):
-        this.user_username_and_code_length_limit = int(cfg["user_username_and_code_length_limit"])
+        # Quick fix, this config has to be rebuilt
+        CoreConfig.username_code_length = int(cfg["username_code_length"])
+        CoreConfig.username_changeable = cfg["username_changeable"]
 
     def _configure_majority(self, cfg):
         this.age_of_majority = int(cfg["age_of_majority"])
 
     def _configure_currency(self, cfg):
         this.currency = str(cfg["currency"])
 
@@ -171,22 +172,22 @@
         CoreConfig.is_valid_health_facility_contract_required = cfg["is_valid_health_facility_contract_required"]
         CoreConfig.secondary_calendar = cfg["secondary_calendar"]
 
     def ready(self):
         from .models import ModuleConfiguration
         cfg = ModuleConfiguration.get_or_default(MODULE_NAME, DEFAULT_CFG)
         self._configure_calendar(cfg)
-        self._configure_username_code_length(cfg)
-        self._configure_user_username_and_code_length_limit(cfg)
+        self._configure_user_config(cfg)
         self._configure_majority(cfg)
         self._configure_auto_provisioning(cfg)
         self._configure_graphql(cfg)
         self._configure_currency(cfg)
         self._configure_permissions(cfg)
         self._configure_additional_settings(cfg)
 
-        self.password_reset_template = cfg["password_reset_template"]
+        CoreConfig.password_reset_template = cfg["password_reset_template"]
+        CoreConfig.locked_user_password_hash = cfg["locked_user_password_hash"]
 
         # The scheduler starts as soon as it gets a job, which could be before Django is ready, so we enable it here
         from core import scheduler
         if settings.SCHEDULER_AUTOSTART:
             scheduler.start()
```

### Comparing `openimis-be-core-1.6.0/core/calendars/ad_calendar.py` & `openimis_be_core-1.7.0/core/calendars/ad_calendar.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/calendars/ne_calendar.py` & `openimis_be_core-1.7.0/core/calendars/ne_calendar.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/calendars/test_ad_calendar.py` & `openimis_be_core-1.7.0/core/calendars/test_ad_calendar.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/calendars/test_ne_calendar.py` & `openimis_be_core-1.7.0/core/calendars/test_ne_calendar.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/custom_filters/custom_filter_registry_point.py` & `openimis_be_core-1.7.0/core/custom_filters/custom_filter_registry_point.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/custom_filters/custom_filter_wizard_interface.py` & `openimis_be_core-1.7.0/core/custom_filters/custom_filter_wizard_interface.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/custom_filters/custom_filter_wizard_storage.py` & `openimis_be_core-1.7.0/core/custom_filters/custom_filter_wizard_storage.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/custom_lookups.py` & `openimis_be_core-1.7.0/core/custom_lookups.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from django.db.models import Lookup, JSONField
 from django.db.models.lookups import Contains
+from itertools import chain
+
+from django.conf import settings
+
 
 
-@JSONField.register_lookup
 class JsonContains(Lookup):
-    lookup_name = 'jsoncontains'
+    lookup_name = 'contains'
 
     sql_server_json_key_prefix = '$'
     sql_server_nested_json_separator = '.'
     BASE_SQL = '(JSON_VALUE(cast({} as nvarchar(max)), %s)=%s)'
 
-    def as_sql(self, qn, connection):
-        lhs, lhs_params = self.process_lhs(qn, connection)
-        rhs, rhs_params = self.process_rhs(qn, connection)
-
-        rhs_params[0].prepare(connection)
-        params = self._build_sql_params(lhs, rhs_params[0].adapted)
-        sql_statement = ' AND '.join([self.BASE_SQL.format(lhs) for _ in range(0, len(rhs_params[0].adapted))])
+    def as_sql(self, compiler, connection):
+        
+        lhs, lhs_params = self.process_lhs(compiler, connection)
+        rhs, rhs_params = self.process_rhs(compiler, connection)
+        # have the json section and value of the json section in params
+        params = list(chain.from_iterable([[f"'{list(rhs_params[0].keys())[_]}'", f"'{rhs_params[0][list(rhs_params[0].keys())[_]][0]}'"] for _ in range(0, len(rhs_params[0]))]))
+        sql_statement = ' AND '.join([self.BASE_SQL.format(lhs)    for _ in range(0, len(rhs_params[0]))])
         return sql_statement, params
 
     def _prepare_dict_value(self, json_ext):
         def flatten(dictionary, separator, prefix):
             return {
                 prefix + separator + key if prefix else key: value
                 for nested_key, nested_value in dictionary.items()
@@ -37,17 +40,22 @@
         for json_key, expected_value in adjusted_conditions.items():
             # conditions.append(entity)
             conditions.append(json_key)
             conditions.append(expected_value)
         return conditions
 
 
-@JSONField.register_lookup
 class JsonContainsKey(Contains):
-    lookup_name = 'jsoncontainskey'
+    lookup_name = 'containskey'
 
     def __init__(self, lhs, rhs):
         rhs = f'"{rhs}":'
         super().__init__(lhs, rhs)
 
     def get_rhs_op(self, connection, rhs):
         return connection.operators['contains'] % rhs
+    
+    
+if settings.MSSQL:
+    JSONField.register_lookup(JsonContains)
+    JSONField.register_lookup(JsonContainsKey)
+
```

### Comparing `openimis-be-core-1.6.0/core/datetimes/ad_datetime.py` & `openimis_be_core-1.7.0/core/datetimes/ad_datetime.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,26 +105,39 @@
     @classmethod
     def from_ad_datetime(cls, value):
         if value is None:
             return None
         return AdDatetime(value.year, value.month, value.day,
                           value.hour, value.minute, value.second, value.microsecond,
                           value.tzinfo)
+    
+    def __hash__(self):
+        return super().__hash__()
 
     def to_ad_datetime(self):
         return self
 
-    def __eq__(self, other):
-        if other is None:
-            return super(AdDatetime, self).__eq__(other)
+    def _date_operation(self, operation, other):
+
+        if not other :
+            return operation(other)
         if isinstance(other, py_datetime.datetime):
-            return super(AdDatetime, self).__eq__(other)
+            return operation(other)
         if isinstance(other, py_datetime.date):
-            return super(AdDatetime, self).__eq__(AdDatetime.from_ad_date(other))
-        return self - other == datetimedelta()
+            return operation(AdDatetime.from_ad_date(other))
+    
+    def __eq__(self, other):
+        result = self._date_operation(super(AdDatetime, self).__eq__,other)
+        return result if result else self - other ==  datetimedelta()
+    
+    def __gt__(self, other):
+        return self._date_operation(super(AdDatetime, self).__gt__,other)
+    def __lt__(self, other):
+        return self._date_operation(super(AdDatetime, self).__lt__,other)
+
 
     @classmethod
     def _convert_op_res(cls, res):
         if isinstance(res, py_datetime.datetime):
             return AdDatetime.from_ad_datetime(res)
         return res
```

### Comparing `openimis-be-core-1.6.0/core/datetimes/ne_datetime.py` & `openimis_be_core-1.7.0/core/datetimes/ne_datetime.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/datetimes/shared.py` & `openimis_be_core-1.7.0/core/datetimes/shared.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import timedelta
+from datetime import timedelta, date, datetime
 
 __all__ = ["is_midnight", "datetimedelta"]
 
 
 def _cmperror(x, y):
     raise TypeError("can't compare '%s' to '%s'" % (
                     type(x).__name__, type(y).__name__))
@@ -98,37 +98,42 @@
         dt = self._add_months(dt)
         return dt + self._timedelta
 
     def add_to_datetime(self, datetime):
         return self.add_to_date(datetime)
 
     def __add__(self, other):
-        if isinstance(other, datetimedelta):
+        if isinstance(other, (datetimedelta)):
             return datetimedelta(years=self.years + other.years,
                                  months=self.months + other.months,
                                  days=self.days + other.days,
                                  seconds=self.seconds + other.seconds,
                                  microseconds=self.microseconds + other.microseconds)
+        elif isinstance(other, (date, datetime)):
+            return self.add_to_date( other)
         return NotImplemented
 
-    __radd__ = __add__
+    def __radd__(self, other):
+        return self.__add__(other)
 
     def __sub__(self, other):
-        if isinstance(other, datetimedelta):
+        if isinstance(other, (datetimedelta)):
             return datetimedelta(years=self.years - other.years,
                                  months=self.months - other.months,
                                  days=self.days - other.days,
                                  seconds=self.seconds - other.seconds,
                                  microseconds=self.microseconds - other.microseconds)
         return NotImplemented
 
     def __rsub__(self, other):
-        if isinstance(other, datetimedelta):
-            return -self + other
-        return NotImplemented
+        if isinstance(other, (date, datetime)):
+            sub = - self
+            return sub.__add__(other)
+        return self.__sub__(other)
+
 
     def __neg__(self):
         return datetimedelta(years=-self.years,
                              months=-self.months,
                              days=-self.days,
                              seconds=-self.seconds,
                              microseconds=-self.microseconds)
```

### Comparing `openimis-be-core-1.6.0/core/datetimes/test_ad_datetime.py` & `openimis_be_core-1.7.0/core/datetimes/test_ad_datetime.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/datetimes/test_ne_datetime.py` & `openimis_be_core-1.7.0/core/datetimes/test_ne_datetime.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/datetimes/test_shared.py` & `openimis_be_core-1.7.0/core/datetimes/test_shared.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/fields.py` & `openimis_be_core-1.7.0/core/fields.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/forms.py` & `openimis_be_core-1.7.0/core/forms.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/gql/export_mixin.py` & `openimis_be_core-1.7.0/core/gql/export_mixin.py`

 * *Files 12% similar despite different names*

```diff
@@ -99,16 +99,20 @@
                 f"Query {cls} doesn't provide resolve function for {field_name}. "
                 f"CSV export cannot be created")
 
         def exporter(cls, self, info, **kwargs):
             custom_filters = kwargs.pop("customFilters", None)
             export_fields = [cls._adjust_notation(f) for f in kwargs.pop('fields')]
             fields_mapping = json.loads(kwargs.pop('fields_columns'))
+
+            source_field = getattr(cls, field_name)
+            filter_kwargs = {k: v for k, v in kwargs.items() if k in source_field.filtering_args}
+
             qs = default_resolve(None, info, **kwargs)
-            qs = qs.filter(**kwargs)
+            qs = qs.filter(**filter_kwargs)
             qs = cls.__append_custom_filters(custom_filters, qs)
             export_file = ExportableQueryModel\
                 .create_csv_export(qs, export_fields, info.context.user, column_names=fields_mapping,
                                    patches=cls.get_patches_for_field(field_name))
 
             return export_file.name
```

### Comparing `openimis-be-core-1.6.0/core/gql/gql_mutations/base_mutation.py` & `openimis_be_core-1.7.0/core/gql/gql_mutations/base_mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/gql/gql_mutations/exceptions.py` & `openimis_be_core-1.7.0/core/gql/gql_mutations/exceptions.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/gql/gql_mutations/mutation_by_filter.py` & `openimis_be_core-1.7.0/core/gql/gql_mutations/mutation_by_filter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/gql_queries.py` & `openimis_be_core-1.7.0/core/gql_queries.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/jwt.py` & `openimis_be_core-1.7.0/core/jwt.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/jwt_authentication.py` & `openimis_be_core-1.7.0/core/jwt_authentication.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,18 +25,20 @@
         if not token:
             return
 
         # Do not pass context to avoid to try to get user from request to get his private key.
         try:
             user = get_user_by_token(token)
         except (jwt.PyJWTError, JSONWebTokenError) as exc:
+            raise exceptions.AuthenticationFailed("INCORRECT_CREDENTIALS") from exc
+        except Exception as exc:
             raise exceptions.AuthenticationFailed(str(exc)) from exc
-
-        if CoreConfig.is_valid_health_facility_contract_required:
-            if (hasattr(user, 'health_facility') and hasattr(user.health_facility, 'contract_end_date') and
-                    user.health_facility.contract_end_date > date.today()):
-                raise exceptions.AuthenticationFailed("HF_CONTRACT_INVALID")
+        else:
+            if CoreConfig.is_valid_health_facility_contract_required:
+                if not (hasattr(user, 'health_facility') and hasattr(user.health_facility, 'contract_end_date') and
+                        user.health_facility.contract_end_date > date.today()):
+                    raise exceptions.AuthenticationFailed("HF_CONTRACT_INVALID")
 
         return user, None
 
     def enforce_csrf(self, request):
         return  # To not perform the csrf during checking auth header
```

### Comparing `openimis-be-core-1.6.0/core/migration_to_history_model/create_temp_tables.py` & `openimis_be_core-1.7.0/core/migration_to_history_model/create_temp_tables.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migration_to_history_model/patch_table_data.py` & `openimis_be_core-1.7.0/core/migration_to_history_model/patch_table_data.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0001_initial.py` & `openimis_be_core-1.7.0/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0002_auto_20190726_0701.py` & `openimis_be_core-1.7.0/core/migrations/0002_auto_20190726_0701.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0003_control_mutationlog.py` & `openimis_be_core-1.7.0/core/migrations/0003_control_mutationlog.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0004_auto_20190830_1625.py` & `openimis_be_core-1.7.0/core/migrations/0004_auto_20190830_1625.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0005_group_usergroup.py` & `openimis_be_core-1.7.0/core/migrations/0005_group_usergroup.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0006_fieldcontrol.py` & `openimis_be_core-1.7.0/core/migrations/0006_fieldcontrol.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0008_officer_role_roleright_userrole.py` & `openimis_be_core-1.7.0/core/migrations/0008_officer_role_roleright_userrole.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0010_rolemutation.py` & `openimis_be_core-1.7.0/core/migrations/0010_rolemutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0011_auto_20210324_1528.py` & `openimis_be_core-1.7.0/core/migrations/0011_auto_20210324_1528.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0012_users_officers_admins.py` & `openimis_be_core-1.7.0/core/migrations/0012_users_officers_admins.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0013_users_api.py` & `openimis_be_core-1.7.0/core/migrations/0013_users_api.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0014_users.py` & `openimis_be_core-1.7.0/core/migrations/0014_users.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0015_missing_roles.py` & `openimis_be_core-1.7.0/core/migrations/0015_missing_roles.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0016_add_last_login_on_interactive_user.py` & `openimis_be_core-1.7.0/core/migrations/0016_add_last_login_on_interactive_user.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0017_exportablequerymodel.py` & `openimis_be_core-1.7.0/core/migrations/0017_exportablequerymodel.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0018_auto_20230318_1551.py` & `openimis_be_core-1.7.0/core/migrations/0018_auto_20230318_1551.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0020_add_missing_fields_to_django_scheme.py` & `openimis_be_core-1.7.0/core/migrations/0020_add_missing_fields_to_django_scheme.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0021_set_managed_to_true.py` & `openimis_be_core-1.7.0/core/migrations/0021_set_managed_to_true.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0022_auto_20230516_1742.py` & `openimis_be_core-1.7.0/core/migrations/0022_auto_20230516_1742.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/migrations/0023_alter_jsonext_column_in_tblOfficer.py` & `openimis_be_core-1.7.0/core/migrations/0023_alter_jsonext_column_in_tblOfficer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/report.py` & `openimis_be_core-1.7.0/core/report.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/reports/registers_status.py` & `openimis_be_core-1.7.0/core/reports/registers_status.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/reports/user_activity.py` & `openimis_be_core-1.7.0/core/reports/user_activity.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/scheduler.py` & `openimis_be_core-1.7.0/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/schema.py` & `openimis_be_core-1.7.0/core/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -146,44 +146,93 @@
         if isinstance(o, decimal.Decimal):
             return float(o)
         return super().default(o)
 
 
 _mutation_signal_params = ["user", "mutation_module",
                            "mutation_class", "mutation_log_id", "data"]
-signal_mutation = dispatch.Signal(providing_args=_mutation_signal_params)
+signal_mutation = dispatch.Signal(_mutation_signal_params)
 signal_mutation_module_validate = {}
 signal_mutation_module_before_mutating = {}
 signal_mutation_module_after_mutating = {}
 
 for module in sys.modules:
-    signal_mutation_module_validate[module] = dispatch.Signal(providing_args=_mutation_signal_params)
-    signal_mutation_module_before_mutating[module] = dispatch.Signal(providing_args=_mutation_signal_params)
+    signal_mutation_module_validate[module] = dispatch.Signal(_mutation_signal_params)
+    signal_mutation_module_before_mutating[module] = dispatch.Signal(_mutation_signal_params)
     signal_mutation_module_after_mutating[module] = \
-        dispatch.Signal(providing_args=_mutation_signal_params + ["error_messages"])
+        dispatch.Signal(_mutation_signal_params + ["error_messages"])
 
 
 class OpenIMISMutation(graphene.relay.ClientIDMutation):
     """
     This class is the generic Mutation for openIMIS. It will save the mutation content into the MutationLog,
     submit it to validation, perform the potentially asynchronous mutation itself and update the MutationLog status.
     """
 
     class Meta:
         abstract = True
 
     internal_id = graphene.Field(graphene.String)
 
+
     class Input:
         client_mutation_label = graphene.String(max_length=255, required=False)
         client_mutation_details = graphene.List(graphene.String)
         mutation_extensions = ParsedJSONString(
             description="Extension data to be used by signals. Will not be pushed to mutation implementation.")
 
     @classmethod
+    def coerce_mutation_data(cls, input_data, input_class = None):
+        if input_class is None:
+            input_class=cls.Input
+        coerced_data = {}
+        # Iterate through the input data dictionary
+        for key, value in input_data.items():
+            if hasattr(input_class, key):
+                # Get the field type from the input class
+                field = getattr(input_class, key)
+                # If the field type is List and the value is a list
+                if field.__class__ == graphene.List and isinstance(value, list):
+                    # Check if the list items need coercion
+                    inner_type = field.of_type
+                    coerced_list = []
+                    for item in value:
+                        if isinstance(item, str):
+                            coerced_list.append(inner_type.parse_value(item))
+                        elif inner_type.__class__ == graphene.utils.subclass_with_meta.SubclassWithMeta_Meta:
+                            coerced_list.append(cls.coerce_mutation_data(item, input_class = inner_type))
+                        else:
+                            coerced_list.append(item)
+                    coerced_data[key] = coerced_list
+                elif field.__class__ == graphene.types.field.Field and isinstance(field.type, graphene.types.enum.EnumMeta):
+                    # If the field type is Enum
+                    if hasattr(field.type,value):
+                        coerced_data[key] = str(getattr(field.type,value).value)
+                    else: 
+                        coerced_data[key] = value
+                elif field.__class__ == graphene.types.field.Field and isinstance(field.type,graphene.types.structures.NonNull)\
+                    and isinstance(field.type._of_type,graphene.types.enum.EnumMeta):
+                    # If the field type is Enum
+                    if hasattr(field.type,value):
+                        coerced_data[key] = str(getattr(field.type._of_type,value).value)
+                    else: 
+                        coerced_data[key] = value
+                elif field.__class__ == graphene.types.field.Field:
+                    coerced_data[key] = cls.coerce_mutation_data(value, input_class = field._type)
+                elif isinstance(value, str):
+                    coerced_data[key] = field.parse_value(value)
+                else:
+                    coerced_data[key] = value
+            else:
+                logger.debug(f"key {key} not in {cls.__name__}")
+                coerced_data[key] = value
+           
+        return coerced_data
+        
+    @classmethod
     def async_mutate(cls, user, **data) -> List[Dict[str, Any]]:
         """
         This method has to be overridden in the subclasses to implement the actual mutation.
         The response should contain a boolean for success and an error message that will be saved into the DB
         :param user: contains the logged user or None
         :param data: all parameters passed to the mutation
         :return: error_message if None is returned, the response is considered to be a success
@@ -224,49 +273,50 @@
             logger.debug("[OpenIMISMutation %s] Sending signals", mutation_log.id)
             results = signal_mutation.send(
                 sender=cls,
                 mutation_log_id=mutation_log.id,
                 data=data,
                 user=info.context.user,
                 mutation_module=cls._mutation_module,
-                mutation_class=cls._mutation_class,
+                mutation_class=cls.__name__,
             )
             results.extend(
                 signal_mutation_module_validate[cls._mutation_module].send(
                     sender=cls,
                     mutation_log_id=mutation_log.id,
                     data=data,
                     user=info.context.user,
                     mutation_module=cls._mutation_module,
-                    mutation_class=cls._mutation_class,
+                    mutation_class=cls.__name__,
                 )
             )
             errors = [err for r in results for err in r[1]]
             logger.debug(
                 "[OpenIMISMutation %s] signals sent, got errors back: %d",
                 mutation_log.id,
                 len(errors),
             )
             if errors:
                 mutation_log.mark_as_failed(json.dumps(errors))
                 return cls(internal_id=mutation_log.id)
 
             signal_mutation_module_before_mutating[cls._mutation_module].send(
                 sender=cls, mutation_log_id=mutation_log.id, data=data, user=info.context.user,
-                mutation_module=cls._mutation_module, mutation_class=cls._mutation_class
+                mutation_module=cls._mutation_module, mutation_class=cls.__name__
             )
             logger.debug("[OpenIMISMutation %s] before mutate signal sent", mutation_log.id)
             if core.async_mutations:
                 logger.debug("[OpenIMISMutation %s] Sending async mutation", mutation_log.id)
                 openimis_mutation_async.delay(
-                    mutation_log.id, cls._mutation_module, cls._mutation_class)
+                    mutation_log.id, cls._mutation_module, cls.__name__)
             else:
                 logger.debug("[OpenIMISMutation %s] mutating...", mutation_log.id)
                 try:
                     mutation_data = data.copy()
+                    #mutation_data = cls.coerce_mutation_data(json.loads(json.dumps(data, cls=OpenIMISJSONEncoder))) #data.copy() 
                     mutation_data.pop("mutation_extensions", None)
                     messages = cls.async_mutate(
                         info.context.user if info.context and info.context.user else None,
                         **mutation_data)
                     # TODO this code is necessary for autogenerate functionality to work
                     # TODO General mutation code should be reworked
                     if mutation_data.get('autogenerate', False) and isinstance(messages, Dict):
@@ -288,15 +338,15 @@
                     error_messages = exc
                     logger.error("async_mutate threw an exception. It should have gotten this far.", exc_info=exc)
                     # Record the failure of the mutation but don't include details for security reasons
                     mutation_log.mark_as_failed(f"The mutation threw a {type(exc)}, check logs for details")
                 logger.debug("[OpenIMISMutation %s] send post mutation signal", mutation_log.id)
                 signal_mutation_module_after_mutating[cls._mutation_module].send(
                     sender=cls, mutation_log_id=mutation_log.id, data=data, user=info.context.user,
-                    mutation_module=cls._mutation_module, mutation_class=cls._mutation_class,
+                    mutation_module=cls._mutation_module, mutation_class=cls.__name__,
                     error_messages=error_messages
                 )
         except Exception as exc:
             logger.error(f"Exception while processing mutation id {mutation_log.id}", exc_info=exc)
             mutation_log.mark_as_failed(exc)
 
         return cls(internal_id=mutation_log.id)
@@ -428,14 +478,15 @@
     mutation_logs = OrderedDjangoFilterConnectionField(
         MutationLogGQLType, orderBy=graphene.List(of_type=graphene.String))
 
     role = OrderedDjangoFilterConnectionField(
         RoleGQLType,
         orderBy=graphene.List(of_type=graphene.String),
         is_system=graphene.Boolean(),
+        role_right=graphene.Int(),
         system_role_id=graphene.Int(),
         show_history=graphene.Boolean(),
         client_mutation_id=graphene.String(),
         str=graphene.String(description="Text search on any field")
     )
 
     role_right = OrderedDjangoFilterConnectionField(
@@ -657,16 +708,16 @@
             raise PermissionError("Unauthorized")
 
         user_filters = []
         user_query = User.objects.exclude(t_user__isnull=False)
 
         show_deleted = kwargs.get('showDeleted', False)
         if not show_deleted and not kwargs.get('id', None):
-            
-            #active_users_ids = [user.id for user in user_query if user.is_active]
+
+            # active_users_ids = [user.id for user in user_query if user.is_active]
             user_filters.append(Q(i_user__isnull=True) | Q(*filter_validity(prefix='i_user__')))
 
         text_search = kwargs.get("str")  # Poorly chosen name, avoid of shadowing "str"
         if text_search:
             user_filters.append(Q(username__icontains=text_search) |
                                 Q(i_user__last_name__icontains=text_search) |
                                 Q(officer__last_name__icontains=text_search) |
@@ -756,14 +807,18 @@
 
     def resolve_role(self, info, **kwargs):
         if not info.context.user.has_perms(CoreConfig.gql_query_roles_perms):
             raise PermissionError("Unauthorized")
         filters = []
         query = Role.objects
 
+        role_right = kwargs.get("role_right", None)
+        if role_right:
+            filters.append(Q(rights__validity_to__isnull=True, rights__right_id=role_right))
+
         text_search = kwargs.get("str")
         if text_search:
             filters.append(Q(name__icontains=text_search))
 
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
             filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
@@ -836,15 +891,16 @@
         return ModulePermissionsListGQLType(list(config))
 
     def resolve_custom_filters(self, info, **kwargs):
         user = info.context.user
         if type(user) is AnonymousUser or not user.id:
             raise PermissionError("Unauthorized")
 
-        module_name, object_type_name, uuid_of_object, additional_params = Query._obtain_params_from_custom_filter_graphql_query(**kwargs)
+        module_name, object_type_name, uuid_of_object, additional_params = Query._obtain_params_from_custom_filter_graphql_query(
+            **kwargs)
         custom_filter_list_output = Query._obtain_definition_of_custom_filter_from_hub(
             module_name, object_type_name, uuid_of_object, additional_params
         )
         possible_filters = Query._build_possible_custom_filter_options(custom_filter_list_output)
         return CustomFilterGQLType(
             type=object_type_name,
             code=module_name,
@@ -1336,14 +1392,17 @@
         raise ValidationError(_("mutation.user_no_email_provided"))
 
     username = data.get('username')
 
     if len(username) > CoreConfig.username_code_length:
         raise ValidationError(_("mutation.user_username_too_long"))
 
+    if not CoreConfig.username_changeable and current_user.username != username:
+        raise ValidationError(_("mutation.user_username_not_changeable"))
+
     if "client_mutation_id" in data:
         data.pop('client_mutation_id')
     if "client_mutation_label" in data:
         data.pop('client_mutation_label')
     user_uuid = data.pop('uuid') if 'uuid' in data else None
 
     if UT_INTERACTIVE in data["user_types"]:
@@ -1514,16 +1573,19 @@
     @classmethod
     def mutate(cls, root, info, **kwargs):
         username = kwargs.get("username")
         # consider auto-provisioning
         if username:
             # get_or_create will auto-provision from tblUsers if applicable
             user = User.objects.get_or_create(username=username)
-            if user:
+            if not user:
                 logger.debug("Authentication with %s failed and could not be fetched from tblUsers", username)
+            else:
+                kwargs[User.USERNAME_FIELD] = user[0].username
+
         return super().mutate(cls, info, **kwargs)
 
 
 class Mutation(graphene.ObjectType):
     create_role = CreateRoleMutation.Field()
     update_role = UpdateRoleMutation.Field()
     delete_role = DeleteRoleMutation.Field()
```

### Comparing `openimis-be-core-1.6.0/core/serializers.py` & `openimis_be_core-1.7.0/core/serializers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from rest_framework import serializers
+
+from .apps import CoreConfig
 from .models import User, InteractiveUser, TechnicalUser
 
 
 class InteractiveUserSerializer(serializers.ModelSerializer):
     language = serializers.PrimaryKeyRelatedField(many=False, read_only=True)
+    has_password = serializers.SerializerMethodField()
+
+    def get_has_password(self, obj):
+        return obj.stored_password != CoreConfig.locked_user_password_hash
 
     class Meta:
         model = InteractiveUser
         fields = ('id', 'language', 'last_name',
-                  'other_names', 'health_facility_id', 'rights')
+                  'other_names', 'health_facility_id', 'rights', 'has_password')
 
 
 class TechnicalUserSerializer(serializers.ModelSerializer):
     class Meta:
         model = TechnicalUser
         fields = ('id', 'language', 'username', 'email')
```

### Comparing `openimis-be-core-1.6.0/core/service_signals.py` & `openimis_be_core-1.7.0/core/service_signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         self.__signals_before = []
         self.__signals_after = []
 
         if not providing_args:
             self.__before_service_signal = None
             self.__after_service_signal = None
         else:
-            self.__before_service_signal = dispatch.Signal(providing_args=providing_args)
-            self.__after_service_signal = dispatch.Signal(providing_args=providing_args + ['result'])
+            self.__before_service_signal = dispatch.Signal(providing_args)
+            self.__after_service_signal = dispatch.Signal(providing_args + ['result'])
 
     @property
     def connected_signals(self):
         return {
             'before': self.__signals_before,
             'after': self.__signals_after
         }
@@ -67,16 +67,16 @@
         else:
             self.__connection_queue[bind_type].put(func)
 
     def register_signal(self, providing_args):
         if self.is_signal_registered():
             raise ValueError(f"Signal {self} already registered.")
 
-        self.__before_service_signal = dispatch.Signal(providing_args=providing_args)
-        self.__after_service_signal = dispatch.Signal(providing_args=providing_args + ['result'])
+        self.__before_service_signal = dispatch.Signal(providing_args)
+        self.__after_service_signal = dispatch.Signal(providing_args + ['result'])
         self._connect_queued()
 
     def is_signal_registered(self):
         return self.__before_service_signal is not None and self.__after_service_signal is not None
 
     def _add_connection(self, func, bind_type):
         if bind_type == ServiceSignalBindType.BEFORE:
```

### Comparing `openimis-be-core-1.6.0/core/services/base.py` & `openimis_be_core-1.7.0/core/services/base.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/services/userServices.py` & `openimis_be_core-1.7.0/core/services/userServices.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         created = False
     else:
         i_user = InteractiveUser(**data_subset)
         if "password" in data:
             i_user.set_password(data["password"])
         else:
             # No password provided for creation, will have to be set later.
-            i_user.stored_password = "locked"
+            i_user.stored_password = CoreConfig.locked_user_password_hash
         created = True
 
     i_user.save()
     create_or_update_user_roles(i_user, data["roles"], audit_user_id)
     if "districts" in data:
         create_or_update_user_districts(
             i_user, data["districts"], data_subset["audit_user_id"]
@@ -230,15 +230,16 @@
 def change_user_password(logged_user, username_to_update=None, old_password=None, new_password=None):
     if username_to_update and username_to_update != logged_user.username:
         if not logged_user.has_perms(CoreConfig.gql_mutation_update_users_perms):
             raise PermissionDenied("unauthorized")
         user_to_update = User.objects.get(username=username_to_update)
     else:
         user_to_update = logged_user
-        if not old_password or not user_to_update.check_password(old_password):
+        old_password_match = old_password and user_to_update.check_password(old_password)
+        if not (old_password_match or user_to_update.stored_password == CoreConfig.locked_user_password_hash):
             raise ValidationError(_("core.wrong_old_password"))
 
     user_to_update.set_password(new_password)
     user_to_update.save()
 
 
 def set_user_password(request, username, token, password):
```

### Comparing `openimis-be-core-1.6.0/core/services/utils/serviceUtils.py` & `openimis_be_core-1.7.0/core/services/utils/serviceUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,11 +72,8 @@
         "detail": "",
     }
 
 
 def get_generic_type(generic_type: Union[str, ContentType]):
     if isinstance(generic_type, ContentType):
         return generic_type
-    elif isinstance(generic_type, str):
-        return ContentType.objects.get(model__iexact=generic_type.lower())
-    else:
-        return ContentType.objects.get(model__iexact=str(generic_type).lower())
+    return ContentType.objects.get(model__iexact=str(generic_type).lower())
```

### Comparing `openimis-be-core-1.6.0/core/signals.py` & `openimis_be_core-1.7.0/core/signals.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/tasks.py` & `openimis_be_core-1.7.0/core/tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,19 +27,23 @@
 
         if mutation.user and mutation.user.language:
             lang = mutation.user.language
             if isinstance(lang, Language):
                 translation.activate(lang.code)
             else:
                 translation.activate(lang)
-        error_messages = mutation_class.async_mutate(mutation.user, **json.loads(mutation.json_content))
+        error_messages = mutation_class.async_mutate(mutation.user, **mutation_class.coerce_mutation_data(json.loads(mutation.json_content)))
         if not error_messages:
             mutation.mark_as_successful()
         else:
-            mutation.mark_as_failed(json.dumps(error_messages))
+            logger.debug(f"error :{error_messages}")
+            try:
+                mutation.mark_as_failed(json.dumps(error_messages))
+            except:
+                mutation.mark_as_failed(error_messages)
         return "OK"
     except Exception as exc:
         if mutation:
             mutation.mark_as_failed(str(exc))
         logger.warning(f"Exception while processing mutation id {mutation_id}", exc_info=True)
         raise exc
```

### Comparing `openimis-be-core-1.6.0/core/test_models.py` & `openimis_be_core-1.7.0/core/test_models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/test_security.py` & `openimis_be_core-1.7.0/core/test_security.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/test_services.py` & `openimis_be_core-1.7.0/core/test_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import importlib
 import logging
 
 from django.db import connection
 from django.test.client import RequestFactory
 from django.apps import apps
-
+import datetime
 import core
 from core.models import InteractiveUser, Officer, UserRole
 from core.services import (
     create_or_update_interactive_user,
     create_or_update_core_user,
     create_or_update_officer,
     create_or_update_claim_admin,
@@ -277,15 +277,15 @@
         self.assertEquals(officer.other_names, "Other 1 2 3")
         self.assertEquals(officer.audit_user_id, 999)
         self.assertTrue(officer.has_login)
         self.assertTrue(officer.phone_communication)
         self.assertEquals(officer.location_id, 1)
         self.assertEquals(officer.substitution_officer_id, 1)
         self.assertEquals(officer.address, "Multi\nline\naddress")
-        self.assertEquals(officer.works_to, "2025-01-01")
+        self.assertEquals(str(officer.works_to.date()), "2025-01-01")
         self.assertEquals(
             list(
                 OfficerVillage.objects.filter(validity_to__isnull=True, officer=officer)
                 .order_by("location_id")
                 .values_list("location_id", flat=True)
             ),
             [22, 35, 50],
@@ -324,15 +324,15 @@
         self.assertEquals(officer.other_names, "Other 1 2 3")
         self.assertEquals(officer.audit_user_id, 999)
         self.assertTrue(officer.has_login)
         self.assertTrue(officer.phone_communication)
         self.assertEquals(officer.location_id, 1)
         self.assertEquals(officer.substitution_officer_id, 1)
         self.assertEquals(officer.address, "Multi\nline\naddress")
-        self.assertEquals(officer.works_to, "2025-01-01")
+        self.assertEquals(str(officer.works_to.date()), "2025-01-01")
         self.assertEquals(
             list(
                 OfficerVillage.objects.filter(validity_to__isnull=True, officer=officer)
                 .order_by("location_id")
                 .values_list("location_id", flat=True)
             ),
             [22, 35, 50],
@@ -348,15 +348,15 @@
                 other_names="Other updated",
                 dob="1999-01-01",
                 phone="+00000",
                 email="imis@bar.be",
                 location_id=17,
                 village_ids=[22],
                 substitution_officer_id=None,
-                works_to="2025-05-05",
+                works_to=datetime.date(2025,5,5),
                 phone_communication=False,
                 address="updated address",
             ),
             audit_user_id=111,
             connected=True,
         )
         self.assertFalse(created)
@@ -366,15 +366,15 @@
         self.assertEquals(officer2.other_names, "Other updated")
         self.assertEquals(officer2.audit_user_id, 111)
         self.assertTrue(officer2.has_login)
         self.assertFalse(officer2.phone_communication)
         self.assertEquals(officer2.location_id, 17)
         self.assertIsNone(officer2.substitution_officer_id)
         self.assertEquals(officer2.address, "updated address")
-        self.assertEquals(officer2.works_to, "2025-05-05")
+        self.assertEquals(str(officer2.works_to.date()), "2025-05-05")
         self.assertEquals(
             list(
                 OfficerVillage.objects.filter(
                     validity_to__isnull=True, officer=officer2
                 )
                 .order_by("location_id")
                 .values_list("location_id", flat=True)
```

### Comparing `openimis-be-core-1.6.0/core/test_utils.py` & `openimis_be_core-1.7.0/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/tests.py` & `openimis_be_core-1.7.0/core/tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/utils.py` & `openimis_be_core-1.7.0/core/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,25 @@
+import uuid
+import json
+from importlib import import_module
+from typing import Type, Dict, Any
+
+import jsonschema
+
 import core
 import ast
 import graphene
+from django.apps import AppConfig
+from django.http import FileResponse
 from django.db.models import Q
 from django.utils.translation import gettext as _
 import logging
 from django.apps import apps
 from django.core.exceptions import PermissionDenied
-
+from django.core.files.storage import default_storage
 
 logger = logging.getLogger(__file__)
 
 __all__ = [
     "TimeUtils",
     "full_class_name",
     "comparable",
@@ -56,31 +65,30 @@
         return not self.__eq__(other)
 
     cls.__eq__ = __eq__
     cls.__ne__ = __ne__
     return cls
 
 
-def filter_validity(arg="validity", prefix = '', **kwargs):
+def filter_validity(arg="validity", prefix='', **kwargs):
     validity = kwargs.get(arg)
     if validity is None:
-        return (
-            Q(**{f'{prefix}legacy_id__isnull':True}),
+        return [
             Q(**{f'{prefix}validity_to__isnull':True})
-        )
-    return (
+        ]
+    return [
         Q(**{f'{prefix}validity_from__lte':validity}),
         Q(**{f'{prefix}validity_to__isnull':True}) | Q(**{f'{prefix}validity_to__gte':validity})
-    )
+    ]
 
 
 def filter_validity_business_model(arg='dateValidFrom__Gte', arg2='dateValidTo__Lte', **kwargs):
     date_valid_from = kwargs.get(arg)
     date_valid_to = kwargs.get(arg2)
-    #default scenario
+    # default scenario
     if not date_valid_from and not date_valid_to:
         today = core.datetime.datetime.now()
         return __place_the_filters(date_start=today, date_end=None)
 
     # scenario - only date valid to set
     if not date_valid_from and date_valid_to:
         today = core.datetime.datetime.now()
@@ -195,14 +203,15 @@
 
 class ExtendedConnection(graphene.Connection):
     """
     Adds total_count and edge_count to Graphene connections. To use, simply add to the
     Graphene object definition Meta:
     `connection_class = ExtendedConnection`
     """
+
     class Meta:
         abstract = True
 
     total_count = graphene.Int()
     edge_count = graphene.Int()
 
     def resolve_total_count(self, info, **kwargs):
@@ -230,14 +239,15 @@
     return module
 
 
 class ExtendedRelayConnection(graphene.relay.Connection):
     """
     Adds total_count and edge_count to Graphene Relay connections.
     """
+
     class Meta:
         abstract = True
 
     total_count = graphene.Int()
     edge_count = graphene.Int()
 
     def resolve_total_count(self, info, **kwargs):
@@ -258,34 +268,128 @@
 
 def insert_role_right_for_system(system_role, right_id):
     RoleRight = apps.get_model("core", "RoleRight")
     Role = apps.get_model("core", "Role")
     existing_role = Role.objects.filter(is_system=system_role, validity_to__isnull=True).first()
     if not existing_role:
         logger.warning("Migration requested a role_right for system role %s but couldn't find that role", system_role)
-    role_right = RoleRight.objects.filter(role=existing_role, right_id=right_id).first()
-    if not role_right:
-        role_right = RoleRight.objects.create(role=existing_role, right_id=right_id)
+    else:
+        role_right = RoleRight.objects.filter(role=existing_role, right_id=right_id).first()
+        if not role_right:
+            role_right = RoleRight.objects.create(role=existing_role, right_id=right_id)
 
-    return role_right
+        return role_right
 
 
 def remove_role_right_for_system(system_role, right_id):
     RoleRight = apps.get_model("core", "RoleRight")
     Role = apps.get_model("core", "Role")
     existing_role = Role.objects.filter(is_system=system_role, validity_to__isnull=True).first()
     if not existing_role:
-        logger.warning("Migration requested to remove a role_right for system role %s but couldn't find that role", system_role)
+        logger.warning("Migration requested to remove a role_right for system role %s but couldn't find that role",
+                       system_role)
     role_right = RoleRight.objects.filter(role=existing_role, right_id=right_id).first()
     if role_right:
         role_right.delete()
         logger.info("Role right removed for system role %s and right ID %s", system_role, right_id)
     else:
         logger.warning("Role right not found for system role %s and right ID %s", system_role, right_id)
 
 
 def convert_to_python_value(string):
     try:
         value = ast.literal_eval(string)
         return value
     except (SyntaxError, ValueError):
         return string
+
+
+def is_valid_uuid(string):
+    try:
+        uuid_obj = uuid.UUID(str(string))
+        return True
+    except ValueError:
+        return False
+
+
+def validate_json_schema(schema):
+    try:
+        if not isinstance(schema, dict):
+            schema = json.loads(schema)
+        jsonschema.Draft7Validator.check_schema(schema)
+        return []
+    except jsonschema.exceptions.SchemaError as schema_error:
+        return [{"message": _("core.utils.schema_validation.invalid_schema" % {
+            'error': str(schema_error)
+        })}]
+    except ValueError as json_error:
+        return [{"message": _("core.utils.schema_validation.invalid_json" % {
+            'error': str(json_error)
+        })}]
+
+
+class DefaultStorageFileHandler:
+    def __init__(self, file_path):
+        self.file_path = file_path
+
+    def save_file(self, file):
+        self.check_file_path()
+        default_storage.save(self.file_path, file)
+        file.seek(0)
+
+    def remove_file(self):
+        if default_storage.exists(self.file_path):
+            default_storage.delete(self.file_path)
+
+    def get_file_content(self):
+        if not default_storage.exists(self.file_path):
+            raise FileNotFoundError("File does not exist at the specified path.")
+        with default_storage.open(self.file_path, 'rb') as source:
+            return source.read()
+
+    def get_file_response_csv(self, file_name=None):
+        if not default_storage.exists(self.file_path):
+            raise FileNotFoundError("File does not exist at the specified path.")
+        response = FileResponse(default_storage.open(self.file_path, 'rb'))
+        response['Content-Type'] = 'text/csv'
+        response['Content-Disposition'] = f'attachment; filename="{file_name if file_name else "default.csv"}"'
+        return response
+
+    def check_file_path(self):
+        if default_storage.exists(self.file_path):
+            raise FileExistsError("File already exists at the specified path.")
+
+    @staticmethod
+    def list_files(directory):
+        """
+        Get a list of files in the specified directory within default storage.
+        """
+        return default_storage.listdir(directory)
+
+
+class ConfigUtilMixin:
+    @classmethod
+    def _load_config_fields(cls, default_cfg: Dict[str, Any]):
+        """
+        Load all config fields that match current AppConfig class fields, all custom fields have to be loaded separately
+        """
+        for field in default_cfg:
+            if hasattr(cls, field):
+                setattr(cls, field, default_cfg[field])
+
+    @classmethod
+    def _load_config_function(cls, function_name, path):
+        """
+        Load a function specified as module path into config.
+        Example:
+        "core.apps.function" will be loaded as "from core.apps import function" and assigned as "cls.function_name"
+        """
+        try:
+            mod, name = path.rsplit(".", 1)
+            if not mod or not name:
+                raise ImportError("Invalid function path, module and function name are required")
+            module = import_module(mod)
+            function = getattr(module, name)
+            setattr(cls, function_name, function)
+        except ImportError as e:
+            logger.error(f'Failed to configure function "%s" as "%s.%s": %s',
+                         path, cls.__name__, function_name, str(e))
```

### Comparing `openimis-be-core-1.6.0/core/validation/obligatoryFieldValidation.py` & `openimis_be_core-1.7.0/core/validation/obligatoryFieldValidation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/validation/uniqueCodeValidationMixin.py` & `openimis_be_core-1.7.0/core/validation/uniqueCodeValidationMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/views.py` & `openimis_be_core-1.7.0/core/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from rest_framework.decorators import action, api_view
 from rest_framework.exceptions import PermissionDenied
 from rest_framework.response import Response
 from rest_framework.permissions import IsAuthenticated
 from .models import User, ExportableQueryModel
 from .scheduler import scheduler
 from .serializers import UserSerializer
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 class UserViewSet(viewsets.ModelViewSet):
     queryset = User.objects.all()
     serializer_class = UserSerializer
     # If we don't specify the IsAuthenticated, the framework will look for the core.user_view permission and prevent
     # any access from non-admin users
@@ -35,15 +35,15 @@
     if not export:
         raise Http404
     elif export.user != request.user:
         raise PermissionDenied({"message": _("Only user requesting export can fetch request")})
     elif export.is_deleted:
         return Response(data='Export csv file was removed from server.', status=status.HTTP_410_GONE)
 
-    export_file_name = F"export_{export.model}_{strftime(export.create_date, '%d/%m/%Y')}.csv"
+    export_file_name = F"export_{export.model}_{strftime(export.create_date, '%d_%m_%Y')}.csv"
     return StreamingHttpResponse(
         (row for row in export.content.file.readlines()),
         content_type="text/csv",
         headers={'Content-Disposition': F'attachment; filename="{export_file_name}"'},
     )
```

### Comparing `openimis-be-core-1.6.0/core/websocket/abstract_websocket_client.py` & `openimis_be_core-1.7.0/core/websocket/abstract_websocket_client.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/websocket/async_websocket_client.py` & `openimis_be_core-1.7.0/core/websocket/async_websocket_client.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/core/websocket/base_websocket_client.py` & `openimis_be_core-1.7.0/core/websocket/base_websocket_client.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.6.0/openimis_be_core.egg-info/PKG-INFO` & `openimis_be_core-1.7.0/openimis_be_core.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-core
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Core reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -23,7 +23,8 @@
 Requires-Dist: django-db-signals
 Requires-Dist: djangorestframework
 Requires-Dist: cached-property
 Requires-Dist: nepalicalendar
 Requires-Dist: django-simple-history
 Requires-Dist: django-dirtyfields
 Requires-Dist: websocket-client
+Requires-Dist: jsonschema
```

### Comparing `openimis-be-core-1.6.0/openimis_be_core.egg-info/SOURCES.txt` & `openimis_be_core-1.7.0/openimis_be_core.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 core/apps.py
 core/custom_lookups.py
 core/fields.py
 core/forms.py
 core/gql_queries.py
 core/jwt.py
 core/jwt_authentication.py
-core/models.py
 core/report.py
 core/scheduler.py
 core/schema.py
 core/security.py
 core/serializers.py
 core/service_signals.py
 core/signals.py
@@ -78,29 +77,41 @@
 core/migrations/0019_extended_field.py
 core/migrations/0020_add_missing_fields_to_django_scheme.py
 core/migrations/0021_set_managed_to_true.py
 core/migrations/0022_auto_20230516_1742.py
 core/migrations/0023_alter_jsonext_column_in_tblOfficer.py
 core/migrations/0024_alter_usergroup_options.py
 core/migrations/0025_mutationlog_json_ext.py
+core/migrations/0026_mutationlog_autogenerated_code.py
+core/migrations/0027_alter_interactiveuser_last_login_and_more.py
+core/migrations/0028_alter_moduleconfiguration_module.py
 core/migrations/__init__.py
+core/models/__init__.py
+core/models/base.py
+core/models/base_mutation.py
+core/models/history_model.py
+core/models/openimis_graphql_test_case.py
+core/models/user.py
+core/models/user_mutation.py
+core/models/versioned_model.py
 core/reports/__init__.py
 core/reports/registers_status.py
 core/reports/user_activity.py
 core/services/__init__.py
 core/services/base.py
 core/services/roleServices.py
 core/services/userServices.py
 core/services/utils/__init__.py
 core/services/utils/serviceUtils.py
 core/templates/password_reset.txt
 core/validation/__init__.py
 core/validation/base.py
 core/validation/objectExistsValidationMixin.py
 core/validation/obligatoryFieldValidation.py
+core/validation/stringFieldValidationMixin.py
 core/validation/uniqueCodeValidationMixin.py
 core/websocket/__init__.py
 core/websocket/abstract_websocket_client.py
 core/websocket/async_websocket_client.py
 core/websocket/base_websocket_client.py
 openimis_be_core.egg-info/PKG-INFO
 openimis_be_core.egg-info/SOURCES.txt
```

### Comparing `openimis-be-core-1.6.0/setup.py` & `openimis_be_core-1.7.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-core',
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Core reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
@@ -23,15 +23,16 @@
         'django',
         'django-db-signals',
         'djangorestframework',
         'cached-property',
         'nepalicalendar',
         'django-simple-history',
         'django-dirtyfields',
-        'websocket-client'
+        'websocket-client',
+        'jsonschema',
     ],
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
         'Intended Audience :: Developers',
```

