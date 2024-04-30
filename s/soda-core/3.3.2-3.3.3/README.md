# Comparing `tmp/soda_core-3.3.2.tar.gz` & `tmp/soda_core-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_core-3.3.2.tar", last modified: Wed Apr 24 15:25:56 2024, max compression
+gzip compressed data, was "soda_core-3.3.3.tar", last modified: Tue Apr 30 11:50:27 2024, max compression
```

## Comparing `soda_core-3.3.2.tar` & `soda_core-3.3.3.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.431682 soda_core-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 15:25:40.000000 soda_core-3.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-24 15:25:56.431682 soda_core-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:25:56.431682 soda_core-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-24 15:25:40.000000 soda_core-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.411682 soda_core-3.3.2/soda/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.411682 soda_core-3.3.2/soda/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    23383 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.411682 soda_core-3.3.2/soda/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/cloud/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/cloud/dbt_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/cloud/historic_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/cloud/soda_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.411682 soda_core-3.3.2/soda/common/
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/attributes_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/aws_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/exception_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/json_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/random_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/string_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/undefined_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/common/yaml_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.415682 soda_core-3.3.2/soda/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/configuration/configuration_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.407682 soda_core-3.3.2/soda/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.415682 soda_core-3.3.2/soda/core/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/core/api/data_source_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.415682 soda_core-3.3.2/soda/execution/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.419682 soda_core-3.3.2/soda/execution/check/
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/anomaly_detection_metric_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/anomaly_metric_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/automated_monitoring_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/change_over_time_metric_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    23253 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/discover_tables_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/distribution_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/freshness_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/group_by_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/group_evolution_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/metric_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6021 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/profile_columns_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/reference_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/row_count_comparison_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/sample_tables_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    21687 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/schema_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/user_defined_failed_rows_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check/user_defined_failed_rows_expression_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/check_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    56258 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/data_source_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/data_source_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/derived_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/identity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.419682 soda_core-3.3.2/soda/execution/metric/
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/metric/column_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/metric/derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/metric/group_by_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/metric/group_evolution_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/metric/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/metric/numeric_query_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/metric/query_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/metric/reference_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/metric/schema_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/metric/user_defined_failed_rows_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/metric/user_defined_numeric_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/partition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.423682 soda_core-3.3.2/soda/execution/query/
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/query/aggregation_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/query/duplicates_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/query/group_by_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/query/group_evolution_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/query/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/query/reference_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/query/sample_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/query/schema_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/query/user_defined_failed_rows_expression_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/query/user_defined_failed_rows_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/query/user_defined_numeric_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/schema_comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/table.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/execution/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.423682 soda_core-3.3.2/soda/model/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/model/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.423682 soda_core-3.3.2/soda/profiling/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/profiling/discover_table_result_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/profiling/discover_tables_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/profiling/discover_tables_result_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/profiling/numeric_column_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/profiling/profile_columns_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/profiling/sample_tables_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/profiling/text_column_profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.423682 soda_core-3.3.2/soda/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sampler/db_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sampler/default_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sampler/http_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sampler/log_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sampler/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sampler/sample_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sampler/sample_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sampler/sample_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sampler/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sampler/soda_cloud_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    45305 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.427682 soda_core-3.3.2/soda/sodacl/
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/anomaly_detection_metric_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/anomaly_metric_check_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.431682 soda_core-3.3.2/soda/sodacl/antlr/
--rw-r--r--   0 runner    (1001) docker     (127)    17988 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/antlr/SodaCLAntlrLexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15369 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/antlr/SodaCLAntlrListener.py
--rw-r--r--   0 runner    (1001) docker     (127)   122618 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/antlr/SodaCLAntlrParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/antlr/SodaCLAntlrVisitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/change_over_time_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/change_over_time_metric_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/column_checks_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/column_configurations_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/columnset_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/data_source_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/data_source_scan_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/distribution_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/file_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/for_each_column_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/for_each_dataset_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/format_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/freshness_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/group_by_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/group_evolution_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/metric_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/metric_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/missing_and_valid_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/name_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/partition_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/reference_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/row_count_comparison_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/schema_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/sodacl_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)    92900 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/sodacl_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/table_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/tableset_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/threshold_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/user_defined_failed_rows_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/sodacl/user_defined_failed_rows_expression_check_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.431682 soda_core-3.3.2/soda/telemetry/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/telemetry/memory_span_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/telemetry/soda_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/telemetry/soda_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-24 15:25:40.000000 soda_core-3.3.2/soda/telemetry/soda_tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:56.431682 soda_core-3.3.2/soda_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-24 15:25:56.000000 soda_core-3.3.2/soda_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-24 15:25:56.000000 soda_core-3.3.2/soda_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:25:56.000000 soda_core-3.3.2/soda_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-24 15:25:56.000000 soda_core-3.3.2/soda_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-24 15:25:56.000000 soda_core-3.3.2/soda_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:25:56.000000 soda_core-3.3.2/soda_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.544847 soda_core-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 11:50:11.000000 soda_core-3.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 11:50:27.544847 soda_core-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 11:50:27.544847 soda_core-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-30 11:50:11.000000 soda_core-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.520846 soda_core-3.3.3/soda/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.524846 soda_core-3.3.3/soda/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    23383 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.524846 soda_core-3.3.3/soda/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/cloud/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/cloud/dbt_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/cloud/historic_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/cloud/soda_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.524846 soda_core-3.3.3/soda/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/attributes_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/aws_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/exception_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/json_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/random_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/string_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/undefined_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/common/yaml_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.524846 soda_core-3.3.3/soda/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/configuration/configuration_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.520846 soda_core-3.3.3/soda/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.524846 soda_core-3.3.3/soda/core/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/core/api/data_source_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.528846 soda_core-3.3.3/soda/execution/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.532847 soda_core-3.3.3/soda/execution/check/
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/anomaly_detection_metric_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/anomaly_metric_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/automated_monitoring_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/change_over_time_metric_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23233 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/discover_tables_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/distribution_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/freshness_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/group_by_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/group_evolution_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/metric_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6021 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/profile_columns_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/reference_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/row_count_comparison_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/sample_tables_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21687 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/schema_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/user_defined_failed_rows_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check/user_defined_failed_rows_expression_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/check_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56258 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/data_source_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/data_source_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/derived_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/identity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.532847 soda_core-3.3.3/soda/execution/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/metric/column_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/metric/derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/metric/group_by_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/metric/group_evolution_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/metric/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/metric/numeric_query_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/metric/query_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/metric/reference_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/metric/schema_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/metric/user_defined_failed_rows_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/metric/user_defined_numeric_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/partition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.532847 soda_core-3.3.3/soda/execution/query/
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/query/aggregation_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/query/duplicates_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/query/group_by_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/query/group_evolution_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/query/reference_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/query/sample_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/query/schema_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/query/user_defined_failed_rows_expression_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/query/user_defined_failed_rows_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/query/user_defined_numeric_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/schema_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/execution/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.532847 soda_core-3.3.3/soda/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/model/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.536846 soda_core-3.3.3/soda/profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/profiling/discover_table_result_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/profiling/discover_tables_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/profiling/discover_tables_result_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/profiling/numeric_column_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/profiling/profile_columns_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/profiling/sample_tables_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/profiling/text_column_profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.536846 soda_core-3.3.3/soda/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sampler/db_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sampler/default_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sampler/http_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sampler/log_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sampler/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sampler/sample_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sampler/sample_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sampler/sample_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sampler/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sampler/soda_cloud_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45305 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.540847 soda_core-3.3.3/soda/sodacl/
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/anomaly_detection_metric_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/anomaly_metric_check_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.540847 soda_core-3.3.3/soda/sodacl/antlr/
+-rw-r--r--   0 runner    (1001) docker     (127)    17988 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/antlr/SodaCLAntlrLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15369 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/antlr/SodaCLAntlrListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)   122618 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/antlr/SodaCLAntlrParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/antlr/SodaCLAntlrVisitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/change_over_time_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/change_over_time_metric_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/column_checks_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/column_configurations_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/columnset_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/data_source_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/data_source_scan_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/distribution_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/file_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/for_each_column_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/for_each_dataset_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/format_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/freshness_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/group_by_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/group_evolution_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/metric_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/metric_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/missing_and_valid_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/name_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/partition_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/reference_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/row_count_comparison_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/schema_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/sodacl_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93135 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/sodacl_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/table_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/tableset_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/threshold_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/user_defined_failed_rows_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/sodacl/user_defined_failed_rows_expression_check_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.544847 soda_core-3.3.3/soda/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/telemetry/memory_span_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/telemetry/soda_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/telemetry/soda_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-30 11:50:11.000000 soda_core-3.3.3/soda/telemetry/soda_tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:27.544847 soda_core-3.3.3/soda_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 11:50:27.000000 soda_core-3.3.3/soda_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-30 11:50:27.000000 soda_core-3.3.3/soda_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 11:50:27.000000 soda_core-3.3.3/soda_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 11:50:27.000000 soda_core-3.3.3/soda_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-30 11:50:27.000000 soda_core-3.3.3/soda_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 11:50:27.000000 soda_core-3.3.3/soda_core.egg-info/top_level.txt
```

### Comparing `soda_core-3.3.2/LICENSE` & `soda_core-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/PKG-INFO` & `soda_core-3.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soda-core
-Version: 3.3.2
+Version: 3.3.3
 Summary: Soda Core library & CLI
 Author: Soda Data N.V.
 Author-email: info@soda.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `soda_core-3.3.2/setup.py` & `soda_core-3.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_namespace_packages, setup
 
 package_name = "soda-core"
 # Managed by tbump - do not change manually
-package_version = "3.3.2"
+package_version = "3.3.3"
 description = "Soda Core"
 
 requires = [
     "markupsafe>=2.0.1,<=2.1.2",
     "Jinja2>=2.11,<4.0",
     "click~=8.0",
     "ruamel.yaml>=0.17.0,<0.18.0",
```

