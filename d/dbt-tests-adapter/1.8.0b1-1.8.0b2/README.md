# Comparing `tmp/dbt_tests_adapter-1.8.0b1.tar.gz` & `tmp/dbt_tests_adapter-1.8.0b2.tar.gz`

## Comparing `dbt_tests_adapter-1.8.0b1.tar` & `dbt_tests_adapter-1.8.0b2.tar`

### file list

```diff
@@ -1,156 +1,158 @@
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/__about__.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/aliases/fixtures.py
--rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/aliases/test_aliases.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/__init__.py
--rw-r--r--   0        0        0     7617 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/expected_catalog.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/files.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_adapter_methods.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_base.py
--rw-r--r--   0        0        0    12770 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_docs_generate.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_empty.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_ephemeral.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_generic_tests.py
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_incremental.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_singular_tests.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_snapshot_check_cols.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_snapshot_timestamp.py
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_table_materialization.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_validate_connection.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/caching/test_caching.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/catalog/files.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/catalog/relation_types.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/column_types/fixtures.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/column_types/test_column_types.py
--rw-r--r--   0        0        0    14694 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/concurrency/test_concurrency.py
--rw-r--r--   0        0        0    11094 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/constraints/fixtures.py
--rw-r--r--   0        0        0    18494 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/constraints/test_constraints.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_clone/fixtures.py
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_clone/test_dbt_clone.py
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_debug/test_dbt_debug.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_show/fixtures.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_show/test_dbt_show.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/empty/test_empty.py
--rw-r--r--   0        0        0    12159 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/ephemeral/test_ephemeral.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/base_grants.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_incremental_grants.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_invalid_grants.py
--rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_model_grants.py
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_seed_grants.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_snapshot_grants.py
--rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/fixtures.py
--rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/test_model_hooks.py
--rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/test_run_hooks.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/data/seed_model.sql
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/data/seed_run.sql
--rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/fixtures.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_predicates.py
--rw-r--r--   0        0        0    17895 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_unique_id.py
--rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/materialized_view/basic.py
--rw-r--r--   0        0        0    10573 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/materialized_view/changes.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/materialized_view/files.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/persist_docs/fixtures.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/persist_docs/test_persist_docs.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/python_model/test_python_model.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/python_model/test_spark.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/query_comment/fixtures.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/query_comment/test_query_comment.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/relations/test_changing_relation_type.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/relations/test_dropping_schema_named.py
--rw-r--r--   0        0        0    19870 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_copy/fixtures.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_copy/test_copy_uppercase.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_copy/test_simple_copy.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/fixtures.py
--rw-r--r--   0        0        0    33348 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/seed_bom.csv
--rw-r--r--   0        0        0   111485 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/seeds.py
--rw-r--r--   0        0        0    14662 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/test_seed.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/test_seed_type_override.py
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/common.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/seeds.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/snapshots.py
--rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/test_snapshot.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/_files.py
--rw-r--r--   0        0        0    13105 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/basic.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/fixtures.py
--rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/unit_testing/test_case_insensitivity.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/unit_testing/test_invalid_input.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/unit_testing/test_types.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/base_array_utils.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/base_utils.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_any_value.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_array_append.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_array_concat.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_array_construct.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_bool_or.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_cast_bool_to_text.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_concat.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_date_spine.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_date_trunc.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_dateadd.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_datediff.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_equals.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_escape_single_quotes.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_except.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_generate_series.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_get_intervals_between.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_get_powers_of_two.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_hash.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_intersect.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_last_day.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_length.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_listagg.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_null_compare.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_position.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_replace.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_right.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_safe_cast.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_split_part.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_string_literal.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_any_value.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_array_append.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_array_concat.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_array_construct.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_bool_or.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_cast_bool_to_text.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_concat.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_current_timestamp.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_date_spine.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_date_trunc.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_dateadd.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_datediff.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_equals.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_escape_single_quotes.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_except.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_generate_series.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_get_intervals_between.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_get_powers_of_two.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_hash.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_intersect.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_last_day.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_length.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_listagg.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_null_compare.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_position.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_replace.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_right.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_safe_cast.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_split_part.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_string_literal.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_timestamps.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_validate_sql.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/base_data_type_macro.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_bigint.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_boolean.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_float.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_int.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_numeric.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_string.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_timestamp.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/.gitignore
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/README.md
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/pyproject.toml
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/PKG-INFO
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/__about__.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/aliases/fixtures.py
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/aliases/test_aliases.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/__init__.py
+-rw-r--r--   0        0        0     7617 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/expected_catalog.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/files.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_adapter_methods.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_base.py
+-rw-r--r--   0        0        0    12770 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_docs_generate.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_empty.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_ephemeral.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_generic_tests.py
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_incremental.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_singular_tests.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_snapshot_check_cols.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_snapshot_timestamp.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_table_materialization.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_validate_connection.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/caching/test_caching.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/catalog/files.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/catalog/relation_types.py
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/column_types/fixtures.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/column_types/test_column_types.py
+-rw-r--r--   0        0        0    14694 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/concurrency/test_concurrency.py
+-rw-r--r--   0        0        0    11094 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/constraints/fixtures.py
+-rw-r--r--   0        0        0    18494 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/constraints/test_constraints.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/dbt_clone/fixtures.py
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/dbt_clone/test_dbt_clone.py
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/dbt_debug/test_dbt_debug.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/dbt_show/fixtures.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/dbt_show/test_dbt_show.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/empty/test_empty.py
+-rw-r--r--   0        0        0    12159 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/ephemeral/test_ephemeral.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/grants/base_grants.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/grants/test_incremental_grants.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/grants/test_invalid_grants.py
+-rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/grants/test_model_grants.py
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/grants/test_seed_grants.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/grants/test_snapshot_grants.py
+-rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/hooks/fixtures.py
+-rw-r--r--   0        0        0    16029 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/hooks/test_model_hooks.py
+-rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/hooks/test_run_hooks.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/hooks/data/seed_model.sql
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/hooks/data/seed_run.sql
+-rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/incremental/fixtures.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/incremental/test_incremental_predicates.py
+-rw-r--r--   0        0        0    17895 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/incremental/test_incremental_unique_id.py
+-rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/materialized_view/basic.py
+-rw-r--r--   0        0        0    10573 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/materialized_view/changes.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/materialized_view/files.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/persist_docs/fixtures.py
+-rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/persist_docs/test_persist_docs.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/python_model/test_python_model.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/python_model/test_spark.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/query_comment/fixtures.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/query_comment/test_query_comment.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/relations/test_changing_relation_type.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/relations/test_dropping_schema_named.py
+-rw-r--r--   0        0        0    19870 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_copy/fixtures.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_copy/test_copy_uppercase.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_copy/test_simple_copy.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_seed/fixtures.py
+-rw-r--r--   0        0        0    33348 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_seed/seed_bom.csv
+-rw-r--r--   0        0        0   111485 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_seed/seeds.py
+-rw-r--r--   0        0        0    14662 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_seed/test_seed.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_seed/test_seed_type_override.py
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_snapshot/common.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_snapshot/seeds.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_snapshot/snapshots.py
+-rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_snapshot/test_snapshot.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/store_test_failures_tests/_files.py
+-rw-r--r--   0        0        0    13105 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/store_test_failures_tests/basic.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/store_test_failures_tests/fixtures.py
+-rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/unit_testing/test_case_insensitivity.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/unit_testing/test_invalid_input.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/unit_testing/test_types.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/base_array_utils.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/base_utils.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_any_value.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_array_append.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_array_concat.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_array_construct.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_bool_or.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_cast.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_cast_bool_to_text.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_concat.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_date_spine.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_date_trunc.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_dateadd.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_datediff.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_equals.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_escape_single_quotes.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_except.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_generate_series.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_get_intervals_between.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_get_powers_of_two.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_hash.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_intersect.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_last_day.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_length.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_listagg.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_null_compare.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_position.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_replace.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_right.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_safe_cast.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_split_part.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_string_literal.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_any_value.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_array_append.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_array_concat.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_array_construct.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_bool_or.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_cast.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_cast_bool_to_text.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_concat.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_current_timestamp.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_date_spine.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_date_trunc.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_dateadd.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_datediff.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_equals.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_escape_single_quotes.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_except.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_generate_series.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_get_intervals_between.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_get_powers_of_two.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_hash.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_intersect.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_last_day.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_length.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_listagg.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_null_compare.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_position.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_replace.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_right.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_safe_cast.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_split_part.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_string_literal.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_timestamps.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_validate_sql.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/base_data_type_macro.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/test_type_bigint.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/test_type_boolean.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/test_type_float.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/test_type_int.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/test_type_numeric.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/test_type_string.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/test_type_timestamp.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/.gitignore
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/README.md
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/pyproject.toml
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b2/PKG-INFO
```

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/aliases/fixtures.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/aliases/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/aliases/test_aliases.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/aliases/test_aliases.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/expected_catalog.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/expected_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/files.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/files.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_adapter_methods.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_adapter_methods.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_base.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_base.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_docs_generate.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_docs_generate.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_empty.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_empty.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_ephemeral.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_generic_tests.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_generic_tests.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_incremental.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_incremental.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_singular_tests.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_singular_tests.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_snapshot_check_cols.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_snapshot_check_cols.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_snapshot_timestamp.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_snapshot_timestamp.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_table_materialization.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/basic/test_table_materialization.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/caching/test_caching.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/caching/test_caching.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/catalog/relation_types.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/catalog/relation_types.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/column_types/fixtures.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/column_types/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/column_types/test_column_types.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/column_types/test_column_types.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/concurrency/test_concurrency.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/concurrency/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/constraints/fixtures.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/constraints/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/constraints/test_constraints.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/constraints/test_constraints.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_clone/fixtures.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/dbt_clone/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_clone/test_dbt_clone.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/dbt_clone/test_dbt_clone.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_debug/test_dbt_debug.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/dbt_debug/test_dbt_debug.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_show/fixtures.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/dbt_show/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_show/test_dbt_show.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/dbt_show/test_dbt_show.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/empty/test_empty.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/empty/test_empty.py`

 * *Files 20% similar despite different names*

```diff
@@ -68,9 +68,28 @@
         self.assert_row_count(project, "model", 3)
 
         # run with empty - 0 expected rows in output
         run_dbt(["run", "--empty"])
         self.assert_row_count(project, "model", 0)
 
 
