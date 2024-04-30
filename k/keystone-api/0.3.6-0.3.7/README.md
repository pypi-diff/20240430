# Comparing `tmp/keystone_api-0.3.6.tar.gz` & `tmp/keystone_api-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keystone_api-0.3.6.tar", max compression
+gzip compressed data, was "keystone_api-0.3.7.tar", max compression
```

## Comparing `keystone_api-0.3.6.tar` & `keystone_api-0.3.7.tar`

### file list

```diff
@@ -1,130 +1,134 @@
--rw-r--r--   0        0        0    13578 2024-04-23 17:27:02.679097 keystone_api-0.3.6/README.md
--rw-r--r--   0        0        0      428 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/admin_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/admin_utils/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/__init__.py
--rw-r--r--   0        0        0     2619 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/clean.py
--rw-r--r--   0        0        0     2820 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py
--rw-r--r--   0        0        0      471 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/keystone_autocomplete
--rw-r--r--   0        0        0     3618 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/quickstart.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/__init__.py
--rw-r--r--   0        0        0     4543 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/admin.py
--rw-r--r--   0        0        0     2173 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/managers.py
--rw-r--r--   0        0        0     3420 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/migrations/0001_initial.py
--rw-r--r--   0        0        0     1298 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/migrations/0002_initial.py
--rw-r--r--   0        0        0     1063 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/migrations/__init__.py
--rw-r--r--   0        0        0     5191 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/models.py
--rw-r--r--   0        0        0     3347 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/permissions.py
--rw-r--r--   0        0        0     1917 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/serializers.py
--rw-r--r--   0        0        0     4324 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/tasks.py
--rw-r--r--   0        0        0      516 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/urls.py
--rw-r--r--   0        0        0     3246 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/views.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/authentication/__init__.py
--rw-r--r--   0        0        0      572 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/authentication/tasks.py
--rw-r--r--   0        0        0      444 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/authentication/urls.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/health/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/health/tests/__init__.py
--rw-r--r--   0        0        0     3199 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/health/tests/test_views.py
--rw-r--r--   0        0        0      244 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/health/urls.py
--rw-r--r--   0        0        0     2066 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/health/views.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/__init__.py
--rw-r--r--   0        0        0     1101 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/handlers.py
--rw-r--r--   0        0        0     1828 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/middleware.py
--rw-r--r--   0        0        0     1959 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/migrations/0001_initial.py
--rw-r--r--   0        0        0      644 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/migrations/__init__.py
--rw-r--r--   0        0        0     1400 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/models.py
--rw-r--r--   0        0        0      868 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/serializers.py
--rw-r--r--   0        0        0      709 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tasks.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tests/handlers/__init__.py
--rw-r--r--   0        0        0     2560 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tests/handlers/test_DBHandler.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tests/middleware/__init__.py
--rw-r--r--   0        0        0     2390 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tests/tasks/__init__.py
--rw-r--r--   0        0        0     1791 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py
--rw-r--r--   0        0        0      278 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/urls.py
--rw-r--r--   0        0        0      949 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/views.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/openapi/__init__.py
--rw-r--r--   0        0        0      326 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/openapi/urls.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/__init__.py
--rw-r--r--   0        0        0     1705 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/admin.py
--rw-r--r--   0        0        0     1261 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/managers.py
--rw-r--r--   0        0        0     1677 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/migrations/0001_initial.py
--rw-r--r--   0        0        0      437 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/migrations/0002_grant_grant_number.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/migrations/__init__.py
--rw-r--r--   0        0        0     1776 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/models.py
--rw-r--r--   0        0        0     2862 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/permissions.py
--rw-r--r--   0        0        0      928 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/serializers.py
--rw-r--r--   0        0        0      338 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/urls.py
--rw-r--r--   0        0        0     1554 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/views.py
--rw-r--r--   0        0        0      141 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/scheduler/__init__.py
--rw-r--r--   0        0        0     1029 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/scheduler/admin.py
--rw-r--r--   0        0        0      654 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/scheduler/apps.py
--rw-r--r--   0        0        0     1344 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/scheduler/celery.py
--rw-r--r--   0        0        0      875 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/scheduler/checks.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/__init__.py
--rw-r--r--   0        0        0     1307 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/admin.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/management/commands/__init__.py
--rw-r--r--   0        0        0     1056 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/management/commands/ldap_update.py
--rw-r--r--   0        0        0     3134 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/managers.py
--rw-r--r--   0        0        0     3018 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/migrations/0001_initial.py
--rw-r--r--   0        0        0      405 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/migrations/0002_user_is_ldap_user.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/migrations/__init__.py
--rw-r--r--   0        0        0     2370 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/models.py
--rw-r--r--   0        0        0      913 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/permissions.py
--rw-r--r--   0        0        0      887 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/serializers.py
--rw-r--r--   0        0        0     2095 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tasks.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/test_managers/__init__.py
--rw-r--r--   0        0        0     1374 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py
--rw-r--r--   0        0        0     2399 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/test_managers/test_UserManager.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/test_models/__init__.py
--rw-r--r--   0        0        0     3210 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py
--rw-r--r--   0        0        0      471 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/test_models/test_User.py
--rw-r--r--   0        0        0      748 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/utils.py
--rw-r--r--   0        0        0      329 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/urls.py
--rw-r--r--   0        0        0     1329 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/views.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/main/__init__.py
--rw-r--r--   0        0        0      169 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/main/asgi.py
--rw-r--r--   0        0        0     7971 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/main/settings.py
--rw-r--r--   0        0        0     1058 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/main/urls.py
--rw-r--r--   0        0        0      168 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/main/wsgi.py
--rwxr-xr-x   0        0        0      556 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/manage.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/plugins/__init__.py
--rw-r--r--   0        0        0     4728 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/plugins/slurm.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/__init__.py
--rw-r--r--   0        0        0     2923 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_allocations.py
--rw-r--r--   0        0        0     4229 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_allocations_pk.py
--rw-r--r--   0        0        0     2929 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_clusters.py
--rw-r--r--   0        0        0     3104 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_clusters_pk.py
--rw-r--r--   0        0        0     5631 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_requests.py
--rw-r--r--   0        0        0     5351 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_requests_pk.py
--rw-r--r--   0        0        0     2898 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_reviews.py
--rw-r--r--   0        0        0     4202 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_reviews_pk.py
--rw-r--r--   0        0        0     3921 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/fixtures/multi_research_group.yaml
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/health/__init__.py
--rw-r--r--   0        0        0     3073 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/health/test.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/logging/__init__.py
--rw-r--r--   0        0        0     2871 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/logging/test_apps.py
--rw-r--r--   0        0        0     2879 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/logging/test_requests.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/openapi/__init__.py
--rw-r--r--   0        0        0     2867 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/openapi/test_json.py
--rw-r--r--   0        0        0     2867 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/openapi/test_yaml.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/research/__init__.py
--rw-r--r--   0        0        0     5611 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/research/test_grants.py
--rw-r--r--   0        0        0     4524 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/research/test_grants_pk.py
--rw-r--r--   0        0        0     5782 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/research/test_publications.py
--rw-r--r--   0        0        0     4438 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/research/test_publications_pk.py
--rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/users/__init__.py
--rw-r--r--   0        0        0     2981 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/users/test_researchgroups.py
--rw-r--r--   0        0        0     4244 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/users/test_researchgroups_pk.py
--rw-r--r--   0        0        0     2964 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/users/test_users.py
--rw-r--r--   0        0        0     4471 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/users/test_users_pk.py
--rw-r--r--   0        0        0     2022 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/utils.py
--rw-r--r--   0        0        0      957 2024-04-23 17:27:23.310962 keystone_api-0.3.6/pyproject.toml
--rw-r--r--   0        0        0    14773 1970-01-01 00:00:00.000000 keystone_api-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    13578 2024-04-30 20:23:18.059406 keystone_api-0.3.7/README.md
+-rw-r--r--   0        0        0      428 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/admin_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/admin_utils/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/__init__.py
+-rw-r--r--   0        0        0     2619 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/clean.py
+-rw-r--r--   0        0        0     2820 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py
+-rw-r--r--   0        0        0      471 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/keystone_autocomplete
+-rw-r--r--   0        0        0     3618 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/quickstart.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/__init__.py
+-rw-r--r--   0        0        0     4543 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/admin.py
+-rw-r--r--   0        0        0     2173 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/managers.py
+-rw-r--r--   0        0        0     3420 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1298 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/migrations/0002_initial.py
+-rw-r--r--   0        0        0     1063 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/migrations/__init__.py
+-rw-r--r--   0        0        0     5191 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/models.py
+-rw-r--r--   0        0        0     3347 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/permissions.py
+-rw-r--r--   0        0        0     1917 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/serializers.py
+-rw-r--r--   0        0        0     4324 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/tasks.py
+-rw-r--r--   0        0        0      516 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/urls.py
+-rw-r--r--   0        0        0     3246 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/allocations/views.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/authentication/__init__.py
+-rw-r--r--   0        0        0      572 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/authentication/tasks.py
+-rw-r--r--   0        0        0      444 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/authentication/urls.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/health/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/health/tests/__init__.py
+-rw-r--r--   0        0        0     3199 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/health/tests/test_views.py
+-rw-r--r--   0        0        0      244 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/health/urls.py
+-rw-r--r--   0        0        0     2066 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/health/views.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/__init__.py
+-rw-r--r--   0        0        0     2496 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/admin.py
+-rw-r--r--   0        0        0     1101 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/handlers.py
+-rw-r--r--   0        0        0     1828 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/middleware.py
+-rw-r--r--   0        0        0     1959 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/migrations/0001_initial.py
+-rw-r--r--   0        0        0      644 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py
+-rw-r--r--   0        0        0      638 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/migrations/0003_taskresult.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/migrations/__init__.py
+-rw-r--r--   0        0        0     1645 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/models.py
+-rw-r--r--   0        0        0     1112 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/serializers.py
+-rw-r--r--   0        0        0      709 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tasks.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tests/handlers/__init__.py
+-rw-r--r--   0        0        0     2560 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tests/handlers/test_DBHandler.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tests/middleware/__init__.py
+-rw-r--r--   0        0        0     2390 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tests/tasks/__init__.py
+-rw-r--r--   0        0        0     1791 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py
+-rw-r--r--   0        0        0      322 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/urls.py
+-rw-r--r--   0        0        0     1284 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/logging/views.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/openapi/__init__.py
+-rw-r--r--   0        0        0      326 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/openapi/urls.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/__init__.py
+-rw-r--r--   0        0        0     1705 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/admin.py
+-rw-r--r--   0        0        0     1261 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/managers.py
+-rw-r--r--   0        0        0     1677 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/migrations/0001_initial.py
+-rw-r--r--   0        0        0      437 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/migrations/0002_grant_grant_number.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/migrations/__init__.py
+-rw-r--r--   0        0        0     1776 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/models.py
+-rw-r--r--   0        0        0     2862 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/permissions.py
+-rw-r--r--   0        0        0      928 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/serializers.py
+-rw-r--r--   0        0        0      338 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/urls.py
+-rw-r--r--   0        0        0     1554 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/research_products/views.py
+-rw-r--r--   0        0        0      141 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/scheduler/__init__.py
+-rw-r--r--   0        0        0      834 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/scheduler/admin.py
+-rw-r--r--   0        0        0      654 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/scheduler/apps.py
+-rw-r--r--   0        0        0     1344 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/scheduler/celery.py
+-rw-r--r--   0        0        0      875 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/scheduler/checks.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/__init__.py
+-rw-r--r--   0        0        0     1307 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/admin.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/management/commands/__init__.py
+-rw-r--r--   0        0        0     1056 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/management/commands/ldap_update.py
+-rw-r--r--   0        0        0     3134 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/managers.py
+-rw-r--r--   0        0        0     3018 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/migrations/0001_initial.py
+-rw-r--r--   0        0        0      405 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/migrations/0002_user_is_ldap_user.py
+-rw-r--r--   0        0        0      402 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/migrations/0003_alter_researchgroup_name.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/migrations/__init__.py
+-rw-r--r--   0        0        0     2383 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/models.py
+-rw-r--r--   0        0        0      913 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/permissions.py
+-rw-r--r--   0        0        0      887 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/serializers.py
+-rw-r--r--   0        0        0     2095 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/tasks.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.059406 keystone_api-0.3.7/keystone_api/apps/users/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/tests/test_managers/__init__.py
+-rw-r--r--   0        0        0     1374 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py
+-rw-r--r--   0        0        0     2399 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/tests/test_managers/test_UserManager.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/tests/test_models/__init__.py
+-rw-r--r--   0        0        0     3210 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py
+-rw-r--r--   0        0        0      471 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/tests/test_models/test_User.py
+-rw-r--r--   0        0        0      748 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/tests/utils.py
+-rw-r--r--   0        0        0      329 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/urls.py
+-rw-r--r--   0        0        0     1329 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/apps/users/views.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/main/__init__.py
+-rw-r--r--   0        0        0      169 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/main/asgi.py
+-rw-r--r--   0        0        0     8125 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/main/settings.py
+-rw-r--r--   0        0        0     1058 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/main/urls.py
+-rw-r--r--   0        0        0      168 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/main/wsgi.py
+-rwxr-xr-x   0        0        0      556 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/manage.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/plugins/__init__.py
+-rw-r--r--   0        0        0     4728 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/plugins/slurm.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/__init__.py
+-rw-r--r--   0        0        0     2923 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_allocations.py
+-rw-r--r--   0        0        0     4229 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_allocations_pk.py
+-rw-r--r--   0        0        0     2929 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_clusters.py
+-rw-r--r--   0        0        0     3104 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_clusters_pk.py
+-rw-r--r--   0        0        0     5631 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_requests.py
+-rw-r--r--   0        0        0     5351 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_requests_pk.py
+-rw-r--r--   0        0        0     2898 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_reviews.py
+-rw-r--r--   0        0        0     4202 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/allocations/test_reviews_pk.py
+-rw-r--r--   0        0        0     3921 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/fixtures/multi_research_group.yaml
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/health/__init__.py
+-rw-r--r--   0        0        0     3073 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/health/test.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/logging/__init__.py
+-rw-r--r--   0        0        0     2871 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/logging/test_apps.py
+-rw-r--r--   0        0        0     2879 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/logging/test_requests.py
+-rw-r--r--   0        0        0     2873 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/logging/test_tasks.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/openapi/__init__.py
+-rw-r--r--   0        0        0     2867 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/openapi/test_json.py
+-rw-r--r--   0        0        0     2867 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/openapi/test_yaml.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/research/__init__.py
+-rw-r--r--   0        0        0     5611 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/research/test_grants.py
+-rw-r--r--   0        0        0     4524 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/research/test_grants_pk.py
+-rw-r--r--   0        0        0     5782 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/research/test_publications.py
+-rw-r--r--   0        0        0     4438 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/research/test_publications_pk.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/users/__init__.py
+-rw-r--r--   0        0        0     2981 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/users/test_researchgroups.py
+-rw-r--r--   0        0        0     4244 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/users/test_researchgroups_pk.py
+-rw-r--r--   0        0        0     2964 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/users/test_users.py
+-rw-r--r--   0        0        0     4471 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/users/test_users_pk.py
+-rw-r--r--   0        0        0     2022 2024-04-30 20:23:18.063406 keystone_api-0.3.7/keystone_api/tests/utils.py
+-rw-r--r--   0        0        0      957 2024-04-30 20:23:38.111181 keystone_api-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0    14773 1970-01-01 00:00:00.000000 keystone_api-0.3.7/PKG-INFO
```

### Comparing `keystone_api-0.3.6/README.md` & `keystone_api-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/clean.py` & `keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/clean.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py` & `keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/quickstart.py` & `keystone_api-0.3.7/keystone_api/apps/admin_utils/management/commands/quickstart.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/allocations/admin.py` & `keystone_api-0.3.7/keystone_api/apps/allocations/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/allocations/managers.py` & `keystone_api-0.3.7/keystone_api/apps/allocations/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/allocations/migrations/0001_initial.py` & `keystone_api-0.3.7/keystone_api/apps/allocations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/allocations/migrations/0002_initial.py` & `keystone_api-0.3.7/keystone_api/apps/allocations/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py` & `keystone_api-0.3.7/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/allocations/models.py` & `keystone_api-0.3.7/keystone_api/apps/allocations/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/allocations/permissions.py` & `keystone_api-0.3.7/keystone_api/apps/allocations/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/allocations/serializers.py` & `keystone_api-0.3.7/keystone_api/apps/allocations/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/allocations/tasks.py` & `keystone_api-0.3.7/keystone_api/apps/allocations/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/allocations/urls.py` & `keystone_api-0.3.7/keystone_api/apps/allocations/urls.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/allocations/views.py` & `keystone_api-0.3.7/keystone_api/apps/allocations/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/authentication/tasks.py` & `keystone_api-0.3.7/keystone_api/apps/authentication/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/health/tests/test_views.py` & `keystone_api-0.3.7/keystone_api/apps/health/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/health/views.py` & `keystone_api-0.3.7/keystone_api/apps/health/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/logging/handlers.py` & `keystone_api-0.3.7/keystone_api/apps/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/logging/middleware.py` & `keystone_api-0.3.7/keystone_api/apps/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/logging/migrations/0001_initial.py` & `keystone_api-0.3.7/keystone_api/apps/logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py` & `keystone_api-0.3.7/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/logging/models.py` & `keystone_api-0.3.7/keystone_api/apps/research_products/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,38 +3,53 @@
 Model objects are used to define the expected schema for individual database
 tables and provide an object-oriented interface for executing database logic.
 Each model reflects a different database and defines low-level defaults for how
 the associated table/fields/records are presented by parent interfaces.
 """
 
 from django.db import models
+from django.template.defaultfilters import truncatechars
 
-from apps.users.models import User
+from apps.users.models import ResearchGroup
+from .managers import *
 
-__all__ = ['AppLog', 'RequestLog']
+__all__ = ['Grant', 'Publication']
 
 
-class AppLog(models.Model):
-    """An application log entry"""
+class Grant(models.Model):
+    """Metadata for a funding grant"""
 
-    name = models.CharField(max_length=100)
-    level = models.CharField(max_length=10)
-    pathname = models.CharField(max_length=260)
-    lineno = models.IntegerField()
-    message = models.TextField()
-    func = models.CharField(max_length=80, blank=True, null=True)
-    sinfo = models.TextField(blank=True, null=True)
-    time = models.DateTimeField(auto_now_add=True)
+    title = models.CharField(max_length=250)
+    agency = models.CharField(max_length=100)
+    amount = models.DecimalField(decimal_places=2, max_digits=14)
+    grant_number = models.CharField(max_length=250)
+    fiscal_year = models.IntegerField()
+    start_date = models.DateField()
+    end_date = models.DateField()
 
+    group = models.ForeignKey(ResearchGroup, on_delete=models.CASCADE)
 
-class RequestLog(models.Model):
-    """Log entry for an incoming HTTP request"""
+    objects = GrantManager()
 
-    method = models.CharField(max_length=10)
-    endpoint = models.CharField(max_length=100)
-    response_code = models.PositiveSmallIntegerField()
-    body_request = models.TextField()
-    body_response = models.TextField()
-    remote_address = models.CharField(max_length=40, null=True)
-    time = models.DateTimeField(auto_now_add=True)
+    def __str__(self) -> str:
+        """Return the grant title truncated to 50 characters"""
 
-    user = models.ForeignKey(User, on_delete=models.SET_NULL, null=True)
+        return truncatechars(self.title, 100)
+
+
+class Publication(models.Model):
+    """Metadata for an academic publication"""
+
+    title = models.CharField(max_length=250)
+    abstract = models.TextField()
+    date = models.DateField('Publication Date')
+    journal = models.CharField(max_length=100)
+    doi = models.CharField(max_length=50, unique=True, null=True, blank=True)
+
+    group = models.ForeignKey(ResearchGroup, on_delete=models.CASCADE)
+
+    objects = PublicationManager()
+
+    def __str__(self) -> str:
+        """Return the publication title truncated to 50 characters"""
+
+        return truncatechars(self.title, 100)
```

### Comparing `keystone_api-0.3.6/keystone_api/apps/logging/serializers.py` & `keystone_api-0.3.7/keystone_api/apps/research_products/serializers.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 creation.
 """
 
 from rest_framework import serializers
 
 from .models import *
 
