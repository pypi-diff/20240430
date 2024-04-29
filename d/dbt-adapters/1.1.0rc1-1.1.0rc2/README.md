# Comparing `tmp/dbt_adapters-1.1.0rc1.tar.gz` & `tmp/dbt_adapters-1.1.0rc2.tar.gz`

## Comparing `dbt_adapters-1.1.0rc1.tar` & `dbt_adapters-1.1.0rc2.tar`

### file list

```diff
@@ -1,154 +1,154 @@
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/__about__.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/__init__.py
--rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/cache.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/capability.py
--rw-r--r--   0        0        0     9423 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/factory.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/py.typed
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/reference_keys.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/utils.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/base/README.md
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/base/__init__.py
--rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/base/column.py
--rw-r--r--   0        0        0    16921 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/base/connections.py
--rw-r--r--   0        0        0    68316 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/base/impl.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/base/meta.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/base/plugin.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/base/query_headers.py
--rw-r--r--   0        0        0    15642 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/base/relation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/clients/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/clients/jinja.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/contracts/__init__.py
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/contracts/connection.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/contracts/macros.py
--rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/contracts/relation.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/events/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/events/__init__.py
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/events/adapter_types.proto
--rw-r--r--   0        0        0    26480 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/events/adapter_types_pb2.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/events/base_types.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/events/logging.py
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/events/types.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/exceptions/__init__.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/exceptions/alias.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/exceptions/cache.py
--rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/exceptions/compilation.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/exceptions/connection.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/exceptions/database.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/relation_configs/README.md
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/relation_configs/__init__.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/relation_configs/config_base.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/relation_configs/config_change.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/relation_configs/config_validation.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/sql/__init__.py
--rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/sql/connections.py
--rw-r--r--   0        0        0    10722 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/adapters/sql/impl.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/py.typed
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/__init__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/dbt_project.yml
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/docs/overview.md
--rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/apply_grants.sql
--rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/columns.sql
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/freshness.sql
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/indexes.sql
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/metadata.sql
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/persist_docs.sql
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/relation.sql
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/schema.sql
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/show.sql
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/timestamps.sql
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/validate_sql.sql
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/etc/datetime.sql
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/etc/statement.sql
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/generic_test_sql/not_null.sql
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/generic_test_sql/relationships.sql
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/generic_test_sql/unique.sql
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/configs.sql
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/hooks.sql
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view.sql
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/table.sql
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/view.sql
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/clone/can_clone_table.sql
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/clone/clone.sql
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/clone/create_or_replace_clone.sql
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/seeds/helpers.sql
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/seeds/seed.sql
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/tests/helpers.sql
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/tests/test.sql
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/tests/unit.sql
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/python_model/python.sql
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/create.sql
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/create_backup.sql
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/create_intermediate.sql
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/drop.sql
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/drop_backup.sql
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/rename.sql
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/rename_intermediate.sql
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/replace.sql
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/schema.sql
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/materialized_view/alter.sql
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/materialized_view/create.sql
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/materialized_view/drop.sql
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/materialized_view/refresh.sql
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/materialized_view/rename.sql
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/materialized_view/replace.sql
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/table/create.sql
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/table/drop.sql
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/table/rename.sql
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/table/replace.sql
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/view/create.sql
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/view/drop.sql
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/view/rename.sql
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/view/replace.sql
--rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/any_value.sql
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/array_append.sql
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/array_concat.sql
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/array_construct.sql
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/bool_or.sql
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/cast.sql
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/concat.sql
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/data_types.sql
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/date_spine.sql
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/date_trunc.sql
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/dateadd.sql
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/datediff.sql
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/escape_single_quotes.sql
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/except.sql
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/generate_series.sql
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/hash.sql
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/intersect.sql
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/last_day.sql
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/length.sql
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/listagg.sql
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/literal.sql
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/position.sql
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/replace.sql
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/right.sql
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/safe_cast.sql
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/split_part.sql
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/dbt/include/global_project/tests/generic/builtin.sql
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/LICENSE
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/README.md
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/__about__.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/__init__.py
+-rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/cache.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/capability.py
+-rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/factory.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/py.typed
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/reference_keys.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/utils.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/README.md
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/__init__.py
+-rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/column.py
+-rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/connections.py
+-rw-r--r--   0        0        0    68352 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/impl.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/meta.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/plugin.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/query_headers.py
+-rw-r--r--   0        0        0    16173 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/relation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/clients/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/clients/jinja.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/contracts/__init__.py
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/contracts/connection.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/contracts/macros.py
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/contracts/relation.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/events/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/events/__init__.py
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/events/adapter_types.proto
+-rw-r--r--   0        0        0    26480 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/events/adapter_types_pb2.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/events/base_types.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/events/logging.py
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/events/types.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/alias.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/cache.py
+-rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/compilation.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/connection.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/database.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/README.md
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/__init__.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/config_base.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/config_change.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/config_validation.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/sql/__init__.py
+-rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/sql/connections.py
+-rw-r--r--   0        0        0    10722 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/sql/impl.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/py.typed
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/__init__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/dbt_project.yml
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/docs/overview.md
+-rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/apply_grants.sql
+-rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/columns.sql
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/freshness.sql
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/indexes.sql
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/metadata.sql
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/persist_docs.sql
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/relation.sql
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/schema.sql
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/show.sql
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/timestamps.sql
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/validate_sql.sql
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/etc/datetime.sql
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/etc/statement.sql
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/generic_test_sql/not_null.sql
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/generic_test_sql/relationships.sql
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/generic_test_sql/unique.sql
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/configs.sql
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/hooks.sql
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/materialized_view.sql
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/table.sql
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/view.sql
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/clone/can_clone_table.sql
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/clone/clone.sql
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/clone/create_or_replace_clone.sql
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/seeds/seed.sql
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/tests/helpers.sql
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/tests/test.sql
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/tests/unit.sql
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/python_model/python.sql
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/create.sql
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/create_backup.sql
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/create_intermediate.sql
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/drop.sql
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/drop_backup.sql
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/rename.sql
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/rename_intermediate.sql
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/replace.sql
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/schema.sql
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/create.sql
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/refresh.sql
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/rename.sql
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/replace.sql
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/table/create.sql
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/table/drop.sql
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/table/rename.sql
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/table/replace.sql
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/view/create.sql
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/view/drop.sql
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/view/rename.sql
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/view/replace.sql
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/any_value.sql
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/array_append.sql
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/array_concat.sql
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/array_construct.sql
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/bool_or.sql
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/cast.sql
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/concat.sql
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/data_types.sql
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/date_spine.sql
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/date_trunc.sql
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/dateadd.sql
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/datediff.sql
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/except.sql
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/generate_series.sql
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/hash.sql
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/intersect.sql
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/last_day.sql
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/length.sql
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/listagg.sql
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/literal.sql
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/position.sql
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/replace.sql
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/right.sql
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/safe_cast.sql
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/split_part.sql
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/tests/generic/builtin.sql
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/LICENSE
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/README.md
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/PKG-INFO
```

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/cache.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/cache.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/capability.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/capability.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/factory.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,25 +97,22 @@
 
         return plugin.credentials
 
     def register_adapter(
         self,
         config: AdapterRequiredConfig,
         mp_context: SpawnContext,
-        adapter_registered_log_level: Optional[EventLevel] = EventLevel.INFO
+        adapter_registered_log_level: Optional[EventLevel] = EventLevel.INFO,
     ) -> None:
         adapter_name = config.credentials.type
         adapter_type = self.get_adapter_class_by_name(adapter_name)
         adapter_version = self._adapter_version(adapter_name)
         fire_event(
-            AdapterRegistered(
-                adapter_name=adapter_name,
-                adapter_version=adapter_version
-            ),
-            level=adapter_registered_log_level
+            AdapterRegistered(adapter_name=adapter_name, adapter_version=adapter_version),
+            level=adapter_registered_log_level,
         )
         with self.lock:
             if adapter_name in self.adapters:
                 # this shouldn't really happen...
                 return
 
             adapter: Adapter = adapter_type(config, mp_context)  # type: ignore