+class BaseTestEmptyInlineSourceRef(BaseTestEmpty):
+    @pytest.fixture(scope="class")
+    def models(self):
+        model_sql = """
+            select * from {{ source('seed_sources', 'raw_source') }} as raw_source
+            """
+
+        return {
+            "model.sql": model_sql,
+            "sources.yml": schema_sources_yml,
+        }
+
+    def test_run_with_empty(self, project):
+        # create source from seed
+        run_dbt(["seed"])
+        run_dbt(["run", "--empty", "--debug"])
+        self.assert_row_count(project, "model", 0)
+
+
 class TestEmpty(BaseTestEmpty):
     pass
```

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/ephemeral/test_ephemeral.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/ephemeral/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/base_grants.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/grants/base_grants.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_incremental_grants.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/grants/test_incremental_grants.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_invalid_grants.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/grants/test_invalid_grants.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_model_grants.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/grants/test_model_grants.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_seed_grants.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/grants/test_seed_grants.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_snapshot_grants.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/grants/test_snapshot_grants.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/fixtures.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/hooks/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/test_model_hooks.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/hooks/test_model_hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 
 from dbt_common.exceptions import CompilationError
+
 # TODO: does this belong in dbt-tests-adapter?
 from dbt.exceptions import ParsingError
 import pytest
 
 from dbt.tests.adapter.hooks import fixtures
 from dbt.tests.util import run_dbt, write_file
```

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/test_run_hooks.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/hooks/test_run_hooks.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/fixtures.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/incremental/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_predicates.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/incremental/test_incremental_predicates.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_unique_id.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/incremental/test_incremental_unique_id.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/materialized_view/basic.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/materialized_view/basic.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/materialized_view/changes.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/materialized_view/changes.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/persist_docs/fixtures.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/persist_docs/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/persist_docs/test_persist_docs.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/persist_docs/test_persist_docs.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/python_model/test_python_model.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/python_model/test_python_model.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/python_model/test_spark.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/python_model/test_spark.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/query_comment/fixtures.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/query_comment/fixtures.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 {%- endmacro -%}
 
 
 {%- macro query_header_args(message) -%}
   {%- set comment_dict = dict(
     app='dbt++',
     macro_version='0.1.0',
-    dbt_version=dbt_version,
     message='blah: '~ message) -%}
   {{ return(comment_dict) }}
 {%- endmacro -%}
 
 
 {%- macro ordered_to_json(dct) -%}
 {{ tojson(dct, sort_keys=True) }}
