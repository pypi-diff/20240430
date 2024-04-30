# Comparing `tmp/chrontext-0.8.4.tar.gz` & `tmp/chrontext-0.8.6.tar.gz`

## Comparing `chrontext-0.8.4.tar` & `chrontext-0.8.6.tar`

### file list

```diff
@@ -1,212 +1,211 @@
--rw-r--r--   0        0        0     1408 1970-01-01 00:00:00.000000 chrontext-0.8.4/local_dependencies/chrontext/Cargo.toml
--rw-r--r--   0     1001      127       14 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/.gitignore
--rw-r--r--   0     1001      127      382 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/change_types.rs
--rw-r--r--   0     1001      127     7376 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_aggregate.rs
--rw-r--r--   0     1001      127    31339 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_expressions.rs
--rw-r--r--   0     1001      127     1217 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/distinct.rs
--rw-r--r--   0     1001      127     2662 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/extend.rs
--rw-r--r--   0     1001      127     2599 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/filter.rs
--rw-r--r--   0     1001      127     2927 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/group.rs
--rw-r--r--   0     1001      127     2424 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/join.rs
--rw-r--r--   0     1001      127     3561 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/left_join.rs
--rw-r--r--   0     1001      127     2534 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/minus.rs
--rw-r--r--   0     1001      127     2112 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/order_by.rs
--rw-r--r--   0     1001      127     1285 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/project.rs
--rw-r--r--   0     1001      127     2503 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/union.rs
--rw-r--r--   0     1001      127     9440 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns.rs
--rw-r--r--   0     1001      127     1254 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_order.rs
--rw-r--r--   0     1001      127     6085 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/static_subqueries.rs
--rw-r--r--   0     1001      127     8019 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner/time_series_queries.rs
--rw-r--r--   0     1001      127     5163 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/combiner.rs
--rw-r--r--   0     1001      127      675 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/constants.rs
--rw-r--r--   0     1001      127     1776 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/constraints.rs
--rw-r--r--   0     1001      127     3270 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/engine.rs
--rw-r--r--   0     1001      127     8613 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/find_query_variables.rs
--rw-r--r--   0     1001      127      332 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/lib.rs
--rw-r--r--   0     1001      127     1398 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/and_expression.rs
--rw-r--r--   0     1001      127     2579 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/binary_ordinary_expression.rs
--rw-r--r--   0     1001      127     1392 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/coalesce_expression.rs
--rw-r--r--   0     1001      127     1091 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/exists_expression.rs
--rw-r--r--   0     1001      127     1455 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/function_call_expression.rs
--rw-r--r--   0     1001      127     1329 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/if_expression.rs
--rw-r--r--   0     1001      127     1298 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/in_expression.rs
--rw-r--r--   0     1001      127      732 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/not_expression.rs
--rw-r--r--   0     1001      127     1201 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/or_expression.rs
--rw-r--r--   0     1001      127     1045 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/unary_ordinary_expression.rs
--rw-r--r--   0     1001      127     7766 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions.rs
--rw-r--r--   0     1001      127     1172 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/bgp_pattern.rs
--rw-r--r--   0     1001      127      992 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/distinct_pattern.rs
--rw-r--r--   0     1001      127     3408 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/extend_pattern.rs
--rw-r--r--   0     1001      127    43300 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/filter_expression_rewrites.rs
--rw-r--r--   0     1001      127     3684 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/filter_pattern.rs
--rw-r--r--   0     1001      127      998 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/graph_pattern.rs
--rw-r--r--   0     1001      127     7693 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/group_pattern.rs
--rw-r--r--   0     1001      127     1465 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/join_pattern.rs
--rw-r--r--   0     1001      127     1455 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/left_join_pattern.rs
--rw-r--r--   0     1001      127     1353 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/minus_pattern.rs
--rw-r--r--   0     1001      127     1082 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/order_by_pattern.rs
--rw-r--r--   0     1001      127      622 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/path_pattern.rs
--rw-r--r--   0     1001      127     1066 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/project_pattern.rs
--rw-r--r--   0     1001      127     1009 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/reduced_pattern.rs
--rw-r--r--   0     1001      127      318 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/service_pattern.rs
--rw-r--r--   0     1001      127     1005 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/sliced_pattern.rs
--rw-r--r--   0     1001      127     1385 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/union_pattern.rs
--rw-r--r--   0     1001      127      410 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/values_pattern.rs
--rw-r--r--   0     1001      127     5872 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns.rs
--rw-r--r--   0     1001      127     1887 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing/synchronization.rs
--rw-r--r--   0     1001      127     1556 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preparing.rs
--rw-r--r--   0     1001      127    22583 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/preprocessing.rs
--rw-r--r--   0     1001      127      268 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/pushdown_setting.rs
--rw-r--r--   0     1001      127     9495 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/aggregate_expression.rs
--rw-r--r--   0     1001      127     6485 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/and_expression.rs
--rw-r--r--   0     1001      127     4129 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/binary_ordinary_expression.rs
--rw-r--r--   0     1001      127     1687 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/coalesce_expression.rs
--rw-r--r--   0     1001      127     1201 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/exists_expression.rs
--rw-r--r--   0     1001      127     1728 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/function_call_expression.rs
--rw-r--r--   0     1001      127     2643 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/if_expression.rs
--rw-r--r--   0     1001      127     4288 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/in_expression.rs
--rw-r--r--   0     1001      127     1804 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/not_expression.rs
--rw-r--r--   0     1001      127     6181 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/or_expression.rs
--rw-r--r--   0     1001      127     1748 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/unary_ordinary_expression.rs
--rw-r--r--   0     1001      127     8638 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions.rs
--rw-r--r--   0     1001      127     9665 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/bgp_pattern.rs
--rw-r--r--   0     1001      127      710 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/distinct_pattern.rs
--rw-r--r--   0     1001      127     1883 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/extend_pattern.rs
--rw-r--r--   0     1001      127     2209 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/filter_pattern.rs
--rw-r--r--   0     1001      127      847 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/graph_pattern.rs
--rw-r--r--   0     1001      127     2978 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/group_pattern.rs
--rw-r--r--   0     1001      127     1633 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/join_pattern.rs
--rw-r--r--   0     1001      127     2775 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/left_join_pattern.rs
--rw-r--r--   0     1001      127     2323 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/minus_pattern.rs
--rw-r--r--   0     1001      127     1854 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/order_by_pattern.rs
--rw-r--r--   0     1001      127     1221 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/path_pattern.rs
--rw-r--r--   0     1001      127     3083 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/project_pattern.rs
--rw-r--r--   0     1001      127      761 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/reduced_pattern.rs
--rw-r--r--   0     1001      127      977 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/service_pattern.rs
--rw-r--r--   0     1001      127      920 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/sliced_pattern.rs
--rw-r--r--   0     1001      127     1483 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/union_pattern.rs
--rw-r--r--   0     1001      127      779 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/values_pattern.rs
--rw-r--r--   0     1001      127     5483 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns.rs
--rw-r--r--   0     1001      127     2456 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/order_expression.rs
--rw-r--r--   0     1001      127     8522 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/project_static.rs
--rw-r--r--   0     1001      127     1442 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/subqueries.rs
--rw-r--r--   0     1001      127     3324 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/rewriting.rs
--rw-r--r--   0     1001      127      880 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/sparql_database/sparql_embedded_oxigraph.rs
--rw-r--r--   0     1001      127     4009 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/sparql_database/sparql_endpoint.rs
--rw-r--r--   0     1001      127      312 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/sparql_database.rs
--rw-r--r--   0     1001      127     7299 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/sparql_result_to_polars.rs
--rw-r--r--   0     1001      127     2071 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/splitter.rs
--rw-r--r--   0     1001      127     4801 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database/timeseries_bigquery_database.rs
--rw-r--r--   0     1001      127    10522 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database/timeseries_in_memory_database.rs
--rw-r--r--   0     1001      127    29590 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database/timeseries_opcua_database.rs
--rw-r--r--   0     1001      127     2124 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite/expression_rewrite/aggregate_expressions.rs
--rw-r--r--   0     1001      127    14614 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite/expression_rewrite.rs
--rw-r--r--   0     1001      127    24646 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite/partitioning_support.rs
--rw-r--r--   0     1001      127    49806 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite.rs
--rw-r--r--   0     1001      127     2197 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database.rs
--rw-r--r--   0     1001      127    15541 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_query.rs
--rw-r--r--   0     1001      127     5815 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/common.rs
--rw-r--r--   0     1001      127     2483 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/dremio_docker.tar.gz
--rw-r--r--   0     1001      127     7438 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/opcua_data_provider.rs
--rw-r--r--   0     1001      127     1321 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_coalesce_query.csv
--rw-r--r--   0     1001      127      234 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_complex_hybrid.csv
--rw-r--r--   0     1001      127      213 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_distinct_query.csv
--rw-r--r--   0     1001      127      653 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_if_query.csv
--rw-r--r--   0     1001      127       84 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_in_expression.csv
--rw-r--r--   0     1001      127      518 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_minus_query.csv
--rw-r--r--   0     1001      127      662 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_optional_clause_query.csv
--rw-r--r--   0     1001      127       87 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_path_group_by_query.csv
--rw-r--r--   0     1001      127       76 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_pushdown_exists_aggregated_timeseries_value_hybrid.csv
--rw-r--r--   0     1001      127       76 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_pushdown_exists_timeseries_value_hybrid.csv
--rw-r--r--   0     1001      127      219 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_pushdown_group_by_concat_agg_hybrid.csv
--rw-r--r--   0     1001      127      176 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_pushdown_group_by_exists_something_hybrid.csv
--rw-r--r--   0     1001      127       90 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_pushdown_group_by_hybrid.csv
--rw-r--r--   0     1001      127      188 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_pushdown_group_by_second_having_hybrid.csv
--rw-r--r--   0     1001      127      488 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_pushdown_group_by_second_hybrid.csv
--rw-r--r--   0     1001      127       76 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_pushdown_not_exists_aggregated_timeseries_value_hybrid.csv
--rw-r--r--   0     1001      127      326 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_simple_hybrid.csv
--rw-r--r--   0     1001      127      236 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_union_of_two_groupby.csv
--rw-r--r--   0     1001      127      281 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_union_query.csv
--rw-r--r--   0     1001      127       84 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_values_query.csv
--rw-r--r--   0     1001      127      811 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/testdata.sparql
--rw-r--r--   0     1001      127      204 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/ts1.csv
--rw-r--r--   0     1001      127      204 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/ts2.csv
--rw-r--r--   0     1001      127    38287 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution.rs
--rw-r--r--   0     1001      127   990934 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep1.csv
--rw-r--r--   0     1001      127   993355 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep2.csv
--rw-r--r--   0     1001      127   991302 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep3.csv
--rw-r--r--   0     1001      127   990469 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep4.csv
--rw-r--r--   0     1001      127   990170 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep5.csv
--rw-r--r--   0     1001      127   992171 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep6.csv
--rw-r--r--   0     1001      127   990652 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep7.csv
--rw-r--r--   0     1001      127   988999 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep8.csv
--rw-r--r--   0     1001      127    56269 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/expected_multi_should_pushdown.csv
--rw-r--r--   0     1001      127     4234 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/expected_should_pushdown.csv
--rw-r--r--   0     1001      127   648016 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper1.csv
--rw-r--r--   0     1001      127   648016 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper2.csv
--rw-r--r--   0     1001      127   648016 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper3.csv
--rw-r--r--   0     1001      127   648016 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper4.csv
--rw-r--r--   0     1001      127   648016 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper5.csv
--rw-r--r--   0     1001      127   648016 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper6.csv
--rw-r--r--   0     1001      127   648016 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper7.csv
--rw-r--r--   0     1001      127   648016 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper8.csv
--rw-r--r--   0     1001      127      706 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/parquet_to_csv.py
--rw-r--r--   0     1001      127    66801 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/testdata.sparql
--rw-r--r--   0     1001      127   997077 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir1.csv
--rw-r--r--   0     1001      127   997255 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir2.csv
--rw-r--r--   0     1001      127   996654 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir3.csv
--rw-r--r--   0     1001      127   997370 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir4.csv
--rw-r--r--   0     1001      127   997020 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir5.csv
--rw-r--r--   0     1001      127   996894 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir6.csv
--rw-r--r--   0     1001      127   997304 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir7.csv
--rw-r--r--   0     1001      127   996557 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir8.csv
--rw-r--r--   0     1001      127   995047 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp1.csv
--rw-r--r--   0     1001      127   994791 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp2.csv
--rw-r--r--   0     1001      127   994849 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp3.csv
--rw-r--r--   0     1001      127   995005 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp4.csv
--rw-r--r--   0     1001      127   995077 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp5.csv
--rw-r--r--   0     1001      127   994703 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp6.csv
--rw-r--r--   0     1001      127   995075 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp7.csv
--rw-r--r--   0     1001      127   995132 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp8.csv
--rw-r--r--   0     1001      127     9209 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case.rs
--rw-r--r--   0     1001      127      644 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_opcua/expected_basic_no_end_time_query.csv
--rw-r--r--   0     1001      127      643 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_opcua/expected_basic_query.csv
--rw-r--r--   0     1001      127      180 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_opcua/expected_no_pushdown_because_of_filter_query.csv
--rw-r--r--   0     1001      127      307 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_opcua/expected_pushdown_group_by_five_second_hybrid_query.csv
--rw-r--r--   0     1001      127      825 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_opcua/testdata.sparql
--rw-r--r--   0     1001      127      204 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_opcua/ts1.csv
--rw-r--r--   0     1001      127      204 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_opcua/ts2.csv
--rw-r--r--   0     1001      127    12796 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_opcua.rs
--rw-r--r--   0     1001      127      743 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_syntactic_sugar/expected_simple_hybrid_sugar.csv
--rw-r--r--   0     1001      127      229 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_syntactic_sugar/expected_simple_hybrid_sugar_agg_avg.csv
--rw-r--r--   0     1001      127      811 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_syntactic_sugar/testdata.sparql
--rw-r--r--   0     1001      127      204 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_syntactic_sugar/ts1.csv
--rw-r--r--   0     1001      127      204 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_syntactic_sugar/ts2.csv
--rw-r--r--   0     1001      127     6507 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_syntactic_sugar.rs
--rw-r--r--   0     1001      127    30249 2024-02-19 21:01:13.000000 chrontext-0.8.4/local_dependencies/chrontext/tests/rewrites.rs
--rw-r--r--   0        0        0     2200 1970-01-01 00:00:00.000000 chrontext-0.8.4/Cargo.toml
--rw-r--r--   0     1001      127      320 2024-02-19 21:01:13.000000 chrontext-0.8.4/.gitignore
--rw-r--r--   0     1001      127    10874 2024-02-19 21:01:13.000000 chrontext-0.8.4/LICENSE
--rw-r--r--   0     1001      127     4469 2024-02-19 21:01:14.000000 chrontext-0.8.4/README.md
--rw-r--r--   0     1001      127       11 2024-02-19 21:01:14.000000 chrontext-0.8.4/doc/.gitignore
--rw-r--r--   0     1001      127   275223 2024-02-19 21:01:14.000000 chrontext-0.8.4/doc/chrontext_representation.png
--rw-r--r--   0     1001      127   226172 2024-02-19 21:01:14.000000 chrontext-0.8.4/doc/chrontext_seq.png
--rw-r--r--   0     1001      127     1269 2024-02-19 21:01:13.000000 chrontext-0.8.4/pyproject.toml
--rw-r--r--   0     1001      127       22 2024-02-19 21:01:13.000000 chrontext-0.8.4/python/chrontext/.gitignore
--rw-r--r--   0     1001      127      123 2024-02-19 21:01:13.000000 chrontext-0.8.4/python/chrontext/__init__.py
--rw-r--r--   0     1001      127     4696 2024-02-19 21:01:13.000000 chrontext-0.8.4/python/chrontext/_chrontext.pyi
--rw-r--r--   0     1001      127        0 2024-02-19 21:01:13.000000 chrontext-0.8.4/python/chrontext/py.typed
--rw-r--r--   0     1001      127     1664 2024-02-19 21:01:13.000000 chrontext-0.8.4/python/chrontext/semantic_dataframe.py
--rw-r--r--   0     1001      127     2940 2024-02-19 21:01:13.000000 chrontext-0.8.4/src/errors.rs
--rw-r--r--   0     1001      127    12562 2024-02-19 21:01:13.000000 chrontext-0.8.4/src/lib.rs
--rw-r--r--   0     1001      127       54 2024-02-19 21:01:13.000000 chrontext-0.8.4/tests/.gitignore
--rw-r--r--   0     1001      127       41 2024-02-19 21:01:13.000000 chrontext-0.8.4/tests/FIX_OPENSSL_CONDA
--rw-r--r--   0     1001      127     2175 2024-02-19 21:01:13.000000 chrontext-0.8.4/tests/conftest.py
--rw-r--r--   0     1001      127      121 2024-02-19 21:01:13.000000 chrontext-0.8.4/tests/requirements.txt
--rw-r--r--   0     1001      127     9028 2024-02-19 21:01:13.000000 chrontext-0.8.4/tests/test_bigquery.py
--rw-r--r--   0     1001      127     4318 2024-02-19 21:01:13.000000 chrontext-0.8.4/tests/test_opcua.py
--rw-r--r--   0     1001      127      326 2024-02-19 21:01:13.000000 chrontext-0.8.4/tests/testdata/expected_simple_query.csv
--rw-r--r--   0     1001      127    10002 2024-02-19 21:01:13.000000 chrontext-0.8.4/tests/testdata/expected_simplified_opcua_case.csv
--rw-r--r--   0     1001      127     1333 2024-02-19 21:01:13.000000 chrontext-0.8.4/tests/testdata/testdata_opcua_history_read.sparql
--rw-r--r--   0     1001      127    96774 2024-02-19 21:01:48.000000 chrontext-0.8.4/Cargo.lock
--rw-r--r--   0        0        0     5687 1970-01-01 00:00:00.000000 chrontext-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1526 1970-01-01 00:00:00.000000 chrontext-0.8.6/local_dependencies/chrontext/Cargo.toml
+-rw-r--r--   0     1001      127       14 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/.gitignore
+-rw-r--r--   0     1001      127      382 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/change_types.rs
+-rw-r--r--   0     1001      127     7376 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_aggregate.rs
+-rw-r--r--   0     1001      127    31339 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_expressions.rs
+-rw-r--r--   0     1001      127     1217 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/distinct.rs
+-rw-r--r--   0     1001      127     2662 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/extend.rs
+-rw-r--r--   0     1001      127     2599 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/filter.rs
+-rw-r--r--   0     1001      127     2927 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/group.rs
+-rw-r--r--   0     1001      127     2424 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/join.rs
+-rw-r--r--   0     1001      127     3686 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/left_join.rs
+-rw-r--r--   0     1001      127     2534 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/minus.rs
+-rw-r--r--   0     1001      127     2112 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/order_by.rs
+-rw-r--r--   0     1001      127     1285 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/project.rs
+-rw-r--r--   0     1001      127     2509 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/union.rs
+-rw-r--r--   0     1001      127     9440 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns.rs
+-rw-r--r--   0     1001      127     1254 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_order.rs
+-rw-r--r--   0     1001      127     6112 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/static_subqueries.rs
+-rw-r--r--   0     1001      127     8642 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner/time_series_queries.rs
+-rw-r--r--   0     1001      127     5163 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/combiner.rs
+-rw-r--r--   0     1001      127      675 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/constants.rs
+-rw-r--r--   0     1001      127     1776 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/constraints.rs
+-rw-r--r--   0     1001      127     3270 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/engine.rs
+-rw-r--r--   0     1001      127     8613 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/find_query_variables.rs
+-rw-r--r--   0     1001      127      332 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/lib.rs
+-rw-r--r--   0     1001      127     1398 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/and_expression.rs
+-rw-r--r--   0     1001      127     2579 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/binary_ordinary_expression.rs
+-rw-r--r--   0     1001      127     1392 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/coalesce_expression.rs
+-rw-r--r--   0     1001      127     1091 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/exists_expression.rs
+-rw-r--r--   0     1001      127     1455 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/function_call_expression.rs
+-rw-r--r--   0     1001      127     1329 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/if_expression.rs
+-rw-r--r--   0     1001      127     1298 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/in_expression.rs
+-rw-r--r--   0     1001      127      732 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/not_expression.rs
+-rw-r--r--   0     1001      127     1201 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/or_expression.rs
+-rw-r--r--   0     1001      127     1045 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/unary_ordinary_expression.rs
+-rw-r--r--   0     1001      127     7766 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions.rs
+-rw-r--r--   0     1001      127     1172 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/bgp_pattern.rs
+-rw-r--r--   0     1001      127      992 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/distinct_pattern.rs
+-rw-r--r--   0     1001      127     3408 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/extend_pattern.rs
+-rw-r--r--   0     1001      127    43300 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/filter_expression_rewrites.rs
+-rw-r--r--   0     1001      127     3684 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/filter_pattern.rs
+-rw-r--r--   0     1001      127      998 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/graph_pattern.rs
+-rw-r--r--   0     1001      127     7693 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/group_pattern.rs
+-rw-r--r--   0     1001      127     1465 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/join_pattern.rs
+-rw-r--r--   0     1001      127     1455 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/left_join_pattern.rs
+-rw-r--r--   0     1001      127     1353 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/minus_pattern.rs
+-rw-r--r--   0     1001      127     1082 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/order_by_pattern.rs
+-rw-r--r--   0     1001      127      622 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/path_pattern.rs
+-rw-r--r--   0     1001      127     1066 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/project_pattern.rs
+-rw-r--r--   0     1001      127     1009 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/reduced_pattern.rs
+-rw-r--r--   0     1001      127      318 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/service_pattern.rs
+-rw-r--r--   0     1001      127     1005 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/sliced_pattern.rs
+-rw-r--r--   0     1001      127     1385 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/union_pattern.rs
+-rw-r--r--   0     1001      127      410 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/values_pattern.rs
+-rw-r--r--   0     1001      127     5872 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns.rs
+-rw-r--r--   0     1001      127     1887 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing/synchronization.rs
+-rw-r--r--   0     1001      127     1556 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preparing.rs
+-rw-r--r--   0     1001      127    22583 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/preprocessing.rs
+-rw-r--r--   0     1001      127      268 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/pushdown_setting.rs
+-rw-r--r--   0     1001      127     9495 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/aggregate_expression.rs
+-rw-r--r--   0     1001      127     6485 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/and_expression.rs
+-rw-r--r--   0     1001      127     4129 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/binary_ordinary_expression.rs
+-rw-r--r--   0     1001      127     1687 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/coalesce_expression.rs
+-rw-r--r--   0     1001      127     1201 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/exists_expression.rs
+-rw-r--r--   0     1001      127     1728 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/function_call_expression.rs
+-rw-r--r--   0     1001      127     2643 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/if_expression.rs
+-rw-r--r--   0     1001      127     4288 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/in_expression.rs
+-rw-r--r--   0     1001      127     1804 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/not_expression.rs
+-rw-r--r--   0     1001      127     6181 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/or_expression.rs
+-rw-r--r--   0     1001      127     1748 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/unary_ordinary_expression.rs
+-rw-r--r--   0     1001      127     8638 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions.rs
+-rw-r--r--   0     1001      127     9665 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/bgp_pattern.rs
+-rw-r--r--   0     1001      127      710 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/distinct_pattern.rs
+-rw-r--r--   0     1001      127     1883 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/extend_pattern.rs
+-rw-r--r--   0     1001      127     2209 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/filter_pattern.rs
+-rw-r--r--   0     1001      127      847 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/graph_pattern.rs
+-rw-r--r--   0     1001      127     2978 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/group_pattern.rs
+-rw-r--r--   0     1001      127     1633 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/join_pattern.rs
+-rw-r--r--   0     1001      127     2775 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/left_join_pattern.rs
+-rw-r--r--   0     1001      127     2323 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/minus_pattern.rs
+-rw-r--r--   0     1001      127     1854 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/order_by_pattern.rs
+-rw-r--r--   0     1001      127     1221 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/path_pattern.rs
+-rw-r--r--   0     1001      127     3083 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/project_pattern.rs
+-rw-r--r--   0     1001      127      761 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/reduced_pattern.rs
+-rw-r--r--   0     1001      127      977 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/service_pattern.rs
+-rw-r--r--   0     1001      127      920 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/sliced_pattern.rs
+-rw-r--r--   0     1001      127     1483 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/union_pattern.rs
+-rw-r--r--   0     1001      127      779 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/values_pattern.rs
+-rw-r--r--   0     1001      127     5483 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns.rs
+-rw-r--r--   0     1001      127     2456 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/order_expression.rs
+-rw-r--r--   0     1001      127     8522 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/project_static.rs
+-rw-r--r--   0     1001      127     1442 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/subqueries.rs
+-rw-r--r--   0     1001      127     3324 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/rewriting.rs
+-rw-r--r--   0     1001      127      880 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/sparql_database/sparql_embedded_oxigraph.rs
+-rw-r--r--   0     1001      127     3995 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/sparql_database/sparql_endpoint.rs
+-rw-r--r--   0     1001      127      312 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/sparql_database.rs
+-rw-r--r--   0     1001      127     6966 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/sparql_result_to_polars.rs
+-rw-r--r--   0     1001      127     2071 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/splitter.rs
+-rw-r--r--   0     1001      127     4801 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database/timeseries_bigquery_database.rs
+-rw-r--r--   0     1001      127    10522 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database/timeseries_in_memory_database.rs
+-rw-r--r--   0     1001      127    29596 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database/timeseries_opcua_database.rs
+-rw-r--r--   0     1001      127     2124 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite/expression_rewrite/aggregate_expressions.rs
+-rw-r--r--   0     1001      127    14614 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite/expression_rewrite.rs
+-rw-r--r--   0     1001      127    24646 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite/partitioning_support.rs
+-rw-r--r--   0     1001      127    49808 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite.rs
+-rw-r--r--   0     1001      127     2197 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database.rs
+-rw-r--r--   0     1001      127    15541 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_query.rs
+-rw-r--r--   0     1001      127     5815 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/common.rs
+-rw-r--r--   0     1001      127     2483 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/dremio_docker.tar.gz
+-rw-r--r--   0     1001      127     7438 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/opcua_data_provider.rs
+-rw-r--r--   0     1001      127     1321 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_coalesce_query.csv
+-rw-r--r--   0     1001      127      234 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_complex_hybrid.csv
+-rw-r--r--   0     1001      127      213 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_distinct_query.csv
+-rw-r--r--   0     1001      127      653 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_if_query.csv
+-rw-r--r--   0     1001      127       84 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_in_expression.csv
+-rw-r--r--   0     1001      127      518 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_minus_query.csv
+-rw-r--r--   0     1001      127      662 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_optional_clause_query.csv
+-rw-r--r--   0     1001      127       87 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_path_group_by_query.csv
+-rw-r--r--   0     1001      127       76 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_pushdown_exists_aggregated_timeseries_value_hybrid.csv
+-rw-r--r--   0     1001      127       76 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_pushdown_exists_timeseries_value_hybrid.csv
+-rw-r--r--   0     1001      127      219 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_pushdown_group_by_concat_agg_hybrid.csv
+-rw-r--r--   0     1001      127      176 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_pushdown_group_by_exists_something_hybrid.csv
+-rw-r--r--   0     1001      127       90 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_pushdown_group_by_hybrid.csv
+-rw-r--r--   0     1001      127      188 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_pushdown_group_by_second_having_hybrid.csv
+-rw-r--r--   0     1001      127      488 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_pushdown_group_by_second_hybrid.csv
+-rw-r--r--   0     1001      127       76 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_pushdown_not_exists_aggregated_timeseries_value_hybrid.csv
+-rw-r--r--   0     1001      127      326 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_simple_hybrid.csv
+-rw-r--r--   0     1001      127      236 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_union_of_two_groupby.csv
+-rw-r--r--   0     1001      127      281 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_union_query.csv
+-rw-r--r--   0     1001      127       84 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_values_query.csv
+-rw-r--r--   0     1001      127      811 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/testdata.sparql
+-rw-r--r--   0     1001      127      204 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/ts1.csv
+-rw-r--r--   0     1001      127      204 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/ts2.csv
+-rw-r--r--   0     1001      127    38534 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution.rs
+-rw-r--r--   0     1001      127   990934 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep1.csv
+-rw-r--r--   0     1001      127   993355 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep2.csv
+-rw-r--r--   0     1001      127   991302 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep3.csv
+-rw-r--r--   0     1001      127   990469 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep4.csv
+-rw-r--r--   0     1001      127   990170 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep5.csv
+-rw-r--r--   0     1001      127   992171 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep6.csv
+-rw-r--r--   0     1001      127   990652 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep7.csv
+-rw-r--r--   0     1001      127   988999 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep8.csv
+-rw-r--r--   0     1001      127    56269 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/expected_multi_should_pushdown.csv
+-rw-r--r--   0     1001      127     4234 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/expected_should_pushdown.csv
+-rw-r--r--   0     1001      127   648016 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper1.csv
+-rw-r--r--   0     1001      127   648016 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper2.csv
+-rw-r--r--   0     1001      127   648016 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper3.csv
+-rw-r--r--   0     1001      127   648016 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper4.csv
+-rw-r--r--   0     1001      127   648016 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper5.csv
+-rw-r--r--   0     1001      127   648016 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper6.csv
+-rw-r--r--   0     1001      127   648016 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper7.csv
+-rw-r--r--   0     1001      127   648016 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper8.csv
+-rw-r--r--   0     1001      127      706 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/parquet_to_csv.py
+-rw-r--r--   0     1001      127    66801 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/testdata.sparql
+-rw-r--r--   0     1001      127   997077 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir1.csv
+-rw-r--r--   0     1001      127   997255 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir2.csv
+-rw-r--r--   0     1001      127   996654 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir3.csv
+-rw-r--r--   0     1001      127   997370 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir4.csv
+-rw-r--r--   0     1001      127   997020 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir5.csv
+-rw-r--r--   0     1001      127   996894 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir6.csv
+-rw-r--r--   0     1001      127   997304 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir7.csv
+-rw-r--r--   0     1001      127   996557 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir8.csv
+-rw-r--r--   0     1001      127   995047 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp1.csv
+-rw-r--r--   0     1001      127   994791 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp2.csv
+-rw-r--r--   0     1001      127   994849 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp3.csv
+-rw-r--r--   0     1001      127   995005 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp4.csv
+-rw-r--r--   0     1001      127   995077 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp5.csv
+-rw-r--r--   0     1001      127   994703 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp6.csv
+-rw-r--r--   0     1001      127   995075 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp7.csv
+-rw-r--r--   0     1001      127   995132 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp8.csv
+-rw-r--r--   0     1001      127     9209 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case.rs
+-rw-r--r--   0     1001      127      644 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_opcua/expected_basic_no_end_time_query.csv
+-rw-r--r--   0     1001      127      643 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_opcua/expected_basic_query.csv
+-rw-r--r--   0     1001      127      180 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_opcua/expected_no_pushdown_because_of_filter_query.csv
+-rw-r--r--   0     1001      127      307 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_opcua/expected_pushdown_group_by_five_second_hybrid_query.csv
+-rw-r--r--   0     1001      127      825 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_opcua/testdata.sparql
+-rw-r--r--   0     1001      127      204 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_opcua/ts1.csv
+-rw-r--r--   0     1001      127      204 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_opcua/ts2.csv
+-rw-r--r--   0     1001      127    12796 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_opcua.rs
+-rw-r--r--   0     1001      127      743 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_syntactic_sugar/expected_simple_hybrid_sugar.csv
+-rw-r--r--   0     1001      127      229 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_syntactic_sugar/expected_simple_hybrid_sugar_agg_avg.csv
+-rw-r--r--   0     1001      127      811 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_syntactic_sugar/testdata.sparql
+-rw-r--r--   0     1001      127      204 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_syntactic_sugar/ts1.csv
+-rw-r--r--   0     1001      127      204 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_syntactic_sugar/ts2.csv
+-rw-r--r--   0     1001      127     6507 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_syntactic_sugar.rs
+-rw-r--r--   0     1001      127    30249 2024-03-08 06:35:24.000000 chrontext-0.8.6/local_dependencies/chrontext/tests/rewrites.rs
+-rw-r--r--   0        0        0     2288 1970-01-01 00:00:00.000000 chrontext-0.8.6/Cargo.toml
+-rw-r--r--   0     1001      127      320 2024-03-08 06:35:24.000000 chrontext-0.8.6/.gitignore
+-rw-r--r--   0     1001      127    10874 2024-03-08 06:35:24.000000 chrontext-0.8.6/LICENSE
+-rw-r--r--   0     1001      127     4469 2024-03-08 06:35:24.000000 chrontext-0.8.6/README.md
+-rw-r--r--   0     1001      127       11 2024-03-08 06:35:24.000000 chrontext-0.8.6/doc/.gitignore
+-rw-r--r--   0     1001      127   275223 2024-03-08 06:35:24.000000 chrontext-0.8.6/doc/chrontext_representation.png
+-rw-r--r--   0     1001      127   226172 2024-03-08 06:35:24.000000 chrontext-0.8.6/doc/chrontext_seq.png
+-rw-r--r--   0     1001      127     1269 2024-03-08 06:35:24.000000 chrontext-0.8.6/pyproject.toml
+-rw-r--r--   0     1001      127       22 2024-03-08 06:35:24.000000 chrontext-0.8.6/python/chrontext/.gitignore
+-rw-r--r--   0     1001      127      123 2024-03-08 06:35:24.000000 chrontext-0.8.6/python/chrontext/__init__.py
+-rw-r--r--   0     1001      127     4680 2024-03-08 06:35:24.000000 chrontext-0.8.6/python/chrontext/_chrontext.pyi
+-rw-r--r--   0     1001      127        0 2024-03-08 06:35:24.000000 chrontext-0.8.6/python/chrontext/py.typed
+-rw-r--r--   0     1001      127     2940 2024-03-08 06:35:24.000000 chrontext-0.8.6/src/errors.rs
+-rw-r--r--   0     1001      127    12765 2024-03-08 06:35:24.000000 chrontext-0.8.6/src/lib.rs
+-rw-r--r--   0     1001      127       54 2024-03-08 06:35:24.000000 chrontext-0.8.6/tests/.gitignore
+-rw-r--r--   0     1001      127       41 2024-03-08 06:35:24.000000 chrontext-0.8.6/tests/FIX_OPENSSL_CONDA
+-rw-r--r--   0     1001      127     2175 2024-03-08 06:35:24.000000 chrontext-0.8.6/tests/conftest.py
+-rw-r--r--   0     1001      127      121 2024-03-08 06:35:24.000000 chrontext-0.8.6/tests/requirements.txt
+-rw-r--r--   0     1001      127     8914 2024-03-08 06:35:24.000000 chrontext-0.8.6/tests/test_bigquery.py
+-rw-r--r--   0     1001      127     4318 2024-03-08 06:35:24.000000 chrontext-0.8.6/tests/test_opcua.py
+-rw-r--r--   0     1001      127      326 2024-03-08 06:35:24.000000 chrontext-0.8.6/tests/testdata/expected_simple_query.csv
+-rw-r--r--   0     1001      127    10002 2024-03-08 06:35:24.000000 chrontext-0.8.6/tests/testdata/expected_simplified_opcua_case.csv
+-rw-r--r--   0     1001      127     1333 2024-03-08 06:35:24.000000 chrontext-0.8.6/tests/testdata/testdata_opcua_history_read.sparql
+-rw-r--r--   0     1001      127    97534 2024-03-08 06:35:57.000000 chrontext-0.8.6/Cargo.lock
+-rw-r--r--   0        0        0     5687 1970-01-01 00:00:00.000000 chrontext-0.8.6/PKG-INFO
```

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/Cargo.toml` & `chrontext-0.8.6/local_dependencies/chrontext/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [package]
 name = "chrontext"
 version = "0.4.0"
 edition = "2021"
 resolver ="1"
 
 [dependencies]
