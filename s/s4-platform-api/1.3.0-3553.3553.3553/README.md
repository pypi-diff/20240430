# Comparing `tmp/s4_platform_api-1.3.0.tar.gz` & `tmp/s4_platform_api-3553.3553.3553.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s4_platform_api-1.3.0.tar", max compression
+gzip compressed data, was "s4_platform_api-3553.3553.3553.tar", max compression
```

## Comparing `s4_platform_api-1.3.0.tar` & `s4_platform_api-3553.3553.3553.tar`

### file list

```diff
@@ -1,71 +1,73 @@
--rw-r--r--   0        0        0     1076 2024-04-02 22:19:02.696388 s4_platform_api-1.3.0/LICENSE
--rw-r--r--   0        0        0       76 2024-04-02 22:19:02.696388 s4_platform_api-1.3.0/README.md
--rw-r--r--   0        0        0      760 2024-04-02 22:19:15.080399 s4_platform_api-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       20 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/.env
--rw-r--r--   0        0        0        0 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/__init__.py
--rw-r--r--   0        0        0    14537 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/api.py
--rw-r--r--   0        0        0     1530 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/authentication_utils.py
--rw-r--r--   0        0        0     3829 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/changeset/changeset.py
--rw-r--r--   0        0        0     1437 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/changeset/changeset_config.py
--rw-r--r--   0        0        0     1019 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/changeset/deploy_changeset.py
--rw-r--r--   0        0        0     2256 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/claim/claim.py
--rw-r--r--   0        0        0     6752 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/connection.py
--rw-r--r--   0        0        0     1444 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/constants.py
--rw-r--r--   0        0        0     2233 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/deployment/deployment.py
--rw-r--r--   0        0        0     2174 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/entity/ad_hoc_entity.py
--rw-r--r--   0        0        0     8301 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/entity/entity.py
--rw-r--r--   0        0        0     1015 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/entity/field_value.py
--rw-r--r--   0        0        0     1196 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/entity_location/entity_location.py
--rw-r--r--   0        0        0     7065 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/entity_type/entity_type.py
--rw-r--r--   0        0        0     2424 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/environment/environment.py
--rw-r--r--   0        0        0      584 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/environment/environment_configuration.py
--rw-r--r--   0        0        0     2193 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/environment/migration_plan.py
--rw-r--r--   0        0        0      246 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/faas/custom_errors.py
--rw-r--r--   0        0        0     2749 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/faas/faas_function.py
--rw-r--r--   0        0        0     5635 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/faas/faas_utils.py
--rw-r--r--   0        0        0     4437 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/file/file_reference.py
--rw-r--r--   0        0        0     1184 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/function/function.py
--rw-r--r--   0        0        0      248 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/internal/base_model.py
--rw-r--r--   0        0        0     1221 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/internal/base_schema.py
--rw-r--r--   0        0        0      637 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/internal/camel_case_schema.py
--rw-r--r--   0        0        0     2717 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/internal/fields_mixin.py
--rw-r--r--   0        0        0     2153 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/internal/lazy_property.py
--rw-r--r--   0        0        0     2030 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/internal/lazy_property_list.py
--rw-r--r--   0        0        0       80 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/internal/sort_direction.py
--rw-r--r--   0        0        0        0 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/link_config/__init__.py
--rw-r--r--   0        0        0      791 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/link_config/link_config.py
--rw-r--r--   0        0        0      564 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/link_config/new_workbook_link.py
--rw-r--r--   0        0        0      674 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/page_config/page_config.py
--rw-r--r--   0        0        0      801 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/page_config/page_container.py
--rw-r--r--   0        0        0      618 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/page_config/page_container_page_config.py
--rw-r--r--   0        0        0     3229 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/ProspectiveTaskSummary.py
--rw-r--r--   0        0        0      728 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/function_list.py
--rw-r--r--   0        0        0      910 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/function_status.py
--rw-r--r--   0        0        0     1287 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/io_group.py
--rw-r--r--   0        0        0     2162 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/prospective_entity.py
--rw-r--r--   0        0        0     1024 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/prospective_field_value.py
--rw-r--r--   0        0        0    14272 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/prospective_task.py
--rw-r--r--   0        0        0     3260 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/search.py
--rw-r--r--   0        0        0      370 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/copy_forward_config.py
--rw-r--r--   0        0        0     2471 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/field_config.py
--rw-r--r--   0        0        0     1886 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/field_type.py
--rw-r--r--   0        0        0      749 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/field_validation.py
--rw-r--r--   0        0        0      639 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/from_pool_config.py
--rw-r--r--   0        0        0     1914 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/group_config.py
--rw-r--r--   0        0        0     1343 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/io_group_config.py
--rw-r--r--   0        0        0     1561 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/pattern.py
--rw-r--r--   0        0        0     4627 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/prospective_task_config.py
--rw-r--r--   0        0        0     2568 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/queue/entity.py
--rw-r--r--   0        0        0      874 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/queue/field_value.py
--rw-r--r--   0        0        0     1023 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/queue/queue.py
--rw-r--r--   0        0        0      416 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/shared_schemas/field_restriction.py
--rw-r--r--   0        0        0      549 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/shared_schemas/field_search_request.py
--rw-r--r--   0        0        0      534 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/shared_schemas/iri_list_schema.py
--rw-r--r--   0        0        0      648 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/shared_schemas/sort_order.py
--rw-r--r--   0        0        0     1585 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/task/ad_hoc_task.py
--rw-r--r--   0        0        0     6115 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/task/task.py
--rw-r--r--   0        0        0      834 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/tenant_config/tenant_config.py
--rw-r--r--   0        0        0      562 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/workflow/config_mapping.py
--rw-r--r--   0        0        0     1948 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/workflow/workflow.py
--rw-r--r--   0        0        0        0 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/py.typed
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 s4_platform_api-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/LICENSE
+-rw-r--r--   0        0        0       76 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/README.md
+-rw-r--r--   0        0        0      794 2024-04-30 20:48:13.314416 s4_platform_api-3553.3553.3553/pyproject.toml
+-rw-r--r--   0        0        0       20 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/.env
+-rw-r--r--   0        0        0        0 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/__init__.py
+-rw-r--r--   0        0        0    17057 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/api.py
+-rw-r--r--   0        0        0     1530 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/authentication_utils.py
+-rw-r--r--   0        0        0     3829 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/changeset/changeset.py
+-rw-r--r--   0        0        0     1437 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/changeset/changeset_config.py
+-rw-r--r--   0        0        0     1019 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/changeset/deploy_changeset.py
+-rw-r--r--   0        0        0     2256 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/claim/claim.py
+-rw-r--r--   0        0        0      742 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/config/config.py
+-rw-r--r--   0        0        0     6877 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/connection.py
+-rw-r--r--   0        0        0     1607 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/constants.py
+-rw-r--r--   0        0        0     2233 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/deployment/deployment.py
+-rw-r--r--   0        0        0     2174 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/entity/ad_hoc_entity.py
+-rw-r--r--   0        0        0     8301 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/entity/entity.py
+-rw-r--r--   0        0        0     1015 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/entity/field_value.py
+-rw-r--r--   0        0        0     1196 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/entity_location/entity_location.py
+-rw-r--r--   0        0        0     7065 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/entity_type/entity_type.py
+-rw-r--r--   0        0        0     2424 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/environment/environment.py
+-rw-r--r--   0        0        0      584 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/environment/environment_configuration.py
+-rw-r--r--   0        0        0     2193 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/environment/migration_plan.py
+-rw-r--r--   0        0        0      246 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/faas/custom_errors.py
+-rw-r--r--   0        0        0     2749 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/faas/faas_function.py
+-rw-r--r--   0        0        0     5635 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/faas/faas_utils.py
+-rw-r--r--   0        0        0     4437 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/file/file_reference.py
+-rw-r--r--   0        0        0     1184 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/function/function.py
+-rw-r--r--   0        0        0      248 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/internal/base_model.py
+-rw-r--r--   0        0        0     1221 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/internal/base_schema.py
+-rw-r--r--   0        0        0      637 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/internal/camel_case_schema.py
+-rw-r--r--   0        0        0     2717 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/internal/fields_mixin.py
+-rw-r--r--   0        0        0     2153 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/internal/lazy_property.py
+-rw-r--r--   0        0        0     2030 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/internal/lazy_property_list.py
+-rw-r--r--   0        0        0       80 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/internal/sort_direction.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/link_config/__init__.py
+-rw-r--r--   0        0        0      791 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/link_config/link_config.py
+-rw-r--r--   0        0        0      564 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/link_config/new_workbook_link.py
+-rw-r--r--   0        0        0      674 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/page_config/page_config.py
+-rw-r--r--   0        0        0      801 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/page_config/page_container.py
+-rw-r--r--   0        0        0      618 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/page_config/page_container_page_config.py
+-rw-r--r--   0        0        0     3229 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task/ProspectiveTaskSummary.py
+-rw-r--r--   0        0        0      728 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task/function_list.py
+-rw-r--r--   0        0        0      910 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task/function_status.py
+-rw-r--r--   0        0        0     1287 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task/io_group.py
+-rw-r--r--   0        0        0     2162 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task/prospective_entity.py
+-rw-r--r--   0        0        0     1024 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task/prospective_field_value.py
+-rw-r--r--   0        0        0    14272 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task/prospective_task.py
+-rw-r--r--   0        0        0     3260 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task/search.py
+-rw-r--r--   0        0        0      370 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/copy_forward_config.py
+-rw-r--r--   0        0        0     2471 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/field_config.py
+-rw-r--r--   0        0        0     1966 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/field_type.py
+-rw-r--r--   0        0        0      749 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/field_validation.py
+-rw-r--r--   0        0        0      639 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/from_pool_config.py
+-rw-r--r--   0        0        0     1914 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/group_config.py
+-rw-r--r--   0        0        0     1343 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/io_group_config.py
+-rw-r--r--   0        0        0     1561 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/pattern.py
+-rw-r--r--   0        0        0     4627 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/prospective_task_config.py
+-rw-r--r--   0        0        0     2568 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/queue/entity.py
+-rw-r--r--   0        0        0      874 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/queue/field_value.py
+-rw-r--r--   0        0        0     1023 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/queue/queue.py
+-rw-r--r--   0        0        0      416 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/shared_schemas/field_restriction.py
+-rw-r--r--   0        0        0      549 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/shared_schemas/field_search_request.py
+-rw-r--r--   0        0        0      534 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/shared_schemas/iri_list_schema.py
+-rw-r--r--   0        0        0      648 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/shared_schemas/sort_order.py
+-rw-r--r--   0        0        0     1642 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/storage_view_config/storage_view_config.py
+-rw-r--r--   0        0        0     1585 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/task/ad_hoc_task.py
+-rw-r--r--   0        0        0     6115 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/task/task.py
+-rw-r--r--   0        0        0      834 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/tenant_config/tenant_config.py
+-rw-r--r--   0        0        0      562 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/workflow/config_mapping.py
+-rw-r--r--   0        0        0     1948 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/platform/workflow/workflow.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:48:01.414254 s4_platform_api-3553.3553.3553/s4/py.typed
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 s4_platform_api-3553.3553.3553/PKG-INFO
```

### Comparing `s4_platform_api-1.3.0/LICENSE` & `s4_platform_api-3553.3553.3553/LICENSE`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/pyproject.toml` & `s4_platform_api-3553.3553.3553/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "s4-platform-api"
 # version dynamically populated by CI for releases
-version = "1.3.0"
+version = "3553.3553.3553"
 description = "A general purpose library for interacting with the Semaphore Platform API"
 authors = ["Semaphore Solutions <info@semaphoresolutions.ca>"]
 readme = "README.md"
 packages = [{include = "s4"}]
 license = "MIT"
 exclude = ["README.internal.md"]
 
@@ -13,14 +13,15 @@
 python = "^3.9"
 python-dotenv = "^0.19.2"
 requests = "^2.31.0"
 marshmallow = "^3.15.0"
 marshmallow-enum = "^1.5.1"
 pyjson5 = "*"
 ddtrace = "^1.17.0"
+cyclonedx-bom = "^4.1.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.0"
 pytest-mock = "^3.7.0"
 mypy = "0.971"
 pip-licenses = "4.0.0"
 deepdiff = "^6.7.1"
```