```

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/query_comment/test_query_comment.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/query_comment/test_query_comment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from importlib import import_module
 
 import pytest
 from dbt_common.exceptions import DbtRuntimeError
 
 from dbt.tests.adapter.query_comment import fixtures
 from dbt.tests.util import run_dbt_and_capture
 
@@ -49,27 +48,23 @@
 
     def test_matches_comment(self, project):
         logs = self.run_get_json()
         assert r"/* dbt macros\nare pretty cool */\n" in logs
 
 
 class BaseMacroArgsQueryComments(BaseDefaultQueryComments):
-    @pytest.fixture(scope="class")
-    def get_package_version(self, project):
-        return import_module("." + project.adapter_type, "dbt.adapters").__version__.version
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {"query-comment": "{{ return(ordered_to_json(query_header_args(target.name))) }}"}
 
-    def test_matches_comment(self, project, get_package_version):
+    def test_matches_comment(self, project):
         logs = self.run_get_json()
         expected_dct = {
             "app": "dbt++",
-            "dbt_version": get_package_version,
             "macro_version": "0.1.0",
             "message": f"blah: {project.adapter.config.target_name}",
         }
         expected = r"/* {} */\n".format(json.dumps(expected_dct, sort_keys=True)).replace(
             '"', r"\""
         )
         assert expected in logs
```

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/relations/test_changing_relation_type.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/relations/test_changing_relation_type.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/relations/test_dropping_schema_named.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/relations/test_dropping_schema_named.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_copy/fixtures.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_copy/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_copy/test_copy_uppercase.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_copy/test_copy_uppercase.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_copy/test_simple_copy.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_copy/test_simple_copy.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/fixtures.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_seed/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/seed_bom.csv` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_seed/seed_bom.csv`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/seeds.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_seed/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/test_seed.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_seed/test_seed.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/test_seed_type_override.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_seed/test_seed_type_override.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/common.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_snapshot/common.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/seeds.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_snapshot/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/snapshots.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_snapshot/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/test_snapshot.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/simple_snapshot/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/_files.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/store_test_failures_tests/_files.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/basic.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/store_test_failures_tests/basic.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/fixtures.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/store_test_failures_tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/unit_testing/test_case_insensitivity.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/unit_testing/test_case_insensitivity.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/unit_testing/test_invalid_input.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/unit_testing/test_invalid_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,21 +42,27 @@
             "my_upstream_model.sql": my_upstream_model_sql,
             "unit_tests.yml": test_my_model_yml,
         }
 
     def test_invalid_input(self, project):
         results = run_dbt(["run"])
         assert len(results) == 2
