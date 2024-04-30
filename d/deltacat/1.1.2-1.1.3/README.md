# Comparing `tmp/deltacat-1.1.2.tar.gz` & `tmp/deltacat-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deltacat-1.1.2.tar", last modified: Wed Apr 24 19:54:46 2024, max compression
+gzip compressed data, was "dist/deltacat-1.1.3.tar", last modified: Tue Apr 30 02:54:02 2024, max compression
```

## Comparing `deltacat-1.1.2.tar` & `deltacat-1.1.3.tar`

### file list

```diff
@@ -1,268 +1,268 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 19:42:40.000000 deltacat-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-24 19:54:46.000000 deltacat-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-24 19:42:40.000000 deltacat-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/aws/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/aws/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/aws/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/aws/redshift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/aws/redshift/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/aws/redshift/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/aws/redshift/model/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    24118 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/aws/s3u.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/benchmarking/benchmark_parquet_reads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/benchmarking/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/catalog/default_catalog_impl/
--rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/catalog/default_catalog_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/catalog/delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/catalog/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/catalog/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/catalog/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/catalog/model/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/catalog/model/table_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/compactor/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27612 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/compaction_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/compactor/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/model/compact_partition_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    30547 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/model/compaction_session_audit_info.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/model/compactor_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/model/dedupe_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/model/delta_annotated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/model/delta_file_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/model/delta_file_locator.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/model/hash_bucket_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/model/materialize_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/model/primary_key_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/model/pyarrow_write_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/model/repartition_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/model/round_completion_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/model/table_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/repartition_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/compactor/steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/steps/dedupe.py
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/steps/hash_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/steps/materialize.py
--rw-r--r--   0 runner    (1001) docker     (127)    10960 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/steps/repartition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/compactor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17303 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/utils/primary_key_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/utils/round_completion_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/utils/sort_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor/utils/system_columns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25576 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/compaction_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/deletes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/deletes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/deletes/delete_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/deletes/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/deletes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/model/hash_bucket_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/model/hash_bucket_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/model/merge_file_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/model/merge_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/model/merge_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/steps/hash_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    21657 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/steps/merge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/utils/content_type_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/utils/dedupe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/utils/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/utils/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/utils/primary_key_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    13780 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/compactor_v2/utils/task_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/merge_on_read/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/merge_on_read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/merge_on_read/daft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/merge_on_read/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/merge_on_read/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/merge_on_read/model/merge_on_read_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/merge_on_read/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/merge_on_read/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/merge_on_read/utils/delta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/metastats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/metastats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/metastats/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/metastats/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18731 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/metastats/meta_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/metastats/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/metastats/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/metastats/model/partition_stats_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/metastats/model/stats_cluster_size_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/metastats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/metastats/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/metastats/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/metastats/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/metastats/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/metastats/utils/ray_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/stats/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/stats/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/stats/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/stats/models/delta_column_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/stats/models/delta_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/stats/models/delta_stats_cache_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/stats/models/manifest_entry_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/stats/models/stats_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/stats/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/compute/stats/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/stats/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/stats/utils/intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/stats/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/compute/stats/utils/manifest_stats_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/io/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/io/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/io/aws/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/io/aws/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22599 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/io/aws/redshift/redshift_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/io/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/io/file_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/io/memcached_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/io/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/io/ray_plasma_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/io/read_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/io/redis_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/io/s3_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21649 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/storage/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/storage/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/storage/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/storage/model/delete_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/storage/model/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/storage/model/list_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/storage/model/locator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/storage/model/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/storage/model/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/storage/model/sort_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/storage/model/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/storage/model/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/storage/model/table_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/storage/model/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/tests/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/aws/test_clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/tests/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/catalog/test_default_catalog_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/tests/compute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72082 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/compact_partition_test_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/tests/compute/compactor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/compactor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/tests/compute/compactor/steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/compactor/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/compactor/steps/test_repartition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/tests/compute/compactor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/compactor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/compactor/utils/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/tests/compute/compactor_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/compactor_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/compactor_v2/test_compaction_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/compactor_v2/test_hashlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/tests/compute/compactor_v2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/compactor_v2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/compactor_v2/utils/test_task_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/test_compact_partition_incremental.py
--rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/test_compact_partition_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/test_util_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/test_util_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/compute/test_util_create_table_deltas_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/tests/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/io/test_cloudpickle_bug_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/io/test_file_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/io/test_memcached_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/io/test_ray_plasma_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/io/test_redis_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/io/test_s3_object_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/tests/local_deltacat_storage/
--rw-r--r--   0 runner    (1001) docker     (127)    35466 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/local_deltacat_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/tests/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/stats/test_intervals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/test_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/test_utils/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/test_utils/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/test_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/tests/utils/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/utils/test_cloudpickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/utils/test_daft.py
--rw-r--r--   0 runner    (1001) docker     (127)    19429 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/utils/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/utils/test_pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/utils/test_record_batch_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/tests/utils/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/types/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/types/partial_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/types/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/cloudpickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/daft.py
--rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/placement.py
--rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/pyarrow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat/utils/ray_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/ray_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/ray_utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/ray_utils/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/ray_utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/ray_utils/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/ray_utils/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/s3fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-24 19:42:40.000000 deltacat-1.1.2/deltacat/utils/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 19:54:46.000000 deltacat-1.1.2/deltacat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:54:46.000000 deltacat-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-24 19:42:40.000000 deltacat-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 02:42:11.000000 deltacat-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-30 02:54:02.000000 deltacat-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-30 02:42:11.000000 deltacat-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/aws/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/aws/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/aws/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/aws/redshift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/aws/redshift/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/aws/redshift/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/aws/redshift/model/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24118 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/aws/s3u.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/benchmarking/benchmark_parquet_reads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/benchmarking/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/catalog/default_catalog_impl/
+-rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/catalog/default_catalog_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/catalog/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/catalog/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/catalog/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/catalog/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/catalog/model/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/catalog/model/table_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27612 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/compaction_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/compact_partition_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30547 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/compaction_session_audit_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/compactor_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/dedupe_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/delta_annotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/delta_file_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/delta_file_locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/hash_bucket_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/materialize_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/pyarrow_write_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/repartition_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/round_completion_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/table_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/repartition_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/steps/dedupe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/steps/hash_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/steps/materialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10960 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/steps/repartition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17303 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/utils/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/utils/round_completion_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/utils/sort_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/utils/system_columns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25141 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/compaction_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/delete_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/model/hash_bucket_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/model/hash_bucket_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/model/merge_file_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/model/merge_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/model/merge_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/steps/hash_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21657 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/steps/merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/content_type_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/dedupe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13780 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/task_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/daft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/model/merge_on_read_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/utils/delta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/metastats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/metastats/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18731 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/meta_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/metastats/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/model/partition_stats_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/model/stats_cluster_size_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/metastats/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/utils/ray_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/stats/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/models/delta_column_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/models/delta_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/models/delta_stats_cache_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/models/manifest_entry_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/models/stats_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/stats/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/utils/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/utils/manifest_stats_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/io/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/io/aws/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/aws/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22599 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/aws/redshift/redshift_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/file_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/memcached_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/ray_plasma_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/read_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/redis_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/s3_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21649 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/storage/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/delete_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/list_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/sort_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/table_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/aws/test_clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/catalog/test_default_catalog_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72082 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compact_partition_test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/steps/test_repartition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/utils/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/compute/compactor_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor_v2/test_compaction_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor_v2/test_hashlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/compute/compactor_v2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor_v2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor_v2/utils/test_task_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/test_compact_partition_incremental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/test_compact_partition_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/test_util_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/test_util_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/test_util_create_table_deltas_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/io/test_cloudpickle_bug_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/io/test_file_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/io/test_memcached_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/io/test_ray_plasma_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/io/test_redis_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/io/test_s3_object_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/local_deltacat_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)    35466 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/local_deltacat_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/stats/test_intervals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/test_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/test_utils/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/test_utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/test_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/test_cloudpickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/test_daft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/test_pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/test_record_batch_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/types/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/types/partial_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/types/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/cloudpickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/daft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/pyarrow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/utils/ray_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/ray_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/ray_utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/ray_utils/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/ray_utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/ray_utils/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/ray_utils/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/s3fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-30 02:54:01.000000 deltacat-1.1.3/deltacat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 02:54:01.000000 deltacat-1.1.3/deltacat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-30 02:54:01.000000 deltacat-1.1.3/deltacat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 02:54:01.000000 deltacat-1.1.3/deltacat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 02:54:02.000000 deltacat-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-30 02:42:11.000000 deltacat-1.1.3/setup.py
```

### Comparing `deltacat-1.1.2/PKG-INFO` & `deltacat-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltacat
-Version: 1.1.2
+Version: 1.1.3
 Summary: A scalable, fast, ACID-compliant Data Catalog powered by Ray.
 Home-page: https://github.com/ray-project/deltacat
 Author: Ray Team
 License: UNKNOWN
 Description: # DeltaCAT
         
         DeltaCAT is a Pythonic Data Catalog powered by Ray.