### Comparing `s4_platform_api-1.3.0/s4/platform/api.py` & `s4_platform_api-3553.3553.3553/s4/platform/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,18 @@
 from s4.platform.environment.environment import Environment, EnvironmentSchema
 from s4.platform.environment.environment_configuration import EnvironmentConfiguration
 from s4.platform.environment.migration_plan import MigrationPlan
 from s4.platform.file.file_reference import FileReference
 from s4.platform.function.function import Function, FunctionSchema
 from s4.platform.link_config.link_config import LinkConfig, LinkConfigSchema
 from s4.platform.page_config.page_config import PageConfig, PageConfigSchema
+from s4.platform.config.config import Config, ConfigSchema
+from s4.platform.storage_view_config.storage_view_config import StorageViewConfig, StorageViewConfigSchema
 from s4.platform.page_config.page_container import PageContainer, PageContainerSchema
-from s4.platform.prospective_task.prospective_task import ProspectiveTask
+from s4.platform.prospective_task.prospective_task import ProspectiveTask, ProspectiveTaskSchema
 from s4.platform.prospective_task.search import (
     SortDescriptor,
     ProspectiveTaskSummaryPage,
     ProspectiveTaskSearchRequest,
     ProspectiveTaskSearchRequestSchema,
     ProspectiveTaskSummaryPageSchema,
 )