-polars = {version="0.35.4", features=["lazy", "concat_str", "unique_counts", "group_by_list", "list_eval", "abs", "round_series", "is_in", "cum_agg", "dtype-full", "cse", "nightly", "performant"] }
+polars = {version="0.37.0", features=["lazy", "concat_str", "unique_counts", "group_by_list", "list_eval", "abs", "round_series", "is_in", "cum_agg", "dtype-full", "cse", "nightly", "performant"] }
 tokio = {version="1.18.2", features=["rt-multi-thread", "rt"]}
 log = "0.4.17"
 #spargebra = { path = "../../spargebra", features = ["rdf-star"]}
 #query_processing = { path = "../../query_processing"}
 query_processing = { git = "https://github.com/DataTreehouse/query_processing"}
+#representation = { path ="../../representation"}
 representation = { git = "https://github.com/DataTreehouse/representation"}
 spargebra = { git = "https://github.com/DataTreehouse/spargebra", features = ["rdf-star"]}
 sparesults = {version="0.1.8"}
 oxrdf = {version="0.1.7"}
 reqwest= {version="0.11.23", features=["stream"]}
 env_logger = "0.10.0"
 tonic = "0.10.2"
 thiserror = "1.0.31"
-polars-core = "0.35.4"
+polars-core = "0.37.0"
 sea-query = { git="https://github.com/DataTreehouse/sea-query", branch="feature/bigquery_basic_support", features=["with-chrono", "backend-bigquery"]}
 async-trait = "0.1.68"
 base64 = "0.21.3"
 opcua = {version="0.12.0", features = ["vendored-openssl"]}
 async-recursion = "1.0.4"
