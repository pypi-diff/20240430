# Comparing `tmp/resc_backend-3.0.2.tar.gz` & `tmp/resc_backend-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_backend-3.0.2.tar", last modified: Fri Apr 19 10:39:53 2024, max compression
+gzip compressed data, was "resc_backend-4.0.0.tar", last modified: Tue Apr 30 15:21:35 2024, max compression
```

## Comparing `resc_backend-3.0.2.tar` & `resc_backend-4.0.0.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:53.816582 resc_backend-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 10:39:49.000000 resc_backend-3.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-04-19 10:39:53.816582 resc_backend-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-19 10:39:49.000000 resc_backend-3.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-19 10:39:53.816582 resc_backend-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 10:39:49.000000 resc_backend-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:53.800582 resc_backend-3.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:53.804582 resc_backend-3.0.2/src/resc_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:53.804582 resc_backend-3.0.2/src/resc_backend/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/bin/rabbitmq_bootup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:53.804582 resc_backend-3.0.2/src/resc_backend/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/db/engine_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:53.804582 resc_backend-3.0.2/src/resc_backend/db/model/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/db/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/db/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/db/model/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/db/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/db/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/db/model/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/db/model/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/db/model/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/db/model/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/db/model/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/db/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/db/model/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:53.808582 resc_backend-3.0.2/src/resc_backend/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/helpers/dict_remapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/helpers/environment_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:53.808582 resc_backend-3.0.2/src/resc_backend/helpers/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/helpers/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/helpers/rabbitmq/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:53.808582 resc_backend-3.0.2/src/resc_backend/resc_web_service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:53.808582 resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)    34231 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:53.812582 resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
--rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    13081 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    20677 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    17679 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:53.812582 resc_backend-3.0.2/src/resc_backend/resc_web_service/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/helpers/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/helpers/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:53.816582 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/audit_count_over_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/date_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/date_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/finding_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/finding_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/pagination_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/repository_enriched.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/rule_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/status_count.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/time_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/vcs_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:53.816582 resc_backend-3.0.2/src/resc_backend/resc_web_service_interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service_interface/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service_interface/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service_interface/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service_interface/scans.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-19 10:39:49.000000 resc_backend-3.0.2/src/resc_backend/resc_web_service_interface/vcs_instances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:39:53.804582 resc_backend-3.0.2/src/resc_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-04-19 10:39:53.000000 resc_backend-3.0.2/src/resc_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-19 10:39:53.000000 resc_backend-3.0.2/src/resc_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:39:53.000000 resc_backend-3.0.2/src/resc_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-19 10:39:53.000000 resc_backend-3.0.2/src/resc_backend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:39:53.000000 resc_backend-3.0.2/src/resc_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-19 10:39:53.000000 resc_backend-3.0.2/src/resc_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 10:39:53.000000 resc_backend-3.0.2/src/resc_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.881999 resc_backend-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 15:21:29.000000 resc_backend-4.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-04-30 15:21:35.881999 resc_backend-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-30 15:21:29.000000 resc_backend-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-30 15:21:29.000000 resc_backend-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 15:21:35.885999 resc_backend-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-30 15:21:29.000000 resc_backend-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.865998 resc_backend-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.865998 resc_backend-4.0.0/src/resc_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.869998 resc_backend-4.0.0/src/resc_backend/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/bin/rabbitmq_bootup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.869998 resc_backend-4.0.0/src/resc_backend/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/engine_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.869998 resc_backend-4.0.0/src/resc_backend/db/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.869998 resc_backend-4.0.0/src/resc_backend/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/dict_remapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/environment_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.873998 resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.873998 resc_backend-4.0.0/src/resc_backend/resc_web_service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.873998 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34253 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16397 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.877998 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20677 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17679 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.877998 resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.881999 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/audit_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/date_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/date_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/pagination_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/repository_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/status_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/time_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/vcs_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.881999 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/vcs_instances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.881999 resc_backend-4.0.0/src/resc_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/top_level.txt
```

### Comparing `resc_backend-3.0.2/LICENSE.md` & `resc_backend-4.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/PKG-INFO` & `resc_backend-4.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: resc_backend
-Version: 3.0.2
-Summary: Repository Scanner - Backend
-Home-page: https://github.com/ABNAMRO/repository-scanner
-Author: ABN AMRO
-Author-email: resc@nl.abnamro.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # Repository Scanner Backend (RESC-Backend)
 [![Python][python-shield]][python-url]
 [![FastAPI][fast-api-shield]][fast-api-url]
 [![SQLAlchemy][sqlalchemy-shield]][sqlalchemy-url]
 [![Celery][celery-shield]][celery-url]
 [![Pydantic][pydantic-shield]][pydantic-url]
 [![RabbitMQ][rabbitmq-shield]][rabbitmq-url]