```

### Comparing `deltacat-1.1.2/README.md` & `deltacat-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/__init__.py` & `deltacat-1.1.3/deltacat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     SortOrder,
 )
 from deltacat.types.media import ContentEncoding, ContentType, TableType
 from deltacat.types.tables import TableWriteMode
 
 deltacat.logs.configure_deltacat_logger(logging.getLogger(__name__))
 
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 
 
 __all__ = [
     "__version__",
     "all_catalogs",
     "alter_table",
     "create_table",
```

### Comparing `deltacat-1.1.2/deltacat/aws/clients.py` & `deltacat-1.1.3/deltacat/aws/clients.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/aws/redshift/model/manifest.py` & `deltacat-1.1.3/deltacat/aws/redshift/model/manifest.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/aws/s3u.py` & `deltacat-1.1.3/deltacat/aws/s3u.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/benchmarking/benchmark_parquet_reads.py` & `deltacat-1.1.3/deltacat/benchmarking/benchmark_parquet_reads.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/benchmarking/conftest.py` & `deltacat-1.1.3/deltacat/benchmarking/conftest.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/catalog/default_catalog_impl/__init__.py` & `deltacat-1.1.3/deltacat/catalog/default_catalog_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/catalog/delegate.py` & `deltacat-1.1.3/deltacat/catalog/delegate.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/catalog/interface.py` & `deltacat-1.1.3/deltacat/catalog/interface.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/catalog/model/catalog.py` & `deltacat-1.1.3/deltacat/catalog/model/catalog.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/catalog/model/table_definition.py` & `deltacat-1.1.3/deltacat/catalog/model/table_definition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/__init__.py` & `deltacat-1.1.3/deltacat/compute/compactor/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/compaction_session.py` & `deltacat-1.1.3/deltacat/compute/compactor/compaction_session.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/model/compact_partition_params.py` & `deltacat-1.1.3/deltacat/compute/compactor/model/compact_partition_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/model/compaction_session_audit_info.py` & `deltacat-1.1.3/deltacat/compute/compactor/model/compaction_session_audit_info.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/model/delta_annotated.py` & `deltacat-1.1.3/deltacat/compute/compactor/model/delta_annotated.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/model/delta_file_envelope.py` & `deltacat-1.1.3/deltacat/compute/compactor/model/delta_file_envelope.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/model/delta_file_locator.py` & `deltacat-1.1.3/deltacat/compute/compactor/model/delta_file_locator.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/model/materialize_result.py` & `deltacat-1.1.3/deltacat/compute/compactor/model/materialize_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/model/primary_key_index.py` & `deltacat-1.1.3/deltacat/compute/compactor/model/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/model/pyarrow_write_result.py` & `deltacat-1.1.3/deltacat/compute/compactor/model/pyarrow_write_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/model/round_completion_info.py` & `deltacat-1.1.3/deltacat/compute/compactor/model/round_completion_info.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/model/table_object_store.py` & `deltacat-1.1.3/deltacat/compute/compactor/model/table_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/repartition_session.py` & `deltacat-1.1.3/deltacat/compute/compactor/repartition_session.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/steps/dedupe.py` & `deltacat-1.1.3/deltacat/compute/compactor/steps/dedupe.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/steps/hash_bucket.py` & `deltacat-1.1.3/deltacat/compute/compactor/steps/hash_bucket.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/steps/materialize.py` & `deltacat-1.1.3/deltacat/compute/compactor/steps/materialize.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/steps/repartition.py` & `deltacat-1.1.3/deltacat/compute/compactor/steps/repartition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/utils/io.py` & `deltacat-1.1.3/deltacat/compute/compactor/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/utils/primary_key_index.py` & `deltacat-1.1.3/deltacat/compute/compactor/utils/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/utils/round_completion_file.py` & `deltacat-1.1.3/deltacat/compute/compactor/utils/round_completion_file.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/utils/sort_key.py` & `deltacat-1.1.3/deltacat/compute/compactor/utils/sort_key.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor/utils/system_columns.py` & `deltacat-1.1.3/deltacat/compute/compactor/utils/system_columns.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/compaction_session.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/compaction_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 )
 from deltacat.compute.compactor_v2.utils.task_options import (
     hash_bucket_resource_options_provider,
     merge_resource_options_provider,
     local_merge_resource_options_provider,
 )
 from deltacat.compute.compactor.model.compactor_version import CompactorVersion