@@ -195,17 +192,17 @@
         return self.lookup_adapter(name).CONSTRAINT_SUPPORT  # type: ignore
 
 
 FACTORY: AdapterContainer = AdapterContainer()
 
 
 def register_adapter(
-        config: AdapterRequiredConfig,
-        mp_context: SpawnContext,
-        adapter_registered_log_level: Optional[EventLevel] = EventLevel.INFO
+    config: AdapterRequiredConfig,
+    mp_context: SpawnContext,
+    adapter_registered_log_level: Optional[EventLevel] = EventLevel.INFO,
 ) -> None:
     FACTORY.register_adapter(config, mp_context, adapter_registered_log_level)
 
 
 def get_adapter(config: AdapterRequiredConfig):
     return FACTORY.lookup_adapter(config.credentials.type)
```

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/protocol.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/protocol.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,25 +43,23 @@
 
 
 Self = TypeVar("Self", bound="RelationProtocol")
 
 
 class RelationProtocol(Protocol):
     @classmethod
-    def get_default_quote_policy(cls) -> Policy:
-        ...
+    def get_default_quote_policy(cls) -> Policy: ...
 
     @classmethod
     def create_from(
         cls: Type[Self],
         quoting: HasQuoting,
         relation_config: RelationConfig,
         **kwargs: Any,
-    ) -> Self:
-        ...
+    ) -> Self: ...
 
 
 AdapterConfig_T = TypeVar("AdapterConfig_T", bound=AdapterConfig)
 ConnectionManager_T = TypeVar("ConnectionManager_T", bound=ConnectionManagerProtocol)
 Relation_T = TypeVar("Relation_T", bound=RelationProtocol)
 Column_T = TypeVar("Column_T", bound=ColumnProtocol)
 
@@ -69,16 +67,15 @@
 class MacroContextGeneratorCallable(Protocol):
     def __call__(
         self,
         macro_protocol: MacroProtocol,
         config: AdapterRequiredConfig,
         macro_resolver: MacroResolverProtocol,
         package_name: Optional[str],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
 
 # TODO CT-211
 class AdapterProtocol(  # type: ignore[misc]
     Protocol,
     Generic[
         AdapterConfig_T,
@@ -92,85 +89,62 @@
     # See: https://github.com/python/mypy/issues/5144
     AdapterSpecificConfigs: Type[AdapterConfig_T]
     Column: Type[Column_T]
     Relation: Type[Relation_T]
     ConnectionManager: Type[ConnectionManager_T]
     connections: ConnectionManager_T
 
-    def __init__(self, config: AdapterRequiredConfig) -> None:
-        ...
+    def __init__(self, config: AdapterRequiredConfig) -> None: ...
 
-    def set_macro_resolver(self, macro_resolver: MacroResolverProtocol) -> None:
-        ...
+    def set_macro_resolver(self, macro_resolver: MacroResolverProtocol) -> None: ...
 
-    def get_macro_resolver(self) -> Optional[MacroResolverProtocol]:
-        ...
+    def get_macro_resolver(self) -> Optional[MacroResolverProtocol]: ...
 
-    def clear_macro_resolver(self) -> None:
-        ...
+    def clear_macro_resolver(self) -> None: ...
 
     def set_macro_context_generator(
         self,
         macro_context_generator: MacroContextGeneratorCallable,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @classmethod
     def type(cls) -> str:
         pass
 
-    def set_query_header(self, query_header_context: Dict[str, Any]) -> None:
-        ...
+    def set_query_header(self, query_header_context: Dict[str, Any]) -> None: ...
 
     @staticmethod
-    def get_thread_identifier() -> Hashable:
-        ...
+    def get_thread_identifier() -> Hashable: ...
 
-    def get_thread_connection(self) -> Connection:
-        ...
+    def get_thread_connection(self) -> Connection: ...
 
-    def set_thread_connection(self, conn: Connection) -> None:
-        ...
+    def set_thread_connection(self, conn: Connection) -> None: ...
 
-    def get_if_exists(self) -> Optional[Connection]:
-        ...
+    def get_if_exists(self) -> Optional[Connection]: ...
 
-    def clear_thread_connection(self) -> None:
-        ...
+    def clear_thread_connection(self) -> None: ...
 
-    def clear_transaction(self) -> None:
-        ...
+    def clear_transaction(self) -> None: ...
 
-    def exception_handler(self, sql: str) -> ContextManager:
-        ...
+    def exception_handler(self, sql: str) -> ContextManager: ...
 
-    def set_connection_name(self, name: Optional[str] = None) -> Connection:
-        ...
+    def set_connection_name(self, name: Optional[str] = None) -> Connection: ...
 
-    def cancel_open(self) -> Optional[List[str]]:
-        ...
+    def cancel_open(self) -> Optional[List[str]]: ...
 
-    def open(cls, connection: Connection) -> Connection:
-        ...
+    def open(cls, connection: Connection) -> Connection: ...
 
-    def release(self) -> None:
-        ...
+    def release(self) -> None: ...
 
-    def cleanup_all(self) -> None:
-        ...
+    def cleanup_all(self) -> None: ...
 
-    def begin(self) -> None:
-        ...
+    def begin(self) -> None: ...
 
-    def commit(self) -> None:
-        ...
+    def commit(self) -> None: ...
 
-    def close(cls, connection: Connection) -> Connection:
-        ...
+    def close(cls, connection: Connection) -> Connection: ...
 
-    def commit_if_has_connection(self) -> None:
-        ...
+    def commit_if_has_connection(self) -> None: ...
 
     def execute(
         self, sql: str, auto_begin: bool = False, fetch: bool = False
-    ) -> Tuple[AdapterResponse, "agate.Table"]:
-        ...
+    ) -> Tuple[AdapterResponse, "agate.Table"]: ...
```

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/reference_keys.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/reference_keys.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/utils.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/base/README.md` & `dbt_adapters-1.1.0rc2/dbt/adapters/base/README.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/base/column.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/base/column.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/base/connections.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/base/connections.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,17 @@
                 transaction_open=False,
                 handle=None,
                 credentials=self.profile.credentials,
             )
             conn.handle = LazyHandle(self.open)
             # Add the connection to thread_connections for this thread
             self.set_thread_connection(conn)