-__all__ = ['AppLogSerializer', 'RequestLogSerializer']
+__all__ = ['GrantSerializer', 'PublicationSerializer']
 
 
-class AppLogSerializer(serializers.ModelSerializer):
-    """Object serializer for the `AppLog` class"""
+class PublicationSerializer(serializers.ModelSerializer):
+    """Object serializer for the `Publication` class"""
 
     class Meta:
         """Serializer settings"""
 
-        model = AppLog
+        model = Publication
         fields = '__all__'
+        read_only = ['group']
 
 
-class RequestLogSerializer(serializers.ModelSerializer):
-    """Object serializer for the `RequestLog` class"""
+class GrantSerializer(serializers.ModelSerializer):
+    """Object serializer for the `Grant` class"""
 
     class Meta:
         """Serializer settings"""
 
-        model = RequestLog
+        model = Grant
         fields = '__all__'
+        read_only = ['group']
```

### Comparing `keystone_api-0.3.6/keystone_api/apps/logging/tasks.py` & `keystone_api-0.3.7/keystone_api/apps/logging/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/logging/tests/handlers/test_DBHandler.py` & `keystone_api-0.3.7/keystone_api/apps/logging/tests/handlers/test_DBHandler.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py` & `keystone_api-0.3.7/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py` & `keystone_api-0.3.7/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/logging/views.py` & `keystone_api-0.3.7/keystone_api/apps/logging/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Application logic for rendering HTML templates and handling HTTP requests.
 
 View objects handle the processing of incoming HTTP requests and return the
 appropriately rendered HTML template or other HTTP response.
 """
 
-from rest_framework import viewsets, permissions
+from rest_framework import permissions, viewsets
 
 from .models import *
 from .serializers import *
 
-__all__ = ['AppLogViewSet', 'RequestLogViewSet']
+__all__ = ['AppLogViewSet', 'RequestLogViewSet', 'TaskResultViewSet']
 
 
 class AppLogViewSet(viewsets.ReadOnlyModelViewSet):
     """Returns application log data"""
 
     queryset = AppLog.objects.all()
     serializer_class = AppLogSerializer
@@ -24,7 +24,16 @@
 class RequestLogViewSet(viewsets.ReadOnlyModelViewSet):
     """Returns HTTP request log data"""
 
     queryset = RequestLog.objects.all()
     serializer_class = RequestLogSerializer
     filterset_fields = '__all__'
     permission_classes = [permissions.IsAuthenticated, permissions.IsAdminUser]
+
+
+class TaskResultViewSet(viewsets.ReadOnlyModelViewSet):
+    """Returns results from scheduled background tasks"""
+
+    queryset = TaskResult.objects.all()
+    serializer_class = TaskResultSerializer
+    filterset_fields = '__all__'
+    permission_classes = [permissions.IsAuthenticated, permissions.IsAdminUser]
```

### Comparing `keystone_api-0.3.6/keystone_api/apps/research_products/admin.py` & `keystone_api-0.3.7/keystone_api/apps/research_products/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/research_products/managers.py` & `keystone_api-0.3.7/keystone_api/apps/research_products/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/research_products/migrations/0001_initial.py` & `keystone_api-0.3.7/keystone_api/apps/research_products/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/research_products/permissions.py` & `keystone_api-0.3.7/keystone_api/apps/research_products/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/research_products/views.py` & `keystone_api-0.3.7/keystone_api/apps/research_products/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/scheduler/admin.py` & `keystone_api-0.3.7/keystone_api/apps/scheduler/admin.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,20 +8,16 @@
 
 settings.JAZZMIN_SETTINGS['icons'].update({
     'django_celery_beat.ClockedSchedule': 'fa fa-clock',
     'django_celery_beat.CrontabSchedule': 'fa fa-asterisk',
     'django_celery_beat.IntervalSchedule': 'fa fa-redo',
     'django_celery_beat.SolarSchedule': 'fa fa-sun',
     'django_celery_beat.PeriodicTask': 'fa fa-check',
-    'django_celery_results.TaskResult': 'fa fa-tasks',
-    'django_celery_results.GroupResult': 'fa fa-list-alt',
 })
 
 settings.JAZZMIN_SETTINGS['order_with_respect_to'].extend([
     'django_celery_beat.PeriodicTask',
     'django_celery_beat.IntervalSchedule',
     'django_celery_beat.ClockedSchedule',
     'django_celery_beat.CrontabSchedule',
     'django_celery_beat.SolarSchedule',
-    'django_celery_results.TaskResult',
-    'django_celery_results.GroupResult',
 ])
```

### Comparing `keystone_api-0.3.6/keystone_api/apps/scheduler/apps.py` & `keystone_api-0.3.7/keystone_api/apps/scheduler/apps.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/scheduler/celery.py` & `keystone_api-0.3.7/keystone_api/apps/scheduler/celery.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/scheduler/checks.py` & `keystone_api-0.3.7/keystone_api/apps/scheduler/checks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/users/admin.py` & `keystone_api-0.3.7/keystone_api/apps/users/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/users/management/commands/ldap_update.py` & `keystone_api-0.3.7/keystone_api/apps/users/management/commands/ldap_update.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/users/managers.py` & `keystone_api-0.3.7/keystone_api/apps/users/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/users/migrations/0001_initial.py` & `keystone_api-0.3.7/keystone_api/apps/users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/users/models.py` & `keystone_api-0.3.7/keystone_api/apps/users/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     EMAIL_FIELD = "email"
     REQUIRED_FIELDS = ['email', 'first_name', 'last_name']
 
 
 class ResearchGroup(models.Model):
     """A user research group tied to a slurm account"""
 
-    name = models.CharField(max_length=255)
+    name = models.CharField(max_length=255, unique=True)
     pi = models.ForeignKey(User, on_delete=models.CASCADE, related_name='research_group_pi')
     admins = models.ManyToManyField(User, related_name='research_group_admins', blank=True)
     members = models.ManyToManyField(User, related_name='research_group_unprivileged', blank=True)
 
     objects = ResearchGroupManager()
 
     def get_all_members(self) -> tuple[User]:
```

### Comparing `keystone_api-0.3.6/keystone_api/apps/users/permissions.py` & `keystone_api-0.3.7/keystone_api/apps/users/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/users/serializers.py` & `keystone_api-0.3.7/keystone_api/apps/users/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/users/tasks.py` & `keystone_api-0.3.7/keystone_api/apps/users/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py` & `keystone_api-0.3.7/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/users/tests/test_managers/test_UserManager.py` & `keystone_api-0.3.7/keystone_api/apps/users/tests/test_managers/test_UserManager.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py` & `keystone_api-0.3.7/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/users/tests/utils.py` & `keystone_api-0.3.7/keystone_api/apps/users/tests/utils.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/apps/users/views.py` & `keystone_api-0.3.7/keystone_api/apps/users/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/main/settings.py` & `keystone_api-0.3.7/keystone_api/main/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,9 +258,14 @@
         }
     },
     "loggers": {
         "": {
             "level": env.str('CONFIG_LOG_LEVEL', 'WARNING'),
             "handlers": ["db"],
         },
+        "apps": {
+            "level": env.str('CONFIG_LOG_LEVEL', 'WARNING'),
+            "handlers": ["db"],
+            "propagate": False,
+        },
     }
 }
```

### Comparing `keystone_api-0.3.6/keystone_api/main/urls.py` & `keystone_api-0.3.7/keystone_api/main/urls.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/manage.py` & `keystone_api-0.3.7/keystone_api/manage.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/plugins/slurm.py` & `keystone_api-0.3.7/keystone_api/plugins/slurm.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/allocations/test_allocations.py` & `keystone_api-0.3.7/keystone_api/tests/allocations/test_allocations.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/allocations/test_allocations_pk.py` & `keystone_api-0.3.7/keystone_api/tests/allocations/test_allocations_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/allocations/test_clusters.py` & `keystone_api-0.3.7/keystone_api/tests/allocations/test_clusters.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/allocations/test_clusters_pk.py` & `keystone_api-0.3.7/keystone_api/tests/allocations/test_clusters_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/allocations/test_requests.py` & `keystone_api-0.3.7/keystone_api/tests/allocations/test_requests.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/allocations/test_requests_pk.py` & `keystone_api-0.3.7/keystone_api/tests/allocations/test_requests_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/allocations/test_reviews.py` & `keystone_api-0.3.7/keystone_api/tests/allocations/test_reviews.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/allocations/test_reviews_pk.py` & `keystone_api-0.3.7/keystone_api/tests/allocations/test_reviews_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/fixtures/multi_research_group.yaml` & `keystone_api-0.3.7/keystone_api/tests/fixtures/multi_research_group.yaml`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/health/test.py` & `keystone_api-0.3.7/keystone_api/tests/health/test.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/logging/test_apps.py` & `keystone_api-0.3.7/keystone_api/tests/logging/test_apps.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/logging/test_requests.py` & `keystone_api-0.3.7/keystone_api/tests/logging/test_requests.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/openapi/test_json.py` & `keystone_api-0.3.7/keystone_api/tests/openapi/test_json.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/openapi/test_yaml.py` & `keystone_api-0.3.7/keystone_api/tests/openapi/test_yaml.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/research/test_grants.py` & `keystone_api-0.3.7/keystone_api/tests/research/test_grants.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/research/test_grants_pk.py` & `keystone_api-0.3.7/keystone_api/tests/research/test_grants_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/research/test_publications.py` & `keystone_api-0.3.7/keystone_api/tests/research/test_publications.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/research/test_publications_pk.py` & `keystone_api-0.3.7/keystone_api/tests/research/test_publications_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/users/test_researchgroups.py` & `keystone_api-0.3.7/keystone_api/tests/users/test_researchgroups.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/users/test_researchgroups_pk.py` & `keystone_api-0.3.7/keystone_api/tests/users/test_researchgroups_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/users/test_users.py` & `keystone_api-0.3.7/keystone_api/tests/users/test_users.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/users/test_users_pk.py` & `keystone_api-0.3.7/keystone_api/tests/users/test_users_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/keystone_api/tests/utils.py` & `keystone_api-0.3.7/keystone_api/tests/utils.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.6/pyproject.toml` & `keystone_api-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "keystone-api"
-version = "0.3.6"
+version = "0.3.7"
 readme = "README.md"
 description = "A REST API for managing user resource allocations on HPC systems."
 authors = ["Pitt Center for Research Computing"]
 keywords = ["Pitt", "CRC", "HPC", "django"]
 
 [tool.poetry.scripts]
 keystone-api = "keystone_api.manage:main"
```

### Comparing `keystone_api-0.3.6/PKG-INFO` & `keystone_api-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystone-api
-Version: 0.3.6
+Version: 0.3.7
 Summary: A REST API for managing user resource allocations on HPC systems.
 Keywords: Pitt,CRC,HPC,django
 Author: Pitt Center for Research Computing
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