-from deltacat.utils.metrics import MetricsActor, METRICS_CONFIG_ACTOR_NAME
 
 if importlib.util.find_spec("memray"):
     import memray
 
 
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
 
@@ -115,23 +114,14 @@
         return round_completion_file_s3_url
 
 
 def _execute_compaction(
     params: CompactPartitionParams, **kwargs
 ) -> Tuple[Optional[Partition], Optional[RoundCompletionInfo], Optional[str]]:
 
-    if params.metrics_config:
-        logger.info(
-            f"Setting metrics config with target: {params.metrics_config.metrics_target}"
-        )
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
-        ray.get(metrics_actor.set_metrics_config.remote(params.metrics_config))
-
     rcf_source_partition_locator = (
         params.rebase_source_partition_locator or params.source_partition_locator
     )
 
     base_audit_url = rcf_source_partition_locator.path(
         f"s3://{params.compaction_artifact_s3_bucket}/compaction-audit"
     )
```

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/constants.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/constants.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/deletes/delete_strategy.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/delete_strategy.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/deletes/model.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/model.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/deletes/utils.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/utils.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/model/hash_bucket_input.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/model/hash_bucket_input.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/model/merge_file_group.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/model/merge_file_group.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/model/merge_input.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/model/merge_input.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/steps/hash_bucket.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/steps/hash_bucket.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/steps/merge.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/steps/merge.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/utils/content_type_params.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/utils/content_type_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/utils/dedupe.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/utils/dedupe.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/utils/delta.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/utils/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/utils/io.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/utils/merge.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/utils/merge.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/utils/primary_key_index.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/utils/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/compactor_v2/utils/task_options.py` & `deltacat-1.1.3/deltacat/compute/compactor_v2/utils/task_options.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/merge_on_read/daft.py` & `deltacat-1.1.3/deltacat/compute/merge_on_read/daft.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/merge_on_read/model/merge_on_read_params.py` & `deltacat-1.1.3/deltacat/compute/merge_on_read/model/merge_on_read_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/merge_on_read/utils/delta.py` & `deltacat-1.1.3/deltacat/compute/merge_on_read/utils/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/metastats/meta_stats.py` & `deltacat-1.1.3/deltacat/compute/metastats/meta_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/metastats/model/partition_stats_dict.py` & `deltacat-1.1.3/deltacat/compute/metastats/model/partition_stats_dict.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/metastats/model/stats_cluster_size_estimator.py` & `deltacat-1.1.3/deltacat/compute/metastats/model/stats_cluster_size_estimator.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/metastats/stats.py` & `deltacat-1.1.3/deltacat/compute/metastats/stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/metastats/utils/constants.py` & `deltacat-1.1.3/deltacat/compute/metastats/utils/constants.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/metastats/utils/io.py` & `deltacat-1.1.3/deltacat/compute/metastats/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py` & `deltacat-1.1.3/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/metastats/utils/ray_utils.py` & `deltacat-1.1.3/deltacat/compute/metastats/utils/ray_utils.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/stats/basic.py` & `deltacat-1.1.3/deltacat/compute/stats/basic.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/stats/models/delta_column_stats.py` & `deltacat-1.1.3/deltacat/compute/stats/models/delta_column_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/stats/models/delta_stats.py` & `deltacat-1.1.3/deltacat/compute/stats/models/delta_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/stats/models/delta_stats_cache_result.py` & `deltacat-1.1.3/deltacat/compute/stats/models/delta_stats_cache_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/stats/models/manifest_entry_stats.py` & `deltacat-1.1.3/deltacat/compute/stats/models/manifest_entry_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/stats/models/stats_result.py` & `deltacat-1.1.3/deltacat/compute/stats/models/stats_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/stats/utils/intervals.py` & `deltacat-1.1.3/deltacat/compute/stats/utils/intervals.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/stats/utils/io.py` & `deltacat-1.1.3/deltacat/compute/stats/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/compute/stats/utils/manifest_stats_file.py` & `deltacat-1.1.3/deltacat/compute/stats/utils/manifest_stats_file.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/constants.py` & `deltacat-1.1.3/deltacat/constants.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/io/aws/redshift/redshift_datasource.py` & `deltacat-1.1.3/deltacat/io/aws/redshift/redshift_datasource.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/io/dataset.py` & `deltacat-1.1.3/deltacat/io/dataset.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/io/file_object_store.py` & `deltacat-1.1.3/deltacat/io/file_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/io/memcached_object_store.py` & `deltacat-1.1.3/deltacat/io/memcached_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/io/object_store.py` & `deltacat-1.1.3/deltacat/io/object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/io/ray_plasma_object_store.py` & `deltacat-1.1.3/deltacat/io/ray_plasma_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/io/read_api.py` & `deltacat-1.1.3/deltacat/io/read_api.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/io/redis_object_store.py` & `deltacat-1.1.3/deltacat/io/redis_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/io/s3_object_store.py` & `deltacat-1.1.3/deltacat/io/s3_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/logs.py` & `deltacat-1.1.3/deltacat/logs.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/storage/__init__.py` & `deltacat-1.1.3/deltacat/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/storage/interface.py` & `deltacat-1.1.3/deltacat/storage/interface.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/storage/model/delete_parameters.py` & `deltacat-1.1.3/deltacat/storage/model/delete_parameters.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/storage/model/delta.py` & `deltacat-1.1.3/deltacat/storage/model/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/storage/model/list_result.py` & `deltacat-1.1.3/deltacat/storage/model/list_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/storage/model/locator.py` & `deltacat-1.1.3/deltacat/storage/model/locator.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/storage/model/namespace.py` & `deltacat-1.1.3/deltacat/storage/model/namespace.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/storage/model/partition.py` & `deltacat-1.1.3/deltacat/storage/model/partition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/storage/model/sort_key.py` & `deltacat-1.1.3/deltacat/storage/model/sort_key.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/storage/model/stream.py` & `deltacat-1.1.3/deltacat/storage/model/stream.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/storage/model/table.py` & `deltacat-1.1.3/deltacat/storage/model/table.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/storage/model/table_version.py` & `deltacat-1.1.3/deltacat/storage/model/table_version.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/storage/model/types.py` & `deltacat-1.1.3/deltacat/storage/model/types.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/aws/test_clients.py` & `deltacat-1.1.3/deltacat/tests/aws/test_clients.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/catalog/test_default_catalog_impl.py` & `deltacat-1.1.3/deltacat/tests/catalog/test_default_catalog_impl.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py` & `deltacat-1.1.3/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/compute/compact_partition_test_cases.py` & `deltacat-1.1.3/deltacat/tests/compute/compact_partition_test_cases.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/compute/compactor/steps/test_repartition.py` & `deltacat-1.1.3/deltacat/tests/compute/compactor/steps/test_repartition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/compute/compactor/utils/test_io.py` & `deltacat-1.1.3/deltacat/tests/compute/compactor/utils/test_io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/compute/compactor_v2/test_compaction_session.py` & `deltacat-1.1.3/deltacat/tests/compute/compactor_v2/test_compaction_session.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/compute/compactor_v2/utils/test_task_options.py` & `deltacat-1.1.3/deltacat/tests/compute/compactor_v2/utils/test_task_options.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/compute/test_compact_partition_incremental.py` & `deltacat-1.1.3/deltacat/tests/compute/test_compact_partition_incremental.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/compute/test_compact_partition_params.py` & `deltacat-1.1.3/deltacat/tests/compute/test_compact_partition_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py` & `deltacat-1.1.3/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/compute/test_util_common.py` & `deltacat-1.1.3/deltacat/tests/compute/test_util_common.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/compute/test_util_constant.py` & `deltacat-1.1.3/deltacat/tests/compute/test_util_constant.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/compute/test_util_create_table_deltas_repo.py` & `deltacat-1.1.3/deltacat/tests/compute/test_util_create_table_deltas_repo.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/io/test_cloudpickle_bug_fix.py` & `deltacat-1.1.3/deltacat/tests/io/test_cloudpickle_bug_fix.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/io/test_file_object_store.py` & `deltacat-1.1.3/deltacat/tests/io/test_file_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/io/test_memcached_object_store.py` & `deltacat-1.1.3/deltacat/tests/io/test_memcached_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/io/test_ray_plasma_object_store.py` & `deltacat-1.1.3/deltacat/tests/io/test_ray_plasma_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/io/test_redis_object_store.py` & `deltacat-1.1.3/deltacat/tests/io/test_redis_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/io/test_s3_object_store.py` & `deltacat-1.1.3/deltacat/tests/io/test_s3_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/local_deltacat_storage/__init__.py` & `deltacat-1.1.3/deltacat/tests/local_deltacat_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/stats/test_intervals.py` & `deltacat-1.1.3/deltacat/tests/stats/test_intervals.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/test_utils/pyarrow.py` & `deltacat-1.1.3/deltacat/tests/test_utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/test_utils/storage.py` & `deltacat-1.1.3/deltacat/tests/test_utils/storage.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/utils/test_cloudpickle.py` & `deltacat-1.1.3/deltacat/tests/utils/test_cloudpickle.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/utils/test_daft.py` & `deltacat-1.1.3/deltacat/tests/utils/test_daft.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/utils/test_metrics.py` & `deltacat-1.1.3/deltacat/tests/utils/test_metrics.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import unittest
 from unittest.mock import MagicMock, ANY, call
-import ray
 from deltacat.utils.metrics import (
     metrics,
     success_metric,
     failure_metric,
     latency_metric,
-    MetricsActor,
-    METRICS_CONFIG_ACTOR_NAME,
+    MetricsConfigCache,
     MetricsConfig,
     MetricsTarget,
     METRICS_TARGET_TO_EMITTER_DICT,
 )
 from deltacat.utils.performance import timed_invocation
 
 
@@ -39,19 +37,16 @@
     raise ValueError()
 
 
 class TestMetricsAnnotation(unittest.TestCase):
     def test_metrics_annotation_sanity(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         metrics_annotated_method(mock)
 
         mock.assert_called_once()
         self.assertEqual(2, mock_target.call_count)
         mock_target.assert_has_calls(
@@ -69,19 +64,16 @@
             ],
             any_order=True,
         )
 
     def test_metrics_annotation_when_error(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         self.assertRaises(ValueError, lambda: metrics_annotated_method_error(mock))
 
         mock.assert_not_called()
         self.assertEqual(3, mock_target.call_count)
         mock_target.assert_has_calls(
@@ -104,19 +96,16 @@
             ],
             any_order=True,
         )
 
     def test_metrics_with_prefix_annotation_sanity(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         metrics_with_prefix_annotated_method(mock)
 
         mock.assert_called_once()
         self.assertEqual(2, mock_target.call_count)
         mock_target.assert_has_calls(
@@ -130,19 +119,16 @@
             ],
             any_order=True,
         )
 
     def test_metrics_annotation_performance(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action with annotation
         _, actual_latency = timed_invocation(metrics_annotated_method, mock)
         _, second_call_latency = timed_invocation(metrics_annotated_method, mock)
 
         mock.assert_called()
         self.assertEqual(4, mock_target.call_count)
@@ -151,19 +137,16 @@
             actual_latency,
             "Second call to actor must be much faster",
         )
 
     def test_metrics_with_prefix_annotation_when_error(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         self.assertRaises(
             ValueError, lambda: metrics_with_prefix_annotated_method_error(mock)
         )
 
         mock.assert_not_called()
@@ -181,23 +164,18 @@
                     metrics_config=ANY,
                     value=ANY,
                 ),
             ],
             any_order=True,
         )
 
-    def test_metrics_with_prefix_annotation_without_actor(self):
+    def test_metrics_with_prefix_annotation_without_config(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
-
-        # explicitly making sure actor is killed
-        ray.kill(metrics_actor)
+        MetricsConfigCache.metrics_config = None
 
         # action
         self.assertRaises(
             ValueError, lambda: metrics_with_prefix_annotated_method_error(mock)
         )
 
         mock.assert_not_called()
@@ -224,19 +202,16 @@
     raise ValueError()
 
 
 class TestLatencyMetricAnnotation(unittest.TestCase):
     def test_annotation_sanity(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         latency_metric_annotated_method(mock)
 
         mock.assert_called_once()
         self.assertEqual(1, mock_target.call_count)
         mock_target.assert_has_calls(
@@ -249,19 +224,16 @@
             ],
             any_order=True,
         )
 
     def test_annotation_when_error(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         self.assertRaises(
             ValueError, lambda: latency_metric_annotated_method_error(mock)
         )
 
         mock.assert_not_called()
@@ -276,58 +248,47 @@
             ],
             any_order=True,
         )
 
     def test_annotation_with_args_sanity(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         latency_metric_with_name_annotated_method(mock)
 
         mock.assert_called_once()
         self.assertEqual(1, mock_target.call_count)
         mock_target.assert_has_calls(
             [call(metrics_name="test", metrics_config=ANY, value=ANY)], any_order=True
         )
 
     def test_annotation_with_args_when_error(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         self.assertRaises(
             ValueError, lambda: latency_metric_with_name_annotated_method_error(mock)
         )
 
         mock.assert_not_called()
         self.assertEqual(1, mock_target.call_count)
         mock_target.assert_has_calls(
             [call(metrics_name="test", metrics_config=ANY, value=ANY)], any_order=True
         )
 
-    def test_annotation_without_actor(self):
+    def test_annotation_without_config(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
-
-        # explicitly making sure actor is killed
-        ray.kill(metrics_actor)
+        MetricsConfigCache.metrics_config = None
 
         # action
         self.assertRaises(
             ValueError, lambda: latency_metric_with_name_annotated_method_error(mock)
         )
 
         mock.assert_not_called()
@@ -354,19 +315,16 @@
     raise ValueError()
 
 
 class TestSuccessMetricAnnotation(unittest.TestCase):
     def test_annotation_sanity(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         success_metric_annotated_method(mock)
 
         mock.assert_called_once()
         self.assertEqual(1, mock_target.call_count)
         mock_target.assert_has_calls(
@@ -379,72 +337,58 @@
             ],
             any_order=True,
         )
 
     def test_annotation_when_error(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         self.assertRaises(
             ValueError, lambda: success_metric_annotated_method_error(mock)
         )
 
         mock.assert_not_called()
         mock_target.assert_not_called()
 
     def test_annotation_with_args_sanity(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         success_metric_with_name_annotated_method(mock)
 
         mock.assert_called_once()
         self.assertEqual(1, mock_target.call_count)
         mock_target.assert_has_calls(
             [call(metrics_name="test", metrics_config=ANY, value=ANY)], any_order=True
         )
 
     def test_annotation_with_args_when_error(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         self.assertRaises(
             ValueError, lambda: success_metric_with_name_annotated_method_error(mock)
         )
 
         mock.assert_not_called()
         mock_target.assert_not_called()
 
-    def test_annotation_without_actor(self):
+    def test_annotation_without_config(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
-
-        # explicitly making sure actor is killed
-        ray.kill(metrics_actor)
+        MetricsConfigCache.metrics_config = None
 
         # action
         success_metric_annotated_method(mock)
 
         mock.assert_called_once()
         mock_target.assert_not_called()
 
@@ -469,34 +413,28 @@
     raise ValueError()
 
 
 class TestFailureMetricAnnotation(unittest.TestCase):
     def test_annotation_sanity(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         failure_metric_annotated_method(mock)
 
         mock.assert_called_once()
         mock_target.assert_not_called()
 
     def test_annotation_when_error(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         self.assertRaises(
             ValueError, lambda: failure_metric_annotated_method_error(mock)
         )
 
         mock.assert_not_called()
@@ -516,34 +454,28 @@
             ],
             any_order=True,
         )
 
     def test_annotation_with_args_sanity(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         failure_metric_with_name_annotated_method(mock)
 
         mock.assert_called_once()
         mock_target.assert_not_called()
 
     def test_annotation_with_args_when_error(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
         config = MetricsConfig("us-east-1", MetricsTarget.NOOP)
-        ray.get(metrics_actor.set_metrics_config.remote(config))
+        MetricsConfigCache.metrics_config = config
 
         # action
         self.assertRaises(
             ValueError, lambda: failure_metric_with_name_annotated_method_error(mock)
         )
 
         mock.assert_not_called()
@@ -552,23 +484,18 @@
             [
                 call(metrics_name="test.ValueError", metrics_config=ANY, value=ANY),
                 call(metrics_name="test", metrics_config=ANY, value=ANY),
             ],
             any_order=True,
         )
 
-    def test_annotation_without_actor(self):
+    def test_annotation_without_config(self):
         mock, mock_target = MagicMock(), MagicMock()
         METRICS_TARGET_TO_EMITTER_DICT[MetricsTarget.NOOP] = mock_target
-        metrics_actor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
-
-        # explicitly making sure actor is killed
-        ray.kill(metrics_actor)
+        MetricsConfigCache.metrics_config = None
 
         # action
         self.assertRaises(
             ValueError, lambda: failure_metric_with_name_annotated_method_error(mock)
         )
 
         mock.assert_not_called()
```