### Comparing `soda_core-3.3.2/soda/cli/cli.py` & `soda_core-3.3.3/soda/cli/cli.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/cloud/cloud.py` & `soda_core-3.3.3/soda/cloud/cloud.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/cloud/historic_descriptor.py` & `soda_core-3.3.3/soda/cloud/historic_descriptor.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/cloud/soda_cloud.py` & `soda_core-3.3.3/soda/cloud/soda_cloud.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/common/attributes_handler.py` & `soda_core-3.3.3/soda/common/attributes_handler.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/common/aws_credentials.py` & `soda_core-3.3.3/soda/common/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/common/config_helper.py` & `soda_core-3.3.3/soda/common/config_helper.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/common/exceptions.py` & `soda_core-3.3.3/soda/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/common/file_system.py` & `soda_core-3.3.3/soda/common/file_system.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/common/jinja.py` & `soda_core-3.3.3/soda/common/jinja.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/common/json_helper.py` & `soda_core-3.3.3/soda/common/json_helper.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/common/log.py` & `soda_core-3.3.3/soda/common/log.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/common/logs.py` & `soda_core-3.3.3/soda/common/logs.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/common/parser.py` & `soda_core-3.3.3/soda/common/parser.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/common/query_helper.py` & `soda_core-3.3.3/soda/common/query_helper.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/common/yaml_helper.py` & `soda_core-3.3.3/soda/common/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/configuration/configuration.py` & `soda_core-3.3.3/soda/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/configuration/configuration_parser.py` & `soda_core-3.3.3/soda/configuration/configuration_parser.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/core/api/data_source_utils.py` & `soda_core-3.3.3/soda/core/api/data_source_utils.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/anomaly_detection_metric_check.py` & `soda_core-3.3.3/soda/execution/check/anomaly_detection_metric_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/anomaly_metric_check.py` & `soda_core-3.3.3/soda/execution/check/anomaly_metric_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/automated_monitoring_run.py` & `soda_core-3.3.3/soda/execution/check/automated_monitoring_run.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/change_over_time_metric_check.py` & `soda_core-3.3.3/soda/execution/check/change_over_time_metric_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/check.py` & `soda_core-3.3.3/soda/execution/check/check.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,16 +377,16 @@
                 "diagnostics": self.get_cloud_diagnostics_dict(),
             }
         )
 
         # "contract check id" is a property used by contracts implementation.
         # Here we propagate it from the check source configuration to the check result so that
         # the contracts implementation can correlate the sodacl check result with the contract check