-            fire_event(NewConnection(conn_name=conn_name, conn_type=self.TYPE, node_info=get_node_info()))
+            fire_event(
+                NewConnection(conn_name=conn_name, conn_type=self.TYPE, node_info=get_node_info())
+            )
         else:  # existing connection either wasn't open or didn't have the right name
             if conn.state != "open":
                 conn.handle = LazyHandle(self.open)
             if conn.name != conn_name:
                 orig_conn_name: str = conn.name or ""
                 conn.name = conn_name
                 fire_event(ConnectionReused(orig_conn_name=orig_conn_name, conn_name=conn_name))
```

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/base/impl.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/base/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1324,22 +1324,24 @@
               for each request the method made to compute the freshness for the provided sources.
             * the second element is a dictionary mapping an input source BaseRelation to a FreshnessResponse,
               if it was possible to calculate a FreshnessResponse for the source.
         """
         # Track schema, identifiers of sources for lookup from batch query
         schema_identifier_to_source = {
             (
-                source.path.get_lowered_part(ComponentName.Schema),
-                source.path.get_lowered_part(ComponentName.Identifier),
+                source.path.get_lowered_part(ComponentName.Schema),  # type: ignore
+                source.path.get_lowered_part(ComponentName.Identifier),  # type: ignore
             ): source
             for source in sources
         }
 
         # Group metadata sources by information schema -- one query per information schema will be necessary
-        sources_by_info_schema: Dict[InformationSchema, List[BaseRelation]] = self._get_catalog_relations_by_info_schema(sources)
+        sources_by_info_schema: Dict[InformationSchema, List[BaseRelation]] = (
+            self._get_catalog_relations_by_info_schema(sources)
+        )
 
         freshness_responses: Dict[BaseRelation, FreshnessResponse] = {}
         adapter_responses: List[Optional[AdapterResponse]] = []
         for (
             information_schema,
             sources_for_information_schema,
         ) in sources_by_info_schema.items():
@@ -1389,29 +1391,28 @@
             "max_loaded_at": max_loaded_at,
             "snapshotted_at": snapshotted_at,
             "age": age,
         }
 
         return freshness
 
-    def _parse_freshness_row(self, row: "agate.Row", table: "agate.Table") -> Tuple[Any, FreshnessResponse]:
+    def _parse_freshness_row(
+        self, row: "agate.Row", table: "agate.Table"
+    ) -> Tuple[Any, FreshnessResponse]:
         from dbt_common.clients.agate_helper import get_column_value_uncased
 
         try:
             last_modified_val = get_column_value_uncased("last_modified", row)
             snapshotted_at_val = get_column_value_uncased("snapshotted_at", row)
             identifier = get_column_value_uncased("identifier", row)
             schema = get_column_value_uncased("schema", row)
         except Exception:
             raise MacroResultError(GET_RELATION_LAST_MODIFIED_MACRO_NAME, table)
 
-        freshness_response = self._create_freshness_response(
-            last_modified_val,
-            snapshotted_at_val
-        )
+        freshness_response = self._create_freshness_response(last_modified_val, snapshotted_at_val)
         raw_relation = schema.lower().strip(), identifier.lower().strip()
         return raw_relation, freshness_response
 
     def pre_model_hook(self, config: Mapping[str, Any]) -> Any:
         """A hook for running some operation before the model materialization
         runs. The hook can assume it has a connection available.
```

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/base/meta.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/base/meta.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/base/plugin.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/base/plugin.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/base/query_headers.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/base/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/base/relation.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/base/relation.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,17 @@
     quote_character: str = '"'
     # Python 3.11 requires that these use default_factory instead of simple default
     # ValueError: mutable default <class 'dbt.contracts.relation.Policy'> for field include_policy is not allowed: use default_factory
     include_policy: Policy = field(default_factory=lambda: Policy())
     quote_policy: Policy = field(default_factory=lambda: Policy())
     dbt_created: bool = False
     limit: Optional[int] = None