### Comparing `deltacat-1.1.2/deltacat/tests/utils/test_pyarrow.py` & `deltacat-1.1.3/deltacat/tests/utils/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/utils/test_record_batch_tables.py` & `deltacat-1.1.3/deltacat/tests/utils/test_record_batch_tables.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/tests/utils/test_resources.py` & `deltacat-1.1.3/deltacat/tests/utils/test_resources.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/types/media.py` & `deltacat-1.1.3/deltacat/types/media.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/types/partial_download.py` & `deltacat-1.1.3/deltacat/types/partial_download.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/types/tables.py` & `deltacat-1.1.3/deltacat/types/tables.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/arguments.py` & `deltacat-1.1.3/deltacat/utils/arguments.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/cloudpickle.py` & `deltacat-1.1.3/deltacat/utils/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/common.py` & `deltacat-1.1.3/deltacat/utils/common.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/daft.py` & `deltacat-1.1.3/deltacat/utils/daft.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/metrics.py` & `deltacat-1.1.3/deltacat/utils/metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from dataclasses import dataclass
 from typing import Optional
 
 import logging
-import ray
 import time
 import functools
 
 from aws_embedded_metrics import metric_scope
 from aws_embedded_metrics.config import get_config
 from aws_embedded_metrics.logger.metrics_logger import MetricsLogger
 from deltacat import logs