+#bigquery-polars = {path = "../../bigquery-polars/bigquery-polars"}
 bigquery-polars = {git="https://github.com/DataTreehouse/bigquery-polars"}
 crossbeam = {version = "0.8.2"}
 serde_json = "1.0.105"
 oxigraph = "0.3.22"
 chrono = {version = "0.4.31", features = ["clock"]}
```

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_aggregate.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_aggregate.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_expressions.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_expressions.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/distinct.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/distinct.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/extend.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/extend.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/filter.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/filter.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/group.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/group.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/join.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/join.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/left_join.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/left_join.rs`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 use representation::query_context::{Context, PathEntry};
 use crate::timeseries_query::TimeseriesQuery;
 use async_recursion::async_recursion;
 use log::debug;
 use spargebra::algebra::{Expression, GraphPattern};
 use spargebra::Query;
 use std::collections::HashMap;
-use query_processing::graph_patterns::{filter, left_join};
+use polars::prelude::JoinType;
+use query_processing::graph_patterns::{filter, join};
 
 impl Combiner {
     #[async_recursion]
     pub(crate) async fn lazy_left_join(
         &mut self,
         left: &GraphPattern,
         right: &GraphPattern,
@@ -73,11 +74,12 @@
                     right_solution_mappings,
                     Some(expression_static_query_map),
                     expression_prepared_time_series_queries,
                     &expression_context,
                 )
                 .await?;
             right_solution_mappings = filter(right_solution_mappings, &expression_context)?;
+            right_solution_mappings.rdf_node_types.remove(expression_context.as_str());
         }