@@ -67,14 +69,24 @@
 
     #
     # ProspectiveTask
     #
     def start_workflow(self, workflow_iri: str) -> ProspectiveTask:
         return ProspectiveTask.start_workflow(self.connection, workflow_iri)
 
+    def start_workflow_with_input_entities(self, workflow_id: str, entity_iris: list[str]) -> list[ProspectiveTask]:
+        schema = ProspectiveTaskSchema(many=True)
+        request_body = {
+            "data": entity_iris
+        }
+        result = self.connection.post_json(f"workflow/{workflow_id}/start/toProspectiveTasks", request_body)
+
+        return schema.load(result)
+
+
     def prospective_task_by_id(self, id_: str) -> ProspectiveTask:
         return ProspectiveTask.by_id(self.connection, id_)
 
     def prospective_task_create(
         self, workflow_iri: str, activity_id: str, input_entity_iris: list[str]
     ) -> ProspectiveTask:
         return ProspectiveTask.create(
@@ -344,14 +356,33 @@
     # Entity Location
     #
     def get_locations_for_entities(self, entity_iris: list[str]) -> list[EntityLocation]:
         result = self.connection.post_json_array("entityLocation", entity_iris)
         return EntityLocationSchema(many=True).load(result)
 
     #
+    # Generic Config
+    #
+    def post_config(self, config: Config) -> Config:
+        schema = ConfigSchema()
+        payload = schema.dump(config)
+        result = self.connection.post_json("config", payload)
+        return schema.load(result)
+
+    def get_config_by_id(self, config_id: str) -> Config:
+        schema = ConfigSchema()
+        result = self.connection.fetch_json(f"config/{config_id}")
+        return schema.load(result)
+
+    def get_configs_for_environment(self, environment_name: str) -> list[Config]:
+        schema = ConfigSchema(many=True)
+        result = self.connection.fetch_json(f"environment/{environment_name}/configs")
+        return schema.load(result)
+
+    #
     # Link Config
     #
     def config_link_create(self, link_config: LinkConfig) -> LinkConfig:
         schema = LinkConfigSchema()
         payload = schema.dump(link_config)
         result = self.connection.post_json("linkConfig", payload)
         return schema.load(result)
@@ -367,14 +398,41 @@
 
     def post_page_container(self, page_container: PageContainer) -> PageContainer:
         schema = PageContainerSchema()
         payload = schema.dump(page_container)
         result = self.connection.post_json("config/pageContainer", payload)
         return schema.load(result)
 
+
+    #
+    # Storage View Config
+    #
+    def post_storage_view_config(self, storage_view_config: StorageViewConfig) -> StorageViewConfig:
+        schema = StorageViewConfigSchema()
+        payload = schema.dump(storage_view_config)
+        result = self.connection.post_json("config/storageView", payload)
+        return schema.load(result)
+
+    def get_storage_view_config_by_id(self, storage_view_config_id: str) -> StorageViewConfig:
+        schema = StorageViewConfigSchema()
+        result = self.connection.fetch_json(f"config/storageView/{storage_view_config_id}")
+        return schema.load(result)
+
+    def get_storage_view_config_for_environment(self, environment_name:str) -> StorageViewConfig:
+        config_schema = ConfigSchema(many=True)
+        params = {
+            "configType": "StorageViewConfig"
+        }
+        configs = self.connection.fetch_json(f"environment/{environment_name}/configs", params)
+        configs_loaded: list[Config] = config_schema.load(configs)
+        if len(configs_loaded) > 1:
+            raise ValueError("environment can only have one storage view config")
+        storage_view_config_id = configs_loaded[0].iri.split("/")[-1]
+        return self.get_storage_view_config_by_id(storage_view_config_id)
+
     #
     # Tenant Config
     #
     def post_tenant_config(self, tenant_config: TenantConfig) -> TenantConfig:
         schema = TenantConfigSchema()
         payload = schema.dump(tenant_config)
         result = self.connection.post_json("tenantConfig", payload)
```

### Comparing `s4_platform_api-1.3.0/s4/platform/authentication_utils.py` & `s4_platform_api-3553.3553.3553/s4/platform/authentication_utils.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/changeset/changeset.py` & `s4_platform_api-3553.3553.3553/s4/platform/changeset/changeset.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/changeset/changeset_config.py` & `s4_platform_api-3553.3553.3553/s4/platform/changeset/changeset_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/changeset/deploy_changeset.py` & `s4_platform_api-3553.3553.3553/s4/platform/changeset/deploy_changeset.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/claim/claim.py` & `s4_platform_api-3553.3553.3553/s4/platform/claim/claim.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/connection.py` & `s4_platform_api-3553.3553.3553/s4/platform/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,33 +53,34 @@
         if self._access_token:
             self.session.headers.update(
                 {"Authorization": "Bearer " + self._access_token}
             )
 
         if environment_name:
             self.session.headers.update(({"X-S4-Env": environment_name}))
+            self.environment_name = environment_name
 
     #
     # Returns a new Connection object for the specified environment
     #
     def get_connection_for_env(self, environment_name: str):
         return Connection(
             self.platform_uri,
             self._access_token,
             self._host_namespace,
             environment_name,
         )
 
-    def fetch_json(self, relative_path: str) -> Optional[dict]:
+    def fetch_json(self, relative_path: str, params: dict = None) -> Optional[dict]:
         absolute_path = f"{self.platform_uri}/{relative_path}"
-        return self.fetch_json_from_absolute_path(absolute_path)
+        return self.fetch_json_from_absolute_path(absolute_path, params=params)
 
-    def fetch_json_from_absolute_path(self, absolute_path: str) -> Optional[dict]:
+    def fetch_json_from_absolute_path(self, absolute_path: str, params: dict = None) -> Optional[dict]:
         request_path = self.rewrite_host_namespace_url(absolute_path)
-        r = self.session.get(request_path)
+        r = self.session.get(request_path, params=params)
         return self._handle_optional_json_response(r)
 
     def fetch_json_from_iri(self, iri: str, params: dict = None) -> Optional[dict]:
         rewritten_iri = self.rewrite_host_namespace_url(iri)
         r = self.session.get(rewritten_iri, params=params)
         return self._handle_optional_json_response(r)
```

### Comparing `s4_platform_api-1.3.0/s4/platform/deployment/deployment.py` & `s4_platform_api-3553.3553.3553/s4/platform/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/entity/ad_hoc_entity.py` & `s4_platform_api-3553.3553.3553/s4/platform/entity/ad_hoc_entity.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/entity/entity.py` & `s4_platform_api-3553.3553.3553/s4/platform/entity/entity.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/entity/field_value.py` & `s4_platform_api-3553.3553.3553/s4/platform/entity/field_value.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/entity_location/entity_location.py` & `s4_platform_api-3553.3553.3553/s4/platform/entity_location/entity_location.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/entity_type/entity_type.py` & `s4_platform_api-3553.3553.3553/s4/platform/entity_type/entity_type.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/environment/environment.py` & `s4_platform_api-3553.3553.3553/s4/platform/environment/environment.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/environment/environment_configuration.py` & `s4_platform_api-3553.3553.3553/s4/platform/environment/environment_configuration.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/environment/migration_plan.py` & `s4_platform_api-3553.3553.3553/s4/platform/environment/migration_plan.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/faas/faas_function.py` & `s4_platform_api-3553.3553.3553/s4/platform/faas/faas_function.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/faas/faas_utils.py` & `s4_platform_api-3553.3553.3553/s4/platform/faas/faas_utils.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/file/file_reference.py` & `s4_platform_api-3553.3553.3553/s4/platform/file/file_reference.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/function/function.py` & `s4_platform_api-3553.3553.3553/s4/platform/function/function.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/internal/base_schema.py` & `s4_platform_api-3553.3553.3553/s4/platform/internal/base_schema.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/internal/camel_case_schema.py` & `s4_platform_api-3553.3553.3553/s4/platform/internal/camel_case_schema.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/internal/fields_mixin.py` & `s4_platform_api-3553.3553.3553/s4/platform/internal/fields_mixin.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/internal/lazy_property.py` & `s4_platform_api-3553.3553.3553/s4/platform/internal/lazy_property.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/internal/lazy_property_list.py` & `s4_platform_api-3553.3553.3553/s4/platform/internal/lazy_property_list.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/link_config/link_config.py` & `s4_platform_api-3553.3553.3553/s4/platform/link_config/link_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/link_config/new_workbook_link.py` & `s4_platform_api-3553.3553.3553/s4/platform/link_config/new_workbook_link.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/page_config/page_config.py` & `s4_platform_api-3553.3553.3553/s4/platform/page_config/page_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/page_config/page_container.py` & `s4_platform_api-3553.3553.3553/s4/platform/page_config/page_container.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/page_config/page_container_page_config.py` & `s4_platform_api-3553.3553.3553/s4/platform/page_config/page_container_page_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task/ProspectiveTaskSummary.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task/ProspectiveTaskSummary.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task/function_list.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task/function_list.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task/function_status.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task/function_status.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task/io_group.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task/io_group.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task/prospective_entity.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task/prospective_entity.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task/prospective_field_value.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task/prospective_field_value.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task/prospective_task.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task/prospective_task.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task/search.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task/search.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task_config/field_config.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/field_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task_config/field_type.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/field_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     )
     JSON = (
         "http://www.semaphoresolutions.com/schema/2020/platform#text/json"
     )
     SEQUENCE_TYPE = (
         "http://www.semaphoresolutions.com/schema/2020/platform#Sequence"
     )