+    require_alias: bool = (
+        True  # used to govern whether to add an alias when render_limited is called
+    )
 
     # register relation types that can be renamed for the purpose of replacing relations using stages and backups
     # adding a relation type here also requires defining the associated rename macro
     # e.g. adding RelationType.View in dbt-postgres requires that you define:
     # include/postgres/macros/relations/view/rename.sql::postgres__get_rename_view_sql()
     renameable_relations: SerializableIterable = field(default_factory=frozenset)
 
@@ -201,22 +204,30 @@
                     path_part = self.quoted(path_part)
             yield key, path_part
 
     def render(self) -> str:
         # if there is nothing set, this will return the empty string.
         return ".".join(part for _, part in self._render_iterator() if part is not None)
 
+    def _render_limited_alias(self) -> str:
+        """Some databases require an alias for subqueries (postgres, mysql) for all others we want to avoid adding
+        an alias as it has the potential to introduce issues with the query if the user also defines an alias.
+        """
+        if self.require_alias:
+            return f" _dbt_limit_subq_{self.table}"
+        return ""
+
     def render_limited(self) -> str:
         rendered = self.render()
         if self.limit is None:
             return rendered
         elif self.limit == 0:
-            return f"(select * from {rendered} where false limit 0) _dbt_limit_subq"
+            return f"(select * from {rendered} where false limit 0){self._render_limited_alias()}"
         else:
-            return f"(select * from {rendered} limit {self.limit}) _dbt_limit_subq"
+            return f"(select * from {rendered} limit {self.limit}){self._render_limited_alias()}"
 
     def quoted(self, identifier):
         return "{quote_char}{identifier}{quote_char}".format(
             quote_char=self.quote_character,
             identifier=identifier,
         )
```

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/clients/jinja.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/contracts/connection.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/contracts/relation.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/contracts/relation.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,19 +36,17 @@
     quoting: Dict[str, Any]
     unique_key: Union[str, List[str], None]
     on_schema_change: Optional[str]
     on_configuration_change: OnConfigurationChangeOption
     contract: MaterializationContract
     extra: Dict[str, Any]
 
-    def __contains__(self, item):
-        ...
+    def __contains__(self, item): ...
 
-    def __delitem__(self, key):
-        ...
+    def __delitem__(self, key): ...
 
 
 class RelationConfig(Protocol):
     resource_type: str
     name: str
     description: str
     database: str
```

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/events/README.md` & `dbt_adapters-1.1.0rc2/dbt/adapters/events/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Adding a New Event
 * Add a new message in types.proto, and a second message with the same name + "Msg". The "Msg" message should have two fields, an "info" field of EventInfo, and a "data" field referring to the message name without "Msg"
 * run the protoc compiler to update adapter_types_pb2.py:   make adapter_proto_types
 * Add a wrapping class in core/dbt/adapters/event/types.py with a Level superclass  plus code and message methods
 
 We have switched from using betterproto to using google protobuf, because of a lack of support for Struct fields in betterproto.
 