@@ -241,9 +228,7 @@
 [ci-shield]: https://img.shields.io/github/actions/workflow/status/abnamro/repository-scanner/backend-ci.yaml?logo=github
 [database-shield]: https://img.shields.io/badge/Azure%20SQL%20Edge-blue?logo=microsoftazure
 [database-url]: https://azure.microsoft.com/en-us/services/sql-edge
 [ci-url]: https://github.com/abnamro/repository-scanner/actions/workflows/backend-ci.yaml
 [sonar-cloud-shield]: https://sonarcloud.io/api/project_badges/measure?project=abnamro-resc_resc-backend&metric=alert_status
 [sonar-cloud-url]: https://sonarcloud.io/summary/new_code?id=abnamro-resc_resc-backend
   
-
-
```

### Comparing `resc_backend-3.0.2/setup.cfg` & `resc_backend-4.0.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [metadata]
 name = resc_backend
 description = Repository Scanner - Backend
-version = 3.0.2
+version = 4.0.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE.md
 requirements_files = file: requirements.txt
 
 [options]
-python_requires = >=3.9
+python_requires = >=3.12
 include_package_data = False
 zip_safe = False
 package_dir = = src
 packages = find:
 
 [options.packages.find]
 where = src
```

### Comparing `resc_backend-3.0.2/src/resc_backend/bin/rabbitmq_bootup.py` & `resc_backend-4.0.0/src/resc_backend/bin/rabbitmq_bootup.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/common.py` & `resc_backend-4.0.0/src/resc_backend/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Standard Library
 import logging.config
-from distutils.sysconfig import get_python_lib
+import sysconfig
 from os import path
 
 # Third Party
 import pkg_resources
 
 logger = logging.getLogger(__name__)
 
 
 def get_logging_settings_path():
-    if path.isfile(get_python_lib() + "/resc"):
-        base_dir = get_python_lib() + "/resc"
+    if path.isfile(sysconfig.get_path('purelib') + "/resc"):
+        base_dir = sysconfig.get_path('purelib') + "/resc"
     else:
         base_dir = path.dirname(__file__)
 
     return base_dir + "/static/logging.ini"
 
 
 def initialise_logs(log_file_path: str, debug=True):
```

### Comparing `resc_backend-3.0.2/src/resc_backend/constants.py` & `resc_backend-4.0.0/src/resc_backend/constants.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/db/connection.py` & `resc_backend-4.0.0/src/resc_backend/db/connection.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/db/engine_azure.py` & `resc_backend-4.0.0/src/resc_backend/db/engine_azure.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/db/model/__init__.py` & `resc_backend-4.0.0/src/resc_backend/db/model/__init__.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/db/model/audit.py` & `resc_backend-4.0.0/src/resc_backend/db/model/audit.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class DBaudit(Base):
     __tablename__ = "audit"
     id_ = Column("id", Integer, primary_key=True)
     finding_id = Column(Integer, ForeignKey("finding.id"), nullable=False)
     status = Column(
         Enum(FindingStatus),
-        default=FindingStatus.NOT_ANALYZED,
+        default=FindingStatus.NOT_ANALYZED.value,
         server_default=text("NOT_ANALYZED"),
         nullable=False,
     )
     auditor = Column(String(200))
     comment = Column(String(255), nullable=True)
     timestamp = Column(DateTime, nullable=False, default=datetime.utcnow)
     is_latest = Column(Boolean, nullable=False, default=False, server_default=text("0"))