-        
+
         _, out = run_dbt_and_capture(
             ["test", "--select", "test_name:test_invalid_input_column_name"], expect_pass=False
         )
-        assert "Invalid column name: 'invalid_column_name' in unit test fixture for 'my_upstream_model'." in out
-        
+        assert (
+            "Invalid column name: 'invalid_column_name' in unit test fixture for 'my_upstream_model'."
+            in out
+        )
+
         _, out = run_dbt_and_capture(
             ["test", "--select", "test_name:test_invalid_expect_column_name"], expect_pass=False
         )
-        assert "Invalid column name: 'invalid_column_name' in unit test fixture for expected output." in out
+        assert (
+            "Invalid column name: 'invalid_column_name' in unit test fixture for expected output."
+            in out
+        )
 
 
 class TestPostgresUnitTestInvalidInput(BaseUnitTestInvalidInput):
     pass
```

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/unit_testing/test_types.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/unit_testing/test_types.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/base_array_utils.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/base_array_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/base_utils.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/base_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_any_value.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_any_value.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_array_concat.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_array_concat.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_bool_or.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_bool_or.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_concat.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_concat.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_date_spine.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_date_spine.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_date_trunc.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_date_trunc.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_dateadd.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_dateadd.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_datediff.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_datediff.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_equals.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_equals.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_escape_single_quotes.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_escape_single_quotes.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_except.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_except.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_generate_series.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_generate_series.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_get_intervals_between.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_get_intervals_between.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_get_powers_of_two.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_get_powers_of_two.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_hash.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_hash.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_intersect.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_intersect.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_last_day.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_last_day.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_listagg.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_listagg.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_null_compare.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_null_compare.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_position.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_position.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_replace.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_replace.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_right.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_right.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_split_part.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_split_part.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_string_literal.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/fixture_string_literal.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_any_value.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_any_value.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_bool_or.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_bool_or.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_cast_bool_to_text.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_cast_bool_to_text.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_concat.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_concat.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_current_timestamp.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_current_timestamp.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_date_trunc.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_date_trunc.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_dateadd.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_dateadd.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_datediff.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_datediff.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_equals.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_equals.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_escape_single_quotes.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_escape_single_quotes.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_except.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_except.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_generate_series.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_generate_series.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_get_intervals_between.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_get_intervals_between.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_get_powers_of_two.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_get_powers_of_two.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_hash.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_hash.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_intersect.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_intersect.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_last_day.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_last_day.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_length.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_length.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_listagg.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_listagg.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_null_compare.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_null_compare.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_position.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_position.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_replace.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_replace.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_right.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_right.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_safe_cast.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_safe_cast.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_split_part.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_split_part.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_string_literal.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_string_literal.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_timestamps.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_validate_sql.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/test_validate_sql.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/base_data_type_macro.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/base_data_type_macro.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_bigint.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/test_type_bigint.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_boolean.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/test_type_boolean.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_float.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/test_type_float.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_int.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/test_type_int.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_numeric.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/test_type_numeric.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_string.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/test_type_string.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_timestamp.py` & `dbt_tests_adapter-1.8.0b2/dbt/tests/adapter/utils/data_types/test_type_timestamp.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/.gitignore` & `dbt_tests_adapter-1.8.0b2/.gitignore`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -149,8 +149,8 @@
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
 # PyCharm