-The google protobuf interface is janky and very much non-Pythonic. The "generated" classes in types_pb2.py do not resemble regular Python classes. They do not have normal constructors; they can only be constructed empty. They can be "filled" by setting fields individually or using a json_format method like ParseDict.  We have wrapped the logging events with a class (in types.py) which allows using a constructor -- keywords only, no positional parameters. 
+The google protobuf interface is janky and very much non-Pythonic. The "generated" classes in types_pb2.py do not resemble regular Python classes. They do not have normal constructors; they can only be constructed empty. They can be "filled" by setting fields individually or using a json_format method like ParseDict.  We have wrapped the logging events with a class (in types.py) which allows using a constructor -- keywords only, no positional parameters.
 
 ## Required for Every Event
 
 - a method `code`, that's unique across events
 - assign a log level by using the Level mixin: `DebugLevel`, `InfoLevel`, `WarnLevel`, or `ErrorLevel`
 - a message()
```

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/events/adapter_types.proto` & `dbt_adapters-1.1.0rc2/dbt/adapters/events/adapter_types.proto`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/events/adapter_types_pb2.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/events/adapter_types_pb2.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/events/base_types.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/events/logging.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/events/logging.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/events/types.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/events/types.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/exceptions/__init__.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/exceptions/alias.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/alias.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/exceptions/cache.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/cache.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/exceptions/compilation.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/compilation.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/exceptions/database.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/database.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/relation_configs/README.md` & `dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RelationConfig
 This package serves as an initial abstraction for managing the inspection of existing relations and determining
-changes on those relations. It arose from the materialized view work and is currently only supporting 
+changes on those relations. It arose from the materialized view work and is currently only supporting
 materialized views for Postgres and Redshift as well as dynamic tables for Snowflake. There are three main
 classes in this package.
 
 ## RelationConfigBase
 This is a very small class that only has a `from_dict()` method and a default `NotImplementedError()`. At some
 point this could be replaced by a more robust framework, like `mashumaro` or `pydantic`.