```

### Comparing `resc_backend-3.0.2/src/resc_backend/db/model/finding.py` & `resc_backend-4.0.0/src/resc_backend/db/model/finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/db/model/repository.py` & `resc_backend-4.0.0/src/resc_backend/db/model/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/db/model/rule.py` & `resc_backend-4.0.0/src/resc_backend/db/model/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/db/model/rule_allow_list.py` & `resc_backend-4.0.0/src/resc_backend/db/model/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/db/model/rule_pack.py` & `resc_backend-4.0.0/src/resc_backend/db/model/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/db/model/scan.py` & `resc_backend-4.0.0/src/resc_backend/db/model/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/db/model/vcs_instance.py` & `resc_backend-4.0.0/src/resc_backend/db/model/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/helpers/dict_remapper.py` & `resc_backend-4.0.0/src/resc_backend/helpers/dict_remapper.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/helpers/environment_wrapper.py` & `resc_backend-4.0.0/src/resc_backend/helpers/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/helpers/rabbitmq/configuration.py` & `resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py` & `resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/api.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/api.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/cache_manager.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/cache_manager.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/configuration.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/audit.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/detailed_finding.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/detailed_finding.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             DBVcsInstance.provider_type.in_(findings_filter.vcs_providers)
         )
 
     if findings_filter.project_name:
         query = query.where(DBrepository.project_key == findings_filter.project_name)
 
     if findings_filter.finding_statuses:
-        if FindingStatus.NOT_ANALYZED in findings_filter.finding_statuses:
+        if FindingStatus.NOT_ANALYZED.value in findings_filter.finding_statuses:
             query = query.where(
                 (DBaudit.status.in_(findings_filter.finding_statuses))
                 | (DBaudit.status == None)  # noqa: E711
             )
         else:
             query = query.where(DBaudit.status.in_(findings_filter.finding_statuses))
     return query