@@ -18,15 +17,14 @@
 from ray.util import get_node_ip_address
 
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
 
 DEFAULT_DELTACAT_METRICS_NAMESPACE = "ray-deltacat-metrics"
 DEFAULT_DELTACAT_LOG_GROUP_NAME = "ray-deltacat-metrics-EMF-logs"
 DEFAULT_DELTACAT_LOG_STREAM_CALLABLE = get_node_ip_address
-METRICS_CONFIG_ACTOR_NAME = "metrics-config-actor"
 
 
 class MetricsTarget(str, Enum):
     CLOUDWATCH = "cloudwatch"
     CLOUDWATCH_EMF = "cloudwatch_emf"
     NOOP = "noop"
 
@@ -183,31 +181,21 @@
 METRICS_TARGET_TO_EMITTER_DICT: Dict[str, Callable] = {
     MetricsTarget.CLOUDWATCH: _emit_cloudwatch_metrics,
     MetricsTarget.CLOUDWATCH_EMF: _emit_cloudwatch_emf_metrics,
     MetricsTarget.NOOP: _emit_noop_metrics,
 }
 
 
-@ray.remote
-class MetricsActor:
+class MetricsConfigCache:
     metrics_config: MetricsConfig = None
 
-    def set_metrics_config(self, config: MetricsConfig) -> None:
-        self.metrics_config = config
-
-    def get_metrics_config(self) -> MetricsConfig:
-        return self.metrics_config
-
 
 def _emit_ignore_exceptions(name: Optional[str], value: Any):
     try:
-        config_cache: MetricsActor = MetricsActor.options(
-            name=METRICS_CONFIG_ACTOR_NAME, get_if_exists=True
-        ).remote()
-        config = ray.get(config_cache.get_metrics_config.remote())
+        config = MetricsConfigCache.metrics_config
         if config:
             _emit_metrics(metrics_name=name, value=value, metrics_config=config)
     except BaseException as ex:
         logger.warning("Emitting metrics failed", ex)
 
 
 def emit_timer_metrics(metrics_name, value, metrics_config, **kwargs):
@@ -218,15 +206,22 @@
         **kwargs,
     )
 
 
 def latency_metric(original_func=None, name: Optional[str] = None):
     """
     A decorator that emits latency metrics of a function
-    based on configured metrics config.
+    based on configured metrics config. Hence, make sure to set it in all worker processes:
+
+    def setup_cache():
+        from deltacat.utils.metrics import MetricsConfigCache
+        MetricsConfigCache.metrics_config = metrics_config
+
+    setup_cache();
+    ray.init(address="auto", runtime_env={"worker_process_setup_hook": setup_cache})
     """
 
     def _decorate(func):
         metrics_name = name or f"{func.__name__}_time"
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
@@ -244,15 +239,22 @@
 
     return _decorate
 
 
 def success_metric(original_func=None, name: Optional[str] = None):
     """
     A decorator that emits success metrics of a function
-    based on configured metrics config.
+    based on configured metrics config. Hence, make sure to set it in all worker processes:
+
+    def setup_cache():
+        from deltacat.utils.metrics import MetricsConfigCache
+        MetricsConfigCache.metrics_config = metrics_config
+
+    setup_cache();
+    ray.init(address="auto", runtime_env={"worker_process_setup_hook": setup_cache})
     """
 
     def _decorate(func):
         metrics_name = name or f"{func.__name__}_success_count"
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
@@ -267,15 +269,22 @@
 
     return _decorate
 
 
 def failure_metric(original_func=None, name: Optional[str] = None):
     """
     A decorator that emits failure metrics of a function
-    based on configured metrics config.
+    based on configured metrics config. Hence, make sure to set it in all worker processes:
+
+    def setup_cache():
+        from deltacat.utils.metrics import MetricsConfigCache
+        MetricsConfigCache.metrics_config = metrics_config
+
+    setup_cache();
+    ray.init(address="auto", runtime_env={"worker_process_setup_hook": setup_cache})
     """
 
     def _decorate(func):
         metrics_name = name or f"{func.__name__}_failure_count"
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
@@ -297,15 +306,23 @@
         return _decorate(original_func)
 
     return _decorate
 
 
 def metrics(original_func=None, prefix: Optional[str] = None):
     """
-    A decorator that emits all metrics for a function.
+    A decorator that emits all metrics for a function. This decorator depends
+    on a metrics config. Hence, make sure to set it in all worker processes:
+
+    def setup_cache():
+        from deltacat.utils.metrics import MetricsConfigCache
+        MetricsConfigCache.metrics_config = metrics_config
+
+    setup_cache();
+    ray.init(address="auto", runtime_env={"worker_process_setup_hook": setup_cache})
     """
 
     def _decorate(func):
         name = prefix or func.__name__
         failure_metrics_name = f"{name}_failure_count"
         success_metrics_name = f"{name}_success_count"
         latency_metrics_name = f"{name}_time"