```

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/relation_configs/config_base.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/config_base.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/relation_configs/config_change.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/config_change.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,13 +12,15 @@
     create = "create"
     drop = "drop"
 
 
 @dataclass(frozen=True, eq=True, unsafe_hash=True)
 class RelationConfigChange(RelationConfigBase, ABC):
     action: RelationConfigChangeAction
-    context: Hashable  # this is usually a RelationConfig, e.g. IndexConfig, but shouldn't be limited
+    context: (
+        Hashable  # this is usually a RelationConfig, e.g. IndexConfig, but shouldn't be limited
+    )
 
     @property
     @abstractmethod
     def requires_full_refresh(self) -> bool:
         raise self._not_implemented_error()
```

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/relation_configs/config_validation.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/config_validation.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/sql/connections.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/sql/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/adapters/sql/impl.py` & `dbt_adapters-1.1.0rc2/dbt/adapters/sql/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/docs/overview.md` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/docs/overview.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/apply_grants.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/columns.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/columns.sql`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
       {%- if col['data_type'] is not defined -%}
         {%- do col_err.append(col['name']) -%}
       {#-- If this column's type is just 'numeric' then it is missing precision/scale, raise a warning --#}
       {%- elif col['data_type'].strip().lower() in ('numeric', 'decimal', 'number') -%}
         {%- do col_naked_numeric.append(col['name']) -%}
       {%- endif -%}
       {% set col_name = adapter.quote(col['name']) if col.get('quote') else col['name'] %}
-      cast(null as {{ col['data_type'] }}) as {{ col_name }}{{ ", " if not loop.last }}
+      {{ cast('null', col['data_type']) }} as {{ col_name }}{{ ", " if not loop.last }}
     {%- endfor -%}
     {%- if (col_err | length) > 0 -%}
       {{ exceptions.column_type_missing(column_names=col_err) }}
     {%- elif (col_naked_numeric | length) > 0 -%}
       {{ exceptions.warn("Detected columns with numeric type and unspecified precision/scale, this can lead to unintended rounding: " ~ col_naked_numeric ~ "`") }}
     {%- endif -%}
 {% endmacro %}
```

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/freshness.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/indexes.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/metadata.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/persist_docs.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/relation.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/schema.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/show.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/show.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/adapters/timestamps.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/etc/datetime.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/etc/datetime.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/etc/statement.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/configs.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/configs.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/hooks.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/table.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/view.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/clone/clone.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/clone/clone.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/seeds/helpers.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/seeds/seed.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/seeds/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/tests/helpers.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/tests/helpers.sql`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -37,8 +37,8 @@
     {{ expected_fixture_sql }}
   ) _dbt_internal_unit_test_expected
 )
 -- Union actual and expected results
 select * from dbt_internal_unit_test_actual
 union all
 select * from dbt_internal_unit_test_expected