```

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/finding.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/finding.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     if statuses_filter:
         query = query.join(
             DBaudit,
             (DBaudit.finding_id == DBfinding.id_) & (DBaudit.is_latest == True),  # noqa: E712
             isouter=True,
         )
 
-        if FindingStatus.NOT_ANALYZED in statuses_filter:
+        if FindingStatus.NOT_ANALYZED.value in statuses_filter:
             query = query.where(
                 DBaudit.status.in_(statuses_filter) | (DBaudit.status == None)  # noqa: E711
             )
         else:
             query = query.where(DBaudit.status.in_(statuses_filter))
 
     query = query.where(DBscanFinding.scan_id.in_(scan_ids))
@@ -240,15 +240,15 @@
         if findings_filter.project_name:
             query = query.where(
                 DBrepository.project_key == findings_filter.project_name
             )
         if findings_filter.rule_names:
             query = query.where(DBfinding.rule_name.in_(findings_filter.rule_names))
         if findings_filter.finding_statuses:
-            if FindingStatus.NOT_ANALYZED in findings_filter.finding_statuses:
+            if FindingStatus.NOT_ANALYZED.value in findings_filter.finding_statuses:
                 query = query.where(
                     DBaudit.status.in_(findings_filter.finding_statuses)
                     | (DBaudit.status == None)  # noqa: E711
                 )
             else:
                 query = query.where(
                     DBaudit.status.in_(findings_filter.finding_statuses)
@@ -330,25 +330,24 @@
         query = query.join(
             DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance
         )
 
     if finding_statuses:
         query = query.join(
             DBaudit,
-            (DBaudit.finding_id == DBscanFinding.finding_id)
-            & (DBaudit.is_latest == True),  # noqa: E712
+            (DBaudit.finding_id == DBfinding.id_) & (DBaudit.is_latest == True),  # noqa: E712
             isouter=True,
         )
 
     if scan_id > 0:
         query = query.join(DBscanFinding, DBscanFinding.finding_id == DBfinding.id_)
         query = query.where(DBscanFinding.scan_id == scan_id)
     else:
         if finding_statuses:
-            if FindingStatus.NOT_ANALYZED in finding_statuses:
+            if FindingStatus.NOT_ANALYZED.value in finding_statuses:
                 query = query.where(
                     DBaudit.status.in_(finding_statuses) | (DBaudit.status == None)  # noqa: E711
                 )
             else:
                 query = query.where(DBaudit.status.in_(finding_statuses))
 
         if vcs_providers:
@@ -393,25 +392,25 @@
         count of findings
     """
     query = db_connection.query(
         func.count(DBfinding.id_).label("status_count"), DBaudit.status
     )
     query = query.join(
         DBaudit,
-        (DBaudit.finding_id == DBscanFinding.finding_id) & (DBaudit.is_latest == True),  # noqa: E712
+        (DBaudit.finding_id == DBfinding.id_) & (DBaudit.is_latest == True),  # noqa: E712
         isouter=True,
     )
 
     if scan_ids and len(scan_ids) > 0:
         query = query.join(DBscanFinding, DBscanFinding.finding_id == DBfinding.id_)
         query = query.join(DBscan, DBscan.id_ == DBscanFinding.scan_id)
         query = query.where(DBscan.id_.in_(scan_ids))
 
     if finding_statuses:
-        if FindingStatus.NOT_ANALYZED in finding_statuses:
+        if FindingStatus.NOT_ANALYZED.value in finding_statuses:
             query = query.where(
                 DBaudit.status.in_(finding_statuses) | (DBaudit.status == None)  # noqa: E711
             )
         else:
             query = query.where(DBaudit.status.in_(finding_statuses))
     if rule_name:
         query = query.where(DBfinding.rule_name == rule_name)
@@ -447,15 +446,15 @@
     max_base_scan_subquery = max_base_scan_subquery.where(
         DBscan.scan_type == ScanType.BASE
     )
     if rule_pack_versions:
         max_base_scan_subquery = max_base_scan_subquery.where(
             DBscan.rule_pack.in_(rule_pack_versions)
         )
-    max_base_scan_subquery = max_base_scan_subquery.group_by(
+    max_base_scan_subquery: Query = max_base_scan_subquery.group_by(
         DBscan.repository_id
     ).subquery()
 
     query = query.join(DBscanFinding, DBfinding.id_ == DBscanFinding.finding_id)
     query = query.join(
         max_base_scan_subquery,
         DBfinding.repository_id == max_base_scan_subquery.c.repository_id,
@@ -486,15 +485,15 @@
         query = query.join(rule_tag_subquery, DBrule.id_ == rule_tag_subquery.c.rule_id)
 
     if rule_pack_versions:
         query = query.where(DBscan.rule_pack.in_(rule_pack_versions))
 
     query = query.join(
         DBaudit,
-        (DBaudit.finding_id == DBscanFinding.finding_id) & (DBaudit.is_latest == True),  # noqa: E712
+        (DBaudit.finding_id == DBfinding.id_) & (DBaudit.is_latest == True),  # noqa: E712
         isouter=True,
     )
     query = query.group_by(DBfinding.rule_name, DBaudit.status)
     query = query.order_by(DBfinding.rule_name, DBaudit.status)
     status_counts = query.all()
 
     rule_count_dict = {}
@@ -506,23 +505,23 @@
             "under_review": 0,
             "clarification_required": 0,
             "total_findings_count": 0,
         }
 
     for status_count in status_counts:
         rule_count_dict[status_count[0]]["total_findings_count"] += status_count[2]
-        if status_count[1] == FindingStatus.NOT_ANALYZED or status_count[1] is None:
+        if status_count[1] == FindingStatus.NOT_ANALYZED.value or status_count[1] is None:
             rule_count_dict[status_count[0]]["not_analyzed"] += status_count[2]
-        elif status_count[1] == FindingStatus.FALSE_POSITIVE:
+        elif status_count[1] == FindingStatus.FALSE_POSITIVE.value:
             rule_count_dict[status_count[0]]["false_positive"] += status_count[2]
-        elif status_count[1] == FindingStatus.TRUE_POSITIVE:
+        elif status_count[1] == FindingStatus.TRUE_POSITIVE.value:
             rule_count_dict[status_count[0]]["true_positive"] += status_count[2]
-        elif status_count[1] == FindingStatus.UNDER_REVIEW:
+        elif status_count[1] == FindingStatus.UNDER_REVIEW.value:
             rule_count_dict[status_count[0]]["under_review"] += status_count[2]
-        elif status_count[1] == FindingStatus.CLARIFICATION_REQUIRED:
+        elif status_count[1] == FindingStatus.CLARIFICATION_REQUIRED.value:
             rule_count_dict[status_count[0]]["clarification_required"] += status_count[
                 2
             ]
 
     return rule_count_dict
 
 
@@ -930,15 +929,15 @@
         query = query.join(
             DBaudit,
             (DBaudit.finding_id == DBfinding.id_)
             & (DBaudit.id_ == max_audit_subquery.c.audit_id),
             isouter=True,
         )
         query = query.where(
-            (DBaudit.id_ == None) | (DBaudit.status == FindingStatus.NOT_ANALYZED)  # noqa: E711
+            (DBaudit.id_ == None) | (DBaudit.status == FindingStatus.NOT_ANALYZED.value)  # noqa: E711
         )
         query = query.group_by(DBVcsInstance.provider_type)
         all_tables.append(query)
 
     # union
     unioned_query = union(*all_tables)
     count_over_time = db_connection.execute(unioned_query).all()
```

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/repository.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,23 +399,23 @@
             "not_analyzed": 0,
             "under_review": 0,
             "clarification_required": 0,
             "total_findings_count": 0,
         }
     for status_count in status_counts:
         repo_count_dict[status_count[0]]["total_findings_count"] += status_count[2]
