# Comparing `tmp/forestadmin_agent_toolkit-1.7.0.tar.gz` & `tmp/forestadmin_agent_toolkit-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_toolkit-1.7.0.tar", max compression
+gzip compressed data, was "forestadmin_agent_toolkit-1.8.0.tar", max compression
```

## Comparing `forestadmin_agent_toolkit-1.7.0.tar` & `forestadmin_agent_toolkit-1.8.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0        0 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/README.md
--rw-r--r--   0        0        0        0 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/__init__.py
--rw-r--r--   0        0        0     9526 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/agent.py
--rw-r--r--   0        0        0      135 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/exceptions.py
--rw-r--r--   0        0        0     2477 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/forest_logger.py
--rw-r--r--   0        0        0     4152 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/options.py
--rw-r--r--   0        0        0        0 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/actions/__init__.py
--rw-r--r--   0        0        0     2305 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/actions/requests.py
--rw-r--r--   0        0        0     9544 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/actions/resources.py
--rw-r--r--   0        0        0      464 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/base.py
--rw-r--r--   0        0        0        0 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/__init__.py
--rw-r--r--   0        0        0     1055 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py
--rw-r--r--   0        0        0     2780 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/charts_collection.py
--rw-r--r--   0        0        0     1912 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
--rw-r--r--   0        0        0    17490 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/crud.py
--rw-r--r--   0        0        0    22065 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/crud_related.py
--rw-r--r--   0        0        0     4348 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/decorators.py
--rw-r--r--   0        0        0      148 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/exceptions.py
--rw-r--r--   0        0        0    13069 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/filter.py
--rw-r--r--   0        0        0     5509 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/requests.py
--rw-r--r--   0        0        0    12193 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/stats.py
--rw-r--r--   0        0        0      935 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/ip_white_list_resource.py
--rw-r--r--   0        0        0        0 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/security/__init__.py
--rw-r--r--   0        0        0      427 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/security/exceptions.py
--rw-r--r--   0        0        0     4696 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/security/resources.py
--rw-r--r--   0        0        0        0 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 15:04:40.750577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/permissions/__init__.py
--rw-r--r--   0        0        0     1695 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py
--rw-r--r--   0        0        0      176 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/permissions/options.py
--rw-r--r--   0        0        0     9001 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/permissions/permission_service.py
--rw-r--r--   0        0        0     3261 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/permissions/permissions_functions.py
--rw-r--r--   0        0        0      406 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/permissions/permissions_types.py
--rw-r--r--   0        0        0     5276 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py
--rw-r--r--   0        0        0     3200 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py
--rw-r--r--   0        0        0     1010 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/serializers/__init__.py
--rw-r--r--   0        0        0    10346 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/serializers/json_api.py
--rw-r--r--   0        0        0        0 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     3663 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/authentication.py
--rw-r--r--   0        0        0     4557 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/context.py
--rw-r--r--   0        0        0     1252 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/context_variable_injector.py
--rw-r--r--   0        0        0      655 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/context_variable_instantiator.py
--rw-r--r--   0        0        0     1230 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/context_variables.py
--rw-r--r--   0        0        0     1661 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/csv.py
--rw-r--r--   0        0        0        0 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
--rw-r--r--   0        0        0     3019 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/action_fields.py
--rw-r--r--   0        0        0     6276 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
--rw-r--r--   0        0        0     4229 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
--rw-r--r--   0        0        0     2298 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
--rw-r--r--   0        0        0     5069 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
--rw-r--r--   0        0        0    13958 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py
--rw-r--r--   0        0        0     2461 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
--rw-r--r--   0        0        0     8562 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
--rw-r--r--   0        0        0      506 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
--rw-r--r--   0        0        0     9931 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/type.py
--rw-r--r--   0        0        0     1281 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/validation.py
--rw-r--r--   0        0        0     7303 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/http.py
--rw-r--r--   0        0        0     1774 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/id.py
--rw-r--r--   0        0        0     1889 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/ip_whitelist_util.py
--rw-r--r--   0        0        0      513 2024-04-25 15:04:40.754577 forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/token.py
--rw-r--r--   0        0        0     1776 2024-04-25 15:05:00.866517 forestadmin_agent_toolkit-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/__init__.py
+-rw-r--r--   0        0        0     9526 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/agent.py
+-rw-r--r--   0        0        0      135 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/exceptions.py
+-rw-r--r--   0        0        0     2477 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/forest_logger.py
+-rw-r--r--   0        0        0     4152 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/options.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/actions/__init__.py
+-rw-r--r--   0        0        0     2305 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/actions/requests.py
+-rw-r--r--   0        0        0     9544 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/actions/resources.py
+-rw-r--r--   0        0        0      464 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/base.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/__init__.py
+-rw-r--r--   0        0        0     1055 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py
+-rw-r--r--   0        0        0     2780 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/charts_collection.py
+-rw-r--r--   0        0        0     1912 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
+-rw-r--r--   0        0        0    17490 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/crud.py
+-rw-r--r--   0        0        0    22065 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/crud_related.py
+-rw-r--r--   0        0        0     4348 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/decorators.py
+-rw-r--r--   0        0        0      148 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/exceptions.py
+-rw-r--r--   0        0        0    13206 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/filter.py
+-rw-r--r--   0        0        0     5509 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/requests.py
+-rw-r--r--   0        0        0    12193 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/stats.py
+-rw-r--r--   0        0        0      935 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/ip_white_list_resource.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/security/__init__.py
+-rw-r--r--   0        0        0      427 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/security/exceptions.py
+-rw-r--r--   0        0        0     4696 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/security/resources.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/permissions/__init__.py
+-rw-r--r--   0        0        0     1695 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py
+-rw-r--r--   0        0        0      176 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/permissions/options.py
+-rw-r--r--   0        0        0     9001 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/permissions/permission_service.py
+-rw-r--r--   0        0        0     3261 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/permissions/permissions_functions.py
+-rw-r--r--   0        0        0      406 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/permissions/permissions_types.py
+-rw-r--r--   0        0        0     5276 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py
+-rw-r--r--   0        0        0     3200 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py
+-rw-r--r--   0        0        0     1010 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/serializers/__init__.py
+-rw-r--r--   0        0        0    10346 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/serializers/json_api.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     3663 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/authentication.py
+-rw-r--r--   0        0        0     4554 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/context.py
+-rw-r--r--   0        0        0     1252 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/context_variable_injector.py
+-rw-r--r--   0        0        0      655 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/context_variable_instantiator.py
+-rw-r--r--   0        0        0     1230 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/context_variables.py
+-rw-r--r--   0        0        0     1661 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/csv.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
+-rw-r--r--   0        0        0     3019 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/action_fields.py
+-rw-r--r--   0        0        0     6276 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
+-rw-r--r--   0        0        0     4229 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
+-rw-r--r--   0        0        0     2298 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
+-rw-r--r--   0        0        0     5069 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
+-rw-r--r--   0        0        0    13958 2024-04-30 08:42:53.133048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py
+-rw-r--r--   0        0        0     2461 2024-04-30 08:42:53.137048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
+-rw-r--r--   0        0        0     8562 2024-04-30 08:42:53.137048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
+-rw-r--r--   0        0        0      506 2024-04-30 08:42:53.137048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
+-rw-r--r--   0        0        0     9931 2024-04-30 08:42:53.137048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/type.py
+-rw-r--r--   0        0        0     1281 2024-04-30 08:42:53.137048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/validation.py
+-rw-r--r--   0        0        0     7303 2024-04-30 08:42:53.137048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/http.py
+-rw-r--r--   0        0        0     1774 2024-04-30 08:42:53.137048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/id.py
+-rw-r--r--   0        0        0     1889 2024-04-30 08:42:53.137048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/ip_whitelist_util.py
+-rw-r--r--   0        0        0      513 2024-04-30 08:42:53.137048 forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/token.py
+-rw-r--r--   0        0        0     1776 2024-04-30 08:43:09.168994 forestadmin_agent_toolkit-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.8.0/PKG-INFO
```

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/agent.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/agent.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/forest_logger.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/forest_logger.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/options.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/options.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/actions/requests.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/actions/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/actions/resources.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/actions/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/charts_collection.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/charts_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/charts_datasource.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/charts_datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/crud.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/crud.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/crud_related.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/crud_related.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/decorators.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/decorators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/filter.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,23 +100,26 @@
                 ids = []
         return ids, exclude_ids
 
     raise Exception()
 
 
 def parse_sort(request: Union[RequestCollection, RequestRelationCollection]):
-    sort_string: Optional[str] = _subset_or_query(request, "sort")
-    if not sort_string:
+    raw_sort_string: Optional[str] = _subset_or_query(request, "sort")
+    if not raw_sort_string:
         return SortFactory.by_primary_keys(_get_collection(request))
 
-    sort_field = sort_string.replace(".", ":")
-    is_descending = sort_string[0] == "-"
-    if is_descending:
-        sort_field = sort_field[1:]
-    return Sort([{"field": sort_field, "ascending": not is_descending}])
+    sort_list = []
+    for sort_string in raw_sort_string.split(","):
+        sort_field = sort_string.replace(".", ":")
+        is_descending = sort_string[0] == "-"
+        if is_descending:
+            sort_field = sort_field[1:]
+        sort_list.append({"field": sort_field, "ascending": not is_descending})
+    return Sort(sort_list)
 
 
 def parse_page(request: Request) -> Page:
     items_per_page: Optional[int] = None
     page_to_skip: Optional[int] = None
     if request.body:
         subset_query = _all_records_subset_query(request)
@@ -234,17 +237,16 @@
         PrimitiveType.DATE_ONLY: lambda value: f"{value}",
         PrimitiveType.BOOLEAN: lambda value: (
             STRING_TO_BOOLEAN[value.lower()] if isinstance(value, str) else not not value
         ),
     }
 
     return_value = value
-    if isinstance(expected_type, list) and isinstance(value, str):
-        return_value = [v.strip() for v in value.split(",")]
-
+    if isinstance(expected_type, list):
+        return_value = [v.strip() for v in value.split(",")] if isinstance(value, str) else value
         return_value = [
             _cast_to_type(item, expected_type[0])
             for item in return_value
             if not (expected_type[0] == PrimitiveType.NUMBER and not _is_str_a_number(item))
         ]
     elif expected_type in expected_type_to_cast.keys():
         method = expected_type_to_cast[expected_type]  # type:ignore
```

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/requests.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/collections/stats.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/collections/stats.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/ip_white_list_resource.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/ip_white_list_resource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/resources/security/resources.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/resources/security/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/permissions/permission_service.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/permissions/permission_service.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/permissions/permissions_functions.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/permissions/permissions_functions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/serializers/__init__.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/services/serializers/json_api.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/services/serializers/json_api.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/authentication.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/authentication.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/context.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 class Request:
     method: RequestMethod
     body: Optional[Dict[str, Any]] = None
     query: Optional[Dict[str, Any]] = None
     headers: Optional[Dict[str, str]] = None
     user: Optional[User] = None