-        if self.check_cfg.source_configurations and "contract check id" in self.check_cfg.source_configurations:
-            self.dict["contract_check_id"] = self.check_cfg.source_configurations.get("contract check id")
+        if self.check_cfg.source_configurations and "identity" in self.check_cfg.source_configurations:
+            self.dict["source_identity"] = self.check_cfg.source_configurations.get("identity")
 
         return self.dict
 
     def get_cloud_diagnostics_dict(self) -> dict:
         csv_max_length = Cloud.CSV_TEXT_MAX_LENGTH
 
         cloud_diagnostics = {
```

### Comparing `soda_core-3.3.2/soda/execution/check/discover_tables_run.py` & `soda_core-3.3.3/soda/execution/check/discover_tables_run.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/distribution_check.py` & `soda_core-3.3.3/soda/execution/check/distribution_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/freshness_check.py` & `soda_core-3.3.3/soda/execution/check/freshness_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/group_by_check.py` & `soda_core-3.3.3/soda/execution/check/group_by_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/group_evolution_check.py` & `soda_core-3.3.3/soda/execution/check/group_evolution_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/metric_check.py` & `soda_core-3.3.3/soda/execution/check/metric_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/profile_columns_run.py` & `soda_core-3.3.3/soda/execution/check/profile_columns_run.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/reference_check.py` & `soda_core-3.3.3/soda/execution/check/reference_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/row_count_comparison_check.py` & `soda_core-3.3.3/soda/execution/check/row_count_comparison_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/sample_tables_run.py` & `soda_core-3.3.3/soda/execution/check/sample_tables_run.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/schema_check.py` & `soda_core-3.3.3/soda/execution/check/schema_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/user_defined_failed_rows_check.py` & `soda_core-3.3.3/soda/execution/check/user_defined_failed_rows_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/check/user_defined_failed_rows_expression_check.py` & `soda_core-3.3.3/soda/execution/check/user_defined_failed_rows_expression_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/column.py` & `soda_core-3.3.3/soda/execution/column.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/data_source.py` & `soda_core-3.3.3/soda/execution/data_source.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/data_source_manager.py` & `soda_core-3.3.3/soda/execution/data_source_manager.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/data_source_scan.py` & `soda_core-3.3.3/soda/execution/data_source_scan.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/data_type.py` & `soda_core-3.3.3/soda/execution/data_type.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/derived_formula.py` & `soda_core-3.3.3/soda/execution/derived_formula.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/identity.py` & `soda_core-3.3.3/soda/execution/identity.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/metric/column_metrics.py` & `soda_core-3.3.3/soda/execution/metric/column_metrics.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/metric/derived_metric.py` & `soda_core-3.3.3/soda/execution/metric/derived_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/metric/group_by_metric.py` & `soda_core-3.3.3/soda/execution/metric/group_by_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/metric/group_evolution_metric.py` & `soda_core-3.3.3/soda/execution/metric/group_evolution_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/metric/metric.py` & `soda_core-3.3.3/soda/execution/metric/metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/metric/numeric_query_metric.py` & `soda_core-3.3.3/soda/execution/metric/numeric_query_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/metric/query_metric.py` & `soda_core-3.3.3/soda/execution/metric/query_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/metric/reference_metric.py` & `soda_core-3.3.3/soda/execution/metric/reference_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/metric/schema_metric.py` & `soda_core-3.3.3/soda/execution/metric/schema_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/metric/user_defined_failed_rows_metric.py` & `soda_core-3.3.3/soda/execution/metric/user_defined_failed_rows_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/metric/user_defined_numeric_metric.py` & `soda_core-3.3.3/soda/execution/metric/user_defined_numeric_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/partition.py` & `soda_core-3.3.3/soda/execution/partition.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/query/aggregation_query.py` & `soda_core-3.3.3/soda/execution/query/aggregation_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/query/duplicates_query.py` & `soda_core-3.3.3/soda/execution/query/duplicates_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/query/group_by_query.py` & `soda_core-3.3.3/soda/execution/query/group_by_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/query/group_evolution_query.py` & `soda_core-3.3.3/soda/execution/query/group_evolution_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/query/query.py` & `soda_core-3.3.3/soda/execution/query/query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/query/reference_query.py` & `soda_core-3.3.3/soda/execution/query/reference_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/query/sample_query.py` & `soda_core-3.3.3/soda/execution/query/sample_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/query/schema_query.py` & `soda_core-3.3.3/soda/execution/query/schema_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/query/user_defined_failed_rows_expression_query.py` & `soda_core-3.3.3/soda/execution/query/user_defined_failed_rows_expression_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/query/user_defined_failed_rows_query.py` & `soda_core-3.3.3/soda/execution/query/user_defined_failed_rows_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/query/user_defined_numeric_query.py` & `soda_core-3.3.3/soda/execution/query/user_defined_numeric_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/schema_comparator.py` & `soda_core-3.3.3/soda/execution/schema_comparator.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/execution/table.py` & `soda_core-3.3.3/soda/execution/table.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/profiling/discover_table_result_table.py` & `soda_core-3.3.3/soda/profiling/discover_table_result_table.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/profiling/discover_tables_result.py` & `soda_core-3.3.3/soda/profiling/discover_tables_result.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/profiling/discover_tables_result_column.py` & `soda_core-3.3.3/soda/profiling/discover_tables_result_column.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/profiling/numeric_column_profiler.py` & `soda_core-3.3.3/soda/profiling/numeric_column_profiler.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/profiling/profile_columns_result.py` & `soda_core-3.3.3/soda/profiling/profile_columns_result.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/profiling/sample_tables_result.py` & `soda_core-3.3.3/soda/profiling/sample_tables_result.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/profiling/text_column_profiler.py` & `soda_core-3.3.3/soda/profiling/text_column_profiler.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sampler/db_sample.py` & `soda_core-3.3.3/soda/sampler/db_sample.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sampler/default_sampler.py` & `soda_core-3.3.3/soda/sampler/default_sampler.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sampler/http_sampler.py` & `soda_core-3.3.3/soda/sampler/http_sampler.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sampler/log_sampler.py` & `soda_core-3.3.3/soda/sampler/log_sampler.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sampler/sample_context.py` & `soda_core-3.3.3/soda/sampler/sample_context.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sampler/sample_ref.py` & `soda_core-3.3.3/soda/sampler/sample_ref.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sampler/sample_schema.py` & `soda_core-3.3.3/soda/sampler/sample_schema.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sampler/soda_cloud_sampler.py` & `soda_core-3.3.3/soda/sampler/soda_cloud_sampler.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/scan.py` & `soda_core-3.3.3/soda/scan.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/anomaly_detection_metric_check_cfg.py` & `soda_core-3.3.3/soda/sodacl/anomaly_detection_metric_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/anomaly_metric_check_cfg.py` & `soda_core-3.3.3/soda/sodacl/anomaly_metric_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/antlr/SodaCLAntlrLexer.py` & `soda_core-3.3.3/soda/sodacl/antlr/SodaCLAntlrLexer.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/antlr/SodaCLAntlrListener.py` & `soda_core-3.3.3/soda/sodacl/antlr/SodaCLAntlrListener.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/antlr/SodaCLAntlrParser.py` & `soda_core-3.3.3/soda/sodacl/antlr/SodaCLAntlrParser.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/antlr/SodaCLAntlrVisitor.py` & `soda_core-3.3.3/soda/sodacl/antlr/SodaCLAntlrVisitor.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/change_over_time_cfg.py` & `soda_core-3.3.3/soda/sodacl/change_over_time_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/change_over_time_metric_check_cfg.py` & `soda_core-3.3.3/soda/sodacl/change_over_time_metric_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/check_cfg.py` & `soda_core-3.3.3/soda/sodacl/check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/data_source_check_cfg.py` & `soda_core-3.3.3/soda/sodacl/data_source_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/data_source_scan_cfg.py` & `soda_core-3.3.3/soda/sodacl/data_source_scan_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/distribution_check_cfg.py` & `soda_core-3.3.3/soda/sodacl/distribution_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/format_cfg.py` & `soda_core-3.3.3/soda/sodacl/format_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/freshness_check_cfg.py` & `soda_core-3.3.3/soda/sodacl/freshness_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/group_by_check_cfg.py` & `soda_core-3.3.3/soda/sodacl/group_by_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/group_evolution_check_cfg.py` & `soda_core-3.3.3/soda/sodacl/group_evolution_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/location.py` & `soda_core-3.3.3/soda/sodacl/location.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/metric_check_cfg.py` & `soda_core-3.3.3/soda/sodacl/metric_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/missing_and_valid_cfg.py` & `soda_core-3.3.3/soda/sodacl/missing_and_valid_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/partition_cfg.py` & `soda_core-3.3.3/soda/sodacl/partition_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/reference_check_cfg.py` & `soda_core-3.3.3/soda/sodacl/reference_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/row_count_comparison_check_cfg.py` & `soda_core-3.3.3/soda/sodacl/row_count_comparison_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/schema_check_cfg.py` & `soda_core-3.3.3/soda/sodacl/schema_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/sodacl_cfg.py` & `soda_core-3.3.3/soda/sodacl/sodacl_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/sodacl_parser.py` & `soda_core-3.3.3/soda/sodacl/sodacl_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 
 ANOMALY_DETECTION_CONFIGS = "model"
 ANOMALY_DETECTION_TRAINING_DATASET_CONFIGS = "training_dataset_parameters"
 ANOMALY_DETECTION_TAKE_OVER_EXISTING_ANOMALY_SCORE_CHECK = "take_over_existing_anomaly_score_check"
 ANOMALY_DETECTION_SEVERITY_LEVEL_PARAMETERS = "severity_level_parameters"
 ANOMALY_DETECTION_WARN_ONLY = "warn_only"
 ATTRIBUTES = "attributes"
-CONTRACT_CHECK_ID = "contract check id"
 FAIL = "fail"
 FAIL_CONDITION = "fail condition"
 FAIL_QUERY = "fail query"
 FILTER = "filter"
 IDENTITY = "identity"
 KEY_COLUMNS = "key columns"
 NAME = "name"
@@ -637,25 +636,31 @@
                 if "filter" == configuration_key:
                     filter = configuration_value.strip()
                 elif "condition" == configuration_key:
                     condition = configuration_value.strip()
                 elif "method" == configuration_key:
                     method = configuration_value.strip()
                 elif configuration_key.endswith("expression"):
-                    metric_expression = configuration_value.strip()
-                    configuration_metric_name = (
-                        configuration_key[: -len(" expression")]
-                        if len(configuration_key) > len(" expression")
-                        else None
-                    )
-                    if configuration_metric_name != metric_name:
+                    if configuration_value is None:
                         self.logs.error(
-                            f'In configuration "{configuration_key}" the metric name must match exactly the metric name in the check "{metric_name}"',
+                            f'In configuration "{configuration_key}" no value is provided',
                             location=self.location,
                         )
+                    else:
+                        metric_expression = configuration_value.strip()
+                        configuration_metric_name = (
+                            configuration_key[: -len(" expression")]
+                            if len(configuration_key) > len(" expression")
+                            else None
+                        )
+                        if configuration_metric_name != metric_name:
+                            self.logs.error(
+                                f'In configuration "{configuration_key}" the metric name must match exactly the metric name in the check "{metric_name}"',
+                                location=self.location,
+                            )
                 elif configuration_key.endswith("query") or configuration_key.endswith("sql_file"):
                     if configuration_key.endswith("sql_file"):
                         fs = file_system()
                         sql_file_path = fs.join(fs.dirname(self.path_stack.file_path), configuration_value.strip())
                         metric_query = dedent(fs.file_read_as_str(sql_file_path)).strip()
                         configuration_metric_name = (
                             configuration_key[: -len(" sql_file")]
@@ -704,15 +709,14 @@
                     NAME,
                     IDENTITY,
                     WARN,
                     FAIL,
                     SAMPLES_LIMIT,
                     ATTRIBUTES,
                     ANOMALY_DETECTION_WARN_ONLY,
-                    CONTRACT_CHECK_ID,
                 ]:
                     if metric_name != "distribution_difference":
                         self.logs.error(
                             f"Skipping unsupported check configuration: {configuration_key}",
                             doc="metric_check_configurations",
                             location=self.location,
                         )
@@ -1372,15 +1376,15 @@
         samples_limit = None
         if isinstance(check_configurations, dict):
             self._push_path_element(check_str, check_configurations)
             name = self._get_optional(NAME, str)
             samples_limit = self._get_optional(SAMPLES_LIMIT, int)
 
             for configuration_key in check_configurations:
-                if configuration_key not in [NAME, SAMPLES_LIMIT, ATTRIBUTES, CONTRACT_CHECK_ID]:
+                if configuration_key not in [NAME, SAMPLES_LIMIT, ATTRIBUTES]:
                     self.logs.error(
                         f"Invalid reference check configuration key {configuration_key}", location=self.location
                     )
             self._pop_path_element()
 
         return ReferenceCheckCfg(
             source_header=header_str,
```

### Comparing `soda_core-3.3.2/soda/sodacl/table_cfg.py` & `soda_core-3.3.3/soda/sodacl/table_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/threshold_cfg.py` & `soda_core-3.3.3/soda/sodacl/threshold_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/user_defined_failed_rows_check_cfg.py` & `soda_core-3.3.3/soda/sodacl/user_defined_failed_rows_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/sodacl/user_defined_failed_rows_expression_check_cfg.py` & `soda_core-3.3.3/soda/sodacl/user_defined_failed_rows_expression_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/telemetry/memory_span_exporter.py` & `soda_core-3.3.3/soda/telemetry/memory_span_exporter.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/telemetry/soda_exporter.py` & `soda_core-3.3.3/soda/telemetry/soda_exporter.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/telemetry/soda_telemetry.py` & `soda_core-3.3.3/soda/telemetry/soda_telemetry.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda/telemetry/soda_tracer.py` & `soda_core-3.3.3/soda/telemetry/soda_tracer.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.2/soda_core.egg-info/PKG-INFO` & `soda_core-3.3.3/soda_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soda-core
-Version: 3.3.2
+Version: 3.3.3
 Summary: Soda Core library & CLI
 Author: Soda Data N.V.
 Author-email: info@soda.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `soda_core-3.3.2/soda_core.egg-info/SOURCES.txt` & `soda_core-3.3.3/soda_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