-        if status_count[1] == FindingStatus.NOT_ANALYZED or status_count[1] is None:
+        if status_count[1] == FindingStatus.NOT_ANALYZED.value or status_count[1] is None:
             repo_count_dict[status_count[0]]["not_analyzed"] += status_count[2]
-        elif status_count[1] == FindingStatus.FALSE_POSITIVE:
+        elif status_count[1] == FindingStatus.FALSE_POSITIVE.value:
             repo_count_dict[status_count[0]]["false_positive"] += status_count[2]
-        elif status_count[1] == FindingStatus.TRUE_POSITIVE:
+        elif status_count[1] == FindingStatus.TRUE_POSITIVE.value:
             repo_count_dict[status_count[0]]["true_positive"] += status_count[2]
-        elif status_count[1] == FindingStatus.UNDER_REVIEW:
+        elif status_count[1] == FindingStatus.UNDER_REVIEW.value:
             repo_count_dict[status_count[0]]["under_review"] += status_count[2]
-        elif status_count[1] == FindingStatus.CLARIFICATION_REQUIRED:
+        elif status_count[1] == FindingStatus.CLARIFICATION_REQUIRED.value:
             repo_count_dict[status_count[0]]["clarification_required"] += status_count[
                 2
             ]
 
     return repo_count_dict