-    client_ip: Optional[str] = (None,)
+    client_ip: Optional[str] = None
 
     def __init__(
         self,
         method: RequestMethod,
         body: Optional[Dict[str, Any]] = None,
         query: Optional[Dict[str, Any]] = None,
         headers: Optional[Dict[str, str]] = None,
```

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/context_variable_injector.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/context_variable_injector.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/context_variable_instantiator.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/context_variable_instantiator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/context_variables.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/context_variables.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/csv.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/csv.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/action_fields.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/action_fields.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/action_values.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/action_values.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/emitter.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/emitter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/filterable.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/filterable.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/type.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/type.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/forest_schema/validation.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/forest_schema/validation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/http.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/http.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/id.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/id.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/ip_whitelist_util.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/ip_whitelist_util.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/forestadmin/agent_toolkit/utils/token.py` & `forestadmin_agent_toolkit-1.8.0/forestadmin/agent_toolkit/utils/token.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.7.0/pyproject.toml` & `forestadmin_agent_toolkit-1.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-toolkit"
 description = "agent toolkit for forestadmin python agent"
-version = "1.7.0"
+version = "1.8.0"
 authors = [ "Valentin Monté <valentinm@forestadmin.com>", "Julien Barreau <julien.barreau@forestadmin.com>",]
 readme = "README.md"
 repository = "https://github.com/ForestAdmin/agent-python"
 documentation = "https://docs.forestadmin.com/developer-guide-agents-python/"
 homepage = "https://www.forestadmin.com"
 [[tool.poetry.packages]]
 include = "forestadmin"
@@ -19,15 +19,15 @@
 typing-extensions = ">=4.2.0, <5.0"
 aiohttp = "~=3.9"
 oic = "~=1.4"
 pyjwt = "^2"
 cachetools = "~=5.2"
 marshmallow-jsonapi = ">=0.24.0, <1.0"
 sseclient-py = "^1.5"
-forestadmin-datasource-toolkit = "1.7.0"
+forestadmin-datasource-toolkit = "1.8.0"
 [[tool.poetry.dependencies.pandas]]
 version = ">=1.4.0"
 python = ">=3.8"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 version = "~0.2.1"
 python = "<3.9"
```

### Comparing `forestadmin_agent_toolkit-1.7.0/PKG-INFO` & `forestadmin_agent_toolkit-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: forestadmin-agent-toolkit
-Version: 1.7.0
+Version: 1.8.0
 Summary: agent toolkit for forestadmin python agent
 Home-page: https://www.forestadmin.com
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9,<4.0)
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: cachetools (>=5.2,<6.0)
-Requires-Dist: forestadmin-datasource-toolkit (==1.7.0)
+Requires-Dist: forestadmin-datasource-toolkit (==1.8.0)
 Requires-Dist: marshmallow-jsonapi (>=0.24.0,<1.0)
 Requires-Dist: oic (>=1.4,<2.0)
 Requires-Dist: pandas (>=1.4.0) ; python_version >= "3.8"
 Requires-Dist: pyjwt (>=2,<3)
 Requires-Dist: sseclient-py (>=1.5,<2.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0)
 Project-URL: Documentation, https://docs.forestadmin.com/developer-guide-agents-python/
```