```

### Comparing `deltacat-1.1.2/deltacat/utils/numpy.py` & `deltacat-1.1.3/deltacat/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/pandas.py` & `deltacat-1.1.3/deltacat/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/performance.py` & `deltacat-1.1.3/deltacat/utils/performance.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/placement.py` & `deltacat-1.1.3/deltacat/utils/placement.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/pyarrow.py` & `deltacat-1.1.3/deltacat/utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/ray_utils/collections.py` & `deltacat-1.1.3/deltacat/utils/ray_utils/collections.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/ray_utils/concurrency.py` & `deltacat-1.1.3/deltacat/utils/ray_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/ray_utils/dataset.py` & `deltacat-1.1.3/deltacat/utils/ray_utils/dataset.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/ray_utils/runtime.py` & `deltacat-1.1.3/deltacat/utils/ray_utils/runtime.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/resources.py` & `deltacat-1.1.3/deltacat/utils/resources.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/s3fs.py` & `deltacat-1.1.3/deltacat/utils/s3fs.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat/utils/schema.py` & `deltacat-1.1.3/deltacat/utils/schema.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/deltacat.egg-info/PKG-INFO` & `deltacat-1.1.3/deltacat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltacat
-Version: 1.1.2
+Version: 1.1.3
 Summary: A scalable, fast, ACID-compliant Data Catalog powered by Ray.
 Home-page: https://github.com/ray-project/deltacat
 Author: Ray Team
 License: UNKNOWN
 Description: # DeltaCAT
         
         DeltaCAT is a Pythonic Data Catalog powered by Ray.
```

### Comparing `deltacat-1.1.2/deltacat.egg-info/SOURCES.txt` & `deltacat-1.1.3/deltacat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.2/setup.py` & `deltacat-1.1.3/setup.py`

 * *Files identical despite different names*