```

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/rule.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/rule_pack.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/rule_tag.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule_tag.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/scan.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/scan.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,23 +176,23 @@
             db_connection,
             scan_ids=scan_ids_latest_to_base,
             finding_statuses=FindingStatus,
         )
         for finding in findings_count_by_status:
             finding_status = finding[1]
             count = finding[0]
-            if finding_status == FindingStatus.TRUE_POSITIVE:
+            if finding_status == FindingStatus.TRUE_POSITIVE.value:
                 true_positive_count = count
-            if finding_status == FindingStatus.FALSE_POSITIVE:
+            if finding_status == FindingStatus.FALSE_POSITIVE.value:
                 false_positive_count = count
-            if finding_status == FindingStatus.NOT_ANALYZED or finding_status is None:
+            if finding_status == FindingStatus.NOT_ANALYZED.value or finding_status is None:
                 not_analyzed_count += count
-            if finding_status == FindingStatus.UNDER_REVIEW:
+            if finding_status == FindingStatus.UNDER_REVIEW.value:
                 under_review_count = count
-            if finding_status == FindingStatus.CLARIFICATION_REQUIRED:
+            if finding_status == FindingStatus.CLARIFICATION_REQUIRED.value:
                 clarification_required_count = count
 
     total_findings_count = (
         true_positive_count
         + false_positive_count
         + not_analyzed_count
         + under_review_count
```

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/scan_finding.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/scan_finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/crud/vcs_instance.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/dependencies.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/dependencies.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/common.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/common.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/detailed_findings.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/findings.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/health.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/metrics.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
 def get_finding_audit_count_over_time(
     db_connection: Session = Depends(get_db_connection),
     weeks: Optional[int] = Query(default=13, ge=1),
-    audit_status: Optional[FindingStatus] = Query(default=FindingStatus.TRUE_POSITIVE),
+    audit_status: Optional[FindingStatus] = Query(default=FindingStatus.TRUE_POSITIVE.value),
 ) -> list[FindingCountOverTime]:
     """
         Retrieve count of audited findings over time for given weeks per vcs provider
     - **db_connection**: Session of the database connection
     - **weeks**: Nr of weeks for which to retrieve the audit status count
     - **audit_status**: audit status for which to retrieve the counts, defaults to True positive
     - **return**: [DateCountModel]
```

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/repositories.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/repositories.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/rule_packs.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/rules.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,34 +123,34 @@
 
     for rule_name, rule_counts in rule_finding_counts.items():
         rule_finding_count = RuleFindingCountModel(
             rule_name=rule_name, finding_count=rule_counts["total_findings_count"]
         )
         rule_finding_count.finding_statuses_count.append(
             StatusCount(
-                status=FindingStatus.TRUE_POSITIVE, count=rule_counts["true_positive"]
+                status=FindingStatus.TRUE_POSITIVE.value, count=rule_counts["true_positive"]
             )
         )
         rule_finding_count.finding_statuses_count.append(
             StatusCount(
-                status=FindingStatus.FALSE_POSITIVE, count=rule_counts["false_positive"]
+                status=FindingStatus.FALSE_POSITIVE.value, count=rule_counts["false_positive"]
             )
         )
         rule_finding_count.finding_statuses_count.append(
             StatusCount(
-                status=FindingStatus.NOT_ANALYZED, count=rule_counts["not_analyzed"]
+                status=FindingStatus.NOT_ANALYZED.value, count=rule_counts["not_analyzed"]
             )
         )
         rule_finding_count.finding_statuses_count.append(
             StatusCount(
-                status=FindingStatus.UNDER_REVIEW, count=rule_counts["under_review"]
+                status=FindingStatus.UNDER_REVIEW.value, count=rule_counts["under_review"]
             )
         )
         rule_finding_count.finding_statuses_count.append(
             StatusCount(
-                status=FindingStatus.CLARIFICATION_REQUIRED,
+                status=FindingStatus.CLARIFICATION_REQUIRED.value,
                 count=rule_counts["clarification_required"],
             )
         )
         rule_findings_counts.append(rule_finding_count)
 
     return rule_findings_counts
```

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/scans.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/scans.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/endpoints/vcs_instances.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/filters.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/filters.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/helpers/exception_handler.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/exception_handler.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/helpers/rule.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/audit.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/detailed_finding.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/detailed_finding.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     column_start: conint(gt=-1)
     column_end: conint(gt=-1)
     commit_id: constr(max_length=120)
     commit_message: str
     commit_timestamp: datetime.datetime
     author: constr(max_length=200)
     email: constr(max_length=100)
-    status: Optional[FindingStatus] = FindingStatus.NOT_ANALYZED
+    status: Optional[FindingStatus] = FindingStatus.NOT_ANALYZED.value
     comment: Optional[constr(max_length=255)] = None
     rule_name: constr(max_length=200)
     rule_pack: constr(max_length=100)
     project_key: constr(min_length=1, max_length=100)
     repository_name: constr(min_length=1, max_length=100)
     repository_url: HttpUrl
     timestamp: datetime.datetime
@@ -75,15 +75,15 @@
     ) -> str:
         github_commit_url = f"{repository_url}/commit/{commit_id}?path=/{file_path}"
         return github_commit_url
 
     @root_validator
     def build_commit_url(cls, values) -> Dict:
         if values["status"] is None:
-            values["status"] = FindingStatus.NOT_ANALYZED
+            values["status"] = FindingStatus.NOT_ANALYZED.value
         if values["comment"] is None:
             values["comment"] = ""
         if values["vcs_provider"] == VCSProviders.BITBUCKET:
             values["commit_url"] = cls.build_bitbucket_commit_url(
                 repository_url=values["repository_url"],
                 repository_name=values["repository_name"],
                 project_key=values["project_key"],
```

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/finding.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/finding_count_model.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding_count_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/pagination_model.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/pagination_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/repository.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/repository_enriched.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/repository_enriched.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/rule.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/rule_allow_list.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/rule_count_model.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_count_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/rule_pack.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/scan.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service/schema/vcs_instance.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service_interface/findings.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service_interface/repositories.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/repositories.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service_interface/rule_packs.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/rule_packs.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend/resc_web_service_interface/vcs_instances.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/vcs_instances.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.0.2/src/resc_backend.egg-info/PKG-INFO` & `resc_backend-4.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,39 @@
 Metadata-Version: 2.1
-Name: resc-backend
-Version: 3.0.2
+Name: resc_backend
+Version: 4.0.0
 Summary: Repository Scanner - Backend
 Home-page: https://github.com/ABNAMRO/repository-scanner
+Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.9
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: celery==5.3.1
+Requires-Dist: amqp==5.1.1
+Requires-Dist: requests==2.31.0
+Requires-Dist: sqlalchemy==2.0.20
+Requires-Dist: alembic==1.11.2
+Requires-Dist: fastapi==0.110.2
+Requires-Dist: typing==3.7.4.3
+Requires-Dist: pydantic==1.10.15
+Requires-Dist: uvicorn==0.17.6
+Requires-Dist: waitress==2.1.2
+Requires-Dist: pyjwt[crypto]==2.8.0
+Requires-Dist: cryptography==42.0.4
+Requires-Dist: tenacity==8.2.2
+Requires-Dist: tomlkit==0.12.1
+Requires-Dist: python-multipart==0.0.7
+Requires-Dist: aiofiles==0.8.0
+Requires-Dist: packaging==23.1
+Requires-Dist: fastapi-cache2==0.2.1
+Requires-Dist: redis==4.6.0
+Requires-Dist: azure-identity==1.15.0
+Requires-Dist: setuptools==69.5.1
 
 # Repository Scanner Backend (RESC-Backend)
 [![Python][python-shield]][python-url]
 [![FastAPI][fast-api-shield]][fast-api-url]
 [![SQLAlchemy][sqlalchemy-shield]][sqlalchemy-url]
 [![Celery][celery-shield]][celery-url]
 [![Pydantic][pydantic-shield]][pydantic-url]
@@ -241,9 +261,7 @@
 [ci-shield]: https://img.shields.io/github/actions/workflow/status/abnamro/repository-scanner/backend-ci.yaml?logo=github
 [database-shield]: https://img.shields.io/badge/Azure%20SQL%20Edge-blue?logo=microsoftazure
 [database-url]: https://azure.microsoft.com/en-us/services/sql-edge
 [ci-url]: https://github.com/abnamro/repository-scanner/actions/workflows/backend-ci.yaml
 [sonar-cloud-shield]: https://sonarcloud.io/api/project_badges/measure?project=abnamro-resc_resc-backend&metric=alert_status
 [sonar-cloud-url]: https://sonarcloud.io/summary/new_code?id=abnamro-resc_resc-backend
   
-
-
```

### Comparing `resc_backend-3.0.2/src/resc_backend.egg-info/SOURCES.txt` & `resc_backend-4.0.0/src/resc_backend.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE.md
+README.md
 requirements.txt
 setup.cfg
 setup.py
 src/resc_backend/__init__.py
 src/resc_backend/common.py
 src/resc_backend/constants.py
 src/resc_backend.egg-info/PKG-INFO
```