-{%- endmacro %}
+{%- endmacro %}
```

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/tests/test.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/materializations/tests/unit.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/tests/unit.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/python_model/python.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/create.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/create.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/create_backup.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/create_backup.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/create_intermediate.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/create_intermediate.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/drop.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/drop.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/rename.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/rename.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/replace.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/materialized_view/alter.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/materialized_view/drop.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/drop.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/table/create.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/table/create.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/view/create.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/relations/view/replace.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/view/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             {{ exceptions.raise_compiler_error(
                 "Invalid column name: '" ~ column_name ~ "' in unit test fixture for " ~ fixture_name ~ "."
                 "\nAccepted columns for " ~ fixture_name ~ " are: " ~ (column_name_to_data_types.keys()|list)
             ) }}
         {%- endif -%}
 
         {%- set column_type = column_name_to_data_types[column_name] %}
-        
+
         {#-- sanitize column_value: wrap yaml strings in quotes, apply cast --#}
         {%- set column_value_clean = column_value -%}
         {%- if column_value is string -%}
             {%- set column_value_clean = dbt.string_literal(dbt.escape_single_quotes(column_value)) -%}
         {%- elif column_value is none -%}
             {%- set column_value_clean = 'null' -%}
         {%- endif -%}
```

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/data_types.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/date_spine.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/date_spine.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/generate_series.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/generate_series.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/listagg.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/macros/utils/split_part.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/dbt/include/global_project/tests/generic/builtin.sql` & `dbt_adapters-1.1.0rc2/dbt/include/global_project/tests/generic/builtin.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/.gitignore` & `dbt_adapters-1.1.0rc2/.gitignore`

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

### Comparing `dbt_adapters-1.1.0rc1/LICENSE` & `dbt_adapters-1.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/README.md` & `dbt_adapters-1.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc1/pyproject.toml` & `dbt_adapters-1.1.0rc2/pyproject.toml`

 * *Files 18% similar despite different names*

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
     "dbt-common<2.0",
     "pytz>=2015.7",
     # installed via dbt-common but used directly
     "agate>=1.0,<2.0",
     "mashumaro[msgpack]>=3.0,<4.0",
@@ -50,43 +51,24 @@
 
 [tool.hatch.build.targets.wheel]
 include = ["dbt/adapters", "dbt/include", "dbt/__init__.py"]
 
 [tool.hatch.envs.default]
 dependencies = [
     "dbt_common @ git+https://github.com/dbt-labs/dbt-common.git",
+    'pre-commit==3.7.0;python_version>="3.9"',
+    'pre-commit==3.5.0;python_version=="3.8"',
 ]
-
-[tool.hatch.envs.lint]
-detached = true
-dependencies = [
-    "black>=24.3",
-    "flake8",
-    "Flake8-pyproject",
-]
-[tool.hatch.envs.lint.scripts]
-all = [
-    "- black-only",
-    "- flake8-only",
-]
-black-only = "python -m black ."
-flake8-only = "python -m flake8 ."
-
-[tool.hatch.envs.typecheck]
-dependencies = [
-    "mypy",
-    "types-PyYAML",
-    "types-protobuf",
-    "types-pytz",
-]
-[tool.hatch.envs.typecheck.scripts]
-all = "python -m mypy ."
+[tool.hatch.envs.default.scripts]
+dev = "pre-commit install"
+code-quality = "pre-commit run --all-files"
 
 [tool.hatch.envs.unit-tests]
 dependencies = [
+    "dbt_common @ git+https://github.com/dbt-labs/dbt-common.git",
     "pytest",
     "pytest-dotenv",
     "pytest-xdist",
 ]
 [tool.hatch.envs.unit-tests.scripts]
 all = "python -m pytest {args:tests/unit}"
 
@@ -110,45 +92,16 @@
 check-sdist = [
     "check-wheel-contents dist/*.whl --ignore W007,W008",
     "find ./dist/dbt_adapters-*.gz -maxdepth 1 -type f | xargs python -m pip install --force-reinstall --find-links=dist/",
     "pip freeze | grep dbt-adapters",
 ]
 protobuf = "protoc -I=./dbt/adapters/events --python_out=./dbt/adapters/events ./dbt/adapters/events/adapter_types.proto"
 
-[tool.black]
-extend-exclude = "dbt/adapters/events/adapter_types_pb2.py"
-line-length = 99
-target-version = ['py38']
-
-[tool.flake8]
-select = ["E", "W", "F"]
-ignore = ["E203", "E501", "E741", "W503", "W504"]
-exclude = [
-    "dbt/adapters/events/adapter_types_pb2.py",
-    "tests/functional",
-    "venv",
-]
-per-file-ignores = ["*/__init__.py: F401"]
-
 [tool.mypy]
-namespace_packages = true
-show_error_codes = true
-explicit_package_bases = true
-ignore_missing_imports = true
-pretty = true
 mypy_path = "third-party-stubs/"
-files = [
-    "dbt",
-    "tests/unit",
-]
-exclude = [
-    "dbt/adapters/events/adapter_types_pb2.py",
-    "dbt-tests-adapter/dbt/__init__.py",  # overlaps with `dbt/__init__.py` as expected for namespaces
-    "venv",
-]
 [[tool.mypy.overrides]]
 module = ["dbt.adapters.events.adapter_types_pb2"]
 follow_imports = "skip"
 
 [tool.pytest]
 env_files = ["test.env"]
 testpaths = [
```

### Comparing `dbt_adapters-1.1.0rc1/PKG-INFO` & `dbt_adapters-1.1.0rc2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dbt-adapters
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: The set of adapter protocols and base functionality that supports integration with dbt-core
 Project-URL: Homepage, https://github.com/dbt-labs/dbt-adapters
 Project-URL: Documentation, https://docs.getdbt.com
 Project-URL: Repository, https://github.com/dbt-labs/dbt-adapters.git
 Project-URL: Issues, https://github.com/dbt-labs/dbt-adapters/issues
 Project-URL: Changelog, https://github.com/dbt-labs/dbt-adapters/blob/main/CHANGELOG.md
 Author-email: dbt Labs <info@dbtlabs.com>
@@ -16,14 +16,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8.0
 Requires-Dist: agate<2.0,>=1.0
 Requires-Dist: dbt-common<2.0
 Requires-Dist: mashumaro[msgpack]<4.0,>=3.0
 Requires-Dist: protobuf<5.0,>=3.0
 Requires-Dist: pytz>=2015.7
 Requires-Dist: typing-extensions<5.0,>=4.0
```