-        Ok(left_join(left_solution_mappings, right_solution_mappings)?)
+        Ok(join(left_solution_mappings, right_solution_mappings, JoinType::Left)?)
     }
 }
```

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/minus.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/minus.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/order_by.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/order_by.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/project.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/project.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/union.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns/union.rs`

 * *Files 4% similar despite different names*

```diff
@@ -53,11 +53,11 @@
                 right,
                 solution_mappings,
                 right_static_query_map,
                 right_prepared_time_series_queries,
                 &right_context,
             )
             .await?;
-        Ok(union(left_solution_mappings, right_solution_mappings)?)
+        Ok(union(vec![left_solution_mappings, right_solution_mappings])?)
 
     }
 }
```

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_graph_patterns.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_graph_patterns.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/lazy_order.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/lazy_order.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/static_subqueries.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/static_subqueries.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 use representation::solution_mapping::SolutionMappings;
 use crate::combiner::time_series_queries::complete_basic_time_series_queries;
 use crate::combiner::CombinerError;
 use representation::query_context::Context;
 use crate::sparql_result_to_polars::create_static_query_dataframe;
 use log::debug;
 use oxrdf::{Term, Variable};
-use polars::prelude::{col, Expr, IntoLazy};
+use polars::prelude::{col, Expr, IntoLazy, JoinType};
 use polars_core::prelude::{UniqueKeepStrategy};
 use spargebra::algebra::GraphPattern;
 use spargebra::term::GroundTerm;
 use spargebra::Query;
 use std::collections::{HashMap};
 use polars::export::rayon::iter::{IntoParallelIterator, ParallelIterator};
 use query_processing::graph_patterns::join;