+    TASK_IRI = "http://www.semaphoresolutions.com/schema/2020/platform#taskIri"
 
     @staticmethod
     def from_str(value: str) -> Optional["FieldType"]:
         for (name, member) in FieldType.__members__.items():
             if member.value == value:
                 return member
         return None
```

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task_config/field_validation.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/field_validation.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task_config/from_pool_config.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/from_pool_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task_config/group_config.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/group_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task_config/io_group_config.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/io_group_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task_config/pattern.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/pattern.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/prospective_task_config/prospective_task_config.py` & `s4_platform_api-3553.3553.3553/s4/platform/prospective_task_config/prospective_task_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/queue/entity.py` & `s4_platform_api-3553.3553.3553/s4/platform/queue/entity.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/queue/field_value.py` & `s4_platform_api-3553.3553.3553/s4/platform/queue/field_value.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/queue/queue.py` & `s4_platform_api-3553.3553.3553/s4/platform/queue/queue.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/shared_schemas/field_search_request.py` & `s4_platform_api-3553.3553.3553/s4/platform/shared_schemas/field_search_request.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/shared_schemas/iri_list_schema.py` & `s4_platform_api-3553.3553.3553/s4/platform/shared_schemas/iri_list_schema.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/shared_schemas/sort_order.py` & `s4_platform_api-3553.3553.3553/s4/platform/shared_schemas/sort_order.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/task/ad_hoc_task.py` & `s4_platform_api-3553.3553.3553/s4/platform/task/ad_hoc_task.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/task/task.py` & `s4_platform_api-3553.3553.3553/s4/platform/task/task.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/tenant_config/tenant_config.py` & `s4_platform_api-3553.3553.3553/s4/platform/tenant_config/tenant_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/workflow/config_mapping.py` & `s4_platform_api-3553.3553.3553/s4/platform/workflow/config_mapping.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/s4/platform/workflow/workflow.py` & `s4_platform_api-3553.3553.3553/s4/platform/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.3.0/PKG-INFO` & `s4_platform_api-3553.3553.3553/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: s4-platform-api
-Version: 1.3.0
+Version: 3553.3553.3553
 Summary: A general purpose library for interacting with the Semaphore Platform API
 License: MIT
 Author: Semaphore Solutions
 Author-email: info@semaphoresolutions.ca
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: cyclonedx-bom (>=4.1.4,<5.0.0)
 Requires-Dist: ddtrace (>=1.17.0,<2.0.0)
 Requires-Dist: marshmallow (>=3.15.0,<4.0.0)
 Requires-Dist: marshmallow-enum (>=1.5.1,<2.0.0)
 Requires-Dist: pyjson5
 Requires-Dist: python-dotenv (>=0.19.2,<0.20.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
```