-.idea/
+.idea/
```

### Comparing `dbt_tests_adapter-1.8.0b1/README.md` & `dbt_tests_adapter-1.8.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0b1/pyproject.toml` & `dbt_tests_adapter-1.8.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     # TODO: remove `dbt-core` dependency
     "dbt-core>=1.8.0a1,<1.9.0",
     # `dbt-tests-adapter` will ultimately depend on the packages below
     # `dbt-tests-adapter` temporarily uses `dbt-core` for a dbt runner
     # `dbt-core` takes the packages below as dependencies, so they are unpinned to avoid conflicts
```

### Comparing `dbt_tests_adapter-1.8.0b1/PKG-INFO` & `dbt_tests_adapter-1.8.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dbt-tests-adapter
-Version: 1.8.0b1
+Version: 1.8.0b2
 Summary: The set of reusable tests and test fixtures used to test common functionality
 Project-URL: Homepage, https://github.com/dbt-labs/dbt-adapters
 Project-URL: Documentation, https://docs.getdbt.com
 Project-URL: Repository, https://github.com/dbt-labs/dbt-adapters.git
 Project-URL: Issues, https://github.com/dbt-labs/dbt-adapters/issues
 Project-URL: Changelog, https://github.com/dbt-labs/dbt-adapters/blob/main/CHANGELOG.md
 Author-email: dbt Labs <info@dbtlabs.com>
@@ -15,14 +15,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8.0
 Requires-Dist: dbt-adapters
 Requires-Dist: dbt-core<1.9.0,>=1.8.0a1
 Requires-Dist: pyyaml
 Provides-Extra: build
 Requires-Dist: check-wheel-contents; extra == 'build'
 Requires-Dist: twine; extra == 'build'
```