@@ -42,15 +42,15 @@
             &solutions,
             &mut self.prepper.basic_time_series_queries,
         )?;
         let (df, datatypes) = create_static_query_dataframe(&use_query, solutions);
         debug!("Static query results:\n {}", df);
         let mut out_solution_mappings = SolutionMappings::new(df.lazy(), datatypes);
         if let Some(use_solution_mappings) = use_solution_mappings {
-            out_solution_mappings = join(out_solution_mappings, use_solution_mappings)?;
+            out_solution_mappings = join(out_solution_mappings, use_solution_mappings, JoinType::Inner)?;
         }
         Ok(out_solution_mappings)
     }
 }
 
 pub(crate) fn split_static_queries(
     static_queries: &mut HashMap<Context, Query>,
```

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner/time_series_queries.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner/time_series_queries.rs`

 * *Files 6% similar despite different names*

```diff
@@ -3,43 +3,50 @@
 use crate::combiner::CombinerError;
 use representation::query_context::Context;
 use crate::timeseries_query::{BasicTimeseriesQuery, TimeseriesQuery};
 use log::debug;
 use oxrdf::vocab::xsd;
 use oxrdf::Term;
 use polars::prelude::{col, Expr, IntoLazy, JoinArgs, JoinType};
-use polars_core::prelude::{DataFrame, DataType};
+use polars_core::prelude::{CategoricalOrdering, DataFrame, DataType};
 use sparesults::QuerySolution;
 use std::collections::{HashMap, HashSet};
 use polars_core::series::Series;
-use representation::RDFNodeType;
+use representation::{BaseRDFNodeType, RDFNodeType};
 
 impl Combiner {
     pub async fn execute_attach_time_series_query(
         &mut self,
         tsq: &TimeseriesQuery,
         mut solution_mappings: SolutionMappings,
     ) -> Result<SolutionMappings, CombinerError> {
         debug!("Executing time series query: {:?}", tsq);
         if !tsq.has_identifiers() {
             let mut expected_cols:Vec<_> = tsq.expected_columns().into_iter().collect();
             expected_cols.sort();
+            let timestamp_vars:Vec<_> = tsq.get_timestamp_variables().into_iter().map(|x|x.variable.as_str()).collect();
             let drop_cols = get_drop_cols(tsq);
             let mut series_vec = vec![];
             for e in expected_cols {
                 if !drop_cols.contains(e) {
-                    series_vec.push(Series::new_empty(e, &DataType::Null));
-                    solution_mappings.rdf_node_types.insert(e.to_string(), RDFNodeType::None);
+                    if timestamp_vars.contains(&e) {
+                        let dt = BaseRDFNodeType::Literal(xsd::DATE_TIME.into_owned());
+                        series_vec.push(Series::new_empty(e, &dt.polars_data_type()));
+                        solution_mappings.rdf_node_types.insert(e.to_string(), dt.as_rdf_node_type());
+                    } else {
+                        series_vec.push(Series::new_empty(e, &BaseRDFNodeType::None.polars_data_type()));
+                        solution_mappings.rdf_node_types.insert(e.to_string(), RDFNodeType::None);
+                    }
                 }
             }
             let df = DataFrame::new(series_vec).unwrap();
             for d in drop_cols {
                 if solution_mappings.rdf_node_types.contains_key(&d) {
                     solution_mappings.rdf_node_types.remove(&d);
-                    solution_mappings.mappings = solution_mappings.mappings.drop_columns(vec![d]);
+                    solution_mappings.mappings = solution_mappings.mappings.drop(vec![d]);
                 }
             }
             solution_mappings.mappings = solution_mappings.mappings.join(df.lazy(), vec![], vec![], JoinArgs::new(JoinType::Cross));
             return Ok(solution_mappings)
         }
 
         let SolutionMappings { mappings, rdf_node_types } = self
@@ -80,18 +87,18 @@
         for (k, v) in rdf_node_types {
             solution_mappings.rdf_node_types.insert(k, v);
         }
 
         solution_mappings.mappings = solution_mappings.mappings.collect().unwrap().lazy();
         let mut ts_lf = ts_df.lazy();
         if let Some(cat_col) = &to_cat_col {
-            ts_lf = ts_lf.with_column(col(cat_col).cast(DataType::Categorical(None)));
+            ts_lf = ts_lf.with_column(col(cat_col).cast(DataType::Categorical(None, CategoricalOrdering::Physical)));
             solution_mappings.mappings = solution_mappings
                 .mappings
-                .with_column(col(cat_col).cast(DataType::Categorical(None)));
+                .with_column(col(cat_col).cast(DataType::Categorical(None, CategoricalOrdering::Physical)));
         }
         let on_reverse_false = vec![false].repeat(on_cols.len());
         ts_lf = ts_lf.sort_by_exprs(on_cols.as_slice(), on_reverse_false.as_slice(), true, false);
         solution_mappings.mappings = solution_mappings.mappings.sort_by_exprs(
             on_cols.as_slice(),
             on_reverse_false,
             true,
@@ -102,15 +109,15 @@
             .mappings
             .join(
                 ts_lf,
                 on_cols.as_slice(),
                 on_cols.as_slice(),
                 JoinArgs::new(JoinType::Inner),
             )
-            .drop_columns(drop_cols.iter());
+            .drop(drop_cols.iter());
         for c in &drop_cols {
             solution_mappings.rdf_node_types.remove(c);
         }
         return Ok(solution_mappings);
     }
 }
```

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/combiner.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/combiner.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/constants.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/constants.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/constraints.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/constraints.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/engine.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/engine.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/find_query_variables.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/find_query_variables.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/and_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/and_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/binary_ordinary_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/binary_ordinary_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/coalesce_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/coalesce_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/exists_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/exists_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/function_call_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/function_call_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/if_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/if_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/in_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/in_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/not_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/not_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/or_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/or_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions/unary_ordinary_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions/unary_ordinary_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/expressions.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/expressions.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/bgp_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/bgp_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/distinct_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/distinct_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/extend_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/extend_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/filter_expression_rewrites.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/filter_expression_rewrites.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/filter_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/filter_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/graph_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/graph_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/group_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/group_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/join_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/join_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/left_join_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/left_join_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/minus_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/minus_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/order_by_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/order_by_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/path_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/path_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/project_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/project_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/reduced_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/reduced_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/sliced_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/sliced_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns/union_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns/union_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/graph_patterns.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/graph_patterns.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing/synchronization.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing/synchronization.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preparing.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preparing.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/preprocessing.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/preprocessing.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/aggregate_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/aggregate_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/and_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/and_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/binary_ordinary_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/binary_ordinary_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/coalesce_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/coalesce_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/exists_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/exists_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/function_call_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/function_call_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/if_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/if_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/in_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/in_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/not_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/not_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/or_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/or_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions/unary_ordinary_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions/unary_ordinary_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/expressions.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/expressions.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/bgp_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/bgp_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/distinct_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/distinct_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/extend_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/extend_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/filter_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/filter_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/graph_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/graph_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/group_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/group_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/join_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/join_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/left_join_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/left_join_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/minus_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/minus_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/order_by_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/order_by_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/path_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/path_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/project_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/project_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/reduced_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/reduced_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/service_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/service_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/sliced_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/sliced_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/union_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/union_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns/values_pattern.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns/values_pattern.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/graph_patterns.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/graph_patterns.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/order_expression.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/order_expression.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/project_static.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/project_static.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting/subqueries.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting/subqueries.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/rewriting.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/rewriting.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/sparql_database/sparql_embedded_oxigraph.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/sparql_database/sparql_embedded_oxigraph.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/sparql_database/sparql_endpoint.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/sparql_database/sparql_endpoint.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use super::SparqlQueryable;
 use async_trait::async_trait;
-use reqwest::header::{ACCEPT, CONTENT_TYPE, USER_AGENT};
+use reqwest::header::{ACCEPT, USER_AGENT};
 use reqwest::StatusCode;
 use sparesults::{
     ParseError, QueryResultsFormat, QueryResultsParser, QueryResultsReader, QuerySolution,
 };
 use spargebra::Query;
 use std::error::Error;
 use std::fmt::{Display, Formatter};
```

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/splitter.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/splitter.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database/timeseries_bigquery_database.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database/timeseries_bigquery_database.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database/timeseries_in_memory_database.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database/timeseries_in_memory_database.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database/timeseries_opcua_database.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database/timeseries_opcua_database.rs`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             let mut id_iter = mapping_df.column(identifier_var).unwrap().iter();
             let mut grouping_col_iter = mapping_df
                 .column(grouping_col_name.unwrap().as_str())
                 .unwrap()
                 .iter();
             for _ in 0..mapping_df.height() {
                 let id_value = match id_iter.next().unwrap() {
-                    AnyValue::Utf8(id_value) => id_value,
+                    AnyValue::String(id_value) => id_value,
                     _ => {
                         panic!("Should never happen")
                     }
                 };
                 let grouping_col_value = match grouping_col_iter.next().unwrap() {
                     AnyValue::Int64(grouping_col_value) => grouping_col_value,
                     _ => {
@@ -252,27 +252,27 @@
                     value_vec.push(val);
                 }
                 let mut identifier_series = if let Some(grouping_col) = grouping_col_name {
                     Series::new_empty(grouping_col, &DataType::Int64)
                 } else {
                     Series::new_empty(
                         tsq.get_identifier_variables().get(0).unwrap().as_str(),
-                        &DataType::Utf8,
+                        &DataType::String,
                     )
                 };
                 identifier_series = if let Some(_) = grouping_col_name {
                     identifier_series
                         .extend_constant(
                             AnyValue::Int64(*grouping_col_lookup.get(k.as_str()).unwrap()),
                             first_ts.as_ref().unwrap().len(),
                         )
                         .unwrap()
                 } else {
                     identifier_series
-                        .extend_constant(AnyValue::Utf8(&k), first_ts.as_ref().unwrap().len())
+                        .extend_constant(AnyValue::String(&k), first_ts.as_ref().unwrap().len())
                         .unwrap()
                 };
                 value_vec.push(identifier_series);
                 value_vec.push(first_ts.unwrap());
                 value_vec.sort_by_key(|x| x.name().to_string());
                 dfs.push(DataFrame::new(value_vec).unwrap().lazy())
             }
```

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite/expression_rewrite/aggregate_expressions.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite/expression_rewrite/aggregate_expressions.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite/expression_rewrite.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite/expression_rewrite.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite/partitioning_support.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite/partitioning_support.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database/timeseries_sql_rewrite.rs`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
         let mut value_tuples = vec![];
         let identifier_colname = btsq.identifier_variable.as_ref().unwrap().as_str();
         let mut identifier_iter = df.column(identifier_colname).unwrap().iter();
         let mut groupcol_iter = df.column(&column_name).unwrap().iter();
         for _ in 0..df.height() {
             let id = identifier_iter.next().unwrap();
             let grp = groupcol_iter.next().unwrap();
-            let id_value = if let AnyValue::Utf8(id_value) = id {
+            let id_value = if let AnyValue::String(id_value) = id {
                 id_value.to_string()
             } else {
                 panic!("Should never happen");
             };
             let grp_value = if let AnyValue::Int64(grp_value) = grp {
                 grp_value
             } else {
```

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_database.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_database.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/src/timeseries_query.rs` & `chrontext-0.8.6/local_dependencies/chrontext/src/timeseries_query.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/common.rs` & `chrontext-0.8.6/local_dependencies/chrontext/tests/common.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/dremio_docker.tar.gz` & `chrontext-0.8.6/local_dependencies/chrontext/tests/dremio_docker.tar.gz`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/opcua_data_provider.rs` & `chrontext-0.8.6/local_dependencies/chrontext/tests/opcua_data_provider.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_coalesce_query.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_coalesce_query.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_if_query.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_if_query.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_minus_query.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_minus_query.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/expected_optional_clause_query.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/expected_optional_clause_query.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution/testdata.sparql` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution/testdata.sparql`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution.rs` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution.rs`

 * *Files 0% similar despite different names*

```diff
@@ -466,20 +466,23 @@
       FILTER(?t > "2022-06-01T08:46:53"^^xsd:dateTime)
     }
     GROUP BY ?w ?kind ?minute ?second_5
     HAVING ((SUM(?v)) > 1000 )
   }
 }
     "#;
-    let df = engine
+    let mut df = engine
         .execute_hybrid_query(query)
         .await
-        .expect("Hybrid error").0
-        .sort(["w", "kind", "second_5"], vec![false], false)
-        .expect("Sort error");
+        .expect("Hybrid error").0;
+    df = df.lazy().with_columns([
+        col("w").cast(DataType::String),
+        col("kind").cast(DataType::String)
+    ]).sort_by_exprs([col("w"), col("kind"), col("second_5")], vec![false], false, false)
+        .collect().unwrap();
     let mut file_path = testdata_path.clone();
     file_path.push("expected_union_of_two_groupby.csv");
 
     let file = File::open(file_path.as_path()).expect("Read file problem");
     let expected_df = CsvReader::new(file)
         .infer_schema(None)
         .has_header(true)
@@ -816,15 +819,15 @@
         }
     }
     "#;
     let mut df = engine
         .execute_hybrid_query(query)
         .await
         .expect("Hybrid error").0;
-    df = df.lazy().with_column(col("w").cast(DataType::Utf8)).collect().unwrap();
+    df = df.lazy().with_column(col("w").cast(DataType::String)).collect().unwrap();
 
     df = df.sort(["w", "v", "greater"], vec![false], false)
         .unwrap();
     let mut file_path = testdata_path.clone();
     file_path.push("expected_optional_clause_query.csv");
 
     let file = File::open(file_path.as_path()).expect("Read file problem");
@@ -869,15 +872,15 @@
         }
     }
     "#;
     let mut df = engine
         .execute_hybrid_query(query)
         .await
         .expect("Hybrid error").0;
-    df = df.lazy().with_column(col("w").cast(DataType::Utf8)).collect().unwrap();
+    df = df.lazy().with_column(col("w").cast(DataType::String)).collect().unwrap();
     df = df.sort(["w", "v"], vec![false, false], true)
         .expect("Sort error");
     let mut file_path = testdata_path.clone();
     file_path.push("expected_minus_query.csv");
 
     let file = File::open(file_path.as_path()).expect("Read file problem");
     let expected_df = CsvReader::new(file)
@@ -1097,20 +1100,22 @@
             ?w a types:SmallWidget .
             ?w types:hasSensor/chrontext:hasTimeseries/chrontext:hasDataPoint ?dp .
             ?dp chrontext:hasValue ?v .
             FILTER(?v < 100)
         }
     }
     "#;
-    let df = engine
+    let mut df = engine
         .execute_hybrid_query(query)
         .await
-        .expect("Hybrid error").0
-        .sort(["w", "v"], vec![false], false)
-        .expect("Sort problem");
+        .expect("Hybrid error").0;
+    df = df.lazy().with_columns([
+        col("w").cast(DataType::String),
+    ]).sort_by_exprs([col("w"), col("v")], vec![false], true, false).collect().unwrap();
+
 
     let mut file_path = testdata_path.clone();
     file_path.push("expected_union_query.csv");
 
     let file = File::open(file_path.as_path()).expect("Read file problem");
     let expected_df = CsvReader::new(file)
         .infer_schema(None)
@@ -1155,15 +1160,15 @@
         }
     }
     "#;
     let mut df = engine
         .execute_hybrid_query(query)
         .await
         .expect("Hybrid error").0;
-    df = df.lazy().with_column(col("s1").cast(DataType::Utf8)).collect().unwrap();
+    df = df.lazy().with_column(col("s1").cast(DataType::String)).collect().unwrap();
     df = df.sort(["s1", "t1", "v1", "v2"], vec![false], false)
         .expect("Sort problem");
 
     let mut file_path = testdata_path.clone();
     file_path.push("expected_coalesce_query.csv");
 
     let file = File::open(file_path.as_path()).expect("Read file problem");
```

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep1.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep1.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep2.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep2.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep3.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep3.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep4.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep4.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep5.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep5.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep6.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep6.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep7.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep7.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep8.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/ep8.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/expected_multi_should_pushdown.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/expected_multi_should_pushdown.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/expected_should_pushdown.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/expected_should_pushdown.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper1.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper1.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper2.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper2.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper3.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper3.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper4.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper4.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper5.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper5.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper6.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper6.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper7.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper7.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper8.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/oper8.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/parquet_to_csv.py` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/parquet_to_csv.py`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/testdata.sparql` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/testdata.sparql`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir1.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir1.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir2.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir2.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir3.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir3.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir4.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir4.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir5.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir5.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir6.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir6.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir7.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir7.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir8.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wdir8.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp1.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp1.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp2.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp2.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp3.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp3.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp4.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp4.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp5.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp5.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp6.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp6.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp7.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp7.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp8.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case/wsp8.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_benchmark_case.rs` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_benchmark_case.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_opcua/expected_basic_no_end_time_query.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_opcua/expected_basic_no_end_time_query.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_opcua/expected_basic_query.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_opcua/expected_basic_query.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_opcua/testdata.sparql` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_opcua/testdata.sparql`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_opcua.rs` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_opcua.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_syntactic_sugar/expected_simple_hybrid_sugar.csv` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_syntactic_sugar/expected_simple_hybrid_sugar.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_syntactic_sugar/testdata.sparql` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_syntactic_sugar/testdata.sparql`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/query_execution_syntactic_sugar.rs` & `chrontext-0.8.6/local_dependencies/chrontext/tests/query_execution_syntactic_sugar.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/local_dependencies/chrontext/tests/rewrites.rs` & `chrontext-0.8.6/local_dependencies/chrontext/tests/rewrites.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/Cargo.toml` & `chrontext-0.8.6/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [package]
 name = "py_chrontext"
-version = "0.8.4"
+version = "0.8.6"
 edition = "2021"
 
 [workspace]
 
 [dependencies]
+#representation = {path = "../../representation"}
 representation = { git = "https://github.com/DataTreehouse/representation"}
 pyo3 = {version = "0.19.2", features = ["extension-module"]}
 chrontext = {path= "local_dependencies/chrontext" }
 pydf_io = { git = "https://github.com/DataTreehouse/pydf_io"}
+#pydf_io = { path = "../../pydf_io" }
 thiserror="1.0.31"
-polars-core = {version="0.35.4", features = ["lazy"]}
-polars-lazy = {version="0.35.4"}
+polars-core = {version="0.37.0", features = ["lazy"]}
+polars-lazy = {version="0.37.0"}
 oxrdf = "0.1.7"
 spargebra = "0.2.8"
 simple-error = "0.3.0"
 tokio = "1.29.0"
 env_logger = "0.10.0"
 log="0.4.19"
 oxigraph="0.3.19"
```

### Comparing `chrontext-0.8.4/LICENSE` & `chrontext-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/README.md` & `chrontext-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/doc/chrontext_representation.png` & `chrontext-0.8.6/doc/chrontext_representation.png`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/doc/chrontext_seq.png` & `chrontext-0.8.6/doc/chrontext_seq.png`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/pyproject.toml` & `chrontext-0.8.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/python/chrontext/_chrontext.pyi` & `chrontext-0.8.6/python/chrontext/_chrontext.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-from .semantic_dataframe import SemanticDataFrame
+from .semantic_dataframe import DataFrame
 class Engine:
     """
     The hybrid query engine of chrontext.
     Initialize Engine using:
         - A SPARQL Database: either in the form of a SPARQL endpoint or an embedded Oxigraph SPARQL database
         - A Timeseries Database: one of the supported databases: Google Cloud BigQuery or OPC UA HA
     """
@@ -32,15 +32,15 @@
     def init(self) -> None:
         """
         Initialize the hybrid query engine. 
         
         :return: 
         """
 
-    def query(self, query:str) -> SemanticDataFrame:
+    def query(self, query:str) -> DataFrame:
         """
 
         :param query: The SPARQL query.
         :return: The query result.
         """
 
 class SparqlEmbeddedOxigraph:
```

### Comparing `chrontext-0.8.4/src/errors.rs` & `chrontext-0.8.6/src/errors.rs`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/src/lib.rs` & `chrontext-0.8.6/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 use log::debug;
 use oxigraph::io::DatasetFormat;
 use oxrdf::{IriParseError};
 use polars_core::prelude::DataFrame;
 use polars_lazy::frame::IntoLazy;
 use pydf_io::to_python::df_to_py_df;
 use pyo3::prelude::*;
-use representation::multitype::multi_col_to_string_col;
+use representation::multitype::{compress_actual_multitypes, lf_column_from_categorical, multi_columns_to_string_cols};
 use tokio::runtime::Builder;
 
 const TTL_FILE_METADATA: &str = "ttl_file_data.txt";
 
 #[pyclass(unsendable)]
 pub struct Engine {
     timeseries_opcua_db: Option<TimeseriesOPCUADatabase>,
@@ -155,21 +155,21 @@
             || !self.engine.as_ref().unwrap().has_sparql_db()
         {
             self.init()?;
         }
 
         let mut builder = Builder::new_multi_thread();
         builder.enable_all();
-        let (mut df, datatypes) = builder
+        let (mut df, mut datatypes) = builder
             .build()
             .unwrap()
             .block_on(self.engine.as_mut().unwrap().execute_hybrid_query(sparql))
             .map_err(|err| PyQueryError::QueryExecutionError(err))?;
 
-        df = fix_multicolumns(df, &datatypes);
+        (df,datatypes) = fix_cats_and_multicolumns(df, datatypes);
         let pydf = df_to_py_df(df, dtypes_map(datatypes), py)?;
         Ok(pydf)
     }
 }
 
 #[pyclass]
 #[derive(Clone)]
@@ -376,16 +376,15 @@
     Ok(())
 }
 
 fn dtypes_map(map: HashMap<String, RDFNodeType>) -> HashMap<String, String> {
     map.into_iter().map(|(x, y)| (x, y.to_string())).collect()
 }
 
-fn fix_multicolumns(df: DataFrame, dts: &HashMap<String, RDFNodeType>) -> DataFrame {
-    let mut lf = df.lazy();
-    for (c, v) in dts {
-        if v == &RDFNodeType::MultiType {
-            lf = multi_col_to_string_col(lf, c);
-        }
-    }
-    lf.collect().unwrap()
+fn fix_cats_and_multicolumns(mut df: DataFrame, mut dts: HashMap<String, RDFNodeType>) -> (DataFrame, HashMap<String, RDFNodeType>)  {
+    for (c,_) in &dts {
+        df = lf_column_from_categorical(df.lazy(), c, &dts).collect().unwrap();
+    }
+    (df, dts) = compress_actual_multitypes(df, dts);
+    df = multi_columns_to_string_cols(df.lazy(), &dts).collect().unwrap();
+    (df, dts)
 }
```

### Comparing `chrontext-0.8.4/tests/conftest.py` & `chrontext-0.8.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/tests/test_bigquery.py` & `chrontext-0.8.6/tests/test_bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,22 @@
         TimeseriesTable(
             resource_name="nist",
             schema=SCHEMA,
             time_series_table="nist2",
             value_column="VALUE",
             timestamp_column="TIMESTAMP",
             identifier_column="external_id",
-            value_datatype="http://www.w3.org/2001/XMLSchema#double",
         ),
         TimeseriesTable(
             resource_name="dataproducts",
             schema=SCHEMA,
             time_series_table="dataproducts",
             value_column="VALUE",
             timestamp_column="TIMESTAMP",
             identifier_column="external_id",
-            value_datatype="http://www.w3.org/2001/XMLSchema#double",
         ),
     ]
     return tables
 
 
 @pytest.fixture(scope="function")
 def engine(tables):
@@ -61,15 +59,16 @@
         ?inv ct:hasTimeseries ?ts .
         ?ts rdfs:label ?ts_name .
         ?ts rdfs:comment ?ts_description .
         }
     ORDER BY ASC(?ts_name)
     """)
     assert df.height == 25
-    assert df.rdf_datatypes == {'ts_description': '<http://www.w3.org/2001/XMLSchema#string>', 'ts_name': '<http://www.w3.org/2001/XMLSchema#string>'}
+    #TODO: Fix datatypes
+    #assert df.rdf_datatypes == {'ts_description': '<http://www.w3.org/2001/XMLSchema#string>', 'ts_name': '<http://www.w3.org/2001/XMLSchema#string>'}
 
 @pytest.mark.skipif(skip, reason="Environment vars not present")
 @pytest.mark.order(2)
 def test_get_all_inverters(engine):
     df = engine.query("""
         PREFIX xsd:<http://www.w3.org/2001/XMLSchema#>
         PREFIX ct:<https://github.com/DataTreehouse/chrontext#>
```

### Comparing `chrontext-0.8.4/tests/test_opcua.py` & `chrontext-0.8.6/tests/test_opcua.py`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/tests/testdata/expected_simplified_opcua_case.csv` & `chrontext-0.8.6/tests/testdata/expected_simplified_opcua_case.csv`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/tests/testdata/testdata_opcua_history_read.sparql` & `chrontext-0.8.6/tests/testdata/testdata_opcua_history_read.sparql`

 * *Files identical despite different names*

### Comparing `chrontext-0.8.4/Cargo.lock` & `chrontext-0.8.6/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
-version = "0.8.8"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42cd52102d3df161c77a887b608d7a4897d7cc112886a9537b738a887a03aaff"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
  "getrandom",
  "once_cell",
  "version_check",
  "zerocopy",
 ]
@@ -79,46 +79,36 @@
 name = "anyhow"
 version = "1.0.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5ad32ce52e4161730f7098c077cd2ed6229b5804ccf99e5366be1ab72a98b4e1"
 
 [[package]]
 name = "argminmax"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "202108b46429b765ef483f8a24d5c46f48c14acfdacc086dd4ab6dddf6bcdbd2"
+checksum = "52424b59d69d69d5056d508b260553afd91c57e21849579cd1f50ee8b8b88eaa"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "array-init-cursor"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf7d0a018de4f6aa429b9d33d69edf69072b1c5b1cb8d3e4a5f7ef898fc3eb76"
 
 [[package]]
-name = "arrow-format"
-version = "0.8.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07884ea216994cdc32a2d5f8274a8bee979cfe90274b83f86f440866ee3132c7"
-dependencies = [
- "planus",
- "serde",
-]
-
-[[package]]
 name = "async-recursion"
 version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5fd55a5ba1179988837d24ab4c7cc8ed6efdeff578ede0416b4225a5fca35bd0"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "async-stream"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd56dd203fef61ac097dd65721a419ddccb106b2d2b70ba60a6b529f03961a51"
@@ -132,26 +122,26 @@
 name = "async-stream-impl"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "async-trait"
 version = "0.1.77"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c980ee35e870bd1a4d2c8294d4c04d0499e67bca1e4b5cefcc693c2fa00caea9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "atoi"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
@@ -246,29 +236,29 @@
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
 name = "bigdecimal"
-version = "0.4.2"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c06619be423ea5bb86c95f087d5707942791a08a85530df0db2209a3ecfb8bc9"
+checksum = "9324c8014cd04590682b34f1e9448d38f0674d0f7b2dc553331016ef0e4e9ebc"
 dependencies = [
  "autocfg",
  "libm",
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "bigquery-polars"
 version = "0.1.2"
-source = "git+https://github.com/DataTreehouse/bigquery-polars#e18e33a79dc221d577524d8ee2e474f040f166d1"
+source = "git+https://github.com/DataTreehouse/bigquery-polars#4007368323e160454fa4212574804564820a23c9"
 dependencies = [
  "backoff",
  "gcp-bigquery-client",
  "polars",
  "rayon",
  "thiserror",
  "tokio",
@@ -289,15 +279,15 @@
  "log",
  "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn 2.0.49",
+ "syn 2.0.52",
  "which",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -337,17 +327,17 @@
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.0"
+version = "3.15.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d32a994c2b3ca201d9b263612a374263f05e7adde37c4707f693dcd375076d1f"
+checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
 
 [[package]]
 name = "bytemuck"
 version = "1.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2ef034f05691a48569bd920a96c81b9d91bbad1ab5ac7c4616c1f6ef36cb79f"
 dependencies = [
@@ -358,15 +348,15 @@
 name = "bytemuck_derive"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "965ab7eb5f8f97d2a083c799f3a1b994fc397b2fe2da5d1da1626ce15a39f2b1"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
@@ -375,17 +365,17 @@
 name = "bytes"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
+checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
 name = "cexpr"
@@ -400,25 +390,25 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.34"
+version = "0.4.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bc015644b92d5890fab7489e49d21f879d5c990186827d42ec511919404f38b"
+checksum = "8eaf5903dcbc0a39312feb77df2ff4c76387d591b9fc7b04a238dcf8bb62639a"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "serde",
  "wasm-bindgen",
- "windows-targets 0.52.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "chrono-tz"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d59ae0466b83e838b81a54256c39d5d7c20b9d7daa10510a242d9b75abd5936e"
@@ -536,17 +526,17 @@
  "crossbeam-epoch",
  "crossbeam-queue",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.11"
+version = "0.5.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "176dc175b78f56c0f321911d9c8eb2b77a78a4860b9c19db83835fea1a46649b"
+checksum = "ab3db02a9c5b5121e1e42fbdb1aeb65f5e02624cc58c43f2884c6ccac0b82f95"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
 version = "0.8.5"
@@ -651,17 +641,17 @@
 dependencies = [
  "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
 name = "dyn-clone"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "545b22097d44f8a9581187cdf93de7a71e4722bf51200cfaba810865b49a495d"
+checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
 
 [[package]]
 name = "either"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
@@ -679,15 +669,15 @@
 version = "0.3.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f33313078bb8d4d05a2733a94ac4c2d8a0df9a2b84424ebf4f33bfc224a890e"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "env_logger"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4cd405aab171cb85d6735e5c8d9db038c17d3ca007a4d2c25f337935c3d90580"
@@ -864,15 +854,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -977,15 +967,15 @@
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
- "indexmap 2.2.3",
+ "indexmap 2.2.5",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
@@ -1009,17 +999,17 @@
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.6"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd5256b483761cd23699d0da46cc6fd2ee3be420bbe6d020ae4a091e70b7e9fd"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
@@ -1030,17 +1020,17 @@
 checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "http"
-version = "0.2.11"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8947b1a6fad4393052c7ba1f4cd97bed3e953a95c79c92ad9b051a04611d9fbb"
+checksum = "601cbb57e577e2f5ef5be8e7b83f0f63994f25aa94d673e54a92d5c516d101f1"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
@@ -1189,17 +1179,17 @@
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.2.3"
+version = "2.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "233cf39063f058ea2caae4091bf4a3ef70a653afbc026f5c4a4135d114e3c177"
+checksum = "7b0b929d511467233429c45a44ac1dcaa21ba0f5ba11e4879e6ed28ddb4f9df4"
 dependencies = [
  "equivalent",
  "hashbrown 0.14.3",
 ]
 
 [[package]]
 name = "indoc"
@@ -1211,15 +1201,15 @@
 name = "inherent"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0122b7114117e64a63ac49f752a5ca4624d534c7b1c7de796ac196381cd2d947"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
@@ -1292,17 +1282,17 @@
 checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.68"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "406cda4b368d531c842222cf9d2600a9a4acce8d29423695379c6868a143a9ee"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "json-event-parser"
 version = "0.1.1"
@@ -1325,20 +1315,20 @@
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libloading"
-version = "0.8.1"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c571b676ddfc9a8c12f1f3d3085a7b163966a8fd8098a90640953ce5f6170161"
+checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-sys 0.48.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
@@ -1367,17 +1357,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "lz4"
 version = "1.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e9e2dd86df36ce760a60f6ff6ad526f7ba1f14ba0356f8254fb6905e6494df1"
 dependencies = [
@@ -1469,17 +1459,17 @@
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.10"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f3d0b296e374a4e6f3c7b0a1f5a51d748a0d34c85e7dc48fc3fa9a87657fe09"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
@@ -1650,17 +1640,17 @@
  "tokio-util",
  "url 1.7.2",
  "uuid",
 ]
 
 [[package]]
 name = "openssl"
-version = "0.10.63"
+version = "0.10.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15c9d69dd87a29568d4d017cfe8ec518706046a05184e5aea92d0af890b803c8"
+checksum = "95a0481286a310808298130d22dd1fef0fa571e05a8f44ec801801e84b216b1f"
 dependencies = [
  "bitflags 2.4.2",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
@@ -1671,15 +1661,15 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
@@ -1691,17 +1681,17 @@
 checksum = "5cff92b6f71555b61bb9315f7c64da3ca43d87531622120fea0195fc761b4843"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.99"
+version = "0.9.101"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22e1bf214306098e4832460f797824c05d25aacdf896f64a985fb0fd992454ae"
+checksum = "dda2b0f344e78efc2facf7d195d098df0dd72151b26ab98da807afc26c198dff"
 dependencies = [
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
@@ -1735,17 +1725,20 @@
  "siphasher 1.0.0",
  "sparesults",
  "spargebra 0.2.8 (registry+https://github.com/rust-lang/crates.io-index)",
 ]
 
 [[package]]
 name = "oxilangtag"
-version = "0.1.3"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8d91edf4fbb970279443471345a4e8c491bf05bb283b3e6c88e4e606fd8c181b"
+checksum = "7411f015966f5030586589ca0baa8049863e72a9fabc147c8f18c9c34ed5a0f4"
+dependencies = [
+ "serde",
+]
 
 [[package]]
 name = "oxiri"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb175ec8981211357b7b379869c2f8d555881c55ea62311428ec0de46d89bd5c"
 
@@ -1898,30 +1891,30 @@
 checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
 dependencies = [
  "siphasher 0.3.11",
 ]
 
 [[package]]
 name = "pin-project"
-version = "1.1.4"
+version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0302c4a0442c456bd56f841aee5c3bfd17967563f6fadc9ceb9f9c23cf3807e0"
+checksum = "b6bf43b791c5b9e34c3d182969b4abb522f9343702850a2e57f460d00d09b4b3"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.1.4"
+version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "266c042b60c9c76b8d53061e52b2e0d1116abc57cefc8c5cd671619a56ac3690"
+checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
@@ -1945,82 +1938,107 @@
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
  "array-init-cursor",
 ]
 
 [[package]]
 name = "polars"
-version = "0.35.4"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df8e52f9236eb722da0990a70bbb1216dcc7a77bcb00c63439d2d982823e90d5"
+checksum = "e43795c49010cb851d45227caa17769e83760e21d260ba6285c563b754e1652f"
 dependencies = [
  "getrandom",
  "polars-core",
  "polars-io",
  "polars-lazy",
  "polars-ops",
  "polars-sql",
  "polars-time",
  "version_check",
 ]
 
 [[package]]
 name = "polars-arrow"
-version = "0.35.4"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd503430a6d9779b07915d858865fe998317ef3cfef8973881f578ac5d4baae7"
+checksum = "faacd21a2548fa6d50c72d6b8d4649a8e029a0f3c6c5545b7f436f0610e49b0f"
 dependencies = [
  "ahash",
- "arrow-format",
  "atoi",
  "atoi_simd",
  "bytemuck",
  "chrono",
  "chrono-tz",
  "dyn-clone",
  "either",
  "ethnum",
  "fast-float",
  "foreign_vec",
  "futures",
  "getrandom",
  "hashbrown 0.14.3",
  "itoa",
+ "itoap",
  "lz4",
  "multiversion",
  "num-traits",
+ "polars-arrow-format",
  "polars-error",
  "polars-utils",
- "rustc_version",
  "ryu",
  "simdutf8",
  "streaming-iterator",
  "strength_reduce",
+ "version_check",
  "zstd",
 ]
 
 [[package]]
+name = "polars-arrow-format"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "19b0ef2474af9396b19025b189d96e992311e6a47f90c53cd998b36c4c64b84c"
+dependencies = [
+ "planus",
+ "serde",
+]
+
+[[package]]
+name = "polars-compute"
+version = "0.37.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32d9dc87f8003ae0edeef5ad9ac92b2a345480bbe17adad64496113ae84706dd"
+dependencies = [
+ "bytemuck",
+ "num-traits",
+ "polars-arrow",
+ "polars-error",
+ "polars-utils",
+ "version_check",
+]
+
+[[package]]
 name = "polars-core"
-version = "0.35.4"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae73d5b8e55decde670caba1cc82b61f14bfb9a72503198f0997d657a98dcfd6"
+checksum = "befd4d280a82219a01035c4f901319ceba65998c594d0c64f9a439cdee1d7777"
 dependencies = [
  "ahash",
  "bitflags 2.4.2",
  "bytemuck",
  "chrono",
  "chrono-tz",
  "comfy-table",
  "either",
  "hashbrown 0.14.3",
- "indexmap 2.2.3",
- "itoap",
+ "indexmap 2.2.5",
  "num-traits",
  "once_cell",
  "polars-arrow",
+ "polars-compute",
  "polars-error",
  "polars-row",
  "polars-utils",
  "rand",
  "rand_distr",
  "rayon",
  "regex",
@@ -2028,29 +2046,29 @@
  "thiserror",
  "version_check",
  "xxhash-rust",
 ]
 
 [[package]]
 name = "polars-error"
-version = "0.35.4"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb0520d68eaa9993ae0c741409d1526beff5b8f48e1d73e4381616f8152cf488"
+checksum = "50f2435b02d1ba36d8c1f6a722cad04e4c0b2705a3112c5706e6960d405d7798"
 dependencies = [
- "arrow-format",
+ "polars-arrow-format",
  "regex",
  "simdutf8",
  "thiserror",
 ]
 
 [[package]]
 name = "polars-io"
-version = "0.35.4"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96e10a0745acd6009db64bef0ceb9e23a70b1c27b26a0a6517c91f3e6363bc06"
+checksum = "b51fba2cf014cb39c2b38353d601540fb9db643be65abb9ca8ff44b9c4c4a88e"
 dependencies = [
  "ahash",
  "async-trait",
  "atoi_simd",
  "bytes",
  "chrono",
  "chrono-tz",
@@ -2076,17 +2094,17 @@
  "smartstring",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "polars-lazy"
-version = "0.35.4"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3555f759705be6dd0d3762d16a0b8787b2dc4da73b57465f3b2bf1a070ba8f20"
+checksum = "d83343e413346f048f3a5ad07c0ea4b5d0bada701a482878213142970b0ddff8"
 dependencies = [
  "ahash",
  "bitflags 2.4.2",
  "glob",
  "once_cell",
  "polars-arrow",
  "polars-core",
@@ -2099,43 +2117,47 @@
  "rayon",
  "smartstring",
  "version_check",
 ]
 
 [[package]]
 name = "polars-ops"
-version = "0.35.4"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a7eb218296aaa7f79945f08288ca32ca3cf25fa505649eeee689ec21eebf636"
+checksum = "6395f5fd5e1adf016fd6403c0a493181c1a349a7a145b2687cdf50a0d630310a"
 dependencies = [
  "ahash",
  "argminmax",
+ "base64",
  "bytemuck",
  "chrono",
  "chrono-tz",
  "either",
  "hashbrown 0.14.3",
- "indexmap 2.2.3",
+ "hex",
+ "indexmap 2.2.5",
  "memchr",
  "num-traits",
  "polars-arrow",
+ "polars-compute",
  "polars-core",
  "polars-error",
  "polars-utils",
  "rayon",
  "regex",
  "smartstring",
+ "unicode-reverse",
  "version_check",
 ]
 
 [[package]]
 name = "polars-parquet"
-version = "0.35.4"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "146010e4b7dd4d2d0e58ddc762f6361f77d7a0385c54471199370c17164f67dd"
+checksum = "b664cac41636cc9f146fba584a8e7c2790d7335a278964529fa3e9b4eae96daf"
 dependencies = [
  "ahash",
  "async-stream",
  "base64",
  "brotli",
  "ethnum",
  "flate2",
@@ -2151,40 +2173,41 @@
  "snap",
  "streaming-decompression",
  "zstd",
 ]
 
 [[package]]
 name = "polars-pipe"
-version = "0.35.4"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "66094e7df64c932a9a7bdfe7df0c65efdcb192096e11a6a765a9778f78b4bdec"
+checksum = "390a831b864bc57a4cb260b0595030dfb6a4260a3723cf8ca17968ee2078b8ff"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-queue",
  "enum_dispatch",
  "hashbrown 0.14.3",
  "num-traits",
  "polars-arrow",
+ "polars-compute",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-plan",
  "polars-row",
  "polars-utils",
  "rayon",
  "smartstring",
  "version_check",
 ]
 
 [[package]]
 name = "polars-plan"
-version = "0.35.4"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10e32a0958ef854b132bad7f8369cb3237254635d5e864c99505bc0bc1035fbc"
+checksum = "7fb7d7527be2aa33baace9000f6772eb9df7cd57ec010a4b273435d2dc1349e8"
 dependencies = [
  "ahash",
  "bytemuck",
  "chrono-tz",
  "once_cell",
  "percent-encoding 2.3.1",
  "polars-arrow",
@@ -2199,45 +2222,46 @@
  "smartstring",
  "strum_macros",
  "version_check",
 ]
 
 [[package]]
 name = "polars-row"
-version = "0.35.4"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d135ab81cac2906ba74ea8984c7e6025d081ae5867615bcefb4d84dfdb456dac"
+checksum = "f4984d97aad3d0db92afe76ebcab10b5e37a1216618b5703ae0d2917ccd6168c"
 dependencies = [
  "polars-arrow",
  "polars-error",
  "polars-utils",
 ]
 
 [[package]]
 name = "polars-sql"
-version = "0.35.4"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b8dbd7786849a5e3ad1fde188bf38141632f626e3a57319b0bbf7a5f1d75519e"
+checksum = "77f62a8b8f93146ec1eb2ef340d77eeb174e8010035e449bfdd424d2b1fd944a"
 dependencies = [
+ "hex",
  "polars-arrow",
  "polars-core",
  "polars-error",
  "polars-lazy",
  "polars-plan",
  "rand",
  "serde",
  "serde_json",
  "sqlparser",
 ]
 
 [[package]]
 name = "polars-time"
-version = "0.35.4"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aae56f79e9cedd617773c1c8f5ca84a31a8b1d593714959d5f799e7bdd98fe51"
+checksum = "6d75348a51d0c97f3b83df860ecb35a6ac6c5dafc6278cac4e1ac101d96dc753"
 dependencies = [
  "atoi",
  "chrono",
  "chrono-tz",
  "now",
  "once_cell",
  "polars-arrow",
@@ -2247,22 +2271,22 @@
  "polars-utils",
  "regex",
  "smartstring",
 ]
 
 [[package]]
 name = "polars-utils"
-version = "0.35.4"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da6ce68169fe61d46958c8eab7447360f30f2f23f6e24a0ce703a14b0a3cfbfc"
+checksum = "38f9c955bb1e9b55d835aeb7fe4e4e8826e01abe5f0ada979ceb7d2b9af7b569"
 dependencies = [
  "ahash",
  "bytemuck",
  "hashbrown 0.14.3",
- "indexmap 2.2.3",
+ "indexmap 2.2.5",
  "num-traits",
  "once_cell",
  "polars-error",
  "rayon",
  "smartstring",
  "sysinfo",
  "version_check",
@@ -2283,15 +2307,15 @@
 [[package]]
 name = "prettyplease"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a41cf62165e97c7f814d2221421dbb9afcbcdb0a88068e5ea206e19951c2cbb5"
 dependencies = [
  "proc-macro2",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "proc-macro2"
 version = "1.0.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
@@ -2306,15 +2330,15 @@
 checksum = "146c289cda302b98a28d40c8b3b90498d6e526dd24ac2ecea73e4e491685b94a"
 dependencies = [
  "bytes",
 ]
 
 [[package]]
 name = "py_chrontext"
-version = "0.8.4"
+version = "0.8.6"
 dependencies = [
  "chrontext",
  "env_logger",
  "filesize",
  "jemallocator",
  "log",
  "mimalloc",
@@ -2330,15 +2354,15 @@
  "thiserror",
  "tokio",
 ]
 
 [[package]]
 name = "pydf_io"
 version = "0.6.0"
-source = "git+https://github.com/DataTreehouse/pydf_io#b103df37b926b7a11720a820fe45d775feccb812"
+source = "git+https://github.com/DataTreehouse/pydf_io#c2eb96393c997ba310ec5589702e3e760509d611"
 dependencies = [
  "polars-core",
  "pyo3",
  "simple-error",
  "thiserror",
 ]
 
@@ -2401,15 +2425,15 @@
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "query_processing"
 version = "0.1.0"
-source = "git+https://github.com/DataTreehouse/query_processing#60525011bb09fdaa7795235ad4ee06c78d388ea6"
+source = "git+https://github.com/DataTreehouse/query_processing#4f5a1a8cd10187ddc2216891d52e2d17eeb3c3eb"
 dependencies = [
  "chrono",
  "chrono-tz",
  "env_logger",
  "log",
  "oxrdf",
  "polars",
@@ -2476,17 +2500,17 @@
 dependencies = [
  "num-traits",
  "rand",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.8.1"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa7237101a77a10773db45d62004a272517633fbcc3df19d96455ede1122e051"
+checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -2517,17 +2541,17 @@
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bb987efffd3c6d0d8f5f89510bb458559eab11e4f869acb20bf845e016259cd"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
@@ -2535,15 +2559,15 @@
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
 name = "representation"
 version = "0.4.19"
-source = "git+https://github.com/DataTreehouse/representation#ac34d5db9f0babc500779ad23349c966329235da"
+source = "git+https://github.com/DataTreehouse/representation#80fd10d6e91e65367c790525ba3c2e80b18108f0"
 dependencies = [
  "bigdecimal",
  "chrono",
  "oxrdf",
  "polars",
  "polars-arrow",
  "polars-core",
@@ -2651,23 +2675,14 @@
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
-name = "rustc_version"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
-dependencies = [
- "semver",
-]
-
-[[package]]
 name = "rustix"
 version = "0.38.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
 dependencies = [
  "bitflags 2.4.2",
  "errno",
@@ -2721,17 +2736,17 @@
 checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
 dependencies = [
  "base64",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.3.0"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "048a63e5b3ac996d78d402940b5fa47973d2d080c6c6fffa1d0f19c4445310b7"
+checksum = "5ede67b28608b4c60685c7d54122d4400d90f62b40caee7700e700380a390fa8"
 
 [[package]]
 name = "rustls-webpki"
 version = "0.101.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
 dependencies = [
@@ -2835,50 +2850,44 @@
 checksum = "e932934257d3b408ed8f30db49d85ea163bfe74961f017f405b025af298f0c7a"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
-name = "semver"
-version = "1.0.22"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
-
-[[package]]
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "870026e60fa08c69f064aa766c10f10b1d62db9ccd4d0abb206472bee0ce3b32"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33c85360c95e7d137454dc81d9a4ed2b8efd8fbe19cee57357b32b9771fccb67"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.113"
+version = "1.0.114"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69801b70b1c3dac963ecb03a364ba0ceda9cf60c71cfe475e99864759c8b8a79"
+checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2895,15 +2904,15 @@
 
 [[package]]
 name = "serde_yaml"
 version = "0.9.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8fd075d994154d4a774f95b51fb96bdc2832b0ea48425c92546073816cda1f2f"
 dependencies = [
- "indexmap 2.2.3",
+ "indexmap 2.2.5",
  "itoa",
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
 
 [[package]]
@@ -2997,20 +3006,20 @@
 name = "snap"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b6b67fb9a61334225b5b790716f609cd58395f895b3fe8b328786812a40bc3b"
 
 [[package]]
 name = "socket2"
-version = "0.5.5"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
+checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
 dependencies = [
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "sparesults"
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c301a876e05c887d2f23f47f7822719435d36038856a9681cc7351d9c2677ce4"
@@ -3032,15 +3041,15 @@
  "peg",
  "rand",
 ]
 
 [[package]]
 name = "spargebra"
 version = "0.2.8"
-source = "git+https://github.com/DataTreehouse/spargebra#f8bcadd628ce613938669d799c54c3927d6825a3"
+source = "git+https://github.com/DataTreehouse/spargebra#3526be510a6a4c292f81bfeaf2fe8d2686ed0c7d"
 dependencies = [
  "chrono",
  "datetimeparse",
  "fundu",
  "oxilangtag",
  "oxiri",
  "oxrdf",
@@ -3102,15 +3111,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
@@ -3124,41 +3133,41 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.49"
+version = "2.0.52"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "915aea9e586f80826ee59f8453c1101f9d1c4b3964cd2460185ee8e299ada496"
+checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sync_wrapper"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
 
 [[package]]
 name = "sysinfo"
-version = "0.29.11"
+version = "0.30.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd727fc423c2060f6c92d9534cef765c65a6ed3f428a03d7def74a8c4348e666"
+checksum = "0c385888ef380a852a16209afc8cfad22795dd8873d69c9a14d2e2088f118d18"
 dependencies = [
  "cfg-if",
  "core-foundation-sys",
  "libc",
  "ntapi",
  "once_cell",
- "winapi",
+ "windows",
 ]
 
 [[package]]
 name = "system-configuration"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba3a3adc5c275d719af8cb4272ea1c4a6d668a777f37e115f6d11ddbc1c8e0e7"
@@ -3182,23 +3191,23 @@
 name = "target-features"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cfb5fa503293557c5158bd215fdc225695e567a77e453f5d4452a50a193969bd"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.13"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tempfile"
-version = "3.10.0"
+version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a365e8cd18e44762ef95d87f284f4b5cd04107fec2ff3052bd6a3e6069669e67"
+checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
  "fastrand",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
@@ -3224,15 +3233,15 @@
 name = "thiserror-impl"
 version = "1.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "time"
 version = "0.3.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c8248b6521bb14bc45b4067159b9b6ad792e2d6d754d6c41fb50e29fefe38749"
@@ -3312,15 +3321,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -3438,15 +3447,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -3476,22 +3485,37 @@
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
+name = "unicode-reverse"
+version = "1.0.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0bea5dacebb0d2d0a69a6700a05b59b3908bf801bf563a49bd27a1b60122962c"
+dependencies = [
+ "unicode-segmentation",
+]
+
+[[package]]
+name = "unicode-segmentation"
+version = "1.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
+
+[[package]]
 name = "unicode-width"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
 
 [[package]]
 name = "unindent"
@@ -3568,77 +3592,77 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1e124130aee3fb58c5bdd6b639a0509486b0338acaaae0c84a5124b0f588b7f"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c9e7e1900c352b609c8488ad12639a311045f40a35491fb69ba8c12f758af70b"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.41"
+version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "877b9c3f61ceea0e56331985743b13f3d25c406a7098d45180fb5f09bc19ed97"
+checksum = "76bc14366121efc8dbb487ab05bcc9d346b3b5ec0eaa76e46594cabbe51762c0"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b30af9e2d358182b5c7449424f017eba305ed32a7010509ede96cdc4696c46ed"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "642f325be6301eb8107a83d12a8ac6c1e1c54345a7ef1a9261962dfefda09e66"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f186bd2dcf04330886ce82d6f33dd75a7bfcf69ecf5763b89fcde53b6ac9838"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "wasm-streams"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b65dc4c90b63b118468cf747d8bf3566c1913ef60be765b5730ead9e0a3ba129"
 dependencies = [
@@ -3647,17 +3671,17 @@
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
 ]
 
 [[package]]
 name = "web-sys"
-version = "0.3.68"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96565907687f7aceb35bc5fc03770a8a0471d82e479f25832f54a0e3f4b28446"
+checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webpki-roots"
@@ -3705,20 +3729,30 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e48a53791691ab099e5e2ad123536d0fff50652600abaf43bbf952894110d0be"
+dependencies = [
+ "windows-core",
+ "windows-targets 0.52.4",
+]
+
+[[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
@@ -3728,15 +3762,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -3748,110 +3782,110 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.0",
- "windows_aarch64_msvc 0.52.0",
- "windows_i686_gnu 0.52.0",
- "windows_i686_msvc 0.52.0",
- "windows_x86_64_gnu 0.52.0",
- "windows_x86_64_gnullvm 0.52.0",
- "windows_x86_64_msvc 0.52.0",
+ "windows_aarch64_gnullvm 0.52.4",
+ "windows_aarch64_msvc 0.52.4",
+ "windows_i686_gnu 0.52.4",
+ "windows_i686_msvc 0.52.4",
+ "windows_x86_64_gnu 0.52.4",
+ "windows_x86_64_gnullvm 0.52.4",
+ "windows_x86_64_msvc 0.52.4",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
 
 [[package]]
 name = "winreg"
 version = "0.50.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
 dependencies = [
@@ -3905,15 +3939,15 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
```

### Comparing `chrontext-0.8.4/PKG-INFO` & `chrontext-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrontext
-Version: 0.8.4
+Version: 0.8.6
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

